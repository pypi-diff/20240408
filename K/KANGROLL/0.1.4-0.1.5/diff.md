# Comparing `tmp/KANGROLL-0.1.4.tar.gz` & `tmp/KANGROLL-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/KANGROLL-0.1.4.tar", last modified: Mon Apr  8 15:49:49 2024, max compression
+gzip compressed data, was "dist/KANGROLL-0.1.5.tar", last modified: Mon Apr  8 15:53:44 2024, max compression
```

## Comparing `KANGROLL-0.1.4.tar` & `KANGROLL-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:49:49.781497 KANGROLL-0.1.4/
--rw-r--r--   0 kang       (501) staff       (20)       42 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/.gitignore
--rw-r--r--   0 kang       (501) staff       (20)       55 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/0.command.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:49:49.780743 KANGROLL-0.1.4/KANGROLL.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:49:49.000000 KANGROLL-0.1.4/KANGROLL.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      314 2024-04-08 15:49:49.000000 KANGROLL-0.1.4/KANGROLL.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-08 15:49:49.000000 KANGROLL-0.1.4/KANGROLL.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       15 2024-04-08 15:49:49.000000 KANGROLL-0.1.4/KANGROLL.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)     1092 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/LICENSE
--rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:49:49.781154 KANGROLL-0.1.4/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      224 2024-04-07 23:16:16.000000 KANGROLL-0.1.4/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:49:49.779647 KANGROLL-0.1.4/docs/
--rw-r--r--   0 kang       (501) staff       (20)     3306 2024-04-08 15:17:41.000000 KANGROLL-0.1.4/docs/tip_startup_process_kangroll_github_pypi.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:49:49.780072 KANGROLL-0.1.4/kangroll/
--rw-r--r--   0 kang       (501) staff       (20)       31 2024-04-08 15:16:42.000000 KANGROLL-0.1.4/kangroll/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)      731 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/kangroll/core.py
--rw-r--r--   0 kang       (501) staff       (20)       38 2024-04-08 15:49:49.781560 KANGROLL-0.1.4/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      615 2024-04-08 15:49:48.000000 KANGROLL-0.1.4/setup.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:49:49.780478 KANGROLL-0.1.4/tests/
--rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/tests/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)      311 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/tests/test_core.py
--rw-r--r--   0 kang       (501) staff       (20)      291 2024-04-07 23:16:52.000000 KANGROLL-0.1.4/version.txt
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:53:44.357790 KANGROLL-0.1.5/
+-rw-r--r--   0 kang       (501) staff       (20)       42 2024-04-07 23:15:30.000000 KANGROLL-0.1.5/.gitignore
+-rw-r--r--   0 kang       (501) staff       (20)       55 2024-04-07 23:15:30.000000 KANGROLL-0.1.5/0.command.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:53:44.357201 KANGROLL-0.1.5/KANGROLL.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:53:44.000000 KANGROLL-0.1.5/KANGROLL.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      314 2024-04-08 15:53:44.000000 KANGROLL-0.1.5/KANGROLL.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-08 15:53:44.000000 KANGROLL-0.1.5/KANGROLL.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)       15 2024-04-08 15:53:44.000000 KANGROLL-0.1.5/KANGROLL.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)     1092 2024-04-07 23:15:30.000000 KANGROLL-0.1.5/LICENSE
+-rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:53:44.357512 KANGROLL-0.1.5/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      224 2024-04-07 23:16:16.000000 KANGROLL-0.1.5/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:53:44.356225 KANGROLL-0.1.5/docs/
+-rw-r--r--   0 kang       (501) staff       (20)     3306 2024-04-08 15:17:41.000000 KANGROLL-0.1.5/docs/tip_startup_process_kangroll_github_pypi.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:53:44.356649 KANGROLL-0.1.5/kangroll/
+-rw-r--r--   0 kang       (501) staff       (20)       31 2024-04-08 15:16:42.000000 KANGROLL-0.1.5/kangroll/__init__.py
+-rw-r--r--   0 kang       (501) staff       (20)      731 2024-04-07 23:15:30.000000 KANGROLL-0.1.5/kangroll/core.py
+-rw-r--r--   0 kang       (501) staff       (20)       38 2024-04-08 15:53:44.357848 KANGROLL-0.1.5/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      615 2024-04-08 15:53:43.000000 KANGROLL-0.1.5/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:53:44.356979 KANGROLL-0.1.5/tests/
+-rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-07 23:15:30.000000 KANGROLL-0.1.5/tests/__init__.py
+-rw-r--r--   0 kang       (501) staff       (20)      311 2024-04-07 23:15:30.000000 KANGROLL-0.1.5/tests/test_core.py
+-rw-r--r--   0 kang       (501) staff       (20)      291 2024-04-07 23:16:52.000000 KANGROLL-0.1.5/version.txt
```

### Comparing `KANGROLL-0.1.4/KANGROLL.egg-info/PKG-INFO` & `KANGROLL-0.1.5/KANGROLL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KANGROLL
-Version: 0.1.4
+Version: 0.1.5
 Summary: KANGROLL to buid a bridge between science and nature
 Home-page: https://github.com/williampolicy/kangroll
 Author: Xiaowen Kang
 Author-email: kangxiaowen@Gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `KANGROLL-0.1.4/LICENSE` & `KANGROLL-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `KANGROLL-0.1.4/PKG-INFO` & `KANGROLL-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KANGROLL
-Version: 0.1.4
+Version: 0.1.5
 Summary: KANGROLL to buid a bridge between science and nature
 Home-page: https://github.com/williampolicy/kangroll
 Author: Xiaowen Kang
 Author-email: kangxiaowen@Gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `KANGROLL-0.1.4/docs/tip_startup_process_kangroll_github_pypi.md` & `KANGROLL-0.1.5/docs/tip_startup_process_kangroll_github_pypi.md`

 * *Files identical despite different names*

### Comparing `KANGROLL-0.1.4/kangroll/core.py` & `KANGROLL-0.1.5/kangroll/core.py`

 * *Files identical despite different names*

### Comparing `KANGROLL-0.1.4/setup.py` & `KANGROLL-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="KANGROLL",
-    version='0.1.4',
+    version='0.1.5',
     author="Xiaowen Kang",
     author_email="kangxiaowen@Gmail.com",
     description="KANGROLL to buid a bridge between science and nature",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/williampolicy/kangroll",
     packages=find_packages(),
```

