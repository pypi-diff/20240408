# Comparing `tmp/dalpha-0.4.3.tar.gz` & `tmp/dalpha-0.4.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.4.3.tar", max compression
+gzip compressed data, was "dalpha-0.4.4rc0.tar", max compression
```

## Comparing `dalpha-0.4.3.tar` & `dalpha-0.4.4rc0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.3/README.md
--rw-r--r--   0        0        0    23785 2024-03-25 02:37:47.094337 dalpha-0.4.3/dalpha/__init__.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.3/dalpha/context.py
--rw-r--r--   0        0        0     1716 2024-02-28 08:10:55.063883 dalpha-0.4.3/dalpha/dalpha_openai.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.3/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.3/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.3/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.3/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.3/dalpha/logging/utils.py
--rw-r--r--   0        0        0     5846 2024-03-06 10:11:38.540030 dalpha-0.4.3/dalpha/redis.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.3/dalpha/signal_handler.py
--rw-r--r--   0        0        0      875 2024-03-25 02:37:47.094337 dalpha-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1318 1970-01-01 00:00:00.000000 dalpha-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.4rc0/README.md
+-rw-r--r--   0        0        0    27798 2024-04-08 01:16:34.229539 dalpha-0.4.4rc0/dalpha/__init__.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/context.py
+-rw-r--r--   0        0        0     1716 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/dalpha_openai.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.4rc0/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.4rc0/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     5846 2024-03-06 10:11:38.540030 dalpha-0.4.4rc0/dalpha/redis.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      881 2024-04-08 01:16:34.229539 dalpha-0.4.4rc0/pyproject.toml
+-rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.4rc0/PKG-INFO
```

### Comparing `dalpha-0.4.3/README.md` & `dalpha-0.4.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.3/dalpha/__init__.py` & `dalpha-0.4.4rc0/dalpha/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -131,14 +131,15 @@
         headers = {
         'token': self.token
         }
         print(self.base_url, self.sentry_env, dev_server)
         response = requests.request("GET", os.path.join(self.base_url,f"inferences/{api_id}"), headers = headers)
         if response.status_code != 200:
             logger.warning(f'error from get sqs url / response status_code {response.status_code}: {response.text}')
+            self.service_code = None
         else:
             if self.queue_url is None:
                 self.queue_url = response.json().get('sqs', None)
             self.service_code = response.json().get('serviceCode', None)
 
         if self.queue_url is None:
             logger.warning("sqs url is not set")
@@ -149,18 +150,21 @@
         self.s3 = boto3.client('s3')
         self.sqs = boto3.client('sqs', region_name='ap-northeast-2')
         self.evaluates = {}
         self.use_sqs = use_sqs
         self.poll_time = None
 
         self.use_kafka = False
+        self.kafka_topic = None
+        self.update_record = None
         if kafka_topic is not None and isinstance(kafka_topic, str):
             from dalpha.kafka_cli import get_consumer
             self.kafka_consumer = get_consumer(kafka_topic, api_id)
             self.use_kafka = True
+            self.kafka_topic = kafka_topic
 
         set_context(Context(
             inference_id = api_id,
             service_code = self.service_code,
             env = "exp" if dev_server else "prod"
         ))
 
@@ -254,14 +258,16 @@
 
     def poll(self, max_number_of_messages = 1, mock=True):
         if get_shutdown_requested():
             logger.info(
                 "System shutdown gracefully",
                 event = Event.SHUTDOWN
             )
+            if self.use_kafka:
+                self.kafka_consumer.close()
             sys.exit(0)
         if not isinstance(max_number_of_messages,int): TypeError("max_number_of_messages is not a int")
         if not isinstance(mock, bool): TypeError("mock is not a bool")
         if mock:
             logger.info(
                 "return mock",
                 data = self.mock
@@ -294,15 +300,15 @@
 
             # TODO: filter_valid kafka에도 구현 (receiptHandle은 필요 없으나, 경우에 따라 불필요한 메세지 제거)
 
             if len(ret) == 0:
                 return None
             elif len(ret) == 1:
                 logger.info(
-                    message = "return kafka item",
+                    message = f"return kafka item: {ret[0]}",
                     event = Event.POLL,
                     data = ret[0]
                 )
                 set_context_evaluate(
                     evaluate_id=ret[0]['id'],
                     account_id=ret[0]['accountId']
                 )
@@ -336,15 +342,15 @@
                 ret.append(message_dict)
             
             ret = self.filter_valid(ret)
             if len(ret) == 0:
                 return None
             elif len(ret) == 1:
                 logger.info(
-                    message = "return sqs item",
+                    message = f"return sqs item: {ret[0]}",
                     event = Event.POLL,
                     data = ret[0]
                 )
                 set_context_evaluate(
                     evaluate_id=ret[0]['id'],
                     account_id=ret[0]['accountId']
                 )
@@ -382,14 +388,95 @@
         )
         set_context_evaluate(
             evaluate_id=response.json()['id'],
             account_id=response.json()['accountId']
         )
         self.poll_time = time.time()
         return response.json()
+
+    def update_poll(self):
+        '''
+        data update의 경우 kafka로부터 data update event가 담긴 메세지를 받아온다.
+        '''
+        record = self.kafka_consumer.poll(
+            timeout_ms=5000,
+            max_records=1,
+            update_offsets=True, # poll 하자마자 commit을 바로 하는게 아니라, commit시 자동으로 offset을 업데이트
+        )
+        
+        ret = []
+        self.record = record
+        v = record.values()
+        for messages in v:
+            if not isinstance(messages, list):
+                logger.error(f"unexpected kafka message format: {type(message)}")
+                break
+            for message in messages:
+                try:
+                    message_dict = json.loads(message.value.decode('utf-8'))
+                except json.JSONDecodeError:
+                    logger.error("유효한 JSON 형식이 아닙니다.")
+                    continue
+                self.evaluates[message.key] = message.offset
+                ret.append(message_dict['payload'])
+
+        if len(ret) == 0:
+            return None
+        elif len(ret) == 1:
+            logger.info(
+                message = f"return kafka item: {ret[0]}",
+                event = Event.POLL,
+                data = ret[0]
+            )
+            self.poll_time = time.time()
+            return ret[0]
+        else:
+            logger.info(
+                message = f"return kafka item: {ret}",
+                event = Event.POLL,
+                data = ret
+            )
+            self.poll_time = time.time()
+            return ret
+        
+    def update_complete(self, output={}, alert = False):
+        '''
+        data update 파이프라인에서의 validate이라고 보면 된다.
+        update가 끝난뒤 이 함수를 통해서 kafka의 offset을 commit한다.
+        원한다면 slack alert를 보낼 수 있다.
+        '''
+        self.kafka_consumer.commit()
+        logger.info(
+            message = "update_complete payload",
+            event = Event.VALIDATE,
+            data = output
+        )
+        if alert:
+            self.slack_alert(
+                '#alert_data_update',
+                f"update_complete payload for topic: {self.kafka_topic} - result: {output}"
+            )
+        
+    def update_error(self, output={}, alert = False):
+        '''
+        data update 파이프라인에서의 validate_error이라고 보면 된다.
+        update 도중 에러가 발생했을 때 이 함수를 통해서 kafka의 offset을 commit한다.
+        원한다면 slack alert를 보낼 수 있다.
+        '''
+        self.kafka_consumer.commit()
+        logger.info(
+            message = "update_error payload",
+            event = Event.VALIDATE_ERROR,
+            data = output
+        )
+        if alert:
+            self.slack_alert(
+                '#alert_data_update',
+                f"update_error payload for topic: {self.kafka_topic} - result: {output}"
+            )
         
     def validate(self, evaluate_id, output, mock=True, log=True, inference_time=None, usage=1):
         try:
             if mock:
                 logger.info(message = f"validate payload - {output}")
                 return
             if inference_time == None and self.poll_time != None:
@@ -578,8 +665,26 @@
             }
 
             response = requests.request("PUT", url, headers=headers)
             if response.status_code != 200:
                 raise Exception(f'error from stop_instance / response status_code {response.status_code}')
 
         except Exception as e:
-            raise Exception(f"error from stop_instance\n{e}")
+            raise Exception(f"error from stop_instance\n{e}")
+        
+    def slack_alert(self, channel_name, text):
+        '''
+        channel_name : slack 채널 id 또는 #채널명
+        text : 보낼 메세지
+        원하는 slack channel에 메세지를 보내는 함수
+        '''
+        headers = {
+            'Content-Type': 'application/json',
+            'Authorization': f'Bearer xoxb-4286174283573-6855321848326-Z2QnHswtlITp5gNQj7eXVHjP'
+        }
+        payload = {
+            "channel": channel_name,
+            "text": text
+        }
+        response = requests.request("POST", 'https://slack.com/api/chat.postMessage', headers=headers, data=json.dumps(payload))
+        if response.status_code != 200:
+            logger.warning(f'error from slack_alert / response status_code {response.status_code}: {response.text}')
```

### Comparing `dalpha-0.4.3/dalpha/context.py` & `dalpha-0.4.4rc0/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.3/dalpha/dalpha_openai.py` & `dalpha-0.4.4rc0/dalpha/dalpha_openai.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.3/dalpha/logging/__init__.py` & `dalpha-0.4.4rc0/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.3/dalpha/logging/log_formatter.py` & `dalpha-0.4.4rc0/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.3/dalpha/logging/utils.py` & `dalpha-0.4.4rc0/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.3/dalpha/redis.py` & `dalpha-0.4.4rc0/dalpha/redis.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.3/pyproject.toml` & `dalpha-0.4.4rc0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.4.3"
+version = "0.4.4rc0"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -16,15 +16,15 @@
 kafka-python = "^2.0.2"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.4.3"
+version = "0.4.4rc0"
 authors = [
   { name="Beomseok", email="beomseok.lee@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dalpha-0.4.3/PKG-INFO` & `dalpha-0.4.4rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.4.3
+Version: 0.4.4rc0
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

