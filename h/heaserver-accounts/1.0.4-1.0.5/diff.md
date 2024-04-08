# Comparing `tmp/heaserver-accounts-1.0.4.tar.gz` & `tmp/heaserver-accounts-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-accounts-1.0.4.tar", last modified: Fri Apr  5 19:50:15 2024, max compression
+gzip compressed data, was "heaserver-accounts-1.0.5.tar", last modified: Mon Apr  8 18:30:50 2024, max compression
```

## Comparing `heaserver-accounts-1.0.4.tar` & `heaserver-accounts-1.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.100082 heaserver-accounts-1.0.4/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/.gitignore
--rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5504 2024-04-05 19:50:15.099005 heaserver-accounts-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4196 2024-04-05 19:01:13.000000 heaserver-accounts-1.0.4/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/RELEASING.md
--rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.922949 heaserver-accounts-1.0.4/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.923977 heaserver-accounts-1.0.4/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.015649 heaserver-accounts-1.0.4/integrationtests/heaserver/accountintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/integrationtests/heaserver/accountintegrationtest/__init__.py
--rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/integrationtests/heaserver/accountintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     7748 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.4/integrationtests/heaserver/accountintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/requirements_dev.txt
--rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-05 19:50:15.100082 heaserver-accounts-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1825 2024-04-05 19:48:53.000000 heaserver-accounts-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.926044 heaserver-accounts-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.925003 heaserver-accounts-1.0.4/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.032575 heaserver-accounts-1.0.4/src/heaserver/account/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/src/heaserver/account/__init__.py
--rw-rw-rw-   0        0        0    45036 2024-04-05 18:57:12.000000 heaserver-accounts-1.0.4/src/heaserver/account/service.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.042306 heaserver-accounts-1.0.4/src/heaserver/account/wstl/
--rw-rw-rw-   0        0        0    11424 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.4/src/heaserver/account/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.097822 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/
--rw-rw-rw-   0        0        0     5504 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 19:50:14.000000 heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.927113 heaserver-accounts-1.0.4/tests/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:14.927113 heaserver-accounts-1.0.4/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:50:15.095821 heaserver-accounts-1.0.4/tests/heaserver/accounttest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.4/tests/heaserver/accounttest/__init__.py
--rw-rw-rw-   0        0        0     7466 2024-04-01 23:50:21.000000 heaserver-accounts-1.0.4/tests/heaserver/accounttest/test_all.py
--rw-rw-rw-   0        0        0     5146 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.4/tests/heaserver/accounttest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.490111 heaserver-accounts-1.0.5/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/.gitignore
+-rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5566 2024-04-08 18:30:50.489110 heaserver-accounts-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4258 2024-04-08 18:29:06.000000 heaserver-accounts-1.0.5/README.md
+-rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/RELEASING.md
+-rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.332111 heaserver-accounts-1.0.5/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.332111 heaserver-accounts-1.0.5/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.412110 heaserver-accounts-1.0.5/integrationtests/heaserver/accountintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/integrationtests/heaserver/accountintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/integrationtests/heaserver/accountintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     7748 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.5/integrationtests/heaserver/accountintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/requirements_dev.txt
+-rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-08 18:30:50.490111 heaserver-accounts-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2024-04-08 18:30:00.000000 heaserver-accounts-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.334112 heaserver-accounts-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.334112 heaserver-accounts-1.0.5/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.425108 heaserver-accounts-1.0.5/src/heaserver/account/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/src/heaserver/account/__init__.py
+-rw-rw-rw-   0        0        0    45036 2024-04-05 19:52:47.000000 heaserver-accounts-1.0.5/src/heaserver/account/service.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.432111 heaserver-accounts-1.0.5/src/heaserver/account/wstl/
+-rw-rw-rw-   0        0        0    11424 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.5/src/heaserver/account/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.488109 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/
+-rw-rw-rw-   0        0        0     5566 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.335111 heaserver-accounts-1.0.5/tests/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.335111 heaserver-accounts-1.0.5/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.486110 heaserver-accounts-1.0.5/tests/heaserver/accounttest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/tests/heaserver/accounttest/__init__.py
+-rw-rw-rw-   0        0        0     7466 2024-04-05 19:52:47.000000 heaserver-accounts-1.0.5/tests/heaserver/accounttest/test_all.py
+-rw-rw-rw-   0        0        0     5146 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.5/tests/heaserver/accounttest/testcase.py
```

### Comparing `heaserver-accounts-1.0.4/Dockerfile` & `heaserver-accounts-1.0.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.4/LICENSE` & `heaserver-accounts-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.4/PKG-INFO` & `heaserver-accounts-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.0.4
+Version: 1.0.5
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.2.0
+Requires-Dist: heaserver~=1.3.0
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.0.5
+* Improved performance getting accounts.
+
 ## Version 1.0.4
 * Corrected caching issue.
 
 ## Version 1.0.3
 * Improved error handling when the user lacks authorization for some AWS account information.
 
 ## Version 1.0.2
```

### Comparing `heaserver-accounts-1.0.4/README.md` & `heaserver-accounts-1.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.0.5
+* Improved performance getting accounts.
+
 ## Version 1.0.4
 * Corrected caching issue.
 
 ## Version 1.0.3
 * Improved error handling when the user lacks authorization for some AWS account information.
 
 ## Version 1.0.2
```

### Comparing `heaserver-accounts-1.0.4/RELEASING.md` & `heaserver-accounts-1.0.5/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.4/integrationtests/heaserver/accountintegrationtest/testcase.py` & `heaserver-accounts-1.0.5/integrationtests/heaserver/accountintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.4/run-swaggerui.py` & `heaserver-accounts-1.0.5/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.4/setup.py` & `heaserver-accounts-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-accounts',
-    version='1.0.4',
+    version='1.0.5',
     description="Manages account information",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.account'],
     package_data={'heaserver.account': ['wstl/*.json']},
     install_requires=[
-        'heaserver~=1.2.0'
+        'heaserver~=1.3.0'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
```

### Comparing `heaserver-accounts-1.0.4/src/heaserver/account/service.py` & `heaserver-accounts-1.0.5/src/heaserver/account/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.4/src/heaserver/account/wstl/all.json` & `heaserver-accounts-1.0.5/src/heaserver/account/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/PKG-INFO` & `heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.0.4
+Version: 1.0.5
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.2.0
+Requires-Dist: heaserver~=1.3.0
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.0.5
+* Improved performance getting accounts.
+
 ## Version 1.0.4
 * Corrected caching issue.
 
 ## Version 1.0.3
 * Improved error handling when the user lacks authorization for some AWS account information.
 
 ## Version 1.0.2
```

### Comparing `heaserver-accounts-1.0.4/src/heaserver_accounts.egg-info/SOURCES.txt` & `heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.4/tests/heaserver/accounttest/test_all.py` & `heaserver-accounts-1.0.5/tests/heaserver/accounttest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.4/tests/heaserver/accounttest/testcase.py` & `heaserver-accounts-1.0.5/tests/heaserver/accounttest/testcase.py`

 * *Files identical despite different names*

