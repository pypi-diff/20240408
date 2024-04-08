# Comparing `tmp/dmk_packages-0.5.0.tar.gz` & `tmp/dmk_packages-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmk_packages-0.5.0.tar", last modified: Thu Apr  4 02:58:35 2024, max compression
+gzip compressed data, was "dmk_packages-0.6.0.tar", last modified: Mon Apr  8 08:19:32 2024, max compression
```

## Comparing `dmk_packages-0.5.0.tar` & `dmk_packages-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.611972 dmk_packages-0.5.0/
--rw-r--r--   0 layla      (501) staff       (20)    11347 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/LICENSE
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-04-04 02:58:35.611608 dmk_packages-0.5.0/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)     1365 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/README.md
--rw-r--r--   0 layla      (501) staff       (20)      584 2024-04-04 02:20:18.000000 dmk_packages-0.5.0/pyproject.toml
--rw-r--r--   0 layla      (501) staff       (20)       38 2024-04-04 02:58:35.612067 dmk_packages-0.5.0/setup.cfg
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.599755 dmk_packages-0.5.0/src/
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.603373 dmk_packages-0.5.0/src/dmk_packages/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/src/dmk_packages/__init__.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.609429 dmk_packages-0.5.0/src/dmk_packages/crawler/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/src/dmk_packages/crawler/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     2321 2024-04-03 06:07:52.000000 dmk_packages-0.5.0/src/dmk_packages/crawler/naver_blog.py
--rw-r--r--   0 layla      (501) staff       (20)    15349 2024-04-01 06:49:53.000000 dmk_packages-0.5.0/src/dmk_packages/crawler/naver_search_volume.py
--rw-r--r--   0 layla      (501) staff       (20)    12855 2024-04-04 02:18:34.000000 dmk_packages-0.5.0/src/dmk_packages/crawler/youtube.py
--rw-r--r--   0 layla      (501) staff       (20)     2258 2024-04-04 01:44:42.000000 dmk_packages-0.5.0/src/dmk_packages/crawler/youtube_test.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.610452 dmk_packages-0.5.0/src/dmk_packages/database/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/src/dmk_packages/database/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     3057 2024-04-03 06:07:52.000000 dmk_packages-0.5.0/src/dmk_packages/database/database.py
--rw-r--r--   0 layla      (501) staff       (20)     1895 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/src/dmk_packages/naver_datalab.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.611084 dmk_packages-0.5.0/src/dmk_packages.egg-info/
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-04-04 02:58:35.000000 dmk_packages-0.5.0/src/dmk_packages.egg-info/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)      571 2024-04-04 02:58:35.000000 dmk_packages-0.5.0/src/dmk_packages.egg-info/SOURCES.txt
--rw-r--r--   0 layla      (501) staff       (20)        1 2024-04-04 02:58:35.000000 dmk_packages-0.5.0/src/dmk_packages.egg-info/dependency_links.txt
--rw-r--r--   0 layla      (501) staff       (20)       41 2024-04-04 02:58:35.000000 dmk_packages-0.5.0/src/dmk_packages.egg-info/requires.txt
--rw-r--r--   0 layla      (501) staff       (20)       13 2024-04-04 02:58:35.000000 dmk_packages-0.5.0/src/dmk_packages.egg-info/top_level.txt
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-08 08:19:32.064192 dmk_packages-0.6.0/
+-rw-r--r--   0 tommie     (501) staff       (20)    11347 2024-04-04 04:45:57.000000 dmk_packages-0.6.0/LICENSE
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-08 08:19:32.063923 dmk_packages-0.6.0/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)     1365 2024-04-04 04:45:57.000000 dmk_packages-0.6.0/README.md
+-rw-r--r--   0 tommie     (501) staff       (20)      584 2024-04-08 08:18:59.000000 dmk_packages-0.6.0/pyproject.toml
+-rw-r--r--   0 tommie     (501) staff       (20)       38 2024-04-08 08:19:32.064247 dmk_packages-0.6.0/setup.cfg
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-08 08:19:32.059236 dmk_packages-0.6.0/src/
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-08 08:19:32.060568 dmk_packages-0.6.0/src/dmk_packages/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.0/src/dmk_packages/__init__.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-08 08:19:32.063083 dmk_packages-0.6.0/src/dmk_packages/crawler/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.0/src/dmk_packages/crawler/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     9103 2024-04-04 08:41:16.000000 dmk_packages-0.6.0/src/dmk_packages/crawler/bigkinds.py
+-rw-r--r--   0 tommie     (501) staff       (20)     9527 2024-04-08 08:14:20.000000 dmk_packages-0.6.0/src/dmk_packages/crawler/clien.py
+-rw-r--r--   0 tommie     (501) staff       (20)     8120 2024-04-04 08:51:59.000000 dmk_packages-0.6.0/src/dmk_packages/crawler/fnguide.py
+-rw-r--r--   0 tommie     (501) staff       (20)     3842 2024-04-04 08:44:08.000000 dmk_packages-0.6.0/src/dmk_packages/crawler/fnguide_pdf_update.py
+-rw-r--r--   0 tommie     (501) staff       (20)     2321 2024-04-04 04:45:57.000000 dmk_packages-0.6.0/src/dmk_packages/crawler/naver_blog.py
+-rw-r--r--   0 tommie     (501) staff       (20)    15349 2024-04-04 04:45:57.000000 dmk_packages-0.6.0/src/dmk_packages/crawler/naver_search_volume.py
+-rw-r--r--   0 tommie     (501) staff       (20)    12855 2024-04-04 04:45:57.000000 dmk_packages-0.6.0/src/dmk_packages/crawler/youtube.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-08 08:19:32.063421 dmk_packages-0.6.0/src/dmk_packages/database/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.0/src/dmk_packages/database/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     3057 2024-04-04 04:45:57.000000 dmk_packages-0.6.0/src/dmk_packages/database/database.py
+-rw-r--r--   0 tommie     (501) staff       (20)     1895 2024-04-04 04:45:57.000000 dmk_packages-0.6.0/src/dmk_packages/naver_datalab.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-08 08:19:32.063625 dmk_packages-0.6.0/src/dmk_packages.egg-info/
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-08 08:19:32.000000 dmk_packages-0.6.0/src/dmk_packages.egg-info/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)      684 2024-04-08 08:19:32.000000 dmk_packages-0.6.0/src/dmk_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 tommie     (501) staff       (20)        1 2024-04-08 08:19:32.000000 dmk_packages-0.6.0/src/dmk_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       41 2024-04-08 08:19:32.000000 dmk_packages-0.6.0/src/dmk_packages.egg-info/requires.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       13 2024-04-08 08:19:32.000000 dmk_packages-0.6.0/src/dmk_packages.egg-info/top_level.txt
```

### Comparing `dmk_packages-0.5.0/LICENSE` & `dmk_packages-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.5.0/PKG-INFO` & `dmk_packages-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.5.0
+Version: 0.6.0
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.5.0/README.md` & `dmk_packages-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.5.0/pyproject.toml` & `dmk_packages-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmk_packages"
-version = "0.5.0"
+version = "0.6.0"
 authors = [{ name = "DataMarketingKorea", email = "infra@datamarketing.co.kr" }]
 description = "Common packages for DataMKTKorea"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["SQLAlchemy", "python-dotenv", "psycopg2-binary"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `dmk_packages-0.5.0/src/dmk_packages/crawler/naver_blog.py` & `dmk_packages-0.6.0/src/dmk_packages/crawler/naver_blog.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.5.0/src/dmk_packages/crawler/naver_search_volume.py` & `dmk_packages-0.6.0/src/dmk_packages/crawler/naver_search_volume.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.5.0/src/dmk_packages/crawler/youtube.py` & `dmk_packages-0.6.0/src/dmk_packages/crawler/youtube.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.5.0/src/dmk_packages/database/database.py` & `dmk_packages-0.6.0/src/dmk_packages/database/database.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.5.0/src/dmk_packages/naver_datalab.py` & `dmk_packages-0.6.0/src/dmk_packages/naver_datalab.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.5.0/src/dmk_packages.egg-info/PKG-INFO` & `dmk_packages-0.6.0/src/dmk_packages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.5.0
+Version: 0.6.0
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

