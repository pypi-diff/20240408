# Comparing `tmp/stringx-0.4.0.tar.gz` & `tmp/stringx-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringx-0.4.0.tar", last modified: Fri Apr  5 12:49:33 2024, max compression
+gzip compressed data, was "stringx-0.5.0.tar", last modified: Sun Apr  7 23:16:49 2024, max compression
```

## Comparing `stringx-0.4.0.tar` & `stringx-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-03-18 00:39:05.484210 stringx-0.4.0/LICENSE
--rw-r--r--   0        0        0     3218 2024-04-04 00:16:00.373070 stringx-0.4.0/README.md
--rw-r--r--   0        0        0     1783 2024-04-05 12:49:33.259956 stringx-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2006 2024-04-05 12:44:27.699955 stringx-0.4.0/src/stringx/__init__.py
--rw-r--r--   0        0        0     2923 2024-04-05 12:48:49.719956 stringx-0.4.0/src/stringx/client.py
--rw-r--r--   0        0        0        0 2024-04-03 22:27:23.943070 stringx-0.4.0/src/stringx/py.typed
--rw-r--r--   0        0        0        0 2024-03-18 00:39:05.504210 stringx-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      163 2024-04-04 00:02:15.343066 stringx-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     5002 2024-04-04 23:44:22.050896 stringx-0.4.0/tests/test_client.py
--rw-r--r--   0        0        0     1353 2024-04-05 12:40:11.419953 stringx-0.4.0/tests/test_stringx.py
--rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 stringx-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-31 00:59:04.811433 stringx-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3218 2024-04-06 18:33:50.727021 stringx-0.5.0/README.md
+-rw-r--r--   0        0        0     1956 2024-04-07 23:16:49.965364 stringx-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2454 2024-04-07 09:35:43.938850 stringx-0.5.0/src/stringx/__init__.py
+-rw-r--r--   0        0        0     3531 2024-04-07 23:16:04.948859 stringx-0.5.0/src/stringx/client.py
+-rw-r--r--   0        0        0        0 2024-04-06 18:33:50.731021 stringx-0.5.0/src/stringx/py.typed
+-rw-r--r--   0        0        0        0 2024-03-31 00:59:04.811433 stringx-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-06 18:33:50.731021 stringx-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     5745 2024-04-06 19:39:23.926995 stringx-0.5.0/tests/test_client.py
+-rw-r--r--   0        0        0     1535 2024-04-06 19:40:15.725374 stringx-0.5.0/tests/test_stringx.py
+-rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 stringx-0.5.0/PKG-INFO
```

### Comparing `stringx-0.4.0/LICENSE` & `stringx-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stringx-0.4.0/README.md` & `stringx-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     identity="me@example.com"
 ) as client:
     ...
 ```
 
 Regardless of how you choose to do it, STRINGX always appends its own information to your identity.
 
-Using one of the clients instantiated above as example, the `caller_identity` parameters passed to the STRING API would be `my_project_name (python-stringx/0.3.0)`.
+Using one of the clients instantiated above as example, the `caller_identity` parameters passed to the STRING API would be `my_project_name (python-stringx/x.y.z)`.
 
 ## Documentation
 
 🚧🚧🚧
 
 Refer to the official [API documentation](https://string-db.org/help/api) for details.
```

### Comparing `stringx-0.4.0/pyproject.toml` & `stringx-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 description = "STRING DB API Client"
 authors = [
     { name = "Hugo Cachitas", email = "hcachitas@gmail.com" },
 ]
 dependencies = [
     "httpx>=0.27.0",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 readme = "README.md"
 keywords = [
     "string",
     "api",
     "client",
     "httpx",
     "sib",
@@ -34,24 +34,22 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Science/Research",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Typing :: Typed",
 ]
 dynamic = []
-version = "0.4.0"
+version = "0.5.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pypi.org/project/stringx"
 Repository = "https://github.com/cachitas/stringx"
@@ -59,24 +57,24 @@
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=8.1.1",
     "pytest-httpx>=0.30.0",
     "ruff>=0.3.5",
     "mypy>=1.9.0",
-]
-examples = [
-    "pandas>=2.2.1",
-    "ipykernel>=6.29.4",
+    "tox-pdm>=0.7.2",
 ]
 
 [tool.pdm.version]
 source = "file"
 path = "src/stringx/client.py"
 
+[tool.pdm.scripts]
+test = "pytest -v tests/"
+
 [tool.ruff]
 extend-include = [
     "*.ipynb",
 ]
 
 [tool.ruff.lint]
 select = [
@@ -84,7 +82,20 @@
     "C4",
     "E",
     "F",
     "I",
     "W",
     "UP",
 ]
+
+[tool.mypy]
+mypy_path = "$MYPY_CONFIG_FILE_DIR/src"
+strict = true
+warn_return_any = true
+warn_unused_configs = true
+
+[tool.pytest.ini_options]
+xfail_strict = true
+markers = [
+    "network: tests that need network",
+    "integration: integration tests",
+]
```

### Comparing `stringx-0.4.0/src/stringx/__init__.py` & `stringx-0.5.0/src/stringx/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,10 +75,28 @@
         return (
             client.homology(identifiers=identifiers, species=species)
             .raise_for_status()
             .json()
         )
 
 
+def enrichment(
+    identifiers: list[str],
+    species: int,
+    *,
+    background_identifiers: list[str] | None = None,
+) -> typing.Any:
+    with Client(identity=identity) as client:
+        return (
+            client.enrichment(
+                identifiers=identifiers,
+                species=species,
+                background_identifiers=background_identifiers,
+            )
+            .raise_for_status()
+            .json()
+        )
+
+
 def version():
     with Client(identity=identity) as client:
         return client.version()
```

### Comparing `stringx-0.4.0/src/stringx/client.py` & `stringx-0.5.0/src/stringx/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 import httpx
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 logger = logging.getLogger("stringx")
 
 
 class Client(httpx.Client):
     def __init__(self, identity: str, base_url: str = "https://string-db.org") -> None:
         if not identity:
@@ -97,11 +97,32 @@
         params = httpx.QueryParams(
             identifiers="\r".join(identifiers),
             species=species,
         )
 
         return self.post(url, params=params)
 
+    def enrichment(
+        self,
+        identifiers: list[str],
+        species: int,
+        *,
+        background_identifiers: list[str] | None = None,
+        format: str | None = None,
+    ) -> httpx.Response:
+        url = f"api/{format or self.format}/enrichment"
+
+        params = httpx.QueryParams(
+            identifiers="\r".join(identifiers),
+            species=species,
+        )
+        if background_identifiers:
+            params = params.add(
+                "background_string_identifiers", "\r".join(background_identifiers)
+            )
+
+        return self.post(url, params=params)
+
     def version(self) -> str:
         request = self.build_request("GET", "api/json/version")
         request.url = request.url.copy_remove_param("caller_identity")
         return self.send(request).json()
```

### Comparing `stringx-0.4.0/tests/test_client.py` & `stringx-0.5.0/tests/test_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -156,14 +156,40 @@
             },
         ),
     )
 
     test_client.homology(identifiers, species, format=format)
 
 
+@pytest.mark.parametrize("format", ["tsv", "tsv-no-header", "json", "xml"])
+def test_enrichment(httpx_mock, test_client, format):
+    identifiers = ["id1"]
+    background_identifiers = ["id2"]
+    species = 1234
+
+    httpx_mock.add_response(
+        url=httpx.URL(
+            f"https://string-db.org/api/{format}/enrichment",
+            params={
+                "identifiers": identifiers,
+                "background_string_identifiers": background_identifiers,
+                "species": species,
+                "caller_identity": test_client.identity,
+            },
+        ),
+    )
+
+    test_client.enrichment(
+        identifiers,
+        species,
+        background_identifiers=background_identifiers,
+        format=format,
+    )
+
+
 def test_version(httpx_mock, test_client):
     httpx_mock.add_response(
         url=httpx.URL("https://string-db.org/api/json/version"),
         method="GET",
         json=[
             {
                 "string_version": "12.0",
```

### Comparing `stringx-0.4.0/tests/test_stringx.py` & `stringx-0.5.0/tests/test_stringx.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,7 +45,13 @@
     stringx.interaction_partners(["id1"], 1234)
     stringx.interaction_partners(["id1"], 1234, limit=10)
 
 
 def test_homology(httpx_mock):
     httpx_mock.add_response(json=True)
     stringx.homology(["id1"], 1234)
+
+
+def test_enrichment(httpx_mock):
+    httpx_mock.add_response(json=True)
+    stringx.enrichment(["id1"], 1234)
+    stringx.enrichment(["id1"], 1234, background_identifiers=["id2"])
```

### Comparing `stringx-0.4.0/PKG-INFO` & `stringx-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: stringx
-Version: 0.4.0
+Version: 0.5.0
 Summary: STRING DB API Client
 Keywords: string api client httpx sib cpr embl biodata elixir protein gene interaction
 Author-Email: Hugo Cachitas <hcachitas@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://pypi.org/project/stringx
 Project-URL: Repository, https://github.com/cachitas/stringx
 Project-URL: Issues, https://github.com/cachitas/stringx/issues
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Requires-Dist: httpx>=0.27.0
 Description-Content-Type: text/markdown
 
 # STRINGX
 
 [![PyPI Version](https://img.shields.io/pypi/v/stringx?label=PyPI&logo=pypi&logoColor=white&color=006dad)](https://pypi.org/project/stringx/)
 [![Python Version](https://img.shields.io/pypi/pyversions/stringx?label=Python&logo=python&logoColor=white&color=006dad)](https://pypi.org/project/stringx/)
@@ -95,15 +93,15 @@
     identity="me@example.com"
 ) as client:
     ...
 ```
 
 Regardless of how you choose to do it, STRINGX always appends its own information to your identity.
 
-Using one of the clients instantiated above as example, the `caller_identity` parameters passed to the STRING API would be `my_project_name (python-stringx/0.3.0)`.
+Using one of the clients instantiated above as example, the `caller_identity` parameters passed to the STRING API would be `my_project_name (python-stringx/x.y.z)`.
 
 ## Documentation
 
 🚧🚧🚧
 
 Refer to the official [API documentation](https://string-db.org/help/api) for details.
```

