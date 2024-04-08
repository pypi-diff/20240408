# Comparing `tmp/jsii-1.96.0.tar.gz` & `tmp/jsii-1.97.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsii-1.96.0.tar", last modified: Fri Mar 22 17:47:02 2024, max compression
+gzip compressed data, was "jsii-1.97.0.tar", last modified: Mon Apr  8 20:14:54 2024, max compression
```

## Comparing `jsii-1.96.0.tar` & `jsii-1.97.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:47:02.429356 jsii-1.96.0/
--rw-rw-r--   0 root         (0) root         (0)    11386 2024-03-22 17:24:20.000000 jsii-1.96.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       88 2024-03-22 17:24:20.000000 jsii-1.96.0/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)       77 2024-03-22 17:24:20.000000 jsii-1.96.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    79739 2024-03-22 17:47:02.429356 jsii-1.96.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    78518 2024-03-22 17:46:36.000000 jsii-1.96.0/README.md
--rw-rw-r--   0 root         (0) root         (0)      333 2024-03-22 17:24:20.000000 jsii-1.96.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-22 17:47:02.429356 jsii-1.96.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1754 2024-03-22 17:24:20.000000 jsii-1.96.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:47:02.421356 jsii-1.96.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:47:02.425356 jsii-1.96.0/src/jsii/
--rw-rw-r--   0 root         (0) root         (0)     1568 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      348 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/__meta__.py
--rw-rw-r--   0 root         (0) root         (0)      107 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/_compat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:47:02.425356 jsii-1.96.0/src/jsii/_embedded/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/_embedded/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:47:02.425356 jsii-1.96.0/src/jsii/_embedded/jsii/
--rw-r--r--   0 root         (0) root         (0)      302 2024-03-22 17:46:38.000000 jsii-1.96.0/src/jsii/_embedded/jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   158418 2024-03-22 17:46:38.000000 jsii-1.96.0/src/jsii/_embedded/jsii/bin__jsii-runtime.js
--rw-r--r--   0 root         (0) root         (0)   247388 2024-03-22 17:46:38.000000 jsii-1.96.0/src/jsii/_embedded/jsii/bin__jsii-runtime.js.map
--rw-r--r--   0 root         (0) root         (0)   831553 2024-03-22 17:46:38.000000 jsii-1.96.0/src/jsii/_embedded/jsii/lib__program.js
--rw-r--r--   0 root         (0) root         (0)  1203459 2024-03-22 17:46:38.000000 jsii-1.96.0/src/jsii/_embedded/jsii/lib__program.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:47:02.425356 jsii-1.96.0/src/jsii/_kernel/
--rw-rw-r--   0 root         (0) root         (0)    17033 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/_kernel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:47:02.429356 jsii-1.96.0/src/jsii/_kernel/providers/
--rw-rw-r--   0 root         (0) root         (0)      116 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/_kernel/providers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2795 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/_kernel/providers/base.py
--rw-rw-r--   0 root         (0) root         (0)    14427 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/_kernel/providers/process.py
--rw-rw-r--   0 root         (0) root         (0)     4892 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/_kernel/types.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-03-22 17:46:38.000000 jsii-1.96.0/src/jsii/_metadata.json
--rw-rw-r--   0 root         (0) root         (0)     7674 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/_reference_map.py
--rw-rw-r--   0 root         (0) root         (0)     5743 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/_runtime.py
--rw-rw-r--   0 root         (0) root         (0)      584 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/_utils.py
--rw-rw-r--   0 root         (0) root         (0)       96 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/compat.py
--rw-rw-r--   0 root         (0) root         (0)      387 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/errors.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/py.typed
--rw-rw-r--   0 root         (0) root         (0)     1497 2024-03-22 17:24:20.000000 jsii-1.96.0/src/jsii/python.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:47:02.429356 jsii-1.96.0/src/jsii.egg-info/
--rw-r--r--   0 root         (0) root         (0)    79739 2024-03-22 17:47:02.000000 jsii-1.96.0/src/jsii.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      966 2024-03-22 17:47:02.000000 jsii-1.96.0/src/jsii.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-22 17:47:02.000000 jsii-1.96.0/src/jsii.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      144 2024-03-22 17:47:02.000000 jsii-1.96.0/src/jsii.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-22 17:47:02.000000 jsii-1.96.0/src/jsii.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:47:02.429356 jsii-1.96.0/tests/
--rw-rw-r--   0 root         (0) root         (0)    38968 2024-03-22 17:24:20.000000 jsii-1.96.0/tests/test_compliance.py
--rw-rw-r--   0 root         (0) root         (0)     4065 2024-03-22 17:24:20.000000 jsii-1.96.0/tests/test_invoke_bin.py
--rw-rw-r--   0 root         (0) root         (0)     2316 2024-03-22 17:24:20.000000 jsii-1.96.0/tests/test_python.py
--rw-rw-r--   0 root         (0) root         (0)     8410 2024-03-22 17:24:20.000000 jsii-1.96.0/tests/test_runtime_type_checking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:14:54.633726 jsii-1.97.0/
+-rw-rw-r--   0 root         (0) root         (0)    11386 2024-04-08 19:51:20.000000 jsii-1.97.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       88 2024-04-08 19:51:20.000000 jsii-1.97.0/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)       77 2024-04-08 19:51:20.000000 jsii-1.97.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    79739 2024-04-08 20:14:54.633726 jsii-1.97.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    78518 2024-04-08 20:14:27.000000 jsii-1.97.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)      333 2024-04-08 19:51:20.000000 jsii-1.97.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 20:14:54.633726 jsii-1.97.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1754 2024-04-08 19:51:20.000000 jsii-1.97.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:14:54.625726 jsii-1.97.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:14:54.625726 jsii-1.97.0/src/jsii/
+-rw-rw-r--   0 root         (0) root         (0)     1568 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      348 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/__meta__.py
+-rw-rw-r--   0 root         (0) root         (0)      107 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/_compat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:14:54.629726 jsii-1.97.0/src/jsii/_embedded/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/_embedded/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:14:54.629726 jsii-1.97.0/src/jsii/_embedded/jsii/
+-rw-r--r--   0 root         (0) root         (0)      302 2024-04-08 20:14:30.000000 jsii-1.97.0/src/jsii/_embedded/jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   158418 2024-04-08 20:14:30.000000 jsii-1.97.0/src/jsii/_embedded/jsii/bin__jsii-runtime.js
+-rw-r--r--   0 root         (0) root         (0)   247388 2024-04-08 20:14:30.000000 jsii-1.97.0/src/jsii/_embedded/jsii/bin__jsii-runtime.js.map
+-rw-r--r--   0 root         (0) root         (0)   831553 2024-04-08 20:14:30.000000 jsii-1.97.0/src/jsii/_embedded/jsii/lib__program.js
+-rw-r--r--   0 root         (0) root         (0)  1203459 2024-04-08 20:14:30.000000 jsii-1.97.0/src/jsii/_embedded/jsii/lib__program.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:14:54.629726 jsii-1.97.0/src/jsii/_kernel/
+-rw-rw-r--   0 root         (0) root         (0)    17033 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/_kernel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:14:54.629726 jsii-1.97.0/src/jsii/_kernel/providers/
+-rw-rw-r--   0 root         (0) root         (0)      116 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/_kernel/providers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2795 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/_kernel/providers/base.py
+-rw-rw-r--   0 root         (0) root         (0)    14427 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/_kernel/providers/process.py
+-rw-rw-r--   0 root         (0) root         (0)     4892 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/_kernel/types.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-08 20:14:30.000000 jsii-1.97.0/src/jsii/_metadata.json
+-rw-rw-r--   0 root         (0) root         (0)     7674 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/_reference_map.py
+-rw-rw-r--   0 root         (0) root         (0)     5743 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/_runtime.py
+-rw-rw-r--   0 root         (0) root         (0)      584 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/_utils.py
+-rw-rw-r--   0 root         (0) root         (0)       96 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/compat.py
+-rw-rw-r--   0 root         (0) root         (0)      387 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/errors.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/py.typed
+-rw-rw-r--   0 root         (0) root         (0)     1497 2024-04-08 19:51:20.000000 jsii-1.97.0/src/jsii/python.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:14:54.629726 jsii-1.97.0/src/jsii.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    79739 2024-04-08 20:14:54.000000 jsii-1.97.0/src/jsii.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      966 2024-04-08 20:14:54.000000 jsii-1.97.0/src/jsii.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 20:14:54.000000 jsii-1.97.0/src/jsii.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      144 2024-04-08 20:14:54.000000 jsii-1.97.0/src/jsii.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-08 20:14:54.000000 jsii-1.97.0/src/jsii.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 20:14:54.629726 jsii-1.97.0/tests/
+-rw-rw-r--   0 root         (0) root         (0)    38968 2024-04-08 19:51:20.000000 jsii-1.97.0/tests/test_compliance.py
+-rw-rw-r--   0 root         (0) root         (0)     4065 2024-04-08 19:51:20.000000 jsii-1.97.0/tests/test_invoke_bin.py
+-rw-rw-r--   0 root         (0) root         (0)     2316 2024-04-08 19:51:20.000000 jsii-1.97.0/tests/test_python.py
+-rw-rw-r--   0 root         (0) root         (0)     8410 2024-04-08 19:51:20.000000 jsii-1.97.0/tests/test_runtime_type_checking.py
```

### Comparing `jsii-1.96.0/LICENSE` & `jsii-1.97.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/PKG-INFO` & `jsii-1.97.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsii
-Version: 1.96.0
+Version: 1.97.0
 Summary: Python client for jsii runtime
 Home-page: https://github.com/aws/jsii
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/aws/jsii
 Project-URL: Source, https://github.com/aws/jsii.git
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jsii-1.96.0/README.md` & `jsii-1.97.0/README.md`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/setup.py` & `jsii-1.97.0/setup.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/__init__.py` & `jsii-1.97.0/src/jsii/__init__.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/_embedded/jsii/bin__jsii-runtime.js` & `jsii-1.97.0/src/jsii/_embedded/jsii/bin__jsii-runtime.js`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/_embedded/jsii/bin__jsii-runtime.js.map` & `jsii-1.97.0/src/jsii/_embedded/jsii/bin__jsii-runtime.js.map`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/_embedded/jsii/lib__program.js` & `jsii-1.97.0/src/jsii/_embedded/jsii/lib__program.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -19091,15 +19091,15 @@
     },
     9796: module => {
         "use strict";
         module.exports = require("zlib");
     },
     4147: module => {
         "use strict";
-        module.exports = JSON.parse('{"name":"@jsii/runtime","version":"1.96.0","description":"jsii runtime kernel process","license":"Apache-2.0","author":{"name":"Amazon Web Services","url":"https://aws.amazon.com"},"homepage":"https://github.com/aws/jsii","bugs":{"url":"https://github.com/aws/jsii/issues"},"repository":{"type":"git","url":"https://github.com/aws/jsii.git","directory":"packages/@jsii/runtime"},"engines":{"node":">= 14.17.0"},"main":"lib/index.js","types":"lib/index.d.ts","bin":{"jsii-runtime":"bin/jsii-runtime"},"scripts":{"build":"tsc --build && chmod +x bin/jsii-runtime && npx webpack-cli && npm run lint","watch":"tsc --build -w","lint":"eslint . --ext .js,.ts --ignore-path=.gitignore --ignore-pattern=webpack.config.js","lint:fix":"yarn lint --fix","test":"jest","test:update":"jest -u","package":"package-js"},"dependencies":{"@jsii/kernel":"^1.96.0","@jsii/check-node":"1.96.0","@jsii/spec":"^1.96.0"},"devDependencies":{"@scope/jsii-calc-base":"^1.96.0","@scope/jsii-calc-lib":"^1.96.0","jsii-build-tools":"^1.96.0","jsii-calc":"^3.20.120","source-map-loader":"^4.0.1","webpack":"^5.89.0","webpack-cli":"^5.1.4"}}');
+        module.exports = JSON.parse('{"name":"@jsii/runtime","version":"1.97.0","description":"jsii runtime kernel process","license":"Apache-2.0","author":{"name":"Amazon Web Services","url":"https://aws.amazon.com"},"homepage":"https://github.com/aws/jsii","bugs":{"url":"https://github.com/aws/jsii/issues"},"repository":{"type":"git","url":"https://github.com/aws/jsii.git","directory":"packages/@jsii/runtime"},"engines":{"node":">= 14.17.0"},"main":"lib/index.js","types":"lib/index.d.ts","bin":{"jsii-runtime":"bin/jsii-runtime"},"scripts":{"build":"tsc --build && chmod +x bin/jsii-runtime && npx webpack-cli && npm run lint","watch":"tsc --build -w","lint":"eslint . --ext .js,.ts --ignore-path=.gitignore --ignore-pattern=webpack.config.js","lint:fix":"yarn lint --fix","test":"jest","test:update":"jest -u","package":"package-js"},"dependencies":{"@jsii/kernel":"^1.97.0","@jsii/check-node":"1.97.0","@jsii/spec":"^1.97.0"},"devDependencies":{"@scope/jsii-calc-base":"^1.97.0","@scope/jsii-calc-lib":"^1.97.0","jsii-build-tools":"^1.97.0","jsii-calc":"^3.20.120","source-map-loader":"^4.0.1","webpack":"^5.89.0","webpack-cli":"^5.1.4"}}');
     },
     5277: module => {
         "use strict";
         module.exports = JSON.parse('{"$id":"https://raw.githubusercontent.com/ajv-validator/ajv/master/lib/refs/data.json#","description":"Meta-schema for $data reference (JSON AnySchema extension proposal)","type":"object","required":["$data"],"properties":{"$data":{"type":"string","anyOf":[{"format":"relative-json-pointer"},{"format":"json-pointer"}]}},"additionalProperties":false}');
     },
     7538: module => {
         "use strict";
```

### Comparing `jsii-1.96.0/src/jsii/_embedded/jsii/lib__program.js.map` & `jsii-1.97.0/src/jsii/_embedded/jsii/lib__program.js.map`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/_kernel/__init__.py` & `jsii-1.97.0/src/jsii/_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/_kernel/providers/base.py` & `jsii-1.97.0/src/jsii/_kernel/providers/base.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/_kernel/providers/process.py` & `jsii-1.97.0/src/jsii/_kernel/providers/process.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/_kernel/types.py` & `jsii-1.97.0/src/jsii/_kernel/types.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/_reference_map.py` & `jsii-1.97.0/src/jsii/_reference_map.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/_runtime.py` & `jsii-1.97.0/src/jsii/_runtime.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/_utils.py` & `jsii-1.97.0/src/jsii/_utils.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii/python.py` & `jsii-1.97.0/src/jsii/python.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/src/jsii.egg-info/PKG-INFO` & `jsii-1.97.0/src/jsii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsii
-Version: 1.96.0
+Version: 1.97.0
 Summary: Python client for jsii runtime
 Home-page: https://github.com/aws/jsii
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/aws/jsii
 Project-URL: Source, https://github.com/aws/jsii.git
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jsii-1.96.0/src/jsii.egg-info/SOURCES.txt` & `jsii-1.97.0/src/jsii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/tests/test_compliance.py` & `jsii-1.97.0/tests/test_compliance.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/tests/test_invoke_bin.py` & `jsii-1.97.0/tests/test_invoke_bin.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/tests/test_python.py` & `jsii-1.97.0/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `jsii-1.96.0/tests/test_runtime_type_checking.py` & `jsii-1.97.0/tests/test_runtime_type_checking.py`

 * *Files identical despite different names*

