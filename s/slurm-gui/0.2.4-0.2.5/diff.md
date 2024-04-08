# Comparing `tmp/slurm-gui-0.2.4.tar.gz` & `tmp/slurm-gui-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm-gui-0.2.4.tar", last modified: Mon Apr  8 07:41:53 2024, max compression
+gzip compressed data, was "slurm-gui-0.2.5.tar", last modified: Mon Apr  8 07:44:02 2024, max compression
```

## Comparing `slurm-gui-0.2.4.tar` & `slurm-gui-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:41:53.781117 slurm-gui-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 07:41:49.000000 slurm-gui-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 07:41:53.781117 slurm-gui-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 07:41:49.000000 slurm-gui-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:41:53.781117 slurm-gui-0.2.4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    23275 2024-04-08 07:41:49.000000 slurm-gui-0.2.4/bin/tsqueue
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 07:41:53.781117 slurm-gui-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-08 07:41:49.000000 slurm-gui-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:41:53.781117 slurm-gui-0.2.4/slurm_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 07:41:53.000000 slurm-gui-0.2.4/slurm_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 07:41:53.000000 slurm-gui-0.2.4/slurm_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:41:53.000000 slurm-gui-0.2.4/slurm_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 07:41:53.000000 slurm-gui-0.2.4/slurm_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:41:53.000000 slurm-gui-0.2.4/slurm_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:44:02.127151 slurm-gui-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 07:43:57.000000 slurm-gui-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 07:44:02.127151 slurm-gui-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 07:43:57.000000 slurm-gui-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:44:02.127151 slurm-gui-0.2.5/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23275 2024-04-08 07:43:57.000000 slurm-gui-0.2.5/bin/tsqueue
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 07:44:02.127151 slurm-gui-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-08 07:43:57.000000 slurm-gui-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:44:02.127151 slurm-gui-0.2.5/slurm_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 07:44:02.000000 slurm-gui-0.2.5/slurm_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 07:44:02.000000 slurm-gui-0.2.5/slurm_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:44:02.000000 slurm-gui-0.2.5/slurm_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 07:44:02.000000 slurm-gui-0.2.5/slurm_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:44:02.000000 slurm-gui-0.2.5/slurm_gui.egg-info/top_level.txt
```

### Comparing `slurm-gui-0.2.4/LICENSE` & `slurm-gui-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-gui-0.2.4/PKG-INFO` & `slurm-gui-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-gui
-Version: 0.2.4
+Version: 0.2.5
 Summary: GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework
 Home-page: https://github.com/dirkpetersen/slurm-gui
 Author: Dirk Petersen
 Author-email: no-email@no-domain.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `slurm-gui-0.2.4/README.md` & `slurm-gui-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `slurm-gui-0.2.4/bin/tsqueue` & `slurm-gui-0.2.5/bin/tsqueue`

 * *Files identical despite different names*

### Comparing `slurm-gui-0.2.4/setup.py` & `slurm-gui-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 def read_requirements():
     print('os.listdir():', os.listdir())
     for root, dirs, files in os.walk("."):
         file_path = ''
         if "requirements.txt" in files:
             file_path = os.path.join(root, "requirements.txt")
         elif "requires.txt" in files:
-            file_path = os.path.join(root, "requires.txt")
-        print('requirements.txt:', file_path)
+            file_path = os.path.join(root, "requires.txt")        
         if file_path:
+            print('requirements.txt:', file_path)
             with open(file_path, 'r') as file:
                 return file.read().splitlines()
     return []
 
 setuptools.setup(
     name=pkgname,
     version=get_version(),
```

### Comparing `slurm-gui-0.2.4/slurm_gui.egg-info/PKG-INFO` & `slurm-gui-0.2.5/slurm_gui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-gui
-Version: 0.2.4
+Version: 0.2.5
 Summary: GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework
 Home-page: https://github.com/dirkpetersen/slurm-gui
 Author: Dirk Petersen
 Author-email: no-email@no-domain.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

