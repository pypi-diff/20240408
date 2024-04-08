# Comparing `tmp/myllm-4.8.0.tar.gz` & `tmp/myllm-4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myllm-4.8.0.tar", max compression
+gzip compressed data, was "myllm-4.8.1.tar", max compression
```

## Comparing `myllm-4.8.0.tar` & `myllm-4.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-06 07:37:08.382699 myllm-4.8.0/LICENSE
--rw-r--r--   0        0        0     3014 2024-04-06 07:37:08.382699 myllm-4.8.0/README.md
--rw-r--r--   0        0        0       95 2024-04-06 07:37:48.243262 myllm-4.8.0/myllm/__init__.py
--rw-r--r--   0        0        0      772 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/config.py
--rw-r--r--   0        0        0     3094 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/default_settings.toml
--rw-r--r--   0        0        0      131 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/__init__.py
--rw-r--r--   0        0        0     4643 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/client.py
--rw-r--r--   0        0        0     1986 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/g4f.py
--rw-r--r--   0        0        0     2193 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/not_working/gemini.py
--rw-r--r--   0        0        0     2308 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/not_working/petals.py
--rw-r--r--   0        0        0     2068 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/openai.py
--rw-r--r--   0        0        0     7197 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/main.py
--rw-r--r--   0        0        0     3928 2024-04-06 07:37:48.239262 myllm-4.8.0/pyproject.toml
--rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 myllm-4.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-08 04:53:13.960209 myllm-4.8.1/LICENSE
+-rw-r--r--   0        0        0     3014 2024-04-08 04:53:13.960209 myllm-4.8.1/README.md
+-rw-r--r--   0        0        0       95 2024-04-08 04:53:53.336490 myllm-4.8.1/myllm/__init__.py
+-rw-r--r--   0        0        0      772 2024-04-08 04:53:13.960209 myllm-4.8.1/myllm/config.py
+-rw-r--r--   0        0        0     3094 2024-04-08 04:53:13.964210 myllm-4.8.1/myllm/default_settings.toml
+-rw-r--r--   0        0        0      131 2024-04-08 04:53:13.964210 myllm-4.8.1/myllm/handler/__init__.py
+-rw-r--r--   0        0        0     4643 2024-04-08 04:53:13.964210 myllm-4.8.1/myllm/handler/client.py
+-rw-r--r--   0        0        0     1986 2024-04-08 04:53:13.964210 myllm-4.8.1/myllm/handler/g4f.py
+-rw-r--r--   0        0        0     2193 2024-04-08 04:53:13.964210 myllm-4.8.1/myllm/handler/not_working/gemini.py
+-rw-r--r--   0        0        0     2308 2024-04-08 04:53:13.964210 myllm-4.8.1/myllm/handler/not_working/petals.py
+-rw-r--r--   0        0        0     2068 2024-04-08 04:53:13.964210 myllm-4.8.1/myllm/handler/openai.py
+-rw-r--r--   0        0        0     7197 2024-04-08 04:53:13.964210 myllm-4.8.1/myllm/main.py
+-rw-r--r--   0        0        0     3930 2024-04-08 04:53:53.336490 myllm-4.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 myllm-4.8.1/PKG-INFO
```

### Comparing `myllm-4.8.0/LICENSE` & `myllm-4.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myllm-4.8.0/README.md` & `myllm-4.8.1/README.md`

 * *Files identical despite different names*

### Comparing `myllm-4.8.0/myllm/config.py` & `myllm-4.8.1/myllm/config.py`

 * *Files identical despite different names*

### Comparing `myllm-4.8.0/myllm/default_settings.toml` & `myllm-4.8.1/myllm/default_settings.toml`

 * *Files identical despite different names*

### Comparing `myllm-4.8.0/myllm/handler/client.py` & `myllm-4.8.1/myllm/handler/client.py`

 * *Files identical despite different names*

### Comparing `myllm-4.8.0/myllm/handler/g4f.py` & `myllm-4.8.1/myllm/handler/g4f.py`

 * *Files identical despite different names*

### Comparing `myllm-4.8.0/myllm/handler/not_working/gemini.py` & `myllm-4.8.1/myllm/handler/not_working/gemini.py`

 * *Files identical despite different names*

### Comparing `myllm-4.8.0/myllm/handler/not_working/petals.py` & `myllm-4.8.1/myllm/handler/not_working/petals.py`

 * *Files identical despite different names*

### Comparing `myllm-4.8.0/myllm/handler/openai.py` & `myllm-4.8.1/myllm/handler/openai.py`

 * *Files identical despite different names*

### Comparing `myllm-4.8.0/myllm/main.py` & `myllm-4.8.1/myllm/main.py`

 * *Files identical despite different names*

### Comparing `myllm-4.8.0/pyproject.toml` & `myllm-4.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MyLLM"
-version = "4.8.0"
+version = "4.8.1"
 description = "A python package to interact with llm model supported by g4f and langchain."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["chatgpt","llm","ai","llama","ai", "g4f", "freegpt"]
 packages = [
     {include = "myllm"}
@@ -23,15 +23,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = ">=0.95.2"
 uvicorn = ">=0.22.0"
 dynaconf = ">=3.2.0"
 loguru = ">=0.6.0"
 httpx = ">=0.24.1"
-g4f = "0.2.8.0"
+g4f = "0.2.8.2"
 js2py = "^0.74"
 PyExecJS2="1.6.1"
 curl_cffi = "0.6.2"
 Brotli = "1.1.0"
 openai = "1.16.2"
 # petals = "2.2.0.post1"
 # transformers = "4.32"
@@ -165,27 +165,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `myllm-4.8.0/PKG-INFO` & `myllm-4.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyLLM
-Version: 4.8.0
+Version: 4.8.1
 Summary: A python package to interact with llm model supported by g4f and langchain.
 License: MIT
 Keywords: chatgpt,llm,ai,llama,ai,g4f,freegpt
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Brotli (==1.1.0)
 Requires-Dist: PyExecJS2 (==1.6.1)
 Requires-Dist: curl_cffi (==0.6.2)
 Requires-Dist: dynaconf (>=3.2.0)
 Requires-Dist: fastapi (>=0.95.2)
-Requires-Dist: g4f (==0.2.8.0)
+Requires-Dist: g4f (==0.2.8.2)
 Requires-Dist: httpx (>=0.24.1)
 Requires-Dist: js2py (>=0.74,<0.75)
 Requires-Dist: loguru (>=0.6.0)
 Requires-Dist: openai (==1.16.2)
 Requires-Dist: uvicorn (>=0.22.0)
 Project-URL: Changelog, https://github.com/mraniki/MyLLM/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/MyLLM/issues
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: MyLLM Version: 4.8.0 Summary: A python package to
+Metadata-Version: 2.1 Name: MyLLM Version: 4.8.1 Summary: A python package to
 interact with llm model supported by g4f and langchain. License: MIT Keywords:
 chatgpt,llm,ai,llama,ai,g4f,freegpt Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: Brotli (==1.1.0) Requires-Dist:
 PyExecJS2 (==1.6.1) Requires-Dist: curl_cffi (==0.6.2) Requires-Dist: dynaconf
-(>=3.2.0) Requires-Dist: fastapi (>=0.95.2) Requires-Dist: g4f (==0.2.8.0)
+(>=3.2.0) Requires-Dist: fastapi (>=0.95.2) Requires-Dist: g4f (==0.2.8.2)
 Requires-Dist: httpx (>=0.24.1) Requires-Dist: js2py (>=0.74,<0.75) Requires-
 Dist: loguru (>=0.6.0) Requires-Dist: openai (==1.16.2) Requires-Dist: uvicorn
 (>=0.22.0) Project-URL: Changelog, https://github.com/mraniki/MyLLM/blob/dev/
 CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/MyLLM/issues
 Project-URL: Support, https://github.com/mraniki/MyLLM/discussions Description-
 Content-Type: text/markdown
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_W_i_k_i_-
```

