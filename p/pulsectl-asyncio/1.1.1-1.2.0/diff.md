# Comparing `tmp/pulsectl-asyncio-1.1.1.tar.gz` & `tmp/pulsectl-asyncio-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsectl-asyncio-1.1.1.tar", last modified: Thu Jun  1 18:11:23 2023, max compression
+gzip compressed data, was "pulsectl-asyncio-1.2.0.tar", last modified: Mon Apr  8 18:48:23 2024, max compression
```

## Comparing `pulsectl-asyncio-1.1.1.tar` & `pulsectl-asyncio-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/pulsectl_asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio/pa_asyncio_mainloop.py
--rw-r--r--   0 runner    (1001) docker     (123)    27164 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio/pulsectl_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-01 18:11:23.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-01 18:11:23.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:11:23.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 18:11:23.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 18:11:23.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/tests/test_async_with_dummy_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:48:23.009158 pulsectl-asyncio-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-08 18:48:15.000000 pulsectl-asyncio-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-04-08 18:48:23.009158 pulsectl-asyncio-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-08 18:48:15.000000 pulsectl-asyncio-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:48:23.009158 pulsectl-asyncio-1.2.0/pulsectl_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:48:15.000000 pulsectl-asyncio-1.2.0/pulsectl_asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15498 2024-04-08 18:48:15.000000 pulsectl-asyncio-1.2.0/pulsectl_asyncio/pa_asyncio_mainloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27565 2024-04-08 18:48:15.000000 pulsectl-asyncio-1.2.0/pulsectl_asyncio/pulsectl_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:48:23.009158 pulsectl-asyncio-1.2.0/pulsectl_asyncio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-04-08 18:48:22.000000 pulsectl-asyncio-1.2.0/pulsectl_asyncio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-08 18:48:23.000000 pulsectl-asyncio-1.2.0/pulsectl_asyncio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:48:22.000000 pulsectl-asyncio-1.2.0/pulsectl_asyncio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 18:48:22.000000 pulsectl-asyncio-1.2.0/pulsectl_asyncio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 18:48:23.000000 pulsectl-asyncio-1.2.0/pulsectl_asyncio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 18:48:15.000000 pulsectl-asyncio-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-08 18:48:23.009158 pulsectl-asyncio-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:48:23.009158 pulsectl-asyncio-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20261 2024-04-08 18:48:15.000000 pulsectl-asyncio-1.2.0/tests/test_async_with_dummy_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-08 18:48:15.000000 pulsectl-asyncio-1.2.0/tests/test_examples.py
```

### Comparing `pulsectl-asyncio-1.1.1/LICENSE` & `pulsectl-asyncio-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.1.1/PKG-INFO` & `pulsectl-asyncio-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsectl-asyncio
-Version: 1.1.1
+Version: 1.2.0
 Summary: Asyncio frontend for the pulsectl Python bindings of libpulse
 Home-page: https://github.com/mhthies/pulsectl-asyncio
 Author: Michael Thies
 Author-email: mail@mhthies.de
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -17,14 +17,15 @@
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Multimedia :: Sound/Audio :: Mixers
 Classifier: Operating System :: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pulsectl<=24.4.0,>=23.5.0
 
 # pulsectl-asyncio
 
 This library provides an Python 3 asyncio interface on top of the [pulsectl](https://github.com/mk-fg/python-pulse-control) library for monitoring and controlling the PulseAudio sound server.
 
 *pulsectl* is a Python ctypes wrapper of the PulseAudio client C library `libpulse`, providing a high-level interface to PulseAudio's source/sink/stream handling and volume mixing. 
 It has originally been forked from the internal code of the [pulsemixer](https://github.com/GeorgeFilipkin/pulsemixer/) command line application.
```

### Comparing `pulsectl-asyncio-1.1.1/README.md` & `pulsectl-asyncio-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.1.1/pulsectl_asyncio/pa_asyncio_mainloop.py` & `pulsectl-asyncio-1.2.0/pulsectl_asyncio/pa_asyncio_mainloop.py`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.1.1/pulsectl_asyncio/pulsectl_async.py` & `pulsectl-asyncio-1.2.0/pulsectl_asyncio/pulsectl_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,14 +426,21 @@
 		assert_pulse_object(obj)
 		method = {
 			PulseSinkInfo: self.sink_default_set,
 			PulseSourceInfo: self.source_default_set }.get(type(obj))
 		if not method: raise NotImplementedError(type(obj))
 		await method(obj)
 
+	async def sink_default_get(self):
+		'Wrapper around server_info() to return sink for default_sink_name there.'
+		return await self.get_sink_by_name((await self.server_info()).default_sink_name)
+	async def source_default_get(self):
+		'Wrapper around server_info() to return source for default_source_name there.'
+		return await self.get_source_by_name((await self.server_info()).default_source_name)
+
 	async def mute(self, obj, mute=True):
 		assert_pulse_object(obj)
 		method = {
 			PulseSinkInfo: self.sink_mute,
 			PulseSinkInputInfo: self.sink_input_mute,
 			PulseSourceInfo: self.source_mute,
 			PulseSourceOutputInfo: self.source_output_mute }.get(type(obj))
```

### Comparing `pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/PKG-INFO` & `pulsectl-asyncio-1.2.0/pulsectl_asyncio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsectl-asyncio
-Version: 1.1.1
+Version: 1.2.0
 Summary: Asyncio frontend for the pulsectl Python bindings of libpulse
 Home-page: https://github.com/mhthies/pulsectl-asyncio
 Author: Michael Thies
 Author-email: mail@mhthies.de
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -17,14 +17,15 @@
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Multimedia :: Sound/Audio :: Mixers
 Classifier: Operating System :: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pulsectl<=24.4.0,>=23.5.0
 
 # pulsectl-asyncio
 
 This library provides an Python 3 asyncio interface on top of the [pulsectl](https://github.com/mk-fg/python-pulse-control) library for monitoring and controlling the PulseAudio sound server.
 
 *pulsectl* is a Python ctypes wrapper of the PulseAudio client C library `libpulse`, providing a high-level interface to PulseAudio's source/sink/stream handling and volume mixing. 
 It has originally been forked from the internal code of the [pulsemixer](https://github.com/GeorgeFilipkin/pulsemixer/) command line application.
```

### Comparing `pulsectl-asyncio-1.1.1/setup.cfg` & `pulsectl-asyncio-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pulsectl-asyncio
-version = 1.1.1
+version = 1.2.0
 url = https://github.com/mhthies/pulsectl-asyncio
 author = Michael Thies
 author_email = mail@mhthies.de
 description = Asyncio frontend for the pulsectl Python bindings of libpulse
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
@@ -23,14 +23,14 @@
 	Operating System :: POSIX
 	Development Status :: 5 - Production/Stable
 
 [options]
 packages = pulsectl_asyncio
 python_requires = >=3.6
 install_requires = 
-	pulsectl >=23.5.0,<=23.5.2
+	pulsectl >=23.5.0,<=24.4.0
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pulsectl-asyncio-1.1.1/tests/test_async_with_dummy_instance.py` & `pulsectl-asyncio-1.2.0/tests/test_async_with_dummy_instance.py`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.1.1/tests/test_examples.py` & `pulsectl-asyncio-1.2.0/tests/test_examples.py`

 * *Files identical despite different names*

