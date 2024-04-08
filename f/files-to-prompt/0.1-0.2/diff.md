# Comparing `tmp/files-to-prompt-0.1.tar.gz` & `tmp/files-to-prompt-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "files-to-prompt-0.1.tar", last modified: Fri Mar 22 15:48:59 2024, max compression
+gzip compressed data, was "files-to-prompt-0.2.tar", last modified: Mon Apr  8 05:40:47 2024, max compression
```

## Comparing `files-to-prompt-0.1.tar` & `files-to-prompt-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:48:59.313097 files-to-prompt-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-22 15:48:51.000000 files-to-prompt-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-03-22 15:48:59.313097 files-to-prompt-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-22 15:48:51.000000 files-to-prompt-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:48:59.309097 files-to-prompt-0.1/files_to_prompt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:48:51.000000 files-to-prompt-0.1/files_to_prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-22 15:48:51.000000 files-to-prompt-0.1/files_to_prompt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-22 15:48:51.000000 files-to-prompt-0.1/files_to_prompt/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:48:59.313097 files-to-prompt-0.1/files_to_prompt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-03-22 15:48:59.000000 files-to-prompt-0.1/files_to_prompt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-22 15:48:59.000000 files-to-prompt-0.1/files_to_prompt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:48:59.000000 files-to-prompt-0.1/files_to_prompt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-22 15:48:59.000000 files-to-prompt-0.1/files_to_prompt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-22 15:48:59.000000 files-to-prompt-0.1/files_to_prompt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-22 15:48:59.000000 files-to-prompt-0.1/files_to_prompt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-22 15:48:51.000000 files-to-prompt-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 15:48:59.313097 files-to-prompt-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:48:59.313097 files-to-prompt-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-22 15:48:51.000000 files-to-prompt-0.1/tests/test_files_to_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.618260 files-to-prompt-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 05:40:41.000000 files-to-prompt-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-08 05:40:47.618260 files-to-prompt-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-08 05:40:41.000000 files-to-prompt-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.614260 files-to-prompt-0.2/files_to_prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:41.000000 files-to-prompt-0.2/files_to_prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 05:40:41.000000 files-to-prompt-0.2/files_to_prompt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-08 05:40:41.000000 files-to-prompt-0.2/files_to_prompt/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.618260 files-to-prompt-0.2/files_to_prompt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-08 05:40:47.000000 files-to-prompt-0.2/files_to_prompt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 05:40:47.000000 files-to-prompt-0.2/files_to_prompt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:40:47.000000 files-to-prompt-0.2/files_to_prompt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 05:40:47.000000 files-to-prompt-0.2/files_to_prompt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 05:40:47.000000 files-to-prompt-0.2/files_to_prompt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 05:40:47.000000 files-to-prompt-0.2/files_to_prompt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-08 05:40:41.000000 files-to-prompt-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:40:47.618260 files-to-prompt-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.618260 files-to-prompt-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-04-08 05:40:41.000000 files-to-prompt-0.2/tests/test_files_to_prompt.py
```

### Comparing `files-to-prompt-0.1/LICENSE` & `files-to-prompt-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `files-to-prompt-0.1/PKG-INFO` & `files-to-prompt-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: files-to-prompt
-Version: 0.1
+Version: 0.2
 Summary: Concatenate a directory full of files into a single prompt for use with LLMs
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/files-to-prompt
 Project-URL: Changelog, https://github.com/simonw/files-to-prompt/releases
 Project-URL: Issues, https://github.com/simonw/files-to-prompt/issues
 Project-URL: CI, https://github.com/simonw/files-to-prompt/actions
@@ -27,45 +27,52 @@
 
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install files-to-prompt
 ```
+
 ## Usage
 
-To use `files-to-prompt`, provide the path to the directory you want to process:
+To use `files-to-prompt`, provide the path to one or more files or directories you want to process:
 
 ```bash
-files-to-prompt path/to/directory
+files-to-prompt path/to/file_or_directory [path/to/another/file_or_directory ...]
 ```
 
-This will output the contents of every file in the directory and its subdirectories, with each file preceded by its relative path and separated by `---`.
+This will output the contents of every file, with each file preceded by its relative path and separated by `---`.
 
 ### Options
 
 - `--include-hidden`: Include files and folders starting with `.` (hidden files and directories).
   ```bash
   files-to-prompt path/to/directory --include-hidden
   ```
 
 - `--ignore-gitignore`: Ignore `.gitignore` files and include all files.
   ```bash
   files-to-prompt path/to/directory --ignore-gitignore
   ```
 
+- `--ignore <pattern>`: Specify one or more patterns to ignore. Can be used multiple times.
+  ```bash
+  files-to-prompt path/to/directory --ignore "*.log" --ignore "temp*"
+  ```
+
 ### Example
 
 Suppose you have a directory structure like this:
 
 ```
 my_directory/
 ├── file1.txt
 ├── file2.txt
 ├── .hidden_file.txt
+├── temp.log
 └── subdirectory/
     └── file3.txt
 ```
 
 Running `files-to-prompt my_directory` will output:
 
 ```
@@ -88,23 +95,45 @@
 ```
 my_directory/.hidden_file.txt
 ---
 Contents of .hidden_file.txt
 ---
 ...
 ```
+
+If you run `files-to-prompt my_directory --ignore "*.log"`, the output will exclude `temp.log`:
+
+```
+my_directory/file1.txt
+---
+Contents of file1.txt
+---
+my_directory/file2.txt
+---
+Contents of file2.txt
+---
+my_directory/subdirectory/file3.txt
+---
+Contents of file3.txt
+---
+```
+
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
+
 ```bash
 cd files-to-prompt
 python -m venv venv
 source venv/bin/activate
 ```
+
 Now install the dependencies and test dependencies:
+
 ```bash
 pip install -e '.[test]'
 ```
+
 To run the tests:
 ```bash
 pytest
 ```
```

### Comparing `files-to-prompt-0.1/README.md` & `files-to-prompt-0.2/files_to_prompt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: files-to-prompt
+Version: 0.2
+Summary: Concatenate a directory full of files into a single prompt for use with LLMs
+Author: Simon Willison
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/simonw/files-to-prompt
+Project-URL: Changelog, https://github.com/simonw/files-to-prompt/releases
+Project-URL: Issues, https://github.com/simonw/files-to-prompt/issues
+Project-URL: CI, https://github.com/simonw/files-to-prompt/actions
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+
 # files-to-prompt
 
 [![PyPI](https://img.shields.io/pypi/v/files-to-prompt.svg)](https://pypi.org/project/files-to-prompt/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/files-to-prompt?include_prereleases&label=changelog)](https://github.com/simonw/files-to-prompt/releases)
 [![Tests](https://github.com/simonw/files-to-prompt/actions/workflows/test.yml/badge.svg)](https://github.com/simonw/files-to-prompt/actions/workflows/test.yml)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/files-to-prompt/blob/master/LICENSE)
 
@@ -9,45 +27,52 @@
 
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install files-to-prompt
 ```
+
 ## Usage
 
-To use `files-to-prompt`, provide the path to the directory you want to process:
+To use `files-to-prompt`, provide the path to one or more files or directories you want to process:
 
 ```bash
-files-to-prompt path/to/directory
+files-to-prompt path/to/file_or_directory [path/to/another/file_or_directory ...]
 ```
 
-This will output the contents of every file in the directory and its subdirectories, with each file preceded by its relative path and separated by `---`.
+This will output the contents of every file, with each file preceded by its relative path and separated by `---`.
 
 ### Options
 
 - `--include-hidden`: Include files and folders starting with `.` (hidden files and directories).
   ```bash
   files-to-prompt path/to/directory --include-hidden
   ```
 
 - `--ignore-gitignore`: Ignore `.gitignore` files and include all files.
   ```bash
   files-to-prompt path/to/directory --ignore-gitignore
   ```
 
+- `--ignore <pattern>`: Specify one or more patterns to ignore. Can be used multiple times.
+  ```bash
+  files-to-prompt path/to/directory --ignore "*.log" --ignore "temp*"
+  ```
+
 ### Example
 
 Suppose you have a directory structure like this:
 
 ```
 my_directory/
 ├── file1.txt
 ├── file2.txt
 ├── .hidden_file.txt
+├── temp.log
 └── subdirectory/
     └── file3.txt
 ```
 
 Running `files-to-prompt my_directory` will output:
 
 ```
@@ -70,23 +95,45 @@
 ```
 my_directory/.hidden_file.txt
 ---
 Contents of .hidden_file.txt
 ---
 ...
 ```
+
+If you run `files-to-prompt my_directory --ignore "*.log"`, the output will exclude `temp.log`:
+
+```
+my_directory/file1.txt
+---
+Contents of file1.txt
+---
+my_directory/file2.txt
+---
+Contents of file2.txt
+---
+my_directory/subdirectory/file3.txt
+---
+Contents of file3.txt
+---
+```
+
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
+
 ```bash
 cd files-to-prompt
 python -m venv venv
 source venv/bin/activate
 ```
+
 Now install the dependencies and test dependencies:
+
 ```bash
 pip install -e '.[test]'
 ```
+
 To run the tests:
 ```bash
 pytest
 ```
```

### Comparing `files-to-prompt-0.1/files_to_prompt/cli.py` & `files-to-prompt-0.2/files_to_prompt/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,67 +19,99 @@
         with open(gitignore_path, "r") as f:
             return [
                 line.strip() for line in f if line.strip() and not line.startswith("#")
             ]
     return []
 
 
+def process_path(
+    path, include_hidden, ignore_gitignore, gitignore_rules, ignore_patterns
+):
+    if os.path.isfile(path):
+        with open(path, "r") as f:
+            file_contents = f.read()
+        click.echo(path)
+        click.echo("---")
+        click.echo(file_contents)
+        click.echo()
+        click.echo("---")
+    elif os.path.isdir(path):
+        for root, dirs, files in os.walk(path):
+            if not include_hidden:
+                dirs[:] = [d for d in dirs if not d.startswith(".")]
+                files = [f for f in files if not f.startswith(".")]
+
+            if not ignore_gitignore:
+                gitignore_rules.extend(read_gitignore(root))
+                dirs[:] = [
+                    d
+                    for d in dirs
+                    if not should_ignore(os.path.join(root, d), gitignore_rules)
+                ]
+                files = [
+                    f
+                    for f in files
+                    if not should_ignore(os.path.join(root, f), gitignore_rules)
+                ]
+
+            if ignore_patterns:
+                files = [
+                    f
+                    for f in files
+                    if not any(fnmatch(f, pattern) for pattern in ignore_patterns)
+                ]
+
+            for file in files:
+                file_path = os.path.join(root, file)
+                with open(file_path, "r") as f:
+                    file_contents = f.read()
+
+                click.echo(file_path)
+                click.echo("---")
+                click.echo(file_contents)
+                click.echo()
+                click.echo("---")
+
+
 @click.command()
-@click.argument(
-    "path",
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, readable=True),
-)
+@click.argument("paths", nargs=-1, type=click.Path(exists=True))
 @click.option(
     "--include-hidden",
     is_flag=True,
     help="Include files and folders starting with .",
 )
 @click.option(
     "--ignore-gitignore",
     is_flag=True,
     help="Ignore .gitignore files and include all files",
 )
+@click.option(
+    "ignore_patterns",
+    "--ignore",
+    multiple=True,
+    default=[],
+    help="List of patterns to ignore",
+)
 @click.version_option()
-def cli(path, include_hidden, ignore_gitignore):
+def cli(paths, include_hidden, ignore_gitignore, ignore_patterns):
     """
-    Takes a path to a folder and outputs every file in that folder,
+    Takes one or more paths to files or directories and outputs every file,
     recursively, each one preceded with its filename like this:
 
     path/to/file.py
     ----
     Contents of file.py goes here
 
     ---
     path/to/file2.py
     ---
     ...
     """
-    gitignore_rules = [] if ignore_gitignore else read_gitignore(path)
-
-    for root, dirs, files in os.walk(path):
-        if not include_hidden:
-            dirs[:] = [d for d in dirs if not d.startswith(".")]
-            files = [f for f in files if not f.startswith(".")]
-
+    gitignore_rules = []
+    for path in paths:
+        if not os.path.exists(path):
+            raise click.BadArgumentUsage(f"Path does not exist: {path}")
         if not ignore_gitignore:
-            gitignore_rules.extend(read_gitignore(root))
-            dirs[:] = [
-                d
-                for d in dirs
-                if not should_ignore(os.path.join(root, d), gitignore_rules)
-            ]
-            files = [
-                f
-                for f in files
-                if not should_ignore(os.path.join(root, f), gitignore_rules)
-            ]
-
-        for file in files:
-            file_path = os.path.join(root, file)
-            with open(file_path, "r") as f:
-                file_contents = f.read()
-
-            click.echo(file_path)
-            click.echo("---")
-            click.echo(file_contents)
-            click.echo()
-            click.echo("---")
+            gitignore_rules.extend(read_gitignore(os.path.dirname(path)))
+        process_path(
+            path, include_hidden, ignore_gitignore, gitignore_rules, ignore_patterns
+        )
```

### Comparing `files-to-prompt-0.1/pyproject.toml` & `files-to-prompt-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "files-to-prompt"
-version = "0.1"
+version = "0.2"
 description = "Concatenate a directory full of files into a single prompt for use with LLMs"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
```

