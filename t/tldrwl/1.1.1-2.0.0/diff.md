# Comparing `tmp/tldrwl-1.1.1.tar.gz` & `tmp/tldrwl-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldrwl-1.1.1.tar", last modified: Fri May 26 18:49:13 2023, max compression
+gzip compressed data, was "tldrwl-2.0.0.tar", last modified: Mon Apr  8 04:14:35 2024, max compression
```

## Comparing `tldrwl-1.1.1.tar` & `tldrwl-2.0.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.951544 tldrwl-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 18:48:58.000000 tldrwl-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-05-26 18:49:13.951544 tldrwl-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-05-26 18:48:58.000000 tldrwl-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 18:48:58.000000 tldrwl-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 18:49:13.951544 tldrwl-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-26 18:48:58.000000 tldrwl-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.947544 tldrwl-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.947544 tldrwl-1.1.1/tests/manual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/inject_urls_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/super_short_text_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/text_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/webpage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tests/manual/youtube_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.947544 tldrwl-1.1.1/tldrwl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/ai_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.951544 tldrwl-1.1.1/tldrwl/summarizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/summarizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/summarizers/gpt_35_turbo_text_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/summarizers/text_ada_001_text_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/summarizers/text_summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.951544 tldrwl-1.1.1/tldrwl/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/transformers/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/transformers/webpage_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-26 18:48:58.000000 tldrwl-1.1.1/tldrwl/transformers/youtube_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:49:13.951544 tldrwl-1.1.1/tldrwl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-05-26 18:49:13.000000 tldrwl-1.1.1/tldrwl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-26 18:49:13.000000 tldrwl-1.1.1/tldrwl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:49:13.000000 tldrwl-1.1.1/tldrwl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 18:49:13.000000 tldrwl-1.1.1/tldrwl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 18:49:13.000000 tldrwl-1.1.1/tldrwl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:35.805956 tldrwl-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 04:14:31.000000 tldrwl-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-08 04:14:35.805956 tldrwl-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16211 2024-04-08 04:14:31.000000 tldrwl-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 04:14:31.000000 tldrwl-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 04:14:35.805956 tldrwl-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 04:14:31.000000 tldrwl-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:35.801956 tldrwl-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:35.805956 tldrwl-2.0.0/tests/manual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tests/manual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tests/manual/inject_urls_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tests/manual/super_short_text_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tests/manual/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tests/manual/text_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tests/manual/webpage_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tests/manual/youtube_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:35.805956 tldrwl-2.0.0/tldrwl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/ai_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:35.805956 tldrwl-2.0.0/tldrwl/summarizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/summarizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/summarizers/chat_completions_text_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/summarizers/text_summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:35.805956 tldrwl-2.0.0/tldrwl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/transformers/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/transformers/webpage_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-08 04:14:31.000000 tldrwl-2.0.0/tldrwl/transformers/youtube_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:14:35.805956 tldrwl-2.0.0/tldrwl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-08 04:14:35.000000 tldrwl-2.0.0/tldrwl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-08 04:14:35.000000 tldrwl-2.0.0/tldrwl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:14:35.000000 tldrwl-2.0.0/tldrwl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 04:14:35.000000 tldrwl-2.0.0/tldrwl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 04:14:35.000000 tldrwl-2.0.0/tldrwl.egg-info/top_level.txt
```

### Comparing `tldrwl-1.1.1/PKG-INFO` & `tldrwl-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 1.1.1
+Version: 2.0.0
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: openai<2.0.0,>=1.16.2
+Requires-Dist: youtube-transcript-api<0.7.0,>=0.6.0
+Requires-Dist: beautifulsoup4<5.0.0,>=4.12.0
+Requires-Dist: requests<3.0.0,>=2.30.0
+Requires-Dist: aiohttp<4.0.0,>=3.8.0
 
 [![PyPI](https://img.shields.io/pypi/v/tldrwl.svg)](https://pypi.python.org/pypi/tldrwl)
 
 # tldrwl (too long, didn't read/watch/listen)
 
 ## Install
 
@@ -74,17 +79,16 @@
 ## Caveats
 
 - Requires an OpenAI API key
   - Export to env: `export OPENAI_API_KEY="<your api key here>"`
 - Slow
   - Small articles take ~20 seconds, longer articles and videos take a few minutes. There is probably some more optimization to be had.
 - Cost
-  - Can be expensive - by default, this uses the "gpt-3.5-turbo" model, which costs $0.002 / 1000 tokens.
-  - To minimize cost, the library currently limits the number of input characters to 120,000. This limits the cost of a request to a maximum of ~$0.062. In the future, I may add a flag to modify or remove this limit.
-  - If you pass `--cheap` to the command line, the ada model will be used, which is 5x cheaper, but not very good.
+  - Can be expensive - by default, this uses the "gpt-3.5-turbo" model, which is much cheaper than gpt4
+  - To minimize cost, the library currently limits the number of input characters to 120,000.
 
 To illustrate speed and cost: [This wikipedia page](https://en.wikipedia.org/wiki/List_of_common_misconceptions) hits the maximum limit:
 
 ```
 Running async
 Summary(text='The Wikipedia page "List of common misconceptions" provides a comprehensive list of popular misconceptions and myths in various fields, including arts and culture, business, food and cooking, history, science and mathematics, and film and television. The page corrects commonly held false beliefs that arise from old wives\' tales, superstitions, pseudoscience, and fallacies, among others. The page is divided into sections that relate to different areas of knowledge with listed misconceptions and concise corrections. The page is dynamic and can be regularly updated by readers with reliable sources, and encourages people to be critical of information presented to distinguish fact from fiction. The article debunks several popular myths across fields, including the belief that Santa Claus\'s current image was created by The Coca-Cola Company, the association of the term "zombie" with beings from the film Dawn of the Dead, and the myth that Eskimos have a disproportionate number of words for snow. It also clarifies that sign languages are not universal, and each country has its own native sign language, and police officers are allowed to lie during undercover work. The page corrects misconceptions related to religion and history, such as Mary\'s immaculate conception, the paternity of Paul the Apostle, and the belief that the First Council of Nicaea established the books of the Bible. Additionally, the page debunks common historical myths, such as the belief that Christopher Columbus believed in a flat Earth and that the Plymouth Colony settlers wore Puritan attire. The page covers several misconceptions related to biology, evolution and paleontology, including the myth that cockroaches are radiation-resistant and that honey bees are essential to human food production. It also clarifies common misconceptions related to healthcare and nutrition, such as the belief that exercise-induced muscle soreness is caused by lactic acid build-up and that covering the head prevents heat loss more effectively than other body parts. The page concludes by emphasizing the importance of distinguishing fact from fiction and being critical of information presented.', num_tokens=30749, model=<Model.GPT35TURBO: 'gpt-3.5-turbo'>)
 summary.estimated_cost_usd=0.061498000000000004
```

### Comparing `tldrwl-1.1.1/README.md` & `tldrwl-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,16 @@
 ## Caveats
 
 - Requires an OpenAI API key
   - Export to env: `export OPENAI_API_KEY="<your api key here>"`
 - Slow
   - Small articles take ~20 seconds, longer articles and videos take a few minutes. There is probably some more optimization to be had.
 - Cost
-  - Can be expensive - by default, this uses the "gpt-3.5-turbo" model, which costs $0.002 / 1000 tokens.
-  - To minimize cost, the library currently limits the number of input characters to 120,000. This limits the cost of a request to a maximum of ~$0.062. In the future, I may add a flag to modify or remove this limit.
-  - If you pass `--cheap` to the command line, the ada model will be used, which is 5x cheaper, but not very good.
+  - Can be expensive - by default, this uses the "gpt-3.5-turbo" model, which is much cheaper than gpt4
+  - To minimize cost, the library currently limits the number of input characters to 120,000.
 
 To illustrate speed and cost: [This wikipedia page](https://en.wikipedia.org/wiki/List_of_common_misconceptions) hits the maximum limit:
 
 ```
 Running async
 Summary(text='The Wikipedia page "List of common misconceptions" provides a comprehensive list of popular misconceptions and myths in various fields, including arts and culture, business, food and cooking, history, science and mathematics, and film and television. The page corrects commonly held false beliefs that arise from old wives\' tales, superstitions, pseudoscience, and fallacies, among others. The page is divided into sections that relate to different areas of knowledge with listed misconceptions and concise corrections. The page is dynamic and can be regularly updated by readers with reliable sources, and encourages people to be critical of information presented to distinguish fact from fiction. The article debunks several popular myths across fields, including the belief that Santa Claus\'s current image was created by The Coca-Cola Company, the association of the term "zombie" with beings from the film Dawn of the Dead, and the myth that Eskimos have a disproportionate number of words for snow. It also clarifies that sign languages are not universal, and each country has its own native sign language, and police officers are allowed to lie during undercover work. The page corrects misconceptions related to religion and history, such as Mary\'s immaculate conception, the paternity of Paul the Apostle, and the belief that the First Council of Nicaea established the books of the Bible. Additionally, the page debunks common historical myths, such as the belief that Christopher Columbus believed in a flat Earth and that the Plymouth Colony settlers wore Puritan attire. The page covers several misconceptions related to biology, evolution and paleontology, including the myth that cockroaches are radiation-resistant and that honey bees are essential to human food production. It also clarifies common misconceptions related to healthcare and nutrition, such as the belief that exercise-induced muscle soreness is caused by lactic acid build-up and that covering the head prevents heat loss more effectively than other body parts. The page concludes by emphasizing the importance of distinguishing fact from fiction and being critical of information presented.', num_tokens=30749, model=<Model.GPT35TURBO: 'gpt-3.5-turbo'>)
 summary.estimated_cost_usd=0.061498000000000004
```

### Comparing `tldrwl-1.1.1/setup.py` & `tldrwl-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="tldrwl",
-    version="1.1.1",
+    version="2.0.0",
     author="Jacob Rodal",
     author_email="dev@jrodal.com",
     description="Too long, didn't read/watch/listen",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrodal98/tldrwl",
     packages=setuptools.find_packages(),
```

### Comparing `tldrwl-1.1.1/tests/manual/test_helper.py` & `tldrwl-2.0.0/tests/manual/test_helper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 #!/usr/bin/env python3
 # www.jrodal.com
 
 import time
-import sys
 import asyncio
 from tldrwl.logger import init_logging
 from tldrwl.summarize import Summarizer
-from tldrwl.summarizers.text_ada_001_text_summarizer import TextAda001TextSummarizer
+from tldrwl.summarizers.chat_completions_text_summarizer import (
+    ChatCompletionsTextSummarizer,
+)
 
 
 def main_sync(text: str) -> None:
     print("Sync test")
     start = time.time()
-    if "cheap" in sys.argv:
-        text_summarizer = TextAda001TextSummarizer()
-    else:
-        text_summarizer = None
+    text_summarizer = ChatCompletionsTextSummarizer()
 
     summary = Summarizer(text_summarizer=text_summarizer).summarize_sync(text)
     end = time.time()
 
     print(summary)
     print(f"{summary.estimated_cost_usd=}")
     print(f"runtime: {end - start:.4f}s")
 
 
 async def main_async(text: str) -> None:
     print("Async test")
     start = time.time()
-    if "cheap" in sys.argv:
-        text_summarizer = TextAda001TextSummarizer()
-    else:
-        text_summarizer = None
+    text_summarizer = ChatCompletionsTextSummarizer()
     summary = await Summarizer(text_summarizer=text_summarizer).summarize_async(text)
     end = time.time()
 
     print(summary)
     print(f"{summary.estimated_cost_usd=}")
     print(f"runtime: {end - start:.4f}s")
```

### Comparing `tldrwl-1.1.1/tests/manual/text_test.py` & `tldrwl-2.0.0/tests/manual/text_test.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.1/tldrwl/__main__.py` & `tldrwl-2.0.0/tldrwl/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # www.jrodal.com
 
 import argparse
 import asyncio
 
 from tldrwl.summarize import Summarizer
 from tldrwl.logger import init_logging
-from tldrwl.summarizers.text_ada_001_text_summarizer import (
-    TextAda001TextSummarizer,
+from tldrwl.summarizers.chat_completions_text_summarizer import (
+    ChatCompletionsTextSummarizer,
 )
+from tldrwl.ai_interface import Model
 
 
 async def main():
     parser = argparse.ArgumentParser(description="Input (Text or URL to summarize)")
     parser.add_argument("input", type=str, help="Input (Text or URL to summarize)")
     parser.add_argument(
         "--disable-logging", action="store_true", help="Turn logging off"
@@ -22,30 +23,29 @@
     )
     parser.add_argument(
         "--very-verbose-logging",
         action="store_true",
         help="very verbose logging (include third party logs)",
     )
     parser.add_argument(
-        "--cheap",
-        action="store_true",
-        help="Try to make the run cheaper (e.g. using less powerful models like Ada)",
+        "--model",
+        type=Model,
+        choices=list(Model),
+        default=None,
+        help="Model to use for summarization",
     )
     args = parser.parse_args()
 
     init_logging(
         disable_logging=args.disable_logging,
         verbose_logging=args.verbose_logging,
         very_verbose_logging=args.very_verbose_logging,
     )
 
-    if args.cheap:
-        text_summarizer = TextAda001TextSummarizer()
-    else:
-        text_summarizer = None
+    text_summarizer = ChatCompletionsTextSummarizer(model=args.model)
 
     summary = await Summarizer(text_summarizer=text_summarizer).summarize_async(
         args.input
     )
     print(f"Summary: {summary.text}")
     print(f"Estimated cost (usd): ${summary.estimated_cost_usd:.4f}")
```

### Comparing `tldrwl-1.1.1/tldrwl/ai_interface.py` & `tldrwl-2.0.0/tldrwl/ai_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,35 +8,52 @@
 
 from tldrwl.exception import TldrwlAsyncioRunInEventLoop, TldrwlException
 from tldrwl.register import Register
 
 
 class Model(Enum):
     GPT35TURBO = "gpt-3.5-turbo"
-    TEXTADA001 = "text-ada-001"
+    GPT4 = "gpt-4"
 
     @property
-    def cost_per_1000_tokens(self) -> float:
+    def cost_per_1000_prompt_tokens(self) -> float:
         if self is self.GPT35TURBO:
-            return 0.002
-        if self is self.TEXTADA001:
-            return 0.0004
+            return 0.0005
+        elif self is self.GPT4:
+            return 0.03
         else:
             return 0
 
+    @property
+    def cost_per_1000_completion_tokens(self) -> float:
+        if self is self.GPT35TURBO:
+            return 0.0015
+        elif self is self.GPT4:
+            return 0.06
+        else:
+            return 0
+
+    @classmethod
+    def default_model(cls) -> "Model":
+        return cls.GPT35TURBO
+
 
 @dataclass
 class Summary:
     text: str
-    num_tokens: int
+    prompt_tokens: int
+    completion_tokens: int
     model: Model
 
     @property
     def estimated_cost_usd(self) -> float:
-        return self.num_tokens * self.model.cost_per_1000_tokens * (1 / 1000)
+        return (
+            (self.prompt_tokens * self.model.cost_per_1000_prompt_tokens)
+            + (self.completion_tokens * self.model.cost_per_1000_completion_tokens)
+        ) * (1 / 1000)
 
 
 class AiInterface(ABC):
     @abstractmethod
     async def _summarize_async(self, text: str) -> Summary:
         pass
```

### Comparing `tldrwl-1.1.1/tldrwl/exception.py` & `tldrwl-2.0.0/tldrwl/exception.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.1/tldrwl/logger.py` & `tldrwl-2.0.0/tldrwl/logger.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.1/tldrwl/register.py` & `tldrwl-2.0.0/tldrwl/register.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.1/tldrwl/summarize.py` & `tldrwl-2.0.0/tldrwl/summarize.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 import logging
 import asyncio
 
 from typing import Optional
 
 from tldrwl.ai_interface import AiInterface, Summary
 from tldrwl.summarizers.text_summarizer import TextSummarizer
-from tldrwl.summarizers.gpt_35_turbo_text_summarizer import Gpt35TurboTextSummarizer
+from tldrwl.summarizers.chat_completions_text_summarizer import ChatCompletionsTextSummarizer
 from tldrwl.transformers.webpage_transformer import WebpageTransformer
 from tldrwl.transformers.youtube_transformer import YoutubeTransformer
 
 
 class Summarizer(AiInterface):
     def __init__(self, *, text_summarizer: Optional[TextSummarizer] = None) -> None:
         super().__init__()
         self._logger = logging.getLogger(__name__)
-        self._summarizer = text_summarizer or Gpt35TurboTextSummarizer()
+        self._summarizer = text_summarizer or ChatCompletionsTextSummarizer()
 
     async def _transform_text(self, text: str) -> str:
         if YoutubeTransformer.is_youtube_url(text):
             self._logger.debug(f"Using YoutubeSummarizer on {text}")
             return await YoutubeTransformer(text).get_text()
         elif WebpageTransformer.is_url(text):
             self._logger.debug(f"Using WebpageSummarizer on {text}")
```

### Comparing `tldrwl-1.1.1/tldrwl/summarizers/text_summarizer.py` & `tldrwl-2.0.0/tldrwl/summarizers/text_summarizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,35 +16,35 @@
 class TextSummarizer(AiInterface):
     MAX_TOKEN_RESPONSE: int = 1500
     MAX_TOKEN_INPUT: int = 250
 
     def __init__(
         self,
         *,
-        model: Model = Model.GPT35TURBO,
+        model: Model | None = None,
         prompt_string: str = "Write a detailed summary of the following:\n\n{}\n",
         chunk_size: int = 12000,
         max_num_chunks: int = 10,
     ) -> None:
         super().__init__()
-        self._model = model
+        self._model = model or Model.default_model()
         self._prompt_string = prompt_string
         self._chunk_size = chunk_size
         self._max_num_chunks = max_num_chunks
         self._logger = logging.getLogger(__name__)
 
     @abstractmethod
     async def _query_openai(self, text: str, max_tokens: int) -> Summary:
         pass
 
     async def _summarize_chunk_async(self, chunk: str, max_tokens: int) -> Summary:
         for _ in range(0, 3):
             try:
                 return await self._query_openai(chunk, max_tokens)
-            except openai.error.RateLimitError:  # pyright: ignore
+            except openai.RateLimitError:  # pyright: ignore
                 retry_interval = 3
                 self._logger.debug(
                     f"Rate limited by openai - resting for {retry_interval}s"
                 )
                 await asyncio.sleep(retry_interval)
 
         raise TldrwlRateLimitError.make_error("Rate limited after 3 attempts")
@@ -81,11 +81,13 @@
             # of hoping that this will work - maybe catch this exception?
             # noqa openai.error.InvalidRequestError: This model's maximum context length is 4097 tokens. However, you requested 4612 tokens (3112 in the messages, 1500 in the completion). Please reduce the length of the messages or completion.
             final_summary = await self._summarize_chunk_async(
                 final_input, max_tokens=self.MAX_TOKEN_RESPONSE
             )
             return Summary(
                 text=final_summary.text,
-                num_tokens=final_summary.num_tokens
-                + sum(s.num_tokens for s in summaries),
+                prompt_tokens=final_summary.prompt_tokens
+                + sum(s.prompt_tokens for s in summaries),
+                completion_tokens=final_summary.completion_tokens
+                + sum(s.completion_tokens for s in summaries),
                 model=self._model,
             )
```

### Comparing `tldrwl-1.1.1/tldrwl/transformers/webpage_transformer.py` & `tldrwl-2.0.0/tldrwl/transformers/webpage_transformer.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.1/tldrwl/transformers/youtube_transformer.py` & `tldrwl-2.0.0/tldrwl/transformers/youtube_transformer.py`

 * *Files identical despite different names*

### Comparing `tldrwl-1.1.1/tldrwl.egg-info/PKG-INFO` & `tldrwl-2.0.0/tldrwl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 1.1.1
+Version: 2.0.0
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: openai<2.0.0,>=1.16.2
+Requires-Dist: youtube-transcript-api<0.7.0,>=0.6.0
+Requires-Dist: beautifulsoup4<5.0.0,>=4.12.0
+Requires-Dist: requests<3.0.0,>=2.30.0
+Requires-Dist: aiohttp<4.0.0,>=3.8.0
 
 [![PyPI](https://img.shields.io/pypi/v/tldrwl.svg)](https://pypi.python.org/pypi/tldrwl)
 
 # tldrwl (too long, didn't read/watch/listen)
 
 ## Install
 
@@ -74,17 +79,16 @@
 ## Caveats
 
 - Requires an OpenAI API key
   - Export to env: `export OPENAI_API_KEY="<your api key here>"`
 - Slow
   - Small articles take ~20 seconds, longer articles and videos take a few minutes. There is probably some more optimization to be had.
 - Cost
-  - Can be expensive - by default, this uses the "gpt-3.5-turbo" model, which costs $0.002 / 1000 tokens.
-  - To minimize cost, the library currently limits the number of input characters to 120,000. This limits the cost of a request to a maximum of ~$0.062. In the future, I may add a flag to modify or remove this limit.
-  - If you pass `--cheap` to the command line, the ada model will be used, which is 5x cheaper, but not very good.
+  - Can be expensive - by default, this uses the "gpt-3.5-turbo" model, which is much cheaper than gpt4
+  - To minimize cost, the library currently limits the number of input characters to 120,000.
 
 To illustrate speed and cost: [This wikipedia page](https://en.wikipedia.org/wiki/List_of_common_misconceptions) hits the maximum limit:
 
 ```
 Running async
 Summary(text='The Wikipedia page "List of common misconceptions" provides a comprehensive list of popular misconceptions and myths in various fields, including arts and culture, business, food and cooking, history, science and mathematics, and film and television. The page corrects commonly held false beliefs that arise from old wives\' tales, superstitions, pseudoscience, and fallacies, among others. The page is divided into sections that relate to different areas of knowledge with listed misconceptions and concise corrections. The page is dynamic and can be regularly updated by readers with reliable sources, and encourages people to be critical of information presented to distinguish fact from fiction. The article debunks several popular myths across fields, including the belief that Santa Claus\'s current image was created by The Coca-Cola Company, the association of the term "zombie" with beings from the film Dawn of the Dead, and the myth that Eskimos have a disproportionate number of words for snow. It also clarifies that sign languages are not universal, and each country has its own native sign language, and police officers are allowed to lie during undercover work. The page corrects misconceptions related to religion and history, such as Mary\'s immaculate conception, the paternity of Paul the Apostle, and the belief that the First Council of Nicaea established the books of the Bible. Additionally, the page debunks common historical myths, such as the belief that Christopher Columbus believed in a flat Earth and that the Plymouth Colony settlers wore Puritan attire. The page covers several misconceptions related to biology, evolution and paleontology, including the myth that cockroaches are radiation-resistant and that honey bees are essential to human food production. It also clarifies common misconceptions related to healthcare and nutrition, such as the belief that exercise-induced muscle soreness is caused by lactic acid build-up and that covering the head prevents heat loss more effectively than other body parts. The page concludes by emphasizing the importance of distinguishing fact from fiction and being critical of information presented.', num_tokens=30749, model=<Model.GPT35TURBO: 'gpt-3.5-turbo'>)
 summary.estimated_cost_usd=0.061498000000000004
```

### Comparing `tldrwl-1.1.1/tldrwl.egg-info/SOURCES.txt` & `tldrwl-2.0.0/tldrwl.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,13 @@
 tldrwl/summarize.py
 tldrwl.egg-info/PKG-INFO
 tldrwl.egg-info/SOURCES.txt
 tldrwl.egg-info/dependency_links.txt
 tldrwl.egg-info/requires.txt
 tldrwl.egg-info/top_level.txt
 tldrwl/summarizers/__init__.py
-tldrwl/summarizers/gpt_35_turbo_text_summarizer.py
-tldrwl/summarizers/text_ada_001_text_summarizer.py
+tldrwl/summarizers/chat_completions_text_summarizer.py
 tldrwl/summarizers/text_summarizer.py
 tldrwl/transformers/__init__.py
 tldrwl/transformers/transformer.py
 tldrwl/transformers/webpage_transformer.py
 tldrwl/transformers/youtube_transformer.py
```

