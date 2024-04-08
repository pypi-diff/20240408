# Comparing `tmp/bioimageio-chatbot-0.1.92.tar.gz` & `tmp/bioimageio-chatbot-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio-chatbot-0.1.92.tar", last modified: Fri Apr  5 20:49:17 2024, max compression
+gzip compressed data, was "bioimageio-chatbot-0.1.93.tar", last modified: Mon Apr  8 18:18:45 2024, max compression
```

## Comparing `bioimageio-chatbot-0.1.92.tar` & `bioimageio-chatbot-0.1.93.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.672400 bioimageio-chatbot-0.1.92/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-04-05 20:49:17.672400 bioimageio-chatbot-0.1.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.668400 bioimageio-chatbot-0.1.92/bioimageio_chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.668400 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/bia_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/biii_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/docs_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/vision_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.668400 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/gpts_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/jsonschema_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/knowledge_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.672400 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-04-05 20:49:17.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-05 20:49:17.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:49:17.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 20:49:17.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 20:49:17.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:49:17.672400 bioimageio-chatbot-0.1.92/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.672400 bioimageio-chatbot-0.1.92/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/tests/test_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/tests/test_chatbot_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/tests/test_eval_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/tests/test_knowledge_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:18:45.119007 bioimageio-chatbot-0.1.93/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-04-08 18:18:45.119007 bioimageio-chatbot-0.1.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:18:45.115007 bioimageio-chatbot-0.1.93/bioimageio_chatbot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19805 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:18:45.119007 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/bia_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/biii_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/docs_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/vision_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:18:45.119007 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/web_search_extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/gpts_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/jsonschema_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/knowledge_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:18:45.119007 bioimageio-chatbot-0.1.93/bioimageio_chatbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-04-08 18:18:45.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-08 18:18:45.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:18:45.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 18:18:45.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 18:18:45.000000 bioimageio-chatbot-0.1.93/bioimageio_chatbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:18:45.119007 bioimageio-chatbot-0.1.93/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:18:45.119007 bioimageio-chatbot-0.1.93/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/tests/test_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/tests/test_chatbot_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/tests/test_eval_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 18:18:32.000000 bioimageio-chatbot-0.1.93/tests/test_knowledge_base.py
```

### Comparing `bioimageio-chatbot-0.1.92/LICENSE` & `bioimageio-chatbot-0.1.93/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/PKG-INFO` & `bioimageio-chatbot-0.1.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio-chatbot
-Version: 0.1.92
+Version: 0.1.93
 Summary: Your Personal Assistant in BioImage Analysis.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: schema-agents>=0.1.46
 Requires-Dist: imjoy-rpc>=0.5.48.post2
 Requires-Dist: requests
 Requires-Dist: pypdf
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.92 Summary: Your
+Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.93 Summary: Your
 Personal Assistant in BioImage Analysis. Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.46 Requires-
 Dist: imjoy-rpc>=0.5.48.post2 Requires-Dist: requests Requires-Dist: pypdf
 Requires-Dist: pillow Requires-Dist: matplotlib Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm Requires-Dist: aiofiles Requires-Dist: langchain>=0.1.6
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas Requires-Dist: duckduckgo-
 search>=5.1.0 Requires-Dist: rank-bm25 Requires-Dist: langchain-openai
```

### Comparing `bioimageio-chatbot-0.1.92/README.md` & `bioimageio-chatbot-0.1.93/README.md`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/__main__.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/__main__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot.py`

 * *Files 6% similar despite different names*

```diff
@@ -177,14 +177,27 @@
     )
 
     nina = Role(
         instructions=nina_instructions,
         actions=[respond_to_user],
         model="gpt-4-0125-preview",
     )
+    
+    skyler_instructions = (
+        "As Skyler, your focus is on serving as an assistant in bioimage analysis. "
+        "Address only inquiries related to bioimage analysis, ensuring your responses are not only accurate, concise, and logical, but also educational and engaging. "
+        "Your mission is to decipher the user's needs through clarifying questions, help user by invoking the provided tools."
+    )
+
+    skyler = Role(
+        instructions=skyler_instructions,
+        actions=[respond_to_user],
+        model="gpt-4-0125-preview",
+    )
+
 
     # convert to a list
     all_extensions = [
         {"id": ext.id, "name": ext.name, "description": ext.description} for ext in builtin_extensions
     ]
     # remove item with 'book' in all_extensions
     melman_extensions = [
@@ -198,18 +211,20 @@
     # only keep the item with 'book' in all_extensions
     nina_extensions = [
         ext for ext in all_extensions if "books" == ext["id"]
     ] + [
         ext for ext in all_extensions if ext["id"] == "web"
     ]
 
+    skyler_extensions = []
     return [
         {"name": "Melman", "agent": melman, "extensions": melman_extensions, "code_interpreter": False, "alias": "BioImage Seeker", "icon": "https://bioimage.io/static/img/bioimage-io-icon.svg", "welcome_message": "Hi there! I'm Melman. I am help you navigate the bioimage analysis tools and provide information about bioimage analysis. How can I help you today?"},
         {"name": "Nina", "agent": nina, "extensions": nina_extensions, "code_interpreter": False, "alias": "BioImage Tutor", "icon": "https://bioimage.io/static/img/bioimage-io-icon.svg", "welcome_message": "Hi there! I'm Nina, I can help with your learning journey in bioimage analysis. How can I help you today?"},
         {"name": "Bridget", "agent": bridget, "extensions": bridget_extensions, "code_interpreter": True, "alias": "BioImage Analyst", "icon": "https://bioimage.io/static/img/bioimage-io-icon.svg", "welcome_message": "Hi there! I'm Bridget, I can help you with your image analysis tasks. Please mount your data folder and let me know how I can assist you today."},
+        {"name": "Skyler", "agent": skyler, "extensions": skyler_extensions, "code_interpreter": False, "alias": "BioImage Explorer", "icon": "https://bioimage.io/static/img/bioimage-io-icon.svg", "welcome_message": "Hi there! I'm Skyler. How can I help you today?"},
     ]
 
 
 async def save_chat_history(chat_log_full_path, chat_his_dict):
     # Serialize the chat history to a json string
     chat_history_json = json.dumps(chat_his_dict)
```

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/__init__.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/bia_extension.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/bia_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/biii_extension.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/biii_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/docs_extension.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/docs_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/vision_extension.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/vision_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/evaluation.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/evaluation.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/gpts_action.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/gpts_action.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/jsonschema_pydantic.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/jsonschema_pydantic.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/knowledge_base.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot/utils.py` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/PKG-INFO` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio-chatbot
-Version: 0.1.92
+Version: 0.1.93
 Summary: Your Personal Assistant in BioImage Analysis.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: schema-agents>=0.1.46
 Requires-Dist: imjoy-rpc>=0.5.48.post2
 Requires-Dist: requests
 Requires-Dist: pypdf
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.92 Summary: Your
+Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.93 Summary: Your
 Personal Assistant in BioImage Analysis. Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.46 Requires-
 Dist: imjoy-rpc>=0.5.48.post2 Requires-Dist: requests Requires-Dist: pypdf
 Requires-Dist: pillow Requires-Dist: matplotlib Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm Requires-Dist: aiofiles Requires-Dist: langchain>=0.1.6
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas Requires-Dist: duckduckgo-
 search>=5.1.0 Requires-Dist: rank-bm25 Requires-Dist: langchain-openai
```

### Comparing `bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/SOURCES.txt` & `bioimageio-chatbot-0.1.93/bioimageio_chatbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/pyproject.toml` & `bioimageio-chatbot-0.1.93/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "bioimageio-chatbot"
-version = "0.1.92"
+version = "0.1.93"
 readme = "README.md"
 description = "Your Personal Assistant in BioImage Analysis."
 dependencies = [
   "schema-agents>=0.1.46",
   "imjoy-rpc>=0.5.48.post2",
   "requests",
   "pypdf",
```

### Comparing `bioimageio-chatbot-0.1.92/tests/test_chatbot.py` & `bioimageio-chatbot-0.1.93/tests/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/tests/test_chatbot_answer.py` & `bioimageio-chatbot-0.1.93/tests/test_chatbot_answer.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.92/tests/test_eval_agent.py` & `bioimageio-chatbot-0.1.93/tests/test_eval_agent.py`

 * *Files identical despite different names*

