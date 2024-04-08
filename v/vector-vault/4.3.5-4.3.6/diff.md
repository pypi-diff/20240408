# Comparing `tmp/vector_vault-4.3.5.tar.gz` & `tmp/vector_vault-4.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.3.5.tar", last modified: Mon Apr  8 20:22:31 2024, max compression
+gzip compressed data, was "vector_vault-4.3.6.tar", last modified: Mon Apr  8 20:53:48 2024, max compression
```

## Comparing `vector_vault-4.3.5.tar` & `vector_vault-4.3.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 20:22:31.998572 vector_vault-4.3.5/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.3.5/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-08 20:22:31.998426 vector_vault-4.3.5/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.3.5/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-08 20:22:31.998608 vector_vault-4.3.5/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-08 20:22:09.000000 vector_vault-4.3.5/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 20:22:31.995596 vector_vault-4.3.5/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-08 20:22:31.000000 vector_vault-4.3.5/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-08 20:22:31.000000 vector_vault-4.3.5/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-08 20:22:31.000000 vector_vault-4.3.5/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-08 20:22:31.000000 vector_vault-4.3.5/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-08 20:22:31.000000 vector_vault-4.3.5/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 20:22:31.998230 vector_vault-4.3.5/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.3.5/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.3.5/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.3.5/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5996 2024-04-08 20:07:11.000000 vector_vault-4.3.5/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.3.5/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.3.5/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-08 20:07:01.000000 vector_vault-4.3.5/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-08 20:06:58.000000 vector_vault-4.3.5/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62232 2024-04-08 20:22:05.000000 vector_vault-4.3.5/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.3.5/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.3.5/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 20:53:48.831695 vector_vault-4.3.6/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.3.6/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-08 20:53:48.831552 vector_vault-4.3.6/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.3.6/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-08 20:53:48.831730 vector_vault-4.3.6/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-08 20:53:13.000000 vector_vault-4.3.6/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 20:53:48.827488 vector_vault-4.3.6/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-08 20:53:48.000000 vector_vault-4.3.6/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-08 20:53:48.000000 vector_vault-4.3.6/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-08 20:53:48.000000 vector_vault-4.3.6/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-08 20:53:48.000000 vector_vault-4.3.6/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-08 20:53:48.000000 vector_vault-4.3.6/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 20:53:48.831260 vector_vault-4.3.6/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.3.6/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.3.6/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.3.6/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5996 2024-04-08 20:07:11.000000 vector_vault-4.3.6/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.3.6/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.3.6/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-08 20:07:01.000000 vector_vault-4.3.6/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-08 20:06:58.000000 vector_vault-4.3.6/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62668 2024-04-08 20:53:06.000000 vector_vault-4.3.6/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.3.6/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.3.6/vectorvault/wrap.py
```

### Comparing `vector_vault-4.3.5/LICENSE` & `vector_vault-4.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.5/PKG-INFO` & `vector_vault-4.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.3.5
+Version: 4.3.6
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.3.5/README.md` & `vector_vault-4.3.6/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.5/setup.py` & `vector_vault-4.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.3.5",
+    version="4.3.6",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.3.5/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.3.6/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.3.5
+Version: 4.3.6
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.3.5/vectorvault/ai.py` & `vector_vault-4.3.6/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.5/vectorvault/cloud_api.py` & `vector_vault-4.3.6/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.5/vectorvault/cloudmanager.py` & `vector_vault-4.3.6/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.5/vectorvault/creds.py` & `vector_vault-4.3.6/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.5/vectorvault/download.py` & `vector_vault-4.3.6/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.5/vectorvault/itemize.py` & `vector_vault-4.3.6/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.5/vectorvault/tools_gpt.py` & `vector_vault-4.3.6/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.5/vectorvault/vault.py` & `vector_vault-4.3.6/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,31 +84,29 @@
         try:
             self.cloud_manager = CloudManager(self.user, self.api, self.vault)
             print(f'Connected vault: {self.vault}') if self.verbose else 0 
         except Exception as e:
             print('API KEY NOT FOUND or no internet connection!', e)
             # user can still use the get_chat() function without an api key
             self.cloud_manager = None
-
-        T(target=self.init_vecs)
+  
+        self.vectors = get_vectors(self.dims)
         self.x = 0
         self.x_checked = False
+        self.x_loaded_checked = False
         self.vecs_loaded = False
         self.map = {}
         self.items = []
         self.last_time = None
         self.saved_already = False
         self.ai_loaded = False
         self.tools = ToolsGPT(verbose=verbose)
         self.rate_limiter = RateLimiter(max_attempts=30)
         self.cuid = conversation_user_id
 
-    def init_vecs(self):
-        self.vectors = get_vectors(self.dims)
-
     def get_vaults(self, vault: str = None):
         '''
             Returns a list of vaults within the current vault directory 
         '''
         vault = self.vault if vault is None else vault
         if self.cloud_manager is None:
            time.sleep(.3)
@@ -133,31 +131,31 @@
                 return 0
 
 
     def get_tokens(self, text: str):
         '''
             Returns the number of tokens for any given text
         '''
-        self.load_ai()
+        self.load_ai() if not self.ai_loaded else None
         return self.ai.get_tokens(text)
     
 
     def get_distance(self, id1: int, id2: int):
         '''
             Returns the distance between two vectors - item ids are needed to compare
         '''
-        self.check_index()
+        self.check_index_loaded()
         return self.vectors.get_distance(id1, id2)
     
 
     def get_item_vector(self, item_id: int):
         '''
             Returns the vector from an item id
         '''
-        self.check_index()
+        self.check_index_loaded()
         return self.vectors.get_item_vector(item_id)
 
 
     def load_ai(self):
         self.ai_loaded = True
         self.ai = AI(verbose=self.verbose)
         self.ai.context_prompt = self.fetch_custom_prompt()
@@ -381,22 +379,31 @@
         '''
             Edit and save any item's metadata
         '''
         self.cloud_manager.upload_to_cloud(cloud_name(self.vault, self.map[str(item_id)], self.user, self.api, meta=True), json.dumps(metadata))
         print(f'Item {item_id} metadata saved') if self.verbose else 0
 
 
-    def check_index(self):
-        if not self.x_checked:
+    def check_index_loaded(self):
+        if not self.x_loaded_checked:
             start_time = time.time()
             if self.cloud_manager.vault_exists(name_vecs(self.vault, self.user, self.api)):
                 if not self.vecs_loaded:
                     self.load_vectors()
-                self.reload_vectors()
-            
+
+            self.x_loaded_checked = True
+            print("initialize index --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
+
+    def check_index(self):
+        if not self.x_checked:
+            start_time = time.time()
+            if self.cloud_manager.vault_exists(name_vecs(self.vault, self.user, self.api)):
+                if self.vecs_loaded:
+                    self.reload_vectors()
+
             self.x_checked = True
             print("initialize index --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
                 
 
     def load_mapping(self, vault = None):
         '''Internal function only'''
         vault = vault if vault else self.vault 
@@ -423,14 +430,27 @@
         self.vectors.load(temp_file_path)
         os.remove(temp_file_path)
         t.join()
         self.vecs_loaded = True
         print("get load vectors --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
 
 
+    def reload_vectors(self):
+        num_existing_items = self.vectors.get_n_items()
+        new_index = get_vectors(self.dims)
+        count = -1
+        for i in range(num_existing_items):
+            count += 1
+            vector = self.vectors.get_item_vector(i)
+            new_index.add_item(i, vector)
+        self.x = count + 1
+        self.vectors = new_index
+        self.vecs_loaded = False
+
+
     def make_3d_map(self, highlight_id: int = None, return_html: bool = False):
         from kneed import KneeLocator
         from sklearn.cluster import DBSCAN
         from sklearn.neighbors import NearestNeighbors
         from sklearn.manifold import TSNE
         import plotly.graph_objs as go
 
@@ -520,26 +540,14 @@
         fig = go.Figure(data=data, layout=layout)
         if return_html:
             return fig.to_html(full_html=False, include_plotlyjs='cdn')
         else:
             fig.show()
 
 
-    def reload_vectors(self):
-        num_existing_items = self.vectors.get_n_items()
-        new_index = get_vectors(self.dims)
-        count = -1
-        for i in range(num_existing_items):
-            count += 1
-            vector = self.vectors.get_item_vector(i)
-            new_index.add_item(i, vector)
-        self.x = count + 1
-        self.vectors = new_index
-
-
     def upload_vectors(self, vault = None):
         vault = vault if vault else self.vault
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             vector_temp_file_path = temp_file.name
             self.vectors.save(vector_temp_file_path)
             byte = os.path.getsize(vector_temp_file_path)
             self.cloud_manager.upload_temp_file(vector_temp_file_path, name_vecs(vault, self.user, self.api, byte))
@@ -932,16 +940,15 @@
                 (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
                 Answer:
             """ 
             response = vault.get_chat(text, chat_history, get_context=True, custom_prompt=my_prompt)
             ```
 
         '''
-        if not self.ai_loaded:
-            self.load_ai()
+        self.load_ai() if not self.ai_loaded else None
         model = model.lower()
         start_time = time.time()
     
         history = self.get_conversation_history(self.cuid, text) if self.cuid else history
         
         if text: 
             inputs = [text]
@@ -1078,16 +1085,15 @@
 
                 (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
                 Answer:
             """ 
             response = vault.print_stream(vault.get_chat_stream(text, chat_history, get_context = True, custom_prompt=my_prompt))
             ```
         '''
-        if not self.ai_loaded:
-            self.load_ai()
+        self.load_ai() if not self.ai_loaded else None
         model = model.lower()
         start_time = time.time()
     
         history = self.get_conversation_history(self.cuid, text) if self.cuid else history
 
         if text:
             inputs = [text]
```

### Comparing `vector_vault-4.3.5/vectorvault/vecreq.py` & `vector_vault-4.3.6/vectorvault/vecreq.py`

 * *Files identical despite different names*

