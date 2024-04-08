# Comparing `tmp/dip-coater-0.6.0.tar.gz` & `tmp/dip-coater-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dip-coater-0.6.0.tar", last modified: Mon Apr  8 07:24:37 2024, max compression
+gzip compressed data, was "dip-coater-0.7.0.tar", last modified: Mon Apr  8 07:45:11 2024, max compression
```

## Comparing `dip-coater-0.6.0.tar` & `dip-coater-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.112260 dip-coater-0.6.0/
--rw-r--r--   0 rik      (459800007) staff       (20)      100 2024-04-05 10:30:51.000000 dip-coater-0.6.0/MANIFEST.in
--rw-r--r--   0 rik      (459800007) staff       (20)     1676 2024-04-08 07:24:37.112081 dip-coater-0.6.0/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)     1094 2024-04-05 14:59:18.000000 dip-coater-0.6.0/README.md
--rw-r--r--   0 rik      (459800007) staff       (20)      843 2024-04-08 07:24:28.000000 dip-coater-0.6.0/pyproject.toml
--rw-r--r--   0 rik      (459800007) staff       (20)       38 2024-04-08 07:24:37.112305 dip-coater-0.6.0/setup.cfg
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.109475 dip-coater-0.6.0/src/
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.110074 dip-coater-0.6.0/src/MyRPi/
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.110180 dip-coater-0.6.0/src/MyRPi/GPIO/
--rw-r--r--   0 rik      (459800007) staff       (20)       26 2024-04-05 10:42:43.000000 dip-coater-0.6.0/src/MyRPi/GPIO/__init__.py
--rw-r--r--   0 rik      (459800007) staff       (20)      220 2024-04-04 11:42:49.000000 dip-coater-0.6.0/src/MyRPi/_GPIO.py
--rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-04 11:31:25.000000 dip-coater-0.6.0/src/MyRPi/__init__.py
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.110904 dip-coater-0.6.0/src/dip_coater/
--rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-05 10:07:42.000000 dip-coater-0.6.0/src/dip_coater/__init__.py
--rw-r--r--   0 rik      (459800007) staff       (20)     1263 2024-04-05 12:41:54.000000 dip-coater-0.6.0/src/dip_coater/help.md
--rw-r--r--   0 rik      (459800007) staff       (20)     4253 2024-04-05 10:58:01.000000 dip-coater-0.6.0/src/dip_coater/motor.py
--rw-r--r--   0 rik      (459800007) staff       (20)    10651 2024-04-05 13:20:19.000000 dip-coater-0.6.0/src/dip_coater/tui.py
--rw-r--r--   0 rik      (459800007) staff       (20)     1801 2024-04-05 13:00:49.000000 dip-coater-0.6.0/src/dip_coater/tui.tcss
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:24:37.111836 dip-coater-0.6.0/src/dip_coater.egg-info/
--rw-r--r--   0 rik      (459800007) staff       (20)     1676 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)      454 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/SOURCES.txt
--rw-r--r--   0 rik      (459800007) staff       (20)        1 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/dependency_links.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       51 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/entry_points.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       48 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/requires.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       17 2024-04-08 07:24:37.000000 dip-coater-0.6.0/src/dip_coater.egg-info/top_level.txt
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:45:11.009164 dip-coater-0.7.0/
+-rw-r--r--   0 rik      (459800007) staff       (20)      100 2024-04-05 10:30:51.000000 dip-coater-0.7.0/MANIFEST.in
+-rw-r--r--   0 rik      (459800007) staff       (20)     1942 2024-04-08 07:45:11.008950 dip-coater-0.7.0/PKG-INFO
+-rw-r--r--   0 rik      (459800007) staff       (20)     1292 2024-04-08 07:44:49.000000 dip-coater-0.7.0/README.md
+-rw-r--r--   0 rik      (459800007) staff       (20)      936 2024-04-08 07:32:35.000000 dip-coater-0.7.0/pyproject.toml
+-rw-r--r--   0 rik      (459800007) staff       (20)       38 2024-04-08 07:45:11.009221 dip-coater-0.7.0/setup.cfg
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:45:11.005083 dip-coater-0.7.0/src/
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:45:11.005948 dip-coater-0.7.0/src/MyRPi/
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:45:11.006091 dip-coater-0.7.0/src/MyRPi/GPIO/
+-rw-r--r--   0 rik      (459800007) staff       (20)       26 2024-04-05 10:42:43.000000 dip-coater-0.7.0/src/MyRPi/GPIO/__init__.py
+-rw-r--r--   0 rik      (459800007) staff       (20)      220 2024-04-04 11:42:49.000000 dip-coater-0.7.0/src/MyRPi/_GPIO.py
+-rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-04 11:31:25.000000 dip-coater-0.7.0/src/MyRPi/__init__.py
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:45:11.007390 dip-coater-0.7.0/src/dip_coater/
+-rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-05 10:07:42.000000 dip-coater-0.7.0/src/dip_coater/__init__.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     1263 2024-04-05 12:41:54.000000 dip-coater-0.7.0/src/dip_coater/help.md
+-rw-r--r--   0 rik      (459800007) staff       (20)     4253 2024-04-05 10:58:01.000000 dip-coater-0.7.0/src/dip_coater/motor.py
+-rw-r--r--   0 rik      (459800007) staff       (20)    10651 2024-04-05 13:20:19.000000 dip-coater-0.7.0/src/dip_coater/tui.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     1801 2024-04-05 13:00:49.000000 dip-coater-0.7.0/src/dip_coater/tui.tcss
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 07:45:11.008629 dip-coater-0.7.0/src/dip_coater.egg-info/
+-rw-r--r--   0 rik      (459800007) staff       (20)     1942 2024-04-08 07:45:10.000000 dip-coater-0.7.0/src/dip_coater.egg-info/PKG-INFO
+-rw-r--r--   0 rik      (459800007) staff       (20)      454 2024-04-08 07:45:11.000000 dip-coater-0.7.0/src/dip_coater.egg-info/SOURCES.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)        1 2024-04-08 07:45:11.000000 dip-coater-0.7.0/src/dip_coater.egg-info/dependency_links.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       51 2024-04-08 07:45:11.000000 dip-coater-0.7.0/src/dip_coater.egg-info/entry_points.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       48 2024-04-08 07:45:11.000000 dip-coater-0.7.0/src/dip_coater.egg-info/requires.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       17 2024-04-08 07:45:11.000000 dip-coater-0.7.0/src/dip_coater.egg-info/top_level.txt
```

### Comparing `dip-coater-0.6.0/PKG-INFO` & `dip-coater-0.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: dip-coater
-Version: 0.6.0
+Version: 0.7.0
 Author-email: Rik Huygen <rik.huygen@kuleuven.be>
 License: MIT License
+Project-URL: repository, https://github.com/IvS-KULeuven/dip_coater
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
@@ -44,16 +45,16 @@
 
 ```
 $ dip-coater
 ```
 
 This will show the following App in your terminal:
 
-![](images/dip-coater-dark.png)
+![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-dark.png)
 
 If you prefer light mode, press the `d` key.
 
-![](images/dip-coater-light.png)
+![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-light.png)
 
 Further help is available in the App by pressing the 'h' key:
 
-![](images/dip-coater-help-screen.png)
+![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-help-screen.png)
```

### Comparing `dip-coater-0.6.0/README.md` & `dip-coater-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 ```
 $ dip-coater
 ```
 
 This will show the following App in your terminal:
 
-![](images/dip-coater-dark.png)
+![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-dark.png)
 
 If you prefer light mode, press the `d` key.
 
-![](images/dip-coater-light.png)
+![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-light.png)
 
 Further help is available in the App by pressing the 'h' key:
 
-![](images/dip-coater-help-screen.png)
+![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-help-screen.png)
```

### Comparing `dip-coater-0.6.0/pyproject.toml` & `dip-coater-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dip-coater"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
     {name="Rik Huygen", email="rik.huygen@kuleuven.be"}
 ]
 license = { text = "MIT License" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -21,21 +21,25 @@
 
 dependencies = [
     "textual",
     "textual-dev",
     "rpimotorlib"
 ]
 
+[project.urls]
+repository = "https://github.com/IvS-KULeuven/dip_coater"
+
 [project.optional-dependencies]
 rpi = ["RPi.GPIO"]
 
 [project.scripts]
 dip-coater = "dip_coater.tui:main"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 dip_coater = [
     "*.tcss",
     "*.md",
+    "images/*.png"
 ]
```

### Comparing `dip-coater-0.6.0/src/dip_coater/help.md` & `dip-coater-0.7.0/src/dip_coater/help.md`

 * *Files identical despite different names*

### Comparing `dip-coater-0.6.0/src/dip_coater/motor.py` & `dip-coater-0.7.0/src/dip_coater/motor.py`

 * *Files identical despite different names*

### Comparing `dip-coater-0.6.0/src/dip_coater/tui.py` & `dip-coater-0.7.0/src/dip_coater/tui.py`

 * *Files identical despite different names*

### Comparing `dip-coater-0.6.0/src/dip_coater/tui.tcss` & `dip-coater-0.7.0/src/dip_coater/tui.tcss`

 * *Files identical despite different names*

### Comparing `dip-coater-0.6.0/src/dip_coater.egg-info/PKG-INFO` & `dip-coater-0.7.0/src/dip_coater.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: dip-coater
-Version: 0.6.0
+Version: 0.7.0
 Author-email: Rik Huygen <rik.huygen@kuleuven.be>
 License: MIT License
+Project-URL: repository, https://github.com/IvS-KULeuven/dip_coater
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
@@ -44,16 +45,16 @@
 
 ```
 $ dip-coater
 ```
 
 This will show the following App in your terminal:
 
-![](images/dip-coater-dark.png)
+![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-dark.png)
 
 If you prefer light mode, press the `d` key.
 
-![](images/dip-coater-light.png)
+![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-light.png)
 
 Further help is available in the App by pressing the 'h' key:
 
-![](images/dip-coater-help-screen.png)
+![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-help-screen.png)
```

