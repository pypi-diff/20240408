# Comparing `tmp/StringDataDeque-0.9.10.tar.gz` & `tmp/StringDataDeque-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StringDataDeque-0.9.10.tar", last modified: Sun Apr  7 23:40:48 2024, max compression
+gzip compressed data, was "StringDataDeque-1.0.0.tar", last modified: Mon Apr  8 05:26:16 2024, max compression
```

## Comparing `StringDataDeque-0.9.10.tar` & `StringDataDeque-1.0.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:40:48.977373 StringDataDeque-0.9.10/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:40:48.969372 StringDataDeque-0.9.10/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:40:48.969372 StringDataDeque-0.9.10/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.github/workflows/black.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.github/workflows/dapperdata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.github/workflows/tomlsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.github/workflows/tox.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43391 2024-04-07 23:40:48.977373 StringDataDeque-0.9.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:40:48.973372 StringDataDeque-0.9.10/StringDataDeque.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43391 2024-04-07 23:40:48.000000 StringDataDeque-0.9.10/StringDataDeque.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-07 23:40:48.000000 StringDataDeque-0.9.10/StringDataDeque.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:40:48.000000 StringDataDeque-0.9.10/StringDataDeque.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-07 23:40:48.000000 StringDataDeque-0.9.10/StringDataDeque.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 23:40:48.000000 StringDataDeque-0.9.10/StringDataDeque.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/check_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:40:48.973372 StringDataDeque-0.9.10/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/docs/index.rst.bak
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:40:48.973372 StringDataDeque-0.9.10/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/docs/source/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/docs/source/stringdatadeque.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 23:40:48.977373 StringDataDeque-0.9.10/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:40:48.965372 StringDataDeque-0.9.10/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:40:48.973372 StringDataDeque-0.9.10/src/stringdatadeque/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/src/stringdatadeque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/src/stringdatadeque/encryptedstringdeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/src/stringdatadeque/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/src/stringdatadeque/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12091 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/src/stringdatadeque/stringdatadeque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:40:48.973372 StringDataDeque-0.9.10/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/tests/default.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/tests/private.pem
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/tests/test_encryptedssgtringdeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/tests/test_stringdatadeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-07 23:40:44.000000 StringDataDeque-0.9.10/tests/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.108085 StringDataDeque-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.100085 StringDataDeque-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.100085 StringDataDeque-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/dapperdata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/tomlsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.github/workflows/tox.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43420 2024-04-08 05:26:16.108085 StringDataDeque-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.104085 StringDataDeque-1.0.0/StringDataDeque.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43420 2024-04-08 05:26:16.000000 StringDataDeque-1.0.0/StringDataDeque.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-08 05:26:16.000000 StringDataDeque-1.0.0/StringDataDeque.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:26:16.000000 StringDataDeque-1.0.0/StringDataDeque.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-08 05:26:16.000000 StringDataDeque-1.0.0/StringDataDeque.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 05:26:16.000000 StringDataDeque-1.0.0/StringDataDeque.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/check_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.104085 StringDataDeque-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/index.rst.bak
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.104085 StringDataDeque-1.0.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/source/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/docs/source/stringdatadeque.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:26:16.108085 StringDataDeque-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.100085 StringDataDeque-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.104085 StringDataDeque-1.0.0/src/stringdatadeque/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/src/stringdatadeque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10212 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/src/stringdatadeque/encryptedstringdeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/src/stringdatadeque/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/src/stringdatadeque/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18233 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/src/stringdatadeque/stringdatadeque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:26:16.104085 StringDataDeque-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/default.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/test_encryptedssgtringdeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/test_stringdatadeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-08 05:26:11.000000 StringDataDeque-1.0.0/tests/timing.py
```

### Comparing `StringDataDeque-0.9.10/.github/workflows/pypi.yaml` & `StringDataDeque-1.0.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/.github/workflows/tox.yaml` & `StringDataDeque-1.0.0/.github/workflows/tox.yaml`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/.gitignore` & `StringDataDeque-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/.pre-commit-config.yaml` & `StringDataDeque-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/LICENSE` & `StringDataDeque-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/PKG-INFO` & `StringDataDeque-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringDataDeque
-Version: 0.9.10
+Version: 1.0.0
 Summary: Useful when building a string from data that can be converted into a string, in parts.
 Author: R.Broderick
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -722,48 +722,48 @@
 
 ## Uses
 
 This is designed to be a drop-in replacement for when you might want to append to a string in a loop.
 
 ### Benefits
 * Around 5 times faster than the naive implementation of appending to a string, such as
-    ```
+    ```python
     x = ""
     for x in collection:
         x+="new string"
     ```
 * Provides many extra features that help simply code.
 
 ## Examples
-```
-sd = StringDeque(sep-"\n")
+```python
+sd = StringDeque(sep="\n")
 for x in collection:
     sd += x
 # StringDeque is a specialization of StringDataDeque where conversion func is "str"
 # this allows any datatype to be used which can convert to str
 sd += 1
 print(sd)
 ```
 
 You can also pipe data into the StringDeque
-```
+```python
 sd = StringDeque()
 sd = [1,2,3,4,5] | sd
 # or
 sd |= [1,2,3,4,5]
 ```
 
 StringDataDeque implements the "contains" method so you can search within it
-```
+```python
 sd = StringDeque(["line_one","line_two"],sep="\n")
 if "line_one" in sd:
     print("yes")
 ```
 
 If you need more control over how data is added to the deque either use StringDataDeque or one of its subclasses.
-```
+```python
 # convert_func is called when data is added, and format_func is called when data is printed.
 int_sdd =StringDataDeque(data="test", convert_func=int, format_func=str,sep=" ")
 int_sdd |= ["1","2","3","4","5"]
 assert int_sdd[0] == 1
 assert str(int_sdd) == "1 2 3 4 5"
 ```
```

### Comparing `StringDataDeque-0.9.10/README.md` & `StringDataDeque-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,48 +10,48 @@
 
 ## Uses
 
 This is designed to be a drop-in replacement for when you might want to append to a string in a loop.
 
 ### Benefits
 * Around 5 times faster than the naive implementation of appending to a string, such as
-    ```
+    ```python
     x = ""
     for x in collection:
         x+="new string"
     ```
 * Provides many extra features that help simply code.
 
 ## Examples
-```
-sd = StringDeque(sep-"\n")
+```python
+sd = StringDeque(sep="\n")
 for x in collection:
     sd += x
 # StringDeque is a specialization of StringDataDeque where conversion func is "str"
 # this allows any datatype to be used which can convert to str
 sd += 1
 print(sd)
 ```
 
 You can also pipe data into the StringDeque
-```
+```python
 sd = StringDeque()
 sd = [1,2,3,4,5] | sd
 # or
 sd |= [1,2,3,4,5]
 ```
 
 StringDataDeque implements the "contains" method so you can search within it
-```
+```python
 sd = StringDeque(["line_one","line_two"],sep="\n")
 if "line_one" in sd:
     print("yes")
 ```
 
 If you need more control over how data is added to the deque either use StringDataDeque or one of its subclasses.
-```
+```python
 # convert_func is called when data is added, and format_func is called when data is printed.
 int_sdd =StringDataDeque(data="test", convert_func=int, format_func=str,sep=" ")
 int_sdd |= ["1","2","3","4","5"]
 assert int_sdd[0] == 1
 assert str(int_sdd) == "1 2 3 4 5"
 ```
```

### Comparing `StringDataDeque-0.9.10/StringDataDeque.egg-info/PKG-INFO` & `StringDataDeque-1.0.0/StringDataDeque.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringDataDeque
-Version: 0.9.10
+Version: 1.0.0
 Summary: Useful when building a string from data that can be converted into a string, in parts.
 Author: R.Broderick
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -722,48 +722,48 @@
 
 ## Uses
 
 This is designed to be a drop-in replacement for when you might want to append to a string in a loop.
 
 ### Benefits
 * Around 5 times faster than the naive implementation of appending to a string, such as
-    ```
+    ```python
     x = ""
     for x in collection:
         x+="new string"
     ```
 * Provides many extra features that help simply code.
 
 ## Examples
-```
-sd = StringDeque(sep-"\n")
+```python
+sd = StringDeque(sep="\n")
 for x in collection:
     sd += x
 # StringDeque is a specialization of StringDataDeque where conversion func is "str"
 # this allows any datatype to be used which can convert to str
 sd += 1
 print(sd)
 ```
 
 You can also pipe data into the StringDeque
-```
+```python
 sd = StringDeque()
 sd = [1,2,3,4,5] | sd
 # or
 sd |= [1,2,3,4,5]
 ```
 
 StringDataDeque implements the "contains" method so you can search within it
-```
+```python
 sd = StringDeque(["line_one","line_two"],sep="\n")
 if "line_one" in sd:
     print("yes")
 ```
 
 If you need more control over how data is added to the deque either use StringDataDeque or one of its subclasses.
-```
+```python
 # convert_func is called when data is added, and format_func is called when data is printed.
 int_sdd =StringDataDeque(data="test", convert_func=int, format_func=str,sep=" ")
 int_sdd |= ["1","2","3","4","5"]
 assert int_sdd[0] == 1
 assert str(int_sdd) == "1 2 3 4 5"
 ```
```

### Comparing `StringDataDeque-0.9.10/StringDataDeque.egg-info/SOURCES.txt` & `StringDataDeque-1.0.0/StringDataDeque.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/check_names.py` & `StringDataDeque-1.0.0/check_names.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/docs/Makefile` & `StringDataDeque-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/docs/conf.py` & `StringDataDeque-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/docs/make.bat` & `StringDataDeque-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/docs/source/stringdatadeque.rst` & `StringDataDeque-1.0.0/docs/source/stringdatadeque.rst`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/justfile` & `StringDataDeque-1.0.0/justfile`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/pyproject.toml` & `StringDataDeque-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=67.0", "setuptools_scm[toml]>=7.1"]
 
 [project]
 authors = [{"name" = "R.Broderick"}]
 description = "Useful when building a string from data that can be converted into a string, in parts."
-version = "0.9.10"
+version = "1.0.0"
 license = {"file" = "LICENSE"}
 name = "StringDataDeque"
 readme = {file = "README.md", content-type = "text/markdown"}
 dependencies = ["beartype", "typing-extensions; python_version < '3.12'"]
 requires-python = ">=3.10.0"
 
 [project.optional-dependencies]
@@ -77,14 +77,15 @@
 # docstrings.
 #
 # This only has an effect when the `docstring-code-format` setting is
 # enabled.
 docstring-code-line-length = "dynamic"
 
 [tool.ruff.lint]
+typing-modules = ["beartype.typing"]
 select = ["ALL"]
 ignore = [
   "B024",
   "PIE790",
   "T201",
   "PYI013",
   "ANN101",
```

### Comparing `StringDataDeque-0.9.10/requirements-dev.txt` & `StringDataDeque-1.0.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/src/stringdatadeque/__init__.py` & `StringDataDeque-1.0.0/src/stringdatadeque/__init__.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/src/stringdatadeque/protocols.py` & `StringDataDeque-1.0.0/src/stringdatadeque/protocols.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-"""Holds Protocols and types."""
-
-import builtins
-from collections.abc import Sequence
-from typing import Annotated
-from typing import Protocol
-from typing import TypeVar
-from typing import runtime_checkable
-
-from beartype.vale import Is  # pyright: ignore[reportUnknownVariableType]
-from beartype.vale import IsInstance  # pyright: ignore[reportUnknownVariableType]
-
-
-@runtime_checkable
-class Printable(Protocol):  # pragma: no cover
-    """Used to denote class implements custom __str__ method."""
-
-    def __str__(self) -> str:
-        """Class should implement custom str method."""
-        ...
-
-
-def _defines_str(obj: object) -> bool:
-    return type(obj).__name__ in dir(builtins) or type(obj).__str__ != object.__str__
-
-
-Builtin_or_DefinesDunderStr = Annotated[Printable, Is[_defines_str]]
-
-
-T = TypeVar("T")
-# Type hint matching any non-string sequence *WHOSE ITEMS ARE ALL STRINGS.*
-SequenceNonstrOfStr = Annotated[Sequence[str], ~IsInstance[str]]
-# Type hint matching any non-string sequence
-SequenceNonStr = Annotated[Sequence[T], ~IsInstance[str]]
+"""Holds Protocols and types."""
+
+import builtins
+from collections.abc import Sequence
+from typing import Annotated
+from typing import Protocol
+from typing import TypeVar
+from typing import runtime_checkable
+
+from beartype.vale import Is  # pyright: ignore[reportUnknownVariableType]
+from beartype.vale import IsInstance  # pyright: ignore[reportUnknownVariableType]
+
+
+@runtime_checkable
+class Printable(Protocol):  # pragma: no cover
+    """Used to denote class implements custom __str__ method."""
+
+    def __str__(self) -> str:
+        """Class should implement custom str method."""
+        ...
+
+
+def _defines_str(obj: object) -> bool:
+    """Check if an object defines a custom `__str__` method.
+
+    :param obj: An object to check.
+    :type obj: object
+
+    :return: True if the object defines a custom `__str__` method, False otherwise.
+    :rtype: bool
+    """
+    return type(obj).__name__ in dir(builtins) or type(obj).__str__ != object.__str__
+
+
+Builtin_or_DefinesDunderStr = Annotated[Printable, Is[_defines_str]]
+
+
+T = TypeVar("T")
+# Type hint matching any non-string sequence *WHOSE ITEMS ARE ALL STRINGS.*
+SequenceNonstrOfStr = Annotated[Sequence[str], ~IsInstance[str]]
+# Type hint matching any non-string sequence
+SequenceNonStr = Annotated[Sequence[T], ~IsInstance[str]]
```

### Comparing `StringDataDeque-0.9.10/tests/private.pem` & `StringDataDeque-1.0.0/tests/private.pem`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/tests/test_encryptedssgtringdeque.py` & `StringDataDeque-1.0.0/tests/test_encryptedssgtringdeque.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/tests/test_stringdatadeque.py` & `StringDataDeque-1.0.0/tests/test_stringdatadeque.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-0.9.10/tests/timing.py` & `StringDataDeque-1.0.0/tests/timing.py`

 * *Files identical despite different names*

