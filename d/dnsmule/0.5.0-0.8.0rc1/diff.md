# Comparing `tmp/dnsmule-0.5.0.tar.gz` & `tmp/dnsmule-0.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnsmule-0.5.0.tar", last modified: Sat May 13 17:40:08 2023, max compression
+gzip compressed data, was "dnsmule-0.8.0rc1.tar", last modified: Mon Apr  8 13:36:10 2024, max compression
```

## Comparing `dnsmule-0.5.0.tar` & `dnsmule-0.8.0rc1.tar`

### file list

```diff
@@ -1,55 +1,41 @@
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.226354 dnsmule-0.5.0/
--rw-r--r--   0 jonium     (501) staff       (20)     1063 2023-02-15 09:31:46.000000 dnsmule-0.5.0/LICENSE
--rw-r--r--   0 jonium     (501) staff       (20)     8013 2023-05-13 17:40:08.226134 dnsmule-0.5.0/PKG-INFO
--rw-r--r--   0 jonium     (501) staff       (20)     7194 2023-05-13 11:50:37.000000 dnsmule-0.5.0/README.md
--rw-r--r--   0 jonium     (501) staff       (20)       38 2023-05-13 17:40:08.226404 dnsmule-0.5.0/setup.cfg
--rw-r--r--   0 jonium     (501) staff       (20)     1691 2023-05-13 11:50:37.000000 dnsmule-0.5.0/setup.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.211698 dnsmule-0.5.0/src/
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.214478 dnsmule-0.5.0/src/DNSMule.egg-info/
--rw-r--r--   0 jonium     (501) staff       (20)     8013 2023-05-13 17:40:08.000000 dnsmule-0.5.0/src/DNSMule.egg-info/PKG-INFO
--rw-r--r--   0 jonium     (501) staff       (20)     1377 2023-05-13 17:40:08.000000 dnsmule-0.5.0/src/DNSMule.egg-info/SOURCES.txt
--rw-r--r--   0 jonium     (501) staff       (20)        1 2023-05-13 17:40:08.000000 dnsmule-0.5.0/src/DNSMule.egg-info/dependency_links.txt
--rw-r--r--   0 jonium     (501) staff       (20)       88 2023-05-13 17:40:08.000000 dnsmule-0.5.0/src/DNSMule.egg-info/requires.txt
--rw-r--r--   0 jonium     (501) staff       (20)        8 2023-05-13 17:40:08.000000 dnsmule-0.5.0/src/DNSMule.egg-info/top_level.txt
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.215765 dnsmule-0.5.0/src/dnsmule/
--rw-r--r--   0 jonium     (501) staff       (20)      232 2023-03-21 09:59:05.000000 dnsmule-0.5.0/src/dnsmule/__init__.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.219038 dnsmule-0.5.0/src/dnsmule/backends/
--rw-r--r--   0 jonium     (501) staff       (20)       60 2023-03-13 07:50:12.000000 dnsmule-0.5.0/src/dnsmule/backends/__init__.py
--rw-r--r--   0 jonium     (501) staff       (20)      860 2023-05-10 10:10:12.000000 dnsmule-0.5.0/src/dnsmule/backends/abstract.py
--rw-r--r--   0 jonium     (501) staff       (20)     3081 2023-05-13 17:23:22.000000 dnsmule-0.5.0/src/dnsmule/backends/dnspython.py
--rw-r--r--   0 jonium     (501) staff       (20)      330 2023-05-10 10:10:12.000000 dnsmule-0.5.0/src/dnsmule/backends/noop.py
--rw-r--r--   0 jonium     (501) staff       (20)     1210 2023-05-10 10:10:12.000000 dnsmule-0.5.0/src/dnsmule/baseclasses.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.220649 dnsmule-0.5.0/src/dnsmule/definitions/
--rw-r--r--   0 jonium     (501) staff       (20)      129 2023-03-21 09:59:05.000000 dnsmule-0.5.0/src/dnsmule/definitions/__init__.py
--rw-r--r--   0 jonium     (501) staff       (20)       89 2023-03-21 09:59:05.000000 dnsmule-0.5.0/src/dnsmule/definitions/domain.py
--rw-r--r--   0 jonium     (501) staff       (20)     1265 2023-05-13 13:31:06.000000 dnsmule-0.5.0/src/dnsmule/definitions/record.py
--rw-r--r--   0 jonium     (501) staff       (20)     2077 2023-05-10 10:10:12.000000 dnsmule-0.5.0/src/dnsmule/definitions/result.py
--rw-r--r--   0 jonium     (501) staff       (20)     6866 2023-03-21 09:59:05.000000 dnsmule-0.5.0/src/dnsmule/definitions/rrtype.py
--rw-r--r--   0 jonium     (501) staff       (20)       80 2023-03-21 09:59:05.000000 dnsmule-0.5.0/src/dnsmule/definitions/tag.py
--rw-r--r--   0 jonium     (501) staff       (20)     5573 2023-05-13 12:34:41.000000 dnsmule-0.5.0/src/dnsmule/loader.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.221042 dnsmule-0.5.0/src/dnsmule/logger/
--rw-r--r--   0 jonium     (501) staff       (20)       31 2023-03-21 09:59:05.000000 dnsmule-0.5.0/src/dnsmule/logger/__init__.py
--rw-r--r--   0 jonium     (501) staff       (20)      108 2023-03-21 09:59:05.000000 dnsmule-0.5.0/src/dnsmule/logger/logger.py
--rw-r--r--   0 jonium     (501) staff       (20)     3646 2023-05-13 12:53:27.000000 dnsmule-0.5.0/src/dnsmule/mule.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.221730 dnsmule-0.5.0/src/dnsmule/plugins/
--rw-r--r--   0 jonium     (501) staff       (20)       38 2023-03-21 09:59:05.000000 dnsmule-0.5.0/src/dnsmule/plugins/__init__.py
--rw-r--r--   0 jonium     (501) staff       (20)     1191 2023-05-10 10:10:12.000000 dnsmule-0.5.0/src/dnsmule/plugins/abstract.py
--rw-r--r--   0 jonium     (501) staff       (20)      189 2023-05-10 10:10:12.000000 dnsmule-0.5.0/src/dnsmule/plugins/noop.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.222984 dnsmule-0.5.0/src/dnsmule/rules/
--rw-r--r--   0 jonium     (501) staff       (20)       77 2023-03-13 07:50:12.000000 dnsmule-0.5.0/src/dnsmule/rules/__init__.py
--rw-r--r--   0 jonium     (501) staff       (20)     2664 2023-05-10 10:10:12.000000 dnsmule-0.5.0/src/dnsmule/rules/entities.py
--rw-r--r--   0 jonium     (501) staff       (20)     1197 2023-05-09 14:36:29.000000 dnsmule-0.5.0/src/dnsmule/rules/factories.py
--rw-r--r--   0 jonium     (501) staff       (20)     2259 2023-03-21 09:59:05.000000 dnsmule-0.5.0/src/dnsmule/rules/rules.py
--rw-r--r--   0 jonium     (501) staff       (20)     3308 2023-05-10 10:10:12.000000 dnsmule-0.5.0/src/dnsmule/rules/ruletypes.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.224567 dnsmule-0.5.0/src/dnsmule/storages/
--rw-r--r--   0 jonium     (501) staff       (20)      323 2023-05-11 15:45:45.000000 dnsmule-0.5.0/src/dnsmule/storages/__init__.py
--rw-r--r--   0 jonium     (501) staff       (20)     8021 2023-05-13 14:16:58.000000 dnsmule-0.5.0/src/dnsmule/storages/abstract.py
--rw-r--r--   0 jonium     (501) staff       (20)     1300 2023-05-10 13:59:37.000000 dnsmule-0.5.0/src/dnsmule/storages/dictstorage.py
--rw-r--r--   0 jonium     (501) staff       (20)     4103 2023-05-11 18:44:21.000000 dnsmule-0.5.0/src/dnsmule/storages/mongodbstorage.py
--rw-r--r--   0 jonium     (501) staff       (20)     1731 2023-05-13 14:18:38.000000 dnsmule-0.5.0/src/dnsmule/storages/redisstorage.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.225125 dnsmule-0.5.0/src/dnsmule/utils/
--rw-r--r--   0 jonium     (501) staff       (20)       20 2023-05-10 10:10:12.000000 dnsmule-0.5.0/src/dnsmule/utils/__init__.py
--rw-r--r--   0 jonium     (501) staff       (20)     3653 2023-05-10 11:17:54.000000 dnsmule-0.5.0/src/dnsmule/utils/misc.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:40:08.225627 dnsmule-0.5.0/test/
--rw-r--r--   0 jonium     (501) staff       (20)     1054 2023-05-10 10:10:12.000000 dnsmule-0.5.0/test/test_baseclasses.py
--rw-r--r--   0 jonium     (501) staff       (20)     5105 2023-05-13 12:54:08.000000 dnsmule-0.5.0/test/test_mule.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:10.934992 dnsmule-0.8.0rc1/
+-rw-r--r--   0 jonium     (501) staff       (20)     1063 2023-02-15 09:31:46.000000 dnsmule-0.8.0rc1/LICENSE
+-rw-r--r--   0 jonium     (501) staff       (20)     7402 2024-04-08 13:36:10.934786 dnsmule-0.8.0rc1/PKG-INFO
+-rw-r--r--   0 jonium     (501) staff       (20)     6241 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/README.md
+-rw-r--r--   0 jonium     (501) staff       (20)       38 2024-04-08 13:36:10.935027 dnsmule-0.8.0rc1/setup.cfg
+-rw-r--r--   0 jonium     (501) staff       (20)     1691 2023-05-13 11:50:37.000000 dnsmule-0.8.0rc1/setup.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:10.927589 dnsmule-0.8.0rc1/src/
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:10.933761 dnsmule-0.8.0rc1/src/DNSMule.egg-info/
+-rw-r--r--   0 jonium     (501) staff       (20)     7402 2024-04-08 13:36:10.000000 dnsmule-0.8.0rc1/src/DNSMule.egg-info/PKG-INFO
+-rw-r--r--   0 jonium     (501) staff       (20)     1034 2024-04-08 13:36:10.000000 dnsmule-0.8.0rc1/src/DNSMule.egg-info/SOURCES.txt
+-rw-r--r--   0 jonium     (501) staff       (20)        1 2024-04-08 13:36:10.000000 dnsmule-0.8.0rc1/src/DNSMule.egg-info/dependency_links.txt
+-rw-r--r--   0 jonium     (501) staff       (20)       88 2024-04-08 13:36:10.000000 dnsmule-0.8.0rc1/src/DNSMule.egg-info/requires.txt
+-rw-r--r--   0 jonium     (501) staff       (20)        8 2024-04-08 13:36:10.000000 dnsmule-0.8.0rc1/src/DNSMule.egg-info/top_level.txt
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:10.930299 dnsmule-0.8.0rc1/src/dnsmule/
+-rw-r--r--   0 jonium     (501) staff       (20)      311 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/__init__.py
+-rw-r--r--   0 jonium     (501) staff       (20)     1206 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/__main__.py
+-rw-r--r--   0 jonium     (501) staff       (20)     8055 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/api.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:10.932033 dnsmule-0.8.0rc1/src/dnsmule/backends/
+-rw-r--r--   0 jonium     (501) staff       (20)      341 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/backends/__init__.py
+-rw-r--r--   0 jonium     (501) staff       (20)     2138 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/backends/csvfile.py
+-rw-r--r--   0 jonium     (501) staff       (20)     1368 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/backends/data.py
+-rw-r--r--   0 jonium     (501) staff       (20)     3593 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/backends/dnspython.py
+-rw-r--r--   0 jonium     (501) staff       (20)     1962 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/backends/doh.py
+-rw-r--r--   0 jonium     (501) staff       (20)      255 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/backends/noop.py
+-rw-r--r--   0 jonium     (501) staff       (20)     2593 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/loader.py
+-rw-r--r--   0 jonium     (501) staff       (20)     6950 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/rrtype.py
+-rw-r--r--   0 jonium     (501) staff       (20)     4740 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/rules.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:10.933164 dnsmule-0.8.0rc1/src/dnsmule/storages/
+-rw-r--r--   0 jonium     (501) staff       (20)      226 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/storages/__init__.py
+-rw-r--r--   0 jonium     (501) staff       (20)     1802 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/storages/db_mongo.py
+-rw-r--r--   0 jonium     (501) staff       (20)     2159 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/storages/db_mysql.py
+-rw-r--r--   0 jonium     (501) staff       (20)      905 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/storages/db_redis.py
+-rw-r--r--   0 jonium     (501) staff       (20)     1790 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/storages/db_sqlite.py
+-rw-r--r--   0 jonium     (501) staff       (20)      438 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/storages/dictionary.py
+-rw-r--r--   0 jonium     (501) staff       (20)     1020 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/storages/key_value.py
+-rw-r--r--   0 jonium     (501) staff       (20)      358 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/storages/noop.py
+-rw-r--r--   0 jonium     (501) staff       (20)     4254 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/src/dnsmule/utils.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:10.933578 dnsmule-0.8.0rc1/test/
+-rw-r--r--   0 jonium     (501) staff       (20)      531 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/test/test_loader.py
+-rw-r--r--   0 jonium     (501) staff       (20)     3010 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/test/test_mule.py
+-rw-r--r--   0 jonium     (501) staff       (20)      960 2024-04-08 13:27:27.000000 dnsmule-0.8.0rc1/test/test_rrtype.py
```

### Comparing `dnsmule-0.5.0/LICENSE` & `dnsmule-0.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dnsmule-0.5.0/PKG-INFO` & `dnsmule-0.8.0rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnsmule
-Version: 0.5.0
+Version: 0.8.0rc1
 Summary: Rule based dependency scanning and service fingerprinting via DNS
 Home-page: https://github.com/joniumGit/dnsmule
 Author: joniumGit
 Author-email: 52005121+joniumGit@users.noreply.github.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/joniumGit/dnsmule/issues
 Project-URL: Source, https://github.com/joniumGit/dnsmule
@@ -13,146 +13,177 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyyaml
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: redis; extra == "dev"
+Requires-Dist: pymongo; extra == "dev"
+Requires-Dist: dnspython; extra == "dev"
 Provides-Extra: full
-License-File: LICENSE
+Requires-Dist: redis; extra == "full"
+Requires-Dist: pymongo; extra == "full"
+Requires-Dist: dnspython; extra == "full"
 
 # DNSMule
 
 [![codecov](https://codecov.io/gh/joniumGit/dnsmule/branch/master/graph/badge.svg?token=54DPREJIFU)](https://codecov.io/gh/joniumGit/dnsmule)
 
 Package for rule based dependency scanning and service fingerprinting via DNS.
 
-This package provides utilities for writing and evaluating verbose and easy to read rule definitions in _YAML_-format.
-There are two builtin rule formats with more available as plugins.
+This package provides utilities for writing and evaluating verbose and easy to read rule definitions in YAML-format.
+There some builtin rule formats with more available as plugins.
+
+## Note: 0.8.0 is not compatible with 0.5.0
+
+Due to needing the implementation to be less bloated, teh structure was changed.
+There is now much less code and useless features were removed.
+
+Here is the gist:
+
+- The API has been slimmed down
+    - Almost no "hacked" attributes
+        - Only the `context` is "injected" into rules when processing
+        - Context contains `mule`, `rules`, `storage` and `backend`
+    - Record has had its `result` property removed
+    - Record has been simplified
+    - Everything is now optionally a context manager
+        - Allows easy initialization and de-initialization
+        - Storage, Mule and Backend are entered together
+        - Rules are entered once per scan
+    - Rules were reworked to be simple callables
+        - New signature `__call__(Record, Result) -> None`
+        - Scan result is now explicitly given to the rule
+        - Result is modified by the rule and nothing is returned to reduce complexity
+        - Removed rule priority
+            - Now simply respects insertion order
+        - Added batch rules
+            - Signature `__call__(List[Record], Result) -> None`
+            - Batches are run at the end of processing
+        - Added ANY matching rules
+            - Will get called using all produced records
+            - Note: Only record types with active rules are scanned
+        - Created additional built-in rule types
+        - Storage was slimmed down
+            - Now a storage simply has `store` and `fetch`
+            - Additional storage types for databses
+        - Backends were simplified
+            - Added some utility backends
+- Redesigned the YAML loader and Plugin handling
+    - Now there is no hacky loading going on
+    - Plugins are implicit and do no hooking
+    - Plugins only extend rule, storage and backend type scan options
+- Example server was removed completely
+    - Did not have time to rewrite it yet
+    - Nearly useless without search
+- Adds a command line runner for rules (WIP)
 
 ## Installation
 
 ```shell
 pip install dnsmule[full] dnsmule_plugins[full]
 ```
 
 This will install everything available for DNSMule. You can also choose to install components as necessary.
 
 For installing from the repo you can use:
 
 ```shell
-pip install -e .
+pip install -e . ./plugins
 ```
 
 ## Overview
 
-The DNSMule tool is composed in the following way:
+The DNSMule tool takes YAML config as input and uses it to scan a domain:
+
+```shell
+python -m dnsmule --config rules/rules.yml example.com
+```
+
+This will give output like:
 
-- DNSMule
-    - Backend
-    - Rules
-        - Rule
-    - Plugins
+````json
+{
+  "name": "example.com",
+  "types": [
+    "TXT",
+    "A"
+  ],
+  "tags": [],
+  "data": {}
+}
+````
 
 ## Examples
 
-Check out the examples in the [examples](examples) folder. They should get you up and running quickly.
+Check out the examples in the [examples](examples) folder.
+They should get you up and running quickly.
+The examples show some of the features available in DNSMule.
 
 ## YAML Configuration
 
 ### Summary
 
 The tool configuration is done through one or multiple rule configuration files. The file structure is defined in the
 [schema file](rules/rules-schema.yml). In addition to some builtin rule types, it is possible to create new types by
 registering handlers or rules programmatically.
 
-Rules support registration per DNS record type and priority for controlling invocation order.
+Rules support registration per DNS record type, as well as batch or any types:
 
 ```yaml
-version: '0.0.1'
-rules:
-  - name: o365
-    priority: 10
-    type: dns.regex
-    record: txt
-    config:
-      pattern: '^MS=ms'
-      identification: MICROSOFT::O365
-  - name: ses
-    type: dns.regex
-    record: txt
-    config:
-      pattern: '^amazonses:'
-      identification: AMAZON::SES
-```
-
-#### Example
-
-```python
-from dnsmule.definitions import Record, Result
-from dnsmule.rules import Rules, Rule
-
-rules: Rules
-
-...
-
-
-@rules.add.A[10]
-def my_scan(record: Record) -> Result:
-    from dnsmule.logger import get_logger
-    get_logger().info('Address %s', record)
-    return record.tag('MY::SCAN')
-
-
-@rules.register('my.rule')
-def create_my_rule(**arguments) -> Rule:
-    ...
-```
-
-Here the `add` is used to directly register a new rule into the ruleset with a given priority. The `register` call
-creates a new handler for rules of type `my.rule`. Any future `my.rule` creations from YAML or code would be routed to
-this factory function.
-
-See the examples folder for more examples and how to use rules in code.
-
-### Plugins and Backends
+plugins:
+  - 'sample_module'
 
-#### Plugins
+storage:
+  type: 'dict'
+  config: { }
 
-It is possible to register plugins using the YAML file:
+backend:
+  type: 'data'
+  config:
+    'example.com':
+      - name: 'example.com'
+        type: 'A'
+        data: '127.0.0.1'
 
-```yaml
-plugins:
-  - name: dnsmule_plugins.CertCheckPlugin
+rules:
+  - name: 'Sample'
+    type: 'sample'
+    record: 'any'
+
+  - name: 'Match digits'
+    type: 'regex'
+    record: 'A'
     config:
-      callback: false
-```
-
-These are required to extend the `dnsmule.plugins.Plugin` class.
-Plugins are evaluated and initialized before rules.
-Any rules requiring a plugin should list their plugin in this block.
-Plugins are only initialized once and if a plugin already exists in the receiving DNSMule instance
-it will be ignored.
-
-#### Backends
+      name: 'TEST'
+      regex: '\d+'
+      label: 'label'
+
+  - name: 'Add timestamp'
+    type: 'timestamp'
+    record: 'batch'
+
+  - name: 'Mark as test'
+    type: 'dynamic'
+    record: 'any'
+    config:
+      code: |
+        from dnsmule.utils import extend_set
 
-It is possible to define a single backend in a YAML file:
 
-```yaml
-backend:
-  name: 'dnspython.DNSPythonBackend'
-  config:
-    timeout: 5.5
-    resolver: 8.8.8.8
+        def process(record: Record, result: Result):
+            result.data['test'] = True
 ```
 
-The backend must extend the `dnsmule.backends.Backend` class.
-This declaration is ignored if this is not used in `DNSMule.load` or `DNSMule(file=file)`.
-
 ## Editor Support
 
 #### Type Hints and JSON Schema (IntelliJ IDEA, PyCharm, etc.)
 
 It is possible to register the schema file as a custom JSON schema in IntelliJ editors.
 This will give access to typehints and schema validation inside rule files and is especially nice for dynamic rule
 definitions as you get full editor features for python inside the snippets.
@@ -171,123 +202,48 @@
     check the schema for more info
   suffix: ''
 ```
 
 Currently, this supports `dns.regex` pattern regex language injection and `dns.dynamic` rule code language injection.
 Type hints and quick documentation are available.
 
-## Builtin Rules
-
-#### Regex rules
-
-Regex rules can be defined with either one `pattern` or multiple `patterns`.
-An example is in the following snippet:
-
-```yml
-rules:
-  - name: test
-    type: dns.regex
-    record: txt
-    config:
-      pattern: '^.*\.hello_world\.'
-      identification: HELLO::WORLD
-      flags:
-        - UNICODE
-        - DOTALL
-  - name: generic_verification
-    type: dns.regex
-    record: txt
-    priority: 10
-    description: Generic Site Regex Collection
-    config:
-      patterns:
-        - '^(.+)(?:-(?:site|domain))?-verification='
-        - '^(.+)(?:site|domain)verification'
-        - '^(.+)_verify_'
-        - '^(\w+)-code:'
-      group: 1
-```
-
-The full definition and additional info is available from the schema file, examples, and code.
-
-#### Dynamic Rules
+## Dynamic Rules
 
 Dynamic rules are defined as code snippets with one or two methods
 
 An init method that is invoked once after creation
 
 ```python
 def init() -> None:
-    add_rule(...)
+    ...
 ```
 
 A process function that is invoked once for each record
 
 ```python
-def process(record: Record) -> Result:
-    add_rule(...)
-    return record.result()
-```
-
-Both of these functions have access to the following rule creation method:
-
-```python
-def add_rule(
-        record_type: Union[str, int, RRType],
-        rule_type: str,
-        name: str,
-        *,
-        priority: int = 0,
-        **options,
-) -> None:
-    """
-    :param record_type: Valid DNS record type as text, int, or type
-    :param rule_type:   Valid rule type factory e.g. dns.regex
-    :param name:        Name of the created rule
-    :param priority:    Priority for the created rule, default 0
-    :param options:     Any additional options for the rule factory
-    """
+def process(record: Record, result: Result) -> None:
+    ...
 ```
 
 The only globals passed to these methods are:
 
 - \_\_builtins\_\_
-- RRType, Record, Result, Domain, Tag, Config
+- RRType, Record, Result, Domain, Config
     - The Config contains the `config` property passed to the rule from YAML
-- add_rule
 - Any additional globals created by the code itself
 
 When the code is exec'd the result is inspected for:
 
-- init function without parameters
-- process function with a single parameter
+- init function
+- process function
 
 Some notes:
 
-- The init function is invoked exactly once.
-- The process function is invoked exactly once for every single Record.
-- Any rules created from the init method will be invoked for every suitable record.
-- Any rules created from the process method will be invoked for suitable records found after creation.
-- Creating DynamicRules from init or process is considered undefined behaviour and care should be taken
-    - The user should call init manually and include fail-safes for only calling it once
-    - The add_rule callback might not be available so you need to pass it manually to the rule
-
-## Other
-
-### Example server
-
-The repo has a `Dockerfile` for easily running the tool using an example server in Docker:
-
-```shell
-$ ./build-image
-$ ./run-server
-```
-
-### Notice
-
-This package is under active development.
+- The init function is invoked every time the rule context is entered
+    - Take note that this happens on every scan
+- The process function is invoked exactly once for a single Record
+- Any rules created from the init method will be invoked for every suitable record
 
-### Additional
+## Notice
 
-- RnD Scripts under [scripts](scripts)
-- Example server under [server](server)
-- Examples for coding under [examples](examples)
+This package is under development.
+Pull requests are welcome, but will only be accepted after 0.8.0 is complete and my thesis is done.
```

### Comparing `dnsmule-0.5.0/README.md` & `dnsmule-0.8.0rc1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,135 +1,157 @@
 # DNSMule
 
 [![codecov](https://codecov.io/gh/joniumGit/dnsmule/branch/master/graph/badge.svg?token=54DPREJIFU)](https://codecov.io/gh/joniumGit/dnsmule)
 
 Package for rule based dependency scanning and service fingerprinting via DNS.
 
-This package provides utilities for writing and evaluating verbose and easy to read rule definitions in _YAML_-format.
-There are two builtin rule formats with more available as plugins.
+This package provides utilities for writing and evaluating verbose and easy to read rule definitions in YAML-format.
+There some builtin rule formats with more available as plugins.
+
+## Note: 0.8.0 is not compatible with 0.5.0
+
+Due to needing the implementation to be less bloated, teh structure was changed.
+There is now much less code and useless features were removed.
+
+Here is the gist:
+
+- The API has been slimmed down
+    - Almost no "hacked" attributes
+        - Only the `context` is "injected" into rules when processing
+        - Context contains `mule`, `rules`, `storage` and `backend`
+    - Record has had its `result` property removed
+    - Record has been simplified
+    - Everything is now optionally a context manager
+        - Allows easy initialization and de-initialization
+        - Storage, Mule and Backend are entered together
+        - Rules are entered once per scan
+    - Rules were reworked to be simple callables
+        - New signature `__call__(Record, Result) -> None`
+        - Scan result is now explicitly given to the rule
+        - Result is modified by the rule and nothing is returned to reduce complexity
+        - Removed rule priority
+            - Now simply respects insertion order
+        - Added batch rules
+            - Signature `__call__(List[Record], Result) -> None`
+            - Batches are run at the end of processing
+        - Added ANY matching rules
+            - Will get called using all produced records
+            - Note: Only record types with active rules are scanned
+        - Created additional built-in rule types
+        - Storage was slimmed down
+            - Now a storage simply has `store` and `fetch`
+            - Additional storage types for databses
+        - Backends were simplified
+            - Added some utility backends
+- Redesigned the YAML loader and Plugin handling
+    - Now there is no hacky loading going on
+    - Plugins are implicit and do no hooking
+    - Plugins only extend rule, storage and backend type scan options
+- Example server was removed completely
+    - Did not have time to rewrite it yet
+    - Nearly useless without search
+- Adds a command line runner for rules (WIP)
 
 ## Installation
 
 ```shell
 pip install dnsmule[full] dnsmule_plugins[full]
 ```
 
 This will install everything available for DNSMule. You can also choose to install components as necessary.
 
 For installing from the repo you can use:
 
 ```shell
-pip install -e .
+pip install -e . ./plugins
 ```
 
 ## Overview
 
-The DNSMule tool is composed in the following way:
+The DNSMule tool takes YAML config as input and uses it to scan a domain:
+
+```shell
+python -m dnsmule --config rules/rules.yml example.com
+```
 
-- DNSMule
-    - Backend
-    - Rules
-        - Rule
-    - Plugins
+This will give output like:
+
+````json
+{
+  "name": "example.com",
+  "types": [
+    "TXT",
+    "A"
+  ],
+  "tags": [],
+  "data": {}
+}
+````
 
 ## Examples
 
-Check out the examples in the [examples](examples) folder. They should get you up and running quickly.
+Check out the examples in the [examples](examples) folder.
+They should get you up and running quickly.
+The examples show some of the features available in DNSMule.
 
 ## YAML Configuration
 
 ### Summary
 
 The tool configuration is done through one or multiple rule configuration files. The file structure is defined in the
 [schema file](rules/rules-schema.yml). In addition to some builtin rule types, it is possible to create new types by
 registering handlers or rules programmatically.
 
-Rules support registration per DNS record type and priority for controlling invocation order.
+Rules support registration per DNS record type, as well as batch or any types:
 
 ```yaml
-version: '0.0.1'
-rules:
-  - name: o365
-    priority: 10
-    type: dns.regex
-    record: txt
-    config:
-      pattern: '^MS=ms'
-      identification: MICROSOFT::O365
-  - name: ses
-    type: dns.regex
-    record: txt
-    config:
-      pattern: '^amazonses:'
-      identification: AMAZON::SES
-```
-
-#### Example
-
-```python
-from dnsmule.definitions import Record, Result
-from dnsmule.rules import Rules, Rule
-
-rules: Rules
-
-...
-
-
-@rules.add.A[10]
-def my_scan(record: Record) -> Result:
-    from dnsmule.logger import get_logger
-    get_logger().info('Address %s', record)
-    return record.tag('MY::SCAN')
-
-
-@rules.register('my.rule')
-def create_my_rule(**arguments) -> Rule:
-    ...
-```
-
-Here the `add` is used to directly register a new rule into the ruleset with a given priority. The `register` call
-creates a new handler for rules of type `my.rule`. Any future `my.rule` creations from YAML or code would be routed to
-this factory function.
-
-See the examples folder for more examples and how to use rules in code.
-
-### Plugins and Backends
+plugins:
+  - 'sample_module'
 
-#### Plugins
+storage:
+  type: 'dict'
+  config: { }
 
-It is possible to register plugins using the YAML file:
+backend:
+  type: 'data'
+  config:
+    'example.com':
+      - name: 'example.com'
+        type: 'A'
+        data: '127.0.0.1'
 
-```yaml
-plugins:
-  - name: dnsmule_plugins.CertCheckPlugin
+rules:
+  - name: 'Sample'
+    type: 'sample'
+    record: 'any'
+
+  - name: 'Match digits'
+    type: 'regex'
+    record: 'A'
     config:
-      callback: false
-```
-
-These are required to extend the `dnsmule.plugins.Plugin` class.
-Plugins are evaluated and initialized before rules.
-Any rules requiring a plugin should list their plugin in this block.
-Plugins are only initialized once and if a plugin already exists in the receiving DNSMule instance
-it will be ignored.
-
-#### Backends
+      name: 'TEST'
+      regex: '\d+'
+      label: 'label'
+
+  - name: 'Add timestamp'
+    type: 'timestamp'
+    record: 'batch'
+
+  - name: 'Mark as test'
+    type: 'dynamic'
+    record: 'any'
+    config:
+      code: |
+        from dnsmule.utils import extend_set
 
-It is possible to define a single backend in a YAML file:
 
-```yaml
-backend:
-  name: 'dnspython.DNSPythonBackend'
-  config:
-    timeout: 5.5
-    resolver: 8.8.8.8
+        def process(record: Record, result: Result):
+            result.data['test'] = True
 ```
 
-The backend must extend the `dnsmule.backends.Backend` class.
-This declaration is ignored if this is not used in `DNSMule.load` or `DNSMule(file=file)`.
-
 ## Editor Support
 
 #### Type Hints and JSON Schema (IntelliJ IDEA, PyCharm, etc.)
 
 It is possible to register the schema file as a custom JSON schema in IntelliJ editors.
 This will give access to typehints and schema validation inside rule files and is especially nice for dynamic rule
 definitions as you get full editor features for python inside the snippets.
@@ -148,123 +170,48 @@
     check the schema for more info
   suffix: ''
 ```
 
 Currently, this supports `dns.regex` pattern regex language injection and `dns.dynamic` rule code language injection.
 Type hints and quick documentation are available.
 
-## Builtin Rules
-
-#### Regex rules
-
-Regex rules can be defined with either one `pattern` or multiple `patterns`.
-An example is in the following snippet:
-
-```yml
-rules:
-  - name: test
-    type: dns.regex
-    record: txt
-    config:
-      pattern: '^.*\.hello_world\.'
-      identification: HELLO::WORLD
-      flags:
-        - UNICODE
-        - DOTALL
-  - name: generic_verification
-    type: dns.regex
-    record: txt
-    priority: 10
-    description: Generic Site Regex Collection
-    config:
-      patterns:
-        - '^(.+)(?:-(?:site|domain))?-verification='
-        - '^(.+)(?:site|domain)verification'
-        - '^(.+)_verify_'
-        - '^(\w+)-code:'
-      group: 1
-```
-
-The full definition and additional info is available from the schema file, examples, and code.
-
-#### Dynamic Rules
+## Dynamic Rules
 
 Dynamic rules are defined as code snippets with one or two methods
 
 An init method that is invoked once after creation
 
 ```python
 def init() -> None:
-    add_rule(...)
+    ...
 ```
 
 A process function that is invoked once for each record
 
 ```python
-def process(record: Record) -> Result:
-    add_rule(...)
-    return record.result()
-```
-
-Both of these functions have access to the following rule creation method:
-
-```python
-def add_rule(
-        record_type: Union[str, int, RRType],
-        rule_type: str,
-        name: str,
-        *,
-        priority: int = 0,
-        **options,
-) -> None:
-    """
-    :param record_type: Valid DNS record type as text, int, or type
-    :param rule_type:   Valid rule type factory e.g. dns.regex
-    :param name:        Name of the created rule
-    :param priority:    Priority for the created rule, default 0
-    :param options:     Any additional options for the rule factory
-    """
+def process(record: Record, result: Result) -> None:
+    ...
 ```
 
 The only globals passed to these methods are:
 
 - \_\_builtins\_\_
-- RRType, Record, Result, Domain, Tag, Config
+- RRType, Record, Result, Domain, Config
     - The Config contains the `config` property passed to the rule from YAML
-- add_rule
 - Any additional globals created by the code itself
 
 When the code is exec'd the result is inspected for:
 
-- init function without parameters
-- process function with a single parameter
+- init function
+- process function
 
 Some notes:
 
-- The init function is invoked exactly once.
-- The process function is invoked exactly once for every single Record.
-- Any rules created from the init method will be invoked for every suitable record.
-- Any rules created from the process method will be invoked for suitable records found after creation.
-- Creating DynamicRules from init or process is considered undefined behaviour and care should be taken
-    - The user should call init manually and include fail-safes for only calling it once
-    - The add_rule callback might not be available so you need to pass it manually to the rule
-
-## Other
-
-### Example server
-
-The repo has a `Dockerfile` for easily running the tool using an example server in Docker:
-
-```shell
-$ ./build-image
-$ ./run-server
-```
-
-### Notice
-
-This package is under active development.
+- The init function is invoked every time the rule context is entered
+    - Take note that this happens on every scan
+- The process function is invoked exactly once for a single Record
+- Any rules created from the init method will be invoked for every suitable record
 
-### Additional
+## Notice
 
-- RnD Scripts under [scripts](scripts)
-- Example server under [server](server)
-- Examples for coding under [examples](examples)
+This package is under development.
+Pull requests are welcome, but will only be accepted after 0.8.0 is complete and my thesis is done.
```

### Comparing `dnsmule-0.5.0/setup.py` & `dnsmule-0.8.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dnsmule-0.5.0/src/DNSMule.egg-info/PKG-INFO` & `dnsmule-0.8.0rc1/src/DNSMule.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnsmule
-Version: 0.5.0
+Version: 0.8.0rc1
 Summary: Rule based dependency scanning and service fingerprinting via DNS
 Home-page: https://github.com/joniumGit/dnsmule
 Author: joniumGit
 Author-email: 52005121+joniumGit@users.noreply.github.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/joniumGit/dnsmule/issues
 Project-URL: Source, https://github.com/joniumGit/dnsmule
@@ -13,146 +13,177 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyyaml
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: redis; extra == "dev"
+Requires-Dist: pymongo; extra == "dev"
+Requires-Dist: dnspython; extra == "dev"
 Provides-Extra: full
-License-File: LICENSE
+Requires-Dist: redis; extra == "full"
+Requires-Dist: pymongo; extra == "full"
+Requires-Dist: dnspython; extra == "full"
 
 # DNSMule
 
 [![codecov](https://codecov.io/gh/joniumGit/dnsmule/branch/master/graph/badge.svg?token=54DPREJIFU)](https://codecov.io/gh/joniumGit/dnsmule)
 
 Package for rule based dependency scanning and service fingerprinting via DNS.
 
-This package provides utilities for writing and evaluating verbose and easy to read rule definitions in _YAML_-format.
-There are two builtin rule formats with more available as plugins.
+This package provides utilities for writing and evaluating verbose and easy to read rule definitions in YAML-format.
+There some builtin rule formats with more available as plugins.
+
+## Note: 0.8.0 is not compatible with 0.5.0
+
+Due to needing the implementation to be less bloated, teh structure was changed.
+There is now much less code and useless features were removed.
+
+Here is the gist:
+
+- The API has been slimmed down
+    - Almost no "hacked" attributes
+        - Only the `context` is "injected" into rules when processing
+        - Context contains `mule`, `rules`, `storage` and `backend`
+    - Record has had its `result` property removed
+    - Record has been simplified
+    - Everything is now optionally a context manager
+        - Allows easy initialization and de-initialization
+        - Storage, Mule and Backend are entered together
+        - Rules are entered once per scan
+    - Rules were reworked to be simple callables
+        - New signature `__call__(Record, Result) -> None`
+        - Scan result is now explicitly given to the rule
+        - Result is modified by the rule and nothing is returned to reduce complexity
+        - Removed rule priority
+            - Now simply respects insertion order
+        - Added batch rules
+            - Signature `__call__(List[Record], Result) -> None`
+            - Batches are run at the end of processing
+        - Added ANY matching rules
+            - Will get called using all produced records
+            - Note: Only record types with active rules are scanned
+        - Created additional built-in rule types
+        - Storage was slimmed down
+            - Now a storage simply has `store` and `fetch`
+            - Additional storage types for databses
+        - Backends were simplified
+            - Added some utility backends
+- Redesigned the YAML loader and Plugin handling
+    - Now there is no hacky loading going on
+    - Plugins are implicit and do no hooking
+    - Plugins only extend rule, storage and backend type scan options
+- Example server was removed completely
+    - Did not have time to rewrite it yet
+    - Nearly useless without search
+- Adds a command line runner for rules (WIP)
 
 ## Installation
 
 ```shell
 pip install dnsmule[full] dnsmule_plugins[full]
 ```
 
 This will install everything available for DNSMule. You can also choose to install components as necessary.
 
 For installing from the repo you can use:
 
 ```shell
-pip install -e .
+pip install -e . ./plugins
 ```
 
 ## Overview
 
-The DNSMule tool is composed in the following way:
+The DNSMule tool takes YAML config as input and uses it to scan a domain:
+
+```shell
+python -m dnsmule --config rules/rules.yml example.com
+```
+
+This will give output like:
 
-- DNSMule
-    - Backend
-    - Rules
-        - Rule
-    - Plugins
+````json
+{
+  "name": "example.com",
+  "types": [
+    "TXT",
+    "A"
+  ],
+  "tags": [],
+  "data": {}
+}
+````
 
 ## Examples
 
-Check out the examples in the [examples](examples) folder. They should get you up and running quickly.
+Check out the examples in the [examples](examples) folder.
+They should get you up and running quickly.
+The examples show some of the features available in DNSMule.
 
 ## YAML Configuration
 
 ### Summary
 
 The tool configuration is done through one or multiple rule configuration files. The file structure is defined in the
 [schema file](rules/rules-schema.yml). In addition to some builtin rule types, it is possible to create new types by
 registering handlers or rules programmatically.
 
-Rules support registration per DNS record type and priority for controlling invocation order.
+Rules support registration per DNS record type, as well as batch or any types:
 
 ```yaml
-version: '0.0.1'
-rules:
-  - name: o365
-    priority: 10
-    type: dns.regex
-    record: txt
-    config:
-      pattern: '^MS=ms'
-      identification: MICROSOFT::O365
-  - name: ses
-    type: dns.regex
-    record: txt
-    config:
-      pattern: '^amazonses:'
-      identification: AMAZON::SES
-```
-
-#### Example
-
-```python
-from dnsmule.definitions import Record, Result
-from dnsmule.rules import Rules, Rule
-
-rules: Rules
-
-...
-
-
-@rules.add.A[10]
-def my_scan(record: Record) -> Result:
-    from dnsmule.logger import get_logger
-    get_logger().info('Address %s', record)
-    return record.tag('MY::SCAN')
-
-
-@rules.register('my.rule')
-def create_my_rule(**arguments) -> Rule:
-    ...
-```
-
-Here the `add` is used to directly register a new rule into the ruleset with a given priority. The `register` call
-creates a new handler for rules of type `my.rule`. Any future `my.rule` creations from YAML or code would be routed to
-this factory function.
-
-See the examples folder for more examples and how to use rules in code.
-
-### Plugins and Backends
+plugins:
+  - 'sample_module'
 
-#### Plugins
+storage:
+  type: 'dict'
+  config: { }
 
-It is possible to register plugins using the YAML file:
+backend:
+  type: 'data'
+  config:
+    'example.com':
+      - name: 'example.com'
+        type: 'A'
+        data: '127.0.0.1'
 
-```yaml
-plugins:
-  - name: dnsmule_plugins.CertCheckPlugin
+rules:
+  - name: 'Sample'
+    type: 'sample'
+    record: 'any'
+
+  - name: 'Match digits'
+    type: 'regex'
+    record: 'A'
     config:
-      callback: false
-```
-
-These are required to extend the `dnsmule.plugins.Plugin` class.
-Plugins are evaluated and initialized before rules.
-Any rules requiring a plugin should list their plugin in this block.
-Plugins are only initialized once and if a plugin already exists in the receiving DNSMule instance
-it will be ignored.
-
-#### Backends
+      name: 'TEST'
+      regex: '\d+'
+      label: 'label'
+
+  - name: 'Add timestamp'
+    type: 'timestamp'
+    record: 'batch'
+
+  - name: 'Mark as test'
+    type: 'dynamic'
+    record: 'any'
+    config:
+      code: |
+        from dnsmule.utils import extend_set
 
-It is possible to define a single backend in a YAML file:
 
-```yaml
-backend:
-  name: 'dnspython.DNSPythonBackend'
-  config:
-    timeout: 5.5
-    resolver: 8.8.8.8
+        def process(record: Record, result: Result):
+            result.data['test'] = True
 ```
 
-The backend must extend the `dnsmule.backends.Backend` class.
-This declaration is ignored if this is not used in `DNSMule.load` or `DNSMule(file=file)`.
-
 ## Editor Support
 
 #### Type Hints and JSON Schema (IntelliJ IDEA, PyCharm, etc.)
 
 It is possible to register the schema file as a custom JSON schema in IntelliJ editors.
 This will give access to typehints and schema validation inside rule files and is especially nice for dynamic rule
 definitions as you get full editor features for python inside the snippets.
@@ -171,123 +202,48 @@
     check the schema for more info
   suffix: ''
 ```
 
 Currently, this supports `dns.regex` pattern regex language injection and `dns.dynamic` rule code language injection.
 Type hints and quick documentation are available.
 
-## Builtin Rules
-
-#### Regex rules
-
-Regex rules can be defined with either one `pattern` or multiple `patterns`.
-An example is in the following snippet:
-
-```yml
-rules:
-  - name: test
-    type: dns.regex
-    record: txt
-    config:
-      pattern: '^.*\.hello_world\.'
-      identification: HELLO::WORLD
-      flags:
-        - UNICODE
-        - DOTALL
-  - name: generic_verification
-    type: dns.regex
-    record: txt
-    priority: 10
-    description: Generic Site Regex Collection
-    config:
-      patterns:
-        - '^(.+)(?:-(?:site|domain))?-verification='
-        - '^(.+)(?:site|domain)verification'
-        - '^(.+)_verify_'
-        - '^(\w+)-code:'
-      group: 1
-```
-
-The full definition and additional info is available from the schema file, examples, and code.
-
-#### Dynamic Rules
+## Dynamic Rules
 
 Dynamic rules are defined as code snippets with one or two methods
 
 An init method that is invoked once after creation
 
 ```python
 def init() -> None:
-    add_rule(...)
+    ...
 ```
 
 A process function that is invoked once for each record
 
 ```python
-def process(record: Record) -> Result:
-    add_rule(...)
-    return record.result()
-```
-
-Both of these functions have access to the following rule creation method:
-
-```python
-def add_rule(
-        record_type: Union[str, int, RRType],
-        rule_type: str,
-        name: str,
-        *,
-        priority: int = 0,
-        **options,
-) -> None:
-    """
-    :param record_type: Valid DNS record type as text, int, or type
-    :param rule_type:   Valid rule type factory e.g. dns.regex
-    :param name:        Name of the created rule
-    :param priority:    Priority for the created rule, default 0
-    :param options:     Any additional options for the rule factory
-    """
+def process(record: Record, result: Result) -> None:
+    ...
 ```
 
 The only globals passed to these methods are:
 
 - \_\_builtins\_\_
-- RRType, Record, Result, Domain, Tag, Config
+- RRType, Record, Result, Domain, Config
     - The Config contains the `config` property passed to the rule from YAML
-- add_rule
 - Any additional globals created by the code itself
 
 When the code is exec'd the result is inspected for:
 
-- init function without parameters
-- process function with a single parameter
+- init function
+- process function
 
 Some notes:
 
-- The init function is invoked exactly once.
-- The process function is invoked exactly once for every single Record.
-- Any rules created from the init method will be invoked for every suitable record.
-- Any rules created from the process method will be invoked for suitable records found after creation.
-- Creating DynamicRules from init or process is considered undefined behaviour and care should be taken
-    - The user should call init manually and include fail-safes for only calling it once
-    - The add_rule callback might not be available so you need to pass it manually to the rule
-
-## Other
-
-### Example server
-
-The repo has a `Dockerfile` for easily running the tool using an example server in Docker:
-
-```shell
-$ ./build-image
-$ ./run-server
-```
-
-### Notice
-
-This package is under active development.
+- The init function is invoked every time the rule context is entered
+    - Take note that this happens on every scan
+- The process function is invoked exactly once for a single Record
+- Any rules created from the init method will be invoked for every suitable record
 
-### Additional
+## Notice
 
-- RnD Scripts under [scripts](scripts)
-- Example server under [server](server)
-- Examples for coding under [examples](examples)
+This package is under development.
+Pull requests are welcome, but will only be accepted after 0.8.0 is complete and my thesis is done.
```

### Comparing `dnsmule-0.5.0/src/dnsmule/backends/dnspython.py` & `dnsmule-0.8.0rc1/src/dnsmule/backends/dnspython.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-from os import getenv
-from random import choice
+from logging import getLogger
 from typing import Dict, Any, Callable, Coroutine, Iterable
 
 from dns.exception import DNSException
 from dns.message import Message, make_query
 from dns.query import udp_with_fallback, https, quic, udp, tcp, tls
 from dns.rdata import Rdata
 from dns.rdatatype import RdataType
+from dns.resolver import Resolver
 from dns.rrset import RRset
 
-from .abstract import Backend
-from ..definitions import Record, RRType, Domain
-from ..logger import get_logger
+from ..api import Backend, Record, Domain, RRType
 
-Querier = Callable[..., Coroutine[Any, Any, Message]]
+LOGGER = 'dnsmule.backends.dnspython'
 
 
 def default_query(query: Message, *args, **kwargs):
     response, used_tcp = udp_with_fallback(query, *args, **kwargs)
     if used_tcp:
-        get_logger().debug('Used TCP fallback query\n%s', query)
+        getLogger(LOGGER).debug('Used TCP fallback query\n%s', query)
     return response
 
 
 def message_to_record(message: Message) -> Iterable[Record]:
     result_set: RRset
     record_data: Rdata
     from itertools import chain
     for result_set in chain(message.answer, message.additional):
         for record_data in result_set:
             rtype = RRType.from_any(record_data.rdtype)
             yield DNSPythonRecord(
                 type=rtype,
-                domain=Domain(result_set.name.to_text(omit_final_dot=True)),
+                name=Domain(result_set.name.to_text(omit_final_dot=True)),
                 data=record_data,
             )
 
 
 class DNSPythonRecord(Record):
     data: Rdata
 
@@ -44,63 +42,73 @@
     def text(self) -> str:
         return self.data.to_text().removeprefix('"').removesuffix('"')
 
     def __getattr__(self, item):
         return getattr(self.data, item)
 
 
+Querier = Callable[..., Coroutine[Any, Any, Message]]
+
+
 class DNSPythonBackend(Backend):
+    """
+    DNSPython backend for querying DNS records
+
+    Can be configured with::
+
+        timeout     <int>   Timeout for queries
+        querier     <str>   Querier to use (see DNSPython docs for all query types)
+                            This is a `dns.query` attribute.
+                            Default: tcp with udp fallback
+        resolver    <str>   Resolver address to use for DNS queries
+                            Default: System default from `Resolver().nameservers[0]`
+    """
+    type = 'dnspython'
+
     _SUPPORTED_QUERY_TYPES: Dict[str, Querier] = {
         'tcp': tcp,
         'udp': udp,
         'tls': tls,
         'quic': quic,
         'https': https,
         'default': default_query,
     }
 
-    _DEFAULT_RESOLVER = getenv('DNSMULE_DEFAULT_RESOLVER', choice([
-        '208.67.222.222',
-        '208.67.220.220',
-        '1.1.1.1',
-        '1.0.0.1',
-        '8.8.8.8',
-        '8.8.4.4',
-    ]))
-
-    timeout: float = 2
-    querier: str = 'default'
-    resolver: str = _DEFAULT_RESOLVER
-
     _querier: Querier
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(
+            self,
+            *,
+            timeout: float = 2,
+            querier: str = 'default',
+            resolver: str = None,
+    ):
+        super(DNSPythonBackend, self).__init__()
+        self.timeout = timeout
+        self.querier = querier
+        self.resolver = resolver
+        self._logger = getLogger(LOGGER)
         try:
             self._querier = DNSPythonBackend._SUPPORTED_QUERY_TYPES[self.querier]
         except KeyError:
             raise ValueError(f'Invalid query mode ({self.querier})')
-        get_logger().info('DNSPYTHON: Resolver: %s', self.resolver)
+        if not self.resolver:
+            self.resolver = Resolver().nameservers[0]
+        self._logger.debug('Resolver: %s', self.resolver)
 
     def _dns_query(
             self,
             host: str,
             *types: int,
     ) -> Iterable[Message]:
         for dns_type in types:
             query = make_query(host, RdataType.make(dns_type))
             try:
                 response = self._querier(query, self.resolver, timeout=self.timeout)
                 yield response
             except DNSException as e:
-                get_logger().error('%s\n%s', 'Failed query', query, exc_info=e)
+                self._logger.error('%s\n%s', 'Failed query', query, exc_info=e)
 
-    def _query(self, target: Domain, *types: RRType) -> Iterable[Record]:
+    def scan(self, target: Domain, *types: RRType) -> Iterable[Record]:
         for message in self._dns_query(target, *types):
             for record in message_to_record(message):
                 yield record
-
-
-__all__ = [
-    'DNSPythonBackend',
-    'DNSPythonRecord',
-]
```

### Comparing `dnsmule-0.5.0/src/dnsmule/definitions/rrtype.py` & `dnsmule-0.8.0rc1/src/dnsmule/rrtype.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,20 +363,20 @@
     ZONEMD: int = 63
     """
     Message Digest Over Zone Data
     """
 
     SVCB: int = 64
     """
-    General Purpose Service Binding
+    General-purpose service binding
     """
 
     HTTPS: int = 65
     """
-    Service Binding type for use with HTTP
+    SVCB-compatible type for use with HTTP
     """
 
     SPF: int = 99
     """
 
     """
 
@@ -486,14 +486,19 @@
     """
 
     AMTRELAY: int = 260
     """
     Automatic Multicast Tunneling Relay
     """
 
+    RESINFO: int = 261
+    """
+    Resolver Information as Key/Value Pairs
+    """
+
     TA: int = 32768
     """
     DNSSEC Trust Authorities
     """
 
     DLV: int = 32769
     """
```

### Comparing `dnsmule-0.5.0/src/dnsmule/utils/misc.py` & `dnsmule-0.8.0rc1/src/dnsmule/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 from pathlib import Path
-from typing import Union, Iterator, TypeVar, Any, Dict, Tuple, Iterable
+from typing import Union, TypeVar, Any, Dict, Tuple, Iterable
 
 K = TypeVar('K')
 V = TypeVar('V')
 R = TypeVar('R')
-T = TypeVar('T')
-
-
-def empty() -> Iterator[Any]:
-    """An empty iterable
-    """
-    return iter([])
 
 
 def join_values(a: Dict[K, V], b: Dict[K, R]) -> Iterable[Tuple[V, R]]:
     """Yields the values from two dicts for keys that are present in both
     """
     for k, v in a.items():
         if k in b:
@@ -27,15 +20,15 @@
 
 def txt_stripped(line):
     return line.strip()
 
 
 def load_data(file: Union[str, Path], limit: int = -1):
     """
-    Loads target data from either a .csv of .txt file
+    Loads target data from either a .csv or .txt file
 
     If the file is a .csv file it is assumed to be of the form:
 
     * index1,target1
     * index2,target2
 
     Otherwise, it is assumed to be a file of the form:
@@ -105,15 +98,15 @@
             a[k] = (*a[k], *b[k])
         elif isinstance(a[k], frozenset):
             a[k] = frozenset((*a[k], *b[k]))
         else:
             a[k] += b[k]
 
 
-def extend_set(data: Dict[str, Any], key: str, values: Iterable[Any]):
+def extend_set(data: Dict[str, Any], key: str, *values: Any):
     """
     Appends values to a list based set in a dictionary
 
     **Note:** This is inefficient as it uses list traversal to check duplicates
 
     **Note:** This also de-duplicates the existing collection
     """
@@ -122,14 +115,46 @@
         values = [*data[key], *values]
     for v in values:
         if v not in target:
             target.append(v)
     data[key] = target
 
 
+def extend_list(data: Dict[str, Any], key: str, *values: Any):
+    """
+    Appends values to a list in a dictionary
+    """
+    if key in data:
+        data[key] = [*data[key], *values]
+    else:
+        data[key] = [*values]
+
+
+def jsonize(value):
+    """
+    Jsonizes a couple of outliers in the standard collections
+
+    :param value: Anything
+    :return: Something hopefully JSON compatible
+    """
+    if isinstance(value, dict):
+        return {
+            k: jsonize(v)
+            for k, v in value.items()
+        }
+    elif isinstance(value, (list, tuple, set, frozenset)):
+        return [
+            jsonize(item)
+            for item in value
+        ]
+    else:
+        return value
+
+
 __all__ = [
     'load_data',
     'left_merge',
     'extend_set',
-    'empty',
+    'extend_list',
     'join_values',
+    'jsonize',
 ]
```

