# Comparing `tmp/microchain-python-0.3.4.tar.gz` & `tmp/microchain-python-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microchain-python-0.3.4.tar", last modified: Wed Mar 27 11:38:03 2024, max compression
+gzip compressed data, was "microchain-python-0.3.5.tar", last modified: Mon Apr  8 09:34:07 2024, max compression
```

## Comparing `microchain-python-0.3.4.tar` & `microchain-python-0.3.5.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:38:03.763333 microchain-python-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-03-27 11:38:00.000000 microchain-python-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-03-27 11:38:03.763333 microchain-python-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-03-27 11:38:00.000000 microchain-python-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:38:03.759333 microchain-python-0.3.4/microchain/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-27 11:38:00.000000 microchain-python-0.3.4/microchain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:38:03.763333 microchain-python-0.3.4/microchain/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 11:38:00.000000 microchain-python-0.3.4/microchain/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-03-27 11:38:00.000000 microchain-python-0.3.4/microchain/engine/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-03-27 11:38:00.000000 microchain-python-0.3.4/microchain/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-27 11:38:00.000000 microchain-python-0.3.4/microchain/engine/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-27 11:38:00.000000 microchain-python-0.3.4/microchain/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:38:03.763333 microchain-python-0.3.4/microchain/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 11:38:00.000000 microchain-python-0.3.4/microchain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-03-27 11:38:00.000000 microchain-python-0.3.4/microchain/models/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-27 11:38:00.000000 microchain-python-0.3.4/microchain/models/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-27 11:38:00.000000 microchain-python-0.3.4/microchain/models/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:38:03.763333 microchain-python-0.3.4/microchain_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-03-27 11:38:03.000000 microchain-python-0.3.4/microchain_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-27 11:38:03.000000 microchain-python-0.3.4/microchain_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 11:38:03.000000 microchain-python-0.3.4/microchain_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-27 11:38:03.000000 microchain-python-0.3.4/microchain_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-27 11:38:03.000000 microchain-python-0.3.4/microchain_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 11:38:03.763333 microchain-python-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-27 11:38:00.000000 microchain-python-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.260300 microchain-python-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-08 09:33:54.000000 microchain-python-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-08 09:34:07.260300 microchain-python-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-08 09:33:54.000000 microchain-python-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.256300 microchain-python-0.3.5/microchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.256300 microchain-python-0.3.5/microchain/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/engine/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/engine/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.256300 microchain-python-0.3.5/microchain/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/models/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/models/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/models/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.256300 microchain-python-0.3.5/microchain_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-08 09:34:07.000000 microchain-python-0.3.5/microchain_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 09:34:07.000000 microchain-python-0.3.5/microchain_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:34:07.000000 microchain-python-0.3.5/microchain_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 09:34:07.000000 microchain-python-0.3.5/microchain_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 09:34:07.000000 microchain-python-0.3.5/microchain_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:34:07.260300 microchain-python-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-08 09:33:54.000000 microchain-python-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.256300 microchain-python-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-08 09:33:54.000000 microchain-python-0.3.5/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-08 09:33:54.000000 microchain-python-0.3.5/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 09:33:54.000000 microchain-python-0.3.5/tests/test_openai.py
```

### Comparing `microchain-python-0.3.4/LICENSE` & `microchain-python-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.4/PKG-INFO` & `microchain-python-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microchain-python
-Version: 0.3.4
+Version: 0.3.5
 Home-page: 
 Author: Federico A. Galatolo
 Author-email: federico.galatolo@unipi.it
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microchain-python-0.3.4/README.md` & `microchain-python-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.4/microchain/engine/agent.py` & `microchain-python-0.3.5/microchain/engine/agent.py`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.4/microchain/engine/engine.py` & `microchain-python-0.3.5/microchain/engine/engine.py`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.4/microchain/engine/function.py` & `microchain-python-0.3.5/microchain/engine/function.py`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.4/microchain/functions.py` & `microchain-python-0.3.5/microchain/functions.py`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.4/microchain/models/generators.py` & `microchain-python-0.3.5/microchain/models/generators.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,27 +18,28 @@
         self.client = openai.OpenAI(
             api_key=self.api_key,
             base_url=self.api_base
         )
     
     def __call__(self, messages, stop=None):
         import openai
+        oai_error = openai.error.OpenAIError if hasattr(openai, "error") else openai.OpenAIError
         assert isinstance(messages, list), "messages must be a list of messages https://platform.openai.com/docs/guides/text-generation/chat-completions-api"
 
         try:
             response = self.client.chat.completions.create(
                 model=self.model,
                 messages=messages,
                 temperature=self.temperature,
                 max_tokens=self.max_tokens,
                 top_p=self.top_p,
                 stop=stop,
                 timeout=self.timeout
             )
-        except openai.error.OpenAIError as e:
+        except oai_error as e:
             print(colored(f"Error: {e}", "red"))
             return "Error: timeout"
         
         output = response.choices[0].message.content.strip()
 
         return output
     
@@ -61,26 +62,27 @@
         self.client = openai.OpenAI(
             api_key=self.api_key,
             base_url=self.api_base
         )
     
     def __call__(self, prompt, stop=None):
         import openai
+        oai_error = openai.error.OpenAIError if hasattr(openai, "error") else openai.OpenAIError
         assert isinstance(prompt, str), "prompt must be a string https://platform.openai.com/docs/guides/text-generation/chat-completions-api"
 
         try:
             response = self.client.completions.create(
                 model=self.model,
                 prompt=prompt,
                 temperature=self.temperature,
                 max_tokens=self.max_tokens,
                 top_p=self.top_p,
                 stop=stop
             )
-        except openai.error.OpenAIError as e:
+        except oai_error as e:
             print(colored(f"Error: {e}", "red"))
             return "Error: timeout"
         
         output = response.choices[0].text.strip()
 
         return output
```

### Comparing `microchain-python-0.3.4/microchain/models/templates.py` & `microchain-python-0.3.5/microchain/models/templates.py`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.4/microchain_python.egg-info/PKG-INFO` & `microchain-python-0.3.5/microchain_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microchain-python
-Version: 0.3.4
+Version: 0.3.5
 Home-page: 
 Author: Federico A. Galatolo
 Author-email: federico.galatolo@unipi.it
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microchain-python-0.3.4/setup.py` & `microchain-python-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), "README.md"), "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="microchain-python",
-    version="0.3.4",
+    version="0.3.5",
     author="Federico A. Galatolo",
     author_email="federico.galatolo@unipi.it",
     description="",
     url="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["microchain", "microchain.models", "microchain.engine"],
```

