# Comparing `tmp/transdoc-0.2.0.tar.gz` & `tmp/transdoc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transdoc-0.2.0.tar", max compression
+gzip compressed data, was "transdoc-0.2.1.tar", max compression
```

## Comparing `transdoc-0.2.0.tar` & `transdoc-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1073 2024-04-06 12:30:46.705493 transdoc-0.2.0/LICENSE
--rw-r--r--   0        0        0     3931 2024-04-06 12:30:46.705493 transdoc-0.2.0/README.md
--rw-r--r--   0        0        0     1463 2024-04-06 12:30:46.705493 transdoc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6006 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__cli/__init__.py
--rw-r--r--   0        0        0     1277 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__cli/mutex.py
--rw-r--r--   0        0        0      648 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__collect_rules.py
--rw-r--r--   0        0        0       74 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__consts.py
--rw-r--r--   0        0        0      337 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__init__.py
--rw-r--r--   0        0        0      201 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__main__.py
--rw-r--r--   0        0        0      228 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__rule.py
--rw-r--r--   0        0        0    10125 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__transformer.py
--rw-r--r--   0        0        0      888 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/errors.py
--rw-r--r--   0        0        0        0 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/py.typed
--rw-r--r--   0        0        0     4661 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/rules/__attributes.py
--rw-r--r--   0        0        0      387 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/rules/__file_contents.py
--rw-r--r--   0        0        0      381 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/rules/__init__.py
--rw-r--r--   0        0        0     1294 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/rules/__markdown_docs_link.py
--rw-r--r--   0        0        0     5068 1970-01-01 00:00:00.000000 transdoc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-08 04:10:24.498050 transdoc-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3932 2024-04-08 04:10:24.498050 transdoc-0.2.1/README.md
+-rw-r--r--   0        0        0     1463 2024-04-08 04:10:24.498050 transdoc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1332 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/__cli/__init__.py
+-rw-r--r--   0        0        0     5093 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/__cli/main.py
+-rw-r--r--   0        0        0     1277 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/__cli/mutex.py
+-rw-r--r--   0        0        0      648 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/__collect_rules.py
+-rw-r--r--   0        0        0       74 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/__consts.py
+-rw-r--r--   0        0        0      358 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/__main__.py
+-rw-r--r--   0        0        0      228 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/__rule.py
+-rw-r--r--   0        0        0    10125 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/__transformer.py
+-rw-r--r--   0        0        0      888 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/errors.py
+-rw-r--r--   0        0        0        0 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/py.typed
+-rw-r--r--   0        0        0     4661 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/rules/__attributes.py
+-rw-r--r--   0        0        0      387 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/rules/__file_contents.py
+-rw-r--r--   0        0        0      381 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/rules/__init__.py
+-rw-r--r--   0        0        0     1294 2024-04-08 04:10:24.502050 transdoc-0.2.1/transdoc/rules/__markdown_docs_link.py
+-rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 transdoc-0.2.1/PKG-INFO
```

### Comparing `transdoc-0.2.0/LICENSE` & `transdoc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.0/README.md` & `transdoc-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -170,9 +170,9 @@
 ```
 
 In a file `build.py`:
 
 ```py
 import transdoc
 
-exit(transdoc.cli("src", "rules.py", "build_dir", force=True))
+exit(transdoc.main("src", "rules.py", "build_dir", force=True))
 ```
```

### Comparing `transdoc-0.2.0/pyproject.toml` & `transdoc-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transdoc"
-version = "0.2.0"
+version = "0.2.1"
 description = "A simple tool for transforming Python docstrings by embedding results from Python function calls"
 authors = ["Miguel Guthridge <hello@miguelguthridge.com>"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/MiguelGuthridge/transdoc"
 # documentation = "https://miguelguthridge.github.io/transdoc/"
```

### Comparing `transdoc-0.2.0/transdoc/__cli/__init__.py` & `transdoc-0.2.1/transdoc/__cli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-"""
-# Transdoc / CLI / Main
-
-Main entrypoint to the Transdoc CLI.
-"""
 import importlib.util
 import os
 import sys
-import click
 from pathlib import Path
 from dataclasses import dataclass
 from typing import Optional
 from types import ModuleType
 from traceback import print_exception
 import importlib
-from .mutex import Mutex
 
-from transdoc import VERSION, transform
+from transdoc import transform
+from transdoc.__consts import VERSION
 from transdoc.errors import TransdocTransformationError
 from transdoc.__collect_rules import collect_rules
 
 
 def display_error_list(errors: list[str]) -> int:
     """
     Display errors and exit the program
@@ -73,51 +67,15 @@
 @dataclass
 class FileMapping:
     input: Path
     output: Optional[Path]
     transform: bool
 
 
-@click.command("transdoc")
-@click.argument(
-    'input',
-    type=click.Path(exists=True, path_type=Path),
-    # help='Path to the input file or directory',
-)
-@click.option(
-    '-r',
-    '--rule-file',
-    type=click.Path(exists=True, path_type=Path),
-    required=True,
-    help='Path to any Python file/module containing rules for Transdoc to use',
-)
-@click.option(
-    '-o',
-    '--output',
-    type=click.Path(exists=False, path_type=Path),
-    help='Path to the output file or directory',
-    cls=Mutex,
-    mutex_with=["dryrun"],
-)
-@click.option(
-    '-d',
-    '--dryrun',
-    is_flag=True,
-    help="Don't produce any output files",
-)
-@click.option(
-    '-f',
-    '--force',
-    is_flag=True,
-    help='Forcefully overwrite the output file/directory',
-    cls=Mutex,
-    mutex_with=["dryrun"],
-)
-@click.version_option(VERSION)
-def cli(
+def main(
     input: Path,
     rule_file: Path,
     output: Optional[Path] = None,
     *,
     dryrun: bool = False,
     force: bool = False,
 ) -> int:
```

### Comparing `transdoc-0.2.0/transdoc/__cli/mutex.py` & `transdoc-0.2.1/transdoc/__cli/mutex.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.0/transdoc/__collect_rules.py` & `transdoc-0.2.1/transdoc/__collect_rules.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.0/transdoc/__transformer.py` & `transdoc-0.2.1/transdoc/__transformer.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.0/transdoc/errors.py` & `transdoc-0.2.1/transdoc/errors.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.0/transdoc/rules/__attributes.py` & `transdoc-0.2.1/transdoc/rules/__attributes.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.0/transdoc/rules/__markdown_docs_link.py` & `transdoc-0.2.1/transdoc/rules/__markdown_docs_link.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.0/PKG-INFO` & `transdoc-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transdoc
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple tool for transforming Python docstrings by embedding results from Python function calls
 Home-page: https://github.com/MiguelGuthridge/transdoc
 License: MIT
 Keywords: documentation,source,transform,parse,pre-processor
 Author: Miguel Guthridge
 Author-email: hello@miguelguthridge.com
 Requires-Python: >=3.10,<4.0
@@ -197,10 +197,10 @@
 ```
 
 In a file `build.py`:
 
 ```py
 import transdoc
 
-exit(transdoc.cli("src", "rules.py", "build_dir", force=True))
+exit(transdoc.main("src", "rules.py", "build_dir", force=True))
 ```
```

