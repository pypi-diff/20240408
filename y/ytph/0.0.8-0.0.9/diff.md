# Comparing `tmp/ytph-0.0.8.tar.gz` & `tmp/ytph-0.0.9.tar.gz`

## Comparing `ytph-0.0.8.tar` & `ytph-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,11 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ytph-0.0.8/.idea/.gitignore
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 ytph-0.0.8/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 ytph-0.0.8/.idea/modules.xml
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 ytph-0.0.8/.idea/workspace.xml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ytph-0.0.8/.idea/ytph.iml
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ytph-0.0.8/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ytph-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ytph-0.0.8/src/ytph/__about__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ytph-0.0.8/src/ytph/__init__.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ytph-0.0.8/src/ytph/email.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ytph-0.0.8/src/ytph/iban.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 ytph-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 ytph-0.0.8/README.md
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 ytph-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 ytph-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 ytph-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ytph-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ytph-0.0.9/src/ytph/__about__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ytph-0.0.9/src/ytph/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ytph-0.0.9/src/ytph/email.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ytph-0.0.9/src/ytph/iban.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 ytph-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 ytph-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 ytph-0.0.9/README.md
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 ytph-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 ytph-0.0.9/PKG-INFO
```

### Comparing `ytph-0.0.8/LICENSE.txt` & `ytph-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ytph-0.0.8/README.md` & `ytph-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ytph-0.0.8/pyproject.toml` & `ytph-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -75,7 +75,33 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.ruff]
+select = [
+    "F",
+    "E",
+    "B",
+    "W",
+    "I",
+    "S",
+    "UP",
+    "DJ",
+    "TD",
+    "C4",
+    "PIE",
+    "ERA",
+    "RUF",
+    "LOG",
+    "PTH",
+    "INT",
+    "FURB",
+]
+ignore = ["E501", "F403", "F405", "RUF012", "TD003"]
+ignore-init-module-imports = true
+
+[tool.black]
+target-version = ["py311"]
```

### Comparing `ytph-0.0.8/PKG-INFO` & `ytph-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytph
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Documentation, https://github.com/unknown/ytph#readme
 Project-URL: Issues, https://github.com/unknown/ytph/issues
 Project-URL: Source, https://github.com/unknown/ytph
 Author-email: yanivtoledano <yanivtoledano@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

