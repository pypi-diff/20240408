# Comparing `tmp/jsw_jzyunqi-1.0.1.tar.gz` & `tmp/jsw_jzyunqi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsw_jzyunqi-1.0.1.tar", max compression
+gzip compressed data, was "jsw_jzyunqi-1.0.2.tar", max compression
```

## Comparing `jsw_jzyunqi-1.0.1.tar` & `jsw_jzyunqi-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      188 2024-04-08 02:55:52.224430 jsw_jzyunqi-1.0.1/README.md
--rw-r--r--   0        0        0      174 2024-04-08 02:36:08.077700 jsw_jzyunqi-1.0.1/jsw_jzyunqi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 02:31:23.925330 jsw_jzyunqi-1.0.1/jsw_jzyunqi/mbw/__init__.py
--rw-r--r--   0        0        0     2476 2024-04-08 02:54:34.568587 jsw_jzyunqi-1.0.1/jsw_jzyunqi/mbw/scrapy_publish.py
--rw-r--r--   0        0        0       90 2024-04-08 02:41:02.347157 jsw_jzyunqi-1.0.1/jsw_jzyunqi/mbw/settings.py
--rw-r--r--   0        0        0      438 2024-04-08 02:41:10.685917 jsw_jzyunqi-1.0.1/jsw_jzyunqi/mbw/spider_auth.py
--rw-r--r--   0        0        0      447 2024-04-08 03:24:46.962695 jsw_jzyunqi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 jsw_jzyunqi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      188 2024-04-08 02:55:52.224430 jsw_jzyunqi-1.0.2/README.md
+-rw-r--r--   0        0        0      174 2024-04-08 02:36:08.077700 jsw_jzyunqi-1.0.2/jsw_jzyunqi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 02:31:23.925330 jsw_jzyunqi-1.0.2/jsw_jzyunqi/mbw/__init__.py
+-rw-r--r--   0        0        0     2414 2024-04-08 03:29:20.591379 jsw_jzyunqi-1.0.2/jsw_jzyunqi/mbw/scrapy_publish.py
+-rw-r--r--   0        0        0       90 2024-04-08 02:41:02.347157 jsw_jzyunqi-1.0.2/jsw_jzyunqi/mbw/settings.py
+-rw-r--r--   0        0        0      438 2024-04-08 02:41:10.685917 jsw_jzyunqi-1.0.2/jsw_jzyunqi/mbw/spider_auth.py
+-rw-r--r--   0        0        0      447 2024-04-08 03:30:02.296236 jsw_jzyunqi-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 jsw_jzyunqi-1.0.2/PKG-INFO
```

### Comparing `jsw_jzyunqi-1.0.1/jsw_jzyunqi/mbw/scrapy_publish.py` & `jsw_jzyunqi-1.0.2/jsw_jzyunqi/mbw/scrapy_publish.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,27 +8,27 @@
     def __init__(self, **kwargs):
         # scrapy + spider context
         self.scrapy:Any = kwargs.get('scrapy')
         self.ctx:Any = kwargs.get('ctx')
 
         # custom settings
         self.source_domain = kwargs.get('source_domain')
-        self.target_id_key = kwargs.get('target_id_key', 'post_id')
+        self.id_key = kwargs.get('id_key', 'post_id')
         self.db_command = kwargs.get('db_command')
-        self.api_action = kwargs.get('api_action', 'add')
+        self.api_path = kwargs.get('api_path', '/api/python/post/add')
 
         # auth token
         self.token = spider_auth()
 
     def publish(self, items):
         for item in items:
             yield self.publish_one(item)
 
     def publish_one(self, item):
-        api_url = f'{SPIDER_API_URL}/api/python/post/{self.api_action}'
+        api_url = f'{SPIDER_API_URL}{self.api_path}'
         token = self.token
         ctx = self.ctx
         ctx.logger.info('Current data id is %s' % item.get('article_id'))
         # post json to api
         headers = {'Content-Type': 'application/json', 'Authorization': f'bearer {token}'}
         json_body = json.dumps({
             'title': item.get('title'),
@@ -50,16 +50,16 @@
         )
 
     def parse_api_response(self, response):
         record = response.meta['record']
         status = response.status
         text = response.text
         ctx = self.ctx
-        target_id_key = self.target_id_key
-        target_id_value = record.get(target_id_key)
+        id_key = self.id_key
+        id_value = record.get(id_key)
         db_command = self.db_command
 
         if status == 200:
             ctx.logger.info('Data id %s is inserted' % record.get('article_id'))
             payload = {
                 'insert2db_response': None,
                 'is_crawled': True,
@@ -67,13 +67,13 @@
 
         else:
             ctx.logger.error('Data id %s is failed' % record.get('article_id'))
             payload = {
                 'insert2db_response': {'status': status, 'body': text},
             }
 
-        payload[target_id_key] = target_id_value
+        payload[id_key] = id_value
 
         yield {
             'command': db_command,
             'payload': payload
         }
```

### Comparing `jsw_jzyunqi-1.0.1/PKG-INFO` & `jsw_jzyunqi-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsw-jzyunqi
-Version: 1.0.1
+Version: 1.0.2
 Summary: python tools for jzyunqi.
 Home-page: https://js.work
 Author: aric
 Author-email: 1290657123@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

