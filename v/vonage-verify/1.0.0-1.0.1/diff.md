# Comparing `tmp/vonage-verify-1.0.0.tar.gz` & `tmp/vonage-verify-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-verify-1.0.0.tar", last modified: Thu Apr  4 05:14:01 2024, max compression
+gzip compressed data, was "vonage-verify-1.0.1.tar", last modified: Mon Apr  8 15:22:51 2024, max compression
```

## Comparing `vonage-verify-1.0.0.tar` & `vonage-verify-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.666921 vonage-verify-1.0.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     2884 2024-04-04 05:14:01.664692 vonage-verify-1.0.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     2110 2024-04-04 05:14:00.000000 vonage-verify-1.0.0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-04 05:14:00.000000 vonage-verify-1.0.0/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      832 2024-04-04 05:14:00.000000 vonage-verify-1.0.0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-04 05:14:01.667003 vonage-verify-1.0.0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.628481 vonage-verify-1.0.0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.646897 vonage-verify-1.0.0/src/vonage_verify/
--rw-r--r--   0 mkahan     (503) staff       (20)      582 2024-04-04 05:14:00.000000 vonage-verify-1.0.0/src/vonage_verify/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      141 2024-04-04 05:14:00.000000 vonage-verify-1.0.0/src/vonage_verify/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1291 2024-04-04 05:14:00.000000 vonage-verify-1.0.0/src/vonage_verify/language_codes.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1957 2024-04-04 05:14:00.000000 vonage-verify-1.0.0/src/vonage_verify/requests.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1319 2024-04-04 05:14:00.000000 vonage-verify-1.0.0/src/vonage_verify/responses.py
--rw-r--r--   0 mkahan     (503) staff       (20)     7464 2024-04-04 05:14:00.000000 vonage-verify-1.0.0/src/vonage_verify/verify.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.660268 vonage-verify-1.0.0/src/vonage_verify.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     2884 2024-04-04 05:14:01.000000 vonage-verify-1.0.0/src/vonage_verify.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      427 2024-04-04 05:14:01.000000 vonage-verify-1.0.0/src/vonage_verify.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-04 05:14:01.000000 vonage-verify-1.0.0/src/vonage_verify.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-04 05:14:01.000000 vonage-verify-1.0.0/src/vonage_verify.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       14 2024-04-04 05:14:01.000000 vonage-verify-1.0.0/src/vonage_verify.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.313634 vonage-verify-1.0.1/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2884 2024-04-08 15:22:51.312735 vonage-verify-1.0.1/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     2110 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      832 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-08 15:22:51.313958 vonage-verify-1.0.1/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.295217 vonage-verify-1.0.1/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.304479 vonage-verify-1.0.1/src/vonage_verify/
+-rw-r--r--   0 mkahan     (503) staff       (20)      582 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      141 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1296 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/language_codes.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1957 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/requests.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1319 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/responses.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     7464 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/verify.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.312005 vonage-verify-1.0.1/src/vonage_verify.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2884 2024-04-08 15:22:51.000000 vonage-verify-1.0.1/src/vonage_verify.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      427 2024-04-08 15:22:51.000000 vonage-verify-1.0.1/src/vonage_verify.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-08 15:22:51.000000 vonage-verify-1.0.1/src/vonage_verify.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-08 15:22:51.000000 vonage-verify-1.0.1/src/vonage_verify.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       14 2024-04-08 15:22:51.000000 vonage-verify-1.0.1/src/vonage_verify.egg-info/top_level.txt
```

### Comparing `vonage-verify-1.0.0/PKG-INFO` & `vonage-verify-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vonage-verify
-Version: 1.0.0
+Version: 1.0.1
 Summary: Vonage verify package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-http-client>=1.2.0
+Requires-Dist: vonage-http-client>=1.2.1
 Requires-Dist: vonage-utils>=1.0.1
 Requires-Dist: pydantic>=2.6.1
 
 # Vonage Verify Package
 
 This package contains the code to use Vonage's Verify API in Python. This package includes methods for working with 2-factor authentication (2FA) messages sent via SMS or TTS.
```

### Comparing `vonage-verify-1.0.0/README.md` & `vonage-verify-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vonage-verify-1.0.0/backend_shim.py` & `vonage-verify-1.0.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-verify-1.0.0/pyproject.toml` & `vonage-verify-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = 'vonage-verify'
-version = '1.0.0'
+version = '1.0.1'
 description = 'Vonage verify package'
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
-  "vonage-http-client>=1.2.0",
+  "vonage-http-client>=1.2.1",
   "vonage-utils>=1.0.1",
   "pydantic>=2.6.1",
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
```

### Comparing `vonage-verify-1.0.0/src/vonage_verify/__init__.py` & `vonage-verify-1.0.1/src/vonage_verify/__init__.py`

 * *Files identical despite different names*

### Comparing `vonage-verify-1.0.0/src/vonage_verify/language_codes.py` & `vonage-verify-1.0.1/src/vonage_verify/language_codes.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     tr_tr = 'tr-tr'
     vi_vn = 'vi-vn'
     yue_cn = 'yue-cn'
     zh_cn = 'zh-cn'
     zh_tw = 'zh-tw'
 
 
-class Psd2LanguageCode(Enum):
+class Psd2LanguageCode(str, Enum):
     en_gb = 'en-gb'
     bg_bg = 'bg-bg'
     cs_cz = 'cs-cz'
     da_dk = 'da-dk'
     de_de = 'de-de'
     ee_et = 'ee-et'
     el_gr = 'el-gr'
```

### Comparing `vonage-verify-1.0.0/src/vonage_verify/requests.py` & `vonage-verify-1.0.1/src/vonage_verify/requests.py`

 * *Files identical despite different names*

### Comparing `vonage-verify-1.0.0/src/vonage_verify/responses.py` & `vonage-verify-1.0.1/src/vonage_verify/responses.py`

 * *Files identical despite different names*

### Comparing `vonage-verify-1.0.0/src/vonage_verify/verify.py` & `vonage-verify-1.0.1/src/vonage_verify/verify.py`

 * *Files identical despite different names*

### Comparing `vonage-verify-1.0.0/src/vonage_verify.egg-info/PKG-INFO` & `vonage-verify-1.0.1/src/vonage_verify.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vonage-verify
-Version: 1.0.0
+Version: 1.0.1
 Summary: Vonage verify package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-http-client>=1.2.0
+Requires-Dist: vonage-http-client>=1.2.1
 Requires-Dist: vonage-utils>=1.0.1
 Requires-Dist: pydantic>=2.6.1
 
 # Vonage Verify Package
 
 This package contains the code to use Vonage's Verify API in Python. This package includes methods for working with 2-factor authentication (2FA) messages sent via SMS or TTS.
```

