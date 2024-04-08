# Comparing `tmp/mavlinkHandler-0.0.4.tar.gz` & `tmp/mavlinkHandler-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mavlinkHandler-0.0.4.tar", last modified: Sun Apr  7 08:29:12 2024, max compression
+gzip compressed data, was "mavlinkHandler-0.0.5.tar", last modified: Sun Apr  7 08:57:43 2024, max compression
```

## Comparing `mavlinkHandler-0.0.4.tar` & `mavlinkHandler-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:29:12.423054 mavlinkHandler-0.0.4/
--rw-r--r--   0 thatcher   (501) staff       (20)    35149 2024-04-07 07:45:38.000000 mavlinkHandler-0.0.4/LICENSE
--rw-r--r--   0 thatcher   (501) staff       (20)     1184 2024-04-07 08:29:12.422839 mavlinkHandler-0.0.4/PKG-INFO
--rw-r--r--   0 thatcher   (501) staff       (20)      573 2024-04-07 08:13:11.000000 mavlinkHandler-0.0.4/README.md
-drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:29:12.421669 mavlinkHandler-0.0.4/mavlinkHandler/
--rw-r--r--   0 thatcher   (501) staff       (20)      100 2024-04-07 07:55:01.000000 mavlinkHandler-0.0.4/mavlinkHandler/__init__.py
--rw-r--r--   0 thatcher   (501) staff       (20)     7331 2024-04-07 07:53:19.000000 mavlinkHandler-0.0.4/mavlinkHandler/mavlinkHandler.py
-drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:29:12.422618 mavlinkHandler-0.0.4/mavlinkHandler.egg-info/
--rw-r--r--   0 thatcher   (501) staff       (20)     1184 2024-04-07 08:29:12.000000 mavlinkHandler-0.0.4/mavlinkHandler.egg-info/PKG-INFO
--rw-r--r--   0 thatcher   (501) staff       (20)      275 2024-04-07 08:29:12.000000 mavlinkHandler-0.0.4/mavlinkHandler.egg-info/SOURCES.txt
--rw-r--r--   0 thatcher   (501) staff       (20)        1 2024-04-07 08:29:12.000000 mavlinkHandler-0.0.4/mavlinkHandler.egg-info/dependency_links.txt
--rw-r--r--   0 thatcher   (501) staff       (20)       61 2024-04-07 08:29:12.000000 mavlinkHandler-0.0.4/mavlinkHandler.egg-info/requires.txt
--rw-r--r--   0 thatcher   (501) staff       (20)       15 2024-04-07 08:29:12.000000 mavlinkHandler-0.0.4/mavlinkHandler.egg-info/top_level.txt
--rw-r--r--   0 thatcher   (501) staff       (20)       38 2024-04-07 08:29:12.423100 mavlinkHandler-0.0.4/setup.cfg
--rw-r--r--   0 thatcher   (501) staff       (20)      814 2024-04-07 08:29:07.000000 mavlinkHandler-0.0.4/setup.py
+drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:57:43.765747 mavlinkHandler-0.0.5/
+-rw-r--r--   0 thatcher   (501) staff       (20)    35149 2024-04-07 07:45:38.000000 mavlinkHandler-0.0.5/LICENSE
+-rw-r--r--   0 thatcher   (501) staff       (20)     1190 2024-04-07 08:57:43.765516 mavlinkHandler-0.0.5/PKG-INFO
+-rw-r--r--   0 thatcher   (501) staff       (20)      579 2024-04-07 08:57:18.000000 mavlinkHandler-0.0.5/README.md
+drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:57:43.764304 mavlinkHandler-0.0.5/mavlinkHandler/
+-rw-r--r--   0 thatcher   (501) staff       (20)      100 2024-04-07 07:55:01.000000 mavlinkHandler-0.0.5/mavlinkHandler/__init__.py
+-rw-r--r--   0 thatcher   (501) staff       (20)     7331 2024-04-07 07:53:19.000000 mavlinkHandler-0.0.5/mavlinkHandler/mavlinkHandler.py
+drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:57:43.765286 mavlinkHandler-0.0.5/mavlinkHandler.egg-info/
+-rw-r--r--   0 thatcher   (501) staff       (20)     1190 2024-04-07 08:57:43.000000 mavlinkHandler-0.0.5/mavlinkHandler.egg-info/PKG-INFO
+-rw-r--r--   0 thatcher   (501) staff       (20)      275 2024-04-07 08:57:43.000000 mavlinkHandler-0.0.5/mavlinkHandler.egg-info/SOURCES.txt
+-rw-r--r--   0 thatcher   (501) staff       (20)        1 2024-04-07 08:57:43.000000 mavlinkHandler-0.0.5/mavlinkHandler.egg-info/dependency_links.txt
+-rw-r--r--   0 thatcher   (501) staff       (20)       61 2024-04-07 08:57:43.000000 mavlinkHandler-0.0.5/mavlinkHandler.egg-info/requires.txt
+-rw-r--r--   0 thatcher   (501) staff       (20)       15 2024-04-07 08:57:43.000000 mavlinkHandler-0.0.5/mavlinkHandler.egg-info/top_level.txt
+-rw-r--r--   0 thatcher   (501) staff       (20)       38 2024-04-07 08:57:43.765791 mavlinkHandler-0.0.5/setup.cfg
+-rw-r--r--   0 thatcher   (501) staff       (20)      814 2024-04-07 08:57:40.000000 mavlinkHandler-0.0.5/setup.py
```

### Comparing `mavlinkHandler-0.0.4/LICENSE` & `mavlinkHandler-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mavlinkHandler-0.0.4/PKG-INFO` & `mavlinkHandler-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavlinkHandler
-Version: 0.0.4
+Version: 0.0.5
 Summary: A controller library for UAVs, compatible with both ArduPilot and DroneKit
 Home-page: https://github.com/0EA/mavlinkHandler
 Author: Nurullah Eren Acar
 Author-email: n.erenacar13@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -19,18 +19,18 @@
 
 [![PyPI](https://img.shields.io/pypi/v/mavlinkhandler.svg)](https://pypi.org/project/mavlinkhandler/)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/your-username/mavlinkHandler/blob/main/LICENSE)
 
 mavlinkHandler is a controller library for UAVs, compatible with both ArduPilot and DroneKit.
 
 ## Installation
-
 You can install mavlinkHandler using pip:
+```
 pip install mavlinkHandler
+```
 
 ## Usage
-
 ```
 from mavlinkHandler import MAVLinkHandlerDronekit as MAVLinkHandler
 
 mavlink_handler = MAVLinkHandler('127.0.0.1:14591')
 ```
```

### Comparing `mavlinkHandler-0.0.4/README.md` & `mavlinkHandler-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 [![PyPI](https://img.shields.io/pypi/v/mavlinkhandler.svg)](https://pypi.org/project/mavlinkhandler/)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/your-username/mavlinkHandler/blob/main/LICENSE)
 
 mavlinkHandler is a controller library for UAVs, compatible with both ArduPilot and DroneKit.
 
 ## Installation
-
 You can install mavlinkHandler using pip:
+```
 pip install mavlinkHandler
+```
 
 ## Usage
-
 ```
 from mavlinkHandler import MAVLinkHandlerDronekit as MAVLinkHandler
 
 mavlink_handler = MAVLinkHandler('127.0.0.1:14591')
 ```
```

### Comparing `mavlinkHandler-0.0.4/mavlinkHandler/mavlinkHandler.py` & `mavlinkHandler-0.0.5/mavlinkHandler/mavlinkHandler.py`

 * *Files identical despite different names*

### Comparing `mavlinkHandler-0.0.4/mavlinkHandler.egg-info/PKG-INFO` & `mavlinkHandler-0.0.5/mavlinkHandler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavlinkHandler
-Version: 0.0.4
+Version: 0.0.5
 Summary: A controller library for UAVs, compatible with both ArduPilot and DroneKit
 Home-page: https://github.com/0EA/mavlinkHandler
 Author: Nurullah Eren Acar
 Author-email: n.erenacar13@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -19,18 +19,18 @@
 
 [![PyPI](https://img.shields.io/pypi/v/mavlinkhandler.svg)](https://pypi.org/project/mavlinkhandler/)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/your-username/mavlinkHandler/blob/main/LICENSE)
 
 mavlinkHandler is a controller library for UAVs, compatible with both ArduPilot and DroneKit.
 
 ## Installation
-
 You can install mavlinkHandler using pip:
+```
 pip install mavlinkHandler
+```
 
 ## Usage
-
 ```
 from mavlinkHandler import MAVLinkHandlerDronekit as MAVLinkHandler
 
 mavlink_handler = MAVLinkHandler('127.0.0.1:14591')
 ```
```

### Comparing `mavlinkHandler-0.0.4/setup.py` & `mavlinkHandler-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="mavlinkHandler",
-    version="0.0.4",
+    version="0.0.5",
     author="Nurullah Eren Acar",
     author_email="n.erenacar13@gmail.com",
     description="A controller library for UAVs, compatible with both ArduPilot and DroneKit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0EA/mavlinkHandler",
     packages=setuptools.find_packages(),
```

