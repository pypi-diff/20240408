# Comparing `tmp/telegram_collector-0.0.9.tar.gz` & `tmp/telegram_collector-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.0.9.tar", last modified: Tue Apr  2 09:18:39 2024, max compression
+gzip compressed data, was "telegram_collector-0.1.0.tar", last modified: Sun Apr  7 15:50:34 2024, max compression
```

## Comparing `telegram_collector-0.0.9.tar` & `telegram_collector-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 09:18:39.478093 telegram_collector-0.0.9/
--rw-rw-rw-   0        0        0      287 2024-04-02 09:18:39.477121 telegram_collector-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 09:18:39.478093 telegram_collector-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      735 2024-04-02 09:18:27.000000 telegram_collector-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 09:18:39.470585 telegram_collector-0.0.9/telegram_collector/
--rw-rw-rw-   0        0        0     5170 2024-04-02 09:18:27.000000 telegram_collector-0.0.9/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0      361 2024-04-02 08:47:19.000000 telegram_collector-0.0.9/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2542 2024-04-02 09:09:01.000000 telegram_collector-0.0.9/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-02 09:18:39.477121 telegram_collector-0.0.9/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-02 09:18:39.000000 telegram_collector-0.0.9/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-04-02 09:18:39.000000 telegram_collector-0.0.9/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 09:18:39.000000 telegram_collector-0.0.9/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      248 2024-04-02 09:18:39.000000 telegram_collector-0.0.9/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-02 09:18:39.000000 telegram_collector-0.0.9/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-02 09:18:39.000000 telegram_collector-0.0.9/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 15:50:34.992291 telegram_collector-0.1.0/
+-rw-rw-rw-   0        0        0      287 2024-04-07 15:50:34.991274 telegram_collector-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-07 15:50:34.992291 telegram_collector-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-04-07 15:48:31.000000 telegram_collector-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:50:34.979948 telegram_collector-0.1.0/telegram_collector/
+-rw-rw-rw-   0        0        0     4947 2024-04-07 15:40:00.000000 telegram_collector-0.1.0/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0     1893 2024-04-07 15:48:31.000000 telegram_collector-0.1.0/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2560 2024-04-02 12:28:41.000000 telegram_collector-0.1.0/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:50:34.990131 telegram_collector-0.1.0/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.0.9/telegram_collector/__init__.py` & `telegram_collector-0.1.0/telegram_collector/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import asyncio
-import configparser
 import math
-import python_socks
 from telethon import *
 from .util import *
 
 
 class TelegramCollector:
     def __init__(self):
         self.dest_dialogs = None
@@ -18,36 +16,19 @@
         self.proxy_ip = None
         self.proxy_port = None
         self.session_name = None
         self.src_dialog_ids = None
         self.dest_dialog_ids = None
         self.iter_val = None
         self.use_proxy = None
+        self.proxy = None
 
-        self.parser = configparser.ConfigParser()
-        self.parser.read('tg.ini')
-
-    async def __do_init(self):
-        # 参数
-        self.proxy_type = python_socks.ProxyType.SOCKS5
-        self.api_id = get_config(self.parser, 'api_id', 0)
-        self.api_hash = get_config(self.parser, 'api_hash', '0')
-        self.proxy_ip = get_config(self.parser, 'proxy_ip', '127.0.0.1')
-        self.proxy_port = get_config(self.parser, 'proxy_port', 7890)
-        self.session_name = get_config(self.parser, 'session_name', 'tg_session')
-        self.src_dialog_ids = get_config(self.parser, 'src_dialog_ids', [])
-        self.dest_dialog_ids = get_config(self.parser, 'dest_dialog_ids', [])
-        self.iter_val = get_config(self.parser, 'iter_val', 1000)
-        self.use_proxy = get_config(self.parser, 'use_proxy', True)
-
-        proxy = (self.proxy_type, self.proxy_ip, self.proxy_port) if self.use_proxy else None
-        self.client = TelegramClient(self.session_name, self.api_id, self.api_hash,
-                                     proxy=proxy)
+    async def __do_async_init(self):
+        self.client = TelegramClient(self.session_name, self.api_id, self.api_hash, proxy=self.proxy)
         await self.client.start()
-
         self.my_dialogs = await self.__get_my_dialogs()
         self.src_dialogs = await self.__get_src_dialogs()
         self.dest_dialogs = await self.__get_dest_dialogs()
 
     async def __get_my_dialogs(self):
         dialogs = await self.client.get_dialogs()
         await print_dialogs(dialogs)
@@ -75,17 +56,16 @@
         return all_messages
 
     async def __refresh_history_messages(self):
         messages = await self.__get_history_messages()
         messages = await filter_messages(messages)
         return messages
 
-    async def __send_messages(self, messages):
+    async def __send_messages(self, messages, delay=2.5):
         count = 0
-        delay = 2.5
         for message in messages:
             count += 1
             print(count, end='.')
             for dest_dialog in self.dest_dialogs:
                 try:
                     await self.client.send_message(entity=dest_dialog, message=message)
                 except Exception as e:
@@ -115,28 +95,45 @@
         message = event.message
         src_dialog_id = event.message.chat_id
         print('get: ', message)
         if message_is_video_or_photo(message) and src_dialog_id in self.src_dialog_ids:
             await self.__send_messages([message])
 
     # 流式汇总增量消息
-    async def __send_current_message_src_to_dest(self):
+    async def __send_new_message_src_to_dest(self):
         self.client.add_event_handler(self.callback, events.NewMessage(incoming=True))
-
         try:
             while True:
                 await asyncio.sleep(1)
         finally:
             await self.__terminate_client()
 
-    def send_current_message_src_to_dest(self):
-        asyncio.run(self.__send_current_message_src_to_dest())
+    async def __send_current_message_src_to_dest_outdated(self):
+        try:
+            while True:
+                await asyncio.sleep(2)
+                min_id = 0
+                for src_dialog in self.src_dialogs:
+                    messages = await self.client.get_messages(src_dialog, min_id=min_id)
+                    min_id = messages[0].id
+                    for message in messages:
+                        print(message)
+                        if message_is_video_or_photo(message):
+                            await self.__send_messages([message], delay=0.1)
+        finally:
+            await self.__terminate_client()
 
-    def send_history_message_src_to_dest(self):
-        asyncio.run(self.__send_history_message_src_to_dest())
+    def send_new_message_src_to_dest(self):
+
+        async def cluster():
+            await self.__do_async_init()
+            await self.__send_new_message_src_to_dest()
 
-    def do_init(self):
-        asyncio.run(self.__do_init())
+        asyncio.run(cluster())
+
+    def send_history_message_src_to_dest(self):
 
+        async def cluster():
+            await self.__do_async_init()
+            await self.__send_history_message_src_to_dest()
 
-def console():
-    print("hello world!")
+        asyncio.run(cluster())
```

### Comparing `telegram_collector-0.0.9/telegram_collector/util.py` & `telegram_collector-0.1.0/telegram_collector/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,21 +55,21 @@
 
 
 def get_config(parser, option, fallback, section='default'):
     if parser.has_section(section):
         if parser.has_option(section, option):
             if fallback is None:
                 return parser.get(section, option)
-            elif type(fallback) == bool:
+            elif isinstance(fallback, bool):
                 return parser.getboolean(section, option)
-            elif type(fallback) == str:
+            elif isinstance(fallback, str):
                 return parser.get(section, option)
-            elif type(fallback) == int:
+            elif isinstance(fallback, int):
                 return parser.getint(section, option)
-            elif type(fallback) == list:
+            elif isinstance(fallback, list):
                 return list(map(lambda x: int(x), parser.get(section, option).split(',')))
     return fallback
 
 
 async def split_message(part, _iter_val, messages):
     end = part * _iter_val
     start = end - _iter_val
@@ -80,8 +80,8 @@
 async def filter_messages(messages):
     start = len(messages)
     messages = get_video_or_photo_message(messages)
     messages = unique_messages(messages)
     messages = sort_messages(messages)
     end = len(messages)
     print('\nbefore filter: ', start, 'after filter: ', end)
-    return messages
+    return messages
```

