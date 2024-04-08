# Comparing `tmp/sprocketship-0.1.4.tar.gz` & `tmp/sprocketship-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.1.4.tar", last modified: Sat Apr  6 22:17:51 2024, max compression
+gzip compressed data, was "sprocketship-0.2.0.tar", last modified: Sun Apr  7 21:27:43 2024, max compression
```

## Comparing `sprocketship-0.1.4.tar` & `sprocketship-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:17:51.763069 sprocketship-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 22:17:47.000000 sprocketship-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 22:17:47.000000 sprocketship-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-06 22:17:51.763069 sprocketship-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-06 22:17:47.000000 sprocketship-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-06 22:17:47.000000 sprocketship-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 22:17:51.763069 sprocketship-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:17:51.759069 sprocketship-0.1.4/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-06 22:17:47.000000 sprocketship-0.1.4/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:17:51.763069 sprocketship-0.1.4/sprocketship/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-06 22:17:47.000000 sprocketship-0.1.4/sprocketship/templates/javascript.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:17:51.763069 sprocketship-0.1.4/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:43.199732 sprocketship-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-07 21:27:39.000000 sprocketship-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 21:27:39.000000 sprocketship-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-07 21:27:43.199732 sprocketship-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-07 21:27:39.000000 sprocketship-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-07 21:27:39.000000 sprocketship-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:27:43.199732 sprocketship-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:43.199732 sprocketship-0.2.0/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-07 21:27:39.000000 sprocketship-0.2.0/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:43.199732 sprocketship-0.2.0/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-07 21:27:39.000000 sprocketship-0.2.0/sprocketship/templates/javascript.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:43.199732 sprocketship-0.2.0/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-07 21:27:43.000000 sprocketship-0.2.0/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-07 21:27:43.000000 sprocketship-0.2.0/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:27:43.000000 sprocketship-0.2.0/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 21:27:43.000000 sprocketship-0.2.0/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 21:27:43.000000 sprocketship-0.2.0/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-07 21:27:43.000000 sprocketship-0.2.0/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.1.4/LICENSE` & `sprocketship-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.1.4/PKG-INFO` & `sprocketship-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.1.4
+Version: 0.2.0
 Summary: Better stored procedure management
-Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
+Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
-Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
+Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: snowflake
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.1.4 Summary: Better stored
-procedure management Author-email: Nicklaus Roacb
+Metadata-Version: 2.1 Name: sprocketship Version: 0.2.0 Summary: Better stored
+procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
-Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
+Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
 [Issues][issues-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-
```

### Comparing `sprocketship-0.1.4/README.md` & `sprocketship-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sprocketship-0.1.4/pyproject.toml` & `sprocketship-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.1.4"
+version = "0.2.0"
 authors = [
-  { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
+  { name="Nicklaus Roach", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
     "snowflake",
     "ABSQL",
@@ -24,8 +24,8 @@
 ]
 
 [project.scripts]
 sprocketship = "sprocketship.cli:main"
 
 [project.urls]
 Homepage = "https://github.com/nicklausroach/sprocketship"
-Issues = "https://github.com/pypa/nicklausroach/sprocketship"
+Issues = "https://github.com/nicklausroach/sprocketship/issues"
```

### Comparing `sprocketship-0.1.4/sprocketship/cli.py` & `sprocketship-0.2.0/sprocketship/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -70,7 +70,37 @@
         except Exception as e:
             msg = click.style(f"{proc['name']} ", fg='red', bold=True)
             msg += click.style(f"could not be launched into schema ", fg='white', bold=True)
             msg += click.style(f"{proc['database']}.{proc['schema']}", fg='blue', bold=True)
             click.echo(msg)
             click.echo(e, err=True)
             click.echo(rendered_proc)
+
+
+@main.command()
+@click.argument("dir", default=".")
+@click.option("--target", default="target/sprocketship")
+def build(dir, target):
+    click.echo(click.style(f"⚙️ Building sprocketship!", fg='white', bold=True))
+    # Open config in current directory
+
+    Path(os.path.join(dir, target)).mkdir(parents=True, exist_ok=True)
+
+    data = render_file(os.path.join(dir, '.sprocketship.yml'), return_dict=True)
+
+    # Get the configurations for each procedure and attach relative path to file directory
+    configs_with_paths = extract_configs(data["procedures"])
+    procs = list(itertools.chain(*configs_with_paths.values()))
+
+    for proc in procs:
+        try:
+            rendered_proc = create_javascript_stored_procedure(**proc, **{'project_dir': dir})
+            with open(os.path.join(dir, target, proc["name"] + ".sql"), '+a') as f:
+                f.write(rendered_proc)
+            msg = click.style(f"{proc['name']} ", fg='green', bold=True)
+            msg += click.style(f"successfully built", fg='white', bold=True)
+            click.echo(msg)
+        except Exception as e:
+            msg = click.style(f"{proc['name']} ", fg='red', bold=True)
+            msg += click.style(f"could not be built", fg='white', bold=True)
+            click.echo(msg)
+            click.echo(e, err=True)
```

### Comparing `sprocketship-0.1.4/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.2.0/sprocketship.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.1.4
+Version: 0.2.0
 Summary: Better stored procedure management
-Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
+Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
-Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
+Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: snowflake
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.1.4 Summary: Better stored
-procedure management Author-email: Nicklaus Roacb
+Metadata-Version: 2.1 Name: sprocketship Version: 0.2.0 Summary: Better stored
+procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
-Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
+Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
 [Issues][issues-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-
```

