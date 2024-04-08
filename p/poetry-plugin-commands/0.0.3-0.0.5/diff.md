# Comparing `tmp/poetry_plugin_commands-0.0.3.tar.gz` & `tmp/poetry_plugin_commands-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_commands-0.0.3.tar", max compression
+gzip compressed data, was "poetry_plugin_commands-0.0.5.tar", max compression
```

## Comparing `poetry_plugin_commands-0.0.3.tar` & `poetry_plugin_commands-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.3/LICENSE
--rw-r--r--   0        0        0     1932 2024-04-07 23:55:38.326799 poetry_plugin_commands-0.0.3/README.md
--rw-r--r--   0        0        0     3210 2024-04-08 00:04:08.938771 poetry_plugin_commands-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.3/src/poetry_plugin_commands/__init__.py
--rw-r--r--   0        0        0     1066 2024-04-07 23:16:24.616932 poetry_plugin_commands-0.0.3/src/poetry_plugin_commands/command.py
--rw-r--r--   0        0        0     1511 2024-04-07 21:56:30.935201 poetry_plugin_commands-0.0.3/src/poetry_plugin_commands/plugins.py
--rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1928 2024-04-08 01:11:27.879544 poetry_plugin_commands-0.0.5/README.md
+-rw-r--r--   0        0        0     3210 2024-04-08 01:12:36.287540 poetry_plugin_commands-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.5/src/poetry_plugin_commands/__init__.py
+-rw-r--r--   0        0        0     1112 2024-04-08 00:27:30.593692 poetry_plugin_commands-0.0.5/src/poetry_plugin_commands/command.py
+-rw-r--r--   0        0        0     1644 2024-04-08 00:44:09.905636 poetry_plugin_commands-0.0.5/src/poetry_plugin_commands/plugins.py
+-rw-r--r--   0        0        0     3551 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.5/PKG-INFO
```

### Comparing `poetry_plugin_commands-0.0.3/LICENSE` & `poetry_plugin_commands-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.3/README.md` & `poetry_plugin_commands-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 ### Usage
 
 1. **Installation**:
 
    Install the plugin using Poetry:
 
    ```bash
-   pip install --user poetry-plugin-commands
+   pip install poetry-plugin-commands
    ```
 
    or
 
    ```bash
-   poetry self add poetry-plugin-commands
+   pip install --user poetry-plugin-commands
    ```
 
    or at least
 
    ```bash
    poetry self add poetry-plugin-commands
    ```
```

### Comparing `poetry_plugin_commands-0.0.3/pyproject.toml` & `poetry_plugin_commands-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-commands"
-version = "0.0.3"
+version = "0.0.5"
 description = "Poetry plugin for simple custom user commands execution."
 readme = "README.md"
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
```

### Comparing `poetry_plugin_commands-0.0.3/src/poetry_plugin_commands/command.py` & `poetry_plugin_commands-0.0.5/src/poetry_plugin_commands/command.py`

 * *Files 17% similar despite different names*

```diff
@@ -46,8 +46,9 @@
 
 	@property
 	def default_groups(self: UserCommand) -> set[str]:
 		return {MAIN_GROUP}
 
 
 	def handle(self: UserCommand) -> int:
+		# TODO: Optionally show execution command..
 		return system(self.command)  # noqa: S605
```

### Comparing `poetry_plugin_commands-0.0.3/src/poetry_plugin_commands/plugins.py` & `poetry_plugin_commands-0.0.5/src/poetry_plugin_commands/plugins.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 	def commands(self: UserCommandsApplicationPlugin) -> list[type[Command]]:
 		"""Property with plugin own commands and user's commands.
 
 		User's commands are auto-generated from toml plugin's section shell commands.
 		"""
 		toml_content: dict[str, Any] = self.poetry.pyproject.data
 
+		# TODO: Exec field or catch options of poetry's run command (mb better make something like crun?)
+		# TODO: Make profiles for ux..
 		user_commands = toml_content['tool']['poetry']['plugins'][self.plugin_section]
 
 		# TODO: Support python commands using toml's optioned values..
 		commands = [
 			UserCommand._new_cls(alias, command)  # noqa: SLF001
 			for alias, command in user_commands.items()
 		]
```

### Comparing `poetry_plugin_commands-0.0.3/PKG-INFO` & `poetry_plugin_commands-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-commands
-Version: 0.0.3
+Version: 0.0.5
 Summary: Poetry plugin for simple custom user commands execution.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -39,21 +39,21 @@
 ### Usage
 
 1. **Installation**:
 
    Install the plugin using Poetry:
 
    ```bash
-   pip install --user poetry-plugin-commands
+   pip install poetry-plugin-commands
    ```
 
    or
 
    ```bash
-   poetry self add poetry-plugin-commands
+   pip install --user poetry-plugin-commands
    ```
 
    or at least
 
    ```bash
    poetry self add poetry-plugin-commands
    ```
```

