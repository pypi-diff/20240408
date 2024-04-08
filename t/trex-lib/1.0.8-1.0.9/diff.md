# Comparing `tmp/trex-lib-1.0.8.tar.gz` & `tmp/trex-lib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trex-lib-1.0.8.tar", last modified: Wed Oct  4 04:19:13 2023, max compression
+gzip compressed data, was "dist/trex-lib-1.0.9.tar", last modified: Thu Nov  9 07:58:11 2023, max compression
```

## Comparing `trex-lib-1.0.8.tar` & `trex-lib-1.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-10-04 04:19:13.000000 trex-lib-1.0.8/
--rw-r--r--   0 jacklok    (501) staff       (20)     1052 2020-09-03 05:31:42.000000 trex-lib-1.0.8/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-1.0.8/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-10-04 04:19:13.000000 trex-lib-1.0.8/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-1.0.8/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2021-08-13 04:29:57.000000 trex-lib-1.0.8/pyproject.toml
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-10-04 04:19:13.000000 trex-lib-1.0.8/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)     1202 2023-10-04 04:18:44.000000 trex-lib-1.0.8/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trex_lib.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trex_lib.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1274 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trex_lib.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trex_lib.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)      292 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trex_lib.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       14 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trex_lib.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trexlib/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-1.0.8/trexlib/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5053 2023-08-16 14:56:05.000000 trex-lib-1.0.8/trexlib/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trexlib/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-1.0.8/trexlib/libs/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trexlib/libs/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-02-13 02:03:08.000000 trex-lib-1.0.8/trexlib/libs/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9782 2023-03-28 03:00:42.000000 trex-lib-1.0.8/trexlib/libs/controllers/task_base_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trexlib/libs/firebase/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2022-06-09 04:14:24.000000 trex-lib-1.0.8/trexlib/libs/firebase/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      378 2022-06-09 06:38:00.000000 trex-lib-1.0.8/trexlib/libs/firebase/firebase_helper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trexlib/libs/flask_wtf/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-1.0.8/trexlib/libs/flask_wtf/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-1.0.8/trexlib/libs/flask_wtf/crsf_ext.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trexlib/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-1.0.8/trexlib/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trexlib/utils/common/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-1.0.8/trexlib/utils/common/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4514 2022-09-26 14:54:31.000000 trex-lib-1.0.8/trexlib/utils/common/common_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      926 2023-08-30 15:08:13.000000 trex-lib-1.0.8/trexlib/utils/common/config_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-1.0.8/trexlib/utils/common/conftest.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-1.0.8/trexlib/utils/common/crm_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1573 2021-04-21 02:37:36.000000 trex-lib-1.0.8/trexlib/utils/common/currency_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2707 2021-09-16 10:19:23.000000 trex-lib-1.0.8/trexlib/utils/common/date_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-1.0.8/trexlib/utils/common/float_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4201 2021-03-04 08:12:18.000000 trex-lib-1.0.8/trexlib/utils/common/format_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1086 2020-09-04 07:48:19.000000 trex-lib-1.0.8/trexlib/utils/common/pagination_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1087 2021-06-24 07:11:43.000000 trex-lib-1.0.8/trexlib/utils/common/phone_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      825 2021-08-13 09:35:21.000000 trex-lib-1.0.8/trexlib/utils/common/user_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      840 2021-07-01 09:54:24.000000 trex-lib-1.0.8/trexlib/utils/crypto_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-10-04 04:19:13.000000 trex-lib-1.0.8/trexlib/utils/google/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-1.0.8/trexlib/utils/google/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12907 2021-08-20 10:49:32.000000 trex-lib-1.0.8/trexlib/utils/google/bigquery_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4173 2023-10-04 04:18:11.000000 trex-lib-1.0.8/trexlib/utils/google/cloud_tasks_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1364 2023-03-08 04:49:28.000000 trex-lib-1.0.8/trexlib/utils/google/gcloud_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-1.0.8/trexlib/utils/log_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3215 2021-08-13 04:41:06.000000 trex-lib-1.0.8/trexlib/utils/security_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8212 2023-08-16 09:12:40.000000 trex-lib-1.0.8/trexlib/utils/sms_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4946 2023-08-16 03:30:52.000000 trex-lib-1.0.8/trexlib/utils/string_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-1.0.8/trexlib/utils/url_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1052 2020-09-03 05:31:42.000000 trex-lib-1.0.9/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-1.0.9/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-11-09 07:58:11.000000 trex-lib-1.0.9/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-1.0.9/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2021-08-13 04:29:57.000000 trex-lib-1.0.9/pyproject.toml
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-11-09 07:58:11.000000 trex-lib-1.0.9/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)     1202 2023-11-09 07:57:38.000000 trex-lib-1.0.9/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1274 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)      292 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       14 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-1.0.9/trexlib/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5053 2023-08-16 14:56:05.000000 trex-lib-1.0.9/trexlib/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-1.0.9/trexlib/libs/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/libs/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-02-13 02:03:08.000000 trex-lib-1.0.9/trexlib/libs/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9782 2023-03-28 03:00:42.000000 trex-lib-1.0.9/trexlib/libs/controllers/task_base_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/libs/firebase/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2022-06-09 04:14:24.000000 trex-lib-1.0.9/trexlib/libs/firebase/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      378 2022-06-09 06:38:00.000000 trex-lib-1.0.9/trexlib/libs/firebase/firebase_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/libs/flask_wtf/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-1.0.9/trexlib/libs/flask_wtf/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-1.0.9/trexlib/libs/flask_wtf/crsf_ext.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-1.0.9/trexlib/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/utils/common/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-1.0.9/trexlib/utils/common/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4514 2022-09-26 14:54:31.000000 trex-lib-1.0.9/trexlib/utils/common/common_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      926 2023-08-30 15:08:13.000000 trex-lib-1.0.9/trexlib/utils/common/config_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-1.0.9/trexlib/utils/common/conftest.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-1.0.9/trexlib/utils/common/crm_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1573 2021-04-21 02:37:36.000000 trex-lib-1.0.9/trexlib/utils/common/currency_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3706 2023-11-09 07:11:16.000000 trex-lib-1.0.9/trexlib/utils/common/date_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-1.0.9/trexlib/utils/common/float_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4201 2021-03-04 08:12:18.000000 trex-lib-1.0.9/trexlib/utils/common/format_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1086 2020-09-04 07:48:19.000000 trex-lib-1.0.9/trexlib/utils/common/pagination_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1087 2021-06-24 07:11:43.000000 trex-lib-1.0.9/trexlib/utils/common/phone_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      825 2021-08-13 09:35:21.000000 trex-lib-1.0.9/trexlib/utils/common/user_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      840 2021-07-01 09:54:24.000000 trex-lib-1.0.9/trexlib/utils/crypto_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/utils/google/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-1.0.9/trexlib/utils/google/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12907 2021-08-20 10:49:32.000000 trex-lib-1.0.9/trexlib/utils/google/bigquery_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4283 2023-10-04 04:35:54.000000 trex-lib-1.0.9/trexlib/utils/google/cloud_tasks_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1364 2023-03-08 04:49:28.000000 trex-lib-1.0.9/trexlib/utils/google/gcloud_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-1.0.9/trexlib/utils/log_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3215 2021-08-13 04:41:06.000000 trex-lib-1.0.9/trexlib/utils/security_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8212 2023-08-16 09:12:40.000000 trex-lib-1.0.9/trexlib/utils/sms_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4946 2023-08-16 03:30:52.000000 trex-lib-1.0.9/trexlib/utils/string_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-1.0.9/trexlib/utils/url_util.py
```

### Comparing `trex-lib-1.0.8/LICENSE` & `trex-lib-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/setup.py` & `trex-lib-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-lib',  
-     version='1.0.8',
+     version='1.0.9',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex Core library package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-lib",
      packages=setuptools.find_packages(),
```

### Comparing `trex-lib-1.0.8/trex_lib.egg-info/SOURCES.txt` & `trex-lib-1.0.9/trex_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/conf.py` & `trex-lib-1.0.9/trexlib/conf.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/libs/controllers/task_base_routes.py` & `trex-lib-1.0.9/trexlib/libs/controllers/task_base_routes.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/common/common_util.py` & `trex-lib-1.0.9/trexlib/utils/common/common_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/common/config_util.py` & `trex-lib-1.0.9/trexlib/utils/common/config_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/common/crm_util.py` & `trex-lib-1.0.9/trexlib/utils/common/crm_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/common/currency_util.py` & `trex-lib-1.0.9/trexlib/utils/common/currency_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/common/date_util.py` & `trex-lib-1.0.9/trexlib/utils/common/date_util.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Created on 19 May 2020
 
 @author: jacklok
 '''
  
 from datetime import datetime, timedelta
 from dateutil.relativedelta import relativedelta
+from trexlib import conf
+import pytz
 
 
 def parse_date(date_value, date_separator='/', full_year_date_format='%d/%m/%Y', short_year_date_format='%d/%m/%y'):
     if date_value is not None:
         #logging.info('parse_date: date_value=%s', date_value)
         _d_array = date_value.split(date_separator)
         if len(_d_array)==3:
@@ -69,11 +71,35 @@
 def last_day_of_month(date):
     if date.month == 12:
         return date.replace(day=31)
     return date.replace(month=date.month+1, day=1) - timedelta(days=1)
 
 def to_day_of_year(datetime_input):
     return datetime_input.timetuple().tm_yday
+
+def from_utc_datetime_to_local_datetime(datetime_value, country_code=conf.DEFAULT_COUNTRY_CODE, datetime_format=None):
+    
+    if datetime_format is None:
+        datetime_format = '%d/%m/%Y %H:%M:%S'
+        
+    if isinstance(datetime_value, str):
+        datetime_value = datetime.strptime(datetime_value, datetime_format)
+        
+    utc_datetime = datetime(datetime_value.year, 
+                            datetime_value.month, 
+                            datetime_value.day, 
+                            datetime_value.hour, 
+                            datetime_value.minute, 
+                            datetime_value.second, 
+                            tzinfo=pytz.utc)
+    
+    country_code        = country_code.upper()
+    country_timezones   = pytz.country_timezones[country_code]
+    country_timezone    = pytz.timezone(country_timezones[0])
+    
+    local_datetime = utc_datetime.astimezone(country_timezone)
+    
+    return local_datetime
```

### Comparing `trex-lib-1.0.8/trexlib/utils/common/format_util.py` & `trex-lib-1.0.9/trexlib/utils/common/format_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/common/pagination_util.py` & `trex-lib-1.0.9/trexlib/utils/common/pagination_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/common/phone_util.py` & `trex-lib-1.0.9/trexlib/utils/common/phone_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/common/user_util.py` & `trex-lib-1.0.9/trexlib/utils/common/user_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/crypto_util.py` & `trex-lib-1.0.9/trexlib/utils/crypto_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/google/bigquery_util.py` & `trex-lib-1.0.9/trexlib/utils/google/bigquery_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/google/cloud_tasks_util.py` & `trex-lib-1.0.9/trexlib/utils/google/cloud_tasks_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         # The API expects a payload of type bytes.
         converted_payload = payload.encode()
         
         logger.debug('create_task: converted_payload=%s', converted_payload)
     
         # Add the payload to the request.
         task["http_request"]["body"] = converted_payload
-    
+    else:
+        task["http_request"]["headers"] = {"Content-type": "application/x-www-form-urlencoded"}
+        
     
     if headers is not None:
         for k,v in headers.items():
             task["http_request"]["headers"][k]=v
             
     
     task["http_request"]["headers"]['X-task-id']        = task_id
```

### Comparing `trex-lib-1.0.8/trexlib/utils/google/gcloud_util.py` & `trex-lib-1.0.9/trexlib/utils/google/gcloud_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/security_util.py` & `trex-lib-1.0.9/trexlib/utils/security_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/sms_util.py` & `trex-lib-1.0.9/trexlib/utils/sms_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/string_util.py` & `trex-lib-1.0.9/trexlib/utils/string_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.8/trexlib/utils/url_util.py` & `trex-lib-1.0.9/trexlib/utils/url_util.py`

 * *Files identical despite different names*

