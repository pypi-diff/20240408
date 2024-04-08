# Comparing `tmp/python-teamcity-0.3.0.tar.gz` & `tmp/python-teamcity-0.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-teamcity-0.3.0.tar", last modified: Mon Apr  8 16:04:59 2024, max compression
+gzip compressed data, was "python-teamcity-0.3.0.dev1.tar", last modified: Sun Apr  7 16:21:26 2024, max compression
```

## Comparing `python-teamcity-0.3.0.tar` & `python-teamcity-0.3.0.dev1.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-08 16:04:59.928404 python-teamcity-0.3.0/
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-08 16:04:59.917558 python-teamcity-0.3.0/.github/
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-08 16:04:59.920520 python-teamcity-0.3.0/.github/workflows/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     2778 2024-03-09 11:42:19.000000 python-teamcity-0.3.0/.github/workflows/codeql.yml
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      104 2024-04-08 16:04:59.000000 python-teamcity-0.3.0/AUTHORS
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1865 2024-04-08 16:04:59.000000 python-teamcity-0.3.0/ChangeLog
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1072 2024-03-09 11:42:19.000000 python-teamcity-0.3.0/LICENSE
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1091 2024-04-08 16:04:59.928234 python-teamcity-0.3.0/PKG-INFO
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       65 2024-03-09 11:42:19.000000 python-teamcity-0.3.0/README.md
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-08 16:04:59.923112 python-teamcity-0.3.0/examples/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.3.0/examples/__init__.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-08 15:56:27.000000 python-teamcity-0.3.0/examples/example_auth.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-08 15:56:27.000000 python-teamcity-0.3.0/examples/example_build.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      479 2024-04-08 15:56:27.000000 python-teamcity-0.3.0/examples/example_change.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1032 2024-04-08 15:56:54.000000 python-teamcity-0.3.0/examples/example_const.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      502 2024-04-08 15:56:27.000000 python-teamcity-0.3.0/examples/example_project.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     3194 2024-04-03 11:54:17.000000 python-teamcity-0.3.0/examples/example_test.py
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-08 16:04:59.927807 python-teamcity-0.3.0/python_teamcity.egg-info/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1091 2024-04-08 16:04:59.000000 python-teamcity-0.3.0/python_teamcity.egg-info/PKG-INFO
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      631 2024-04-08 16:04:59.000000 python-teamcity-0.3.0/python_teamcity.egg-info/SOURCES.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-04-08 16:04:59.000000 python-teamcity-0.3.0/python_teamcity.egg-info/dependency_links.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-03-14 09:27:40.000000 python-teamcity-0.3.0/python_teamcity.egg-info/not-zip-safe
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       47 2024-04-08 16:04:59.000000 python-teamcity-0.3.0/python_teamcity.egg-info/pbr.json
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-04-08 16:04:59.000000 python-teamcity-0.3.0/python_teamcity.egg-info/requires.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-04-08 16:04:59.000000 python-teamcity-0.3.0/python_teamcity.egg-info/top_level.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        8 2024-03-09 11:42:19.000000 python-teamcity-0.3.0/requirements.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      900 2024-04-08 16:04:59.928740 python-teamcity-0.3.0/setup.cfg
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      128 2024-03-09 11:42:19.000000 python-teamcity-0.3.0/setup.py
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-08 16:04:59.927000 python-teamcity-0.3.0/teamcity/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       31 2024-03-09 11:42:19.000000 python-teamcity-0.3.0/teamcity/__init__.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)    27880 2024-04-08 15:56:27.000000 python-teamcity-0.3.0/teamcity/teamcity.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      449 2024-04-08 15:56:27.000000 python-teamcity-0.3.0/teamcity/teamcity_const.py
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-08 16:04:59.927440 python-teamcity-0.3.0/tests/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.3.0/tests/__init__.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.737389 python-teamcity-0.3.0.dev1/
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.726424 python-teamcity-0.3.0.dev1/.github/
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.729466 python-teamcity-0.3.0.dev1/.github/workflows/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     2778 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/.github/workflows/codeql.yml
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      104 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/AUTHORS
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1693 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/ChangeLog
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1072 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/LICENSE
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1096 2024-04-07 16:21:26.737206 python-teamcity-0.3.0.dev1/PKG-INFO
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       65 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/README.md
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.731741 python-teamcity-0.3.0.dev1/examples/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/examples/__init__.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:17.000000 python-teamcity-0.3.0.dev1/examples/example_auth.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:17.000000 python-teamcity-0.3.0.dev1/examples/example_build.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      479 2024-04-07 16:13:56.000000 python-teamcity-0.3.0.dev1/examples/example_change.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1034 2024-04-03 11:54:17.000000 python-teamcity-0.3.0.dev1/examples/example_const.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     3194 2024-04-03 11:54:17.000000 python-teamcity-0.3.0.dev1/examples/example_test.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.736752 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1096 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/PKG-INFO
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      603 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/SOURCES.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/dependency_links.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-03-14 09:27:40.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/not-zip-safe
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       47 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/pbr.json
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/requires.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/top_level.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        8 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/requirements.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      900 2024-04-07 16:21:26.737750 python-teamcity-0.3.0.dev1/setup.cfg
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      128 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/setup.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.735818 python-teamcity-0.3.0.dev1/teamcity/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       31 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/teamcity/__init__.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)    27124 2024-04-07 16:17:59.000000 python-teamcity-0.3.0.dev1/teamcity/teamcity.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      449 2024-04-04 09:43:54.000000 python-teamcity-0.3.0.dev1/teamcity/teamcity_const.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.736414 python-teamcity-0.3.0.dev1/tests/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/tests/__init__.py
```

### Comparing `python-teamcity-0.3.0/.github/workflows/codeql.yml` & `python-teamcity-0.3.0.dev1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.3.0/ChangeLog` & `python-teamcity-0.3.0.dev1/ChangeLog`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 CHANGES
 =======
 
-v0.3.0
-------
-
-* Support to get project build type. Add details parameter:True to get details, False to return build type id list
-* Add get\_project\_build\_types function
 * Add support for fetching build queue changes and refactor authentication
 
 v0.2.9
 ------
 
 * Support to get latest build detail by build type id
```

### Comparing `python-teamcity-0.3.0/LICENSE` & `python-teamcity-0.3.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.3.0/PKG-INFO` & `python-teamcity-0.3.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-teamcity
-Version: 0.3.0
+Version: 0.3.0.dev1
 Summary: Python library for triggering TeamCity by REST API
 Home-page: https://github.com/norbread2003/python-teamcity
 Author: Yunlin Tan
 Author-email: tanyunlin2003@norbread.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `python-teamcity-0.3.0/examples/example_const.py` & `python-teamcity-0.3.0.dev1/examples/example_const.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,10 +33,9 @@
 """
 import os
 
 # It is recommended to obtain TeamCity authorization via environment variables.
 TEAMCITY_SERVER = os.environ.get('TEAMCITY_SERVER', None)
 TEAMCITY_TOKENS = os.environ.get('TEAMCITY_TOKENS', None)
 
-EX_BUILD_ID = 0  # Replace with your build_id
-EX_BUILD_TYPE_ID = 'Test'  # Replace with your build_type_id
-EX_PROJECT_ID = 'Test'  # Replace with your project_id
+EX_BUILD_ID = 35193036  # Replace with your build_id
+EX_BUILD_TYPE_ID = 'Tools_TeamcityBuildStatsCollector_StaticDataCollection'  # Replace with your build_type_id
```

### Comparing `python-teamcity-0.3.0/examples/example_test.py` & `python-teamcity-0.3.0.dev1/examples/example_test.py`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.3.0/python_teamcity.egg-info/PKG-INFO` & `python-teamcity-0.3.0.dev1/python_teamcity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-teamcity
-Version: 0.3.0
+Version: 0.3.0.dev1
 Summary: Python library for triggering TeamCity by REST API
 Home-page: https://github.com/norbread2003/python-teamcity
 Author: Yunlin Tan
 Author-email: tanyunlin2003@norbread.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `python-teamcity-0.3.0/python_teamcity.egg-info/SOURCES.txt` & `python-teamcity-0.3.0.dev1/python_teamcity.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 setup.py
 .github/workflows/codeql.yml
 examples/__init__.py
 examples/example_auth.py
 examples/example_build.py
 examples/example_change.py
 examples/example_const.py
-examples/example_project.py
 examples/example_test.py
 python_teamcity.egg-info/PKG-INFO
 python_teamcity.egg-info/SOURCES.txt
 python_teamcity.egg-info/dependency_links.txt
 python_teamcity.egg-info/not-zip-safe
 python_teamcity.egg-info/pbr.json
 python_teamcity.egg-info/requires.txt
```

### Comparing `python-teamcity-0.3.0/setup.cfg` & `python-teamcity-0.3.0.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.3.0/teamcity/teamcity.py` & `python-teamcity-0.3.0.dev1/teamcity/teamcity.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,32 +445,14 @@
                 logging.info(f'No pending changes found for build type {build_type_id}.')
                 return list()
         except Exception as ex:
             logging.error(ex)
             logging.error(f'Failed to get pending changes from TeamCity.')
             return list()
 
-    def get_project_build_types(self, project_id, details=True):
-        """Get project build types by project id from TeamCity.
-
-        :param project_id: project id in TeamCity.
-        :param details: True to get details, False to return build type id list.
-        :return: list of build types or list of build type ids.
-        """
-        url = f'projects/id:{project_id}/buildTypes'
-        try:
-            if details:
-                return self.get_request(url)['buildType']
-            else:
-                return [build['id'] for build in self.get_request(url)['buildType']]
-        except Exception as ex:
-            logging.error(ex)
-            logging.error(f'Failed to get project {project_id} build types.')
-            return list()
-
     def get_user(self, username='') -> dict:
         """Get user by username from TeamCity.
 
         :param username: username, if empty - get current user
         :return: user dict, for example:
 
         {'username': 'teamcity', 'name': 'Teamcity', 'id': 200, 'email': 'support@jetbrains.com',
```

