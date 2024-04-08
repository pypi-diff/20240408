# Comparing `tmp/meldrx_fhir_client-0.0.6.tar.gz` & `tmp/meldrx_fhir_client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meldrx_fhir_client-0.0.6.tar", last modified: Tue Mar 19 20:42:27 2024, max compression
+gzip compressed data, was "meldrx_fhir_client-0.0.8.tar", last modified: Mon Apr  8 12:54:10 2024, max compression
```

## Comparing `meldrx_fhir_client-0.0.6.tar` & `meldrx_fhir_client-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ericmorgan   (501) staff       (20)        0 2024-03-19 20:42:27.963865 meldrx_fhir_client-0.0.6/
--rw-r--r--   0 ericmorgan   (501) staff       (20)     1080 2024-03-19 20:42:27.963712 meldrx_fhir_client-0.0.6/PKG-INFO
--rw-r--r--   0 ericmorgan   (501) staff       (20)      438 2024-02-23 15:53:10.000000 meldrx_fhir_client-0.0.6/README.md
-drwxr-xr-x   0 ericmorgan   (501) staff       (20)        0 2024-03-19 20:42:27.961867 meldrx_fhir_client-0.0.6/meldrx_fhir_client/
--rw-r--r--   0 ericmorgan   (501) staff       (20)     4084 2024-03-19 20:42:01.000000 meldrx_fhir_client-0.0.6/meldrx_fhir_client/FHIRClient.py
--rw-r--r--   0 ericmorgan   (501) staff       (20)       34 2024-02-23 14:35:05.000000 meldrx_fhir_client-0.0.6/meldrx_fhir_client/__init__.py
-drwxr-xr-x   0 ericmorgan   (501) staff       (20)        0 2024-03-19 20:42:27.963031 meldrx_fhir_client-0.0.6/meldrx_fhir_client.egg-info/
--rw-r--r--   0 ericmorgan   (501) staff       (20)     1080 2024-03-19 20:42:27.000000 meldrx_fhir_client-0.0.6/meldrx_fhir_client.egg-info/PKG-INFO
--rw-r--r--   0 ericmorgan   (501) staff       (20)      293 2024-03-19 20:42:27.000000 meldrx_fhir_client-0.0.6/meldrx_fhir_client.egg-info/SOURCES.txt
--rw-r--r--   0 ericmorgan   (501) staff       (20)        1 2024-03-19 20:42:27.000000 meldrx_fhir_client-0.0.6/meldrx_fhir_client.egg-info/dependency_links.txt
--rw-r--r--   0 ericmorgan   (501) staff       (20)       25 2024-03-19 20:42:27.000000 meldrx_fhir_client-0.0.6/meldrx_fhir_client.egg-info/top_level.txt
--rw-r--r--   0 ericmorgan   (501) staff       (20)       38 2024-03-19 20:42:27.963904 meldrx_fhir_client-0.0.6/setup.cfg
--rw-r--r--   0 ericmorgan   (501) staff       (20)      896 2024-03-19 20:42:13.000000 meldrx_fhir_client-0.0.6/setup.py
-drwxr-xr-x   0 ericmorgan   (501) staff       (20)        0 2024-03-19 20:42:27.963436 meldrx_fhir_client-0.0.6/tests/
--rw-r--r--   0 ericmorgan   (501) staff       (20)        0 2024-02-23 14:47:05.000000 meldrx_fhir_client-0.0.6/tests/__init__.py
--rw-r--r--   0 ericmorgan   (501) staff       (20)     2666 2024-03-19 20:02:22.000000 meldrx_fhir_client-0.0.6/tests/test_FHIRClient.py
+drwxr-xr-x   0 ericmorgan   (501) staff       (20)        0 2024-04-08 12:54:10.712206 meldrx_fhir_client-0.0.8/
+-rw-r--r--   0 ericmorgan   (501) staff       (20)     1080 2024-04-08 12:54:10.712080 meldrx_fhir_client-0.0.8/PKG-INFO
+-rw-r--r--   0 ericmorgan   (501) staff       (20)      438 2024-02-23 15:53:10.000000 meldrx_fhir_client-0.0.8/README.md
+drwxr-xr-x   0 ericmorgan   (501) staff       (20)        0 2024-04-08 12:54:10.710952 meldrx_fhir_client-0.0.8/meldrx_fhir_client/
+-rw-r--r--   0 ericmorgan   (501) staff       (20)     4078 2024-04-04 14:28:36.000000 meldrx_fhir_client-0.0.8/meldrx_fhir_client/FHIRClient.py
+-rw-r--r--   0 ericmorgan   (501) staff       (20)       34 2024-02-23 14:35:05.000000 meldrx_fhir_client-0.0.8/meldrx_fhir_client/__init__.py
+drwxr-xr-x   0 ericmorgan   (501) staff       (20)        0 2024-04-08 12:54:10.711550 meldrx_fhir_client-0.0.8/meldrx_fhir_client.egg-info/
+-rw-r--r--   0 ericmorgan   (501) staff       (20)     1080 2024-04-08 12:54:10.000000 meldrx_fhir_client-0.0.8/meldrx_fhir_client.egg-info/PKG-INFO
+-rw-r--r--   0 ericmorgan   (501) staff       (20)      293 2024-04-08 12:54:10.000000 meldrx_fhir_client-0.0.8/meldrx_fhir_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ericmorgan   (501) staff       (20)        1 2024-04-08 12:54:10.000000 meldrx_fhir_client-0.0.8/meldrx_fhir_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ericmorgan   (501) staff       (20)       25 2024-04-08 12:54:10.000000 meldrx_fhir_client-0.0.8/meldrx_fhir_client.egg-info/top_level.txt
+-rw-r--r--   0 ericmorgan   (501) staff       (20)       38 2024-04-08 12:54:10.712258 meldrx_fhir_client-0.0.8/setup.cfg
+-rw-r--r--   0 ericmorgan   (501) staff       (20)      896 2024-04-08 12:54:01.000000 meldrx_fhir_client-0.0.8/setup.py
+drwxr-xr-x   0 ericmorgan   (501) staff       (20)        0 2024-04-08 12:54:10.711772 meldrx_fhir_client-0.0.8/tests/
+-rw-r--r--   0 ericmorgan   (501) staff       (20)        0 2024-02-23 14:47:05.000000 meldrx_fhir_client-0.0.8/tests/__init__.py
+-rw-r--r--   0 ericmorgan   (501) staff       (20)     2666 2024-03-19 20:02:22.000000 meldrx_fhir_client-0.0.8/tests/test_FHIRClient.py
```

### Comparing `meldrx_fhir_client-0.0.6/PKG-INFO` & `meldrx_fhir_client-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meldrx_fhir_client
-Version: 0.0.6
+Version: 0.0.8
 Summary: A simple FHIR client for MeldRX.
 Home-page: https://github.com/darena-solutions/meldrx-client-py
 Author: EM
 Author-email: eric@darenasolutions.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `meldrx_fhir_client-0.0.6/meldrx_fhir_client/FHIRClient.py` & `meldrx_fhir_client-0.0.8/meldrx_fhir_client/FHIRClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         access_token = base64.b64encode(access_token.encode('utf-8')).decode('utf-8')
         return FHIRClient(base_url, access_token, "Basic")
 
     # Initialize the FHIRClient with a client secret...
     @staticmethod
     def for_client_secret(meldrx_base_url, workspace_id, client_id, client_secret, scope):
         token_url = meldrx_base_url + '/' + workspace_id + '/connect/token'
-        fhir_url = meldrx_base_url + '/api/meldrxfhir/' + workspace_id
+        fhir_url = meldrx_base_url + '/api/fhir/' + workspace_id
 
         # Do a client secret post to get an access token...
         data = {
             'grant_type': 'client_credentials',
             'scope': scope,
         }
         headers = {
```

### Comparing `meldrx_fhir_client-0.0.6/meldrx_fhir_client.egg-info/PKG-INFO` & `meldrx_fhir_client-0.0.8/meldrx_fhir_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meldrx-fhir-client
-Version: 0.0.6
+Version: 0.0.8
 Summary: A simple FHIR client for MeldRX.
 Home-page: https://github.com/darena-solutions/meldrx-client-py
 Author: EM
 Author-email: eric@darenasolutions.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `meldrx_fhir_client-0.0.6/setup.py` & `meldrx_fhir_client-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 setup(
     name='meldrx_fhir_client',
     description='A simple FHIR client for MeldRX.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/darena-solutions/meldrx-client-py',
-    version='0.0.6',
+    version='0.0.8',
     author='EM',
     author_email='eric@darenasolutions.com',
     packages=find_packages(),
     install_requires=[],
     tests_require=['pytest'],
     test_suite='tests',
     classifiers=[
```

### Comparing `meldrx_fhir_client-0.0.6/tests/test_FHIRClient.py` & `meldrx_fhir_client-0.0.8/tests/test_FHIRClient.py`

 * *Files identical despite different names*

