# Comparing `tmp/apptrackr-0.2.0.tar.gz` & `tmp/apptrackr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.2.0.tar", max compression
+gzip compressed data, was "apptrackr-0.2.1.tar", max compression
```

## Comparing `apptrackr-0.2.0.tar` & `apptrackr-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.2.0/README.md
--rw-r--r--   0        0        0     1315 2024-04-08 10:04:25.590137 apptrackr-0.2.0/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.2.0/apptrackr/model/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-06 11:11:27.442305 apptrackr-0.2.0/apptrackr/model/migrations.py
--rw-r--r--   0        0        0      767 2024-04-06 19:30:04.565191 apptrackr-0.2.0/apptrackr/model/model.py
--rw-r--r--   0        0        0     1892 2024-04-08 05:37:54.923684 apptrackr-0.2.0/apptrackr/model/utils.py
--rw-r--r--   0        0        0      560 2024-04-08 05:36:37.348441 apptrackr-0.2.0/apptrackr/modules/config.py
--rw-r--r--   0        0        0    10071 2024-04-08 09:42:25.883499 apptrackr-0.2.0/apptrackr/modules/storage.py
--rw-r--r--   0        0        0      492 2024-04-08 10:34:15.465395 apptrackr-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 apptrackr-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.2.1/README.md
+-rw-r--r--   0        0        0     1315 2024-04-08 11:07:28.588800 apptrackr-0.2.1/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.2.1/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-06 11:11:27.442305 apptrackr-0.2.1/apptrackr/model/migrations.py
+-rw-r--r--   0        0        0      767 2024-04-06 19:30:04.565191 apptrackr-0.2.1/apptrackr/model/model.py
+-rw-r--r--   0        0        0     1892 2024-04-08 05:37:54.923684 apptrackr-0.2.1/apptrackr/model/utils.py
+-rw-r--r--   0        0        0      560 2024-04-08 05:36:37.348441 apptrackr-0.2.1/apptrackr/modules/config.py
+-rw-r--r--   0        0        0    10154 2024-04-08 14:28:47.983920 apptrackr-0.2.1/apptrackr/modules/storage.py
+-rw-r--r--   0        0        0      550 2024-04-08 15:00:48.036023 apptrackr-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 apptrackr-0.2.1/PKG-INFO
```

### Comparing `apptrackr-0.2.0/apptrackr/main.py` & `apptrackr-0.2.1/apptrackr/main.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.0/apptrackr/model/migrations.py` & `apptrackr-0.2.1/apptrackr/model/migrations.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.0/apptrackr/model/model.py` & `apptrackr-0.2.1/apptrackr/model/model.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.0/apptrackr/model/utils.py` & `apptrackr-0.2.1/apptrackr/model/utils.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.0/apptrackr/modules/config.py` & `apptrackr-0.2.1/apptrackr/modules/config.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.0/apptrackr/modules/storage.py` & `apptrackr-0.2.1/apptrackr/modules/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         application_details["location"] = location
 
     if date:
         application_details["date"] = date
 
     application = Applications(**application_details)
     application.save()
+    typer.secho(f"Application to {name} add successfully!", fg=typer.colors.GREEN)
 
 
 @storage.command()
 def fetch_applications(
     name: Annotated[
         Optional[str],
         typer.Option("--name", "-n", help="Filter by application name"),
```

### Comparing `apptrackr-0.2.0/PKG-INFO` & `apptrackr-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apptrackr
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: MIT
 Author: Aradhya Tripathi
 Author-email: 67282231+Aradhya-Tripathi@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

