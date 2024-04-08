# Comparing `tmp/getgauge-cli-1.6.4.tar.gz` & `tmp/getgauge-cli-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getgauge-cli-1.6.4.tar", last modified: Mon Mar 11 06:34:12 2024, max compression
+gzip compressed data, was "getgauge-cli-1.6.6.tar", last modified: Mon Apr  8 03:23:12 2024, max compression
```

## Comparing `getgauge-cli-1.6.4.tar` & `getgauge-cli-1.6.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 06:34:12.492596 getgauge-cli-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-11 06:33:57.000000 getgauge-cli-1.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-11 06:34:12.492596 getgauge-cli-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-11 06:33:57.000000 getgauge-cli-1.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 06:34:12.492596 getgauge-cli-1.6.4/getgauge_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-11 06:34:12.000000 getgauge-cli-1.6.4/getgauge_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-11 06:34:12.000000 getgauge-cli-1.6.4/getgauge_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 06:34:12.000000 getgauge-cli-1.6.4/getgauge_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-11 06:34:12.000000 getgauge-cli-1.6.4/getgauge_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 06:34:12.000000 getgauge-cli-1.6.4/getgauge_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 06:34:12.492596 getgauge-cli-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-03-11 06:34:10.000000 getgauge-cli-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:23:12.015881 getgauge-cli-1.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 03:22:58.000000 getgauge-cli-1.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-08 03:23:12.015881 getgauge-cli-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-08 03:22:58.000000 getgauge-cli-1.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:23:12.015881 getgauge-cli-1.6.6/getgauge_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-08 03:23:11.000000 getgauge-cli-1.6.6/getgauge_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-08 03:23:11.000000 getgauge-cli-1.6.6/getgauge_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:23:11.000000 getgauge-cli-1.6.6/getgauge_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 03:23:11.000000 getgauge-cli-1.6.6/getgauge_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:23:11.000000 getgauge-cli-1.6.6/getgauge_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 03:23:12.015881 getgauge-cli-1.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-08 03:23:11.000000 getgauge-cli-1.6.6/setup.py
```

### Comparing `getgauge-cli-1.6.4/PKG-INFO` & `getgauge-cli-1.6.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getgauge-cli
-Version: 1.6.4
+Version: 1.6.6
 Home-page: https://github.com/getgauge/gauge
 Author: getgauge
 Author-email: getgauge@googlegroups.com
 Maintainer: getgauge
 License: Apache-2.0
 Platform: Windows
 Platform: Linux
@@ -21,79 +21,50 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: markdown
 
 # PIP Installer for getgauge-cli tool
 
-This `setup.py` file is used for installed getgauge-cli tool.
-the version number is manually bumped for now.
+This `setup.py` file is used for installing the getgauge-cli tool. The Python package can be installed multiple ways:
 
-Python package can be installed through multiple ways
+## using pip
+
+- pre-requisite: pip should be installed and available on machine
+- run the command `pip install getgauge-cli`
 
 ## using setup.py
 
 - Navigate to the current directory `gauge\build\pip\`
 - Run `python build.py --install` on command prompt (it will install the latest released version)
 - To install a specific version set `GAUGE_VERSION` environment variable.
 
-## using pip
-
-- pre-requisite: pip should be installed and available on machine
-- run the command `pip install getgauge-cli`
-
 ## Check to ensure getgauge-cli is installed
 
 - Once the package has been setup. please exit the current terminal and relaunch terminal again
 - run the command `gauge` , you should be able to see similar output
 ```
 Usage:
   gauge <command> [flags] [args]
 
-Examples:
-  gauge run specs/
-  gauge run --parallel specs/
-
-Commands:
-  config      Change global configurations
-  daemon      Run as a daemon
-  docs        Generate documentation using specified plugin
-  format      Formats the specified spec files
-  help        Help about any command
-  init        Initialize project structure in the current directory
-  install     Download and install plugin(s)
-  list        List specifications, scenarios or tags for a gauge project
-  man         Generate man pages
-  run         Run specs
-  uninstall   Uninstalls a plugin
-  update      Updates a plugin
-  validate    Check for validation and parse errors
-  version     Print Gauge and plugin versions
-
-Flags:
-  -d, --dir string         Set the working directory for the current command, accepts a path relative to current directory (default ".")
-  -h, --help               Help for gauge
-  -l, --log-level string   Set level of logging to debug, info, warning, error or critical (default "info")
-  -m, --machine-readable   Prints output in JSON format
-  -v, --version            Print Gauge and plugin versions
-
-Use "gauge [command] --help" for more information about a command.
-Complete manual is available at https://manpage.gauge.org/.
+# ...etc
 ```
 
 ## Using setup.py
 - Install required dep by running `python/python3 -m pip install requirements.txt`.
 - Check through and obtain a valid tag/build number from [releases](https://github.com/getgauge/gauge/releases)
 - Run the command `python build.py --install` (set GAUGE_VERSION env to install specific version)
 - This would install the version as specified along with latest release of Gauge-CLI Version
 
-- Run the command `python build.py --dist` to generate the PyPi distrubutable (set GAUGE_VERSION env to install specific version)
+- Run the command `python build.py --dist` to generate the PyPi distributable (set GAUGE_VERSION env to install specific version)
 
 ## Uninstalling Gauge CLI
 
 Gauge CLI uninstall should be done manually for now.
 Run the following command on your prompt
 ```
 $ pip uninstall gauge-cli
```

### Comparing `getgauge-cli-1.6.4/README.md` & `getgauge-cli-1.6.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,40 @@
 # PIP Installer for getgauge-cli tool
 
-This `setup.py` file is used for installed getgauge-cli tool.
-the version number is manually bumped for now.
+This `setup.py` file is used for installing the getgauge-cli tool. The Python package can be installed multiple ways:
 
-Python package can be installed through multiple ways
+## using pip
+
+- pre-requisite: pip should be installed and available on machine
+- run the command `pip install getgauge-cli`
 
 ## using setup.py
 
 - Navigate to the current directory `gauge\build\pip\`
 - Run `python build.py --install` on command prompt (it will install the latest released version)
 - To install a specific version set `GAUGE_VERSION` environment variable.
 
-## using pip
-
-- pre-requisite: pip should be installed and available on machine
-- run the command `pip install getgauge-cli`
-
 ## Check to ensure getgauge-cli is installed
 
 - Once the package has been setup. please exit the current terminal and relaunch terminal again
 - run the command `gauge` , you should be able to see similar output
 ```
 Usage:
   gauge <command> [flags] [args]
 
-Examples:
-  gauge run specs/
-  gauge run --parallel specs/
-
-Commands:
-  config      Change global configurations
-  daemon      Run as a daemon
-  docs        Generate documentation using specified plugin
-  format      Formats the specified spec files
-  help        Help about any command
-  init        Initialize project structure in the current directory
-  install     Download and install plugin(s)
-  list        List specifications, scenarios or tags for a gauge project
-  man         Generate man pages
-  run         Run specs
-  uninstall   Uninstalls a plugin
-  update      Updates a plugin
-  validate    Check for validation and parse errors
-  version     Print Gauge and plugin versions
-
-Flags:
-  -d, --dir string         Set the working directory for the current command, accepts a path relative to current directory (default ".")
-  -h, --help               Help for gauge
-  -l, --log-level string   Set level of logging to debug, info, warning, error or critical (default "info")
-  -m, --machine-readable   Prints output in JSON format
-  -v, --version            Print Gauge and plugin versions
-
-Use "gauge [command] --help" for more information about a command.
-Complete manual is available at https://manpage.gauge.org/.
+# ...etc
 ```
 
 ## Using setup.py
 - Install required dep by running `python/python3 -m pip install requirements.txt`.
 - Check through and obtain a valid tag/build number from [releases](https://github.com/getgauge/gauge/releases)
 - Run the command `python build.py --install` (set GAUGE_VERSION env to install specific version)
 - This would install the version as specified along with latest release of Gauge-CLI Version
 
-- Run the command `python build.py --dist` to generate the PyPi distrubutable (set GAUGE_VERSION env to install specific version)
+- Run the command `python build.py --dist` to generate the PyPi distributable (set GAUGE_VERSION env to install specific version)
 
 ## Uninstalling Gauge CLI
 
 Gauge CLI uninstall should be done manually for now.
 Run the following command on your prompt
 ```
 $ pip uninstall gauge-cli
```

### Comparing `getgauge-cli-1.6.4/getgauge_cli.egg-info/PKG-INFO` & `getgauge-cli-1.6.6/getgauge_cli.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getgauge-cli
-Version: 1.6.4
+Version: 1.6.6
 Home-page: https://github.com/getgauge/gauge
 Author: getgauge
 Author-email: getgauge@googlegroups.com
 Maintainer: getgauge
 License: Apache-2.0
 Platform: Windows
 Platform: Linux
@@ -21,79 +21,50 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: markdown
 
 # PIP Installer for getgauge-cli tool
 
-This `setup.py` file is used for installed getgauge-cli tool.
-the version number is manually bumped for now.
+This `setup.py` file is used for installing the getgauge-cli tool. The Python package can be installed multiple ways:
 
-Python package can be installed through multiple ways
+## using pip
+
+- pre-requisite: pip should be installed and available on machine
+- run the command `pip install getgauge-cli`
 
 ## using setup.py
 
 - Navigate to the current directory `gauge\build\pip\`
 - Run `python build.py --install` on command prompt (it will install the latest released version)
 - To install a specific version set `GAUGE_VERSION` environment variable.
 
-## using pip
-
-- pre-requisite: pip should be installed and available on machine
-- run the command `pip install getgauge-cli`
-
 ## Check to ensure getgauge-cli is installed
 
 - Once the package has been setup. please exit the current terminal and relaunch terminal again
 - run the command `gauge` , you should be able to see similar output
 ```
 Usage:
   gauge <command> [flags] [args]
 
-Examples:
-  gauge run specs/
-  gauge run --parallel specs/
-
-Commands:
-  config      Change global configurations
-  daemon      Run as a daemon
-  docs        Generate documentation using specified plugin
-  format      Formats the specified spec files
-  help        Help about any command
-  init        Initialize project structure in the current directory
-  install     Download and install plugin(s)
-  list        List specifications, scenarios or tags for a gauge project
-  man         Generate man pages
-  run         Run specs
-  uninstall   Uninstalls a plugin
-  update      Updates a plugin
-  validate    Check for validation and parse errors
-  version     Print Gauge and plugin versions
-
-Flags:
-  -d, --dir string         Set the working directory for the current command, accepts a path relative to current directory (default ".")
-  -h, --help               Help for gauge
-  -l, --log-level string   Set level of logging to debug, info, warning, error or critical (default "info")
-  -m, --machine-readable   Prints output in JSON format
-  -v, --version            Print Gauge and plugin versions
-
-Use "gauge [command] --help" for more information about a command.
-Complete manual is available at https://manpage.gauge.org/.
+# ...etc
 ```
 
 ## Using setup.py
 - Install required dep by running `python/python3 -m pip install requirements.txt`.
 - Check through and obtain a valid tag/build number from [releases](https://github.com/getgauge/gauge/releases)
 - Run the command `python build.py --install` (set GAUGE_VERSION env to install specific version)
 - This would install the version as specified along with latest release of Gauge-CLI Version
 
-- Run the command `python build.py --dist` to generate the PyPi distrubutable (set GAUGE_VERSION env to install specific version)
+- Run the command `python build.py --dist` to generate the PyPi distributable (set GAUGE_VERSION env to install specific version)
 
 ## Uninstalling Gauge CLI
 
 Gauge CLI uninstall should be done manually for now.
 Run the following command on your prompt
 ```
 $ pip uninstall gauge-cli
```

### Comparing `getgauge-cli-1.6.4/setup.py` & `getgauge-cli-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import platform
 import zipfile
 import os
 import sys
 
 
-_version = "1.6.4"
+_version = "1.6.6"
 _latest_version = ""
 
 
 class CustomInstallCommand(install):
     """Customized setuptools install command to download and setup."""
 
     _base_url = 'https://api.github.com/repos/getgauge/gauge/releases'
@@ -33,15 +33,15 @@
         return requests.get(url)
 
     def set_released_version(self):
         global _latest_version
         _latest_version = json.loads(self._get(self._base_url).text)[0]['tag_name'].replace('v', '')
 
     def _get_gauge_file(self):
-        if self._os_name is 'win32':
+        if self._os_name == 'win32':
             return 'gauge.exe'
         else:
             return 'gauge'
 
     def _gauge_package_fetch(self):
         package_name = 'gauge-%s-%s.%s' % (_version,
                                            self._os_name, self._get_arch())
@@ -59,15 +59,15 @@
         target_path = os.path.join(
             self.install_scripts, self._get_gauge_file())
         source_path = os.path.join(os.getcwd(), self._get_gauge_file())
         if os.path.isfile(target_path):
             os.remove(target_path)
         if os.path.isfile(source_path):
             self.move_file(source_path, target_path)
-            if self._os_name is not "win32":
+            if self._os_name != "win32":
                 if sys.version_info[0] == 3:
                     os.chmod(target_path, 0o755)
                 if sys.version_info[0] < 3:
                     os.chmod(target_path, 755)
 
     def run(self):
         """Custom Install / Run Command."""
```

