# Comparing `tmp/celldega-0.1.2.tar.gz` & `tmp/celldega-0.1.3.tar.gz`

## Comparing `celldega-0.1.2.tar` & `celldega-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 celldega-0.1.2/src/celldega/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 celldega-0.1.2/src/celldega/static/widget.css
--rw-r--r--   0        0        0   913414 2020-02-02 00:00:00.000000 celldega-0.1.2/src/celldega/static/widget.js
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 celldega-0.1.2/.gitignore
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 celldega-0.1.2/README.md
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 celldega-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 celldega-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 celldega-0.1.3/src/celldega/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 celldega-0.1.3/src/celldega/static/widget.css
+-rw-r--r--   0        0        0  6841087 2020-02-02 00:00:00.000000 celldega-0.1.3/src/celldega/static/widget.js
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 celldega-0.1.3/.gitignore
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 celldega-0.1.3/README.md
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 celldega-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 celldega-0.1.3/PKG-INFO
```

### Comparing `celldega-0.1.2/src/celldega/__init__.py` & `celldega-0.1.3/src/celldega/__init__.py`

 * *Files identical despite different names*

### Comparing `celldega-0.1.2/README.md` & `celldega-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `celldega-0.1.2/pyproject.toml` & `celldega-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "celldega"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = ["anywidget"]
 readme = "README.md"
 
 [project.optional-dependencies]
 dev = ["watchfiles", "jupyterlab"]
 
 # automatically add the dev feature to the default env (e.g., hatch shell)
```

### Comparing `celldega-0.1.2/PKG-INFO` & `celldega-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: celldega
-Version: 0.1.2
+Version: 0.1.3
 Requires-Dist: anywidget
 Provides-Extra: dev
 Requires-Dist: jupyterlab; extra == 'dev'
 Requires-Dist: watchfiles; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # celldega
```

