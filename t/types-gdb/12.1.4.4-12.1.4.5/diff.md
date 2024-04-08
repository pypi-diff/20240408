# Comparing `tmp/types-gdb-12.1.4.4.tar.gz` & `tmp/types-gdb-12.1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-gdb-12.1.4.4.tar", last modified: Tue Mar 14 15:21:28 2023, max compression
+gzip compressed data, was "types-gdb-12.1.4.5.tar", last modified: Sun Aug 13 21:12:02 2023, max compression
```

## Comparing `types-gdb-12.1.4.4.tar` & `types-gdb-12.1.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:21:28.326492 types-gdb-12.1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-14 15:21:27.000000 types-gdb-12.1.4.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-14 15:21:27.000000 types-gdb-12.1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-14 15:21:28.326492 types-gdb-12.1.4.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:21:28.326492 types-gdb-12.1.4.4/gdb-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-14 15:21:27.000000 types-gdb-12.1.4.4/gdb-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    20112 2023-03-14 15:21:05.000000 types-gdb-12.1.4.4/gdb-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-03-14 15:21:05.000000 types-gdb-12.1.4.4/gdb-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:21:05.000000 types-gdb-12.1.4.4/gdb-stubs/printing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-14 15:21:05.000000 types-gdb-12.1.4.4/gdb-stubs/prompt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-14 15:21:05.000000 types-gdb-12.1.4.4/gdb-stubs/types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-14 15:21:05.000000 types-gdb-12.1.4.4/gdb-stubs/unwinder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-14 15:21:05.000000 types-gdb-12.1.4.4/gdb-stubs/xmethod.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 15:21:28.326492 types-gdb-12.1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-03-14 15:21:27.000000 types-gdb-12.1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:21:28.326492 types-gdb-12.1.4.4/types_gdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-14 15:21:28.000000 types-gdb-12.1.4.4/types_gdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-14 15:21:28.000000 types-gdb-12.1.4.4/types_gdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 15:21:28.000000 types-gdb-12.1.4.4/types_gdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-14 15:21:28.000000 types-gdb-12.1.4.4/types_gdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 21:12:02.061986 types-gdb-12.1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-08-13 21:12:01.000000 types-gdb-12.1.4.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-13 21:12:01.000000 types-gdb-12.1.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-13 21:12:02.061986 types-gdb-12.1.4.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 21:12:02.061986 types-gdb-12.1.4.5/gdb-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-13 21:12:01.000000 types-gdb-12.1.4.5/gdb-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    20112 2023-08-13 21:10:50.000000 types-gdb-12.1.4.5/gdb-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-13 21:10:50.000000 types-gdb-12.1.4.5/gdb-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-13 21:10:50.000000 types-gdb-12.1.4.5/gdb-stubs/printing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-13 21:10:50.000000 types-gdb-12.1.4.5/gdb-stubs/prompt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-13 21:10:50.000000 types-gdb-12.1.4.5/gdb-stubs/types.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-13 21:10:50.000000 types-gdb-12.1.4.5/gdb-stubs/unwinder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-13 21:10:50.000000 types-gdb-12.1.4.5/gdb-stubs/xmethod.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-13 21:12:02.061986 types-gdb-12.1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-13 21:12:01.000000 types-gdb-12.1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 21:12:02.061986 types-gdb-12.1.4.5/types_gdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-13 21:12:02.000000 types-gdb-12.1.4.5/types_gdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-13 21:12:02.000000 types-gdb-12.1.4.5/types_gdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-13 21:12:02.000000 types-gdb-12.1.4.5/types_gdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-13 21:12:02.000000 types-gdb-12.1.4.5/types_gdb.egg-info/top_level.txt
```

### Comparing `types-gdb-12.1.4.4/CHANGELOG.md` & `types-gdb-12.1.4.5/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 12.1.4.5 (2023-08-13)
+
+Fill in all missing `upstream_repository` fields (#10571)
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 12.1.4.4 (2023-03-14)
 
 Fix typos in `extra_description` fields (#9883)
 
 ## 12.1.4.3 (2023-02-01)
 
 Bump black to 23.1.0 (#9647)
```

### Comparing `types-gdb-12.1.4.4/PKG-INFO` & `types-gdb-12.1.4.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-gdb
-Version: 12.1.4.4
+Version: 12.1.4.5
 Summary: Typing stubs for gdb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/gdb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -24,8 +24,10 @@
 `gdb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/gdb. All fixes for
 types and metadata should be contributed there.
 
 Type hints for GDB's [Python API](https://sourceware.org/gdb/onlinedocs/gdb/Python-API.html). Note that this API is available only when running Python scripts under GDB: it is not possible to install the `gdb` package separately, for instance using `pip`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7e0b9b44dea0b170081cafd596c2804089dc2125`.
+This package was generated from typeshed commit `22b055a147b5d672bf7e1f58cc6bf52cc526b35f` and was tested
+with mypy 1.4.1, pyright 1.1.320, and
+pytype 2023.7.21.
```

### Comparing `types-gdb-12.1.4.4/gdb-stubs/__init__.pyi` & `types-gdb-12.1.4.5/gdb-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-gdb-12.1.4.4/gdb-stubs/events.pyi` & `types-gdb-12.1.4.5/gdb-stubs/events.pyi`

 * *Files identical despite different names*

### Comparing `types-gdb-12.1.4.4/gdb-stubs/printing.pyi` & `types-gdb-12.1.4.5/gdb-stubs/printing.pyi`

 * *Files identical despite different names*

### Comparing `types-gdb-12.1.4.4/gdb-stubs/types.pyi` & `types-gdb-12.1.4.5/gdb-stubs/types.pyi`

 * *Files identical despite different names*

### Comparing `types-gdb-12.1.4.4/gdb-stubs/xmethod.pyi` & `types-gdb-12.1.4.5/gdb-stubs/xmethod.pyi`

 * *Files identical despite different names*

### Comparing `types-gdb-12.1.4.4/setup.py` & `types-gdb-12.1.4.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 `gdb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/gdb. All fixes for
 types and metadata should be contributed there.
 
 Type hints for GDB's [Python API](https://sourceware.org/gdb/onlinedocs/gdb/Python-API.html). Note that this API is available only when running Python scripts under GDB: it is not possible to install the `gdb` package separately, for instance using `pip`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7e0b9b44dea0b170081cafd596c2804089dc2125`.
+This package was generated from typeshed commit `22b055a147b5d672bf7e1f58cc6bf52cc526b35f` and was tested
+with mypy 1.4.1, pyright 1.1.320, and
+pytype 2023.7.21.
 '''.lstrip()
 
 setup(name=name,
-      version="12.1.4.4",
+      version="12.1.4.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/gdb.md",
```

### Comparing `types-gdb-12.1.4.4/types_gdb.egg-info/PKG-INFO` & `types-gdb-12.1.4.5/types_gdb.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-gdb
-Version: 12.1.4.4
+Version: 12.1.4.5
 Summary: Typing stubs for gdb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/gdb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -24,8 +24,10 @@
 `gdb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/gdb. All fixes for
 types and metadata should be contributed there.
 
 Type hints for GDB's [Python API](https://sourceware.org/gdb/onlinedocs/gdb/Python-API.html). Note that this API is available only when running Python scripts under GDB: it is not possible to install the `gdb` package separately, for instance using `pip`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7e0b9b44dea0b170081cafd596c2804089dc2125`.
+This package was generated from typeshed commit `22b055a147b5d672bf7e1f58cc6bf52cc526b35f` and was tested
+with mypy 1.4.1, pyright 1.1.320, and
+pytype 2023.7.21.
```

