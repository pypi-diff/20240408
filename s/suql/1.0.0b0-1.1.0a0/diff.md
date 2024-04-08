# Comparing `tmp/suql-1.0.0b0.tar.gz` & `tmp/suql-1.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.0.0b0.tar", last modified: Fri Apr  5 23:43:51 2024, max compression
+gzip compressed data, was "suql-1.1.0a0.tar", last modified: Mon Apr  8 18:27:27 2024, max compression
```

## Comparing `suql-1.0.0b0.tar` & `suql-1.1.0a0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-04-05 23:43:51.804317 suql-1.0.0b0/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.0.0b0/LICENSE
--rw-------   0 oval      (1000) users      (100)     4616 2024-04-05 23:43:51.804317 suql-1.0.0b0/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4162 2024-04-05 23:43:18.000000 suql-1.0.0b0/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-04-05 23:43:51.804317 suql-1.0.0b0/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1423 2024-04-05 23:43:25.000000 suql-1.0.0b0/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-05 23:43:51.780317 suql-1.0.0b0/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-04-05 23:43:51.784317 suql-1.0.0b0/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17330 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    16980 2024-04-05 23:43:18.000000 suql-1.0.0b0/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     7895 2024-04-05 17:58:35.000000 suql-1.0.0b0/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     4095 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)    12070 2024-04-05 18:02:21.000000 suql-1.0.0b0/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-05 23:43:51.800317 suql-1.0.0b0/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.0.0b0/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-04-05 23:43:51.804317 suql-1.0.0b0/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.0.0b0/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    59411 2024-04-05 23:43:18.000000 suql-1.0.0b0/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.0.0b0/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-05 23:43:51.784317 suql-1.0.0b0/src/suql.egg-info/
--rw-------   0 oval      (1000) users      (100)     4616 2024-04-05 23:43:51.000000 suql-1.0.0b0/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-04-05 23:43:51.000000 suql-1.0.0b0/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-04-05 23:43:51.000000 suql-1.0.0b0/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      217 2024-04-05 23:43:51.000000 suql-1.0.0b0/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-04-05 23:43:51.000000 suql-1.0.0b0/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-08 18:27:27.455707 suql-1.1.0a0/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.0a0/LICENSE
+-rw-------   0 oval      (1000) users      (100)     4614 2024-04-08 18:27:27.455707 suql-1.1.0a0/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4160 2024-04-06 00:00:52.000000 suql-1.1.0a0/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-04-08 18:27:27.455707 suql-1.1.0a0/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1423 2024-04-08 18:27:24.000000 suql-1.1.0a0/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-08 18:27:27.451707 suql-1.1.0a0/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-04-08 18:27:27.451707 suql-1.1.0a0/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.0a0/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.0a0/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    16980 2024-04-07 05:13:01.000000 suql-1.1.0a0/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8646 2024-04-06 00:50:57.000000 suql-1.1.0a0/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     4095 2024-04-03 06:02:28.000000 suql-1.1.0a0/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)    12093 2024-04-06 00:13:31.000000 suql-1.1.0a0/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-08 18:27:27.451707 suql-1.1.0a0/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.0a0/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.0a0/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.0a0/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.0a0/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.0a0/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.0a0/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.0a0/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.0a0/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.0a0/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-08 18:27:27.451707 suql-1.1.0a0/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.0a0/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    61780 2024-04-07 06:57:06.000000 suql-1.1.0a0/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.0a0/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-08 18:27:27.451707 suql-1.1.0a0/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     4614 2024-04-08 18:27:27.000000 suql-1.1.0a0/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-04-08 18:27:27.000000 suql-1.1.0a0/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-04-08 18:27:27.000000 suql-1.1.0a0/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      217 2024-04-08 18:27:27.000000 suql-1.1.0a0/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-04-08 18:27:27.000000 suql-1.1.0a0/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.0.0b0/LICENSE` & `suql-1.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.0.0b0/PKG-INFO` & `suql-1.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.0.0b0
+Version: 1.1.0a0
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -62,15 +62,15 @@
 
 There are two main ways of installing the SUQL library.
 
 ## Install from `pip`
 
 Ideal for integrating the SUQL compiler in a larger codebase / system. See [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/install_pip.md) for details.
 
-## Install from source**
+## Install from source
 
 Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
 
 ## Agent tutorial
 
 Check out [conv_agent.md](https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more information on best practices for using SUQL to power your conversational agent.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.0.0b0 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.0a0 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
            ************ SSUUQQLL ((SSttrruuccttuurreedd aanndd UUnnssttrruuccttuurreedd QQuueerryy LLaanngguuaaggee))
                          _[[_aa_rr_XX_ii_vv_]]_[[_GG_ii_tt_hh_uu_bb_ _SS_tt_aa_rr_ss_]] ************
@@ -30,15 +30,15 @@
 text to be easily combined with structured constraints. Here is one high-level
 example: ![An example for using SUQL](https://github.com/stanford-oval/suql/
 blob/main/figures/figure2.png?raw=true) For more details, see our paper at
 https://arxiv.org/abs/2311.09818. # Installation / Usage tutorial There are two
 main ways of installing the SUQL library. ## Install from `pip` Ideal for
 integrating the SUQL compiler in a larger codebase / system. See
 [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/
-install_pip.md) for details. ## Install from source** Ideal for using this repo
+install_pip.md) for details. ## Install from source Ideal for using this repo
 to build a SUQL-powered conversational interface to your data out-of-the-box,
 like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See
 [docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_source.md) for details. ## Agent tutorial Check out [conv_agent.md]
 (https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more
 information on best practices for using SUQL to power your conversational
 agent. # Bugs / Contribution If you encounter a problem, first check
```

### Comparing `suql-1.0.0b0/README.md` & `suql-1.1.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 There are two main ways of installing the SUQL library.
 
 ## Install from `pip`
 
 Ideal for integrating the SUQL compiler in a larger codebase / system. See [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/install_pip.md) for details.
 
-## Install from source**
+## Install from source
 
 Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
 
 ## Agent tutorial
 
 Check out [conv_agent.md](https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more information on best practices for using SUQL to power your conversational agent.
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
 text to be easily combined with structured constraints. Here is one high-level
 example: ![An example for using SUQL](https://github.com/stanford-oval/suql/
 blob/main/figures/figure2.png?raw=true) For more details, see our paper at
 https://arxiv.org/abs/2311.09818. # Installation / Usage tutorial There are two
 main ways of installing the SUQL library. ## Install from `pip` Ideal for
 integrating the SUQL compiler in a larger codebase / system. See
 [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/
-install_pip.md) for details. ## Install from source** Ideal for using this repo
+install_pip.md) for details. ## Install from source Ideal for using this repo
 to build a SUQL-powered conversational interface to your data out-of-the-box,
 like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See
 [docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_source.md) for details. ## Agent tutorial Check out [conv_agent.md]
 (https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more
 information on best practices for using SUQL to power your conversational
 agent. # Bugs / Contribution If you encounter a problem, first check
```

### Comparing `suql-1.0.0b0/setup.py` & `suql-1.1.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.0.0b0"
+version = "1.1.0a0"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
```

### Comparing `suql-1.0.0b0/src/suql/agent.py` & `suql-1.1.0a0/src/suql/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         postprocess=False,
     )
     print("directly generated SUQL query: {}".format(generated_suql))
     postprocessed_suql = postprocess_suql(generated_suql)
 
     suql_execute_start_time = time.time()
     final_res, column_names, cache = suql_execute(
-        postprocessed_suql, fts_fields=[("restaurants", "name")]
+        postprocessed_suql, {"restaurants": "_id"}, fts_fields=[("restaurants", "name")]
     )
     suql_execute_end_time = time.time()
 
     results_for_ned = extract_id_name(final_res, column_names)
     final_res = clean_up_response(final_res, column_names)
 
     return (
```

### Comparing `suql-1.0.0b0/src/suql/faiss_embedding.py` & `suql-1.1.0a0/src/suql/faiss_embedding.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0b0/src/suql/free_text_fcns_server.py` & `suql-1.1.0a0/src/suql/free_text_fcns_server.py`

 * *Files 15% similar despite different names*

```diff
@@ -176,15 +176,41 @@
 def get_hours_request_extracted(hours_request):
     intervals = hours_request.split("-")
     hours_request_extracted = [[int(y) for y in x.split(".")] for x in intervals]
     return hours_request_extracted
 
 
 def get_restaurant_hours_extracted(restaurant_hours):
-    from suql.agent import handle_opening_hours
+    def handle_opening_hours(input_dict):
+        """
+        Custom function to convert opening hours into LLM-readable formats.
+        """
+        order = [
+            "Monday",
+            "Tuesday",
+            "Wednesday",
+            "Thursday",
+            "Friday",
+            "Saturday",
+            "Sunday",
+        ]
+
+        def get_order_index(x):
+            try:
+                return order.index(x["day_of_the_week"])
+            except ValueError:
+                return len(order)  # or any default value
+
+        res = []
+        input_dict = sorted(input_dict, key=lambda x: get_order_index(x))
+        for i in input_dict:
+            res.append(
+                f'open from {i["open_time"]} to {i["close_time"]} on {i["day_of_the_week"]}'
+            )
+        return res
 
     restaurant_hours = json.loads(restaurant_hours)
     restaurant_hours = handle_opening_hours(restaurant_hours)
     restaurant_hours_extracted = []
     for hours in restaurant_hours:
         hours_tokenized = re.split("open from | to | on ", hours)
         _, start, end, day = hours_tokenized
```

### Comparing `suql-1.0.0b0/src/suql/postgresql_connection.py` & `suql-1.1.0a0/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0b0/src/suql/prompt_continuation.py` & `suql-1.1.0a0/src/suql/prompt_continuation.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from typing import List
 
 import openai
 from openai import OpenAI
 
-client = OpenAI()
 import os
 import time
 import traceback
 from functools import partial
 from threading import Thread
 
 from jinja2 import Environment, FileSystemLoader, select_autoescape
@@ -31,22 +30,16 @@
 jinja_environment = Environment(
     loader=FileSystemLoader(os.path.dirname(os.path.abspath(__file__))),
     autoescape=select_autoescape(),
     trim_blocks=True,
     lstrip_blocks=True,
     line_comment_prefix="#",
 )
-# # uncomment if using Azure OpenAI
-openai.api_type == "open_ai"
-# openai.api_type = "azure"
-# openai.api_base = "https://ovalopenairesource.openai.azure.com/"
-# openai.api_version = "2023-05-15"
 
 ENABLE_CACHING = False
-
 if ENABLE_CACHING:
     import pymongo
     mongo_client = pymongo.MongoClient("localhost", 27017)
     prompt_cache_db = mongo_client["open_ai_prompts"]["caches"]
 
 # inference_cost_per_1000_tokens = {'ada': 0.0004, 'babbage': 0.0005, 'curie': 0.002, 'davinci': 0.02, 'turbo': 0.003, 'gpt-4': 0.03} # for Azure
 inference_input_cost_per_1000_tokens = {
@@ -78,14 +71,20 @@
             inference_input_cost_per_1000_tokens[model_name],
             inference_output_cost_per_1000_tokens[model_name],
         )
     raise ValueError("Did not recognize GPT model name %s" % model_name)
 
 
 def openai_chat_completion_with_backoff(**kwargs):
+    client = OpenAI()
+    # # uncomment if using Azure OpenAI
+    openai.api_type == "open_ai"
+    # openai.api_type = "azure"
+    # openai.api_base = "https://ovalopenairesource.openai.azure.com/"
+    # openai.api_version = "2023-05-15"
     global total_cost
     ret = client.chat.completions.create(**kwargs)
     num_prompt_tokens = ret.usage.prompt_tokens
     num_completion_tokens = ret.usage.completion_tokens
     prompt_cost, completion_cost = _model_name_to_cost(kwargs["model"])
     total_cost += (
         num_prompt_tokens / 1000 * prompt_cost
```

### Comparing `suql-1.0.0b0/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.0a0/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.0.0b0/src/suql/prompts/opening_hours.prompt` & `suql-1.1.0a0/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.0.0b0/src/suql/prompts/parser_suql.prompt` & `suql-1.1.0a0/src/suql/prompts/parser_suql.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.0.0b0/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.0a0/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.0.0b0/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.0a0/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.0.0b0/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.0a0/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import random
 import string
 import time
 import traceback
 from collections import defaultdict
 from copy import deepcopy
-from typing import List
+from typing import List, Union
 
 import pglast
 import requests
 from pglast import parse_sql
 from pglast.ast import *
 from pglast.enums.parsenodes import A_Expr_Kind
 from pglast.enums.primnodes import BoolExprType, CoercionForm
@@ -21,62 +21,46 @@
 from sympy.logic.boolalg import And, Not, Or, to_dnf
 
 from suql.postgresql_connection import execute_sql, execute_sql_with_column_info
 from suql.prompt_continuation import llm_generate
 from suql.utils import num_tokens_from_string
 
 # System parameters, do not modify
-SET_FREE_TEXT_FCNS = ["answer"]
-verified_res = {}
+_SET_FREE_TEXT_FCNS = ["answer"]
+_verified_res = {}
 
-# Embedding server address
-EMBEDDING_SERVER_ADDRESS = "http://127.0.0.1:8501"
-# This denotes the model used by the SUQL compiler for all verification purposes
-MODEL = "gpt-3.5-turbo-0613"
-# This denotes whether to attempt verify against all columns
-# TODO: not yet used now
-VERIFY_ALL_COLUMNS = True
-# This denotes the max number of items per LIMIT number to be sent to GPT for verification
-MAX_VERIFY = 20
-
-# A list of declared tuples with their unique IDs
-# e.g. TABLE_W_IDS = {"courses": "course_id", "ratings": "rating_id"}
-# e.g. TABLE_W_IDS = {"restaurants": "_id"}
-TABLE_W_IDS = {"restaurants": "_id"}
-
-
-def generate_random_string(length=12):
+def _generate_random_string(length=12):
     characters = string.ascii_lowercase + string.digits
     random_string = "".join(random.choice(characters) for _ in range(length))
     return random_string
 
 
-class FreeTextFcnVisitor(Visitor):
+class _FreeTextFcnVisitor(Visitor):
     def __init__(self) -> None:
         super().__init__()
-        self.set_free_text_fcns = SET_FREE_TEXT_FCNS
+        self._SET_FREE_TEXT_FCNS = _SET_FREE_TEXT_FCNS
         self.res = False
 
     def __call__(self, node):
         super().__call__(node)
 
     def visit_FuncCall(self, ancestors, node: pglast.ast.FuncCall):
         for i in node.funcname:
-            if i.sval in self.set_free_text_fcns:
+            if i.sval in self._SET_FREE_TEXT_FCNS:
                 self.res = True
                 return
 
 
-def if_contains_free_text_fcn(node):
-    visitor = FreeTextFcnVisitor()
+def _if_contains_free_text_fcn(node):
+    visitor = _FreeTextFcnVisitor()
     visitor(node)
     return visitor.res
 
 
-class TypeCastAnswer(Visitor):
+class _TypeCastAnswer(Visitor):
     def __init__(self) -> None:
         super().__init__()
 
     def __call__(self, node):
         super().__call__(node)
 
     def visit_TypeCast(self, ancestors, node: TypeCast):
@@ -91,45 +75,45 @@
             if len(node.arg.args) == 2:
                 type_name = node.typeName.names[-1].sval
                 node.arg.args = tuple(
                     list(node.arg.args) + [A_Const(val=String(sval=type_name))]
                 )
 
 
-class IfAllStructural(Visitor):
+class _IfAllStructural(Visitor):
     def __init__(self) -> None:
         super().__init__()
         self.res = True
 
     def __call__(self, node):
         super().__call__(node)
 
     def visit_A_Expr(self, ancestors, node: A_Expr):
         if self.res is False:
             return
 
         def is_structural(expr):
             if (
                 isinstance(expr, FuncCall)
-                and ".".join(map(lambda x: x.sval, expr.funcname)) in SET_FREE_TEXT_FCNS
+                and ".".join(map(lambda x: x.sval, expr.funcname)) in _SET_FREE_TEXT_FCNS
             ):
                 return False
             return True
 
         if not (is_structural(node.lexpr) and is_structural(node.rexpr)):
             self.res = False
 
 
-def get_sublink_parent(ancestor):
+def _get_sublink_parent(ancestor):
     if ancestor.node is not None and not isinstance(ancestor.node, tuple):
         return ancestor.node
-    return get_sublink_parent(ancestor.parent)
+    return _get_sublink_parent(ancestor.parent)
 
 
-class IfInvovlesSubquery(Visitor):
+class _IfInvovlesSubquery(Visitor):
     def __init__(self) -> None:
         super().__init__()
         self.sublinks = []
         self.ancestors = []
 
     def __call__(self, node):
         super().__call__(node)
@@ -151,82 +135,97 @@
         res = []
         closest_parent = None
         for sublink, ancestor in zip(self.sublinks, self.ancestors):
             # first get the actual parent node
             if ancestor.parent is None:
                 continue
             else:
-                closest_parent = get_sublink_parent(ancestor.parent)
+                closest_parent = _get_sublink_parent(ancestor.parent)
             if closest_parent == closest_parent:
                 res.append(sublink)
         return res
 
 
-def if_all_structural(node):
-    visitor = IfAllStructural()
+def _if_all_structural(node):
+    visitor = _IfAllStructural()
     visitor(node)
     return visitor.res
 
 
-class SelectVisitor(Visitor):
+class _SelectVisitor(Visitor):
     def __init__(
         self,
         fts_fields,
         embedding_server_address,
         select_username,
         select_userpswd,
         create_username,
         create_userpswd,
+        table_w_ids,
+        llm_model_name,
+        max_verify
     ) -> None:
         super().__init__()
         self.tmp_tables = []
         # this cache is to store classifier results for sturctured fields (e.g. cuisines in restaurants)
         self.cache = defaultdict(dict)
         self.fts_fields = fts_fields
         self.embedding_server_address = embedding_server_address
 
         # stores credentials
         self.select_username = select_username
         self.select_userpswd = select_userpswd
         self.create_username = create_username
         self.create_userpswd = create_userpswd
+        
+        # store table_w_ids
+        self.table_w_ids = table_w_ids
+        
+        # store default LLM
+        self.llm_model_name = llm_model_name
+        
+        # store max verify param
+        self.max_verify = max_verify
 
     def __call__(self, node):
         super().__call__(node)
 
     def visit_SelectStmt(self, ancestors, node: SelectStmt):
-        type_cast_answer_visitor = TypeCastAnswer()
+        type_cast_answer_visitor = _TypeCastAnswer()
         type_cast_answer_visitor(node)
 
         if not node.whereClause:
             return
 
         # First, understand whether this involves subquery. If it does, then starts with that first and builds upwards
         # If that subquery in turn involves other subqueries, then recursive calls take care of it
-        subquery_visitor = IfInvovlesSubquery()
+        subquery_visitor = _IfInvovlesSubquery()
         subquery_visitor(node)
         sublinks = subquery_visitor.return_top_level_sublinks()
         for sublink in sublinks:
             self.visit_SelectStmt(None, sublink)
 
-        freeTextFcnVisitor = FreeTextFcnVisitor()
+        freeTextFcnVisitor = _FreeTextFcnVisitor()
         freeTextFcnVisitor(node.whereClause)
 
         if freeTextFcnVisitor.res:
-            tmp_table_name = "temp_table_{}".format(generate_random_string())
+            tmp_table_name = "temp_table_{}".format(_generate_random_string())
             self.tmp_tables.append(tmp_table_name)
 
             # main entry point for SUQL compiler optimization
-            results, column_info = analyze_SelectStmt(
+            results, column_info = _analyze_SelectStmt(
                 node,
                 self.cache,
                 self.fts_fields,
                 self.embedding_server_address,
                 self.select_username,
                 self.select_userpswd,
+                self.table_w_ids,
+                self.llm_model_name,
+                self.max_verify
             )
 
             # based on results and column_info, insert a temporary table
             column_create_stmt = ",\n".join(
                 list(map(lambda x: f'"{x[0]}" {x[1]}', column_info))
             )
             create_stmt = f"CREATE TABLE {tmp_table_name} (\n{column_create_stmt}\n); GRANT SELECT ON {tmp_table_name} TO {self.select_username};"
@@ -264,20 +263,21 @@
 
             # finally, modify the existing sql with tmp_table_name
             node.fromClause = (
                 RangeVar(relname=tmp_table_name, inh=True, relpersistence="p"),
             )
             node.whereClause = None
         else:
-            classify_db_fields(
+            _classify_db_fields(
                 node,
                 self.cache,
                 self.fts_fields,
                 self.select_username,
                 self.select_userpswd,
+                self.llm_model_name
             )
 
     def serialize_cache(self):
         def print_value(x):
             if isinstance(x, String):
                 return x.sval
             elif isinstance(x, Integer):
@@ -307,34 +307,34 @@
                 drop_stmt,
                 user=self.create_username,
                 password=self.create_userpswd,
                 commit_in_lieu_fetch=True,
             )
 
 
-class PredicateMapping:
+class _PredicateMapping:
     def __init__(self) -> None:
         self.symbols2predicate = {}
         self.counter = 0
 
-    def add_mapping(self, predicate: BoolExpr or A_Expr) -> Symbol:
+    def add_mapping(self, predicate: Union[BoolExpr, A_Expr]) -> Symbol:
         res = symbols(str(self.counter))
         self.symbols2predicate[res] = predicate
         self.counter += 1
         return res
 
     def retrieve_predicate(self, symbol):
         return self.symbols2predicate[symbol]
 
 
-def convert2dnf(predicate):
-    predicate_mapping = PredicateMapping()
+def _convert2dnf(predicate):
+    predicate_mapping = _PredicateMapping()
 
     def predicate2symbol(_predicate: BoolExpr):
-        if if_all_structural(_predicate):
+        if _if_all_structural(_predicate):
             return predicate_mapping.add_mapping(_predicate)
 
         if isinstance(_predicate, A_Expr):
             return predicate_mapping.add_mapping(_predicate)
         if _predicate.boolop == BoolExprType.AND_EXPR:
             return And(*(predicate2symbol(x) for x in _predicate.args))
         if _predicate.boolop == BoolExprType.OR_EXPR:
@@ -369,17 +369,17 @@
     elif isinstance(predicate, BoolExpr):
         symbol_predicate = predicate2symbol(predicate)
         dnf_symbol_predicate = to_dnf(symbol_predicate)
         sql_expr = symbol2predicate(dnf_symbol_predicate)
         return sql_expr
 
 
-def verify(document, field, query, operator, value):
-    if (document, field, query, operator, value) in verified_res:
-        return verified_res[(document, field, query, operator, value)]
+def _verify(document, field, query, operator, value, llm_model_name):
+    if (document, field, query, operator, value) in _verified_res:
+        return _verified_res[(document, field, query, operator, value)]
 
     # construct the answer part
     if operator == "=":
         answer = value
     else:
         answer = operator + " " + value
 
@@ -387,53 +387,61 @@
         template_file="prompts/verification.prompt",
         prompt_parameter_values={
             "document": document,
             "field": field[1],  # field is a tuple (table_name, field_name)
             "query": query,
             "answer": answer,
         },
-        engine=MODEL,
+        engine=llm_model_name,
         temperature=0,
         stop_tokens=["\n"],
         max_tokens=30,
         postprocess=False,
     )[0]
 
     if "the answer is correct" in res.lower():
         res = True
     else:
         res = False
-    verified_res[(document, field, query, operator, value)] = res
+    _verified_res[(document, field, query, operator, value)] = res
     return res
 
 
-def verify_single_res(doc, field_query_list):
+def _verify_single_res(doc, field_query_list, llm_model_name):
     # verify for each stmt, if any stmt fails to verify, exclude it
     all_found = True
     found_stmt = []
     for i, entry in enumerate(field_query_list):
         field, query, operator, value = entry
 
         # this function helps with list processing
         # for a list, verify against each one, if any returns true then return that
         def verify_single_value(single_value, single_column_name):
             res = False
             # if this is a string, then directly verify:
             if isinstance(single_value, str):
-                res = verify(single_value, single_column_name, query, operator, value)
+                res = _verify(
+                    single_value,
+                    single_column_name,
+                    query,
+                    operator,
+                    value,
+                    llm_model_name
+                )
             # otherwise it is a list. Go over the list until if one verifies
             else:
                 assert isinstance(single_value, list)
                 for current_column_each_value in single_value:
-                    if verify(
+                    if _verify(
                         current_column_each_value,
                         single_column_name,
                         query,
                         operator,
                         value,
+                        llm_model_name
                     ):
                         res = True
                         break
             return res
 
         # if there are three elements in doc, then this indicates that we are in the mode
         # of attempting to verify all columns
@@ -462,15 +470,15 @@
                         break
 
                 # if still can't find an answer, then this row is hopeless and should be rejected
                 if not all_found:
                     break
 
         else:
-            if not verify(doc[1][i], field, query, operator, value):
+            if not _verify(doc[1][i], field, query, operator, value, llm_model_name):
                 all_found = False
                 break
             else:
                 found_stmt.append(
                     "Verified answer({}, '{}') {} {} in table = {} based on document: {}".format(
                         field[1], query, operator, value, field[0], doc[1][i]
                     )
@@ -479,15 +487,15 @@
         print("\n".join(found_stmt))
     elif found_stmt:
         print("partially verified: " + "\n".join(found_stmt))
 
     return all_found
 
 
-def parallel_filtering(fcn, source: list, limit, enforce_ordering=False):
+def _parallel_filtering(fcn, source: list, limit, enforce_ordering=False):
     true_count = 0
     true_items = set()
 
     # build a dictionary with index -> true/false/None
     # which indicates whether an item has been verified
     ordered_results = {i: None for i in range(len(source))}
 
@@ -525,45 +533,48 @@
                 else:
                     res.append(item[0])
         return res
 
     return true_items
 
 
-def retrieve_and_verify(
+def _retrieve_and_verify(
     node: SelectStmt,
     field_query_list,
     existing_results,
     column_info,
     limit,
     embedding_server_address,
+    table_w_ids,
+    llm_model_name,
+    max_verify,
     parallel=True,
     fetch_all=False,
 ):
     # field_query_list is a list of tuples, each entry of the tuple are:
     # 0st: field: field to do retrieval on
     # 1st: query: query for retrieval model
     # 2nd: operator: operator to compare against
     # 3rd: value: value to compare against
     #
     # existing_results: existing results to run retrieval on, this is a list of tuples
     # column_info: this is a list of tuples, first element is column name and second is type
     # limit: max number of returned results
     if len(node.fromClause) == 1 and isinstance(node.fromClause[0], RangeVar):
-        id_field_name = TABLE_W_IDS[node.fromClause[0].relname]
+        id_field_name = table_w_ids[node.fromClause[0].relname]
         single_table = True
         id_index = list(map(lambda x: x[0], column_info)).index(id_field_name)
         id_list = list(map(lambda x: x[id_index], existing_results))
     elif len(node.fromClause) == 1 and isinstance(node.fromClause[0], JoinExpr):
         single_table = False
         id_list = {}
         for arg in [node.fromClause[0].larg, node.fromClause[0].rarg]:
             if isinstance(arg, RangeVar):
                 table_name = arg.relname
-                id_field_name = TABLE_W_IDS[table_name]
+                id_field_name = table_w_ids[table_name]
                 id_index = list(map(lambda x: x[0], column_info)).index(
                     f"{table_name}^{id_field_name}"
                 )
                 id_list[table_name] = list(map(lambda x: x[id_index], existing_results))
         # also append a special "_id_join" field to keep track
         column_info = [("_id_join", "int4")] + column_info
         _id_join_index = list(map(lambda x: x[0], column_info)).index("_id_join")
@@ -579,17 +590,17 @@
         id_index = list(map(lambda x: x[0], column_info)).index("_id_join")
         id_list = list(map(lambda x: x[id_index], existing_results))
     else:
         # some yet-to-be-discovered cases?
         raise ValueError()
 
     start_time = time.time()
-    # clean previous verified_res, to avoid determistic caching (this could be removed)
-    global verified_res
-    verified_res = {}
+    # clean previous _verified_res, to avoid determistic caching (this could be removed)
+    global _verified_res
+    _verified_res = {}
 
     if fetch_all:
         # first get all free text fields:
         all_free_text_columns = []
         # NOTE: uncomment the following to enable going to multiple columns for filtering
         for each_column_info in column_info:
             # NOTE: HybridQA-specific
@@ -628,15 +639,15 @@
             )
     else:
         start_time = time.time()
         data = {
             "id_list": id_list,
             "field_query_list": list(map(lambda x: (x[0], x[1]), field_query_list)),
             "top": limit
-            * MAX_VERIFY,  # return MAX_VERIFY times the ordered amount, for GPT filtering purposes
+            * max_verify,  # return max_verify times the ordered amount, for GPT filtering purposes
         }
         data["single_table"] = single_table
 
         # Send a POST request
         response = requests.post(
             embedding_server_address + "/search",
             json=data,
@@ -649,24 +660,24 @@
         for res in parsed_result:
             if res not in filtered_parsed_result:
                 filtered_parsed_result.append(res)
         parsed_result = filtered_parsed_result
 
     if parallel:
         # parallelize verification calls
-        id_res = parallel_filtering(
-            lambda x: verify_single_res(x, field_query_list),
+        id_res = _parallel_filtering(
+            lambda x: _verify_single_res(x, field_query_list, llm_model_name),
             parsed_result,
             limit,
             enforce_ordering=True if node.sortClause is not None else False,
         )
     else:
         id_res = []
         for each_res in parsed_result:
-            if verify_single_res(each_res, field_query_list):
+            if _verify_single_res(each_res, field_query_list, llm_model_name):
                 id_res.append(each_res[0])
 
     end_time = time.time()
     print("retrieve + verification time {}s".format(end_time - start_time))
 
     if single_table:
         res = list(filter(lambda x: x[id_index] in id_res, existing_results))
@@ -674,15 +685,15 @@
         res = [
             i[1:]
             for i in list(filter(lambda x: x[id_index] in id_res, existing_results))
         ]
     return res
 
 
-def get_a_expr_field_value(node: A_Expr, no_check=False):
+def _get_a_expr_field_value(node: A_Expr, no_check=False):
     if isinstance(node.lexpr, ColumnRef):
         column = node.lexpr
         value = node.rexpr
     elif isinstance(node.rexpr, ColumnRef):
         column = node.rexpr
         value = node.lexpr
     elif no_check:
@@ -694,15 +705,15 @@
         return column_name, value_res
     elif no_check:
         return None, None
     else:
         raise ValueError()
 
 
-def replace_a_expr_field(node: A_Expr, ancestors: Ancestor, new_value):
+def _replace_a_expr_field(node: A_Expr, ancestors: Ancestor, new_value):
     def find_value_column(node: A_Expr):
         if isinstance(node.lexpr, ColumnRef):
             column = node.lexpr
             value = node.rexpr
         else:
             column = node.rexpr
             value = node.lexpr
@@ -739,15 +750,15 @@
             new_args = [x for x in new_args if x != node]
             ancestors.parent.node.args = tuple(new_args)
     else:
         _, value = find_value_column(node)
         value.val = new_value
 
 
-def greedy_search_comma(input_string, predefined_list):
+def _greedy_search_comma(input_string, predefined_list):
     chunks = input_string.split(",")
     results = []
     buffer = ""
 
     for chunk in chunks:
         buffer = buffer + chunk if buffer else chunk
 
@@ -766,53 +777,54 @@
 
     return results
 
 
 # NOTE: this function is used if an ENUM field contains commas
 # in which case asking an LLM to output a comma-seperated list could be problematic
 # currently unused
-def get_comma_separated_numbers(input_string):
+def _get_comma_separated_numbers(input_string):
     try:
         # Remove spaces from the input string and then split it into a list of values using a comma as the separator
         values = input_string.replace(" ", "").split(",")
 
         # Convert each value to a float and store them in a list
         num_values = [int(value) for value in values]
 
         return num_values  # Return the list of numbers
     except ValueError:
         # If a ValueError is raised, it means at least one value is not a valid number, so return False
         return False
 
 
-class StructuralClassification(Visitor):
+class _StructuralClassification(Visitor):
     def __init__(
-        self, node: SelectStmt, cache, fts_fields, select_username, select_userpswd
+        self, node: SelectStmt, cache, fts_fields, select_username, select_userpswd, llm_model_name
     ) -> None:
         super().__init__()
         self.node = node
         self.cache = cache
         self.fts_fields = fts_fields
         self.select_username = select_username
         self.select_userpswd = select_userpswd
+        self.llm_model_name = llm_model_name
 
     def __call__(self, node):
         super().__call__(node)
 
     def visit_A_Expr(self, ancestors: Ancestor, node: A_Expr):
         # TODO: handle containment clauses
         if isinstance(node.name[0], String) and node.name[0].sval in ["@>", "<@"]:
             parsed_res = True
-            replace_a_expr_field(node, ancestors, parsed_res)
+            _replace_a_expr_field(node, ancestors, parsed_res)
             return
 
         # if this appears in projection, disregard
         if ancestors.find_nearest(ResTarget) is not None:
             return
-        assert if_all_structural(node)
+        assert _if_all_structural(node)
 
         if isinstance(node.lexpr, SubLink) or isinstance(node.rexpr, SubLink):
             # if there is a subquery, skip classification
             return
 
         if isinstance(node.lexpr, ColumnRef) and isinstance(node.rexpr, ColumnRef):
             return
@@ -837,15 +849,15 @@
         # if this is one of the fields declared to be used with fts (full text search), convert so:
         for table_name, field_name in self.fts_fields:
             if (
                 len(self.node.fromClause) == 1
                 and isinstance(self.node.fromClause[0], RangeVar)
                 and node.name[0].sval in ["~~", "~~*", "="]
             ):
-                n_field_name, n_value_name = get_a_expr_field_value(node, no_check=True)
+                n_field_name, n_value_name = _get_a_expr_field_value(node, no_check=True)
                 if (
                     table_name == self.node.fromClause[0].relname
                     and field_name == n_field_name
                 ):
                     node.lexpr = FuncCall(
                         funcname=(String(sval="websearch_to_tsquery"),),
                         args=(
@@ -899,15 +911,15 @@
             )
             res = True
 
         if not res:
             print("determined the above predicate returns no result")
             # try to classify into one of the known values
             # first, we need to find out what is the value here - some heuristics here to find out
-            column_name, value_res = get_a_expr_field_value(node)
+            column_name, value_res = _get_a_expr_field_value(node)
 
             if isinstance(value_res, String):
                 value_res_clear = value_res.sval
             elif isinstance(value_res, Integer):
                 value_res_clear = value_res.ival
             elif isinstance(value_res, Float):
                 value_res_clear = value_res.fval
@@ -919,15 +931,15 @@
                     column_name, value_res_clear
                 )
             )
 
             # first check if this is already in the cache
             # TODO: for best performance move this before the execution above
             if column_name in self.cache and value_res_clear in self.cache[column_name]:
-                replace_a_expr_field(
+                _replace_a_expr_field(
                     node, ancestors, self.cache[column_name][value_res_clear]
                 )
             else:
                 # first understand whether this field is of type TEXT or TEXT[]
                 column_type = None
                 for column_info in column_infos:
                     if column_info[0] == column_name:
@@ -985,52 +997,53 @@
                     res = llm_generate(
                         "prompts/field_classification.prompt",
                         {
                             "predicted_field_value": value_res_clear,
                             "field_value_choices": field_value_choices,
                             "field_name": column_name,
                         },
-                        engine=MODEL,
+                        engine=self.llm_model_name,
                         temperature=0,
                         stop_tokens=["\n"],
                         max_tokens=100,
                         postprocess=False,
                     )[0]
                     if res in field_value_choices:
-                        replace_a_expr_field(node, ancestors, String(sval=(res)))
+                        _replace_a_expr_field(node, ancestors, String(sval=(res)))
                         self.cache[column_name][value_res_clear] = String(sval=(res))
                     # tries to parse it as a list
                     else:
-                        parsed_res = greedy_search_comma(res, field_value_choices)
+                        parsed_res = _greedy_search_comma(res, field_value_choices)
                         if parsed_res:
                             parsed_res = tuple(
                                 map(lambda x: String(sval=(x)), parsed_res)
                             )
-                            replace_a_expr_field(node, ancestors, parsed_res)
+                            _replace_a_expr_field(node, ancestors, parsed_res)
                             self.cache[column_name][value_res_clear] = parsed_res
 
 
-def classify_db_fields(
+def _classify_db_fields(
     node: SelectStmt,
     cache: dict,
     fts_fields: List,
     select_username: str,
     select_userpswd: str,
+    llm_model_name: str
 ):
     # we expect all atomic predicates under `predicate` to only involve stru fields
     # (no `answer` function)
     # the goal of this function is to determine which predicate leads to no results
     # for a field without results, try to classify into one of the existing fields
-    visitor = StructuralClassification(
-        node, cache, fts_fields, select_username, select_userpswd
+    visitor = _StructuralClassification(
+        node, cache, fts_fields, select_username, select_userpswd, llm_model_name
     )
     visitor(node)
 
 
-class Replace_Original_Target_Visitor(Visitor):
+class _Replace_Original_Target_Visitor(Visitor):
     def __init__(self, table_column_mapping={}) -> None:
         super().__init__()
         self.table_column_mapping: dict = table_column_mapping
 
     def __call__(self, node):
         super().__call__(node)
 
@@ -1045,41 +1058,43 @@
                     if res is not None:
                         # the same field appears twice, this means that the original syntax is problematic
                         break
                     res = (String(sval=f"{table_name}^{node.fields[0].sval}"),)
             node.fields = res
 
 
-def execute_structural_sql(
+def _execute_structural_sql(
     original_node: SelectStmt,
     predicate: BoolExpr,
     cache: dict,
     fts_fields: List,
     select_username: str,
     select_userpswd: str,
+    llm_model_name: str
 ):
     node = deepcopy(original_node)
     # change projection to include everything
     # there are a couple of cases here
     # the simplest case is if it is one table
     if len(node.fromClause) == 1 and isinstance(node.fromClause[0], RangeVar):
         node.targetList = (ResTarget(val=ColumnRef(fields=(A_Star(),))),)
     # these are full joins
     elif len(node.fromClause) == 1 and isinstance(node.fromClause[0], JoinExpr):
         all_projection_fields = []
         table_column_mapping = {}
         for table in [node.fromClause[0].larg, node.fromClause[0].rarg]:
             # find out what columns this table has
-            _, columns = execute_structural_sql(
+            _, columns = _execute_structural_sql(
                 SelectStmt(fromClause=(table,)),
                 None,
                 cache,
                 fts_fields,
                 select_username,
                 select_userpswd,
+                llm_model_name
             )
             # give the projection fields new names
             projection_table_name = (
                 table.alias.aliasname if table.alias is not None else table.relname
             )
             table_column_mapping[projection_table_name] = columns
 
@@ -1093,32 +1108,33 @@
                         )
                     ),
                 )
                 all_projection_fields.append(new_projection_clause)
         node.targetList = tuple(all_projection_fields)
 
         # if we replaced the names, we also need to propagate the names to the original `node` in projections
-        replace_original_target_visitor = Replace_Original_Target_Visitor(
+        replace_original_target_visitor = _Replace_Original_Target_Visitor(
             table_column_mapping=table_column_mapping
         )
         replace_original_target_visitor(original_node.targetList)
         if original_node.sortClause is not None:
             replace_original_target_visitor(original_node.sortClause)
     # next, there are tuple joins (self joins)
     elif len(node.fromClause) > 1 and isinstance(node.fromClause, tuple):
         all_projection_fields = []
         for table in node.fromClause:
             # find out what columns this table has
-            _, columns = execute_structural_sql(
+            _, columns = _execute_structural_sql(
                 SelectStmt(fromClause=(table,)),
                 None,
                 cache,
                 fts_fields,
                 select_username,
                 select_userpswd,
+                llm_model_name
             )
             # give the projection fields new names
             projection_table_name = (
                 table.alias.aliasname if table.alias is not None else table.relname
             )
             for column in columns:
                 new_projection_clause = ResTarget(
@@ -1130,15 +1146,15 @@
                         )
                     ),
                 )
                 all_projection_fields.append(new_projection_clause)
         node.targetList = tuple(all_projection_fields)
 
         # if we replaced the names, we also need to propagate the names to the original `node` in projections
-        replace_original_target_visitor = Replace_Original_Target_Visitor()
+        replace_original_target_visitor = _Replace_Original_Target_Visitor()
         replace_original_target_visitor(original_node.targetList)
         if original_node.sortClause is not None:
             replace_original_target_visitor(original_node.sortClause)
 
     # Some other cases?
     else:
         node.targetList = (ResTarget(val=ColumnRef(fields=(A_Star(),))),)
@@ -1148,33 +1164,35 @@
     node.limitOffset = None
     # change predicates
     node.whereClause = predicate
     node.groupClause = None
     node.havingClause = None
 
     # only queries that involve only structural parts can be executed
-    assert if_all_structural(node)
+    assert _if_all_structural(node)
 
     # deal with sturctural field classification
-    classify_db_fields(node, cache, fts_fields, select_username, select_userpswd)
+    _classify_db_fields(node, cache, fts_fields, select_username, select_userpswd, llm_model_name)
 
     sql = RawStream()(node)
-    print("execute_structural_sql executing sql: {}".format(sql))
     return execute_sql_with_column_info(
         sql, user=select_username, password=select_userpswd
     )
 
 
-def execute_free_text_queries(
+def _execute_free_text_queries(
     node,
     predicate: BoolExpr,
     existing_results,
     column_info,
     limit,
     embedding_server_address,
+    table_w_ids,
+    llm_model_name,
+    max_verify
 ):
     # the predicate should only contain an atomic unstructural query
     # or an AND of multiple unstructural query (NOT of an unstructural query is considered to be atmoic)
     def assert_A_Const_Or_Tuple_A_Const(v):
         if isinstance(v, A_Const):
             return True
 
@@ -1195,34 +1213,34 @@
             elif isinstance(i.val, Integer):
                 res.append(i.val.ival)
             else:
                 raise ValueError()
         return tuple(res)
 
     def breakdown_unstructural_query(predicate: A_Expr):
-        assert if_contains_free_text_fcn(predicate.lexpr) or if_contains_free_text_fcn(
+        assert _if_contains_free_text_fcn(predicate.lexpr) or _if_contains_free_text_fcn(
             predicate.rexpr
         )
-        if if_contains_free_text_fcn(predicate.lexpr) and if_contains_free_text_fcn(
+        if _if_contains_free_text_fcn(predicate.lexpr) and _if_contains_free_text_fcn(
             predicate.rexpr
         ):
             raise ValueError(
                 "cannot optimize for predicate containing free text functions on both side of expression: {}".format(
                     RawStream()(predicate)
                 )
             )
 
         free_text_clause = (
             predicate.lexpr
-            if if_contains_free_text_fcn(predicate.lexpr)
+            if _if_contains_free_text_fcn(predicate.lexpr)
             else predicate.rexpr
         )
         value_clause = (
             predicate.lexpr
-            if not if_contains_free_text_fcn(predicate.lexpr)
+            if not _if_contains_free_text_fcn(predicate.lexpr)
             else predicate.rexpr
         )
         assert isinstance(free_text_clause, FuncCall)
         assert assert_A_Const_Or_Tuple_A_Const(value_clause)
 
         query_lst = list(
             filter(lambda x: isinstance(x, A_Const), free_text_clause.args)
@@ -1268,266 +1286,322 @@
     # TODO: handle cases with NOT
 
     if predicate is None:
         return existing_results
     if isinstance(predicate, A_Expr):
         field, query, operator, value = breakdown_unstructural_query(predicate)
         return (
-            retrieve_and_verify(
+            _retrieve_and_verify(
                 node,
                 [(field, query, operator, value)],
                 existing_results,
                 column_info,
                 limit,
                 embedding_server_address,
+                table_w_ids,
+                llm_model_name,
+                max_verify
             ),
             column_info,
         )
 
     elif isinstance(predicate, BoolExpr) and predicate.boolop == BoolExprType.AND_EXPR:
         field_query_list = []
         for a_pred in predicate.args:
             field_query_list.append(breakdown_unstructural_query(a_pred))
 
         return (
-            retrieve_and_verify(
+            _retrieve_and_verify(
                 node,
                 field_query_list,
                 existing_results,
                 column_info,
                 limit,
                 embedding_server_address,
+                table_w_ids,
+                llm_model_name,
+                max_verify
             ),
             column_info,
         )
 
     else:
         raise ValueError(
             "expects predicate to only contain atomic unstructural query, AND of them, or an NOT of atomic unsturctured query. However, this predicate is not: {}".format(
                 RawStream()(predicate)
             )
         )
 
 
-def execute_and(
+def _execute_and(
     sql_dnf_predicates,
     node: SelectStmt,
     limit,
     cache: dict,
     fts_fields: List,
     embedding_server_address,
     select_username,
     select_userpswd,
+    table_w_ids,
+    llm_model_name,
+    max_verify
 ):
     # there should not exist any OR expression inside sql_dnf_predicates
 
     if (
         isinstance(sql_dnf_predicates, BoolExpr)
         and sql_dnf_predicates.boolop == BoolExprType.AND_EXPR
     ):
         # find the structural part
         structural_predicates = tuple(
-            filter(lambda x: if_all_structural(x), sql_dnf_predicates.args)
+            filter(lambda x: _if_all_structural(x), sql_dnf_predicates.args)
         )
         if len(structural_predicates) == 0:
             structural_predicates = None
         elif len(structural_predicates) == 1:
             structural_predicates = structural_predicates[0]
         else:
             structural_predicates = BoolExpr(
                 boolop=BoolExprType.AND_EXPR, args=structural_predicates
             )
 
         # execute structural part
-        structural_res, column_info = execute_structural_sql(
+        structural_res, column_info = _execute_structural_sql(
             node,
             structural_predicates,
             cache,
             fts_fields,
             select_username,
             select_userpswd,
+            llm_model_name
         )
 
         free_text_predicates = tuple(
-            filter(lambda x: not if_all_structural(x), sql_dnf_predicates.args)
+            filter(lambda x: not _if_all_structural(x), sql_dnf_predicates.args)
         )
         if len(free_text_predicates) == 1:
             free_text_predicates = free_text_predicates[0]
         else:
             free_text_predicates = BoolExpr(
                 boolop=BoolExprType.AND_EXPR, args=free_text_predicates
             )
 
-        return execute_free_text_queries(
+        return _execute_free_text_queries(
             node,
             free_text_predicates,
             structural_res,
             column_info,
             limit,
             embedding_server_address,
+            table_w_ids,
+            llm_model_name,
+            max_verify
         )
 
     elif isinstance(sql_dnf_predicates, A_Expr) or (
         isinstance(sql_dnf_predicates, BoolExpr)
         and sql_dnf_predicates.boolop == BoolExprType.NOT_EXPR
     ):
-        if if_all_structural(sql_dnf_predicates):
-            return execute_structural_sql(
+        if _if_all_structural(sql_dnf_predicates):
+            return _execute_structural_sql(
                 node,
                 sql_dnf_predicates,
                 cache,
                 fts_fields,
                 select_username,
                 select_userpswd,
+                llm_model_name
             )
         else:
-            all_results, column_info = execute_structural_sql(
-                node, None, cache, fts_fields, select_username, select_userpswd
+            all_results, column_info = _execute_structural_sql(
+                node, None, cache, fts_fields, select_username, select_userpswd, llm_model_name
             )
-            return execute_free_text_queries(
+            return _execute_free_text_queries(
                 node,
                 sql_dnf_predicates,
                 all_results,
                 column_info,
                 limit,
                 embedding_server_address,
+                table_w_ids,
+                llm_model_name,
+                max_verify
             )
 
 
-def analyze_SelectStmt(
+def _analyze_SelectStmt(
     node: SelectStmt,
     cache: dict,
     fts_fields: List,
     embedding_server_address: str,
     select_username: str,
     select_userpswd: str,
+    table_w_ids: dict,
+    llm_model_name: str,
+    max_verify: str
 ):
     limit = node.limitCount.val.ival if node.limitCount else -1
-    sql_dnf_predicates = convert2dnf(node.whereClause)
+    sql_dnf_predicates = _convert2dnf(node.whereClause)
 
     # if it is an OR, then order the predicates in structural -> unstructual
     # execute these predicates in order, until the limit is reached
     if (
         isinstance(sql_dnf_predicates, BoolExpr)
         and sql_dnf_predicates.boolop == BoolExprType.OR_EXPR
     ):
         choices = sorted(
-            sql_dnf_predicates.args, key=lambda x: if_all_structural(x), reverse=True
+            sql_dnf_predicates.args, key=lambda x: _if_all_structural(x), reverse=True
         )
         res = []
         for choice in choices:
-            choice_res, column_info = execute_and(
+            choice_res, column_info = _execute_and(
                 choice,
                 node,
                 limit - len(res),
                 cache,
                 fts_fields,
                 embedding_server_address,
                 select_username,
                 select_userpswd,
+                table_w_ids,
+                llm_model_name,
+                max_verify
             )
             res.extend(choice_res)
 
             # at any time, if there is enough results, return that
             if len(res) >= limit and limit != -1:
                 break
 
         return res, column_info
 
     elif (
         isinstance(sql_dnf_predicates, BoolExpr)
         and sql_dnf_predicates.boolop == BoolExprType.AND_EXPR
     ):
-        return execute_and(
+        return _execute_and(
             sql_dnf_predicates,
             node,
             limit,
             cache,
             fts_fields,
             embedding_server_address,
             select_username,
             select_userpswd,
+            table_w_ids,
+            llm_model_name,
+            max_verify
         )
 
     elif isinstance(sql_dnf_predicates, A_Expr) or (
         isinstance(sql_dnf_predicates, BoolExpr)
         and sql_dnf_predicates.boolop == BoolExprType.NOT_EXPR
     ):
-        return execute_and(
+        return _execute_and(
             sql_dnf_predicates,
             node,
             limit,
             cache,
             fts_fields,
             embedding_server_address,
             select_username,
             select_userpswd,
+            table_w_ids,
+            llm_model_name,
+            max_verify
         )
     else:
         raise ValueError(
             "Expects sql to be in DNF, but is not: {}".format(
                 RawStream()(sql_dnf_predicates)
             )
         )
 
 
 def suql_execute(
     suql,
+    table_w_ids,
     fts_fields=[],
+    llm_model_name="gpt-3.5-turbo-0125",
+    max_verify=20,
     loggings="",
     disable_try_catch=False,
-    embedding_server_address=EMBEDDING_SERVER_ADDRESS,
+    embedding_server_address="http://127.0.0.1:8501",
     select_username="select_user",
     select_userpswd="select_user",
     create_username="creator_role",
     create_userpswd="creator_role",
 ):
     """
     Main entry point to the SUQL Python-based compiler.
 
-    Parameters:
-    `suql` (str): The to-be-executed suql query,
+    # Parameters:
+    `suql` (str): The to-be-executed suql query.
+    
+    `table_w_ids` (dict): A dictionary where each key is a table name, and each value is the corresponding
+        unique ID column name in this table, e.g., `table_w_ids = {"restaurants": "_id"}`, meaning that the
+        relevant tables to the SUQL compiler include only the `restaurants` table, which has unique ID column `_id`.
+        
     `fts_fields` (List[str], optional): Fields that should use PostgreSQL's Full Text Search (FTS) operators;
         The SUQL compiler would change certain string operators like "=" to use PostgreSQL's FTS operators.
         It uses `websearch_to_tsquery` and the `@@` operator to match against these fields.
-
+        
+    `llm_model_name` (str, optional): The LLM to be used by the SUQL compiler.
+        Defaults to `gpt-3.5-turbo-0125`.
+        
+    `max_verify` (str): For each LIMIT x clause, `max_verify * x` results will be retrieved together from
+        the embedding model for LLM to verify. Defaults to 20.
+        
     `loggings` (str, optional): Prefix for error case loggings. Errors are written to a "_suql_error_log.txt"
         file by default.
-    `disable_try_catch` (bool, optional): whether to disable try-catch (errors would directly propagate to caller)
-    `embedding_server_address` (str, optional): the embedding server address. Defaults to 'http://127.0.0.1:8501'
+        
+    `disable_try_catch` (bool, optional): whether to disable try-catch (errors would directly propagate to caller).
+    
+    `embedding_server_address` (str, optional): the embedding server address. Defaults to 'http://127.0.0.1:8501'.
+    
     `select_username` (str, optional): user name with select privilege in db. Defaults to "select_user".
+    
     `select_userpswd` (str, optional): above user's password with select privilege in db. Defaults to "select_user".
+    
     `create_username` (str, optional): user name with create privilege in db. Defaults to "creator_role".
+    
     `create_userpswd` (str, optional): above user's password with create privilege in db. Defaults to "creator_role".
 
-    Returns:
-    `results` (List[[*]]): A list of returned database results. Each inner list stores a row of returned result
-    `column_names` (List[str]): A list of database column names in the same order as `results`
-    `cache` (Dict()): Debugging information from the SUQL compiler
+    # Returns:
+    `results` (List[[*]]): A list of returned database results. Each inner list stores a row of returned result.
+    
+    `column_names` (List[str]): A list of database column names in the same order as `results`.
+    
+    `cache` (Dict()): Debugging information from the SUQL compiler.
 
-    Example:
+    # Example:
     ```
-    suql_execute("SELECT * FROM restaurants WHERE
-    answer(reviews, 'is this restaurant family-friendly?') = 'yes'", fts_fields=[("restaurants", "name")])
+    suql_execute(
+        "SELECT * FROM restaurants WHERE answer(reviews, 'is this restaurant family-friendly?') = 'yes'",
+        {"restaurants": "_id"},
+        fts_fields=[("restaurants", "name")])
     ```
 
     In restaurants, one would likely need to apply FTS on the name of the restaurants
     since for queries that search by name, e.g.:
     ```
     suql_execute("SELECT * FROM restaurants WHERE name = 'mcdonalds'", fts_fields=[("restaurants", "name")])
     ```
     Ideally, this query should match against all `Mcdonald's`, as opposed to just 'mcdonalds'.
     FTS helps with such cases.
     """
-    results, column_names, cache = suql_execute_single(
+    results, column_names, cache = _suql_execute_single(
         suql,
+        table_w_ids,
+        fts_fields,
+        llm_model_name,
+        max_verify,
         embedding_server_address,
         loggings,
         disable_try_catch,
-        fts_fields,
         select_username,
         select_userpswd,
         create_username,
         create_userpswd,
     )
     if results == []:
         return results, column_names, cache
@@ -1543,53 +1617,62 @@
         if all_no_results == False:
             break
 
     # TODO: handle cases to go to multiple projection fields, from hybridQA
     return results, column_names, cache
 
 
-def suql_execute_single(
+def _suql_execute_single(
     suql,
+    table_w_ids,
+    fts_fields,
+    llm_model_name,
+    max_verify,
     embedding_server_address,
     loggings,
     disable_try_catch,
-    fts_fields,
     select_username,
     select_userpswd,
     create_username,
     create_userpswd,
 ):
     results = []
     column_names = []
     cache = {}
 
     if disable_try_catch:
-        visitor = SelectVisitor(
+        visitor = _SelectVisitor(
             fts_fields,
             embedding_server_address,
             select_username,
             select_userpswd,
             create_username,
             create_userpswd,
+            table_w_ids,
+            llm_model_name,
+            max_verify
         )
         root = parse_sql(suql)
         visitor(root)
         second_sql = RawStream()(root)
         cache = visitor.serialize_cache()
 
         return execute_sql(second_sql, user=select_username, password=select_userpswd)
     else:
         try:
-            visitor = SelectVisitor(
+            visitor = _SelectVisitor(
                 fts_fields,
                 embedding_server_address,
                 select_username,
                 select_userpswd,
                 create_username,
                 create_userpswd,
+                table_w_ids,
+                llm_model_name,
+                max_verify
             )
             root = parse_sql(suql)
             visitor(root)
             second_sql = RawStream()(root)
             cache = visitor.serialize_cache()
 
             results, column_names, cache = execute_sql(
```

### Comparing `suql-1.0.0b0/src/suql/utils.py` & `suql-1.1.0a0/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0b0/src/suql.egg-info/PKG-INFO` & `suql-1.1.0a0/src/suql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.0.0b0
+Version: 1.1.0a0
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -62,15 +62,15 @@
 
 There are two main ways of installing the SUQL library.
 
 ## Install from `pip`
 
 Ideal for integrating the SUQL compiler in a larger codebase / system. See [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/install_pip.md) for details.
 
-## Install from source**
+## Install from source
 
 Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
 
 ## Agent tutorial
 
 Check out [conv_agent.md](https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more information on best practices for using SUQL to power your conversational agent.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.0.0b0 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.0a0 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
            ************ SSUUQQLL ((SSttrruuccttuurreedd aanndd UUnnssttrruuccttuurreedd QQuueerryy LLaanngguuaaggee))
                          _[[_aa_rr_XX_ii_vv_]]_[[_GG_ii_tt_hh_uu_bb_ _SS_tt_aa_rr_ss_]] ************
@@ -30,15 +30,15 @@
 text to be easily combined with structured constraints. Here is one high-level
 example: ![An example for using SUQL](https://github.com/stanford-oval/suql/
 blob/main/figures/figure2.png?raw=true) For more details, see our paper at
 https://arxiv.org/abs/2311.09818. # Installation / Usage tutorial There are two
 main ways of installing the SUQL library. ## Install from `pip` Ideal for
 integrating the SUQL compiler in a larger codebase / system. See
 [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/
-install_pip.md) for details. ## Install from source** Ideal for using this repo
+install_pip.md) for details. ## Install from source Ideal for using this repo
 to build a SUQL-powered conversational interface to your data out-of-the-box,
 like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See
 [docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_source.md) for details. ## Agent tutorial Check out [conv_agent.md]
 (https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more
 information on best practices for using SUQL to power your conversational
 agent. # Bugs / Contribution If you encounter a problem, first check
```

### Comparing `suql-1.0.0b0/src/suql.egg-info/SOURCES.txt` & `suql-1.1.0a0/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

