# Comparing `tmp/blint-2.0.7.tar.gz` & `tmp/blint-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blint-2.0.7.tar", max compression
+gzip compressed data, was "blint-2.1.0.tar", max compression
```

## Comparing `blint-2.0.7.tar` & `blint-2.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1068 2024-04-07 21:55:22.516859 blint-2.0.7/LICENSE
--rw-r--r--   0        0        0     6215 2024-04-07 21:55:22.516859 blint-2.0.7/README.md
--rw-r--r--   0        0        0        0 2024-04-07 21:55:22.516859 blint-2.0.7/blint/__init__.py
--rw-r--r--   0        0        0    24122 2024-04-07 21:55:22.516859 blint-2.0.7/blint/analysis.py
--rw-r--r--   0        0        0    13955 2024-04-07 21:55:22.516859 blint-2.0.7/blint/android.py
--rw-r--r--   0        0        0    56201 2024-04-07 21:55:22.516859 blint-2.0.7/blint/binary.py
--rw-r--r--   0        0        0     2794 2024-04-07 21:55:22.516859 blint-2.0.7/blint/checks.py
--rw-r--r--   0        0        0     6198 2024-04-07 21:55:22.520859 blint-2.0.7/blint/cli.py
--rw-r--r--   0        0        0    20365 2024-04-07 21:55:22.520859 blint-2.0.7/blint/config.py
--rw-r--r--   0        0        0      324 2024-04-07 21:55:22.520859 blint-2.0.7/blint/cyclonedx/README.md
--rw-r--r--   0        0        0        0 2024-04-07 21:55:22.520859 blint-2.0.7/blint/cyclonedx/__init__.py
--rw-r--r--   0        0        0    20843 2024-04-07 21:55:22.520859 blint-2.0.7/blint/cyclonedx/spdx.py
--rw-r--r--   0        0        0   169203 2024-04-07 21:55:22.520859 blint-2.0.7/blint/cyclonedx/spec.py
--rw-r--r--   0        0        0        0 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/__init__.py
--rw-r--r--   0        0        0     1498 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_entries_generic.yml
--rw-r--r--   0        0        0     2358 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_entries_pe.yml
--rw-r--r--   0        0        0    15418 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_exe_go.yml
--rw-r--r--   0        0        0   124932 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_imports_pe.yml
--rw-r--r--   0        0        0     8155 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_methods_generic.yml
--rw-r--r--   0        0        0     5764 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_methods_mips.yml
--rw-r--r--   0        0        0     2409 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_monero_generic.yml
--rw-r--r--   0        0        0     1522 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_monero_go.yml
--rw-r--r--   0        0        0      994 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_monero_rust
--rw-r--r--   0        0        0      994 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_monero_rust.yml
--rw-r--r--   0        0        0     5646 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_rootkits_win.yml
--rw-r--r--   0        0        0     3507 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_symbols_antiforensic.yml
--rw-r--r--   0        0        0     2943 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_symbols_generic.yml
--rw-r--r--   0        0        0     1277 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_symbols_hooka.yml
--rw-r--r--   0        0        0    23537 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_symbols_macho.yml
--rw-r--r--   0        0        0    10425 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_symbols_rust.yml
--rw-r--r--   0        0        0    11038 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/rules.yml
--rw-r--r--   0        0        0      936 2024-04-07 21:55:22.520859 blint-2.0.7/blint/logger.py
--rw-r--r--   0        0        0    23205 2024-04-07 21:55:22.520859 blint-2.0.7/blint/sbom.py
--rw-r--r--   0        0        0    14323 2024-04-07 21:55:22.520859 blint-2.0.7/blint/utils.py
--rw-r--r--   0        0        0     1812 2024-04-07 21:55:22.524859 blint-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     7401 1970-01-01 00:00:00.000000 blint-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-08 14:45:06.242225 blint-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6215 2024-04-08 14:45:06.242225 blint-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 14:45:06.242225 blint-2.1.0/blint/__init__.py
+-rw-r--r--   0        0        0    24122 2024-04-08 14:45:06.242225 blint-2.1.0/blint/analysis.py
+-rw-r--r--   0        0        0    13955 2024-04-08 14:45:06.242225 blint-2.1.0/blint/android.py
+-rw-r--r--   0        0        0    56201 2024-04-08 14:45:06.242225 blint-2.1.0/blint/binary.py
+-rw-r--r--   0        0        0     2794 2024-04-08 14:45:06.242225 blint-2.1.0/blint/checks.py
+-rw-r--r--   0        0        0     6198 2024-04-08 14:45:06.242225 blint-2.1.0/blint/cli.py
+-rw-r--r--   0        0        0    20365 2024-04-08 14:45:06.242225 blint-2.1.0/blint/config.py
+-rw-r--r--   0        0        0      324 2024-04-08 14:45:06.242225 blint-2.1.0/blint/cyclonedx/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 14:45:06.242225 blint-2.1.0/blint/cyclonedx/__init__.py
+-rw-r--r--   0        0        0    20843 2024-04-08 14:45:06.242225 blint-2.1.0/blint/cyclonedx/spdx.py
+-rw-r--r--   0        0        0   169203 2024-04-08 14:45:06.242225 blint-2.1.0/blint/cyclonedx/spec.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:45:06.242225 blint-2.1.0/blint/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:45:06.242225 blint-2.1.0/blint/data/annotations/__init__.py
+-rw-r--r--   0        0        0     1498 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_entries_generic.yml
+-rw-r--r--   0        0        0     2358 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_entries_pe.yml
+-rw-r--r--   0        0        0    15418 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_exe_go.yml
+-rw-r--r--   0        0        0   124932 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_imports_pe.yml
+-rw-r--r--   0        0        0     8155 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_methods_generic.yml
+-rw-r--r--   0        0        0     5764 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_methods_mips.yml
+-rw-r--r--   0        0        0     2409 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_monero_generic.yml
+-rw-r--r--   0        0        0     1522 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_monero_go.yml
+-rw-r--r--   0        0        0      994 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_monero_rust
+-rw-r--r--   0        0        0      994 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_monero_rust.yml
+-rw-r--r--   0        0        0     5646 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_rootkits_win.yml
+-rw-r--r--   0        0        0     3507 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_symbols_antiforensic.yml
+-rw-r--r--   0        0        0     2943 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_symbols_generic.yml
+-rw-r--r--   0        0        0     1277 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_symbols_hooka.yml
+-rw-r--r--   0        0        0    23537 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_symbols_macho.yml
+-rw-r--r--   0        0        0    10425 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/annotations/review_symbols_rust.yml
+-rw-r--r--   0        0        0    11038 2024-04-08 14:45:06.246225 blint-2.1.0/blint/data/rules.yml
+-rw-r--r--   0        0        0      936 2024-04-08 14:45:06.246225 blint-2.1.0/blint/logger.py
+-rw-r--r--   0        0        0    23280 2024-04-08 14:45:06.246225 blint-2.1.0/blint/sbom.py
+-rw-r--r--   0        0        0    14323 2024-04-08 14:45:06.246225 blint-2.1.0/blint/utils.py
+-rw-r--r--   0        0        0     1812 2024-04-08 14:45:06.250225 blint-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7401 1970-01-01 00:00:00.000000 blint-2.1.0/PKG-INFO
```

### Comparing `blint-2.0.7/LICENSE` & `blint-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/README.md` & `blint-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/analysis.py` & `blint-2.1.0/blint/analysis.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/android.py` & `blint-2.1.0/blint/android.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/binary.py` & `blint-2.1.0/blint/binary.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/checks.py` & `blint-2.1.0/blint/checks.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/cli.py` & `blint-2.1.0/blint/cli.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/config.py` & `blint-2.1.0/blint/config.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/cyclonedx/spdx.py` & `blint-2.1.0/blint/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/cyclonedx/spec.py` & `blint-2.1.0/blint/cyclonedx/spec.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_entries_generic.yml` & `blint-2.1.0/blint/data/annotations/review_entries_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_entries_pe.yml` & `blint-2.1.0/blint/data/annotations/review_entries_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_exe_go.yml` & `blint-2.1.0/blint/data/annotations/review_exe_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_imports_pe.yml` & `blint-2.1.0/blint/data/annotations/review_imports_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_methods_generic.yml` & `blint-2.1.0/blint/data/annotations/review_methods_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_methods_mips.yml` & `blint-2.1.0/blint/data/annotations/review_methods_mips.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_monero_generic.yml` & `blint-2.1.0/blint/data/annotations/review_monero_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_monero_go.yml` & `blint-2.1.0/blint/data/annotations/review_monero_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_monero_rust` & `blint-2.1.0/blint/data/annotations/review_monero_rust`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_monero_rust.yml` & `blint-2.1.0/blint/data/annotations/review_monero_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_rootkits_win.yml` & `blint-2.1.0/blint/data/annotations/review_rootkits_win.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_symbols_antiforensic.yml` & `blint-2.1.0/blint/data/annotations/review_symbols_antiforensic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_symbols_generic.yml` & `blint-2.1.0/blint/data/annotations/review_symbols_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_symbols_hooka.yml` & `blint-2.1.0/blint/data/annotations/review_symbols_hooka.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_symbols_macho.yml` & `blint-2.1.0/blint/data/annotations/review_symbols_macho.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/annotations/review_symbols_rust.yml` & `blint-2.1.0/blint/data/annotations/review_symbols_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/data/rules.yml` & `blint-2.1.0/blint/data/rules.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/logger.py` & `blint-2.1.0/blint/logger.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/blint/sbom.py` & `blint-2.1.0/blint/sbom.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import base64
 import binascii
 import codecs
 import os
-import urllib.parse
 import uuid
 from datetime import datetime
 from typing import Any, Dict
 
 from rich.progress import Progress
 
 from blint.android import collect_app_metadata
@@ -522,15 +521,15 @@
             evidence=create_component_evidence(v.get("path"), 1.0) if v.get("path") else {},
             properties=[
                 Property(name="internal:serviceable", value=str(v.get("serviceable")).lower()),
                 Property(name="internal:hash_path", value=v.get("hashPath")),
             ],
         )
         if hash_content:
-            comp.hashes = Hash(alg=HashAlg.SHA_512, content=hash_content),
+            comp.hashes = [Hash(alg=HashAlg.SHA_512, content=hash_content)],
         comp.bom_ref = RefType(purl)
         components.append(comp)
     targets: dict[str, dict[str, dict]] = dotnet_deps.get("targets", {})
     for _, tv in targets.items():
         for k, v in tv.items():
             tmp_a = k.split("/")
             purl = f"pkg:nuget/{tmp_a[0]}@{tmp_a[1]}"
@@ -555,15 +554,17 @@
     """
     components = []
     # Key is the name and value is the version
     # We need to construct a purl by pretending the module name is the name with no namespace
     # This would make this compatible with cdxgen and depscan
     # See https://github.com/CycloneDX/cdxgen/issues/897
     for k, v in go_deps.items():
-        purl = f"""pkg:golang/{urllib.parse.quote_plus(k)}@{v.get("version")}"""
+        # See #83
+        # purl specification uses namespace hack for go to make this identifier use slash
+        purl = f"""pkg:golang/{k.lower()}@{v.get("version")}"""
         comp = Component(
             type=Type.library,
             name=k,
             version=v.get("version"),
             purl=purl,
             scope=Scope.required,
             evidence=create_component_evidence(k, 1.0)
@@ -572,15 +573,15 @@
         if v.get("hash"):
             try:
                 hash_content = codecs.encode(base64.b64decode(v.get("hash").removeprefix("h1:"), validate=True),
                                              encoding="hex")
             except binascii.Error:
                 hash_content = str(v.get("hash").removeprefix("h1:"))
         if hash_content:
-            comp.hashes = Hash(alg=HashAlg.SHA_256, content=hash_content)
+            comp.hashes = [Hash(alg=HashAlg.SHA_256, content=hash_content)]
         comp.bom_ref = RefType(f"""pkg:golang/{k}@{v.get("version")}""")
         components.append(comp)
     return components
 
 
 def track_dependency(
         dependencies_dict: dict[str, set], parent_component: Component, app_components: list[Component]
```

### Comparing `blint-2.0.7/blint/utils.py` & `blint-2.1.0/blint/utils.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.7/pyproject.toml` & `blint-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blint"
-version = "2.0.7"
+version = "2.1.0"
 description = "Linter and SBOM generator for binary files."
 authors = ["Prabhu Subramanian <prabhu@appthreat.com>", "Caroline Russell <caroline@appthreat.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/OWASP-dep-scan/blint"
 repository = "https://github.com/OWASP-dep-scan/blint"
 keywords = ["linter", "binary", "security", "sast"]
```

### Comparing `blint-2.0.7/PKG-INFO` & `blint-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blint
-Version: 2.0.7
+Version: 2.1.0
 Summary: Linter and SBOM generator for binary files.
 Home-page: https://github.com/OWASP-dep-scan/blint
 License: MIT
 Keywords: linter,binary,security,sast
 Author: Prabhu Subramanian
 Author-email: prabhu@appthreat.com
 Requires-Python: >=3.10,<3.13
```

