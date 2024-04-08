# Comparing `tmp/aup_manager-2.0.4.tar.gz` & `tmp/aup_manager-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aup_manager-2.0.4.tar", last modified: Fri Jan 26 17:21:01 2024, max compression
+gzip compressed data, was "aup_manager-2.0.5.tar", last modified: Mon Apr  8 08:30:18 2024, max compression
```

## Comparing `aup_manager-2.0.4.tar` & `aup_manager-2.0.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0     1001 root         (0)        0 2024-01-26 17:21:01.189159 aup_manager-2.0.4/
--rw-rw-rw-   0     1001 root         (0)     1560 2024-01-26 17:20:40.000000 aup_manager-2.0.4/LICENSE
--rw-rw-rw-   0     1001 root         (0)       52 2024-01-26 17:20:40.000000 aup_manager-2.0.4/MANIFEST.in
--rw-r--r--   0     1001 root         (0)      568 2024-01-26 17:21:01.189159 aup_manager-2.0.4/PKG-INFO
--rw-rw-rw-   0     1001 root         (0)      507 2024-01-26 17:20:40.000000 aup_manager-2.0.4/README.md
-drwxr-xr-x   0     1001 root         (0)        0 2024-01-26 17:21:01.185159 aup_manager-2.0.4/aup_manager/
--rw-rw-rw-   0     1001 root         (0)      434 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/__init__.py
--rw-rw-rw-   0     1001 root         (0)     1479 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/config-template.yaml
-drwxr-xr-x   0     1001 root         (0)        0 2024-01-26 17:21:01.185159 aup_manager-2.0.4/aup_manager/connectors/
--rw-rw-rw-   0     1001 root         (0)     1577 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/connectors/ConnectorInterface.py
--rw-rw-rw-   0     1001 root         (0)     1785 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/connectors/MongodbConnector.py
--rw-rw-rw-   0     1001 root         (0)     4490 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/connectors/PerunConnector.py
--rw-rw-rw-   0     1001 root         (0)      279 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/connectors/__init__.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-01-26 17:21:01.185159 aup_manager-2.0.4/aup_manager/db/
--rw-rw-rw-   0     1001 root         (0)     7305 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/db/DatabaseInterface.py
--rw-rw-rw-   0     1001 root         (0)    11887 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/db/MongodbDatabase.py
--rw-rw-rw-   0     1001 root         (0)      174 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/db/__init__.py
--rw-rw-rw-   0     1001 root         (0)    15911 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/flask_app.py
--rw-rw-rw-   0     1001 root         (0)     2937 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/models.py
--rw-rw-rw-   0     1001 root         (0)     4026 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/openapi-specification.yaml
-drwxr-xr-x   0     1001 root         (0)        0 2024-01-26 17:21:01.185159 aup_manager-2.0.4/aup_manager/static/
-drwxr-xr-x   0     1001 root         (0)        0 2024-01-26 17:21:01.185159 aup_manager-2.0.4/aup_manager/static/assets/
--rw-rw-rw-   0     1001 root         (0)      405 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/static/assets/caret-down-solid.svg
--rw-rw-rw-   0     1001 root         (0)    26084 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/static/index.js
--rw-rw-rw-   0     1001 root         (0)    21738 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/static/package-lock.json
--rw-rw-rw-   0     1001 root         (0)      498 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/static/package.json
-drwxr-xr-x   0     1001 root         (0)        0 2024-01-26 17:21:01.185159 aup_manager-2.0.4/aup_manager/static/scss/
--rw-rw-rw-   0     1001 root         (0)      166 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/static/scss/_stepper.scss
--rw-rw-rw-   0     1001 root         (0)      318 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/static/scss/custom.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-01-26 17:21:01.189159 aup_manager-2.0.4/aup_manager/templates/
--rw-rw-rw-   0     1001 root         (0)     2273 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/templates/accept_aups.html
--rw-rw-rw-   0     1001 root         (0)      823 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/templates/aup_overview.html
--rw-rw-rw-   0     1001 root         (0)      988 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/templates/base.html
--rw-rw-rw-   0     1001 root         (0)     5633 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/templates/create_aup.html
--rw-rw-rw-   0     1001 root         (0)      428 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/templates/login.html
--rw-rw-rw-   0     1001 root         (0)    11233 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/templates/manage_aups.html
--rw-rw-rw-   0     1001 root         (0)      224 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/templates/text_message.html
--rw-rw-rw-   0     1001 root         (0)      535 2024-01-26 17:20:40.000000 aup_manager-2.0.4/aup_manager/templates/unauthorized.html
-drwxr-xr-x   0     1001 root         (0)        0 2024-01-26 17:21:01.185159 aup_manager-2.0.4/aup_manager.egg-info/
--rw-r--r--   0     1001 root         (0)      568 2024-01-26 17:21:01.000000 aup_manager-2.0.4/aup_manager.egg-info/PKG-INFO
--rw-r--r--   0     1001 root         (0)     1145 2024-01-26 17:21:01.000000 aup_manager-2.0.4/aup_manager.egg-info/SOURCES.txt
--rw-r--r--   0     1001 root         (0)        1 2024-01-26 17:21:01.000000 aup_manager-2.0.4/aup_manager.egg-info/dependency_links.txt
--rw-r--r--   0     1001 root         (0)      159 2024-01-26 17:21:01.000000 aup_manager-2.0.4/aup_manager.egg-info/requires.txt
--rw-r--r--   0     1001 root         (0)       12 2024-01-26 17:21:01.000000 aup_manager-2.0.4/aup_manager.egg-info/top_level.txt
--rw-rw-rw-   0     1001 root         (0)       90 2024-01-26 17:21:01.189159 aup_manager-2.0.4/setup.cfg
--rw-rw-rw-   0     1001 root         (0)     1127 2024-01-26 17:20:40.000000 aup_manager-2.0.4/setup.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.662981 aup_manager-2.0.5/
+-rw-rw-rw-   0     1001 root         (0)     1560 2024-04-08 08:29:51.000000 aup_manager-2.0.5/LICENSE
+-rw-rw-rw-   0     1001 root         (0)       52 2024-04-08 08:29:51.000000 aup_manager-2.0.5/MANIFEST.in
+-rw-r--r--   0     1001 root         (0)      568 2024-04-08 08:30:18.662981 aup_manager-2.0.5/PKG-INFO
+-rw-rw-rw-   0     1001 root         (0)      507 2024-04-08 08:29:51.000000 aup_manager-2.0.5/README.md
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.654981 aup_manager-2.0.5/aup_manager/
+-rw-rw-rw-   0     1001 root         (0)      434 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     1479 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/config-template.yaml
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/connectors/
+-rw-rw-rw-   0     1001 root         (0)     1577 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/connectors/ConnectorInterface.py
+-rw-rw-rw-   0     1001 root         (0)     1785 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/connectors/MongodbConnector.py
+-rw-rw-rw-   0     1001 root         (0)     4490 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/connectors/PerunConnector.py
+-rw-rw-rw-   0     1001 root         (0)      279 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/connectors/__init__.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/db/
+-rw-rw-rw-   0     1001 root         (0)     7305 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/db/DatabaseInterface.py
+-rw-rw-rw-   0     1001 root         (0)    11887 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/db/MongodbDatabase.py
+-rw-rw-rw-   0     1001 root         (0)      174 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/db/__init__.py
+-rw-rw-rw-   0     1001 root         (0)    15944 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/flask_app.py
+-rw-rw-rw-   0     1001 root         (0)     2937 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/models.py
+-rw-rw-rw-   0     1001 root         (0)     4026 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/openapi-specification.yaml
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/static/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/static/assets/
+-rw-rw-rw-   0     1001 root         (0)      405 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/assets/caret-down-solid.svg
+-rw-rw-rw-   0     1001 root         (0)    26084 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/index.js
+-rw-rw-rw-   0     1001 root         (0)    21684 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/package-lock.json
+-rw-rw-rw-   0     1001 root         (0)      498 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/package.json
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/static/scss/
+-rw-rw-rw-   0     1001 root         (0)      166 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/scss/_stepper.scss
+-rw-rw-rw-   0     1001 root         (0)      318 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/scss/custom.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/templates/
+-rw-rw-rw-   0     1001 root         (0)     2273 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/accept_aups.html
+-rw-rw-rw-   0     1001 root         (0)      823 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/aup_overview.html
+-rw-rw-rw-   0     1001 root         (0)      988 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/base.html
+-rw-rw-rw-   0     1001 root         (0)     5633 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/create_aup.html
+-rw-rw-rw-   0     1001 root         (0)      428 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/login.html
+-rw-rw-rw-   0     1001 root         (0)    11233 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/manage_aups.html
+-rw-rw-rw-   0     1001 root         (0)      224 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/text_message.html
+-rw-rw-rw-   0     1001 root         (0)      535 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/unauthorized.html
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager.egg-info/
+-rw-r--r--   0     1001 root         (0)      568 2024-04-08 08:30:18.000000 aup_manager-2.0.5/aup_manager.egg-info/PKG-INFO
+-rw-r--r--   0     1001 root         (0)     1145 2024-04-08 08:30:18.000000 aup_manager-2.0.5/aup_manager.egg-info/SOURCES.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-04-08 08:30:18.000000 aup_manager-2.0.5/aup_manager.egg-info/dependency_links.txt
+-rw-r--r--   0     1001 root         (0)      159 2024-04-08 08:30:18.000000 aup_manager-2.0.5/aup_manager.egg-info/requires.txt
+-rw-r--r--   0     1001 root         (0)       12 2024-04-08 08:30:18.000000 aup_manager-2.0.5/aup_manager.egg-info/top_level.txt
+-rw-rw-rw-   0     1001 root         (0)       90 2024-04-08 08:30:18.662981 aup_manager-2.0.5/setup.cfg
+-rw-rw-rw-   0     1001 root         (0)     1127 2024-04-08 08:29:51.000000 aup_manager-2.0.5/setup.py
```

### Comparing `aup_manager-2.0.4/LICENSE` & `aup_manager-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/PKG-INFO` & `aup_manager-2.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aup_manager
-Version: 2.0.4
+Version: 2.0.5
 Summary: app for management of acceptable use policies with API for approving them
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/aup-manager.git
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: pymongo==4.6.1
 Requires-Dist: jsonpatch==1.33
```

### Comparing `aup_manager-2.0.4/aup_manager/config-template.yaml` & `aup_manager-2.0.5/aup_manager/config-template.yaml`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/connectors/ConnectorInterface.py` & `aup_manager-2.0.5/aup_manager/connectors/ConnectorInterface.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/connectors/MongodbConnector.py` & `aup_manager-2.0.5/aup_manager/connectors/MongodbConnector.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/connectors/PerunConnector.py` & `aup_manager-2.0.5/aup_manager/connectors/PerunConnector.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/db/DatabaseInterface.py` & `aup_manager-2.0.5/aup_manager/db/DatabaseInterface.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/db/MongodbDatabase.py` & `aup_manager-2.0.5/aup_manager/db/MongodbDatabase.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/flask_app.py` & `aup_manager-2.0.5/aup_manager/flask_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,18 @@
     nonce = session.pop("nonce", None)
     callback_url = session.pop("callback_url", None)
     aup_ids = session.pop("aup_ids", None)
     if not user_id or not nonce or not callback_url or not aup_ids:
         return Response(json.dumps({"fail": "Missing attribute in session."}), 400)
 
     internal_request = DATABASE.get_request_by_nonce(nonce)
-    if not request or internal_request.status != internal_request.status.FAILURE:
+    if (
+        not internal_request
+        or internal_request.status != internal_request.status.FAILURE
+    ):
         return Response(json.dumps({"fail": "Invalid nonce."}), 403)
     __save_acceptances(user_id, aup_ids)
     DATABASE.make_request_success(internal_request.get_id())
     return redirect(callback_url + "?" + parse.urlencode({"nonce": nonce}))
 
 
 @flask_app.route("/get_accept_result/<message>")
```

### Comparing `aup_manager-2.0.4/aup_manager/models.py` & `aup_manager-2.0.5/aup_manager/models.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/openapi-specification.yaml` & `aup_manager-2.0.5/aup_manager/openapi-specification.yaml`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/static/index.js` & `aup_manager-2.0.5/aup_manager/static/index.js`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/static/package-lock.json` & `aup_manager-2.0.5/aup_manager/static/package-lock.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996865889212828%*

 * *Differences: {"'packages'": "{'node_modules/browserslist': {'version': '4.23.0', 'resolved': "*

 * *               "'https://registry.npmjs.org/browserslist/-/browserslist-4.23.0.tgz', 'integrity': "*

 * *               "'sha512-QW8HiM1shhT2GuzkvklfjcKDiWFXHOeFCIA/huJPwHsslwcydgk7X+z2zXpEijP98UCY7HbubZt5J2Zgvf0CaQ==', "*

 * *               "'dependencies': {'caniuse-lite': '^1.0.30001587', 'electron-to-chromium': "*

 * *               "'^1.4.668'}}, 'node_modules/caniuse-lite': {'version': '1.0.30001591', 'resolved': "*

 * *               "'htt […]*

```diff
@@ -140,16 +140,16 @@
             "version": "3.0.2"
         },
         "node_modules/browserslist": {
             "bin": {
                 "browserslist": "cli.js"
             },
             "dependencies": {
-                "caniuse-lite": "^1.0.30001565",
-                "electron-to-chromium": "^1.4.601",
+                "caniuse-lite": "^1.0.30001587",
+                "electron-to-chromium": "^1.4.668",
                 "node-releases": "^2.0.14",
                 "update-browserslist-db": "^1.0.13"
             },
             "engines": {
                 "node": "^6 || ^7 || ^8 || ^9 || ^10 || ^11 || ^12 || >=13.7"
             },
             "funding": [
@@ -162,17 +162,17 @@
                     "url": "https://tidelift.com/funding/github/npm/browserslist"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-0UgcrvQmBDvZHFGdYUehrCNIazki7/lUP3kkoi/r3YB2amZbFM9J43ZRkJTXBUZK4gmx56+Sqk9+Vs9mwZx9+A==",
-            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.22.2.tgz",
-            "version": "4.22.2"
+            "integrity": "sha512-QW8HiM1shhT2GuzkvklfjcKDiWFXHOeFCIA/huJPwHsslwcydgk7X+z2zXpEijP98UCY7HbubZt5J2Zgvf0CaQ==",
+            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.23.0.tgz",
+            "version": "4.23.0"
         },
         "node_modules/caniuse-lite": {
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/browserslist"
                 },
@@ -181,17 +181,17 @@
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-u5AUVkixruKHJjw/pj9wISlcMpgFWzSrczLZbrqBSxukQixmg0SJ5sZTpvaFvxU0HoQKd4yoyAogyrAz9pzJnA==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001579.tgz",
-            "version": "1.0.30001579"
+            "integrity": "sha512-PCzRMei/vXjJyL5mJtzNiUCKP59dm8Apqc3PH8gJkMnMXZGox93RbE76jHsmLwmIo6/3nsYIpJtx0O7u5PqFuQ==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001591.tgz",
+            "version": "1.0.30001591"
         },
         "node_modules/chokidar": {
             "dependencies": {
                 "anymatch": "~3.1.2",
                 "braces": "~3.0.2",
                 "glob-parent": "~5.1.2",
                 "is-binary-path": "~2.1.0",
@@ -199,44 +199,41 @@
                 "normalize-path": "~3.0.0",
                 "readdirp": "~3.6.0"
             },
             "dev": true,
             "engines": {
                 "node": ">= 8.10.0"
             },
-            "funding": [
-                {
-                    "type": "individual",
-                    "url": "https://paulmillr.com/funding/"
-                }
-            ],
-            "integrity": "sha512-Dr3sfKRP6oTcjf2JmUmFJfeVMvXBdegxB0iVQ5eb2V10uFJUCAS8OByZdVAyVb8xXNz3GjjTgj9kLWsZTqE6kw==",
+            "funding": {
+                "url": "https://paulmillr.com/funding/"
+            },
+            "integrity": "sha512-7VT13fmjotKpGipCW9JEQAusEPE+Ei8nl6/g4FBAmIm0GOOLMua9NDDo/DWp0ZAxCr3cPq5ZpBqmPAQgDda2Pw==",
             "optionalDependencies": {
                 "fsevents": "~2.3.2"
             },
-            "resolved": "https://registry.npmjs.org/chokidar/-/chokidar-3.5.3.tgz",
-            "version": "3.5.3"
+            "resolved": "https://registry.npmjs.org/chokidar/-/chokidar-3.6.0.tgz",
+            "version": "3.6.0"
         },
         "node_modules/dompurify": {
             "integrity": "sha512-kxxKlPEDa6Nc5WJi+qRgPbOAbgTpSULL+vI3NUXsZMlkJxTqYI9wg5ZTay2sFrdZRWHPWNi+EdAhcJf81WtoMQ==",
             "resolved": "https://registry.npmjs.org/dompurify/-/dompurify-2.4.7.tgz",
             "version": "2.4.7"
         },
         "node_modules/electron-to-chromium": {
-            "integrity": "sha512-z/6oZ/Muqk4BaE7P69bXhUhpJbUM9ZJeka43ZwxsDshKtePns4mhBlh8bU5+yrnOnz3fhG82XLzGUXazOmsWnA==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.640.tgz",
-            "version": "1.4.640"
+            "integrity": "sha512-GatzRKnGPS1go29ep25reM94xxd1Wj8ritU0yRhCJ/tr1Bg8gKnm6R9O/yPOhGQBoLMZ9ezfrpghNaTw97C/PQ==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.689.tgz",
+            "version": "1.4.689"
         },
         "node_modules/escalade": {
             "engines": {
                 "node": ">=6"
             },
-            "integrity": "sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==",
-            "resolved": "https://registry.npmjs.org/escalade/-/escalade-3.1.1.tgz",
-            "version": "3.1.1"
+            "integrity": "sha512-ErCHMCae19vR8vQGe50xIsVomy19rg6gFu3+r3jkEO46suLMWBksvVyoGgQV+jOfl84ZSOSlmv6Gxa89PmTGmA==",
+            "resolved": "https://registry.npmjs.org/escalade/-/escalade-3.1.2.tgz",
+            "version": "3.1.2"
         },
         "node_modules/fill-range": {
             "dependencies": {
                 "to-regex-range": "^5.0.1"
             },
             "dev": true,
             "engines": {
@@ -282,17 +279,17 @@
             },
             "integrity": "sha512-AOIgSQCepiJYwP3ARnGx+5VnTu2HBYdzbGP45eLw1vr3zB3vZLeyed1sC9hnbcOc9/SrMyM5RPQrkGz4aS9Zow==",
             "resolved": "https://registry.npmjs.org/glob-parent/-/glob-parent-5.1.2.tgz",
             "version": "5.1.2"
         },
         "node_modules/immutable": {
             "dev": true,
-            "integrity": "sha512-fsXeu4J4i6WNWSikpI88v/PcVflZz+6kMhUfIwc5SY+poQRPnaf5V7qds6SUyUN3cVxEzuCab7QIoLOQ+DQ1wA==",
-            "resolved": "https://registry.npmjs.org/immutable/-/immutable-4.3.4.tgz",
-            "version": "4.3.4"
+            "integrity": "sha512-8eabxkth9gZatlwl5TBuJnCsoTADlL6ftEr7A4qgdaTsPyreilDSnUk57SO+jfKcNtxPa22U5KK6DSeAYhpBJw==",
+            "resolved": "https://registry.npmjs.org/immutable/-/immutable-4.3.5.tgz",
+            "version": "4.3.5"
         },
         "node_modules/is-binary-path": {
             "dependencies": {
                 "binary-extensions": "^2.0.0"
             },
             "dev": true,
             "engines": {
@@ -418,18 +415,18 @@
                     "url": "https://tidelift.com/funding/github/npm/postcss"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-Kkpbhhdjw2qQs2O2DGX+8m5OVqEcbB9HRBvuYM9pgrjEFUg30A9LmXNlTAUj4S9kgtGyrMbTzVjH7E+s5Re2yg==",
+            "integrity": "sha512-u5U8qYpBCpN13BsiEB0CbR1Hhh4Gc0zLFuedrHJKMctHCHAGrMdG0PRM/KErzAL3CU6/eckEtmHNB3x6e3c0vA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.33.tgz",
-            "version": "8.4.33"
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.35.tgz",
+            "version": "8.4.35"
         },
         "node_modules/postcss-value-parser": {
             "integrity": "sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==",
             "resolved": "https://registry.npmjs.org/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz",
             "version": "4.2.0"
         },
         "node_modules/prosemirror-commands": {
@@ -454,17 +451,17 @@
             "version": "1.3.2"
         },
         "node_modules/prosemirror-inputrules": {
             "dependencies": {
                 "prosemirror-state": "^1.0.0",
                 "prosemirror-transform": "^1.0.0"
             },
-            "integrity": "sha512-z1GRP2vhh5CihYMQYsJSa1cOwXb3SYxALXOIfAkX8nZserARtl9LiL+CEl+T+OFIsXc3mJIHKhbsmRzC0HDAXA==",
-            "resolved": "https://registry.npmjs.org/prosemirror-inputrules/-/prosemirror-inputrules-1.3.0.tgz",
-            "version": "1.3.0"
+            "integrity": "sha512-6ygpPRuTJ2lcOXs9JkefieMst63wVJBgHZGl5QOytN7oSZs3Co/BYbc3Yx9zm9H37Bxw8kVzCnDsihsVsL4yEg==",
+            "resolved": "https://registry.npmjs.org/prosemirror-inputrules/-/prosemirror-inputrules-1.4.0.tgz",
+            "version": "1.4.0"
         },
         "node_modules/prosemirror-keymap": {
             "dependencies": {
                 "prosemirror-state": "^1.0.0",
                 "w3c-keyname": "^2.2.0"
             },
             "integrity": "sha512-EAlXoksqC6Vbocqc0GtzCruZEzYgrn+iiGnNjsJsH4mrnIGex4qbLdWWNza3AW5W36ZRrlBID0eM6bdKH4OStQ==",
@@ -499,17 +496,17 @@
         },
         "node_modules/prosemirror-view": {
             "dependencies": {
                 "prosemirror-model": "^1.16.0",
                 "prosemirror-state": "^1.0.0",
                 "prosemirror-transform": "^1.1.0"
             },
-            "integrity": "sha512-pvxiOoD4shW41X5bYDjRQk3DSG4fMqxh36yPMt7VYgU3dWRmqFzWJM/R6zeo1KtC8nyk717ZbQND3CC9VNeptw==",
-            "resolved": "https://registry.npmjs.org/prosemirror-view/-/prosemirror-view-1.32.7.tgz",
-            "version": "1.32.7"
+            "integrity": "sha512-62qkYgSJIkwIMMCpuGuPzc52DiK1Iod6TWoIMxP4ja6BTD4yO8kCUL64PZ/WhH/dJ9fW0CDO39FhH1EMyhUFEg==",
+            "resolved": "https://registry.npmjs.org/prosemirror-view/-/prosemirror-view-1.33.1.tgz",
+            "version": "1.33.1"
         },
         "node_modules/readdirp": {
             "dependencies": {
                 "picomatch": "^2.2.1"
             },
             "dev": true,
             "engines": {
```

### Comparing `aup_manager-2.0.4/aup_manager/templates/accept_aups.html` & `aup_manager-2.0.5/aup_manager/templates/accept_aups.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/templates/aup_overview.html` & `aup_manager-2.0.5/aup_manager/templates/aup_overview.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/templates/base.html` & `aup_manager-2.0.5/aup_manager/templates/base.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/templates/create_aup.html` & `aup_manager-2.0.5/aup_manager/templates/create_aup.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/templates/manage_aups.html` & `aup_manager-2.0.5/aup_manager/templates/manage_aups.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager/templates/unauthorized.html` & `aup_manager-2.0.5/aup_manager/templates/unauthorized.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/aup_manager.egg-info/PKG-INFO` & `aup_manager-2.0.5/aup_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aup-manager
-Version: 2.0.4
+Version: 2.0.5
 Summary: app for management of acceptable use policies with API for approving them
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/aup-manager.git
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: pymongo==4.6.1
 Requires-Dist: jsonpatch==1.33
```

### Comparing `aup_manager-2.0.4/aup_manager.egg-info/SOURCES.txt` & `aup_manager-2.0.5/aup_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.4/setup.py` & `aup_manager-2.0.5/setup.py`

 * *Files identical despite different names*

