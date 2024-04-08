# Comparing `tmp/KANGROLL-0.1.0.tar.gz` & `tmp/KANGROLL-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/KANGROLL-0.1.0.tar", last modified: Sun Apr  7 17:01:52 2024, max compression
+gzip compressed data, was "dist/KANGROLL-0.1.4.tar", last modified: Mon Apr  8 15:49:49 2024, max compression
```

## Comparing `KANGROLL-0.1.0.tar` & `KANGROLL-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-07 17:01:52.528993 KANGROLL-0.1.0/
--rw-r--r--   0 kang       (501) staff       (20)       42 2024-04-07 16:58:20.000000 KANGROLL-0.1.0/.gitignore
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-07 17:01:52.528385 KANGROLL-0.1.0/KANGROLL.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)      652 2024-04-07 17:01:52.000000 KANGROLL-0.1.0/KANGROLL.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      301 2024-04-07 17:01:52.000000 KANGROLL-0.1.0/KANGROLL.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-07 17:01:52.000000 KANGROLL-0.1.0/KANGROLL.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       15 2024-04-07 17:01:52.000000 KANGROLL-0.1.0/KANGROLL.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)     1092 2024-04-07 16:58:58.000000 KANGROLL-0.1.0/LICENSE
--rw-r--r--   0 kang       (501) staff       (20)      652 2024-04-07 17:01:52.528705 KANGROLL-0.1.0/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      196 2024-04-07 16:59:11.000000 KANGROLL-0.1.0/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-07 17:01:52.526818 KANGROLL-0.1.0/docs/
--rw-r--r--   0 kang       (501) staff       (20)     3303 2024-04-07 16:57:00.000000 KANGROLL-0.1.0/docs/tip_startup_process_kangroll_github_pypi.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-07 17:01:52.527368 KANGROLL-0.1.0/kangroll/
--rw-r--r--   0 kang       (501) staff       (20)       31 2024-04-07 16:58:01.000000 KANGROLL-0.1.0/kangroll/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)      731 2024-04-07 16:56:57.000000 KANGROLL-0.1.0/kangroll/core.py
--rw-r--r--   0 kang       (501) staff       (20)       38 2024-04-07 17:01:52.529060 KANGROLL-0.1.0/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      615 2024-04-07 17:00:37.000000 KANGROLL-0.1.0/setup.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-07 17:01:52.528016 KANGROLL-0.1.0/tests/
--rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-07 16:57:19.000000 KANGROLL-0.1.0/tests/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)      311 2024-04-07 16:57:39.000000 KANGROLL-0.1.0/tests/test_core.py
--rw-r--r--   0 kang       (501) staff       (20)       87 2024-04-07 17:01:02.000000 KANGROLL-0.1.0/version.txt
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:49:49.781497 KANGROLL-0.1.4/
+-rw-r--r--   0 kang       (501) staff       (20)       42 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/.gitignore
+-rw-r--r--   0 kang       (501) staff       (20)       55 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/0.command.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:49:49.780743 KANGROLL-0.1.4/KANGROLL.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:49:49.000000 KANGROLL-0.1.4/KANGROLL.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      314 2024-04-08 15:49:49.000000 KANGROLL-0.1.4/KANGROLL.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-08 15:49:49.000000 KANGROLL-0.1.4/KANGROLL.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)       15 2024-04-08 15:49:49.000000 KANGROLL-0.1.4/KANGROLL.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)     1092 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/LICENSE
+-rw-r--r--   0 kang       (501) staff       (20)      680 2024-04-08 15:49:49.781154 KANGROLL-0.1.4/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      224 2024-04-07 23:16:16.000000 KANGROLL-0.1.4/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:49:49.779647 KANGROLL-0.1.4/docs/
+-rw-r--r--   0 kang       (501) staff       (20)     3306 2024-04-08 15:17:41.000000 KANGROLL-0.1.4/docs/tip_startup_process_kangroll_github_pypi.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:49:49.780072 KANGROLL-0.1.4/kangroll/
+-rw-r--r--   0 kang       (501) staff       (20)       31 2024-04-08 15:16:42.000000 KANGROLL-0.1.4/kangroll/__init__.py
+-rw-r--r--   0 kang       (501) staff       (20)      731 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/kangroll/core.py
+-rw-r--r--   0 kang       (501) staff       (20)       38 2024-04-08 15:49:49.781560 KANGROLL-0.1.4/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      615 2024-04-08 15:49:48.000000 KANGROLL-0.1.4/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2024-04-08 15:49:49.780478 KANGROLL-0.1.4/tests/
+-rw-r--r--   0 kang       (501) staff       (20)        1 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/tests/__init__.py
+-rw-r--r--   0 kang       (501) staff       (20)      311 2024-04-07 23:15:30.000000 KANGROLL-0.1.4/tests/test_core.py
+-rw-r--r--   0 kang       (501) staff       (20)      291 2024-04-07 23:16:52.000000 KANGROLL-0.1.4/version.txt
```

### Comparing `KANGROLL-0.1.0/KANGROLL.egg-info/PKG-INFO` & `KANGROLL-0.1.4/KANGROLL.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: KANGROLL
-Version: 0.1.0
+Version: 0.1.4
 Summary: KANGROLL to buid a bridge between science and nature
 Home-page: https://github.com/williampolicy/kangroll
 Author: Xiaowen Kang
 Author-email: kangxiaowen@Gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kangroll
 kangroll Language for Kangroll theory
 
-/Users/kang/1.MainWorkSapce_Kang/code_pythonanywhere/kangroll
-
+/Users/kang/1.MainWorkSapce_Kang/code_pypi/kangroll
+Change the folder location. well done.
 
 
 
 # KANGROLL
 
 Describe what KANGROLL does, how to install it, and how to use it.
```

### Comparing `KANGROLL-0.1.0/LICENSE` & `KANGROLL-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `KANGROLL-0.1.0/PKG-INFO` & `KANGROLL-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: KANGROLL
-Version: 0.1.0
+Version: 0.1.4
 Summary: KANGROLL to buid a bridge between science and nature
 Home-page: https://github.com/williampolicy/kangroll
 Author: Xiaowen Kang
 Author-email: kangxiaowen@Gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kangroll
 kangroll Language for Kangroll theory
 
-/Users/kang/1.MainWorkSapce_Kang/code_pythonanywhere/kangroll
-
+/Users/kang/1.MainWorkSapce_Kang/code_pypi/kangroll
+Change the folder location. well done.
 
 
 
 # KANGROLL
 
 Describe what KANGROLL does, how to install it, and how to use it.
```

### Comparing `KANGROLL-0.1.0/docs/tip_startup_process_kangroll_github_pypi.md` & `KANGROLL-0.1.4/docs/tip_startup_process_kangroll_github_pypi.md`

 * *Files 0% similar despite different names*

```diff
@@ -121,7 +121,9 @@
 1. 在本地开发环境中使用以上结构和文件创建您的库。
 2. 使用Git追踪代码变更，并定期将更改推送到GitHub仓库。
 3. 编写和运行单元测试，确保代码的稳定性和可靠性。
 4. 当库准备就绪并且经过彻底测试后，按照上述PyPI发布流程将其发布。
 
 通过这个结构和流程，您可以创建一个专业级别的Python库，并确保它的可维护性和易用性。
 
+-
+
```

### Comparing `KANGROLL-0.1.0/kangroll/core.py` & `KANGROLL-0.1.4/kangroll/core.py`

 * *Files identical despite different names*

### Comparing `KANGROLL-0.1.0/setup.py` & `KANGROLL-0.1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="KANGROLL",
-    version="0.1.0",
+    version='0.1.4',
     author="Xiaowen Kang",
     author_email="kangxiaowen@Gmail.com",
     description="KANGROLL to buid a bridge between science and nature",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/williampolicy/kangroll",
     packages=find_packages(),
```

