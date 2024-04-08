# Comparing `tmp/pnostic-0.8.8.tar.gz` & `tmp/pnostic-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnostic-0.8.8.tar", last modified: Mon Nov 20 19:03:01 2023, max compression
+gzip compressed data, was "pnostic-0.8.9.tar", last modified: Mon Nov 20 19:38:12 2023, max compression
```

## Comparing `pnostic-0.8.8.tar` & `pnostic-0.8.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:03:01.168587 pnostic-0.8.8/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1074 2023-11-20 19:02:52.000000 pnostic-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-11-20 19:03:01.168587 pnostic-0.8.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)      121 2023-11-20 19:02:52.000000 pnostic-0.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:03:01.168587 pnostic-0.8.8/pnostic/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:03:01.168587 pnostic-0.8.8/pnostic/envelopers/
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/envelopers/LiveGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/envelopers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:03:01.168587 pnostic-0.8.8/pnostic/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/loggers/Printr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/loggers/RawSave.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/loggers/ToCSV.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/loggers/ToCSVCompressed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/loggers/ToJSON.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/loggers/ToJSONL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/loggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:03:01.168587 pnostic-0.8.8/pnostic/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/providers/SingleFile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:03:01.168587 pnostic-0.8.8/pnostic/runners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/runners/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:03:01.168587 pnostic-0.8.8/pnostic/seclusion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/seclusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/seclusion/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/seclusion/titan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37271 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2023-11-20 19:02:52.000000 pnostic-0.8.8/pnostic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:03:01.168587 pnostic-0.8.8/pnostic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-11-20 19:03:01.000000 pnostic-0.8.8/pnostic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-11-20 19:03:01.000000 pnostic-0.8.8/pnostic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 19:03:01.000000 pnostic-0.8.8/pnostic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-20 19:03:01.000000 pnostic-0.8.8/pnostic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-20 19:03:01.000000 pnostic-0.8.8/pnostic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 19:03:01.172587 pnostic-0.8.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3463 2023-11-20 19:02:52.000000 pnostic-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:12.808532 pnostic-0.8.9/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1074 2023-11-20 19:38:04.000000 pnostic-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2023-11-20 19:38:12.808532 pnostic-0.8.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)      121 2023-11-20 19:38:04.000000 pnostic-0.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:12.804532 pnostic-0.8.9/pnostic/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:12.804532 pnostic-0.8.9/pnostic/envelopers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/envelopers/LiveGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/envelopers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:12.804532 pnostic-0.8.9/pnostic/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/loggers/Printr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/loggers/RawSave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/loggers/ToCSV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/loggers/ToCSVCompressed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/loggers/ToJSON.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/loggers/ToJSONL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/loggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:12.804532 pnostic-0.8.9/pnostic/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/providers/SingleFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:12.804532 pnostic-0.8.9/pnostic/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/runners/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:12.808532 pnostic-0.8.9/pnostic/seclusion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/seclusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/seclusion/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/seclusion/titan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37279 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2023-11-20 19:38:04.000000 pnostic-0.8.9/pnostic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:38:12.804532 pnostic-0.8.9/pnostic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2023-11-20 19:38:12.000000 pnostic-0.8.9/pnostic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2023-11-20 19:38:12.000000 pnostic-0.8.9/pnostic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 19:38:12.000000 pnostic-0.8.9/pnostic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-20 19:38:12.000000 pnostic-0.8.9/pnostic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-20 19:38:12.000000 pnostic-0.8.9/pnostic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 19:38:12.808532 pnostic-0.8.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3463 2023-11-20 19:38:04.000000 pnostic-0.8.9/setup.py
```

### Comparing `pnostic-0.8.8/LICENSE` & `pnostic-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/PKG-INFO` & `pnostic-0.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnostic
-Version: 0.8.8
+Version: 0.8.9
 Summary: My short description for my project.
 Home-page: https://github.com/franceme/pnostic
 Author: Miles Frantz
 Author-email: frantzme@vt.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pnostic-0.8.8/pnostic/envelopers/LiveGraph.py` & `pnostic-0.8.9/pnostic/envelopers/LiveGraph.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic/loggers/Printr.py` & `pnostic-0.8.9/pnostic/loggers/Printr.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic/loggers/RawSave.py` & `pnostic-0.8.9/pnostic/loggers/RawSave.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic/loggers/ToCSV.py` & `pnostic-0.8.9/pnostic/loggers/ToCSV.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic/loggers/ToCSVCompressed.py` & `pnostic-0.8.9/pnostic/loggers/ToCSVCompressed.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic/loggers/ToJSON.py` & `pnostic-0.8.9/pnostic/loggers/ToJSON.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic/loggers/ToJSONL.py` & `pnostic-0.8.9/pnostic/loggers/ToJSONL.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic/providers/SingleFile.py` & `pnostic-0.8.9/pnostic/providers/SingleFile.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic/runners/simple.py` & `pnostic-0.8.9/pnostic/runners/simple.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic/seclusion/core.py` & `pnostic-0.8.9/pnostic/seclusion/core.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic/seclusion/titan.py` & `pnostic-0.8.9/pnostic/seclusion/titan.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic/structure.py` & `pnostic-0.8.9/pnostic/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -978,15 +978,15 @@
                 except Exception as e:
                     _,_, exc_tb = sys.exc_info();fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
                     msg = ":> Hit an unexpected error {0} @ {1}:{2}".format(e, fname, exc_tb.tb_lineno)
                     self.loggerSet.emergency(msg)
                     logy.send(msg)
 
 
-                execution_output = self.seclusion_env(obj, runner)
+                execution_output = self.seclusion_env.process(obj, runner)
                 startTime=execution_output.start_date_time
                 endTime=execution_output.end_date_time
                 output =execution_output.result
 
                 logy.send("␁ Finished Scanning {0} {1}".format(obj.str_type(), obj.path))
                 if endTime is None:
                     endTime = startTime
```

### Comparing `pnostic-0.8.8/pnostic/utils.py` & `pnostic-0.8.9/pnostic/utils.py`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/pnostic.egg-info/PKG-INFO` & `pnostic-0.8.9/pnostic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnostic
-Version: 0.8.8
+Version: 0.8.9
 Summary: My short description for my project.
 Home-page: https://github.com/franceme/pnostic
 Author: Miles Frantz
 Author-email: frantzme@vt.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pnostic-0.8.8/pnostic.egg-info/SOURCES.txt` & `pnostic-0.8.9/pnostic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pnostic-0.8.8/setup.py` & `pnostic-0.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.8.8"
+VERSION = "0.8.9"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

