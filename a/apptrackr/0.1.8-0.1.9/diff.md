# Comparing `tmp/apptrackr-0.1.8.tar.gz` & `tmp/apptrackr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.1.8.tar", max compression
+gzip compressed data, was "apptrackr-0.1.9.tar", max compression
```

## Comparing `apptrackr-0.1.8.tar` & `apptrackr-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.8/README.md
--rw-r--r--   0        0        0      303 2024-04-06 10:55:26.554890 apptrackr-0.1.8/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.8/apptrackr/model/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-06 11:11:27.442305 apptrackr-0.1.8/apptrackr/model/migrations.py
--rw-r--r--   0        0        0      767 2024-04-06 10:17:28.998913 apptrackr-0.1.8/apptrackr/model/model.py
--rw-r--r--   0        0        0      833 2024-04-06 09:22:12.817203 apptrackr-0.1.8/apptrackr/modules/sources.py
--rw-r--r--   0        0        0       95 2024-04-06 10:10:55.875981 apptrackr-0.1.8/apptrackr/modules/status.py
--rw-r--r--   0        0        0     9172 2024-04-06 10:52:29.213958 apptrackr-0.1.8/apptrackr/modules/storage.py
--rw-r--r--   0        0        0      454 2024-04-06 11:12:07.929197 apptrackr-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 apptrackr-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.9/README.md
+-rw-r--r--   0        0        0      658 2024-04-08 05:38:17.510840 apptrackr-0.1.9/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.9/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-06 11:11:27.442305 apptrackr-0.1.9/apptrackr/model/migrations.py
+-rw-r--r--   0        0        0      767 2024-04-06 19:30:04.565191 apptrackr-0.1.9/apptrackr/model/model.py
+-rw-r--r--   0        0        0     1892 2024-04-08 05:37:54.923684 apptrackr-0.1.9/apptrackr/model/utils.py
+-rw-r--r--   0        0        0      560 2024-04-08 05:36:37.348441 apptrackr-0.1.9/apptrackr/modules/config.py
+-rw-r--r--   0        0        0     9799 2024-04-06 13:24:45.745608 apptrackr-0.1.9/apptrackr/modules/storage.py
+-rw-r--r--   0        0        0      474 2024-04-08 05:39:17.777092 apptrackr-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 apptrackr-0.1.9/PKG-INFO
```

### Comparing `apptrackr-0.1.8/apptrackr/model/migrations.py` & `apptrackr-0.1.9/apptrackr/model/migrations.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.1.8/apptrackr/model/model.py` & `apptrackr-0.1.9/apptrackr/model/model.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.1.8/apptrackr/modules/storage.py` & `apptrackr-0.1.9/apptrackr/modules/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,14 +236,28 @@
     name: Optional[str] = typer.Option(
         None, "--name", "-n", help="Name of the application"
     ),
     application_id: Optional[int] = typer.Option(
         None, "--id", "-i", help="ID of the application"
     ),
 ) -> None:
+    """Modify attributes of an application stored in the database.
+
+    Args:
+        name (Optional[str], optional): Name of the application. Defaults to None.
+        application_id (Optional[int], optional): ID of the application. Defaults to None.
+
+    Returns:
+        None
+
+    This function prompts the user to select an application either by name or ID, and then allows them to choose which attributes to modify.
+    After selecting the attributes, the user can input new values for those attributes, which will be updated in the database.
+    If neither name nor ID is provided, the function raises an error.
+    """
+
     def _modify(id: int) -> None:
         can_modify = ["name", "status", "location", "date", "apply_link"]
         to_modify = questionary.checkbox(
             "Select the column you want to modify", choices=can_modify
         ).ask()
         if not to_modify:
             raise typer.Exit(-1)
```

### Comparing `apptrackr-0.1.8/PKG-INFO` & `apptrackr-0.1.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: apptrackr
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: MIT
 Author: Aradhya Tripathi
 Author-email: 67282231+Aradhya-Tripathi@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: humanize (>=4.9.0,<5.0.0)
 Requires-Dist: peewee (>=3.17.1,<4.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.12.0,<0.13.0)
 Description-Content-Type: text/markdown
```

