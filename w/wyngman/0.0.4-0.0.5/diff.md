# Comparing `tmp/wyngman-0.0.4.tar.gz` & `tmp/wyngman-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyngman-0.0.4.tar", last modified: Mon Apr 25 00:34:49 2022, max compression
+gzip compressed data, was "wyngman-0.0.5.tar", last modified: Mon Apr  8 19:19:49 2024, max compression
```

## Comparing `wyngman-0.0.4.tar` & `wyngman-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 razintailor   (501) staff       (20)        0 2022-04-25 00:34:49.411768 wyngman-0.0.4/
--rwxrwxrwx   0 razintailor   (501) staff       (20)     1069 2022-02-19 20:41:52.000000 wyngman-0.0.4/LICENSE
--rw-r--r--   0 razintailor   (501) staff       (20)     2939 2022-04-25 00:34:49.411840 wyngman-0.0.4/PKG-INFO
--rwxrwxrwx   0 razintailor   (501) staff       (20)     1891 2022-04-24 20:34:15.000000 wyngman-0.0.4/README.md
--rwxr-xr-x   0 razintailor   (501) staff       (20)     1719 2022-04-25 00:34:49.412319 wyngman-0.0.4/setup.cfg
--rwxrwxrwx   0 razintailor   (501) staff       (20)       38 2022-02-19 20:41:52.000000 wyngman-0.0.4/setup.py
-drwxr-xr-x   0 razintailor   (501) staff       (20)        0 2022-04-25 00:34:49.410813 wyngman-0.0.4/wyngman/
--rwxr-xr-x   0 razintailor   (501) staff       (20)        0 2022-04-24 21:11:33.000000 wyngman-0.0.4/wyngman/__init__.py
--rwxr-xr-x   0 razintailor   (501) staff       (20)     3472 2022-04-24 21:19:27.000000 wyngman-0.0.4/wyngman/aws_arg_parser.py
--rwxr-xr-x   0 razintailor   (501) staff       (20)     8724 2022-04-24 23:59:11.000000 wyngman-0.0.4/wyngman/cognito.py
--rwxr-xr-x   0 razintailor   (501) staff       (20)      235 2022-04-24 21:23:02.000000 wyngman-0.0.4/wyngman/constants.py
--rwxr-xr-x   0 razintailor   (501) staff       (20)     2216 2022-04-24 23:57:33.000000 wyngman-0.0.4/wyngman/main.py
--rwxr-xr-x   0 razintailor   (501) staff       (20)     1922 2022-04-24 21:36:02.000000 wyngman-0.0.4/wyngman/utils.py
-drwxr-xr-x   0 razintailor   (501) staff       (20)        0 2022-04-25 00:34:49.411661 wyngman-0.0.4/wyngman.egg-info/
--rw-r--r--   0 razintailor   (501) staff       (20)     2939 2022-04-25 00:34:49.000000 wyngman-0.0.4/wyngman.egg-info/PKG-INFO
--rw-r--r--   0 razintailor   (501) staff       (20)      343 2022-04-25 00:34:49.000000 wyngman-0.0.4/wyngman.egg-info/SOURCES.txt
--rw-r--r--   0 razintailor   (501) staff       (20)        1 2022-04-25 00:34:49.000000 wyngman-0.0.4/wyngman.egg-info/dependency_links.txt
--rw-r--r--   0 razintailor   (501) staff       (20)       46 2022-04-25 00:34:49.000000 wyngman-0.0.4/wyngman.egg-info/entry_points.txt
--rw-r--r--   0 razintailor   (501) staff       (20)      159 2022-04-25 00:34:49.000000 wyngman-0.0.4/wyngman.egg-info/requires.txt
--rw-r--r--   0 razintailor   (501) staff       (20)        8 2022-04-25 00:34:49.000000 wyngman-0.0.4/wyngman.egg-info/top_level.txt
+drwxr-xr-x   0 razintailor   (501) staff       (20)        0 2024-04-08 19:19:49.424665 wyngman-0.0.5/
+-rwxr-xr-x   0 razintailor   (501) staff       (20)     1069 2024-04-07 21:25:56.000000 wyngman-0.0.5/LICENSE
+-rw-r--r--   0 razintailor   (501) staff       (20)     3445 2024-04-08 19:19:49.424575 wyngman-0.0.5/PKG-INFO
+-rwxr-xr-x   0 razintailor   (501) staff       (20)     2080 2024-04-07 21:25:56.000000 wyngman-0.0.5/README.md
+-rwxr-xr-x   0 razintailor   (501) staff       (20)     1757 2024-04-08 19:19:49.424980 wyngman-0.0.5/setup.cfg
+-rwxr-xr-x   0 razintailor   (501) staff       (20)       38 2024-04-07 21:25:56.000000 wyngman-0.0.5/setup.py
+drwxr-xr-x   0 razintailor   (501) staff       (20)        0 2024-04-08 19:19:49.423262 wyngman-0.0.5/wyngman/
+-rwxr-xr-x   0 razintailor   (501) staff       (20)        0 2024-04-07 21:25:56.000000 wyngman-0.0.5/wyngman/__init__.py
+-rwxr-xr-x   0 razintailor   (501) staff       (20)     3472 2024-04-07 21:25:56.000000 wyngman-0.0.5/wyngman/aws_arg_parser.py
+-rwxr-xr-x   0 razintailor   (501) staff       (20)     8724 2024-04-07 21:25:56.000000 wyngman-0.0.5/wyngman/cognito.py
+-rwxr-xr-x   0 razintailor   (501) staff       (20)      285 2024-04-07 21:47:24.000000 wyngman-0.0.5/wyngman/constants.py
+-rwxr-xr-x   0 razintailor   (501) staff       (20)     2216 2024-04-07 21:25:56.000000 wyngman-0.0.5/wyngman/main.py
+-rwxr-xr-x   0 razintailor   (501) staff       (20)     1584 2024-04-07 21:52:33.000000 wyngman-0.0.5/wyngman/utils.py
+drwxr-xr-x   0 razintailor   (501) staff       (20)        0 2024-04-08 19:19:49.424338 wyngman-0.0.5/wyngman.egg-info/
+-rw-r--r--   0 razintailor   (501) staff       (20)     3445 2024-04-08 19:19:49.000000 wyngman-0.0.5/wyngman.egg-info/PKG-INFO
+-rw-r--r--   0 razintailor   (501) staff       (20)      343 2024-04-08 19:19:49.000000 wyngman-0.0.5/wyngman.egg-info/SOURCES.txt
+-rw-r--r--   0 razintailor   (501) staff       (20)        1 2024-04-08 19:19:49.000000 wyngman-0.0.5/wyngman.egg-info/dependency_links.txt
+-rw-r--r--   0 razintailor   (501) staff       (20)       46 2024-04-08 19:19:49.000000 wyngman-0.0.5/wyngman.egg-info/entry_points.txt
+-rw-r--r--   0 razintailor   (501) staff       (20)      157 2024-04-08 19:19:49.000000 wyngman-0.0.5/wyngman.egg-info/requires.txt
+-rw-r--r--   0 razintailor   (501) staff       (20)        8 2024-04-08 19:19:49.000000 wyngman-0.0.5/wyngman.egg-info/top_level.txt
```

### Comparing `wyngman-0.0.4/LICENSE` & `wyngman-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wyngman-0.0.4/PKG-INFO` & `wyngman-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 Metadata-Version: 2.1
 Name: wyngman
-Version: 0.0.4
+Version: 0.0.5
 Summary: wyngman is a Python package that provides needed functionalities of AWS Toolkit that are otherwise difficult to achieve with the standard cli or not possible currently.
 Home-page: https://github.com/Razin-Tailor/wyngman
 Author: Razin Tailor
 Author-email: razintailorpy@gmail.com
 License: MIT
 Keywords: AWS,Cognito,amazon web service
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3
+Requires-Dist: halo
+Requires-Dist: pandas>=1.2
+Requires-Dist: pyfiglet
+Requires-Dist: python-dotenv
+Requires-Dist: tabulate
+Requires-Dist: inquirer
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: importlib-resources; python_version < "3.7"
 
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) ![coverage](https://img.shields.io/badge/coverage-81%25-green)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) ![coverage](https://img.shields.io/badge/coverage-81%25-green) [![Downloads](https://pepy.tech/badge/wyngman)](https://pepy.tech/project/wyngman) [![Downloads](https://pepy.tech/badge/wyngman/month)](https://pepy.tech/project/wyngman) [![Downloads](https://pepy.tech/badge/wyngman/week)](https://pepy.tech/project/wyngman)
 
 # Wyngman: An AWS Utility Helper Tool
 
 ### What is it?
 
 wyngman is a Python package that provides needed functionalities of AWS Toolkit that are otherwise difficult to achieve with the standard cli or not possible currently. It aims to be the fundamental high-level utility helper tool for achieving more from AWS Services in Python.
 
@@ -34,15 +43,14 @@
 
 # Currently Supporting
 
 ## AWS Cognito
 
 A Querying support for AWS Cognito
 
-- Support to Query **ALL** users instead of the standard limit of _60_
 - Support to Query Users **Before** a certain UserCreationDate
 - Support to Query Users **After** a certain UserCreationDate
 - Support to **Save as CSV**
 
 # Installation
 
 ```bash
@@ -74,9 +82,7 @@
   --count, -c           Return Count of users
   --before BEFORE, -b BEFORE
                         All users before date Date in format yyyy-mm-dd
   --after AFTER, -a AFTER
                         All users after date Date in format yyyy-mm-dd
   --save, -s            Save as a CSV file
 ```
-
-
```

### Comparing `wyngman-0.0.4/README.md` & `wyngman-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) ![coverage](https://img.shields.io/badge/coverage-81%25-green)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) ![coverage](https://img.shields.io/badge/coverage-81%25-green) [![Downloads](https://pepy.tech/badge/wyngman)](https://pepy.tech/project/wyngman) [![Downloads](https://pepy.tech/badge/wyngman/month)](https://pepy.tech/project/wyngman) [![Downloads](https://pepy.tech/badge/wyngman/week)](https://pepy.tech/project/wyngman)
 
 # Wyngman: An AWS Utility Helper Tool
 
 ### What is it?
 
 wyngman is a Python package that provides needed functionalities of AWS Toolkit that are otherwise difficult to achieve with the standard cli or not possible currently. It aims to be the fundamental high-level utility helper tool for achieving more from AWS Services in Python.
 
@@ -10,15 +10,14 @@
 
 # Currently Supporting
 
 ## AWS Cognito
 
 A Querying support for AWS Cognito
 
-- Support to Query **ALL** users instead of the standard limit of _60_
 - Support to Query Users **Before** a certain UserCreationDate
 - Support to Query Users **After** a certain UserCreationDate
 - Support to **Save as CSV**
 
 # Installation
 
 ```bash
```

### Comparing `wyngman-0.0.4/setup.cfg` & `wyngman-0.0.5/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wyngman
-version = 0.0.4
+version = 0.0.5
 description = wyngman is a Python package that provides needed functionalities of AWS Toolkit that are otherwise difficult to achieve with the standard cli or not possible currently.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Razin-Tailor/wyngman
 author = Razin Tailor
 author_email = razintailorpy@gmail.com
 license = MIT
@@ -14,28 +14,29 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 keywords = AWS, Cognito, amazon web service
 
 [options]
 packages = find:
 install_requires = 
 	boto3
 	halo
 	pandas>=1.2
 	pyfiglet
 	python-dotenv
 	tabulate
-	PyInquirer
+	inquirer
 	importlib-metadata;python_version<"3.8"
 	importlib-resources;python_version<"3.7"
 python_requires = >=3.6.1
 
 [options.packages.find]
 exclude = 
 	tests*
```

### Comparing `wyngman-0.0.4/wyngman/aws_arg_parser.py` & `wyngman-0.0.5/wyngman/aws_arg_parser.py`

 * *Files identical despite different names*

### Comparing `wyngman-0.0.4/wyngman/cognito.py` & `wyngman-0.0.5/wyngman/cognito.py`

 * *Files identical despite different names*

### Comparing `wyngman-0.0.4/wyngman/main.py` & `wyngman-0.0.5/wyngman/main.py`

 * *Files identical despite different names*

### Comparing `wyngman-0.0.4/wyngman.egg-info/PKG-INFO` & `wyngman-0.0.5/wyngman.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 Metadata-Version: 2.1
 Name: wyngman
-Version: 0.0.4
+Version: 0.0.5
 Summary: wyngman is a Python package that provides needed functionalities of AWS Toolkit that are otherwise difficult to achieve with the standard cli or not possible currently.
 Home-page: https://github.com/Razin-Tailor/wyngman
 Author: Razin Tailor
 Author-email: razintailorpy@gmail.com
 License: MIT
 Keywords: AWS,Cognito,amazon web service
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3
+Requires-Dist: halo
+Requires-Dist: pandas>=1.2
+Requires-Dist: pyfiglet
+Requires-Dist: python-dotenv
+Requires-Dist: tabulate
+Requires-Dist: inquirer
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: importlib-resources; python_version < "3.7"
 
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) ![coverage](https://img.shields.io/badge/coverage-81%25-green)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) ![coverage](https://img.shields.io/badge/coverage-81%25-green) [![Downloads](https://pepy.tech/badge/wyngman)](https://pepy.tech/project/wyngman) [![Downloads](https://pepy.tech/badge/wyngman/month)](https://pepy.tech/project/wyngman) [![Downloads](https://pepy.tech/badge/wyngman/week)](https://pepy.tech/project/wyngman)
 
 # Wyngman: An AWS Utility Helper Tool
 
 ### What is it?
 
 wyngman is a Python package that provides needed functionalities of AWS Toolkit that are otherwise difficult to achieve with the standard cli or not possible currently. It aims to be the fundamental high-level utility helper tool for achieving more from AWS Services in Python.
 
@@ -34,15 +43,14 @@
 
 # Currently Supporting
 
 ## AWS Cognito
 
 A Querying support for AWS Cognito
 
-- Support to Query **ALL** users instead of the standard limit of _60_
 - Support to Query Users **Before** a certain UserCreationDate
 - Support to Query Users **After** a certain UserCreationDate
 - Support to **Save as CSV**
 
 # Installation
 
 ```bash
@@ -74,9 +82,7 @@
   --count, -c           Return Count of users
   --before BEFORE, -b BEFORE
                         All users before date Date in format yyyy-mm-dd
   --after AFTER, -a AFTER
                         All users after date Date in format yyyy-mm-dd
   --save, -s            Save as a CSV file
 ```
-
-
```

