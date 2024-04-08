# Comparing `tmp/plus_slurm-0.2.1.tar.gz` & `tmp/plus_slurm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plus_slurm-0.2.1.tar", last modified: Fri May  5 12:41:19 2023, max compression
+gzip compressed data, was "plus_slurm-0.2.2.tar", last modified: Mon Apr  8 14:16:00 2024, max compression
```

## Comparing `plus_slurm-0.2.1.tar` & `plus_slurm-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-05 12:41:19.877760 plus_slurm-0.2.1/
--rw-r--r--   0 th        (1011) th        (1011)    35078 2022-08-08 13:55:25.000000 plus_slurm-0.2.1/LICENSE
--rw-r--r--   0 th        (1011) th        (1011)       97 2022-08-08 13:47:18.000000 plus_slurm-0.2.1/MANIFEST.in
--rw-r--r--   0 th        (1011) th        (1011)     1035 2023-05-05 12:41:19.877760 plus_slurm-0.2.1/PKG-INFO
--rw-r--r--   0 th        (1011) th        (1011)      407 2022-08-24 09:22:58.000000 plus_slurm-0.2.1/README.md
--rw-r--r--   0 th        (1011) th        (1011)        5 2023-05-05 12:38:10.000000 plus_slurm-0.2.1/VERSION
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-05 12:41:19.872760 plus_slurm-0.2.1/plus_slurm/
--rw-r--r--   0 th        (1011) th        (1011)      949 2023-05-05 12:37:55.000000 plus_slurm-0.2.1/plus_slurm/__init__.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-05 12:41:19.877760 plus_slurm-0.2.1/plus_slurm/jinja2_templates/
--rw-r--r--   0 th        (1011) th        (1011)     3040 2023-04-27 11:56:08.000000 plus_slurm-0.2.1/plus_slurm/jinja2_templates/runner.py
--rw-r--r--   0 th        (1011) th        (1011)      395 2023-01-09 12:10:38.000000 plus_slurm-0.2.1/plus_slurm/jinja2_templates/submit.sh
--rw-r--r--   0 th        (1011) th        (1011)     8429 2022-08-24 12:16:21.000000 plus_slurm-0.2.1/plus_slurm/job.py
--rw-r--r--   0 th        (1011) th        (1011)    16755 2023-05-05 12:37:55.000000 plus_slurm-0.2.1/plus_slurm/jobcluster.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-05 12:41:19.876760 plus_slurm-0.2.1/plus_slurm.egg-info/
--rw-r--r--   0 th        (1011) th        (1011)     1035 2023-05-05 12:41:19.000000 plus_slurm-0.2.1/plus_slurm.egg-info/PKG-INFO
--rw-r--r--   0 th        (1011) th        (1011)      357 2023-05-05 12:41:19.000000 plus_slurm-0.2.1/plus_slurm.egg-info/SOURCES.txt
--rw-r--r--   0 th        (1011) th        (1011)        1 2023-05-05 12:41:19.000000 plus_slurm-0.2.1/plus_slurm.egg-info/dependency_links.txt
--rw-r--r--   0 th        (1011) th        (1011)       45 2023-05-05 12:41:19.000000 plus_slurm-0.2.1/plus_slurm.egg-info/requires.txt
--rw-r--r--   0 th        (1011) th        (1011)       11 2023-05-05 12:41:19.000000 plus_slurm-0.2.1/plus_slurm.egg-info/top_level.txt
--rw-r--r--   0 th        (1011) th        (1011)       38 2023-05-05 12:41:19.877760 plus_slurm-0.2.1/setup.cfg
--rw-r--r--   0 th        (1011) th        (1011)     1426 2022-08-25 14:01:46.000000 plus_slurm-0.2.1/setup.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-08 14:16:00.266187 plus_slurm-0.2.2/
+-rw-r--r--   0 th        (1011) th        (1011)    35078 2022-08-08 13:55:25.000000 plus_slurm-0.2.2/LICENSE
+-rw-r--r--   0 th        (1011) th        (1011)       97 2022-08-08 13:47:18.000000 plus_slurm-0.2.2/MANIFEST.in
+-rw-r--r--   0 th        (1011) th        (1011)     1170 2024-04-08 14:16:00.265187 plus_slurm-0.2.2/PKG-INFO
+-rw-r--r--   0 th        (1011) th        (1011)      407 2022-08-24 09:22:58.000000 plus_slurm-0.2.2/README.md
+-rw-r--r--   0 th        (1011) th        (1011)        5 2024-04-08 14:15:44.000000 plus_slurm-0.2.2/VERSION
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-08 14:16:00.263187 plus_slurm-0.2.2/plus_slurm/
+-rw-r--r--   0 th        (1011) th        (1011)      949 2023-05-05 12:37:55.000000 plus_slurm-0.2.2/plus_slurm/__init__.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-08 14:16:00.264187 plus_slurm-0.2.2/plus_slurm/jinja2_templates/
+-rw-r--r--   0 th        (1011) th        (1011)     3040 2023-04-27 11:56:08.000000 plus_slurm-0.2.2/plus_slurm/jinja2_templates/runner.py
+-rw-r--r--   0 th        (1011) th        (1011)      521 2024-04-08 14:15:25.000000 plus_slurm-0.2.2/plus_slurm/jinja2_templates/submit.sh
+-rw-r--r--   0 th        (1011) th        (1011)     8429 2022-08-24 12:16:21.000000 plus_slurm-0.2.2/plus_slurm/job.py
+-rw-r--r--   0 th        (1011) th        (1011)    17289 2024-04-08 14:15:25.000000 plus_slurm-0.2.2/plus_slurm/jobcluster.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-08 14:16:00.263187 plus_slurm-0.2.2/plus_slurm.egg-info/
+-rw-r--r--   0 th        (1011) th        (1011)     1170 2024-04-08 14:16:00.000000 plus_slurm-0.2.2/plus_slurm.egg-info/PKG-INFO
+-rw-r--r--   0 th        (1011) th        (1011)      408 2024-04-08 14:16:00.000000 plus_slurm-0.2.2/plus_slurm.egg-info/SOURCES.txt
+-rw-r--r--   0 th        (1011) th        (1011)        1 2024-04-08 14:16:00.000000 plus_slurm-0.2.2/plus_slurm.egg-info/dependency_links.txt
+-rw-r--r--   0 th        (1011) th        (1011)       45 2024-04-08 14:16:00.000000 plus_slurm-0.2.2/plus_slurm.egg-info/requires.txt
+-rw-r--r--   0 th        (1011) th        (1011)       11 2024-04-08 14:16:00.000000 plus_slurm-0.2.2/plus_slurm.egg-info/top_level.txt
+-rw-r--r--   0 th        (1011) th        (1011)       38 2024-04-08 14:16:00.266187 plus_slurm-0.2.2/setup.cfg
+-rw-r--r--   0 th        (1011) th        (1011)     1426 2022-08-25 14:01:46.000000 plus_slurm-0.2.2/setup.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-08 14:16:00.265187 plus_slurm-0.2.2/tests/
+-rw-r--r--   0 th        (1011) th        (1011)     1392 2023-04-27 11:52:36.000000 plus_slurm-0.2.2/tests/test_nested_jobs.py
+-rw-r--r--   0 th        (1011) th        (1011)     8453 2024-04-08 14:15:25.000000 plus_slurm-0.2.2/tests/test_plus_slurm.py
```

### Comparing `plus_slurm-0.2.1/LICENSE` & `plus_slurm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.2.1/PKG-INFO` & `plus_slurm-0.2.2/plus_slurm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
-Name: plus_slurm
-Version: 0.2.1
+Name: plus-slurm
+Version: 0.2.2
 Summary: Convenient Python Abstraction for the Slurm based cluster at the PLUS
 Home-page: https://gitlab.com/thht/plus-slurm
 Author: Thomas Hartmann
 Author-email: thomas.hartmann@th-ht.de
 License: GPL3
 Keywords: Slurm
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jinja2
+Requires-Dist: future
+Requires-Dist: humanfriendly
+Requires-Dist: six
+Requires-Dist: numpy
+Requires-Dist: psutil
 
 # plus_slurm
 A python module to make it simple to submit jobs to the Slurm based cluster directly from python
 
 ## Documentation
 https://plus-slurm.readthedocs.io
```

### Comparing `plus_slurm-0.2.1/plus_slurm/__init__.py` & `plus_slurm-0.2.2/plus_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.2.1/plus_slurm/jinja2_templates/runner.py` & `plus_slurm-0.2.2/plus_slurm/jinja2_templates/runner.py`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.2.1/plus_slurm/job.py` & `plus_slurm-0.2.2/plus_slurm/job.py`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.2.1/plus_slurm/jobcluster.py` & `plus_slurm-0.2.2/plus_slurm/jobcluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     Parameters
     ----------
     required_ram : :class:`str`, :class:`float`, :class:`int`, optional
         The amount of RAM required to run one Job in megabytes. A string like
         "2G" or "200M" will be converted accordingly.
     request_cpus : :class:`int`, optional
         The number of CPUs requested
+    qos : :class:`str`, optional
+        The quality of service to use.
     request_time : :class:`int`, optional
         Maximum duration of a job in minutes.
     jobs_dir ::class:`str`, optional
         Folder to put all the jobs in. This one needs to be on the shared
         filesystem (so somewhere under /mnt/obob)
     inc_jobsdir ::class:`str`, optional
         If this is set to True (default), jobs_dir is the parent folder for all
@@ -80,37 +82,46 @@
     max_jobs_per_jobcluster : :class:`int`, optional
         Slurm only allows a certain number of jobs per array job
         (1000 by default).
         If the number of jobs to be submitted is higher that this number, jobs
         will be split in more than one array job.
     append_to_path : :class:`str`, optional
         Path to append to the python module search path.
+    extra_slurm_args : class:`list`, optional
+        Extra arguments for slurm sbatch. These get appended as is with
+        the `#SBATCH` prefix.
     """
 
     _slurm_submit = '/usr/bin/sbatch'
     _runner_template = 'runner.py'
     _submit_template = 'submit.sh'
 
     def __init__(self, required_ram='2G', request_cpus=1, jobs_dir='jobs',
                  request_time=10,
                  inc_jobsdir=True,
+                 qos=None,
                  python_bin=None, working_directory=None,
                  exclude_nodes=None, max_jobs_per_jobcluster=1000,
-                 append_to_path=None):
+                 append_to_path=None,
+                 extra_slurm_args=None):
         self.required_ram = required_ram
         self.request_time = request_time
         self.request_cpus = request_cpus
         self.jobs_dir = jobs_dir
         self.inc_jobsdir = inc_jobsdir
         self.python_bin = python_bin
         self.working_directory = working_directory
         self._output_folder = None
         self._exclude_nodes = exclude_nodes
         self._max_jobs_per_jobcluster = max_jobs_per_jobcluster
         self._append_to_path = append_to_path
+        self._qos = qos
+        self._extra_slurm_args = extra_slurm_args
+        if self._extra_slurm_args is None:
+            self._extra_slurm_args = list()
 
         self._jobs = list()
 
         self._jinja_env = jinja2.Environment(
             loader=jinja2.PackageLoader('plus_slurm', 'jinja2_templates'),
             trim_blocks=True,
             lstrip_blocks=True
@@ -251,15 +262,17 @@
             'request_cpus': self.request_cpus,
             'request_time': self.request_time,
             'uuid': str(uuid.uuid4()),
             'python_home': self.python_home,
             'n_jobs': len(self._current_jobs_submitting),
             'working_directory': self.working_directory,
             'exclude_nodes': self._exclude_nodes,
-            'append_to_path': self._append_to_path
+            'append_to_path': self._append_to_path,
+            'qos': self._qos,
+            'extra_slurm_args': self._extra_slurm_args
         }
 
     @property
     def jobs_submitted(self):
         return tuple(self._jobs_submitted)
 
     @property
```

### Comparing `plus_slurm-0.2.1/plus_slurm.egg-info/PKG-INFO` & `plus_slurm-0.2.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
-Name: plus-slurm
-Version: 0.2.1
+Name: plus_slurm
+Version: 0.2.2
 Summary: Convenient Python Abstraction for the Slurm based cluster at the PLUS
 Home-page: https://gitlab.com/thht/plus-slurm
 Author: Thomas Hartmann
 Author-email: thomas.hartmann@th-ht.de
 License: GPL3
 Keywords: Slurm
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jinja2
+Requires-Dist: future
+Requires-Dist: humanfriendly
+Requires-Dist: six
+Requires-Dist: numpy
+Requires-Dist: psutil
 
 # plus_slurm
 A python module to make it simple to submit jobs to the Slurm based cluster directly from python
 
 ## Documentation
 https://plus-slurm.readthedocs.io
```

### Comparing `plus_slurm-0.2.1/setup.py` & `plus_slurm-0.2.2/setup.py`

 * *Files identical despite different names*

