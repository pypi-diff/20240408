# Comparing `tmp/reprompt-0.0.6rc47.post1.tar.gz` & `tmp/reprompt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.6rc47.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.6rc47.post1.tar` & `reprompt-0.0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      334 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      472 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      368 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.pypirc
--rw-r--r--   0        0        0      459 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1127 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/LICENSE
--rw-r--r--   0        0        0    15834 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/README.md
--rw-r--r--   0        0        0      634 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-08 02:07:42.220345 reprompt-0.0.6rc47.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/docs/workflows.md
--rw-r--r--   0        0        0     6649 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/src/README.md
--rw-r--r--   0        0        0     1491 2024-04-08 02:07:56.136521 reprompt-0.0.6rc47.post1/src/reprompt/__init__.py
--rw-r--r--   0        0        0      859 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/src/reprompt/background_task_manager.py
--rw-r--r--   0        0        0      162 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/src/reprompt/config.py
--rw-r--r--   0        0        0     2119 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/src/reprompt/custom_httpx.py
--rw-r--r--   0        0        0     2338 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/tests/conftest.py
--rw-r--r--   0        0        0      511 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/tests/openai_example_script.py
--rw-r--r--   0        0        0      283 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/tests/test_init.py
--rw-r--r--   0        0        0     1673 2024-04-08 02:07:42.224345 reprompt-0.0.6rc47.post1/tests/test_openai_tracing.py
--rw-r--r--   0        0        0    17745 1970-01-01 00:00:00.000000 reprompt-0.0.6rc47.post1/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-04 23:08:33.473524 reprompt-0.0.7/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-04 23:08:33.473643 reprompt-0.0.7/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-04 23:08:33.473790 reprompt-0.0.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-04 23:08:33.473883 reprompt-0.0.7/.github/template-sync.yml
+-rw-r--r--   0        0        0      472 2024-04-07 21:52:20.071061 reprompt-0.0.7/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-07 21:52:20.071267 reprompt-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-04 23:08:33.474206 reprompt-0.0.7/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      368 2024-04-04 23:08:33.474380 reprompt-0.0.7/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-04 23:08:33.474462 reprompt-0.0.7/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-04 23:08:33.474551 reprompt-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-04 23:08:33.474640 reprompt-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-04 23:08:33.474722 reprompt-0.0.7/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-04 23:08:33.474853 reprompt-0.0.7/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-04 23:08:33.474937 reprompt-0.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0     1127 2024-04-07 21:52:20.071438 reprompt-0.0.7/LICENSE
+-rw-r--r--   0        0        0    15834 2024-04-07 21:52:20.071934 reprompt-0.0.7/README.md
+-rw-r--r--   0        0        0      634 2024-04-04 23:08:33.475348 reprompt-0.0.7/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-04 23:08:33.475439 reprompt-0.0.7/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-04 23:08:33.475525 reprompt-0.0.7/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-04 23:08:33.475604 reprompt-0.0.7/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-04 23:08:33.475685 reprompt-0.0.7/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-04 23:08:33.475772 reprompt-0.0.7/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-04 23:08:33.475852 reprompt-0.0.7/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-04 23:08:33.475929 reprompt-0.0.7/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-04 23:08:33.476081 reprompt-0.0.7/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-04 23:08:33.476163 reprompt-0.0.7/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-04 23:08:33.476254 reprompt-0.0.7/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-04 23:08:33.476339 reprompt-0.0.7/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-04 23:08:33.476409 reprompt-0.0.7/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-04 23:08:33.476479 reprompt-0.0.7/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-04 23:08:33.476563 reprompt-0.0.7/docs/workflows.md
+-rw-r--r--   0        0        0     6649 2024-04-07 21:52:20.072547 reprompt-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-04 23:08:33.476873 reprompt-0.0.7/src/README.md
+-rw-r--r--   0        0        0     1478 2024-04-08 16:17:45.140585 reprompt-0.0.7/src/reprompt/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-07 23:40:24.407699 reprompt-0.0.7/src/reprompt/background_task_manager.py
+-rw-r--r--   0        0        0      162 2024-04-07 21:52:20.072817 reprompt-0.0.7/src/reprompt/config.py
+-rw-r--r--   0        0        0     2119 2024-04-07 23:19:14.207089 reprompt-0.0.7/src/reprompt/custom_httpx.py
+-rw-r--r--   0        0        0     2338 2024-04-07 23:50:31.283965 reprompt-0.0.7/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-04 23:08:33.477233 reprompt-0.0.7/tests/conftest.py
+-rw-r--r--   0        0        0      511 2024-04-07 21:52:20.073113 reprompt-0.0.7/tests/openai_example_script.py
+-rw-r--r--   0        0        0      283 2024-04-07 21:52:20.073222 reprompt-0.0.7/tests/test_init.py
+-rw-r--r--   0        0        0     1673 2024-04-07 21:52:20.073331 reprompt-0.0.7/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0    17735 1970-01-01 00:00:00.000000 reprompt-0.0.7/PKG-INFO
```

### Comparing `reprompt-0.0.6rc47.post1/.devcontainer/devcontainer.json` & `reprompt-0.0.7/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.7/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/.gitignore` & `reprompt-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/.pre-commit-config.yaml` & `reprompt-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/.vscode/settings.json` & `reprompt-0.0.7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/LICENSE` & `reprompt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/README.md` & `reprompt-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/docs/Makefile` & `reprompt-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/docs/conf.py` & `reprompt-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/docs/make.bat` & `reprompt-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/docs/pylint.md` & `reprompt-0.0.7/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/pyproject.toml` & `reprompt-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/src/reprompt/__init__.py` & `reprompt-0.0.7/src/reprompt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .custom_httpx import setup_monkey_patch
 from .tracing import FunctionTrace, write_traces
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 # IMPORTANT: setting version for Reprompt package
-__version__ = "0.0.6""-rc47-post1"
+__version__ = "0.0.7"
 # IMPORTANT: All the functions we want to expose publicly from the reprompt module
 __all__ = ["init", "FunctionTrace", "write_traces"]
 
 
 def init(api_base_url: str = None, api_key: str = None, autocapture: bool = False):
     """
     Initializes the reprompt SDK with the given API base URL and API key.
```

### Comparing `reprompt-0.0.6rc47.post1/src/reprompt/background_task_manager.py` & `reprompt-0.0.7/src/reprompt/background_task_manager.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/src/reprompt/custom_httpx.py` & `reprompt-0.0.7/src/reprompt/custom_httpx.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/src/reprompt/tracing.py` & `reprompt-0.0.7/src/reprompt/tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/tests/conftest.py` & `reprompt-0.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/tests/test_openai_tracing.py` & `reprompt-0.0.7/tests/test_openai_tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6rc47.post1/PKG-INFO` & `reprompt-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprompt
-Version: 0.0.6rc47.post1
+Version: 0.0.7
 Summary: Reprompt
 Author-email: Lukas Martinelli <me@lukasmartinelli.ch>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

