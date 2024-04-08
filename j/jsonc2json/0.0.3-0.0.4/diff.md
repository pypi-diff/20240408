# Comparing `tmp/jsonc2json-0.0.3.tar.gz` & `tmp/jsonc2json-0.0.4.tar.gz`

## Comparing `jsonc2json-0.0.3.tar` & `jsonc2json-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      235 1970-01-01 00:00:00.000000 jsonc2json-0.0.3/Cargo.toml
--rw-r--r--   0     1001      127     1052 2024-02-20 17:39:44.000000 jsonc2json-0.0.3/README.md
--rw-r--r--   0     1001      127     1578 2024-02-20 17:39:44.000000 jsonc2json-0.0.3/src/lib.rs
--rw-r--r--   0     1001      127     7835 2024-02-20 17:39:44.000000 jsonc2json-0.0.3/Cargo.lock
--rw-r--r--   0     1001      127     1140 2024-02-20 17:39:44.000000 jsonc2json-0.0.3/pyproject.toml
--rw-r--r--   0     1001      127      112 2024-02-20 17:39:44.000000 jsonc2json-0.0.3/python/jsonc2json/_jsonc2json.pyi
--rw-r--r--   0     1001      127      813 2024-02-20 17:39:44.000000 jsonc2json-0.0.3/python/jsonc2json/__main__.py
--rw-r--r--   0     1001      127     2127 2024-02-20 17:39:44.000000 jsonc2json-0.0.3/python/jsonc2json/__init__.py
--rw-r--r--   0     1001      127        0 2024-02-20 17:39:44.000000 jsonc2json-0.0.3/python/jsonc2json/py.typed
--rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 jsonc2json-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      235 1970-01-01 00:00:00.000000 jsonc2json-0.0.4/Cargo.toml
+-rw-r--r--   0     1001      127     1052 2024-04-08 19:26:37.000000 jsonc2json-0.0.4/README.md
+-rw-r--r--   0     1001      127     1839 2024-04-08 19:26:37.000000 jsonc2json-0.0.4/src/lib.rs
+-rw-r--r--   0     1001      127     8076 2024-04-08 19:26:37.000000 jsonc2json-0.0.4/Cargo.lock
+-rw-r--r--   0     1001      127     1161 2024-04-08 19:26:37.000000 jsonc2json-0.0.4/pyproject.toml
+-rw-r--r--   0     1001      127     2127 2024-04-08 19:26:37.000000 jsonc2json-0.0.4/python/jsonc2json/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-08 19:26:37.000000 jsonc2json-0.0.4/python/jsonc2json/py.typed
+-rw-r--r--   0     1001      127      813 2024-04-08 19:26:37.000000 jsonc2json-0.0.4/python/jsonc2json/__main__.py
+-rw-r--r--   0     1001      127      112 2024-04-08 19:26:37.000000 jsonc2json-0.0.4/python/jsonc2json/_jsonc2json.pyi
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 jsonc2json-0.0.4/PKG-INFO
```

### Comparing `jsonc2json-0.0.3/README.md` & `jsonc2json-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jsonc2json-0.0.3/src/lib.rs` & `jsonc2json-0.0.4/src/lib.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,44 @@
+use std::io::{ErrorKind, Read};
+use std::vec::Vec;
+
 use json_comments::StripComments;
+
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
+use pyo3::pybacked::{PyBackedBytes, PyBackedStr};
 use pyo3::types::PyBytes;
-use std::io::{ErrorKind, Read};
-use std::vec::Vec;
 
-// Bytes function
+#[derive(FromPyObject)]
+pub enum BytesOrString {
+    Str(PyBackedStr),
+    Bytes(PyBackedBytes),
+}
+
+/// Strip comments from JSON bytes and return JSON as a bytes object
 #[pyfunction]
-fn jsonc2json_bin<'a>(py: Python<'a>, b: &[u8]) -> PyResult<&'a PyBytes> {
+fn jsonc2json_bin<'a>(py: Python<'a>, b: &[u8]) -> PyResult<Bound<'a, PyBytes>> {
     let mut buf = Vec::new();
     let result = StripComments::new(b).read_to_end(&mut buf);
     match result {
         Ok(_) => {
-            let pbres = PyBytes::new(py, &buf[..]);
-            Ok(pbres)
+            let py_bytes = PyBytes::new_bound(py, &buf);
+            Ok(py_bytes)
         }
         Err(e) => {
             if e.kind() == ErrorKind::InvalidData {
                 Err(PyValueError::new_err("Invalid JSON"))
             } else {
                 Err(PyValueError::new_err("Unknown error"))
             }
         }
     }
 }
 
-// string function
+/// Strip comments from JSON string and return JSON as a string
 #[pyfunction]
 fn jsonc2json_str(string: String) -> PyResult<String> {
     let mut stripped = String::new();
     let result = StripComments::new(string.as_bytes()).read_to_string(&mut stripped);
     match result {
         Ok(_) => Ok(stripped),
         Err(e) => {
@@ -41,13 +50,13 @@
         }
     }
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 #[pyo3(name = "_jsonc2json")]
-fn libjsonc2json(_py: Python, m: &PyModule) -> PyResult<()> {
+fn libjsonc2json(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add("__version_lib__", env!("CARGO_PKG_VERSION"))?;
     m.add_function(wrap_pyfunction!(jsonc2json_str, m)?)?;
     m.add_function(wrap_pyfunction!(jsonc2json_bin, m)?)?;
     Ok(())
 }
```

### Comparing `jsonc2json-0.0.3/Cargo.lock` & `jsonc2json-0.0.4/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 name = "json_comments"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9dbbfed4e59ba9750e15ba154fdfd9329cee16ff3df539c2666b70f58cc32105"
 
 [[package]]
 name = "jsonc2json"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
  "json_comments",
  "pyo3",
 ]
 
 [[package]]
 name = "libc"
@@ -97,79 +97,87 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.35"
```

### Comparing `jsonc2json-0.0.3/pyproject.toml` & `jsonc2json-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [build-system]
 requires = ['maturin>=0.14.16,<2']
 build-backend = "maturin"
 
 [project]
 name = "jsonc2json"
-version = "0.0.3"
+version = "0.0.4"
 description = "jsonc2json ~ convert jsonc 2 json ~ python + rust"
 requires-python = ">=3.8"
 license = "MIT OR Apache-2.0"
 keywords = ["json", "jsonc", "rust", "pyo3"]
-readme = "README.md"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
 ]
 authors = [{ name = "Jesse Rubin", email = "jessekrubin@gmail.com" }]
 maintainers = [{ name = "Jesse Rubin", email = "jessekrubin@gmail.com" }]
+dynamic = [
+    "version",
+    "readme"
+]
 
 [project.urls]
 documentation = "https://github.com/jessekrubin/jsonc2json"
 homepage = "https://github.com/jessekrubin/jsonc2json"
 source = "https://github.com/jessekrubin/jsonc2json"
 
 [tool.maturin]
```

### Comparing `jsonc2json-0.0.3/python/jsonc2json/__main__.py` & `jsonc2json-0.0.4/python/jsonc2json/__main__.py`

 * *Files identical despite different names*

### Comparing `jsonc2json-0.0.3/python/jsonc2json/__init__.py` & `jsonc2json-0.0.4/python/jsonc2json/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonc2json-0.0.3/PKG-INFO` & `jsonc2json-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jsonc2json
-Version: 0.0.3
+Version: 0.0.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Summary: jsonc2json ~ convert jsonc 2 json ~ python + rust
 Keywords: json,jsonc,rust,pyo3
 Author-email: Jesse Rubin <jessekrubin@gmail.com>
```

