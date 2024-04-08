# Comparing `tmp/best-ec2-1.1.1.tar.gz` & `tmp/best-ec2-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "best-ec2-1.1.1.tar", last modified: Tue Mar 26 18:08:11 2024, max compression
+gzip compressed data, was "best-ec2-1.1.2.tar", last modified: Mon Apr  8 16:10:22 2024, max compression
```

## Comparing `best-ec2-1.1.1.tar` & `best-ec2-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:11.507863 best-ec2-1.1.1/
--rw-r--r--   0 root         (0) root         (0)    16833 2024-03-26 18:08:11.507863 best-ec2-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    16216 2024-03-26 18:07:45.000000 best-ec2-1.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 18:07:45.000000 best-ec2-1.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      789 2024-03-26 18:08:11.507863 best-ec2-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-03-26 18:07:45.000000 best-ec2-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:11.500863 best-ec2-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:11.504863 best-ec2-1.1.1/src/best_ec2/
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/aws_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/best_ec2.py
--rw-rw-rw-   0 root         (0) root         (0)     8416 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/best_ec2_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     1248 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1693 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6423 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      966 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/spot_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:11.506863 best-ec2-1.1.1/src/best_ec2/strategies/
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/strategies/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3653 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/strategies/abstract_sort_strategy.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/strategies/sort_on_demand_strategy.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/strategies/sort_spot_strategy.py
--rw-rw-rw-   0 root         (0) root         (0)     1005 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/strategies/sort_strategy_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4763 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/types.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-03-26 18:07:45.000000 best-ec2-1.1.1/src/best_ec2/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:11.506863 best-ec2-1.1.1/src/best_ec2.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16833 2024-03-26 18:08:11.000000 best-ec2-1.1.1/src/best_ec2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      775 2024-03-26 18:08:11.000000 best-ec2-1.1.1/src/best_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 18:08:11.000000 best-ec2-1.1.1/src/best_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-26 18:08:11.000000 best-ec2-1.1.1/src/best_ec2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-26 18:08:11.000000 best-ec2-1.1.1/src/best_ec2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:11.506863 best-ec2-1.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)    12201 2024-03-26 18:07:45.000000 best-ec2-1.1.1/tests/test_int.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.073442 best-ec2-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)    16771 2024-04-08 16:10:22.073442 best-ec2-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    16216 2024-04-08 16:09:55.000000 best-ec2-1.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:09:55.000000 best-ec2-1.1.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-04-08 16:10:22.073442 best-ec2-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-08 16:09:55.000000 best-ec2-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.065442 best-ec2-1.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.069442 best-ec2-1.1.2/src/best_ec2/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/aws_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/best_ec2.py
+-rw-rw-rw-   0 root         (0) root         (0)     8416 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/best_ec2_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1693 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6423 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/spot_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.072442 best-ec2-1.1.2/src/best_ec2/strategies/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/strategies/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3653 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/strategies/abstract_sort_strategy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/strategies/sort_on_demand_strategy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/strategies/sort_spot_strategy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/strategies/sort_strategy_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4763 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.072442 best-ec2-1.1.2/src/best_ec2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16771 2024-04-08 16:10:22.000000 best-ec2-1.1.2/src/best_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      775 2024-04-08 16:10:22.000000 best-ec2-1.1.2/src/best_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:10:22.000000 best-ec2-1.1.2/src/best_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-08 16:10:22.000000 best-ec2-1.1.2/src/best_ec2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-08 16:10:22.000000 best-ec2-1.1.2/src/best_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.072442 best-ec2-1.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12201 2024-04-08 16:09:55.000000 best-ec2-1.1.2/tests/test_int.py
```

### Comparing `best-ec2-1.1.1/PKG-INFO` & `best-ec2-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: best-ec2
-Version: 1.1.1
+Version: 1.1.2
 Summary: Best EC2, the smart solution designed to optimize your Amazon EC2 instance type selection process. The app simplifies the challenge of choosing the optimal EC2 instance type that matches your specific requirements, balancing performance, cost, and computing needs.
-Home-page: https://gitlab.com/aliaksei.kankou/best-ec2
+Home-page: https://gitlab.com/aliaksei-kankou/best-ec2/python-package
 Author: Aliaksei Kankou
 Author-email: aliaksei.kankou@gmail.com
-Project-URL: Bug Tracker, https://gitlab.com/aliaksei.kankou/best-ec2/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: boto3>=1.29.2
 
 # Best EC2
 
 Best EC2, the smart solution designed to optimize your Amazon EC2 instance type selection process. The app simplifies the challenge of choosing the optimal EC2 instance type that matches your specific requirements, balancing performance, cost, and computing needs.
```

### Comparing `best-ec2-1.1.1/README.md` & `best-ec2-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/setup.cfg` & `best-ec2-1.1.2/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 [metadata]
 name = best-ec2
-version = 1.1.1
+version = 1.1.2
 author = Aliaksei Kankou
 author_email = aliaksei.kankou@gmail.com
 description = Best EC2, the smart solution designed to optimize your Amazon EC2 instance type selection process. The app simplifies the challenge of choosing the optimal EC2 instance type that matches your specific requirements, balancing performance, cost, and computing needs.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://gitlab.com/aliaksei.kankou/best-ec2
-project_urls = 
-	Bug Tracker = https://gitlab.com/aliaksei.kankou/best-ec2/issues
+url = https://gitlab.com/aliaksei-kankou/best-ec2/python-package
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8.0
 install_requires =
```

### Comparing `best-ec2-1.1.1/src/best_ec2/aws_utils.py` & `best-ec2-1.1.2/src/best_ec2/aws_utils.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/best_ec2.py` & `best-ec2-1.1.2/src/best_ec2/best_ec2.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/best_ec2_impl.py` & `best-ec2-1.1.2/src/best_ec2/best_ec2_impl.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/cache.py` & `best-ec2-1.1.2/src/best_ec2/cache.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/constants.py` & `best-ec2-1.1.2/src/best_ec2/constants.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/exceptions.py` & `best-ec2-1.1.2/src/best_ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/filters.py` & `best-ec2-1.1.2/src/best_ec2/filters.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/spot_utils.py` & `best-ec2-1.1.2/src/best_ec2/spot_utils.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/strategies/abstract_sort_strategy.py` & `best-ec2-1.1.2/src/best_ec2/strategies/abstract_sort_strategy.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/strategies/sort_on_demand_strategy.py` & `best-ec2-1.1.2/src/best_ec2/strategies/sort_on_demand_strategy.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/strategies/sort_spot_strategy.py` & `best-ec2-1.1.2/src/best_ec2/strategies/sort_spot_strategy.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/strategies/sort_strategy_factory.py` & `best-ec2-1.1.2/src/best_ec2/strategies/sort_strategy_factory.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/types.py` & `best-ec2-1.1.2/src/best_ec2/types.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2/validators.py` & `best-ec2-1.1.2/src/best_ec2/validators.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/src/best_ec2.egg-info/PKG-INFO` & `best-ec2-1.1.2/src/best_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: best-ec2
-Version: 1.1.1
+Version: 1.1.2
 Summary: Best EC2, the smart solution designed to optimize your Amazon EC2 instance type selection process. The app simplifies the challenge of choosing the optimal EC2 instance type that matches your specific requirements, balancing performance, cost, and computing needs.
-Home-page: https://gitlab.com/aliaksei.kankou/best-ec2
+Home-page: https://gitlab.com/aliaksei-kankou/best-ec2/python-package
 Author: Aliaksei Kankou
 Author-email: aliaksei.kankou@gmail.com
-Project-URL: Bug Tracker, https://gitlab.com/aliaksei.kankou/best-ec2/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: boto3>=1.29.2
 
 # Best EC2
 
 Best EC2, the smart solution designed to optimize your Amazon EC2 instance type selection process. The app simplifies the challenge of choosing the optimal EC2 instance type that matches your specific requirements, balancing performance, cost, and computing needs.
```

### Comparing `best-ec2-1.1.1/src/best_ec2.egg-info/SOURCES.txt` & `best-ec2-1.1.2/src/best_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.1/tests/test_int.py` & `best-ec2-1.1.2/tests/test_int.py`

 * *Files identical despite different names*

