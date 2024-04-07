# Comparing `tmp/privacypass-0.2.1.tar.gz` & `tmp/privacypass-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/privacypass-0.2.1.tar", last modified: Mon Jan 24 11:43:05 2022, max compression
+gzip compressed data, was "privacypass-0.2.2.tar", last modified: Sun Apr  7 23:08:37 2024, max compression
```

## Comparing `privacypass-0.2.1.tar` & `privacypass-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:43:05.739887 privacypass-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1089 2022-01-24 11:42:43.000000 privacypass-0.2.1/.drone.yml
--rw-r--r--   0 root         (0) root         (0)      282 2022-01-24 11:42:43.000000 privacypass-0.2.1/.flake8
--rw-r--r--   0 root         (0) root         (0)       89 2022-01-24 11:42:43.000000 privacypass-0.2.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)      184 2022-01-24 11:42:43.000000 privacypass-0.2.1/.mypy.ini
--rw-r--r--   0 root         (0) root         (0)      817 2022-01-24 11:42:43.000000 privacypass-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1027 2022-01-24 11:42:43.000000 privacypass-0.2.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1070 2022-01-24 11:42:43.000000 privacypass-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4354 2022-01-24 11:43:05.739887 privacypass-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      164 2022-01-24 11:42:43.000000 privacypass-0.2.1/Pipfile
--rw-r--r--   0 root         (0) root         (0)     7352 2022-01-24 11:42:43.000000 privacypass-0.2.1/Pipfile.lock
--rw-r--r--   0 root         (0) root         (0)     3283 2022-01-24 11:42:43.000000 privacypass-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:43:05.735887 privacypass-0.2.1/docs/
--rw-r--r--   0 root         (0) root         (0)   150990 2022-01-24 11:42:43.000000 privacypass-0.2.1/docs/firefox_tokens.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:43:05.736887 privacypass-0.2.1/privacypass/
--rw-r--r--   0 root         (0) root         (0)       69 2022-01-24 11:42:43.000000 privacypass-0.2.1/privacypass/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2053 2022-01-24 11:42:43.000000 privacypass-0.2.1/privacypass/privacypass.py
--rw-r--r--   0 root         (0) root         (0)     1715 2022-01-24 11:42:43.000000 privacypass-0.2.1/privacypass/voprf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:43:05.738887 privacypass-0.2.1/privacypass.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4354 2022-01-24 11:43:05.000000 privacypass-0.2.1/privacypass.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      411 2022-01-24 11:43:05.000000 privacypass-0.2.1/privacypass.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-24 11:43:05.000000 privacypass-0.2.1/privacypass.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-01-24 11:43:05.000000 privacypass-0.2.1/privacypass.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-01-24 11:43:05.000000 privacypass-0.2.1/privacypass.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      215 2022-01-24 11:42:43.000000 privacypass-0.2.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-24 11:43:05.739887 privacypass-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1437 2022-01-24 11:42:43.000000 privacypass-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 23:08:37.244420 privacypass-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-04-07 23:08:17.000000 privacypass-0.2.2/.drone.yml
+-rw-r--r--   0 root         (0) root         (0)      282 2024-04-07 23:08:17.000000 privacypass-0.2.2/.flake8
+-rw-r--r--   0 root         (0) root         (0)       89 2024-04-07 23:08:17.000000 privacypass-0.2.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      184 2024-04-07 23:08:17.000000 privacypass-0.2.2/.mypy.ini
+-rw-r--r--   0 root         (0) root         (0)      817 2024-04-07 23:08:17.000000 privacypass-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-04-07 23:08:17.000000 privacypass-0.2.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-07 23:08:17.000000 privacypass-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3825 2024-04-07 23:08:37.243420 privacypass-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-07 23:08:17.000000 privacypass-0.2.2/Pipfile
+-rw-r--r--   0 root         (0) root         (0)     8793 2024-04-07 23:08:17.000000 privacypass-0.2.2/Pipfile.lock
+-rw-r--r--   0 root         (0) root         (0)     3283 2024-04-07 23:08:17.000000 privacypass-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 23:08:37.240420 privacypass-0.2.2/docs/
+-rw-r--r--   0 root         (0) root         (0)   150990 2024-04-07 23:08:17.000000 privacypass-0.2.2/docs/firefox_tokens.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 23:08:37.241420 privacypass-0.2.2/privacypass/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-07 23:08:17.000000 privacypass-0.2.2/privacypass/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2024-04-07 23:08:17.000000 privacypass-0.2.2/privacypass/privacypass.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2024-04-07 23:08:17.000000 privacypass-0.2.2/privacypass/voprf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 23:08:37.243420 privacypass-0.2.2/privacypass.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3825 2024-04-07 23:08:37.000000 privacypass-0.2.2/privacypass.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-07 23:08:37.000000 privacypass-0.2.2/privacypass.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 23:08:37.000000 privacypass-0.2.2/privacypass.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 23:08:37.000000 privacypass-0.2.2/privacypass.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-07 23:08:37.000000 privacypass-0.2.2/privacypass.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      169 2024-04-07 23:08:17.000000 privacypass-0.2.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 23:08:37.244420 privacypass-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1437 2024-04-07 23:08:17.000000 privacypass-0.2.2/setup.py
```

### Comparing `privacypass-0.2.1/.drone.yml` & `privacypass-0.2.2/.drone.yml`

 * *Files identical despite different names*

### Comparing `privacypass-0.2.1/.pre-commit-config.yaml` & `privacypass-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `privacypass-0.2.1/CHANGELOG.md` & `privacypass-0.2.2/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 ### Added
 ### Changed
 ### Deprecated
 ### Removed
 ### Fixed
 ### Security
 
+## [0.2.2]
+### Security
+- Updated cryptography library to 42.0.4
+
 ## [0.2.1]
 ### Fixed
 - redemption_header() returns token with value
 
 ## [0.2.0]
 ### Added
 - privacypass: redemption_header()
@@ -27,10 +31,12 @@
 - voprf: derive_key() - Derives the shared key used for redemption MACs
 - voprf: create_request_binding()
 - privacypass: redemption_token()
 - docs: Initial README
 - docs: Firefox Token extraction steps in README
 - docs: Usage example
 
-[Unreleased]: https://github.com/sergebakharev/privacypass/compare/v0.2.0...HEAD
+[Unreleased]: https://github.com/sergebakharev/privacypass/compare/v0.2.2...HEAD
+[0.2.2]: https://github.com/sergebakharev/privacypass/releases/tag/v0.2.2
+[0.2.1]: https://github.com/sergebakharev/privacypass/releases/tag/v0.2.1
 [0.2.0]: https://github.com/sergebakharev/privacypass/releases/tag/v0.2.0
 [0.1.0]: https://github.com/sergebakharev/privacypass/releases/tag/v0.1.0
```

### Comparing `privacypass-0.2.1/LICENSE` & `privacypass-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `privacypass-0.2.1/README.md` & `privacypass-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `privacypass-0.2.1/docs/firefox_tokens.png` & `privacypass-0.2.2/docs/firefox_tokens.png`

 * *Files identical despite different names*

### Comparing `privacypass-0.2.1/privacypass/privacypass.py` & `privacypass-0.2.2/privacypass/privacypass.py`

 * *Files identical despite different names*

### Comparing `privacypass-0.2.1/privacypass/voprf.py` & `privacypass-0.2.2/privacypass/voprf.py`

 * *Files identical despite different names*

### Comparing `privacypass-0.2.1/setup.py` & `privacypass-0.2.2/setup.py`

 * *Files identical despite different names*

