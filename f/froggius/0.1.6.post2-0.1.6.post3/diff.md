# Comparing `tmp/froggius-0.1.6.post2.tar.gz` & `tmp/froggius-0.1.6.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froggius-0.1.6.post2.tar", last modified: Wed Apr  3 14:52:14 2024, max compression
+gzip compressed data, was "froggius-0.1.6.post3.tar", last modified: Mon Apr  8 16:02:53 2024, max compression
```

## Comparing `froggius-0.1.6.post2.tar` & `froggius-0.1.6.post3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:14.752254 froggius-0.1.6.post2/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-03 14:52:08.000000 froggius-0.1.6.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-03 14:52:14.752254 froggius-0.1.6.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-03 14:52:08.000000 froggius-0.1.6.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:14.752254 froggius-0.1.6.post2/froggius/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 14:52:12.000000 froggius-0.1.6.post2/froggius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-03 14:52:12.000000 froggius-0.1.6.post2/froggius/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:14.752254 froggius-0.1.6.post2/froggius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-03 14:52:14.000000 froggius-0.1.6.post2/froggius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 14:52:14.000000 froggius-0.1.6.post2/froggius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:52:14.000000 froggius-0.1.6.post2/froggius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 14:52:14.000000 froggius-0.1.6.post2/froggius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:52:14.752254 froggius-0.1.6.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-03 14:52:12.000000 froggius-0.1.6.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:02:53.065500 froggius-0.1.6.post3/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-08 16:02:31.000000 froggius-0.1.6.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-08 16:02:53.061500 froggius-0.1.6.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-08 16:02:31.000000 froggius-0.1.6.post3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:02:53.061500 froggius-0.1.6.post3/froggius/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-08 16:02:48.000000 froggius-0.1.6.post3/froggius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-08 16:02:48.000000 froggius-0.1.6.post3/froggius/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:02:53.061500 froggius-0.1.6.post3/froggius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-08 16:02:53.000000 froggius-0.1.6.post3/froggius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-08 16:02:53.000000 froggius-0.1.6.post3/froggius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:02:53.000000 froggius-0.1.6.post3/froggius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 16:02:53.000000 froggius-0.1.6.post3/froggius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:02:53.065500 froggius-0.1.6.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-08 16:02:48.000000 froggius-0.1.6.post3/setup.py
```

### Comparing `froggius-0.1.6.post2/LICENSE` & `froggius-0.1.6.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `froggius-0.1.6.post2/PKG-INFO` & `froggius-0.1.6.post3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.6.post2
-Summary: Froggius is a dumb easy logging tool for python
+Version: 0.1.6.post3
+Summary: Froggius is a lightweight and dumb easy logging libary for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
 License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -23,21 +23,35 @@
   <img src="https://img.shields.io/github/languages/code-size/zlElo/Froggius" alt="GitHub code size in bytes" />
   <img src="https://img.shields.io/github/last-commit/zlElo/Froggius" alt="GitHub last commit" />
   <img src="https://img.shields.io/github/commit-activity/m/zlElo/Froggius" alt="GitHub commit activity month" />
   <img src="https://img.shields.io/github/license/zlElo/Froggius" alt="GitHub license" />
 </p>
 
 # Froggius
-Froggius is a lightweight and dumb easy logging tool for python
+Froggius is a lightweight and dumb easy logging libary for python
 
 ---------
 
 ## Introduction
 Froggius is a lightweight python libary, which is designed for easy to use logging for all your programs. It makes it easy for everybody, but also brings a lot of options to configure it like you need it. An very interesting feature for example is the error catching for functions, which makes it easy to log unexpected errors, warnings etc.
 
+## Advantages of froggius
+Froggius is like in the introduction already said very lightweight and designed for efficiency, which means that the speed of the logging is much faster than other libarys. How fast it is, can you see in this line chart:
+
+<p align="center">
+  <img src="https://github.com/zlElo/Froggius/blob/main/res/tests/froggius_exec.png?raw=true" style="width: 770px">
+</p>
+
+This example runs following debug command 60 times and prints every time the log to the console and stdout:
+```py
+frogger.debug('Example Debug Message')
+```
+
+This massive speed improvement helps your program, to log like you need it without performance disadvantages.
+
 ## Installation
 You can install Froggius with following command:
 ```
 pip install froggius
 ```
 
 Alternatively you can clone this repository and install then:
```

### Comparing `froggius-0.1.6.post2/README.md` & `froggius-0.1.6.post3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,35 @@
   <img src="https://img.shields.io/github/languages/code-size/zlElo/Froggius" alt="GitHub code size in bytes" />
   <img src="https://img.shields.io/github/last-commit/zlElo/Froggius" alt="GitHub last commit" />
   <img src="https://img.shields.io/github/commit-activity/m/zlElo/Froggius" alt="GitHub commit activity month" />
   <img src="https://img.shields.io/github/license/zlElo/Froggius" alt="GitHub license" />
 </p>
 
 # Froggius
-Froggius is a lightweight and dumb easy logging tool for python
+Froggius is a lightweight and dumb easy logging libary for python
 
 ---------
 
 ## Introduction
 Froggius is a lightweight python libary, which is designed for easy to use logging for all your programs. It makes it easy for everybody, but also brings a lot of options to configure it like you need it. An very interesting feature for example is the error catching for functions, which makes it easy to log unexpected errors, warnings etc.
 
+## Advantages of froggius
+Froggius is like in the introduction already said very lightweight and designed for efficiency, which means that the speed of the logging is much faster than other libarys. How fast it is, can you see in this line chart:
+
+<p align="center">
+  <img src="https://github.com/zlElo/Froggius/blob/main/res/tests/froggius_exec.png?raw=true" style="width: 770px">
+</p>
+
+This example runs following debug command 60 times and prints every time the log to the console and stdout:
+```py
+frogger.debug('Example Debug Message')
+```
+
+This massive speed improvement helps your program, to log like you need it without performance disadvantages.
+
 ## Installation
 You can install Froggius with following command:
 ```
 pip install froggius
 ```
 
 Alternatively you can clone this repository and install then:
@@ -139,8 +153,8 @@
 ```py
 # configure print_out and file_path for everything
 logger = Froggius(print_out=False, file_path='tests/example.log')
 
 logger.debug('Test normal', print_out=True) # everything is not printed, but this line is printed
 logger.error('Test error')
 logger.information('Test information')
-```
+```
```

### Comparing `froggius-0.1.6.post2/froggius/logger.py` & `froggius-0.1.6.post3/froggius/logger.py`

 * *Files identical despite different names*

### Comparing `froggius-0.1.6.post2/froggius.egg-info/PKG-INFO` & `froggius-0.1.6.post3/froggius.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.6.post2
-Summary: Froggius is a dumb easy logging tool for python
+Version: 0.1.6.post3
+Summary: Froggius is a lightweight and dumb easy logging libary for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
 License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -23,21 +23,35 @@
   <img src="https://img.shields.io/github/languages/code-size/zlElo/Froggius" alt="GitHub code size in bytes" />
   <img src="https://img.shields.io/github/last-commit/zlElo/Froggius" alt="GitHub last commit" />
   <img src="https://img.shields.io/github/commit-activity/m/zlElo/Froggius" alt="GitHub commit activity month" />
   <img src="https://img.shields.io/github/license/zlElo/Froggius" alt="GitHub license" />
 </p>
 
 # Froggius
-Froggius is a lightweight and dumb easy logging tool for python
+Froggius is a lightweight and dumb easy logging libary for python
 
 ---------
 
 ## Introduction
 Froggius is a lightweight python libary, which is designed for easy to use logging for all your programs. It makes it easy for everybody, but also brings a lot of options to configure it like you need it. An very interesting feature for example is the error catching for functions, which makes it easy to log unexpected errors, warnings etc.
 
+## Advantages of froggius
+Froggius is like in the introduction already said very lightweight and designed for efficiency, which means that the speed of the logging is much faster than other libarys. How fast it is, can you see in this line chart:
+
+<p align="center">
+  <img src="https://github.com/zlElo/Froggius/blob/main/res/tests/froggius_exec.png?raw=true" style="width: 770px">
+</p>
+
+This example runs following debug command 60 times and prints every time the log to the console and stdout:
+```py
+frogger.debug('Example Debug Message')
+```
+
+This massive speed improvement helps your program, to log like you need it without performance disadvantages.
+
 ## Installation
 You can install Froggius with following command:
 ```
 pip install froggius
 ```
 
 Alternatively you can clone this repository and install then:
```

### Comparing `froggius-0.1.6.post2/setup.py` & `froggius-0.1.6.post3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="froggius",
     packages=find_packages(include=["froggius"]),
-    description="Froggius is a dumb easy logging tool for python",
+    description="Froggius is a lightweight and dumb easy logging libary for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MPL-2.0",
-    version="0.1.6-2",
+    version="0.1.6-3",
     author="zlElo",
     author_email="mail@zlelo.de",
     url="https://github.com/zlElo/Froggius",
     keywords=["logging", "logger", "easy-to-use", "log"],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

