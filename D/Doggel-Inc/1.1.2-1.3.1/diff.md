# Comparing `tmp/Doggel-Inc-1.1.2.tar.gz` & `tmp/Doggel_Inc-1.3.1.tar.gz`

## Comparing `Doggel-Inc-1.1.2.tar` & `Doggel_Inc-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,24 @@
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)      651 2023-12-02 16:35:37.000000 Doggel_Inc/AI/AI.py
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)      147 2023-12-02 16:33:35.000000 Doggel_Inc/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)     1689 2023-12-02 16:36:29.000000 Doggel_Inc/__pycache__/AI.cpython-311.pyc
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)      987 2023-12-02 16:46:01.000000 Doggel-Inc-1.1.2/setup.py
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)        1 2023-12-02 17:01:29.000000 Doggel-Inc-1.1.2/Doggel_Inc.egg-info/top_level.txt
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)      185 2023-12-02 17:01:29.000000 Doggel-Inc-1.1.2/Doggel_Inc.egg-info/SOURCES.txt
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)        1 2023-12-02 17:01:29.000000 Doggel-Inc-1.1.2/Doggel_Inc.egg-info/dependency_links.txt
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)      735 2023-12-02 17:01:29.000000 Doggel-Inc-1.1.2/Doggel_Inc.egg-info/PKG-INFO
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)        8 2023-12-02 17:01:29.000000 Doggel-Inc-1.1.2/Doggel_Inc.egg-info/requires.txt
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)      735 2023-12-02 17:01:30.000000 Doggel-Inc-1.1.2/PKG-INFO
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)     1270 2023-12-02 16:44:26.000000 Doggel-Inc-1.1.2/LICENSE
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (997)       38 2023-12-02 17:01:30.000000 Doggel-Inc-1.1.2/setup.cfg
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      700 2024-04-08 21:08:55.000000 Doggel_Inc-1.3.1/PKG-INFO
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)       38 2024-04-08 21:08:55.000000 Doggel_Inc-1.3.1/setup.cfg
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      700 2024-04-08 21:08:54.000000 Doggel_Inc-1.3.1/Doggel_Inc.egg-info/PKG-INFO
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      184 2024-04-08 21:08:54.000000 Doggel_Inc-1.3.1/Doggel_Inc.egg-info/SOURCES.txt
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)        1 2024-04-08 21:08:54.000000 Doggel_Inc-1.3.1/Doggel_Inc.egg-info/dependency_links.txt
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)       19 2024-04-08 21:08:54.000000 Doggel_Inc-1.3.1/Doggel_Inc.egg-info/requires.txt
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)        1 2024-04-08 21:08:54.000000 Doggel_Inc-1.3.1/Doggel_Inc.egg-info/top_level.txt
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      913 2024-04-08 21:06:41.000000 Doggel_Inc-1.3.1/setup.py
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)       41 2024-04-08 21:06:57.000000 Doggel_Inc-1.3.1/README
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      147 2023-12-02 16:33:35.000000 Doggel_Inc/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     1689 2023-12-02 16:36:29.000000 Doggel_Inc/__pycache__/AI.cpython-311.pyc
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     3290 2024-04-08 20:28:43.000000 Doggel_Inc/DICord/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     1627 2024-04-08 20:28:43.000000 Doggel_Inc/DICord/__pycache__/channel.cpython-311.pyc
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     1222 2024-04-08 18:02:11.000000 Doggel_Inc/DICord/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     8294 2024-04-08 20:50:07.000000 Doggel_Inc/DICord/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     1521 2024-04-08 18:35:42.000000 Doggel_Inc/DICord/__pycache__/msg.cpython-311.pyc
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      708 2024-04-08 16:28:26.000000 Doggel_Inc/DICord/__pycache__/transformer.cpython-311.pyc
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     1370 2024-04-08 20:28:29.000000 Doggel_Inc/DICord/user.py
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     3509 2024-04-08 20:49:57.000000 Doggel_Inc/DICord/__init__.py
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      398 2024-04-08 18:00:53.000000 Doggel_Inc/DICord/message.py
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      136 2024-04-08 16:12:02.000000 Doggel_Inc/DICord/transformer.py
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      502 2024-04-08 18:35:06.000000 Doggel_Inc/DICord/msg.py
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      619 2024-04-08 20:28:08.000000 Doggel_Inc/DICord/channel.py
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      647 2024-04-07 17:11:43.000000 Doggel_Inc/AI/AI.py
```

### Doggel_Inc/AI/AI.py

```diff
@@ -7,12 +7,12 @@
     apikey = key
 
 async def request(user_id, user_name, message):
     
     global apikey
     request_headers = {'Authorization': apikey}
     async with aiohttp.ClientSession() as session:                                     
-        api_url = 'http://us3.techstar.host:55565/request'
+        api_url = 'https://diai.doggelinc.site/request'
         request_data = {'message': message,'message-author-id': user_id,'message-author-user': user_name,'function': "ai"}
         async with session.post(api_url, json=request_data, headers=request_headers) as response:
             api_response = await response.json()
-            return api_response
+            return api_response
```

### Comparing `Doggel-Inc-1.1.2/setup.py` & `Doggel_Inc-1.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='Doggel-Inc',  # Replace with your package name
-    version='1.1.2',  # Replace with your package version
-    description='Doggeł Inc AI package for request to make ppls life easier',
+    name='Doggel_Inc', 
+    version='1.3.1', 
+    description='Doggeł Inc packages',
     author='Lordpomind',
     author_email='lordpomind@gmail.com',
     url='',  
+    package_data={
+        'Doggel_Inc': ["src/*"]
+    },
     packages=find_packages(),  
-    install_requires=[  # List your package dependencies here
-        'aiohttp'      
+    install_requires=[  
+        'aiohttp', 'websockets'      
     ],
     classifiers=[  
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',        
         'Programming Language :: Python :: 3.10',        
         'Programming Language :: Python :: 3.11',
     ],
-)
+)
```

### Comparing `Doggel-Inc-1.1.2/Doggel_Inc.egg-info/PKG-INFO` & `Doggel_Inc-1.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
-Name: Doggel-Inc
-Version: 1.1.2
-Summary: Doggeł Inc AI package for request to make ppls life easier
+Name: Doggel_Inc
+Version: 1.3.1
+Summary: Doggeł Inc packages
 Home-page: 
 Author: Lordpomind
 Author-email: lordpomind@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE
 Requires-Dist: aiohttp
+Requires-Dist: websockets
```

### Comparing `Doggel-Inc-1.1.2/PKG-INFO` & `Doggel_Inc-1.3.1/Doggel_Inc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
-Name: Doggel-Inc
-Version: 1.1.2
-Summary: Doggeł Inc AI package for request to make ppls life easier
+Name: Doggel_Inc
+Version: 1.3.1
+Summary: Doggeł Inc packages
 Home-page: 
 Author: Lordpomind
 Author-email: lordpomind@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE
 Requires-Dist: aiohttp
+Requires-Dist: websockets
```

