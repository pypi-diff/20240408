# Comparing `tmp/nonebot_plugin_auto_bot_selector-0.1.0.tar.gz` & `tmp/nonebot_plugin_auto_bot_selector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_auto_bot_selector-0.1.0.tar", last modified: Mon Apr  8 07:13:55 2024, max compression
+gzip compressed data, was "nonebot_plugin_auto_bot_selector-0.2.0.tar", last modified: Mon Apr  8 07:22:11 2024, max compression
```

## Comparing `nonebot_plugin_auto_bot_selector-0.1.0.tar` & `nonebot_plugin_auto_bot_selector-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1090 2024-04-08 06:12:11.915049 nonebot_plugin_auto_bot_selector-0.1.0/LICENSE
--rw-r--r--   0        0        0       36 2024-04-08 05:39:51.733384 nonebot_plugin_auto_bot_selector-0.1.0/README.md
--rw-r--r--   0        0        0     1178 2024-04-08 07:13:55.208164 nonebot_plugin_auto_bot_selector-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1420 2024-04-08 06:26:07.272462 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/__init__.py
--rw-r--r--   0        0        0      226 2024-04-08 06:18:56.201261 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/__init__.py
--rw-r--r--   0        0        0      890 2024-04-08 06:18:53.429775 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/dodo.py
--rw-r--r--   0        0        0     2011 2024-04-08 06:18:47.033926 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/kaiheila.py
--rw-r--r--   0        0        0     1897 2024-04-08 06:18:44.078855 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/onebot_v11.py
--rw-r--r--   0        0        0     4056 2024-04-08 06:26:07.272462 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/onebot_v12.py
--rw-r--r--   0        0        0      904 2024-04-08 06:09:44.798043 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/qq.py
--rw-r--r--   0        0        0     1174 2024-04-08 06:09:39.746925 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/red.py
--rw-r--r--   0        0        0     3745 2024-04-08 06:26:07.273467 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/satori.py
--rw-r--r--   0        0        0      409 2024-04-07 05:18:50.735312 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/expection.py
--rw-r--r--   0        0        0     1837 2024-04-08 06:26:07.273467 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/registries.py
--rw-r--r--   0        0        0     6178 2024-04-08 06:22:13.230088 nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/target.py
--rw-r--r--   0        0        0        0 2024-04-08 05:39:51.734383 nonebot_plugin_auto_bot_selector-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 nonebot_plugin_auto_bot_selector-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/LICENSE
+-rw-r--r--   0        0        0       35 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/README.md
+-rw-r--r--   0        0        0     1178 2024-04-08 07:22:11.034241 nonebot_plugin_auto_bot_selector-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1364 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/__init__.py
+-rw-r--r--   0        0        0      219 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/__init__.py
+-rw-r--r--   0        0        0      860 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/dodo.py
+-rw-r--r--   0        0        0     1949 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/kaiheila.py
+-rw-r--r--   0        0        0     1837 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3943 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/onebot_v12.py
+-rw-r--r--   0        0        0      872 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/qq.py
+-rw-r--r--   0        0        0     1133 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/red.py
+-rw-r--r--   0        0        0     3632 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/satori.py
+-rw-r--r--   0        0        0      396 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/expection.py
+-rw-r--r--   0        0        0     1775 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/registries.py
+-rw-r--r--   0        0        0     5927 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/target.py
+-rw-r--r--   0        0        0     3049 2024-04-08 07:22:07.806260 nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/utils/alconna.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:22:07.810260 nonebot_plugin_auto_bot_selector-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 nonebot_plugin_auto_bot_selector-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_auto_bot_selector-0.1.0/LICENSE` & `nonebot_plugin_auto_bot_selector-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 MountainDash
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 MountainDash
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nonebot_plugin_auto_bot_selector-0.1.0/pyproject.toml` & `nonebot_plugin_auto_bot_selector-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-auto-bot-selector"
-version = "0.1.0"
+version = "0.2.0"
 description = "Default template for PDM package"
 authors = [
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.1",
     "typing-extensions>=4.11.0",
```

### Comparing `nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/dodo.py` & `nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/dodo.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from contextlib import suppress
-from typing import List
-
-from nonebot.adapters import Bot as BaseBot
-
-from ..registries import register_list_targets
-from ..target import (
-    PlatformTarget,
-    TargetDoDoChannel,
-)
-
-with suppress(ImportError):
-    from nonebot.adapters.dodo import Adapter
-    from nonebot.adapters.dodo import Bot as BotDodo
-
-    adapter_name = Adapter.get_name()
-
-    @register_list_targets(adapter_name)
-    async def list_targets(bot: BaseBot) -> List[PlatformTarget]:
-        assert isinstance(bot, BotDodo)
-        targets = []
-        for island in await bot.get_island_list():
-            for channel in await bot.get_channel_list(
-                island_source_id=island.island_source_id
-            ):
-                targets.append(TargetDoDoChannel(channel_id=channel.channel_id))
-
-        # TODO: 私聊
-
-        return targets
+from contextlib import suppress
+from typing import List
+
+from nonebot.adapters import Bot as BaseBot
+
+from ..registries import register_list_targets
+from ..target import (
+    PlatformTarget,
+    TargetDoDoChannel,
+)
+
+with suppress(ImportError):
+    from nonebot.adapters.dodo import Adapter
+    from nonebot.adapters.dodo import Bot as BotDodo
+
+    adapter_name = Adapter.get_name()
+
+    @register_list_targets(adapter_name)
+    async def list_targets(bot: BaseBot) -> List[PlatformTarget]:
+        assert isinstance(bot, BotDodo)
+        targets = []
+        for island in await bot.get_island_list():
+            for channel in await bot.get_channel_list(
+                island_source_id=island.island_source_id
+            ):
+                targets.append(TargetDoDoChannel(channel_id=channel.channel_id))
+
+        # TODO: 私聊
+
+        return targets
```

### Comparing `nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/onebot_v11.py` & `nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/onebot_v11.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from contextlib import suppress
-from typing import List
-
-from nonebot.adapters import Bot
-
-from ..registries import PlatformTarget, add_cache, register_list_targets, remove_cache
-from ..target import TargetQQGroup, TargetQQPrivate, target_changed
-
-with suppress(ImportError):
-    from nonebot.adapters.onebot.v11 import (
-        Adapter,
-        FriendAddNoticeEvent,
-        GroupDecreaseNoticeEvent,
-        GroupIncreaseNoticeEvent,
-    )
-    from nonebot.adapters.onebot.v11 import Bot as BotOB11
-
-    adapter_name = Adapter.get_name()
-
-    @register_list_targets(adapter_name)
-    async def list_targets(bot: Bot) -> List[PlatformTarget]:
-        assert isinstance(bot, BotOB11)
-
-        targets = []
-        try:
-            groups = await bot.get_group_list()
-        except Exception:
-            groups = []
-
-        for group in groups:
-            group_id = group["group_id"]
-            target = TargetQQGroup(group_id=group_id)
-            targets.append(target)
-
-        # 获取好友列表
-        try:
-            users = await bot.get_friend_list()
-        except Exception:
-            users = []
-
-        for user in users:
-            user_id = user["user_id"]
-            target = TargetQQPrivate(user_id=user_id)
-            targets.append(target)
-
-        return targets
-
-    @target_changed.handle()
-    async def _(bot: Bot, event: GroupDecreaseNoticeEvent):
-        if event.is_tome():
-            await remove_cache(bot, TargetQQGroup(group_id=event.group_id))
-
-    @target_changed.handle()
-    async def _(bot: Bot, event: GroupIncreaseNoticeEvent):
-        if event.is_tome():
-            await add_cache(bot, TargetQQGroup(group_id=event.group_id))
-
-    @target_changed.handle()
-    async def _(bot: Bot, event: FriendAddNoticeEvent):
-        await add_cache(bot, TargetQQPrivate(user_id=event.user_id))
+from contextlib import suppress
+from typing import List
+
+from nonebot.adapters import Bot
+
+from ..registries import PlatformTarget, add_cache, register_list_targets, remove_cache
+from ..target import TargetQQGroup, TargetQQPrivate, target_changed
+
+with suppress(ImportError):
+    from nonebot.adapters.onebot.v11 import (
+        Adapter,
+        FriendAddNoticeEvent,
+        GroupDecreaseNoticeEvent,
+        GroupIncreaseNoticeEvent,
+    )
+    from nonebot.adapters.onebot.v11 import Bot as BotOB11
+
+    adapter_name = Adapter.get_name()
+
+    @register_list_targets(adapter_name)
+    async def list_targets(bot: Bot) -> List[PlatformTarget]:
+        assert isinstance(bot, BotOB11)
+
+        targets = []
+        try:
+            groups = await bot.get_group_list()
+        except Exception:
+            groups = []
+
+        for group in groups:
+            group_id = group["group_id"]
+            target = TargetQQGroup(group_id=group_id)
+            targets.append(target)
+
+        # 获取好友列表
+        try:
+            users = await bot.get_friend_list()
+        except Exception:
+            users = []
+
+        for user in users:
+            user_id = user["user_id"]
+            target = TargetQQPrivate(user_id=user_id)
+            targets.append(target)
+
+        return targets
+
+    @target_changed.handle()
+    async def _(bot: Bot, event: GroupDecreaseNoticeEvent):
+        if event.is_tome():
+            await remove_cache(bot, TargetQQGroup(group_id=event.group_id))
+
+    @target_changed.handle()
+    async def _(bot: Bot, event: GroupIncreaseNoticeEvent):
+        if event.is_tome():
+            await add_cache(bot, TargetQQGroup(group_id=event.group_id))
+
+    @target_changed.handle()
+    async def _(bot: Bot, event: FriendAddNoticeEvent):
+        await add_cache(bot, TargetQQPrivate(user_id=event.user_id))
```

### Comparing `nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/onebot_v12.py` & `nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/onebot_v12.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-from contextlib import suppress
-from typing import List
-
-from nonebot.adapters import Bot as BaseBot
-
-from ..registries import PlatformTarget, add_cache, register_list_targets, remove_cache
-from ..target import (
-    TargetOB12Unknow,
-    TargetQQGroup,
-    TargetQQGuildChannel,
-    TargetQQPrivate,
-    target_changed,
-)
-
-with suppress(ImportError):
-    from nonebot.adapters.onebot.v12 import (
-        Adapter,
-        Bot,
-        FriendDecreaseEvent,
-        FriendIncreaseEvent,
-        GroupMemberDecreaseEvent,
-        GroupMemberIncreaseEvent,
-    )
-    from nonebot.adapters.onebot.v12.exception import UnsupportedAction
-
-    adapter_name = Adapter.get_name()
-
-    @register_list_targets(adapter_name)
-    async def list_targets(bot: BaseBot) -> List[PlatformTarget]:
-        assert isinstance(bot, Bot)
-
-        targets = []
-        try:
-            friends = await bot.get_friend_list()
-            for friend in friends:
-                platform = bot.platform
-                if platform == "qq":
-                    targets.append(TargetQQPrivate(user_id=int(friend["user_id"])))
-                elif platform == "qqguild":
-                    # FIXME: 怎么获取 src_guild_id 捏？
-                    pass
-                else:
-                    targets.append(
-                        TargetOB12Unknow(
-                            platform=platform,
-                            detail_type="private",
-                            user_id=friend["user_id"],
-                        )
-                    )
-
-        except UnsupportedAction:  # pragma: no cover
-            pass
-
-        try:
-            groups = await bot.get_group_list()
-            for group in groups:
-                platform = bot.platform
-                if platform == "qq":
-                    targets.append(TargetQQGroup(group_id=int(group["group_id"])))
-                else:
-                    targets.append(
-                        TargetOB12Unknow(
-                            platform=platform,
-                            detail_type="group",
-                            group_id=group["group_id"],
-                        )
-                    )
-
-        except UnsupportedAction:  # pragma: no cover
-            pass
-
-        try:
-            guilds = await bot.get_guild_list()
-            for guild in guilds:
-                channels = await bot.get_channel_list(guild_id=guild["guild_id"])
-                for channel in channels:
-                    platform = bot.platform
-                    if platform == "qqguild":
-                        targets.append(
-                            TargetQQGuildChannel(channel_id=int(channel["channel_id"]))
-                        )
-                    else:
-                        targets.append(
-                            TargetOB12Unknow(
-                                platform=platform,
-                                detail_type="channel",
-                                channel_id=channel["channel_id"],
-                                guild_id=guild["guild_id"],
-                            )
-                        )
-
-        except UnsupportedAction:  # pragma: no cover
-            pass
-
-        return targets
-
-    @target_changed.handle()
-    async def _(bot: BaseBot, event: GroupMemberIncreaseEvent):
-        if event.user_id == bot.self_id:
-            await add_cache(bot, TargetQQGroup(group_id=int(event.group_id)))
-
-    @target_changed.handle()
-    async def _(bot: BaseBot, event: GroupMemberDecreaseEvent):
-        if event.user_id == bot.self_id:
-            await remove_cache(bot, TargetQQGroup(group_id=int(event.group_id)))
-
-    @target_changed.handle()
-    async def _(bot: BaseBot, event: FriendIncreaseEvent):
-        await add_cache(bot, TargetQQPrivate(user_id=int(event.user_id)))
-
-    @target_changed.handle()
-    async def _(bot: BaseBot, event: FriendDecreaseEvent):
-        await remove_cache(bot, TargetQQPrivate(user_id=int(event.user_id)))
+from contextlib import suppress
+from typing import List
+
+from nonebot.adapters import Bot as BaseBot
+
+from ..registries import PlatformTarget, add_cache, register_list_targets, remove_cache
+from ..target import (
+    TargetOB12Unknow,
+    TargetQQGroup,
+    TargetQQGuildChannel,
+    TargetQQPrivate,
+    target_changed,
+)
+
+with suppress(ImportError):
+    from nonebot.adapters.onebot.v12 import (
+        Adapter,
+        Bot,
+        FriendDecreaseEvent,
+        FriendIncreaseEvent,
+        GroupMemberDecreaseEvent,
+        GroupMemberIncreaseEvent,
+    )
+    from nonebot.adapters.onebot.v12.exception import UnsupportedAction
+
+    adapter_name = Adapter.get_name()
+
+    @register_list_targets(adapter_name)
+    async def list_targets(bot: BaseBot) -> List[PlatformTarget]:
+        assert isinstance(bot, Bot)
+
+        targets = []
+        try:
+            friends = await bot.get_friend_list()
+            for friend in friends:
+                platform = bot.platform
+                if platform == "qq":
+                    targets.append(TargetQQPrivate(user_id=int(friend["user_id"])))
+                elif platform == "qqguild":
+                    # FIXME: 怎么获取 src_guild_id 捏？
+                    pass
+                else:
+                    targets.append(
+                        TargetOB12Unknow(
+                            platform=platform,
+                            detail_type="private",
+                            user_id=friend["user_id"],
+                        )
+                    )
+
+        except UnsupportedAction:  # pragma: no cover
+            pass
+
+        try:
+            groups = await bot.get_group_list()
+            for group in groups:
+                platform = bot.platform
+                if platform == "qq":
+                    targets.append(TargetQQGroup(group_id=int(group["group_id"])))
+                else:
+                    targets.append(
+                        TargetOB12Unknow(
+                            platform=platform,
+                            detail_type="group",
+                            group_id=group["group_id"],
+                        )
+                    )
+
+        except UnsupportedAction:  # pragma: no cover
+            pass
+
+        try:
+            guilds = await bot.get_guild_list()
+            for guild in guilds:
+                channels = await bot.get_channel_list(guild_id=guild["guild_id"])
+                for channel in channels:
+                    platform = bot.platform
+                    if platform == "qqguild":
+                        targets.append(
+                            TargetQQGuildChannel(channel_id=int(channel["channel_id"]))
+                        )
+                    else:
+                        targets.append(
+                            TargetOB12Unknow(
+                                platform=platform,
+                                detail_type="channel",
+                                channel_id=channel["channel_id"],
+                                guild_id=guild["guild_id"],
+                            )
+                        )
+
+        except UnsupportedAction:  # pragma: no cover
+            pass
+
+        return targets
+
+    @target_changed.handle()
+    async def _(bot: BaseBot, event: GroupMemberIncreaseEvent):
+        if event.user_id == bot.self_id:
+            await add_cache(bot, TargetQQGroup(group_id=int(event.group_id)))
+
+    @target_changed.handle()
+    async def _(bot: BaseBot, event: GroupMemberDecreaseEvent):
+        if event.user_id == bot.self_id:
+            await remove_cache(bot, TargetQQGroup(group_id=int(event.group_id)))
+
+    @target_changed.handle()
+    async def _(bot: BaseBot, event: FriendIncreaseEvent):
+        await add_cache(bot, TargetQQPrivate(user_id=int(event.user_id)))
+
+    @target_changed.handle()
+    async def _(bot: BaseBot, event: FriendDecreaseEvent):
+        await remove_cache(bot, TargetQQPrivate(user_id=int(event.user_id)))
```

### Comparing `nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/qq.py` & `nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/qq.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from contextlib import suppress
-from typing import List
-
-from nonebot.adapters import Bot as BaseBot
-
-from ..registries import PlatformTarget, register_list_targets
-from ..target import TargetQQGuildChannel
-
-with suppress(ImportError):
-    from nonebot.adapters.qq import Adapter, Bot
-
-    adapter_name = Adapter.get_name()
-
-    @register_list_targets(adapter_name)
-    async def list_targets(bot: BaseBot) -> List[PlatformTarget]:
-        assert isinstance(bot, Bot)
-
-        targets = []
-
-        # TODO: 私聊
-
-        guilds = await bot.guilds()
-        for guild in guilds:
-            channels = await bot.get_channels(guild_id=guild.id)
-            for channel in channels:
-                targets.append(
-                    TargetQQGuildChannel(
-                        channel_id=int(channel.id),
-                    )
-                )
-
-        return targets
+from contextlib import suppress
+from typing import List
+
+from nonebot.adapters import Bot as BaseBot
+
+from ..registries import PlatformTarget, register_list_targets
+from ..target import TargetQQGuildChannel
+
+with suppress(ImportError):
+    from nonebot.adapters.qq import Adapter, Bot
+
+    adapter_name = Adapter.get_name()
+
+    @register_list_targets(adapter_name)
+    async def list_targets(bot: BaseBot) -> List[PlatformTarget]:
+        assert isinstance(bot, Bot)
+
+        targets = []
+
+        # TODO: 私聊
+
+        guilds = await bot.guilds()
+        for guild in guilds:
+            channels = await bot.get_channels(guild_id=guild.id)
+            for channel in channels:
+                targets.append(
+                    TargetQQGuildChannel(
+                        channel_id=int(channel.id),
+                    )
+                )
+
+        return targets
```

### Comparing `nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/red.py` & `nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/red.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from contextlib import suppress
-from typing import List
-
-from nonebot.adapters import Bot
-
-from ..registries import PlatformTarget, register_list_targets
-from ..target import TargetQQGroup, TargetQQPrivate
-
-with suppress(ImportError):
-    from nonebot.adapters.red import (
-        Adapter,
-    )
-    from nonebot.adapters.red import Bot as BotRed
-
-    adapter_name = Adapter.get_name()
-
-    @register_list_targets(adapter_name)
-    async def list_targets(bot: Bot) -> List[PlatformTarget]:
-        assert isinstance(bot, BotRed)
-
-        targets = []
-        try:
-            groups = await bot.get_groups()
-        except Exception:
-            groups = []
-        for group in groups:
-            group_id = int(group.groupCode)
-            target = TargetQQGroup(group_id=group_id)
-            targets.append(target)
-
-        # 获取好友列表
-        try:
-            users = await bot.get_friends()
-        except Exception:
-            users = []
-        for user in users:
-            user_id = int(user.uin)
-            target = TargetQQPrivate(user_id=user_id)
-            targets.append(target)
-
-        return targets
+from contextlib import suppress
+from typing import List
+
+from nonebot.adapters import Bot
+
+from ..registries import PlatformTarget, register_list_targets
+from ..target import TargetQQGroup, TargetQQPrivate
+
+with suppress(ImportError):
+    from nonebot.adapters.red import (
+        Adapter,
+    )
+    from nonebot.adapters.red import Bot as BotRed
+
+    adapter_name = Adapter.get_name()
+
+    @register_list_targets(adapter_name)
+    async def list_targets(bot: Bot) -> List[PlatformTarget]:
+        assert isinstance(bot, BotRed)
+
+        targets = []
+        try:
+            groups = await bot.get_groups()
+        except Exception:
+            groups = []
+        for group in groups:
+            group_id = int(group.groupCode)
+            target = TargetQQGroup(group_id=group_id)
+            targets.append(target)
+
+        # 获取好友列表
+        try:
+            users = await bot.get_friends()
+        except Exception:
+            users = []
+        for user in users:
+            user_id = int(user.uin)
+            target = TargetQQPrivate(user_id=user_id)
+            targets.append(target)
+
+        return targets
```

### Comparing `nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/adapters/satori.py` & `nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/adapters/satori.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-from contextlib import suppress
-from functools import partial
-from typing import (
-    Awaitable,
-    Generic,
-    List,
-    Optional,
-    Protocol,
-    TypeVar,
-)
-
-from nonebot import logger
-from nonebot.adapters import Bot
-from nonebot.compat import PYDANTIC_V2, ConfigDict
-from nonebot.exception import ActionFailed
-from pydantic import BaseModel
-
-from ..registries import register_list_targets
-from ..target import (
-    PlatformTarget,
-    TargetQQGroup,
-    TargetQQPrivate,
-    TargetSatoriUnknown,
-)
-
-with suppress(ImportError):
-    from nonebot.adapters.satori import Adapter
-    from nonebot.adapters.satori import Bot as BotSatori
-
-    adapter_name = Adapter.get_name()
-
-    T = TypeVar("T")
-
-    if PYDANTIC_V2:
-
-        class PageResult(BaseModel, Generic[T]):  # type: ignore
-            data: List[T]
-            next: Optional[str] = None
-
-            model_config: ConfigDict = ConfigDict(extra="allow")  # type: ignore
-
-    else:
-
-        from pydantic.generics import GenericModel
-
-        class PageResult(GenericModel, Generic[T]):
-            data: List[T]
-            next: Optional[str] = None
-
-            class Config:
-                extra = "allow"
-
-    class PagedAPI(Generic[T], Protocol):
-        def __call__(
-            self, *, next_token: Optional[str] = None
-        ) -> Awaitable[PageResult[T]]: ...
-
-    async def _fetch_all(paged_api: PagedAPI[T]) -> List[T]:
-        results = []
-        # nonebor-adapter-satori < 0.10.2 的 `channel_list` API 会因为 next_token 为 None 而报错
-        token = None
-        while True:
-            resp = await paged_api(next_token=token)
-            results.extend(resp.data)
-            if resp.next is None:
-                logger.debug("No more pages to fetch")
-                break
-            token = resp.next
-            logger.debug(f"Fetching next page with token: {token}")
-        return results
-
-    @register_list_targets(adapter_name)
-    async def list_targets(bot: Bot) -> List[PlatformTarget]:
-        assert isinstance(bot, BotSatori)
-
-        targets = []
-        # 获取群组列表
-        try:
-            guilds = await _fetch_all(bot.guild_list)
-            logger.debug(f"Found {len(guilds)} guilds(groups)")
-            for guild in guilds:
-                logger.debug(f"featching -> {guild}")
-                channels = await _fetch_all(
-                    partial(bot.channel_list, guild_id=guild.id)
-                )
-                for channel in channels:
-                    if bot.platform in ["qq", "red", "chronocat"]:
-                        target = TargetQQGroup(group_id=int(channel.id))
-                    else:
-                        target = TargetSatoriUnknown(
-                            platform=bot.platform, channel_id=channel.id
-                        )
-                    targets.append(target)
-        except ActionFailed as e:  # pragma: no cover
-            logger.warning(
-                f"Satori({bot.platform}) does not support fetching channel list: {e}"
-            )
-
-        # 获取好友列表
-        try:
-            users = await _fetch_all(bot.friend_list)
-            for user in users:
-                if bot.platform in ["qq", "red", "chronocat"]:
-                    target = TargetQQPrivate(user_id=int(user.id))
-                else:
-                    target = TargetSatoriUnknown(platform=bot.platform, user_id=user.id)
-                targets.append(target)
-        except ActionFailed as e:  # pragma: no cover
-            logger.warning(
-                f"Satori({bot.platform}) does not support fetching friend list: {e}"
-            )
-
-        return targets
+from contextlib import suppress
+from functools import partial
+from typing import (
+    Awaitable,
+    Generic,
+    List,
+    Optional,
+    Protocol,
+    TypeVar,
+)
+
+from nonebot import logger
+from nonebot.adapters import Bot
+from nonebot.compat import PYDANTIC_V2, ConfigDict
+from nonebot.exception import ActionFailed
+from pydantic import BaseModel
+
+from ..registries import register_list_targets
+from ..target import (
+    PlatformTarget,
+    TargetQQGroup,
+    TargetQQPrivate,
+    TargetSatoriUnknown,
+)
+
+with suppress(ImportError):
+    from nonebot.adapters.satori import Adapter
+    from nonebot.adapters.satori import Bot as BotSatori
+
+    adapter_name = Adapter.get_name()
+
+    T = TypeVar("T")
+
+    if PYDANTIC_V2:
+
+        class PageResult(BaseModel, Generic[T]):  # type: ignore
+            data: List[T]
+            next: Optional[str] = None
+
+            model_config: ConfigDict = ConfigDict(extra="allow")  # type: ignore
+
+    else:
+
+        from pydantic.generics import GenericModel
+
+        class PageResult(GenericModel, Generic[T]):
+            data: List[T]
+            next: Optional[str] = None
+
+            class Config:
+                extra = "allow"
+
+    class PagedAPI(Generic[T], Protocol):
+        def __call__(
+            self, *, next_token: Optional[str] = None
+        ) -> Awaitable[PageResult[T]]: ...
+
+    async def _fetch_all(paged_api: PagedAPI[T]) -> List[T]:
+        results = []
+        # nonebor-adapter-satori < 0.10.2 的 `channel_list` API 会因为 next_token 为 None 而报错
+        token = None
+        while True:
+            resp = await paged_api(next_token=token)
+            results.extend(resp.data)
+            if resp.next is None:
+                logger.debug("No more pages to fetch")
+                break
+            token = resp.next
+            logger.debug(f"Fetching next page with token: {token}")
+        return results
+
+    @register_list_targets(adapter_name)
+    async def list_targets(bot: Bot) -> List[PlatformTarget]:
+        assert isinstance(bot, BotSatori)
+
+        targets = []
+        # 获取群组列表
+        try:
+            guilds = await _fetch_all(bot.guild_list)
+            logger.debug(f"Found {len(guilds)} guilds(groups)")
+            for guild in guilds:
+                logger.debug(f"featching -> {guild}")
+                channels = await _fetch_all(
+                    partial(bot.channel_list, guild_id=guild.id)
+                )
+                for channel in channels:
+                    if bot.platform in ["qq", "red", "chronocat"]:
+                        target = TargetQQGroup(group_id=int(channel.id))
+                    else:
+                        target = TargetSatoriUnknown(
+                            platform=bot.platform, channel_id=channel.id
+                        )
+                    targets.append(target)
+        except ActionFailed as e:  # pragma: no cover
+            logger.warning(
+                f"Satori({bot.platform}) does not support fetching channel list: {e}"
+            )
+
+        # 获取好友列表
+        try:
+            users = await _fetch_all(bot.friend_list)
+            for user in users:
+                if bot.platform in ["qq", "red", "chronocat"]:
+                    target = TargetQQPrivate(user_id=int(user.id))
+                else:
+                    target = TargetSatoriUnknown(platform=bot.platform, user_id=user.id)
+                targets.append(target)
+        except ActionFailed as e:  # pragma: no cover
+            logger.warning(
+                f"Satori({bot.platform}) does not support fetching friend list: {e}"
+            )
+
+        return targets
```

### Comparing `nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/registries.py` & `nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/registries.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import asyncio
-import json
-from typing import Awaitable, Callable, Dict, List, Set
-
-from nonebot import logger
-from nonebot.adapters import Bot
-from nonebot.compat import model_dump
-
-from .target import PlatformTarget
-
-BOT_CACHE: Dict[Bot, Set[PlatformTarget]] = dict()
-BOT_CACHE_LOCK = asyncio.Lock()
-
-ListTargetsFunc = Callable[[Bot], Awaitable[List[PlatformTarget]]]
-
-list_targets_map: Dict[str, ListTargetsFunc] = {}
-
-
-def register_list_targets(adapter: str):
-    def wrapper(func: ListTargetsFunc):
-        list_targets_map[adapter] = func
-        return func
-
-    return wrapper
-
-
-async def add_cache(bot: Bot, target: PlatformTarget):
-    async with BOT_CACHE_LOCK:
-        BOT_CACHE[bot].add(target)
-    info_current()
-
-
-async def remove_cache(bot: Bot, target: PlatformTarget):
-    async with BOT_CACHE_LOCK:
-        BOT_CACHE[bot].remove(target)
-    info_current()
-
-
-async def refresh_bot(bot: Bot):
-    BOT_CACHE.pop(bot, None)
-    adapter_name = bot.adapter.get_name()
-    print(adapter_name)
-    print(list_targets_map)
-    if list_targets := list_targets_map.get(adapter_name):
-        try:
-            logger.debug(
-                f"executing list targets {list_targets} of adapter {adapter_name}"
-            )
-            targets = await list_targets(bot)
-            BOT_CACHE[bot] = set(targets)
-        except Exception:
-            logger.exception(f"{bot} get list targets failed")
-    else:
-        logger.warning(f"no available list targets function for adapter {adapter_name}")
-    info_current()
-
-
-def info_current():
-    log_info = {}
-    for bot, platform_target_set in BOT_CACHE.items():
-        log_info[str(bot)] = [model_dump(target) for target in platform_target_set]
-    logger.trace(f"current bot-platform_target: {json.dumps(log_info)}")
+import asyncio
+import json
+from typing import Awaitable, Callable, Dict, List, Set
+
+from nonebot import logger
+from nonebot.adapters import Bot
+from nonebot.compat import model_dump
+
+from .target import PlatformTarget
+
+BOT_CACHE: Dict[Bot, Set[PlatformTarget]] = dict()
+BOT_CACHE_LOCK = asyncio.Lock()
+
+ListTargetsFunc = Callable[[Bot], Awaitable[List[PlatformTarget]]]
+
+list_targets_map: Dict[str, ListTargetsFunc] = {}
+
+
+def register_list_targets(adapter: str):
+    def wrapper(func: ListTargetsFunc):
+        list_targets_map[adapter] = func
+        return func
+
+    return wrapper
+
+
+async def add_cache(bot: Bot, target: PlatformTarget):
+    async with BOT_CACHE_LOCK:
+        BOT_CACHE[bot].add(target)
+    info_current()
+
+
+async def remove_cache(bot: Bot, target: PlatformTarget):
+    async with BOT_CACHE_LOCK:
+        BOT_CACHE[bot].remove(target)
+    info_current()
+
+
+async def refresh_bot(bot: Bot):
+    BOT_CACHE.pop(bot, None)
+    adapter_name = bot.adapter.get_name()
+    print(adapter_name)
+    print(list_targets_map)
+    if list_targets := list_targets_map.get(adapter_name):
+        try:
+            logger.debug(
+                f"executing list targets {list_targets} of adapter {adapter_name}"
+            )
+            targets = await list_targets(bot)
+            BOT_CACHE[bot] = set(targets)
+        except Exception:
+            logger.exception(f"{bot} get list targets failed")
+    else:
+        logger.warning(f"no available list targets function for adapter {adapter_name}")
+    info_current()
+
+
+def info_current():
+    log_info = {}
+    for bot, platform_target_set in BOT_CACHE.items():
+        log_info[str(bot)] = [model_dump(target) for target in platform_target_set]
+    logger.trace(f"current bot-platform_target: {json.dumps(log_info)}")
```

### Comparing `nonebot_plugin_auto_bot_selector-0.1.0/src/nonebot_plugin_auto_bot_selector/target.py` & `nonebot_plugin_auto_bot_selector-0.2.0/src/nonebot_plugin_auto_bot_selector/target.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-import json
-from abc import ABC
-from enum import Enum
-from typing import (
-    Any,
-    ClassVar,
-    Dict,
-    Literal,
-    Optional,
-)
-
-from nonebot.compat import PYDANTIC_V2, ConfigDict, type_validate_python
-from nonebot.plugin import on_notice
-from pydantic import BaseModel
-from typing_extensions import Self
-
-target_changed = on_notice(block=False)
-
-
-class SupportedPlatform(str, Enum):
-    qq_group = "QQ Group"
-    qq_private = "QQ Private"
-    qq_group_openid = "QQ Group OpenID"
-    qq_private_openid = "QQ Private OpenID"
-    qq_guild_channel = "QQ Guild Channel"
-    qq_guild_direct = "QQ Guild Direct"
-    kaiheila_channel = "Kaiheila Channel"
-    kaiheila_private = "Kaiheila Private"
-    unknown_ob12 = "Unknow Onebot 12 Platform"
-    unknown_satori = "Unknown Satori Platform"
-    dodo_channel = "DoDo Channel"
-    dodo_private = "DoDo Private"
-
-
-class Level(Enum):
-    MetaBase = 1
-    Base = 2
-    Normal = 3
-
-
-class SerializationMeta(BaseModel, ABC):
-    _index_key: ClassVar[str]
-    _deserializer_dict: ClassVar[Dict]
-    _level: ClassVar[Level] = Level.MetaBase
-
-    if PYDANTIC_V2:
-        model_config = ConfigDict(
-            frozen=True,
-            from_attributes=True,
-        )  # type: ignore
-
-        @classmethod
-        def __pydantic_init_subclass__(cls, *args, **kwargs) -> None:
-            cls._register_subclass(cls.model_fields)
-
-    else:
-
-        class Config:
-            frozen = True
-            orm_mode = True
-
-        @classmethod
-        def __init_subclass__(cls, *args, **kwargs) -> None:
-            cls._register_subclass(cls.__fields__)
-
-            super().__init_subclass__(*args, **kwargs)
-
-    @classmethod
-    def _register_subclass(cls, fields) -> None:
-        if cls._level == Level.MetaBase:
-            cls._level = Level.Base
-            cls._deserializer_dict = {}
-        elif cls._level == Level.Base:
-            cls._level = Level.Normal
-            cls._deserializer_dict[fields[cls._index_key].default] = cls
-        elif cls._level == Level.Normal:
-            pass
-        else:
-            raise RuntimeError("SerializationMeta init error")
-
-    @classmethod
-    def deserialize(cls, source: Any) -> Self:
-        if isinstance(source, str):
-            raw_obj = json.loads(source)
-        else:
-            raw_obj = source
-
-        key = raw_obj.get(cls._index_key)
-        assert key
-        return type_validate_python(cls._deserializer_dict[key], raw_obj)
-
-
-class PlatformTarget(SerializationMeta):
-    _index_key = "platform_type"
-
-    platform_type: SupportedPlatform
-
-    if PYDANTIC_V2:
-        model_config = ConfigDict(
-            frozen=True,
-            from_attributes=True,
-        )  # type: ignore
-    else:
-
-        class Config:
-            frozen = True
-            orm_mode = True
-
-
-class TargetQQGroup(PlatformTarget):
-    """QQ群
-
-    参数
-        group_id: 群号
-    """
-
-    platform_type: Literal[SupportedPlatform.qq_group] = SupportedPlatform.qq_group
-    group_id: int
-
-
-class TargetQQPrivate(PlatformTarget):
-    """QQ私聊
-
-    参数
-        user_id: QQ号
-    """
-
-    platform_type: Literal[SupportedPlatform.qq_private] = SupportedPlatform.qq_private
-    user_id: int
-
-
-class TargetQQGuildChannel(PlatformTarget):
-    """QQ频道子频道
-
-    参数
-        channel_id: 子频道号
-    """
-
-    platform_type: Literal[SupportedPlatform.qq_guild_channel] = (
-        SupportedPlatform.qq_guild_channel
-    )
-    channel_id: int
-
-
-class TargetQQGuildDirect(PlatformTarget):
-    """QQ频道私聊
-
-    参数
-        recipient_id: 接收人ID
-        source_guild_id: 来自的频道号
-    """
-
-    platform_type: Literal[SupportedPlatform.qq_guild_direct] = (
-        SupportedPlatform.qq_guild_direct
-    )
-    recipient_id: int
-    source_guild_id: int
-
-
-class TargetOB12Unknow(PlatformTarget):
-    """暂未识别的 Onebot v12 发送目标
-
-    参数
-        detail_type: "private" or "group" or "channel"
-        user_id, group_id, channel_id, guild_id: 同 ob12 定义
-    """
-
-    platform_type: Literal[SupportedPlatform.unknown_ob12] = (
-        SupportedPlatform.unknown_ob12
-    )
-    platform: str
-    detail_type: Literal["private", "group", "channel"]
-    user_id: Optional[str] = None
-    group_id: Optional[str] = None
-    guild_id: Optional[str] = None
-    channel_id: Optional[str] = None
-
-
-class TargetSatoriUnknown(PlatformTarget):
-    """暂未识别的 Satori 发送目标
-
-    参数
-        platform: 平台名
-        user_id: 用户 ID
-        guild_id: 群组 ID
-        channel_id: 频道 ID
-    """
-
-    platform_type: Literal[SupportedPlatform.unknown_satori] = (
-        SupportedPlatform.unknown_satori
-    )
-    platform: str
-    user_id: Optional[str] = None
-    guild_id: Optional[str] = None
-    channel_id: Optional[str] = None
-
-
-class TargetKaiheilaChannel(PlatformTarget):
-    """开黑啦频道
-
-    参数
-        channel_id: 频道ID
-    """
-
-    platform_type: Literal[SupportedPlatform.kaiheila_channel] = (
-        SupportedPlatform.kaiheila_channel
-    )
-    channel_id: str
-
-
-class TargetKaiheilaPrivate(PlatformTarget):
-    """开黑啦私聊
-
-    参数
-        user_id: 接收人ID
-    """
-
-    platform_type: Literal[SupportedPlatform.kaiheila_private] = (
-        SupportedPlatform.kaiheila_private
-    )
-    user_id: str
-
-
-class TargetDoDoChannel(PlatformTarget):
-    """DoDo Channel
-
-    参数
-        channel_id: 频道ID
-        dodo_source_id: 用户 ID(可选)
-    """
-
-    platform_type: Literal[SupportedPlatform.dodo_channel] = (
-        SupportedPlatform.dodo_channel
-    )
-    channel_id: str
-    dodo_source_id: Optional[str] = None
-
-
-class TargetDoDoPrivate(PlatformTarget):
-    """DoDo Private
-
-    参数
-        dodo_source_id: 用户 ID
-        island_source_id: 群 ID
-    """
-
-    platform_type: Literal[SupportedPlatform.dodo_private] = (
-        SupportedPlatform.dodo_private
-    )
-    island_source_id: str
-    dodo_source_id: str
+import json
+from abc import ABC
+from enum import Enum
+from typing import (
+    Any,
+    ClassVar,
+    Dict,
+    Literal,
+    Optional,
+)
+
+from nonebot.compat import PYDANTIC_V2, ConfigDict, type_validate_python
+from nonebot.plugin import on_notice
+from pydantic import BaseModel
+from typing_extensions import Self
+
+target_changed = on_notice(block=False)
+
+
+class SupportedPlatform(str, Enum):
+    qq_group = "QQ Group"
+    qq_private = "QQ Private"
+    qq_group_openid = "QQ Group OpenID"
+    qq_private_openid = "QQ Private OpenID"
+    qq_guild_channel = "QQ Guild Channel"
+    qq_guild_direct = "QQ Guild Direct"
+    kaiheila_channel = "Kaiheila Channel"
+    kaiheila_private = "Kaiheila Private"
+    unknown_ob12 = "Unknow Onebot 12 Platform"
+    unknown_satori = "Unknown Satori Platform"
+    dodo_channel = "DoDo Channel"
+    dodo_private = "DoDo Private"
+
+
+class Level(Enum):
+    MetaBase = 1
+    Base = 2
+    Normal = 3
+
+
+class SerializationMeta(BaseModel, ABC):
+    _index_key: ClassVar[str]
+    _deserializer_dict: ClassVar[Dict]
+    _level: ClassVar[Level] = Level.MetaBase
+
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            frozen=True,
+            from_attributes=True,
+        )  # type: ignore
+
+        @classmethod
+        def __pydantic_init_subclass__(cls, *args, **kwargs) -> None:
+            cls._register_subclass(cls.model_fields)
+
+    else:
+
+        class Config:
+            frozen = True
+            orm_mode = True
+
+        @classmethod
+        def __init_subclass__(cls, *args, **kwargs) -> None:
+            cls._register_subclass(cls.__fields__)
+
+            super().__init_subclass__(*args, **kwargs)
+
+    @classmethod
+    def _register_subclass(cls, fields) -> None:
+        if cls._level == Level.MetaBase:
+            cls._level = Level.Base
+            cls._deserializer_dict = {}
+        elif cls._level == Level.Base:
+            cls._level = Level.Normal
+            cls._deserializer_dict[fields[cls._index_key].default] = cls
+        elif cls._level == Level.Normal:
+            pass
+        else:
+            raise RuntimeError("SerializationMeta init error")
+
+    @classmethod
+    def deserialize(cls, source: Any) -> Self:
+        if isinstance(source, str):
+            raw_obj = json.loads(source)
+        else:
+            raw_obj = source
+
+        key = raw_obj.get(cls._index_key)
+        assert key
+        return type_validate_python(cls._deserializer_dict[key], raw_obj)
+
+
+class PlatformTarget(SerializationMeta):
+    _index_key = "platform_type"
+
+    platform_type: SupportedPlatform
+
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            frozen=True,
+            from_attributes=True,
+        )  # type: ignore
+    else:
+
+        class Config:
+            frozen = True
+            orm_mode = True
+
+
+class TargetQQGroup(PlatformTarget):
+    """QQ群
+
+    参数
+        group_id: 群号
+    """
+
+    platform_type: Literal[SupportedPlatform.qq_group] = SupportedPlatform.qq_group
+    group_id: int
+
+
+class TargetQQPrivate(PlatformTarget):
+    """QQ私聊
+
+    参数
+        user_id: QQ号
+    """
+
+    platform_type: Literal[SupportedPlatform.qq_private] = SupportedPlatform.qq_private
+    user_id: int
+
+
+class TargetQQGuildChannel(PlatformTarget):
+    """QQ频道子频道
+
+    参数
+        channel_id: 子频道号
+    """
+
+    platform_type: Literal[SupportedPlatform.qq_guild_channel] = (
+        SupportedPlatform.qq_guild_channel
+    )
+    channel_id: int
+
+
+class TargetQQGuildDirect(PlatformTarget):
+    """QQ频道私聊
+
+    参数
+        recipient_id: 接收人ID
+        source_guild_id: 来自的频道号
+    """
+
+    platform_type: Literal[SupportedPlatform.qq_guild_direct] = (
+        SupportedPlatform.qq_guild_direct
+    )
+    recipient_id: int
+    source_guild_id: int
+
+
+class TargetOB12Unknow(PlatformTarget):
+    """暂未识别的 Onebot v12 发送目标
+
+    参数
+        detail_type: "private" or "group" or "channel"
+        user_id, group_id, channel_id, guild_id: 同 ob12 定义
+    """
+
+    platform_type: Literal[SupportedPlatform.unknown_ob12] = (
+        SupportedPlatform.unknown_ob12
+    )
+    platform: str
+    detail_type: Literal["private", "group", "channel"]
+    user_id: Optional[str] = None
+    group_id: Optional[str] = None
+    guild_id: Optional[str] = None
+    channel_id: Optional[str] = None
+
+
+class TargetSatoriUnknown(PlatformTarget):
+    """暂未识别的 Satori 发送目标
+
+    参数
+        platform: 平台名
+        user_id: 用户 ID
+        guild_id: 群组 ID
+        channel_id: 频道 ID
+    """
+
+    platform_type: Literal[SupportedPlatform.unknown_satori] = (
+        SupportedPlatform.unknown_satori
+    )
+    platform: str
+    user_id: Optional[str] = None
+    guild_id: Optional[str] = None
+    channel_id: Optional[str] = None
+
+
+class TargetKaiheilaChannel(PlatformTarget):
+    """开黑啦频道
+
+    参数
+        channel_id: 频道ID
+    """
+
+    platform_type: Literal[SupportedPlatform.kaiheila_channel] = (
+        SupportedPlatform.kaiheila_channel
+    )
+    channel_id: str
+
+
+class TargetKaiheilaPrivate(PlatformTarget):
+    """开黑啦私聊
+
+    参数
+        user_id: 接收人ID
+    """
+
+    platform_type: Literal[SupportedPlatform.kaiheila_private] = (
+        SupportedPlatform.kaiheila_private
+    )
+    user_id: str
+
+
+class TargetDoDoChannel(PlatformTarget):
+    """DoDo Channel
+
+    参数
+        channel_id: 频道ID
+        dodo_source_id: 用户 ID(可选)
+    """
+
+    platform_type: Literal[SupportedPlatform.dodo_channel] = (
+        SupportedPlatform.dodo_channel
+    )
+    channel_id: str
+    dodo_source_id: Optional[str] = None
+
+
+class TargetDoDoPrivate(PlatformTarget):
+    """DoDo Private
+
+    参数
+        dodo_source_id: 用户 ID
+        island_source_id: 群 ID
+    """
+
+    platform_type: Literal[SupportedPlatform.dodo_private] = (
+        SupportedPlatform.dodo_private
+    )
+    island_source_id: str
+    dodo_source_id: str
```

### Comparing `nonebot_plugin_auto_bot_selector-0.1.0/PKG-INFO` & `nonebot_plugin_auto_bot_selector-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-auto-bot-selector
-Version: 0.1.0
+Version: 0.2.0
 Summary: Default template for PDM package
 Author-Email: Well404 <well_404@outlook.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: typing-extensions>=4.11.0
 Requires-Dist: nonebot-adapter-onebot>=2.4.3; extra == "dev"
```

