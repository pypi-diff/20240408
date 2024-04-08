# Comparing `tmp/arcsecond-3.0.2.tar.gz` & `tmp/arcsecond-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcsecond-3.0.2.tar", last modified: Sun Mar 31 14:46:04 2024, max compression
+gzip compressed data, was "arcsecond-3.0.3.tar", last modified: Mon Apr  8 12:34:40 2024, max compression
```

## Comparing `arcsecond-3.0.2.tar` & `arcsecond-3.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-03-31 14:46:04.613695 arcsecond-3.0.2/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1072 2018-07-30 07:31:57.000000 arcsecond-3.0.2/LICENSE
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-03-31 14:46:04.613601 arcsecond-3.0.2/PKG-INFO
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1029 2024-03-31 14:10:14.000000 arcsecond-3.0.2/README.md
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-03-31 14:46:04.601387 arcsecond-3.0.2/arcsecond/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      269 2024-03-31 14:45:36.000000 arcsecond-3.0.2/arcsecond/__init__.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-03-31 14:46:04.608433 arcsecond-3.0.2/arcsecond/api/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      203 2024-03-31 12:00:54.000000 arcsecond-3.0.2/arcsecond/api/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4409 2024-03-31 14:33:51.000000 arcsecond-3.0.2/arcsecond/api/config.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      304 2024-03-31 14:42:08.000000 arcsecond-3.0.2/arcsecond/api/constants.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4198 2024-03-31 12:57:46.000000 arcsecond-3.0.2/arcsecond/api/endpoint.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2443 2024-03-31 13:03:41.000000 arcsecond-3.0.2/arcsecond/api/main.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     6312 2024-03-31 14:44:54.000000 arcsecond-3.0.2/arcsecond/cli.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      149 2024-03-31 12:00:33.000000 arcsecond-3.0.2/arcsecond/errors.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2277 2024-03-31 14:34:46.000000 arcsecond-3.0.2/arcsecond/options.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-03-31 14:46:04.611448 arcsecond-3.0.2/arcsecond/uploader/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2024-03-21 21:27:31.000000 arcsecond-3.0.2/arcsecond/uploader/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1377 2024-03-31 07:22:21.000000 arcsecond-3.0.2/arcsecond/uploader/constants.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4060 2024-03-31 13:08:01.000000 arcsecond-3.0.2/arcsecond/uploader/context.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2453 2024-03-31 13:04:03.000000 arcsecond-3.0.2/arcsecond/uploader/errors.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1060 2024-03-31 14:43:40.000000 arcsecond-3.0.2/arcsecond/uploader/logger.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4725 2024-03-31 07:26:36.000000 arcsecond-3.0.2/arcsecond/uploader/uploader.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2801 2024-03-31 07:23:32.000000 arcsecond-3.0.2/arcsecond/uploader/utils.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     3477 2024-03-31 14:44:07.000000 arcsecond-3.0.2/arcsecond/uploader/walker.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-03-31 14:46:04.605177 arcsecond-3.0.2/arcsecond.egg-info/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-03-31 14:46:04.000000 arcsecond-3.0.2/arcsecond.egg-info/PKG-INFO
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      877 2024-03-31 14:46:04.000000 arcsecond-3.0.2/arcsecond.egg-info/SOURCES.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-03-31 14:46:04.000000 arcsecond-3.0.2/arcsecond.egg-info/dependency_links.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       49 2024-03-31 14:46:04.000000 arcsecond-3.0.2/arcsecond.egg-info/entry_points.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-03-31 14:46:04.000000 arcsecond-3.0.2/arcsecond.egg-info/not-zip-safe
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       55 2024-03-31 14:46:04.000000 arcsecond-3.0.2/arcsecond.egg-info/requires.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       16 2024-03-31 14:46:04.000000 arcsecond-3.0.2/arcsecond.egg-info/top_level.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       61 2024-03-31 14:46:04.614042 arcsecond-3.0.2/setup.cfg
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1621 2024-03-24 20:33:09.000000 arcsecond-3.0.2/setup.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-03-31 14:46:04.597459 arcsecond-3.0.2/tests/
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-03-31 14:46:04.612222 arcsecond-3.0.2/tests/cli/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.0.2/tests/cli/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1551 2024-03-31 12:07:38.000000 arcsecond-3.0.2/tests/cli/test_cli_options.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1383 2024-03-29 18:20:59.000000 arcsecond-3.0.2/tests/cli/test_config.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-03-31 14:46:04.613061 arcsecond-3.0.2/tests/module/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.0.2/tests/module/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1133 2024-03-29 09:03:34.000000 arcsecond-3.0.2/tests/module/test_arcsecond_root.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1092 2024-03-29 18:42:28.000000 arcsecond-3.0.2/tests/module/test_login.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.645067 arcsecond-3.0.3/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1072 2018-07-30 07:31:57.000000 arcsecond-3.0.3/LICENSE
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-04-08 12:34:40.644999 arcsecond-3.0.3/PKG-INFO
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1029 2024-03-31 14:10:14.000000 arcsecond-3.0.3/README.md
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.638539 arcsecond-3.0.3/arcsecond/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      269 2024-04-08 12:34:16.000000 arcsecond-3.0.3/arcsecond/__init__.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.640847 arcsecond-3.0.3/arcsecond/api/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      203 2024-03-31 12:00:54.000000 arcsecond-3.0.3/arcsecond/api/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     4643 2024-04-08 12:33:03.000000 arcsecond-3.0.3/arcsecond/api/config.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      304 2024-03-31 14:42:08.000000 arcsecond-3.0.3/arcsecond/api/constants.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     4198 2024-03-31 12:57:46.000000 arcsecond-3.0.3/arcsecond/api/endpoint.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     2443 2024-03-31 13:03:41.000000 arcsecond-3.0.3/arcsecond/api/main.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     6312 2024-03-31 14:44:54.000000 arcsecond-3.0.3/arcsecond/cli.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      149 2024-03-31 12:00:33.000000 arcsecond-3.0.3/arcsecond/errors.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     2277 2024-03-31 14:34:46.000000 arcsecond-3.0.3/arcsecond/options.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.643275 arcsecond-3.0.3/arcsecond/uploader/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2024-03-21 21:27:31.000000 arcsecond-3.0.3/arcsecond/uploader/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1377 2024-03-31 07:22:21.000000 arcsecond-3.0.3/arcsecond/uploader/constants.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     4060 2024-03-31 13:08:01.000000 arcsecond-3.0.3/arcsecond/uploader/context.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     2453 2024-03-31 13:04:03.000000 arcsecond-3.0.3/arcsecond/uploader/errors.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1060 2024-03-31 14:43:40.000000 arcsecond-3.0.3/arcsecond/uploader/logger.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     4725 2024-03-31 07:26:36.000000 arcsecond-3.0.3/arcsecond/uploader/uploader.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     2801 2024-03-31 07:23:32.000000 arcsecond-3.0.3/arcsecond/uploader/utils.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     3477 2024-03-31 14:44:07.000000 arcsecond-3.0.3/arcsecond/uploader/walker.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.639710 arcsecond-3.0.3/arcsecond.egg-info/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/PKG-INFO
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      877 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/SOURCES.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/dependency_links.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       49 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/entry_points.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/not-zip-safe
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       55 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/requires.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       16 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/top_level.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       61 2024-04-08 12:34:40.645298 arcsecond-3.0.3/setup.cfg
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1621 2024-03-24 20:33:09.000000 arcsecond-3.0.3/setup.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.636900 arcsecond-3.0.3/tests/
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.643977 arcsecond-3.0.3/tests/cli/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.0.3/tests/cli/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1551 2024-03-31 12:07:38.000000 arcsecond-3.0.3/tests/cli/test_cli_options.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1383 2024-03-29 18:20:59.000000 arcsecond-3.0.3/tests/cli/test_config.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.644655 arcsecond-3.0.3/tests/module/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.0.3/tests/module/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1133 2024-03-29 09:03:34.000000 arcsecond-3.0.3/tests/module/test_arcsecond_root.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1092 2024-03-29 18:42:28.000000 arcsecond-3.0.3/tests/module/test_login.py
```

### Comparing `arcsecond-3.0.2/LICENSE` & `arcsecond-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/PKG-INFO` & `arcsecond-3.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcsecond
-Version: 3.0.2
+Version: 3.0.3
 Summary:  CLI for arcsecond.io
 Home-page: https://github.com/arcsecond-io/cli
 Author: Cedric Foellmi
 Author-email: cedric@arcsecond.io
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `arcsecond-3.0.2/README.md` & `arcsecond-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond/api/config.py` & `arcsecond-3.0.3/arcsecond/api/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     @classmethod
     def file_path(cls) -> Path:
         _config_dir_path = ArcsecondConfig.dir_path()
         _config_file_path = _config_dir_path / 'config.ini'
         if ArcsecondConfig.__old_config_file_path().exists() and not _config_file_path.exists():
             _config_dir_path.mkdir(parents=True, exist_ok=True)
             shutil.move(str(ArcsecondConfig.__old_config_file_path()), str(_config_file_path))
+        elif not _config_file_path.exists():
+            _config_file_path.parents[0].mkdir(parents=True, exist_ok=True)
+            _config_file_path.touch()
         return _config_file_path
 
     @property
     def is_logged_in(self) -> bool:
         if self.__section is None:
             return False
         return self.__section.get('access_key') is not None or \
@@ -61,15 +64,18 @@
 
     @property
     def is_using_cli(self) -> Optional[bool]:
         return self.__state.is_using_cli
 
     @property
     def api_name(self) -> Optional[str]:
-        return self.__state.api_name
+        result = self.__state.api_name
+        if not result:
+            result = 'main'
+        return result
 
     @property
     def api_server(self) -> Optional[str]:
         result = self.__read_key('api_server')
         if self.api_name == 'main' and (result is None or result == ''):
             result = ARCSECOND_API_URL_PROD
         return result
```

### Comparing `arcsecond-3.0.2/arcsecond/api/endpoint.py` & `arcsecond-3.0.3/arcsecond/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond/api/main.py` & `arcsecond-3.0.3/arcsecond/api/main.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond/cli.py` & `arcsecond-3.0.3/arcsecond/cli.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond/options.py` & `arcsecond-3.0.3/arcsecond/options.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond/uploader/constants.py` & `arcsecond-3.0.3/arcsecond/uploader/constants.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond/uploader/context.py` & `arcsecond-3.0.3/arcsecond/uploader/context.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond/uploader/errors.py` & `arcsecond-3.0.3/arcsecond/uploader/errors.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond/uploader/logger.py` & `arcsecond-3.0.3/arcsecond/uploader/logger.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond/uploader/uploader.py` & `arcsecond-3.0.3/arcsecond/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond/uploader/utils.py` & `arcsecond-3.0.3/arcsecond/uploader/utils.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond/uploader/walker.py` & `arcsecond-3.0.3/arcsecond/uploader/walker.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/arcsecond.egg-info/PKG-INFO` & `arcsecond-3.0.3/arcsecond.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcsecond
-Version: 3.0.2
+Version: 3.0.3
 Summary:  CLI for arcsecond.io
 Home-page: https://github.com/arcsecond-io/cli
 Author: Cedric Foellmi
 Author-email: cedric@arcsecond.io
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `arcsecond-3.0.2/arcsecond.egg-info/SOURCES.txt` & `arcsecond-3.0.3/arcsecond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/setup.py` & `arcsecond-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/tests/cli/test_cli_options.py` & `arcsecond-3.0.3/tests/cli/test_cli_options.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/tests/cli/test_config.py` & `arcsecond-3.0.3/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/tests/module/test_arcsecond_root.py` & `arcsecond-3.0.3/tests/module/test_arcsecond_root.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.2/tests/module/test_login.py` & `arcsecond-3.0.3/tests/module/test_login.py`

 * *Files identical despite different names*

