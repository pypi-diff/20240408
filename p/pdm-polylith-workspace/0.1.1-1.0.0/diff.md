# Comparing `tmp/pdm_polylith_workspace-0.1.1.tar.gz` & `tmp/pdm_polylith_workspace-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_polylith_workspace-0.1.1.tar", max compression
+gzip compressed data, was "pdm_polylith_workspace-1.0.0.tar", max compression
```

## Comparing `pdm_polylith_workspace-0.1.1.tar` & `pdm_polylith_workspace-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1008 2024-01-23 21:16:34.627315 pdm_polylith_workspace-0.1.1/README.md
--rw-r--r--   0        0        0      568 2024-02-05 13:17:26.176815 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/configuration/__init__.py
--rw-r--r--   0        0        0     2194 2024-02-05 13:17:26.177666 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/configuration/core.py
--rw-r--r--   0        0        0      255 2024-02-05 13:17:26.179710 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/parsing/__init__.py
--rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/parsing/core.py
--rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/parsing/rewrite.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623045 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/pdm/__init__.py
--rw-r--r--   0        0        0     1150 2024-02-05 13:17:26.182214 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/pdm/core.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623415 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/pdm/hooks/__init__.py
--rw-r--r--   0        0        0      643 2024-02-05 13:17:26.182718 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py
--rw-r--r--   0        0        0     1022 2024-02-05 13:17:26.183431 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.621252 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/pdm_workspace_hooks/__init__.py
--rw-r--r--   0        0        0      465 2024-02-05 13:17:26.179490 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/pdm_workspace_hooks/core.py
--rw-r--r--   0        0        0      545 2024-02-05 13:17:26.180707 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/repo/__init__.py
--rw-r--r--   0        0        0      862 2024-02-05 13:17:26.181541 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/repo/repo.py
--rw-r--r--   0        0        0      409 2024-02-05 13:17:26.177948 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/toml/__init__.py
--rw-r--r--   0        0        0     2173 2024-02-05 13:17:26.179086 pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/toml/core.py
--rw-r--r--   0        0        0      645 2024-02-05 13:17:26.176266 pdm_polylith_workspace-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 pdm_polylith_workspace-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1008 2024-01-23 21:16:34.627315 pdm_polylith_workspace-1.0.0/README.md
+-rw-r--r--   0        0        0      568 2024-04-08 06:18:29.082224 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/configuration/__init__.py
+-rw-r--r--   0        0        0     2194 2024-04-08 06:18:29.083066 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/configuration/core.py
+-rw-r--r--   0        0        0      255 2024-04-08 06:18:29.085193 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/parsing/__init__.py
+-rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/parsing/core.py
+-rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/parsing/rewrite.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623045 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/__init__.py
+-rw-r--r--   0        0        0     1150 2024-04-08 06:18:29.087705 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/core.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623415 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/hooks/__init__.py
+-rw-r--r--   0        0        0      643 2024-04-08 06:18:29.088206 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py
+-rw-r--r--   0        0        0     1022 2024-04-08 06:18:29.088916 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.621252 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm_workspace_hooks/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-08 06:18:29.084970 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm_workspace_hooks/core.py
+-rw-r--r--   0        0        0      545 2024-04-08 06:18:29.086211 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-08 06:18:29.087058 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/repo.py
+-rw-r--r--   0        0        0      467 2024-04-08 06:18:29.083338 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     2920 2024-04-08 06:18:29.084564 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/toml/core.py
+-rw-r--r--   0        0        0      645 2024-04-08 06:18:29.081665 pdm_polylith_workspace-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 pdm_polylith_workspace-1.0.0/PKG-INFO
```

### Comparing `pdm_polylith_workspace-0.1.1/README.md` & `pdm_polylith_workspace-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/configuration/__init__.py` & `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/configuration/core.py` & `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/configuration/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/parsing/core.py` & `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/parsing/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/parsing/rewrite.py` & `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/pdm/core.py` & `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py` & `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py` & `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/repo/__init__.py` & `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/repo/get.py` & `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/repo/repo.py` & `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-0.1.1/pdm_polylith_workspace/polylith/toml/core.py` & `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/toml/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from functools import reduce
 from pathlib import Path
 from typing import List, Union
 import tomlkit
 from pdm_polylith_workspace.polylith import repo
 
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

### Comparing `pdm_polylith_workspace-0.1.1/pyproject.toml` & `pdm_polylith_workspace-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdm-polylith-workspace"
-version = "0.1.1"
+version = "1.0.0"
 description = "a PDM build hook for a Polylith workspace"
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 authors = ["David Vujic"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `pdm_polylith_workspace-0.1.1/PKG-INFO` & `pdm_polylith_workspace-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-polylith-workspace
-Version: 0.1.1
+Version: 1.0.0
 Summary: a PDM build hook for a Polylith workspace
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

