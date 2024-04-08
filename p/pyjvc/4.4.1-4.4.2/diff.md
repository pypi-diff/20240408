# Comparing `tmp/pyjvc-4.4.1.tar.gz` & `tmp/pyjvc-4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjvc-4.4.1.tar", last modified: Sun Apr  7 23:44:32 2024, max compression
+gzip compressed data, was "pyjvc-4.4.2.tar", last modified: Mon Apr  8 00:16:56 2024, max compression
```

## Comparing `pyjvc-4.4.1.tar` & `pyjvc-4.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:44:32.919622 pyjvc-4.4.1/
--rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.1/LICENSE
--rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-07 23:44:32.919427 pyjvc-4.4.1/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.1/README.md
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:44:32.916655 pyjvc-4.4.1/jvc_projector/
--rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.1/jvc_projector/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     8881 2024-03-20 01:40:47.000000 pyjvc-4.4.1/jvc_projector/command_runner.py
--rw-r--r--   0 ilan       (501) staff       (20)    10032 2024-04-01 00:26:47.000000 pyjvc-4.4.1/jvc_projector/commands.py
--rw-r--r--   0 ilan       (501) staff       (20)      200 2024-02-17 18:22:01.000000 pyjvc-4.4.1/jvc_projector/error_classes.py
--rw-r--r--   0 ilan       (501) staff       (20)    17611 2024-03-31 23:24:15.000000 pyjvc-4.4.1/jvc_projector/jvc_projector.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:44:32.919185 pyjvc-4.4.1/pyJVC.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-07 23:44:32.000000 pyjvc-4.4.1/pyJVC.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      491 2024-04-07 23:44:32.000000 pyjvc-4.4.1/pyJVC.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-07 23:44:32.000000 pyjvc-4.4.1/pyJVC.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       20 2024-04-07 23:44:32.000000 pyjvc-4.4.1/pyJVC.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-07 23:44:32.919667 pyjvc-4.4.1/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      634 2024-04-07 23:44:11.000000 pyjvc-4.4.1/setup.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:44:32.918843 pyjvc-4.4.1/tests/
--rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.1/tests/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.1/tests/test_commander.py
--rw-r--r--   0 ilan       (501) staff       (20)     8345 2024-03-20 01:40:47.000000 pyjvc-4.4.1/tests/test_coordinator.py
--rw-r--r--   0 ilan       (501) staff       (20)    14935 2024-03-20 01:40:47.000000 pyjvc-4.4.1/tests/test_loop.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:16:56.824573 pyjvc-4.4.2/
+-rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.2/LICENSE
+-rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-08 00:16:56.824337 pyjvc-4.4.2/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.2/README.md
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:16:56.820242 pyjvc-4.4.2/jvc_projector/
+-rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.2/jvc_projector/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     9120 2024-04-08 00:14:11.000000 pyjvc-4.4.2/jvc_projector/command_runner.py
+-rw-r--r--   0 ilan       (501) staff       (20)    10032 2024-04-01 00:26:47.000000 pyjvc-4.4.2/jvc_projector/commands.py
+-rw-r--r--   0 ilan       (501) staff       (20)      200 2024-02-17 18:22:01.000000 pyjvc-4.4.2/jvc_projector/error_classes.py
+-rw-r--r--   0 ilan       (501) staff       (20)    17944 2024-04-08 00:05:42.000000 pyjvc-4.4.2/jvc_projector/jvc_projector.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:16:56.822924 pyjvc-4.4.2/pyJVC.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-08 00:16:56.000000 pyjvc-4.4.2/pyJVC.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      491 2024-04-08 00:16:56.000000 pyjvc-4.4.2/pyJVC.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-08 00:16:56.000000 pyjvc-4.4.2/pyJVC.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       20 2024-04-08 00:16:56.000000 pyjvc-4.4.2/pyJVC.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-08 00:16:56.824619 pyjvc-4.4.2/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      634 2024-04-08 00:16:51.000000 pyjvc-4.4.2/setup.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:16:56.822620 pyjvc-4.4.2/tests/
+-rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.2/tests/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.2/tests/test_commander.py
+-rw-r--r--   0 ilan       (501) staff       (20)     8345 2024-03-20 01:40:47.000000 pyjvc-4.4.2/tests/test_coordinator.py
+-rw-r--r--   0 ilan       (501) staff       (20)    14935 2024-03-20 01:40:47.000000 pyjvc-4.4.2/tests/test_loop.py
```

### Comparing `pyjvc-4.4.1/LICENSE` & `pyjvc-4.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.1/PKG-INFO` & `pyjvc-4.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.1
+Version: 4.4.2
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.1/README.md` & `pyjvc-4.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.1/jvc_projector/command_runner.py` & `pyjvc-4.4.2/jvc_projector/command_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,78 +109,77 @@
 
     async def _do_command(
         self,
         final_cmd: bytes,
         ack: bytes,
         command_type: bytes,
     ) -> tuple[Union[str, bytes]]:
-        self.logger.debug("final_cmd: %s with ack %s", final_cmd, ack)
-        # ensure this doesnt run with dead client
-        if self.writer is None:
-            self.logger.debug("Writer is closed")
-            raise ConnectionClosedError("writer is none")
-
-        self.logger.debug("do_command sending command: %s", final_cmd)
-        # send the command
-        try:
-            self.logger.debug("acquiring command lock")
-            async with self.lock:
+        async with self.lock:
+            self.logger.debug("final_cmd: %s with ack %s", final_cmd, ack)
+            # ensure this doesnt run with dead client
+            if self.writer is None:
+                self.logger.debug("Writer is closed")
+                raise ConnectionClosedError("writer is none")
+
+            self.logger.debug("do_command sending command: %s", final_cmd)
+            # send the command
+            try:
+                self.logger.debug("acquiring command lock")
                 self.writer.write(final_cmd)
                 await self.writer.drain()
-            self.logger.debug("released command lock")
-        except BrokenPipeError as err:
-            self.logger.error(
-                "BrokenPipeError in _do_command restarting connection: %s", err
-            )
-            # Attempt to reconnect or handle the broken pipe scenario
-            raise ConnectionClosedError("Broken pipe") from err
-        except ConnectionResetError as err:
-            self.logger.debug("ConnectionResetError in _do_command: %s", err)
-            # Handle connection reset specifically, if different from broken pipe
-            raise ConnectionClosedError("Connection reset") from err
-        except ConnectionError as err:
-            # reaching this means the writer was closed somewhere
-            self.logger.debug("ConnectionError in _do_command: %s", err)
-            raise ConnectionClosedError(err) from err
-        # if we send a command that returns info, the projector will send
-        # an ack, followed by the actual message. Check to see if the ack sent by
-        # projector is correct, then return the message.
-
-        ack_value = Header.ack.value + Header.pj_unit.value + ack + Footer.close.value
-        self.logger.debug("constructed ack_value: %s", ack_value)
-
-        # Receive the acknowledgement from PJ
-        try:
-            # read everything
-            self.logger.debug("acquiring command read lock")
-            async with self.lock:
+                self.logger.debug("released command lock")
+            except BrokenPipeError as err:
+                self.logger.error(
+                    "BrokenPipeError in _do_command restarting connection: %s", err
+                )
+                # Attempt to reconnect or handle the broken pipe scenario
+                raise ConnectionClosedError("Broken pipe") from err
+            except ConnectionResetError as err:
+                self.logger.debug("ConnectionResetError in _do_command: %s", err)
+                # Handle connection reset specifically, if different from broken pipe
+                raise ConnectionClosedError("Connection reset") from err
+            except ConnectionError as err:
+                # reaching this means the writer was closed somewhere
+                self.logger.debug("ConnectionError in _do_command: %s", err)
+                raise ConnectionClosedError(err) from err
+            # if we send a command that returns info, the projector will send
+            # an ack, followed by the actual message. Check to see if the ack sent by
+            # projector is correct, then return the message.
+
+            ack_value = Header.ack.value + Header.pj_unit.value + ack + Footer.close.value
+            self.logger.debug("constructed ack_value: %s", ack_value)
+
+            # Receive the acknowledgement from PJ
+            try:
+                # read everything
+                self.logger.debug("acquiring command read lock")
+                # TODO: its probably way more reliable to read everything and just search for the data we want
                 msg = await self.reader.read(len(ack_value))
                 self.logger.debug("received msg in _do_command: %s", msg)
 
-            # read the actual message, if any
-            if msg == b"":  # if we got a blank response
-                self.logger.debug("Got a blank response")
-                raise BlankMessageError("Got a blank response")
-            if command_type == Header.operation.value:
-                return msg, True
-            else:
-                async with self.lock:
+                # read the actual message, if any
+                if msg == b"":  # if we got a blank response
+                    self.logger.debug("Got a blank response")
+                    raise BlankMessageError("Got a blank response")
+                if command_type == Header.operation.value:
+                    return msg, True
+                else:
                     ref_msg = await self.reader.read(1000)
-                self.logger.debug("received ref_msg in _do_command: %s", ref_msg)
-                # msg = await self._check_received_msg(received_ack, ack_value, command_type)
-                self.logger.debug("finished reading ref_msg")
-                return ref_msg.replace(ack_value, b"")
-        except socket.timeout as err:
-            error = f"Timed out. Command {final_cmd} may grayed out or cmd is running already."
-            self.logger.debug(err)
-            raise CommandTimeoutError(error) from err
-
-        except ConnectionRefusedError as err:
-            self.logger.debug(err)
-            raise ConnectionRefusedError(error) from err
+                    self.logger.debug("received ref_msg in _do_command: %s", ref_msg)
+                    # msg = await self._check_received_msg(received_ack, ack_value, command_type)
+                    self.logger.debug("finished reading ref_msg")
+                    return ref_msg.replace(ack_value, b"")
+            except socket.timeout as err:
+                error = f"Timed out. Command {final_cmd} may grayed out or cmd is running already."
+                self.logger.debug(err)
+                raise CommandTimeoutError(error) from err
+
+            except ConnectionRefusedError as err:
+                self.logger.debug(err)
+                raise ConnectionRefusedError(error) from err
 
     # TODO: use this to construct commands from a list that is a str like ["menu,menu"]
     def construct_command(
         self, raw_command: str, command_type: bytes
     ) -> tuple[bytes, ACKs]:
         """
         Transform commands into their byte values from the string value
```

### Comparing `pyjvc-4.4.1/jvc_projector/commands.py` & `pyjvc-4.4.2/jvc_projector/commands.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.1/jvc_projector/jvc_projector.py` & `pyjvc-4.4.2/jvc_projector/jvc_projector.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         self.writer: asyncio.StreamWriter = None
 
         self.model_family = ""
         self.connection_open = False
         # attribute mapping
         self.attributes = JVCAttributes()
         self.lock = asyncio.Lock()
+        self.attr_lock = asyncio.Lock()
+        self.exec_lock = asyncio.Lock()
 
         self.commander = JVCCommander(
             options.host,
             options.port,
             options.password,
             options.connect_timeout,
             logger,
@@ -234,41 +236,42 @@
 
 
         command_type: which operation, like ! or ? (default = !)
 
         Returns
             value: str (to be cast into other types),
         """
-        self.logger.debug(
-            "exec_command Executing command: %s - %s", command, command_type
-        )
-        retries = 0
-        while retries < 3:
-            try:
-                res = await self.commander.send_command(command, command_type)
-                if not res:
-                    self.logger.debug("Command failed. Retrying")
-                    retries += 1
+        async with self.exec_lock:
+            self.logger.debug(
+                "exec_command Executing command: %s - %s", command, command_type
+            )
+            retries = 0
+            while retries < 3:
+                try:
+                    res = await self.commander.send_command(command, command_type)
+                    if not res:
+                        self.logger.debug("Command failed. Retrying")
+                        retries += 1
+                        continue
+                    return res
+                except (
+                    ConnectionClosedError,
+                    CommandTimeoutError,
+                    ConnectionRefusedError,
+                    BrokenPipeError,
+                ):
+                    self.logger.debug(
+                        "Connection closed. Opening new connection. Retry your command"
+                    )
+                    # open connection and try again
+                    await self.open_connection()
+                    await asyncio.sleep(1)
                     continue
-                return res
-            except (
-                ConnectionClosedError,
-                CommandTimeoutError,
-                ConnectionRefusedError,
-                BrokenPipeError,
-            ):
-                self.logger.debug(
-                    "Connection closed. Opening new connection. Retry your command"
-                )
-                # open connection and try again
-                await self.open_connection()
-                await asyncio.sleep(1)
-                continue
 
-        return None
+            return None
 
     async def close_connection(self):
         """Close the projector connection asynchronously"""
         try:
             if self.writer:
                 self.writer.close()
                 await self.writer.wait_closed()
@@ -298,40 +301,41 @@
         """
         return await self.exec_command("power,off")
 
     async def _get_attribute(self, command: str, replace: bool = True) -> str:
         """
         Generic function to get the current attribute asynchronously
         """
-        cmd_tup = Commands[command].value
-        cmd_enum = cmd_tup[1]
-        ack = cmd_tup[2]
-        self.logger.debug("Getting attribute %s with tuple %s", command, cmd_tup)
-        try:
-            state = await self.exec_command(command, Header.reference.value)
-            if not state:
-                self.logger.debug("%s Command failed", command)
-                return ""
-            if replace:
-                # remove the returned headers
-                r = self.commander.replace_headers(state)
-                if not isinstance(r, bytes):
-                    self.logger.error("Attribute %s is not bytes", command)
+        async with self.attr_lock:
+            cmd_tup = Commands[command].value
+            cmd_enum = cmd_tup[1]
+            ack = cmd_tup[2]
+            self.logger.debug("Getting attribute %s with tuple %s", command, cmd_tup)
+            try:
+                state = await self.exec_command(command, Header.reference.value)
+                if not state:
+                    self.logger.debug("%s Command failed", command)
                     return ""
-                self.logger.debug("Attribute %s is %s", command, r)
-                # look up the enum value like b"1" -> on in PowerModes
-                return cmd_enum(r.replace(ack.value, b"")).name
-            else:
+                if replace:
+                    # remove the returned headers
+                    r = self.commander.replace_headers(state)
+                    if not isinstance(r, bytes):
+                        self.logger.error("Attribute %s is not bytes", command)
+                        return ""
+                    self.logger.debug("Attribute %s is %s", command, r)
+                    # look up the enum value like b"1" -> on in PowerModes
+                    return cmd_enum(r.replace(ack.value, b"")).name
+
                 return state
-        except ValueError as err:
-            self.logger.error("Attribute not found - %s", err)
-            raise
-        except AttributeError as err:
-            self.logger.error("tried to access name on non-enum: %s", err)
-            return ""
+            except ValueError as err:
+                self.logger.error("Attribute not found - %s", err)
+                raise
+            except AttributeError as err:
+                self.logger.error("tried to access name on non-enum: %s", err)
+                return ""
 
     async def get_low_latency_state(self) -> str:
         """
         Get the current state of LL
         """
         return await self._get_attribute("low_latency") == LowLatencyModes.on.name
```

### Comparing `pyjvc-4.4.1/pyJVC.egg-info/PKG-INFO` & `pyjvc-4.4.2/pyJVC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.1
+Version: 4.4.2
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.1/setup.py` & `pyjvc-4.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyjvc",
-    version="4.4.1",
+    version="4.4.2",
     author="iloveicedgreentea2",
     description="A package to control JVC projectors over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/jvc_projector_improved",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `pyjvc-4.4.1/tests/test_commander.py` & `pyjvc-4.4.2/tests/test_commander.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.1/tests/test_coordinator.py` & `pyjvc-4.4.2/tests/test_coordinator.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.1/tests/test_loop.py` & `pyjvc-4.4.2/tests/test_loop.py`

 * *Files identical despite different names*

