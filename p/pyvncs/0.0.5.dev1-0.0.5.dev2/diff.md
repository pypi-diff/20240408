# Comparing `tmp/pyvncs-0.0.5.dev1.tar.gz` & `tmp/pyvncs-0.0.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvncs-0.0.5.dev1.tar", last modified: Mon Apr  8 03:44:53 2024, max compression
+gzip compressed data, was "pyvncs-0.0.5.dev2.tar", last modified: Mon Apr  8 03:52:04 2024, max compression
```

## Comparing `pyvncs-0.0.5.dev1.tar` & `pyvncs-0.0.5.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:44:53.449296 pyvncs-0.0.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-08 03:44:47.000000 pyvncs-0.0.5.dev1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 03:44:53.449296 pyvncs-0.0.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-08 03:44:47.000000 pyvncs-0.0.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:44:53.449296 pyvncs-0.0.5.dev1/pyvncs/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 03:44:47.000000 pyvncs-0.0.5.dev1/pyvncs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15011 2024-04-08 03:44:47.000000 pyvncs-0.0.5.dev1/pyvncs/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:44:53.449296 pyvncs-0.0.5.dev1/pyvncs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 03:44:53.000000 pyvncs-0.0.5.dev1/pyvncs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 03:44:53.000000 pyvncs-0.0.5.dev1/pyvncs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:44:53.000000 pyvncs-0.0.5.dev1/pyvncs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:44:53.000000 pyvncs-0.0.5.dev1/pyvncs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 03:44:53.000000 pyvncs-0.0.5.dev1/pyvncs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 03:44:53.000000 pyvncs-0.0.5.dev1/pyvncs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 03:44:53.449296 pyvncs-0.0.5.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-08 03:44:47.000000 pyvncs-0.0.5.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:52:04.901193 pyvncs-0.0.5.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-08 03:51:58.000000 pyvncs-0.0.5.dev2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-08 03:52:04.901193 pyvncs-0.0.5.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-08 03:51:58.000000 pyvncs-0.0.5.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:52:04.901193 pyvncs-0.0.5.dev2/pyvncs/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 03:51:58.000000 pyvncs-0.0.5.dev2/pyvncs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15011 2024-04-08 03:51:58.000000 pyvncs-0.0.5.dev2/pyvncs/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:52:04.901193 pyvncs-0.0.5.dev2/pyvncs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-08 03:52:04.000000 pyvncs-0.0.5.dev2/pyvncs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 03:52:04.000000 pyvncs-0.0.5.dev2/pyvncs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:52:04.000000 pyvncs-0.0.5.dev2/pyvncs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:52:04.000000 pyvncs-0.0.5.dev2/pyvncs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 03:52:04.000000 pyvncs-0.0.5.dev2/pyvncs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 03:52:04.000000 pyvncs-0.0.5.dev2/pyvncs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 03:52:04.901193 pyvncs-0.0.5.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-08 03:51:58.000000 pyvncs-0.0.5.dev2/setup.py
```

### Comparing `pyvncs-0.0.5.dev1/README.md` & `pyvncs-0.0.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `pyvncs-0.0.5.dev1/pyvncs/__init__.py` & `pyvncs-0.0.5.dev2/pyvncs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvncs-0.0.5.dev1/pyvncs/server.py` & `pyvncs-0.0.5.dev2/pyvncs/server.py`

 * *Files identical despite different names*

### Comparing `pyvncs-0.0.5.dev1/setup.py` & `pyvncs-0.0.5.dev2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,10 +16,10 @@
     setup_requires=["setuptools-git-versioning"],
     description="A 3rd-party package of pyvncs since the author has not published it to pypi",
     long_description="A 3rd-party package of pyvncs since the author has not published it to pypi",
     url="http://github.com/darkpixel/pyvncs",
     author="Matias Fernandez",
     author_email="matias.fernandez@gmail.com",
     packages=["pyvncs"],
-    install_requires=["pyDes", "pynput", "numpy", "Pillow-PIL", "elevate", "pyautogui"],
+    install_requires=["pyDes", "pynput", "numpy", "Pillow-PIL"],
     zip_safe=False,
 )
```

