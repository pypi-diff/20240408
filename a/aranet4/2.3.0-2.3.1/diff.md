# Comparing `tmp/aranet4-2.3.0.tar.gz` & `tmp/aranet4-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aranet4-2.3.0.tar", last modified: Fri Apr  5 17:06:52 2024, max compression
+gzip compressed data, was "aranet4-2.3.1.tar", last modified: Mon Apr  8 15:37:34 2024, max compression
```

## Comparing `aranet4-2.3.0.tar` & `aranet4-2.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-05 17:06:52.293854 aranet4-2.3.0/
--rw-r--r--   0 pi        (1000) pi        (1000)     1071 2023-12-06 11:57:48.000000 aranet4-2.3.0/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     6477 2024-04-05 17:06:52.277854 aranet4-2.3.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     6079 2023-12-06 11:57:48.000000 aranet4-2.3.0/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-05 17:06:52.245854 aranet4-2.3.0/aranet4/
--rw-r--r--   0 pi        (1000) pi        (1000)      129 2024-04-05 16:46:51.000000 aranet4-2.3.0/aranet4/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7886 2024-04-05 16:45:21.000000 aranet4-2.3.0/aranet4/aranetctl.py
--rw-r--r--   0 pi        (1000) pi        (1000)    35313 2024-04-05 16:35:20.000000 aranet4-2.3.0/aranet4/client.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-05 17:06:52.273854 aranet4-2.3.0/aranet4.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     6477 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      273 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       60 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-04-05 17:06:52.293854 aranet4-2.3.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      759 2024-04-05 16:47:26.000000 aranet4-2.3.0/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-08 15:37:34.665964 aranet4-2.3.1/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1071 2023-12-06 11:57:48.000000 aranet4-2.3.1/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     6464 2024-04-08 15:37:34.649964 aranet4-2.3.1/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     6079 2023-12-06 11:57:48.000000 aranet4-2.3.1/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-08 15:37:34.633964 aranet4-2.3.1/aranet4/
+-rw-r--r--   0 pi        (1000) pi        (1000)      129 2024-04-08 13:05:57.000000 aranet4-2.3.1/aranet4/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7886 2024-04-08 15:37:07.000000 aranet4-2.3.1/aranet4/aranetctl.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    35420 2024-04-08 15:30:15.000000 aranet4-2.3.1/aranet4/client.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-08 15:37:34.645964 aranet4-2.3.1/aranet4.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6464 2024-04-08 15:37:33.000000 aranet4-2.3.1/aranet4.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      273 2024-04-08 15:37:34.000000 aranet4-2.3.1/aranet4.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-08 15:37:33.000000 aranet4-2.3.1/aranet4.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       60 2024-04-08 15:37:33.000000 aranet4-2.3.1/aranet4.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       15 2024-04-08 15:37:33.000000 aranet4-2.3.1/aranet4.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        8 2024-04-08 15:37:33.000000 aranet4-2.3.1/aranet4.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-04-08 15:37:34.665964 aranet4-2.3.1/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      746 2024-04-08 13:05:48.000000 aranet4-2.3.1/setup.py
```

### Comparing `aranet4-2.3.0/LICENSE` & `aranet4-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aranet4-2.3.0/PKG-INFO` & `aranet4-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.3.0
-Summary: Aranet4 and Aranet2 Python client
+Version: 2.3.1
+Summary: Aranet Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aranet4-2.3.0/README.md` & `aranet4-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `aranet4-2.3.0/aranet4/aranetctl.py` & `aranet4-2.3.1/aranet4/aranetctl.py`

 * *Files identical despite different names*

### Comparing `aranet4-2.3.0/aranet4/client.py` & `aranet4-2.3.1/aranet4/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,19 +370,18 @@
             has_manufacurer_data = Aranet4.MANUFACTURER_ID in ad_data.manufacturer_data
             self.rssi = ad_data.rssi
 
             if has_manufacurer_data:
                 mf_data = ManufacturerData()
                 raw_bytes = bytearray(ad_data.manufacturer_data[Aranet4.MANUFACTURER_ID])
 
-                # Basic info
-                if raw_bytes[0] == 33 and raw_bytes[1] != 33:
-                    # For some reason, this is dropped for Aranet4
+                if (not device.name and len(raw_bytes) in [7,22]) or "Aranet4" in device.name:
                     raw_bytes.insert(0,0)
 
+                # Basic info
                 value_fmt = "<BBBB"
                 value = struct.unpack(value_fmt, raw_bytes[1:5])
                 mf_data.decode(value)
                 self.manufacturer_data = mf_data
 
                 # Extended info / measurements
                 aranetv = raw_bytes[0]
@@ -512,14 +511,19 @@
         if not re.match(self.REGEX_ADDR, address.lower()):
             raise Aranet4Error("Invalid device address")
 
         self.address = address
         self.device = BleakClient(address)
         self.reading = True
 
+    def __del__(self):
+        """Close remote"""
+        if self.device.is_connected:
+            asyncio.shield(self.device.disconnect())
+
     async def connect(self):
         """Connect to remote device"""
         await self.device.connect()
 
     async def current_readings(self, details: bool = False):
         """Extract current readings from remote device"""
         readings = CurrentReading()
```

### Comparing `aranet4-2.3.0/aranet4.egg-info/PKG-INFO` & `aranet4-2.3.1/aranet4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.3.0
-Summary: Aranet4 and Aranet2 Python client
+Version: 2.3.1
+Summary: Aranet Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aranet4-2.3.0/setup.py` & `aranet4-2.3.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aranet4",
-    version="2.3.0",
-    description="Aranet4 and Aranet2 Python client",
+    version="2.3.1",
+    description="Aranet Python client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anrijs/Aranet4-Python",
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

