# Comparing `tmp/tmdsclient-0.1.19.tar.gz` & `tmp/tmdsclient-0.1.20.tar.gz`

## Comparing `tmdsclient-0.1.19.tar` & `tmdsclient-0.1.20.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/README.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/domain-specific-terms.txt
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/requirements.txt
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.github/dependabot.yml
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.github/workflows/dev_test.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-spell_check.in
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-spell_check.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/src/_tmdsclient_version.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/src/tmdsclient/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/src/tmdsclient/py.typed
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/src/tmdsclient/client/__init__.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/src/tmdsclient/client/config.py
--rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/src/tmdsclient/client/tmdsclient.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/src/tmdsclient/models/__init__.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/src/tmdsclient/models/netzvertrag.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/src/tmdsclient/models/patches.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/LICENSE
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/pyproject.toml
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 tmdsclient-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/README.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/domain-specific-terms.txt
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/requirements.txt
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/dependabot.yml
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/dev_test.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-spell_check.in
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-spell_check.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/_tmdsclient_version.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/py.typed
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/client/__init__.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/client/config.py
+-rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/client/tmdsclient.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/models/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/models/bo4e_stub.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/models/netzvertrag.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/models/patches.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/LICENSE
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/pyproject.toml
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/PKG-INFO
```

### Comparing `tmdsclient-0.1.19/.pre-commit-config.yaml` & `tmdsclient-0.1.20/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/README.md` & `tmdsclient-0.1.20/README.md`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/requirements.txt` & `tmdsclient-0.1.20/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,13 +30,13 @@
     # via
     #   aiohttp
     #   yarl
 pydantic==2.6.4
     # via tmdsclient (pyproject.toml)
 pydantic-core==2.16.3
     # via pydantic
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   pydantic
     #   pydantic-core
 yarl==1.9.4
     # via aiohttp
```

### Comparing `tmdsclient-0.1.19/tox.ini` & `tmdsclient-0.1.20/tox.ini`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/.github/dependabot.yml` & `tmdsclient-0.1.20/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/.github/workflows/codeql-analysis.yml` & `tmdsclient-0.1.20/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/.github/workflows/coverage.yml` & `tmdsclient-0.1.20/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/.github/workflows/dependabot_automerge.yml` & `tmdsclient-0.1.20/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/.github/workflows/dev_test.yml` & `tmdsclient-0.1.20/.github/workflows/dev_test.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/.github/workflows/formatting.yml` & `tmdsclient-0.1.20/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/.github/workflows/packaging_test.yml` & `tmdsclient-0.1.20/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/.github/workflows/python-publish.yml` & `tmdsclient-0.1.20/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/.github/workflows/pythonlint.yml` & `tmdsclient-0.1.20/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/.github/workflows/unittests.yml` & `tmdsclient-0.1.20/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/dev_requirements/requirements-linting.txt` & `tmdsclient-0.1.20/dev_requirements/requirements-linting.txt`

 * *Files 0% similar despite different names*

```diff
@@ -29,12 +29,12 @@
     # via pylint-pydantic
 pylint-pydantic==0.3.2
     # via -r dev_requirements/requirements-linting.in
 tomli==2.0.1
     # via pylint
 tomlkit==0.11.6
     # via pylint
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   astroid
     #   pydantic
     #   pydantic-core
```

### Comparing `tmdsclient-0.1.19/dev_requirements/requirements-packaging.txt` & `tmdsclient-0.1.20/dev_requirements/requirements-packaging.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,77 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile dev_requirements/requirements-packaging.in
 #
-build==1.1.1
+build==1.2.1
     # via -r dev_requirements/requirements-packaging.in
 certifi==2024.2.2
     # via requests
+cffi==1.16.0
+    # via cryptography
 charset-normalizer==3.3.2
     # via requests
-colorama==0.4.6
-    # via build
+cryptography==42.0.5
+    # via secretstorage
 docutils==0.20.1
     # via readme-renderer
 idna==3.6
     # via requests
 importlib-metadata==7.0.2
     # via
     #   keyring
     #   twine
 jaraco-classes==3.3.1
     # via keyring
+jeepney==0.8.0
+    # via
+    #   keyring
+    #   secretstorage
 keyring==24.3.1
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
     # via jaraco-classes
 nh3==0.2.15
     # via readme-renderer
 packaging==24.0
     # via build
 pkginfo==1.10.0
     # via twine
+pycparser==2.21
+    # via cffi
 pygments==2.17.2
     # via
     #   readme-renderer
     #   rich
 pyproject-hooks==1.0.0
     # via build
-pywin32-ctypes==0.2.2
-    # via keyring
 readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.7.1
     # via twine
+secretstorage==3.3.3
+    # via keyring
+tomli==2.0.1
+    # via
+    #   build
+    #   pyproject-hooks
 twine==5.0.0
     # via -r dev_requirements/requirements-packaging.in
 urllib3==2.2.1
     # via
     #   requests
     #   twine
 zipp==3.18.1
```

### Comparing `tmdsclient-0.1.19/dev_requirements/requirements-tests.txt` & `tmdsclient-0.1.20/dev_requirements/requirements-tests.txt`

 * *Files 13% similar despite different names*

```diff
@@ -32,13 +32,13 @@
     # via pytest
 pluggy==1.4.0
     # via pytest
 pytest==8.1.1
     # via
     #   -r dev_requirements/requirements-tests.in
     #   pytest-asyncio
-pytest-asyncio==0.23.5.post1
+pytest-asyncio==0.23.6
     # via -r dev_requirements/requirements-tests.in
 tomli==2.0.1
     # via pytest
 yarl==1.9.4
     # via aiohttp
```

### Comparing `tmdsclient-0.1.19/src/tmdsclient/client/config.py` & `tmdsclient-0.1.20/src/tmdsclient/client/config.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/src/tmdsclient/client/tmdsclient.py` & `tmdsclient-0.1.20/src/tmdsclient/client/tmdsclient.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/src/tmdsclient/models/netzvertrag.py` & `tmdsclient-0.1.20/src/tmdsclient/models/netzvertrag.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,28 @@
 """
 
 from enum import StrEnum
 from uuid import UUID
 
 from pydantic import AwareDatetime, BaseModel, ConfigDict, Field, RootModel
 
+from tmdsclient.models.bo4e_stub import Menge
+
+
+class Vertragsteil(BaseModel):
+    """
+    BO4E COM Vertragsteil
+    """
+
+    vertragsteilbeginn: AwareDatetime
+    vertragsteilende: AwareDatetime | None = None
+    lokation: str
+    jahresverbrauchsprognose: Menge | None = None
+    kundenwert: Menge | None = None
+
 
 class Vertragsstatus(StrEnum):
     """
     Abbildung einer Statusinformation für Verträge.
     """
 
     # copied instead of imported from bo4e because: https://github.com/bo4e/BO4E-python/issues/724
@@ -33,14 +47,15 @@
     model_config = ConfigDict(extra="allow", populate_by_name=True)
     vertragsnummer: str
     vertragsbeginn: AwareDatetime
     vertragsende: AwareDatetime | None = None
     vertragstatus: Vertragsstatus
     # note that in TMDS / BO4E.net the property is called "vertragstatus" but in Python 'vertragsstatus'
     # https://github.com/Hochfrequenz/BO4E-dotnet/issues/417
+    vertragsteile: list[Vertragsteil] | None = None
 
 
 class TmdsMarktlokation(BaseModel):
     """tmds wrapper around a bo4e marktlokation"""
 
     model_config = ConfigDict(extra="allow", populate_by_name=True)
     id: str  #: e.g. '32631452574'
```

### Comparing `tmdsclient-0.1.19/src/tmdsclient/models/patches.py` & `tmdsclient-0.1.20/src/tmdsclient/models/patches.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/.gitignore` & `tmdsclient-0.1.20/.gitignore`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/LICENSE` & `tmdsclient-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/pyproject.toml` & `tmdsclient-0.1.20/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.19/PKG-INFO` & `tmdsclient-0.1.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tmdsclient
-Version: 0.1.19
+Version: 0.1.20
 Summary: Fully typed, async client library for Technical Master Data Service (TMDS)
 Project-URL: Changelog, https://github.com/Hochfrequenz/tmdsclient.py/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/tmdsclient.py
 Author-email: Hochfreuqenz Unternehmensberatung GmbH <info+github@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
 Keywords: technical master data,tmds
```

