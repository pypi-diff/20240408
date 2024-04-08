# Comparing `tmp/dev_toolbox-0.1.8.tar.gz` & `tmp/dev_toolbox-0.1.9.tar.gz`

## Comparing `dev_toolbox-0.1.8.tar` & `dev_toolbox-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/taplo.toml
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/.github/workflows/main.yml
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/.vscode/settings.json
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/__main__.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/_types.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/_version.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/attrdict.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/multi_file.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/cli/__init__.py
--rwxr-xr-x   0        0        0     1898 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/cli/tree.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/cli/version_bump.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/data_structures/__init__.py
--rwxr-xr-x   0        0        0     3549 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/data_structures/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/decorators/__init__.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/decorators/timer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/reflection_tools/__init__.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/src/dev_toolbox/reflection_tools/class_hierarchy.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/tests/attrdict_test.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/tests/timer_test.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/LICENSE
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/README.md
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 dev_toolbox-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/taplo.toml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/.vscode/settings.json
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/__main__.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/_types.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/_version.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/attrdict.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/multi_file.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/cli/__init__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/cli/html_table.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/cli/ruff_doc.py
+-rwxr-xr-x   0        0        0     1898 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/cli/tree.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/cli/version_bump.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/data_structures/__init__.py
+-rwxr-xr-x   0        0        0     3549 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/data_structures/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/decorators/__init__.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/decorators/timer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/reflection_tools/__init__.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/src/dev_toolbox/reflection_tools/class_hierarchy.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/tests/attrdict_test.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/tests/timer_test.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/LICENSE
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/README.md
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 dev_toolbox-0.1.9/PKG-INFO
```

### Comparing `dev_toolbox-0.1.8/.pre-commit-config.yaml` & `dev_toolbox-0.1.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
       - id: taplo
   - repo: https://github.com/asottile/reorder-python-imports
     rev: v3.12.0
     hooks:
       - id: reorder-python-imports
         args: [--py37-plus, --add-import, "from __future__ import annotations"]
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.0
+    rev: v0.3.4
     hooks:
       - id: ruff
         types_or: [python, pyi, jupyter]
         args: [--fix]
       - id: ruff-format
         types_or: [python, pyi, jupyter]
   - repo: https://github.com/pre-commit/pre-commit-hooks
@@ -24,15 +24,15 @@
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: debug-statements
       - id: name-tests-test
       - id: requirements-txt-fixer
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         additional_dependencies: [types-all]
   - repo: local
     hooks:
       - id: hatch-test
         name: hatch-test
```

### Comparing `dev_toolbox-0.1.8/taplo.toml` & `dev_toolbox-0.1.9/taplo.toml`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/.vscode/settings.json` & `dev_toolbox-0.1.9/.vscode/settings.json`

 * *Files 15% similar despite different names*

```diff
@@ -23,9 +23,16 @@
     "--application-directories=.:src",
     "--add-import 'from __future__ import annotations'",
   ],
   "python.testing.pytestArgs": [
     "tests"
   ],
   "python.testing.unittestEnabled": false,
-  "python.testing.pytestEnabled": true
+  "python.testing.pytestEnabled": true,
+  "python.analysis.typeCheckingMode": "basic",
+  "python.analysis.exclude": [
+    "reportShadowedImports"
+  ],
+  "python.analysis.diagnosticSeverityOverrides": {
+    "reportShadowedImports": "none"
+  }
 }
```

### Comparing `dev_toolbox-0.1.8/src/dev_toolbox/attrdict.py` & `dev_toolbox-0.1.9/src/dev_toolbox/attrdict.py`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/src/dev_toolbox/multi_file.py` & `dev_toolbox-0.1.9/src/dev_toolbox/multi_file.py`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/src/dev_toolbox/cli/tree.py` & `dev_toolbox-0.1.9/src/dev_toolbox/cli/tree.py`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/src/dev_toolbox/cli/version_bump.py` & `dev_toolbox-0.1.9/src/dev_toolbox/cli/version_bump.py`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/src/dev_toolbox/data_structures/tree.py` & `dev_toolbox-0.1.9/src/dev_toolbox/data_structures/tree.py`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/src/dev_toolbox/decorators/timer.py` & `dev_toolbox-0.1.9/src/dev_toolbox/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/src/dev_toolbox/reflection_tools/class_hierarchy.py` & `dev_toolbox-0.1.9/src/dev_toolbox/reflection_tools/class_hierarchy.py`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/tests/attrdict_test.py` & `dev_toolbox-0.1.9/tests/attrdict_test.py`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/tests/timer_test.py` & `dev_toolbox-0.1.9/tests/timer_test.py`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/.gitignore` & `dev_toolbox-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/LICENSE` & `dev_toolbox-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/README.md` & `dev_toolbox-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dev_toolbox-0.1.8/pyproject.toml` & `dev_toolbox-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 Source = "https://github.com/FlavioAmurrioCS/dev-toolbox"
 
 [project.scripts]
 dev-toolbox = "dev_toolbox.cli:dev_toolbox"
 dev-hierarchy = "dev_toolbox.reflection_tools.class_hierarchy:main"
 dev-tree = "dev_toolbox.cli.tree:main"
 dev-version-bump = "dev_toolbox.cli.version_bump:main"
+dev-ruff-doc = "dev_toolbox.cli.ruff_doc:main"
+dev-html-table = "dev_toolbox.cli.html_table:main"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/dev_toolbox/_version.py"
```

### Comparing `dev_toolbox-0.1.8/PKG-INFO` & `dev_toolbox-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dev-toolbox
-Version: 0.1.8
+Version: 0.1.9
 Project-URL: Documentation, https://github.com/FlavioAmurrioCS/dev-toolbox#readme
 Project-URL: Issues, https://github.com/FlavioAmurrioCS/dev-toolbox/issues
 Project-URL: Source, https://github.com/FlavioAmurrioCS/dev-toolbox
 Author-email: Flavio Amurrio <25621374+FlavioAmurrioCS@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

