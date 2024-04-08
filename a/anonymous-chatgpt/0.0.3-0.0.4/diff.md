# Comparing `tmp/anonymous-chatgpt-0.0.3.tar.gz` & `tmp/anonymous-chatgpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anonymous-chatgpt-0.0.3.tar", last modified: Sun Apr  7 14:59:48 2024, max compression
+gzip compressed data, was "anonymous-chatgpt-0.0.4.tar", last modified: Mon Apr  8 18:20:38 2024, max compression
```

## Comparing `anonymous-chatgpt-0.0.3.tar` & `anonymous-chatgpt-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2024-04-07 14:59:48.123327 anonymous-chatgpt-0.0.3/
--rw-rw-r--   0 meet      (1000) meet      (1000)     1890 2024-04-07 14:59:48.123327 anonymous-chatgpt-0.0.3/PKG-INFO
--rw-r--r--   0 meet      (1000) meet      (1000)     1541 2024-04-06 16:23:35.000000 anonymous-chatgpt-0.0.3/README.md
-drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2024-04-07 14:59:48.123327 anonymous-chatgpt-0.0.3/anonymous_chatgpt/
--rw-rw-r--   0 meet      (1000) meet      (1000)       19 2024-04-06 16:17:19.000000 anonymous-chatgpt-0.0.3/anonymous_chatgpt/__init__.py
--rw-r--r--   0 meet      (1000) meet      (1000)       58 2024-04-07 14:56:38.000000 anonymous-chatgpt-0.0.3/anonymous_chatgpt/__main__.py
--rw-rw-r--   0 meet      (1000) meet      (1000)     5599 2024-04-07 14:56:32.000000 anonymous-chatgpt-0.0.3/anonymous_chatgpt/app.py
-drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2024-04-07 14:59:48.123327 anonymous-chatgpt-0.0.3/anonymous_chatgpt.egg-info/
--rw-rw-r--   0 meet      (1000) meet      (1000)     1890 2024-04-07 14:59:48.000000 anonymous-chatgpt-0.0.3/anonymous_chatgpt.egg-info/PKG-INFO
--rw-rw-r--   0 meet      (1000) meet      (1000)      351 2024-04-07 14:59:48.000000 anonymous-chatgpt-0.0.3/anonymous_chatgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)        1 2024-04-07 14:59:48.000000 anonymous-chatgpt-0.0.3/anonymous_chatgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)       56 2024-04-07 14:59:48.000000 anonymous-chatgpt-0.0.3/anonymous_chatgpt.egg-info/entry_points.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)        9 2024-04-07 14:59:48.000000 anonymous-chatgpt-0.0.3/anonymous_chatgpt.egg-info/requires.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)       18 2024-04-07 14:59:48.000000 anonymous-chatgpt-0.0.3/anonymous_chatgpt.egg-info/top_level.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)       38 2024-04-07 14:59:48.123327 anonymous-chatgpt-0.0.3/setup.cfg
--rw-r--r--   0 meet      (1000) meet      (1000)      892 2024-04-07 14:58:51.000000 anonymous-chatgpt-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:20:38.941116 anonymous-chatgpt-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-08 18:20:38.941116 anonymous-chatgpt-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-08 18:20:34.000000 anonymous-chatgpt-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:20:38.941116 anonymous-chatgpt-0.0.4/anonymous_chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 18:20:34.000000 anonymous-chatgpt-0.0.4/anonymous_chatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 18:20:34.000000 anonymous-chatgpt-0.0.4/anonymous_chatgpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-08 18:20:34.000000 anonymous-chatgpt-0.0.4/anonymous_chatgpt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:20:38.941116 anonymous-chatgpt-0.0.4/anonymous_chatgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-08 18:20:38.000000 anonymous-chatgpt-0.0.4/anonymous_chatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-08 18:20:38.000000 anonymous-chatgpt-0.0.4/anonymous_chatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:20:38.000000 anonymous-chatgpt-0.0.4/anonymous_chatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 18:20:38.000000 anonymous-chatgpt-0.0.4/anonymous_chatgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 18:20:38.000000 anonymous-chatgpt-0.0.4/anonymous_chatgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 18:20:38.000000 anonymous-chatgpt-0.0.4/anonymous_chatgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:20:38.941116 anonymous-chatgpt-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-08 18:20:34.000000 anonymous-chatgpt-0.0.4/setup.py
```

### Comparing `anonymous-chatgpt-0.0.3/PKG-INFO` & `anonymous-chatgpt-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: anonymous-chatgpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Client to interact with OpenAI's ChatGPT(GPT-3) model without authentication
 Home-page: https://github.com/Mr-Destructive/anonymous-chatgpt
 Author: Meet Gor
 Author-email: gormeet711@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: requests
 
 # Anonymous ChatGPT Client 
 
 - Access basic ChatGPT model without authentication
 
 OpenAI recently made the ChatGPT model accessible anonymously. You can access it without authentication.
 Read more about it in the [official docs](https://openai.com/blog/start-using-chatgpt-instantly)
@@ -26,37 +25,47 @@
 
 ## Usage
 
 ### CLI
 
 ```bash
 chatgpt --prompt "hello world"
+
+OR 
+
+chatgpt --chat
 ```
 
+
 #### CLI Demonstration
 
 ![Anonymous ChatGPT Demo](https://meetgor-cdn.pages.dev/anonymous-chatgpt-demo.gif)
 
 ### Package
 
-```bash
-from anonymous_chatgpt import chat
+```python
+from anonymous_chatgpt import chat_prompt, ChatGPT
 
 
-message = chat(prompt="hello world")
+message = chat_promt(prompt="hello world")
 print(message)
+
+# For chat
+
+chatgpt = ChatGPT()
+
+resp1 = chatgpt.chat(prompt="hello, my name is John")
+resp2 = chatgpt.chat(prompt="what is my name?")
 ```
 
 
 ## Process of creating a authentication-less client
 
 1. Send the first request to the ChatGPT API i.e. `chat.openai.com`
 2. The response of that request has cookies for authentication(not user just user-agent and csrf tokens)
 3. Those cookies are carried in all the upcoming requests
 4. Send the second request to the [Sential API](https://techcommunity.microsoft.com/t5/manufacturing/introduction-to-openai-and-microsoft-sentinel/ba-p/3761907) i.e. `/backend-anon/sentinel/chat-requirements`
 5. This request gives us the `sentinel-token` which is the token used for authentication and authorization of the requests (not users).
 6. We use this token in all the subsequent requests
 7. The third request is the actual request to the **Anonymous Conversation** endpoint i.e. `/backend-anon/conversation`
 8. This is a streamed request which returns the response in the form of chunks
 
-
-
```

### Comparing `anonymous-chatgpt-0.0.3/README.md` & `anonymous-chatgpt-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,40 @@
 
 ## Usage
 
 ### CLI
 
 ```bash
 chatgpt --prompt "hello world"
+
+OR 
+
+chatgpt --chat
 ```
 
+
 #### CLI Demonstration
 
 ![Anonymous ChatGPT Demo](https://meetgor-cdn.pages.dev/anonymous-chatgpt-demo.gif)
 
 ### Package
 
-```bash
-from anonymous_chatgpt import chat
+```python
+from anonymous_chatgpt import chat_prompt, ChatGPT
 
 
-message = chat(prompt="hello world")
+message = chat_promt(prompt="hello world")
 print(message)
+
+# For chat
+
+chatgpt = ChatGPT()
+
+resp1 = chatgpt.chat(prompt="hello, my name is John")
+resp2 = chatgpt.chat(prompt="what is my name?")
 ```
 
 
 ## Process of creating a authentication-less client
 
 1. Send the first request to the ChatGPT API i.e. `chat.openai.com`
 2. The response of that request has cookies for authentication(not user just user-agent and csrf tokens)
```

### Comparing `anonymous-chatgpt-0.0.3/anonymous_chatgpt/app.py` & `anonymous-chatgpt-0.0.4/anonymous_chatgpt/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         resp = json.loads(msgs[-2])
         messages = resp.get("message", {}).get("content", {}).get("parts", [])
         if len(messages) > 0:
             resp_message["message"] = messages[0]
     return resp_message
 
 
-def chat():
+def chat_cli():
     parent_id = str(uuid.uuid4())
     msg_id = str(uuid.uuid4())
     prompt = input("user >> ")
     data = {
         "action": "next",
         "messages": [
             {
@@ -140,33 +140,87 @@
             response.raise_for_status()
         resp = response.text
         msgs = resp.split("\ndata:")
         if len(msgs) > 1:
             resp = json.loads(msgs[-2])
             messages = resp.get("message", {}).get("content", {}).get("parts", [])
             if len(messages) > 0:
-                print("bot >> ", messages[0])
+                print("chatgpt >> ", messages[0])
                 data.get("messages",[]).append(
                     {
                         "id": str(uuid.uuid4()),
                         "author": {"role": "assistant"},
                         "content": {"content_type": "text", "parts": [messages[0]]},
                         "metadata": {},
                     }
                 )
             prompt = input("user >> ")
 
+class ChatGPT:
+    def __init__(self):
+        self.parent_id = str(uuid.uuid4())
+        self.msg_id = str(uuid.uuid4())
+        self.base_conversation_config = {
+            "action": "next",
+            "messages": [
+                {
+                    "id": f"{self.msg_id}",
+                    "author": {"role": "user"},
+                    "content": {"content_type": "text", "parts": []},
+                    "metadata": {},
+                }
+            ],
+            "parent_message_id": f"{self.parent_id}",
+            "model": "text-davinci-002-render-sha",
+            "timezone_offset_min": -330,
+            "history_and_training_disabled": True,
+            "conversation_mode": {"kind": "primary_assistant"},
+            "force_paragen": False,
+            "force_paragen_model_slug": "",
+            "force_nulligen": False,
+            "force_rate_limit": False,
+        }
+        self.conversation = self.base_conversation_config
+
+    def chat(self, prompt):
+        self.prompt_message = prompt
+        data = self.conversation
+        messages = data.get("messages", [])
+        if messages:
+            messages[0].get("content", {}).get("parts", []).append(prompt)
+        self.conversation = data
+        request_client, headers = prepare_chat_request()
+        url = f"{BASE_URL}/backend-anon/conversation"
+
+        response = request_client.post(url, headers=headers, json=self.conversation)
+        if response.status_code != 200:
+            response.raise_for_status()
+        resp = response.text
+        msgs = resp.split("\ndata:")
+        if len(msgs) > 1:
+            resp = json.loads(msgs[-2])
+            messages = resp.get("message", {}).get("content", {}).get("parts", [])
+            if len(messages) > 0:
+                self.conversation.get("messages",[]).append(
+                    {
+                        "id": str(uuid.uuid4()),
+                        "author": {"role": "assistant"},
+                        "content": {"content_type": "text", "parts": [messages[0]]},
+                        "metadata": {},
+                    }
+                )
+                return messages[0]
 
 def main():
     args = argparse.ArgumentParser()
     args.add_argument("--prompt", type=str)
     args.add_argument("--chat", action="store_true")
     args = args.parse_args()
     prompt = args.prompt
     if args.chat:
-        chat()
+        chat_cli()
     else:
         response = chat_prompt(prompt)
         print(response)
 
 if __name__ == "__main__":
     main()
```

### Comparing `anonymous-chatgpt-0.0.3/anonymous_chatgpt.egg-info/PKG-INFO` & `anonymous-chatgpt-0.0.4/anonymous_chatgpt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: anonymous-chatgpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Client to interact with OpenAI's ChatGPT(GPT-3) model without authentication
 Home-page: https://github.com/Mr-Destructive/anonymous-chatgpt
 Author: Meet Gor
 Author-email: gormeet711@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: requests
 
 # Anonymous ChatGPT Client 
 
 - Access basic ChatGPT model without authentication
 
 OpenAI recently made the ChatGPT model accessible anonymously. You can access it without authentication.
 Read more about it in the [official docs](https://openai.com/blog/start-using-chatgpt-instantly)
@@ -26,37 +25,47 @@
 
 ## Usage
 
 ### CLI
 
 ```bash
 chatgpt --prompt "hello world"
+
+OR 
+
+chatgpt --chat
 ```
 
+
 #### CLI Demonstration
 
 ![Anonymous ChatGPT Demo](https://meetgor-cdn.pages.dev/anonymous-chatgpt-demo.gif)
 
 ### Package
 
-```bash
-from anonymous_chatgpt import chat
+```python
+from anonymous_chatgpt import chat_prompt, ChatGPT
 
 
-message = chat(prompt="hello world")
+message = chat_promt(prompt="hello world")
 print(message)
+
+# For chat
+
+chatgpt = ChatGPT()
+
+resp1 = chatgpt.chat(prompt="hello, my name is John")
+resp2 = chatgpt.chat(prompt="what is my name?")
 ```
 
 
 ## Process of creating a authentication-less client
 
 1. Send the first request to the ChatGPT API i.e. `chat.openai.com`
 2. The response of that request has cookies for authentication(not user just user-agent and csrf tokens)
 3. Those cookies are carried in all the upcoming requests
 4. Send the second request to the [Sential API](https://techcommunity.microsoft.com/t5/manufacturing/introduction-to-openai-and-microsoft-sentinel/ba-p/3761907) i.e. `/backend-anon/sentinel/chat-requirements`
 5. This request gives us the `sentinel-token` which is the token used for authentication and authorization of the requests (not users).
 6. We use this token in all the subsequent requests
 7. The third request is the actual request to the **Anonymous Conversation** endpoint i.e. `/backend-anon/conversation`
 8. This is a streamed request which returns the response in the form of chunks
 
-
-
```

### Comparing `anonymous-chatgpt-0.0.3/setup.py` & `anonymous-chatgpt-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 PACKAGE_NAME = "anonymous-chatgpt"
 AUTHOR = "Meet Gor"
 AUTHOR_EMAIL = "gormeet711@gmail.com"
 URL = "https://github.com/Mr-Destructive/anonymous-chatgpt"
 
 DESCRIPTION = (
     "A Python Client to interact with OpenAI's ChatGPT(GPT-3) model without authentication"
```

