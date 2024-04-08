# Comparing `tmp/gitlab-job-exec-1.5.106.tar.gz` & `tmp/gitlab-job-exec-1.5.108.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-job-exec-1.5.106.tar", last modified: Tue Oct  3 11:31:04 2023, max compression
+gzip compressed data, was "gitlab-job-exec-1.5.108.tar", last modified: Mon Apr  8 16:08:42 2024, max compression
```

## Comparing `gitlab-job-exec-1.5.106.tar` & `gitlab-job-exec-1.5.108.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 11:31:04.070887 gitlab-job-exec-1.5.106/
--rw-r--r--   0 root         (0) root         (0)     7157 2023-10-03 11:31:04.069887 gitlab-job-exec-1.5.106/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5686 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 11:31:04.067888 gitlab-job-exec-1.5.106/gitlab_job_exec/
--rwxrwxrwx   0 root         (0) root         (0)    17561 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/gitlab_job_exec/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7919 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/gitlab_job_exec/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 11:31:04.068888 gitlab-job-exec-1.5.106/gitlab_job_exec.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7157 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/gitlab_job_exec.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      371 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/gitlab_job_exec.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/gitlab_job_exec.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/gitlab_job_exec.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/gitlab_job_exec.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/gitlab_job_exec.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-03 11:31:04.070887 gitlab-job-exec-1.5.106/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1571 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 11:31:04.069887 gitlab-job-exec-1.5.106/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14255 2023-10-03 11:31:03.000000 gitlab-job-exec-1.5.106/tests/test_gitlab_job_exec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:08:42.618053 gitlab-job-exec-1.5.108/
+-rw-r--r--   0 root         (0) root         (0)     7157 2024-04-08 16:08:42.618053 gitlab-job-exec-1.5.108/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5686 2024-04-08 16:08:41.000000 gitlab-job-exec-1.5.108/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:08:42.616053 gitlab-job-exec-1.5.108/gitlab_job_exec/
+-rwxrwxrwx   0 root         (0) root         (0)    17561 2024-04-08 16:08:41.000000 gitlab-job-exec-1.5.108/gitlab_job_exec/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7919 2024-04-08 16:08:41.000000 gitlab-job-exec-1.5.108/gitlab_job_exec/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:08:42.617053 gitlab-job-exec-1.5.108/gitlab_job_exec.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7157 2024-04-08 16:08:42.000000 gitlab-job-exec-1.5.108/gitlab_job_exec.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      371 2024-04-08 16:08:42.000000 gitlab-job-exec-1.5.108/gitlab_job_exec.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:08:42.000000 gitlab-job-exec-1.5.108/gitlab_job_exec.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-08 16:08:42.000000 gitlab-job-exec-1.5.108/gitlab_job_exec.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-08 16:08:42.000000 gitlab-job-exec-1.5.108/gitlab_job_exec.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-08 16:08:42.000000 gitlab-job-exec-1.5.108/gitlab_job_exec.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 16:08:42.618053 gitlab-job-exec-1.5.108/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-08 16:08:41.000000 gitlab-job-exec-1.5.108/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:08:42.618053 gitlab-job-exec-1.5.108/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:08:41.000000 gitlab-job-exec-1.5.108/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2024-04-08 16:08:41.000000 gitlab-job-exec-1.5.108/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14255 2024-04-08 16:08:41.000000 gitlab-job-exec-1.5.108/tests/test_gitlab_job_exec.py
```

### Comparing `gitlab-job-exec-1.5.106/PKG-INFO` & `gitlab-job-exec-1.5.108/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-job-exec
-Version: 1.5.106
+Version: 1.5.108
 Summary: Execute GitLab-CI docker jobs
 Home-page: https://gitlab.com/uncrns/gitlab-job-exec
 Author: Uncrns
 Author-email: uncrns.devs@gmail.com
 License: UNKNOWN
 Description: ## GitLab-CI Job Executor
```

### Comparing `gitlab-job-exec-1.5.106/README.md` & `gitlab-job-exec-1.5.108/README.md`

 * *Files identical despite different names*

### Comparing `gitlab-job-exec-1.5.106/gitlab_job_exec/__init__.py` & `gitlab-job-exec-1.5.108/gitlab_job_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlab-job-exec-1.5.106/gitlab_job_exec/cli.py` & `gitlab-job-exec-1.5.108/gitlab_job_exec/cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-job-exec-1.5.106/gitlab_job_exec.egg-info/PKG-INFO` & `gitlab-job-exec-1.5.108/gitlab_job_exec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-job-exec
-Version: 1.5.106
+Version: 1.5.108
 Summary: Execute GitLab-CI docker jobs
 Home-page: https://gitlab.com/uncrns/gitlab-job-exec
 Author: Uncrns
 Author-email: uncrns.devs@gmail.com
 License: UNKNOWN
 Description: ## GitLab-CI Job Executor
```

### Comparing `gitlab-job-exec-1.5.106/setup.py` & `gitlab-job-exec-1.5.108/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab-job-exec-1.5.106/tests/test_cli.py` & `gitlab-job-exec-1.5.108/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-job-exec-1.5.106/tests/test_gitlab_job_exec.py` & `gitlab-job-exec-1.5.108/tests/test_gitlab_job_exec.py`

 * *Files identical despite different names*

