# Comparing `tmp/lambkid-0.1.3.tar.gz` & `tmp/lambkid-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.1.3.tar", last modified: Mon Apr  8 02:27:12 2024, max compression
+gzip compressed data, was "lambkid-0.1.4.tar", last modified: Mon Apr  8 02:34:25 2024, max compression
```

## Comparing `lambkid-0.1.3.tar` & `lambkid-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 02:27:12.509691 lambkid-0.1.3/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1894 2024-04-08 02:27:12.507697 lambkid-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-04-01 08:32:16.000000 lambkid-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 02:27:12.490742 lambkid-0.1.3/docs/
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.1.3/docs/install.md
--rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.1.3/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.1.3/docs/sshclient.md
-drwxrwxrwx   0        0        0        0 2024-04-08 02:27:12.492736 lambkid-0.1.3/lambkid/
--rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.1.3/lambkid/__init__.py
--rw-rw-rw-   0        0        0      185 2024-04-08 02:20:24.000000 lambkid-0.1.3/lambkid/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:27:12.505730 lambkid-0.1.3/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.1.3/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1406 2024-04-07 15:19:33.000000 lambkid-0.1.3/lambkid/libs/log.py
--rw-rw-rw-   0        0        0     1242 2024-04-08 02:04:32.000000 lambkid-0.1.3/lambkid/libs/minio_client.py
--rw-rw-rw-   0        0        0     6886 2024-04-02 06:59:39.000000 lambkid-0.1.3/lambkid/libs/ssh.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:27:12.506699 lambkid-0.1.3/lambkid.egg-info/
--rw-rw-rw-   0        0        0     1894 2024-04-08 02:27:12.000000 lambkid-0.1.3/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-04-08 02:27:12.000000 lambkid-0.1.3/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 02:27:12.000000 lambkid-0.1.3/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-08 02:27:12.000000 lambkid-0.1.3/lambkid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-08 02:27:12.000000 lambkid-0.1.3/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 02:27:12.000000 lambkid-0.1.3/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 02:27:12.509691 lambkid-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1827 2024-04-08 02:27:07.000000 lambkid-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:34:25.879036 lambkid-0.1.4/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1894 2024-04-08 02:34:25.877041 lambkid-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-04-01 08:32:16.000000 lambkid-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 02:34:25.849115 lambkid-0.1.4/docs/
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.1.4/docs/install.md
+-rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.1.4/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.1.4/docs/sshclient.md
+drwxrwxrwx   0        0        0        0 2024-04-08 02:34:25.851110 lambkid-0.1.4/lambkid/
+-rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.1.4/lambkid/__init__.py
+-rw-rw-rw-   0        0        0      103 2024-04-08 02:34:11.000000 lambkid-0.1.4/lambkid/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:34:25.874049 lambkid-0.1.4/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.1.4/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1406 2024-04-07 15:19:33.000000 lambkid-0.1.4/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0     1242 2024-04-08 02:34:11.000000 lambkid-0.1.4/lambkid/libs/minio_client.py
+-rw-rw-rw-   0        0        0     6886 2024-04-02 06:59:39.000000 lambkid-0.1.4/lambkid/libs/ssh.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:34:25.876043 lambkid-0.1.4/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     1894 2024-04-08 02:34:25.000000 lambkid-0.1.4/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-08 02:34:25.000000 lambkid-0.1.4/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:34:25.000000 lambkid-0.1.4/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-08 02:34:25.000000 lambkid-0.1.4/lambkid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-08 02:34:25.000000 lambkid-0.1.4/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 02:34:25.000000 lambkid-0.1.4/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 02:34:25.879036 lambkid-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1822 2024-04-08 02:34:19.000000 lambkid-0.1.4/setup.py
```

### Comparing `lambkid-0.1.3/LICENSE` & `lambkid-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.3/PKG-INFO` & `lambkid-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.3
+Version: 0.1.4
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.1.3/README.md` & `lambkid-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.3/docs/log.md` & `lambkid-0.1.4/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.3/docs/sshclient.md` & `lambkid-0.1.4/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.3/lambkid/libs/log.py` & `lambkid-0.1.4/lambkid/libs/log.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.3/lambkid/libs/minio_client.py` & `lambkid-0.1.4/lambkid/libs/minio_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from minio import Minio
 from lambkid import log
 
-class MinIO:
+class minio:
     def upload_file(username,minio_url,access_key,secret_key,bucket_name,object_name,file_path,content_type="text/plain;charset=utf-8"):
         """
         upload file to minio server
         :param minio_url:  url of minio server
         :param access_key:  access key
         :param scret_key:  secret key
         :param bucket_name:  bucket name
```

### Comparing `lambkid-0.1.3/lambkid/libs/ssh.py` & `lambkid-0.1.4/lambkid/libs/ssh.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.3/lambkid.egg-info/PKG-INFO` & `lambkid-0.1.4/lambkid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.3
+Version: 0.1.4
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.1.3/setup.py` & `lambkid-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         long_desc=f.read()
 except:
     long_desc=""
 
 
 setup(
     name="lambkid",
-    version="0.1.3",
+    version="0.1.4",
     description="lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
@@ -29,15 +29,15 @@
         "paramiko",
         "fire"
     ],
     include_package_data=True,
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'lambkid=lambkid.cli:main'
+            'lambkid=lambkid.cli'
         ],
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: System :: Logging',
         'License :: OSI Approved :: MIT License',
```

