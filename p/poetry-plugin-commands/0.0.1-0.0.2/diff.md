# Comparing `tmp/poetry_plugin_commands-0.0.1.tar.gz` & `tmp/poetry_plugin_commands-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_commands-0.0.1.tar", max compression
+gzip compressed data, was "poetry_plugin_commands-0.0.2.tar", max compression
```

## Comparing `poetry_plugin_commands-0.0.1.tar` & `poetry_plugin_commands-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.1/LICENSE
--rw-r--r--   0        0        0     1784 2024-04-07 23:23:50.335907 poetry_plugin_commands-0.0.1/README.md
--rw-r--r--   0        0        0     3103 2024-04-07 23:38:30.478857 poetry_plugin_commands-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.1/src/poetry_plugin_commands/__init__.py
--rw-r--r--   0        0        0     1066 2024-04-07 23:16:24.616932 poetry_plugin_commands-0.0.1/src/poetry_plugin_commands/command.py
--rw-r--r--   0        0        0     1511 2024-04-07 21:56:30.935201 poetry_plugin_commands-0.0.1/src/poetry_plugin_commands/plugins.py
--rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1932 2024-04-07 23:55:38.326799 poetry_plugin_commands-0.0.2/README.md
+-rw-r--r--   0        0        0     3103 2024-04-07 23:53:46.253806 poetry_plugin_commands-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.2/src/poetry_plugin_commands/__init__.py
+-rw-r--r--   0        0        0     1066 2024-04-07 23:16:24.616932 poetry_plugin_commands-0.0.2/src/poetry_plugin_commands/command.py
+-rw-r--r--   0        0        0     1511 2024-04-07 21:56:30.935201 poetry_plugin_commands-0.0.2/src/poetry_plugin_commands/plugins.py
+-rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.2/PKG-INFO
```

### Comparing `poetry_plugin_commands-0.0.1/LICENSE` & `poetry_plugin_commands-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.1/README.md` & `poetry_plugin_commands-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,27 @@
 ### Usage
 
 1. **Installation**:
 
    Install the plugin using Poetry:
 
    ```bash
-   poetry self add poetry-command-aliases
+   pip install --user poetry-plugin-commands
+   ```
+
+   or
+
+   ```bash
+   poetry self add poetry-plugin-commands
+   ```
+
+   or at least
+
+   ```bash
+   poetry self add poetry-plugin-commands
    ```
 
 2. **Define Aliases**:
 
    Add your aliases to the `pyproject.toml` file under the `[tool.poetry.plugins.commands]` section:
 
    ```toml
```

### Comparing `poetry_plugin_commands-0.0.1/pyproject.toml` & `poetry_plugin_commands-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-commands"
-version = "0.0.1"
+version = "0.0.2"
 description = "Poetry plugin for simple custom user commands execution."
 readme = "README.md"
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
```

### Comparing `poetry_plugin_commands-0.0.1/src/poetry_plugin_commands/command.py` & `poetry_plugin_commands-0.0.2/src/poetry_plugin_commands/command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.1/src/poetry_plugin_commands/plugins.py` & `poetry_plugin_commands-0.0.2/src/poetry_plugin_commands/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.1/PKG-INFO` & `poetry_plugin_commands-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-commands
-Version: 0.0.1
+Version: 0.0.2
 Summary: Poetry plugin for simple custom user commands execution.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -39,15 +39,27 @@
 ### Usage
 
 1. **Installation**:
 
    Install the plugin using Poetry:
 
    ```bash
-   poetry self add poetry-command-aliases
+   pip install --user poetry-plugin-commands
+   ```
+
+   or
+
+   ```bash
+   poetry self add poetry-plugin-commands
+   ```
+
+   or at least
+
+   ```bash
+   poetry self add poetry-plugin-commands
    ```
 
 2. **Define Aliases**:
 
    Add your aliases to the `pyproject.toml` file under the `[tool.poetry.plugins.commands]` section:
 
    ```toml
```

