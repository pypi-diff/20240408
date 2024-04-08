# Comparing `tmp/prefab_cloud_python-0.9.0.tar.gz` & `tmp/prefab_cloud_python-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefab_cloud_python-0.9.0.tar", max compression
+gzip compressed data, was "prefab_cloud_python-0.9.1.tar", max compression
```

## Comparing `prefab_cloud_python-0.9.0.tar` & `prefab_cloud_python-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1054 2023-06-13 00:50:55.374694 prefab_cloud_python-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0      708 2024-01-12 22:38:49.125813 prefab_cloud_python-0.9.0/README.md
--rw-r--r--   0        0        0      117 2024-01-12 22:38:49.126947 prefab_cloud_python-0.9.0/prefab_cloud_python/__init__.py
--rw-r--r--   0        0        0     3502 2024-01-12 22:38:49.127654 prefab_cloud_python-0.9.0/prefab_cloud_python/_processors.py
--rw-r--r--   0        0        0     3909 2024-01-12 19:52:42.161292 prefab_cloud_python-0.9.0/prefab_cloud_python/client.py
--rw-r--r--   0        0        0    10495 2024-01-13 22:50:06.083509 prefab_cloud_python-0.9.0/prefab_cloud_python/config_client.py
--rw-r--r--   0        0        0     2404 2024-01-13 22:50:06.083904 prefab_cloud_python-0.9.0/prefab_cloud_python/config_loader.py
--rw-r--r--   0        0        0     5569 2024-01-12 23:07:41.790732 prefab_cloud_python-0.9.0/prefab_cloud_python/config_parser.py
--rw-r--r--   0        0        0     1723 2024-01-13 22:50:06.084105 prefab_cloud_python-0.9.0/prefab_cloud_python/config_resolver.py
--rw-r--r--   0        0        0     6220 2024-01-13 22:55:17.889451 prefab_cloud_python-0.9.0/prefab_cloud_python/config_value_unwrapper.py
--rw-r--r--   0        0        0      730 2024-01-12 20:05:46.269667 prefab_cloud_python-0.9.0/prefab_cloud_python/config_value_wrapper.py
--rw-r--r--   0        0        0     3448 2024-01-13 22:50:06.084612 prefab_cloud_python-0.9.0/prefab_cloud_python/context.py
--rw-r--r--   0        0        0      173 2023-06-24 16:32:43.359796 prefab_cloud_python-0.9.0/prefab_cloud_python/context_shape.py
--rw-r--r--   0        0        0     2023 2023-06-24 16:32:43.359874 prefab_cloud_python-0.9.0/prefab_cloud_python/context_shape_aggregator.py
--rw-r--r--   0        0        0     4026 2024-01-12 23:07:41.791553 prefab_cloud_python-0.9.0/prefab_cloud_python/criteria_evaluator.py
--rw-r--r--   0        0        0      900 2024-01-13 22:55:17.889665 prefab_cloud_python-0.9.0/prefab_cloud_python/encryption.py
--rw-r--r--   0        0        0     1344 2023-06-12 23:26:42.577722 prefab_cloud_python-0.9.0/prefab_cloud_python/feature_flag_client.py
--rw-r--r--   0        0        0     2368 2023-06-24 16:32:43.359956 prefab_cloud_python-0.9.0/prefab_cloud_python/log_path_aggregator.py
--rw-r--r--   0        0        0     2504 2024-01-12 22:38:49.129471 prefab_cloud_python-0.9.0/prefab_cloud_python/logger_client.py
--rw-r--r--   0        0        0     7110 2024-01-13 22:50:06.084893 prefab_cloud_python-0.9.0/prefab_cloud_python/options.py
--rw-r--r--   0        0        0     1612 2023-06-24 16:32:43.360281 prefab_cloud_python-0.9.0/prefab_cloud_python/read_write_lock.py
--rw-r--r--   0        0        0     1108 2024-01-12 23:07:41.791928 prefab_cloud_python-0.9.0/prefab_cloud_python/weighted_value_resolver.py
--rw-r--r--   0        0        0      964 2023-06-24 16:27:49.008894 prefab_cloud_python-0.9.0/prefab_cloud_python/yaml_parser.py
--rw-r--r--   0        0        0    25941 2024-01-12 23:07:41.792524 prefab_cloud_python-0.9.0/prefab_pb2.py
--rw-r--r--   0        0        0      159 2024-01-12 19:43:14.137966 prefab_cloud_python-0.9.0/prefab_pb2_grpc.py
--rw-r--r--   0        0        0     1060 2024-01-13 22:58:24.716888 prefab_cloud_python-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 prefab_cloud_python-0.9.0/setup.py
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 prefab_cloud_python-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-01-12 22:18:18.741328 prefab_cloud_python-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     1782 2024-02-09 00:12:36.631238 prefab_cloud_python-0.9.1/README.md
+-rw-r--r--   0        0        0      117 2024-02-12 21:28:51.365410 prefab_cloud_python-0.9.1/prefab_cloud_python/__init__.py
+-rw-r--r--   0        0        0     3502 2024-02-12 21:28:51.365542 prefab_cloud_python-0.9.1/prefab_cloud_python/_processors.py
+-rw-r--r--   0        0        0     3909 2024-02-12 21:28:51.365790 prefab_cloud_python-0.9.1/prefab_cloud_python/client.py
+-rw-r--r--   0        0        0    10495 2024-02-12 21:39:32.761071 prefab_cloud_python-0.9.1/prefab_cloud_python/config_client.py
+-rw-r--r--   0        0        0     2404 2024-02-12 21:39:32.761355 prefab_cloud_python-0.9.1/prefab_cloud_python/config_loader.py
+-rw-r--r--   0        0        0     5569 2024-02-12 21:28:51.366595 prefab_cloud_python-0.9.1/prefab_cloud_python/config_parser.py
+-rw-r--r--   0        0        0     1723 2024-02-12 21:28:51.366814 prefab_cloud_python-0.9.1/prefab_cloud_python/config_resolver.py
+-rw-r--r--   0        0        0     6220 2024-02-12 21:28:51.367207 prefab_cloud_python-0.9.1/prefab_cloud_python/config_value_unwrapper.py
+-rw-r--r--   0        0        0      730 2024-02-12 21:28:51.367720 prefab_cloud_python-0.9.1/prefab_cloud_python/config_value_wrapper.py
+-rw-r--r--   0        0        0     3448 2024-02-12 21:28:51.368050 prefab_cloud_python-0.9.1/prefab_cloud_python/context.py
+-rw-r--r--   0        0        0      173 2024-01-12 22:18:18.743335 prefab_cloud_python-0.9.1/prefab_cloud_python/context_shape.py
+-rw-r--r--   0        0        0     2023 2024-02-12 21:28:51.368361 prefab_cloud_python-0.9.1/prefab_cloud_python/context_shape_aggregator.py
+-rw-r--r--   0        0        0     4026 2024-02-12 21:28:51.368450 prefab_cloud_python-0.9.1/prefab_cloud_python/criteria_evaluator.py
+-rw-r--r--   0        0        0      900 2024-02-12 21:28:51.368756 prefab_cloud_python-0.9.1/prefab_cloud_python/encryption.py
+-rw-r--r--   0        0        0     1344 2024-02-12 21:28:51.368914 prefab_cloud_python-0.9.1/prefab_cloud_python/feature_flag_client.py
+-rw-r--r--   0        0        0     2368 2024-02-12 21:28:51.369074 prefab_cloud_python-0.9.1/prefab_cloud_python/log_path_aggregator.py
+-rw-r--r--   0        0        0     2504 2024-02-12 21:28:51.369175 prefab_cloud_python-0.9.1/prefab_cloud_python/logger_client.py
+-rw-r--r--   0        0        0     7110 2024-02-12 21:28:51.369396 prefab_cloud_python-0.9.1/prefab_cloud_python/options.py
+-rw-r--r--   0        0        0     1612 2024-02-12 21:28:51.369538 prefab_cloud_python-0.9.1/prefab_cloud_python/read_write_lock.py
+-rw-r--r--   0        0        0     1108 2024-01-16 20:27:10.501413 prefab_cloud_python-0.9.1/prefab_cloud_python/weighted_value_resolver.py
+-rw-r--r--   0        0        0      964 2024-02-12 21:28:51.369701 prefab_cloud_python-0.9.1/prefab_cloud_python/yaml_parser.py
+-rw-r--r--   0        0        0    25941 2024-01-16 20:27:10.501712 prefab_cloud_python-0.9.1/prefab_pb2.py
+-rw-r--r--   0        0        0      159 2024-02-12 21:28:51.369793 prefab_cloud_python-0.9.1/prefab_pb2_grpc.py
+-rw-r--r--   0        0        0     1060 2024-02-12 21:39:56.720829 prefab_cloud_python-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2956 1970-01-01 00:00:00.000000 prefab_cloud_python-0.9.1/PKG-INFO
```

### Comparing `prefab_cloud_python-0.9.0/LICENSE.txt` & `prefab_cloud_python-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/_processors.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/_processors.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/client.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/client.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/config_client.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/config_client.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/config_loader.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/config_loader.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/config_parser.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/config_parser.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/config_resolver.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/config_resolver.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/config_value_unwrapper.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/config_value_unwrapper.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/config_value_wrapper.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/config_value_wrapper.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/context.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/context.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/context_shape_aggregator.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/context_shape_aggregator.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/criteria_evaluator.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/criteria_evaluator.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/encryption.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/encryption.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/feature_flag_client.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/feature_flag_client.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/log_path_aggregator.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/log_path_aggregator.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/logger_client.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/logger_client.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/options.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/options.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/read_write_lock.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/weighted_value_resolver.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/weighted_value_resolver.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_cloud_python/yaml_parser.py` & `prefab_cloud_python-0.9.1/prefab_cloud_python/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/prefab_pb2.py` & `prefab_cloud_python-0.9.1/prefab_pb2.py`

 * *Files identical despite different names*

### Comparing `prefab_cloud_python-0.9.0/pyproject.toml` & `prefab_cloud_python-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prefab-cloud-python"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python client for Prefab Feature Flags, Dynamic log levels, and Config as a Service: https://www.prefab.cloud"
 license = "MIT"
 authors = ["Michael Berkowitz <michael.berkowitz@gmail.com>"]
 maintainers = ["Michael Berkowitz <michael.berkowitz@gmail.com>"]
 readme = "README.md"
 homepage = "https://www.prefab.cloud"
 repository = "https://github.com/prefab-cloud/prefab-cloud-python"
```

### Comparing `prefab_cloud_python-0.9.0/PKG-INFO` & `prefab_cloud_python-0.9.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: prefab-cloud-python
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for Prefab Feature Flags, Dynamic log levels, and Config as a Service: https://www.prefab.cloud
 Home-page: https://www.prefab.cloud
 License: MIT
 Author: Michael Berkowitz
 Author-email: michael.berkowitz@gmail.com
 Maintainer: Michael Berkowitz
 Maintainer-email: michael.berkowitz@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cryptography (>=41.0.7)
 Requires-Dist: grpcio (>=1.48.4)
 Requires-Dist: mmh3 (>=3.0.0,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: sseclient-py (>=1.7.2,<2.0.0)
 Requires-Dist: structlog (>=22.3,<23.0)
@@ -56,7 +57,45 @@
 result = client.enabled("my-first-feature-flag", context=context)
 
 print("my-first-feature-flag is:", result)
 ```
 
 See full documentation https://docs.prefab.cloud/docs/sdks/python
 
+## Development
+
+1. Ensure that `poetry` is installed: https://python-poetry.org/docs/#installation
+2. From the root of this directory, run `poetry install` to ensure dependencies are installed
+3. `poetry run python` to open a Python REPL with access to the project dependencies
+
+### Running tests
+
+To run all tests, including integration tests
+
+```bash
+poetry run pytest tests
+```
+
+To run only local tests and skip integration tests
+
+```bash
+poetry run pytest tests -k "not integration"
+```
+
+To run only one specific test file
+
+```bash
+poetry run pytest tests/name_of_test_file.py
+```
+
+### Releasing
+
+1. Run pre-commit hooks to check and fix formatting, other rule enforcement.
+   `poetry run pre-commit run --show-diff-on-failure --color=always --all-files`
+2. On a branch
+   1. Update the version in `pyproject.toml`
+   2. Update `CHANGELOG.md`
+3. Merge the branch
+4. `git tag <version> && git push --tags`
+5. `poetry release --build`
+   1. To do this you will need an [pypi.org](https://pypi.org) account, and to be added to this project (ask Michael for an invitation)
+
```

