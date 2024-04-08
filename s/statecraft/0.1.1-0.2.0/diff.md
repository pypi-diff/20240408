# Comparing `tmp/statecraft-0.1.1.tar.gz` & `tmp/statecraft-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statecraft-0.1.1.tar", last modified: Wed Apr  3 11:28:06 2024, max compression
+gzip compressed data, was "statecraft-0.2.0.tar", max compression
```

## Comparing `statecraft-0.1.1.tar` & `statecraft-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,14 @@
-drwxr-xr-x   0 Kola       (501) staff       (20)        0 2024-04-03 11:28:06.848269 statecraft-0.1.1/
--rw-r--r--   0 Kola       (501) staff       (20)    11358 2024-04-03 11:02:42.000000 statecraft-0.1.1/LICENSE
--rw-r--r--   0 Kola       (501) staff       (20)     3324 2024-04-03 11:28:06.848023 statecraft-0.1.1/PKG-INFO
--rw-r--r--   0 Kola       (501) staff       (20)     3207 2024-04-03 10:35:56.000000 statecraft-0.1.1/README.md
--rw-r--r--   0 Kola       (501) staff       (20)      983 2024-04-03 11:21:45.000000 statecraft-0.1.1/pyproject.toml
--rw-r--r--   0 Kola       (501) staff       (20)       38 2024-04-03 11:28:06.848354 statecraft-0.1.1/setup.cfg
--rw-r--r--   0 Kola       (501) staff       (20)      371 2024-04-03 11:26:47.000000 statecraft-0.1.1/setup.py
-drwxr-xr-x   0 Kola       (501) staff       (20)        0 2024-04-03 11:28:06.846545 statecraft-0.1.1/statecraft/
--rw-r--r--   0 Kola       (501) staff       (20)      236 2024-04-03 10:36:07.000000 statecraft-0.1.1/statecraft/__init__.py
--rw-r--r--   0 Kola       (501) staff       (20)      849 2024-03-27 00:09:23.000000 statecraft-0.1.1/statecraft/_setup.py
--rw-r--r--   0 Kola       (501) staff       (20)     4148 2024-04-03 10:38:43.000000 statecraft-0.1.1/statecraft/client.py
--rw-r--r--   0 Kola       (501) staff       (20)    10281 2024-04-03 10:43:20.000000 statecraft-0.1.1/statecraft/core.py
--rw-r--r--   0 Kola       (501) staff       (20)      287 2024-03-26 13:46:51.000000 statecraft-0.1.1/statecraft/metadata.py
--rw-r--r--   0 Kola       (501) staff       (20)      368 2024-03-26 15:52:01.000000 statecraft-0.1.1/statecraft/models.py
--rw-r--r--   0 Kola       (501) staff       (20)     1682 2024-04-03 10:35:22.000000 statecraft-0.1.1/statecraft/states_list.py
--rw-r--r--   0 Kola       (501) staff       (20)      195 2024-03-27 00:03:59.000000 statecraft-0.1.1/statecraft/user_attributes.py
--rw-r--r--   0 Kola       (501) staff       (20)      398 2024-03-26 15:06:22.000000 statecraft-0.1.1/statecraft/utils.py
-drwxr-xr-x   0 Kola       (501) staff       (20)        0 2024-04-03 11:28:06.847702 statecraft-0.1.1/statecraft.egg-info/
--rw-r--r--   0 Kola       (501) staff       (20)     3324 2024-04-03 11:28:06.000000 statecraft-0.1.1/statecraft.egg-info/PKG-INFO
--rw-r--r--   0 Kola       (501) staff       (20)      381 2024-04-03 11:28:06.000000 statecraft-0.1.1/statecraft.egg-info/SOURCES.txt
--rw-r--r--   0 Kola       (501) staff       (20)        1 2024-04-03 11:28:06.000000 statecraft-0.1.1/statecraft.egg-info/dependency_links.txt
--rw-r--r--   0 Kola       (501) staff       (20)       11 2024-04-03 11:28:06.000000 statecraft-0.1.1/statecraft.egg-info/top_level.txt
+-rw-r--r--   0        0        0    11358 2024-04-03 11:02:42.934332 statecraft-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3125 2024-04-06 21:45:35.753326 statecraft-0.2.0/README.md
+-rw-r--r--   0        0        0      993 2024-04-08 09:40:25.775390 statecraft-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      236 2024-04-03 10:36:07.499173 statecraft-0.2.0/statecraft/__init__.py
+-rw-r--r--   0        0        0      849 2024-03-27 00:09:23.511207 statecraft-0.2.0/statecraft/_setup.py
+-rw-r--r--   0        0        0     1816 2024-04-07 23:03:02.330960 statecraft-0.2.0/statecraft/cache.py
+-rw-r--r--   0        0        0     4513 2024-04-07 23:03:02.332394 statecraft-0.2.0/statecraft/client.py
+-rw-r--r--   0        0        0    16342 2024-04-07 23:03:02.334208 statecraft-0.2.0/statecraft/core.py
+-rw-r--r--   0        0        0      287 2024-03-26 13:46:51.357963 statecraft-0.2.0/statecraft/metadata.py
+-rw-r--r--   0        0        0      417 2024-04-07 23:03:02.340045 statecraft-0.2.0/statecraft/models.py
+-rw-r--r--   0        0        0     1682 2024-04-03 10:35:22.202552 statecraft-0.2.0/statecraft/states_list.py
+-rw-r--r--   0        0        0      195 2024-03-27 00:03:59.367245 statecraft-0.2.0/statecraft/user_attributes.py
+-rw-r--r--   0        0        0      838 2024-04-07 23:03:02.340438 statecraft-0.2.0/statecraft/utils.py
+-rw-r--r--   0        0        0     4370 1970-01-01 00:00:00.000000 statecraft-0.2.0/PKG-INFO
```

### Comparing `statecraft-0.1.1/LICENSE` & `statecraft-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `statecraft-0.1.1/PKG-INFO` & `statecraft-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-Metadata-Version: 2.1
-Name: statecraft
-Version: 0.1.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# 🪄 Statecraft -  Store, manage and remix states for SSMs and Stateful models
+# 🪄 Statecraft -  Load, store and remix states for SSMs, Mamba and Stateful models
 
 ## TL;DR
 
 With statecraft you can easily load states from a file or from the community repository and use them in your SSMs or stateful models. The interface is just like Huggingface's Transformers library:
 
 ```python
 from statecraft import StatefulModel
@@ -28,19 +22,19 @@
 ```
 
 ## ✨ Other Features
 
 - Use `model.build_state()` to generate a new state from your context.
 - Use `model.save_state()` or `model.save_current_state` to save your state to a file so that you can use it again in the future.
 - With `model.load_state()` you can load a state either from a file or from the community repository.
+  - To see the states that are available in the community repository, visit the [Statecraft Hub](https://statecrafthub.com) or use `statecraft.list_states()`.
 
 ## 🔍 Coming Soon
 
 - Right now we only support Mamba models (in all sizes), as more SSMs and Stateful models begin to come onto Huggingface, we will support them too.
-- The statecraft community repository is available right now and a front-end for this is coming so you can view all of the community-contributed states. Right now, you can see the available states by running `statecraft.show_available_states()`.
 - We're also looking at RAG-like generation approaches where you automatically retrieve the `state` instead of `context`, watch this space 👀
 
 ## 🧙 Conceptually
 
 Currently, we often use RAG to give a transformer contextual information.
 
 With Mamba-like models, you could instead imagine having a library of states created by running the model over specialised data. States could be shared kinda like LoRAs for image models.
```

### Comparing `statecraft-0.1.1/pyproject.toml` & `statecraft-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "statecraft"
-version = "0.1.0"
+version = "0.2.0"
 description = "Store, manage and remix states for SSMs and other Stateful models"
 authors = ["koayon <koayon@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "statecraft"}]
-requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Typing :: Typed",
 ]
 
 [tool.poetry.urls]
 Repository = "https://github.com/koayon/statecraft.git"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+einops= "^0.6.1"
+pydantic = "^2.5.3"
+python = "^3.8"
 python-dotenv = "^0.19.1"
-responses = "^0.13.4"
-torch = "2.1.2"
-transformers = "4.40.0.dev0"
-pydantic = "2.5.3"
-Requests = "2.31.0"
-typer = "0.7.0"
+Requests = "^2.31.0"
+torch = "^2.1.2"
+transformers = "^4.39.3"
+typer = "^0.7.0"
+accelerate = "^0.29.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pylint = "^2.17.4"
-setuptools = "67.7.2"
+setuptools = "^67.7.2"
+poetry = "^1.8.2"
```

### Comparing `statecraft-0.1.1/statecraft/_setup.py` & `statecraft-0.2.0/statecraft/_setup.py`

 * *Files identical despite different names*

### Comparing `statecraft-0.1.1/statecraft/client.py` & `statecraft-0.2.0/statecraft/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 import requests
 
 from statecraft.metadata import SSMStateMetadata
 from statecraft.models import StateOut, StatesOut
 from statecraft.user_attributes import UserAttributes
 from statecraft.utils import get_default_cache_dir
 
-BASE_URL = "https://www.api.statecrafthub.com/"
-LOCAL_URL = "http://localhost/"
+BASE_URL = "https://www.api.statecrafthub.com"
+LOCAL_URL = "http://localhost"
 
 
 class StatecraftClient:
 
     def __init__(self, base_url: str = BASE_URL):
         self.base_url = base_url
-        self.states_url = f"{base_url}states/"
+        self.states_url = f"{base_url}/states"
 
     def get_state(self, model_name: str, state_name: str) -> bytes:
-        full_url = os.path.join(self.states_url, model_name, state_name)
+        full_url = f"{self.states_url}/{model_name}/{state_name}"
 
         response = requests.get(full_url)
 
         if response.status_code == 200:
             raw_bytes = response.content
             print("Got state - raw_bytes: ", raw_bytes[:100])
             return raw_bytes
@@ -33,15 +33,15 @@
             raise ValueError(f"Failed to get state: {response.text}")
 
     def upload_state(
         self,
         metadata: SSMStateMetadata,
         state_path: Union[Path, str],
     ) -> str:
-        url = self.states_url
+        url = f"{self.states_url}/"
 
         print(url)
 
         state_short_name = metadata.state_name.split("/")[-1]
 
         user_attributes = self._fetch_user_attrs()
         username = user_attributes.username
@@ -84,24 +84,34 @@
     def get_states(self, model_name: str) -> list[str]:
         model_user_name, model_short_name = model_name.split("/")
         query_params = {
             "model_user_name": model_user_name,
             "model_short_name": model_short_name,
         }
 
+        url = f"{self.states_url}/"
+
         response = requests.get(
-            self.states_url,
+            url,
             params=query_params,
         )
         print(response.text)
-        parsed_response: list[dict[str, str]] = response.json()  # StatesOut
+        parsed_response = response.json()  # StatesOut
+
+        if isinstance(parsed_response, list):  # Previous API version
+            states_out = StatesOut(states=parsed_response, total_count=len(parsed_response))
+        else:  # Current API version
+            states_out = StatesOut(
+                states=parsed_response.get("states"),
+                total_count=parsed_response.get("total_count"),
+            )
 
         states_list = [
-            f'{response_state_dict["model_name"]}/{response_state_dict["state_name"]}'
-            for response_state_dict in parsed_response
+            f"{response_state_dict.model_name}/{response_state_dict.state_name}"
+            for response_state_dict in states_out.states
         ]
 
         return states_list
 
     def create_user(self, username: str, email: str) -> int:
         response = requests.post(
             os.path.join(self.base_url, "users"),
```

### Comparing `statecraft-0.1.1/statecraft/states_list.py` & `statecraft-0.2.0/statecraft/states_list.py`

 * *Files identical despite different names*

