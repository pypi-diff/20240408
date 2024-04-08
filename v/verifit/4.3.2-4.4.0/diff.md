# Comparing `tmp/verifit-4.3.2.tar.gz` & `tmp/verifit-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifit-4.3.2.tar", last modified: Mon Apr  8 11:45:06 2024, max compression
+gzip compressed data, was "verifit-4.4.0.tar", last modified: Mon Apr  8 17:41:35 2024, max compression
```

## Comparing `verifit-4.3.2.tar` & `verifit-4.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:45:06.751893 verifit-4.3.2/
--rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-4.3.2/LICENSE
--rw-r--r--   0 sorel      (501) staff       (20)       97 2024-04-08 11:37:12.000000 verifit-4.3.2/MANIFEST.in
--rw-r--r--   0 sorel      (501) staff       (20)    14519 2024-04-08 11:45:06.751535 verifit-4.3.2/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)    12537 2024-04-08 11:41:14.000000 verifit-4.3.2/Readme.md
--rw-r--r--   0 sorel      (501) staff       (20)     1020 2024-04-08 11:44:50.000000 verifit-4.3.2/pyproject.toml
--rw-r--r--   0 sorel      (501) staff       (20)      132 2024-04-06 17:38:40.000000 verifit-4.3.2/requirements.txt
--rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-08 11:45:06.752038 verifit-4.3.2/setup.cfg
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:45:06.739814 verifit-4.3.2/src/
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:45:06.750111 verifit-4.3.2/src/verifit/
--rw-r--r--   0 sorel      (501) staff       (20)      164 2023-11-15 09:10:11.000000 verifit-4.3.2/src/verifit/__init__.py
--rw-r--r--   0 sorel      (501) staff       (20)     1241 2023-11-15 08:17:34.000000 verifit-4.3.2/src/verifit/cache.py
--rw-r--r--   0 sorel      (501) staff       (20)      419 2023-11-15 08:25:40.000000 verifit-4.3.2/src/verifit/config.py
--rw-r--r--   0 sorel      (501) staff       (20)      255 2023-09-28 07:05:33.000000 verifit-4.3.2/src/verifit/date_tools.py
--rw-r--r--   0 sorel      (501) staff       (20)      381 2023-11-15 08:29:15.000000 verifit-4.3.2/src/verifit/driver.py
--rw-r--r--   0 sorel      (501) staff       (20)     7152 2024-04-08 11:44:20.000000 verifit-4.3.2/src/verifit/http_server.py
--rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-4.3.2/src/verifit/json_web_token.py
--rw-r--r--   0 sorel      (501) staff       (20)     1969 2023-11-15 09:05:55.000000 verifit-4.3.2/src/verifit/login.py
--rw-r--r--   0 sorel      (501) staff       (20)     1317 2023-11-15 09:19:37.000000 verifit-4.3.2/src/verifit/retrieve.py
--rw-r--r--   0 sorel      (501) staff       (20)      305 2024-04-08 07:50:18.000000 verifit-4.3.2/src/verifit/schema.graphql
--rw-r--r--   0 sorel      (501) staff       (20)     1275 2024-03-01 16:43:55.000000 verifit-4.3.2/src/verifit/web_sockets.py
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 11:45:06.751261 verifit-4.3.2/verifit.egg-info/
--rw-r--r--   0 sorel      (501) staff       (20)    14519 2024-04-08 11:45:06.000000 verifit-4.3.2/verifit.egg-info/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)      486 2024-04-08 11:45:06.000000 verifit-4.3.2/verifit.egg-info/SOURCES.txt
--rw-r--r--   0 sorel      (501) staff       (20)        1 2024-04-08 11:45:06.000000 verifit-4.3.2/verifit.egg-info/dependency_links.txt
--rw-r--r--   0 sorel      (501) staff       (20)       87 2024-04-08 11:45:06.000000 verifit-4.3.2/verifit.egg-info/requires.txt
--rw-r--r--   0 sorel      (501) staff       (20)        8 2024-04-08 11:45:06.000000 verifit-4.3.2/verifit.egg-info/top_level.txt
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 17:41:35.894821 verifit-4.4.0/
+-rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-4.4.0/LICENSE
+-rw-r--r--   0 sorel      (501) staff       (20)       97 2024-04-08 11:37:12.000000 verifit-4.4.0/MANIFEST.in
+-rw-r--r--   0 sorel      (501) staff       (20)    14615 2024-04-08 17:41:35.894534 verifit-4.4.0/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)    12633 2024-04-08 17:41:02.000000 verifit-4.4.0/Readme.md
+-rw-r--r--   0 sorel      (501) staff       (20)     1020 2024-04-08 14:52:55.000000 verifit-4.4.0/pyproject.toml
+-rw-r--r--   0 sorel      (501) staff       (20)      132 2024-04-06 17:38:40.000000 verifit-4.4.0/requirements.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-08 17:41:35.894865 verifit-4.4.0/setup.cfg
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 17:41:35.888049 verifit-4.4.0/src/
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 17:41:35.893302 verifit-4.4.0/src/verifit/
+-rw-r--r--   0 sorel      (501) staff       (20)      164 2023-11-15 09:10:11.000000 verifit-4.4.0/src/verifit/__init__.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1241 2023-11-15 08:17:34.000000 verifit-4.4.0/src/verifit/cache.py
+-rw-r--r--   0 sorel      (501) staff       (20)      419 2023-11-15 08:25:40.000000 verifit-4.4.0/src/verifit/config.py
+-rw-r--r--   0 sorel      (501) staff       (20)      255 2023-09-28 07:05:33.000000 verifit-4.4.0/src/verifit/date_tools.py
+-rw-r--r--   0 sorel      (501) staff       (20)      381 2023-11-15 08:29:15.000000 verifit-4.4.0/src/verifit/driver.py
+-rw-r--r--   0 sorel      (501) staff       (20)     7694 2024-04-08 17:36:59.000000 verifit-4.4.0/src/verifit/http_server.py
+-rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-4.4.0/src/verifit/json_web_token.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1969 2023-11-15 09:05:55.000000 verifit-4.4.0/src/verifit/login.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1317 2023-11-15 09:19:37.000000 verifit-4.4.0/src/verifit/retrieve.py
+-rw-r--r--   0 sorel      (501) staff       (20)      305 2024-04-08 07:50:18.000000 verifit-4.4.0/src/verifit/schema.graphql
+-rw-r--r--   0 sorel      (501) staff       (20)     1275 2024-03-01 16:43:55.000000 verifit-4.4.0/src/verifit/web_sockets.py
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 17:41:35.894307 verifit-4.4.0/verifit.egg-info/
+-rw-r--r--   0 sorel      (501) staff       (20)    14615 2024-04-08 17:41:35.000000 verifit-4.4.0/verifit.egg-info/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)      486 2024-04-08 17:41:35.000000 verifit-4.4.0/verifit.egg-info/SOURCES.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        1 2024-04-08 17:41:35.000000 verifit-4.4.0/verifit.egg-info/dependency_links.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       87 2024-04-08 17:41:35.000000 verifit-4.4.0/verifit.egg-info/requires.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        8 2024-04-08 17:41:35.000000 verifit-4.4.0/verifit.egg-info/top_level.txt
```

### Comparing `verifit-4.3.2/LICENSE` & `verifit-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `verifit-4.3.2/PKG-INFO` & `verifit-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 4.3.2
+Version: 4.4.0
 Summary: Verify It: Automatic Testing helper tools & sample tests
 Author-email: Sorel Mitra <sorelmitra@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 sorelmitra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -230,15 +230,15 @@
     - Log in using a driver, which is a plain function.  We use a driver for this because logging in is particular to the API that each project has.  The driver does the actual call to the API endpoint for login, and returns the access token.  The framework caches the access token and its expiration date.
     - Log in from a cached token using a driver.
     - Building authorization values:
       - For HTTP headers.
       - For the Python GraphQL client.
 - `prop.py`:  Access dictionary properties without raising exceptions, and with default values.
 - `retrieve.py`.  Shortcut functions for calling to HTTP or GraphQL endpoints, with unified logging.
-- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.  It also provides a GraphQL server, that serves a sample schema, and also supports serving a custom schema.
+- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and puts the response in a `multiprocessing.Queue`, so responses for multiple calls can be checked in a test.  It supports a different response for each call.  It also provides a GraphQL server, that serves a sample schema, and also supports serving a custom schema.
 - `web_sockets.py`.  Simplifies Web-Sockets testing by offering functions for listening in background for received packages, and sending data.
 
 
 
 
 # Development
```

### Comparing `verifit-4.3.2/Readme.md` & `verifit-4.4.0/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     - Log in using a driver, which is a plain function.  We use a driver for this because logging in is particular to the API that each project has.  The driver does the actual call to the API endpoint for login, and returns the access token.  The framework caches the access token and its expiration date.
     - Log in from a cached token using a driver.
     - Building authorization values:
       - For HTTP headers.
       - For the Python GraphQL client.
 - `prop.py`:  Access dictionary properties without raising exceptions, and with default values.
 - `retrieve.py`.  Shortcut functions for calling to HTTP or GraphQL endpoints, with unified logging.
-- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.  It also provides a GraphQL server, that serves a sample schema, and also supports serving a custom schema.
+- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and puts the response in a `multiprocessing.Queue`, so responses for multiple calls can be checked in a test.  It supports a different response for each call.  It also provides a GraphQL server, that serves a sample schema, and also supports serving a custom schema.
 - `web_sockets.py`.  Simplifies Web-Sockets testing by offering functions for listening in background for received packages, and sending data.
 
 
 
 
 # Development
```

### Comparing `verifit-4.3.2/pyproject.toml` & `verifit-4.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 packages = ['verifit']
 
 [tool.check-manifest]
 ignore = [".pytest_cache/*", "node_modules/**/*"]
 
 [project]
 name = "verifit"
-version = "4.3.2"
+version = "4.4.0"
 description = "Verify It: Automatic Testing helper tools & sample tests"
 readme = "Readme.md"
 authors = [{ name = "Sorel Mitra", email = "sorelmitra@yahoo.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `verifit-4.3.2/src/verifit/cache.py` & `verifit-4.4.0/src/verifit/cache.py`

 * *Files identical despite different names*

### Comparing `verifit-4.3.2/src/verifit/http_server.py` & `verifit-4.4.0/src/verifit/http_server.py`

 * *Files 23% similar despite different names*

```diff
@@ -52,56 +52,71 @@
 
     @staticmethod
     def graphql_url():
         return f"{HttpConfig.base_url()}{HttpConfig.GRAPHQL_PATH}"
 
 
 KEY_QUEUE = 'queue'
-KEY_CALLS_COUNT = 'calls_count'
-KEY_STATUS_TO_RETURN = 'status_to_return'
-KEY_SUCCEED_AT_ATTEMPT_NO = 'succeed_at_attempt_no'
+KEY_ENDPOINT_INDEX = 'endpoint_index'
+KEY_ENDPOINT_RESULTS = 'endpoint_results'
+KEY_ENDPOINT_PREVIOUS_CALL_FAILED = 'endpoint_previous_call_failed'
+KEY_ENDPOINT_CURRENT_PAYLOAD = 'endpoint_current_payload'
 KEY_GRAPHQL_SCHEMA = 'graphql_schema'
 
 
 @cache
 def get_store():
     return {}
 
 
 class EndpointResult:
-    def __init__(self, *, success, status_code, response_data):
-        self.success = success
+    def __init__(self, *, status_code=200, response_data=None):
         self.status_code = status_code
         self.response_data = response_data
 
+    def is_successful(self):
+        return 200 <= self.status_code <= 299
+
 
 def determine_endpoint_result() -> EndpointResult:
     store = get_store()
-    status_to_return = store.get(KEY_STATUS_TO_RETURN)
-    succeed_at_attempt_no = store.get(KEY_SUCCEED_AT_ATTEMPT_NO)
-    calls_count = store.get(KEY_CALLS_COUNT)
-    calls_count = calls_count + 1
-    store[KEY_CALLS_COUNT] = calls_count
-    if succeed_at_attempt_no > 0:
-        if calls_count >= succeed_at_attempt_no:
-            status_to_return = 202
-    success = 200 <= status_to_return <= 299
-    response = {"success": success}
-    return EndpointResult(
-        success=success, status_code=status_to_return, response_data=response)
+    endpoint_results: list[EndpointResult] = store.get(KEY_ENDPOINT_RESULTS)
+    endpoint_index = store.get(KEY_ENDPOINT_INDEX)
+
+    if endpoint_index < len(endpoint_results):
+        endpoint_result = endpoint_results[endpoint_index]
+    else:
+        current_payload = store.get(KEY_ENDPOINT_CURRENT_PAYLOAD, None)
+        endpoint_result = EndpointResult(
+            status_code=200,
+            response_data=current_payload if current_payload is not None else {"success": True}
+        )
+
+    if store.get(KEY_ENDPOINT_PREVIOUS_CALL_FAILED) and endpoint_result.is_successful():
+        endpoint_result.status_code = 202
+
+    if not endpoint_result.is_successful():
+        store[KEY_ENDPOINT_PREVIOUS_CALL_FAILED] = True
+
+    print(f"Endpoint {endpoint_index} Result: {endpoint_result.status_code} {endpoint_result.response_data}")
+
+    endpoint_index = endpoint_index + 1
+    store[KEY_ENDPOINT_INDEX] = endpoint_index
+    return endpoint_result
 
 
 @api().route(HttpConfig.POST_PATH, methods=['POST'])
 def post_listener():
     store = get_store()
     q = store.get(KEY_QUEUE)
-    post_response = request.json
-    print(f"Post Payload: {post_response}")
+    post_payload = request.json
+    print(f"Post Payload: {post_payload}")
+    store[KEY_ENDPOINT_CURRENT_PAYLOAD] = post_payload
     endpoint_result = determine_endpoint_result()
-    q.put(post_response if endpoint_result.success else endpoint_result.response_data)
+    q.put(endpoint_result.response_data)
     return json.dumps(endpoint_result.response_data), endpoint_result.status_code
 
 
 @api().route(HttpConfig.GET_PATH, methods=['GET'])
 def get_listener():
     store = get_store()
     q = store.get(KEY_QUEUE)
@@ -110,29 +125,31 @@
     return json.dumps(endpoint_result.response_data), endpoint_result.status_code
 
 
 @api().route(HttpConfig.PUT_PATH, methods=['PUT'])
 def put_listener():
     store = get_store()
     q = store.get(KEY_QUEUE)
-    put_response = request.json
-    print(f"Put Payload: {put_response}")
+    put_payload = request.json
+    print(f"Put Payload: {put_payload}")
+    store[KEY_ENDPOINT_CURRENT_PAYLOAD] = put_payload
     endpoint_result = determine_endpoint_result()
-    q.put(put_response if endpoint_result.success else endpoint_result.response_data)
+    q.put(endpoint_result.response_data)
     return json.dumps(endpoint_result.response_data), endpoint_result.status_code
 
 
 @api().route(HttpConfig.PATCH_PATH, methods=['PATCH'])
 def patch_listener():
     store = get_store()
     q = store.get(KEY_QUEUE)
-    patch_response = request.json
-    print(f"Patch Payload: {patch_response}")
+    patch_payload = request.json
+    print(f"Patch Payload: {patch_payload}")
+    store[KEY_ENDPOINT_CURRENT_PAYLOAD] = patch_payload
     endpoint_result = determine_endpoint_result()
-    q.put(patch_response if endpoint_result.success else endpoint_result.response_data)
+    q.put(endpoint_result.response_data)
     return json.dumps(endpoint_result.response_data), endpoint_result.status_code
 
 
 @api().route(HttpConfig.DELETE_PATH, methods=['DELETE'])
 def delete_listener():
     store = get_store()
     q = store.get(KEY_QUEUE)
@@ -155,15 +172,15 @@
     status_code = 200 if success else 400
     return jsonify(result), status_code
 
 
 @convert_kwargs_to_snake_case
 def get_notice_resolver(_obj, _info, id):
     endpoint_result = determine_endpoint_result()
-    if endpoint_result.success:
+    if endpoint_result.is_successful():
         payload = {
             "success": True,
             "notice": {
                 "id": id,
                 "title": 'foo notice'
             }
         }
@@ -175,15 +192,15 @@
     print(f"GraphQL Get Notice Payload: {payload}")
     return payload
 
 
 @convert_kwargs_to_snake_case
 def create_notice_resolver(_obj, _info, title):
     endpoint_result = determine_endpoint_result()
-    if endpoint_result.success:
+    if endpoint_result.is_successful():
         payload = {
             "success": True,
             "notice": {
                 "id": 'foo',
                 "title": title
             }
         }
@@ -193,20 +210,19 @@
             "errors": [f"Notice item not created"]
         }
     print(f"GraphQL Create Notice Payload: {payload}")
     return payload
 
 
 def http_server_start_process(
-        response_queue, status_to_return, succeed_at_attempt_no, graphql_schema):
+        response_queue, endpoint_results: list[EndpointResult], graphql_schema):
     store = get_store()
     store[KEY_QUEUE] = response_queue
-    store[KEY_CALLS_COUNT] = 0
-    store[KEY_STATUS_TO_RETURN] = status_to_return
-    store[KEY_SUCCEED_AT_ATTEMPT_NO] = succeed_at_attempt_no
+    store[KEY_ENDPOINT_INDEX] = 0
+    store[KEY_ENDPOINT_RESULTS] = [] if endpoint_results is None else endpoint_results
 
     if graphql_schema is None:
         type_definitions = load_schema_from_path(os.path.join(get_script_dir(), "schema.graphql"))
         query = ObjectType("Query")
         query.set_field("getNotice", get_notice_resolver)
         mutation = ObjectType("Mutation")
         mutation.set_field("createNotice", create_notice_resolver)
@@ -216,18 +232,18 @@
     else:
         store[KEY_GRAPHQL_SCHEMA] = graphql_schema()
 
     api().run(port=HttpConfig.PORT)
 
 
 def http_server_start(
-        *, response_queue, status=200, succeed_at_attempt_no=0, graphql_schema=None):
+        *, response_queue, endpoint_results: list[EndpointResult]=None, graphql_schema=None):
     server = Process(
         target=http_server_start_process,
-        args=(response_queue, status, succeed_at_attempt_no, graphql_schema))
+        args=(response_queue, endpoint_results, graphql_schema))
     server.start()
     time.sleep(2)
     return server
 
 
 def http_server_stop(server):
     server.terminate()
```

### Comparing `verifit-4.3.2/src/verifit/login.py` & `verifit-4.4.0/src/verifit/login.py`

 * *Files identical despite different names*

### Comparing `verifit-4.3.2/src/verifit/retrieve.py` & `verifit-4.4.0/src/verifit/retrieve.py`

 * *Files identical despite different names*

### Comparing `verifit-4.3.2/src/verifit/web_sockets.py` & `verifit-4.4.0/src/verifit/web_sockets.py`

 * *Files identical despite different names*

### Comparing `verifit-4.3.2/verifit.egg-info/PKG-INFO` & `verifit-4.4.0/verifit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 4.3.2
+Version: 4.4.0
 Summary: Verify It: Automatic Testing helper tools & sample tests
 Author-email: Sorel Mitra <sorelmitra@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 sorelmitra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -230,15 +230,15 @@
     - Log in using a driver, which is a plain function.  We use a driver for this because logging in is particular to the API that each project has.  The driver does the actual call to the API endpoint for login, and returns the access token.  The framework caches the access token and its expiration date.
     - Log in from a cached token using a driver.
     - Building authorization values:
       - For HTTP headers.
       - For the Python GraphQL client.
 - `prop.py`:  Access dictionary properties without raising exceptions, and with default values.
 - `retrieve.py`.  Shortcut functions for calling to HTTP or GraphQL endpoints, with unified logging.
-- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and returns the received payload in a `multiprocessing.Queue`.  It also provides a GraphQL server, that serves a sample schema, and also supports serving a custom schema.
+- `http_server.py`.  Tiny HTTP server, that provides a few endpoints, and puts the response in a `multiprocessing.Queue`, so responses for multiple calls can be checked in a test.  It supports a different response for each call.  It also provides a GraphQL server, that serves a sample schema, and also supports serving a custom schema.
 - `web_sockets.py`.  Simplifies Web-Sockets testing by offering functions for listening in background for received packages, and sending data.
 
 
 
 
 # Development
```

