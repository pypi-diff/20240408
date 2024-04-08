# Comparing `tmp/shadeorb-0.0.2.tar.gz` & `tmp/shadeorb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadeorb-0.0.2.tar", max compression
+gzip compressed data, was "shadeorb-0.0.3.tar", max compression
```

## Comparing `shadeorb-0.0.2.tar` & `shadeorb-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1082 2024-02-22 14:59:41.815004 shadeorb-0.0.2/LICENSE
--rw-r--r--   0        0        0       54 2024-02-22 14:58:42.492844 shadeorb-0.0.2/README.md
--rw-r--r--   0        0        0      780 2024-02-23 22:02:23.363945 shadeorb-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      102 2024-02-22 14:55:16.382287 shadeorb-0.0.2/shadeorb/__init__.py
--rw-r--r--   0        0        0      691 2024-02-22 14:55:16.382287 shadeorb-0.0.2/shadeorb/const.py
--rw-r--r--   0        0        0       95 2024-02-22 14:55:16.382287 shadeorb-0.0.2/shadeorb/exceptions.py
--rw-r--r--   0        0        0      404 2024-02-22 14:55:16.382287 shadeorb-0.0.2/shadeorb/models.py
--rw-r--r--   0        0        0    18351 2024-02-23 14:08:18.139778 shadeorb-0.0.2/shadeorb/orb.py
--rw-r--r--   0        0        0     2275 2024-02-23 12:17:13.635551 shadeorb-0.0.2/shadeorb/protocol.py
--rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 shadeorb-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-08 11:36:06.120201 shadeorb-0.0.3/LICENSE
+-rw-r--r--   0        0        0       54 2024-04-08 11:36:06.120201 shadeorb-0.0.3/README.md
+-rw-r--r--   0        0        0      796 2024-04-08 11:36:06.120201 shadeorb-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      154 2024-04-08 11:36:06.120201 shadeorb-0.0.3/shadeorb/__init__.py
+-rw-r--r--   0        0        0      693 2024-04-08 11:36:06.120201 shadeorb-0.0.3/shadeorb/const.py
+-rw-r--r--   0        0        0       96 2024-04-08 11:36:06.120201 shadeorb-0.0.3/shadeorb/exceptions.py
+-rw-r--r--   0        0        0      409 2024-04-08 11:36:06.120201 shadeorb-0.0.3/shadeorb/models.py
+-rw-r--r--   0        0        0    18549 2024-04-08 11:36:06.120201 shadeorb-0.0.3/shadeorb/orb.py
+-rw-r--r--   0        0        0     2440 2024-04-08 11:36:06.120201 shadeorb-0.0.3/shadeorb/protocol.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 shadeorb-0.0.3/PKG-INFO
```

### Comparing `shadeorb-0.0.2/LICENSE` & `shadeorb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shadeorb-0.0.2/pyproject.toml` & `shadeorb-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shadeorb"
-version = "0.0.2"
+version = "0.0.3"
 description = "Package to control Shade ORB lights"
 authors = ["Yngvi Thor Sigurjonsson <blitzkopf@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/blitzkopf/shadeorb"
 repository = "https://github.com/blitzkopf/shadeorb"
 keywords = ["shadeorb", "lights", "bleak", "bluetooth", "homeassistant"]
@@ -16,14 +16,15 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 bleak = "^0.21.1"
 bleak-retry-connector = "^3.4.0"
 bitstruct = "^8.19.0"
+ruff = "^0.3.5"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `shadeorb-0.0.2/shadeorb/const.py` & `shadeorb-0.0.3/shadeorb/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#BASE_UUID_FORMAT = "0000{}-0000-1000-8000-00805f9b34fb"
+# BASE_UUID_FORMAT = "0000{}-0000-1000-8000-00805f9b34fb"
 BASE_UUID_FORMAT = "0000{}-3d1c-019e-ab4a-65fd86e87333"
 # "00001523-3d1c-019e-ab4a-65fd86e87333'
 # '00001521-3d1c-019e-ab4a-65fd86e87333'
 # '00001522-3d1c-019e-ac4a-65fd86e87333'
 
 
 # "ff01" - 0x97 socket - LEDnetWF010097DAB37A, LEDnetWF01001C49D272
@@ -16,8 +16,8 @@
 POSSIBLE_WRITE_CHARACTERISTIC_UUIDS = [
     BASE_UUID_FORMAT.format(part) for part in ["1523"]
 ]
 POSSIBLE_READ_CHARACTERISTIC_UUIDS = [
     BASE_UUID_FORMAT.format(part) for part in ["1527"]
 ]
 
-QUERY_STATE_BYTES = bytearray([0xEF, 0x01, 0x77])
+QUERY_STATE_BYTES = bytearray([0xEF, 0x01, 0x77])
```

### Comparing `shadeorb-0.0.2/shadeorb/orb.py` & `shadeorb-0.0.3/shadeorb/orb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import logging
 
 from collections.abc import Callable
 from dataclasses import replace
-from typing import Any, TypeVar
 
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
 from bleak.backends.service import BleakGATTCharacteristic, BleakGATTServiceCollection
 from bleak.exc import BleakDBusError
 from bleak_retry_connector import BLEAK_RETRY_EXCEPTIONS as BLEAK_EXCEPTIONS
 from bleak_retry_connector import (
@@ -32,36 +31,40 @@
 _LOGGER = logging.getLogger(__name__)
 
 DEFAULT_ATTEMPTS = 3
 
 
 class ORB:
     def __init__(
-        self, ble_device: BLEDevice,
+        self,
+        ble_device: BLEDevice,
         cmd_prefix: str,
-        advertisement_data: AdvertisementData | None = None
+        advertisement_data: AdvertisementData | None = None,
     ) -> None:
         self._ble_device = ble_device
-        self._cmd_prefix = bytes.fromhex(cmd_prefix.translate({ord(i): None for i in ' -:'}))
+        self._cmd_prefix = bytes.fromhex(
+            cmd_prefix.translate({ord(i): None for i in " -:"})
+        )
         self._advertisement_data = advertisement_data
         self._operation_lock = asyncio.Lock()
         self._state = ORBState()
         self._connect_lock: asyncio.Lock = asyncio.Lock()
         self._read_char: BleakGATTCharacteristic | None = None
         self._write_char: BleakGATTCharacteristic | None = None
         self._disconnect_timer: asyncio.TimerHandle | None = None
         self._client: BleakClientWithServiceCache | None = None
         self._expected_disconnect = False
         self.loop = asyncio.get_running_loop()
         self._callbacks: list[Callable[[ORBState], None]] = []
-        #self._model_data: ORBModel | None = None
-        #self._protocol: PROTOCOL_TYPES | None = None
-        self._protocol= ORBProtocol()
+        # self._model_data: ORBModel | None = None
+        # self._protocol: PROTOCOL_TYPES | None = None
+        self._protocol = ORBProtocol()
 
         self._resolve_protocol_event = asyncio.Event()
+
     def set_ble_device_and_advertisement_data(
         self, ble_device: BLEDevice, advertisement_data: AdvertisementData
     ) -> None:
         """Set the ble device."""
         self._ble_device = ble_device
         self._advertisement_data = advertisement_data
 
@@ -102,47 +105,50 @@
     def on(self) -> bool:
         _LOGGER.debug("%s: Getting power %s", self.name, self._state.power)
         return self._state.power
 
     @property
     def effect_list(self):
         """Return the list of supported effects."""
-        return ['0','1','2','3','4','5','6','7']
+        return ["0", "1", "2", "3", "4", "5", "6", "7"]
 
     async def update(self) -> None:
         """Update the Orb."""
         await self._ensure_connected()
-        #await self._resolve_protocol()
+        # await self._resolve_protocol()
         _LOGGER.debug("%s: Updating", self.name)
         assert self._protocol is not None  # nosec
         # I have no idea how to get the state of the orb
-        #command = self._protocol.construct_state_query()
-        #await self._send_command([command])
+        # command = self._protocol.construct_state_query()
+        # await self._send_command([command])
         ## YS: this really should not be here
         self._fire_callbacks()
 
-
     async def turn_on(self) -> None:
         """Turn on."""
         _LOGGER.debug("%s: Turn on", self.name)
         assert self._protocol is not None  # nosec
-        await self._send_command(self._protocol.construct_state_change(self._cmd_prefix,True))
+        await self._send_command(
+            self._protocol.construct_state_change(self._cmd_prefix, True)
+        )
         self._state = replace(self._state, power=True)
         self._fire_callbacks()
 
     async def turn_off(self) -> None:
         """Turn off."""
         _LOGGER.debug("%s: Turn off", self.name)
         assert self._protocol is not None  # nosec
-        await self._send_command(self._protocol.construct_state_change(self._cmd_prefix,False))
+        await self._send_command(
+            self._protocol.construct_state_change(self._cmd_prefix, False)
+        )
         self._state = replace(self._state, power=False)
         self._fire_callbacks()
 
     async def set_edge_rgbw(
-        self, rgbw: tuple[int, int, int,int], brightness: int | None = None
+        self, rgbw: tuple[int, int, int, int], brightness: int | None = None
     ) -> None:
         """Set rgb."""
         _LOGGER.debug("%s: Set rgb: %s brightness: %s", self.name, rgbw, brightness)
         for value in rgbw:
             if not 0 <= value <= 4095:
                 raise ValueError("Value {} is outside the valid range of 0-4095")
         # if brightness is not None:
@@ -150,30 +156,33 @@
         _LOGGER.debug("%s: Set rgbw after brightness: %s", self.name, rgbw)
         assert self._protocol is not None  # nosec
 
         command = self._protocol.construct_levels_change(
             self._cmd_prefix,
             *self._state.inner_warm_cold,
             *self._state.outer_warm_cold,
-            rgbw[3], *rgbw[0:3], 
+            rgbw[3],
+            *rgbw[0:3],
         )
-        print('Command:',command.hex())
+        print("Command:", command.hex())
         await self._send_command(command)
         self._state = replace(
             self._state,
             edge_rgbw=rgbw,
-            #preset_pattern=1 if self.dream else self.preset_pattern_num,
+            # preset_pattern=1 if self.dream else self.preset_pattern_num,
         )
         self._fire_callbacks()
 
     async def set_inner_whites(
         self, whites: tuple[int, int], brightness: int | None = None
     ) -> None:
         """Set rgb."""
-        _LOGGER.debug("%s: Set light 0 whites: %s brightness: %s", self.name, whites, brightness)
+        _LOGGER.debug(
+            "%s: Set light 0 whites: %s brightness: %s", self.name, whites, brightness
+        )
         for value in whites:
             if not 0 <= value <= 4095:
                 raise ValueError("Value {} is outside the valid range of 0-4095")
         # if brightness is not None:
         #     rgb = self._calculate_brightness(rgb, brightness)
         _LOGGER.debug("%s: Set whites after brightness: %s", self.name, whites)
         assert self._protocol is not None  # nosec
@@ -181,28 +190,30 @@
         command = self._protocol.construct_levels_change(
             self._cmd_prefix,
             *whites,
             *self._state.outer_warm_cold,
             self._state.edge_rgbw[3],
             *self._state.edge_rgbw[0:3],
         )
-        print('Command:',command.hex())
+        print("Command:", command.hex())
         await self._send_command(command)
         self._state = replace(
             self._state,
             inner_warm_cold=whites,
-            #preset_pattern=1 if self.dream else self.preset_pattern_num,
+            # preset_pattern=1 if self.dream else self.preset_pattern_num,
         )
         self._fire_callbacks()
 
     async def set_outer_whites(
         self, whites: tuple[int, int], brightness: int | None = None
     ) -> None:
         """Set rgb."""
-        _LOGGER.debug("%s: Set light 0 whites: %s brightness: %s", self.name, whites, brightness)
+        _LOGGER.debug(
+            "%s: Set light 0 whites: %s brightness: %s", self.name, whites, brightness
+        )
         for value in whites:
             if not 0 <= value <= 4095:
                 raise ValueError("Value {} is outside the valid range of 0-4095")
         # if brightness is not None:
         #     rgb = self._calculate_brightness(rgb, brightness)
         _LOGGER.debug("%s: Set whites after brightness: %s", self.name, whites)
         assert self._protocol is not None  # nosec
@@ -210,32 +221,33 @@
         command = self._protocol.construct_levels_change(
             self._cmd_prefix,
             *self._state.inner_warm_cold,
             *whites,
             self._state.edge_rgbw[3],
             *self._state.edge_rgbw[0:3],
         )
-        print('Command:',command.hex())
+        print("Command:", command.hex())
         await self._send_command(command)
         self._state = replace(
             self._state,
             outer_warm_cold=whites,
-            #preset_pattern=1 if self.dream else self.preset_pattern_num,
+            # preset_pattern=1 if self.dream else self.preset_pattern_num,
         )
         self._fire_callbacks()
 
     async def set_effect(self, effect: str, brightness: int) -> None:
         """Set an effect."""
-        _LOGGER.debug("%s: Set effect: %s brightness: %s", self.name, effect, brightness)
+        _LOGGER.debug(
+            "%s: Set effect: %s brightness: %s", self.name, effect, brightness
+        )
         assert self._protocol is not None
-        command = self._protocol.construct_effect_start(self._cmd_prefix,int(effect))
+        command = self._protocol.construct_effect_start(self._cmd_prefix, int(effect))
         await self._send_command(command)
         self._fire_callbacks()
 
-
     async def stop(self) -> None:
         """Stop the ORB."""
         _LOGGER.debug("%s: Stop", self.name)
         await self._execute_disconnect()
 
     # def _calculate_brightness(
     #     self, rgb: tuple[int, int, int], level: int
@@ -316,14 +328,15 @@
             )
             return
         _LOGGER.warning(
             "%s: Device unexpectedly disconnected; RSSI: %s",
             self.name,
             self.rssi,
         )
+
     def _disconnect(self) -> None:
         """Disconnect from device."""
         self._disconnect_timer = None
         asyncio.create_task(self._execute_timed_disconnect())
 
     async def _execute_timed_disconnect(self) -> None:
         """Execute timed disconnection."""
@@ -348,14 +361,15 @@
                     try:
                         await client.stop_notify(read_char)
                     except BleakError:
                         _LOGGER.debug(
                             "%s: Failed to stop notifications", self.name, exc_info=True
                         )
                 await client.disconnect()
+
     async def _ensure_connected(self) -> None:
         """Ensure connection to device is established."""
         if self._connect_lock.locked():
             _LOGGER.debug(
                 "%s: Connection already in progress, waiting for it to complete; RSSI: %s",
                 self.name,
                 self.rssi,
@@ -419,15 +433,16 @@
             raise
 
     async def _send_command(
         self, commands: list[bytes] | bytes, retry: int | None = None
     ) -> None:
         """Send command to device and read response."""
         await self._ensure_connected()
-        #await self._resolve_protocol()
+        print("sending to :", self._client.address)
+        # await self._resolve_protocol()
         if not isinstance(commands, list):
             commands = [commands]
         await self._send_command_while_connected(commands, retry)
 
     async def _send_command_while_connected(
         self, commands: list[bytes], retry: int | None = None
     ) -> None:
@@ -487,8 +502,8 @@
             if char := services.get_characteristic(characteristic):
                 self._read_char = char
                 break
         for characteristic in POSSIBLE_WRITE_CHARACTERISTIC_UUIDS:
             if char := services.get_characteristic(characteristic):
                 self._write_char = char
                 break
-        return bool(self._read_char and self._write_char)
+        return bool(self._read_char and self._write_char)
```

### Comparing `shadeorb-0.0.2/shadeorb/protocol.py` & `shadeorb-0.0.3/shadeorb/protocol.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from bitstruct import pack as bitpack
 from struct import pack
-from typing import Dict, List, NamedTuple, Optional, Tuple, Union
+from typing import List
+
 
 class ORBProtocol:
 
     def construct_message(self, raw_bytes: bytearray) -> bytearray:
         """Original protocol uses no checksum."""
         return raw_bytes
 
@@ -14,57 +15,69 @@
         return 0x01
 
     @property
     def off_byte(self) -> int:
         """The off byte."""
         return 0x00
 
-    def construct_state_change(self,cmd_prefix: bytes, turn_on: int) -> bytearray:
+    def construct_state_change(self, cmd_prefix: bytes, turn_on: int) -> bytearray:
         """The bytes to send for a state change request."""
         return self.construct_message(
-            bytearray(cmd_prefix) + bytearray([ 0x00, 0x41, 0x06, self.on_byte if turn_on else self.off_byte])
+            bytearray(cmd_prefix)
+            + bytearray([0x00, 0x41, 0x06, self.on_byte if turn_on else self.off_byte])
         )
 
     def construct_levels_change(
         self,
         cmd_prefix: bytes,
         inner_warm_white: int,
         inner_cool_white: int,
         outer_warm_white: int,
         outer_cool_white: int,
         edge_white: int,
         edge_red: int,
         edge_green: int,
         edge_blue: int,
-        #write_mode: LevelWriteMode,
+        # write_mode: LevelWriteMode,
     ) -> List[bytearray]:
         """The bytes to send for a level change request."""
-        inner_bytes=bitpack('u12u12',inner_warm_white,inner_cool_white)
-        print('inner_bytes:',inner_bytes.hex())
-        outer_bytes=bitpack('u12u12',outer_warm_white,outer_cool_white)
-        print('inner_bytes:',outer_bytes.hex())
-        print('Colors:',edge_red,edge_green,edge_blue,edge_white)
-        edge_bytes=bitpack('u12u12u12u12',edge_white,edge_red,edge_green,edge_blue)
-        print('edge_bytes:',edge_bytes.hex())
+        inner_bytes = bitpack("u12u12", inner_warm_white, inner_cool_white)
+        print("inner_bytes:", inner_bytes.hex())
+        outer_bytes = bitpack("u12u12", outer_warm_white, outer_cool_white)
+        print("inner_bytes:", outer_bytes.hex())
+        print("Colors:", edge_red, edge_green, edge_blue, edge_white)
+        edge_bytes = bitpack(
+            "u12u12u12u12", edge_white, edge_red, edge_green, edge_blue
+        )
+        print("edge_bytes:", edge_bytes.hex())
         return self.construct_message(
-            bytearray(cmd_prefix) 
+            bytearray(cmd_prefix)
             + bytearray(
                 [
-                    0x00, 0x41, 0x11, 0xFF,
+                    0x00,
+                    0x41,
+                    0x11,
+                    0xFF,
                 ]
-            )+inner_bytes+outer_bytes+edge_bytes
+            )
+            + inner_bytes
+            + outer_bytes
+            + edge_bytes
         )
-    
+
     def construct_effect_start(
         self,
         cmd_prefix: bytes,
         effect: int,
     ) -> List[bytearray]:
         """The bytes to send for a level change request."""
         return self.construct_message(
-            bytearray(cmd_prefix) 
+            bytearray(cmd_prefix)
             + bytearray(
                 [
-                     0xC0, 0x01, 0x01, 
+                    0xC0,
+                    0x01,
+                    0x01,
                 ]
-            )+pack('B',effect)
-        )
+            )
+            + pack("B", effect)
+        )
```

### Comparing `shadeorb-0.0.2/PKG-INFO` & `shadeorb-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadeorb
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to control Shade ORB lights
 Home-page: https://github.com/blitzkopf/shadeorb
 License: MIT
 Keywords: shadeorb,lights,bleak,bluetooth,homeassistant
 Author: Yngvi Thor Sigurjonsson
 Author-email: blitzkopf@gmail.com
 Requires-Python: >=3.10,<3.13
@@ -14,13 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Home Automation
 Requires-Dist: bitstruct (>=8.19.0,<9.0.0)
 Requires-Dist: bleak (>=0.21.1,<0.22.0)
 Requires-Dist: bleak-retry-connector (>=3.4.0,<4.0.0)
+Requires-Dist: ruff (>=0.3.5,<0.4.0)
 Project-URL: Repository, https://github.com/blitzkopf/shadeorb
 Description-Content-Type: text/markdown
 
 # shadeorb
 Python package to control Shade ORB lights
```

