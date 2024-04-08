# Comparing `tmp/git-keeper-client-1.0.3.tar.gz` & `tmp/git-keeper-client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-keeper-client-1.0.3.tar", last modified: Fri Mar 10 19:57:13 2023, max compression
+gzip compressed data, was "git-keeper-client-1.1.0.tar", last modified: Mon Apr  8 14:13:58 2024, max compression
```

## Comparing `git-keeper-client-1.0.3.tar` & `git-keeper-client-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:57:13.894845 git-keeper-client-1.0.3/
--rw-r--r--   0 nws       (1000) nws       (1000)    32386 2021-09-08 21:14:19.000000 git-keeper-client-1.0.3/LICENSE
--rw-r--r--   0 nws       (1000) nws       (1000)     1147 2023-03-10 19:57:13.894845 git-keeper-client-1.0.3/PKG-INFO
--rw-r--r--   0 nws       (1000) nws       (1000)      310 2021-09-08 21:14:19.000000 git-keeper-client-1.0.3/README.md
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:57:13.891512 git-keeper-client-1.0.3/git_keeper_client.egg-info/
--rw-r--r--   0 nws       (1000) nws       (1000)     1147 2023-03-10 19:57:13.000000 git-keeper-client-1.0.3/git_keeper_client.egg-info/PKG-INFO
--rw-r--r--   0 nws       (1000) nws       (1000)      804 2023-03-10 19:57:13.000000 git-keeper-client-1.0.3/git_keeper_client.egg-info/SOURCES.txt
--rw-r--r--   0 nws       (1000) nws       (1000)        1 2023-03-10 19:57:13.000000 git-keeper-client-1.0.3/git_keeper_client.egg-info/dependency_links.txt
--rw-r--r--   0 nws       (1000) nws       (1000)       49 2023-03-10 19:57:13.000000 git-keeper-client-1.0.3/git_keeper_client.egg-info/entry_points.txt
--rw-r--r--   0 nws       (1000) nws       (1000)       37 2023-03-10 19:57:13.000000 git-keeper-client-1.0.3/git_keeper_client.egg-info/requires.txt
--rw-r--r--   0 nws       (1000) nws       (1000)       12 2023-03-10 19:57:13.000000 git-keeper-client-1.0.3/git_keeper_client.egg-info/top_level.txt
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:57:13.894845 git-keeper-client-1.0.3/gkeepclient/
--rw-r--r--   0 nws       (1000) nws       (1000)        0 2021-09-08 21:14:19.000000 git-keeper-client-1.0.3/gkeepclient/__init__.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2775 2022-07-29 01:34:13.000000 git-keeper-client-1.0.3/gkeepclient/assignment_uploader.py
--rw-r--r--   0 nws       (1000) nws       (1000)     9456 2022-08-03 14:49:00.000000 git-keeper-client-1.0.3/gkeepclient/client_configuration.py
--rw-r--r--   0 nws       (1000) nws       (1000)    11750 2021-09-08 21:14:19.000000 git-keeper-client-1.0.3/gkeepclient/client_function_decorators.py
--rwxr-xr-x   0 nws       (1000) nws       (1000)     2824 2022-07-29 01:34:13.000000 git-keeper-client-1.0.3/gkeepclient/create_config.py
--rw-r--r--   0 nws       (1000) nws       (1000)     1487 2022-08-03 14:49:00.000000 git-keeper-client-1.0.3/gkeepclient/duration_to_string.py
--rw-r--r--   0 nws       (1000) nws       (1000)    13316 2021-09-08 21:14:19.000000 git-keeper-client-1.0.3/gkeepclient/fetch_submissions.py
--rwxr-xr-x   0 nws       (1000) nws       (1000)    20387 2022-10-21 20:05:12.000000 git-keeper-client-1.0.3/gkeepclient/gkeep.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2466 2022-08-03 14:49:00.000000 git-keeper-client-1.0.3/gkeepclient/new_assignment.py
--rw-r--r--   0 nws       (1000) nws       (1000)     8341 2021-09-08 21:14:19.000000 git-keeper-client-1.0.3/gkeepclient/queries.py
--rw-r--r--   0 nws       (1000) nws       (1000)    30264 2022-09-23 19:11:11.000000 git-keeper-client-1.0.3/gkeepclient/server_actions.py
--rw-r--r--   0 nws       (1000) nws       (1000)    22611 2021-09-08 21:14:19.000000 git-keeper-client-1.0.3/gkeepclient/server_interface.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2041 2021-09-08 21:14:19.000000 git-keeper-client-1.0.3/gkeepclient/server_log_file_reader.py
--rw-r--r--   0 nws       (1000) nws       (1000)     5716 2022-08-03 14:49:00.000000 git-keeper-client-1.0.3/gkeepclient/server_response_poller.py
--rw-r--r--   0 nws       (1000) nws       (1000)     3838 2022-07-26 16:53:32.000000 git-keeper-client-1.0.3/gkeepclient/test_solution.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2022 2021-09-08 21:14:19.000000 git-keeper-client-1.0.3/gkeepclient/text_ui.py
--rw-r--r--   0 nws       (1000) nws       (1000)      216 2023-03-10 19:43:19.000000 git-keeper-client-1.0.3/gkeepclient/version.py
--rw-r--r--   0 nws       (1000) nws       (1000)       63 2023-03-10 19:57:13.894845 git-keeper-client-1.0.3/setup.cfg
--rw-r--r--   0 nws       (1000) nws       (1000)     1287 2021-09-08 21:14:19.000000 git-keeper-client-1.0.3/setup.py
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:13:58.803336 git-keeper-client-1.1.0/
+-rw-r--r--   0 sommerm1   (503) staff       (20)    32386 2020-09-08 19:32:38.000000 git-keeper-client-1.1.0/LICENSE
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1229 2024-04-08 14:13:58.803023 git-keeper-client-1.1.0/PKG-INFO
+-rw-r--r--   0 sommerm1   (503) staff       (20)      310 2020-09-08 19:32:38.000000 git-keeper-client-1.1.0/README.md
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:13:58.801447 git-keeper-client-1.1.0/git_keeper_client.egg-info/
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1229 2024-04-08 14:13:58.000000 git-keeper-client-1.1.0/git_keeper_client.egg-info/PKG-INFO
+-rw-r--r--   0 sommerm1   (503) staff       (20)      861 2024-04-08 14:13:58.000000 git-keeper-client-1.1.0/git_keeper_client.egg-info/SOURCES.txt
+-rw-r--r--   0 sommerm1   (503) staff       (20)        1 2024-04-08 14:13:58.000000 git-keeper-client-1.1.0/git_keeper_client.egg-info/dependency_links.txt
+-rw-r--r--   0 sommerm1   (503) staff       (20)       49 2024-04-08 14:13:58.000000 git-keeper-client-1.1.0/git_keeper_client.egg-info/entry_points.txt
+-rw-r--r--   0 sommerm1   (503) staff       (20)       37 2024-04-08 14:13:58.000000 git-keeper-client-1.1.0/git_keeper_client.egg-info/requires.txt
+-rw-r--r--   0 sommerm1   (503) staff       (20)       12 2024-04-08 14:13:58.000000 git-keeper-client-1.1.0/git_keeper_client.egg-info/top_level.txt
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:13:58.800289 git-keeper-client-1.1.0/gkeepclient/
+-rw-r--r--   0 sommerm1   (503) staff       (20)        0 2019-03-18 18:24:29.000000 git-keeper-client-1.1.0/gkeepclient/__init__.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2775 2023-12-22 15:51:42.000000 git-keeper-client-1.1.0/gkeepclient/assignment_uploader.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     9456 2023-12-22 15:51:42.000000 git-keeper-client-1.1.0/gkeepclient/client_configuration.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    11750 2023-12-22 15:51:42.000000 git-keeper-client-1.1.0/gkeepclient/client_function_decorators.py
+-rwxr-xr-x   0 sommerm1   (503) staff       (20)     2824 2023-12-22 15:51:42.000000 git-keeper-client-1.1.0/gkeepclient/create_config.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1487 2023-12-22 15:51:42.000000 git-keeper-client-1.1.0/gkeepclient/duration_to_string.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    13090 2024-04-08 14:05:07.000000 git-keeper-client-1.1.0/gkeepclient/fetch_submissions.py
+-rwxr-xr-x   0 sommerm1   (503) staff       (20)    21321 2024-04-08 14:05:07.000000 git-keeper-client-1.1.0/gkeepclient/gkeep.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    12323 2024-04-08 14:05:07.000000 git-keeper-client-1.1.0/gkeepclient/local_test.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2466 2023-12-22 15:51:42.000000 git-keeper-client-1.1.0/gkeepclient/new_assignment.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     8341 2023-12-22 15:51:42.000000 git-keeper-client-1.1.0/gkeepclient/queries.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    30282 2024-04-08 14:05:07.000000 git-keeper-client-1.1.0/gkeepclient/server_actions.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    22611 2023-12-22 15:51:42.000000 git-keeper-client-1.1.0/gkeepclient/server_interface.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2041 2020-09-08 19:31:45.000000 git-keeper-client-1.1.0/gkeepclient/server_log_file_reader.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     5716 2023-12-22 15:51:42.000000 git-keeper-client-1.1.0/gkeepclient/server_response_poller.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)        0 2022-07-28 22:12:05.000000 git-keeper-client-1.1.0/gkeepclient/system_commands.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     3904 2024-04-08 14:05:07.000000 git-keeper-client-1.1.0/gkeepclient/test_solution.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2022 2020-09-08 19:31:50.000000 git-keeper-client-1.1.0/gkeepclient/text_ui.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)      216 2024-04-08 14:05:07.000000 git-keeper-client-1.1.0/gkeepclient/version.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)       63 2024-04-08 14:13:58.804321 git-keeper-client-1.1.0/setup.cfg
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1287 2020-09-08 19:32:38.000000 git-keeper-client-1.1.0/setup.py
```

### Comparing `git-keeper-client-1.0.3/LICENSE` & `git-keeper-client-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/PKG-INFO` & `git-keeper-client-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-keeper-client
-Version: 1.0.3
+Version: 1.1.0
 Summary: A git-based system for distributing and collecting programming assignments with automatic feedback.
 Home-page: https://github.com/git-keeper/git-keeper
 Author: Nathan Sommer and Ben Coleman
 Author-email: git-keeper@googlegroups.com
 License: GPL 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Education
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: git-keeper-core
+Requires-Dist: paramiko
+Requires-Dist: argcomplete
 
 # git-keeper-client
 
 This package provides the faculty client for git-keeper, a git-based system for
 distributing, testing, and collecting programming assignments.
 
 For more detailed documentation, see our GitHub repository:
```

### Comparing `git-keeper-client-1.0.3/git_keeper_client.egg-info/PKG-INFO` & `git-keeper-client-1.1.0/git_keeper_client.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-keeper-client
-Version: 1.0.3
+Version: 1.1.0
 Summary: A git-based system for distributing and collecting programming assignments with automatic feedback.
 Home-page: https://github.com/git-keeper/git-keeper
 Author: Nathan Sommer and Ben Coleman
 Author-email: git-keeper@googlegroups.com
 License: GPL 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Education
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: git-keeper-core
+Requires-Dist: paramiko
+Requires-Dist: argcomplete
 
 # git-keeper-client
 
 This package provides the faculty client for git-keeper, a git-based system for
 distributing, testing, and collecting programming assignments.
 
 For more detailed documentation, see our GitHub repository:
```

### Comparing `git-keeper-client-1.0.3/git_keeper_client.egg-info/SOURCES.txt` & `git-keeper-client-1.1.0/git_keeper_client.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 gkeepclient/assignment_uploader.py
 gkeepclient/client_configuration.py
 gkeepclient/client_function_decorators.py
 gkeepclient/create_config.py
 gkeepclient/duration_to_string.py
 gkeepclient/fetch_submissions.py
 gkeepclient/gkeep.py
+gkeepclient/local_test.py
 gkeepclient/new_assignment.py
 gkeepclient/queries.py
 gkeepclient/server_actions.py
 gkeepclient/server_interface.py
 gkeepclient/server_log_file_reader.py
 gkeepclient/server_response_poller.py
+gkeepclient/system_commands.py
 gkeepclient/test_solution.py
 gkeepclient/text_ui.py
 gkeepclient/version.py
```

### Comparing `git-keeper-client-1.0.3/gkeepclient/assignment_uploader.py` & `git-keeper-client-1.1.0/gkeepclient/assignment_uploader.py`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/gkeepclient/client_configuration.py` & `git-keeper-client-1.1.0/gkeepclient/client_configuration.py`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/gkeepclient/client_function_decorators.py` & `git-keeper-client-1.1.0/gkeepclient/client_function_decorators.py`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/gkeepclient/create_config.py` & `git-keeper-client-1.1.0/gkeepclient/create_config.py`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/gkeepclient/duration_to_string.py` & `git-keeper-client-1.1.0/gkeepclient/duration_to_string.py`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/gkeepclient/fetch_submissions.py` & `git-keeper-client-1.1.0/gkeepclient/fetch_submissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from gkeepclient.client_configuration import config
 from gkeepclient.client_function_decorators import config_parsed, \
     server_interface_connected, class_exists
 from gkeepclient.server_interface import server_interface
 from gkeepclient.server_response_poller import ServerResponsePoller, \
     ServerResponseType
 from gkeepclient.text_ui import confirmation
+from gkeepcore.git_clone_url import git_clone_url
 from gkeepcore.git_commands import is_non_bare_repo, git_head_hash, \
     git_pull, git_clone_remote
 from gkeepcore.gkeep_exception import GkeepException
 from gkeepcore.path_utils import student_assignment_repo_path
 from gkeepcore.faculty_class_info import FacultyClassInfo
 
 
@@ -156,31 +157,14 @@
         git_pull(local_repo_path, remote_url)
         hash_cache.set_hash(local_repo_path, remote_head_hash)
         print('success!')
     except GkeepException as e:
         print(str(e))
 
 
-def build_clone_url(path):
-    """
-    Build a git clone URL with the following form:
-
-    ssh://<username>@<hostname>:<port number>/<path>
-
-    The username, hostname, and port number come from the configuration file,
-    which needs to be parsed.
-
-    :param path: path to the repository on the server
-    :return:
-    """
-    return ('ssh://{0}@{1}:{2}/{3}'
-            .format(config.server_username, config.server_host,
-                    config.server_ssh_port, path))
-
-
 def fetch_student_submission(class_name: str, assignment_name: str,
                              assignment_submission_path: str,
                              remote_head_hash: str, remote_repo_path: str,
                              last_first_username: str,
                              hash_cache: FetchedHashCache):
     """
     Fetch a student's submission for an assignment.
@@ -199,15 +183,16 @@
     :param last_first_username: <last name>_<first name>_<username> for student
     :param hash_cache: cache of git commit hashes of local repositories
     """
 
     student_submission_path = os.path.join(assignment_submission_path,
                                            last_first_username)
 
-    remote_git_url = build_clone_url(remote_repo_path)
+    remote_git_url = git_clone_url(config.server_username, config.server_host,
+                                   config.server_ssh_port, remote_repo_path)
 
     # pull if the repo already exists, clone otherwise
     if os.path.isdir(student_submission_path):
         pull_repo_if_updated(student_submission_path, remote_git_url,
                              remote_head_hash, hash_cache)
     else:
         clone_repo(student_submission_path, remote_git_url)
@@ -243,15 +228,16 @@
     assignment_reports_path = os.path.join(assignment_path, 'reports')
 
     hash_cache = FetchedHashCache(assignment_path)
 
     remote_reports_path = info.reports_path(class_name, assignment_name)
     remote_reports_hash = info.reports_hash(class_name, assignment_name)
 
-    remote_git_url = build_clone_url(remote_reports_path)
+    remote_git_url = git_clone_url(config.server_username, config.server_host,
+                                   config.server_ssh_port, remote_reports_path)
 
     if os.path.isdir(assignment_reports_path):
         pull_repo_if_updated(assignment_reports_path, remote_git_url,
                              remote_reports_hash, hash_cache)
     else:
         clone_repo(assignment_reports_path, remote_git_url)
```

### Comparing `git-keeper-client-1.0.3/gkeepclient/gkeep.py` & `git-keeper-client-1.1.0/gkeepclient/gkeep.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 Provides the main entry point for the gkeep client. Parses command line
 arguments and calls the appropriate function.
 """
 
 import sys
 from argparse import ArgumentParser
 
+from gkeepclient.local_test import local_test
 from gkeepclient.version import __version__ as client_version
 from gkeepcore.path_utils import path_to_assignment_name
 from gkeepcore.version import __version__ as core_version
 
 from argcomplete import autocomplete
 from gkeepclient.client_configuration import config
 
@@ -305,14 +306,32 @@
     add_class_name_argument(subparser)
     add_assignment_name_argument(subparser)
     subparser.add_argument('solution_path',
                            metavar='<solution path>',
                            help='path to the solution directory')
 
 
+def add_local_test_subparser(subparsers):
+    """
+    Add a subparser for action 'local_test', which runs an assignment's tests
+    on a local solution directory.
+
+    :param subparsers: subparsers to add to
+    """
+
+    subparser = subparsers.add_parser('local_test',
+                                      help='test a solution locally')
+    subparser.add_argument('--cleanup', '-c', action='store_true',
+                           help='remove copies of directories after testing')
+    add_assignment_path_argument(subparser)
+    subparser.add_argument('solution_path',
+                           metavar='<solution path>',
+                           help='path to the solution directory')
+
+
 def add_config_subparser(subparsers):
     """
     Add a subparser for action 'config', which asks to create a new
     configuration file
     or to overwrite the existing one
 
     :param subparsers: subparsers to add to
@@ -431,14 +450,15 @@
     add_delete_subparser(subparsers)
     add_disable_subparser(subparsers)
     add_fetch_subparser(subparsers)
     add_query_subparser(subparsers)
     add_trigger_subparser(subparsers)
     add_passwd_subparser(subparsers)
     add_test_subparser(subparsers)
+    add_local_test_subparser(subparsers)
     add_config_subparser(subparsers)
     add_status_subparser(subparsers)
     add_add_faculty_subparser(subparsers)
     add_admin_promote_subparser(subparsers)
     add_admin_demote_subparser(subparsers)
 
     return parser
@@ -582,11 +602,14 @@
                     parsed_args.email_address)
     elif action_name == 'admin_promote':
         admin_promote(parsed_args.email_address)
     elif action_name == 'admin_demote':
         admin_demote(parsed_args.email_address)
     elif action_name == 'test':
         test_solution(class_name, assignment_name, parsed_args.solution_path)
+    elif action_name == 'local_test':
+        local_test(parsed_args.assignment_path, parsed_args.solution_path,
+                   parsed_args.cleanup)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `git-keeper-client-1.0.3/gkeepclient/new_assignment.py` & `git-keeper-client-1.1.0/gkeepclient/new_assignment.py`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/gkeepclient/queries.py` & `git-keeper-client-1.1.0/gkeepclient/queries.py`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/gkeepclient/server_actions.py` & `git-keeper-client-1.1.0/gkeepclient/server_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -661,17 +661,18 @@
     except GkeepException as e:
         error = 'Error in {0}: {1}'.format(upload_dir_path, str(e))
         raise GkeepException(error)
 
     validate_assignment_name(upload_dir.assignment_name)
 
     if not os.path.isfile(upload_dir.config_path):
-        print('NOTE: There is no assignment.cfg file for this assignment.')
-        print('      Tests for this assignment will be run using the '
-              'server\'s default environment.')
+        print('NOTE: There is no assignment.cfg file for this assignment. '
+              'Tests for this ')
+        print('      assignment will be run using the server\'s default '
+              'environment.')
 
     if server_interface.assignment_exists(class_name,
                                           upload_dir.assignment_name):
         error = ('Assignment {0} already exists in class {1}'
                  .format(upload_dir.assignment_name, class_name))
         raise GkeepException(error)
```

### Comparing `git-keeper-client-1.0.3/gkeepclient/server_interface.py` & `git-keeper-client-1.1.0/gkeepclient/server_interface.py`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/gkeepclient/server_log_file_reader.py` & `git-keeper-client-1.1.0/gkeepclient/server_log_file_reader.py`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/gkeepclient/server_response_poller.py` & `git-keeper-client-1.1.0/gkeepclient/server_response_poller.py`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/gkeepclient/test_solution.py` & `git-keeper-client-1.1.0/gkeepclient/test_solution.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from tempfile import TemporaryDirectory
 
 from gkeepclient.client_configuration import config
 from gkeepclient.client_function_decorators import config_parsed, \
     server_interface_connected, class_exists, assignment_exists
 from gkeepclient.server_actions import trigger_tests
 from gkeepclient.server_interface import server_interface
+from gkeepcore.git_clone_url import git_clone_url
 from gkeepcore.git_commands import git_clone_remote, git_add_all, git_commit, \
     git_push, git_unstaged_changes_exist
 from gkeepcore.gkeep_exception import GkeepException
 from gkeepcore.system_commands import cp, rm
 
 
 @config_parsed
@@ -69,16 +70,16 @@
 
     server_home_dir = server_interface.my_home_dir()
     server_username = config.server_username
 
     remote_repo_path = os.path.join(server_home_dir, server_username,
                                     class_name, assignment_name) + '.git'
 
-    clone_url = '{}@{}:{}'.format(server_username, config.server_host,
-                                  remote_repo_path)
+    clone_url = git_clone_url(server_username, config.server_host,
+                              config.server_ssh_port, remote_repo_path)
 
     git_clone_remote(clone_url, repo_temp_path)
 
     if os.path.isdir(os.path.join(solution_temp_path, '.git')):
         rm(os.path.join(solution_temp_path, '.git'), recursive=True)
 
     cp(os.path.join(repo_temp_path, '.git'), solution_temp_path,
```

### Comparing `git-keeper-client-1.0.3/gkeepclient/text_ui.py` & `git-keeper-client-1.1.0/gkeepclient/text_ui.py`

 * *Files identical despite different names*

### Comparing `git-keeper-client-1.0.3/setup.py` & `git-keeper-client-1.1.0/setup.py`

 * *Files identical despite different names*

