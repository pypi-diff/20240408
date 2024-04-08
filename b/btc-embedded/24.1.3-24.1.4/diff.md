# Comparing `tmp/btc_embedded-24.1.3.tar.gz` & `tmp/btc_embedded-24.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btc_embedded-24.1.3.tar", last modified: Sun Apr  7 08:01:20 2024, max compression
+gzip compressed data, was "btc_embedded-24.1.4.tar", last modified: Mon Apr  8 11:15:01 2024, max compression
```

## Comparing `btc_embedded-24.1.3.tar` & `btc_embedded-24.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-07 08:01:20.042389 btc_embedded-24.1.3/
--rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/LICENSE.txt
--rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/MANIFEST.in
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-07 08:01:20.042464 btc_embedded-24.1.3/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/README.md
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-07 08:01:20.041504 btc_embedded-24.1.3/btc_embedded/
--rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/btc_embedded/__init__.py
--rw-r--r--   0 thabok     (501) staff       (20)    21391 2024-04-07 08:00:27.000000 btc_embedded-24.1.3/btc_embedded/api.py
--rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/btc_embedded/btc_config.yml
--rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/btc_embedded/btc_summary_report.template
--rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-24.1.3/btc_embedded/config.py
--rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/btc_embedded/reporting.py
--rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/btc_embedded/util.py
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-07 08:01:20.042254 btc_embedded-24.1.3/btc_embedded.egg-info/
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-07 08:01:20.000000 btc_embedded-24.1.3/btc_embedded.egg-info/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)      415 2024-04-07 08:01:20.000000 btc_embedded-24.1.3/btc_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 thabok     (501) staff       (20)        1 2024-04-07 08:01:20.000000 btc_embedded-24.1.3/btc_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 thabok     (501) staff       (20)       16 2024-04-07 08:01:20.000000 btc_embedded-24.1.3/btc_embedded.egg-info/requires.txt
--rw-r--r--   0 thabok     (501) staff       (20)       13 2024-04-07 08:01:20.000000 btc_embedded-24.1.3/btc_embedded.egg-info/top_level.txt
--rw-r--r--   0 thabok     (501) staff       (20)       79 2024-04-07 08:01:20.042695 btc_embedded-24.1.3/setup.cfg
--rw-r--r--   0 thabok     (501) staff       (20)      976 2024-04-07 08:00:31.000000 btc_embedded-24.1.3/setup.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 11:15:01.542532 btc_embedded-24.1.4/
+-rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-24.1.4/LICENSE.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-24.1.4/MANIFEST.in
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-08 11:15:01.542606 btc_embedded-24.1.4/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-24.1.4/README.md
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 11:15:01.541654 btc_embedded-24.1.4/btc_embedded/
+-rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-24.1.4/btc_embedded/__init__.py
+-rw-r--r--   0 thabok     (501) staff       (20)    21478 2024-04-08 11:14:44.000000 btc_embedded-24.1.4/btc_embedded/api.py
+-rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-24.1.4/btc_embedded/btc_config.yml
+-rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-24.1.4/btc_embedded/btc_summary_report.template
+-rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-24.1.4/btc_embedded/config.py
+-rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-24.1.4/btc_embedded/reporting.py
+-rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-24.1.4/btc_embedded/util.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 11:15:01.542403 btc_embedded-24.1.4/btc_embedded.egg-info/
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-08 11:15:01.000000 btc_embedded-24.1.4/btc_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)      415 2024-04-08 11:15:01.000000 btc_embedded-24.1.4/btc_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 thabok     (501) staff       (20)        1 2024-04-08 11:15:01.000000 btc_embedded-24.1.4/btc_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       16 2024-04-08 11:15:01.000000 btc_embedded-24.1.4/btc_embedded.egg-info/requires.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       13 2024-04-08 11:15:01.000000 btc_embedded-24.1.4/btc_embedded.egg-info/top_level.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       79 2024-04-08 11:15:01.542836 btc_embedded-24.1.4/setup.cfg
+-rw-r--r--   0 thabok     (501) staff       (20)      976 2024-04-08 11:14:50.000000 btc_embedded-24.1.4/setup.py
```

### Comparing `btc_embedded-24.1.3/LICENSE.txt` & `btc_embedded-24.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.3/PKG-INFO` & `btc_embedded-24.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc_embedded
-Version: 24.1.3
+Version: 24.1.4
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-24.1.3/README.md` & `btc_embedded-24.1.4/README.md`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.3/btc_embedded/api.py` & `btc_embedded-24.1.4/btc_embedded/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from btc_embedded.config import BTC_CONFIG_ENVVAR_NAME, get_global_config
 
 HEADERS = {'Accept': 'application/json, text/plain', 'Content-Type' : 'application/json'}
 DATE_FORMAT = '%d-%b-%Y %H:%M:%S'
 
 class EPRestApi:
     #Starter for the EP executable
-    def __init__(self, host='http://localhost', port=1337, version=None, install_root=None, install_location=None, lic='', config=None, license_location=None, timeout=120):
+    def __init__(self, host='http://localhost', port=1337, version=None, install_root=None, install_location=None, lic='', config=None, license_location=None, timeout=120, skip_matlab_start=False):
         """
         Wrapper for the BTC EmbeddedPlatform REST API
         - when created without arguments, it uses the default install 
         location & version defined in the global config (btc_config.yml)
         - the global config is identified by the BTC_API_CONFIG_FILE 
         env variable or uses the btc_config.yml file shipped with this module as a fallback
 
@@ -42,15 +42,15 @@
         if version and install_root: install_location = f"{install_root}/ep{version}"
         # fallback: determine based on config
         if not (version and install_location) and 'installationRoot' in config and 'epVersion' in config:
             version = config['epVersion']
             install_location = f"{config['installationRoot']}/ep{config['epVersion']}"
         if not self._is_rest_service_available():
             if platform.system() == 'Windows': self._start_app_windows(version, install_location, port, license_location, lic, config)
-            elif platform.system() == 'Linux': self._start_app_linux()
+            elif platform.system() == 'Linux': self._start_app_linux(skip_matlab_start)
         else:
             print(f'Connected to BTC EmbeddedPlatform REST API at {host}:{self._PORT_}')
             self._apply_preferences(config)
             return
         start_time = time.time()
         print(f'Connecting to BTC EmbeddedPlatform REST API at {host}:{self._PORT_}')
         while not self._is_rest_service_available():
@@ -320,15 +320,15 @@
                 return True
             except OSError:
                 continue
         return False
 
     # start commands depending on OS
 
-    def _start_app_linux(self):
+    def _start_app_linux(self, skip_matlab_start):
         # container use case -> start EP and Matlab
         try:
             ep_ini_path = os.path.join(os.environ['EP_INSTALL_PATH'], 'ep.ini')
             with open(ep_ini_path, 'r') as file:
                 content = file.read()
             version = re.search(r'/ep/(\d+\.\d+[a-zA-Z]*\d+)/', content).group(1)
         except:
@@ -357,15 +357,15 @@
         
         # start ep process
         self.ep_process = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         self.log_file_path = os.environ['LOG_DIR'] + '/current.log'
         self.actively_started = True
         
         # if container has matlab -> assume that this shall be started as well
-        if shutil.which('matlab'): subprocess.Popen('matlab')
+        if shutil.which('matlab') and not skip_matlab_start: subprocess.Popen('matlab')
 
 
     def _start_app_windows(self, version, install_location, port, license_location, lic, config):
         headless_application_id = 'ep.application.headless' if version < '23.3p0' else 'ep.application.headless.HeadlessApplication'
         # check if we have what we need
         if not (version and install_location): raise Exception("Cannot start BTC EmbeddedPlatform. Arguments version and install_location or install_root directory must be specified or configured in a config file (installationRoot)")
         # all good -> prepare start command for BTC EmbeddedPlatform
```

### Comparing `btc_embedded-24.1.3/btc_embedded/btc_config.yml` & `btc_embedded-24.1.4/btc_embedded/btc_config.yml`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.3/btc_embedded/btc_summary_report.template` & `btc_embedded-24.1.4/btc_embedded/btc_summary_report.template`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.3/btc_embedded/config.py` & `btc_embedded-24.1.4/btc_embedded/config.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.3/btc_embedded/reporting.py` & `btc_embedded-24.1.4/btc_embedded/reporting.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.3/btc_embedded/util.py` & `btc_embedded-24.1.4/btc_embedded/util.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.3/btc_embedded.egg-info/PKG-INFO` & `btc_embedded-24.1.4/btc_embedded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc-embedded
-Version: 24.1.3
+Version: 24.1.4
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-24.1.3/setup.py` & `btc_embedded-24.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='btc_embedded',
-    version='24.1.3',
+    version='24.1.4',
     packages=['btc_embedded'],
     include_package_data=True,
     license='MIT',
     description='API wrapper for BTC EmbeddedPlatform 23.3p0 REST API',
     author='Thabo Krick',
     author_email='thabo.krick@btc-embedded.com',
     url='https://github.com/btc-embedded/btc-embedded',
```

