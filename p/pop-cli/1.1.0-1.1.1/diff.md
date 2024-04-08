# Comparing `tmp/pop_cli-1.1.0.tar.gz` & `tmp/pop_cli-1.1.1.tar.gz`

## Comparing `pop_cli-1.1.0.tar` & `pop_cli-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pop_cli-1.1.0/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      602 2020-02-02 00:00:00.000000 pop_cli-1.1.0/src/__main__.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pop_cli-1.1.0/src/config.yaml
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 pop_cli-1.1.0/src/hub/cli.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pop_cli-1.1.0/src/hub/config.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pop_cli-1.1.0/src/hub/console.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pop_cli-1.1.0/src/hub/init.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pop_cli-1.1.0/src/hub/ref.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 pop_cli-1.1.0/src/hub/state.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-1.1.0/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-1.1.0/README.rst
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pop_cli-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pop_cli-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pop_cli-1.1.1/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      602 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/__main__.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/config.yaml
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/cli.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/config.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/console.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/init.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/ref.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/state.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-1.1.1/README.rst
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pop_cli-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pop_cli-1.1.1/PKG-INFO
```

### Comparing `pop_cli-1.1.0/.pre-commit-config.yaml` & `pop_cli-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.0/src/__main__.py` & `pop_cli-1.1.1/src/__main__.py`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.0/src/config.yaml` & `pop_cli-1.1.1/src/config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.0/src/hub/cli.py` & `pop_cli-1.1.1/src/hub/cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.0/src/hub/config.py` & `pop_cli-1.1.1/src/hub/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,9 +21,9 @@
         # Pass all remaining args onto the new parser
         cli=cli,
         parser_args=tuple(opts.cli.args),
         # Override the existing opts with new data from the next cli
         cli_config=hub._dynamic.config.cli_config,
         # Pass the already parsed opts as the new config
         config=new_config,
-        subcommands={},
+        subcommands=hub._dynamic.config.subcommands,
     )
```

### Comparing `pop_cli-1.1.0/src/hub/console.py` & `pop_cli-1.1.1/src/hub/console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.0/src/hub/init.py` & `pop_cli-1.1.1/src/hub/init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.0/src/hub/ref.py` & `pop_cli-1.1.1/src/hub/ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.0/src/hub/state.py` & `pop_cli-1.1.1/src/hub/state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.0/.gitignore` & `pop_cli-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.0/README.rst` & `pop_cli-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.0/pyproject.toml` & `pop_cli-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "1.1.0"
+version = "1.1.1"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `pop_cli-1.1.0/PKG-INFO` & `pop_cli-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 1.1.0
+Version: 1.1.1
 Summary: A POP cli interface
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

