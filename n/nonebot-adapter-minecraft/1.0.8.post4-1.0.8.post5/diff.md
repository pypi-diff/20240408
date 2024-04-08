# Comparing `tmp/nonebot_adapter_minecraft-1.0.8.post4.tar.gz` & `tmp/nonebot_adapter_minecraft-1.0.8.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_minecraft-1.0.8.post4.tar", max compression
+gzip compressed data, was "nonebot_adapter_minecraft-1.0.8.post5.tar", max compression
```

## Comparing `nonebot_adapter_minecraft-1.0.8.post4.tar` & `nonebot_adapter_minecraft-1.0.8.post5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1065 2024-04-05 07:10:05.237191 nonebot_adapter_minecraft-1.0.8.post4/LICENSE
--rw-r--r--   0        0        0     1693 2024-04-05 07:10:05.237191 nonebot_adapter_minecraft-1.0.8.post4/README.md
--rw-r--r--   0        0        0      375 2024-04-05 07:10:05.237191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/__init__.py
--rw-r--r--   0        0        0     8535 2024-04-05 07:10:05.237191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/adapter.py
--rw-r--r--   0        0        0     2317 2024-04-05 07:10:05.237191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/bot.py
--rw-r--r--   0        0        0     1104 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/bot.pyi
--rw-r--r--   0        0        0     3794 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/collator.py
--rw-r--r--   0        0        0      527 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/compat.py
--rw-r--r--   0        0        0      285 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/config.py
--rw-r--r--   0        0        0     1179 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/__init__.py
--rw-r--r--   0        0        0     3533 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/base.py
--rw-r--r--   0        0        0     1703 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/fabric.py
--rw-r--r--   0        0        0      949 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/forge.py
--rw-r--r--   0        0        0      648 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/minecraft.py
--rw-r--r--   0        0        0     1775 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/spigot.py
--rw-r--r--   0        0        0     1250 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/exception.py
--rw-r--r--   0        0        0     4844 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/message.py
--rw-r--r--   0        0        0     5449 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/model.py
--rw-r--r--   0        0        0     1008 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/utils.py
--rw-r--r--   0        0        0      642 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 nonebot_adapter_minecraft-1.0.8.post4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/LICENSE
+-rw-r--r--   0        0        0     1693 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/README.md
+-rw-r--r--   0        0        0      361 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/__init__.py
+-rw-r--r--   0        0        0     8733 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/adapter.py
+-rw-r--r--   0        0        0     2317 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/bot.py
+-rw-r--r--   0        0        0     1165 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/bot.pyi
+-rw-r--r--   0        0        0     3794 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/collator.py
+-rw-r--r--   0        0        0      527 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/compat.py
+-rw-r--r--   0        0        0      310 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/config.py
+-rw-r--r--   0        0        0     1392 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/__init__.py
+-rw-r--r--   0        0        0     3561 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/base.py
+-rw-r--r--   0        0        0     1680 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/fabric.py
+-rw-r--r--   0        0        0      951 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/forge.py
+-rw-r--r--   0        0        0      604 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/minecraft.py
+-rw-r--r--   0        0        0     1775 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/spigot.py
+-rw-r--r--   0        0        0     2138 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/exception.py
+-rw-r--r--   0        0        0     4844 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/message.py
+-rw-r--r--   0        0        0     5468 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/model.py
+-rw-r--r--   0        0        0     1008 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/utils.py
+-rw-r--r--   0        0        0     1549 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/pyproject.toml
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 nonebot_adapter_minecraft-1.0.8.post5/PKG-INFO
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/LICENSE` & `nonebot_adapter_minecraft-1.0.8.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/README.md` & `nonebot_adapter_minecraft-1.0.8.post5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/adapter.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import json
 import asyncio
 import inspect
 import contextlib
 from typing import Any, Dict, Optional, Generator, Type, List
 
-from aiomcrcon import Client as RCONClient, RCONConnectionError, IncorrectPasswordError # type: ignore
+from aiomcrcon import (
+    Client as RCONClient,
+    RCONConnectionError as BaseRCONConnectionError,
+    IncorrectPasswordError as BaseIncorrectPasswordError,
+    ClientNotConnectedError as BaseClientNotConnectedError
+)
 from nonebot import get_plugin_config
 from nonebot.adapters import Adapter as BaseAdapter
 from nonebot.compat import type_validate_python
 from nonebot.drivers import (
     URL,
     Driver,
     WebSocket,
@@ -29,14 +34,15 @@
 
 from . import event
 from .bot import Bot
 from .event import Event
 from .config import Config
 from .collator import Collator
 from .utils import log, get_msg, get_actionbar_msg
+from .exception import IncorrectPasswordError, ClientNotConnectedError, RCONConnectionError
 
 DEFAULT_MODELS: List[Type[Event]] = []
 for model_name in dir(event):
     model = getattr(event, model_name)
     if not inspect.isclass(model) or not issubclass(model, Event):
         continue
     DEFAULT_MODELS.append(model)
@@ -64,15 +70,15 @@
     @overrides(BaseAdapter)
     def get_name(cls) -> str:
         return "Minecraft"
 
     def _setup(self) -> None:
         if isinstance(self.driver, ReverseDriver):
             ws_setup = WebSocketServerSetup(
-                URL("/minecraft/ws"), self.get_name(), self._handle_ws
+                URL("/minecraft/ws"), f"{self.get_name()} WS", self._handle_ws
             )
             self.setup_websocket_server(ws_setup)
 
     @overrides(BaseAdapter)
     async def _call_api(self, bot: Bot, api: str, **data: Any) -> Any:
         websocket = self.connections.get(bot.self_id, None)
         log("DEBUG", f"Calling API <y>{api}</y>")
@@ -92,14 +98,20 @@
                 )
                 websocket_send_body.data = SendTitleBody(send_title=send_title_item)
             elif api == "send_actionbar":
                 websocket_send_body.api = "actionbar"
                 websocket_send_body.data = SendActionBarBody(
                     message_list=get_actionbar_msg(**data)
                 )
+            elif api == "send_rcon_cmd":
+                try:
+                    await bot.rcon.send_cmd(data.get("command"))
+                except BaseClientNotConnectedError:
+                    raise ClientNotConnectedError()
+                return
 
             await websocket.send(websocket_send_body.model_dump_json())
         return
 
     async def _handle_ws(self, websocket: WebSocket) -> None:
         ori_self_id = websocket.request.headers.get("x-self-name")
 
@@ -116,38 +128,46 @@
             await websocket.close(1008, "Duplicate X-Self-Name")
             return
 
         await websocket.accept()
 
         rcon = None
         if server := self.minecraft_config.minecraft_server_rcon.get(self_id):
+            rcon = RCONClient(
+                websocket.__dict__["websocket"].__dict__["scope"]["client"][0],
+                server.rcon_port,
+                server.rcon_password,
+            )
             if server.enable_rcon:
-                rcon = RCONClient(
-                    websocket.__dict__["websocket"].__dict__["scope"]["client"][0],
-                    server.rcon_port,
-                    server.rcon_password,
-                )
                 log(
                     "INFO",
-                    f"Connecting to RCON server for <y>Bot {escape_tag(self_id)}</y>",
+                    f"<y>Connecting</y> RCON for <y>Bot {escape_tag(self_id)}</y>",
                 )
-                if await self._connect_rcon(self_id=self_id, rcon=rcon):
+                try:
+                    await rcon.connect(timeout=server.timeout)
+                except BaseIncorrectPasswordError:
+                    raise IncorrectPasswordError()
+                except BaseClientNotConnectedError:
+                    raise ClientNotConnectedError()
+                except BaseRCONConnectionError as e:
+                    raise RCONConnectionError(e.message, e.error)
+                else:
                     log(
                         "INFO",
-                        f"RCON server for <y>Bot {escape_tag(self_id)}</y> connected",
+                        f"RCON for <y>Bot {escape_tag(self_id)}</y> <g>connected</g>",
                     )
             else:
                 log(
                     "INFO",
-                    f"RCON server for <y>Bot {escape_tag(self_id)}</y> is not enabled",
+                    f"RCON for <y>Bot {escape_tag(self_id)}</y> is not enabled, will not connect",
                 )
         else:
             log(
                 "INFO",
-                f"RCON server for <y>Bot {escape_tag(self_id)}</y> not found, Rcon is disabled",
+                f"RCON configuration for <y>Bot {escape_tag(self_id)}</y> not found, will not connect",
             )
 
         bot = Bot(self, self_id, rcon)
         self.connections[self_id] = websocket
         self.bot_connect(bot)
 
         log("INFO", f"<y>Bot {escape_tag(self_id)}</y> connected")
@@ -166,25 +186,21 @@
                 "<r><bg #f8bbd0>Error while process data from websocket "
                 f"for bot {escape_tag(self_id)}.</bg #f8bbd0></r>",
                 e,
             )
         finally:
             with contextlib.suppress(Exception):
                 await websocket.close()
-                await self._close_rcon(self_id=self_id, rcon=rcon)
+                if rcon:
+                    await rcon.close()
+                    log("INFO", f"RCON for <y>Bot {escape_tag(self_id)}</y> closed")
             self.connections.pop(self_id, None)
             self.bot_disconnect(bot)
 
     @classmethod
-    async def _close_rcon(cls, self_id: str, rcon: Optional[RCONClient] = None):
-        if rcon:
-            await rcon.close()
-            log("INFO", f"RCON server for <y>Bot {escape_tag(self_id)}</y> closed")
-
-    @classmethod
     def add_custom_model(cls, *model: Type[Event]) -> None:
         """插入或覆盖一个自定义的 Event 类型。
 
         参数:
             model: 自定义的 Event 类型
         """
         cls.event_models.add_model(*model)
@@ -228,18 +244,7 @@
         except Exception as e:
             log(
                 "ERROR",
                 "<r><bg #f8bbd0>Failed to parse event. "
                 f"Raw: {escape_tag(str(json_data))}</bg #f8bbd0></r>",
                 e,
             )
-
-    @classmethod
-    async def _connect_rcon(cls, self_id: str, rcon: RCONClient):
-        try:
-            await rcon.connect()
-            return True
-        except RCONConnectionError:
-            log("ERROR", f"<y>Bot {escape_tag(self_id)}</y> failed to connect to RCON: <r>Connection Error</r>")
-        except IncorrectPasswordError:
-            log("ERROR", f"<y>Bot {escape_tag(self_id)}</y> failed to connect to RCON: <r>Incorrect Password</r>")
-        return False
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/bot.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/bot.pyi` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/bot.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -34,7 +34,9 @@
             title: str,
             subtitle: Optional[str] = None,
             fadein: Optional[int] = 10,
             stay: Optional[int] = 70,
             fadeout: Optional[int] = 20,
             **kwargs,
     ) -> Any: ...
+
+    async def send_rcon_cmd(self, command: str) -> Any: ...
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/collator.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/collator.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/compat.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/__init__.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     Event,
     BasePlayer,
     MessageEvent,
     NoticeEvent,
     BaseChatEvent,
     BaseDeathEvent,
     BaseJoinEvent,
-    BaseQuitEvent
+    BaseQuitEvent,
 )
 from .spigot import (
     Player as SpigotPlayer,
     AsyncPlayerChatEvent as SpigotAsyncPlayerChatEvent,
     PlayerDeathEvent as SpigotPlayerDeathEvent,
     PlayerJoinEvent as SpigotPlayerJoinEvent,
     PlayerQuitEvent as SpigotPlayerQuitEvent,
@@ -22,19 +22,19 @@
     PlayerLoggedInEvent as ForgePlayerLoggedInEvent,
     PlayerLoggedOutEvent as ForgePlayerLoggedOutEvent,
     PlayerDeathEvent as ForgePlayerDeathEvent,
     PlayerCommandEvent as ForgePlayerCommandEvent,
 )
 from .minecraft import (
     Player as MinecraftPlayer,
-    MinecraftPlayerChatEvent,
-    MinecraftPlayerJoinEvent,
-    MinecraftPlayerQuitEvent
+    PlayerChatEvent as MinecraftPlayerChatEvent,
+    PlayerJoinEvent as MinecraftPlayerJoinEvent,
+    PlayerQuitEvent as MinecraftPlayerQuitEvent,
 )
 from .fabric import (
     Player as FabricPlayer,
-    FabricServerMessageEvent,
-    FabricServerCommandMessageEvent,
-    FabricServerLivingEntityAfterDeathEvent,
-    FabricServerPlayConnectionJoinEvent,
-    FabricServerPlayConnectionDisconnectEvent
+    ServerMessageEvent as FabricServerMessageEvent,
+    ServerMessageEvent as FabricServerCommandMessageEvent,
+    ServerLivingEntityAfterDeathEvent as FabricServerLivingEntityAfterDeathEvent,
+    ServerPlayConnectionJoinEvent as FabricServerPlayConnectionJoinEvent,
+    ServerPlayConnectionDisconnectEvent as FabricServerPlayConnectionDisconnectEvent,
 )
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/base.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,25 +92,25 @@
 class BaseChatEvent(MessageEvent):
     """聊天事件"""
 
     sub_type: Literal["chat"]
 
     @overrides(Event)
     def get_event_description(self) -> str:
-        return f"Message from @{self.player.nickname} on [{self.server_name}]: {self.message}"
+        return f"Message from @{self.player.nickname} on [{self.server_name}]: {self.message}"  # noqa: E501
 
 
 class BasePlayerCommandEvent(MessageEvent):
     """玩家命令事件"""
 
     sub_type: Literal["player_command"]
 
     @overrides(Event)
     def get_event_description(self) -> str:
-        return f"Command from @{self.player.nickname} on [{self.server_name}]: {self.message}"
+        return f"Command from @{self.player.nickname} on [{self.server_name}]: {self.message}"  # noqa: E501
 
 
 class BaseDeathEvent(MessageEvent):
     """死亡事件"""
 
     sub_type: Literal["death"]
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/fabric.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/fabric.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 from .base import (
     BasePlayer,
     BaseChatEvent,
     BaseDeathEvent,
     BaseJoinEvent,
     BaseQuitEvent,
-    BasePlayerCommandEvent
+    BasePlayerCommandEvent,
 )
 
 
 class Player(BasePlayer):
     """Fabric Player"""
+
     uuid: Optional[str] = None
     ip: Optional[str] = None
     display_name: Optional[str] = None
     movement_speed: Optional[float] = None
 
     block_x: Optional[int] = None
     block_y: Optional[int] = None
@@ -25,35 +26,40 @@
     is_spectator: Optional[bool] = None
     is_sneaking: Optional[bool] = None
     is_sleeping: Optional[bool] = None
     is_climbing: Optional[bool] = None
     is_swimming: Optional[bool] = None
 
 
-class FabricServerMessageEvent(BaseChatEvent):
+class ServerMessageEvent(BaseChatEvent):
     """Fabric FabricServerMessageEvent API"""
+
     event_name: Literal["FabricServerMessageEvent"]
     player: Player
 
 
-class FabricServerCommandMessageEvent(BasePlayerCommandEvent):
+class ServerCommandMessageEvent(BasePlayerCommandEvent):
     """Fabric FabricServerCommandMessageEvent API"""
+
     event_name: Literal["FabricServerCommandMessageEvent"]
     player: Player
 
 
-class FabricServerLivingEntityAfterDeathEvent(BaseDeathEvent):
+class ServerLivingEntityAfterDeathEvent(BaseDeathEvent):
     """Fabric FabricServerLivingEntityAfterDeathEvent API"""
+
     event_name: Literal["FabricServerLivingEntityAfterDeathEvent"]
     player: Player
 
 
-class FabricServerPlayConnectionJoinEvent(BaseJoinEvent):
+class ServerPlayConnectionJoinEvent(BaseJoinEvent):
     """Fabric FabricServerPlayConnectionJoinEvent API"""
+
     event_name: Literal["FabricServerPlayConnectionJoinEvent"]
     player: Player
 
 
-class FabricServerPlayConnectionDisconnectEvent(BaseQuitEvent):
+class ServerPlayConnectionDisconnectEvent(BaseQuitEvent):
     """Fabric FabricServerPlayConnectionDisconnectEvent API"""
+
     event_name: Literal["FabricServerPlayConnectionDisconnectEvent"]
     player: Player
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/forge.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/forge.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 from .base import (
     BasePlayer,
     BaseChatEvent,
     BaseJoinEvent,
     BaseQuitEvent,
     BaseDeathEvent,
-    BasePlayerCommandEvent
+    BasePlayerCommandEvent,
 )
 
 
 class Player(BasePlayer):
     """Forge Player"""
+
     uuid: Optional[str] = None
     ipAddress: Optional[str] = None
     level: Optional[str] = None
     """地图？"""
     speed: Optional[float] = None
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/minecraft.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/minecraft.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from typing import Literal
 
-from .base import (
-    BasePlayer,
-    BaseChatEvent,
-    BaseJoinEvent,
-    BaseQuitEvent
-)
+from .base import BasePlayer, BaseChatEvent, BaseJoinEvent, BaseQuitEvent
 
 
 class Player(BasePlayer):
     """原版 玩家信息"""
 
 
-class MinecraftPlayerChatEvent(BaseChatEvent):
+class PlayerChatEvent(BaseChatEvent):
     """原版 玩家聊天事件"""
+
     event_name: Literal["MinecraftPlayerChatEvent"]
     player: Player
 
 
-class MinecraftPlayerJoinEvent(BaseJoinEvent):
+class PlayerJoinEvent(BaseJoinEvent):
     """原版 玩家加入事件"""
+
     event_name: Literal["MinecraftPlayerJoinEvent"]
     player: Player
 
 
-class MinecraftPlayerQuitEvent(BaseQuitEvent):
+class PlayerQuitEvent(BaseQuitEvent):
     """原版 玩家退出事件"""
+
     event_name: Literal["MinecraftPlayerQuitEvent"]
     player: Player
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/spigot.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/spigot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/exception.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/exception.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 from typing import Optional
+
+from aiomcrcon.errors import (
+    RCONConnectionError as BaseRCONConnectionError,
+    IncorrectPasswordError as BaseIncorrectPasswordError,
+    ClientNotConnectedError as BaseClientNotConnectedError
+)
 from nonebot.drivers import Response
 from nonebot.exception import AdapterException
 from nonebot.exception import ActionFailed as BaseActionFailed
 from nonebot.exception import NetworkError as BaseNetworkError
 from nonebot.exception import ApiNotAvailable as BaseApiNotAvailable
 
 
@@ -31,14 +37,33 @@
     def __init__(self, response: Response):
         self.status_code: int = response.status_code
         self.code: Optional[int] = None
         self.message: Optional[str] = None
         self.data: Optional[dict] = None
 
 
+class RCONConnectionError(NetworkError, BaseRCONConnectionError):
+    def __init__(self, msg: Optional[str] = None, error: Optional[Exception] = None):
+        self.msg = msg
+        self.message = msg
+        self.error = error
+
+
+class IncorrectPasswordError(NetworkError, BaseIncorrectPasswordError):
+    def __init__(self):
+        super().__init__()
+        self.msg = "The password provided to the client was incorrect according to the server."
+
+
+class ClientNotConnectedError(NetworkError, BaseClientNotConnectedError):
+    def __init__(self):
+        super().__init__()
+        self.msg = "The client isn't connected. (Looks like you forgot to call the connect() coroutine!)"
+
+
 class UnauthorizedException(ActionFailed):
     pass
 
 
 class RateLimitException(ActionFailed):
     pass
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/message.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/model.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import List, Optional, Any
+from typing import List, Optional, Any, Union
 
 from pydantic import BaseModel
 
 """
 WebSocket
 """
 
@@ -96,15 +96,15 @@
 
 
 class HoverItem(BaseModel):
     """
     悬停事件中的物品
     """
 
-    id: Optional[str] = None
+    id: Optional[Union[str, int]] = None
     count: Optional[int] = None
     tag: Optional[str] = None
 
 
 class HoverEntity(BaseModel):
     """
     悬停事件中的实体
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/utils.py` & `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post4/PKG-INFO` & `nonebot_adapter_minecraft-1.0.8.post5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-minecraft
-Version: 1.0.8.post4
+Version: 1.0.8.post5
 Summary: NoneBot2与MineCraft Server互通的适配器。
 License: MIT
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aio-mc-rcon (>=3.2.2,<4.0.0)
 Requires-Dist: nonebot2[fastapi] (>=2.2.0,<3.0.0)
+Requires-Dist: pydantic (>=1.10.0,<3.0.0,!=2.5.0,!=2.5.1)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/17TheWord/nonebot-adapter-minecraft/main/assets/logo.png" width="200" height="200" alt="nonebot-adapter-minecraft">
 </p>
 
 <div align="center">
```

