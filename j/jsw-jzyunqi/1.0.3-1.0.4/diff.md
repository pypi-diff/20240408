# Comparing `tmp/jsw_jzyunqi-1.0.3.tar.gz` & `tmp/jsw_jzyunqi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsw_jzyunqi-1.0.3.tar", max compression
+gzip compressed data, was "jsw_jzyunqi-1.0.4.tar", max compression
```

## Comparing `jsw_jzyunqi-1.0.3.tar` & `jsw_jzyunqi-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      188 2024-04-08 02:55:52.224430 jsw_jzyunqi-1.0.3/README.md
--rw-r--r--   0        0        0      174 2024-04-08 02:36:08.077700 jsw_jzyunqi-1.0.3/jsw_jzyunqi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 02:31:23.925330 jsw_jzyunqi-1.0.3/jsw_jzyunqi/mbw/__init__.py
--rw-r--r--   0        0        0     2418 2024-04-08 03:30:46.588832 jsw_jzyunqi-1.0.3/jsw_jzyunqi/mbw/publish_article.py
--rw-r--r--   0        0        0       90 2024-04-08 02:41:02.347157 jsw_jzyunqi-1.0.3/jsw_jzyunqi/mbw/settings.py
--rw-r--r--   0        0        0      438 2024-04-08 02:41:10.685917 jsw_jzyunqi-1.0.3/jsw_jzyunqi/mbw/spider_auth.py
--rw-r--r--   0        0        0      447 2024-04-08 03:31:09.417093 jsw_jzyunqi-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 jsw_jzyunqi-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      188 2024-04-08 02:55:52.224430 jsw_jzyunqi-1.0.4/README.md
+-rw-r--r--   0        0        0      174 2024-04-08 02:36:08.077700 jsw_jzyunqi-1.0.4/jsw_jzyunqi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 02:31:23.925330 jsw_jzyunqi-1.0.4/jsw_jzyunqi/mbw/__init__.py
+-rw-r--r--   0        0        0     2420 2024-04-08 03:32:05.313865 jsw_jzyunqi-1.0.4/jsw_jzyunqi/mbw/publish_article.py
+-rw-r--r--   0        0        0       90 2024-04-08 02:41:02.347157 jsw_jzyunqi-1.0.4/jsw_jzyunqi/mbw/settings.py
+-rw-r--r--   0        0        0      438 2024-04-08 02:41:10.685917 jsw_jzyunqi-1.0.4/jsw_jzyunqi/mbw/spider_auth.py
+-rw-r--r--   0        0        0      447 2024-04-08 03:32:17.313625 jsw_jzyunqi-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 jsw_jzyunqi-1.0.4/PKG-INFO
```

### Comparing `jsw_jzyunqi-1.0.3/jsw_jzyunqi/mbw/publish_article.py` & `jsw_jzyunqi-1.0.4/jsw_jzyunqi/mbw/publish_article.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         # scrapy + spider context
         self.scrapy:Any = kwargs.get('scrapy')
         self.ctx:Any = kwargs.get('ctx')
 
         # custom settings
         self.source_domain = kwargs.get('source_domain')
         self.id_key = kwargs.get('id_key', 'article_id')
-        self.db_command = kwargs.get('db_command')
+        self.command = kwargs.get('command', 'save_articles')
         self.api_path = kwargs.get('api_path', '/api/python/post/add')
 
         # auth token
         self.token = spider_auth()
 
     def publish(self, items):
         for item in items:
@@ -52,15 +52,15 @@
     def parse_api_response(self, response):
         record = response.meta['record']
         status = response.status
         text = response.text
         ctx = self.ctx
         id_key = self.id_key
         id_value = record.get(id_key)
-        db_command = self.db_command
+        command = self.command
 
         if status == 200:
             ctx.logger.info('Data id %s is inserted' % record.get('article_id'))
             payload = {
                 'insert2db_response': None,
                 'is_crawled': True,
             }
@@ -70,10 +70,10 @@
             payload = {
                 'insert2db_response': {'status': status, 'body': text},
             }
 
         payload[id_key] = id_value
 
         yield {
-            'command': db_command,
+            'command': command,
             'payload': payload
         }
```

### Comparing `jsw_jzyunqi-1.0.3/PKG-INFO` & `jsw_jzyunqi-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsw-jzyunqi
-Version: 1.0.3
+Version: 1.0.4
 Summary: python tools for jzyunqi.
 Home-page: https://js.work
 Author: aric
 Author-email: 1290657123@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

