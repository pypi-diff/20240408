# Comparing `tmp/lambkid-0.1.0.tar.gz` & `tmp/lambkid-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.1.0.tar", last modified: Sun Apr  7 15:21:48 2024, max compression
+gzip compressed data, was "lambkid-0.1.1.tar", last modified: Mon Apr  8 02:07:14 2024, max compression
```

## Comparing `lambkid-0.1.0.tar` & `lambkid-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 15:21:48.319026 lambkid-0.1.0/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1873 2024-04-07 15:21:48.317031 lambkid-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-04-01 08:32:16.000000 lambkid-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 15:21:48.282153 lambkid-0.1.0/docs/
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.1.0/docs/install.md
--rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.1.0/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.1.0/docs/sshclient.md
-drwxrwxrwx   0        0        0        0 2024-04-07 15:21:48.290104 lambkid-0.1.0/lambkid/
--rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.1.0/lambkid/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:21:48.306062 lambkid-0.1.0/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.1.0/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1406 2024-04-07 15:19:33.000000 lambkid-0.1.0/lambkid/libs/log.py
--rw-rw-rw-   0        0        0     6886 2024-04-02 06:59:39.000000 lambkid-0.1.0/lambkid/libs/ssh.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:21:48.315037 lambkid-0.1.0/lambkid.egg-info/
--rw-rw-rw-   0        0        0     1873 2024-04-07 15:21:48.000000 lambkid-0.1.0/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-07 15:21:48.000000 lambkid-0.1.0/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 15:21:48.000000 lambkid-0.1.0/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-07 15:21:48.000000 lambkid-0.1.0/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-07 15:21:48.000000 lambkid-0.1.0/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 15:21:48.320023 lambkid-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1700 2024-04-07 15:21:05.000000 lambkid-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:07:14.191539 lambkid-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1894 2024-04-08 02:07:14.189545 lambkid-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-04-01 08:32:16.000000 lambkid-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 02:07:14.149651 lambkid-0.1.1/docs/
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.1.1/docs/install.md
+-rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.1.1/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.1.1/docs/sshclient.md
+drwxrwxrwx   0        0        0        0 2024-04-08 02:07:14.153640 lambkid-0.1.1/lambkid/
+-rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.1.1/lambkid/__init__.py
+-rw-rw-rw-   0        0        0      112 2024-04-08 02:06:13.000000 lambkid-0.1.1/lambkid/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:07:14.178599 lambkid-0.1.1/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.1.1/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1406 2024-04-07 15:19:33.000000 lambkid-0.1.1/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0     1242 2024-04-08 02:04:32.000000 lambkid-0.1.1/lambkid/libs/minio_client.py
+-rw-rw-rw-   0        0        0     6886 2024-04-02 06:59:39.000000 lambkid-0.1.1/lambkid/libs/ssh.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:07:14.188546 lambkid-0.1.1/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     1894 2024-04-08 02:07:14.000000 lambkid-0.1.1/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-08 02:07:14.000000 lambkid-0.1.1/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:07:14.000000 lambkid-0.1.1/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-08 02:07:14.000000 lambkid-0.1.1/lambkid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-08 02:07:14.000000 lambkid-0.1.1/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 02:07:14.000000 lambkid-0.1.1/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 02:07:14.191539 lambkid-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1830 2024-04-08 02:06:42.000000 lambkid-0.1.1/setup.py
```

### Comparing `lambkid-0.1.0/LICENSE` & `lambkid-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.0/PKG-INFO` & `lambkid-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.0
+Version: 0.1.1
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: concurrent_log_handler
 Requires-Dist: paramiko
+Requires-Dist: fire
 
 # lambkid
 
 lambkid is an advance lib abstract from some common use python lib. it aim to supply a more easily and more fewer code for python developer.
 it will practise for life is short and I will choose python.
 
 ## install lambkid
```

### Comparing `lambkid-0.1.0/README.md` & `lambkid-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.0/docs/log.md` & `lambkid-0.1.1/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.0/docs/sshclient.md` & `lambkid-0.1.1/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.0/lambkid/libs/log.py` & `lambkid-0.1.1/lambkid/libs/log.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.0/lambkid/libs/ssh.py` & `lambkid-0.1.1/lambkid/libs/ssh.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.0/lambkid.egg-info/PKG-INFO` & `lambkid-0.1.1/lambkid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.0
+Version: 0.1.1
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: concurrent_log_handler
 Requires-Dist: paramiko
+Requires-Dist: fire
 
 # lambkid
 
 lambkid is an advance lib abstract from some common use python lib. it aim to supply a more easily and more fewer code for python developer.
 it will practise for life is short and I will choose python.
 
 ## install lambkid
```

### Comparing `lambkid-0.1.0/setup.py` & `lambkid-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,32 +7,39 @@
         long_desc=f.read()
 except:
     long_desc=""
 
 
 setup(
     name="lambkid",
-    version="0.1.0",
+    version="0.1.1",
     description="lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
     url="https://github.com/redrose2100/lambkid",
     project_urls={
         "Documentation": "https://github.com/redrose2100/lambkid/blob/master/README.md"
     },
     license="MIT",
     install_requires =[
         "concurrent_log_handler",
-        "paramiko"
+        "paramiko",
+        "fire"
     ],
     include_package_data=True,
+    packages=find_packages(),
+    entry_points={
+        'console_scripts': [
+            'lambkid = lambkid.cli:main',
+        ],
+    },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: System :: Logging',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
@@ -41,10 +48,9 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12'
-    ],
-    packages=find_packages()
+    ]
 )
```

