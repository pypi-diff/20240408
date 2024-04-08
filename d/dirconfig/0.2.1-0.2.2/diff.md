# Comparing `tmp/dirconfig-0.2.1.tar.gz` & `tmp/dirconfig-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirconfig-0.2.1.tar", last modified: Thu Apr  4 21:05:09 2024, max compression
+gzip compressed data, was "dirconfig-0.2.2.tar", last modified: Mon Apr  8 02:42:00 2024, max compression
```

## Comparing `dirconfig-0.2.1.tar` & `dirconfig-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 21:05:09.316445 dirconfig-0.2.1/
--rw-rw-rw-   0        0        0     1087 2024-04-03 00:38:18.000000 dirconfig-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     3051 2024-04-04 21:05:09.315445 dirconfig-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2461 2024-04-04 17:49:18.000000 dirconfig-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 21:05:09.282443 dirconfig-0.2.1/dirconfig/
--rw-rw-rw-   0        0        0        0 2024-04-03 01:36:27.000000 dirconfig-0.2.1/dirconfig/__init__.py
--rw-rw-rw-   0        0        0     4928 2024-04-04 17:47:55.000000 dirconfig-0.2.1/dirconfig/main.py
-drwxrwxrwx   0        0        0        0 2024-04-04 21:05:09.314448 dirconfig-0.2.1/dirconfig.egg-info/
--rw-rw-rw-   0        0        0     3051 2024-04-04 21:05:08.000000 dirconfig-0.2.1/dirconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-04 21:05:09.000000 dirconfig-0.2.1/dirconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 21:05:08.000000 dirconfig-0.2.1/dirconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-04 21:05:08.000000 dirconfig-0.2.1/dirconfig.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-04-04 21:05:08.000000 dirconfig-0.2.1/dirconfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 21:05:08.000000 dirconfig-0.2.1/dirconfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 21:05:09.316445 dirconfig-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-04-04 17:38:47.000000 dirconfig-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:42:00.224287 dirconfig-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-08 02:41:52.000000 dirconfig-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-08 02:42:00.220287 dirconfig-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-08 02:41:52.000000 dirconfig-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:42:00.220287 dirconfig-0.2.2/dirconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:41:52.000000 dirconfig-0.2.2/dirconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-08 02:41:52.000000 dirconfig-0.2.2/dirconfig/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:42:00.220287 dirconfig-0.2.2/dirconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-08 02:42:00.000000 dirconfig-0.2.2/dirconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 02:42:00.000000 dirconfig-0.2.2/dirconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 02:42:00.000000 dirconfig-0.2.2/dirconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 02:42:00.000000 dirconfig-0.2.2/dirconfig.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 02:42:00.000000 dirconfig-0.2.2/dirconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 02:42:00.000000 dirconfig-0.2.2/dirconfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 02:42:00.224287 dirconfig-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-08 02:41:58.000000 dirconfig-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:42:00.220287 dirconfig-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:41:52.000000 dirconfig-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-08 02:41:52.000000 dirconfig-0.2.2/tests/test_main.py
```

### Comparing `dirconfig-0.2.1/PKG-INFO` & `dirconfig-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,97 @@
-Metadata-Version: 2.1
-Name: dirconfig
-Version: 0.2.1
-Summary: A simple directory configuration tool
-Home-page: https://github.com/judahpaul16/dirconfig
-Author: Judah Paul
-Author-email: me@judahpaul.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: watchdog==4.0.0
-
-# dirconfig ðŸ“‚
- Configure what files should be in what folders using an easy-to-read YAML config file.
-
-## Features
-
-- **File Organization**: Automatically move files based on their extension from one directory to another.
-- **Notification System** (Future Feature): Get notified regarding specific events specified in the configuration file.
-- **Automated Backups** (Future Feature): Set up scheduled backups for important directories.
-
-## Installation
-
-Install **dirconfig** using pip:
-
-```sh
-pip install dirconfig
-```
-
-## Configuration
-
-Create a `config.yml` file in your working directory with your automation tasks. Here's an example configuration that organizes `.jpg` and `.pdf` files into separate directories:
-
-```yaml
-tasks:
-  - name: Organize Downloads
-    type: file-organization
-    source: /path/to/your/source/directory
-    rules:
-      - extension: .jpg
-        destination: /path/to/your/destination/for/images
-      - extension: .pdf
-        destination: /path/to/your/destination/for/documents
-```
-
-## Usage
-
-**dirconfig** is designed to run as a daemon, monitoring specified directories and automatically organizing files according to the configurations defined in your `config.yml` file.
-
-### Starting dirconfig
-
-To initiate **dirconfig** and begin the monitoring process, use the following command:
-
-```sh
-dirconfig start
-```
-
-This command starts **dirconfig**, which then operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
-
-To run **dirconfig** as a separate process, use the following command:
-
-```sh
-dirconfig start &
-```
-
-### Stopping dirconfig
-
-To stop the **dirconfig** daemon, execute:
-
-```sh
-dirconfig stop
-```
-
-This command stops the background process of **dirconfig**, halting the monitoring and file organization tasks.
-
-### Advanced Management
-
-For long-term operation or deployment, integrating **dirconfig** with system services or process managers can offer more graceful management, including automatic restarts, logging, and simplified start/stop operations.
-
-## Extending dirconfig
-
-**dirconfig** welcomes enhancements and customization. If you're interested in adding new features or improving the tool, consider contributing to the source code. Your input and contributions are highly appreciated.
-
-## License
-
-**dirconfig** is licensed under the MIT License. See the `LICENSE` file for more details.
+Metadata-Version: 2.1
+Name: dirconfig
+Version: 0.2.2
+Summary: A simple directory configuration tool
+Home-page: https://github.com/judahpaul16/dirconfig
+Author: Judah Paul
+Author-email: me@judahpaul.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dirconfig 📂
+ Configure what files should be in what folders using an easy-to-read YAML config file.
+
+![PyPI](https://img.shields.io/pypi/v/dirconfig)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dirconfig)
+![PyPI - License](https://img.shields.io/pypi/l/dirconfig)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/judahpaul16/dirconfig/workflow.yaml)
+
+## Features
+
+- **File Organization**: Automatically move files based on their extension from one directory to another.
+- **Notification System** (Future Feature): Get notified regarding specific events specified in the configuration file.
+- **Automated Backups** (Future Feature): Set up scheduled backups for important directories.
+
+## Installation
+
+Install **dirconfig** using pip:
+
+```sh
+pip install dirconfig
+```
+
+## Configuration
+
+Create a `config.yml` file in your working directory with your automation tasks. Here's an example configuration that organizes `.jpg` and `.pdf` files into separate directories:
+
+```yaml
+tasks:
+  - name: Organize Downloads
+    type: file-organization
+    source: /path/to/your/source/directory
+    rules:
+      - extension: .jpg
+        destination: /path/to/your/destination/for/images
+      - extension: .pdf
+        destination: /path/to/your/destination/for/documents
+```
+
+## Usage
+
+**dirconfig** is designed to run as a daemon, monitoring specified directories and automatically organizing files according to the configurations defined in your `config.yml` file.
+
+### Starting dirconfig
+
+To initiate **dirconfig** and begin the monitoring process, use the following command:
+
+```sh
+dirconfig start
+```
+
+This command starts **dirconfig**, which then operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
+
+To run **dirconfig** as a separate process, use the following command:
+
+```sh
+dirconfig start &
+```
+
+### Stopping dirconfig
+
+To stop the **dirconfig** daemon, execute:
+
+```sh
+dirconfig stop
+```
+
+This command stops the background process of **dirconfig**, halting the monitoring and file organization tasks.
+
+### Advanced Management
+
+For long-term operation or deployment, integrating **dirconfig** with system services or process managers can offer more graceful management, including automatic restarts, logging, and simplified start/stop operations.
+
+## Extending dirconfig
+
+**dirconfig** welcomes enhancements and customization. If you're interested in adding new features or improving the tool, consider contributing to the source code. Your input and contributions are highly appreciated.
+
+## License
+
+**dirconfig** is licensed under the MIT License. See the `LICENSE` file for more details.
+
+
```

### Comparing `dirconfig-0.2.1/README.md` & `dirconfig-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # dirconfig 📂
  Configure what files should be in what folders using an easy-to-read YAML config file.
 
+![PyPI](https://img.shields.io/pypi/v/dirconfig)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dirconfig)
+![PyPI - License](https://img.shields.io/pypi/l/dirconfig)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/judahpaul16/dirconfig/workflow.yaml)
+
 ## Features
 
 - **File Organization**: Automatically move files based on their extension from one directory to another.
 - **Notification System** (Future Feature): Get notified regarding specific events specified in the configuration file.
 - **Automated Backups** (Future Feature): Set up scheduled backups for important directories.
 
 ## Installation
```

### Comparing `dirconfig-0.2.1/dirconfig/main.py` & `dirconfig-0.2.2/dirconfig/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,134 @@
-from watchdog.events import FileSystemEventHandler
-from watchdog.observers import Observer
-from pathlib import Path
-import argparse
-import logging
-import signal
-import shutil
-import yaml
-import sys
-import os
-
-observer = None
-PID_FILE = 'dirconfig.pid'
-
-class ChangeHandler(FileSystemEventHandler):
-    def __init__(self, tasks):
-        self.tasks = tasks
-
-    def on_any_event(self, event):
-        for task in self.tasks:
-            if task['type'] == 'file-organization':
-                organize_files(task)
-
-def load_config(config_path):
-    with open(config_path, 'r') as file:
-        return yaml.safe_load(file)
-
-def organize_files(task):
-    source = task['source']
-    # Use the current working directory as the base for relative paths.
-    cwd = os.getcwd()
-    
-    # If the source is a relative path, resolve it based on the current working directory.
-    source_path = os.path.abspath(os.path.join(cwd, source)) if source.startswith(".") else os.path.abspath(source)
-    
-    rules = task['rules']
-    
-    for file in os.listdir(source_path):
-        for rule in rules:
-            if file.endswith(rule['extension']):
-                # For destination paths starting with "/", treat them as absolute paths.
-                # Otherwise, treat as relative to the source directory.
-                if rule['destination'].startswith("/"):
-                    dest_path = os.path.abspath(rule['destination'][1:])
-                else:
-                    dest_path = os.path.abspath(os.path.join(source_path, rule['destination']))
-                
-                if not os.path.exists(dest_path):
-                    os.makedirs(dest_path)
-                
-                source_file_path = os.path.join(source_path, file)
-                dest_file_path = os.path.join(dest_path, file)
-                shutil.move(source_file_path, dest_file_path)
-                print(f"Moved: {file} -> {dest_file_path}")
-                logging.info(f"Moved: {file} -> {dest_file_path}")
-
-def signal_handler(signum, frame):
-    print("\nReceived interrupt signal. Stopping dirconfig...")
-    logging.info("Received interrupt signal. Stopping dirconfig...")
-    if observer is not None:
-        observer.stop()
-        observer.join()  # Ensure all threads are joined
-        if os.path.exists(PID_FILE):
-            os.remove(PID_FILE)
-        sys.exit(0)
-
-def start_daemon(config_path):
-    global observer
-    config = load_config(config_path)
-    tasks = config['tasks']
-    observer = Observer()
-    for task in tasks:
-        if task['type'] == 'file-organization':
-            observer.schedule(ChangeHandler(tasks), os.path.abspath(task['source']), recursive=True)
-
-    # Register the signal handler for SIGINT
-    signal.signal(signal.SIGINT, signal_handler)
-
-    observer.start()
-    with open(PID_FILE, 'w') as f:
-        f.write(str(os.getpid()))
-
-    # This loop keeps the script running until the observer is stopped
-    try:
-        while observer.is_alive():
-            observer.join(1)
-    finally:
-        if observer.is_alive():
-            observer.stop()
-            observer.join()
-
-def stop_daemon():
-    try:
-        with open(PID_FILE, 'r') as f:
-            pid = int(f.read())
-        os.kill(pid, signal.SIGTERM)
-    except FileNotFoundError:
-        print("Error: PID file not found. Is the daemon running?")
-        logging.error("Error: PID file not found. Is the daemon running?")
-        sys.exit(1)
-    except ProcessLookupError:
-        print("Error: Process not found. It may have been stopped already.")
-        logging.error("Error: Process not found. It may have been stopped already.")
-        sys.exit(1)
-
-def main():
-    parser = argparse.ArgumentParser(description='dirconfig Daemon')
-    parser.add_argument('action', choices=['start', 'stop'], help='Start or stop the daemon')
-    # Default to 'config.yaml' in the current working directory if not specified
-    parser.add_argument('--config', help='Path to the configuration file', default='config.yaml')
-    parser.add_argument('--log', help='Path to the log file', default='dirconfig.log')
-    args = parser.parse_args()
-
-    # Resolve the absolute path of the configuration file
-    config_path = os.path.abspath(args.config)
-
-    # Initialize logging to log to a file specified by the --log argument.
-    logging.basicConfig(level=logging.INFO, filename=args.log, filemode='a', format='%(asctime)s - %(levelname)s - %(message)s')
-
-    if args.action == 'start':
-        if not os.path.exists(config_path):
-            print(f"Configuration file not found: {config_path}")
-            logging.error(f"Configuration file not found: {config_path}")
-            sys.exit(1)
-        start_daemon(config_path)
-    elif args.action == 'stop':
-        stop_daemon()
-
-if __name__ == "__main__":
-    main()
+from watchdog.events import FileSystemEventHandler
+from watchdog.observers import Observer
+from pathlib import Path
+import argparse
+import logging
+import signal
+import shutil
+import yaml
+import sys
+import os
+
+observer = None
+PID_FILE = 'dirconfig.pid'
+
+class ChangeHandler(FileSystemEventHandler):
+    def __init__(self, tasks):
+        self.tasks = tasks
+
+    def on_any_event(self, event):
+        for task in self.tasks:
+            if task['type'] == 'file-organization':
+                organize_files(task)
+
+def load_config(config_path):
+    with open(config_path, 'r') as file:
+        return yaml.safe_load(file)
+
+def organize_files(task):
+    source = task['source']
+    # Use the current working directory as the base for relative paths.
+    cwd = os.getcwd()
+    
+    # If the source is a relative path, resolve it based on the current working directory.
+    source_path = os.path.abspath(os.path.join(cwd, source)) if source.startswith(".") else os.path.abspath(source)
+    
+    rules = task['rules']
+    
+    for file in os.listdir(source_path):
+        file_extension = os.path.splitext(file)[1]
+        
+        for rule in rules:
+            extensions = [ext.strip() for ext in rule['extension'].split(',')]
+            
+            if file_extension in extensions:
+                # For destination paths starting with "/", treat them as absolute paths.
+                # Otherwise, treat as relative to the source directory.
+                if rule['destination'].startswith("/"):
+                    dest_path = os.path.abspath(rule['destination'][1:])
+                else:
+                    dest_path = os.path.abspath(os.path.join(source_path, rule['destination']))
+                
+                if not os.path.exists(dest_path):
+                    os.makedirs(dest_path)
+                
+                source_file_path = os.path.join(source_path, file)
+                dest_file_path = os.path.join(dest_path, file)
+                shutil.move(source_file_path, dest_file_path)
+                print(f"Moved: {file} -> {dest_file_path}")
+                logging.info(f"Moved: {file} -> {dest_file_path}")
+
+def signal_handler(signum, frame):
+    print("\nReceived interrupt signal. Stopping dirconfig...")
+    logging.info("Received interrupt signal. Stopping dirconfig...")
+    if observer is not None:
+        observer.stop()
+        observer.join()  # Ensure all threads are joined
+        if os.path.exists(PID_FILE):
+            os.remove(PID_FILE)
+        sys.exit(0)
+
+def start_daemon(config_path):
+    global observer
+    config = load_config(config_path)
+    tasks = config['tasks']
+    observer = Observer()
+    for task in tasks:
+        if task['type'] == 'file-organization':
+            observer.schedule(ChangeHandler(tasks), os.path.abspath(task['source']), recursive=True)
+
+    # Register the signal handler for SIGINT
+    signal.signal(signal.SIGINT, signal_handler)
+
+    observer.start()
+    with open(PID_FILE, 'w') as f:
+        f.write(str(os.getpid()))
+
+    # This loop keeps the script running until the observer is stopped
+    try:
+        while observer.is_alive():
+            observer.join(1)
+    finally:
+        if observer.is_alive():
+            observer.stop()
+            observer.join()
+
+def stop_daemon():
+    try:
+        with open(PID_FILE, 'r') as f:
+            pid = int(f.read())
+        os.kill(pid, signal.SIGTERM)
+    except FileNotFoundError:
+        print("Error: PID file not found. Is the daemon running?")
+        logging.error("Error: PID file not found. Is the daemon running?")
+        sys.exit(1)
+    except ProcessLookupError:
+        print("Error: Process not found. It may have been stopped already.")
+        logging.error("Error: Process not found. It may have been stopped already.")
+        sys.exit(1)
+
+def main():
+    parser = argparse.ArgumentParser(description='dirconfig Daemon')
+    parser.add_argument('action', choices=['start', 'stop'], help='Start or stop the daemon')
+    # Default to 'config.yaml' in the current working directory if not specified
+    parser.add_argument('--config', help='Path to the configuration file', default='config.yaml')
+    parser.add_argument('--log', help='Path to the log file', default='dirconfig.log')
+    args = parser.parse_args()
+
+    # Resolve the absolute path of the configuration file
+    config_path = os.path.abspath(args.config)
+
+    # Initialize logging to log to a file specified by the --log argument.
+    logging.basicConfig(level=logging.INFO, filename=args.log, filemode='a', format='%(asctime)s - %(levelname)s - %(message)s')
+
+    if args.action == 'start':
+        if not os.path.exists(config_path):
+            print(f"Configuration file not found: {config_path}")
+            logging.error(f"Configuration file not found: {config_path}")
+            sys.exit(1)
+        start_daemon(config_path)
+    elif args.action == 'stop':
+        stop_daemon()
+
+if __name__ == "__main__":
+    main()
```

### Comparing `dirconfig-0.2.1/dirconfig.egg-info/PKG-INFO` & `dirconfig-0.2.2/dirconfig.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,97 @@
-Metadata-Version: 2.1
-Name: dirconfig
-Version: 0.2.1
-Summary: A simple directory configuration tool
-Home-page: https://github.com/judahpaul16/dirconfig
-Author: Judah Paul
-Author-email: me@judahpaul.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: watchdog==4.0.0
-
-# dirconfig ðŸ“‚
- Configure what files should be in what folders using an easy-to-read YAML config file.
-
-## Features
-
-- **File Organization**: Automatically move files based on their extension from one directory to another.
-- **Notification System** (Future Feature): Get notified regarding specific events specified in the configuration file.
-- **Automated Backups** (Future Feature): Set up scheduled backups for important directories.
-
-## Installation
-
-Install **dirconfig** using pip:
-
-```sh
-pip install dirconfig
-```
-
-## Configuration
-
-Create a `config.yml` file in your working directory with your automation tasks. Here's an example configuration that organizes `.jpg` and `.pdf` files into separate directories:
-
-```yaml
-tasks:
-  - name: Organize Downloads
-    type: file-organization
-    source: /path/to/your/source/directory
-    rules:
-      - extension: .jpg
-        destination: /path/to/your/destination/for/images
-      - extension: .pdf
-        destination: /path/to/your/destination/for/documents
-```
-
-## Usage
-
-**dirconfig** is designed to run as a daemon, monitoring specified directories and automatically organizing files according to the configurations defined in your `config.yml` file.
-
-### Starting dirconfig
-
-To initiate **dirconfig** and begin the monitoring process, use the following command:
-
-```sh
-dirconfig start
-```
-
-This command starts **dirconfig**, which then operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
-
-To run **dirconfig** as a separate process, use the following command:
-
-```sh
-dirconfig start &
-```
-
-### Stopping dirconfig
-
-To stop the **dirconfig** daemon, execute:
-
-```sh
-dirconfig stop
-```
-
-This command stops the background process of **dirconfig**, halting the monitoring and file organization tasks.
-
-### Advanced Management
-
-For long-term operation or deployment, integrating **dirconfig** with system services or process managers can offer more graceful management, including automatic restarts, logging, and simplified start/stop operations.
-
-## Extending dirconfig
-
-**dirconfig** welcomes enhancements and customization. If you're interested in adding new features or improving the tool, consider contributing to the source code. Your input and contributions are highly appreciated.
-
-## License
-
-**dirconfig** is licensed under the MIT License. See the `LICENSE` file for more details.
+Metadata-Version: 2.1
+Name: dirconfig
+Version: 0.2.2
+Summary: A simple directory configuration tool
+Home-page: https://github.com/judahpaul16/dirconfig
+Author: Judah Paul
+Author-email: me@judahpaul.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dirconfig 📂
+ Configure what files should be in what folders using an easy-to-read YAML config file.
+
+![PyPI](https://img.shields.io/pypi/v/dirconfig)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dirconfig)
+![PyPI - License](https://img.shields.io/pypi/l/dirconfig)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/judahpaul16/dirconfig/workflow.yaml)
+
+## Features
+
+- **File Organization**: Automatically move files based on their extension from one directory to another.
+- **Notification System** (Future Feature): Get notified regarding specific events specified in the configuration file.
+- **Automated Backups** (Future Feature): Set up scheduled backups for important directories.
+
+## Installation
+
+Install **dirconfig** using pip:
+
+```sh
+pip install dirconfig
+```
+
+## Configuration
+
+Create a `config.yml` file in your working directory with your automation tasks. Here's an example configuration that organizes `.jpg` and `.pdf` files into separate directories:
+
+```yaml
+tasks:
+  - name: Organize Downloads
+    type: file-organization
+    source: /path/to/your/source/directory
+    rules:
+      - extension: .jpg
+        destination: /path/to/your/destination/for/images
+      - extension: .pdf
+        destination: /path/to/your/destination/for/documents
+```
+
+## Usage
+
+**dirconfig** is designed to run as a daemon, monitoring specified directories and automatically organizing files according to the configurations defined in your `config.yml` file.
+
+### Starting dirconfig
+
+To initiate **dirconfig** and begin the monitoring process, use the following command:
+
+```sh
+dirconfig start
+```
+
+This command starts **dirconfig**, which then operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
+
+To run **dirconfig** as a separate process, use the following command:
+
+```sh
+dirconfig start &
+```
+
+### Stopping dirconfig
+
+To stop the **dirconfig** daemon, execute:
+
+```sh
+dirconfig stop
+```
+
+This command stops the background process of **dirconfig**, halting the monitoring and file organization tasks.
+
+### Advanced Management
+
+For long-term operation or deployment, integrating **dirconfig** with system services or process managers can offer more graceful management, including automatic restarts, logging, and simplified start/stop operations.
+
+## Extending dirconfig
+
+**dirconfig** welcomes enhancements and customization. If you're interested in adding new features or improving the tool, consider contributing to the source code. Your input and contributions are highly appreciated.
+
+## License
+
+**dirconfig** is licensed under the MIT License. See the `LICENSE` file for more details.
+
+
```

### Comparing `dirconfig-0.2.1/setup.py` & `dirconfig-0.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from setuptools import setup, find_packages
-
-setup(
-    name="dirconfig",
-    version="0.2.1",
-    author="Judah Paul",
-    author_email="me@judahpaul.com",
-    description="A simple directory configuration tool",
-    long_description=open('README.md').read(),
-    long_description_content_type="text/markdown",
-    url="https://github.com/judahpaul16/dirconfig",
-    packages=find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',
-    entry_points={
-        "console_scripts": [
-            "dirconfig=dirconfig.main:main",
-        ],
-    },
-    install_requires=[
-        "PyYAML==6.0.1",
-        "watchdog==4.0.0"
-    ],
-)
+from setuptools import setup, find_packages
+
+setup(
+    name="dirconfig",
+    version="0.2.2",
+    author="Judah Paul",
+    author_email="me@judahpaul.com",
+    description="A simple directory configuration tool",
+    long_description=open('README.md').read(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/judahpaul16/dirconfig",
+    packages=find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.6',
+    entry_points={
+        "console_scripts": [
+            "dirconfig=dirconfig.main:main",
+        ],
+    },
+    install_requires=[
+        "PyYAML==6.0.1",
+        "watchdog==4.0.0"
+    ],
+)
```

