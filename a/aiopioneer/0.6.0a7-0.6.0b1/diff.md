# Comparing `tmp/aiopioneer-0.6.0a7.tar.gz` & `tmp/aiopioneer-0.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopioneer-0.6.0a7.tar", last modified: Wed Apr  3 09:53:43 2024, max compression
+gzip compressed data, was "aiopioneer-0.6.0b1.tar", last modified: Mon Apr  8 07:52:57 2024, max compression
```

## Comparing `aiopioneer-0.6.0a7.tar` & `aiopioneer-0.6.0b1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwx---   0 root         (0) adm          (4)        0 2024-04-03 09:53:43.517942 aiopioneer-0.6.0a7/
--rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.6.0a7/LICENSE
--rw-rw----   0 root         (0) adm          (4)    15367 2024-04-03 09:53:43.520438 aiopioneer-0.6.0a7/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)    14715 2024-03-13 09:14:43.000000 aiopioneer-0.6.0a7/README.md
-drwxrwx---   0 root         (0) adm          (4)        0 2024-04-03 09:53:43.337944 aiopioneer-0.6.0a7/aiopioneer/
--rw-rw----   0 root         (0) adm          (4)       68 2024-03-27 20:16:44.000000 aiopioneer-0.6.0a7/aiopioneer/__init__.py
--rw-rw----   0 root         (0) adm          (4)    11031 2024-04-01 16:54:34.000000 aiopioneer-0.6.0a7/aiopioneer/cli.py
--rw-rw----   0 root         (0) adm          (4)    13805 2024-04-01 19:37:10.000000 aiopioneer-0.6.0a7/aiopioneer/commands.py
--rw-rw----   0 root         (0) adm          (4)    15083 2024-04-03 09:53:16.000000 aiopioneer-0.6.0a7/aiopioneer/const.py
--rw-rw----   0 root         (0) adm          (4)    18687 2024-03-27 20:47:07.000000 aiopioneer-0.6.0a7/aiopioneer/param.py
-drwxrwx---   0 root         (0) adm          (4)        0 2024-04-03 09:53:43.487942 aiopioneer-0.6.0a7/aiopioneer/parsers/
--rw-rw----   0 root         (0) adm          (4)     8175 2024-04-03 07:47:01.000000 aiopioneer-0.6.0a7/aiopioneer/parsers/__init__.py
--rw-rw----   0 root         (0) adm          (4)     3419 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a7/aiopioneer/parsers/audio.py
--rw-rw----   0 root         (0) adm          (4)    19209 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a7/aiopioneer/parsers/dsp.py
--rw-rw----   0 root         (0) adm          (4)    25466 2024-03-31 11:50:52.000000 aiopioneer-0.6.0a7/aiopioneer/parsers/information.py
--rw-rw----   0 root         (0) adm          (4)      599 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a7/aiopioneer/parsers/response.py
--rw-rw----   0 root         (0) adm          (4)    23416 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a7/aiopioneer/parsers/settings.py
--rw-rw----   0 root         (0) adm          (4)    15910 2024-04-03 07:56:23.000000 aiopioneer-0.6.0a7/aiopioneer/parsers/system.py
--rw-rw----   0 root         (0) adm          (4)     6987 2024-04-03 07:20:56.000000 aiopioneer-0.6.0a7/aiopioneer/parsers/tuner.py
--rw-rw----   0 root         (0) adm          (4)     8405 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a7/aiopioneer/parsers/video.py
--rw-rw----   0 root         (0) adm          (4)    87127 2024-04-03 09:48:47.000000 aiopioneer-0.6.0a7/aiopioneer/pioneer_avr.py
--rw-rw----   0 root         (0) adm          (4)     5266 2024-04-01 23:17:31.000000 aiopioneer-0.6.0a7/aiopioneer/util.py
-drwxrwx---   0 root         (0) adm          (4)        0 2024-04-03 09:53:43.497942 aiopioneer-0.6.0a7/aiopioneer.egg-info/
--rw-rw----   0 root         (0) adm          (4)    15367 2024-04-03 09:53:42.000000 aiopioneer-0.6.0a7/aiopioneer.egg-info/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)      614 2024-04-03 09:53:43.000000 aiopioneer-0.6.0a7/aiopioneer.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) adm          (4)        1 2024-04-03 09:53:42.000000 aiopioneer-0.6.0a7/aiopioneer.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) adm          (4)       51 2024-04-03 09:53:42.000000 aiopioneer-0.6.0a7/aiopioneer.egg-info/entry_points.txt
--rw-rw----   0 root         (0) adm          (4)       11 2024-04-03 09:53:42.000000 aiopioneer-0.6.0a7/aiopioneer.egg-info/top_level.txt
--rw-rw----   0 root         (0) adm          (4)       38 2024-04-03 09:53:43.528521 aiopioneer-0.6.0a7/setup.cfg
--rw-rw----   0 root         (0) adm          (4)     1101 2024-03-31 08:50:09.000000 aiopioneer-0.6.0a7/setup.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-08 07:52:57.905947 aiopioneer-0.6.0b1/
+-rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.6.0b1/LICENSE
+-rw-rw----   0 root         (0) adm          (4)    15367 2024-04-08 07:52:57.913423 aiopioneer-0.6.0b1/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)    14715 2024-03-13 09:14:43.000000 aiopioneer-0.6.0b1/README.md
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-08 07:52:57.675950 aiopioneer-0.6.0b1/aiopioneer/
+-rw-rw----   0 root         (0) adm          (4)       68 2024-03-27 20:16:44.000000 aiopioneer-0.6.0b1/aiopioneer/__init__.py
+-rw-rw----   0 root         (0) adm          (4)    11031 2024-04-01 16:54:34.000000 aiopioneer-0.6.0b1/aiopioneer/cli.py
+-rw-rw----   0 root         (0) adm          (4)    13805 2024-04-01 19:37:10.000000 aiopioneer-0.6.0b1/aiopioneer/commands.py
+-rw-rw----   0 root         (0) adm          (4)    15083 2024-04-08 07:52:18.000000 aiopioneer-0.6.0b1/aiopioneer/const.py
+-rw-rw----   0 root         (0) adm          (4)    18687 2024-03-27 20:47:07.000000 aiopioneer-0.6.0b1/aiopioneer/param.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-08 07:52:57.875947 aiopioneer-0.6.0b1/aiopioneer/parsers/
+-rw-rw----   0 root         (0) adm          (4)     8175 2024-04-03 07:47:01.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/__init__.py
+-rw-rw----   0 root         (0) adm          (4)     3419 2024-03-13 09:14:44.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/audio.py
+-rw-rw----   0 root         (0) adm          (4)    19209 2024-03-13 09:14:44.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/dsp.py
+-rw-rw----   0 root         (0) adm          (4)    25466 2024-03-31 11:50:52.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/information.py
+-rw-rw----   0 root         (0) adm          (4)      599 2024-03-13 09:14:44.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/response.py
+-rw-rw----   0 root         (0) adm          (4)    23416 2024-03-13 09:14:44.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/settings.py
+-rw-rw----   0 root         (0) adm          (4)    15910 2024-04-03 07:56:23.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/system.py
+-rw-rw----   0 root         (0) adm          (4)     6987 2024-04-03 07:20:56.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/tuner.py
+-rw-rw----   0 root         (0) adm          (4)     8405 2024-03-13 09:14:44.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/video.py
+-rw-rw----   0 root         (0) adm          (4)    87240 2024-04-05 20:17:20.000000 aiopioneer-0.6.0b1/aiopioneer/pioneer_avr.py
+-rw-rw----   0 root         (0) adm          (4)     5266 2024-04-05 20:12:40.000000 aiopioneer-0.6.0b1/aiopioneer/util.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-08 07:52:57.885947 aiopioneer-0.6.0b1/aiopioneer.egg-info/
+-rw-rw----   0 root         (0) adm          (4)    15367 2024-04-08 07:52:56.000000 aiopioneer-0.6.0b1/aiopioneer.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)      614 2024-04-08 07:52:57.000000 aiopioneer-0.6.0b1/aiopioneer.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) adm          (4)        1 2024-04-08 07:52:57.000000 aiopioneer-0.6.0b1/aiopioneer.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) adm          (4)       51 2024-04-08 07:52:57.000000 aiopioneer-0.6.0b1/aiopioneer.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) adm          (4)       11 2024-04-08 07:52:57.000000 aiopioneer-0.6.0b1/aiopioneer.egg-info/top_level.txt
+-rw-rw----   0 root         (0) adm          (4)       38 2024-04-08 07:52:57.918339 aiopioneer-0.6.0b1/setup.cfg
+-rw-rw----   0 root         (0) adm          (4)     1101 2024-03-31 08:50:09.000000 aiopioneer-0.6.0b1/setup.py
```

### Comparing `aiopioneer-0.6.0a7/LICENSE` & `aiopioneer-0.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/PKG-INFO` & `aiopioneer-0.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.6.0a7
+Version: 0.6.0b1
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `aiopioneer-0.6.0a7/README.md` & `aiopioneer-0.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/cli.py` & `aiopioneer-0.6.0b1/aiopioneer/cli.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/commands.py` & `aiopioneer-0.6.0b1/aiopioneer/commands.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/const.py` & `aiopioneer-0.6.0b1/aiopioneer/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Constants for aiopioneer."""
 
 from enum import StrEnum
 
 DEFAULT_PORT = 8102
-VERSION = "0.6.0a7"
+VERSION = "0.6.0b1"
 
 
 class Zones(StrEnum):
     """Valid aiopioneer zones."""
 
     ALL = "ALL"
     Z1 = "1"
```

### Comparing `aiopioneer-0.6.0a7/aiopioneer/param.py` & `aiopioneer-0.6.0b1/aiopioneer/param.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/parsers/__init__.py` & `aiopioneer-0.6.0b1/aiopioneer/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/parsers/audio.py` & `aiopioneer-0.6.0b1/aiopioneer/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/parsers/dsp.py` & `aiopioneer-0.6.0b1/aiopioneer/parsers/dsp.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/parsers/information.py` & `aiopioneer-0.6.0b1/aiopioneer/parsers/information.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/parsers/response.py` & `aiopioneer-0.6.0b1/aiopioneer/parsers/response.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/parsers/settings.py` & `aiopioneer-0.6.0b1/aiopioneer/parsers/settings.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/parsers/system.py` & `aiopioneer-0.6.0b1/aiopioneer/parsers/system.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/parsers/tuner.py` & `aiopioneer-0.6.0b1/aiopioneer/parsers/tuner.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/parsers/video.py` & `aiopioneer-0.6.0b1/aiopioneer/parsers/video.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer/pioneer_avr.py` & `aiopioneer-0.6.0b1/aiopioneer/pioneer_avr.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,28 +321,28 @@
             return
 
         async with self._disconnect_lock:
             _LOGGER.debug("disconnecting AVR connection")
             self.available = False
             self._call_zone_callbacks()
 
-            await self._listener_cancel()
-            await self._responder_cancel()
-            await self._updater_cancel()
             await self._command_queue_cancel()
+            await self._updater_cancel()
+            await self._responder_cancel()
+            await self._listener_cancel()
 
             writer = self._writer
             if writer:
                 # Close AVR connection
                 _LOGGER.debug("closing AVR connection")
                 self._writer.close()
                 try:
                     await self._writer.wait_closed()
                 except Exception as exc:  # pylint: disable=broad-except
-                    _LOGGER.debug("ignoring responder exception %s", str(exc))
+                    _LOGGER.debug("ignoring disconnect exception: %s", str(exc))
             self._reader = None
             self._writer = None
             _LOGGER.info("AVR connection closed")
 
             await self._reconnect_schedule()
 
         _LOGGER.debug(">> PioneerAVR.disconnect() completed")
@@ -1140,16 +1140,16 @@
                 if debug_updater:
                     _LOGGER.debug(">> PioneerAVR._updater() cancelled")
                 break
             except Exception as exc:  # pylint: disable=broad-except
                 event.clear()
                 _LOGGER.error(">> PioneerAVR._updater() exception: %s", str(exc))
                 break
-        if debug_updater:
-            _LOGGER.debug(">> PioneerAVR._updater() completed")
+
+        _LOGGER.debug(">> PioneerAVR._updater() completed")
 
     async def _updater_schedule(self) -> None:
         """Schedule/reschedule the update task."""
         if self.scan_interval:
             _LOGGER.debug(">> PioneerAVR._updater_schedule()")
             await self._updater_cancel()
             self._full_update = True  # always perform full update on schedule
@@ -1300,14 +1300,16 @@
             self._full_update = True
         if self._updater_task:
             if self._params[PARAM_DEBUG_UPDATER]:
                 _LOGGER.debug(">> PioneerAVR.update(): signalling updater task")
             self._update_event.set()
             await asyncio.sleep(0)  # yield to updater task
             if wait:
+                if self._params[PARAM_DEBUG_UPDATER]:
+                    _LOGGER.debug(">> PioneerAVR.update(): waiting for updater task")
                 async with self._update_lock:  # wait for update to complete
                     pass
         else:
             # scan_interval not set, execute update synchronously
             if wait:
                 _LOGGER.error("unable to update AVR in background")
             await self._updater_update()
```

### Comparing `aiopioneer-0.6.0a7/aiopioneer/util.py` & `aiopioneer-0.6.0b1/aiopioneer/util.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/aiopioneer.egg-info/PKG-INFO` & `aiopioneer-0.6.0b1/aiopioneer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.6.0a7
+Version: 0.6.0b1
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `aiopioneer-0.6.0a7/aiopioneer.egg-info/SOURCES.txt` & `aiopioneer-0.6.0b1/aiopioneer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a7/setup.py` & `aiopioneer-0.6.0b1/setup.py`

 * *Files identical despite different names*

