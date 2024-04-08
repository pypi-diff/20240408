# Comparing `tmp/KANGROLL-0.1.6.tar.gz` & `tmp/KANGROLL-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/KANGROLL-0.1.6.tar", last modified: Mon Apr  8 15:56:58 2024, max compression
+gzip compressed data, was "dist/KANGROLL-0.1.7.tar", last modified: Mon Apr  8 15:57:45 2024, max compression
```

## Comparing `KANGROLL-0.1.6.tar` & `KANGROLL-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:56:58.083509 KANGROLL-0.1.6/
--rw-r--r--   0 kang       (501) staff       (20)       42 2024-04-07 23:15:30.000000 KANGROLL-0.1.6/.gitignore
--rw-r--r--   0 kang       (501) staff       (20)       55 2024-04-07 23:15:30.000000 KANGROLL-0.1.6/0.command.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:56:58.082935 KANGROLL-0.1.6/KANGROLL.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:56:57.000000 KANGROLL-0.1.6/KANGROLL.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      314 2024-04-08 15:56:57.000000 KANGROLL-0.1.6/KANGROLL.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-08 15:56:57.000000 KANGROLL-0.1.6/KANGROLL.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       15 2024-04-08 15:56:57.000000 KANGROLL-0.1.6/KANGROLL.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)     1092 2024-04-07 23:15:30.000000 KANGROLL-0.1.6/LICENSE
--rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:56:58.083231 KANGROLL-0.1.6/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      224 2024-04-07 23:16:16.000000 KANGROLL-0.1.6/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:56:58.080949 KANGROLL-0.1.6/docs/
--rw-r--r--   0 kang       (501) staff       (20)     3306 2024-04-08 15:17:41.000000 KANGROLL-0.1.6/docs/tip_startup_process_kangroll_github_pypi.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:56:58.082403 KANGROLL-0.1.6/kangroll/
--rw-r--r--   0 kang       (501) staff       (20)       31 2024-04-08 15:16:42.000000 KANGROLL-0.1.6/kangroll/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)      731 2024-04-07 23:15:30.000000 KANGROLL-0.1.6/kangroll/core.py
--rw-r--r--   0 kang       (501) staff       (20)       38 2024-04-08 15:56:58.083571 KANGROLL-0.1.6/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      615 2024-04-08 15:56:56.000000 KANGROLL-0.1.6/setup.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:56:58.082722 KANGROLL-0.1.6/tests/
--rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-07 23:15:30.000000 KANGROLL-0.1.6/tests/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)      311 2024-04-07 23:15:30.000000 KANGROLL-0.1.6/tests/test_core.py
--rw-r--r--   0 kang       (501) staff       (20)      291 2024-04-07 23:16:52.000000 KANGROLL-0.1.6/version.txt
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:57:45.258946 KANGROLL-0.1.7/
+-rw-r--r--   0 kang       (501) staff       (20)       42 2024-04-07 23:15:30.000000 KANGROLL-0.1.7/.gitignore
+-rw-r--r--   0 kang       (501) staff       (20)       55 2024-04-07 23:15:30.000000 KANGROLL-0.1.7/0.command.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:57:45.258187 KANGROLL-0.1.7/KANGROLL.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:57:45.000000 KANGROLL-0.1.7/KANGROLL.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      314 2024-04-08 15:57:45.000000 KANGROLL-0.1.7/KANGROLL.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-08 15:57:45.000000 KANGROLL-0.1.7/KANGROLL.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)       15 2024-04-08 15:57:45.000000 KANGROLL-0.1.7/KANGROLL.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)     1092 2024-04-07 23:15:30.000000 KANGROLL-0.1.7/LICENSE
+-rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:57:45.258617 KANGROLL-0.1.7/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      224 2024-04-07 23:16:16.000000 KANGROLL-0.1.7/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:57:45.256912 KANGROLL-0.1.7/docs/
+-rw-r--r--   0 kang       (501) staff       (20)     3306 2024-04-08 15:17:41.000000 KANGROLL-0.1.7/docs/tip_startup_process_kangroll_github_pypi.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:57:45.257504 KANGROLL-0.1.7/kangroll/
+-rw-r--r--   0 kang       (501) staff       (20)       31 2024-04-08 15:16:42.000000 KANGROLL-0.1.7/kangroll/__init__.py
+-rw-r--r--   0 kang       (501) staff       (20)      731 2024-04-07 23:15:30.000000 KANGROLL-0.1.7/kangroll/core.py
+-rw-r--r--   0 kang       (501) staff       (20)       38 2024-04-08 15:57:45.259030 KANGROLL-0.1.7/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      615 2024-04-08 15:57:44.000000 KANGROLL-0.1.7/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:57:45.257912 KANGROLL-0.1.7/tests/
+-rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-07 23:15:30.000000 KANGROLL-0.1.7/tests/__init__.py
+-rw-r--r--   0 kang       (501) staff       (20)      311 2024-04-07 23:15:30.000000 KANGROLL-0.1.7/tests/test_core.py
+-rw-r--r--   0 kang       (501) staff       (20)      291 2024-04-07 23:16:52.000000 KANGROLL-0.1.7/version.txt
```

### Comparing `KANGROLL-0.1.6/KANGROLL.egg-info/PKG-INFO` & `KANGROLL-0.1.7/KANGROLL.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KANGROLL
-Version: 0.1.6
+Version: 0.1.7
 Summary: KANGROLL to buid a bridge between science and nature
 Home-page: https://github.com/williampolicy/kangroll
 Author: Xiaowen Kang
 Author-email: kangxiaowen@Gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `KANGROLL-0.1.6/LICENSE` & `KANGROLL-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `KANGROLL-0.1.6/PKG-INFO` & `KANGROLL-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KANGROLL
-Version: 0.1.6
+Version: 0.1.7
 Summary: KANGROLL to buid a bridge between science and nature
 Home-page: https://github.com/williampolicy/kangroll
 Author: Xiaowen Kang
 Author-email: kangxiaowen@Gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `KANGROLL-0.1.6/docs/tip_startup_process_kangroll_github_pypi.md` & `KANGROLL-0.1.7/docs/tip_startup_process_kangroll_github_pypi.md`

 * *Files identical despite different names*

### Comparing `KANGROLL-0.1.6/kangroll/core.py` & `KANGROLL-0.1.7/kangroll/core.py`

 * *Files identical despite different names*

### Comparing `KANGROLL-0.1.6/setup.py` & `KANGROLL-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="KANGROLL",
-    version='0.1.6',
+    version='0.1.7',
     author="Xiaowen Kang",
     author_email="kangxiaowen@Gmail.com",
     description="KANGROLL to buid a bridge between science and nature",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/williampolicy/kangroll",
     packages=find_packages(),
```

