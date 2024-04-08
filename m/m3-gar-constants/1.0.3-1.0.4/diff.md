# Comparing `tmp/m3-gar-constants-1.0.3.tar.gz` & `tmp/m3-gar-constants-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3-gar-constants-1.0.3.tar", last modified: Thu Apr 28 15:30:39 2022, max compression
+gzip compressed data, was "m3-gar-constants-1.0.4.tar", last modified: Mon Apr  8 12:13:06 2024, max compression
```

## Comparing `m3-gar-constants-1.0.3.tar` & `m3-gar-constants-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 15:30:39.373818 m3-gar-constants-1.0.3/
--rw-r--r--   0 root         (0) root         (0)       23 2022-04-28 06:56:28.000000 m3-gar-constants-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      782 2022-04-28 15:30:39.373818 m3-gar-constants-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      159 2022-04-27 13:48:55.000000 m3-gar-constants-1.0.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 15:30:39.372819 m3-gar-constants-1.0.3/m3_gar_constants/
--rw-r--r--   0 root         (0) root         (0)     3753 2022-04-28 15:30:23.000000 m3-gar-constants-1.0.3/m3_gar_constants/__init__.py
--rw-r--r--   0 root         (0) root         (0)       93 2022-04-28 15:30:23.000000 m3-gar-constants-1.0.3/m3_gar_constants/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 15:30:39.373818 m3-gar-constants-1.0.3/m3_gar_constants.egg-info/
--rw-r--r--   0 root         (0) root         (0)      782 2022-04-28 15:30:38.000000 m3-gar-constants-1.0.3/m3_gar_constants.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      264 2022-04-28 15:30:39.000000 m3-gar-constants-1.0.3/m3_gar_constants.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-28 15:30:38.000000 m3-gar-constants-1.0.3/m3_gar_constants.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-04-28 15:30:39.000000 m3-gar-constants-1.0.3/m3_gar_constants.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-04-28 15:30:39.373818 m3-gar-constants-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      116 2022-04-27 13:48:55.000000 m3-gar-constants-1.0.3/setup.py
--rw-r--r--   0 root         (0) root         (0)      897 2022-04-28 06:50:11.000000 m3-gar-constants-1.0.3/setup_kwargs.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:13:06.663895 m3-gar-constants-1.0.4/
+-rw-r--r--   0 toor      (1000) toor      (1000)       23 2022-04-28 06:56:28.000000 m3-gar-constants-1.0.4/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)      763 2024-04-08 12:13:06.662896 m3-gar-constants-1.0.4/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      159 2022-04-27 13:48:55.000000 m3-gar-constants-1.0.4/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:13:06.661896 m3-gar-constants-1.0.4/m3_gar_constants/
+-rw-r--r--   0 toor      (1000) toor      (1000)     3889 2024-04-08 12:13:03.000000 m3-gar-constants-1.0.4/m3_gar_constants/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       93 2024-04-08 12:13:03.000000 m3-gar-constants-1.0.4/m3_gar_constants/version.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:13:06.662896 m3-gar-constants-1.0.4/m3_gar_constants.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)      763 2024-04-08 12:13:06.000000 m3-gar-constants-1.0.4/m3_gar_constants.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      264 2024-04-08 12:13:06.000000 m3-gar-constants-1.0.4/m3_gar_constants.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-08 12:13:06.000000 m3-gar-constants-1.0.4/m3_gar_constants.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       17 2024-04-08 12:13:06.000000 m3-gar-constants-1.0.4/m3_gar_constants.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-04-08 12:13:06.663895 m3-gar-constants-1.0.4/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)      116 2022-04-27 13:48:55.000000 m3-gar-constants-1.0.4/setup.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      897 2022-04-28 06:50:11.000000 m3-gar-constants-1.0.4/setup_kwargs.py
```

### Comparing `m3-gar-constants-1.0.3/PKG-INFO` & `m3-gar-constants-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: m3-gar-constants
-Version: 1.0.3
+Version: 1.0.4
 Summary: GAR constants for m3
 Author: BARS Group
 Author-email: bars@bars.group
 License: MIT license
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 
 Пакет ``m3-gar-constants`` предоставляет необходимые константы
 для библиотек ``m3-gar`` и ``m3-gar-client``.
-
```

### Comparing `m3-gar-constants-1.0.3/m3_gar_constants/__init__.py` & `m3-gar-constants-1.0.4/m3_gar_constants/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,7 +131,10 @@
 DEFAULT_PAGE_LIMIT = 20
 
 # Длительность кэширования по умолчанию 24 часа
 DEFAULT_CACHE_TIMEOUT = 24 * 60 * 60
 
 # Код официальных названий объектов
 CODE_PARAM_TYPES_OFFICIAL = 'Official'
+
+# Кол-во найденных объектов на странице в результатах поисках
+RESULT_PAGE_SIZE = 15
```

### Comparing `m3-gar-constants-1.0.3/m3_gar_constants.egg-info/PKG-INFO` & `m3-gar-constants-1.0.4/m3_gar_constants.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: m3-gar-constants
-Version: 1.0.3
+Version: 1.0.4
 Summary: GAR constants for m3
 Author: BARS Group
 Author-email: bars@bars.group
 License: MIT license
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 
 Пакет ``m3-gar-constants`` предоставляет необходимые константы
 для библиотек ``m3-gar`` и ``m3-gar-client``.
-
```

### Comparing `m3-gar-constants-1.0.3/setup_kwargs.py` & `m3-gar-constants-1.0.4/setup_kwargs.py`

 * *Files identical despite different names*

