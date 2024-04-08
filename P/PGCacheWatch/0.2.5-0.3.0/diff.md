# Comparing `tmp/PGCacheWatch-0.2.5.tar.gz` & `tmp/PGCacheWatch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PGCacheWatch-0.2.5.tar", last modified: Mon Feb 26 08:15:40 2024, max compression
+gzip compressed data, was "PGCacheWatch-0.3.0.tar", last modified: Mon Apr  8 15:48:25 2024, max compression
```

## Comparing `PGCacheWatch-0.2.5.tar` & `PGCacheWatch-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:15:40.291305 PGCacheWatch-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:15:40.279305 PGCacheWatch-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:15:40.283305 PGCacheWatch-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-02-26 08:15:40.291305 PGCacheWatch-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:15:40.283305 PGCacheWatch-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/docs/introduction.md
--rw-r--r--   0 runner    (1001) docker     (127)   124806 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/docs/logo.webp
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/docs/setup.md
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/docs/strategies.md
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 08:15:40.291305 PGCacheWatch-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:15:40.279305 PGCacheWatch-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:15:40.291305 PGCacheWatch-0.2.5/src/PGCacheWatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-02-26 08:15:40.000000 PGCacheWatch-0.2.5/src/PGCacheWatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-02-26 08:15:40.000000 PGCacheWatch-0.2.5/src/PGCacheWatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 08:15:40.000000 PGCacheWatch-0.2.5/src/PGCacheWatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-26 08:15:40.000000 PGCacheWatch-0.2.5/src/PGCacheWatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-26 08:15:40.000000 PGCacheWatch-0.2.5/src/PGCacheWatch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:15:40.287305 PGCacheWatch-0.2.5/src/pgcachewatch/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/src/pgcachewatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/src/pgcachewatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-26 08:15:40.000000 PGCacheWatch-0.2.5/src/pgcachewatch/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/src/pgcachewatch/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/src/pgcachewatch/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/src/pgcachewatch/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/src/pgcachewatch/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/src/pgcachewatch/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/src/pgcachewatch/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/src/pgcachewatch/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/src/pgcachewatch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:15:40.291305 PGCacheWatch-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:15:40.291305 PGCacheWatch-0.2.5/tests/db/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/tests/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/tests/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/tests/test_decoraters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/tests/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/tests/test_listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/tests/test_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-02-26 08:15:14.000000 PGCacheWatch-0.2.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.820888 PGCacheWatch-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.820888 PGCacheWatch-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.824888 PGCacheWatch-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)   124806 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/logo.webp
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/pgb.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/setup.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/strategies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.820888 PGCacheWatch-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.824888 PGCacheWatch-0.3.0/src/pgcachewatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/pgcachewatch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/pg_bouncer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/tests/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_decoraters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_pg_bouncer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_utils.py
```

### Comparing `PGCacheWatch-0.2.5/.github/workflows/ci.yml` & `PGCacheWatch-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/.github/workflows/linting.yml` & `PGCacheWatch-0.3.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/.github/workflows/release.yml` & `PGCacheWatch-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/.gitignore` & `PGCacheWatch-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/LICENSE` & `PGCacheWatch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/PKG-INFO` & `PGCacheWatch-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PGCacheWatch
-Version: 0.2.5
+Version: 0.3.0
 Summary: A Python library for real-time PostgreSQL event-driven cache invalidation.
 Author: janbjorge
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Homepage, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Issues, https://github.com/janbjorge/pgcachewatch/issues
 Project-URL: Repository, https://github.com/janbjorge/pgcachewatch/
@@ -24,38 +24,46 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncpg>=0.27.0
 Requires-Dist: pydantic>=2.0.0
+Requires-Dist: websockets>=12.0.0
 Provides-Extra: dev
 Requires-Dist: asyncpg-stubs; extra == "dev"
 Requires-Dist: fastapi; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: mypy-extensions; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
+Requires-Dist: uvicorn; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
-# PGCacheWatch
+##  🚀 PGCacheWatch - Supercharge Your Caching Strategy 🚀
 [![CI](https://github.com/janbjorge/PGCacheWatch/actions/workflows/ci.yml/badge.svg)](https://github.com/janbjorge/PGCacheWatch/actions/workflows/ci.yml?query=branch%3Amain)
 [![pypi](https://img.shields.io/pypi/v/PGCacheWatch.svg)](https://pypi.python.org/pypi/PGCacheWatch)
 [![downloads](https://static.pepy.tech/badge/PGCacheWatch/month)](https://pepy.tech/project/PGCacheWatch)
 [![versions](https://img.shields.io/pypi/pyversions/PGCacheWatch.svg)](https://github.com/janbjorge/PGCacheWatch)
 
-PGCacheWatch is a Python library that enhances applications with real-time PostgreSQL event notifications, enabling efficient cache invalidation. It leverages the existing PostgreSQL infrastructure to simplify cache management while ensuring performance and data consistency.
+---
+📚 **Documentation**: [Explore the Docs 📖](https://pgcachewatch.readthedocs.io/en/latest/)
+
+🔍 **Source Code**: [View on GitHub 💾](https://github.com/janbjorge/PGCacheWatch/)
+
+---
+PGCacheWatch is the a Python library designed to propel your applications into a new realm of efficiency with real-time PostgreSQL event notifications for cache invalidation. Wave goodbye to stale data and hello to seamless cache management, bolstered performance powered by the robust backbone of PostgreSQL.
 
 ## Example with FastAPI
-This example illustrates the integration of PGCacheWatch with FastAPI to dynamically invalidate cache following database changes, thus maintaining the freshness and consistency of your application's data.
+PGCacheWatch integrates with FastAPI, empowering you to keep your application's data fresh and consistent by dynamically invalidating cache in line with database updates.
 
 ```python
 import contextlib
 import typing
 
 import asyncpg
 from fastapi import FastAPI
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PGCacheWatch-0.2.5/README.md` & `PGCacheWatch-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-# PGCacheWatch
+##  🚀 PGCacheWatch - Supercharge Your Caching Strategy 🚀
 [![CI](https://github.com/janbjorge/PGCacheWatch/actions/workflows/ci.yml/badge.svg)](https://github.com/janbjorge/PGCacheWatch/actions/workflows/ci.yml?query=branch%3Amain)
 [![pypi](https://img.shields.io/pypi/v/PGCacheWatch.svg)](https://pypi.python.org/pypi/PGCacheWatch)
 [![downloads](https://static.pepy.tech/badge/PGCacheWatch/month)](https://pepy.tech/project/PGCacheWatch)
 [![versions](https://img.shields.io/pypi/pyversions/PGCacheWatch.svg)](https://github.com/janbjorge/PGCacheWatch)
 
-PGCacheWatch is a Python library that enhances applications with real-time PostgreSQL event notifications, enabling efficient cache invalidation. It leverages the existing PostgreSQL infrastructure to simplify cache management while ensuring performance and data consistency.
+---
+📚 **Documentation**: [Explore the Docs 📖](https://pgcachewatch.readthedocs.io/en/latest/)
+
+🔍 **Source Code**: [View on GitHub 💾](https://github.com/janbjorge/PGCacheWatch/)
+
+---
+PGCacheWatch is the a Python library designed to propel your applications into a new realm of efficiency with real-time PostgreSQL event notifications for cache invalidation. Wave goodbye to stale data and hello to seamless cache management, bolstered performance powered by the robust backbone of PostgreSQL.
 
 ## Example with FastAPI
-This example illustrates the integration of PGCacheWatch with FastAPI to dynamically invalidate cache following database changes, thus maintaining the freshness and consistency of your application's data.
+PGCacheWatch integrates with FastAPI, empowering you to keep your application's data fresh and consistent by dynamically invalidating cache in line with database updates.
 
 ```python
 import contextlib
 import typing
 
 import asyncpg
 from fastapi import FastAPI
@@ -62,8 +68,8 @@
 async def get_data(user_id: int) -> dict:
     """
     This endpoint uses the cached_query function to return data, demonstrating
     how cache invalidation can be integrated into a web application route.
     """
     # Fetch and return the data using the cached query function.
     return await cached_query(user_id)
-```
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PGCacheWatch-0.2.5/docs/Makefile` & `PGCacheWatch-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/docs/configuration.md` & `PGCacheWatch-0.3.0/docs/configuration.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,10 @@
 # Configuration
 Configuring PGCacheWatch for optimal operation with PostgreSQL involves careful consideration of how you establish and manage your database connections, particularly when using asyncpg for asynchronous communication. Here's a refined approach to configuration, taking into account the nuances of connection pooling, listener persistence, and environmental configuration options.
 
-### Database Connection Configuration
-
-asyncpg offers versatile methods for configuring database connections, including environment variables, connection strings, and direct parameter specification. Here’s how to leverage these methods:
-
-### Environment Variables:
-asyncpg supports setting connection parameters through environment variables, which can simplify configuration management, especially in containerized or cloud environments.
-
-```shell
-   PGUSER=dbuser
-   PGPASSWORD=dbpass
-   PGHOST=localhost
-   PGPORT=5432
-   PGDATABASE=mydatabase
-```
-
-With these environment variables set, you can initiate a connection in asyncpg without explicitly specifying connection details:
-
-```python
-   conn = await asyncpg.connect()
-```
-
-### Connection Strings and Direct Parameters:
-You can specify the database connection details either through a DSN string or by passing parameters directly to the `connect` function, as previously described.
-
 ### Using Connection Pools with PGCacheWatch
 
 While asyncpg’s connection pooling is a powerful feature for managing database connections efficiently, it requires careful handling when used with LISTEN/NOTIFY channels due to the nature of persistent listeners.
 
 #### Persistent Listeners
 When a connection from the pool is used to set up LISTEN commands for notifications, it's important to keep that connection dedicated to listening. Returning the connection to the pool would remove the listeners, as the connection could be reused for other database operations, disrupting the notification flow.
```

### Comparing `PGCacheWatch-0.2.5/docs/examples.md` & `PGCacheWatch-0.3.0/docs/examples.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/docs/index.rst` & `PGCacheWatch-0.3.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,9 @@
    :maxdepth: 1
    :caption: Contents:
 
    introduction
    setup
    configuration
    strategies
+   pgb
    examples
```

### Comparing `PGCacheWatch-0.2.5/docs/introduction.md` & `PGCacheWatch-0.3.0/docs/introduction.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/docs/logo.webp` & `PGCacheWatch-0.3.0/docs/logo.webp`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/docs/make.bat` & `PGCacheWatch-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/docs/setup.md` & `PGCacheWatch-0.3.0/docs/setup.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/docs/strategies.md` & `PGCacheWatch-0.3.0/docs/strategies.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/pyproject.toml` & `PGCacheWatch-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "Topic :: Database",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 dependencies = [
     "asyncpg>=0.27.0",
     "pydantic>=2.0.0",
+    "websockets>=12.0.0",
 ]
 
 [project.urls]
 Documentation = "https://github.com/janbjorge/pgcachewatch/"
 Homepage = "https://github.com/janbjorge/pgcachewatch/"
 Issues = "https://github.com/janbjorge/pgcachewatch/issues"
 Repository = "https://github.com/janbjorge/pgcachewatch/"
@@ -45,14 +46,15 @@
     "fastapi",
     "httpx",
     "mypy-extensions",
     "mypy",
     "pytest-asyncio",
     "pytest",
     "ruff",
+    "uvicorn",
 ]
 docs = [
     "myst-parser",
     "sphinx",
     "sphinx-rtd-theme",
 ]
```

### Comparing `PGCacheWatch-0.2.5/src/PGCacheWatch.egg-info/PKG-INFO` & `PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PGCacheWatch
-Version: 0.2.5
+Version: 0.3.0
 Summary: A Python library for real-time PostgreSQL event-driven cache invalidation.
 Author: janbjorge
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Homepage, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Issues, https://github.com/janbjorge/pgcachewatch/issues
 Project-URL: Repository, https://github.com/janbjorge/pgcachewatch/
@@ -24,38 +24,46 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncpg>=0.27.0
 Requires-Dist: pydantic>=2.0.0
+Requires-Dist: websockets>=12.0.0
 Provides-Extra: dev
 Requires-Dist: asyncpg-stubs; extra == "dev"
 Requires-Dist: fastapi; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: mypy-extensions; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
+Requires-Dist: uvicorn; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
-# PGCacheWatch
+##  🚀 PGCacheWatch - Supercharge Your Caching Strategy 🚀
 [![CI](https://github.com/janbjorge/PGCacheWatch/actions/workflows/ci.yml/badge.svg)](https://github.com/janbjorge/PGCacheWatch/actions/workflows/ci.yml?query=branch%3Amain)
 [![pypi](https://img.shields.io/pypi/v/PGCacheWatch.svg)](https://pypi.python.org/pypi/PGCacheWatch)
 [![downloads](https://static.pepy.tech/badge/PGCacheWatch/month)](https://pepy.tech/project/PGCacheWatch)
 [![versions](https://img.shields.io/pypi/pyversions/PGCacheWatch.svg)](https://github.com/janbjorge/PGCacheWatch)
 
-PGCacheWatch is a Python library that enhances applications with real-time PostgreSQL event notifications, enabling efficient cache invalidation. It leverages the existing PostgreSQL infrastructure to simplify cache management while ensuring performance and data consistency.
+---
+📚 **Documentation**: [Explore the Docs 📖](https://pgcachewatch.readthedocs.io/en/latest/)
+
+🔍 **Source Code**: [View on GitHub 💾](https://github.com/janbjorge/PGCacheWatch/)
+
+---
+PGCacheWatch is the a Python library designed to propel your applications into a new realm of efficiency with real-time PostgreSQL event notifications for cache invalidation. Wave goodbye to stale data and hello to seamless cache management, bolstered performance powered by the robust backbone of PostgreSQL.
 
 ## Example with FastAPI
-This example illustrates the integration of PGCacheWatch with FastAPI to dynamically invalidate cache following database changes, thus maintaining the freshness and consistency of your application's data.
+PGCacheWatch integrates with FastAPI, empowering you to keep your application's data fresh and consistent by dynamically invalidating cache in line with database updates.
 
 ```python
 import contextlib
 import typing
 
 import asyncpg
 from fastapi import FastAPI
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PGCacheWatch-0.2.5/src/PGCacheWatch.egg-info/SOURCES.txt` & `PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 docs/conf.py
 docs/configuration.md
 docs/examples.md
 docs/index.rst
 docs/introduction.md
 docs/logo.webp
 docs/make.bat
+docs/pgb.md
 docs/setup.md
 docs/strategies.md
 src/PGCacheWatch.egg-info/PKG-INFO
 src/PGCacheWatch.egg-info/SOURCES.txt
 src/PGCacheWatch.egg-info/dependency_links.txt
 src/PGCacheWatch.egg-info/requires.txt
 src/PGCacheWatch.egg-info/top_level.txt
@@ -26,19 +27,21 @@
 src/pgcachewatch/__main__.py
 src/pgcachewatch/_version.py
 src/pgcachewatch/cli.py
 src/pgcachewatch/decorators.py
 src/pgcachewatch/listeners.py
 src/pgcachewatch/logconfig.py
 src/pgcachewatch/models.py
+src/pgcachewatch/pg_bouncer.py
 src/pgcachewatch/queries.py
 src/pgcachewatch/strategies.py
 src/pgcachewatch/utils.py
 tests/conftest.py
 tests/test_decoraters.py
 tests/test_fastapi.py
 tests/test_integration.py
 tests/test_listeners.py
+tests/test_pg_bouncer.py
 tests/test_strategies.py
 tests/test_utils.py
 tests/db/Dockerfile
 tests/db/init_db.sh
```

### Comparing `PGCacheWatch-0.2.5/src/pgcachewatch/cli.py` & `PGCacheWatch-0.3.0/src/pgcachewatch/cli.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/src/pgcachewatch/decorators.py` & `PGCacheWatch-0.3.0/src/pgcachewatch/decorators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import asyncio
+from functools import _make_key as make_key
 from typing import Awaitable, Callable, Hashable, Literal, TypeVar
 
 from typing_extensions import ParamSpec
 
-from pgcachewatch import strategies, utils
+from pgcachewatch import strategies
 from pgcachewatch.logconfig import logger
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def cache(
     strategy: strategies.Strategy,
-    statistics_callback: Callable[[Literal["hit", "miss"]], None] | None = None,
+    statistics_callback: Callable[[Literal["hit", "miss"]], None] = lambda _: None,
 ) -> Callable[[Callable[P, Awaitable[T]]], Callable[P, Awaitable[T]]]:
     def outer(fn: Callable[P, Awaitable[T]]) -> Callable[P, Awaitable[T]]:
         cached = dict[Hashable, asyncio.Future[T]]()
 
         async def inner(*args: P.args, **kwargs: P.kwargs) -> T:
             # If db-conn is down, disable cache.
             if not strategy.connection_healthy():
@@ -25,32 +26,28 @@
 
             # Clear cache if we have a event from
             # the database the instructs us to clear.
             if strategy.clear():
                 logger.debug("Cache clear")
                 cached.clear()
 
-            key = utils.make_key(args, kwargs)
+            key = make_key(args, kwargs, typed=False)
 
             try:
                 waiter = cached[key]
             except KeyError:
                 # Cache miss
-                ...
+                logger.debug("Cache miss")
+                statistics_callback("miss")
             else:
                 # Cache hit
                 logger.debug("Cache hit")
-                if statistics_callback:
-                    statistics_callback("hit")
+                statistics_callback("hit")
                 return await waiter
 
-            logger.debug("Cache miss")
-            if statistics_callback:
-                statistics_callback("miss")
-
             # Initialize Future to prevent cache stampedes.
             cached[key] = waiter = asyncio.Future[T]()
 
             try:
                 # # Attempt to compute result and set for waiter
                 waiter.set_result(await fn(*args, **kwargs))
             except Exception as e:
```

### Comparing `PGCacheWatch-0.2.5/src/pgcachewatch/models.py` & `PGCacheWatch-0.3.0/src/pgcachewatch/models.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/src/pgcachewatch/queries.py` & `PGCacheWatch-0.3.0/src/pgcachewatch/queries.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/src/pgcachewatch/strategies.py` & `PGCacheWatch-0.3.0/src/pgcachewatch/strategies.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/src/pgcachewatch/utils.py` & `PGCacheWatch-0.3.0/src/pgcachewatch/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,16 @@
 import asyncio
 import datetime
-import functools
-from typing import Generator, Hashable
+from typing import Generator
 
 import asyncpg
 
 from pgcachewatch import listeners, models
 
 
-def make_key(
-    args: tuple[Hashable, ...],
-    kwds: dict,
-    typed: bool = False,
-) -> Hashable:
-    """
-    Create a cache key from the given function arguments and keyword arguments.
-    """
-    return functools._make_key(args, kwds, typed)
-
-
 async def emit_event(
     conn: asyncpg.Connection | asyncpg.Pool,
     event: models.Event,
 ) -> None:
     """
     Emit an event to the specified PostgreSQL channel.
     """
```

### Comparing `PGCacheWatch-0.2.5/tests/db/init_db.sh` & `PGCacheWatch-0.3.0/tests/db/init_db.sh`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/tests/test_decoraters.py` & `PGCacheWatch-0.3.0/tests/test_decoraters.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/tests/test_fastapi.py` & `PGCacheWatch-0.3.0/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/tests/test_integration.py` & `PGCacheWatch-0.3.0/tests/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import collections
 import datetime
 
 import asyncpg
 import pytest
-from pgcachewatch import cli, decorators, listeners, models, strategies
+from pgcachewatch import cli, decorators, listeners, strategies
 
 
 def utcnow() -> datetime.datetime:
     return datetime.datetime.now(tz=datetime.timezone.utc)
 
 
 async def test_1_install_triggers(
@@ -34,43 +34,44 @@
 async def test_2_caching(
     N: int,
     pgconn: asyncpg.Connection,
     pgpool: asyncpg.Pool,
 ) -> None:
     statistics = collections.Counter[str]()
     listener = listeners.PGEventQueue()
-    await listener.connect(pgconn, models.PGChannel("ch_pgcachewatch_table_change"))
+    await listener.connect(pgconn)
 
     cnt = 0
 
     @decorators.cache(
         strategy=strategies.Greedy(listener=listener),
         statistics_callback=lambda x: statistics.update([x]),
     )
     async def fetch_sysconf() -> list:
         nonlocal cnt
         cnt += 1
         return await pgpool.fetch("SELECT * FROM sysconf")
 
     await asyncio.gather(*[fetch_sysconf() for _ in range(N)])
+
+    # Give a bit of leeway due IO network io.
+    await asyncio.sleep(0.1)
+
     assert cnt == 1
     assert statistics["miss"] == 1
     assert statistics["hit"] == N - 1
 
 
 async def test_3_cache_invalidation_update(
     pgconn: asyncpg.Connection,
     pgpool: asyncpg.Pool,
 ) -> None:
     statistics = collections.Counter[str]()
     listener = listeners.PGEventQueue()
-    await listener.connect(
-        pgconn,
-        models.PGChannel("ch_pgcachewatch_table_change"),
-    )
+    await listener.connect(pgconn)
 
     @decorators.cache(
         strategy=strategies.Greedy(listener=listener),
         statistics_callback=lambda x: statistics.update([x]),
     )
     async def fetch_sysconf() -> list:
         return await pgpool.fetch("SELECT * FROM sysconf")
@@ -93,18 +94,15 @@
 
 async def test_3_cache_invalidation_insert(
     pgconn: asyncpg.Connection,
     pgpool: asyncpg.Pool,
 ) -> None:
     statistics = collections.Counter[str]()
     listener = listeners.PGEventQueue()
-    await listener.connect(
-        pgconn,
-        models.PGChannel("ch_pgcachewatch_table_change"),
-    )
+    await listener.connect(pgconn)
 
     @decorators.cache(
         strategy=strategies.Greedy(listener=listener),
         statistics_callback=lambda x: statistics.update([x]),
     )
     async def fetch_sysconf() -> list:
         return await pgpool.fetch("SELECT * FROM sysconf")
@@ -128,18 +126,15 @@
 
 async def test_3_cache_invalidation_delete(
     pgconn: asyncpg.Connection,
     pgpool: asyncpg.Pool,
 ) -> None:
     statistics = collections.Counter[str]()
     listener = listeners.PGEventQueue()
-    await listener.connect(
-        pgconn,
-        models.PGChannel("ch_pgcachewatch_table_change"),
-    )
+    await listener.connect(pgconn)
 
     @decorators.cache(
         strategy=strategies.Greedy(listener=listener),
         statistics_callback=lambda x: statistics.update([x]),
     )
     async def fetch_sysconf() -> list:
         return await pgpool.fetch("SELECT * FROM sysconf")
```

### Comparing `PGCacheWatch-0.2.5/tests/test_strategies.py` & `PGCacheWatch-0.3.0/tests/test_strategies.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.2.5/tests/test_utils.py` & `PGCacheWatch-0.3.0/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,17 @@
                     table="placeholder",
                 ),
             )
             for _ in range(N)
         ]
     )
 
+    # Give a bit of leeway due IO network io.
+    await asyncio.sleep(0.1)
+
     assert listener.qsize() == N
     events = [listener.get_nowait() for _ in range(N)]
     assert len(events) == N
     assert [e.operation for e in events].count(operation) == N
 
 
 @pytest.mark.parametrize("max_iter", (100, 200, 500))
```

