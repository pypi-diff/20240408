# Comparing `tmp/ark-mainsail-1.0.0.tar.gz` & `tmp/ark-mainsail-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ark-mainsail-1.0.0.tar", last modified: Sun Apr  7 16:23:22 2024, max compression
+gzip compressed data, was "ark-mainsail-1.0.1.tar", last modified: Mon Apr  8 20:57:11 2024, max compression
```

## Comparing `ark-mainsail-1.0.0.tar` & `ark-mainsail-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 16:23:22.089535 ark-mainsail-1.0.0/
--rw-rw-rw-   0        0        0     1063 2024-03-31 14:12:30.000000 ark-mainsail-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2860 2024-04-07 16:23:22.088538 ark-mainsail-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 16:23:22.083552 ark-mainsail-1.0.0/ark_mainsail.egg-info/
--rw-rw-rw-   0        0        0     2860 2024-04-07 16:23:21.000000 ark-mainsail-1.0.0/ark_mainsail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2024-04-07 16:23:21.000000 ark-mainsail-1.0.0/ark_mainsail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       57 2024-04-07 16:23:21.000000 ark-mainsail-1.0.0/ark_mainsail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-07 16:23:21.000000 ark-mainsail-1.0.0/ark_mainsail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2024-04-07 16:23:21.000000 ark-mainsail-1.0.0/ark_mainsail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 16:23:22.040806 ark-mainsail-1.0.0/mainsail/
--rw-rw-rw-   0        0        0     1848 2024-04-01 07:41:04.000000 ark-mainsail-1.0.0/mainsail/__init__.py
--rw-rw-rw-   0        0        0      959 2024-04-07 11:05:54.000000 ark-mainsail-1.0.0/mainsail/config.py
--rw-rw-rw-   0        0        0     1585 2024-03-31 14:12:31.000000 ark-mainsail-1.0.0/mainsail/deserializer.py
--rw-rw-rw-   0        0        0     9663 2024-04-07 05:49:52.000000 ark-mainsail-1.0.0/mainsail/identity.py
--rw-rw-rw-   0        0        0     4092 2024-04-07 13:54:09.000000 ark-mainsail-1.0.0/mainsail/rest.py
--rw-rw-rw-   0        0        0     1884 2024-03-31 14:12:31.000000 ark-mainsail-1.0.0/mainsail/serializer.py
--rw-rw-rw-   0        0        0     9253 2024-04-07 12:56:22.000000 ark-mainsail-1.0.0/mainsail/transaction.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:23:22.047787 ark-mainsail-1.0.0/mainsail/tx/
--rw-rw-rw-   0        0        0     1424 2024-04-07 15:25:42.000000 ark-mainsail-1.0.0/mainsail/tx/__init__.py
--rw-rw-rw-   0        0        0     7078 2024-04-07 12:42:08.000000 ark-mainsail-1.0.0/mainsail/tx/v1.py
--rw-rw-rw-   0        0        0     5057 2024-04-06 14:46:17.000000 ark-mainsail-1.0.0/mainsail/webhook.py
--rw-rw-rw-   0        0        0       42 2024-04-07 16:23:22.095517 ark-mainsail-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1432 2024-04-07 16:21:29.000000 ark-mainsail-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:23:22.080557 ark-mainsail-1.0.0/test/
--rw-rw-rw-   0        0        0       25 2024-04-01 18:54:30.000000 ark-mainsail-1.0.0/test/__init__.py
--rw-rw-rw-   0        0        0     1765 2024-04-06 14:10:01.000000 ark-mainsail-1.0.0/test/test_identity.py
--rw-rw-rw-   0        0        0     3331 2024-04-07 12:59:32.000000 ark-mainsail-1.0.0/test/test_v1_builders.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:57:11.449917 ark-mainsail-1.0.1/
+-rw-rw-rw-   0        0        0     1063 2024-03-31 14:12:30.000000 ark-mainsail-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3136 2024-04-08 20:57:11.447924 ark-mainsail-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-08 20:57:11.419639 ark-mainsail-1.0.1/ark_mainsail.egg-info/
+-rw-rw-rw-   0        0        0     3136 2024-04-08 20:57:10.000000 ark-mainsail-1.0.1/ark_mainsail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2024-04-08 20:57:10.000000 ark-mainsail-1.0.1/ark_mainsail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 20:57:10.000000 ark-mainsail-1.0.1/ark_mainsail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-08 20:57:10.000000 ark-mainsail-1.0.1/ark_mainsail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2024-04-08 20:57:10.000000 ark-mainsail-1.0.1/ark_mainsail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 20:57:11.398697 ark-mainsail-1.0.1/mainsail/
+-rw-rw-rw-   0        0        0     1848 2024-04-01 07:41:04.000000 ark-mainsail-1.0.1/mainsail/__init__.py
+-rw-rw-rw-   0        0        0      961 2024-04-07 19:01:11.000000 ark-mainsail-1.0.1/mainsail/config.py
+-rw-rw-rw-   0        0        0     1585 2024-03-31 14:12:31.000000 ark-mainsail-1.0.1/mainsail/deserializer.py
+-rw-rw-rw-   0        0        0     9663 2024-04-07 05:49:52.000000 ark-mainsail-1.0.1/mainsail/identity.py
+-rw-rw-rw-   0        0        0     4092 2024-04-07 13:54:09.000000 ark-mainsail-1.0.1/mainsail/rest.py
+-rw-rw-rw-   0        0        0     1884 2024-03-31 14:12:31.000000 ark-mainsail-1.0.1/mainsail/serializer.py
+-rw-rw-rw-   0        0        0     9253 2024-04-07 12:56:22.000000 ark-mainsail-1.0.1/mainsail/transaction.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:57:11.405677 ark-mainsail-1.0.1/mainsail/tx/
+-rw-rw-rw-   0        0        0     1424 2024-04-07 15:25:42.000000 ark-mainsail-1.0.1/mainsail/tx/__init__.py
+-rw-rw-rw-   0        0        0     7078 2024-04-07 12:42:08.000000 ark-mainsail-1.0.1/mainsail/tx/v1.py
+-rw-rw-rw-   0        0        0     5057 2024-04-06 14:46:17.000000 ark-mainsail-1.0.1/mainsail/webhook.py
+-rw-rw-rw-   0        0        0       42 2024-04-08 20:57:11.450915 ark-mainsail-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1569 2024-04-08 20:57:04.000000 ark-mainsail-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:57:11.416648 ark-mainsail-1.0.1/test/
+-rw-rw-rw-   0        0        0       25 2024-04-01 18:54:30.000000 ark-mainsail-1.0.1/test/__init__.py
+-rw-rw-rw-   0        0        0     1765 2024-04-06 14:10:01.000000 ark-mainsail-1.0.1/test/test_identity.py
+-rw-rw-rw-   0        0        0     3331 2024-04-07 12:59:32.000000 ark-mainsail-1.0.1/test/test_v1_builders.py
```

### Comparing `ark-mainsail-1.0.0/LICENSE` & `ark-mainsail-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/PKG-INFO` & `ark-mainsail-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: ark-mainsail
-Version: 1.0.0
-Summary: light api compatible with ARK blockchain and forks
+Version: 1.0.1
+Summary: Interact with ARK blockchain and forks
 Home-page: https://github.com/Moustikitos/python-mainsail
 Author: Toons
 Author-email: moustikitos@gmail.com
 Maintainer: Toons
 Maintainer-email: moustikitos@gmail.com
 License: Copyright 2024, MIT licence
+Project-URL: Bug Reports, https://github.com/Moustikitos/python-mainsail/issues
+Project-URL: Funding, https://github.com/Moustikitos/python-mainsail?tab=readme-ov-file#support-this-project
+Project-URL: Source, https://github.com/Moustikitos/python-mainsail/
 Keywords: api,ark,blockchain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +23,15 @@
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: base58
 Requires-Dist: pyaes
 Requires-Dist: blspy
+Requires-Dist: cSecp256k1
 
 # python-mainsail
 
 This package aims to provide a simple implementation to bake offline `Ark`
 transaction and interact with the blockchain API.
 
 ```python
```

### Comparing `ark-mainsail-1.0.0/ark_mainsail.egg-info/PKG-INFO` & `ark-mainsail-1.0.1/ark_mainsail.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: ark-mainsail
-Version: 1.0.0
-Summary: light api compatible with ARK blockchain and forks
+Version: 1.0.1
+Summary: Interact with ARK blockchain and forks
 Home-page: https://github.com/Moustikitos/python-mainsail
 Author: Toons
 Author-email: moustikitos@gmail.com
 Maintainer: Toons
 Maintainer-email: moustikitos@gmail.com
 License: Copyright 2024, MIT licence
+Project-URL: Bug Reports, https://github.com/Moustikitos/python-mainsail/issues
+Project-URL: Funding, https://github.com/Moustikitos/python-mainsail?tab=readme-ov-file#support-this-project
+Project-URL: Source, https://github.com/Moustikitos/python-mainsail/
 Keywords: api,ark,blockchain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +23,15 @@
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: base58
 Requires-Dist: pyaes
 Requires-Dist: blspy
+Requires-Dist: cSecp256k1
 
 # python-mainsail
 
 This package aims to provide a simple implementation to bake offline `Ark`
 transaction and interact with the blockchain API.
 
 ```python
```

### Comparing `ark-mainsail-1.0.0/ark_mainsail.egg-info/SOURCES.txt` & `ark-mainsail-1.0.1/ark_mainsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/mainsail/__init__.py` & `ark-mainsail-1.0.1/mainsail/__init__.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/mainsail/config.py` & `ark-mainsail-1.0.1/mainsail/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
     if os.path.exists(path):
         _clear()
         with open(path, "rb") as input:
             for attr, value in pickle.load(input).items():
                 setattr(sys.modules[__name__], attr, value)
                 _track.append(attr)
         return True
-    return False
+    return False
```

### Comparing `ark-mainsail-1.0.0/mainsail/deserializer.py` & `ark-mainsail-1.0.1/mainsail/deserializer.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/mainsail/identity.py` & `ark-mainsail-1.0.1/mainsail/identity.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/mainsail/rest.py` & `ark-mainsail-1.0.1/mainsail/rest.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/mainsail/serializer.py` & `ark-mainsail-1.0.1/mainsail/serializer.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/mainsail/transaction.py` & `ark-mainsail-1.0.1/mainsail/transaction.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/mainsail/tx/__init__.py` & `ark-mainsail-1.0.1/mainsail/tx/__init__.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/mainsail/tx/v1.py` & `ark-mainsail-1.0.1/mainsail/tx/v1.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/mainsail/webhook.py` & `ark-mainsail-1.0.1/mainsail/webhook.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/setup.py` & `ark-mainsail-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # -*- coding:utf-8 -*-
 
-import setuptools
 from setuptools import setup
 
+
 with open("README.md") as f2:
     LONG_DESCRIPTION = f2.read()
 
 kw = {
-    "version": "1.0.0",
+    "version": "1.0.1",
     "name": "ark-mainsail",
     "keywords": ["api", "ark", "blockchain"],
     "author": "Toons",
     "author_email": "moustikitos@gmail.com",
     "maintainer": "Toons",
     "maintainer_email": "moustikitos@gmail.com",
     "url": "https://github.com/Moustikitos/python-mainsail",
+    "project_urls": {  # Optional
+        "Bug Reports": "https://github.com/Moustikitos/python-mainsail/issues",
+        "Funding": "https://github.com/Moustikitos/python-mainsail?tab=readme-ov-file#support-this-project",
+        "Source": "https://github.com/Moustikitos/python-mainsail/",
+    },
     "include_package_data": True,
-    "description": "light api compatible with ARK blockchain and forks",
+    "description": "Interact with ARK blockchain and forks",
     "long_description": LONG_DESCRIPTION,
     "long_description_content_type": "text/markdown",
-    "install_requires": ["requests", "base58", "pyaes", "blspy"],
-    "dependency_links": [
-        "https://github.com/Moustikitos/fast-curve#egg=cSecp256k1",
-    ],
+    "install_requires": ["requests", "base58", "pyaes", "blspy", "cSecp256k1"],
     "license": "Copyright 2024, MIT licence",
     "classifiers": [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
-    "package_dir": {"": "."},
-    # "packages": setuptools.find_packages(),
+    "package_dir": {"": "."}
 }
 
 setup(**kw)
```

### Comparing `ark-mainsail-1.0.0/test/test_identity.py` & `ark-mainsail-1.0.1/test/test_identity.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.0/test/test_v1_builders.py` & `ark-mainsail-1.0.1/test/test_v1_builders.py`

 * *Files identical despite different names*

