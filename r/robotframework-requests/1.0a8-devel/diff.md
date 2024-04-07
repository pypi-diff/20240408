# Comparing `tmp/robotframework-requests-1.0a8.tar.gz` & `tmp/robotframework-requests-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-requests-1.0a8.tar", last modified: Tue Nov 14 22:33:29 2023, max compression
+gzip compressed data, was "dist/robotframework-requests-0.1.tar", last modified: Fri Sep  2 05:56:17 2011, max compression
```

## Comparing `robotframework-requests-1.0a8.tar` & `robotframework-requests-0.1.tar`

### file list

```diff
@@ -1,25 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 22:33:29.509219 robotframework-requests-1.0a8/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2023-11-14 22:33:29.509219 robotframework-requests-1.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5973 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 22:33:29.509219 robotframework-requests-1.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 22:33:29.505219 robotframework-requests-1.0a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 22:33:29.509219 robotframework-requests-1.0a8/src/RequestsLibrary/
--rw-r--r--   0 runner    (1001) docker     (127)    15891 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/src/RequestsLibrary/RequestsKeywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/src/RequestsLibrary/RequestsOnSessionKeywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    26195 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/src/RequestsLibrary/SessionKeywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/src/RequestsLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/src/RequestsLibrary/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/src/RequestsLibrary/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/src/RequestsLibrary/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/src/RequestsLibrary/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-14 22:33:20.000000 robotframework-requests-1.0a8/src/RequestsLibrary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 22:33:29.509219 robotframework-requests-1.0a8/src/robotframework_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2023-11-14 22:33:29.000000 robotframework-requests-1.0a8/src/robotframework_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-11-14 22:33:29.000000 robotframework-requests-1.0a8/src/robotframework_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 22:33:29.000000 robotframework-requests-1.0a8/src/robotframework_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-14 22:33:29.000000 robotframework-requests-1.0a8/src/robotframework_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-14 22:33:29.000000 robotframework-requests-1.0a8/src/robotframework_requests.egg-info/top_level.txt
+drwxr-xr-x   0 bulkan     (501) staff       (20)        0 2011-09-02 05:56:17.000000 robotframework-requests-0.1/
+-rw-r--r--   0 bulkan     (501) staff       (20)      718 2011-09-02 05:56:17.000000 robotframework-requests-0.1/PKG-INFO
+-rw-r--r--   0 bulkan     (501) staff       (20)       62 2011-09-01 05:42:38.000000 robotframework-requests-0.1/setup.cfg
+-rw-r--r--   0 bulkan     (501) staff       (20)     1168 2011-09-02 05:56:14.000000 robotframework-requests-0.1/setup.py
+drwxr-xr-x   0 bulkan     (501) staff       (20)        0 2011-09-02 05:56:17.000000 robotframework-requests-0.1/src/
+drwxr-xr-x   0 bulkan     (501) staff       (20)        0 2011-09-02 05:56:17.000000 robotframework-requests-0.1/src/RequestsLibrary/
+-rw-r--r--   0 bulkan     (501) staff       (20)      116 2011-09-02 04:21:50.000000 robotframework-requests-0.1/src/RequestsLibrary/__init__.py
+-rw-r--r--   0 bulkan     (501) staff       (20)     3784 2011-09-02 04:14:39.000000 robotframework-requests-0.1/src/RequestsLibrary/keywords.py
+-rw-r--r--   0 bulkan     (501) staff       (20)       16 2011-09-02 05:55:00.000000 robotframework-requests-0.1/src/RequestsLibrary/version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

