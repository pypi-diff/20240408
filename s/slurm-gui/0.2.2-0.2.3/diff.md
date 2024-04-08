# Comparing `tmp/slurm-gui-0.2.2.tar.gz` & `tmp/slurm-gui-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm-gui-0.2.2.tar", last modified: Mon Apr  8 06:10:10 2024, max compression
+gzip compressed data, was "slurm-gui-0.2.3.tar", last modified: Mon Apr  8 06:24:36 2024, max compression
```

## Comparing `slurm-gui-0.2.2.tar` & `slurm-gui-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:10:10.713274 slurm-gui-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 06:10:02.000000 slurm-gui-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 06:10:10.713274 slurm-gui-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 06:10:02.000000 slurm-gui-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:10:10.713274 slurm-gui-0.2.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    23275 2024-04-08 06:10:02.000000 slurm-gui-0.2.2/bin/tsqueue
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 06:10:10.713274 slurm-gui-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-08 06:10:02.000000 slurm-gui-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:10:10.713274 slurm-gui-0.2.2/slurm_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 06:10:10.000000 slurm-gui-0.2.2/slurm_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 06:10:10.000000 slurm-gui-0.2.2/slurm_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:10:10.000000 slurm-gui-0.2.2/slurm_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 06:10:10.000000 slurm-gui-0.2.2/slurm_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:10:10.000000 slurm-gui-0.2.2/slurm_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:24:36.466839 slurm-gui-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 06:24:27.000000 slurm-gui-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 06:24:36.466839 slurm-gui-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 06:24:27.000000 slurm-gui-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:24:36.462839 slurm-gui-0.2.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23275 2024-04-08 06:24:27.000000 slurm-gui-0.2.3/bin/tsqueue
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 06:24:36.466839 slurm-gui-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-08 06:24:27.000000 slurm-gui-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:24:36.466839 slurm-gui-0.2.3/slurm_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 06:24:36.000000 slurm-gui-0.2.3/slurm_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 06:24:36.000000 slurm-gui-0.2.3/slurm_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:24:36.000000 slurm-gui-0.2.3/slurm_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 06:24:36.000000 slurm-gui-0.2.3/slurm_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:24:36.000000 slurm-gui-0.2.3/slurm_gui.egg-info/top_level.txt
```

### Comparing `slurm-gui-0.2.2/LICENSE` & `slurm-gui-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-gui-0.2.2/PKG-INFO` & `slurm-gui-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-gui
-Version: 0.2.2
+Version: 0.2.3
 Summary: GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework
 Home-page: https://github.com/dirkpetersen/slurm-gui
 Author: Dirk Petersen
 Author-email: no-email@no-domain.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `slurm-gui-0.2.2/README.md` & `slurm-gui-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `slurm-gui-0.2.2/bin/tsqueue` & `slurm-gui-0.2.3/bin/tsqueue`

 * *Files identical despite different names*

### Comparing `slurm-gui-0.2.2/setup.py` & `slurm-gui-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,19 @@
         # If there is no tag reference, fallback to a default version
         return "0.0.0"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 def read_requirements():
+    print('os.listdir():', os.listdir())
     requirements_path = os.path.join(currdir, 'requirements.txt')
     if not os.path.exists(requirements_path):
         print(f'Could not find {requirements_path}')
-        return ['textual<0.60']
+        return ['textual']
     with open(requirements_path, 'r', encoding="utf-8") as file:
         return file.read().splitlines()
 
 setup(
     name="slurm-gui",
     version=get_version(),
     author="Dirk Petersen",
```

### Comparing `slurm-gui-0.2.2/slurm_gui.egg-info/PKG-INFO` & `slurm-gui-0.2.3/slurm_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-gui
-Version: 0.2.2
+Version: 0.2.3
 Summary: GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework
 Home-page: https://github.com/dirkpetersen/slurm-gui
 Author: Dirk Petersen
 Author-email: no-email@no-domain.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

