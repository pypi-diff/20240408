# Comparing `tmp/kafka-broker-0.3.9.tar.gz` & `tmp/kafka-broker-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-broker-0.3.9.tar", last modified: Fri Apr  5 12:30:48 2024, max compression
+gzip compressed data, was "kafka-broker-0.4.0.tar", last modified: Mon Apr  8 12:54:17 2024, max compression
```

## Comparing `kafka-broker-0.3.9.tar` & `kafka-broker-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 12:30:48.244239 kafka-broker-0.3.9/
--rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.9/LICENSE
--rw-rw-rw-   0        0        0     4264 2024-04-05 12:30:48.243239 kafka-broker-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.9/README.md
--rw-rw-rw-   0        0        0      851 2024-04-05 12:08:37.000000 kafka-broker-0.3.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 12:30:48.245238 kafka-broker-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:30:48.194647 kafka-broker-0.3.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:30:48.217852 kafka-broker-0.3.9/src/kafka_broker/
--rw-rw-rw-   0        0        0      385 2024-04-05 11:50:25.000000 kafka-broker-0.3.9/src/kafka_broker/__init__.py
--rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.9/src/kafka_broker/base_config.ini
--rw-rw-rw-   0        0        0     6032 2024-04-05 11:51:35.000000 kafka-broker-0.3.9/src/kafka_broker/broker_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:30:48.234239 kafka-broker-0.3.9/src/kafka_broker/classes/
--rw-rw-rw-   0        0        0        0 2024-04-05 11:48:50.000000 kafka-broker-0.3.9/src/kafka_broker/classes/__init__.py
--rw-rw-rw-   0        0        0     2003 2024-04-05 11:38:52.000000 kafka-broker-0.3.9/src/kafka_broker/classes/cache.py
--rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.9/src/kafka_broker/classes/consumer_storage.py
--rw-rw-rw-   0        0        0     2888 2024-04-05 08:36:09.000000 kafka-broker-0.3.9/src/kafka_broker/classes/event_object.py
--rw-rw-rw-   0        0        0     1804 2024-04-05 11:48:32.000000 kafka-broker-0.3.9/src/kafka_broker/classes/event_router.py
--rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.9/src/kafka_broker/config.py
--rw-rw-rw-   0        0        0     3234 2024-04-05 12:30:26.000000 kafka-broker-0.3.9/src/kafka_broker/consumer.py
--rw-rw-rw-   0        0        0      184 2024-04-05 08:27:51.000000 kafka-broker-0.3.9/src/kafka_broker/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:30:48.237237 kafka-broker-0.3.9/src/kafka_broker/exceptions/
--rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.9/src/kafka_broker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.9/src/kafka_broker/exceptions/base.py
--rw-rw-rw-   0        0        0      605 2024-04-05 08:22:05.000000 kafka-broker-0.3.9/src/kafka_broker/exceptions/cache.py
--rw-rw-rw-   0        0        0     1368 2024-04-05 12:30:30.000000 kafka-broker-0.3.9/src/kafka_broker/producer.py
--rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.9/src/kafka_broker/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-05 12:30:48.239670 kafka-broker-0.3.9/src/kafka_broker.egg-info/
--rw-rw-rw-   0        0        0     4264 2024-04-05 12:30:48.000000 kafka-broker-0.3.9/src/kafka_broker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      812 2024-04-05 12:30:48.000000 kafka-broker-0.3.9/src/kafka_broker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 12:30:48.000000 kafka-broker-0.3.9/src/kafka_broker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-05 12:30:48.000000 kafka-broker-0.3.9/src/kafka_broker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 12:30:48.000000 kafka-broker-0.3.9/src/kafka_broker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 12:30:48.238237 kafka-broker-0.3.9/tests/
--rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.9/tests/test_event_object.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.590570 kafka-broker-0.4.0/
+-rw-rw-rw-   0        0        0     1090 2023-11-07 12:59:41.000000 kafka-broker-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     4264 2024-04-08 12:54:17.585570 kafka-broker-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-11-17 10:11:05.000000 kafka-broker-0.4.0/README.md
+-rw-rw-rw-   0        0        0      851 2024-04-08 12:53:55.000000 kafka-broker-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 12:54:17.591568 kafka-broker-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.474334 kafka-broker-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.518929 kafka-broker-0.4.0/src/kafka_broker/
+-rw-rw-rw-   0        0        0      385 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-11-20 13:43:40.000000 kafka-broker-0.4.0/src/kafka_broker/base_config.ini
+-rw-rw-rw-   0        0        0     6006 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/broker_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.558371 kafka-broker-0.4.0/src/kafka_broker/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/classes/__init__.py
+-rw-rw-rw-   0        0        0     2003 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/classes/cache.py
+-rw-rw-rw-   0        0        0     2190 2023-11-17 10:11:05.000000 kafka-broker-0.4.0/src/kafka_broker/classes/consumer_storage.py
+-rw-rw-rw-   0        0        0     2888 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/classes/event_object.py
+-rw-rw-rw-   0        0        0     3206 2024-04-08 12:47:05.000000 kafka-broker-0.4.0/src/kafka_broker/classes/event_router.py
+-rw-rw-rw-   0        0        0     1167 2023-11-17 10:11:05.000000 kafka-broker-0.4.0/src/kafka_broker/config.py
+-rw-rw-rw-   0        0        0     3234 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/consumer.py
+-rw-rw-rw-   0        0        0      184 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.566903 kafka-broker-0.4.0/src/kafka_broker/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-11-20 10:24:31.000000 kafka-broker-0.4.0/src/kafka_broker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      462 2024-04-08 12:44:45.000000 kafka-broker-0.4.0/src/kafka_broker/exceptions/base.py
+-rw-rw-rw-   0        0        0      605 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/exceptions/cache.py
+-rw-rw-rw-   0        0        0     1368 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/producer.py
+-rw-rw-rw-   0        0        0        0 2024-04-08 10:30:04.000000 kafka-broker-0.4.0/src/kafka_broker/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.573456 kafka-broker-0.4.0/src/kafka_broker/schemas/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:56:29.000000 kafka-broker-0.4.0/src/kafka_broker/schemas/__init__.py
+-rw-rw-rw-   0        0        0      345 2024-04-08 12:41:26.000000 kafka-broker-0.4.0/src/kafka_broker/schemas/log.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.580003 kafka-broker-0.4.0/src/kafka_broker.egg-info/
+-rw-rw-rw-   0        0        0     4264 2024-04-08 12:54:17.000000 kafka-broker-0.4.0/src/kafka_broker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2024-04-08 12:54:17.000000 kafka-broker-0.4.0/src/kafka_broker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 12:54:17.000000 kafka-broker-0.4.0/src/kafka_broker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-08 12:54:17.000000 kafka-broker-0.4.0/src/kafka_broker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-08 12:54:17.000000 kafka-broker-0.4.0/src/kafka_broker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 12:54:17.576469 kafka-broker-0.4.0/tests/
+-rw-rw-rw-   0        0        0      356 2023-11-17 10:11:05.000000 kafka-broker-0.4.0/tests/test_event_object.py
```

### Comparing `kafka-broker-0.3.9/LICENSE` & `kafka-broker-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.9/PKG-INFO` & `kafka-broker-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.9
+Version: 0.4.0
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.9/README.md` & `kafka-broker-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.9/pyproject.toml` & `kafka-broker-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kafka-broker"
-version = "0.3.9"
+version = "0.4.0"
 authors = [
   { name="Tijmen Simons", email="tijmen.simons@student.hu.nl" },
   { name="Ivar Stek", email="ivar.stek@student.hu.nl" },
 ]
 description = "A python package implementation for the confluent kafka package. Managing producing and consuming."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `kafka-broker-0.3.9/src/kafka_broker/broker_manager.py` & `kafka-broker-0.4.0/src/kafka_broker/broker_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,17 @@
         if not self.consumer:
             kafka_config = self.config["kafka.default"]
             kafka_config.update(self.config["kafka.consumer"])
             self.consumer = Consumer(kafka_config)
             self.consumer.subscribe([self.config["general"]["current_location"]])
         return consume(self.consumer, self.logger)
 
-    @deprecated("It says depricated, but it might still work. It will not be updated anymore.")
+    @deprecated(
+        "It says depricated, but it might still work. It will not be updated anymore."
+    )
     def init_consumer_app(self, app):
         """Setup the consumer on a FastAPI instance.
 
         Parameters
         ----------
         app : FastAPI
             The FastAPI app.
@@ -152,37 +154,32 @@
     def reply(
         self,
         event_object: EventObject,
         status_code: int,
         msg: str,
         data: Any = None,
     ):
-        data = self._format_data(data)
-
-        event_object.data = {
-            "status_code": status_code,
-            "message": msg,
-            "payload": data,
-        }
+        event_object.data = BrokerManager._format_data(data)
+        event_object.as_reply(message=msg, status_code=status_code)
 
         event_object.status = EventStatus.COMPLETED
         event_object.event = "respond"
 
         self.cache.update(event_object)
 
     def send(
         self,
         event_object: EventObject,
         module: str,
         event: str,
         data: Any = None,
         **kwargs,
     ):
-        data = self._format_data(data)
+        data = BrokerManager._format_data(data)
 
         event_object.event = event
         event_object.data = {"payload": data, **kwargs}
 
         self.produce(module, event_object)
 
 
-broker_manager = BrokerManager()
+broker_manager = BrokerManager()
```

### Comparing `kafka-broker-0.3.9/src/kafka_broker/classes/cache.py` & `kafka-broker-0.4.0/src/kafka_broker/classes/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.9/src/kafka_broker/classes/consumer_storage.py` & `kafka-broker-0.4.0/src/kafka_broker/classes/consumer_storage.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.9/src/kafka_broker/classes/event_object.py` & `kafka-broker-0.4.0/src/kafka_broker/classes/event_object.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.9/src/kafka_broker/config.py` & `kafka-broker-0.4.0/src/kafka_broker/config.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.9/src/kafka_broker/consumer.py` & `kafka-broker-0.4.0/src/kafka_broker/consumer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.9/src/kafka_broker/exceptions/cache.py` & `kafka-broker-0.4.0/src/kafka_broker/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.9/src/kafka_broker/producer.py` & `kafka-broker-0.4.0/src/kafka_broker/producer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.9/src/kafka_broker.egg-info/PKG-INFO` & `kafka-broker-0.4.0/src/kafka_broker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.9
+Version: 0.4.0
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.9/src/kafka_broker.egg-info/SOURCES.txt` & `kafka-broker-0.4.0/src/kafka_broker.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 src/kafka_broker/classes/cache.py
 src/kafka_broker/classes/consumer_storage.py
 src/kafka_broker/classes/event_object.py
 src/kafka_broker/classes/event_router.py
 src/kafka_broker/exceptions/__init__.py
 src/kafka_broker/exceptions/base.py
 src/kafka_broker/exceptions/cache.py
+src/kafka_broker/schemas/__init__.py
+src/kafka_broker/schemas/log.py
 tests/test_event_object.py
```

