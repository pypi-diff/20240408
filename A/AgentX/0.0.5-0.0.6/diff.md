# Comparing `tmp/AgentX-0.0.5.tar.gz` & `tmp/AgentX-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AgentX-0.0.5.tar", last modified: Wed Apr  3 14:21:39 2024, max compression
+gzip compressed data, was "AgentX-0.0.6.tar", last modified: Mon Apr  8 08:26:36 2024, max compression
```

## Comparing `AgentX-0.0.5.tar` & `AgentX-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:21:39.551454 AgentX-0.0.5/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1076 2024-01-16 11:44:18.000000 AgentX-0.0.5/LICENSE
--rw-r--r--   0 erfan     (1000) erfan     (1000)     4428 2024-04-03 14:21:39.551454 AgentX-0.0.5/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2907 2024-04-02 10:50:31.000000 AgentX-0.0.5/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1388 2024-04-03 14:20:39.000000 AgentX-0.0.5/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2024-04-03 14:21:39.551454 AgentX-0.0.5/setup.cfg
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:21:39.547454 AgentX-0.0.5/src/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-03 14:21:39.547454 AgentX-0.0.5/src/AgentX.egg-info/
--rw-r--r--   0 erfan     (1000) erfan     (1000)     4428 2024-04-03 14:21:39.000000 AgentX-0.0.5/src/AgentX.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      201 2024-04-03 14:21:39.000000 AgentX-0.0.5/src/AgentX.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-04-03 14:21:39.000000 AgentX-0.0.5/src/AgentX.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      236 2024-04-03 14:21:39.000000 AgentX-0.0.5/src/AgentX.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-04-03 14:21:39.000000 AgentX-0.0.5/src/AgentX.egg-info/top_level.txt
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-08 08:26:36.733141 AgentX-0.0.6/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1076 2024-04-08 08:24:45.000000 AgentX-0.0.6/LICENSE
+-rw-r--r--   0 erfan     (1000) erfan     (1000)     4699 2024-04-08 08:26:36.733141 AgentX-0.0.6/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2907 2024-04-08 08:24:45.000000 AgentX-0.0.6/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1617 2024-04-08 08:24:45.000000 AgentX-0.0.6/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2024-04-08 08:26:36.733141 AgentX-0.0.6/setup.cfg
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-08 08:26:36.733141 AgentX-0.0.6/src/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-08 08:26:36.733141 AgentX-0.0.6/src/AgentX.egg-info/
+-rw-r--r--   0 erfan     (1000) erfan     (1000)     4699 2024-04-08 08:26:36.000000 AgentX-0.0.6/src/AgentX.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      201 2024-04-08 08:26:36.000000 AgentX-0.0.6/src/AgentX.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-04-08 08:26:36.000000 AgentX-0.0.6/src/AgentX.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      404 2024-04-08 08:26:36.000000 AgentX-0.0.6/src/AgentX.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-04-08 08:26:36.000000 AgentX-0.0.6/src/AgentX.egg-info/top_level.txt
```

### Comparing `AgentX-0.0.5/LICENSE` & `AgentX-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.5/PKG-INFO` & `AgentX-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AgentX
-Version: 0.0.5
+Version: 0.0.6
 Summary: AgentX: Seamlessly integrate intelligent agents into your projects. Empower your applications with advanced AI capabilities.
 Author-email: Erfan Zare Chavoshi <erfanzare810@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/erfanzar/AgentX
 Project-URL: Issues, https://github.com/erfanzar/AgentX/issues
 Project-URL: Documentation, https://erfanzar.github.io/AgentX
 Classifier: Programming Language :: Python :: 3
@@ -12,34 +12,42 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: transformers
-Requires-Dist: gradio
-Requires-Dist: fastapi
-Requires-Dist: termcolor
+Requires-Dist: typing~=3.7.4.3
+Requires-Dist: ipython~=8.17.2
+Requires-Dist: tqdm~=4.64.1
+Requires-Dist: pydantic==2.5.3
+Requires-Dist: setuptools~=68.1.2
+Requires-Dist: gradio~=4.25.0
+Requires-Dist: numpy~=1.26.2
+Requires-Dist: uvicorn~=0.23.2
+Requires-Dist: pydantic-core==2.14.6
+Requires-Dist: requests~=2.31.0
+Requires-Dist: transformers>=4.36.1
+Requires-Dist: huggingface-hub>=0.20.1
+Requires-Dist: absl-py==2.0.0
+Requires-Dist: Jinja2~=3.1.2
 Provides-Extra: rag
 Requires-Dist: faiss-cpu; extra == "rag"
 Requires-Dist: sentence_transformers; extra == "rag"
 Requires-Dist: pymupdf; extra == "rag"
 Requires-Dist: python-docx; extra == "rag"
 Provides-Extra: torch
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: bitsandbytes; extra == "torch"
 Provides-Extra: ollama
 Requires-Dist: ollama; extra == "ollama"
 Provides-Extra: gguf
 Requires-Dist: llama-cpp-python; extra == "gguf"
-Provides-Extra: gradio
-Requires-Dist: gradio==4.14.0; extra == "gradio"
 Provides-Extra: all
-Requires-Dist: AgentX[gguf,gradio,ollama,rag,torch]; extra == "all"
+Requires-Dist: AgentX[gguf,ollama,rag,torch]; extra == "all"
 
 # AgentX
 
 AgentX is a versatile toolkit designed to seamlessly integrate intelligent agents into your projects. With AgentX,
 developers can effortlessly bridge the gap between different frameworks and platforms, empowering their applications
 with advanced AI capabilities. AgentX facilitates the connection and collaboration of diverse agents, enhancing the
 synergy between neural networks and decision-making processes. Whether you're working on machine learning, robotics, or
```

### Comparing `AgentX-0.0.5/README.md` & `AgentX-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.5/src/AgentX.egg-info/PKG-INFO` & `AgentX-0.0.6/src/AgentX.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AgentX
-Version: 0.0.5
+Version: 0.0.6
 Summary: AgentX: Seamlessly integrate intelligent agents into your projects. Empower your applications with advanced AI capabilities.
 Author-email: Erfan Zare Chavoshi <erfanzare810@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/erfanzar/AgentX
 Project-URL: Issues, https://github.com/erfanzar/AgentX/issues
 Project-URL: Documentation, https://erfanzar.github.io/AgentX
 Classifier: Programming Language :: Python :: 3
@@ -12,34 +12,42 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: transformers
-Requires-Dist: gradio
-Requires-Dist: fastapi
-Requires-Dist: termcolor
+Requires-Dist: typing~=3.7.4.3
+Requires-Dist: ipython~=8.17.2
+Requires-Dist: tqdm~=4.64.1
+Requires-Dist: pydantic==2.5.3
+Requires-Dist: setuptools~=68.1.2
+Requires-Dist: gradio~=4.25.0
+Requires-Dist: numpy~=1.26.2
+Requires-Dist: uvicorn~=0.23.2
+Requires-Dist: pydantic-core==2.14.6
+Requires-Dist: requests~=2.31.0
+Requires-Dist: transformers>=4.36.1
+Requires-Dist: huggingface-hub>=0.20.1
+Requires-Dist: absl-py==2.0.0
+Requires-Dist: Jinja2~=3.1.2
 Provides-Extra: rag
 Requires-Dist: faiss-cpu; extra == "rag"
 Requires-Dist: sentence_transformers; extra == "rag"
 Requires-Dist: pymupdf; extra == "rag"
 Requires-Dist: python-docx; extra == "rag"
 Provides-Extra: torch
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: bitsandbytes; extra == "torch"
 Provides-Extra: ollama
 Requires-Dist: ollama; extra == "ollama"
 Provides-Extra: gguf
 Requires-Dist: llama-cpp-python; extra == "gguf"
-Provides-Extra: gradio
-Requires-Dist: gradio==4.14.0; extra == "gradio"
 Provides-Extra: all
-Requires-Dist: AgentX[gguf,gradio,ollama,rag,torch]; extra == "all"
+Requires-Dist: AgentX[gguf,ollama,rag,torch]; extra == "all"
 
 # AgentX
 
 AgentX is a versatile toolkit designed to seamlessly integrate intelligent agents into your projects. With AgentX,
 developers can effortlessly bridge the gap between different frameworks and platforms, empowering their applications
 with advanced AI capabilities. AgentX facilitates the connection and collaboration of diverse agents, enhancing the
 synergy between neural networks and decision-making processes. Whether you're working on machine learning, robotics, or
```

