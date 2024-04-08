# Comparing `tmp/atypical-0.2.0.tar.gz` & `tmp/atypical-0.3.0.tar.gz`

## Comparing `atypical-0.2.0.tar` & `atypical-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/__init__.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/currency.py
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/email.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/money.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/phone.py
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/url.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 atypical-0.2.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 atypical-0.2.0/LICENSE
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 atypical-0.2.0/README.md
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 atypical-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 atypical-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 atypical-0.3.0/atypical/__init__.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 atypical-0.3.0/atypical/currency.py
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 atypical-0.3.0/atypical/email.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 atypical-0.3.0/atypical/money.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 atypical-0.3.0/atypical/phone.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 atypical-0.3.0/atypical/templated.py
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 atypical-0.3.0/atypical/url.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 atypical-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 atypical-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 atypical-0.3.0/README.md
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 atypical-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 atypical-0.3.0/PKG-INFO
```

### Comparing `atypical-0.2.0/atypical/currency.py` & `atypical-0.3.0/atypical/currency.py`

 * *Files identical despite different names*

### Comparing `atypical-0.2.0/atypical/email.py` & `atypical-0.3.0/atypical/email.py`

 * *Files identical despite different names*

### Comparing `atypical-0.2.0/atypical/money.py` & `atypical-0.3.0/atypical/money.py`

 * *Files identical despite different names*

### Comparing `atypical-0.2.0/atypical/phone.py` & `atypical-0.3.0/atypical/phone.py`

 * *Files identical despite different names*

### Comparing `atypical-0.2.0/atypical/url.py` & `atypical-0.3.0/atypical/url.py`

 * *Files identical despite different names*

### Comparing `atypical-0.2.0/.gitignore` & `atypical-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `atypical-0.2.0/LICENSE` & `atypical-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atypical-0.2.0/README.md` & `atypical-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `atypical-0.2.0/pyproject.toml` & `atypical-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [bumpver]
-current_version = "0.2.0"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version: {old_version} → {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
```

### Comparing `atypical-0.2.0/PKG-INFO` & `atypical-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: atypical
-Version: 0.2.0
+Version: 0.3.0
 Summary: Type handling and normalization for non-standard types like email, phone numbers, money, dates, etc. serializable and deserializable as JSON, JSON Schema, and Pydantic.
 Project-URL: Homepage, https://github.com/goodcleanfun/atypical
 Project-URL: Repository, https://github.com/goodcleanfun/atypical
 Author: Al Barrentine
 License-Expression: MIT
 License-File: LICENSE
 Keywords: atypical,utils
```

