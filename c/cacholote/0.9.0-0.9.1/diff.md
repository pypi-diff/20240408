# Comparing `tmp/cacholote-0.9.0.tar.gz` & `tmp/cacholote-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacholote-0.9.0.tar", last modified: Mon Mar 18 14:25:31 2024, max compression
+gzip compressed data, was "cacholote-0.9.1.tar", last modified: Fri Mar 22 15:36:51 2024, max compression
```

## Comparing `cacholote-0.9.0.tar` & `cacholote-0.9.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:31.537638 cacholote-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-18 14:25:20.000000 cacholote-0.9.0/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:31.525638 cacholote-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:31.529638 cacholote-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-03-18 14:25:20.000000 cacholote-0.9.0/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-03-18 14:25:20.000000 cacholote-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-18 14:25:20.000000 cacholote-0.9.0/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-18 14:25:20.000000 cacholote-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-18 14:25:20.000000 cacholote-0.9.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-18 14:25:20.000000 cacholote-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-18 14:25:20.000000 cacholote-0.9.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    17003 2024-03-18 14:25:31.533638 cacholote-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-18 14:25:20.000000 cacholote-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:31.529638 cacholote-0.9.0/cacholote/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-18 14:25:20.000000 cacholote-0.9.0/cacholote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-18 14:25:20.000000 cacholote-0.9.0/cacholote/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-03-18 14:25:20.000000 cacholote-0.9.0/cacholote/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-03-18 14:25:20.000000 cacholote-0.9.0/cacholote/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-18 14:25:20.000000 cacholote-0.9.0/cacholote/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-18 14:25:20.000000 cacholote-0.9.0/cacholote/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-03-18 14:25:20.000000 cacholote-0.9.0/cacholote/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)    14391 2024-03-18 14:25:20.000000 cacholote-0.9.0/cacholote/extra_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:20.000000 cacholote-0.9.0/cacholote/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-18 14:25:20.000000 cacholote-0.9.0/cacholote/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-18 14:25:31.000000 cacholote-0.9.0/cacholote/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:31.533638 cacholote-0.9.0/cacholote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17003 2024-03-18 14:25:31.000000 cacholote-0.9.0/cacholote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-18 14:25:31.000000 cacholote-0.9.0/cacholote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 14:25:31.000000 cacholote-0.9.0/cacholote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-18 14:25:31.000000 cacholote-0.9.0/cacholote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-18 14:25:31.000000 cacholote-0.9.0/cacholote.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:31.533638 cacholote-0.9.0/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-18 14:25:20.000000 cacholote-0.9.0/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-18 14:25:20.000000 cacholote-0.9.0/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:31.533638 cacholote-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-18 14:25:20.000000 cacholote-0.9.0/docs/DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-18 14:25:20.000000 cacholote-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-18 14:25:20.000000 cacholote-0.9.0/docs/OBJECT-STORAGE-DESIGN.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:31.533638 cacholote-0.9.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:20.000000 cacholote-0.9.0/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:31.533638 cacholote-0.9.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:20.000000 cacholote-0.9.0/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-18 14:25:20.000000 cacholote-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-18 14:25:20.000000 cacholote-0.9.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-18 14:25:20.000000 cacholote-0.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-18 14:25:20.000000 cacholote-0.9.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-18 14:25:20.000000 cacholote-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 14:25:31.537638 cacholote-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:31.533638 cacholote-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-18 14:25:20.000000 cacholote-0.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-18 14:25:20.000000 cacholote-0.9.0/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-18 14:25:20.000000 cacholote-0.9.0/tests/test_01_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-18 14:25:20.000000 cacholote-0.9.0/tests/test_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-18 14:25:20.000000 cacholote-0.9.0/tests/test_10_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-03-18 14:25:20.000000 cacholote-0.9.0/tests/test_20_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-03-18 14:25:20.000000 cacholote-0.9.0/tests/test_30_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-03-18 14:25:20.000000 cacholote-0.9.0/tests/test_40_xarray_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-03-18 14:25:20.000000 cacholote-0.9.0/tests/test_50_io_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-03-18 14:25:20.000000 cacholote-0.9.0/tests/test_60_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.158450 cacholote-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-22 15:36:40.000000 cacholote-0.9.1/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.150450 cacholote-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.150450 cacholote-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-03-22 15:36:40.000000 cacholote-0.9.1/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-03-22 15:36:40.000000 cacholote-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-22 15:36:40.000000 cacholote-0.9.1/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-22 15:36:40.000000 cacholote-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-22 15:36:40.000000 cacholote-0.9.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-22 15:36:40.000000 cacholote-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-22 15:36:40.000000 cacholote-0.9.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    17003 2024-03-22 15:36:51.158450 cacholote-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-22 15:36:40.000000 cacholote-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.154450 cacholote-0.9.1/cacholote/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14391 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/extra_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.158450 cacholote-0.9.1/cacholote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17003 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.154450 cacholote-0.9.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-22 15:36:40.000000 cacholote-0.9.1/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-22 15:36:40.000000 cacholote-0.9.1/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.154450 cacholote-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/OBJECT-STORAGE-DESIGN.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.154450 cacholote-0.9.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.154450 cacholote-0.9.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-22 15:36:40.000000 cacholote-0.9.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-22 15:36:40.000000 cacholote-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 15:36:51.158450 cacholote-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.158450 cacholote-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_01_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_10_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_20_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_30_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_40_xarray_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_50_io_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_60_clean.py
```

### Comparing `cacholote-0.9.0/.cruft.json` & `cacholote-0.9.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/.github/workflows/on-push.yml` & `cacholote-0.9.1/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/.gitignore` & `cacholote-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/.pre-commit-config.yaml` & `cacholote-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/LICENSE` & `cacholote-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/Makefile` & `cacholote-0.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/PKG-INFO` & `cacholote-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.9.0
+Version: 0.9.1
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-0.9.0/README.md` & `cacholote-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/cacholote/__init__.py` & `cacholote-0.9.1/cacholote/__init__.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/cacholote/cache.py` & `cacholote-0.9.1/cacholote/cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/cacholote/clean.py` & `cacholote-0.9.1/cacholote/clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,23 +138,23 @@
         unknown_sizes = {
             k: v for k, v in self.file_sizes.items() if k not in files_to_skip
         }
         if unknown_sizes:
             with config.get().instantiated_sessionmaker() as session:
                 for cache_entry in session.scalars(sa.select(database.CacheEntry)):
                     for file in _get_files_from_cache_entry(cache_entry):
-                        unknown_sizes.pop(file)
+                        unknown_sizes.pop(file, 0)
         return unknown_sizes
 
     def delete_unknown_files(
         self, lock_validity_period: float | None, recursive: bool
     ) -> None:
         unknown_sizes = self.get_unknown_sizes(lock_validity_period)
         for urlpath in unknown_sizes:
-            self.file_sizes.pop(urlpath)
+            self.file_sizes.pop(urlpath, 0)
         self.remove_files(
             list(unknown_sizes),
             recursive=recursive,
             msg="deleting unknown files",
         )
         self.log_disk_usage()
```

### Comparing `cacholote-0.9.0/cacholote/config.py` & `cacholote-0.9.1/cacholote/config.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/cacholote/database.py` & `cacholote-0.9.1/cacholote/database.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/cacholote/decode.py` & `cacholote-0.9.1/cacholote/decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/cacholote/encode.py` & `cacholote-0.9.1/cacholote/encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/cacholote/extra_encoders.py` & `cacholote-0.9.1/cacholote/extra_encoders.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/cacholote/utils.py` & `cacholote-0.9.1/cacholote/utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/cacholote.egg-info/PKG-INFO` & `cacholote-0.9.1/cacholote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.9.0
+Version: 0.9.1
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-0.9.0/cacholote.egg-info/SOURCES.txt` & `cacholote-0.9.1/cacholote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/ci/environment-ci.yml` & `cacholote-0.9.1/ci/environment-ci.yml`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/docs/DESIGN.rst` & `cacholote-0.9.1/docs/DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/docs/Makefile` & `cacholote-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/docs/OBJECT-STORAGE-DESIGN.rst` & `cacholote-0.9.1/docs/OBJECT-STORAGE-DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/docs/conf.py` & `cacholote-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/docs/make.bat` & `cacholote-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/pyproject.toml` & `cacholote-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/tests/conftest.py` & `cacholote-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/tests/test_01_settings.py` & `cacholote-0.9.1/tests/test_01_settings.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/tests/test_02_utils.py` & `cacholote-0.9.1/tests/test_02_utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/tests/test_10_decode.py` & `cacholote-0.9.1/tests/test_10_decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/tests/test_20_encode.py` & `cacholote-0.9.1/tests/test_20_encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/tests/test_30_cache.py` & `cacholote-0.9.1/tests/test_30_cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/tests/test_40_xarray_encoder.py` & `cacholote-0.9.1/tests/test_40_xarray_encoder.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/tests/test_50_io_encoder.py` & `cacholote-0.9.1/tests/test_50_io_encoder.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.0/tests/test_60_clean.py` & `cacholote-0.9.1/tests/test_60_clean.py`

 * *Files identical despite different names*

