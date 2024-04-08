# Comparing `tmp/aibridge_test-0.2.7.tar.gz` & `tmp/aibridge_test-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.2.7.tar", last modified: Fri Apr  5 09:42:12 2024, max compression
+gzip compressed data, was "aibridge_test-0.2.8.tar", last modified: Mon Apr  8 07:59:08 2024, max compression
```

## Comparing `aibridge_test-0.2.7.tar` & `aibridge_test-0.2.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.274545 aibridge_test-0.2.7/
-drwxrwxrwx   0        0        0        0 2024-04-05 09:42:11.957546 aibridge_test-0.2.7/AIBridge/
--rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.2.7/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.042545 aibridge_test-0.2.7/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     8944 2024-04-02 05:11:26.000000 aibridge_test-0.2.7/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0    12813 2024-04-04 11:48:13.000000 aibridge_test-0.2.7/AIBridge/ai_services/anthropic_ai.py
--rw-rw-rw-   0        0        0    11900 2024-04-05 09:25:51.000000 aibridge_test-0.2.7/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    14053 2024-04-04 11:46:45.000000 aibridge_test-0.2.7/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.7/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    11525 2024-04-04 09:42:06.000000 aibridge_test-0.2.7/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.7/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.2.7/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.2.7/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.057546 aibridge_test-0.2.7/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     7564 2024-04-05 09:34:27.000000 aibridge_test-0.2.7/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.2.7/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.091546 aibridge_test-0.2.7/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.109542 aibridge_test-0.2.7/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.2.7/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.133544 aibridge_test-0.2.7/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.2.7/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.2.7/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.151561 aibridge_test-0.2.7/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.174552 aibridge_test-0.2.7/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.2.7/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/LICENSE
--rw-rw-rw-   0        0        0    21534 2024-04-05 09:42:12.270546 aibridge_test-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 09:42:12.258543 aibridge_test-0.2.7/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21534 2024-04-05 09:42:11.000000 aibridge_test-0.2.7/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2024-04-05 09:42:11.000000 aibridge_test-0.2.7/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 09:42:11.000000 aibridge_test-0.2.7/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2024-04-05 09:42:11.000000 aibridge_test-0.2.7/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-05 09:42:11.000000 aibridge_test-0.2.7/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 09:42:12.275545 aibridge_test-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     2863 2024-04-05 08:20:15.000000 aibridge_test-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.884324 aibridge_test-0.2.8/
+drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.594322 aibridge_test-0.2.8/AIBridge/
+-rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.2.8/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.668323 aibridge_test-0.2.8/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     8944 2024-04-02 05:11:26.000000 aibridge_test-0.2.8/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0    13216 2024-04-08 07:03:19.000000 aibridge_test-0.2.8/AIBridge/ai_services/anthropic_ai.py
+-rw-rw-rw-   0        0        0    11900 2024-04-05 09:25:51.000000 aibridge_test-0.2.8/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    14053 2024-04-04 11:46:45.000000 aibridge_test-0.2.8/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.8/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11525 2024-04-04 09:42:06.000000 aibridge_test-0.2.8/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.8/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.2.8/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.2.8/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.694322 aibridge_test-0.2.8/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     7561 2024-04-08 06:59:23.000000 aibridge_test-0.2.8/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.2.8/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.727323 aibridge_test-0.2.8/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.744325 aibridge_test-0.2.8/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.2.8/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.760326 aibridge_test-0.2.8/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.2.8/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.2.8/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.777324 aibridge_test-0.2.8/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.798323 aibridge_test-0.2.8/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.2.8/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0    21534 2024-04-08 07:59:08.881330 aibridge_test-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.879331 aibridge_test-0.2.8/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21534 2024-04-08 07:59:08.000000 aibridge_test-0.2.8/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-04-08 07:59:08.000000 aibridge_test-0.2.8/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 07:59:08.000000 aibridge_test-0.2.8/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2024-04-08 07:59:08.000000 aibridge_test-0.2.8/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 07:59:08.000000 aibridge_test-0.2.8/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 07:59:08.885325 aibridge_test-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     2863 2024-04-08 07:57:56.000000 aibridge_test-0.2.8/setup.py
```

### Comparing `aibridge_test-0.2.7/AIBridge/__init__.py` & `aibridge_test-0.2.8/AIBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.2.8/AIBridge/ai_services/ai21labs_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.2.8/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/anthropic_ai.py` & `aibridge_test-0.2.8/AIBridge/ai_services/anthropic_ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,15 @@
                     elif _formatter == "json":
                         schema = json.loads(format_structure[index])
                     functions = (
                         AnthropicsFunctionCall.construct_format_tool_for_claude_prompt(
                             parameters=schema
                         )
                     )
+                    print(functions)
                     response = self.execute_prompt_function_calling(
                         api_key=api_key,
                         model=model,
                         messages=message_data,
                         n=variation_count,
                         functions_call=functions,
                         max_tokens=max_tokens,
@@ -259,19 +260,25 @@
                 print(response)
                 tokens = response.usage.input_tokens + response.usage.output_tokens
                 token_used = token_used + tokens
                 for index, res in enumerate(response.content):
                     content = res.text
                     if func_call:
                         json_content = IntoJson.xml_to_json(content)
-                        print(json_content)
                         content = json_content["function_calls"][0]["invoke"][
                             "parameters"
                         ]
                         if isinstance(content, dict):
+                            for key, value in content.items():
+                                if isinstance(value, str):
+                                    try:
+                                        new_val = json.loads(value)
+                                        content[key] = new_val
+                                    except json.JSONDecodeError:
+                                        ...
                             content = json.dumps(content)
 
                     if output_format:
                         try:
                             if _formatter == "csv":
                                 content = FromJson.json_to_csv(json.loads(content))
                             elif _formatter == "xml":
```

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.2.8/AIBridge/ai_services/cohere_llm.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.2.8/AIBridge/ai_services/geminin_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.2.8/AIBridge/ai_services/image_optimisaton.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.2.8/AIBridge/ai_services/openai_images.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.2.8/AIBridge/ai_services/openai_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.2.8/AIBridge/ai_services/palm_chat.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.2.8/AIBridge/ai_services/palm_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/process_mq.py` & `aibridge_test-0.2.8/AIBridge/ai_services/process_mq.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.2.8/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/constant/common.py` & `aibridge_test-0.2.8/AIBridge/constant/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                 if isinstance(value, dict):
                     j_type = "object"
                     key_dict += (
                         f"<name>{key}</name>\n<type>{j_type}</type>\n"
                         + create_function_call(value)
                     )
                 elif isinstance(value, list):
-                    type_ = ("array",)
+                    type_ = "array"
                     key_dict += f"<name>{key}</name>\n<type>{type_}</type>"
 
                     if value:
                         if isinstance(value[0], str):
                             key_dict += f"\n<description>{value[0]}</description>\n"
                         elif isinstance(value[0], dict):
                             key_dict += create_function_call(value[0])
```

### Comparing `aibridge_test-0.2.7/AIBridge/constant/constant.py` & `aibridge_test-0.2.8/AIBridge/constant/constant.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/database/db_layer.py` & `aibridge_test-0.2.8/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/database/no_sql_service.py` & `aibridge_test-0.2.8/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/database/session.py` & `aibridge_test-0.2.8/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/database/sql_service.py` & `aibridge_test-0.2.8/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/exceptions.py` & `aibridge_test-0.2.8/AIBridge/exceptions.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/output_validation/convertors.py` & `aibridge_test-0.2.8/AIBridge/output_validation/convertors.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/output_validation/validations.py` & `aibridge_test-0.2.8/AIBridge/output_validation/validations.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.2.8/AIBridge/prompts/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.2.8/AIBridge/prompts/prompts_save.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.2.8/AIBridge/prompts/prompts_varibales.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.2.8/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.2.8/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.2.8/AIBridge/queue_integration/response_class.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/AIBridge/setconfig.py` & `aibridge_test-0.2.8/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/LICENSE` & `aibridge_test-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/PKG-INFO` & `aibridge_test-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.7
+Version: 0.2.8
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.2.7/README.md` & `aibridge_test-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.2.8/aibridge_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.7
+Version: 0.2.8
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.2.7/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.2.8/aibridge_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.7/setup.py` & `aibridge_test-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.2.7"
+VERSION = "0.2.8"
 REQUIRED = [
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
```

