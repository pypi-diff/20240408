# Comparing `tmp/granian-1.2.0.tar.gz` & `tmp/granian-1.2.1.tar.gz`

## Comparing `granian-1.2.0.tar` & `granian-1.2.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 granian-1.2.0/Cargo.toml
--rw-r--r--   0     1001      127     1486 2024-03-18 23:30:29.000000 granian-1.2.0/LICENSE
--rw-r--r--   0     1001      127    10711 2024-03-18 23:30:29.000000 granian-1.2.0/README.md
--rw-r--r--   0     1001      127       81 2024-03-18 23:30:29.000000 granian-1.2.0/granian/__init__.py
--rw-r--r--   0     1001      127       36 2024-03-18 23:30:29.000000 granian-1.2.0/granian/__main__.py
--rw-r--r--   0     1001      127      257 2024-03-18 23:30:29.000000 granian-1.2.0/granian/_futures.py
--rw-r--r--   0     1001      127     1571 2024-03-18 23:30:29.000000 granian-1.2.0/granian/_granian.pyi
--rw-r--r--   0     1001      127      143 2024-03-18 23:30:29.000000 granian-1.2.0/granian/_imports.py
--rw-r--r--   0     1001      127     1677 2024-03-18 23:30:29.000000 granian-1.2.0/granian/_internal.py
--rw-r--r--   0     1001      127     2867 2024-03-18 23:30:29.000000 granian-1.2.0/granian/_loops.py
--rw-r--r--   0     1001      127       93 2024-03-18 23:30:29.000000 granian-1.2.0/granian/_types.py
--rw-r--r--   0     1001      127     3895 2024-03-18 23:30:29.000000 granian-1.2.0/granian/asgi.py
--rw-r--r--   0     1001      127     7453 2024-03-18 23:30:29.000000 granian-1.2.0/granian/cli.py
--rw-r--r--   0     1001      127      379 2024-03-18 23:30:29.000000 granian-1.2.0/granian/constants.py
--rw-r--r--   0     1001      127      615 2024-03-18 23:30:29.000000 granian-1.2.0/granian/http.py
--rw-r--r--   0     1001      127     1480 2024-03-18 23:30:29.000000 granian-1.2.0/granian/log.py
--rw-r--r--   0     1001      127      144 2024-03-18 23:30:29.000000 granian-1.2.0/granian/net.py
--rw-r--r--   0     1001      127        0 2024-03-18 23:30:29.000000 granian-1.2.0/granian/py.typed
--rw-r--r--   0     1001      127      745 2024-03-18 23:30:29.000000 granian-1.2.0/granian/rsgi.py
--rw-r--r--   0     1001      127    17780 2024-03-18 23:30:29.000000 granian-1.2.0/granian/server.py
--rw-r--r--   0     1001      127     1281 2024-03-18 23:30:29.000000 granian-1.2.0/granian/wsgi.py
--rw-r--r--   0     1001      127    12664 2024-03-18 23:30:29.000000 granian-1.2.0/src/asgi/callbacks.rs
--rw-r--r--   0     1001      127     2170 2024-03-18 23:30:29.000000 granian-1.2.0/src/asgi/errors.rs
--rw-r--r--   0     1001      127     6352 2024-03-18 23:30:29.000000 granian-1.2.0/src/asgi/http.rs
--rw-r--r--   0     1001      127    21423 2024-03-18 23:30:29.000000 granian-1.2.0/src/asgi/io.rs
--rw-r--r--   0     1001      127      295 2024-03-18 23:30:29.000000 granian-1.2.0/src/asgi/mod.rs
--rw-r--r--   0     1001      127     4719 2024-03-18 23:30:29.000000 granian-1.2.0/src/asgi/serve.rs
--rw-r--r--   0     1001      127      259 2024-03-18 23:30:29.000000 granian-1.2.0/src/asgi/types.rs
--rw-r--r--   0     1001      127     4543 2024-03-18 23:30:29.000000 granian-1.2.0/src/asgi/utils.rs
--rw-r--r--   0     1001      127    13189 2024-03-18 23:30:29.000000 granian-1.2.0/src/callbacks.rs
--rw-r--r--   0     1001      127     2900 2024-03-18 23:30:29.000000 granian-1.2.0/src/conversion.rs
--rw-r--r--   0     1001      127     1345 2024-03-18 23:30:29.000000 granian-1.2.0/src/http.rs
--rw-r--r--   0     1001      127     1298 2024-03-18 23:30:29.000000 granian-1.2.0/src/io.rs
--rw-r--r--   0     1001      127      820 2024-03-18 23:30:29.000000 granian-1.2.0/src/lib.rs
--rw-r--r--   0     1001      127     9701 2024-03-18 23:30:29.000000 granian-1.2.0/src/rsgi/callbacks.rs
--rw-r--r--   0     1001      127      564 2024-03-18 23:30:29.000000 granian-1.2.0/src/rsgi/errors.rs
--rw-r--r--   0     1001      127     5970 2024-03-18 23:30:29.000000 granian-1.2.0/src/rsgi/http.rs
--rw-r--r--   0     1001      127    13201 2024-03-18 23:30:29.000000 granian-1.2.0/src/rsgi/io.rs
--rw-r--r--   0     1001      127      723 2024-03-18 23:30:29.000000 granian-1.2.0/src/rsgi/mod.rs
--rw-r--r--   0     1001      127     4719 2024-03-18 23:30:29.000000 granian-1.2.0/src/rsgi/serve.rs
--rw-r--r--   0     1001      127     8241 2024-03-18 23:30:29.000000 granian-1.2.0/src/rsgi/types.rs
--rw-r--r--   0     1001      127     9459 2024-03-18 23:30:29.000000 granian-1.2.0/src/runtime.rs
--rw-r--r--   0     1001      127     2284 2024-03-18 23:30:29.000000 granian-1.2.0/src/tcp.rs
--rw-r--r--   0     1001      127     1111 2024-03-18 23:30:29.000000 granian-1.2.0/src/tls.rs
--rw-r--r--   0     1001      127     1246 2024-03-18 23:30:29.000000 granian-1.2.0/src/utils.rs
--rw-r--r--   0     1001      127    37189 2024-03-18 23:30:29.000000 granian-1.2.0/src/workers.rs
--rw-r--r--   0     1001      127     4007 2024-03-18 23:30:29.000000 granian-1.2.0/src/ws.rs
--rw-r--r--   0     1001      127     4687 2024-03-18 23:30:29.000000 granian-1.2.0/src/wsgi/callbacks.rs
--rw-r--r--   0     1001      127     1557 2024-03-18 23:30:29.000000 granian-1.2.0/src/wsgi/http.rs
--rw-r--r--   0     1001      127       58 2024-03-18 23:30:29.000000 granian-1.2.0/src/wsgi/mod.rs
--rw-r--r--   0     1001      127     2335 2024-03-18 23:30:29.000000 granian-1.2.0/src/wsgi/serve.rs
--rw-r--r--   0     1001      127     6314 2024-03-18 23:30:29.000000 granian-1.2.0/src/wsgi/types.rs
--rw-r--r--   0     1001      127     4104 2024-03-18 23:30:29.000000 granian-1.2.0/tests/apps/asgi.py
--rw-r--r--   0     1001      127     3140 2024-03-18 23:30:29.000000 granian-1.2.0/tests/apps/rsgi.py
--rw-r--r--   0     1001      127     1123 2024-03-18 23:30:29.000000 granian-1.2.0/tests/apps/wsgi.py
--rw-r--r--   0     1001      127     2402 2024-03-18 23:30:29.000000 granian-1.2.0/tests/conftest.py
--rw-r--r--   0     1001      127       95 2024-03-18 23:30:29.000000 granian-1.2.0/tests/fixtures/media.png
--rw-r--r--   0     1001      127     1139 2024-03-18 23:30:29.000000 granian-1.2.0/tests/fixtures/tls/cert.pem
--rw-r--r--   0     1001      127     1704 2024-03-18 23:30:29.000000 granian-1.2.0/tests/fixtures/tls/key.pem
--rw-r--r--   0     1001      127     2791 2024-03-18 23:30:29.000000 granian-1.2.0/tests/test_asgi.py
--rw-r--r--   0     1001      127     1750 2024-03-18 23:30:29.000000 granian-1.2.0/tests/test_https.py
--rw-r--r--   0     1001      127     2756 2024-03-18 23:30:29.000000 granian-1.2.0/tests/test_rsgi.py
--rw-r--r--   0     1001      127     2611 2024-03-18 23:30:29.000000 granian-1.2.0/tests/test_ws.py
--rw-r--r--   0     1001      127     2300 2024-03-18 23:30:29.000000 granian-1.2.0/tests/test_wsgi.py
--rw-r--r--   0     1001      127    33265 2024-03-18 23:30:29.000000 granian-1.2.0/Cargo.lock
--rw-r--r--   0     1001      127     2904 2024-03-18 23:30:29.000000 granian-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    12889 1970-01-01 00:00:00.000000 granian-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 granian-1.2.1/Cargo.toml
+-rw-r--r--   0     1001      127     1486 2024-04-01 21:50:17.000000 granian-1.2.1/LICENSE
+-rw-r--r--   0     1001      127    10711 2024-04-01 21:50:17.000000 granian-1.2.1/README.md
+-rw-r--r--   0     1001      127       81 2024-04-01 21:50:17.000000 granian-1.2.1/granian/__init__.py
+-rw-r--r--   0     1001      127       36 2024-04-01 21:50:17.000000 granian-1.2.1/granian/__main__.py
+-rw-r--r--   0     1001      127      257 2024-04-01 21:50:17.000000 granian-1.2.1/granian/_futures.py
+-rw-r--r--   0     1001      127     1571 2024-04-01 21:50:17.000000 granian-1.2.1/granian/_granian.pyi
+-rw-r--r--   0     1001      127      143 2024-04-01 21:50:17.000000 granian-1.2.1/granian/_imports.py
+-rw-r--r--   0     1001      127     1677 2024-04-01 21:50:17.000000 granian-1.2.1/granian/_internal.py
+-rw-r--r--   0     1001      127     2867 2024-04-01 21:50:17.000000 granian-1.2.1/granian/_loops.py
+-rw-r--r--   0     1001      127       93 2024-04-01 21:50:17.000000 granian-1.2.1/granian/_types.py
+-rw-r--r--   0     1001      127     3895 2024-04-01 21:50:17.000000 granian-1.2.1/granian/asgi.py
+-rw-r--r--   0     1001      127     7453 2024-04-01 21:50:17.000000 granian-1.2.1/granian/cli.py
+-rw-r--r--   0     1001      127      379 2024-04-01 21:50:17.000000 granian-1.2.1/granian/constants.py
+-rw-r--r--   0     1001      127      615 2024-04-01 21:50:17.000000 granian-1.2.1/granian/http.py
+-rw-r--r--   0     1001      127     1480 2024-04-01 21:50:17.000000 granian-1.2.1/granian/log.py
+-rw-r--r--   0     1001      127      144 2024-04-01 21:50:17.000000 granian-1.2.1/granian/net.py
+-rw-r--r--   0     1001      127        0 2024-04-01 21:50:17.000000 granian-1.2.1/granian/py.typed
+-rw-r--r--   0     1001      127      745 2024-04-01 21:50:17.000000 granian-1.2.1/granian/rsgi.py
+-rw-r--r--   0     1001      127    17839 2024-04-01 21:50:17.000000 granian-1.2.1/granian/server.py
+-rw-r--r--   0     1001      127     1281 2024-04-01 21:50:17.000000 granian-1.2.1/granian/wsgi.py
+-rw-r--r--   0     1001      127    12664 2024-04-01 21:50:17.000000 granian-1.2.1/src/asgi/callbacks.rs
+-rw-r--r--   0     1001      127     2170 2024-04-01 21:50:17.000000 granian-1.2.1/src/asgi/errors.rs
+-rw-r--r--   0     1001      127     6352 2024-04-01 21:50:17.000000 granian-1.2.1/src/asgi/http.rs
+-rw-r--r--   0     1001      127    22164 2024-04-01 21:50:17.000000 granian-1.2.1/src/asgi/io.rs
+-rw-r--r--   0     1001      127      295 2024-04-01 21:50:17.000000 granian-1.2.1/src/asgi/mod.rs
+-rw-r--r--   0     1001      127     4719 2024-04-01 21:50:17.000000 granian-1.2.1/src/asgi/serve.rs
+-rw-r--r--   0     1001      127      259 2024-04-01 21:50:17.000000 granian-1.2.1/src/asgi/types.rs
+-rw-r--r--   0     1001      127     4543 2024-04-01 21:50:17.000000 granian-1.2.1/src/asgi/utils.rs
+-rw-r--r--   0     1001      127    13165 2024-04-01 21:50:17.000000 granian-1.2.1/src/callbacks.rs
+-rw-r--r--   0     1001      127     2900 2024-04-01 21:50:17.000000 granian-1.2.1/src/conversion.rs
+-rw-r--r--   0     1001      127     1345 2024-04-01 21:50:17.000000 granian-1.2.1/src/http.rs
+-rw-r--r--   0     1001      127     1298 2024-04-01 21:50:17.000000 granian-1.2.1/src/io.rs
+-rw-r--r--   0     1001      127      820 2024-04-01 21:50:17.000000 granian-1.2.1/src/lib.rs
+-rw-r--r--   0     1001      127     9701 2024-04-01 21:50:17.000000 granian-1.2.1/src/rsgi/callbacks.rs
+-rw-r--r--   0     1001      127      564 2024-04-01 21:50:17.000000 granian-1.2.1/src/rsgi/errors.rs
+-rw-r--r--   0     1001      127     5970 2024-04-01 21:50:17.000000 granian-1.2.1/src/rsgi/http.rs
+-rw-r--r--   0     1001      127    13155 2024-04-01 21:50:17.000000 granian-1.2.1/src/rsgi/io.rs
+-rw-r--r--   0     1001      127      723 2024-04-01 21:50:17.000000 granian-1.2.1/src/rsgi/mod.rs
+-rw-r--r--   0     1001      127     4719 2024-04-01 21:50:17.000000 granian-1.2.1/src/rsgi/serve.rs
+-rw-r--r--   0     1001      127     8689 2024-04-01 21:50:17.000000 granian-1.2.1/src/rsgi/types.rs
+-rw-r--r--   0     1001      127     9459 2024-04-01 21:50:17.000000 granian-1.2.1/src/runtime.rs
+-rw-r--r--   0     1001      127     2284 2024-04-01 21:50:17.000000 granian-1.2.1/src/tcp.rs
+-rw-r--r--   0     1001      127     1111 2024-04-01 21:50:17.000000 granian-1.2.1/src/tls.rs
+-rw-r--r--   0     1001      127     1246 2024-04-01 21:50:17.000000 granian-1.2.1/src/utils.rs
+-rw-r--r--   0     1001      127    37189 2024-04-01 21:50:17.000000 granian-1.2.1/src/workers.rs
+-rw-r--r--   0     1001      127     4007 2024-04-01 21:50:17.000000 granian-1.2.1/src/ws.rs
+-rw-r--r--   0     1001      127     4687 2024-04-01 21:50:17.000000 granian-1.2.1/src/wsgi/callbacks.rs
+-rw-r--r--   0     1001      127     1557 2024-04-01 21:50:17.000000 granian-1.2.1/src/wsgi/http.rs
+-rw-r--r--   0     1001      127       58 2024-04-01 21:50:17.000000 granian-1.2.1/src/wsgi/mod.rs
+-rw-r--r--   0     1001      127     2335 2024-04-01 21:50:17.000000 granian-1.2.1/src/wsgi/serve.rs
+-rw-r--r--   0     1001      127     6314 2024-04-01 21:50:17.000000 granian-1.2.1/src/wsgi/types.rs
+-rw-r--r--   0     1001      127     4104 2024-04-01 21:50:17.000000 granian-1.2.1/tests/apps/asgi.py
+-rw-r--r--   0     1001      127     3140 2024-04-01 21:50:17.000000 granian-1.2.1/tests/apps/rsgi.py
+-rw-r--r--   0     1001      127     1123 2024-04-01 21:50:17.000000 granian-1.2.1/tests/apps/wsgi.py
+-rw-r--r--   0     1001      127     2434 2024-04-01 21:50:17.000000 granian-1.2.1/tests/conftest.py
+-rw-r--r--   0     1001      127       95 2024-04-01 21:50:17.000000 granian-1.2.1/tests/fixtures/media.png
+-rw-r--r--   0     1001      127     1139 2024-04-01 21:50:17.000000 granian-1.2.1/tests/fixtures/tls/cert.pem
+-rw-r--r--   0     1001      127     1704 2024-04-01 21:50:17.000000 granian-1.2.1/tests/fixtures/tls/key.pem
+-rw-r--r--   0     1001      127     2791 2024-04-01 21:50:17.000000 granian-1.2.1/tests/test_asgi.py
+-rw-r--r--   0     1001      127     1750 2024-04-01 21:50:17.000000 granian-1.2.1/tests/test_https.py
+-rw-r--r--   0     1001      127     2756 2024-04-01 21:50:17.000000 granian-1.2.1/tests/test_rsgi.py
+-rw-r--r--   0     1001      127     2611 2024-04-01 21:50:17.000000 granian-1.2.1/tests/test_ws.py
+-rw-r--r--   0     1001      127     2300 2024-04-01 21:50:17.000000 granian-1.2.1/tests/test_wsgi.py
+-rw-r--r--   0     1001      127    33265 2024-04-01 21:50:17.000000 granian-1.2.1/Cargo.lock
+-rw-r--r--   0     1001      127     2904 2024-04-01 21:50:17.000000 granian-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12889 1970-01-01 00:00:00.000000 granian-1.2.1/PKG-INFO
```

### Comparing `granian-1.2.0/Cargo.toml` & `granian-1.2.1/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "granian"
-version = "1.2.0"
+version = "1.2.1"
 description = "A Rust HTTP server for Python applications"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 edition = "2021"
 
 keywords = ["web", "asyncio"]
 
@@ -42,15 +42,15 @@
 pin-project = "1.1"
 pyo3 = { version = "=0.20", features = ["anyhow", "extension-module", "generate-import-lib"] }
 pyo3-asyncio = { version = "=0.20", features = ["tokio-runtime"], git = "https://github.com/gi0baro/pyo3-asyncio.git", rev = "6e3a309" }
 pyo3-log = "=0.8"
 rustls-pemfile = "2.1"
 socket2 = { version = "0.5", features = ["all"] }
 tls-listener = { version = "=0.9", features = ["rustls"] }
-tokio = { version = "1.24", features = ["full"] }
+tokio = { version = "1.37", features = ["full"] }
 tokio-stream = "0.1"
 tokio-tungstenite = "=0.21"
 tokio-util = { version = "0.7", features = ["codec"] }
 
 [profile.release]
 codegen-units = 1
 debug = false
```

### Comparing `granian-1.2.0/LICENSE` & `granian-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/README.md` & `granian-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/granian/_granian.pyi` & `granian-1.2.1/granian/_granian.pyi`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/granian/_internal.py` & `granian-1.2.1/granian/_internal.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/granian/_loops.py` & `granian-1.2.1/granian/_loops.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/granian/asgi.py` & `granian-1.2.1/granian/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/granian/cli.py` & `granian-1.2.1/granian/cli.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/granian/http.py` & `granian-1.2.1/granian/http.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/granian/log.py` & `granian-1.2.1/granian/log.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/granian/rsgi.py` & `granian-1.2.1/granian/rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/granian/server.py` & `granian-1.2.1/granian/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,15 +403,16 @@
     def startup(self, spawn_target, target_loader):
         logger.info(f'Starting granian (main PID: {os.getpid()})')
 
         self.setup_signals()
         self._init_shared_socket()
         sock = socket.socket(fileno=self._sfd)
         sock.set_inheritable(True)
-        logger.info(f'Listening at: {self.bind_addr}:{self.bind_port}')
+        proto = 'https' if self.ssl_ctx[0] else 'http'
+        logger.info(f'Listening at: {proto}://{self.bind_addr}:{self.bind_port}')
 
         self._spawn_workers(sock, spawn_target, target_loader)
         return sock
 
     def shutdown(self, exit_code=0):
         logger.info('Shutting down granian')
         self._stop_workers()
@@ -504,15 +505,15 @@
             if self.interface == Interfaces.WSGI:
                 logger.info('Websockets are not supported on WSGI')
             if self.http == HTTPModes.http2:
                 logger.info('Websockets are not supported on HTTP/2 only')
 
         if setproctitle is not None:
             self.process_name = self.process_name or (
-                f'granian {self.interface.value} {self.bind_addr}:{self.bind_port} {self.target}'
+                f'granian {self.interface} {self.bind_addr}:{self.bind_port} {self.target}'
             )
             setproctitle.setproctitle(self.process_name)
         elif self.process_name is not None:
             logger.error('Setting process name requires the granian[pname] extra')
             sys.exit(1)
 
         serve_method = self._serve_with_reloader if self.reload_on_changes else self._serve
```

### Comparing `granian-1.2.0/granian/wsgi.py` & `granian-1.2.1/granian/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/asgi/callbacks.rs` & `granian-1.2.1/src/asgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/asgi/errors.rs` & `granian-1.2.1/src/asgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/asgi/http.rs` & `granian-1.2.1/src/asgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/asgi/io.rs` & `granian-1.2.1/src/asgi/io.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 use futures::{sink::SinkExt, StreamExt, TryStreamExt};
 use http_body_util::BodyExt;
 use hyper::{
     body,
     header::{HeaderMap, HeaderName, HeaderValue, SERVER as HK_SERVER},
     Response, StatusCode,
 };
-use pyo3::prelude::*;
-use pyo3::types::{PyBytes, PyDict};
+use pyo3::{
+    prelude::*,
+    types::{PyBytes, PyDict},
+};
 use std::{
     borrow::Cow,
     sync::{atomic, Arc, Mutex, RwLock},
 };
 use tokio::{
     fs::File,
     sync::{mpsc, oneshot, Mutex as AsyncMutex},
@@ -74,20 +76,28 @@
 
     #[inline]
     fn send_body<'p>(
         &self,
         py: Python<'p>,
         tx: mpsc::Sender<Result<body::Bytes, anyhow::Error>>,
         body: Box<[u8]>,
+        close: bool,
     ) -> PyResult<&'p PyAny> {
+        let flow_hld = self.flow_tx_waiter.clone();
         future_into_py_futlike(self.rt.clone(), py, async move {
             match tx.send(Ok(body.into())).await {
-                Ok(()) => Ok(()),
+                Ok(()) => {
+                    if close {
+                        flow_hld.notify_one();
+                    }
+                    Ok(())
+                }
                 Err(err) => {
                     log::warn!("ASGI transport tx error: {:?}", err);
+                    flow_hld.notify_one();
                     error_transport!()
                 }
             }
         })
     }
 
     pub fn tx(&self) -> Option<oneshot::Sender<HTTPResponse>> {
@@ -95,52 +105,62 @@
     }
 }
 
 #[pymethods]
 impl ASGIHTTPProtocol {
     fn receive<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
         if *self.flow_rx_exhausted.read().unwrap() {
-            let holder = self.flow_tx_waiter.clone();
+            let flow_hld = self.flow_tx_waiter.clone();
             return future_into_py_futlike(self.rt.clone(), py, async move {
-                let () = holder.notified().await;
+                let () = flow_hld.notified().await;
                 Python::with_gil(|py| {
                     let dict = PyDict::new(py);
                     dict.set_item(pyo3::intern!(py, "type"), pyo3::intern!(py, "http.disconnect"))?;
                     Ok(dict.to_object(py))
                 })
             });
         }
 
         let body_ref = self.request_body.clone();
         let flow_ref = self.flow_rx_exhausted.clone();
+        let flow_hld = self.flow_tx_waiter.clone();
         future_into_py_iter(self.rt.clone(), py, async move {
             let mut bodym = body_ref.lock().await;
             let body = &mut *bodym;
             let mut more_body = false;
             let chunk = match body.next().await {
-                Some(chunk) => {
+                Some(Ok(buf)) => {
                     more_body = true;
-                    chunk
-                        .map(|buf| buf.into_data().unwrap_or_default())
-                        .unwrap_or(body::Bytes::new())
+                    Ok(buf.into_data().unwrap_or_default())
                 }
-                _ => body::Bytes::new(),
+                Some(Err(err)) => Err(err),
+                _ => Ok(body::Bytes::new()),
             };
             if !more_body {
                 let mut flow = flow_ref.write().unwrap();
                 *flow = true;
             }
 
-            Python::with_gil(|py| {
-                let dict = PyDict::new(py);
-                dict.set_item(pyo3::intern!(py, "type"), pyo3::intern!(py, "http.request"))?;
-                dict.set_item(pyo3::intern!(py, "body"), BytesToPy(chunk))?;
-                dict.set_item(pyo3::intern!(py, "more_body"), more_body)?;
-                Ok(dict.to_object(py))
-            })
+            match chunk {
+                Ok(data) => Python::with_gil(|py| {
+                    let dict = PyDict::new(py);
+                    dict.set_item(pyo3::intern!(py, "type"), pyo3::intern!(py, "http.request"))?;
+                    dict.set_item(pyo3::intern!(py, "body"), BytesToPy(data))?;
+                    dict.set_item(pyo3::intern!(py, "more_body"), more_body)?;
+                    Ok(dict.to_object(py))
+                }),
+                _ => {
+                    flow_hld.notify_one();
+                    Python::with_gil(|py| {
+                        let dict = PyDict::new(py);
+                        dict.set_item(pyo3::intern!(py, "type"), pyo3::intern!(py, "http.disconnect"))?;
+                        Ok(dict.to_object(py))
+                    })
+                }
+            }
         })
     }
 
     fn send<'p>(&self, py: Python<'p>, data: &'p PyDict) -> PyResult<&'p PyAny> {
         match adapt_message_type(py, data) {
             Ok(ASGIMessageType::HTTPStart(intent)) => match self.response_started.load(atomic::Ordering::Relaxed) {
                 false => {
@@ -174,31 +194,31 @@
                         let (status, headers) = self.response_intent.lock().unwrap().take().unwrap();
                         let (body_tx, body_rx) = mpsc::channel::<Result<body::Bytes, anyhow::Error>>(1);
                         let body_stream = http_body_util::StreamBody::new(
                             tokio_stream::wrappers::ReceiverStream::new(body_rx).map_ok(hyper::body::Frame::data),
                         );
                         *self.body_tx.lock().unwrap() = Some(body_tx.clone());
                         self.send_response(status, headers, BodyExt::boxed(body_stream));
-                        self.send_body(py, body_tx, body)
+                        self.send_body(py, body_tx, body, false)
                     }
                     (true, true, true) => match &*self.body_tx.lock().unwrap() {
                         Some(tx) => {
                             let tx = tx.clone();
-                            self.send_body(py, tx, body)
+                            self.send_body(py, tx, body, false)
                         }
                         _ => error_flow!(),
                     },
                     (true, false, true) => match self.body_tx.lock().unwrap().take() {
-                        Some(tx) => {
-                            self.flow_tx_waiter.notify_one();
-                            match body.is_empty() {
-                                false => self.send_body(py, tx, body),
-                                true => empty_future_into_py(py),
+                        Some(tx) => match body.is_empty() {
+                            false => self.send_body(py, tx, body, true),
+                            true => {
+                                self.flow_tx_waiter.notify_one();
+                                empty_future_into_py(py)
                             }
-                        }
+                        },
                         _ => error_flow!(),
                     },
                     _ => error_flow!(),
                 }
             }
             Ok(ASGIMessageType::HTTPFile(file_path)) => match (
                 self.response_started.load(atomic::Ordering::Relaxed),
@@ -432,15 +452,15 @@
                     adapt_status_code(py, message)?,
                     adapt_headers(py, message),
                 ))),
                 "http.response.body" => Ok(ASGIMessageType::HTTPBody(adapt_body(py, message))),
                 "http.response.pathsend" => Ok(ASGIMessageType::HTTPFile(adapt_file(py, message)?)),
                 "websocket.accept" => {
                     let subproto: Option<String> = match message.get_item(pyo3::intern!(py, "subprotocol")) {
-                        Ok(Some(item)) => item.extract::<String>().map(Some)?,
+                        Ok(Some(item)) => item.extract::<String>().map(Some).unwrap_or(None),
                         _ => None,
                     };
                     Ok(ASGIMessageType::WSAccept(subproto))
                 }
                 "websocket.close" => Ok(ASGIMessageType::WSClose),
                 "websocket.send" => Ok(ASGIMessageType::WSMessage(ws_message_into_rs(py, message)?)),
                 _ => error_message!(),
```

### Comparing `granian-1.2.0/src/asgi/serve.rs` & `granian-1.2.1/src/asgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/asgi/utils.rs` & `granian-1.2.1/src/asgi/utils.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/callbacks.rs` & `granian-1.2.1/src/callbacks.rs`

 * *Files 1% similar despite different names*

```diff
@@ -260,17 +260,16 @@
 }
 
 #[pyclass(frozen)]
 pub(crate) struct PyFutureResultSetter;
 
 #[pymethods]
 impl PyFutureResultSetter {
-    pub fn __call__(&self, target: &PyAny, value: &PyAny) -> PyResult<()> {
-        target.call1((value,))?;
-        Ok(())
+    pub fn __call__(&self, target: &PyAny, value: &PyAny) {
+        let _ = target.call1((value,));
     }
 }
 
 fn contextvars(py: Python) -> PyResult<&PyAny> {
     Ok(CONTEXTVARS
         .get_or_try_init(py, || py.import("contextvars").map(std::convert::Into::into))?
         .as_ref(py))
```

### Comparing `granian-1.2.0/src/conversion.rs` & `granian-1.2.1/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/http.rs` & `granian-1.2.1/src/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/io.rs` & `granian-1.2.1/src/io.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/lib.rs` & `granian-1.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/rsgi/callbacks.rs` & `granian-1.2.1/src/rsgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/rsgi/errors.rs` & `granian-1.2.1/src/rsgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/rsgi/http.rs` & `granian-1.2.1/src/rsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/rsgi/io.rs` & `granian-1.2.1/src/rsgi/io.rs`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 use super::{
     errors::{error_proto, error_stream},
     types::{PyResponse, PyResponseBody, PyResponseFile},
 };
 use crate::{
     conversion::BytesToPy,
-    // http::HTTPRequest,
     runtime::{future_into_py_futlike, future_into_py_iter, Runtime, RuntimeRef},
     ws::{HyperWebsocket, UpgradeData, WSRxStream, WSStream, WSTxStream},
 };
 
 pub(crate) type WebsocketDetachedTransport = (i32, bool, Option<tokio::task::JoinHandle<()>>);
 
 #[pyclass(frozen, module = "granian._granian")]
@@ -119,43 +118,43 @@
             }
             error_proto!()
         })?;
         Ok(Some(pyfut))
     }
 
     #[pyo3(signature = (status=200, headers=vec![]))]
-    fn response_empty(&self, status: u16, headers: Vec<(String, String)>) {
+    fn response_empty(&self, status: u16, headers: Vec<(&str, &str)>) {
         if let Some(tx) = self.tx.lock().unwrap().take() {
             let _ = tx.send(PyResponse::Body(PyResponseBody::empty(status, headers)));
         }
     }
 
     #[pyo3(signature = (status=200, headers=vec![], body=vec![].into()))]
-    fn response_bytes(&self, status: u16, headers: Vec<(String, String)>, body: Cow<[u8]>) {
+    fn response_bytes(&self, status: u16, headers: Vec<(&str, &str)>, body: Cow<[u8]>) {
         if let Some(tx) = self.tx.lock().unwrap().take() {
             let _ = tx.send(PyResponse::Body(PyResponseBody::from_bytes(status, headers, body)));
         }
     }
 
     #[pyo3(signature = (status=200, headers=vec![], body=String::new()))]
-    fn response_str(&self, status: u16, headers: Vec<(String, String)>, body: String) {
+    fn response_str(&self, status: u16, headers: Vec<(&str, &str)>, body: String) {
         if let Some(tx) = self.tx.lock().unwrap().take() {
             let _ = tx.send(PyResponse::Body(PyResponseBody::from_string(status, headers, body)));
         }
     }
 
     #[pyo3(signature = (status, headers, file))]
-    fn response_file(&self, status: u16, headers: Vec<(String, String)>, file: String) {
+    fn response_file(&self, status: u16, headers: Vec<(&str, &str)>, file: String) {
         if let Some(tx) = self.tx.lock().unwrap().take() {
             let _ = tx.send(PyResponse::File(PyResponseFile::new(status, headers, file)));
         }
     }
 
     #[pyo3(signature = (status=200, headers=vec![]))]
-    fn response_stream<'p>(&self, py: Python<'p>, status: u16, headers: Vec<(String, String)>) -> PyResult<&'p PyAny> {
+    fn response_stream<'p>(&self, py: Python<'p>, status: u16, headers: Vec<(&str, &str)>) -> PyResult<&'p PyAny> {
         if let Some(tx) = self.tx.lock().unwrap().take() {
             let (body_tx, body_rx) = mpsc::channel::<Result<body::Bytes, anyhow::Error>>(1);
             let body_stream = http_body_util::StreamBody::new(
                 tokio_stream::wrappers::ReceiverStream::new(body_rx).map_ok(hyper::body::Frame::data),
             );
             let _ = tx.send(PyResponse::Body(PyResponseBody::new(
                 status,
```

### Comparing `granian-1.2.0/src/rsgi/mod.rs` & `granian-1.2.1/src/rsgi/mod.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/rsgi/serve.rs` & `granian-1.2.1/src/rsgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/rsgi/types.rs` & `granian-1.2.1/src/rsgi/types.rs`

 * *Files 15% similar despite different names*

```diff
@@ -103,18 +103,16 @@
     ($name:ident, $proto:expr) => {
         #[pyclass(frozen, module = "granian._granian")]
         pub(crate) struct $name {
             http_version: Version,
             scheme: Arc<str>,
             method: Method,
             uri: Uri,
-            #[pyo3(get)]
-            server: String,
-            #[pyo3(get)]
-            client: String,
+            server: SocketAddr,
+            client: SocketAddr,
             #[pyo3(get)]
             headers: RSGIHeaders,
         }
 
         impl $name {
             pub fn new(
                 http_version: Version,
@@ -126,16 +124,16 @@
                 headers: HeaderMap,
             ) -> Self {
                 Self {
                     http_version,
                     scheme: scheme.into(),
                     method,
                     uri,
-                    server: server.to_string(),
-                    client: client.to_string(),
+                    server,
+                    client,
                     headers: RSGIHeaders::new(headers),
                 }
             }
         }
 
         #[pymethods]
         impl $name {
@@ -156,14 +154,24 @@
                     Version::HTTP_11 => "1.1",
                     Version::HTTP_2 => "2",
                     Version::HTTP_3 => "3",
                     _ => "1",
                 }
             }
 
+            #[getter(server)]
+            fn get_server(&self) -> String {
+                self.server.to_string()
+            }
+
+            #[getter(client)]
+            fn get_client(&self) -> String {
+                self.client.to_string()
+            }
+
             #[getter(scheme)]
             fn get_scheme(&self) -> &str {
                 &self.scheme
             }
 
             #[getter(method)]
             fn get_method(&self) -> &str {
@@ -193,100 +201,104 @@
 
 pub(crate) enum PyResponse {
     Body(PyResponseBody),
     File(PyResponseFile),
 }
 
 pub(crate) struct PyResponseBody {
-    status: u16,
-    headers: Vec<(String, String)>,
+    status: hyper::StatusCode,
+    headers: HeaderMap,
     body: HTTPResponseBody,
 }
 
 pub(crate) struct PyResponseFile {
-    status: u16,
-    headers: Vec<(String, String)>,
+    status: hyper::StatusCode,
+    headers: HeaderMap,
     file_path: String,
 }
 
-macro_rules! response_head_from_py {
-    ($status:expr, $headers:expr, $res:expr) => {{
-        let mut rh = hyper::http::HeaderMap::new();
-
-        rh.insert(HK_SERVER, HV_SERVER);
+macro_rules! headers_from_py {
+    ($headers:expr) => {{
+        let mut headers = HeaderMap::with_capacity($headers.len() + 3);
+        headers.insert(HK_SERVER, HV_SERVER);
         for (key, value) in $headers {
-            rh.append(
-                HeaderName::from_bytes(key.as_bytes()).unwrap(),
-                HeaderValue::from_str(&value).unwrap(),
+            headers.append(
+                HeaderName::try_from(key).unwrap(),
+                HeaderValue::from_str(value).unwrap(),
             );
         }
-
-        *$res.status_mut() = $status.try_into().unwrap();
-        *$res.headers_mut() = rh;
+        headers
     }};
 }
 
 impl PyResponseBody {
-    pub fn new(status: u16, headers: Vec<(String, String)>, body: HTTPResponseBody) -> Self {
-        Self { status, headers, body }
+    pub fn new(status: u16, headers: Vec<(&str, &str)>, body: HTTPResponseBody) -> Self {
+        Self {
+            status: status.try_into().unwrap(),
+            headers: headers_from_py!(headers),
+            body,
+        }
     }
 
-    pub fn empty(status: u16, headers: Vec<(String, String)>) -> Self {
+    pub fn empty(status: u16, headers: Vec<(&str, &str)>) -> Self {
         Self {
-            status,
-            headers,
+            status: status.try_into().unwrap(),
+            headers: headers_from_py!(headers),
             body: empty_body(),
         }
     }
 
-    pub fn from_bytes(status: u16, headers: Vec<(String, String)>, body: Cow<[u8]>) -> Self {
+    pub fn from_bytes(status: u16, headers: Vec<(&str, &str)>, body: Cow<[u8]>) -> Self {
         let rbody: Box<[u8]> = body.into();
         Self {
-            status,
-            headers,
+            status: status.try_into().unwrap(),
+            headers: headers_from_py!(headers),
             body: http_body_util::Full::new(Bytes::from(rbody))
                 .map_err(|e| match e {})
                 .boxed(),
         }
     }
 
-    pub fn from_string(status: u16, headers: Vec<(String, String)>, body: String) -> Self {
+    pub fn from_string(status: u16, headers: Vec<(&str, &str)>, body: String) -> Self {
         Self {
-            status,
-            headers,
+            status: status.try_into().unwrap(),
+            headers: headers_from_py!(headers),
             body: http_body_util::Full::new(Bytes::from(body))
                 .map_err(|e| match e {})
                 .boxed(),
         }
     }
 
     #[inline]
     pub fn to_response(self) -> hyper::Response<HTTPResponseBody> {
         let mut res = hyper::Response::new(self.body);
-        response_head_from_py!(self.status, &self.headers, res);
+        *res.status_mut() = self.status;
+        *res.headers_mut() = self.headers;
         res
     }
 }
 
 impl PyResponseFile {
-    pub fn new(status: u16, headers: Vec<(String, String)>, file_path: String) -> Self {
+    pub fn new(status: u16, headers: Vec<(&str, &str)>, file_path: String) -> Self {
         Self {
-            status,
-            headers,
+            status: status.try_into().unwrap(),
+            headers: headers_from_py!(headers),
             file_path,
         }
     }
 
-    pub async fn to_response(&self) -> hyper::Response<HTTPResponseBody> {
+    #[inline]
+    pub async fn to_response(self) -> hyper::Response<HTTPResponseBody> {
         match File::open(&self.file_path).await {
             Ok(file) => {
                 let stream = ReaderStream::new(file);
                 let stream_body = http_body_util::StreamBody::new(stream.map_ok(hyper::body::Frame::data));
                 let mut res = hyper::Response::new(BodyExt::map_err(stream_body, std::convert::Into::into).boxed());
-                response_head_from_py!(self.status, &self.headers, res);
+                *res.status_mut() = self.status;
+                *res.headers_mut() = self.headers;
                 res
             }
             Err(_) => {
                 log::info!("Cannot open file {}", &self.file_path);
                 response_404()
             }
         }
```

### Comparing `granian-1.2.0/src/runtime.rs` & `granian-1.2.1/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/tcp.rs` & `granian-1.2.1/src/tcp.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/tls.rs` & `granian-1.2.1/src/tls.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/utils.rs` & `granian-1.2.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/workers.rs` & `granian-1.2.1/src/workers.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/ws.rs` & `granian-1.2.1/src/ws.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/wsgi/callbacks.rs` & `granian-1.2.1/src/wsgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/wsgi/http.rs` & `granian-1.2.1/src/wsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/wsgi/serve.rs` & `granian-1.2.1/src/wsgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/src/wsgi/types.rs` & `granian-1.2.1/src/wsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/tests/apps/asgi.py` & `granian-1.2.1/tests/apps/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/tests/apps/rsgi.py` & `granian-1.2.1/tests/apps/rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/tests/apps/wsgi.py` & `granian-1.2.1/tests/apps/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/tests/conftest.py` & `granian-1.2.1/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 import asyncio
+import multiprocessing as mp
 import os
 import socket
 from contextlib import asynccontextmanager, closing
 from functools import partial
 from pathlib import Path
 
 import pytest
 
+from granian import Granian
+
+
+def _serve(**kwargs):
+    server = Granian(f'tests.apps.{kwargs["interface"]}:app', **kwargs)
+    server.serve()
+
 
 @asynccontextmanager
 async def _server(interface, port, threading_mode, tls=False):
     certs_path = Path.cwd() / 'tests' / 'fixtures' / 'tls'
-    tls_opts = (
-        (f"--ssl-certificate {certs_path / 'cert.pem'} " f"--ssl-keyfile {certs_path / 'key.pem'} ") if tls else ''
-    )
-    cmd = ''.join(
-        [
-            f'granian --interface {interface} --port {port} ',
-            f'--threads 1 --threading-mode {threading_mode} ',
-            tls_opts,
-            '--opt ' if os.getenv('LOOP_OPT') else '',
-            f'tests.apps.{interface}:app',
-        ]
-    )
+    kwargs = {
+        'interface': interface,
+        'port': port,
+        'threading_mode': threading_mode,
+        'loop_opt': bool(os.getenv('LOOP_OPT')),
+    }
+    if tls:
+        kwargs['ssl_cert'] = certs_path / 'cert.pem'
+        kwargs['ssl_key'] = certs_path / 'key.pem'
 
     succeeded, spawn_failures = False, 0
     while spawn_failures < 3:
-        proc = await asyncio.create_subprocess_shell(cmd, env=dict(os.environ))
+        proc = mp.get_context('spawn').Process(target=_serve, kwargs=kwargs)
+        proc.start()
+
         conn_failures = 0
         while conn_failures < 3:
             try:
                 await asyncio.sleep(1.5)
                 sock = socket.create_connection(('127.0.0.1', port), timeout=1)
                 sock.close()
                 succeeded = True
                 break
             except Exception:
                 conn_failures += 1
         if succeeded:
             break
 
         proc.terminate()
-        await proc.wait()
+        proc.join()
         spawn_failures += 1
 
     if not succeeded:
         raise RuntimeError('Cannot bind server')
 
     try:
         yield port
     finally:
         proc.terminate()
-        await proc.wait()
+        proc.join()
 
 
 @pytest.fixture(scope='function')
 def server_port():
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as sock:
         sock.bind(('localhost', 0))
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
```

### Comparing `granian-1.2.0/tests/fixtures/tls/cert.pem` & `granian-1.2.1/tests/fixtures/tls/cert.pem`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/tests/fixtures/tls/key.pem` & `granian-1.2.1/tests/fixtures/tls/key.pem`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/tests/test_asgi.py` & `granian-1.2.1/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/tests/test_https.py` & `granian-1.2.1/tests/test_https.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/tests/test_rsgi.py` & `granian-1.2.1/tests/test_rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/tests/test_ws.py` & `granian-1.2.1/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/tests/test_wsgi.py` & `granian-1.2.1/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/Cargo.lock` & `granian-1.2.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "granian"
-version = "1.2.0"
+version = "1.2.1"
 dependencies = [
  "anyhow",
  "futures",
  "http-body-util",
  "hyper",
  "hyper-util",
  "log",
@@ -959,17 +959,17 @@
  "thiserror",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
```

### Comparing `granian-1.2.0/pyproject.toml` & `granian-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `granian-1.2.0/PKG-INFO` & `granian-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granian
-Version: 1.2.0
+Version: 1.2.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

