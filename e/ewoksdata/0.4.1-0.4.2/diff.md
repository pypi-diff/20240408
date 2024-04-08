# Comparing `tmp/ewoksdata-0.4.1.tar.gz` & `tmp/ewoksdata-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewoksdata-0.4.1.tar", last modified: Wed Mar 20 20:28:05 2024, max compression
+gzip compressed data, was "ewoksdata-0.4.2.tar", last modified: Mon Apr  8 16:55:58 2024, max compression
```

## Comparing `ewoksdata-0.4.1.tar` & `ewoksdata-0.4.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:28:05.095421 ewoksdata-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1732 2024-03-20 20:28:05.095421 ewoksdata-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1260 2024-03-20 20:28:05.099421 ewoksdata-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:28:05.087421 ewoksdata-0.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:28:05.091421 ewoksdata-0.4.1/src/ewoksdata/
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-03-20 20:20:46.000000 ewoksdata-0.4.1/src/ewoksdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:28:05.091421 ewoksdata-0.4.1/src/ewoksdata/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 20:27:58.000000 ewoksdata-0.4.1/src/ewoksdata/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4965 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/bliss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:28:05.091421 ewoksdata-0.4.1/src/ewoksdata/data/blissdata/
--rw-rw-rw-   0 root         (0) root         (0)     1203 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/blissdata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3816 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/blissdata/blissdatav0.py
--rw-rw-rw-   0 root         (0) root         (0)     3054 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/blissdata/blissdatav1.py
--rw-rw-rw-   0 root         (0) root         (0)     3319 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/blissdata/blissdatavid31.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/blissdata/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:28:05.095421 ewoksdata-0.4.1/src/ewoksdata/data/hdf5/
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/hdf5/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6086 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/hdf5/config.py
--rw-rw-rw-   0 root         (0) root         (0)     9872 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/hdf5/dataset_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/hdf5/types.py
--rw-rw-rw-   0 root         (0) root         (0)     3111 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/url.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:28:05.095421 ewoksdata-0.4.1/src/ewoksdata/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 20:27:58.000000 ewoksdata-0.4.1/src/ewoksdata/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:28:05.095421 ewoksdata-0.4.1/src/ewoksdata/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3772 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/tests/data/bliss_scans.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/tests/test_data_bliss.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/tests/test_data_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/tests/test_data_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     4200 2024-03-20 12:03:25.000000 ewoksdata-0.4.1/src/ewoksdata/tests/test_dataset_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:28:05.095421 ewoksdata-0.4.1/src/ewoksdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1732 2024-03-20 20:28:05.000000 ewoksdata-0.4.1/src/ewoksdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1069 2024-03-20 20:28:05.000000 ewoksdata-0.4.1/src/ewoksdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 20:28:05.000000 ewoksdata-0.4.1/src/ewoksdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      313 2024-03-20 20:28:05.000000 ewoksdata-0.4.1/src/ewoksdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-20 20:28:05.000000 ewoksdata-0.4.1/src/ewoksdata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:55:58.401167 ewoksdata-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-08 16:55:58.401167 ewoksdata-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2024-04-08 16:55:58.401167 ewoksdata-0.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:55:58.393168 ewoksdata-0.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:55:58.393168 ewoksdata-0.4.2/src/ewoksdata/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-08 16:34:40.000000 ewoksdata-0.4.2/src/ewoksdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:55:58.397168 ewoksdata-0.4.2/src/ewoksdata/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:55:52.000000 ewoksdata-0.4.2/src/ewoksdata/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4965 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/data/bliss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:55:58.397168 ewoksdata-0.4.2/src/ewoksdata/data/blissdata/
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/data/blissdata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3816 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/data/blissdata/blissdatav0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2024-04-08 16:55:52.000000 ewoksdata-0.4.2/src/ewoksdata/data/blissdata/blissdatav1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3646 2024-04-08 16:55:52.000000 ewoksdata-0.4.2/src/ewoksdata/data/blissdata/blissdatavid31.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/data/blissdata/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:55:58.397168 ewoksdata-0.4.2/src/ewoksdata/data/hdf5/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/data/hdf5/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6086 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/data/hdf5/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9872 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/data/hdf5/dataset_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/data/hdf5/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3111 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/data/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/data/url.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:55:58.397168 ewoksdata-0.4.2/src/ewoksdata/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:55:52.000000 ewoksdata-0.4.2/src/ewoksdata/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:55:58.397168 ewoksdata-0.4.2/src/ewoksdata/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/tests/data/bliss_scans.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/tests/test_data_bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/tests/test_data_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/tests/test_data_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     4200 2024-04-08 11:03:15.000000 ewoksdata-0.4.2/src/ewoksdata/tests/test_dataset_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:55:58.397168 ewoksdata-0.4.2/src/ewoksdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-08 16:55:58.000000 ewoksdata-0.4.2/src/ewoksdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-04-08 16:55:58.000000 ewoksdata-0.4.2/src/ewoksdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:55:58.000000 ewoksdata-0.4.2/src/ewoksdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      313 2024-04-08 16:55:58.000000 ewoksdata-0.4.2/src/ewoksdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-08 16:55:58.000000 ewoksdata-0.4.2/src/ewoksdata.egg-info/top_level.txt
```

### Comparing `ewoksdata-0.4.1/LICENSE.md` & `ewoksdata-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/PKG-INFO` & `ewoksdata-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.4.1
+Version: 0.4.2
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.4.1/setup.cfg` & `ewoksdata-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/data/bliss.py` & `ewoksdata-0.4.2/src/ewoksdata/data/bliss.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/data/blissdata/__init__.py` & `ewoksdata-0.4.2/src/ewoksdata/data/blissdata/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/data/blissdata/blissdatav0.py` & `ewoksdata-0.4.2/src/ewoksdata/data/blissdata/blissdatav0.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/data/blissdata/blissdatavid31.py` & `ewoksdata-0.4.2/src/ewoksdata/data/blissdata/blissdatav1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,91 @@
 from numbers import Number
+from collections import Counter
 from typing import List, Optional
 
 from numpy.typing import ArrayLike
 
 from .exceptions import VersionError
 
 try:
+    from blissdata.beacon.data import BeaconData
+    from blissdata.redis_engine.store import DataStore
     from blissdata.redis_engine.scan import Scan
+    from blissdata.redis_engine.scan import ScanState
     from blissdata.redis_engine.stream import StreamingClient
-    from blissdata.redis_engine.models import ScanState
     from blissdata.redis_engine.exceptions import EndOfStream
+    from blissdata.redis_engine.exceptions import IndexNoMoreThereError
     from blissdata.lima.client import lima_client_factory
-    from blissdata.beacon.data import BeaconData
-    from blissdata import redis_engine
 except ImportError as e:
     raise VersionError(str(e)) from e
 
 
 def iter_bliss_scan_data_from_memory(
     db_name: str,
     lima_names: List[str],
     counter_names: List[str],
     retry_timeout: Optional[Number] = None,
     retry_period: Optional[Number] = None,
 ):
-    _ensure_redis()
-    scan = Scan.load(db_name)
+    data_store = _get_data_store()
+    scan = data_store.load_scan(db_name, scan_cls=Scan)
     buffers = {name: list() for name in lima_names + counter_names}
 
     while scan.state < ScanState.PREPARED:
         scan.update()
-    if scan.state is ScanState.ABORTED:
-        return
 
     lima_streams = dict()
     lima_clients = dict()
     counter_streams = dict()
     for name, stream in scan.streams.items():
         if stream.encoding["type"] == "json" and "lima" in stream.info["format"]:
             if name.split(":")[-2] in lima_names:
                 lima_streams[name] = stream
-                lima_clients[name] = lima_client_factory(stream.info)
+                lima_clients[name] = lima_client_factory(data_store, stream.info)
         elif name.split(":")[-1] in counter_names:
             counter_streams[name] = stream
 
     client = StreamingClient({**lima_streams, **counter_streams})
+    lima_buffer_count = Counter()
 
     while True:
         try:
             output = client.read()
         except EndOfStream:
             break
-        else:
-            for stream, data in output.items():
-                _, payload = data  # drop index
-                if stream.name in lima_streams:
-                    lima_client = lima_clients[stream.name]
-                    prev_len = len(lima_client)
-                    lima_client.update(**payload[-1])
-                    data = lima_client[prev_len - 1 :]
-                    buffers[stream.name.split(":")[-2]].extend(data)
-                else:
-                    buffers[stream.name.split(":")[-1]].extend(payload)
-
-            nyield = min(len(v) for v in buffers.values())
-            if nyield:
-                for i in range(nyield):
-                    yield {name: values[i] for name, values in buffers.items()}
-                buffers = {name: values[nyield:] for name, values in buffers.items()}
+        for stream, (_, payload) in output.items():
+            name_parts = stream.name.split(":")
+            if stream.name in lima_streams:
+                # payload is a sequence of JSON statuses
+                ctr_name = name_parts[-2]
+                last_status = payload[-1]
+                lima_client = lima_clients[stream.name]
+                lima_client.update(**last_status)
+                n_already_read = lima_buffer_count[ctr_name]
+                try:
+                    data = lima_client[n_already_read:]
+                except IndexNoMoreThereError:
+                    continue
+                buffers[ctr_name].extend(data)
+                lima_buffer_count[ctr_name] += len(data)
+            else:
+                # payload is a sequence of data points (0D, 1D, 2D)
+                ctr_name = name_parts[-1]
+                buffers[ctr_name].extend(payload)
+
+        nyield = min(len(v) for v in buffers.values())
+        if nyield:
+            for i in range(nyield):
+                yield {name: values[i] for name, values in buffers.items()}
+            buffers = {name: values[nyield:] for name, values in buffers.items()}
 
 
 def last_lima_image(channel_info: dict) -> ArrayLike:
     """Get last lima image from memory"""
-    _ensure_redis()
-    lima_client = lima_client_factory(channel_info)
+    data_store = _get_data_store()
+    lima_client = lima_client_factory(data_store, channel_info)
     return lima_client.get_last_live_image().array
 
 
-def _ensure_redis() -> None:
-    url = BeaconData().get_redis_data_db()
-    current_url = _current_redis_url()
-    if current_url:
-        if url == current_url:
-            return
-        raise RuntimeError("The Redis URL has changed. Restart the Nexus writer.")
-    redis_engine.set_redis_url(url)
-
-
-def _current_redis_url() -> Optional[str]:
-    if redis_engine._redis is None:
-        return
-    kwargs = redis_engine._redis.connection_pool.connection_kwargs
-    if "path" in kwargs:
-        return f"unix://{kwargs['path']}"
-    else:
-        return f"redis://{kwargs['host']}:{kwargs['port']}"
+def _get_data_store() -> None:
+    redis_url = BeaconData().get_redis_data_db()
+    return DataStore(redis_url)
```

### Comparing `ewoksdata-0.4.1/src/ewoksdata/data/hdf5/__init__.py` & `ewoksdata-0.4.2/src/ewoksdata/data/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/data/hdf5/config.py` & `ewoksdata-0.4.2/src/ewoksdata/data/hdf5/config.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/data/hdf5/dataset_writer.py` & `ewoksdata-0.4.2/src/ewoksdata/data/hdf5/dataset_writer.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/data/nexus.py` & `ewoksdata-0.4.2/src/ewoksdata/data/nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/data/url.py` & `ewoksdata-0.4.2/src/ewoksdata/data/url.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/data/utils.py` & `ewoksdata-0.4.2/src/ewoksdata/data/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/tests/data/bliss_scans.py` & `ewoksdata-0.4.2/src/ewoksdata/tests/data/bliss_scans.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/tests/test_data_bliss.py` & `ewoksdata-0.4.2/src/ewoksdata/tests/test_data_bliss.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/tests/test_data_nexus.py` & `ewoksdata-0.4.2/src/ewoksdata/tests/test_data_nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata/tests/test_dataset_writer.py` & `ewoksdata-0.4.2/src/ewoksdata/tests/test_dataset_writer.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.4.1/src/ewoksdata.egg-info/PKG-INFO` & `ewoksdata-0.4.2/src/ewoksdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.4.1
+Version: 0.4.2
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.4.1/src/ewoksdata.egg-info/SOURCES.txt` & `ewoksdata-0.4.2/src/ewoksdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

