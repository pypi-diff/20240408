# Comparing `tmp/git-keeper-core-1.0.3.tar.gz` & `tmp/git-keeper-core-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-keeper-core-1.0.3.tar", last modified: Fri Mar 10 19:47:09 2023, max compression
+gzip compressed data, was "git-keeper-core-1.1.0.tar", last modified: Mon Apr  8 14:12:39 2024, max compression
```

## Comparing `git-keeper-core-1.0.3.tar` & `git-keeper-core-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:47:09.550189 git-keeper-core-1.0.3/
--rw-r--r--   0 nws       (1000) nws       (1000)    32386 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/LICENSE
--rw-r--r--   0 nws       (1000) nws       (1000)     1064 2023-03-10 19:47:09.550189 git-keeper-core-1.0.3/PKG-INFO
--rw-r--r--   0 nws       (1000) nws       (1000)      306 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/README.md
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:47:09.550189 git-keeper-core-1.0.3/git_keeper_core.egg-info/
--rw-r--r--   0 nws       (1000) nws       (1000)     1064 2023-03-10 19:47:09.000000 git-keeper-core-1.0.3/git_keeper_core.egg-info/PKG-INFO
--rw-r--r--   0 nws       (1000) nws       (1000)      750 2023-03-10 19:47:09.000000 git-keeper-core-1.0.3/git_keeper_core.egg-info/SOURCES.txt
--rw-r--r--   0 nws       (1000) nws       (1000)        1 2023-03-10 19:47:09.000000 git-keeper-core-1.0.3/git_keeper_core.egg-info/dependency_links.txt
--rw-r--r--   0 nws       (1000) nws       (1000)        7 2023-03-10 19:47:09.000000 git-keeper-core-1.0.3/git_keeper_core.egg-info/requires.txt
--rw-r--r--   0 nws       (1000) nws       (1000)       10 2023-03-10 19:47:09.000000 git-keeper-core-1.0.3/git_keeper_core.egg-info/top_level.txt
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:47:09.550189 git-keeper-core-1.0.3/gkeepcore/
--rw-r--r--   0 nws       (1000) nws       (1000)        0 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/gkeepcore/__init__.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2229 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/gkeepcore/action_scripts.py
--rw-r--r--   0 nws       (1000) nws       (1000)      977 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/gkeepcore/assignment.py
--rw-r--r--   0 nws       (1000) nws       (1000)    10776 2022-10-21 20:05:12.000000 git-keeper-core-1.0.3/gkeepcore/assignment_config.py
--rw-r--r--   0 nws       (1000) nws       (1000)     1275 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/gkeepcore/csv_files.py
--rw-r--r--   0 nws       (1000) nws       (1000)     3940 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/gkeepcore/faculty.py
--rw-r--r--   0 nws       (1000) nws       (1000)    13884 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/gkeepcore/faculty_class_info.py
--rw-r--r--   0 nws       (1000) nws       (1000)     7802 2022-06-03 20:00:23.000000 git-keeper-core-1.0.3/gkeepcore/git_commands.py
--rw-r--r--   0 nws       (1000) nws       (1000)      763 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/gkeepcore/gkeep_exception.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2571 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/gkeepcore/local_csv_files.py
--rw-r--r--   0 nws       (1000) nws       (1000)     8072 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/gkeepcore/log_file.py
--rw-r--r--   0 nws       (1000) nws       (1000)    11263 2022-06-03 20:00:23.000000 git-keeper-core-1.0.3/gkeepcore/path_utils.py
--rw-r--r--   0 nws       (1000) nws       (1000)     5386 2022-08-03 14:49:00.000000 git-keeper-core-1.0.3/gkeepcore/shell_command.py
--rw-r--r--   0 nws       (1000) nws       (1000)     5191 2022-07-22 23:35:44.000000 git-keeper-core-1.0.3/gkeepcore/student.py
--rw-r--r--   0 nws       (1000) nws       (1000)    10265 2022-08-05 19:50:53.000000 git-keeper-core-1.0.3/gkeepcore/system_commands.py
--rw-r--r--   0 nws       (1000) nws       (1000)     4237 2022-07-29 01:34:13.000000 git-keeper-core-1.0.3/gkeepcore/upload_directory.py
--rw-r--r--   0 nws       (1000) nws       (1000)     3430 2022-10-21 18:46:05.000000 git-keeper-core-1.0.3/gkeepcore/valid_names.py
--rw-r--r--   0 nws       (1000) nws       (1000)      216 2023-03-10 19:43:19.000000 git-keeper-core-1.0.3/gkeepcore/version.py
--rw-r--r--   0 nws       (1000) nws       (1000)       63 2023-03-10 19:47:09.550189 git-keeper-core-1.0.3/setup.cfg
--rw-r--r--   0 nws       (1000) nws       (1000)     1058 2022-07-19 17:04:59.000000 git-keeper-core-1.0.3/setup.py
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:47:09.550189 git-keeper-core-1.0.3/tests/
--rw-r--r--   0 nws       (1000) nws       (1000)     1580 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/tests/test_path_utils.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2477 2021-09-08 21:14:19.000000 git-keeper-core-1.0.3/tests/test_upload_directory.py
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:12:39.828399 git-keeper-core-1.1.0/
+-rw-r--r--   0 sommerm1   (503) staff       (20)    32386 2020-09-08 19:32:38.000000 git-keeper-core-1.1.0/LICENSE
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1086 2024-04-08 14:12:39.828169 git-keeper-core-1.1.0/PKG-INFO
+-rw-r--r--   0 sommerm1   (503) staff       (20)      306 2020-09-08 19:32:38.000000 git-keeper-core-1.1.0/README.md
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:12:39.827368 git-keeper-core-1.1.0/git_keeper_core.egg-info/
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1086 2024-04-08 14:12:39.000000 git-keeper-core-1.1.0/git_keeper_core.egg-info/PKG-INFO
+-rw-r--r--   0 sommerm1   (503) staff       (20)      801 2024-04-08 14:12:39.000000 git-keeper-core-1.1.0/git_keeper_core.egg-info/SOURCES.txt
+-rw-r--r--   0 sommerm1   (503) staff       (20)        1 2024-04-08 14:12:39.000000 git-keeper-core-1.1.0/git_keeper_core.egg-info/dependency_links.txt
+-rw-r--r--   0 sommerm1   (503) staff       (20)        7 2024-04-08 14:12:39.000000 git-keeper-core-1.1.0/git_keeper_core.egg-info/requires.txt
+-rw-r--r--   0 sommerm1   (503) staff       (20)       10 2024-04-08 14:12:39.000000 git-keeper-core-1.1.0/git_keeper_core.egg-info/top_level.txt
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:12:39.824794 git-keeper-core-1.1.0/gkeepcore/
+-rw-r--r--   0 sommerm1   (503) staff       (20)        0 2019-03-18 18:24:29.000000 git-keeper-core-1.1.0/gkeepcore/__init__.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2229 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/action_scripts.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)      977 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/assignment.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    10933 2024-04-08 14:05:07.000000 git-keeper-core-1.1.0/gkeepcore/assignment_config.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1275 2020-09-08 19:31:45.000000 git-keeper-core-1.1.0/gkeepcore/csv_files.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     3940 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/faculty.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    13884 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/faculty_class_info.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1392 2024-04-08 14:05:07.000000 git-keeper-core-1.1.0/gkeepcore/git_clone_url.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     7802 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/git_commands.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)      763 2020-09-08 19:31:45.000000 git-keeper-core-1.1.0/gkeepcore/gkeep_exception.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2571 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/local_csv_files.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     8072 2020-09-08 19:32:04.000000 git-keeper-core-1.1.0/gkeepcore/log_file.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    11263 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/path_utils.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     5386 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/shell_command.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     5191 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/student.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    10265 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/system_commands.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)      763 2024-04-08 14:05:07.000000 git-keeper-core-1.1.0/gkeepcore/temp_paths.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     4237 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/upload_directory.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     3430 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/gkeepcore/valid_names.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)      216 2024-04-08 14:05:07.000000 git-keeper-core-1.1.0/gkeepcore/version.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)       63 2024-04-08 14:12:39.829157 git-keeper-core-1.1.0/setup.cfg
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1058 2023-12-22 15:51:42.000000 git-keeper-core-1.1.0/setup.py
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:12:39.826413 git-keeper-core-1.1.0/tests/
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1580 2020-09-08 19:31:37.000000 git-keeper-core-1.1.0/tests/test_path_utils.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2477 2020-09-08 19:31:45.000000 git-keeper-core-1.1.0/tests/test_upload_directory.py
```

### Comparing `git-keeper-core-1.0.3/LICENSE` & `git-keeper-core-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/PKG-INFO` & `git-keeper-core-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-keeper-core
-Version: 1.0.3
+Version: 1.1.0
 Summary: Core modules for git-keeper-client and git-keeper-server.
 Home-page: https://github.com/git-keeper/git-keeper
 Author: Nathan Sommer and Ben Coleman
 Author-email: git-keeper@googlegroups.com
 License: GPL 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Education
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
 
 # git-keeper-core
 
 This package is a dependency for git-keeper-client and git-keeper-server. It
 provides functionality that is shared between the two packages.
 
 For more detailed documentation, see our GitHub repository:
```

### Comparing `git-keeper-core-1.0.3/git_keeper_core.egg-info/PKG-INFO` & `git-keeper-core-1.1.0/git_keeper_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-keeper-core
-Version: 1.0.3
+Version: 1.1.0
 Summary: Core modules for git-keeper-client and git-keeper-server.
 Home-page: https://github.com/git-keeper/git-keeper
 Author: Nathan Sommer and Ben Coleman
 Author-email: git-keeper@googlegroups.com
 License: GPL 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Education
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
 
 # git-keeper-core
 
 This package is a dependency for git-keeper-client and git-keeper-server. It
 provides functionality that is shared between the two packages.
 
 For more detailed documentation, see our GitHub repository:
```

### Comparing `git-keeper-core-1.0.3/git_keeper_core.egg-info/SOURCES.txt` & `git-keeper-core-1.1.0/git_keeper_core.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 gkeepcore/__init__.py
 gkeepcore/action_scripts.py
 gkeepcore/assignment.py
 gkeepcore/assignment_config.py
 gkeepcore/csv_files.py
 gkeepcore/faculty.py
 gkeepcore/faculty_class_info.py
+gkeepcore/git_clone_url.py
 gkeepcore/git_commands.py
 gkeepcore/gkeep_exception.py
 gkeepcore/local_csv_files.py
 gkeepcore/log_file.py
 gkeepcore/path_utils.py
 gkeepcore/shell_command.py
 gkeepcore/student.py
 gkeepcore/system_commands.py
+gkeepcore/temp_paths.py
 gkeepcore/upload_directory.py
 gkeepcore/valid_names.py
 gkeepcore/version.py
 tests/test_path_utils.py
 tests/test_upload_directory.py
```

### Comparing `git-keeper-core-1.0.3/gkeepcore/action_scripts.py` & `git-keeper-core-1.1.0/gkeepcore/action_scripts.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/assignment.py` & `git-keeper-core-1.1.0/gkeepcore/assignment.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/assignment_config.py` & `git-keeper-core-1.1.0/gkeepcore/assignment_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -288,26 +288,29 @@
     try:
         run_command(cmd)
     except CommandError:
         raise GkeepException('firejail does not appear to be installed on '
                              'the server')
 
 
-def verify_docker_installed():
+def verify_docker_installed(location='on the server'):
     """
     Determine if Docker is installed.
     Raises GkeepException if Docker is not installed.
+
+    :param location: string used in the exception error message for the
+     location where docker installation is being tested
     """
     cmd = ['docker', '--version']
 
     try:
         run_command(cmd)
     except CommandError:
-        raise GkeepException('docker does not appear to be installed on the '
-                             'server')
+        raise GkeepException('docker does not appear to be installed {}'
+                             .format(location))
 
 
 def verify_docker_image(image):
     """
     Determine whether a Docker image exits.
     Raises GkeepException if the image does not exist
```

### Comparing `git-keeper-core-1.0.3/gkeepcore/csv_files.py` & `git-keeper-core-1.1.0/gkeepcore/csv_files.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/faculty.py` & `git-keeper-core-1.1.0/gkeepcore/faculty.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/faculty_class_info.py` & `git-keeper-core-1.1.0/gkeepcore/faculty_class_info.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/git_commands.py` & `git-keeper-core-1.1.0/gkeepcore/git_commands.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/gkeep_exception.py` & `git-keeper-core-1.1.0/gkeepcore/gkeep_exception.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/local_csv_files.py` & `git-keeper-core-1.1.0/gkeepcore/local_csv_files.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/log_file.py` & `git-keeper-core-1.1.0/gkeepcore/log_file.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/path_utils.py` & `git-keeper-core-1.1.0/gkeepcore/path_utils.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/shell_command.py` & `git-keeper-core-1.1.0/gkeepcore/shell_command.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/student.py` & `git-keeper-core-1.1.0/gkeepcore/student.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/system_commands.py` & `git-keeper-core-1.1.0/gkeepcore/system_commands.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/upload_directory.py` & `git-keeper-core-1.1.0/gkeepcore/upload_directory.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/gkeepcore/valid_names.py` & `git-keeper-core-1.1.0/gkeepcore/valid_names.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/setup.py` & `git-keeper-core-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/tests/test_path_utils.py` & `git-keeper-core-1.1.0/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `git-keeper-core-1.0.3/tests/test_upload_directory.py` & `git-keeper-core-1.1.0/tests/test_upload_directory.py`

 * *Files identical despite different names*

