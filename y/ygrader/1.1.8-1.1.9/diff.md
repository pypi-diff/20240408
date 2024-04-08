# Comparing `tmp/ygrader-1.1.8.tar.gz` & `tmp/ygrader-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygrader-1.1.8.tar", last modified: Thu Sep 15 03:25:40 2022, max compression
+gzip compressed data, was "ygrader-1.1.9.tar", last modified: Thu Sep 15 03:34:28 2022, max compression
```

## Comparing `ygrader-1.1.8.tar` & `ygrader-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2022-09-15 03:25:40.307578 ygrader-1.1.8/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      293 2022-09-15 03:25:40.307578 ygrader-1.1.8/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2022-09-15 03:25:40.307578 ygrader-1.1.8/setup.cfg
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      377 2022-09-15 03:25:30.000000 ygrader-1.1.8/setup.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2022-09-15 03:25:40.307578 ygrader-1.1.8/test/
--rwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)     1071 2022-09-03 19:02:27.000000 ygrader-1.1.8/test/test_interactive.py
--rwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)     2972 2022-09-03 19:02:27.000000 ygrader-1.1.8/test/test_unittest.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2022-09-15 03:25:40.307578 ygrader-1.1.8/ygrader/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      154 2022-09-03 19:02:27.000000 ygrader-1.1.8/ygrader/__init__.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)    32428 2022-09-03 19:46:55.000000 ygrader-1.1.8/ygrader/grader.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     4373 2022-09-03 19:02:27.000000 ygrader-1.1.8/ygrader/grades_csv.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)    12834 2022-09-15 03:25:01.000000 ygrader-1.1.8/ygrader/grading_item.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3488 2022-09-03 19:02:27.000000 ygrader-1.1.8/ygrader/student_repos.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2414 2022-09-03 19:02:27.000000 ygrader-1.1.8/ygrader/upstream_merger.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3777 2022-09-03 19:02:27.000000 ygrader-1.1.8/ygrader/utils.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2022-09-15 03:25:40.307578 ygrader-1.1.8/ygrader.egg-info/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      293 2022-09-15 03:25:40.000000 ygrader-1.1.8/ygrader.egg-info/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      362 2022-09-15 03:25:40.000000 ygrader-1.1.8/ygrader.egg-info/SOURCES.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2022-09-15 03:25:40.000000 ygrader-1.1.8/ygrader.egg-info/dependency_links.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       14 2022-09-15 03:25:40.000000 ygrader-1.1.8/ygrader.egg-info/requires.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        8 2022-09-15 03:25:40.000000 ygrader-1.1.8/ygrader.egg-info/top_level.txt
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2022-09-15 03:34:28.727578 ygrader-1.1.9/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      293 2022-09-15 03:34:28.727578 ygrader-1.1.9/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2022-09-15 03:34:28.727578 ygrader-1.1.9/setup.cfg
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      377 2022-09-15 03:34:13.000000 ygrader-1.1.9/setup.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2022-09-15 03:34:28.727578 ygrader-1.1.9/test/
+-rwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)     1071 2022-09-03 19:02:27.000000 ygrader-1.1.9/test/test_interactive.py
+-rwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)     2972 2022-09-03 19:02:27.000000 ygrader-1.1.9/test/test_unittest.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2022-09-15 03:34:28.727578 ygrader-1.1.9/ygrader/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      154 2022-09-03 19:02:27.000000 ygrader-1.1.9/ygrader/__init__.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)    32428 2022-09-03 19:46:55.000000 ygrader-1.1.9/ygrader/grader.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     4373 2022-09-03 19:02:27.000000 ygrader-1.1.9/ygrader/grades_csv.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)    12834 2022-09-15 03:33:11.000000 ygrader-1.1.9/ygrader/grading_item.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3488 2022-09-03 19:02:27.000000 ygrader-1.1.9/ygrader/student_repos.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2414 2022-09-03 19:02:27.000000 ygrader-1.1.9/ygrader/upstream_merger.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3777 2022-09-03 19:02:27.000000 ygrader-1.1.9/ygrader/utils.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2022-09-15 03:34:28.727578 ygrader-1.1.9/ygrader.egg-info/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      293 2022-09-15 03:34:28.000000 ygrader-1.1.9/ygrader.egg-info/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      362 2022-09-15 03:34:28.000000 ygrader-1.1.9/ygrader.egg-info/SOURCES.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2022-09-15 03:34:28.000000 ygrader-1.1.9/ygrader.egg-info/dependency_links.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       14 2022-09-15 03:34:28.000000 ygrader-1.1.9/ygrader.egg-info/requires.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        8 2022-09-15 03:34:28.000000 ygrader-1.1.9/ygrader.egg-info/top_level.txt
```

### Comparing `ygrader-1.1.8/test/test_interactive.py` & `ygrader-1.1.9/test/test_interactive.py`

 * *Files identical despite different names*

### Comparing `ygrader-1.1.8/test/test_unittest.py` & `ygrader-1.1.9/test/test_unittest.py`

 * *Files identical despite different names*

### Comparing `ygrader-1.1.8/ygrader/grader.py` & `ygrader-1.1.9/ygrader/grader.py`

 * *Files identical despite different names*

### Comparing `ygrader-1.1.8/ygrader/grades_csv.py` & `ygrader-1.1.9/ygrader/grades_csv.py`

 * *Files identical despite different names*

### Comparing `ygrader-1.1.8/ygrader/grading_item.py` & `ygrader-1.1.9/ygrader/grading_item.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -136,16 +136,16 @@
                         len(scores),
                         "values were returned.",
                         "Since feedback is enabled, you should return one extra item that is the feedback, which can be an empty string for no feedback."
                         if self.feedback_enabed
                         else "",
                     )
                 if self.feedback_enabled:
-                    scores = scores[:-1]
                     feedback = scores[-1]
+                    scores = scores[:-1]
 
             if scores == "s":
                 break
             if scores == "b":
                 continue
             if scores == "r":
                 # run again, but don't build
```

### Comparing `ygrader-1.1.8/ygrader/student_repos.py` & `ygrader-1.1.9/ygrader/student_repos.py`

 * *Files identical despite different names*

### Comparing `ygrader-1.1.8/ygrader/upstream_merger.py` & `ygrader-1.1.9/ygrader/upstream_merger.py`

 * *Files identical despite different names*

### Comparing `ygrader-1.1.8/ygrader/utils.py` & `ygrader-1.1.9/ygrader/utils.py`

 * *Files identical despite different names*

