# Comparing `tmp/cjunct-2.0.1.tar.gz` & `tmp/cjunct-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjunct-2.0.1.tar", max compression
+gzip compressed data, was "cjunct-2.0.2.tar", max compression
```

## Comparing `cjunct-2.0.1.tar` & `cjunct-2.0.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-2.0.1/LICENSE
--rw-r--r--   0        0        0     2428 2024-03-31 11:43:25.516186 cjunct-2.0.1/README.md
--rw-r--r--   0        0        0     4651 2024-04-08 10:27:43.590051 cjunct-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      512 2024-04-08 10:02:51.811046 cjunct-2.0.1/src/cjunct/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-2.0.1/src/cjunct/actions/__init__.py
--rw-r--r--   0        0        0     9912 2024-04-08 10:02:51.812886 cjunct-2.0.1/src/cjunct/actions/base.py
--rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-2.0.1/src/cjunct/actions/bundled/__init__.py
--rw-r--r--   0        0        0     6568 2024-03-31 11:43:25.518075 cjunct-2.0.1/src/cjunct/actions/bundled/docker_shell.py
--rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-2.0.1/src/cjunct/actions/bundled/echo.py
--rw-r--r--   0        0        0     2138 2024-03-19 22:06:11.634519 cjunct-2.0.1/src/cjunct/actions/bundled/shell.py
--rw-r--r--   0        0        0      262 2024-04-08 10:02:51.814813 cjunct-2.0.1/src/cjunct/actions/constants.py
--rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-2.0.1/src/cjunct/actions/types.py
--rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-2.0.1/src/cjunct/config/__init__.py
--rw-r--r--   0        0        0     3847 2024-04-08 10:02:51.815841 cjunct-2.0.1/src/cjunct/config/constants/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-01 11:54:38.652885 cjunct-2.0.1/src/cjunct/config/constants/cli.py
--rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-2.0.1/src/cjunct/config/constants/helpers.py
--rw-r--r--   0        0        0     2887 2024-04-08 10:02:51.817068 cjunct-2.0.1/src/cjunct/config/environment.py
--rw-r--r--   0        0        0     4644 2024-04-08 10:02:51.818144 cjunct-2.0.1/src/cjunct/console.py
--rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-2.0.1/src/cjunct/display/__init__.py
--rw-r--r--   0        0        0     1089 2024-04-08 10:02:51.819232 cjunct-2.0.1/src/cjunct/display/base.py
--rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-2.0.1/src/cjunct/display/color.py
--rw-r--r--   0        0        0     4410 2024-04-08 10:02:51.820389 cjunct-2.0.1/src/cjunct/display/default.py
--rw-r--r--   0        0        0     1466 2024-04-08 10:02:51.820998 cjunct-2.0.1/src/cjunct/exceptions.py
--rw-r--r--   0        0        0       74 2024-04-08 10:02:51.821504 cjunct-2.0.1/src/cjunct/loader/__init__.py
--rw-r--r--   0        0        0     9371 2024-04-08 10:02:51.822926 cjunct-2.0.1/src/cjunct/loader/base.py
--rw-r--r--   0        0        0     7349 2024-04-08 10:02:51.824939 cjunct-2.0.1/src/cjunct/loader/default.py
--rw-r--r--   0        0        0      980 2024-04-08 10:02:51.826557 cjunct-2.0.1/src/cjunct/loader/helpers.py
--rw-r--r--   0        0        0     1931 2024-04-08 10:02:51.831758 cjunct-2.0.1/src/cjunct/loader/inspect.py
--rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-2.0.1/src/cjunct/py.typed
--rw-r--r--   0        0        0     2929 2024-04-08 10:02:51.836589 cjunct-2.0.1/src/cjunct/rendering/__init__.py
--rw-r--r--   0        0        0     1554 2024-04-08 10:02:51.839247 cjunct-2.0.1/src/cjunct/rendering/containers.py
--rw-r--r--   0        0        0     4327 2024-04-08 10:27:43.590650 cjunct-2.0.1/src/cjunct/rendering/tokenizing.py
--rw-r--r--   0        0        0     8665 2024-04-08 10:02:51.841751 cjunct-2.0.1/src/cjunct/runner.py
--rw-r--r--   0        0        0     6213 2024-04-08 10:02:51.843759 cjunct-2.0.1/src/cjunct/strategy.py
--rw-r--r--   0        0        0      389 2024-04-08 10:02:51.845757 cjunct-2.0.1/src/cjunct/types.py
--rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-2.0.1/src/cjunct/version.py
--rw-r--r--   0        0        0     4258 2024-04-08 10:02:51.847476 cjunct-2.0.1/src/cjunct/workflow.py
--rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-2.0.2/LICENSE
+-rw-r--r--   0        0        0     2428 2024-03-31 11:43:25.516186 cjunct-2.0.2/README.md
+-rw-r--r--   0        0        0     4651 2024-04-08 15:06:59.397382 cjunct-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      512 2024-04-08 10:02:51.811046 cjunct-2.0.2/src/cjunct/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-2.0.2/src/cjunct/actions/__init__.py
+-rw-r--r--   0        0        0     9912 2024-04-08 10:02:51.812886 cjunct-2.0.2/src/cjunct/actions/base.py
+-rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-2.0.2/src/cjunct/actions/bundled/__init__.py
+-rw-r--r--   0        0        0     6568 2024-03-31 11:43:25.518075 cjunct-2.0.2/src/cjunct/actions/bundled/docker_shell.py
+-rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-2.0.2/src/cjunct/actions/bundled/echo.py
+-rw-r--r--   0        0        0     2138 2024-03-19 22:06:11.634519 cjunct-2.0.2/src/cjunct/actions/bundled/shell.py
+-rw-r--r--   0        0        0      262 2024-04-08 10:02:51.814813 cjunct-2.0.2/src/cjunct/actions/constants.py
+-rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-2.0.2/src/cjunct/actions/types.py
+-rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-2.0.2/src/cjunct/config/__init__.py
+-rw-r--r--   0        0        0     3847 2024-04-08 10:02:51.815841 cjunct-2.0.2/src/cjunct/config/constants/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-01 11:54:38.652885 cjunct-2.0.2/src/cjunct/config/constants/cli.py
+-rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-2.0.2/src/cjunct/config/constants/helpers.py
+-rw-r--r--   0        0        0     2887 2024-04-08 10:02:51.817068 cjunct-2.0.2/src/cjunct/config/environment.py
+-rw-r--r--   0        0        0     4644 2024-04-08 10:02:51.818144 cjunct-2.0.2/src/cjunct/console.py
+-rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-2.0.2/src/cjunct/display/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-08 10:02:51.819232 cjunct-2.0.2/src/cjunct/display/base.py
+-rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-2.0.2/src/cjunct/display/color.py
+-rw-r--r--   0        0        0     4410 2024-04-08 10:02:51.820389 cjunct-2.0.2/src/cjunct/display/default.py
+-rw-r--r--   0        0        0     1466 2024-04-08 10:02:51.820998 cjunct-2.0.2/src/cjunct/exceptions.py
+-rw-r--r--   0        0        0       74 2024-04-08 10:02:51.821504 cjunct-2.0.2/src/cjunct/loader/__init__.py
+-rw-r--r--   0        0        0     9371 2024-04-08 10:02:51.822926 cjunct-2.0.2/src/cjunct/loader/base.py
+-rw-r--r--   0        0        0     7349 2024-04-08 10:02:51.824939 cjunct-2.0.2/src/cjunct/loader/default.py
+-rw-r--r--   0        0        0      980 2024-04-08 10:02:51.826557 cjunct-2.0.2/src/cjunct/loader/helpers.py
+-rw-r--r--   0        0        0     1931 2024-04-08 10:02:51.831758 cjunct-2.0.2/src/cjunct/loader/inspect.py
+-rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-2.0.2/src/cjunct/py.typed
+-rw-r--r--   0        0        0     3060 2024-04-08 15:06:59.397999 cjunct-2.0.2/src/cjunct/rendering/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-08 15:06:59.398482 cjunct-2.0.2/src/cjunct/rendering/constants.py
+-rw-r--r--   0        0        0     2417 2024-04-08 15:06:59.399217 cjunct-2.0.2/src/cjunct/rendering/containers.py
+-rw-r--r--   0        0        0     4327 2024-04-08 10:27:43.590650 cjunct-2.0.2/src/cjunct/rendering/tokenizing.py
+-rw-r--r--   0        0        0     8665 2024-04-08 10:02:51.841751 cjunct-2.0.2/src/cjunct/runner.py
+-rw-r--r--   0        0        0     6213 2024-04-08 10:02:51.843759 cjunct-2.0.2/src/cjunct/strategy.py
+-rw-r--r--   0        0        0      389 2024-04-08 10:02:51.845757 cjunct-2.0.2/src/cjunct/types.py
+-rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-2.0.2/src/cjunct/version.py
+-rw-r--r--   0        0        0     4258 2024-04-08 10:02:51.847476 cjunct-2.0.2/src/cjunct/workflow.py
+-rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-2.0.2/PKG-INFO
```

### Comparing `cjunct-2.0.1/LICENSE` & `cjunct-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/README.md` & `cjunct-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/pyproject.toml` & `cjunct-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cjunct"
-version = "2.0.1"
+version = "2.0.2"
 description = "Declarative task runner"
 license = "MIT"
 authors = [
     "Artem Novikov <artnew@list.ru>",
 ]
 readme = "README.md"
 repository = "https://github.com/reartnew/cjunct"
```

### Comparing `cjunct-2.0.1/src/cjunct/__init__.py` & `cjunct-2.0.2/src/cjunct/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/actions/base.py` & `cjunct-2.0.2/src/cjunct/actions/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/actions/bundled/docker_shell.py` & `cjunct-2.0.2/src/cjunct/actions/bundled/docker_shell.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/actions/bundled/shell.py` & `cjunct-2.0.2/src/cjunct/actions/bundled/shell.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/config/constants/__init__.py` & `cjunct-2.0.2/src/cjunct/config/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/config/constants/cli.py` & `cjunct-2.0.2/src/cjunct/config/constants/cli.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/config/constants/helpers.py` & `cjunct-2.0.2/src/cjunct/config/constants/helpers.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/config/environment.py` & `cjunct-2.0.2/src/cjunct/config/environment.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/console.py` & `cjunct-2.0.2/src/cjunct/console.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/display/base.py` & `cjunct-2.0.2/src/cjunct/display/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/display/color.py` & `cjunct-2.0.2/src/cjunct/display/color.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/display/default.py` & `cjunct-2.0.2/src/cjunct/display/default.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/exceptions.py` & `cjunct-2.0.2/src/cjunct/exceptions.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/loader/base.py` & `cjunct-2.0.2/src/cjunct/loader/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/loader/default.py` & `cjunct-2.0.2/src/cjunct/loader/default.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/loader/helpers.py` & `cjunct-2.0.2/src/cjunct/loader/helpers.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/loader/inspect.py` & `cjunct-2.0.2/src/cjunct/loader/inspect.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/rendering/__init__.py` & `cjunct-2.0.2/src/cjunct/rendering/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,21 +31,24 @@
             c.StrictOutcomeDict if C.STRICT_OUTCOMES_RENDERING else c.LooseDict  # type: ignore
         )
         self._locals: t.Dict[str, t.Any] = {
             "outcomes": c.ActionContainingDict(
                 {name: outcomes_leaf_class(outcomes_map.get(name, {})) for name in action_states}
             ),
             "status": c.ActionContainingDict(action_states),
-            "context": c.ContextDict(context_map),
+            "context": c.ContextDict(data=context_map, render_hook=self.render),
             "environment": c.LooseDict(os.environ),
         }
 
     def render(self, value: str) -> RenderedStringTemplate:
         """Process string data, replacing all @{} occurrences"""
         chunks: t.List[str] = []
+        # Cheap check
+        if "@{" not in value:
+            return RenderedStringTemplate(value)
         for lexeme_type, lexeme_value in TemplarStringLexer(value):
             if lexeme_type == TemplarStringLexer.EXPRESSION:
                 lexeme_value = self._string_template_process_expression(expression=lexeme_value)
             chunks.append(lexeme_value)
         return RenderedStringTemplate("".join(chunks))
 
     @classmethod
```

### Comparing `cjunct-2.0.1/src/cjunct/rendering/containers.py` & `cjunct-2.0.2/src/cjunct/rendering/containers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Templar containers for rendering."""
 
 import typing as t
 
+from .constants import MAX_RECURSION_DEPTH
+from ..actions.types import RenderedStringTemplate
 from ..exceptions import ActionRenderError
 
 __all__ = [
     "LooseDict",
     "StrictOutcomeDict",
     "ActionContainingDict",
     "ContextDict",
@@ -52,10 +54,26 @@
     def _on_key_error(cls, e: KeyError) -> t.Any:
         raise ActionRenderError(f"Action not found: {e}") from e
 
 
 class ContextDict(AttrDict):
     """Context keys representation"""
 
+    def __init__(self, data: t.Mapping[str, str], render_hook: t.Callable[[str], RenderedStringTemplate]) -> None:
+        super().__init__(data)
+        self.__render_hook: t.Callable[[str], RenderedStringTemplate] = render_hook
+        self.__depth: int = 0
+
     @classmethod
     def _on_key_error(cls, e: KeyError) -> t.Any:
         raise ActionRenderError(f"Context key not found: {e}") from e
+
+    def __getitem__(self, item: str):
+        # Context keys can refer to anything else, thus we keep resolving until the template is stable
+        result = str(super().__getitem__(item))
+        while True:
+            self.__depth += 1
+            if self.__depth >= MAX_RECURSION_DEPTH:
+                raise ActionRenderError(f"Recursion depth exceeded: {self.__depth}/{MAX_RECURSION_DEPTH}")
+            if result == (result := self.__render_hook(result)):
+                break
+        return result
```

### Comparing `cjunct-2.0.1/src/cjunct/rendering/tokenizing.py` & `cjunct-2.0.2/src/cjunct/rendering/tokenizing.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/runner.py` & `cjunct-2.0.2/src/cjunct/runner.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/strategy.py` & `cjunct-2.0.2/src/cjunct/strategy.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/src/cjunct/workflow.py` & `cjunct-2.0.2/src/cjunct/workflow.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.1/PKG-INFO` & `cjunct-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjunct
-Version: 2.0.1
+Version: 2.0.2
 Summary: Declarative task runner
 Home-page: https://github.com/reartnew/cjunct
 License: MIT
 Author: Artem Novikov
 Author-email: artnew@list.ru
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 4 - Beta
```

