# Comparing `tmp/openobserve-1.0.0.tar.gz` & `tmp/openobserve-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobserve-1.0.0.tar", last modified: Thu Apr  4 20:30:48 2024, max compression
+gzip compressed data, was "openobserve-1.0.1.tar", last modified: Mon Apr  8 14:34:24 2024, max compression
```

## Comparing `openobserve-1.0.0.tar` & `openobserve-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-04 20:30:48.035321 openobserve-1.0.0/
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1073 2024-04-04 20:27:41.000000 openobserve-1.0.0/LICENSE
--rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2250 2024-04-04 20:30:48.035321 openobserve-1.0.0/PKG-INFO
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1845 2024-04-04 20:27:02.000000 openobserve-1.0.0/README.md
-drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-04 20:30:48.035321 openobserve-1.0.0/openobserve/
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1985 2024-04-04 20:30:30.000000 openobserve-1.0.0/openobserve/__init__.py
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      677 2024-04-04 20:29:50.000000 openobserve-1.0.0/openobserve/generate.py
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      932 2024-04-04 20:29:50.000000 openobserve-1.0.0/openobserve/global_exception_logger.py
-drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-04 20:30:48.035321 openobserve-1.0.0/openobserve.egg-info/
--rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2250 2024-04-04 20:30:48.000000 openobserve-1.0.0/openobserve.egg-info/PKG-INFO
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      287 2024-04-04 20:30:48.000000 openobserve-1.0.0/openobserve.egg-info/SOURCES.txt
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        1 2024-04-04 20:30:48.000000 openobserve-1.0.0/openobserve.egg-info/dependency_links.txt
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)       16 2024-04-04 20:30:48.000000 openobserve-1.0.0/openobserve.egg-info/requires.txt
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)       12 2024-04-04 20:30:48.000000 openobserve-1.0.0/openobserve.egg-info/top_level.txt
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)       38 2024-04-04 20:30:48.035321 openobserve-1.0.0/setup.cfg
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      656 2024-04-04 20:27:41.000000 openobserve-1.0.0/setup.py
+drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-08 14:34:24.706847 openobserve-1.0.1/
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1073 2024-04-04 20:27:41.000000 openobserve-1.0.1/LICENSE
+-rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2238 2024-04-08 14:34:24.706847 openobserve-1.0.1/PKG-INFO
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1833 2024-04-08 14:33:21.000000 openobserve-1.0.1/README.md
+drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-08 14:34:24.702847 openobserve-1.0.1/openobserve/
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1957 2024-04-08 14:34:05.000000 openobserve-1.0.1/openobserve/__init__.py
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      677 2024-04-04 20:29:50.000000 openobserve-1.0.1/openobserve/generate.py
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      932 2024-04-04 20:29:50.000000 openobserve-1.0.1/openobserve/global_exception_logger.py
+drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-08 14:34:24.702847 openobserve-1.0.1/openobserve.egg-info/
+-rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2238 2024-04-08 14:34:24.000000 openobserve-1.0.1/openobserve.egg-info/PKG-INFO
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      287 2024-04-08 14:34:24.000000 openobserve-1.0.1/openobserve.egg-info/SOURCES.txt
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        1 2024-04-08 14:34:24.000000 openobserve-1.0.1/openobserve.egg-info/dependency_links.txt
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)       16 2024-04-08 14:34:24.000000 openobserve-1.0.1/openobserve.egg-info/requires.txt
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)       12 2024-04-08 14:34:24.000000 openobserve-1.0.1/openobserve.egg-info/top_level.txt
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)       38 2024-04-08 14:34:24.706847 openobserve-1.0.1/setup.cfg
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      656 2024-04-08 14:33:21.000000 openobserve-1.0.1/setup.py
```

### Comparing `openobserve-1.0.0/LICENSE` & `openobserve-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openobserve-1.0.0/PKG-INFO` & `openobserve-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 Metadata-Version: 2.1
 Name: openobserve
-Version: 1.0.0
+Version: 1.0.1
 Summary: OpenObserve library
 Author: Krzysztof Żyłka
 Author-email: krzysztofzylka@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: jsonex
 
 # OpenObserve
-Biblioteka do wysyłania logów do OpenObserve
+A library for sending logs to OpenObserve
 
 ## Logi
-Logi błędów biblioteki oraz dla `global_exception_logger` to:
+Logs for library errors and for `global_exception_logger` are located at:
 ```bash
 cd /home/$USER/.openobserve/logs/log.log
 ```
 
-## Konfiguracja
+## Configuration
 ```python
 import openobserve
 openobserve.username = ''
 openobserve.password = ''
 openobserve.host = 'http://127.0.0.1:5080',
-openobserve.stream_global = 'default' #domyślny stream
-openobserve.organization_global = 'default' #domyślna organizacja
-openobserve.ssl_verify = False #weryfikacja ssl hosta
-openobserve.additional_info = False #dodatkowe dane
+openobserve.stream_global = 'default' #default stream
+openobserve.organization_global = 'default' #default organization
+openobserve.ssl_verify = False #SSL host verification
+openobserve.additional_info = False #additional data
 ```
 
-## Wysyłanie loga
-pola `_stream` oraz `_organization` nadpisują `stream_global` oraz `organization_global`
+## Sending a log
+Fields _stream and _organization override stream_global and organization_global
 ```python
 def send(
     job: Any = '',
     level: str = 'INFO',
     _stream: str = None,
     _organization: str = None,
     **kwargs
 )
 ```
-### Przykład
+### Example
 ```python
 import openobserve
 openobserve.send(job='test', _return_data=True,message='test message')
 ```
 Log:
 ```json
 {
     '_timestamp': '2024-03-25T20:10:47.106', 
     'level': 'INFO',
     'job': 'test', 
     'message': 'test message'
 }
 ```
 
-## Dodatkowe dane dla openovserver.additionalinfo
+## Additional data for openobserve.additionalinfo
 ```json
 {
     'hostname': socket.gethostname(),
     'user_name': socket.gethostname(),
     'system': platform.system(),
     'system_architecture': platform.machine(),
     'system_version': platform.version(),
     'system_release': platform.release(),
     'python_version': platform.python_version()
 }
 ```
 
-## Globalne zbieranie błędow
-Kod do globalnego zbierania błędów z projektu
+## Global error collection
+Code for globally collecting errors from the project
 ```python
 import openobserve.global_exception_logger
 
 print(1 / 0)
 ```
-W tym momencie log wysyła się na serwer oraz zapisuje na dysku
-### Konfiguracja
+At this point, the log is sent to the server and saved on disk
+### Configuration
 ```python
 import openobserve.global_exception_logger
 
 openobserve.global_exception_logger.organization_global = 'default'
 openobserve.global_exception_logger.stream_global = 'default'
 ```
```

### Comparing `openobserve-1.0.0/README.md` & `openobserve-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 # OpenObserve
-Biblioteka do wysyłania logów do OpenObserve
+A library for sending logs to OpenObserve
 
 ## Logi
-Logi błędów biblioteki oraz dla `global_exception_logger` to:
+Logs for library errors and for `global_exception_logger` are located at:
 ```bash
 cd /home/$USER/.openobserve/logs/log.log
 ```
 
-## Konfiguracja
+## Configuration
 ```python
 import openobserve
 openobserve.username = ''
 openobserve.password = ''
 openobserve.host = 'http://127.0.0.1:5080',
-openobserve.stream_global = 'default' #domyślny stream
-openobserve.organization_global = 'default' #domyślna organizacja
-openobserve.ssl_verify = False #weryfikacja ssl hosta
-openobserve.additional_info = False #dodatkowe dane
+openobserve.stream_global = 'default' #default stream
+openobserve.organization_global = 'default' #default organization
+openobserve.ssl_verify = False #SSL host verification
+openobserve.additional_info = False #additional data
 ```
 
-## Wysyłanie loga
-pola `_stream` oraz `_organization` nadpisują `stream_global` oraz `organization_global`
+## Sending a log
+Fields _stream and _organization override stream_global and organization_global
 ```python
 def send(
     job: Any = '',
     level: str = 'INFO',
     _stream: str = None,
     _organization: str = None,
     **kwargs
 )
 ```
-### Przykład
+### Example
 ```python
 import openobserve
 openobserve.send(job='test', _return_data=True,message='test message')
 ```
 Log:
 ```json
 {
     '_timestamp': '2024-03-25T20:10:47.106', 
     'level': 'INFO',
     'job': 'test', 
     'message': 'test message'
 }
 ```
 
-## Dodatkowe dane dla openovserver.additionalinfo
+## Additional data for openobserve.additionalinfo
 ```json
 {
     'hostname': socket.gethostname(),
     'user_name': socket.gethostname(),
     'system': platform.system(),
     'system_architecture': platform.machine(),
     'system_version': platform.version(),
     'system_release': platform.release(),
     'python_version': platform.python_version()
 }
 ```
 
-## Globalne zbieranie błędow
-Kod do globalnego zbierania błędów z projektu
+## Global error collection
+Code for globally collecting errors from the project
 ```python
 import openobserve.global_exception_logger
 
 print(1 / 0)
 ```
-W tym momencie log wysyła się na serwer oraz zapisuje na dysku
-### Konfiguracja
+At this point, the log is sent to the server and saved on disk
+### Configuration
 ```python
 import openobserve.global_exception_logger
 
 openobserve.global_exception_logger.organization_global = 'default'
 openobserve.global_exception_logger.stream_global = 'default'
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openobserve-1.0.0/openobserve/__init__.py` & `openobserve-1.0.1/openobserve/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import requests
 import logging
 import json
-import openobserve.validate
 import openobserve.generate
 from requests.auth import HTTPBasicAuth
 from typing import Any
 from jsonex import JsonEx
 
 username = ''
 password = ''
```

### Comparing `openobserve-1.0.0/openobserve/generate.py` & `openobserve-1.0.1/openobserve/generate.py`

 * *Files identical despite different names*

### Comparing `openobserve-1.0.0/openobserve/global_exception_logger.py` & `openobserve-1.0.1/openobserve/global_exception_logger.py`

 * *Files identical despite different names*

### Comparing `openobserve-1.0.0/openobserve.egg-info/PKG-INFO` & `openobserve-1.0.1/openobserve.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 Metadata-Version: 2.1
 Name: openobserve
-Version: 1.0.0
+Version: 1.0.1
 Summary: OpenObserve library
 Author: Krzysztof Żyłka
 Author-email: krzysztofzylka@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: jsonex
 
 # OpenObserve
-Biblioteka do wysyłania logów do OpenObserve
+A library for sending logs to OpenObserve
 
 ## Logi
-Logi błędów biblioteki oraz dla `global_exception_logger` to:
+Logs for library errors and for `global_exception_logger` are located at:
 ```bash
 cd /home/$USER/.openobserve/logs/log.log
 ```
 
-## Konfiguracja
+## Configuration
 ```python
 import openobserve
 openobserve.username = ''
 openobserve.password = ''
 openobserve.host = 'http://127.0.0.1:5080',
-openobserve.stream_global = 'default' #domyślny stream
-openobserve.organization_global = 'default' #domyślna organizacja
-openobserve.ssl_verify = False #weryfikacja ssl hosta
-openobserve.additional_info = False #dodatkowe dane
+openobserve.stream_global = 'default' #default stream
+openobserve.organization_global = 'default' #default organization
+openobserve.ssl_verify = False #SSL host verification
+openobserve.additional_info = False #additional data
 ```
 
-## Wysyłanie loga
-pola `_stream` oraz `_organization` nadpisują `stream_global` oraz `organization_global`
+## Sending a log
+Fields _stream and _organization override stream_global and organization_global
 ```python
 def send(
     job: Any = '',
     level: str = 'INFO',
     _stream: str = None,
     _organization: str = None,
     **kwargs
 )
 ```
-### Przykład
+### Example
 ```python
 import openobserve
 openobserve.send(job='test', _return_data=True,message='test message')
 ```
 Log:
 ```json
 {
     '_timestamp': '2024-03-25T20:10:47.106', 
     'level': 'INFO',
     'job': 'test', 
     'message': 'test message'
 }
 ```
 
-## Dodatkowe dane dla openovserver.additionalinfo
+## Additional data for openobserve.additionalinfo
 ```json
 {
     'hostname': socket.gethostname(),
     'user_name': socket.gethostname(),
     'system': platform.system(),
     'system_architecture': platform.machine(),
     'system_version': platform.version(),
     'system_release': platform.release(),
     'python_version': platform.python_version()
 }
 ```
 
-## Globalne zbieranie błędow
-Kod do globalnego zbierania błędów z projektu
+## Global error collection
+Code for globally collecting errors from the project
 ```python
 import openobserve.global_exception_logger
 
 print(1 / 0)
 ```
-W tym momencie log wysyła się na serwer oraz zapisuje na dysku
-### Konfiguracja
+At this point, the log is sent to the server and saved on disk
+### Configuration
 ```python
 import openobserve.global_exception_logger
 
 openobserve.global_exception_logger.organization_global = 'default'
 openobserve.global_exception_logger.stream_global = 'default'
 ```
```

### Comparing `openobserve-1.0.0/setup.py` & `openobserve-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='openobserve',
-    version='1.0.0',
+    version='1.0.1',
     description='OpenObserve library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Krzysztof Żyłka',
     author_email='krzysztofzylka@yahoo.com',
     install_requires=[
         'requests',
```

