# Comparing `tmp/vector_vault-4.3.3.tar.gz` & `tmp/vector_vault-4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.3.3.tar", last modified: Thu Apr  4 06:19:26 2024, max compression
+gzip compressed data, was "vector_vault-4.3.4.tar", last modified: Mon Apr  8 20:08:36 2024, max compression
```

## Comparing `vector_vault-4.3.3.tar` & `vector_vault-4.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 06:19:26.273832 vector_vault-4.3.3/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.3.3/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 06:19:26.273684 vector_vault-4.3.3/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.3.3/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-04 06:19:26.273868 vector_vault-4.3.3/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-04 06:19:18.000000 vector_vault-4.3.3/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 06:19:26.270388 vector_vault-4.3.3/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 06:19:26.000000 vector_vault-4.3.3/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-04 06:19:26.000000 vector_vault-4.3.3/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-04 06:19:26.000000 vector_vault-4.3.3/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-04 06:19:26.000000 vector_vault-4.3.3/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-04 06:19:26.000000 vector_vault-4.3.3/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 06:19:26.273310 vector_vault-4.3.3/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.3.3/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.3.3/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.3.3/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5982 2024-04-04 06:07:20.000000 vector_vault-4.3.3/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.3.3/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.3.3/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-04 06:07:40.000000 vector_vault-4.3.3/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-04 06:07:37.000000 vector_vault-4.3.3/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62521 2024-04-04 06:19:13.000000 vector_vault-4.3.3/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.3.3/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.3.3/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 20:08:36.793856 vector_vault-4.3.4/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.3.4/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-08 20:08:36.793710 vector_vault-4.3.4/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.3.4/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-08 20:08:36.793911 vector_vault-4.3.4/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-08 20:07:45.000000 vector_vault-4.3.4/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 20:08:36.789716 vector_vault-4.3.4/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-08 20:08:36.000000 vector_vault-4.3.4/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-08 20:08:36.000000 vector_vault-4.3.4/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-08 20:08:36.000000 vector_vault-4.3.4/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-08 20:08:36.000000 vector_vault-4.3.4/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-08 20:08:36.000000 vector_vault-4.3.4/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 20:08:36.793428 vector_vault-4.3.4/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.3.4/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.3.4/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.3.4/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5996 2024-04-08 20:07:11.000000 vector_vault-4.3.4/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.3.4/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.3.4/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-08 20:07:01.000000 vector_vault-4.3.4/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-08 20:06:58.000000 vector_vault-4.3.4/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62383 2024-04-08 20:06:54.000000 vector_vault-4.3.4/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.3.4/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.3.4/vectorvault/wrap.py
```

### Comparing `vector_vault-4.3.3/LICENSE` & `vector_vault-4.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.3/PKG-INFO` & `vector_vault-4.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.3.3
+Version: 4.3.4
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.3.3/README.md` & `vector_vault-4.3.4/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.3/setup.py` & `vector_vault-4.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.3.3",
+    version="4.3.4",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.3.3/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.3.4/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.3.3
+Version: 4.3.4
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.3.3/vectorvault/ai.py` & `vector_vault-4.3.4/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.3/vectorvault/cloud_api.py` & `vector_vault-4.3.4/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.3/vectorvault/cloudmanager.py` & `vector_vault-4.3.4/vectorvault/cloudmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,16 @@
         temp_file_path = self.download_to_temp_file(f'{self.username}.json')
         with open(temp_file_path, 'r') as json_file:
             _map = json.load(json_file)
         os.remove(temp_file_path)
         return _map
     
     def update(self):
-        T(target=call_update, args=(self.user, self.vault, self.api)).start()
+        t = T(target=call_update, args=(self.user, self.vault, self.api))
+        t.start()
     
     def build_update(self):
         _map = self.get_mapping()
         for i in range(len(_map)):
             if _map[i]['vault'] == self.vault:
                 _map[i]['last_use'] = time.time()
                 try:
```

### Comparing `vector_vault-4.3.3/vectorvault/creds.py` & `vector_vault-4.3.4/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.3/vectorvault/download.py` & `vector_vault-4.3.4/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.3/vectorvault/itemize.py` & `vector_vault-4.3.4/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.3/vectorvault/tools_gpt.py` & `vector_vault-4.3.4/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.3/vectorvault/vault.py` & `vector_vault-4.3.4/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -1005,15 +1005,15 @@
                     print(traceback.format_exc())
                     print(f"API Error: {e}. Backing off for {self.rate_limiter.current_delay} seconds.")
                     self.rate_limiter.on_failure()
                     if attempts >= self.rate_limiter.max_attempts:
                         print(f"API Failed too many times, exiting loop: {e}.")
                         break
 
-        self.update_conversation_history(self.cuid, response, user=False) if self.cuid else None
+        self.update_conversation_history(self.cuid, f'User: {text} \n\nAI: {response}', user=False) if self.cuid else None
         print("get chat time --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
             
         return {'response': response, 'context': context} if return_context else response
         
 
     def get_chat_stream(self, text: str = None, history: str = '', summary: bool = False, get_context: bool = False,
                         n_context: int = 4, return_context: bool = False, history_search: bool = False, smart_history_search: bool = False, 
@@ -1125,15 +1125,15 @@
                                     yield word
                                 yield ' '
 
                             self.rate_limiter.on_success()
                         except Exception as e:
                             raise e
                         if counter == len(inputs):
-                            self.update_conversation_history(self.cuid, full_response, user=False) if self.cuid else None
+                            self.update_conversation_history(self.cuid, f'User: {text} \n\nAI: {full_response}', user=False) if self.cuid else None
                             yield '!END'
                             self.rate_limiter.on_success()
                     
                     elif text and get_context and not summary:
                         if smart_history_search:
                             custom_entry = f"Using the current message, with the message history, what is the user is focused on. \nCurrent message: {text}. \n\nPrevious messages: {history}."
                             search_input = self.ai.llm(custom_prompt=custom_entry, model=model, temperature=temperature, timeout=timeout)
@@ -1163,31 +1163,31 @@
                                         if metatag_suffixes:
                                             for i in range(len(metatag)):
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}']) + str(metatag_suffixes[i])
                                         else:
                                             for i in range(len(metatag)):
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
                                 yield item['data']
-                            self.update_conversation_history(self.cuid, full_response, user=False) if self.cuid else None
+                            self.update_conversation_history(self.cuid, f'User: {text} \n\nAI: {full_response}', user=False) if self.cuid else None
                             yield '!END'
                             self.rate_limiter.on_success()
                         else:
-                            self.update_conversation_history(self.cuid, full_response, user=False) if self.cuid else None
+                            self.update_conversation_history(self.cuid, f'User: {text} \n\nAI: {full_response}', user=False) if self.cuid else None
                             yield '!END'
                             self.rate_limiter.on_success()
 
                     else:
                         try:
                             for word in self.ai.llm_stream(segment, history, model=model, custom_prompt=custom_prompt, temperature=temperature):
                                 full_response += word
                                 yield word
                             self.rate_limiter.on_success()
                         except Exception as e:
                             raise e
-                        self.update_conversation_history(self.cuid, full_response, user=False) if self.cuid else None
+                        self.update_conversation_history(self.cuid, f'User: {text} \n\nAI: {full_response}', user=False) if self.cuid else None
                         yield '!END'
 
                     self.rate_limiter.on_success()
                     break
                 except Exception as e:
                     exceptions += 1
                     print(f"API Error: {e}. Applying backoff.")
@@ -1214,15 +1214,15 @@
                         print(f'\n{word}', end='', flush=True)
                     else:
                         print(word, end='', flush=True) 
             else:
                 return full_text
         
 
-    def print_vault_data(self, print_data: bool = True, return_data: bool = False):
+    def print_vault_data(self, return_data: bool = False):
         ''' 
             Function to print vault data 
         ''' 
         vd = self.cloud_manager.get_mapping()
         # Function to format datetime
         def format_datetime(dt, is_timestamp=False):
             if is_timestamp:
@@ -1261,16 +1261,15 @@
         '''
             For cloud application yielding the chat stream, like a flask app
         '''
         for word in function:
             yield f"data: {json.dumps({'data': word})} \n\n"
 
 
-    def update_conversation_history(self, conversation_id, message, metadata_list = None, user = True):
-        message = f'User: {message}' if user else f'AI: {message}'
+    def update_conversation_history(self, conversation_id, message, metadata_list = None):
         try:
             metadata_list = metadata_list if metadata_list else json.loads(self.cloud_manager.download_text_from_cloud(f'user_history/{conversation_id}/metadata'))
         except:
             metadata_list = []
         message_id = f"{time.time():.0f}"  # Current time
         metadata_list.append({ 'M': message_id, 'L': len(message) })
         t1 = T(target=self.cloud_manager.upload_to_cloud, args=(f'user_history/{conversation_id}/{message_id}', message))
@@ -1306,17 +1305,14 @@
         try:
             meta = download_conversation_metadata()
         except:
             meta = None
 
         message_ids = golden_retriever(meta) if meta != None else []
 
-        update = T(target=self.update_conversation_history, args=(conversation_id, message, meta if meta else None))
-        update.start()
-
         print('message_ids:', message_ids) if self.verbose else None
 
         if message_ids != []:
             history_lines = []
             with ThreadPoolExecutor(max_workers=10) as executor:
                 future_to_message_id = {executor.submit(download_conversation_message, message_id): message_id for message_id in message_ids}
 
@@ -1334,15 +1330,14 @@
             for i in vector_similar_results:
                 message_time = datetime.fromtimestamp(float(i['metadata']['name']))
                 data = i['data']
                 vector_history.append(f'{get_time_statement(now, message_time)} {data}')                
 
             history = history + "Vector search conversation history:" + '\n'.join(vector_history)
 
-        update.join()
         return history
 
 
 class RateLimiter:
     def __init__(self, max_attempts=30):
         self.base_delay = 1  # Base delay of 1 second
         self.max_delay = 60  # Maximum delay of 60 seconds
```

### Comparing `vector_vault-4.3.3/vectorvault/vecreq.py` & `vector_vault-4.3.4/vectorvault/vecreq.py`

 * *Files identical despite different names*

