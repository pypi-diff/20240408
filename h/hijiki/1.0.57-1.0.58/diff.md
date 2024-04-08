# Comparing `tmp/hijiki-1.0.57.tar.gz` & `tmp/hijiki-1.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hijiki-1.0.57.tar", last modified: Thu Apr  4 18:24:56 2024, max compression
+gzip compressed data, was "hijiki-1.0.58.tar", last modified: Mon Apr  8 20:47:56 2024, max compression
```

## Comparing `hijiki-1.0.57.tar` & `hijiki-1.0.58.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.162686 hijiki-1.0.57/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 18:23:27.000000 hijiki-1.0.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-04 18:24:56.162686 hijiki-1.0.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-04 18:23:27.000000 hijiki-1.0.57/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.158686 hijiki-1.0.57/hijiki/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.158686 hijiki-1.0.57/hijiki/broker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/broker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/broker/broker_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/broker/hijiki_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/broker/hijiki_rabbit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.158686 hijiki-1.0.57/hijiki/decorator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/decorator/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/hijiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.162686 hijiki-1.0.57/hijiki/publisher/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/publisher/Publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/publisher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.162686 hijiki-1.0.57/hijiki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-04 18:24:56.000000 hijiki-1.0.57/hijiki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-04 18:24:56.000000 hijiki-1.0.57/hijiki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:24:56.000000 hijiki-1.0.57/hijiki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 18:24:56.000000 hijiki-1.0.57/hijiki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 18:24:56.000000 hijiki-1.0.57/hijiki.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:24:56.162686 hijiki-1.0.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-04 18:24:02.000000 hijiki-1.0.57/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.162686 hijiki-1.0.57/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-04 18:23:27.000000 hijiki-1.0.57/tests/test_broker_data_server_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-04 18:23:27.000000 hijiki-1.0.57/tests/test_publisher_consumer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.566949 hijiki-1.0.58/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 20:46:29.000000 hijiki-1.0.58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-08 20:47:56.566949 hijiki-1.0.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-08 20:46:29.000000 hijiki-1.0.58/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.562950 hijiki-1.0.58/hijiki/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.562950 hijiki-1.0.58/hijiki/broker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/broker/broker_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/broker/hijiki_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/broker/hijiki_rabbit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.562950 hijiki-1.0.58/hijiki/decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/decorator/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/hijiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.562950 hijiki-1.0.58/hijiki/publisher/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/publisher/Publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/publisher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.566949 hijiki-1.0.58/hijiki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-08 20:47:56.000000 hijiki-1.0.58/hijiki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 20:47:56.000000 hijiki-1.0.58/hijiki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:47:56.000000 hijiki-1.0.58/hijiki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 20:47:56.000000 hijiki-1.0.58/hijiki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 20:47:56.000000 hijiki-1.0.58/hijiki.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:47:56.566949 hijiki-1.0.58/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-08 20:47:00.000000 hijiki-1.0.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.562950 hijiki-1.0.58/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-08 20:46:29.000000 hijiki-1.0.58/tests/test_broker_data_server_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-08 20:46:29.000000 hijiki-1.0.58/tests/test_broker_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-08 20:46:29.000000 hijiki-1.0.58/tests/test_publisher_consumer_test.py
```

### Comparing `hijiki-1.0.57/LICENSE` & `hijiki-1.0.58/LICENSE`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.57/PKG-INFO` & `hijiki-1.0.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hijiki
-Version: 1.0.57
+Version: 1.0.58
 Summary: Python Rabbit wrapper library to simplify to use Exchanges and Queues with decorators
 Author: Leandro Vilson Battisti
 Keywords: Celery,Kombu,RabbitMQ,decorator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: celery==5.3.4
 Requires-Dist: urllib3<2.0
```

### Comparing `hijiki-1.0.57/README.md` & `hijiki-1.0.58/README.md`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.57/hijiki/broker/broker_data.py` & `hijiki-1.0.58/hijiki/broker/broker_data.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.57/hijiki/broker/hijiki_rabbit.py` & `hijiki-1.0.58/hijiki/broker/hijiki_rabbit.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     callbacks = {}
     _prefix = ""
 
     def __init__(self):
         self.connection = None
         self.broker = None
         self.host = None
-        self.cluster_hosts = []
+        self.cluster_hosts = None
         self.password = None
         self.username = None
         self.queue_exchanges = None
         self.worker = None
         self.port = None
 
     def terminate(self):
@@ -46,21 +46,24 @@
         return self
 
     def with_host(self, host: str):
         self.host = host
         return self
 
     def with_cluster_hosts(self, hosts: str):
-        self.cluster_hosts.append(hosts)
+        self.cluster_hosts = hosts
         return self
 
     def with_port(self, port: str):
         self.port = port
         return self
 
+    def ping(self):
+        return self.broker.ping()
+
     def build(self):
         self.broker = HijikiBroker('worker', self.host, self.username, self.password, self.port, self.cluster_hosts)
         self.connection = self.broker.get_celery_broker().broker_connection()
         self.init_queues()
         return self
 
     def init_queues(self, ):
@@ -94,15 +97,15 @@
 
             queue_dlq.bind(self.connection).declare()
 
             self.queues[name].append(queue)
             self.queues[name + "_dlq"].append(queue_dlq)
 
     def _wrap_function(self, function, callback, queue_name, task=False):
-        
+
         self.callbacks[queue_name].append(callback)
 
         # The function returned by the decorator don't really do
         # anything.  The process_msg callback added to the consumer
         # is what actually responds to messages  from the client
         # on this particular queue.
 
@@ -139,15 +142,15 @@
                 message.ack()
 
         return self._wrap_function(
             func, process_message, queue_name, task=True)
 
     def run(self):
         consumers_without_callbacks = [
-            key 
+            key
             for (key, callbacks) in self.callbacks.items()
             if not callbacks
         ]
 
         for key in consumers_without_callbacks:
             self.callbacks.pop(key)
             self.queues.pop(key)
```

### Comparing `hijiki-1.0.57/hijiki/decorator/worker.py` & `hijiki-1.0.58/hijiki/decorator/worker.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.57/hijiki/publisher/Publisher.py` & `hijiki-1.0.58/hijiki/publisher/Publisher.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.57/hijiki.egg-info/PKG-INFO` & `hijiki-1.0.58/hijiki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hijiki
-Version: 1.0.57
+Version: 1.0.58
 Summary: Python Rabbit wrapper library to simplify to use Exchanges and Queues with decorators
 Author: Leandro Vilson Battisti
 Keywords: Celery,Kombu,RabbitMQ,decorator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: celery==5.3.4
 Requires-Dist: urllib3<2.0
```

### Comparing `hijiki-1.0.57/hijiki.egg-info/SOURCES.txt` & `hijiki-1.0.58/hijiki.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 hijiki/broker/hijiki_broker.py
 hijiki/broker/hijiki_rabbit.py
 hijiki/decorator/__init__.py
 hijiki/decorator/worker.py
 hijiki/publisher/Publisher.py
 hijiki/publisher/__init__.py
 tests/test_broker_data_server_exists.py
+tests/test_broker_ping.py
 tests/test_publisher_consumer_test.py
```

### Comparing `hijiki-1.0.57/tests/test_broker_data_server_exists.py` & `hijiki-1.0.58/tests/test_broker_data_server_exists.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.57/tests/test_publisher_consumer_test.py` & `hijiki-1.0.58/tests/test_publisher_consumer_test.py`

 * *Files identical despite different names*

