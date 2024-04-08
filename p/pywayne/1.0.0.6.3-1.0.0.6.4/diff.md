# Comparing `tmp/pywayne-1.0.0.6.3.tar.gz` & `tmp/pywayne-1.0.0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywayne-1.0.0.6.3.tar", last modified: Fri Mar 29 07:14:33 2024, max compression
+gzip compressed data, was "pywayne-1.0.0.6.4.tar", last modified: Mon Apr  8 10:17:58 2024, max compression
```

## Comparing `pywayne-1.0.0.6.3.tar` & `pywayne-1.0.0.6.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-03-29 07:14:33.564978 pywayne-1.0.0.6.3/
--rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.3/LICENSE
--rw-r--r--   0 wayne      (503) staff       (20)     1023 2024-03-29 07:14:33.564838 pywayne-1.0.0.6.3/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.3/README.md
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-03-29 07:14:33.558438 pywayne-1.0.0.6.3/bin/
--rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.6.3/bin/gettool
--rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.6.3/bin/gettool.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-03-29 07:14:33.560639 pywayne-1.0.0.6.3/pywayne/
--rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.3/pywayne/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)      242 2024-03-29 07:13:41.000000 pywayne-1.0.0.6.3/pywayne/__version__.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-03-29 07:14:33.561708 pywayne-1.0.0.6.3/pywayne/adb/
--rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.3/pywayne/adb/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.3/pywayne/adb/logcat_reader.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-03-29 07:14:33.562805 pywayne-1.0.0.6.3/pywayne/ahrs/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.3/pywayne/ahrs/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.3/pywayne/ahrs/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-03-29 07:14:33.563464 pywayne-1.0.0.6.3/pywayne/calibration/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.3/pywayne/calibration/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.6.3/pywayne/calibration/magnetometer_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.6.3/pywayne/calibration/temporal_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.3/pywayne/data_structure.py
--rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.6.3/pywayne/dsp.py
--rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.6.3/pywayne/gui.py
--rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.3/pywayne/math.py
--rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.3/pywayne/plot.py
--rw-r--r--   0 wayne      (503) staff       (20)    12992 2024-03-29 07:14:11.000000 pywayne-1.0.0.6.3/pywayne/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-03-29 07:14:33.564002 pywayne-1.0.0.6.3/pywayne/vio/
--rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.3/pywayne/vio/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.3/pywayne/vio/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-03-29 07:14:33.564518 pywayne-1.0.0.6.3/pywayne/visualization/
--rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.6.3/pywayne/visualization/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.6.3/pywayne/visualization/pangolin.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-03-29 07:14:33.561334 pywayne-1.0.0.6.3/pywayne.egg-info/
--rw-r--r--   0 wayne      (503) staff       (20)     1023 2024-03-29 07:14:33.000000 pywayne-1.0.0.6.3/pywayne.egg-info/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      692 2024-03-29 07:14:33.000000 pywayne-1.0.0.6.3/pywayne.egg-info/SOURCES.txt
--rw-r--r--   0 wayne      (503) staff       (20)      184 2024-03-29 07:14:33.000000 pywayne-1.0.0.6.3/pywayne.egg-info/dependency_links.txt
--rw-r--r--   0 wayne      (503) staff       (20)      148 2024-03-29 07:14:33.000000 pywayne-1.0.0.6.3/pywayne.egg-info/requires.txt
--rw-r--r--   0 wayne      (503) staff       (20)        8 2024-03-29 07:14:33.000000 pywayne-1.0.0.6.3/pywayne.egg-info/top_level.txt
--rw-r--r--   0 wayne      (503) staff       (20)       38 2024-03-29 07:14:33.565028 pywayne-1.0.0.6.3/setup.cfg
--rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.6.3/setup.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.264108 pywayne-1.0.0.6.4/
+-rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/LICENSE
+-rw-r--r--   0 wayne      (503) staff       (20)     1023 2024-04-08 10:17:58.263984 pywayne-1.0.0.6.4/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/README.md
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.258602 pywayne-1.0.0.6.4/bin/
+-rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.6.4/bin/gettool
+-rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.6.4/bin/gettool.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.260578 pywayne-1.0.0.6.4/pywayne/
+-rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)      242 2024-04-08 10:16:51.000000 pywayne-1.0.0.6.4/pywayne/__version__.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.261608 pywayne-1.0.0.6.4/pywayne/adb/
+-rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.4/pywayne/adb/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.4/pywayne/adb/logcat_reader.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.262125 pywayne-1.0.0.6.4/pywayne/ahrs/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/ahrs/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/ahrs/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.262741 pywayne-1.0.0.6.4/pywayne/calibration/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/calibration/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.6.4/pywayne/calibration/magnetometer_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.6.4/pywayne/calibration/temporal_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/data_structure.py
+-rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.6.4/pywayne/dsp.py
+-rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.6.4/pywayne/gui.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/math.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/plot.py
+-rw-r--r--   0 wayne      (503) staff       (20)    13551 2024-04-08 10:16:51.000000 pywayne-1.0.0.6.4/pywayne/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.263229 pywayne-1.0.0.6.4/pywayne/vio/
+-rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.4/pywayne/vio/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.4/pywayne/vio/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.263684 pywayne-1.0.0.6.4/pywayne/visualization/
+-rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.6.4/pywayne/visualization/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.6.4/pywayne/visualization/pangolin.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.261254 pywayne-1.0.0.6.4/pywayne.egg-info/
+-rw-r--r--   0 wayne      (503) staff       (20)     1023 2024-04-08 10:17:58.000000 pywayne-1.0.0.6.4/pywayne.egg-info/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      692 2024-04-08 10:17:58.000000 pywayne-1.0.0.6.4/pywayne.egg-info/SOURCES.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      184 2024-04-08 10:17:58.000000 pywayne-1.0.0.6.4/pywayne.egg-info/dependency_links.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      148 2024-04-08 10:17:58.000000 pywayne-1.0.0.6.4/pywayne.egg-info/requires.txt
+-rw-r--r--   0 wayne      (503) staff       (20)        8 2024-04-08 10:17:58.000000 pywayne-1.0.0.6.4/pywayne.egg-info/top_level.txt
+-rw-r--r--   0 wayne      (503) staff       (20)       38 2024-04-08 10:17:58.264156 pywayne-1.0.0.6.4/setup.cfg
+-rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.6.4/setup.py
```

### Comparing `pywayne-1.0.0.6.3/LICENSE` & `pywayne-1.0.0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/PKG-INFO` & `pywayne-1.0.0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.6.3
+Version: 1.0.0.6.4
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.6.3/README.md` & `pywayne-1.0.0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/bin/gettool.py` & `pywayne-1.0.0.6.4/bin/gettool.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/pywayne/adb/logcat_reader.py` & `pywayne-1.0.0.6.4/pywayne/adb/logcat_reader.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/pywayne/ahrs/tools.py` & `pywayne-1.0.0.6.4/pywayne/ahrs/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/pywayne/calibration/magnetometer_calibration.py` & `pywayne-1.0.0.6.4/pywayne/calibration/magnetometer_calibration.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/pywayne/data_structure.py` & `pywayne-1.0.0.6.4/pywayne/data_structure.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/pywayne/dsp.py` & `pywayne-1.0.0.6.4/pywayne/dsp.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/pywayne/gui.py` & `pywayne-1.0.0.6.4/pywayne/gui.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/pywayne/math.py` & `pywayne-1.0.0.6.4/pywayne/math.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/pywayne/plot.py` & `pywayne-1.0.0.6.4/pywayne/plot.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/pywayne/tools.py` & `pywayne-1.0.0.6.4/pywayne/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,15 +76,27 @@
     :param func:
     :return:
     """
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         ret = func(*args, **kwargs)
-        plt.get_current_fig_manager().window.showMaximized()
+        backend = plt.get_backend()
+        mgr = plt.get_current_fig_manager()
+
+        if backend.lower() == 'tkagg':
+            mgr.window.state('zoomed')  # TkAgg backend
+        elif backend.lower() == 'wxagg':
+            mgr.frame.Maximize(True)  # wxAgg backend
+        elif backend.lower() == 'qt4agg' or backend.lower() == 'qt5agg':
+            mgr.window.showMaximized()  # Qt4Agg and Qt5Agg backend
+        elif backend.lower() in ['gtk3agg', 'gtk3cairo']:
+            mgr.window.maximize()  # GTK3 backends
+        else:
+            print(f"Warning: '{backend}' backend does not support maximize_figure.")
         return ret
 
     return wrapper
 
 
 def singleton(cls):
     """
```

### Comparing `pywayne-1.0.0.6.3/pywayne/vio/tools.py` & `pywayne-1.0.0.6.4/pywayne/vio/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/pywayne/visualization/pangolin.py` & `pywayne-1.0.0.6.4/pywayne/visualization/pangolin.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/pywayne.egg-info/PKG-INFO` & `pywayne-1.0.0.6.4/pywayne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.6.3
+Version: 1.0.0.6.4
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.6.3/pywayne.egg-info/SOURCES.txt` & `pywayne-1.0.0.6.4/pywayne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.3/setup.py` & `pywayne-1.0.0.6.4/setup.py`

 * *Files identical despite different names*

