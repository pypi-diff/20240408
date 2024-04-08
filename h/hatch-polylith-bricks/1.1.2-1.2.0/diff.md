# Comparing `tmp/hatch_polylith_bricks-1.1.2.tar.gz` & `tmp/hatch_polylith_bricks-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatch_polylith_bricks-1.1.2.tar", max compression
+gzip compressed data, was "hatch_polylith_bricks-1.2.0.tar", max compression
```

## Comparing `hatch_polylith_bricks-1.1.2.tar` & `hatch_polylith_bricks-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3140 2024-01-23 22:26:31.652064 hatch_polylith_bricks-1.1.2/README.md
--rw-r--r--   0        0        0       74 2024-02-04 10:09:00.322938 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/hatch/__init__.py
--rw-r--r--   0        0        0      419 2024-02-04 10:09:00.323201 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/hatch/core.py
--rw-r--r--   0        0        0        0 2024-01-21 11:02:57.120575 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/hatch/hooks/__init__.py
--rw-r--r--   0        0        0     1600 2024-02-04 10:09:00.326542 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py
--rw-r--r--   0        0        0        0 2024-01-21 11:02:57.119034 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/hatch_hooks/__init__.py
--rw-r--r--   0        0        0      192 2024-02-04 10:09:00.322677 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/hatch_hooks/hooks.py
--rw-r--r--   0        0        0      253 2024-02-04 10:09:00.323439 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/parsing/__init__.py
--rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/parsing/core.py
--rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/parsing/rewrite.py
--rw-r--r--   0        0        0      543 2024-02-04 10:09:00.324596 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/repo/__init__.py
--rw-r--r--   0        0        0      861 2024-02-04 10:09:00.325693 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/repo/repo.py
--rw-r--r--   0        0        0      408 2024-02-04 10:09:00.321171 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/toml/__init__.py
--rw-r--r--   0        0        0     2172 2024-02-04 10:09:00.322399 hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/toml/core.py
--rw-r--r--   0        0        0      680 2024-02-04 10:09:00.320615 hatch_polylith_bricks-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 hatch_polylith_bricks-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3140 2024-01-23 22:26:31.652064 hatch_polylith_bricks-1.2.0/README.md
+-rw-r--r--   0        0        0       74 2024-04-08 06:15:46.532447 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-08 06:15:46.532719 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch/core.py
+-rw-r--r--   0        0        0        0 2024-01-21 11:02:57.120575 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch/hooks/__init__.py
+-rw-r--r--   0        0        0     1600 2024-04-08 06:15:46.535651 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py
+-rw-r--r--   0        0        0        0 2024-01-21 11:02:57.119034 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch_hooks/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-08 06:15:46.532144 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch_hooks/hooks.py
+-rw-r--r--   0        0        0      253 2024-04-08 06:15:46.532963 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/parsing/__init__.py
+-rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/parsing/core.py
+-rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/parsing/rewrite.py
+-rw-r--r--   0        0        0      543 2024-04-08 06:15:46.533995 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      861 2024-04-08 06:15:46.534851 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/repo.py
+-rw-r--r--   0        0        0      466 2024-04-08 06:15:46.530537 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     2919 2024-04-08 06:15:46.531856 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/toml/core.py
+-rw-r--r--   0        0        0      680 2024-04-08 06:15:46.529985 hatch_polylith_bricks-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 hatch_polylith_bricks-1.2.0/PKG-INFO
```

### Comparing `hatch_polylith_bricks-1.1.2/README.md` & `hatch_polylith_bricks-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py` & `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/parsing/core.py` & `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/parsing/core.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/parsing/rewrite.py` & `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/repo/__init__.py` & `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/repo/get.py` & `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/repo/repo.py` & `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.1.2/hatch_polylith_bricks/polylith/toml/core.py` & `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/toml/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from functools import reduce
 from pathlib import Path
 from typing import List, Union
 import tomlkit
 from hatch_polylith_bricks.polylith import repo
 
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

### Comparing `hatch_polylith_bricks-1.1.2/pyproject.toml` & `hatch_polylith_bricks-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hatch-polylith-bricks"
-version = "1.1.2"
+version = "1.2.0"
 description = "Hatch build hook plugin for Polylith"
 authors = ['David Vujic']
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 license = "MIT"
 readme = "README.md"
```

### Comparing `hatch_polylith_bricks-1.1.2/PKG-INFO` & `hatch_polylith_bricks-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-polylith-bricks
-Version: 1.1.2
+Version: 1.2.0
 Summary: Hatch build hook plugin for Polylith
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Hatch
 Classifier: License :: OSI Approved :: MIT License
```

