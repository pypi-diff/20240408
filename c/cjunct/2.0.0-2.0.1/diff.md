# Comparing `tmp/cjunct-2.0.0.tar.gz` & `tmp/cjunct-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjunct-2.0.0.tar", max compression
+gzip compressed data, was "cjunct-2.0.1.tar", max compression
```

## Comparing `cjunct-2.0.0.tar` & `cjunct-2.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-2.0.0/LICENSE
--rw-r--r--   0        0        0     2428 2024-03-31 11:43:25.516186 cjunct-2.0.0/README.md
--rw-r--r--   0        0        0     4651 2024-04-08 10:02:51.809616 cjunct-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      512 2024-04-08 10:02:51.811046 cjunct-2.0.0/src/cjunct/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-2.0.0/src/cjunct/actions/__init__.py
--rw-r--r--   0        0        0     9912 2024-04-08 10:02:51.812886 cjunct-2.0.0/src/cjunct/actions/base.py
--rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-2.0.0/src/cjunct/actions/bundled/__init__.py
--rw-r--r--   0        0        0     6568 2024-03-31 11:43:25.518075 cjunct-2.0.0/src/cjunct/actions/bundled/docker_shell.py
--rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-2.0.0/src/cjunct/actions/bundled/echo.py
--rw-r--r--   0        0        0     2138 2024-03-19 22:06:11.634519 cjunct-2.0.0/src/cjunct/actions/bundled/shell.py
--rw-r--r--   0        0        0      262 2024-04-08 10:02:51.814813 cjunct-2.0.0/src/cjunct/actions/constants.py
--rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-2.0.0/src/cjunct/actions/types.py
--rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-2.0.0/src/cjunct/config/__init__.py
--rw-r--r--   0        0        0     3847 2024-04-08 10:02:51.815841 cjunct-2.0.0/src/cjunct/config/constants/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-01 11:54:38.652885 cjunct-2.0.0/src/cjunct/config/constants/cli.py
--rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-2.0.0/src/cjunct/config/constants/helpers.py
--rw-r--r--   0        0        0     2887 2024-04-08 10:02:51.817068 cjunct-2.0.0/src/cjunct/config/environment.py
--rw-r--r--   0        0        0     4644 2024-04-08 10:02:51.818144 cjunct-2.0.0/src/cjunct/console.py
--rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-2.0.0/src/cjunct/display/__init__.py
--rw-r--r--   0        0        0     1089 2024-04-08 10:02:51.819232 cjunct-2.0.0/src/cjunct/display/base.py
--rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-2.0.0/src/cjunct/display/color.py
--rw-r--r--   0        0        0     4410 2024-04-08 10:02:51.820389 cjunct-2.0.0/src/cjunct/display/default.py
--rw-r--r--   0        0        0     1466 2024-04-08 10:02:51.820998 cjunct-2.0.0/src/cjunct/exceptions.py
--rw-r--r--   0        0        0       74 2024-04-08 10:02:51.821504 cjunct-2.0.0/src/cjunct/loader/__init__.py
--rw-r--r--   0        0        0     9371 2024-04-08 10:02:51.822926 cjunct-2.0.0/src/cjunct/loader/base.py
--rw-r--r--   0        0        0     7349 2024-04-08 10:02:51.824939 cjunct-2.0.0/src/cjunct/loader/default.py
--rw-r--r--   0        0        0      980 2024-04-08 10:02:51.826557 cjunct-2.0.0/src/cjunct/loader/helpers.py
--rw-r--r--   0        0        0     1931 2024-04-08 10:02:51.831758 cjunct-2.0.0/src/cjunct/loader/inspect.py
--rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-2.0.0/src/cjunct/py.typed
--rw-r--r--   0        0        0     2929 2024-04-08 10:02:51.836589 cjunct-2.0.0/src/cjunct/rendering/__init__.py
--rw-r--r--   0        0        0     1554 2024-04-08 10:02:51.839247 cjunct-2.0.0/src/cjunct/rendering/containers.py
--rw-r--r--   0        0        0     4282 2024-04-08 10:02:51.840111 cjunct-2.0.0/src/cjunct/rendering/tokenizing.py
--rw-r--r--   0        0        0     8665 2024-04-08 10:02:51.841751 cjunct-2.0.0/src/cjunct/runner.py
--rw-r--r--   0        0        0     6213 2024-04-08 10:02:51.843759 cjunct-2.0.0/src/cjunct/strategy.py
--rw-r--r--   0        0        0      389 2024-04-08 10:02:51.845757 cjunct-2.0.0/src/cjunct/types.py
--rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-2.0.0/src/cjunct/version.py
--rw-r--r--   0        0        0     4258 2024-04-08 10:02:51.847476 cjunct-2.0.0/src/cjunct/workflow.py
--rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2428 2024-03-31 11:43:25.516186 cjunct-2.0.1/README.md
+-rw-r--r--   0        0        0     4651 2024-04-08 10:27:43.590051 cjunct-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      512 2024-04-08 10:02:51.811046 cjunct-2.0.1/src/cjunct/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-2.0.1/src/cjunct/actions/__init__.py
+-rw-r--r--   0        0        0     9912 2024-04-08 10:02:51.812886 cjunct-2.0.1/src/cjunct/actions/base.py
+-rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-2.0.1/src/cjunct/actions/bundled/__init__.py
+-rw-r--r--   0        0        0     6568 2024-03-31 11:43:25.518075 cjunct-2.0.1/src/cjunct/actions/bundled/docker_shell.py
+-rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-2.0.1/src/cjunct/actions/bundled/echo.py
+-rw-r--r--   0        0        0     2138 2024-03-19 22:06:11.634519 cjunct-2.0.1/src/cjunct/actions/bundled/shell.py
+-rw-r--r--   0        0        0      262 2024-04-08 10:02:51.814813 cjunct-2.0.1/src/cjunct/actions/constants.py
+-rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-2.0.1/src/cjunct/actions/types.py
+-rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-2.0.1/src/cjunct/config/__init__.py
+-rw-r--r--   0        0        0     3847 2024-04-08 10:02:51.815841 cjunct-2.0.1/src/cjunct/config/constants/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-01 11:54:38.652885 cjunct-2.0.1/src/cjunct/config/constants/cli.py
+-rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-2.0.1/src/cjunct/config/constants/helpers.py
+-rw-r--r--   0        0        0     2887 2024-04-08 10:02:51.817068 cjunct-2.0.1/src/cjunct/config/environment.py
+-rw-r--r--   0        0        0     4644 2024-04-08 10:02:51.818144 cjunct-2.0.1/src/cjunct/console.py
+-rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-2.0.1/src/cjunct/display/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-08 10:02:51.819232 cjunct-2.0.1/src/cjunct/display/base.py
+-rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-2.0.1/src/cjunct/display/color.py
+-rw-r--r--   0        0        0     4410 2024-04-08 10:02:51.820389 cjunct-2.0.1/src/cjunct/display/default.py
+-rw-r--r--   0        0        0     1466 2024-04-08 10:02:51.820998 cjunct-2.0.1/src/cjunct/exceptions.py
+-rw-r--r--   0        0        0       74 2024-04-08 10:02:51.821504 cjunct-2.0.1/src/cjunct/loader/__init__.py
+-rw-r--r--   0        0        0     9371 2024-04-08 10:02:51.822926 cjunct-2.0.1/src/cjunct/loader/base.py
+-rw-r--r--   0        0        0     7349 2024-04-08 10:02:51.824939 cjunct-2.0.1/src/cjunct/loader/default.py
+-rw-r--r--   0        0        0      980 2024-04-08 10:02:51.826557 cjunct-2.0.1/src/cjunct/loader/helpers.py
+-rw-r--r--   0        0        0     1931 2024-04-08 10:02:51.831758 cjunct-2.0.1/src/cjunct/loader/inspect.py
+-rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-2.0.1/src/cjunct/py.typed
+-rw-r--r--   0        0        0     2929 2024-04-08 10:02:51.836589 cjunct-2.0.1/src/cjunct/rendering/__init__.py
+-rw-r--r--   0        0        0     1554 2024-04-08 10:02:51.839247 cjunct-2.0.1/src/cjunct/rendering/containers.py
+-rw-r--r--   0        0        0     4327 2024-04-08 10:27:43.590650 cjunct-2.0.1/src/cjunct/rendering/tokenizing.py
+-rw-r--r--   0        0        0     8665 2024-04-08 10:02:51.841751 cjunct-2.0.1/src/cjunct/runner.py
+-rw-r--r--   0        0        0     6213 2024-04-08 10:02:51.843759 cjunct-2.0.1/src/cjunct/strategy.py
+-rw-r--r--   0        0        0      389 2024-04-08 10:02:51.845757 cjunct-2.0.1/src/cjunct/types.py
+-rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-2.0.1/src/cjunct/version.py
+-rw-r--r--   0        0        0     4258 2024-04-08 10:02:51.847476 cjunct-2.0.1/src/cjunct/workflow.py
+-rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-2.0.1/PKG-INFO
```

### Comparing `cjunct-2.0.0/LICENSE` & `cjunct-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/README.md` & `cjunct-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/pyproject.toml` & `cjunct-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cjunct"
-version = "2.0.0"
+version = "2.0.1"
 description = "Declarative task runner"
 license = "MIT"
 authors = [
     "Artem Novikov <artnew@list.ru>",
 ]
 readme = "README.md"
 repository = "https://github.com/reartnew/cjunct"
```

### Comparing `cjunct-2.0.0/src/cjunct/__init__.py` & `cjunct-2.0.1/src/cjunct/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/actions/base.py` & `cjunct-2.0.1/src/cjunct/actions/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/actions/bundled/docker_shell.py` & `cjunct-2.0.1/src/cjunct/actions/bundled/docker_shell.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/actions/bundled/shell.py` & `cjunct-2.0.1/src/cjunct/actions/bundled/shell.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/config/constants/__init__.py` & `cjunct-2.0.1/src/cjunct/config/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/config/constants/cli.py` & `cjunct-2.0.1/src/cjunct/config/constants/cli.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/config/constants/helpers.py` & `cjunct-2.0.1/src/cjunct/config/constants/helpers.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/config/environment.py` & `cjunct-2.0.1/src/cjunct/config/environment.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/console.py` & `cjunct-2.0.1/src/cjunct/console.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/display/base.py` & `cjunct-2.0.1/src/cjunct/display/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/display/color.py` & `cjunct-2.0.1/src/cjunct/display/color.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/display/default.py` & `cjunct-2.0.1/src/cjunct/display/default.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/exceptions.py` & `cjunct-2.0.1/src/cjunct/exceptions.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/loader/base.py` & `cjunct-2.0.1/src/cjunct/loader/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/loader/default.py` & `cjunct-2.0.1/src/cjunct/loader/default.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/loader/helpers.py` & `cjunct-2.0.1/src/cjunct/loader/helpers.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/loader/inspect.py` & `cjunct-2.0.1/src/cjunct/loader/inspect.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/rendering/__init__.py` & `cjunct-2.0.1/src/cjunct/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/rendering/containers.py` & `cjunct-2.0.1/src/cjunct/rendering/containers.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/rendering/tokenizing.py` & `cjunct-2.0.1/src/cjunct/rendering/tokenizing.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,20 +96,20 @@
                 if maybe_text := self._data[text_start:]:
                     yield self.TEXT, maybe_text
                 break
 
     def _read_expression(self) -> t.Tuple[int, str]:
         """Use a tokenizer to detect the closing brace"""
         brace_depth: int = 0
-        collected_tokens: t.List[str] = []
+        collected_tokens: t.List[t.Tuple[int, str]] = []
         tokenizer = ExpressionTokenizer(data=self._data[self._caret :])
         while True:
             token_info = tokenizer.get_token()
             if token_info.exact_type == tokenize.LBRACE:
                 brace_depth += 1
             elif token_info.exact_type == tokenize.RBRACE:
                 brace_depth -= 1
                 if brace_depth < 0:
-                    clean_expression: str = "".join(collected_tokens)
+                    clean_expression: str = tokenize.untokenize(collected_tokens)
                     return tokenizer.position, clean_expression
             if token_info.exact_type not in self._IGNORED_TOKENS_TYPES:
-                collected_tokens.append(token_info.string)
+                collected_tokens.append((token_info.type, token_info.string))
```

### Comparing `cjunct-2.0.0/src/cjunct/runner.py` & `cjunct-2.0.1/src/cjunct/runner.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/strategy.py` & `cjunct-2.0.1/src/cjunct/strategy.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/src/cjunct/workflow.py` & `cjunct-2.0.1/src/cjunct/workflow.py`

 * *Files identical despite different names*

### Comparing `cjunct-2.0.0/PKG-INFO` & `cjunct-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjunct
-Version: 2.0.0
+Version: 2.0.1
 Summary: Declarative task runner
 Home-page: https://github.com/reartnew/cjunct
 License: MIT
 Author: Artem Novikov
 Author-email: artnew@list.ru
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 4 - Beta
```

