# Comparing `tmp/tg_flask_sse_common-2.0.8.tar.gz` & `tmp/tg_flask_sse_common-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_flask_sse_common-2.0.8.tar", last modified: Wed Apr  3 09:50:36 2024, max compression
+gzip compressed data, was "tg_flask_sse_common-2.0.9.tar", last modified: Mon Apr  8 08:02:17 2024, max compression
```

## Comparing `tg_flask_sse_common-2.0.8.tar` & `tg_flask_sse_common-2.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 09:50:36.598999 tg_flask_sse_common-2.0.8/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 09:50:36.598774 tg_flask_sse_common-2.0.8/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.8/README.md
--rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 09:50:36.599053 tg_flask_sse_common-2.0.8/setup.cfg
--rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 09:50:22.000000 tg_flask_sse_common-2.0.8/setup.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 09:50:36.597793 tg_flask_sse_common-2.0.8/tg_flask_sse_common/
--rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 09:50:18.000000 tg_flask_sse_common-2.0.8/tg_flask_sse_common/__init__.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_cache.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    20574 2024-04-03 05:16:34.000000 tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_clients.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_constant.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_core.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_message.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    15279 2024-04-03 09:49:59.000000 tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_redis_pub_sub.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 09:50:36.598490 tg_flask_sse_common-2.0.8/tg_flask_sse_common.egg-info/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 09:50:36.000000 tg_flask_sse_common-2.0.8/tg_flask_sse_common.egg-info/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 09:50:36.000000 tg_flask_sse_common-2.0.8/tg_flask_sse_common.egg-info/SOURCES.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 09:50:36.000000 tg_flask_sse_common-2.0.8/tg_flask_sse_common.egg-info/dependency_links.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 09:50:36.000000 tg_flask_sse_common-2.0.8/tg_flask_sse_common.egg-info/top_level.txt
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-08 08:02:17.315771 tg_flask_sse_common-2.0.9/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-08 08:02:17.315546 tg_flask_sse_common-2.0.9/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.9/README.md
+-rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-08 08:02:17.315816 tg_flask_sse_common-2.0.9/setup.cfg
+-rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-08 08:01:55.000000 tg_flask_sse_common-2.0.9/setup.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-08 08:02:17.314499 tg_flask_sse_common-2.0.9/tg_flask_sse_common/
+-rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-08 08:02:01.000000 tg_flask_sse_common-2.0.9/tg_flask_sse_common/__init__.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_cache.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    20787 2024-04-08 08:01:06.000000 tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_clients.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_constant.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_core.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_message.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    15279 2024-04-03 09:49:59.000000 tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_redis_pub_sub.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-08 08:02:17.315303 tg_flask_sse_common-2.0.9/tg_flask_sse_common.egg-info/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-08 08:02:17.000000 tg_flask_sse_common-2.0.9/tg_flask_sse_common.egg-info/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-08 08:02:17.000000 tg_flask_sse_common-2.0.9/tg_flask_sse_common.egg-info/SOURCES.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-08 08:02:17.000000 tg_flask_sse_common-2.0.9/tg_flask_sse_common.egg-info/dependency_links.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-08 08:02:17.000000 tg_flask_sse_common-2.0.9/tg_flask_sse_common.egg-info/top_level.txt
```

### Comparing `tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_cache.py` & `tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_cache.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_clients.py` & `tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,16 @@
 
         for index, sse_connect in enumerate(sse_connect_list):
             if sse_connect.get(self.Field.LATER_RELEASE):
                 release_connect_list.append(index)
 
         # 清理记录的待释放连接
         for index in release_connect_list:
+            if index >= len(sse_connect_list):
+                continue
             sse_connect_list.pop(index)
 
         # 清理记录的频道
         if len(sse_connect_list) == 0:
             self.sse_global_clients.pop(channel)
             release_channel_list.append(channel)
 
@@ -141,31 +143,33 @@
 
     def release_timeout_sse(self):
         """
         移除超时连接对象
         """
         release_channel_list = list()
 
-        for _, channel in enumerate(self.sse_global_clients.keys()):
+        for channel in list(self.sse_global_clients.keys()):
             release_connect_list = list()
 
             sse_connect_list = self.sse_global_clients.get(channel)
             if not sse_connect_list:
                 continue
 
-            for index, sse_connect in enumerate(sse_connect_list):
+            for index, sse_connect in enumerate(list(sse_connect_list)):
                 if not sse_connect:
                     continue
                 connect_time = sse_connect.get(self.Field.CONNECT_TIME, datetime.now())
                 if (datetime.now() - connect_time).seconds > self.max_connect_time:
                     release_connect_list.append(index)
 
             # 清理记录的超时连接
             if len(release_connect_list) > 0:
                 for index in release_connect_list:
+                    if index >= len(sse_connect_list):
+                        continue
                     sse_connect_list.pop(index)
                 print({
                     'title': 'sse-log',
                     'msg': '移除超时连接',
                     'ln_id': self.local_node_id,
                     'channel': channel,
                     'release_connect_list': release_connect_list,
@@ -192,32 +196,34 @@
 
     def release_message_accumulate_sse(self):
         """
         移除消息堆积过多的连接对象
         """
         release_channel_list = list()
 
-        for _, channel in enumerate(self.sse_global_clients.keys()):
+        for channel in list(self.sse_global_clients.keys()):
             release_connect_list = list()
 
             sse_connect_list = self.sse_global_clients.get(channel)
             if not sse_connect_list:
                 continue
 
-            for index, sse_connect in enumerate(sse_connect_list):
+            for index, sse_connect in enumerate(list(sse_connect_list)):
                 if not sse_connect:
                     continue
 
                 message_list = sse_connect.get(self.Field.MESSAGE_LIST, [])
                 if len(message_list) > 200:
                     release_connect_list.append(index)
 
             # 清理记录的消息堆积过多连接
             if len(release_connect_list) > 0:
                 for index in release_connect_list:
+                    if index >= len(sse_connect_list):
+                        continue
                     sse_connect_list.pop(index)
                 print({
                     'title': 'sse-log',
                     'msg': '移除消息堆积过多连接',
                     'ln_id': self.local_node_id,
                     'channel': channel,
                     'release_connect_list': release_connect_list,
@@ -252,15 +258,15 @@
         """
         change_state_count = 0
 
         sse_connect_list = self.sse_global_clients.get(channel)
         if not sse_connect_list:
             return
 
-        for index, sse_connect in enumerate(sse_connect_list):
+        for sse_connect in sse_connect_list:
             if not sse_connect:
                 continue
 
             if sse_connect.get(self.Field.CLIENT_ID) == client_id:
                 sse_connect.update({
                     self.Field.LATER_RELEASE: True,
                     self.Field.RELEASE_REASON: SseListenRsp.CLIENT_DISCONNECT
@@ -317,23 +323,23 @@
         #
         # 1. 每次心跳包时，将清理已经关闭的连接对象
         # 2. 每次心跳包时，将清理超时连接对象 (额外兜底)
         # 3. 每次心跳包时，将检测消息堆积过多的对象 (额外兜底)
         try:
             self.release_timeout_sse()
 
-            for channel in self.sse_global_clients.keys():
+            for channel in list(self.sse_global_clients.keys()):
                 self.release_sse(channel=channel)
 
             self.release_message_accumulate_sse()
         except:
             pass
 
         # 移除完失效连接后，往有效连接中添加心跳消息
-        for channel, sse_connect_list in self.sse_global_clients.items():
+        for channel in self.sse_global_clients.keys():
             self.add_message(
                 channel=channel,
                 message=SseMessage(
                     channel=channel,
                     data=SseSystemEventType.HEARTBEAT,
                     event=SseSystemEventType.HEARTBEAT,
                     _id=str(int(datetime.now().timestamp() * 1000000)),
```

### Comparing `tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_constant.py` & `tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_constant.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_core.py` & `tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_core.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_message.py` & `tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_message.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.8/tg_flask_sse_common/sse_redis_pub_sub.py` & `tg_flask_sse_common-2.0.9/tg_flask_sse_common/sse_redis_pub_sub.py`

 * *Files identical despite different names*

