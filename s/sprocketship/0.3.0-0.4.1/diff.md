# Comparing `tmp/sprocketship-0.3.0.tar.gz` & `tmp/sprocketship-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.3.0.tar", last modified: Mon Apr  8 15:18:43 2024, max compression
+gzip compressed data, was "sprocketship-0.4.1.tar", last modified: Mon Apr  8 15:42:46 2024, max compression
```

## Comparing `sprocketship-0.3.0.tar` & `sprocketship-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:18:43.211547 sprocketship-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 15:18:38.000000 sprocketship-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 15:18:38.000000 sprocketship-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-08 15:18:43.211547 sprocketship-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-08 15:18:38.000000 sprocketship-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-08 15:18:38.000000 sprocketship-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:18:43.211547 sprocketship-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:18:43.211547 sprocketship-0.3.0/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-08 15:18:38.000000 sprocketship-0.3.0/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:18:43.211547 sprocketship-0.3.0/sprocketship/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 15:18:38.000000 sprocketship-0.3.0/sprocketship/templates/javascript.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-08 15:18:38.000000 sprocketship-0.3.0/sprocketship/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:18:43.211547 sprocketship-0.3.0/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-08 15:18:43.000000 sprocketship-0.3.0/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 15:18:43.000000 sprocketship-0.3.0/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:18:43.000000 sprocketship-0.3.0/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 15:18:43.000000 sprocketship-0.3.0/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 15:18:43.000000 sprocketship-0.3.0/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 15:18:43.000000 sprocketship-0.3.0/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:46.637117 sprocketship-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 15:42:42.000000 sprocketship-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 15:42:42.000000 sprocketship-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-08 15:42:46.637117 sprocketship-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-08 15:42:42.000000 sprocketship-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-08 15:42:42.000000 sprocketship-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:42:46.637117 sprocketship-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:46.637117 sprocketship-0.4.1/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-08 15:42:42.000000 sprocketship-0.4.1/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:46.637117 sprocketship-0.4.1/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 15:42:42.000000 sprocketship-0.4.1/sprocketship/templates/javascript.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-08 15:42:42.000000 sprocketship-0.4.1/sprocketship/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:46.637117 sprocketship-0.4.1/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.3.0/LICENSE` & `sprocketship-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.3.0/PKG-INFO` & `sprocketship-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.3.0
+Version: 0.4.1
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.3.0 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.4.1 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
```

### Comparing `sprocketship-0.3.0/README.md` & `sprocketship-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sprocketship-0.3.0/pyproject.toml` & `sprocketship-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.3.0"
+version = "0.4.1"
 authors = [
   { name="Nicklaus Roach", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
```

### Comparing `sprocketship-0.3.0/sprocketship/cli.py` & `sprocketship-0.4.1/sprocketship/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,41 +25,42 @@
 
     con = connector.connect(**data["snowflake"])
 
     # Get the configurations for each procedure and attach relative path to file directory
     configs_with_paths = extract_configs(data["procedures"])
     procs = list(itertools.chain(*configs_with_paths.values()))
 
+    err = False
     for proc in procs:
         try:
             rendered_proc = create_javascript_stored_procedure(
                 **proc, **{"project_dir": dir}
             )
             con.cursor().execute(rendered_proc)
             msg = click.style(f"{proc['name']} ", fg="green", bold=True)
             msg += click.style(f"launched into schema ", fg="white", bold=True)
             msg += click.style(
                 f"{proc['database']}.{proc['schema']}", fg="blue", bold=True
             )
             click.echo(msg)
             if show:
                 click.echo(rendered_proc)
-            exit(0)
         except Exception as e:
+            err = True
             msg = click.style(f"{proc['name']} ", fg="red", bold=True)
             msg += click.style(
                 f"could not be launched into schema ", fg="white", bold=True
             )
             msg += click.style(
                 f"{proc['database']}.{proc['schema']}", fg="blue", bold=True
             )
             click.echo(msg)
             click.echo(e, err=True)
             click.echo(rendered_proc)
-            exit(1)
+    exit(1 if err else 0)
 
 
 @main.command()
 @click.argument("dir", default=".")
 @click.option("--target", default="target/sprocketship")
 def build(dir, target):
     click.echo(click.style(f"⚙️ Building sprocketship!", fg="white", bold=True))
@@ -69,24 +70,25 @@
 
     data = render_file(os.path.join(dir, ".sprocketship.yml"), return_dict=True)
 
     # Get the configurations for each procedure and attach relative path to file directory
     configs_with_paths = extract_configs(data["procedures"])
     procs = list(itertools.chain(*configs_with_paths.values()))
 
+    err = False
     for proc in procs:
         try:
             rendered_proc = create_javascript_stored_procedure(
                 **proc, **{"project_dir": dir}
             )
             with open(os.path.join(dir, target, proc["name"] + ".sql"), "+a") as f:
                 f.write(rendered_proc)
             msg = click.style(f"{proc['name']} ", fg="green", bold=True)
             msg += click.style(f"successfully built", fg="white", bold=True)
             click.echo(msg)
-            exit(0)
         except Exception as e:
+            err = True
             msg = click.style(f"{proc['name']} ", fg="red", bold=True)
             msg += click.style(f"could not be built", fg="white", bold=True)
             click.echo(msg)
             click.echo(e, err=True)
-            exit(1)
+    exit(1 if err else 0)
```

### Comparing `sprocketship-0.3.0/sprocketship/utils.py` & `sprocketship-0.4.1/sprocketship/utils.py`

 * *Files identical despite different names*

### Comparing `sprocketship-0.3.0/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.4.1/sprocketship.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.3.0
+Version: 0.4.1
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.3.0 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.4.1 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
```

