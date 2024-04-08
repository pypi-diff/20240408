# Comparing `tmp/validate_pyproject_schema_store-2024.3.25.tar.gz` & `tmp/validate_pyproject_schema_store-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Mon Apr  1 09:17:48 2024, max compression
```

## Comparing `validate_pyproject_schema_store-2024.3.25.tar` & `validate_pyproject_schema_store-2024.4.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/.pre-commit-config.yaml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/.github/workflows/bump.yml
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/.github/workflows/ci.yml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/py.typed
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/schema.py
--rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/black.schema.json
--rw-r--r--   0        0        0    20516 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
--rw-r--r--   0        0        0    25903 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/hatch.schema.json
--rw-r--r--   0        0        0    44330 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/mypy.schema.json
--rw-r--r--   0        0        0    25354 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/pdm.schema.json
--rw-r--r--   0        0        0    20021 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/poetry.schema.json
--rw-r--r--   0        0        0    63177 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/pyright.schema.json
--rw-r--r--   0        0        0   124654 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/ruff.schema.json
--rw-r--r--   0        0        0    18672 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
--rw-r--r--   0        0        0    13647 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/setuptools.schema.json
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/tool.json
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/tests/test_package.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/tests/test_validate_pyproject.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/tools/sync.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/LICENSE
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/README.md
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/pyproject.toml
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 validate_pyproject_schema_store-2024.3.25/PKG-INFO
+-rw-r--r--   0        0        0     2272 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      305 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     2412 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1007 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/.github/workflows/bump.yml
+-rw-r--r--   0        0        0      843 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1193 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      188 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/py.typed
+-rw-r--r--   0        0        0     1373 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/schema.py
+-rw-r--r--   0        0        0     6871 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/black.schema.json
+-rw-r--r--   0        0        0    20516 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
+-rw-r--r--   0        0        0    25903 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/hatch.schema.json
+-rw-r--r--   0        0        0    44330 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/mypy.schema.json
+-rw-r--r--   0        0        0    25354 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/pdm.schema.json
+-rw-r--r--   0        0        0    20021 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/poetry.schema.json
+-rw-r--r--   0        0        0    63177 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/pyright.schema.json
+-rw-r--r--   0        0        0   125702 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/ruff.schema.json
+-rw-r--r--   0        0        0    18672 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
+-rw-r--r--   0        0        0    13647 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/setuptools.schema.json
+-rw-r--r--   0        0        0      643 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/tool.json
+-rw-r--r--   0        0        0      890 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/tests/test_package.py
+-rw-r--r--   0        0        0      425 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/tests/test_validate_pyproject.py
+-rw-r--r--   0        0        0     2422 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/tools/sync.py
+-rw-r--r--   0        0        0     2218 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/.gitignore
+-rw-r--r--   0        0        0    11358 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/LICENSE
+-rw-r--r--   0        0        0     2081 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/README.md
+-rw-r--r--   0        0        0     5445 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4100 2024-04-01 09:17:48.000000 validate_pyproject_schema_store-2024.4.1/PKG-INFO
```

### Comparing `validate_pyproject_schema_store-2024.3.25/.pre-commit-config.yaml` & `validate_pyproject_schema_store-2024.4.1/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
-  - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: "23.10.1"
-    hooks:
-      - id: black-jupyter
-
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==23.*]
+        additional_dependencies: [black==24.*]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.5.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
@@ -26,37 +21,31 @@
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: name-tests-test
         args: ["--pytest-test-first"]
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: "v1.10.0"
-    hooks:
-      - id: rst-backticks
-      - id: rst-directive-colons
-      - id: rst-inline-touching-normal
-
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.3"
+    rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: '^src/validate_pyproject_schema_store/resources/.*\.json'
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.1.3"
+    rev: "v0.3.4"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
+      - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.6.1"
+    rev: "v1.9.0"
     hooks:
       - id: mypy
         files: src|tests|tools
         args: []
         additional_dependencies:
           - pytest
           - importlib_resources
@@ -67,30 +56,30 @@
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.6"
     hooks:
       - id: codespell
         args: ["-Lcrate"]
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: "v0.9.0.6"
+    rev: "v0.10.0.1"
     hooks:
       - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
         exclude: .pre-commit-config.yaml
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.15
+    rev: v0.16
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.27.0
+    rev: 0.28.1
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
```

### Comparing `validate_pyproject_schema_store-2024.3.25/.github/CONTRIBUTING.md` & `validate_pyproject_schema_store-2024.4.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/.github/matchers/pylint.json` & `validate_pyproject_schema_store-2024.4.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/.github/workflows/bump.yml` & `validate_pyproject_schema_store-2024.4.1/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/.github/workflows/ci.yml` & `validate_pyproject_schema_store-2024.4.1/.github/workflows/ci.yml`

 * *Files 21% similar despite different names*

```diff
@@ -11,32 +11,17 @@
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 env:
   FORCE_COLOR: 3
 
 jobs:
-  pre-commit:
-    name: Format
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v4
-        with:
-          fetch-depth: 0
-      - uses: actions/setup-python@v5
-        with:
-          python-version: "3.x"
-      - uses: pre-commit/action@v3.0.1
-        with:
-          extra_args: --hook-stage manual --all-files
-
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
-    needs: [pre-commit]
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.8", "3.12"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
         include:
@@ -49,16 +34,21 @@
           fetch-depth: 0
 
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           allow-prereleases: true
 
+      - name: Setup uv
+        uses: yezz123/setup-uv@v4
+        with:
+          uv-venv: ".venv"
+
       - name: Install package
-        run: python -m pip install .[test]
+        run: uv pip install -e .[test]
 
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20
 
       - name: Upload coverage report
```

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/schema.py` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/schema.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/black.schema.json` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/black.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/hatch.schema.json` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/hatch.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/mypy.schema.json` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/mypy.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/pdm.schema.json` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/pdm.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/poetry.schema.json` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/poetry.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/pyright.schema.json` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/pyright.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/ruff.schema.json` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/ruff.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944766418661185%*

 * *Differences: {"'definitions'": "{'Flake8CopyrightOptions': {'properties': {'author': {'type': {insert: [(1, "*

 * *                  "'string')], delete: [0]}}, 'notice-rgx': {'description': 'The regular "*

 * *                  'expression used to match the copyright notice, compiled with the '*

 * *                  '[`regex`](https://docs.rs/regex/latest/regex/) crate. Defaults to '*

 * *                  '`(?i)Copyright\\\\s+((?:\\\\(C\\\\)|©)\\\\s+)?\\\\d{4}((-|,\\\\s)\\\\d{4})*`, '*

 * *                  'which matches the following: - `C […]*

```diff
@@ -12,14 +12,20 @@
                 }
             },
             "required": [
                 "msg"
             ],
             "type": "object"
         },
+        "BannedAliases": {
+            "items": {
+                "type": "string"
+            },
+            "type": "array"
+        },
         "ConstantType": {
             "enum": [
                 "bytes",
                 "complex",
                 "float",
                 "int",
                 "str"
@@ -196,44 +202,44 @@
         },
         "Flake8CopyrightOptions": {
             "additionalProperties": false,
             "properties": {
                 "author": {
                     "description": "Author to enforce within the copyright notice. If provided, the author must be present immediately following the copyright notice.",
                     "type": [
-                        "string",
-                        "null"
+                        "null",
+                        "string"
                     ]
                 },
                 "min-file-size": {
                     "description": "A minimum file size (in bytes) required for a copyright notice to be enforced. By default, all files are validated.",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "notice-rgx": {
-                    "description": "The regular expression used to match the copyright notice, compiled with the [`regex`](https://docs.rs/regex/latest/regex/) crate.\n\nDefaults to `(?i)Copyright\\s+((?:\\(C\\)|\u00a9)\\s+)?\\d{4}(-\\d{4})*`, which matches the following: - `Copyright 2023` - `Copyright (C) 2023` - `Copyright 2021-2023` - `Copyright (C) 2021-2023`",
+                    "description": "The regular expression used to match the copyright notice, compiled with the [`regex`](https://docs.rs/regex/latest/regex/) crate. Defaults to `(?i)Copyright\\s+((?:\\(C\\)|\u00a9)\\s+)?\\d{4}((-|,\\s)\\d{4})*`, which matches the following: - `Copyright 2023` - `Copyright (C) 2023` - `Copyright 2021-2023` - `Copyright (C) 2021-2023` - `Copyright (C) 2021, 2023`",
                     "type": [
-                        "string",
-                        "null"
+                        "null",
+                        "string"
                     ]
                 }
             },
             "type": "object"
         },
         "Flake8ErrMsgOptions": {
             "additionalProperties": false,
             "properties": {
                 "max-string-length": {
                     "description": "Maximum string length for string literals in exception messages.",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 }
             },
             "type": "object"
@@ -282,29 +288,26 @@
             "properties": {
                 "aliases": {
                     "additionalProperties": {
                         "type": "string"
                     },
                     "description": "The conventional aliases for imports. These aliases can be extended by the `extend_aliases` option.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "banned-aliases": {
                     "additionalProperties": {
-                        "items": {
-                            "type": "string"
-                        },
-                        "type": "array"
+                        "$ref": "#/definitions/BannedAliases"
                     },
                     "description": "A mapping from module to its banned import aliases.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "banned-from": {
                     "description": "A list of modules that should not be imported from using the `from ... import ...` syntax.\n\nFor example, given `banned-from = [\"pandas\"]`, `from pandas import DataFrame` would be disallowed, while `import pandas` would be allowed.",
                     "items": {
                         "type": "string"
                     },
@@ -316,16 +319,16 @@
                 },
                 "extend-aliases": {
                     "additionalProperties": {
                         "type": "string"
                     },
                     "description": "A mapping from module to conventional import alias. These aliases will be added to the `aliases` mapping.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 }
             },
             "type": "object"
         },
         "Flake8PytestStyleOptions": {
             "additionalProperties": false,
@@ -488,16 +491,16 @@
                 },
                 "banned-api": {
                     "additionalProperties": {
                         "$ref": "#/definitions/ApiBan"
                     },
                     "description": "Specific modules or module members that may not be imported or accessed. Note that this rule is only meant to flag accidental uses, and can be circumvented via `eval` or `importlib`.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "banned-module-level-imports": {
                     "description": "List of specific modules that may not be imported at module level, and should instead be imported lazily (e.g., within a function definition, or an `if TYPE_CHECKING:` block, or some other nested context).",
                     "items": {
                         "type": "string"
                     },
@@ -573,15 +576,15 @@
             "type": "object"
         },
         "FormatOptions": {
             "additionalProperties": false,
             "description": "Configures the way ruff formats your code.",
             "properties": {
                 "docstring-code-format": {
-                    "description": "Whether to format code snippets in docstrings.\n\nWhen this is enabled, Python code examples within docstrings are automatically reformatted.\n\nFor example, when this is enabled, the following code:\n\n```python def f(x): \"\"\" Something about `f`. And an example in doctest format:\n\n>>> f(  x  )\n\nMarkdown is also supported:\n\n```py f(  x  ) ```\n\nAs are reStructuredText literal blocks::\n\nf(  x  )\n\nAnd reStructuredText code blocks:\n\n.. code-block:: python\n\nf(  x  ) \"\"\" pass ```\n\n... will be reformatted (assuming the rest of the options are set to their defaults) as:\n\n```python def f(x): \"\"\" Something about `f`. And an example in doctest format:\n\n>>> f(x)\n\nMarkdown is also supported:\n\n```py f(x) ```\n\nAs are reStructuredText literal blocks::\n\nf(x)\n\nAnd reStructuredText code blocks:\n\n.. code-block:: python\n\nf(x) \"\"\" pass ```\n\nIf a code snippt in a docstring contains invalid Python code or if the formatter would otherwise write invalid Python code, then the code example is ignored by the formatter and kept as-is.\n\nCurrently, doctest, Markdown, reStructuredText literal blocks, and reStructuredText code blocks are all supported and automatically recognized. In the case of unlabeled fenced code blocks in Markdown and reStructuredText literal blocks, the contents are assumed to be Python and reformatted. As with any other format, if the contents aren't valid Python, then the block is left untouched automatically.",
+                    "description": "Whether to format code snippets in docstrings.\n\nWhen this is enabled, Python code examples within docstrings are automatically reformatted.\n\nFor example, when this is enabled, the following code:\n\n```python def f(x): \"\"\" Something about `f`. And an example in doctest format:\n\n>>> f(  x  )\n\nMarkdown is also supported:\n\n```py f(  x  ) ```\n\nAs are reStructuredText literal blocks::\n\nf(  x  )\n\nAnd reStructuredText code blocks:\n\n.. code-block:: python\n\nf(  x  ) \"\"\" pass ```\n\n... will be reformatted (assuming the rest of the options are set to their defaults) as:\n\n```python def f(x): \"\"\" Something about `f`. And an example in doctest format:\n\n>>> f(x)\n\nMarkdown is also supported:\n\n```py f(x) ```\n\nAs are reStructuredText literal blocks::\n\nf(x)\n\nAnd reStructuredText code blocks:\n\n.. code-block:: python\n\nf(x) \"\"\" pass ```\n\nIf a code snippet in a docstring contains invalid Python code or if the formatter would otherwise write invalid Python code, then the code example is ignored by the formatter and kept as-is.\n\nCurrently, doctest, Markdown, reStructuredText literal blocks, and reStructuredText code blocks are all supported and automatically recognized. In the case of unlabeled fenced code blocks in Markdown and reStructuredText literal blocks, the contents are assumed to be Python and reformatted. As with any other format, if the contents aren't valid Python, then the block is left untouched automatically.",
                     "type": [
                         "boolean",
                         "null"
                     ]
                 },
                 "docstring-code-line-length": {
                     "anyOf": [
@@ -662,19 +665,19 @@
                 {
                     "type": "string"
                 }
             ]
         },
         "ImportType": {
             "enum": [
+                "first-party",
                 "future",
+                "local-folder",
                 "standard-library",
-                "third-party",
-                "first-party",
-                "local-folder"
+                "third-party"
             ],
             "type": "string"
         },
         "IndentStyle": {
             "oneOf": [
                 {
                     "description": "Use tabs to indent code.",
@@ -691,15 +694,15 @@
                     "type": "string"
                 }
             ]
         },
         "IndentWidth": {
             "description": "The size of a tab.",
             "format": "uint8",
-            "minimum": 1.0,
+            "minimum": 1,
             "type": "integer"
         },
         "IsortOptions": {
             "additionalProperties": false,
             "properties": {
                 "case-sensitive": {
                     "description": "Sort imports taking into account case sensitivity.",
@@ -731,14 +734,25 @@
                         "type": "string"
                     },
                     "type": [
                         "array",
                         "null"
                     ]
                 },
+                "default-section": {
+                    "anyOf": [
+                        {
+                            "$ref": "#/definitions/ImportSection"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "description": "Define a default section for any imports that don't fit into the specified `section-order`."
+                },
                 "detect-same-package": {
                     "description": "Whether to automatically mark imports from within the same package as first-party. For example, when `detect-same-package = true`, then when analyzing files within the `foo` package, any imports from within the `foo` package will be considered first-party.\n\nThis heuristic is often unnecessary when `src` is configured to detect all first-party sources; however, if `src` is _not_ configured, this heuristic can be useful to detect first-party imports from _within_ (but not _across_) first-party packages.",
                     "type": [
                         "boolean",
                         "null"
                     ]
                 },
@@ -851,15 +865,15 @@
                         "integer",
                         "null"
                     ]
                 },
                 "lines-between-types": {
                     "description": "The number of lines to place between \"direct\" and `import from` imports.\n\nWhen using the formatter, only the values `0` and `1` are compatible because it preserves up to one empty line after imports in nested blocks.",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "no-lines-before": {
                     "description": "A list of sections that should _not_ be delineated from the previous section via empty lines.",
@@ -921,16 +935,16 @@
                         "items": {
                             "type": "string"
                         },
                         "type": "array"
                     },
                     "description": "A list of mappings from section names to modules. By default custom sections are output last, but this can be overridden with `section-order`.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "single-line-exclusions": {
                     "description": "One or more modules to exclude from the single line rule.",
                     "items": {
                         "type": "string"
                     },
@@ -990,22 +1004,22 @@
                     "type": "string"
                 }
             ]
         },
         "LineLength": {
             "description": "The length of a line of text that is considered too long.\n\nThe allowed range of values is 1..=320",
             "format": "uint16",
-            "maximum": 320.0,
-            "minimum": 1.0,
+            "maximum": 320,
+            "minimum": 1,
             "type": "integer"
         },
         "LineWidth": {
             "description": "The maximum visual width to which the formatter should try to limit a line.",
             "format": "uint16",
-            "minimum": 1.0,
+            "minimum": 1,
             "type": "integer"
         },
         "LintOptions": {
             "additionalProperties": false,
             "description": "Configures how ruff checks your code.\n\nOptions specified in the `lint` section take precedence over the deprecated top-level settings.",
             "properties": {
                 "allowed-confusables": {
@@ -1019,16 +1033,16 @@
                         "array",
                         "null"
                     ]
                 },
                 "dummy-variable-rgx": {
                     "description": "A regular expression used to identify \"dummy\" variables, or those which should be ignored when enforcing (e.g.) unused-variable rules. The default expression matches `_`, `__`, and `_var`, but not `_var_`.",
                     "type": [
-                        "string",
-                        "null"
+                        "null",
+                        "string"
                     ]
                 },
                 "exclude": {
                     "description": "A list of file patterns to exclude from linting in addition to the files excluded globally (see [`exclude`](#exclude), and [`extend-exclude`](#extend-exclude)).\n\nExclusions are based on globs, and can be either:\n\n- Single-path patterns, like `.mypy_cache` (to exclude any directory named `.mypy_cache` in the tree), `foo.py` (to exclude any file named `foo.py`), or `foo_*.py` (to exclude any file matching `foo_*.py` ). - Relative patterns, like `directory/foo.py` (to exclude that specific file) or `directory/*.py` (to exclude any Python files in `directory`). Note that these paths are relative to the project root (e.g., the directory containing your `pyproject.toml`).\n\nFor more information on the glob syntax, refer to the [`globset` documentation](https://docs.rs/globset/latest/globset/#syntax).",
                     "items": {
                         "type": "string"
                     },
@@ -1070,16 +1084,16 @@
                         "items": {
                             "$ref": "#/definitions/RuleSelector"
                         },
                         "type": "array"
                     },
                     "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, in addition to any rules excluded by `per-file-ignores`.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "extend-safe-fixes": {
                     "description": "A list of rule codes or prefixes for which unsafe fixes should be considered safe.",
                     "items": {
                         "$ref": "#/definitions/RuleSelector"
                     },
@@ -1322,15 +1336,15 @@
                     },
                     "type": [
                         "array",
                         "null"
                     ]
                 },
                 "ignore-init-module-imports": {
-                    "description": "Avoid automatically removing unused imports in `__init__.py` files. Such imports will still be flagged, but with a dedicated message suggesting that the import is either added to the module's `__all__` symbol, or re-exported with a redundant alias (e.g., `import os as os`).",
+                    "description": "Avoid automatically removing unused imports in `__init__.py` files. Such imports will still be flagged, but with a dedicated message suggesting that the import is either added to the module's `__all__` symbol, or re-exported with a redundant alias (e.g., `import os as os`).\n\nThis option is enabled by default, but you can opt-in to removal of imports via an unsafe fix.",
                     "type": [
                         "boolean",
                         "null"
                     ]
                 },
                 "isort": {
                     "anyOf": [
@@ -1380,16 +1394,16 @@
                         "items": {
                             "$ref": "#/definitions/RuleSelector"
                         },
                         "type": "array"
                     },
                     "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, when considering any matching files.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "preview": {
                     "description": "Whether to enable preview mode. When preview mode is enabled, Ruff will use unstable rules and fixes.",
                     "type": [
                         "boolean",
                         "null"
@@ -1495,42 +1509,42 @@
         },
         "McCabeOptions": {
             "additionalProperties": false,
             "properties": {
                 "max-complexity": {
                     "description": "The maximum McCabe complexity to allow before triggering `C901` errors.",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 }
             },
             "type": "object"
         },
         "ParametrizeNameType": {
             "enum": [
                 "csv",
-                "tuple",
-                "list"
+                "list",
+                "tuple"
             ],
             "type": "string"
         },
         "ParametrizeValuesRowType": {
             "enum": [
-                "tuple",
-                "list"
+                "list",
+                "tuple"
             ],
             "type": "string"
         },
         "ParametrizeValuesType": {
             "enum": [
-                "tuple",
-                "list"
+                "list",
+                "tuple"
             ],
             "type": "string"
         },
         "Pep8NamingOptions": {
             "additionalProperties": false,
             "properties": {
                 "classmethod-decorators": {
@@ -1700,103 +1714,103 @@
                         "array",
                         "null"
                     ]
                 },
                 "max-args": {
                     "description": "Maximum number of arguments allowed for a function or method definition (see: `PLR0913`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-bool-expr": {
                     "description": "Maximum number of Boolean expressions allowed within a single `if` statement (see: `PLR0916`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-branches": {
                     "description": "Maximum number of branches allowed for a function or method body (see: `PLR0912`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-locals": {
                     "description": "Maximum number of local variables allowed for a function or method body (see: `PLR0914`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-nested-blocks": {
                     "description": "Maximum number of nested blocks allowed within a function or method body (see: `PLR1702`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-positional-args": {
                     "description": "Maximum number of positional arguments allowed for a function or method definition (see: `PLR0917`).\n\nIf not specified, defaults to the value of `max-args`.",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-public-methods": {
                     "description": "Maximum number of public methods allowed for a class (see: `PLR0904`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-returns": {
                     "description": "Maximum number of return statements allowed for a function or method body (see `PLR0911`)",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-statements": {
                     "description": "Maximum number of statements allowed for a function or method body (see: `PLR0915`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 }
             },
             "type": "object"
         },
         "PythonVersion": {
             "enum": [
-                "py37",
-                "py38",
-                "py39",
                 "py310",
                 "py311",
-                "py312"
+                "py312",
+                "py37",
+                "py38",
+                "py39"
             ],
             "type": "string"
         },
         "Quote": {
             "oneOf": [
                 {
                     "description": "Use double quotes.",
@@ -1812,17 +1826,17 @@
                     ],
                     "type": "string"
                 }
             ]
         },
         "QuoteStyle": {
             "enum": [
-                "single",
                 "double",
-                "preserve"
+                "preserve",
+                "single"
             ],
             "type": "string"
         },
         "RelativeImportsOrder": {
             "oneOf": [
                 {
                     "description": "Place \"closer\" imports (fewer `.` characters, most local) before \"further\" imports (more `.` characters, least local).",
@@ -1836,14 +1850,17 @@
                     "enum": [
                         "furthest-to-closest"
                     ],
                     "type": "string"
                 }
             ]
         },
+        "RequiredVersion": {
+            "type": "string"
+        },
         "RuleSelector": {
             "enum": [
                 "A",
                 "A0",
                 "A00",
                 "A001",
                 "A002",
@@ -2109,14 +2126,15 @@
                 "E4",
                 "E40",
                 "E401",
                 "E402",
                 "E5",
                 "E50",
                 "E501",
+                "E502",
                 "E7",
                 "E70",
                 "E701",
                 "E702",
                 "E703",
                 "E71",
                 "E711",
@@ -2268,14 +2286,15 @@
                 "FURB169",
                 "FURB17",
                 "FURB171",
                 "FURB177",
                 "FURB18",
                 "FURB180",
                 "FURB181",
+                "FURB187",
                 "G",
                 "G0",
                 "G00",
                 "G001",
                 "G002",
                 "G003",
                 "G004",
@@ -2446,25 +2465,27 @@
                 "PLE",
                 "PLE0",
                 "PLE01",
                 "PLE010",
                 "PLE0100",
                 "PLE0101",
                 "PLE011",
+                "PLE0115",
                 "PLE0116",
                 "PLE0117",
                 "PLE0118",
                 "PLE02",
                 "PLE023",
                 "PLE0237",
                 "PLE024",
                 "PLE0241",
                 "PLE03",
                 "PLE030",
                 "PLE0302",
+                "PLE0304",
                 "PLE0307",
                 "PLE06",
                 "PLE060",
                 "PLE0604",
                 "PLE0605",
                 "PLE064",
                 "PLE0643",
@@ -2487,14 +2508,18 @@
                 "PLE1300",
                 "PLE1307",
                 "PLE131",
                 "PLE1310",
                 "PLE15",
                 "PLE150",
                 "PLE1507",
+                "PLE151",
+                "PLE1519",
+                "PLE152",
+                "PLE1520",
                 "PLE17",
                 "PLE170",
                 "PLE1700",
                 "PLE2",
                 "PLE25",
                 "PLE250",
                 "PLE2502",
@@ -2562,20 +2587,24 @@
                 "PLR630",
                 "PLR6301",
                 "PLW",
                 "PLW0",
                 "PLW01",
                 "PLW010",
                 "PLW0108",
+                "PLW011",
+                "PLW0117",
                 "PLW012",
                 "PLW0120",
                 "PLW0127",
+                "PLW0128",
                 "PLW0129",
                 "PLW013",
                 "PLW0131",
+                "PLW0133",
                 "PLW02",
                 "PLW024",
                 "PLW0245",
                 "PLW04",
                 "PLW040",
                 "PLW0406",
                 "PLW06",
@@ -2878,14 +2907,15 @@
                 "S604",
                 "S605",
                 "S606",
                 "S607",
                 "S608",
                 "S609",
                 "S61",
+                "S610",
                 "S611",
                 "S612",
                 "S7",
                 "S70",
                 "S701",
                 "S702",
                 "SIM",
@@ -3053,14 +3083,17 @@
                 "W19",
                 "W191",
                 "W2",
                 "W29",
                 "W291",
                 "W292",
                 "W293",
+                "W3",
+                "W39",
+                "W391",
                 "W5",
                 "W50",
                 "W505",
                 "W6",
                 "W60",
                 "W605",
                 "YTT",
@@ -3081,26 +3114,26 @@
                 "YTT302",
                 "YTT303"
             ],
             "type": "string"
         },
         "SerializationFormat": {
             "enum": [
-                "text",
+                "azure",
                 "concise",
                 "full",
+                "github",
+                "gitlab",
+                "grouped",
                 "json",
                 "json-lines",
                 "junit",
-                "grouped",
-                "github",
-                "gitlab",
                 "pylint",
-                "azure",
-                "sarif"
+                "sarif",
+                "text"
             ],
             "type": "string"
         },
         "Strictness": {
             "oneOf": [
                 {
                     "description": "Ban imports that extend into the parent module or beyond.",
@@ -3113,17 +3146,14 @@
                     "description": "Ban all relative imports.",
                     "enum": [
                         "all"
                     ],
                     "type": "string"
                 }
             ]
-        },
-        "Version": {
-            "type": "string"
         }
     },
     "properties": {
         "allowed-confusables": {
             "deprecated": true,
             "description": "A list of allowed \"confusable\" Unicode characters to ignore when enforcing `RUF001`, `RUF002`, and `RUF003`.",
             "items": {
@@ -3145,24 +3175,24 @@
                 "array",
                 "null"
             ]
         },
         "cache-dir": {
             "description": "A path to the cache directory.\n\nBy default, Ruff stores cache results in a `.ruff_cache` directory in the current project root.\n\nHowever, Ruff will also respect the `RUFF_CACHE_DIR` environment variable, which takes precedence over that default.\n\nThis setting will override even the `RUFF_CACHE_DIR` environment variable, if set.",
             "type": [
-                "string",
-                "null"
+                "null",
+                "string"
             ]
         },
         "dummy-variable-rgx": {
             "deprecated": true,
             "description": "A regular expression used to identify \"dummy\" variables, or those which should be ignored when enforcing (e.g.) unused-variable rules. The default expression matches `_`, `__`, and `_var`, but not `_var_`.",
             "type": [
-                "string",
-                "null"
+                "null",
+                "string"
             ]
         },
         "exclude": {
             "description": "A list of file patterns to exclude from formatting and linting.\n\nExclusions are based on globs, and can be either:\n\n- Single-path patterns, like `.mypy_cache` (to exclude any directory named `.mypy_cache` in the tree), `foo.py` (to exclude any file named `foo.py`), or `foo_*.py` (to exclude any file matching `foo_*.py` ). - Relative patterns, like `directory/foo.py` (to exclude that specific file) or `directory/*.py` (to exclude any Python files in `directory`). Note that these paths are relative to the project root (e.g., the directory containing your `pyproject.toml`).\n\nFor more information on the glob syntax, refer to the [`globset` documentation](https://docs.rs/globset/latest/globset/#syntax).\n\nNote that you'll typically want to use [`extend-exclude`](#extend-exclude) to modify the excluded paths.",
             "items": {
                 "type": "string"
             },
@@ -3178,16 +3208,16 @@
                 "boolean",
                 "null"
             ]
         },
         "extend": {
             "description": "A path to a local `pyproject.toml` file to merge into this configuration. User home directory and environment variables will be expanded.\n\nTo resolve the current `pyproject.toml` file, Ruff will first resolve this base configuration file, then merge in any properties defined in the current configuration file.",
             "type": [
-                "string",
-                "null"
+                "null",
+                "string"
             ]
         },
         "extend-exclude": {
             "description": "A list of file patterns to omit from formatting and linting, in addition to those specified by `exclude`.\n\nExclusions are based on globs, and can be either:\n\n- Single-path patterns, like `.mypy_cache` (to exclude any directory named `.mypy_cache` in the tree), `foo.py` (to exclude any file named `foo.py`), or `foo_*.py` (to exclude any file matching `foo_*.py` ). - Relative patterns, like `directory/foo.py` (to exclude that specific file) or `directory/*.py` (to exclude any Python files in `directory`). Note that these paths are relative to the project root (e.g., the directory containing your `pyproject.toml`).\n\nFor more information on the glob syntax, refer to the [`globset` documentation](https://docs.rs/globset/latest/globset/#syntax).",
             "items": {
                 "type": "string"
             },
@@ -3234,16 +3264,16 @@
                     "$ref": "#/definitions/RuleSelector"
                 },
                 "type": "array"
             },
             "deprecated": true,
             "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, in addition to any rules excluded by `per-file-ignores`.",
             "type": [
-                "object",
-                "null"
+                "null",
+                "object"
             ]
         },
         "extend-safe-fixes": {
             "deprecated": true,
             "description": "A list of rule codes or prefixes for which unsafe fixes should be considered safe.",
             "items": {
                 "$ref": "#/definitions/RuleSelector"
@@ -3541,15 +3571,15 @@
             "type": [
                 "array",
                 "null"
             ]
         },
         "ignore-init-module-imports": {
             "deprecated": true,
-            "description": "Avoid automatically removing unused imports in `__init__.py` files. Such imports will still be flagged, but with a dedicated message suggesting that the import is either added to the module's `__all__` symbol, or re-exported with a redundant alias (e.g., `import os as os`).",
+            "description": "Avoid automatically removing unused imports in `__init__.py` files. Such imports will still be flagged, but with a dedicated message suggesting that the import is either added to the module's `__all__` symbol, or re-exported with a redundant alias (e.g., `import os as os`).\n\nThis option is enabled by default, but you can opt-in to removal of imports via an unsafe fix.",
             "type": [
                 "boolean",
                 "null"
             ]
         },
         "include": {
             "description": "A list of file patterns to include when linting.\n\nInclusion are based on globs, and should be single-path patterns, like `*.pyw`, to include any file with the `.pyw` extension. `pyproject.toml` is included here not for configuration but because we lint whether e.g. the `[project]` matches the schema.\n\nFor more information on the glob syntax, refer to the [`globset` documentation](https://docs.rs/globset/latest/globset/#syntax).",
@@ -3667,16 +3697,16 @@
                     "$ref": "#/definitions/RuleSelector"
                 },
                 "type": "array"
             },
             "deprecated": true,
             "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, when considering any matching files.",
             "type": [
-                "object",
-                "null"
+                "null",
+                "object"
             ]
         },
         "preview": {
             "description": "Whether to enable preview mode. When preview mode is enabled, Ruff will use unstable rules, fixes, and formatting.",
             "type": [
                 "boolean",
                 "null"
@@ -3741,21 +3771,21 @@
             ],
             "deprecated": true,
             "description": "Options for the `pyupgrade` plugin."
         },
         "required-version": {
             "anyOf": [
                 {
-                    "$ref": "#/definitions/Version"
+                    "$ref": "#/definitions/RequiredVersion"
                 },
                 {
                     "type": "null"
                 }
             ],
-            "description": "Require a specific version of Ruff to be running (useful for unifying results across many environments, e.g., with a `pyproject.toml` file)."
+            "description": "Enforce a requirement on the version of Ruff, to enforce at runtime. If the version of Ruff does not meet the requirement, Ruff will exit with an error.\n\nUseful for unifying results across many environments, e.g., with a `pyproject.toml` file.\n\nAccepts a PEP 440 specifier, like `==0.3.1` or `>=0.3.1`."
         },
         "respect-gitignore": {
             "description": "Whether to automatically exclude files that are ignored by `.ignore`, `.gitignore`, `.git/info/exclude`, and global `gitignore` files. Enabled by default.",
             "type": [
                 "boolean",
                 "null"
             ]
```

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/scikit-build.schema.json` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/scikit-build.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/setuptools.schema.json` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/setuptools.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/src/validate_pyproject_schema_store/resources/tool.json` & `validate_pyproject_schema_store-2024.4.1/src/validate_pyproject_schema_store/resources/tool.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/tests/test_package.py` & `validate_pyproject_schema_store-2024.4.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/tools/sync.py` & `validate_pyproject_schema_store-2024.4.1/tools/sync.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/.gitignore` & `validate_pyproject_schema_store-2024.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/LICENSE` & `validate_pyproject_schema_store-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/README.md` & `validate_pyproject_schema_store-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.3.25/pyproject.toml` & `validate_pyproject_schema_store-2024.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "validate-pyproject-schema-store"
-version = "2024.03.25"
+version = "2024.04.01"
 authors = [
   { name = "Henry Schreiner", email = "henryfs@princeton.edu" },
 ]
 description = "A plugin set for validate-pyproject and schema-store."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -160,15 +160,15 @@
   "YTT",         # flake8-2020
   "EXE",         # flake8-executable
   "NPY",         # NumPy specific rules
   "PD",          # pandas-vet
 ]
 ignore = [
   "PLR",    # Design related pylint codes
-#  "ISC001", # Conflicts with formatter
+  "ISC001", # Conflicts with formatter
 ]
 isort.required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.lint.per-file-ignores]
 "tests/**" = ["T20"]
 "tools/**" = ["T20"]
```

### Comparing `validate_pyproject_schema_store-2024.3.25/PKG-INFO` & `validate_pyproject_schema_store-2024.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: validate-pyproject-schema-store
-Version: 2024.3.25
+Version: 2024.4.1
 Summary: A plugin set for validate-pyproject and schema-store.
 Project-URL: Homepage, https://github.com/henryiii/validate-pyproject-schema-store
 Project-URL: Bug Tracker, https://github.com/henryiii/validate-pyproject-schema-store/issues
 Project-URL: Discussions, https://github.com/henryiii/validate-pyproject-schema-store/discussions
 Project-URL: Changelog, https://github.com/henryiii/validate-pyproject-schema-store/releases
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
```

