# Comparing `tmp/reprompt-0.0.6.tar.gz` & `tmp/reprompt-0.0.6rc45.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.6rc45.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.6.tar` & `reprompt-0.0.6rc45.post1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      334 2024-04-07 00:25:03.403742 reprompt-0.0.6/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-07 00:25:03.403879 reprompt-0.0.6/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-07 00:25:03.404063 reprompt-0.0.6/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-07 00:25:03.404188 reprompt-0.0.6/.github/template-sync.yml
--rw-r--r--   0        0        0      472 2024-04-07 04:50:18.529595 reprompt-0.0.6/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-07 04:50:18.529840 reprompt-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-07 00:25:03.404614 reprompt-0.0.6/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      368 2024-04-07 01:39:00.868788 reprompt-0.0.6/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-07 00:25:03.404977 reprompt-0.0.6/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-07 00:25:03.405111 reprompt-0.0.6/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-07 01:12:32.734093 reprompt-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-07 01:11:22.577276 reprompt-0.0.6/.pypirc
--rw-r--r--   0        0        0      459 2024-04-07 00:25:03.405530 reprompt-0.0.6/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-07 00:25:03.405655 reprompt-0.0.6/.vscode/settings.json
--rw-r--r--   0        0        0     1127 2024-04-07 04:04:06.674601 reprompt-0.0.6/LICENSE
--rw-r--r--   0        0        0    15834 2024-04-07 01:48:53.925616 reprompt-0.0.6/README.md
--rw-r--r--   0        0        0      634 2024-04-07 00:25:03.406066 reprompt-0.0.6/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-07 00:25:03.406173 reprompt-0.0.6/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-07 00:25:03.406277 reprompt-0.0.6/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-07 00:25:03.406376 reprompt-0.0.6/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-07 00:25:03.406480 reprompt-0.0.6/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-07 00:25:03.406590 reprompt-0.0.6/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-07 00:25:03.406687 reprompt-0.0.6/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-07 00:25:03.406789 reprompt-0.0.6/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-07 00:25:03.406919 reprompt-0.0.6/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-07 00:25:03.407022 reprompt-0.0.6/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-07 00:25:03.407129 reprompt-0.0.6/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-07 00:25:03.407228 reprompt-0.0.6/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-07 00:25:03.407318 reprompt-0.0.6/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-07 00:25:03.407408 reprompt-0.0.6/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-07 00:25:03.407512 reprompt-0.0.6/docs/workflows.md
--rw-r--r--   0        0        0     6649 2024-04-07 04:50:41.217958 reprompt-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-07 00:25:03.407795 reprompt-0.0.6/src/README.md
--rw-r--r--   0        0        0     1446 2024-04-07 20:32:01.320898 reprompt-0.0.6/src/reprompt/__init__.py
--rw-r--r--   0        0        0      162 2024-04-07 04:05:08.840231 reprompt-0.0.6/src/reprompt/config.py
--rw-r--r--   0        0        0     2143 2024-04-07 20:32:01.320963 reprompt-0.0.6/src/reprompt/custom_httpx.py
--rw-r--r--   0        0        0     1719 2024-04-07 04:05:08.840801 reprompt-0.0.6/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-07 00:25:03.408249 reprompt-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0      511 2024-04-07 04:04:06.675966 reprompt-0.0.6/tests/openai_example_script.py
--rw-r--r--   0        0        0      283 2024-04-07 20:32:01.321008 reprompt-0.0.6/tests/test_init.py
--rw-r--r--   0        0        0     1673 2024-04-07 20:31:01.502000 reprompt-0.0.6/tests/test_openai_tracing.py
--rw-r--r--   0        0        0    17735 1970-01-01 00:00:00.000000 reprompt-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      472 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      368 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1127 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/LICENSE
+-rw-r--r--   0        0        0    15834 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/README.md
+-rw-r--r--   0        0        0      634 2024-04-07 20:33:23.705697 reprompt-0.0.6rc45.post1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6649 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/src/README.md
+-rw-r--r--   0        0        0     1459 2024-04-07 20:33:37.437677 reprompt-0.0.6rc45.post1/src/reprompt/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/src/reprompt/config.py
+-rw-r--r--   0        0        0     2143 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/src/reprompt/custom_httpx.py
+-rw-r--r--   0        0        0     1719 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/tests/conftest.py
+-rw-r--r--   0        0        0      511 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/tests/openai_example_script.py
+-rw-r--r--   0        0        0      283 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/tests/test_init.py
+-rw-r--r--   0        0        0     1673 2024-04-07 20:33:23.709697 reprompt-0.0.6rc45.post1/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0    17745 1970-01-01 00:00:00.000000 reprompt-0.0.6rc45.post1/PKG-INFO
```

### Comparing `reprompt-0.0.6/.devcontainer/devcontainer.json` & `reprompt-0.0.6rc45.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.6rc45.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/.gitignore` & `reprompt-0.0.6rc45.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/.pre-commit-config.yaml` & `reprompt-0.0.6rc45.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/.vscode/settings.json` & `reprompt-0.0.6rc45.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/LICENSE` & `reprompt-0.0.6rc45.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/README.md` & `reprompt-0.0.6rc45.post1/README.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/docs/Makefile` & `reprompt-0.0.6rc45.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/docs/conf.py` & `reprompt-0.0.6rc45.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/docs/make.bat` & `reprompt-0.0.6rc45.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/docs/pylint.md` & `reprompt-0.0.6rc45.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/pyproject.toml` & `reprompt-0.0.6rc45.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/src/reprompt/__init__.py` & `reprompt-0.0.6rc45.post1/src/reprompt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .custom_httpx import setup_monkey_patch
 from .tracing import FunctionTrace
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 # IMPORTANT: setting version for Reprompt package
-__version__ = "0.0.6"
+__version__ = "0.0.6""-rc45-post1"
 # IMPORTANT: All the functions we want to expose publicly from the reprompt module
 __all__ = ["FunctionTrace", "init", "write_traces_to_file"]
 
 
 def init(api_base_url: str = None, api_key: str = None, autocapture: bool = True):
     """
     Initializes the reprompt SDK with the given API base URL and API key.
```

### Comparing `reprompt-0.0.6/src/reprompt/custom_httpx.py` & `reprompt-0.0.6rc45.post1/src/reprompt/custom_httpx.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/src/reprompt/tracing.py` & `reprompt-0.0.6rc45.post1/src/reprompt/tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/tests/conftest.py` & `reprompt-0.0.6rc45.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/tests/test_openai_tracing.py` & `reprompt-0.0.6rc45.post1/tests/test_openai_tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.6/PKG-INFO` & `reprompt-0.0.6rc45.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprompt
-Version: 0.0.6
+Version: 0.0.6rc45.post1
 Summary: Reprompt
 Author-email: Lukas Martinelli <me@lukasmartinelli.ch>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

