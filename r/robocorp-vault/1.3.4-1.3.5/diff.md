# Comparing `tmp/robocorp_vault-1.3.4.tar.gz` & `tmp/robocorp_vault-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_vault-1.3.4.tar", max compression
+gzip compressed data, was "robocorp_vault-1.3.5.tar", max compression
```

## Comparing `robocorp_vault-1.3.4.tar` & `robocorp_vault-1.3.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     1595 2024-03-08 10:52:25.201022 robocorp_vault-1.3.4/README.md
--rw-r--r--   0        0        0      811 2024-03-08 10:52:25.201022 robocorp_vault-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     4051 2024-03-08 10:52:25.201022 robocorp_vault-1.3.4/src/robocorp/vault/__init__.py
--rw-r--r--   0        0        0    12926 2024-03-08 10:52:25.201022 robocorp_vault-1.3.4/src/robocorp/vault/_adapters.py
--rw-r--r--   0        0        0      112 2024-03-08 10:52:25.201022 robocorp_vault-1.3.4/src/robocorp/vault/_errors.py
--rw-r--r--   0        0        0     6596 2024-03-08 10:52:25.201022 robocorp_vault-1.3.4/src/robocorp/vault/_requests.py
--rw-r--r--   0        0        0     1587 2024-03-08 10:52:25.201022 robocorp_vault-1.3.4/src/robocorp/vault/_secrets.py
--rw-r--r--   0        0        0     1858 2024-03-08 10:52:25.201022 robocorp_vault-1.3.4/src/robocorp/vault/_utils.py
--rw-r--r--   0        0        0     2945 2024-03-08 10:52:25.201022 robocorp_vault-1.3.4/src/robocorp/vault/_vault.py
--rw-r--r--   0        0        0        0 2024-03-08 10:52:25.201022 robocorp_vault-1.3.4/src/robocorp/vault/py.typed
--rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 robocorp_vault-1.3.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1571 2024-04-08 10:13:50.745021 robocorp_vault-1.3.5/README.md
+-rw-r--r--   0        0        0      811 2024-04-08 10:13:50.749021 robocorp_vault-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4051 2024-04-08 10:13:50.749021 robocorp_vault-1.3.5/src/robocorp/vault/__init__.py
+-rw-r--r--   0        0        0    12926 2024-04-08 10:13:50.749021 robocorp_vault-1.3.5/src/robocorp/vault/_adapters.py
+-rw-r--r--   0        0        0      112 2024-04-08 10:13:50.749021 robocorp_vault-1.3.5/src/robocorp/vault/_errors.py
+-rw-r--r--   0        0        0     6596 2024-04-08 10:13:50.749021 robocorp_vault-1.3.5/src/robocorp/vault/_requests.py
+-rw-r--r--   0        0        0     1587 2024-04-08 10:13:50.749021 robocorp_vault-1.3.5/src/robocorp/vault/_secrets.py
+-rw-r--r--   0        0        0     1858 2024-04-08 10:13:50.749021 robocorp_vault-1.3.5/src/robocorp/vault/_utils.py
+-rw-r--r--   0        0        0     2945 2024-04-08 10:13:50.749021 robocorp_vault-1.3.5/src/robocorp/vault/_vault.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:13:50.749021 robocorp_vault-1.3.5/src/robocorp/vault/py.typed
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 robocorp_vault-1.3.5/PKG-INFO
```

### Comparing `robocorp_vault-1.3.4/README.md` & `robocorp_vault-1.3.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 # robocorp-vault
 
-`robocorp-vault` is a library that provides read and write access to the
-[Vault](https://robocorp.com/docs/development-guide/variables-and-secrets/vault)
-in Robocorp Control Room, which can be used to store and retrieve secret values such as passwords.
+`robocorp-vault` is a library that provides read and write access to the [Vault](https://robocorp.com/docs/development-guide/variables-and-secrets/vault) in Robocorp Control Room, which can be used to store and retrieve secret values such as passwords.
 
 ## Getting started
 
-A secret consists of a name, an optional description, and a map of
-keys and values. For instance, one secret can be login credentials for a website,
-which includes both a username and a password:
+A secret consists of a name, an optional description, and a map of keys and values. For instance, one secret can be login credentials for a website, which includes both a username and a password:
 
 ```python
 from robocorp.tasks import task
 from robocorp import vault
 
 @task
 def inspect_secret():
@@ -29,12 +25,12 @@
 - [Hiding values](https://github.com/robocorp/robocorp/blob/master/vault/docs/guides/01-hiding-values.md)
 - [Modifying secrets](https://github.com/robocorp/robocorp/blob/master/vault/docs/guides/02-modifying-secrets.md)
 
 Further user guides and tutorials can be found in [Robocorp Docs](https://robocorp.com/docs).
 
 ## API Reference
 
-Information on specific functions or classes: [robocorp.vault](https://github.com/robocorp/robocorp/blob/master/vault/docs/api/robocorp.vault.md)
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/vault/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
 A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/vault/docs/CHANGELOG.md).
```

### Comparing `robocorp_vault-1.3.4/pyproject.toml` & `robocorp_vault-1.3.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-vault"
-version = "1.3.4"
+version = "1.3.5"
 description = "Robocorp Control Room Vault API integration library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
```

### Comparing `robocorp_vault-1.3.4/src/robocorp/vault/__init__.py` & `robocorp_vault-1.3.5/src/robocorp/vault/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from contextlib import nullcontext
 from functools import lru_cache
 from typing import Any
 
 from ._errors import RobocorpVaultError
 from ._secrets import SecretContainer
 
-__version__ = "1.3.4"
+__version__ = "1.3.5"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @lru_cache
 def _get_vault():
     from ._vault import Vault
```

### Comparing `robocorp_vault-1.3.4/src/robocorp/vault/_adapters.py` & `robocorp_vault-1.3.5/src/robocorp/vault/_adapters.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-1.3.4/src/robocorp/vault/_requests.py` & `robocorp_vault-1.3.5/src/robocorp/vault/_requests.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-1.3.4/src/robocorp/vault/_secrets.py` & `robocorp_vault-1.3.5/src/robocorp/vault/_secrets.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-1.3.4/src/robocorp/vault/_utils.py` & `robocorp_vault-1.3.5/src/robocorp/vault/_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-1.3.4/src/robocorp/vault/_vault.py` & `robocorp_vault-1.3.5/src/robocorp/vault/_vault.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-1.3.4/PKG-INFO` & `robocorp_vault-1.3.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-vault
-Version: 1.3.4
+Version: 1.3.5
 Summary: Robocorp Control Room Vault API integration library
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,23 +18,19 @@
 Requires-Dist: requests (>=2.31,<3.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Project-URL: Repository, https://github.com/robocorp/robocorp/
 Description-Content-Type: text/markdown
 
 # robocorp-vault
 
-`robocorp-vault` is a library that provides read and write access to the
-[Vault](https://robocorp.com/docs/development-guide/variables-and-secrets/vault)
-in Robocorp Control Room, which can be used to store and retrieve secret values such as passwords.
+`robocorp-vault` is a library that provides read and write access to the [Vault](https://robocorp.com/docs/development-guide/variables-and-secrets/vault) in Robocorp Control Room, which can be used to store and retrieve secret values such as passwords.
 
 ## Getting started
 
-A secret consists of a name, an optional description, and a map of
-keys and values. For instance, one secret can be login credentials for a website,
-which includes both a username and a password:
+A secret consists of a name, an optional description, and a map of keys and values. For instance, one secret can be login credentials for a website, which includes both a username and a password:
 
 ```python
 from robocorp.tasks import task
 from robocorp import vault
 
 @task
 def inspect_secret():
@@ -51,13 +47,13 @@
 - [Hiding values](https://github.com/robocorp/robocorp/blob/master/vault/docs/guides/01-hiding-values.md)
 - [Modifying secrets](https://github.com/robocorp/robocorp/blob/master/vault/docs/guides/02-modifying-secrets.md)
 
 Further user guides and tutorials can be found in [Robocorp Docs](https://robocorp.com/docs).
 
 ## API Reference
 
-Information on specific functions or classes: [robocorp.vault](https://github.com/robocorp/robocorp/blob/master/vault/docs/api/robocorp.vault.md)
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/vault/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
 A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/vault/docs/CHANGELOG.md).
```

