# Comparing `tmp/gpp_components-0.0.8.tar.gz` & `tmp/gpp_components-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpp_components-0.0.8.tar", last modified: Tue Dec 26 05:54:52 2023, max compression
+gzip compressed data, was "gpp_components-0.0.9.tar", last modified: Tue Dec 26 06:01:20 2023, max compression
```

## Comparing `gpp_components-0.0.8.tar` & `gpp_components-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-12-26 05:54:52.415839 gpp_components-0.0.8/
--rw-rw-rw-   0        0        0     1097 2023-11-13 03:12:05.000000 gpp_components-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      386 2023-12-26 05:54:52.400929 gpp_components-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       58 2023-11-13 03:12:05.000000 gpp_components-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-12-26 05:54:52.301994 gpp_components-0.0.8/gpp_components/
--rw-rw-rw-   0        0        0       19 2023-12-26 05:13:21.000000 gpp_components-0.0.8/gpp_components/__init__.py
--rw-rw-rw-   0        0        0     1076 2023-12-26 05:13:21.000000 gpp_components-0.0.8/gpp_components/aes.py
--rw-rw-rw-   0        0        0       67 2023-12-26 05:13:21.000000 gpp_components-0.0.8/gpp_components/constant.py
--rw-rw-rw-   0        0        0     4442 2023-12-26 05:13:21.000000 gpp_components-0.0.8/gpp_components/dbConfig.py
--rw-rw-rw-   0        0        0     6755 2023-12-26 05:13:21.000000 gpp_components-0.0.8/gpp_components/handleData.py
--rw-rw-rw-   0        0        0     1629 2023-12-26 05:13:21.000000 gpp_components-0.0.8/gpp_components/lazyImport.py
--rw-rw-rw-   0        0        0      960 2023-12-26 05:13:21.000000 gpp_components-0.0.8/gpp_components/response.py
--rw-rw-rw-   0        0        0     2625 2023-12-26 05:54:03.000000 gpp_components-0.0.8/gpp_components/runOracle.py
--rw-rw-rw-   0        0        0     2880 2023-12-26 05:13:21.000000 gpp_components-0.0.8/gpp_components/sendMail.py
-drwxrwxrwx   0        0        0        0 2023-12-26 05:54:52.384301 gpp_components-0.0.8/gpp_components.egg-info/
--rw-rw-rw-   0        0        0      386 2023-12-26 05:54:51.000000 gpp_components-0.0.8/gpp_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-12-26 05:54:51.000000 gpp_components-0.0.8/gpp_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-26 05:54:51.000000 gpp_components-0.0.8/gpp_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-12-26 05:54:51.000000 gpp_components-0.0.8/gpp_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-12-26 05:54:51.000000 gpp_components-0.0.8/gpp_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-26 05:54:52.417705 gpp_components-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-12-26 05:54:13.000000 gpp_components-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-26 06:01:20.132431 gpp_components-0.0.9/
+-rw-rw-rw-   0        0        0     1097 2023-11-13 03:12:05.000000 gpp_components-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      386 2023-12-26 06:01:20.126373 gpp_components-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2023-11-13 03:12:05.000000 gpp_components-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-12-26 06:01:20.073129 gpp_components-0.0.9/gpp_components/
+-rw-rw-rw-   0        0        0       19 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/__init__.py
+-rw-rw-rw-   0        0        0     1076 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/aes.py
+-rw-rw-rw-   0        0        0       67 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/constant.py
+-rw-rw-rw-   0        0        0     4442 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/dbConfig.py
+-rw-rw-rw-   0        0        0     6755 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/handleData.py
+-rw-rw-rw-   0        0        0     1629 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/lazyImport.py
+-rw-rw-rw-   0        0        0      960 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/response.py
+-rw-rw-rw-   0        0        0     2621 2023-12-26 06:00:55.000000 gpp_components-0.0.9/gpp_components/runOracle.py
+-rw-rw-rw-   0        0        0     2880 2023-12-26 05:13:21.000000 gpp_components-0.0.9/gpp_components/sendMail.py
+drwxrwxrwx   0        0        0        0 2023-12-26 06:01:20.114063 gpp_components-0.0.9/gpp_components.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-12-26 06:01:19.000000 gpp_components-0.0.9/gpp_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-12-26 06:01:19.000000 gpp_components-0.0.9/gpp_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-26 06:01:19.000000 gpp_components-0.0.9/gpp_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-12-26 06:01:19.000000 gpp_components-0.0.9/gpp_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-12-26 06:01:19.000000 gpp_components-0.0.9/gpp_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-26 06:01:20.132431 gpp_components-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-12-26 06:01:09.000000 gpp_components-0.0.9/setup.py
```

### Comparing `gpp_components-0.0.8/LICENSE` & `gpp_components-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.8/gpp_components/aes.py` & `gpp_components-0.0.9/gpp_components/aes.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.8/gpp_components/dbConfig.py` & `gpp_components-0.0.9/gpp_components/dbConfig.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.8/gpp_components/handleData.py` & `gpp_components-0.0.9/gpp_components/handleData.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.8/gpp_components/lazyImport.py` & `gpp_components-0.0.9/gpp_components/lazyImport.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.8/gpp_components/response.py` & `gpp_components-0.0.9/gpp_components/response.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.8/gpp_components/runOracle.py` & `gpp_components-0.0.9/gpp_components/runOracle.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,17 @@
                 data = []
                 for i in self.qs:
                     data.append(dict(zip(col, i)))
                 return data
 
     def runProc(self, sp_name, jsonStr):
         try:
-            cursor = self.conn.cursor()
+            cursor = self.conn.cursor() 
             v_output = cursor.var(cx_Oracle.CLOB)
-            self.cursor.callproc(sp_name, [str(jsonStr), v_output])
+            cursor.callproc(sp_name, [str(jsonStr), v_output])
             return v_output.getvalue()
         except cx_Oracle.DatabaseError as e:
             return Response(False, f"Problem in runSql: {e}")
         finally:
             self.closeConnection()
 
     def getTNS(self, dbJson):
```

### Comparing `gpp_components-0.0.8/gpp_components/sendMail.py` & `gpp_components-0.0.9/gpp_components/sendMail.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.0.8/setup.py` & `gpp_components-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gpp_components",
-    version="0.0.8",
+    version="0.0.9",
     #
     author="L",
     description="for internal use",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT Licence",
     #
```

