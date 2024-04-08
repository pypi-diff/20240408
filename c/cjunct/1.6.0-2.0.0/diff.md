# Comparing `tmp/cjunct-1.6.0.tar.gz` & `tmp/cjunct-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjunct-1.6.0.tar", max compression
+gzip compressed data, was "cjunct-2.0.0.tar", max compression
```

## Comparing `cjunct-1.6.0.tar` & `cjunct-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-1.6.0/LICENSE
--rw-r--r--   0        0        0     2428 2024-03-31 11:43:25.516186 cjunct-1.6.0/README.md
--rw-r--r--   0        0        0     4668 2024-04-01 12:40:21.559835 cjunct-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      525 2024-03-24 21:45:15.470380 cjunct-1.6.0/src/cjunct/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-1.6.0/src/cjunct/actions/__init__.py
--rw-r--r--   0        0        0     9930 2024-03-31 11:43:25.517510 cjunct-1.6.0/src/cjunct/actions/base.py
--rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-1.6.0/src/cjunct/actions/bundled/__init__.py
--rw-r--r--   0        0        0     6568 2024-03-31 11:43:25.518075 cjunct-1.6.0/src/cjunct/actions/bundled/docker_shell.py
--rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-1.6.0/src/cjunct/actions/bundled/echo.py
--rw-r--r--   0        0        0     2138 2024-03-19 22:06:11.634519 cjunct-1.6.0/src/cjunct/actions/bundled/shell.py
--rw-r--r--   0        0        0      283 2024-03-19 22:06:11.635010 cjunct-1.6.0/src/cjunct/actions/constants.py
--rw-r--r--   0        0        0     4524 2024-03-19 22:06:11.635657 cjunct-1.6.0/src/cjunct/actions/net.py
--rw-r--r--   0        0        0      177 2024-03-19 22:11:38.414830 cjunct-1.6.0/src/cjunct/actions/shell.py
--rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-1.6.0/src/cjunct/actions/types.py
--rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-1.6.0/src/cjunct/config/__init__.py
--rw-r--r--   0        0        0     4052 2024-04-01 12:40:21.560998 cjunct-1.6.0/src/cjunct/config/constants/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-01 11:54:38.652885 cjunct-1.6.0/src/cjunct/config/constants/cli.py
--rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-1.6.0/src/cjunct/config/constants/helpers.py
--rw-r--r--   0        0        0     3339 2024-03-31 11:43:25.519612 cjunct-1.6.0/src/cjunct/config/environment.py
--rw-r--r--   0        0        0       79 2024-01-31 10:33:01.984083 cjunct-1.6.0/src/cjunct/config/loaders/__init__.py
--rw-r--r--   0        0        0    10681 2024-03-31 11:43:25.520459 cjunct-1.6.0/src/cjunct/config/loaders/base.py
--rw-r--r--   0        0        0        0 2024-01-31 10:33:01.985153 cjunct-1.6.0/src/cjunct/config/loaders/default/__init__.py
--rw-r--r--   0        0        0     2448 2024-03-31 11:43:25.521134 cjunct-1.6.0/src/cjunct/config/loaders/default/root.py
--rw-r--r--   0        0        0     5724 2024-03-31 11:43:25.521583 cjunct-1.6.0/src/cjunct/config/loaders/default/yaml.py
--rw-r--r--   0        0        0      963 2024-03-19 22:06:11.641292 cjunct-1.6.0/src/cjunct/config/loaders/helpers.py
--rw-r--r--   0        0        0     1931 2024-03-19 22:06:11.641758 cjunct-1.6.0/src/cjunct/config/loaders/inspect.py
--rw-r--r--   0        0        0     4983 2024-04-01 12:40:21.561983 cjunct-1.6.0/src/cjunct/console.py
--rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-1.6.0/src/cjunct/display/__init__.py
--rw-r--r--   0        0        0     1080 2024-03-20 09:52:53.055923 cjunct-1.6.0/src/cjunct/display/base.py
--rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-1.6.0/src/cjunct/display/color.py
--rw-r--r--   0        0        0     4389 2024-03-20 09:52:53.056699 cjunct-1.6.0/src/cjunct/display/default.py
--rw-r--r--   0        0        0     1335 2024-03-20 09:52:53.057410 cjunct-1.6.0/src/cjunct/exceptions.py
--rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-1.6.0/src/cjunct/py.typed
--rw-r--r--   0        0        0     5110 2024-03-19 22:06:11.645780 cjunct-1.6.0/src/cjunct/rendering.py
--rw-r--r--   0        0        0     8638 2024-03-31 11:43:25.522927 cjunct-1.6.0/src/cjunct/runner.py
--rw-r--r--   0        0        0     6162 2024-03-23 08:21:43.685535 cjunct-1.6.0/src/cjunct/strategy.py
--rw-r--r--   0        0        0      393 2024-01-31 10:33:01.991091 cjunct-1.6.0/src/cjunct/types.py
--rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-1.6.0/src/cjunct/version.py
--rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2428 2024-03-31 11:43:25.516186 cjunct-2.0.0/README.md
+-rw-r--r--   0        0        0     4651 2024-04-08 10:02:51.809616 cjunct-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      512 2024-04-08 10:02:51.811046 cjunct-2.0.0/src/cjunct/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-2.0.0/src/cjunct/actions/__init__.py
+-rw-r--r--   0        0        0     9912 2024-04-08 10:02:51.812886 cjunct-2.0.0/src/cjunct/actions/base.py
+-rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-2.0.0/src/cjunct/actions/bundled/__init__.py
+-rw-r--r--   0        0        0     6568 2024-03-31 11:43:25.518075 cjunct-2.0.0/src/cjunct/actions/bundled/docker_shell.py
+-rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-2.0.0/src/cjunct/actions/bundled/echo.py
+-rw-r--r--   0        0        0     2138 2024-03-19 22:06:11.634519 cjunct-2.0.0/src/cjunct/actions/bundled/shell.py
+-rw-r--r--   0        0        0      262 2024-04-08 10:02:51.814813 cjunct-2.0.0/src/cjunct/actions/constants.py
+-rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-2.0.0/src/cjunct/actions/types.py
+-rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-2.0.0/src/cjunct/config/__init__.py
+-rw-r--r--   0        0        0     3847 2024-04-08 10:02:51.815841 cjunct-2.0.0/src/cjunct/config/constants/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-01 11:54:38.652885 cjunct-2.0.0/src/cjunct/config/constants/cli.py
+-rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-2.0.0/src/cjunct/config/constants/helpers.py
+-rw-r--r--   0        0        0     2887 2024-04-08 10:02:51.817068 cjunct-2.0.0/src/cjunct/config/environment.py
+-rw-r--r--   0        0        0     4644 2024-04-08 10:02:51.818144 cjunct-2.0.0/src/cjunct/console.py
+-rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-2.0.0/src/cjunct/display/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-08 10:02:51.819232 cjunct-2.0.0/src/cjunct/display/base.py
+-rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-2.0.0/src/cjunct/display/color.py
+-rw-r--r--   0        0        0     4410 2024-04-08 10:02:51.820389 cjunct-2.0.0/src/cjunct/display/default.py
+-rw-r--r--   0        0        0     1466 2024-04-08 10:02:51.820998 cjunct-2.0.0/src/cjunct/exceptions.py
+-rw-r--r--   0        0        0       74 2024-04-08 10:02:51.821504 cjunct-2.0.0/src/cjunct/loader/__init__.py
+-rw-r--r--   0        0        0     9371 2024-04-08 10:02:51.822926 cjunct-2.0.0/src/cjunct/loader/base.py
+-rw-r--r--   0        0        0     7349 2024-04-08 10:02:51.824939 cjunct-2.0.0/src/cjunct/loader/default.py
+-rw-r--r--   0        0        0      980 2024-04-08 10:02:51.826557 cjunct-2.0.0/src/cjunct/loader/helpers.py
+-rw-r--r--   0        0        0     1931 2024-04-08 10:02:51.831758 cjunct-2.0.0/src/cjunct/loader/inspect.py
+-rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-2.0.0/src/cjunct/py.typed
+-rw-r--r--   0        0        0     2929 2024-04-08 10:02:51.836589 cjunct-2.0.0/src/cjunct/rendering/__init__.py
+-rw-r--r--   0        0        0     1554 2024-04-08 10:02:51.839247 cjunct-2.0.0/src/cjunct/rendering/containers.py
+-rw-r--r--   0        0        0     4282 2024-04-08 10:02:51.840111 cjunct-2.0.0/src/cjunct/rendering/tokenizing.py
+-rw-r--r--   0        0        0     8665 2024-04-08 10:02:51.841751 cjunct-2.0.0/src/cjunct/runner.py
+-rw-r--r--   0        0        0     6213 2024-04-08 10:02:51.843759 cjunct-2.0.0/src/cjunct/strategy.py
+-rw-r--r--   0        0        0      389 2024-04-08 10:02:51.845757 cjunct-2.0.0/src/cjunct/types.py
+-rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-2.0.0/src/cjunct/version.py
+-rw-r--r--   0        0        0     4258 2024-04-08 10:02:51.847476 cjunct-2.0.0/src/cjunct/workflow.py
+-rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-2.0.0/PKG-INFO
```

### Comparing `cjunct-1.6.0/LICENSE` & `cjunct-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cjunct-1.6.0/README.md` & `cjunct-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cjunct-1.6.0/pyproject.toml` & `cjunct-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cjunct"
-version = "1.6.0"
+version = "2.0.0"
 description = "Declarative task runner"
 license = "MIT"
 authors = [
     "Artem Novikov <artnew@list.ru>",
 ]
 readme = "README.md"
 repository = "https://github.com/reartnew/cjunct"
@@ -42,14 +42,15 @@
 pytest-black = "^0.3.12"
 pytest-asyncio = "^0.23.5.post1"
 pytest-bandit = "^0.6.1"
 tox = "^4.14.1"
 pytest-cov = "^4.1.0"
 types-pyyaml = "^6.0.12.20240311"
 setuptools = "^69.2.0"
+pytest-data-suites = "^1.0.5"
 
 [tool.poetry.scripts]
 cjunct = "cjunct.console:main"
 
 [tool.pytest.ini_options]
 testpaths = [
     "src",
@@ -57,26 +58,26 @@
 ]
 addopts = """
 --pylint
 --mypy
 --black
 --bandit
 """
+
 bandit_targets = ["src"]
 filterwarnings = [
     "error",
     "ignore:.*:pytest.PytestWarning",
     "ignore:.*:builtins.DeprecationWarning",
 ]
 
 [tool.coverage.run]
 source = ["src"]
 omit = [
     "src/cjunct/console.py",
-    "src/cjunct/actions/shell.py", # deprecated
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "def __repr__",
     "def __str__",
```

### Comparing `cjunct-1.6.0/src/cjunct/__init__.py` & `cjunct-2.0.0/src/cjunct/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     EmissionScannerActionBase,
 )
 from .actions.types import (
     Stderr,
     StringTemplate,
 )
 from .config.constants import C
-from .config.loaders.default.yaml import DefaultYAMLConfigLoader
-from .display.default import NetPrefixDisplay
+from .display.default import DefaultDisplay
+from .loader.default import DefaultYAMLWorkflowLoader
 from .runner import Runner
 from .strategy import (
     FreeStrategy,
     SequentialStrategy,
     LooseStrategy,
     StrictStrategy,
     StrictSequentialStrategy,
```

### Comparing `cjunct-1.6.0/src/cjunct/actions/base.py` & `cjunct-2.0.0/src/cjunct/actions/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     """Action valid states"""
 
     PENDING = "PENDING"  # Enabled, but not started yet
     RUNNING = "RUNNING"  # Execution in process
     SUCCESS = "SUCCESS"  # Finished without errors
     FAILURE = "FAILURE"  # Erroneous action
     SKIPPED = "SKIPPED"  # May be set by action itself
-    OMITTED = "OMITTED"  # Disabled during interaction or via checklists
+    OMITTED = "OMITTED"  # Disabled during interaction
 
     def __repr__(self) -> str:
         return self.name
 
     __str__ = __repr__
```

### Comparing `cjunct-1.6.0/src/cjunct/actions/bundled/docker_shell.py` & `cjunct-2.0.0/src/cjunct/actions/bundled/docker_shell.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.6.0/src/cjunct/actions/bundled/shell.py` & `cjunct-2.0.0/src/cjunct/actions/bundled/shell.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.6.0/src/cjunct/actions/net.py` & `cjunct-2.0.0/src/cjunct/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,42 @@
-"""ActionNet dedicated module"""
+"""Workflow-related module"""
 
 from __future__ import annotations
 
 import collections
 import typing as t
 
 from classlogging import LoggerMixin
 
-from .base import ActionBase, ActionDependency
-from ..exceptions import IntegrityError
+from .actions.base import ActionBase, ActionDependency
+from .exceptions import IntegrityError
 
 __all__ = [
-    "ActionNet",
+    "Workflow",
 ]
 
 
-class ActionNet(t.Dict[str, ActionBase], LoggerMixin):
+class Workflow(t.Dict[str, ActionBase], LoggerMixin):
     """Action relations map"""
 
     def __init__(
         self,
-        net: t.Dict[str, ActionBase],
-        checklists: t.Optional[t.Dict[str, t.List[str]]] = None,
+        actions_map: t.Dict[str, ActionBase],
         context: t.Optional[t.Dict[str, str]] = None,
     ) -> None:
-        super().__init__(net)
+        super().__init__(actions_map)
         self._entrypoints: t.Set[str] = set()
-        self._checklists: t.Dict[str, t.List[str]] = checklists or {}
         self._tiers_sequence: t.List[t.List[ActionBase]] = []
         self._descendants_map: t.Dict[str, t.Dict[str, ActionDependency]] = collections.defaultdict(dict)
-        self._context: t.Dict[str, str] = context or {}
+        self.context: t.Dict[str, str] = context or {}
         # Check dependencies integrity
         self._establish_descendants()
         # Create order map to check all actions are reachable
         self._allocate_tiers()
 
-    def get_context_value(self, key: str) -> t.Optional[str]:
-        """Obtain raw value of the context key"""
-        return self._context.get(key)
-
     def _establish_descendants(self) -> None:
         missing_non_external_deps: t.Set[str] = set()
         for action in self.values():  # type: ActionBase
             for dependency_action_name, dependency in list(action.ancestors.items()):
                 if dependency_action_name not in self:
                     if dependency.external:
                         # Get rid of missing external deps
@@ -55,15 +49,15 @@
             # Check if there are any dependencies after removal at all
             if not action.ancestors:
                 self._entrypoints.add(action.name)
         if missing_non_external_deps:
             raise IntegrityError(f"Missing actions among dependencies: {sorted(missing_non_external_deps)}")
         # Check entrypoints presence
         if not self._entrypoints:
-            raise IntegrityError("No entrypoints for the graph")
+            raise IntegrityError("No entrypoints for the workflow")
 
     def _allocate_tiers(self) -> None:
         """Use Dijkstra algorithm to introduce partial order.
         The tier is a group of tasks, and it's called finished when all its tasks are processed.
         Tier #0 consists of entrypoints.
         Tier #N consists of all tasks requiring exactly N-1 preceding tiers to be finished.
         """
```

### Comparing `cjunct-1.6.0/src/cjunct/config/constants/__init__.py` & `cjunct-2.0.0/src/cjunct/config/constants/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,17 +48,17 @@
     try:
         return KNOWN_STRATEGIES[name] if name else None
     except KeyError:
         raise ValueError(f"Invalid strategy name: {name!r} (allowed: {sorted(KNOWN_STRATEGIES)})") from None
 
 
 def _get_default_display_class() -> DisplayClassType:
-    from ...display.default import NetPrefixDisplay
+    from ...display.default import DefaultDisplay
 
-    return NetPrefixDisplay
+    return DefaultDisplay
 
 
 def _get_strategy_class_from_cli_arg() -> t.Optional[StrategyClassType]:
     from ...strategy import KNOWN_STRATEGIES
 
     return _maybe_strategy(get_cli_arg("strategy", valid_options=KNOWN_STRATEGIES))
 
@@ -81,33 +81,29 @@
         lambda: maybe_path(Env.CJUNCT_LOG_FILE),
     )
     ENV_FILE: Mandatory[Path] = Mandatory(
         lambda: maybe_path(Env.CJUNCT_ENV_FILE),
         lambda: Path().resolve() / ".env",
     )
     CONTEXT_DIRECTORY: Mandatory[Path] = Mandatory(
-        lambda: get_cli_arg("directory"),
-        lambda: maybe_path(Env.CJUNCT_CONTEXT_DIRECTORY),
         lambda: Path().resolve(),
     )
     INTERACTIVE_MODE: Mandatory[bool] = Mandatory(
         lambda: get_cli_arg("interactive"),
         lambda: False,
     )
     ACTIONS_SOURCE_FILE: Optional[Path] = Optional(
         lambda: maybe_path(get_cli_arg("workflow")),
-        lambda: maybe_path(get_cli_arg("file")),
         lambda: maybe_path(Env.CJUNCT_WORKFLOW_FILE),
-        lambda: maybe_path(Env.CJUNCT_ACTIONS_SOURCE_FILE),
     )
-    CONFIG_LOADER_CLASS: Optional[LoaderClassType] = Optional(
+    WORKFLOW_LOADER_CLASS: Optional[LoaderClassType] = Optional(
         lambda: maybe_class_from_module(
-            path_str=Env.CJUNCT_CONFIG_LOADER_SOURCE_FILE,
-            class_name="ConfigLoader",
-            submodule_name="config.loader",
+            path_str=Env.CJUNCT_WORKFLOW_LOADER_SOURCE_FILE,
+            class_name="WorkflowLoader",
+            submodule_name="workflow.loader",
         )
     )
     ACTION_CLASSES_DIRECTORIES: Mandatory[t.List[str]] = Mandatory(
         lambda: Env.CJUNCT_ACTIONS_CLASS_DEFINITIONS_DIRECTORY,
     )
     DISPLAY_CLASS: Mandatory[DisplayClassType] = Mandatory(
         lambda: maybe_class_from_module(
```

### Comparing `cjunct-1.6.0/src/cjunct/config/constants/cli.py` & `cjunct-2.0.0/src/cjunct/config/constants/cli.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.6.0/src/cjunct/config/constants/helpers.py` & `cjunct-2.0.0/src/cjunct/config/constants/helpers.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.6.0/src/cjunct/config/environment.py` & `cjunct-2.0.0/src/cjunct/config/environment.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,26 +22,19 @@
         Default is ERROR.
     CJUNCT_LOG_FILE:
         Specifies the log file.
         Defaults to the standard error stream.
     CJUNCT_ENV_FILE:
         Which file to load environment variables from. Expected format is k=v.
         Default is .env in the current directory.
-    CJUNCT_CONTEXT_DIRECTORY:
-        [DEPRECATED]
-        Where to look default workflow files for.
-        Default is the current directory.
-    CJUNCT_ACTIONS_SOURCE_FILE:
-        [DEPRECATED]
-        See CJUNCT_WORKFLOW_FILE.
     CJUNCT_WORKFLOW_FILE:
         Workflow file to use.
         Default behaviour is scan the current working directory.
-    CJUNCT_CONFIG_LOADER_SOURCE_FILE:
-        May point a file containing a ConfigLoader class definition, which will replace the default implementation.
+    CJUNCT_WORKFLOW_LOADER_SOURCE_FILE:
+        May point a file containing a WorkflowLoader class definition, which will replace the default implementation.
     CJUNCT_DISPLAY_SOURCE_FILE:
         May point a file containing a Display class definition, which will replace the default implementation.
     CJUNCT_STRATEGY_NAME:
         Specifies the execution strategy.
         Default is 'loose'.
     CJUNCT_FORCE_COLOR:
         When specified, this will force the colored or non-coloured output, according to the setting.
@@ -52,25 +45,23 @@
         A comma-separated list of local directories, which are added to the sys.path while loading any external modules.
         Default is an empty list.
     CJUNCT_ACTIONS_CLASS_DEFINITIONS_DIRECTORY:
         A comma-separated list of local directories, from which all `*.py` files will be considered action definitions.
         Each loaded definition is named after the filename stem and must contain an `Action` class.
         e.g. foo-bar.py may be referenced in a YAML workflow as `type: foo-bar`.
     CJUNCT_STRICT_OUTCOMES_RENDERING:
-        When set to False, rendering a missing outcome key will result in an empty string instead of an error.
-        Default is True.
+        When set to True, rendering a missing outcome key will result in an error instead of an empty string.
+        Default is False.
     """
 
     CJUNCT_LOG_LEVEL: str = OptionalString("")
     CJUNCT_LOG_FILE: str = OptionalString("")
     CJUNCT_ENV_FILE: str = OptionalString("")
-    CJUNCT_CONTEXT_DIRECTORY: str = OptionalString("")  # Will be dropped next major release.
-    CJUNCT_ACTIONS_SOURCE_FILE: str = OptionalString("")  # Will be dropped next major release.
-    CJUNCT_WORKFLOW_FILE: str = OptionalString("")  # Replaces CJUNCT_ACTIONS_SOURCE_FILE
-    CJUNCT_CONFIG_LOADER_SOURCE_FILE: str = OptionalString("")
+    CJUNCT_WORKFLOW_FILE: str = OptionalString("")
+    CJUNCT_WORKFLOW_LOADER_SOURCE_FILE: str = OptionalString("")
     CJUNCT_DISPLAY_SOURCE_FILE: str = OptionalString("")
     CJUNCT_STRATEGY_NAME: str = OptionalString("")
     CJUNCT_FORCE_COLOR: t.Optional[bool] = OptionalTernary(None)  # type: ignore
     CJUNCT_SHELL_INJECT_YIELD_FUNCTION: bool = OptionalBoolean(True)  # type: ignore
     CJUNCT_EXTERNAL_MODULES_PATHS: t.List[str] = OptionalList([])
     CJUNCT_ACTIONS_CLASS_DEFINITIONS_DIRECTORY: t.List[str] = OptionalList([])
-    CJUNCT_STRICT_OUTCOMES_RENDERING: bool = OptionalBoolean(True)  # type: ignore
+    CJUNCT_STRICT_OUTCOMES_RENDERING: bool = OptionalBoolean(False)  # type: ignore
```

### Comparing `cjunct-1.6.0/src/cjunct/config/loaders/base.py` & `cjunct-2.0.0/src/cjunct/loader/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,69 +7,46 @@
 from enum import Enum
 from pathlib import Path
 
 import dacite
 from classlogging import LoggerMixin
 
 from .inspect import get_class_annotations
-from ...actions.base import ActionBase, ArgsBase, ActionDependency
-from ...actions.net import ActionNet
-from ...actions.types import StringTemplate
-from ...exceptions import LoadError
+from ..actions.base import ActionBase, ArgsBase, ActionDependency
+from ..actions.types import StringTemplate
+from ..exceptions import LoadError
+from ..workflow import Workflow
 
 __all__ = [
-    "AbstractBaseConfigLoader",
+    "AbstractBaseWorkflowLoader",
 ]
 
 
-class AbstractBaseConfigLoader(LoggerMixin):
+class AbstractBaseWorkflowLoader(LoggerMixin):
     """Loaders base class"""
 
-    _RESERVED_CHECKLISTS_NAMES: t.Set[str] = {"ALL", "NONE"}
     STATIC_ACTION_FACTORIES: t.Dict[str, t.Type[ActionBase]] = {}
 
     def __init__(self) -> None:
         self._actions: t.Dict[str, ActionBase] = {}
         self._raw_file_names_stack: t.List[str] = []
         self._resolved_file_paths_stack: t.List[Path] = []
-        self._checklists: t.Dict[str, t.List[str]] = {}
         self._gathered_context: t.Dict[str, str] = {}
 
     def _register_action(self, action: ActionBase) -> None:
         if action.name in self._actions:
             self._throw(f"Action declared twice: {action.name!r}")
         self._actions[action.name] = action
 
     def _throw(self, message: str) -> t.NoReturn:
         """Raise loader exception from text"""
         raise LoadError(message=message, stack=self._raw_file_names_stack)
 
-    def load_checklists_from_directory(self, directory: t.Union[str, Path]) -> None:
-        """Parse checklists directory safely"""
-        directory_path: Path = Path(directory)
-        if not directory_path.is_dir():
-            self._throw(f"No such directory: {directory_path}")
-        for checklist_file in directory_path.iterdir():  # type: Path
-            if not checklist_file.is_file():
-                self._throw(f"Checklist is not a file: {checklist_file}")
-            if checklist_file.suffix != ".checklist":
-                self._throw(f"Checklist file has invalid extension: {checklist_file} (should be '.checklist')")
-            checklist_name: str = checklist_file.stem
-            if checklist_name in self._checklists:
-                self._throw(f"Checklist defined twice: {checklist_name!r}")
-            if checklist_name in self._RESERVED_CHECKLISTS_NAMES:
-                self._throw(f"Reserved checklist name used: {checklist_name!r}")
-            self._checklists[checklist_name] = [
-                action_name.strip()
-                for action_name in checklist_file.read_text(encoding="utf-8").splitlines()
-                if action_name.strip()
-            ]
-
     def _internal_load(self, source_file: t.Union[str, Path]) -> None:
-        """Load config partially from file (can be called recursively).
+        """Load workflow partially from file (can be called recursively).
         :param source_file: either Path or string object pointing at a file"""
         with self._read_file(source_file) as file_data:
             self._internal_loads(file_data)
 
     def _get_context(self) -> Path:
         """Return active context directory for relative path resolution"""
         return self._resolved_file_paths_stack[-1].parent if self._resolved_file_paths_stack else Path()
@@ -81,41 +58,41 @@
         if not source_file_raw_path.is_absolute():
             source_file_raw_path = self._get_context() / source_file_raw_path
         source_resolved_file_path = source_file_raw_path.resolve()
         if source_resolved_file_path in self._resolved_file_paths_stack:
             self._throw("Cyclic load")
         self._raw_file_names_stack.append(str(source_file))
         self._resolved_file_paths_stack.append(source_resolved_file_path)
-        self.logger.debug(f"Loading config file: {source_resolved_file_path}")
+        self.logger.debug(f"Loading workflow file: {source_resolved_file_path}")
         try:
             if not source_resolved_file_path.is_file():
-                self._throw(f"Config file not found: {source_resolved_file_path}")
+                self._throw(f"Workflow file not found: {source_resolved_file_path}")
             yield source_resolved_file_path.read_bytes()
         finally:
             self._raw_file_names_stack.pop()
             self._resolved_file_paths_stack.pop()
 
     def _internal_loads(self, data: t.Union[str, bytes]) -> None:
-        """Load config partially from text (can be called recursively)"""
+        """Load workflow partially from text (can be called recursively)"""
         raise NotImplementedError
 
     def _get_action_factory_by_type(self, action_type: str) -> t.Type[ActionBase]:
         if action_type not in self.STATIC_ACTION_FACTORIES:
             self._throw(f"Unknown dispatched type: {action_type}")
         return self.STATIC_ACTION_FACTORIES[action_type]
 
-    def loads(self, data: t.Union[str, bytes]) -> ActionNet:
-        """Load config from text"""
+    def loads(self, data: t.Union[str, bytes]) -> Workflow:
+        """Load workflow from text"""
         self._internal_loads(data=data)
-        return ActionNet(self._actions, context=self._gathered_context)
+        return Workflow(self._actions, context=self._gathered_context)
 
-    def load(self, source_file: t.Union[str, Path]) -> ActionNet:
-        """Load config from file"""
+    def load(self, source_file: t.Union[str, Path]) -> Workflow:
+        """Load workflow from file"""
         self._internal_load(source_file=source_file)
-        return ActionNet(self._actions, context=self._gathered_context)
+        return Workflow(self._actions, context=self._gathered_context)
 
     def build_dependency_from_node(self, dep_node: t.Union[str, dict]) -> t.Tuple[str, ActionDependency]:
         """Unified method to process transform dependency source data"""
         dep_holder: ActionDependency = ActionDependency()
         if isinstance(dep_node, str):
             return dep_node, dep_holder
         if isinstance(dep_node, dict):
```

### Comparing `cjunct-1.6.0/src/cjunct/config/loaders/inspect.py` & `cjunct-2.0.0/src/cjunct/loader/inspect.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.6.0/src/cjunct/console.py` & `cjunct-2.0.0/src/cjunct/console.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,30 +49,19 @@
     def make_metavar(self) -> str:
         """Fixed representation"""
         return f"[{self.NAME}]"
 
 
 @click.group
 @click.option(
-    "-d",
-    "--directory",
-    help="Context directory. Defaults to current working directory. "
-    "Also configurable via the CJUNCT_CONTEXT_DIRECTORY environment variable.",
-)
-@click.option(
     "-l",
     "--log-level",
     help="Logging level. Defaults to ERROR. Also configurable via the CJUNCT_LOG_LEVEL environment variable.",
     type=click.Choice(list(LOG_LEVELS)),
 )
-@click.option(
-    "-f",
-    "--file",
-    help="[DEPRECATED] Workflow file. It is recommended to use the positional argument instead.",
-)
 @cliargs_receiver
 def main() -> None:
     """Declarative task runner"""
 
 
 def wrap_cli_command(func):
     """Standard loading and error handling"""
@@ -126,20 +115,20 @@
         display_class=C.DISPLAY_CLASS,
     ).run_sync()
 
 
 @wrap_cli_command
 @click.argument("workflow", cls=WorkflowPositionalArgument)
 def validate() -> None:
-    """Check configuration validity."""
+    """Check workflow validity."""
     action_num: int = len(
         cjunct.Runner(
             strategy_class=C.STRATEGY_CLASS,
             display_class=C.DISPLAY_CLASS,
-        ).actions
+        ).workflow
     )
     logger.info(f"Located actions number: {action_num}")
 
 
 @main.group
 def info() -> None:
     """Package information."""
```

### Comparing `cjunct-1.6.0/src/cjunct/display/color.py` & `cjunct-2.0.0/src/cjunct/display/color.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.6.0/src/cjunct/display/default.py` & `cjunct-2.0.0/src/cjunct/display/default.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 import typing as t
 
 import inquirer  # type: ignore
 
 from .base import BaseDisplay
 from .color import Color
 from ..actions.base import ActionBase, ActionStatus
-from ..actions.net import ActionNet
 from ..actions.types import Stderr
 from ..exceptions import InteractionError
+from ..workflow import Workflow
 
 __all__ = [
-    "NetPrefixDisplay",
+    "DefaultDisplay",
 ]
 
 
-class NetPrefixDisplay(BaseDisplay):
-    """Prefix-based display for action nets"""
+class DefaultDisplay(BaseDisplay):
+    """Prefix-based default display with colors"""
 
     _STATUS_TO_COLOR: t.Dict[ActionStatus, t.Callable[[str], str]] = {
         ActionStatus.SKIPPED: Color.gray,
         ActionStatus.PENDING: Color.gray,
         ActionStatus.FAILURE: Color.red,
         ActionStatus.RUNNING: lambda x: x,
         ActionStatus.SUCCESS: Color.green,
         ActionStatus.OMITTED: Color.gray,
     }
 
-    def __init__(self, net: ActionNet) -> None:
-        super().__init__(net)
-        self._action_names_max_len = max(map(len, self._actions))
+    def __init__(self, workflow: Workflow) -> None:
+        super().__init__(workflow)
+        self._action_names_max_len = max(map(len, self._workflow))
         self._last_displayed_name: str = ""
 
     def _make_prefix(self, source_name: str, mark: str = " "):
         """Construct prefix based on previous emitter action name"""
         justification_len: int = self._action_names_max_len + 2  # "2" here stands for square brackets
         formatted_name: str = (
             f"[{source_name}]".ljust(justification_len)
@@ -62,33 +62,33 @@
                 message=f"{line_prefix}{Color.red(line)}",
             )
 
     def _display_status_banner(self) -> None:
         """Show a text banner with the status info"""
         justification_len: int = self._action_names_max_len + 9  # "9" here stands for (e.g.) "SUCCESS: "
         self.display(Color.gray("=" * justification_len))
-        for _, action in self._actions.iter_actions_by_tier():
+        for _, action in self._workflow.iter_actions_by_tier():
             color_wrapper: t.Callable[[str], str] = self._STATUS_TO_COLOR[action.status]
             self.display(f"{color_wrapper(action.status.value)}: {action.name}")
 
     def on_finish(self) -> None:
         self._display_status_banner()
 
-    def on_plan_interaction(self, net: ActionNet) -> None:
+    def on_plan_interaction(self, workflow: Workflow) -> None:
         displayed_action_names: t.List[str] = []
         default_selected_action_names: t.List[str] = []
-        for _, action in net.iter_actions_by_tier():
+        for _, action in workflow.iter_actions_by_tier():
             if action.selectable:
                 displayed_action_names.append(action.name)
                 default_selected_action_names.append(action.name)
         selected_action_names: t.List[str] = self._run_dialog(
             displayed_action_names=displayed_action_names,
             default_selected_action_names=default_selected_action_names,
         )
-        for action_name, action in net.items():
+        for action_name, action in workflow.items():
             if action_name not in selected_action_names:
                 action.disable()
 
     @classmethod
     def _run_dialog(
         cls,
         displayed_action_names: t.List[str],
```

### Comparing `cjunct-1.6.0/src/cjunct/exceptions.py` & `cjunct-2.0.0/src/cjunct/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """All intercepted errors"""
 
 import typing as t
 
 __all__ = [
     "ExecutionFailed",
     "ActionRenderError",
+    "RestrictedBuiltinError",
     "ActionUnionRenderError",
     "ActionRunError",
     "BaseError",
     "LoadError",
     "IntegrityError",
     "SourceError",
     "InteractionError",
@@ -19,14 +20,18 @@
     """Some steps failed"""
 
 
 class ActionRenderError(Exception):
     """Action rendering failed"""
 
 
+class RestrictedBuiltinError(Exception):
+    """Action rendering access to a restricted builtin function"""
+
+
 class ActionUnionRenderError(ActionRenderError):
     """Action rendering failed for union field"""
 
 
 class ActionRunError(Exception):
     """Action execution failed"""
 
@@ -43,20 +48,20 @@
     CODE: int = 102
 
     def __init__(self, message: str, stack: t.List[str]) -> None:
         self.message: str = message
         self.stack: t.List[str] = stack
         text: str = message
         if stack:
-            text += f"\n  Current config stack: {' -> '.join(stack)}"
+            text += f"\n  Sources stack: {' -> '.join(stack)}"
         super().__init__(text)
 
 
 class IntegrityError(BaseError):
-    """Action net structure error"""
+    """Workflow structure error"""
 
     CODE: int = 103
 
 
 class SourceError(BaseError):
     """Source file not recognized"""
```

### Comparing `cjunct-1.6.0/src/cjunct/runner.py` & `cjunct-2.0.0/src/cjunct/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,110 +13,110 @@
 from pathlib import Path
 
 import classlogging
 import dacite
 
 from . import types
 from .actions.base import ActionBase, ArgsBase
-from .actions.net import ActionNet
 from .actions.types import StringTemplate, RenderedStringTemplate
 from .config.constants import C
-from .config.loaders.base import AbstractBaseConfigLoader
-from .config.loaders.helpers import get_default_loader_class_for_source
 from .display.base import BaseDisplay
-from .display.default import NetPrefixDisplay
+from .display.default import DefaultDisplay
 from .exceptions import SourceError, ExecutionFailed, ActionRenderError, ActionRunError, ActionUnionRenderError
+from .loader.base import AbstractBaseWorkflowLoader
+from .loader.helpers import get_default_loader_class_for_source
 from .rendering import Templar
 from .strategy import BaseStrategy, LooseStrategy
+from .workflow import Workflow
 
 __all__ = [
     "Runner",
 ]
 
 IOType = io.TextIOBase
 
 
 class Runner(classlogging.LoggerMixin):
     """Main entry object"""
 
     def __init__(
         self,
-        config: t.Union[str, Path, IOType, None] = None,
+        source: t.Union[str, Path, IOType, None] = None,
         loader_class: t.Optional[types.LoaderClassType] = None,
         strategy_class: types.StrategyClassType = LooseStrategy,
-        display_class: types.DisplayClassType = NetPrefixDisplay,
+        display_class: types.DisplayClassType = DefaultDisplay,
     ) -> None:
-        self._config_source: t.Union[Path, IOType] = (
-            self._detect_config_source() if config is None else config if isinstance(config, IOType) else Path(config)
+        self._workflow_source: t.Union[Path, IOType] = (
+            self._detect_workflow_source() if source is None else source if isinstance(source, IOType) else Path(source)
         )
         self._loader_class: types.LoaderClassType = (
-            loader_class or C.CONFIG_LOADER_CLASS or get_default_loader_class_for_source(self._config_source)
+            loader_class or C.WORKFLOW_LOADER_CLASS or get_default_loader_class_for_source(self._workflow_source)
         )
-        self.logger.debug(f"Using config loader class: {self._loader_class}")
+        self.logger.debug(f"Using workflow loader class: {self._loader_class}")
         self._strategy_class: types.StrategyClassType = strategy_class
         self.logger.debug(f"Using strategy class: {self._strategy_class}")
         self._display_class: types.DisplayClassType = display_class
         self.logger.debug(f"Using display class: {self._display_class}")
         self._started: bool = False
         self._outcomes: t.Dict[str, t.Dict[str, t.Any]] = {}
         self._had_failed_actions: bool = False
 
     @functools.cached_property
-    def actions(self) -> ActionNet:
-        """Calculated actions net"""
-        loader: AbstractBaseConfigLoader = self._loader_class()
+    def workflow(self) -> Workflow:
+        """Calculated workflow"""
+        loader: AbstractBaseWorkflowLoader = self._loader_class()
         return (
-            loader.loads(self._config_source.read())
-            if isinstance(self._config_source, io.TextIOBase)
-            else loader.load(self._config_source)
+            loader.loads(self._workflow_source.read())
+            if isinstance(self._workflow_source, io.TextIOBase)
+            else loader.load(self._workflow_source)
         )
 
     @functools.cached_property
     def display(self) -> BaseDisplay:
         """Attached display"""
-        return self._display_class(net=self.actions)
+        return self._display_class(workflow=self.workflow)
 
     @classmethod
-    def _detect_config_source(cls) -> t.Union[Path, IOType]:
+    def _detect_workflow_source(cls) -> t.Union[Path, IOType]:
         if C.ACTIONS_SOURCE_FILE is not None:
             source_file: Path = C.ACTIONS_SOURCE_FILE
             if str(source_file) == "-":
-                cls.logger.info("Using stdin as actions source")
+                cls.logger.info("Using stdin as workflow source")
                 return t.cast(IOType, sys.stdin)
             if not source_file.exists():
-                raise SourceError(f"Pre-configured actions source file does not exist: {source_file}")
-            cls.logger.info(f"Using pre-configured actions source file: {source_file}")
+                raise SourceError(f"Given workflow file does not exist: {source_file}")
+            cls.logger.info(f"Using given workflow file: {source_file}")
             return source_file
         scan_path: Path = C.CONTEXT_DIRECTORY
         cls.logger.debug(f"Looking for workflow files at {str(scan_path)!r}")
-        located_config_file: t.Optional[Path] = None
+        located_source_file: t.Optional[Path] = None
         for candidate_file_name in (
             "cjunct.yml",
             "cjunct.yaml",
         ):  # type: str
-            if (maybe_config_file := scan_path / candidate_file_name).exists():
-                cls.logger.info(f"Detected the workflow source: {str(maybe_config_file)!r}")
-                if located_config_file is not None:
-                    raise SourceError(f"Multiple config sources detected in {scan_path}")
-                located_config_file = maybe_config_file
-        if located_config_file is None:
-            raise SourceError(f"No config source detected in {scan_path}")
-        return located_config_file
+            if (maybe_source_file := scan_path / candidate_file_name).exists():
+                cls.logger.info(f"Detected the workflow source: {str(maybe_source_file)!r}")
+                if located_source_file is not None:
+                    raise SourceError(f"Multiple workflow sources detected in {scan_path}")
+                located_source_file = maybe_source_file
+        if located_source_file is None:
+            raise SourceError(f"No workflow source detected in {scan_path}")
+        return located_source_file
 
     async def run_async(self) -> None:
         """Primary coroutine for all further processing"""
         if self._started:
             raise RuntimeError("Runner has been started more than one time")
         self._started = True
-        strategy: BaseStrategy = self._strategy_class(net=self.actions)
+        strategy: BaseStrategy = self._strategy_class(workflow=self.workflow)
         if C.INTERACTIVE_MODE:
-            self.display.on_plan_interaction(net=self.actions)
+            self.display.on_plan_interaction(workflow=self.workflow)
         background_tasks: t.List[asyncio.Task] = []
         # Prefill outcomes map
-        for action_name in self.actions:
+        for action_name in self.workflow:
             self._outcomes[action_name] = {}
         async for action in strategy:  # type: ActionBase
             if not action.enabled:
                 self.logger.debug(f"Skipping {action} as it is not enabled")
                 continue
             self.logger.trace(f"Allocating action runner for {action.name!r}")
             background_tasks.append(asyncio.create_task(self._run_action(action=action)))
@@ -143,15 +143,16 @@
             display.emit_action_message(source=action, message=message)
 
     async def _run_action(self, action: ActionBase) -> None:
         message: str
         try:
             self._render_action(action)
         except Exception as e:
-            message = f"Action {action.name!r} rendering failed: {e}"
+            details: str = str(e) if isinstance(e, ActionRenderError) else repr(e)
+            message = f"Action {action.name!r} rendering failed: {details}"
             self.display.emit_action_error(source=action, message=message)
             self.logger.warning(message, exc_info=not isinstance(e, ActionRenderError))
             action._internal_fail(e)  # pylint: disable=protected-access
             self._had_failed_actions = True
             return
         try:
             await action
@@ -169,25 +170,25 @@
     def run_sync(self):
         """Wrap async run into an event loop"""
         asyncio.run(self.run_async())
 
     def _render_action(self, action: ActionBase) -> None:
         """Prepare action to execution by rendering its template fields"""
         union_render_errors: t.List[str] = []
+        templar: Templar = Templar(
+            outcomes_map=self._outcomes,
+            action_states={name: self.workflow[name].status.value for name in self.workflow},
+            context_map=self.workflow.context,
+        )
 
         def _string_template_render_hook(value: str) -> RenderedStringTemplate:
-            templar: Templar = Templar(
-                outcomes_getter=self._outcomes.get,
-                status_getter=lambda name: self.actions[name].status.value if name in self.actions else None,
-                raw_context_getter=self.actions.get_context_value,
-            )
             try:
                 return templar.render(value)
-            except ActionRenderError as e:
-                union_render_errors.append(str(e))
+            except ActionRenderError as are:
+                union_render_errors.append(str(are))
                 raise
 
         original_args_dict: dict = asdict(action.args)
         try:
             rendered_args: ArgsBase = dacite.from_dict(
                 data_class=type(action.args),
                 data=original_args_dict,
```

### Comparing `cjunct-1.6.0/src/cjunct/strategy.py` & `cjunct-2.0.0/src/cjunct/strategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import asyncio
 import typing as t
 
 import classlogging
 
 from .actions.base import ActionStatus, ActionBase, ActionSkip
-from .actions.net import ActionNet
+from .workflow import Workflow
 
 ST = t.TypeVar("ST", bound="BaseStrategy")
 
 __all__ = [
     "BaseStrategy",
     "FreeStrategy",
     "SequentialStrategy",
@@ -30,16 +30,16 @@
 
 class BaseStrategy(classlogging.LoggerMixin, t.AsyncIterable[ActionBase]):
     """Strategy abstract base"""
 
     NAME: str = ""
     STRICT: bool = False
 
-    def __init__(self, net: ActionNet) -> None:
-        self._actions = net
+    def __init__(self, workflow: Workflow) -> None:
+        self._workflow = workflow
 
     def __aiter__(self: ST) -> ST:
         return self
 
     async def __anext__(self) -> ActionBase:
         raise NotImplementedError
 
@@ -58,31 +58,31 @@
 
 
 class FreeStrategy(BaseStrategy):
     """Free execution (fully parallel)"""
 
     NAME = "free"
 
-    def __init__(self, net: ActionNet) -> None:
-        super().__init__(net)
-        self._unprocessed: t.List[ActionBase] = list(net.values())
+    def __init__(self, workflow: Workflow) -> None:
+        super().__init__(workflow)
+        self._unprocessed: t.List[ActionBase] = list(workflow.values())
 
     async def __anext__(self) -> ActionBase:
         if not self._unprocessed:
             raise StopAsyncIteration
         return self._unprocessed.pop(0)
 
 
 class SequentialStrategy(FreeStrategy):
     """Sequential execution"""
 
     NAME = "sequential"
 
-    def __init__(self, net: ActionNet) -> None:
-        super().__init__(net)
+    def __init__(self, workflow: Workflow) -> None:
+        super().__init__(workflow)
         self._current: t.Optional[ActionBase] = None
 
     async def __anext__(self) -> ActionBase:
         if self._current is not None:
             try:
                 await self._current
             except Exception:
@@ -95,46 +95,46 @@
 
 
 class LooseStrategy(BaseStrategy):
     """Keep tracking dependencies states"""
 
     NAME = "loose"
 
-    def __init__(self, net: ActionNet) -> None:
-        super().__init__(net)
+    def __init__(self, workflow: Workflow) -> None:
+        super().__init__(workflow)
         # Actions that have been emitted by the strategy and not finished yet
         self._active_actions_map: t.Dict[str, ActionBase] = {}
         # Just a structured mutable copy of the dependency map
-        self._action_blockers: t.Dict[str, t.Set[str]] = {name: set(net[name].ancestors) for name in net}
+        self._action_blockers: t.Dict[str, t.Set[str]] = {name: set(workflow[name].ancestors) for name in workflow}
 
     def _skip_action(self, action: ActionBase) -> None:
         super()._skip_action(action)
         self._active_actions_map.pop(action.name, None)
 
     def _get_maybe_next_action(self) -> t.Optional[ActionBase]:
         """Completely non-optimal (always scan all actions), but readable yet"""
-        done_action_names: t.Set[str] = {action.name for action in self._actions.values() if action.done()}
+        done_action_names: t.Set[str] = {action.name for action in self._workflow.values() if action.done()}
         # Copy into a list for further possible pop
         for maybe_next_action_name, maybe_next_action_blockers in list(self._action_blockers.items()):
             maybe_next_action_blockers -= done_action_names
             if not maybe_next_action_blockers:
                 self.logger.debug(f"Action {maybe_next_action_name!r} is ready for scheduling")
                 self._action_blockers.pop(maybe_next_action_name)
-                next_action: ActionBase = self._actions[maybe_next_action_name]
+                next_action: ActionBase = self._workflow[maybe_next_action_name]
                 self._active_actions_map[next_action.name] = next_action
                 return next_action
         return None
 
     async def __anext__(self) -> ActionBase:
         while True:
             # Get an action and check whether to emit or to skip it
             next_action: ActionBase = await self._next_action()
             self.logger.debug(f"The next action is: {next_action}")
             for ancestor_name, ancestor_dependency in next_action.ancestors.items():
-                ancestor: ActionBase = self._actions[ancestor_name]
+                ancestor: ActionBase = self._workflow[ancestor_name]
                 if ancestor.status in (ActionStatus.FAILURE, ActionStatus.SKIPPED) and (
                     ancestor_dependency.strict or self.STRICT
                 ):
                     self.logger.debug(f"Action {next_action} is qualified as skipped due to strict failure: {ancestor}")
                     self._skip_action(next_action)
                     break
             else:
```

### Comparing `cjunct-1.6.0/PKG-INFO` & `cjunct-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjunct
-Version: 1.6.0
+Version: 2.0.0
 Summary: Declarative task runner
 Home-page: https://github.com/reartnew/cjunct
 License: MIT
 Author: Artem Novikov
 Author-email: artnew@list.ru
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 4 - Beta
```

