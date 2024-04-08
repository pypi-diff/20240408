# Comparing `tmp/KANGROLL-0.1.8.tar.gz` & `tmp/KANGROLL-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/KANGROLL-0.1.8.tar", last modified: Mon Apr  8 15:59:52 2024, max compression
+gzip compressed data, was "dist/KANGROLL-0.1.9.tar", last modified: Mon Apr  8 16:00:17 2024, max compression
```

## Comparing `KANGROLL-0.1.8.tar` & `KANGROLL-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:59:52.400841 KANGROLL-0.1.8/
--rw-r--r--   0 kang       (501) staff       (20)       42 2024-04-07 23:15:30.000000 KANGROLL-0.1.8/.gitignore
--rw-r--r--   0 kang       (501) staff       (20)       55 2024-04-07 23:15:30.000000 KANGROLL-0.1.8/0.command.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:59:52.400186 KANGROLL-0.1.8/KANGROLL.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:59:52.000000 KANGROLL-0.1.8/KANGROLL.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      314 2024-04-08 15:59:52.000000 KANGROLL-0.1.8/KANGROLL.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-08 15:59:52.000000 KANGROLL-0.1.8/KANGROLL.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       15 2024-04-08 15:59:52.000000 KANGROLL-0.1.8/KANGROLL.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)     1092 2024-04-07 23:15:30.000000 KANGROLL-0.1.8/LICENSE
--rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:59:52.400530 KANGROLL-0.1.8/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      224 2024-04-07 23:16:16.000000 KANGROLL-0.1.8/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:59:52.399087 KANGROLL-0.1.8/docs/
--rw-r--r--   0 kang       (501) staff       (20)     3306 2024-04-08 15:17:41.000000 KANGROLL-0.1.8/docs/tip_startup_process_kangroll_github_pypi.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:59:52.399587 KANGROLL-0.1.8/kangroll/
--rw-r--r--   0 kang       (501) staff       (20)       31 2024-04-08 15:16:42.000000 KANGROLL-0.1.8/kangroll/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)      731 2024-04-07 23:15:30.000000 KANGROLL-0.1.8/kangroll/core.py
--rw-r--r--   0 kang       (501) staff       (20)       38 2024-04-08 15:59:52.400895 KANGROLL-0.1.8/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      615 2024-04-08 15:59:51.000000 KANGROLL-0.1.8/setup.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:59:52.399950 KANGROLL-0.1.8/tests/
--rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-07 23:15:30.000000 KANGROLL-0.1.8/tests/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)      311 2024-04-07 23:15:30.000000 KANGROLL-0.1.8/tests/test_core.py
--rw-r--r--   0 kang       (501) staff       (20)      291 2024-04-07 23:16:52.000000 KANGROLL-0.1.8/version.txt
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 16:00:17.281228 KANGROLL-0.1.9/
+-rw-r--r--   0 kang       (501) staff       (20)       42 2024-04-07 23:15:30.000000 KANGROLL-0.1.9/.gitignore
+-rw-r--r--   0 kang       (501) staff       (20)       55 2024-04-07 23:15:30.000000 KANGROLL-0.1.9/0.command.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 16:00:17.280620 KANGROLL-0.1.9/KANGROLL.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 16:00:17.000000 KANGROLL-0.1.9/KANGROLL.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      314 2024-04-08 16:00:17.000000 KANGROLL-0.1.9/KANGROLL.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-08 16:00:17.000000 KANGROLL-0.1.9/KANGROLL.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)       15 2024-04-08 16:00:17.000000 KANGROLL-0.1.9/KANGROLL.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)     1092 2024-04-07 23:15:30.000000 KANGROLL-0.1.9/LICENSE
+-rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 16:00:17.280930 KANGROLL-0.1.9/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      224 2024-04-07 23:16:16.000000 KANGROLL-0.1.9/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 16:00:17.279606 KANGROLL-0.1.9/docs/
+-rw-r--r--   0 kang       (501) staff       (20)     3306 2024-04-08 15:17:41.000000 KANGROLL-0.1.9/docs/tip_startup_process_kangroll_github_pypi.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 16:00:17.280067 KANGROLL-0.1.9/kangroll/
+-rw-r--r--   0 kang       (501) staff       (20)       31 2024-04-08 15:16:42.000000 KANGROLL-0.1.9/kangroll/__init__.py
+-rw-r--r--   0 kang       (501) staff       (20)      731 2024-04-07 23:15:30.000000 KANGROLL-0.1.9/kangroll/core.py
+-rw-r--r--   0 kang       (501) staff       (20)       38 2024-04-08 16:00:17.281290 KANGROLL-0.1.9/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      615 2024-04-08 16:00:16.000000 KANGROLL-0.1.9/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 16:00:17.280397 KANGROLL-0.1.9/tests/
+-rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-07 23:15:30.000000 KANGROLL-0.1.9/tests/__init__.py
+-rw-r--r--   0 kang       (501) staff       (20)      311 2024-04-07 23:15:30.000000 KANGROLL-0.1.9/tests/test_core.py
+-rw-r--r--   0 kang       (501) staff       (20)      291 2024-04-07 23:16:52.000000 KANGROLL-0.1.9/version.txt
```

### Comparing `KANGROLL-0.1.8/KANGROLL.egg-info/PKG-INFO` & `KANGROLL-0.1.9/KANGROLL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KANGROLL
-Version: 0.1.8
+Version: 0.1.9
 Summary: KANGROLL to buid a bridge between science and nature
 Home-page: https://github.com/williampolicy/kangroll
 Author: Xiaowen Kang
 Author-email: kangxiaowen@Gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `KANGROLL-0.1.8/LICENSE` & `KANGROLL-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `KANGROLL-0.1.8/PKG-INFO` & `KANGROLL-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KANGROLL
-Version: 0.1.8
+Version: 0.1.9
 Summary: KANGROLL to buid a bridge between science and nature
 Home-page: https://github.com/williampolicy/kangroll
 Author: Xiaowen Kang
 Author-email: kangxiaowen@Gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `KANGROLL-0.1.8/docs/tip_startup_process_kangroll_github_pypi.md` & `KANGROLL-0.1.9/docs/tip_startup_process_kangroll_github_pypi.md`

 * *Files identical despite different names*

### Comparing `KANGROLL-0.1.8/kangroll/core.py` & `KANGROLL-0.1.9/kangroll/core.py`

 * *Files identical despite different names*

### Comparing `KANGROLL-0.1.8/setup.py` & `KANGROLL-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="KANGROLL",
-    version='0.1.8',
+    version='0.1.9',
     author="Xiaowen Kang",
     author_email="kangxiaowen@Gmail.com",
     description="KANGROLL to buid a bridge between science and nature",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/williampolicy/kangroll",
     packages=find_packages(),
```

