# Comparing `tmp/prodpadlm_client-0.1.1.2.tar.gz` & `tmp/prodpadlm_client-0.1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodpadlm_client-0.1.1.2.tar", last modified: Mon Apr  8 07:50:05 2024, max compression
+gzip compressed data, was "prodpadlm_client-0.1.1.3.tar", last modified: Mon Apr  8 08:02:03 2024, max compression
```

## Comparing `prodpadlm_client-0.1.1.2.tar` & `prodpadlm_client-0.1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 07:50:05.430399 prodpadlm_client-0.1.1.2/
--rw-rw-rw-   0        0        0     1725 2024-04-08 07:50:05.429394 prodpadlm_client-0.1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1413 2024-04-08 07:39:29.000000 prodpadlm_client-0.1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 07:50:05.408808 prodpadlm_client-0.1.1.2/prodpadlm_client/
--rw-rw-rw-   0        0        0       49 2024-04-08 07:45:30.000000 prodpadlm_client-0.1.1.2/prodpadlm_client/__init__.py
--rw-rw-rw-   0        0        0    10761 2024-04-08 07:45:56.000000 prodpadlm_client-0.1.1.2/prodpadlm_client/client.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:50:05.428115 prodpadlm_client-0.1.1.2/prodpadlm_client/resources/
--rw-rw-rw-   0        0        0        0 2024-04-08 07:47:58.000000 prodpadlm_client-0.1.1.2/prodpadlm_client/resources/__init__.py
--rw-rw-rw-   0        0        0     2801 2024-04-08 01:16:13.000000 prodpadlm_client-0.1.1.2/prodpadlm_client/resources/api.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:50:05.425973 prodpadlm_client-0.1.1.2/prodpadlm_client.egg-info/
--rw-rw-rw-   0        0        0     1725 2024-04-08 07:50:04.000000 prodpadlm_client-0.1.1.2/prodpadlm_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-04-08 07:50:05.000000 prodpadlm_client-0.1.1.2/prodpadlm_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 07:50:04.000000 prodpadlm_client-0.1.1.2/prodpadlm_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-08 07:50:04.000000 prodpadlm_client-0.1.1.2/prodpadlm_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-08 07:50:04.000000 prodpadlm_client-0.1.1.2/prodpadlm_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 07:50:05.430399 prodpadlm_client-0.1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      893 2024-04-08 07:49:39.000000 prodpadlm_client-0.1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 08:02:03.383259 prodpadlm_client-0.1.1.3/
+-rw-rw-rw-   0        0        0     1725 2024-04-08 08:02:03.379259 prodpadlm_client-0.1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1413 2024-04-08 07:39:29.000000 prodpadlm_client-0.1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 08:02:03.274857 prodpadlm_client-0.1.1.3/prodpadlm_client/
+-rw-rw-rw-   0        0        0       49 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.3/prodpadlm_client/__init__.py
+-rw-rw-rw-   0        0        0    10761 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.3/prodpadlm_client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-08 08:02:03.377260 prodpadlm_client-0.1.1.3/prodpadlm_client/resources/
+-rw-rw-rw-   0        0        0        0 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.3/prodpadlm_client/resources/__init__.py
+-rw-rw-rw-   0        0        0     2814 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.3/prodpadlm_client/resources/api.py
+drwxrwxrwx   0        0        0        0 2024-04-08 08:02:03.353244 prodpadlm_client-0.1.1.3/prodpadlm_client.egg-info/
+-rw-rw-rw-   0        0        0     1725 2024-04-08 08:02:02.000000 prodpadlm_client-0.1.1.3/prodpadlm_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-04-08 08:02:02.000000 prodpadlm_client-0.1.1.3/prodpadlm_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 08:02:02.000000 prodpadlm_client-0.1.1.3/prodpadlm_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-08 08:02:02.000000 prodpadlm_client-0.1.1.3/prodpadlm_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-08 08:02:02.000000 prodpadlm_client-0.1.1.3/prodpadlm_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 08:02:03.383259 prodpadlm_client-0.1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      893 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.3/setup.py
```

### Comparing `prodpadlm_client-0.1.1.2/PKG-INFO` & `prodpadlm_client-0.1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodpadlm_client
-Version: 0.1.1.2
+Version: 0.1.1.3
 Summary: Production LaunchPad for Language Models [Client] - ⚡ Ship Open Source LLMs to production faster and efficiently ⚡
 Author: Ayo Kehinde Samuel
 License: Apache 2.0
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 
 # ProdPadLM - Client
```

### Comparing `prodpadlm_client-0.1.1.2/README.md` & `prodpadlm_client-0.1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.2/prodpadlm_client/client.py` & `prodpadlm_client-0.1.1.3/prodpadlm_client/client.py`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.2/prodpadlm_client/resources/api.py` & `prodpadlm_client-0.1.1.3/prodpadlm_client/resources/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Iterable, List, Literal, Optional, Required, TypedDict, Union
+from typing import Iterable, List
 import httpx
+from typing_extensions import Literal, Required, TypedDict
 
 from prodpadlm_client.client_types.messages import Message
 
 # default timeout is 10 minutes
 DEFAULT_TIMEOUT = httpx.Timeout(timeout=600.0, connect=5.0)
 DEFAULT_MAX_RETRIES = 2
 DEFAULT_CONNECTION_LIMITS = httpx.Limits(max_connections=1000, max_keepalive_connections=100)
```

### Comparing `prodpadlm_client-0.1.1.2/prodpadlm_client.egg-info/PKG-INFO` & `prodpadlm_client-0.1.1.3/prodpadlm_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodpadlm-client
-Version: 0.1.1.2
+Version: 0.1.1.3
 Summary: Production LaunchPad for Language Models [Client] - ⚡ Ship Open Source LLMs to production faster and efficiently ⚡
 Author: Ayo Kehinde Samuel
 License: Apache 2.0
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 
 # ProdPadLM - Client
```

### Comparing `prodpadlm_client-0.1.1.2/setup.py` & `prodpadlm_client-0.1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "pydantic-settings",
     "langchain==0.1.14",
     "langchain-core==0.1.40",
 ]
 
 setup(
     name='prodpadlm_client',
-    version='0.1.1.2',
+    version='0.1.1.3',
     description='Production LaunchPad for Language Models [Client] - ⚡ Ship Open Source LLMs to production faster and efficiently ⚡',
     author='Ayo Kehinde Samuel',
     packages=find_packages(),
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     license="Apache 2.0",
     license_files="LICENSE.txt",
```

