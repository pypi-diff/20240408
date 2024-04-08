# Comparing `tmp/telegram_collector-0.1.1.tar.gz` & `tmp/telegram_collector-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.1.1.tar", last modified: Mon Apr  8 10:33:37 2024, max compression
+gzip compressed data, was "telegram_collector-0.1.2.tar", last modified: Mon Apr  8 16:23:49 2024, max compression
```

## Comparing `telegram_collector-0.1.1.tar` & `telegram_collector-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 10:33:37.201979 telegram_collector-0.1.1/
--rw-rw-rw-   0        0        0      287 2024-04-08 10:33:37.201979 telegram_collector-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-08 10:33:37.201979 telegram_collector-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-04-08 10:33:34.000000 telegram_collector-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:33:37.191056 telegram_collector-0.1.1/telegram_collector/
--rw-rw-rw-   0        0        0     4947 2024-04-07 15:40:00.000000 telegram_collector-0.1.1/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0     1893 2024-04-07 15:48:31.000000 telegram_collector-0.1.1/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2560 2024-04-02 12:28:41.000000 telegram_collector-0.1.1/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:33:37.200980 telegram_collector-0.1.1/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 16:23:49.708705 telegram_collector-0.1.2/
+-rw-rw-rw-   0        0        0      287 2024-04-08 16:23:49.706714 telegram_collector-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-08 16:23:49.708705 telegram_collector-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-04-08 16:23:31.000000 telegram_collector-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:23:49.698628 telegram_collector-0.1.2/telegram_collector/
+-rw-rw-rw-   0        0        0     5250 2024-04-08 16:23:20.000000 telegram_collector-0.1.2/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0     2110 2024-04-08 16:23:20.000000 telegram_collector-0.1.2/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2546 2024-04-08 16:22:31.000000 telegram_collector-0.1.2/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:23:49.706714 telegram_collector-0.1.2/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-08 16:23:49.000000 telegram_collector-0.1.2/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-04-08 16:23:49.000000 telegram_collector-0.1.2/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:23:49.000000 telegram_collector-0.1.2/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-08 16:23:49.000000 telegram_collector-0.1.2/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-08 16:23:49.000000 telegram_collector-0.1.2/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-08 16:23:49.000000 telegram_collector-0.1.2/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.1.1/setup.py` & `telegram_collector-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='telegram_collector',
-    version='0.1.1',
+    version='0.1.2',
     author='fengleicn',
     author_email='fengleisemail@gmail.com',
     url='https://github.com/fengleicn/telegram_collector',
     description=u'收集电报群组的视频图片消息',
     packages=['telegram_collector'],
     install_requires=['telethon', 'python_socks'],
     entry_points={
```

### Comparing `telegram_collector-0.1.1/telegram_collector/__init__.py` & `telegram_collector-0.1.2/telegram_collector/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,28 @@
         self.proxy_port = None
         self.session_name = None
         self.src_dialog_ids = None
         self.dest_dialog_ids = None
         self.iter_val = None
         self.use_proxy = None
         self.proxy = None
+        self.inited = False
 
     async def __do_async_init(self):
-        self.client = TelegramClient(self.session_name, self.api_id, self.api_hash, proxy=self.proxy)
-        await self.client.start()
-        self.my_dialogs = await self.__get_my_dialogs()
-        self.src_dialogs = await self.__get_src_dialogs()
-        self.dest_dialogs = await self.__get_dest_dialogs()
+        if not self.inited:
+            self.client = TelegramClient(self.session_name, self.api_id, self.api_hash, proxy=self.proxy)
+            await self.client.start()
+            self.my_dialogs = await self.__get_my_dialogs()
+            self.src_dialogs = await self.__get_src_dialogs()
+            self.dest_dialogs = await self.__get_dest_dialogs()
+            self.inited = True
 
     async def __get_my_dialogs(self):
         dialogs = await self.client.get_dialogs()
-        await print_dialogs(dialogs)
+        # await print_dialogs(dialogs)
         return dialogs
 
     async def __get_src_dialogs(self):
         src_dialog = []
         for dialog in self.my_dialogs:
             if dialog.id in self.src_dialog_ids:
                 src_dialog.append(dialog)
@@ -133,7 +136,14 @@
     def send_history_message_src_to_dest(self):
 
         async def cluster():
             await self.__do_async_init()
             await self.__send_history_message_src_to_dest()
 
         asyncio.run(cluster())
+
+    def print_my_dialogs(self):
+        async def cluster():
+            await self.__do_async_init()
+            await print_dialogs(self.my_dialogs)
+
+        asyncio.run(cluster())
```

### Comparing `telegram_collector-0.1.1/telegram_collector/__main__.py` & `telegram_collector-0.1.2/telegram_collector/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,44 +26,46 @@
     tc.src_dialog_ids = get_config(parser, 'src_dialog_ids', [])
     tc.dest_dialog_ids = get_config(parser, 'dest_dialog_ids', [])
     tc.iter_val = get_config(parser, 'iter_val', 1000)
     return tc
 
 
 def create_example_config_file():
+    s = ('[default]\n'
+         'api_id=1\n'
+         'api_hash=1\n'
+         'src_dialog_ids=-1\n'
+         'dest_dialog_ids=1\n'
+         'use_proxy=false\n')
     with open('tg.ini', mode='w') as f:
-        f.write(
-'''
-[default]
-api_id=1
-api_hash=1
-src_dialog_ids=-1
-dest_dialog_ids=1
-use_proxy=false
-'''
-        )
+        f.write(s)
 
 
-def _getopt():
-    return getopt.getopt(sys.argv[1:], "chn")
+def _get_opt():
+    opts, args = getopt.getopt(sys.argv[1:], "abc")
+    for opt, _ in opts:
+        return opt
+    # exit
+    print("-a: collect new messages\n"
+          "-b: collect history messages\n"
+          "-c: create an example config\n"
+          "-p: print dialogs information\n")
+    exit(1)
 
 
 def main():
-    opts, args = _getopt()
-    for opt, arg in opts:
-        if opt == '-c':  # config
-            create_example_config_file()
-            return
-        if opt == '-n':  # new
-            collector = new_telegram_collector()
-            collector.send_new_message_src_to_dest()
-            return
-        if opt == '-h':  # history
-            collector = new_telegram_collector()
-            collector.send_history_message_src_to_dest()
-            return
-
-    print("-c: create example config -h: collect history messages -n: collect new messages")
+    opt = _get_opt()
+    if opt == '-c':  # config
+        create_example_config_file()
+    elif opt == '-a':  # new message
+        collector = new_telegram_collector()
+        collector.send_new_message_src_to_dest()
+    elif opt == '-b':  # history message
+        collector = new_telegram_collector()
+        collector.send_history_message_src_to_dest()
+    elif opt == '-p':
+        collector = new_telegram_collector()
+        collector.print_my_dialogs()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `telegram_collector-0.1.1/telegram_collector/util.py` & `telegram_collector-0.1.2/telegram_collector/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,16 @@
 def sort_messages(messages):
     copy_list = messages.copy()
     copy_list.sort(key=lambda m: get_message_size(m), reverse=True)
     return copy_list
 
 
 async def print_dialogs(dialogs):
-    pass
-    # for dialog in dialogs:
-    #     print(dialog.id, dialog.title)
+    for dialog in dialogs:
+        print(dialog.id, dialog.title)
 
 
 def get_video_or_photo_message(messages):
     ret = []
     for message in messages:
         if message_is_video_or_photo(message):
             ret.append(message)
```

