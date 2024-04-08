# Comparing `tmp/alcedo-0.1.6.tar.gz` & `tmp/alcedo-0.1.7.tar.gz`

## Comparing `alcedo-0.1.6.tar` & `alcedo-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 alcedo-0.1.6/Cargo.toml
--rw-r--r--   0      501       20      392 2024-03-22 18:34:20.000000 alcedo-0.1.6/.gitignore
--rw-r--r--   0      501       20     1072 2024-03-22 05:37:01.000000 alcedo-0.1.6/LICENSE
--rw-r--r--   0      501       20     6769 2024-03-28 09:16:55.000000 alcedo-0.1.6/README.md
--rw-r--r--   0      501       20     1316 2024-04-04 08:08:19.000000 alcedo-0.1.6/alcedo.pyi
--rw-r--r--   0      501       20     2067 2024-03-28 09:17:30.000000 alcedo-0.1.6/benchmarks.md
--rw-r--r--   0      501       20   115533 2024-03-21 16:49:27.000000 alcedo-0.1.6/poetry.lock
--rw-r--r--   0      501       20     2271 2024-04-04 08:08:03.000000 alcedo-0.1.6/pyproject.toml
--rw-r--r--   0      501       20     4023 2024-04-04 08:03:13.000000 alcedo-0.1.6/src/client.rs
--rw-r--r--   0      501       20     3172 2024-04-01 00:41:10.000000 alcedo-0.1.6/src/dictionary.rs
--rw-r--r--   0      501       20     2352 2024-03-23 17:24:27.000000 alcedo-0.1.6/src/json_value.rs
--rw-r--r--   0      501       20     1310 2024-04-01 00:47:44.000000 alcedo-0.1.6/src/lib.rs
--rw-r--r--   0      501       20     1977 2024-03-27 09:09:09.000000 alcedo-0.1.6/src/response.rs
--rw-r--r--   0      501       20   565477 2024-03-22 18:14:20.000000 alcedo-0.1.6/static/alcedo-banner.svg
--rw-r--r--   0      501       20   147962 2024-03-25 08:22:46.000000 alcedo-0.1.6/static/alcedo-preview.png
--rw-r--r--   0      501       20   567105 2024-03-25 06:59:07.000000 alcedo-0.1.6/static/alcedo-preview.svg
--rw-r--r--   0      501       20   363124 2024-03-20 16:54:52.000000 alcedo-0.1.6/static/alcedo.base64
--rw-r--r--   0      501       20   272342 2024-03-20 16:54:36.000000 alcedo-0.1.6/static/alcedo.svg
--rw-r--r--   0      501       20     2721 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/__init__.py
--rw-r--r--   0      501       20     1948 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/conftest.py
--rw-r--r--   0      501       20      479 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/get/__init__.py
--rw-r--r--   0      501       20     1015 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/get/bench.py
--rw-r--r--   0      501       20     1105 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/get/bench_httpx.py
--rw-r--r--   0      501       20     1129 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/get/bench_requests.py
--rw-r--r--   0      501       20      501 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/delete/__init__.py
--rw-r--r--   0      501       20      654 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/delete/bench.py
--rw-r--r--   0      501       20      847 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/delete/bench_aiohttp.py
--rw-r--r--   0      501       20      779 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/delete/bench_httpx.py
--rw-r--r--   0      501       20      804 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/delete/bench_requests.py
--rw-r--r--   0      501       20      495 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/get/__init__.py
--rw-r--r--   0      501       20     1152 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/get/bench.py
--rw-r--r--   0      501       20     1543 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/get/bench_aiohttp.py
--rw-r--r--   0      501       20     1242 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/get/bench_httpx.py
--rw-r--r--   0      501       20     1282 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/get/bench_requests.py
--rw-r--r--   0      501       20      497 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/post/__init__.py
--rw-r--r--   0      501       20      691 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/post/bench.py
--rw-r--r--   0      501       20      893 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/post/bench_aiohttp.py
--rw-r--r--   0      501       20      820 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/post/bench_httpx.py
--rw-r--r--   0      501       20      838 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/post/bench_requests.py
--rw-r--r--   0      501       20      495 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/put/__init__.py
--rw-r--r--   0      501       20      697 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/put/bench.py
--rw-r--r--   0      501       20      890 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/put/bench_aiohttp.py
--rw-r--r--   0      501       20      817 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/put/bench_httpx.py
--rw-r--r--   0      501       20      842 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/put/bench_requests.py
--rw-r--r--   0      501       20      513 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/queried_get/__init__.py
--rw-r--r--   0      501       20     1398 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/queried_get/bench.py
--rw-r--r--   0      501       20     1769 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/queried_get/bench_aiohttp.py
--rw-r--r--   0      501       20     1490 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/queried_get/bench_httpx.py
--rw-r--r--   0      501       20     1530 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/queried_get/bench_requests.py
--rw-r--r--   0      501       20    35157 2024-04-04 08:08:08.000000 alcedo-0.1.6/Cargo.lock
--rw-r--r--   0        0        0     7983 1970-01-01 00:00:00.000000 alcedo-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 alcedo-0.1.7/Cargo.toml
+-rw-r--r--   0      501       20      392 2024-03-22 18:34:20.000000 alcedo-0.1.7/.gitignore
+-rw-r--r--   0      501       20     1072 2024-03-22 05:37:01.000000 alcedo-0.1.7/LICENSE
+-rw-r--r--   0      501       20     6769 2024-03-28 09:16:55.000000 alcedo-0.1.7/README.md
+-rw-r--r--   0      501       20     1473 2024-04-08 10:05:13.000000 alcedo-0.1.7/alcedo.pyi
+-rw-r--r--   0      501       20     2067 2024-04-05 20:30:40.000000 alcedo-0.1.7/benchmarks.md
+-rw-r--r--   0      501       20   115533 2024-04-05 20:30:40.000000 alcedo-0.1.7/poetry.lock
+-rw-r--r--   0      501       20     2271 2024-04-08 10:05:48.000000 alcedo-0.1.7/pyproject.toml
+-rw-r--r--   0      501       20     4089 2024-04-08 09:59:49.000000 alcedo-0.1.7/src/client.rs
+-rw-r--r--   0      501       20     2352 2024-03-23 17:24:27.000000 alcedo-0.1.7/src/json_value.rs
+-rw-r--r--   0      501       20     1319 2024-04-08 09:54:36.000000 alcedo-0.1.7/src/lib.rs
+-rw-r--r--   0      501       20     1977 2024-04-07 18:59:05.000000 alcedo-0.1.7/src/response.rs
+-rw-r--r--   0      501       20     3207 2024-04-08 09:52:46.000000 alcedo-0.1.7/src/serialize_py_object.rs
+-rw-r--r--   0      501       20   565477 2024-03-22 18:14:20.000000 alcedo-0.1.7/static/alcedo-banner.svg
+-rw-r--r--   0      501       20   147962 2024-03-25 08:22:46.000000 alcedo-0.1.7/static/alcedo-preview.png
+-rw-r--r--   0      501       20   567105 2024-03-25 06:59:07.000000 alcedo-0.1.7/static/alcedo-preview.svg
+-rw-r--r--   0      501       20   363124 2024-03-20 16:54:52.000000 alcedo-0.1.7/static/alcedo.base64
+-rw-r--r--   0      501       20   272342 2024-03-20 16:54:36.000000 alcedo-0.1.7/static/alcedo.svg
+-rw-r--r--   0      501       20     2721 2024-04-08 10:06:24.000000 alcedo-0.1.7/tests/__init__.py
+-rw-r--r--   0      501       20     1948 2024-04-08 10:06:03.000000 alcedo-0.1.7/tests/conftest.py
+-rw-r--r--   0      501       20      479 2024-04-08 10:05:23.000000 alcedo-0.1.7/tests/get/__init__.py
+-rw-r--r--   0      501       20     1015 2024-04-08 10:06:46.000000 alcedo-0.1.7/tests/get/bench.py
+-rw-r--r--   0      501       20     1105 2024-04-08 10:07:05.000000 alcedo-0.1.7/tests/get/bench_httpx.py
+-rw-r--r--   0      501       20     1129 2024-04-08 10:07:17.000000 alcedo-0.1.7/tests/get/bench_requests.py
+-rw-r--r--   0      501       20      501 2024-04-08 10:08:28.000000 alcedo-0.1.7/tests/session/delete/__init__.py
+-rw-r--r--   0      501       20      654 2024-04-08 10:09:00.000000 alcedo-0.1.7/tests/session/delete/bench.py
+-rw-r--r--   0      501       20      847 2024-04-08 10:05:31.000000 alcedo-0.1.7/tests/session/delete/bench_aiohttp.py
+-rw-r--r--   0      501       20      779 2024-04-08 10:09:10.000000 alcedo-0.1.7/tests/session/delete/bench_httpx.py
+-rw-r--r--   0      501       20      804 2024-04-08 10:09:25.000000 alcedo-0.1.7/tests/session/delete/bench_requests.py
+-rw-r--r--   0      501       20      495 2024-04-08 10:11:57.000000 alcedo-0.1.7/tests/session/get/__init__.py
+-rw-r--r--   0      501       20     1152 2024-04-08 10:12:08.000000 alcedo-0.1.7/tests/session/get/bench.py
+-rw-r--r--   0      501       20     1543 2024-04-08 10:11:50.000000 alcedo-0.1.7/tests/session/get/bench_aiohttp.py
+-rw-r--r--   0      501       20     1242 2024-04-08 10:12:27.000000 alcedo-0.1.7/tests/session/get/bench_httpx.py
+-rw-r--r--   0      501       20     1282 2024-04-08 10:12:38.000000 alcedo-0.1.7/tests/session/get/bench_requests.py
+-rw-r--r--   0      501       20      497 2024-04-08 10:07:29.000000 alcedo-0.1.7/tests/session/post/__init__.py
+-rw-r--r--   0      501       20      691 2024-04-08 10:07:41.000000 alcedo-0.1.7/tests/session/post/bench.py
+-rw-r--r--   0      501       20      893 2024-04-08 10:06:15.000000 alcedo-0.1.7/tests/session/post/bench_aiohttp.py
+-rw-r--r--   0      501       20      820 2024-04-08 10:07:53.000000 alcedo-0.1.7/tests/session/post/bench_httpx.py
+-rw-r--r--   0      501       20      838 2024-04-08 10:08:16.000000 alcedo-0.1.7/tests/session/post/bench_requests.py
+-rw-r--r--   0      501       20      495 2024-04-08 10:10:08.000000 alcedo-0.1.7/tests/session/put/__init__.py
+-rw-r--r--   0      501       20      697 2024-04-08 10:11:19.000000 alcedo-0.1.7/tests/session/put/bench.py
+-rw-r--r--   0      501       20      890 2024-04-08 10:09:53.000000 alcedo-0.1.7/tests/session/put/bench_aiohttp.py
+-rw-r--r--   0      501       20      817 2024-04-08 10:11:29.000000 alcedo-0.1.7/tests/session/put/bench_httpx.py
+-rw-r--r--   0      501       20      842 2024-04-08 10:11:40.000000 alcedo-0.1.7/tests/session/put/bench_requests.py
+-rw-r--r--   0      501       20      513 2024-04-08 10:13:03.000000 alcedo-0.1.7/tests/session/queried_get/__init__.py
+-rw-r--r--   0      501       20     1398 2024-04-08 10:12:55.000000 alcedo-0.1.7/tests/session/queried_get/bench.py
+-rw-r--r--   0      501       20     1769 2024-04-08 10:11:04.000000 alcedo-0.1.7/tests/session/queried_get/bench_aiohttp.py
+-rw-r--r--   0      501       20     1490 2024-04-08 10:12:47.000000 alcedo-0.1.7/tests/session/queried_get/bench_httpx.py
+-rw-r--r--   0      501       20     1530 2024-04-08 10:09:31.000000 alcedo-0.1.7/tests/session/queried_get/bench_requests.py
+-rw-r--r--   0      501       20    35157 2024-04-08 10:05:08.000000 alcedo-0.1.7/Cargo.lock
+-rw-r--r--   0        0        0     7983 1970-01-01 00:00:00.000000 alcedo-0.1.7/PKG-INFO
```

### Comparing `alcedo-0.1.6/LICENSE` & `alcedo-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.6/README.md` & `alcedo-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.6/alcedo.pyi` & `alcedo-0.1.7/alcedo.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/alcedo.pyi
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-21 00:20
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
 ### Standard packages ###
-from typing import Any, Optional
+from typing import Optional, Union
 
 class Client:
-  def __init__(self, headers: Optional[dict] = None, **kwargs: Any) -> None: ...
+  def __init__(
+    self, headers: Optional[dict] = None, **kwargs: Union[bool, bytes, float, int, str]
+  ) -> None: ...
   def delete(
-    self, url: str, headers: Optional[dict] = None, payload: dict = {}, **kwargs: Any
+    self, url: str, headers: Optional[dict] = None, payload: dict = {}, query: Optional[dict] = None
+  ) -> Response: ...
+  def get(
+    self, url: str, headers: Optional[dict] = None, query: Optional[dict] = None
   ) -> Response: ...
-  def get(self, url: str, headers: Optional[dict] = None, **kwargs: Any) -> Response: ...
   def post(
-    self, url: str, headers: Optional[dict] = None, payload: dict = {}, **kwargs: Any
+    self, url: str, headers: Optional[dict] = None, payload: dict = {}, query: Optional[dict] = None
   ) -> Response: ...
   def put(
-    self, url: str, headers: Optional[dict] = None, payload: dict = {}, **kwargs: Any
+    self, url: str, headers: Optional[dict] = None, payload: dict = {}, query: Optional[dict] = None
   ) -> Response: ...
   def request(
-    self, method: str, url: str, headers: Optional[dict] = None, **kwargs: Any
+    self, method: str, url: str, headers: Optional[dict] = None, query: Optional[dict] = None
   ) -> Response: ...
 
 class Response:
-  def __init__(self, **kwargs: Any) -> None: ...
+  def __init__(self, **kwargs: Union[bool, bytes, float, int, str]) -> None: ...
   def json(self) -> dict: ...
   def text(self) -> str: ...
   def raise_for_status(self) -> None: ...
   def status(self) -> int: ...
   def headers(self) -> dict: ...
 
 def get(url: str, **kwargs: Any) -> Response: ...
```

### Comparing `alcedo-0.1.6/benchmarks.md` & `alcedo-0.1.7/benchmarks.md`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.6/poetry.lock` & `alcedo-0.1.7/poetry.lock`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.6/pyproject.toml` & `alcedo-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 [tool.poetry]
 authors = [ 'Sitt Guruvanich <aekazitt+github@gmail.com>' ]
 description = 'Oxidized and Optimistic HTTP Client for Python'
 license = 'MIT'
 name = 'alcedo'
-version = '0.1.6'
+version = '0.1.7'
 packages = [{include='alcedo.pyi'}]
 
 
 [tool.poetry.dependencies]
 python = '^3.8'
```

### Comparing `alcedo-0.1.6/src/client.rs` & `alcedo-0.1.7/src/client.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 // SPDX-License-Identifier: MIT
 
-use crate::{dictionary::Dictionary, response::Response, APP_USER_AGENT};
+use crate::{response::Response, serialize_py_object::SerializePyObject, APP_USER_AGENT};
 use pyo3::{pyclass, pymethods, PyObject, PyResult, Python};
 use reqwest::blocking::{Client as BlockingClient, RequestBuilder};
 use reqwest::header::{HeaderMap, HeaderName, HeaderValue};
 use reqwest::Method;
 use serde_json::{json, to_string};
 use std::collections::HashMap;
 use std::str::FromStr;
@@ -89,33 +89,33 @@
         let builder = self
             .blocking_client
             .request(Method::from_bytes(method.as_bytes()).unwrap(), url)
             .headers(dict_to_headers(headers.unwrap_or(HashMap::new())));
         let mut req: Result<RequestBuilder, RequestBuilder> = match payload {
             None => Ok(builder),
             Some(value) => Python::with_gil(|py| {
-                let d = Dictionary {
+                let serialized = SerializePyObject {
                     py,
                     obj: value.extract(py).unwrap(),
                 };
                 // let body = to_string(&d).map_err(ser::Error::custom);
-                let body = to_string(&d).unwrap();
+                let body = to_string(&serialized).unwrap();
                 Ok(builder
                     .header("Content-Type", "application/json")
                     .json(&json!(body)))
             }),
         };
         req = match query {
             None => req,
             Some(value) => Python::with_gil(|py| {
-                let d = Dictionary {
+                let serialized = SerializePyObject {
                     py,
                     obj: value.extract(py).unwrap(),
                 };
-                Ok(req.unwrap().query(&d))
+                Ok(req.unwrap().query(&serialized))
             }),
         };
         let response = req.unwrap().send().unwrap();
         let mut h: HashMap<String, String> = HashMap::with_capacity(response.headers().len());
         for (key, value) in response.headers().iter() {
             h.insert(key.to_string(), value.to_str().unwrap().to_string());
         }
```

### Comparing `alcedo-0.1.6/src/dictionary.rs` & `alcedo-0.1.7/src/serialize_py_object.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 // SPDX-License-Identifier: MIT
 
 use pyo3::types::{PyAny, PyDict, PyFloat, PyList, PyTuple};
 use pyo3::{FromPyObject, Python};
 use serde::ser::{self, Serialize, SerializeMap, SerializeSeq, Serializer};
 use std::string::String;
 
-pub struct Dictionary<'p, 'a> {
+pub struct SerializePyObject<'p, 'a> {
     pub py: Python<'p>,
     pub obj: &'a PyAny,
 }
 
-impl<'p, 'a> Serialize for Dictionary<'p, 'a> {
+impl<'p, 'a> Serialize for SerializePyObject<'p, 'a> {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         macro_rules! cast {
             ($f:expr) => {
                 if let Ok(val) = FromPyObject::extract(self.obj) {
@@ -44,36 +44,36 @@
                     map.serialize_key(&key)?;
                 } else {
                     return Err(ser::Error::custom(format_args!(
                         "Dictionary key is not a string: {:?}",
                         key
                     )));
                 }
-                map.serialize_value(&Dictionary {
+                map.serialize_value(&SerializePyObject {
                     py: self.py,
                     obj: value,
                 })?;
             }
             map.end()
         });
 
         cast!(|x: &PyList| {
             let mut seq = serializer.serialize_seq(Some(x.len()))?;
             for element in x {
-                seq.serialize_element(&Dictionary {
+                seq.serialize_element(&SerializePyObject {
                     py: self.py,
                     obj: element,
                 })?
             }
             seq.end()
         });
         cast!(|x: &PyTuple| {
             let mut seq = serializer.serialize_seq(Some(x.len()))?;
             for element in x {
-                seq.serialize_element(&Dictionary {
+                seq.serialize_element(&SerializePyObject {
                     py: self.py,
                     obj: element,
                 })?
             }
             seq.end()
         });
```

### Comparing `alcedo-0.1.6/src/json_value.rs` & `alcedo-0.1.7/src/json_value.rs`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.6/src/lib.rs` & `alcedo-0.1.7/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 use pyo3::{create_exception, pyfunction, pymodule, wrap_pyfunction, Bound, PyResult};
 use reqwest::blocking::get as r_get;
 use std::collections::HashMap;
 use std::str::FromStr;
 static APP_USER_AGENT: &str = concat!(env!("CARGO_PKG_NAME"), "/", env!("CARGO_PKG_VERSION"),);
 
 mod client;
-mod dictionary;
 mod json_value;
 mod response;
+mod serialize_py_object;
 use response::Response;
 
 create_exception!(reqwest, HTTPError, PyException);
 
 #[pyfunction]
 fn get(url: &str) -> PyResult<Response> {
     let response = r_get(url).unwrap();
```

### Comparing `alcedo-0.1.6/src/response.rs` & `alcedo-0.1.7/src/response.rs`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.6/static/alcedo-banner.svg` & `alcedo-0.1.7/static/alcedo-banner.svg`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.6/static/alcedo-preview.png` & `alcedo-0.1.7/static/alcedo-preview.png`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.6/static/alcedo-preview.svg` & `alcedo-0.1.7/static/alcedo-preview.svg`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.6/static/alcedo.base64` & `alcedo-0.1.7/static/alcedo.base64`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.6/static/alcedo.svg` & `alcedo-0.1.7/static/alcedo.svg`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.6/tests/__init__.py` & `alcedo-0.1.7/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/__init__.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-21 13:31
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION: https://www.w3docs.com/snippets/python/what-is-init-py-for.html
 #
 # HISTORY:
 # *************************************************************
 """Module indicating that `~~/tests` directory is present in is a Python package."""
```

### Comparing `alcedo-0.1.6/tests/conftest.py` & `alcedo-0.1.7/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/conftest.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-21 16:42
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/get/bench.py` & `alcedo-0.1.7/tests/get/bench.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/get/bench.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-21 13:31
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/get/bench_httpx.py` & `alcedo-0.1.7/tests/get/bench_httpx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/get/bench_httpx.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-21 13:31
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/get/bench_requests.py` & `alcedo-0.1.7/tests/get/bench_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/get/bench_requests.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-21 16:55
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/delete/bench.py` & `alcedo-0.1.7/tests/session/delete/bench.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/delete/bench.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-28 14:24
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/delete/bench_aiohttp.py` & `alcedo-0.1.7/tests/session/delete/bench_aiohttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/delete/bench_aiohttp.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-28 14:24
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/delete/bench_httpx.py` & `alcedo-0.1.7/tests/session/delete/bench_httpx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/delete/bench_httpx.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-28 14:24
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/delete/bench_requests.py` & `alcedo-0.1.7/tests/session/delete/bench_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/delete/bench_requests.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-28 14:24
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/get/bench.py` & `alcedo-0.1.7/tests/session/get/bench.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/get/bench.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-25 02:00
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/get/bench_aiohttp.py` & `alcedo-0.1.7/tests/session/get/bench_aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/get/bench_aiohttp.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-25 02:00
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/get/bench_httpx.py` & `alcedo-0.1.7/tests/session/get/bench_httpx.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/get/bench_httpx.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-25 02:00
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/get/bench_requests.py` & `alcedo-0.1.7/tests/session/get/bench_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/get/bench_requests.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-25 02:00
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/post/bench.py` & `alcedo-0.1.7/tests/session/put/bench.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
-# FILENAME:    ~~/tests/session/post/bench.py
-# VERSION:     0.1.6
-# CREATED:     2024-03-27 16:29
+# FILENAME:    ~~/tests/session/put/bench.py
+# VERSION:     0.1.7
+# CREATED:     2024-03-28 14:18
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
 ### Local modules ###
 from alcedo import Client, Response
 from tests import *
 
 
-def test_alcedo_client_post_create() -> None:
+def test_alcedo_client_put_update_endpoint() -> None:
   client: Client = Client()
   for i in range(RUNS):
     body: dict = {"hello": "world", "count": i + 1}
-    response: Response = client.post(f"{ TEST_ENDPOINT }/create", payload=body)
-    assert response.json() == {"created": body}
+    response: Response = client.put(f"{ TEST_ENDPOINT }/update", payload=body)
+    assert response.json() == {"updated": body}
```

### Comparing `alcedo-0.1.6/tests/session/post/bench_aiohttp.py` & `alcedo-0.1.7/tests/session/post/bench_aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/post/bench_aiohttp.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-25 02:00
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/post/bench_httpx.py` & `alcedo-0.1.7/tests/session/post/bench_httpx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/post/bench_httpx.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-27 20:58
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/post/bench_requests.py` & `alcedo-0.1.7/tests/session/post/bench_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/post/bench_requests.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-27 19:25
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/put/bench.py` & `alcedo-0.1.7/tests/session/post/bench.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
-# FILENAME:    ~~/tests/session/put/bench.py
-# VERSION:     0.1.6
-# CREATED:     2024-03-28 14:18
+# FILENAME:    ~~/tests/session/post/bench.py
+# VERSION:     0.1.7
+# CREATED:     2024-03-27 16:29
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
 ### Local modules ###
 from alcedo import Client, Response
 from tests import *
 
 
-def test_alcedo_client_put_update_endpoint() -> None:
+def test_alcedo_client_post_create() -> None:
   client: Client = Client()
   for i in range(RUNS):
     body: dict = {"hello": "world", "count": i + 1}
-    response: Response = client.put(f"{ TEST_ENDPOINT }/update", payload=body)
-    assert response.json() == {"updated": body}
+    response: Response = client.post(f"{ TEST_ENDPOINT }/create", payload=body)
+    assert response.json() == {"created": body}
```

### Comparing `alcedo-0.1.6/tests/session/put/bench_aiohttp.py` & `alcedo-0.1.7/tests/session/put/bench_aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/put/bench_aiohttp.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-28 14:18
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/put/bench_httpx.py` & `alcedo-0.1.7/tests/session/put/bench_httpx.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/put/bench_httpx.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-28 14:18
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/put/bench_requests.py` & `alcedo-0.1.7/tests/session/put/bench_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/put/bench_requests.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-03-28 14:18
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/queried_get/__init__.py` & `alcedo-0.1.7/tests/session/queried_get/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/queried_get/__init__.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-04-01 08:07
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION: https://www.w3docs.com/snippets/python/what-is-init-py-for.html
 #
 # HISTORY:
 # *************************************************************
 """
```

### Comparing `alcedo-0.1.6/tests/session/queried_get/bench.py` & `alcedo-0.1.7/tests/session/queried_get/bench.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/queried_get/bench.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-04-01 08:07
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/queried_get/bench_aiohttp.py` & `alcedo-0.1.7/tests/session/queried_get/bench_aiohttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/queried_get/bench_aiohttp.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-04-01 08:07
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/queried_get/bench_httpx.py` & `alcedo-0.1.7/tests/session/queried_get/bench_httpx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/queried_get/bench_httpx.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-04-01 08:07
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/tests/session/queried_get/bench_requests.py` & `alcedo-0.1.7/tests/session/queried_get/bench_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/queried_get/bench_requests.py
-# VERSION:     0.1.6
+# VERSION:     0.1.7
 # CREATED:     2024-04-01 08:07
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `alcedo-0.1.6/Cargo.lock` & `alcedo-0.1.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "alcedo"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "pyo3",
  "reqwest",
  "serde",
  "serde_derive",
  "serde_json",
 ]
```

### Comparing `alcedo-0.1.6/PKG-INFO` & `alcedo-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcedo
-Version: 0.1.6
+Version: 0.1.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Rust
```

