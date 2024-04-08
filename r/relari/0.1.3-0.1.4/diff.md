# Comparing `tmp/relari-0.1.3.tar.gz` & `tmp/relari-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relari-0.1.3.tar", max compression
+gzip compressed data, was "relari-0.1.4.tar", max compression
```

## Comparing `relari-0.1.3.tar` & `relari-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2100 2024-02-29 01:27:03.863704 relari-0.1.3/README.md
--rw-r--r--   0        0        0      464 2024-04-05 01:40:29.931180 relari-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       45 2024-02-29 01:11:53.776218 relari-0.1.3/relari/__init__.py
--rw-r--r--   0        0        0      199 2024-02-29 01:11:53.776623 relari-0.1.3/relari/eval/__init__.py
--rw-r--r--   0        0        0     5142 2024-02-29 01:11:53.776972 relari-0.1.3/relari/eval/dataset.py
--rw-r--r--   0        0        0     4790 2024-02-29 07:20:41.559538 relari-0.1.3/relari/eval/manager.py
--rw-r--r--   0        0        0     1669 2024-02-29 01:11:53.777735 relari-0.1.3/relari/eval/modules.py
--rw-r--r--   0        0        0     3413 2024-02-29 01:11:53.778019 relari-0.1.3/relari/eval/pipeline.py
--rw-r--r--   0        0        0     1771 2024-02-29 01:11:53.778261 relari-0.1.3/relari/eval/result_types.py
--rw-r--r--   0        0        0      123 2024-02-29 01:11:53.778488 relari-0.1.3/relari/eval/types.py
--rw-r--r--   0        0        0     1106 2024-02-29 01:11:53.779119 relari-0.1.3/relari/eval/utils.py
--rw-r--r--   0        0        0     3920 2024-04-05 01:17:20.592928 relari-0.1.3/relari/relari_client.py
--rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 relari-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2100 2024-02-29 01:27:03.863704 relari-0.1.4/README.md
+-rw-r--r--   0        0        0      464 2024-04-06 00:54:47.959958 relari-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-02-29 01:11:53.776218 relari-0.1.4/relari/__init__.py
+-rw-r--r--   0        0        0      199 2024-02-29 01:11:53.776623 relari-0.1.4/relari/eval/__init__.py
+-rw-r--r--   0        0        0     5563 2024-04-05 23:41:22.980593 relari-0.1.4/relari/eval/dataset.py
+-rw-r--r--   0        0        0     4790 2024-02-29 07:20:41.559538 relari-0.1.4/relari/eval/manager.py
+-rw-r--r--   0        0        0     1669 2024-02-29 01:11:53.777735 relari-0.1.4/relari/eval/modules.py
+-rw-r--r--   0        0        0     3413 2024-02-29 01:11:53.778019 relari-0.1.4/relari/eval/pipeline.py
+-rw-r--r--   0        0        0     1771 2024-02-29 01:11:53.778261 relari-0.1.4/relari/eval/result_types.py
+-rw-r--r--   0        0        0      123 2024-02-29 01:11:53.778488 relari-0.1.4/relari/eval/types.py
+-rw-r--r--   0        0        0     1106 2024-02-29 01:11:53.779119 relari-0.1.4/relari/eval/utils.py
+-rw-r--r--   0        0        0     3920 2024-04-05 01:17:20.592928 relari-0.1.4/relari/relari_client.py
+-rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 relari-0.1.4/PKG-INFO
```

### Comparing `relari-0.1.3/README.md` & `relari-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `relari-0.1.3/relari/eval/dataset.py` & `relari-0.1.4/relari/eval/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,14 @@
         dataset._data = data
         dataset._manifest = dataset._infer_manifest()
         dataset._create_dynamic_properties()
         return dataset
 
     def _load_or_infer_manifest(self, manifest_path: typing.Optional[Path]) -> DatasetManifest:
         if manifest_path is None or not manifest_path.exists():
-            warnings.warn(f"Manifest file not found in {manifest_path}, it is suggested to define a manifest.")
             return self._infer_manifest()
         else:
             with open(manifest_path, "r") as manifest_file:
                 manifest = yaml.safe_load(manifest_file)
                 fields = {
                     field_name: DatasetField(
                         name=field_name,
@@ -116,14 +115,26 @@
         # Dynamically add a property for each field
         for field_name, field_info in self._manifest.fields.items():
             setattr(self, field_name, field_info)
 
     def filed_types(self, name: str) -> type:
         return getattr(self, name).type
 
+    def save(self, file_path: typing.Union[str, Path], save_manifest: bool = False):
+        if isinstance(file_path, str):
+            file_path = Path(file_path)
+        with open(file_path, "w") as json_file:
+            for sample in self._data:
+                json_file.write(json.dumps(sample) + "\n")
+
+        if save_manifest:
+            manifest_path = file_path.parent / "manifest.yaml"
+            with open(manifest_path, "w") as manifest_file:
+                manifest_file.write(yaml.dump(self._manifest.to_yaml()))
+
     @property
     def data(self):
         return self._data
 
     @property
     def name(self):
         return self._manifest.name
```

### Comparing `relari-0.1.3/relari/eval/manager.py` & `relari-0.1.4/relari/eval/manager.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.3/relari/eval/modules.py` & `relari-0.1.4/relari/eval/modules.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.3/relari/eval/pipeline.py` & `relari-0.1.4/relari/eval/pipeline.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.3/relari/eval/result_types.py` & `relari-0.1.4/relari/eval/result_types.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.3/relari/eval/utils.py` & `relari-0.1.4/relari/eval/utils.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.3/relari/relari_client.py` & `relari-0.1.4/relari/relari_client.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.3/PKG-INFO` & `relari-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relari
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Pasquale Antonante
 Author-email: pasquale@relari.ai
 Requires-Python: >=3.9.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

