# Comparing `tmp/minchin.md-it.fancy-tasklists-1.0.0.tar.gz` & `tmp/minchin.md-it.fancy-tasklists-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minchin.md-it.fancy-tasklists-1.0.0.tar", last modified: Sat Mar 30 23:21:41 2024, max compression
+gzip compressed data, was "minchin.md-it.fancy-tasklists-1.1.0.tar", last modified: Mon Apr  8 00:50:26 2024, max compression
```

## Comparing `minchin.md-it.fancy-tasklists-1.0.0.tar` & `minchin.md-it.fancy-tasklists-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 23:21:41.599102 minchin.md-it.fancy-tasklists-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-03-30 23:21:41.591102 minchin.md-it.fancy-tasklists-1.0.0/.requirements/
--rw-rw-rw-   0        0        0       16 2024-02-21 01:56:24.000000 minchin.md-it.fancy-tasklists-1.0.0/.requirements/base.in
--rw-rw-rw-   0        0        0       43 2024-02-21 02:30:39.000000 minchin.md-it.fancy-tasklists-1.0.0/.requirements/dev.in
--rw-rw-rw-   0        0        0     2476 2024-03-30 23:21:41.598101 minchin.md-it.fancy-tasklists-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1293 2024-03-30 22:54:02.000000 minchin.md-it.fancy-tasklists-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-30 23:21:41.588101 minchin.md-it.fancy-tasklists-1.0.0/minchin/
-drwxrwxrwx   0        0        0        0 2024-03-30 23:21:41.588101 minchin.md-it.fancy-tasklists-1.0.0/minchin/md_it/
-drwxrwxrwx   0        0        0        0 2024-03-30 23:21:41.596102 minchin.md-it.fancy-tasklists-1.0.0/minchin/md_it/fancy_tasklists/
--rw-rw-rw-   0        0        0     6889 2024-03-30 23:21:34.000000 minchin.md-it.fancy-tasklists-1.0.0/minchin/md_it/fancy_tasklists/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 23:21:41.597102 minchin.md-it.fancy-tasklists-1.0.0/minchin.md_it.fancy_tasklists.egg-info/
--rw-rw-rw-   0        0        0     2476 2024-03-30 23:21:41.000000 minchin.md-it.fancy-tasklists-1.0.0/minchin.md_it.fancy_tasklists.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-03-30 23:21:41.000000 minchin.md-it.fancy-tasklists-1.0.0/minchin.md_it.fancy_tasklists.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 23:21:41.000000 minchin.md-it.fancy-tasklists-1.0.0/minchin.md_it.fancy_tasklists.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-03-30 23:21:41.000000 minchin.md-it.fancy-tasklists-1.0.0/minchin.md_it.fancy_tasklists.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-30 23:21:41.000000 minchin.md-it.fancy-tasklists-1.0.0/minchin.md_it.fancy_tasklists.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2476 2024-03-30 23:14:26.000000 minchin.md-it.fancy-tasklists-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-30 23:21:41.599102 minchin.md-it.fancy-tasklists-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 00:50:26.257055 minchin.md-it.fancy-tasklists-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-08 00:50:26.236057 minchin.md-it.fancy-tasklists-1.1.0/.requirements/
+-rw-rw-rw-   0        0        0       16 2024-02-21 01:56:24.000000 minchin.md-it.fancy-tasklists-1.1.0/.requirements/base.in
+-rw-rw-rw-   0        0        0       43 2024-02-21 02:30:39.000000 minchin.md-it.fancy-tasklists-1.1.0/.requirements/dev.in
+-rw-rw-rw-   0        0        0     2476 2024-04-08 00:50:26.257055 minchin.md-it.fancy-tasklists-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1293 2024-03-30 22:54:02.000000 minchin.md-it.fancy-tasklists-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-08 00:50:26.233055 minchin.md-it.fancy-tasklists-1.1.0/minchin/
+drwxrwxrwx   0        0        0        0 2024-04-08 00:50:26.233055 minchin.md-it.fancy-tasklists-1.1.0/minchin/md_it/
+drwxrwxrwx   0        0        0        0 2024-04-08 00:50:26.253055 minchin.md-it.fancy-tasklists-1.1.0/minchin/md_it/fancy_tasklists/
+-rw-rw-rw-   0        0        0     6899 2024-04-08 00:50:10.000000 minchin.md-it.fancy-tasklists-1.1.0/minchin/md_it/fancy_tasklists/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:50:26.253055 minchin.md-it.fancy-tasklists-1.1.0/minchin.md_it.fancy_tasklists.egg-info/
+-rw-rw-rw-   0        0        0     2476 2024-04-08 00:50:26.000000 minchin.md-it.fancy-tasklists-1.1.0/minchin.md_it.fancy_tasklists.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-04-08 00:50:26.000000 minchin.md-it.fancy-tasklists-1.1.0/minchin.md_it.fancy_tasklists.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 00:50:26.000000 minchin.md-it.fancy-tasklists-1.1.0/minchin.md_it.fancy_tasklists.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-08 00:50:26.000000 minchin.md-it.fancy-tasklists-1.1.0/minchin.md_it.fancy_tasklists.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 00:50:26.000000 minchin.md-it.fancy-tasklists-1.1.0/minchin.md_it.fancy_tasklists.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2476 2024-03-30 23:14:26.000000 minchin.md-it.fancy-tasklists-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 00:50:26.258055 minchin.md-it.fancy-tasklists-1.1.0/setup.cfg
```

### Comparing `minchin.md-it.fancy-tasklists-1.0.0/PKG-INFO` & `minchin.md-it.fancy-tasklists-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minchin.md-it.fancy-tasklists
-Version: 1.0.0
+Version: 1.1.0
 Summary: Fancy Tasklists, for Markdown-IT-py
 Author-email: William Minchin <w_minchin@hotmail.com>
 Maintainer-email: William Minchin <w_minchin@hotmail.com>
 License: ISC
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/minchin.md-it.fancy-tasklists/issues
 Project-URL: Repository, https://github.com/MinchinWeb/minchin.md-it.fancy-tasklists
 Project-URL: Changelog, https://github.com/MinchinWeb/minchin.md-it.fancy-tasklists/blob/master/CHANGELOG.rst
```

### Comparing `minchin.md-it.fancy-tasklists-1.0.0/README.rst` & `minchin.md-it.fancy-tasklists-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `minchin.md-it.fancy-tasklists-1.0.0/minchin/md_it/fancy_tasklists/__init__.py` & `minchin.md-it.fancy-tasklists-1.1.0/minchin/md_it/fancy_tasklists/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Builds task/todo lists out of markdown lists with items starting with [ ]
 (and many valid filler characters).
 """
 
 # Extended by William Minchin
 # Ported to Python by Wolmar Nyberg Åkerström from https://github.com/revin/markdown-it-task-lists
+#
 # ISC License
 # Copyright (c) 2016-18 Revin Guillen
 # Copyright (c) Wolmar Nyberg Åkerström
 # Copyright (c) 2024 William Minchin
 #
 # Permission to use, copy, modify, and/or distribute this software for any
 # purpose with or without fee is hereby granted, provided that the above
@@ -29,30 +30,30 @@
 
 from markdown_it import MarkdownIt
 from markdown_it.rules_core import StateCore
 from markdown_it.token import Token
 
 __title__ = "minchin.md-it.fancy-tasklists"
 __tagline__ = "Fancy Tasklists, for Markdown-IT-Py"
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 __author__ = "William Minchin"
 __email__ = "w_minchin@hotmail.com"
 __license__ = "ISC License"
 __copyright__ = "Copyright 2024 William Minchin"
 __url__ = "https://github.com/MinchinWeb/minchin.md-it.fancy-tasklists"
 
 
 # Regex string to match a whitespace character, as specified in
 # https://github.github.com/gfm/#whitespace-character
 # (spec version 0.29-gfm (2019-04-06))
 _GFM_WHITESPACE_RE = r"[ \t\n\v\f\r]"
 
 # Characters that can be valid "filler"
 # does not include the space
-_VALID_FILLER = r'a-zA-Z0-9/\-><?!*"@\+&~🚿'
+_VALID_FILLER = r'a-zA-Z0-9/\-><?!*"@\+&~🚿🦷⛪'
 
 
 def fancy_tasklists_plugin(
     md: MarkdownIt,
     enabled: bool = False,
     label: bool = False,
     label_after: bool = False,
```

### Comparing `minchin.md-it.fancy-tasklists-1.0.0/minchin.md_it.fancy_tasklists.egg-info/PKG-INFO` & `minchin.md-it.fancy-tasklists-1.1.0/minchin.md_it.fancy_tasklists.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minchin.md-it.fancy-tasklists
-Version: 1.0.0
+Version: 1.1.0
 Summary: Fancy Tasklists, for Markdown-IT-py
 Author-email: William Minchin <w_minchin@hotmail.com>
 Maintainer-email: William Minchin <w_minchin@hotmail.com>
 License: ISC
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/minchin.md-it.fancy-tasklists/issues
 Project-URL: Repository, https://github.com/MinchinWeb/minchin.md-it.fancy-tasklists
 Project-URL: Changelog, https://github.com/MinchinWeb/minchin.md-it.fancy-tasklists/blob/master/CHANGELOG.rst
```

### Comparing `minchin.md-it.fancy-tasklists-1.0.0/pyproject.toml` & `minchin.md-it.fancy-tasklists-1.1.0/pyproject.toml`

 * *Files identical despite different names*

