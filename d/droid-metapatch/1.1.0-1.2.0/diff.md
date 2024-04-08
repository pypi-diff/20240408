# Comparing `tmp/droid_metapatch-1.1.0.tar.gz` & `tmp/droid_metapatch-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droid_metapatch-1.1.0.tar", max compression
+gzip compressed data, was "droid_metapatch-1.2.0.tar", max compression
```

## Comparing `droid_metapatch-1.1.0.tar` & `droid_metapatch-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    12277 2024-04-07 14:09:48.013767 droid_metapatch-1.1.0/README.md
--rw-r--r--   0        0        0      155 2024-04-04 07:42:22.856150 droid_metapatch-1.1.0/metapatch/__init__.py
--rw-r--r--   0        0        0     2533 2024-04-07 09:24:15.339115 droid_metapatch-1.1.0/metapatch/base.py
--rwxr-xr-x   0        0        0     9650 2024-04-07 14:06:52.964592 droid_metapatch-1.1.0/metapatch/cli_util.py
--rw-r--r--   0        0        0    11477 2024-04-07 08:42:30.705814 droid_metapatch-1.1.0/metapatch/metapatch.py
--rw-r--r--   0        0        0     6928 2024-04-04 09:31:45.638933 droid_metapatch-1.1.0/metapatch/options.py
--rw-r--r--   0        0        0      697 2024-04-04 09:40:34.183085 droid_metapatch-1.1.0/metapatch/utils.py
--rw-r--r--   0        0        0      493 2024-04-07 13:25:26.220124 droid_metapatch-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12888 1970-01-01 00:00:00.000000 droid_metapatch-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    12277 2024-04-08 09:00:49.052750 droid_metapatch-1.2.0/README.md
+-rw-r--r--   0        0        0      155 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/__init__.py
+-rw-r--r--   0        0        0     2533 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/base.py
+-rwxr-xr-x   0        0        0     9650 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/cli_util.py
+-rw-r--r--   0        0        0    11837 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/metapatch.py
+-rw-r--r--   0        0        0     6928 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/options.py
+-rw-r--r--   0        0        0      697 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/utils.py
+-rw-r--r--   0        0        0      493 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12888 1970-01-01 00:00:00.000000 droid_metapatch-1.2.0/PKG-INFO
```

### Comparing `droid_metapatch-1.1.0/README.md` & `droid_metapatch-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `droid_metapatch-1.1.0/metapatch/base.py` & `droid_metapatch-1.2.0/metapatch/base.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-1.1.0/metapatch/cli_util.py` & `droid_metapatch-1.2.0/metapatch/cli_util.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-1.1.0/metapatch/metapatch.py` & `droid_metapatch-1.2.0/metapatch/metapatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,17 +48,16 @@
         sections: Dict[str, Dict[str, Option]] = {}
         presets: List[Dict[str, Any]] = []
         for name, opt in cls.__dict__.items():
             if hasattr(opt, "_ispatchoption"):
                 if opt.section not in sections:
                     sections[opt.section] = {}
                 sections[opt.section][name] = opt
-            elif isinstance(opt, Preset):
-                presets.append(opt.asdict(name))
 
+        presets = cls.presets
         section_list: List[Dict[str, Any]] = []
         for section_name, options in sections.items():
             subsection: Dict[str, Any] = {"title": section_name, "options": []}
             for option_name, option in options.items():
                 subsection["options"].append(option.asdict(option_name))
             section_list.append(subsection)
 
@@ -74,15 +73,29 @@
     def presets(cls) -> List[Dict[str, Any]]:
         """Fetch presets."""
         presets: List[Dict[str, Any]] = []
         for name, opt in cls.__dict__.items():
             if isinstance(opt, Preset):
                 presets.append(opt.asdict(name))
 
-        return presets
+        if presets:
+            return presets
+        # No presets defined.
+        # We make a default preset.
+
+        params = {}
+        for name, opt in cls.__dict__.items():
+            if hasattr(opt, "_ispatchoption"):
+                params[name] = opt.default
+        default_preset = {
+            "name": "default",
+            "title": "Default Preset",
+            "parameters": params,
+        }
+        return [default_preset]
 
 
 class PatchGenerator(metaclass=MetaMetaPatch):
     """Patch Generator."""
 
     title: str
     description: str
```

### Comparing `droid_metapatch-1.1.0/metapatch/options.py` & `droid_metapatch-1.2.0/metapatch/options.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-1.1.0/metapatch/utils.py` & `droid_metapatch-1.2.0/metapatch/utils.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-1.1.0/PKG-INFO` & `droid_metapatch-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: droid-metapatch
-Version: 1.1.0
+Version: 1.2.0
 Summary: DROID patch generator
 License: GPL-3.0-only
 Author: Allan Eising
 Author-email: allan@eising.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

