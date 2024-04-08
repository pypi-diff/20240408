# Comparing `tmp/CodingRider-2.1.tar.gz` & `tmp/CodingRider-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodingRider-2.1.tar", last modified: Fri Apr  5 06:36:25 2024, max compression
+gzip compressed data, was "CodingRider-2.2.tar", last modified: Mon Apr  8 06:14:47 2024, max compression
```

## Comparing `CodingRider-2.1.tar` & `CodingRider-2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 06:36:25.170832 CodingRider-2.1/
-drwxrwxrwx   0        0        0        0 2024-04-05 06:36:25.161262 CodingRider-2.1/CodingRider/
--rw-rw-rw-   0        0        0      109 2024-04-05 06:35:16.000000 CodingRider-2.1/CodingRider/__init__.py
--rw-rw-rw-   0        0        0      484 2023-12-25 23:04:18.000000 CodingRider-2.1/CodingRider/__main__.py
--rw-rw-rw-   0        0        0     4609 2023-03-28 08:35:12.000000 CodingRider-2.1/CodingRider/crc.py
--rw-rw-rw-   0        0        0    44020 2024-04-05 00:11:47.000000 CodingRider-2.1/CodingRider/drone.py
--rw-rw-rw-   0        0        0    70439 2024-04-05 00:10:08.000000 CodingRider-2.1/CodingRider/protocol.py
--rw-rw-rw-   0        0        0     7088 2023-11-15 01:18:50.000000 CodingRider-2.1/CodingRider/receiver.py
--rw-rw-rw-   0        0        0     1904 2023-12-25 23:03:04.000000 CodingRider-2.1/CodingRider/storage.py
--rw-rw-rw-   0        0        0    10249 2023-03-28 08:35:12.000000 CodingRider-2.1/CodingRider/system.py
-drwxrwxrwx   0        0        0        0 2024-04-05 06:36:25.168373 CodingRider-2.1/CodingRider.egg-info/
--rw-rw-rw-   0        0        0      626 2024-04-05 06:36:25.000000 CodingRider-2.1/CodingRider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-04-05 06:36:25.000000 CodingRider-2.1/CodingRider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 06:36:25.000000 CodingRider-2.1/CodingRider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-05 06:36:25.000000 CodingRider-2.1/CodingRider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-05 06:36:25.000000 CodingRider-2.1/CodingRider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-03-28 08:35:12.000000 CodingRider-2.1/LICENSE
--rw-rw-rw-   0        0        0       36 2023-03-28 08:35:12.000000 CodingRider-2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      626 2024-04-05 06:36:25.169413 CodingRider-2.1/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-11-15 03:15:25.000000 CodingRider-2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 06:36:25.170832 CodingRider-2.1/setup.cfg
--rw-rw-rw-   0        0        0      772 2024-04-05 06:35:52.000000 CodingRider-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:14:47.974104 CodingRider-2.2/
+drwxrwxrwx   0        0        0        0 2024-04-08 06:14:47.965532 CodingRider-2.2/CodingRider/
+-rw-rw-rw-   0        0        0      109 2024-04-05 06:35:16.000000 CodingRider-2.2/CodingRider/__init__.py
+-rw-rw-rw-   0        0        0      484 2023-12-25 23:04:18.000000 CodingRider-2.2/CodingRider/__main__.py
+-rw-rw-rw-   0        0        0     4609 2023-03-28 08:35:12.000000 CodingRider-2.2/CodingRider/crc.py
+-rw-rw-rw-   0        0        0    44020 2024-04-05 00:11:47.000000 CodingRider-2.2/CodingRider/drone.py
+-rw-rw-rw-   0        0        0    73725 2024-04-08 00:29:36.000000 CodingRider-2.2/CodingRider/protocol.py
+-rw-rw-rw-   0        0        0     7088 2023-11-15 01:18:50.000000 CodingRider-2.2/CodingRider/receiver.py
+-rw-rw-rw-   0        0        0     1904 2023-12-25 23:03:04.000000 CodingRider-2.2/CodingRider/storage.py
+-rw-rw-rw-   0        0        0    10249 2023-03-28 08:35:12.000000 CodingRider-2.2/CodingRider/system.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:14:47.972104 CodingRider-2.2/CodingRider.egg-info/
+-rw-rw-rw-   0        0        0      626 2024-04-08 06:14:47.000000 CodingRider-2.2/CodingRider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-04-08 06:14:47.000000 CodingRider-2.2/CodingRider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 06:14:47.000000 CodingRider-2.2/CodingRider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-08 06:14:47.000000 CodingRider-2.2/CodingRider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-08 06:14:47.000000 CodingRider-2.2/CodingRider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-03-28 08:35:12.000000 CodingRider-2.2/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-03-28 08:35:12.000000 CodingRider-2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      626 2024-04-08 06:14:47.973106 CodingRider-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-11-15 03:15:25.000000 CodingRider-2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 06:14:47.974104 CodingRider-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      772 2024-04-08 00:30:32.000000 CodingRider-2.2/setup.py
```

### Comparing `CodingRider-2.1/CodingRider/crc.py` & `CodingRider-2.2/CodingRider/crc.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.1/CodingRider/drone.py` & `CodingRider-2.2/CodingRider/drone.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.1/CodingRider/protocol.py` & `CodingRider-2.2/CodingRider/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -707,14 +707,172 @@
         return data
 
 
 # Common End
 
 
 
+# Monitor Start
+
+
+class MonitorHeaderType(Enum):
+    
+    Monitor0            = 0x00
+    Monitor4            = 0x01
+    Monitor8            = 0x02
+
+    EndOfType           = 0x03
+
+
+
+class MonitorDataType(Enum):
+    
+    U8          = 0x00,
+    S8          = 0x01,
+    U16         = 0x02,
+    S16         = 0x03,
+    U32         = 0x04,
+    S32         = 0x05,
+    U64         = 0x06,
+    S64         = 0x07,
+    F32         = 0x08,
+    F64         = 0x09,
+
+    EndOfType   = 0x0A
+
+
+
+class MonitorType(ISerializable):
+
+    def __init__(self):
+        self.monitorHeaderType    = MonitorHeaderType.Monitor8
+
+
+    @classmethod
+    def getSize(cls):
+        return 1
+
+
+    def toArray(self):
+        return pack('<B', self.monitorHeaderType.value)
+
+
+    @classmethod
+    def parse(cls, dataArray):
+        data = MonitorType()
+        
+        if len(dataArray) != cls.getSize():
+            return None
+        
+        data.monitorHeaderType, = unpack('<B', dataArray)
+
+        data.monitorHeaderType  = MonitorHeaderType(data.monitorHeaderType)
+
+        return data
+
+
+
+class Monitor0(ISerializable):
+
+    def __init__(self):
+        self.monitorDataType        = MonitorDataType.F32
+        self.index                  = 0
+
+
+    @classmethod
+    def getSize(cls):
+        return 2
+
+
+    def toArray(self):
+        return pack('<BB', self.monitorDataType.value, self.index)
+
+
+    @classmethod
+    def parse(cls, dataArray):
+        data = Monitor0()
+        
+        if len(dataArray) != cls.getSize():
+            return None
+        
+        data.monitorDataType, data.index = unpack('<BB', dataArray)
+
+        data.monitorDataType  = MonitorDataType(data.monitorDataType)
+
+        return data
+
+
+
+class Monitor4(ISerializable):
+
+    def __init__(self):
+        self.systemTime             = 0
+        self.monitorDataType        = MonitorDataType.F32
+        self.index                  = 0
+
+
+    @classmethod
+    def getSize(cls):
+        return 6
+
+
+    def toArray(self):
+        return pack('<IBB', self.systemTime, self.monitorDataType.value, self.index)
+
+
+    @classmethod
+    def parse(cls, dataArray):
+        data = Monitor4()
+        
+        if len(dataArray) != cls.getSize():
+            return None
+        
+        data.systemTime, data.monitorDataType, data.index = unpack('<IBB', dataArray)
+
+        data.monitorDataType  = MonitorDataType(data.monitorDataType)
+
+        return data
+
+
+
+class Monitor8(ISerializable):
+    
+    def __init__(self):
+        self.systemTime             = 0
+        self.monitorDataType        = MonitorDataType.F32
+        self.index                  = 0
+
+
+    @classmethod
+    def getSize(cls):
+        return 10
+
+
+    def toArray(self):
+        return pack('<QBB', self.systemTime, self.monitorDataType.value, self.index)
+
+
+    @classmethod
+    def parse(cls, dataArray):
+        data = Monitor8()
+        
+        if len(dataArray) != cls.getSize():
+            return None
+        
+        data.systemTime, data.monitorDataType, data.index = unpack('<QBB', dataArray)
+
+        data.monitorDataType  = MonitorDataType(data.monitorDataType)
+
+        return data
+
+
+
+# Monitor End
+
+
 
 # Control Start
 
 
 class ControlQuad8(ISerializable):
 
     def __init__(self):
```

### Comparing `CodingRider-2.1/CodingRider/receiver.py` & `CodingRider-2.2/CodingRider/receiver.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.1/CodingRider/storage.py` & `CodingRider-2.2/CodingRider/storage.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.1/CodingRider/system.py` & `CodingRider-2.2/CodingRider/system.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.1/setup.py` & `CodingRider-2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # http://swdeveloper.tistory.com/34
 # https://code.tutsplus.com/ko/tutorials/how-to-share-your-python-packages--cms-26114
 # https://code.tutsplus.com/ko/tutorials/how-to-write-your-own-python-packages--cms-26076
 from setuptools import setup, find_packages
 
 setup(
     name = "CodingRider",
-    version = "2.1",
+    version = "2.2",
     description = "Library for CodingRider",
     author = "ALUX",
     author_email = "devdrone@aluxonline.com",
     url = "https://imssam.me/shop/view.php?index_no=4031",
     packages = find_packages(exclude=['tests']),
     install_requires = [
         'pyserial>=3.4',
```

