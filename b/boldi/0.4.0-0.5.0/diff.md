# Comparing `tmp/boldi-0.4.0.tar.gz` & `tmp/boldi-0.5.0.tar.gz`

## Comparing `boldi-0.4.0.tar` & `boldi-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 boldi-0.4.0/boldi/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boldi-0.4.0/boldi/_version.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boldi-0.4.0/.gitignore
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 boldi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boldi-0.4.0/../../README.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 boldi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 boldi-0.5.0/boldi/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boldi-0.5.0/boldi/_version.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boldi-0.5.0/.gitignore
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 boldi-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boldi-0.5.0/../../README.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 boldi-0.5.0/PKG-INFO
```

### Comparing `boldi-0.4.0/pyproject.toml` & `boldi-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boldi-0.4.0/../../README.md` & `boldi-0.5.0/../../README.md`

 * *Files identical despite different names*

### Comparing `boldi-0.4.0/PKG-INFO` & `boldi-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: boldi
-Version: 0.4.0
+Version: 0.5.0
 Summary: Boldi's Python libraries
 Author-email: Boldizsár Palotás <boldizsar.palotas@gmail.com>
 License: MIT
 Requires-Python: >=3.9
-Requires-Dist: boldi-cli==0.4.0
-Requires-Dist: boldi-ctx==0.4.0
-Requires-Dist: boldi-plugins==0.4.0
+Requires-Dist: boldi-cli==0.5.0
+Requires-Dist: boldi-ctx==0.5.0
+Requires-Dist: boldi-plugins==0.5.0
 Provides-Extra: dev
 Requires-Dist: boldi-dev; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Boldi's Python Libraries
 
 These are Boldi's personal Python libraries.
```

