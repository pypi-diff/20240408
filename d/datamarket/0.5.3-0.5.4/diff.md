# Comparing `tmp/datamarket-0.5.3.tar.gz` & `tmp/datamarket-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamarket-0.5.3.tar", last modified: Tue Apr  2 08:51:56 2024, max compression
+gzip compressed data, was "datamarket-0.5.4.tar", last modified: Mon Apr  8 12:04:33 2024, max compression
```

## Comparing `datamarket-0.5.3.tar` & `datamarket-0.5.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:51:56.958124 datamarket-0.5.3/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)    35149 2024-04-02 08:28:11.000000 datamarket-0.5.3/LICENSE
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1692 2024-04-02 08:51:56.954124 datamarket-0.5.3/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      934 2024-04-02 08:28:11.000000 datamarket-0.5.3/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2024-04-02 08:51:56.958124 datamarket-0.5.3/setup.cfg
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1080 2024-04-02 08:29:41.000000 datamarket-0.5.3/setup.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:51:56.922123 datamarket-0.5.3/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:51:56.930123 datamarket-0.5.3/src/datamarket/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       12 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/__init__.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:51:56.942124 datamarket-0.5.3/src/datamarket/interfaces/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/interfaces/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     3398 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/interfaces/alchemy.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1252 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/interfaces/aws.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2915 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/interfaces/drive.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1344 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/interfaces/ftp.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2730 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/interfaces/nominatim.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2913 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/interfaces/proxy.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2565 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/interfaces/tinybird.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:51:56.946124 datamarket-0.5.3/src/datamarket/params/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/params/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1143 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/params/nominatim.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:51:56.954124 datamarket-0.5.3/src/datamarket/utils/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       20 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/utils/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2270 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/utils/main.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2499 2024-04-02 08:28:11.000000 datamarket-0.5.3/src/datamarket/utils/selenium.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      941 2024-04-02 08:51:09.000000 datamarket-0.5.3/src/datamarket/utils/soda.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:51:56.954124 datamarket-0.5.3/src/datamarket.egg-info/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1692 2024-04-02 08:51:56.000000 datamarket-0.5.3/src/datamarket.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      723 2024-04-02 08:51:56.000000 datamarket-0.5.3/src/datamarket.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2024-04-02 08:51:56.000000 datamarket-0.5.3/src/datamarket.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       86 2024-04-02 08:51:56.000000 datamarket-0.5.3/src/datamarket.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       11 2024-04-02 08:51:56.000000 datamarket-0.5.3/src/datamarket.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:04:33.600136 datamarket-0.5.4/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)    35149 2024-04-02 08:28:11.000000 datamarket-0.5.4/LICENSE
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1692 2024-04-08 12:04:33.600136 datamarket-0.5.4/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      934 2024-04-02 08:28:11.000000 datamarket-0.5.4/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2024-04-08 12:04:33.600136 datamarket-0.5.4/setup.cfg
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1080 2024-04-08 12:03:40.000000 datamarket-0.5.4/setup.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:04:33.592136 datamarket-0.5.4/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:04:33.596136 datamarket-0.5.4/src/datamarket/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       12 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/__init__.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:04:33.596136 datamarket-0.5.4/src/datamarket/interfaces/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/interfaces/__init__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3398 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/interfaces/alchemy.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1252 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/interfaces/aws.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2915 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/interfaces/drive.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1344 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/interfaces/ftp.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2730 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/interfaces/nominatim.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2913 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/interfaces/proxy.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2565 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/interfaces/tinybird.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:04:33.596136 datamarket-0.5.4/src/datamarket/params/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/params/__init__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1143 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/params/nominatim.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:04:33.600136 datamarket-0.5.4/src/datamarket/utils/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       20 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/utils/__init__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      635 2024-04-08 11:53:46.000000 datamarket-0.5.4/src/datamarket/utils/alchemy.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2270 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/utils/main.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2499 2024-04-02 08:28:11.000000 datamarket-0.5.4/src/datamarket/utils/selenium.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      941 2024-04-02 08:51:09.000000 datamarket-0.5.4/src/datamarket/utils/soda.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:04:33.600136 datamarket-0.5.4/src/datamarket.egg-info/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1692 2024-04-08 12:04:33.000000 datamarket-0.5.4/src/datamarket.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      755 2024-04-08 12:04:33.000000 datamarket-0.5.4/src/datamarket.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2024-04-08 12:04:33.000000 datamarket-0.5.4/src/datamarket.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       86 2024-04-08 12:04:33.000000 datamarket-0.5.4/src/datamarket.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       11 2024-04-08 12:04:33.000000 datamarket-0.5.4/src/datamarket.egg-info/top_level.txt
```

### Comparing `datamarket-0.5.3/LICENSE` & `datamarket-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/PKG-INFO` & `datamarket-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.5.3
+Version: 0.5.4
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.5.3/README.md` & `datamarket-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/setup.py` & `datamarket-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "undetected_chromedriver",
     "pendulum",
     "boto3",
 ]
 
 setuptools.setup(
     name="datamarket",
-    version="0.5.3",
+    version="0.5.4",
     author="DataMarket",
     author_email="techsupport@datamarket.es",
     description="Utilities that integrate advance scraping knowledge into just one library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Data-Market/datamarket",
     project_urls={
```

### Comparing `datamarket-0.5.3/src/datamarket/interfaces/alchemy.py` & `datamarket-0.5.4/src/datamarket/interfaces/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/src/datamarket/interfaces/aws.py` & `datamarket-0.5.4/src/datamarket/interfaces/aws.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/src/datamarket/interfaces/drive.py` & `datamarket-0.5.4/src/datamarket/interfaces/drive.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/src/datamarket/interfaces/ftp.py` & `datamarket-0.5.4/src/datamarket/interfaces/ftp.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/src/datamarket/interfaces/nominatim.py` & `datamarket-0.5.4/src/datamarket/interfaces/nominatim.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/src/datamarket/interfaces/proxy.py` & `datamarket-0.5.4/src/datamarket/interfaces/proxy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/src/datamarket/interfaces/tinybird.py` & `datamarket-0.5.4/src/datamarket/interfaces/tinybird.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/src/datamarket/params/nominatim.py` & `datamarket-0.5.4/src/datamarket/params/nominatim.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/src/datamarket/utils/main.py` & `datamarket-0.5.4/src/datamarket/utils/main.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/src/datamarket/utils/selenium.py` & `datamarket-0.5.4/src/datamarket/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/src/datamarket/utils/soda.py` & `datamarket-0.5.4/src/datamarket/utils/soda.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.3/src/datamarket.egg-info/PKG-INFO` & `datamarket-0.5.4/src/datamarket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.5.3
+Version: 0.5.4
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.5.3/src/datamarket.egg-info/SOURCES.txt` & `datamarket-0.5.4/src/datamarket.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,10 +14,11 @@
 src/datamarket/interfaces/ftp.py
 src/datamarket/interfaces/nominatim.py
 src/datamarket/interfaces/proxy.py
 src/datamarket/interfaces/tinybird.py
 src/datamarket/params/__init__.py
 src/datamarket/params/nominatim.py
 src/datamarket/utils/__init__.py
+src/datamarket/utils/alchemy.py
 src/datamarket/utils/main.py
 src/datamarket/utils/selenium.py
 src/datamarket/utils/soda.py
```

