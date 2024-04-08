# Comparing `tmp/apptrackr-0.1.9.tar.gz` & `tmp/apptrackr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.1.9.tar", max compression
+gzip compressed data, was "apptrackr-0.2.0.tar", max compression
```

## Comparing `apptrackr-0.1.9.tar` & `apptrackr-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.1.9/README.md
--rw-r--r--   0        0        0      658 2024-04-08 05:38:17.510840 apptrackr-0.1.9/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.1.9/apptrackr/model/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-06 11:11:27.442305 apptrackr-0.1.9/apptrackr/model/migrations.py
--rw-r--r--   0        0        0      767 2024-04-06 19:30:04.565191 apptrackr-0.1.9/apptrackr/model/model.py
--rw-r--r--   0        0        0     1892 2024-04-08 05:37:54.923684 apptrackr-0.1.9/apptrackr/model/utils.py
--rw-r--r--   0        0        0      560 2024-04-08 05:36:37.348441 apptrackr-0.1.9/apptrackr/modules/config.py
--rw-r--r--   0        0        0     9799 2024-04-06 13:24:45.745608 apptrackr-0.1.9/apptrackr/modules/storage.py
--rw-r--r--   0        0        0      474 2024-04-08 05:39:17.777092 apptrackr-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 apptrackr-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.2.0/README.md
+-rw-r--r--   0        0        0     1315 2024-04-08 10:04:25.590137 apptrackr-0.2.0/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.2.0/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-06 11:11:27.442305 apptrackr-0.2.0/apptrackr/model/migrations.py
+-rw-r--r--   0        0        0      767 2024-04-06 19:30:04.565191 apptrackr-0.2.0/apptrackr/model/model.py
+-rw-r--r--   0        0        0     1892 2024-04-08 05:37:54.923684 apptrackr-0.2.0/apptrackr/model/utils.py
+-rw-r--r--   0        0        0      560 2024-04-08 05:36:37.348441 apptrackr-0.2.0/apptrackr/modules/config.py
+-rw-r--r--   0        0        0    10071 2024-04-08 09:42:25.883499 apptrackr-0.2.0/apptrackr/modules/storage.py
+-rw-r--r--   0        0        0      492 2024-04-08 10:34:15.465395 apptrackr-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 apptrackr-0.2.0/PKG-INFO
```

### Comparing `apptrackr-0.1.9/apptrackr/model/migrations.py` & `apptrackr-0.2.0/apptrackr/model/migrations.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.1.9/apptrackr/model/model.py` & `apptrackr-0.2.0/apptrackr/model/model.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.1.9/apptrackr/model/utils.py` & `apptrackr-0.2.0/apptrackr/model/utils.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.1.9/apptrackr/modules/config.py` & `apptrackr-0.2.0/apptrackr/modules/config.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.1.9/apptrackr/modules/storage.py` & `apptrackr-0.2.0/apptrackr/modules/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from typing import Optional
 
+import questionary
 import typer
 from rich import box
 from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
 
 from apptrackr.model import Applications
-import questionary
 
 storage = typer.Typer()
 console = Console()
 
 
 @storage.command()
 def count(
-    active: Annotated[bool, typer.Option(help="Get only active application")] = False
+    status: Annotated[
+        Optional[str],
+        typer.Option(
+            help="Get applications depending on the status",
+        ),
+    ] = None
 ) -> None:
     """
     Fetch counts of applications.
 
     Args:
-        active (Annotated[ bool, typer.Option, optional): Fetch only active applications.)]=False.
+        active (Annotated[ bool, typer.Option, optional): Get applications depending on the status.)]=False.
     """
-    if active:
-        count = Applications.select().where(Applications.status == "active").count()
+    if status:
+        count = Applications.select().where(Applications.status == status).count()
     else:
         count = Applications.select().count()
 
     typer.echo(
         typer.style(f"Application Count: {count}", fg=typer.colors.BRIGHT_WHITE),
     )
 
@@ -57,15 +62,15 @@
         email_id_used (Annotated[str], typer.Argument, optional): Optional Application date)].
         location (Annotated[ Optional[str], typer.Argument, optional): Optional Job location)]=None.
         date (Annotated[ Optional[str], typer.Argument, optional): Optional Application date)]=None.:
     Raises:
         typer.Exit: For invalid arguments
     """
     if status not in ("active", "rejected", "accepted"):
-        typer.echo("Invalid status argument!")
+        typer.secho("Invalid status argument!", fg=typer.colors.BRIGHT_RED)
         raise typer.Exit(-1)
 
     application_details = {
         "name": name,
         "status": status,
         "apply_link": apply_link,
         "email_id_used": email_id_used,
@@ -130,15 +135,19 @@
         "date": date,
         "apply_link": apply_link,
     }
 
     per_page = 10
     for k, v in columns.items():
         if v:
-            filters.append(getattr(Applications, k) == v)
+            if k == "name":
+                # No one remembers the exact name!
+                filters.append(getattr(Applications, k).contains(v))
+            else:
+                filters.append(getattr(Applications, k) == v)
 
     applications = (
         Applications.select().where(*filters).paginate(page_number or 1, per_page)
         if filters
         else Applications.select().paginate(page_number or 1, per_page)
     )
     table = Table(
@@ -150,15 +159,15 @@
         "Application Link",
         "Email Id Used",
         box=box.MINIMAL,
     )
     for application in applications:
         match application.status:
             case "rejected":
-                style = "red on black"
+                style = "red"
             case "active":
                 style = "yellow"
             case "accepted":
                 style = "green"
             case _:
                 style = "white"
 
@@ -280,15 +289,15 @@
         typer.secho("Enter either the name or the id...")
         raise typer.Exit(-1)
 
     if application_id:
         _modify(application_id)
 
     else:
-        applications = Applications.select().where(Applications.name == name)
+        applications = Applications.select().where(Applications.name.contains(name))
         for application in applications:
             print(
                 application.application_id,
                 application.name,
                 application.status,
                 application.location,
                 application.date,
```

### Comparing `apptrackr-0.1.9/PKG-INFO` & `apptrackr-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: apptrackr
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Aradhya Tripathi
 Author-email: 67282231+Aradhya-Tripathi@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: humanize (>=4.9.0,<5.0.0)
 Requires-Dist: peewee (>=3.17.1,<4.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: trogon (>=0.5.0,<0.6.0)
 Requires-Dist: typer (>=0.12.0,<0.13.0)
 Description-Content-Type: text/markdown
```

