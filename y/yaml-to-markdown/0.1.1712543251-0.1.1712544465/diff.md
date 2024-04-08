# Comparing `tmp/yaml-to-markdown-0.1.1712543251.tar.gz` & `tmp/yaml-to-markdown-0.1.1712544465.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-to-markdown-0.1.1712543251.tar", last modified: Mon Apr  8 02:27:31 2024, max compression
+gzip compressed data, was "yaml-to-markdown-0.1.1712544465.tar", last modified: Mon Apr  8 02:47:46 2024, max compression
```

## Comparing `yaml-to-markdown-0.1.1712543251.tar` & `yaml-to-markdown-0.1.1712544465.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:27:31.660256 yaml-to-markdown-0.1.1712543251/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-08 02:27:31.660256 yaml-to-markdown-0.1.1712543251/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 02:27:31.660256 yaml-to-markdown-0.1.1712543251/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:27:31.656256 yaml-to-markdown-0.1.1712543251/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:27:31.656256 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/convert_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/md_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/md_converter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:27:31.660256 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:47:46.077515 yaml-to-markdown-0.1.1712544465/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 02:46:51.000000 yaml-to-markdown-0.1.1712544465/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-08 02:47:46.077515 yaml-to-markdown-0.1.1712544465/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-08 02:46:51.000000 yaml-to-markdown-0.1.1712544465/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 02:47:46.077515 yaml-to-markdown-0.1.1712544465/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-08 02:46:51.000000 yaml-to-markdown-0.1.1712544465/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:47:46.073516 yaml-to-markdown-0.1.1712544465/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:47:46.073516 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:46:51.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-08 02:46:51.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-08 02:46:51.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/convert_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-08 02:46:51.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/md_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-08 02:46:51.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/md_converter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 02:46:51.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 02:46:51.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:47:46.073516 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-08 02:47:45.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 02:47:46.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 02:47:45.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 02:47:45.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 02:47:45.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 02:47:45.000000 yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown.egg-info/top_level.txt
```

### Comparing `yaml-to-markdown-0.1.1712543251/LICENSE` & `yaml-to-markdown-0.1.1712544465/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712543251/PKG-INFO` & `yaml-to-markdown-0.1.1712544465/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-to-markdown
-Version: 0.1.1712543251
+Version: 0.1.1712544465
 Summary: Converts a YAML/JSON file or python Dict/List to a Markdown file
 Home-page: https://anevis.github.io/yaml-to-markdown/
 Author: anevis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `yaml-to-markdown-0.1.1712543251/README.md` & `yaml-to-markdown-0.1.1712544465/README.md`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712543251/setup.py` & `yaml-to-markdown-0.1.1712544465/setup.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/convert.py` & `yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/convert.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/convert_test.py` & `yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/convert_test.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/md_converter.py` & `yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/md_converter.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/md_converter_test.py` & `yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown/md_converter_test.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/PKG-INFO` & `yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-to-markdown
-Version: 0.1.1712543251
+Version: 0.1.1712544465
 Summary: Converts a YAML/JSON file or python Dict/List to a Markdown file
 Home-page: https://anevis.github.io/yaml-to-markdown/
 Author: anevis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/SOURCES.txt` & `yaml-to-markdown-0.1.1712544465/src/yaml_to_markdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

