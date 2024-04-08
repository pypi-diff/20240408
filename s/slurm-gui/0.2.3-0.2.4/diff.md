# Comparing `tmp/slurm-gui-0.2.3.tar.gz` & `tmp/slurm-gui-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm-gui-0.2.3.tar", last modified: Mon Apr  8 06:24:36 2024, max compression
+gzip compressed data, was "slurm-gui-0.2.4.tar", last modified: Mon Apr  8 07:41:53 2024, max compression
```

## Comparing `slurm-gui-0.2.3.tar` & `slurm-gui-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:24:36.466839 slurm-gui-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 06:24:27.000000 slurm-gui-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 06:24:36.466839 slurm-gui-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 06:24:27.000000 slurm-gui-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:24:36.462839 slurm-gui-0.2.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    23275 2024-04-08 06:24:27.000000 slurm-gui-0.2.3/bin/tsqueue
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 06:24:36.466839 slurm-gui-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-08 06:24:27.000000 slurm-gui-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:24:36.466839 slurm-gui-0.2.3/slurm_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 06:24:36.000000 slurm-gui-0.2.3/slurm_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 06:24:36.000000 slurm-gui-0.2.3/slurm_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:24:36.000000 slurm-gui-0.2.3/slurm_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 06:24:36.000000 slurm-gui-0.2.3/slurm_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:24:36.000000 slurm-gui-0.2.3/slurm_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:41:53.781117 slurm-gui-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 07:41:49.000000 slurm-gui-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 07:41:53.781117 slurm-gui-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 07:41:49.000000 slurm-gui-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:41:53.781117 slurm-gui-0.2.4/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23275 2024-04-08 07:41:49.000000 slurm-gui-0.2.4/bin/tsqueue
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 07:41:53.781117 slurm-gui-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-08 07:41:49.000000 slurm-gui-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:41:53.781117 slurm-gui-0.2.4/slurm_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 07:41:53.000000 slurm-gui-0.2.4/slurm_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 07:41:53.000000 slurm-gui-0.2.4/slurm_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:41:53.000000 slurm-gui-0.2.4/slurm_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 07:41:53.000000 slurm-gui-0.2.4/slurm_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:41:53.000000 slurm-gui-0.2.4/slurm_gui.egg-info/top_level.txt
```

### Comparing `slurm-gui-0.2.3/LICENSE` & `slurm-gui-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-gui-0.2.3/PKG-INFO` & `slurm-gui-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: slurm-gui
-Version: 0.2.3
+Version: 0.2.4
 Summary: GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework
 Home-page: https://github.com/dirkpetersen/slurm-gui
 Author: Dirk Petersen
 Author-email: no-email@no-domain.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: textual<0.60
+Requires-Dist: textual<0.60,>=0.50
 
 # Slurm made easy with slurm-gui ! 
 
 **GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework**
 
 ![PyPI](https://img.shields.io/pypi/v/slurm-gui)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/slurm-gui)
```

### Comparing `slurm-gui-0.2.3/README.md` & `slurm-gui-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `slurm-gui-0.2.3/bin/tsqueue` & `slurm-gui-0.2.4/bin/tsqueue`

 * *Files identical despite different names*

### Comparing `slurm-gui-0.2.3/setup.py` & `slurm-gui-0.2.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-import os, subprocess
-from setuptools import setup, find_packages
+import os, setuptools
 
-currdir = os.path.dirname(__file__)
+pkgname = 'slurm-gui'
+appdesc = "GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework"
+gitrepos = 'dirkpetersen/slurm-gui'
+pyreq = '>=3.8'
+myscripts = ['bin/tsqueue']
 
 def get_version():
     github_ref = os.getenv("GITHUB_REF")
     if github_ref and github_ref.startswith("refs/tags/"):
         # Extract the tag name from the reference
         tag = github_ref.split("/")[-1]
         # Remove the "v" prefix if present
@@ -16,33 +19,38 @@
         return "0.0.0"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 def read_requirements():
     print('os.listdir():', os.listdir())
-    requirements_path = os.path.join(currdir, 'requirements.txt')
-    if not os.path.exists(requirements_path):
-        print(f'Could not find {requirements_path}')
-        return ['textual']
-    with open(requirements_path, 'r', encoding="utf-8") as file:
-        return file.read().splitlines()
+    for root, dirs, files in os.walk("."):
+        file_path = ''
+        if "requirements.txt" in files:
+            file_path = os.path.join(root, "requirements.txt")
+        elif "requires.txt" in files:
+            file_path = os.path.join(root, "requires.txt")
+        print('requirements.txt:', file_path)
+        if file_path:
+            with open(file_path, 'r') as file:
+                return file.read().splitlines()
+    return []
 
-setup(
-    name="slurm-gui",
+setuptools.setup(
+    name=pkgname,
     version=get_version(),
     author="Dirk Petersen",
     author_email="no-email@no-domain.com",
-    description="GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework",
+    description=appdesc,
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/dirkpetersen/slurm-gui",
-    packages=find_packages(),
+    url=f"https://github.com/{gitrepos}",
+    packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.8',
+    python_requires=pyreq,
     install_requires=read_requirements(),
-    scripts=['bin/tsqueue'],
+    scripts=myscripts,
 )
```

### Comparing `slurm-gui-0.2.3/slurm_gui.egg-info/PKG-INFO` & `slurm-gui-0.2.4/slurm_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: slurm-gui
-Version: 0.2.3
+Version: 0.2.4
 Summary: GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework
 Home-page: https://github.com/dirkpetersen/slurm-gui
 Author: Dirk Petersen
 Author-email: no-email@no-domain.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: textual<0.60
+Requires-Dist: textual<0.60,>=0.50
 
 # Slurm made easy with slurm-gui ! 
 
 **GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework**
 
 ![PyPI](https://img.shields.io/pypi/v/slurm-gui)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/slurm-gui)
```

