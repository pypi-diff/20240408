# Comparing `tmp/pdm_polylith_bricks-0.1.2.tar.gz` & `tmp/pdm_polylith_bricks-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_polylith_bricks-0.1.2.tar", max compression
+gzip compressed data, was "pdm_polylith_bricks-1.0.0.tar", max compression
```

## Comparing `pdm_polylith_bricks-0.1.2.tar` & `pdm_polylith_bricks-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2825 2024-01-23 21:16:34.626643 pdm_polylith_bricks-0.1.2/README.md
--rw-r--r--   0        0        0      565 2024-02-05 13:16:14.963895 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/configuration/__init__.py
--rw-r--r--   0        0        0     2191 2024-02-05 13:16:14.964742 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/configuration/core.py
--rw-r--r--   0        0        0      249 2024-02-05 13:16:14.966722 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/parsing/__init__.py
--rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/parsing/core.py
--rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/parsing/rewrite.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623045 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/pdm/__init__.py
--rw-r--r--   0        0        0     1147 2024-02-05 13:16:14.969174 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/pdm/core.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623415 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/pdm/hooks/__init__.py
--rw-r--r--   0        0        0      637 2024-02-05 13:16:14.969648 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py
--rw-r--r--   0        0        0     1019 2024-02-05 13:16:14.970342 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.620904 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/pdm_project_hooks/__init__.py
--rw-r--r--   0        0        0      259 2024-02-05 13:16:14.966503 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/pdm_project_hooks/core.py
--rw-r--r--   0        0        0      539 2024-02-05 13:16:14.967712 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/repo/__init__.py
--rw-r--r--   0        0        0      859 2024-02-05 13:16:14.968554 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/repo/repo.py
--rw-r--r--   0        0        0      406 2024-02-05 13:16:14.965004 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/toml/__init__.py
--rw-r--r--   0        0        0     2170 2024-02-05 13:16:14.966148 pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/toml/core.py
--rw-r--r--   0        0        0      618 2024-02-05 13:16:14.963345 pdm_polylith_bricks-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3507 1970-01-01 00:00:00.000000 pdm_polylith_bricks-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2825 2024-01-23 21:16:34.626643 pdm_polylith_bricks-1.0.0/README.md
+-rw-r--r--   0        0        0      565 2024-04-08 06:17:20.390842 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/configuration/__init__.py
+-rw-r--r--   0        0        0     2191 2024-04-08 06:17:20.391693 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/configuration/core.py
+-rw-r--r--   0        0        0      249 2024-04-08 06:17:20.393823 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/parsing/__init__.py
+-rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/parsing/core.py
+-rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/parsing/rewrite.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623045 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/__init__.py
+-rw-r--r--   0        0        0     1147 2024-04-08 06:17:20.396272 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/core.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623415 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/hooks/__init__.py
+-rw-r--r--   0        0        0      637 2024-04-08 06:17:20.396787 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py
+-rw-r--r--   0        0        0     1019 2024-04-08 06:17:20.398343 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.620904 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm_project_hooks/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-08 06:17:20.393602 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm_project_hooks/core.py
+-rw-r--r--   0        0        0      539 2024-04-08 06:17:20.394816 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-08 06:17:20.395648 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/repo.py
+-rw-r--r--   0        0        0      464 2024-04-08 06:17:20.391973 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     2917 2024-04-08 06:17:20.393228 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/toml/core.py
+-rw-r--r--   0        0        0      618 2024-04-08 06:17:20.390284 pdm_polylith_bricks-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3507 1970-01-01 00:00:00.000000 pdm_polylith_bricks-1.0.0/PKG-INFO
```

### Comparing `pdm_polylith_bricks-0.1.2/README.md` & `pdm_polylith_bricks-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/configuration/__init__.py` & `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/configuration/core.py` & `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/configuration/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/parsing/core.py` & `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/parsing/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/parsing/rewrite.py` & `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/pdm/core.py` & `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py` & `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py` & `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/repo/__init__.py` & `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/repo/get.py` & `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/repo/repo.py` & `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-0.1.2/pdm_polylith_bricks/polylith/toml/core.py` & `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/toml/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from functools import reduce
 from pathlib import Path
 from typing import List, Union
 import tomlkit
 from pdm_polylith_bricks.polylith import repo
 
 def transform_to_package(namespace: str, include: str) -> dict:
     path, _separator, brick = str.partition(include, f'/{namespace}/')
@@ -35,19 +36,39 @@
     return [transform_to_package(namespace, key) for key in includes.keys()]
 
 def get_project_name(data) -> str:
     if repo.is_pep_621_ready(data):
         return data['project']['name']
     return data['tool']['poetry']['name']
 
-def get_project_dependencies(data) -> dict:
-    if repo.is_poetry(data):
-        deps = data['tool']['poetry'].get('dependencies', [])
-        items = set(deps.keys())
+def parse_pep_621_dependency(dep: str) -> dict:
+    parts = re.split('[\\^~=!<>]', dep)
+    name, *_ = parts if parts else ['']
+    version = str.replace(dep, name, '')
+    return {name: version} if name else {}
+
+def parse_poetry_dependency(acc: dict, kv: tuple) -> dict:
+    k, v = kv
+    if isinstance(v, dict):
+        extras = sorted(v.get('extras', []))
+        version = v.get('version', '')
+        name = k + str.replace(f'{extras}', "'", '') if extras else k
+        parsed = {name: version}
     else:
-        deps = data['project'].get('dependencies', [])
-        items = {re.split('[\\^~=!<>]', dep)[0] for dep in deps}
+        parsed = {k: v}
+    return {**acc, **parsed}
+
+def parse_project_dependencies(data) -> dict:
+    if repo.is_poetry(data):
+        deps = data['tool']['poetry'].get('dependencies', {})
+        res: dict = reduce(parse_poetry_dependency, deps.items(), {})
+        return res
+    deps = data['project'].get('dependencies', [])
+    return {k: v for dep in deps for k, v in parse_pep_621_dependency(dep).items()}
+
+def get_project_dependencies(data) -> dict:
+    items = parse_project_dependencies(data)
     return {'items': items, 'source': repo.default_toml}
 
 def read_toml_document(path: Path) -> tomlkit.TOMLDocument:
     with path.open(encoding='utf-8', errors='ignore') as f:
         return tomlkit.loads(f.read())
```

### Comparing `pdm_polylith_bricks-0.1.2/pyproject.toml` & `pdm_polylith_bricks-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdm-polylith-bricks"
-version = "0.1.2"
+version = "1.0.0"
 description = "a PDM build hook for Polylith"
 authors = ["David Vujic"]
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 license = "MIT"
 readme = "README.md"
```

### Comparing `pdm_polylith_bricks-0.1.2/PKG-INFO` & `pdm_polylith_bricks-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-polylith-bricks
-Version: 0.1.2
+Version: 1.0.0
 Summary: a PDM build hook for Polylith
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

