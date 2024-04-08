# Comparing `tmp/pyjvc-4.4.2.tar.gz` & `tmp/pyjvc-4.4.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjvc-4.4.2.tar", last modified: Mon Apr  8 00:16:56 2024, max compression
+gzip compressed data, was "pyjvc-4.4.21.tar", last modified: Mon Apr  8 00:35:32 2024, max compression
```

## Comparing `pyjvc-4.4.2.tar` & `pyjvc-4.4.21.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:16:56.824573 pyjvc-4.4.2/
--rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.2/LICENSE
--rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-08 00:16:56.824337 pyjvc-4.4.2/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.2/README.md
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:16:56.820242 pyjvc-4.4.2/jvc_projector/
--rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.2/jvc_projector/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     9120 2024-04-08 00:14:11.000000 pyjvc-4.4.2/jvc_projector/command_runner.py
--rw-r--r--   0 ilan       (501) staff       (20)    10032 2024-04-01 00:26:47.000000 pyjvc-4.4.2/jvc_projector/commands.py
--rw-r--r--   0 ilan       (501) staff       (20)      200 2024-02-17 18:22:01.000000 pyjvc-4.4.2/jvc_projector/error_classes.py
--rw-r--r--   0 ilan       (501) staff       (20)    17944 2024-04-08 00:05:42.000000 pyjvc-4.4.2/jvc_projector/jvc_projector.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:16:56.822924 pyjvc-4.4.2/pyJVC.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-08 00:16:56.000000 pyjvc-4.4.2/pyJVC.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      491 2024-04-08 00:16:56.000000 pyjvc-4.4.2/pyJVC.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-08 00:16:56.000000 pyjvc-4.4.2/pyJVC.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       20 2024-04-08 00:16:56.000000 pyjvc-4.4.2/pyJVC.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-08 00:16:56.824619 pyjvc-4.4.2/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      634 2024-04-08 00:16:51.000000 pyjvc-4.4.2/setup.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:16:56.822620 pyjvc-4.4.2/tests/
--rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.2/tests/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.2/tests/test_commander.py
--rw-r--r--   0 ilan       (501) staff       (20)     8345 2024-03-20 01:40:47.000000 pyjvc-4.4.2/tests/test_coordinator.py
--rw-r--r--   0 ilan       (501) staff       (20)    14935 2024-03-20 01:40:47.000000 pyjvc-4.4.2/tests/test_loop.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:35:32.471122 pyjvc-4.4.21/
+-rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.21/LICENSE
+-rw-r--r--   0 ilan       (501) staff       (20)     6182 2024-04-08 00:35:32.470905 pyjvc-4.4.21/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.21/README.md
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:35:32.468071 pyjvc-4.4.21/jvc_projector/
+-rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.21/jvc_projector/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     9120 2024-04-08 00:14:11.000000 pyjvc-4.4.21/jvc_projector/command_runner.py
+-rw-r--r--   0 ilan       (501) staff       (20)    10032 2024-04-01 00:26:47.000000 pyjvc-4.4.21/jvc_projector/commands.py
+-rw-r--r--   0 ilan       (501) staff       (20)      200 2024-02-17 18:22:01.000000 pyjvc-4.4.21/jvc_projector/error_classes.py
+-rw-r--r--   0 ilan       (501) staff       (20)    17809 2024-04-08 00:34:07.000000 pyjvc-4.4.21/jvc_projector/jvc_projector.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:35:32.470661 pyjvc-4.4.21/pyJVC.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)     6182 2024-04-08 00:35:32.000000 pyjvc-4.4.21/pyJVC.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      491 2024-04-08 00:35:32.000000 pyjvc-4.4.21/pyJVC.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-08 00:35:32.000000 pyjvc-4.4.21/pyJVC.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       20 2024-04-08 00:35:32.000000 pyjvc-4.4.21/pyJVC.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-08 00:35:32.471168 pyjvc-4.4.21/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      635 2024-04-08 00:35:26.000000 pyjvc-4.4.21/setup.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:35:32.470344 pyjvc-4.4.21/tests/
+-rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.21/tests/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.21/tests/test_commander.py
+-rw-r--r--   0 ilan       (501) staff       (20)     8345 2024-03-20 01:40:47.000000 pyjvc-4.4.21/tests/test_coordinator.py
+-rw-r--r--   0 ilan       (501) staff       (20)    14935 2024-03-20 01:40:47.000000 pyjvc-4.4.21/tests/test_loop.py
```

### Comparing `pyjvc-4.4.2/LICENSE` & `pyjvc-4.4.21/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.2/PKG-INFO` & `pyjvc-4.4.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.2
+Version: 4.4.21
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.2/README.md` & `pyjvc-4.4.21/README.md`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.2/jvc_projector/command_runner.py` & `pyjvc-4.4.21/jvc_projector/command_runner.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.2/jvc_projector/commands.py` & `pyjvc-4.4.21/jvc_projector/commands.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.2/jvc_projector/jvc_projector.py` & `pyjvc-4.4.21/jvc_projector/jvc_projector.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,41 +301,40 @@
         """
         return await self.exec_command("power,off")
 
     async def _get_attribute(self, command: str, replace: bool = True) -> str:
         """
         Generic function to get the current attribute asynchronously
         """
-        async with self.attr_lock:
-            cmd_tup = Commands[command].value
-            cmd_enum = cmd_tup[1]
-            ack = cmd_tup[2]
-            self.logger.debug("Getting attribute %s with tuple %s", command, cmd_tup)
-            try:
-                state = await self.exec_command(command, Header.reference.value)
-                if not state:
-                    self.logger.debug("%s Command failed", command)
+        cmd_tup = Commands[command].value
+        cmd_enum = cmd_tup[1]
+        ack = cmd_tup[2]
+        self.logger.debug("Getting attribute %s with tuple %s", command, cmd_tup)
+        try:
+            state = await self.exec_command(command, Header.reference.value)
+            if not state:
+                self.logger.debug("%s Command failed", command)
+                return ""
+            if replace:
+                # remove the returned headers
+                r = self.commander.replace_headers(state)
+                if not isinstance(r, bytes):
+                    self.logger.error("Attribute %s is not bytes", command)
                     return ""
-                if replace:
-                    # remove the returned headers
-                    r = self.commander.replace_headers(state)
-                    if not isinstance(r, bytes):
-                        self.logger.error("Attribute %s is not bytes", command)
-                        return ""
-                    self.logger.debug("Attribute %s is %s", command, r)
-                    # look up the enum value like b"1" -> on in PowerModes
-                    return cmd_enum(r.replace(ack.value, b"")).name
+                self.logger.debug("Attribute %s is %s", command, r)
+                # look up the enum value like b"1" -> on in PowerModes
+                return cmd_enum(r.replace(ack.value, b"")).name
 
-                return state
-            except ValueError as err:
-                self.logger.error("Attribute not found - %s", err)
-                raise
-            except AttributeError as err:
-                self.logger.error("tried to access name on non-enum: %s", err)
-                return ""
+            return state
+        except ValueError as err:
+            self.logger.error("Attribute not found - %s", err)
+            raise
+        except AttributeError as err:
+            self.logger.error("tried to access name on non-enum: %s", err)
+            return ""
 
     async def get_low_latency_state(self) -> str:
         """
         Get the current state of LL
         """
         return await self._get_attribute("low_latency") == LowLatencyModes.on.name
```

### Comparing `pyjvc-4.4.2/pyJVC.egg-info/PKG-INFO` & `pyjvc-4.4.21/pyJVC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.2
+Version: 4.4.21
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.2/setup.py` & `pyjvc-4.4.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyjvc",
-    version="4.4.2",
+    version="4.4.21",
     author="iloveicedgreentea2",
     description="A package to control JVC projectors over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/jvc_projector_improved",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `pyjvc-4.4.2/tests/test_commander.py` & `pyjvc-4.4.21/tests/test_commander.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.2/tests/test_coordinator.py` & `pyjvc-4.4.21/tests/test_coordinator.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.2/tests/test_loop.py` & `pyjvc-4.4.21/tests/test_loop.py`

 * *Files identical despite different names*

