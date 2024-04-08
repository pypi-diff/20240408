# Comparing `tmp/ragtime-0.0.25.tar.gz` & `tmp/ragtime-0.0.26.tar.gz`

## Comparing `ragtime-0.0.25.tar` & `ragtime-0.0.26.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 ragtime-0.0.25/CONTRIBUTING.md
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.25/deploy/deploy.py
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.25/img/Ragtime_logo.png
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/__init__.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/api.py
--rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/config.py
--rw-r--r--   0        0        0    19120 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/expe.py
--rw-r--r--   0        0        0    38298 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/generators.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/base_folder/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/base_folder/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/base_folder/README.md
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/base_folder/classes.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/base_folder/main.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/base_folder/res/html_templates/basic_template.jinja
--rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
--rw-r--r--   0        0        0    31095 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
--rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.25/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 ragtime-0.0.25/tests/main.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.25/tests/test_quest.json
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ragtime-0.0.25/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.25/LICENSE
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 ragtime-0.0.25/README.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ragtime-0.0.25/pyproject.toml
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 ragtime-0.0.25/PKG-INFO
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 ragtime-0.0.26/CONTRIBUTING.md
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.26/deploy/deploy.py
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.26/img/Ragtime_logo.png
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/api.py
+-rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/config.py
+-rw-r--r--   0        0        0    19120 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/expe.py
+-rw-r--r--   0        0        0    38773 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/generators.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/README.md
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/classes.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/main.py
+-rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/res/html_templates/basic_template.jinja
+-rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
+-rw-r--r--   0        0        0    31095 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
+-rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 ragtime-0.0.26/tests/main.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.26/tests/test_quest.json
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ragtime-0.0.26/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.26/LICENSE
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 ragtime-0.0.26/README.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ragtime-0.0.26/pyproject.toml
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 ragtime-0.0.26/PKG-INFO
```

### Comparing `ragtime-0.0.25/img/Ragtime_logo.png` & `ragtime-0.0.26/img/Ragtime_logo.png`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/__init__.py` & `ragtime-0.0.26/src/ragtime/__init__.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/api.py` & `ragtime-0.0.26/src/ragtime/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     REQ_POST: requests.post,
     REQ_PUT: requests.put,
     REQ_DELETE: requests.delete,
     }
 
 ################
 # call
-@retry(Exception, tries=5, delay=3, jitter=(0,3))
+# @retry(Exception, tries=5, delay=3, jitter=(0,3))
 def call(a_req_type: str, a_url: str, **kwargs) -> Response:
     """Calls API and manages errors
     Args:
         a_req_type: type of request (GET, POST, PUT, DELETE)
         a_url
         *args: variable number of extra argument
         **kwargs: variable number of keyword arguments
```

### Comparing `ragtime-0.0.25/src/ragtime/config.py` & `ragtime-0.0.26/src/ragtime/config.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/expe.py` & `ragtime-0.0.26/src/ragtime/expe.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/generators.py` & `ragtime-0.0.26/src/ragtime/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,16 +453,16 @@
         """Helper function to get the first LLM when only one is provided (like for EvalGenerator and FactGenerator)"""
         if self.llms:
             return self.llms[0]
         else:
             return None
     
     def generate(self, expe:Expe, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, 
-                 only_llms:list[str] = None, save_every:int=0):
-        """Main method calling "gen_for_qa" for each QA in an Expe.
+                 only_llms:list[str] = None, save_every:int=0) -> bool:
+        """Main method calling "gen_for_qa" for each QA in an Expe. Returns False if completed with error, True otherwise
         The main step in generation are :
         - beginning: start of the process - when start_from=beginning, the whole process is executed
 	    - chunks: only for Answer generation - chunk retrieval, if a Retriever is associated with the Answer Generator object
         Takes a Question and returns the Chunks
         - prompt: prompt generation, either directly using the question or with the chunks if any
         Takes a Question + optional Chunks and return a Prompt
         - llm: calling the LLM(s) with the generated prompts
@@ -485,14 +485,16 @@
                 logger.info(f'*** {self.__class__.__name__} for question "{qa.question.text}"')
                 self.gen_for_qa(qa=qa, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms)
                 logger.info(f'End question "{qa.question.text}"')
                 if save_every and (num_q % save_every == 0): expe.save_to_json()
         except Exception as e:
             logger.exception(f"Exception caught - saving what has been done so far:\n{e}")
             expe.save_temp(name=f"Stopped_at_{num_q}_of_{nb_q}_")
+            return False
+        return True
 
     def write_chunks(self, qa:QA):
         """Write chunks in the current qa if a Retriever has been given when creating the object. Ignore otherwise"""
         raise NotImplementedError('Must implement this if you want to use it!')
     
     @abstractmethod
     def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, 
@@ -674,31 +676,39 @@
                                     answer_facts=ans_facts, gold_facts=qa.facts)
 
             # save previous human eval if any
             if prev_eval and prev_eval.human: ans.eval.human = prev_eval.human
 
 def gen_Answers(folder_in:Path, folder_out:Path, json_file: Path|str, prompter:Prompter, llm_names:list[str], retriever:Retriever=None, 
                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
-  """Standard function to generate answers"""
+  """Standard function to generate answers - returns the updated Expe or None if an error occurred"""
   expe:Expe = Expe(json_path=folder_in / json_file)
   ans_gen:AnsGenerator = AnsGenerator(retriever=retriever, llm_names=llm_names, prompter=prompter)
-  ans_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms)
-  expe.save_to_json(path=folder_out / json_file)
-  return expe
+  if ans_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms,
+                      save_every=save_every):
+    expe.save_to_json(path=folder_out / json_file)
+    return expe
+  else:
+    return None
+  
 
 def gen_Facts(folder_in:Path, folder_out:Path, json_file: Path|str, prompter:Prompter, llm_names:list[str],
                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
-  """Standard function to generate facts"""
+  """Standard function to generate facts - returns the updated Expe or None if an error occurred"""
   expe:Expe = Expe(json_path=folder_in / json_file)
   fact_gen:FactGenerator = FactGenerator(llm_names=llm_names, prompter=prompter)
-  fact_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms)
-  expe.save_to_json(path=folder_out / json_file)
-  return expe
+  if fact_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every):
+    expe.save_to_json(path=folder_out / json_file)
+    return expe
+  else:
+    return None
 
 def gen_Evals(folder_in:Path, folder_out:Path, json_file: Path|str, prompter:Prompter, llm_names:list[str],
                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
-  """Standard function to generate evals"""
+  """Standard function to generate evals - returns the updated Expe or None if an error occurred"""
   expe:Expe = Expe(json_path=folder_in / json_file)
   eval_gen:EvalGenerator = EvalGenerator(llm_names=llm_names, prompter=prompter)
-  eval_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms)
-  expe.save_to_json(path=folder_out / json_file)
-  return expe
+  if eval_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every):
+    expe.save_to_json(path=folder_out / json_file)
+    return expe
+  else:
+    return None
```

### Comparing `ragtime-0.0.25/src/ragtime/base_folder/.gitignore` & `ragtime-0.0.26/src/ragtime/base_folder/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/base_folder/LICENSE` & `ragtime-0.0.26/src/ragtime/base_folder/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/base_folder/classes.py` & `ragtime-0.0.26/src/ragtime/base_folder/classes.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx` & `ragtime-0.0.26/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/base_folder/res/html_templates/basic_template.jinja` & `ragtime-0.0.26/src/ragtime/base_folder/res/html_templates/basic_template.jinja`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx` & `ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx` & `ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx` & `ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx` & `ragtime-0.0.26/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/tests/main.py` & `ragtime-0.0.26/tests/main.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/tests/test_quest.json` & `ragtime-0.0.26/tests/test_quest.json`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/.gitignore` & `ragtime-0.0.26/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/LICENSE` & `ragtime-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.25/README.md` & `ragtime-0.0.26/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,20 @@
 - `Eval`: contains a `human` field to store human evaluation of the answer as well as a `auto` field when the evaluation is done automatically. In this case, it also contains an `LLMAnswer` object related to the automatic evaluation
 
 Almost every object in Ragtime 🎹 has a `meta` field, which is a dictionnary where you can store all the extra data you need for your specific use case.
 
 # Examples
 You can now go to [ragtime-projects](https://github.com/recitalAI/ragtime-projects) to see examples of Ragtime 🎹 in action!
 
-# Setting the API keys
-API keys are stored in environment variables locally on your computer.
-## Windows
-If you are using Windows, you should first set the API keys values as:
+# Troubleshooting
+## Setting the API keys on Windows
+API keys are stored in environment variables locally on your computer. If you are using Windows, you should first set the API keys values as:
 ```shell
 setx OPENAI_API_KEY sk-....
 ```
 The list of environment variable names to set, depending on the APIs you need to access, is given in the [LiteLLM documentation](https://litellm.vercel.app/docs/providers).
 
-Once the keys are set, just call `ragtime.config.init_API_keys` with the list of environment variables to make accessible to Python, for instance `init_API_keys(['OPENAI_API_KEY'])`.
+Once the keys are set, just call `ragtime.config.init_API_keys` with the list of environment variables to make accessible to Python, for instance `init_API_keys(['OPENAI_API_KEY'])`.
+
+## Using Google LLMs
+Execute what's indicated in the [LiteLLM documentation](https://litellm.vercel.app/docs/providers/vertex#gemini-pro).
+Also make sure your project has `Vertex AI` API enabled.
```

### Comparing `ragtime-0.0.25/pyproject.toml` & `ragtime-0.0.26/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ragtime"
-version = "0.0.25"
+version = "0.0.26"
 
 authors = [
   { name="Gilles Moyse", email="gilles@recital.ai" },
 ]
 maintainers = [
   { name="reciTAL", email="ragtime@recital.ai" },
 ]
```

### Comparing `ragtime-0.0.25/PKG-INFO` & `ragtime-0.0.26/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragtime
-Version: 0.0.25
+Version: 0.0.26
 Summary: Ragtime 🎹 is an LLMOps framework to automatically evaluate Retrieval Augmented Generation (RAG) systems and compare different RAGs / LLMs
 Project-URL: Homepage, https://github.com/recitalAI/ragtime-package
 Project-URL: Issues, https://github.com/recitalAI/ragtime-package/issues
 Author-email: Gilles Moyse <gilles@recital.ai>
 Maintainer-email: reciTAL <ragtime@recital.ai>
 License: MIT License
         
@@ -74,17 +74,20 @@
 - `Eval`: contains a `human` field to store human evaluation of the answer as well as a `auto` field when the evaluation is done automatically. In this case, it also contains an `LLMAnswer` object related to the automatic evaluation
 
 Almost every object in Ragtime 🎹 has a `meta` field, which is a dictionnary where you can store all the extra data you need for your specific use case.
 
 # Examples
 You can now go to [ragtime-projects](https://github.com/recitalAI/ragtime-projects) to see examples of Ragtime 🎹 in action!
 
-# Setting the API keys
-API keys are stored in environment variables locally on your computer.
-## Windows
-If you are using Windows, you should first set the API keys values as:
+# Troubleshooting
+## Setting the API keys on Windows
+API keys are stored in environment variables locally on your computer. If you are using Windows, you should first set the API keys values as:
 ```shell
 setx OPENAI_API_KEY sk-....
 ```
 The list of environment variable names to set, depending on the APIs you need to access, is given in the [LiteLLM documentation](https://litellm.vercel.app/docs/providers).
 
-Once the keys are set, just call `ragtime.config.init_API_keys` with the list of environment variables to make accessible to Python, for instance `init_API_keys(['OPENAI_API_KEY'])`.
+Once the keys are set, just call `ragtime.config.init_API_keys` with the list of environment variables to make accessible to Python, for instance `init_API_keys(['OPENAI_API_KEY'])`.
+
+## Using Google LLMs
+Execute what's indicated in the [LiteLLM documentation](https://litellm.vercel.app/docs/providers/vertex#gemini-pro).
+Also make sure your project has `Vertex AI` API enabled.
```

