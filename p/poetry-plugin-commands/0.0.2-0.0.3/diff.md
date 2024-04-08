# Comparing `tmp/poetry_plugin_commands-0.0.2.tar.gz` & `tmp/poetry_plugin_commands-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_commands-0.0.2.tar", max compression
+gzip compressed data, was "poetry_plugin_commands-0.0.3.tar", max compression
```

## Comparing `poetry_plugin_commands-0.0.2.tar` & `poetry_plugin_commands-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.2/LICENSE
--rw-r--r--   0        0        0     1932 2024-04-07 23:55:38.326799 poetry_plugin_commands-0.0.2/README.md
--rw-r--r--   0        0        0     3103 2024-04-07 23:53:46.253806 poetry_plugin_commands-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.2/src/poetry_plugin_commands/__init__.py
--rw-r--r--   0        0        0     1066 2024-04-07 23:16:24.616932 poetry_plugin_commands-0.0.2/src/poetry_plugin_commands/command.py
--rw-r--r--   0        0        0     1511 2024-04-07 21:56:30.935201 poetry_plugin_commands-0.0.2/src/poetry_plugin_commands/plugins.py
--rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1932 2024-04-07 23:55:38.326799 poetry_plugin_commands-0.0.3/README.md
+-rw-r--r--   0        0        0     3210 2024-04-08 00:04:08.938771 poetry_plugin_commands-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.3/src/poetry_plugin_commands/__init__.py
+-rw-r--r--   0        0        0     1066 2024-04-07 23:16:24.616932 poetry_plugin_commands-0.0.3/src/poetry_plugin_commands/command.py
+-rw-r--r--   0        0        0     1511 2024-04-07 21:56:30.935201 poetry_plugin_commands-0.0.3/src/poetry_plugin_commands/plugins.py
+-rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.3/PKG-INFO
```

### Comparing `poetry_plugin_commands-0.0.2/LICENSE` & `poetry_plugin_commands-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.2/README.md` & `poetry_plugin_commands-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.2/pyproject.toml` & `poetry_plugin_commands-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-commands"
-version = "0.0.2"
+version = "0.0.3"
 description = "Poetry plugin for simple custom user commands execution."
 readme = "README.md"
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
@@ -31,18 +31,21 @@
 ]
 
 [tool.poetry.urls]
 Homepage = "https://github.com/BlackCatDevel0per/poetry-plugin-commands"
 Documentation = "https://github.com/BlackCatDevel0per/poetry-plugin-commands"  # TODO: ...
 Repository = "https://github.com/BlackCatDevel0per/poetry-plugin-commands"
 
-[tool.poetry.plugins.commands]
-stree = "tree src"
-test_var = "echo $VAR"
-run_app = "PYTHONPATH=src:. poetry run python src/app_launch/main.py"
+## Simple example
+# [tool.poetry.plugins.commands]
+# stree = "tree src"
+# test_var = "echo $VAR"
+# Test this plugin without installing
+# run_env_stree = ".venv/bin/poetry stree"
+# run_app = "PYTHONPATH=src:. poetry run python src/app_launch/main.py"
 
 [tool.ruff]
 line-length = 100
 select = [
 	"RUF",
 	"FBT",
 	"FURB",
```

### Comparing `poetry_plugin_commands-0.0.2/src/poetry_plugin_commands/command.py` & `poetry_plugin_commands-0.0.3/src/poetry_plugin_commands/command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.2/src/poetry_plugin_commands/plugins.py` & `poetry_plugin_commands-0.0.3/src/poetry_plugin_commands/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.2/PKG-INFO` & `poetry_plugin_commands-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-commands
-Version: 0.0.2
+Version: 0.0.3
 Summary: Poetry plugin for simple custom user commands execution.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

