# Comparing `tmp/robocorp_actions-0.1.0.tar.gz` & `tmp/robocorp_actions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_actions-0.1.0.tar", max compression
+gzip compressed data, was "robocorp_actions-0.1.1.tar", max compression
```

## Comparing `robocorp_actions-0.1.0.tar` & `robocorp_actions-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2872 2024-03-15 19:17:12.268989 robocorp_actions-0.1.0/README.md
--rw-r--r--   0        0        0      965 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3596 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/__init__.py
--rw-r--r--   0        0        0       81 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/__main__.py
--rw-r--r--   0        0        0      140 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/_action_options.py
--rw-r--r--   0        0        0     5199 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/_args_dispatcher.py
--rw-r--r--   0        0        0     4243 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/_fixtures.py
--rw-r--r--   0        0        0    11431 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/_lint_action.py
--rw-r--r--   0        0        0     1211 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/_managed_parameters.py
--rw-r--r--   0        0        0      314 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/_protocols.py
--rw-r--r--   0        0        0     2907 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/_request.py
--rw-r--r--   0        0        0     1023 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/_request_impl.py
--rw-r--r--   0        0        0     2123 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/cli.py
--rw-r--r--   0        0        0        0 2024-03-15 19:17:12.272989 robocorp_actions-0.1.0/src/robocorp/actions/py.typed
--rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 robocorp_actions-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2958 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/README.md
+-rw-r--r--   0        0        0      965 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3596 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/__main__.py
+-rw-r--r--   0        0        0      140 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_action_options.py
+-rw-r--r--   0        0        0     5199 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_args_dispatcher.py
+-rw-r--r--   0        0        0     4243 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_fixtures.py
+-rw-r--r--   0        0        0    11967 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_lint_action.py
+-rw-r--r--   0        0        0     1211 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_managed_parameters.py
+-rw-r--r--   0        0        0      314 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_protocols.py
+-rw-r--r--   0        0        0     2907 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_request.py
+-rw-r--r--   0        0        0     1023 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_request_impl.py
+-rw-r--r--   0        0        0     2123 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/cli.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/py.typed
+-rw-r--r--   0        0        0     3650 1970-01-01 00:00:00.000000 robocorp_actions-0.1.1/PKG-INFO
```

### Comparing `robocorp_actions-0.1.0/README.md` & `robocorp_actions-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: robocorp-actions
+Version: 0.1.1
+Summary: Robocorp Actions
+Home-page: https://github.com/robocorp/robocorp/
+License: Apache-2.0
+Author: Fabio Z.
+Author-email: fabio@robocorp.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: robocorp-tasks (==3.0.0)
+Project-URL: Repository, https://github.com/robocorp/robocorp/
+Description-Content-Type: text/markdown
+
 # ⚡️ robocorp-actions
 
 A Python library designed to simplify the development of Python actions _(AI or otherwise)_ to be run with the [Robocorp Action Server](../action_server/).
 
 ## Getting started
 
 If you have not setup Action Server already, see the [🏃‍♂️ Quickstart](https://github.com/robocorp/robocorp#quickstart) on how to do that.
@@ -12,20 +31,19 @@
 from robocorp.actions import action
 
 @action
 def sum_numbers(a: float, b: float) -> float:
     ...
 ```
 
-**And your function is now an ⚡️ action!**
+**And your function is now an ⚡️Action!**
 
 You can now run and debug your action by Starting Action Server with `action-server start` and accessing the UI at http://localhost:8080.
 
-> [!NOTE]
-> Action inputs and outputs support only `int`, `float`, `str`, and `bool` types.
+> Note: Action inputs and outputs support only `int`, `float`, `str` and `bool` types.
 
 ## Describe your action
 
 For an action's purpose and usage to be understood by AI models _(and humans)_ it needs to be documented correctly.
 
 To do that, use [Google Style Docstring](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings) to write a clear and concise description on what your action does and document the action inputs and expected output:
 
@@ -42,16 +60,15 @@
 
     Returns:
         str: The requested weather conditions forecast
     """
     ...
 ```
 
-> [!TIP]
-> Experiment with and iterate the exact documentation wording to get more predictable results when using your action with AI apps.
+> Tip: Experiment with and iterate the exact documentation wording to get more predictable results when using your action with AI apps.
 
 ---
 
 ### Consequential flag
 
 You can explicitly provide the `is_consequential` flag for an action to mark it's operations as "must always prompt the user for confirmation before running" by [OpenAI GPTs](https://platform.openai.com/docs/actions) _(and possibly by other providers)_. If set to `False`, the user will be provided with an "always allow" feature.
 
@@ -64,14 +81,19 @@
 
 To get the full benefits of your actions, the suggested way to run them is using Action Server. But it's also possible to do that directly in command line by passing the named arguments:
 
 ```sh
 python -m robocorp.actions run -- --city=Helsinki --days=3
 ```
 
-### API Reference
+## Guides
+
+- [Request headers](https://github.com/robocorp/robocorp/blob/master/actions/docs/guides/00-request.md)
 
-Information on specific functions or classes: [robocorp.actions](https://github.com/robocorp/robocorp/blob/master/actions/docs/api/README.md)
+## API Reference
 
-### Changelog
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/actions/docs/api/README.md) for extensive documentation.
+
+## Changelog
 
 A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/actions/docs/CHANGELOG.md).
+
```

### Comparing `robocorp_actions-0.1.0/pyproject.toml` & `robocorp_actions-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-actions"
-version = "0.1.0"
+version = "0.1.1"
 description = "Robocorp Actions"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
```

### Comparing `robocorp_actions-0.1.0/src/robocorp/actions/__init__.py` & `robocorp_actions-0.1.1/src/robocorp/actions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Callable, Optional, overload
 
 from ._action_options import ActionOptions
 from ._fixtures import setup, teardown
 from ._protocols import IAction, Status
 from ._request import Request
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @overload
 def action(func: Callable) -> Callable:
     ...
```

### Comparing `robocorp_actions-0.1.0/src/robocorp/actions/_args_dispatcher.py` & `robocorp_actions-0.1.1/src/robocorp/actions/_args_dispatcher.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.0/src/robocorp/actions/_fixtures.py` & `robocorp_actions-0.1.1/src/robocorp/actions/_fixtures.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.0/src/robocorp/actions/_lint_action.py` & `robocorp_actions-0.1.1/src/robocorp/actions/_lint_action.py`

 * *Files 10% similar despite different names*

```diff
@@ -215,43 +215,57 @@
         yield _make_error(
             node,
             "@action without a `return` (an `@action` must have a return value).",
             coldelta=4,
         )
 
 
-def _check_arguments(
+def _check_docstring_contents(
     pm: Optional[PluginManager], node: ast_module.FunctionDef, docstring: str
 ) -> Iterator[Error]:
+    import docstring_parser
     from robocorp.tasks._commands import _is_managed_param
 
+    assert docstring, "Expected docstring to be given."
+
     arguments = node.args
-    if arguments.args:
-        param_name_to_description = {}
-        if docstring:
-            import docstring_parser
-
-            contents = docstring_parser.parse(docstring)
-            for docparam in contents.params:
-                if docparam.description:
-                    param_name_to_description[docparam.arg_name] = docparam.description
-
-            if (
-                not contents.short_description
-                or contents.short_description.strip() == "Args:"
-            ):
-                yield _make_error(
-                    node,
-                    "No description found in docstring. "
-                    "Please update docstring to add it as an LLM needs this info "
-                    "to understand when to call this action.",
-                    coldelta=4,
-                )
-                return
+    contents = docstring_parser.parse(docstring)
+
+    param_name_to_description = {}
+    for docparam in contents.params:
+        if docparam.description:
+            param_name_to_description[docparam.arg_name] = docparam.description
+
+    if not contents.short_description or contents.short_description.strip() == "Args:":
+        yield _make_error(
+            node,
+            "No description found in docstring. "
+            "Please update docstring to add it as an LLM needs this info "
+            "to understand when to call this action.",
+            coldelta=4,
+        )
+        return
+
+    if contents.short_description and contents.long_description:
+        doc_desc = f"{contents.short_description}\n{contents.long_description}"
+    else:
+        doc_desc = contents.long_description or contents.short_description or ""
 
+    doc_desc_len = len(doc_desc)
+    if doc_desc_len > 300:
+        yield _make_error(
+            node,
+            f"Description has {doc_desc_len} chars. OpenAI just supports "
+            "300 chars in the description (note: this may not be a problem "
+            "in other integrations).",
+            coldelta=4,
+            severity=DiagnosticSeverity.Warning,
+        )
+
+    if arguments.args:
         for arg in arguments.args:
             desc = param_name_to_description.pop(arg.arg, None)
             if pm is not None and _is_managed_param(pm, arg.arg):
                 continue
 
             if not desc:
                 yield _make_error(
@@ -281,25 +295,26 @@
                     # We found an @action. Do the needed checks.
 
                     # Check for docstring
                     docstring: str = ast_module.get_docstring(node) or ""
                     if docstring:
                         docstring = docstring.strip()
 
+                    yield from _check_return_type(node)
+                    yield from _check_return_statement(node)
+
                     if not docstring:
                         yield _make_error(
                             node,
                             "@action docstring not found. Please define it as this is what "
                             "an LLM would use to decide whether to call this action.",
                             coldelta=4,
                         )
-
-                    yield from _check_return_type(node)
-                    yield from _check_return_statement(node)
-                    yield from _check_arguments(pm, node, docstring)
+                    else:
+                        yield from _check_docstring_contents(pm, node, docstring)
 
 
 _severity_id_to_severity = {
     DiagnosticSeverity.Error: "error",
     DiagnosticSeverity.Warning: "warning",
     DiagnosticSeverity.Information: "information",
     DiagnosticSeverity.Hint: "hint",
```

### Comparing `robocorp_actions-0.1.0/src/robocorp/actions/_managed_parameters.py` & `robocorp_actions-0.1.1/src/robocorp/actions/_managed_parameters.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.0/src/robocorp/actions/_request.py` & `robocorp_actions-0.1.1/src/robocorp/actions/_request.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.0/src/robocorp/actions/_request_impl.py` & `robocorp_actions-0.1.1/src/robocorp/actions/_request_impl.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.0/src/robocorp/actions/cli.py` & `robocorp_actions-0.1.1/src/robocorp/actions/cli.py`

 * *Files identical despite different names*

