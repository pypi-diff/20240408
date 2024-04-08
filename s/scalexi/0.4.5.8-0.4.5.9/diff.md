# Comparing `tmp/scalexi-0.4.5.8.tar.gz` & `tmp/scalexi-0.4.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalexi-0.4.5.8.tar", last modified: Mon Mar 11 15:35:00 2024, max compression
+gzip compressed data, was "scalexi-0.4.5.9.tar", last modified: Fri Mar 15 11:28:41 2024, max compression
```

## Comparing `scalexi-0.4.5.8.tar` & `scalexi-0.4.5.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-11 15:35:00.175089 scalexi-0.4.5.8/
--rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.5.8/LICENSE
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-03-11 15:35:00.174962 scalexi-0.4.5.8/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.5.8/README.md
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-11 15:35:00.171394 scalexi-0.4.5.8/scalexi/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.8/scalexi/__init__.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-11 15:35:00.172327 scalexi-0.4.5.8/scalexi/data/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.8/scalexi/data/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.5.8/scalexi/data/openai_pricing.json
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-11 15:35:00.172589 scalexi-0.4.5.8/scalexi/dataset_generation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.8/scalexi/dataset_generation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.5.8/scalexi/dataset_generation/prompt_completion.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-11 15:35:00.172979 scalexi-0.4.5.8/scalexi/document_loaders/
--rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.5.8/scalexi/document_loaders/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.5.8/scalexi/document_loaders/context_loaders.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     1142 2024-02-03 12:24:33.000000 scalexi-0.4.5.8/scalexi/document_loaders/pdf_loaders.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-11 15:35:00.173398 scalexi-0.4.5.8/scalexi/llm/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.8/scalexi/llm/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.5.8/scalexi/llm/google_gemini.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.5.8/scalexi/llm/openai_gpt.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-11 15:35:00.173726 scalexi-0.4.5.8/scalexi/llm_evaluation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.8/scalexi/llm_evaluation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.5.8/scalexi/llm_evaluation/evaluate.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-11 15:35:00.174243 scalexi-0.4.5.8/scalexi/openai/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.8/scalexi/openai/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.5.8/scalexi/openai/fine_tuning_api.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    29231 2024-03-11 14:47:48.000000 scalexi-0.4.5.8/scalexi/openai/pricing.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-11 15:35:00.174713 scalexi-0.4.5.8/scalexi/utilities/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.8/scalexi/utilities/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.5.8/scalexi/utilities/data_formatter.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.5.8/scalexi/utilities/logger.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-11 15:35:00.172094 scalexi-0.4.5.8/scalexi.egg-info/
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-03-11 15:35:00.000000 scalexi-0.4.5.8/scalexi.egg-info/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)      796 2024-03-11 15:35:00.000000 scalexi-0.4.5.8/scalexi.egg-info/SOURCES.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-03-11 15:35:00.000000 scalexi-0.4.5.8/scalexi.egg-info/dependency_links.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)      122 2024-03-11 15:35:00.000000 scalexi-0.4.5.8/scalexi.egg-info/requires.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-03-11 15:35:00.000000 scalexi-0.4.5.8/scalexi.egg-info/top_level.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-03-11 15:35:00.175125 scalexi-0.4.5.8/setup.cfg
--rw-r--r--   0 akoubaa    (501) staff       (20)     5384 2024-03-11 15:34:56.000000 scalexi-0.4.5.8/setup.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.465899 scalexi-0.4.5.9/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.5.9/LICENSE
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-03-15 11:28:41.465785 scalexi-0.4.5.9/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.5.9/README.md
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.462472 scalexi-0.4.5.9/scalexi/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/__init__.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.463344 scalexi-0.4.5.9/scalexi/data/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/data/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.5.9/scalexi/data/openai_pricing.json
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.463734 scalexi-0.4.5.9/scalexi/dataset_generation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/dataset_generation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.5.9/scalexi/dataset_generation/prompt_completion.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.464129 scalexi-0.4.5.9/scalexi/document_loaders/
+-rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/document_loaders/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.5.9/scalexi/document_loaders/context_loaders.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     1142 2024-02-03 12:24:33.000000 scalexi-0.4.5.9/scalexi/document_loaders/pdf_loaders.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.464539 scalexi-0.4.5.9/scalexi/llm/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/llm/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.5.9/scalexi/llm/google_gemini.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.5.9/scalexi/llm/openai_gpt.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.464826 scalexi-0.4.5.9/scalexi/llm_evaluation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/llm_evaluation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.5.9/scalexi/llm_evaluation/evaluate.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.465210 scalexi-0.4.5.9/scalexi/openai/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/openai/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.5.9/scalexi/openai/fine_tuning_api.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    30995 2024-03-15 11:25:33.000000 scalexi-0.4.5.9/scalexi/openai/pricing.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.465572 scalexi-0.4.5.9/scalexi/utilities/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.5.9/scalexi/utilities/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.5.9/scalexi/utilities/data_formatter.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.5.9/scalexi/utilities/logger.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-03-15 11:28:41.463086 scalexi-0.4.5.9/scalexi.egg-info/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-03-15 11:28:41.000000 scalexi-0.4.5.9/scalexi.egg-info/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)      796 2024-03-15 11:28:41.000000 scalexi-0.4.5.9/scalexi.egg-info/SOURCES.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-03-15 11:28:41.000000 scalexi-0.4.5.9/scalexi.egg-info/dependency_links.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)      122 2024-03-15 11:28:41.000000 scalexi-0.4.5.9/scalexi.egg-info/requires.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-03-15 11:28:41.000000 scalexi-0.4.5.9/scalexi.egg-info/top_level.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-03-15 11:28:41.465939 scalexi-0.4.5.9/setup.cfg
+-rw-r--r--   0 akoubaa    (501) staff       (20)     5384 2024-03-15 11:28:20.000000 scalexi-0.4.5.9/setup.py
```

### Comparing `scalexi-0.4.5.8/LICENSE` & `scalexi-0.4.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/PKG-INFO` & `scalexi-0.4.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.5.8
+Version: 0.4.5.9
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.5.8/README.md` & `scalexi-0.4.5.9/README.md`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/scalexi/data/openai_pricing.json` & `scalexi-0.4.5.9/scalexi/data/openai_pricing.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/scalexi/dataset_generation/prompt_completion.py` & `scalexi-0.4.5.9/scalexi/dataset_generation/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/scalexi/document_loaders/context_loaders.py` & `scalexi-0.4.5.9/scalexi/document_loaders/context_loaders.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/scalexi/document_loaders/pdf_loaders.py` & `scalexi-0.4.5.9/scalexi/document_loaders/pdf_loaders.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/scalexi/llm/google_gemini.py` & `scalexi-0.4.5.9/scalexi/llm/google_gemini.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/scalexi/llm/openai_gpt.py` & `scalexi-0.4.5.9/scalexi/llm/openai_gpt.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/scalexi/llm_evaluation/evaluate.py` & `scalexi-0.4.5.9/scalexi/llm_evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/scalexi/openai/fine_tuning_api.py` & `scalexi-0.4.5.9/scalexi/openai/fine_tuning_api.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/scalexi/openai/pricing.py` & `scalexi-0.4.5.9/scalexi/openai/pricing.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,14 +319,36 @@
             if model_name in models:
                 return models[model_name]
             else:
                 raise ValueError(f"Model '{model_name}' not found in base models pricing.")
         else:
             return models
 
+    def extract_response_and_token_usage(response):
+        """
+        Extracts the content of the response and token usage from the response message.
+
+        Parameters:
+        - response (dict): The response message received.
+
+        Returns:
+        - tuple: A tuple containing the content of the response and the token usage dictionary.
+        """
+        # Extract the content of the response
+        content = response.choices[0].message.content
+        
+        # Extract the token usage
+        token_usage = {
+            "completion_tokens": response.usage.completion_tokens,
+            "prompt_tokens": response.usage.prompt_tokens,
+            "total_tokens": response.usage.total_tokens
+        }
+        
+        return content, token_usage
+
 
     def get_image_model_pricing(self, model_name=None):
         """
         Retrieves pricing information for image models from the stored pricing data.
 
         This method is designed to provide users with pricing details for various image generation models offered by OpenAI. 
         If a specific model or category name is given, it returns the pricing specific to that model or category. 
@@ -636,7 +658,33 @@
             # Assuming the model 'gpt-3.5-turbo-0613', this returns the total token count for the dataset.
         """
 
         messages = self.load_dataset(dataset_path)
         return self.calculate_token_usage_for_messages(messages, model=model)
     
 
+    def extract_response_and_token_usage_and_cost(self, response, model_name):
+        """
+        Extracts the content of the response, token usage, and estimates the inference cost.
+
+        Parameters:
+        - response (dict): The response message received.
+
+        Returns:
+        - tuple: A tuple containing the content of the response, the token usage dictionary, and the estimated cost.
+        """
+        # Extract the content and token usage
+        content = response.choices[0].message.content
+        print('content:', content)
+        token_usage = {
+            "completion_tokens": response.usage.completion_tokens,
+            "prompt_tokens": response.usage.prompt_tokens,
+            "total_tokens": response.usage.total_tokens
+        }
+        print(token_usage)
+        
+        # Estimate the cost
+        cost = self.estimate_inference_cost(token_usage['prompt_tokens'], token_usage['completion_tokens'], model_name)
+        
+        return content, token_usage, cost
+    
+
```

### Comparing `scalexi-0.4.5.8/scalexi/utilities/data_formatter.py` & `scalexi-0.4.5.9/scalexi/utilities/data_formatter.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/scalexi/utilities/logger.py` & `scalexi-0.4.5.9/scalexi/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/scalexi.egg-info/PKG-INFO` & `scalexi-0.4.5.9/scalexi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.5.8
+Version: 0.4.5.9
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.5.8/scalexi.egg-info/SOURCES.txt` & `scalexi-0.4.5.9/scalexi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.5.8/setup.py` & `scalexi-0.4.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="scalexi",
-    version="0.4.5.8",
+    version="0.4.5.9",
     packages=find_packages(),
     include_package_data=True,
     package_data={'scalexi': ['data/*']},
     install_requires=[
         "pandas",  # Add any package dependencies here
         "openai>=1.10.0", #this package is not compatible with earlier versions of openai
         "sphinx",   # Add any other dependencies as needed
```

