# Comparing `tmp/mkdocs-alias-plugin-0.8.0.tar.gz` & `tmp/mkdocs-alias-plugin-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-alias-plugin-0.8.0.tar", last modified: Sat Apr  6 22:50:37 2024, max compression
+gzip compressed data, was "mkdocs-alias-plugin-0.8.1.tar", last modified: Mon Apr  8 14:48:40 2024, max compression
```

## Comparing `mkdocs-alias-plugin-0.8.0.tar` & `mkdocs-alias-plugin-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:50:37.365961 mkdocs-alias-plugin-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 22:50:32.000000 mkdocs-alias-plugin-0.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-04-06 22:50:37.365961 mkdocs-alias-plugin-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-06 22:50:32.000000 mkdocs-alias-plugin-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:50:37.365961 mkdocs-alias-plugin-0.8.0/alias/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:50:32.000000 mkdocs-alias-plugin-0.8.0/alias/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-06 22:50:32.000000 mkdocs-alias-plugin-0.8.0/alias/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:50:37.365961 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 22:50:37.365961 mkdocs-alias-plugin-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-06 22:50:32.000000 mkdocs-alias-plugin-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:48:40.039539 mkdocs-alias-plugin-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 14:48:31.000000 mkdocs-alias-plugin-0.8.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-08 14:48:40.039539 mkdocs-alias-plugin-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-08 14:48:31.000000 mkdocs-alias-plugin-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:48:40.039539 mkdocs-alias-plugin-0.8.1/alias/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:48:31.000000 mkdocs-alias-plugin-0.8.1/alias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-04-08 14:48:31.000000 mkdocs-alias-plugin-0.8.1/alias/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:48:40.039539 mkdocs-alias-plugin-0.8.1/mkdocs_alias_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-08 14:48:40.000000 mkdocs-alias-plugin-0.8.1/mkdocs_alias_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 14:48:40.000000 mkdocs-alias-plugin-0.8.1/mkdocs_alias_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:48:40.000000 mkdocs-alias-plugin-0.8.1/mkdocs_alias_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 14:48:40.000000 mkdocs-alias-plugin-0.8.1/mkdocs_alias_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 14:48:40.000000 mkdocs-alias-plugin-0.8.1/mkdocs_alias_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 14:48:40.000000 mkdocs-alias-plugin-0.8.1/mkdocs_alias_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:48:40.039539 mkdocs-alias-plugin-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-08 14:48:31.000000 mkdocs-alias-plugin-0.8.1/setup.py
```

### Comparing `mkdocs-alias-plugin-0.8.0/LICENSE.md` & `mkdocs-alias-plugin-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-alias-plugin-0.8.0/PKG-INFO` & `mkdocs-alias-plugin-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-alias-plugin
-Version: 0.8.0
+Version: 0.8.1
 Summary: An MkDocs plugin allowing links to your pages using a custom alias
 Home-page: https://github.com/eddyluten/mkdocs-alias-plugin
 Author: Eddy Luten
 Author-email: eddyluten@gmail.com
 License: MIT
 Keywords: mkdocs python markdown alias link wiki
 Classifier: License :: OSI Approved :: MIT License
@@ -184,14 +184,18 @@
 
 ```zsh
 pylint $(git ls-files '*.py') && pytest -vv
 ```
 
 ## Changelog
 
+## 0.8.1
+
+**Bug Fix:** fixes a bug where annotations would break older versions of Python 3. Bug report: [#9](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/9).
+
 ## 0.8.0
 
 This release adds functionality to replace the titles of aliases containing anchors with the text of the heading that defines them. Enable this feature by setting the plugin option `use_anchor_titles` to true. Feature request: [#8](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/8).
 
 ### 0.7.1
 
 **Bug Fix:** fixes a bug where any alias with the word "text" would break the plugin due to faulty logic. Bug report: [#7](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/7).
```

### Comparing `mkdocs-alias-plugin-0.8.0/README.md` & `mkdocs-alias-plugin-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,18 @@
 
 ```zsh
 pylint $(git ls-files '*.py') && pytest -vv
 ```
 
 ## Changelog
 
+## 0.8.1
+
+**Bug Fix:** fixes a bug where annotations would break older versions of Python 3. Bug report: [#9](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/9).
+
 ## 0.8.0
 
 This release adds functionality to replace the titles of aliases containing anchors with the text of the heading that defines them. Enable this feature by setting the plugin option `use_anchor_titles` to true. Feature request: [#8](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/8).
 
 ### 0.7.1
 
 **Bug Fix:** fixes a bug where any alias with the word "text" would break the plugin due to faulty logic. Bug report: [#7](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/7).
```

### Comparing `mkdocs-alias-plugin-0.8.0/alias/plugin.py` & `mkdocs-alias-plugin-0.8.1/alias/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """mkdocs-alias-plugin
 
 An MkDocs plugin allowing links to your pages using a custom alias.
 """
+from __future__ import annotations
 
 import logging
 import re
 from typing import Match, TypedDict
 
 from markdown import Markdown
 from mkdocs.config import config_options
```

### Comparing `mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/PKG-INFO` & `mkdocs-alias-plugin-0.8.1/mkdocs_alias_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-alias-plugin
-Version: 0.8.0
+Version: 0.8.1
 Summary: An MkDocs plugin allowing links to your pages using a custom alias
 Home-page: https://github.com/eddyluten/mkdocs-alias-plugin
 Author: Eddy Luten
 Author-email: eddyluten@gmail.com
 License: MIT
 Keywords: mkdocs python markdown alias link wiki
 Classifier: License :: OSI Approved :: MIT License
@@ -184,14 +184,18 @@
 
 ```zsh
 pylint $(git ls-files '*.py') && pytest -vv
 ```
 
 ## Changelog
 
+## 0.8.1
+
+**Bug Fix:** fixes a bug where annotations would break older versions of Python 3. Bug report: [#9](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/9).
+
 ## 0.8.0
 
 This release adds functionality to replace the titles of aliases containing anchors with the text of the heading that defines them. Enable this feature by setting the plugin option `use_anchor_titles` to true. Feature request: [#8](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/8).
 
 ### 0.7.1
 
 **Bug Fix:** fixes a bug where any alias with the word "text" would break the plugin due to faulty logic. Bug report: [#7](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/7).
```

### Comparing `mkdocs-alias-plugin-0.8.0/setup.py` & `mkdocs-alias-plugin-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='mkdocs-alias-plugin',
-    version='0.8.0',
+    version='0.8.1',
     description=
     'An MkDocs plugin allowing links to your pages using a custom alias',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown alias link wiki',
     url='https://github.com/eddyluten/mkdocs-alias-plugin',
     author='Eddy Luten',
```

