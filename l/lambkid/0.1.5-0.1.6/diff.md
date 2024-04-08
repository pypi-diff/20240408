# Comparing `tmp/lambkid-0.1.5.tar.gz` & `tmp/lambkid-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.1.5.tar", last modified: Mon Apr  8 03:31:29 2024, max compression
+gzip compressed data, was "lambkid-0.1.6.tar", last modified: Mon Apr  8 03:33:20 2024, max compression
```

## Comparing `lambkid-0.1.5.tar` & `lambkid-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 03:31:29.107018 lambkid-0.1.5/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1894 2024-04-08 03:31:29.106021 lambkid-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-04-01 08:32:16.000000 lambkid-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 03:31:29.089066 lambkid-0.1.5/docs/
--rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.1.5/docs/cli.md
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.1.5/docs/install.md
--rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.1.5/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.1.5/docs/sshclient.md
-drwxrwxrwx   0        0        0        0 2024-04-08 03:31:29.091060 lambkid-0.1.5/lambkid/
--rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.1.5/lambkid/__init__.py
--rw-rw-rw-   0        0        0      847 2024-04-08 03:27:19.000000 lambkid-0.1.5/lambkid/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:31:29.103028 lambkid-0.1.5/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.1.5/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1406 2024-04-07 15:19:33.000000 lambkid-0.1.5/lambkid/libs/log.py
--rw-rw-rw-   0        0        0      825 2024-04-08 02:45:19.000000 lambkid-0.1.5/lambkid/libs/minio_client.py
--rw-rw-rw-   0        0        0     6886 2024-04-02 06:59:39.000000 lambkid-0.1.5/lambkid/libs/ssh.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:31:29.105023 lambkid-0.1.5/lambkid.egg-info/
--rw-rw-rw-   0        0        0     1894 2024-04-08 03:31:29.000000 lambkid-0.1.5/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-04-08 03:31:29.000000 lambkid-0.1.5/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 03:31:29.000000 lambkid-0.1.5/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-08 03:31:29.000000 lambkid-0.1.5/lambkid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-08 03:31:29.000000 lambkid-0.1.5/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 03:31:29.000000 lambkid-0.1.5/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 03:31:29.107018 lambkid-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1822 2024-04-08 03:31:26.000000 lambkid-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:33:20.354258 lambkid-0.1.6/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1894 2024-04-08 03:33:20.353261 lambkid-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-04-01 08:32:16.000000 lambkid-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 03:33:20.336306 lambkid-0.1.6/docs/
+-rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.1.6/docs/cli.md
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.1.6/docs/install.md
+-rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.1.6/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.1.6/docs/sshclient.md
+drwxrwxrwx   0        0        0        0 2024-04-08 03:33:20.338301 lambkid-0.1.6/lambkid/
+-rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.1.6/lambkid/__init__.py
+-rw-rw-rw-   0        0        0      874 2024-04-08 03:33:14.000000 lambkid-0.1.6/lambkid/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:33:20.351266 lambkid-0.1.6/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.1.6/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1406 2024-04-07 15:19:33.000000 lambkid-0.1.6/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0      825 2024-04-08 02:45:19.000000 lambkid-0.1.6/lambkid/libs/minio_client.py
+-rw-rw-rw-   0        0        0     6886 2024-04-02 06:59:39.000000 lambkid-0.1.6/lambkid/libs/ssh.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:33:20.352264 lambkid-0.1.6/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     1894 2024-04-08 03:33:20.000000 lambkid-0.1.6/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-04-08 03:33:20.000000 lambkid-0.1.6/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 03:33:20.000000 lambkid-0.1.6/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-08 03:33:20.000000 lambkid-0.1.6/lambkid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-08 03:33:20.000000 lambkid-0.1.6/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 03:33:20.000000 lambkid-0.1.6/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 03:33:20.354258 lambkid-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1822 2024-04-08 03:33:14.000000 lambkid-0.1.6/setup.py
```

### Comparing `lambkid-0.1.5/LICENSE` & `lambkid-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.5/PKG-INFO` & `lambkid-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.5
+Version: 0.1.6
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.1.5/README.md` & `lambkid-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.5/docs/log.md` & `lambkid-0.1.6/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.5/docs/sshclient.md` & `lambkid-0.1.6/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.5/lambkid/cli.py` & `lambkid-0.1.6/lambkid/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,13 +13,16 @@
         :param file_path:  file path to upload
         :param content_type:  content typek, default text/plain;charset=utf-8
         :return:
         """
         return MinIO().upload_file(minio_url,access_key,secret_key,bucket_name,object_name,file_path,content_type)
 
 
-if __name__=="__main__":
+def main():
     fire.Fire(
         {
             "minio": minio
         }
-    )
+    )
+
+if __name__=="__main__":
+    main()
```

### Comparing `lambkid-0.1.5/lambkid/libs/log.py` & `lambkid-0.1.6/lambkid/libs/log.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.5/lambkid/libs/minio_client.py` & `lambkid-0.1.6/lambkid/libs/minio_client.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.5/lambkid/libs/ssh.py` & `lambkid-0.1.6/lambkid/libs/ssh.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.5/lambkid.egg-info/PKG-INFO` & `lambkid-0.1.6/lambkid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.5
+Version: 0.1.6
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.1.5/setup.py` & `lambkid-0.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         long_desc=f.read()
 except:
     long_desc=""
 
 
 setup(
     name="lambkid",
-    version="0.1.5",
+    version="0.1.6",
     description="lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
```

