# Comparing `tmp/pyjvc-4.4.0.tar.gz` & `tmp/pyjvc-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjvc-4.4.0.tar", last modified: Sat Mar 23 01:20:48 2024, max compression
+gzip compressed data, was "pyjvc-4.4.1.tar", last modified: Sun Apr  7 23:44:32 2024, max compression
```

## Comparing `pyjvc-4.4.0.tar` & `pyjvc-4.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-03-23 01:20:48.538862 pyjvc-4.4.0/
--rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.0/LICENSE
--rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-03-23 01:20:48.538650 pyjvc-4.4.0/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.0/README.md
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-03-23 01:20:48.536415 pyjvc-4.4.0/jvc_projector/
--rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.0/jvc_projector/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     8881 2024-03-20 01:40:47.000000 pyjvc-4.4.0/jvc_projector/command_runner.py
--rw-r--r--   0 ilan       (501) staff       (20)    10033 2024-03-20 01:40:47.000000 pyjvc-4.4.0/jvc_projector/commands.py
--rw-r--r--   0 ilan       (501) staff       (20)      200 2024-02-17 18:22:01.000000 pyjvc-4.4.0/jvc_projector/error_classes.py
--rw-r--r--   0 ilan       (501) staff       (20)    16961 2024-03-20 01:40:47.000000 pyjvc-4.4.0/jvc_projector/jvc_projector.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-03-23 01:20:48.538444 pyjvc-4.4.0/pyJVC.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-03-23 01:20:48.000000 pyjvc-4.4.0/pyJVC.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      491 2024-03-23 01:20:48.000000 pyjvc-4.4.0/pyJVC.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2024-03-23 01:20:48.000000 pyjvc-4.4.0/pyJVC.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       20 2024-03-23 01:20:48.000000 pyjvc-4.4.0/pyJVC.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2024-03-23 01:20:48.538902 pyjvc-4.4.0/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      634 2024-03-23 01:20:42.000000 pyjvc-4.4.0/setup.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-03-23 01:20:48.538156 pyjvc-4.4.0/tests/
--rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.0/tests/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.0/tests/test_commander.py
--rw-r--r--   0 ilan       (501) staff       (20)     8345 2024-03-20 01:40:47.000000 pyjvc-4.4.0/tests/test_coordinator.py
--rw-r--r--   0 ilan       (501) staff       (20)    14935 2024-03-20 01:40:47.000000 pyjvc-4.4.0/tests/test_loop.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:44:32.919622 pyjvc-4.4.1/
+-rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.1/LICENSE
+-rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-07 23:44:32.919427 pyjvc-4.4.1/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.1/README.md
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:44:32.916655 pyjvc-4.4.1/jvc_projector/
+-rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.1/jvc_projector/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     8881 2024-03-20 01:40:47.000000 pyjvc-4.4.1/jvc_projector/command_runner.py
+-rw-r--r--   0 ilan       (501) staff       (20)    10032 2024-04-01 00:26:47.000000 pyjvc-4.4.1/jvc_projector/commands.py
+-rw-r--r--   0 ilan       (501) staff       (20)      200 2024-02-17 18:22:01.000000 pyjvc-4.4.1/jvc_projector/error_classes.py
+-rw-r--r--   0 ilan       (501) staff       (20)    17611 2024-03-31 23:24:15.000000 pyjvc-4.4.1/jvc_projector/jvc_projector.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:44:32.919185 pyjvc-4.4.1/pyJVC.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-07 23:44:32.000000 pyjvc-4.4.1/pyJVC.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      491 2024-04-07 23:44:32.000000 pyjvc-4.4.1/pyJVC.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-07 23:44:32.000000 pyjvc-4.4.1/pyJVC.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       20 2024-04-07 23:44:32.000000 pyjvc-4.4.1/pyJVC.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-07 23:44:32.919667 pyjvc-4.4.1/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      634 2024-04-07 23:44:11.000000 pyjvc-4.4.1/setup.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:44:32.918843 pyjvc-4.4.1/tests/
+-rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.1/tests/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.1/tests/test_commander.py
+-rw-r--r--   0 ilan       (501) staff       (20)     8345 2024-03-20 01:40:47.000000 pyjvc-4.4.1/tests/test_coordinator.py
+-rw-r--r--   0 ilan       (501) staff       (20)    14935 2024-03-20 01:40:47.000000 pyjvc-4.4.1/tests/test_loop.py
```

### Comparing `pyjvc-4.4.0/LICENSE` & `pyjvc-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.0/PKG-INFO` & `pyjvc-4.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.0
+Version: 4.4.1
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.0/README.md` & `pyjvc-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.0/jvc_projector/command_runner.py` & `pyjvc-4.4.1/jvc_projector/command_runner.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.0/jvc_projector/commands.py` & `pyjvc-4.4.1/jvc_projector/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,15 @@
 
 class ThreeD(Enum):
     twoD = b"0"
     auto = b"1"
     sbs = b"3"
     tb = b"4"
 
+
 class ResolutionModes(Enum):
     r_480p = b"02"
     r_576p = b"03"
     r_720p50 = b"04"
     r_720p60 = b"05"
     r_1080i50 = b"06"
     r_1080i60 = b"07"
@@ -384,14 +385,15 @@
     r_8K_7680x4320p30 = b"3A"
     r_8K_7680x4320p25 = b"3B"
     r_8K_7680x4320p24 = b"3C"
     WQHD60 = b"3D"
     WOQHD120 = b"3E"
     r_8K_7680x4320p48 = b"3F"
 
+
 class Commands(Enum):
 
     # these use ! unless otherwise indicated
     # power commands
     power = b"PW", PowerModes, ACKs.power_ack
     power_status = b"PW", PowerModes, ACKs.power_ack
     # lens memory /installation mode commands
@@ -461,15 +463,15 @@
     # NZ Series Laser Dimming commands
     laser_mode = b"PMDC", LaserDimModes, ACKs.picture_ack
     # fw 3.0 and up
     laser_value = b"PMCV", int, ACKs.picture_ack
 
     # Lamp power
     lamp_power = b"PMLP", LampPowerModes, ACKs.picture_ack
-   
+
     # Lamp time
     lamp_time = b"IFLT", int, ACKs.info_ack
 
     # Lens Aperture commands
     aperture = b"PMDI", ApertureModes, ACKs.picture_ack
 
     # Anamorphic commands
```

### Comparing `pyjvc-4.4.0/jvc_projector/jvc_projector.py` & `pyjvc-4.4.1/jvc_projector/jvc_projector.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,34 @@
             self.logger.error("Failed to get model family")
             return "Unsupported"
         model_res = self.commander.replace_headers(res).decode()
         self.logger.debug("Model result is %s", model_res)
 
         return model_map.get(model_res[-4:], "Unsupported")
 
+    async def reset_everything(self) -> None:
+        """
+        resets everything and tries to empty current jvc buffer. Used on error to just clear everything and start over
+        """
+        try:
+            if not self.connection_open:
+                await self.open_connection()
+
+            # clear the buffer
+            while not self.reader.at_eof():
+                try:
+                    await self.reader.read(1024)
+                except asyncio.IncompleteReadError:
+                    break
+
+            return
+        except Exception as e:
+            self.logger.error("Error resetting everything: %s", e)
+            return
+
     async def open_connection(self) -> bool:
         """Open a connection to the projector asynchronously"""
         # If the connection is already open, return True
         if self.writer is not None and not self.writer.is_closing():
             self.logger.info("Connection already open.")
             return True
         while True:
```

### Comparing `pyjvc-4.4.0/pyJVC.egg-info/PKG-INFO` & `pyjvc-4.4.1/pyJVC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.0
+Version: 4.4.1
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.0/setup.py` & `pyjvc-4.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyjvc",
-    version="4.4.0",
+    version="4.4.1",
     author="iloveicedgreentea2",
     description="A package to control JVC projectors over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/jvc_projector_improved",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `pyjvc-4.4.0/tests/test_commander.py` & `pyjvc-4.4.1/tests/test_commander.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.0/tests/test_coordinator.py` & `pyjvc-4.4.1/tests/test_coordinator.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.0/tests/test_loop.py` & `pyjvc-4.4.1/tests/test_loop.py`

 * *Files identical despite different names*

