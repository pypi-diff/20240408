# Comparing `tmp/financial_datasets-0.1.3.tar.gz` & `tmp/financial_datasets-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financial_datasets-0.1.3.tar", max compression
+gzip compressed data, was "financial_datasets-0.1.4.tar", max compression
```

## Comparing `financial_datasets-0.1.3.tar` & `financial_datasets-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.3/LICENSE
--rw-r--r--   0        0        0     3089 2024-04-03 22:32:30.744861 financial_datasets-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.3/financial_datasets/__init__.py
--rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.3/financial_datasets/dataset.py
--rw-r--r--   0        0        0     3772 2024-04-03 22:24:59.390489 financial_datasets-0.1.3/financial_datasets/generator.py
--rw-r--r--   0        0        0      619 2024-04-03 22:35:41.133840 financial_datasets-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3899 1970-01-01 00:00:00.000000 financial_datasets-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3077 2024-04-06 13:31:16.695273 financial_datasets-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.4/financial_datasets/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.4/financial_datasets/dataset.py
+-rw-r--r--   0        0        0      687 2024-04-07 22:00:07.915325 financial_datasets-0.1.4/financial_datasets/filings.py
+-rw-r--r--   0        0        0     6619 2024-04-07 22:01:00.814058 financial_datasets-0.1.4/financial_datasets/generator.py
+-rw-r--r--   0        0        0      642 2024-04-07 22:02:05.481404 financial_datasets-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3931 1970-01-01 00:00:00.000000 financial_datasets-0.1.4/PKG-INFO
```

### Comparing `financial_datasets-0.1.3/LICENSE` & `financial_datasets-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.3/README.md` & `financial_datasets-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Financial Datasets
+# Financial Datasets 🧪
 
 Financial Datasets is an open-source Python library 
 that allows developers to create synthetic financial datasets
 using Large Language Models (LLMs). With this library,
 you can generate realistic financial datasets based on SEC filings
 such as 10-Ks, 10-Qs, and other financial reports.
 
@@ -15,21 +15,20 @@
 - Easy integration with Python projects
 - Customizable data generation options
 
 ## Usage
 
 **Example code:**
 ```python
-import os
 from financial_datasets.generator import DatasetGenerator
 
 texts = ...  # List of texts from SEC filing
 generator = DatasetGenerator(
    model="gpt-4-0125-preview",
-   api_key=os.environ["OPENAI_API_KEY"],
+   api_key="YOUR_OPENAI_API_KEY",
 )
 dataset = generator.generate_from_texts(texts, max_questions=100)
 ```
 
 **Example generated dataset:**
 ```json
 [
@@ -42,15 +41,15 @@
     "question": "By what percentage did Airbnb's net income increase in 2023 compared to the prior year?",
     "answer": "153%",
     "context": "Net income in 2023 increased by 153% to $4.8 billion, compared to the prior year, driven by our revenue growth, increased interest income, discipline in managing our cost structure, and the release of a portion of our valuation allowance on deferred tax assets of $2.9 billion."
   }
 ]
 ```
 
-A full end-to-end code example can be found [here](https://colab.research.google.com/gist/virattt/953304288c8cd257156842d8f8d1062d/intro-financial-datasets.ipynb).
+A full end-to-end code example can be found [here](https://colab.research.google.com/gist/virattt/f9b5a0ae82cc0caab57df5dedc2927c9/intro-financial-datasets.ipynb).
 ## Installation
 
 ### Using pip
 
 You can install the Financial Datasets library using pip:
 
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-# Financial Datasets Financial Datasets is an open-source Python library that
-allows developers to create synthetic financial datasets using Large Language
-Models (LLMs). With this library, you can generate realistic financial datasets
-based on SEC filings such as 10-Ks, 10-Qs, and other financial reports. [!
-[Twitter Follow](https://img.shields.io/twitter/follow/virattt?style=social)]
-(https://twitter.com/virattt) ## Features - Generate synthetic financial
-datasets using LLMs - Supports various SEC filings (10-Ks, 10-Qs, etc.) - Easy
-integration with Python projects - Customizable data generation options ##
-Usage **Example code:** ```python import os from financial_datasets.generator
-import DatasetGenerator texts = ... # List of texts from SEC filing generator =
-DatasetGenerator( model="gpt-4-0125-preview", api_key=os.environ
-["OPENAI_API_KEY"], ) dataset = generator.generate_from_texts(texts,
+# Financial Datasets ð§ª Financial Datasets is an open-source Python library
+that allows developers to create synthetic financial datasets using Large
+Language Models (LLMs). With this library, you can generate realistic financial
+datasets based on SEC filings such as 10-Ks, 10-Qs, and other financial
+reports. [![Twitter Follow](https://img.shields.io/twitter/follow/
+virattt?style=social)](https://twitter.com/virattt) ## Features - Generate
+synthetic financial datasets using LLMs - Supports various SEC filings (10-Ks,
+10-Qs, etc.) - Easy integration with Python projects - Customizable data
+generation options ## Usage **Example code:** ```python from
+financial_datasets.generator import DatasetGenerator texts = ... # List of
+texts from SEC filing generator = DatasetGenerator( model="gpt-4-0125-preview",
+api_key="YOUR_OPENAI_API_KEY", ) dataset = generator.generate_from_texts(texts,
 max_questions=100) ``` **Example generated dataset:** ```json [ { "question":
 "What was Airbnb's revenue in 2023?", "answer": "$9.9 billion", "context": "In
 2023, revenue increased by 18% to $9.9 billion compared to 2022, primarily due
 to a 14% increase in Nights and Experiences Booked of 54.5 million combined
 with higher average daily rates driving a 16% increase in Gross Booking Value
 of $10.0 billion." }, { "question": "By what percentage did Airbnb's net income
 increase in 2023 compared to the prior year?", "answer": "153%", "context":
 "Net income in 2023 increased by 153% to $4.8 billion, compared to the prior
 year, driven by our revenue growth, increased interest income, discipline in
 managing our cost structure, and the release of a portion of our valuation
 allowance on deferred tax assets of $2.9 billion." } ] ``` A full end-to-end
 code example can be found [here](https://colab.research.google.com/gist/
-virattt/953304288c8cd257156842d8f8d1062d/intro-financial-datasets.ipynb). ##
+virattt/f9b5a0ae82cc0caab57df5dedc2927c9/intro-financial-datasets.ipynb). ##
 Installation ### Using pip You can install the Financial Datasets library using
 pip: ``` pip install financial-datasets ``` ### Using Poetry If you prefer to
 use Poetry for dependency management, you can add Financial Datasets to your
 project: ``` poetry add financial-datasets ``` ### From the Repository If you
 want to install the library directly from the repository, follow these steps:
 1. Clone the repository: ``` git clone https://github.com/yourusername/
 financial-datasets.git ``` 2. Navigate to the project directory: ``` cd
```

### Comparing `financial_datasets-0.1.3/pyproject.toml` & `financial_datasets-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "financial-datasets"
-version = "0.1.3"
+version = "0.1.4"
 description = "Financial datasets for LLMs"
 authors = ["Virat Singh <virat@virat.ai>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "financial_datasets"}]
 
 [tool.poetry.dependencies]
@@ -14,14 +14,15 @@
 chromadb = "^0.4.24"
 tiktoken = "^0.6.0"
 anthropic = "^0.21.3"
 instructor = "^0.6.7"
 datasets = "^2.18.0"
 xmltodict = "^0.13.0"
 tqdm = "^4.66.2"
+edgartools = "^2.16.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 twine = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `financial_datasets-0.1.3/PKG-INFO` & `financial_datasets-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: financial-datasets
-Version: 0.1.3
+Version: 0.1.4
 Summary: Financial datasets for LLMs
 License: MIT
 Author: Virat Singh
 Author-email: virat@virat.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: chromadb (>=0.4.24,<0.5.0)
 Requires-Dist: datasets (>=2.18.0,<3.0.0)
+Requires-Dist: edgartools (>=2.16.1,<3.0.0)
 Requires-Dist: instructor (>=0.6.7,<0.7.0)
 Requires-Dist: langchain (>=0.1.13,<0.2.0)
 Requires-Dist: openai (>=1.14.3,<2.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
-# Financial Datasets
+# Financial Datasets 🧪
 
 Financial Datasets is an open-source Python library 
 that allows developers to create synthetic financial datasets
 using Large Language Models (LLMs). With this library,
 you can generate realistic financial datasets based on SEC filings
 such as 10-Ks, 10-Qs, and other financial reports.
 
@@ -38,21 +39,20 @@
 - Easy integration with Python projects
 - Customizable data generation options
 
 ## Usage
 
 **Example code:**
 ```python
-import os
 from financial_datasets.generator import DatasetGenerator
 
 texts = ...  # List of texts from SEC filing
 generator = DatasetGenerator(
    model="gpt-4-0125-preview",
-   api_key=os.environ["OPENAI_API_KEY"],
+   api_key="YOUR_OPENAI_API_KEY",
 )
 dataset = generator.generate_from_texts(texts, max_questions=100)
 ```
 
 **Example generated dataset:**
 ```json
 [
@@ -65,15 +65,15 @@
     "question": "By what percentage did Airbnb's net income increase in 2023 compared to the prior year?",
     "answer": "153%",
     "context": "Net income in 2023 increased by 153% to $4.8 billion, compared to the prior year, driven by our revenue growth, increased interest income, discipline in managing our cost structure, and the release of a portion of our valuation allowance on deferred tax assets of $2.9 billion."
   }
 ]
 ```
 
-A full end-to-end code example can be found [here](https://colab.research.google.com/gist/virattt/953304288c8cd257156842d8f8d1062d/intro-financial-datasets.ipynb).
+A full end-to-end code example can be found [here](https://colab.research.google.com/gist/virattt/f9b5a0ae82cc0caab57df5dedc2927c9/intro-financial-datasets.ipynb).
 ## Installation
 
 ### Using pip
 
 You can install the Financial Datasets library using pip:
 
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1 Name: financial-datasets Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: financial-datasets Version: 0.1.4 Summary:
 Financial datasets for LLMs License: MIT Author: Virat Singh Author-email:
 virat@virat.ai Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: anthropic (>=0.21.3,<0.22.0) Requires-Dist:
 chromadb (>=0.4.24,<0.5.0) Requires-Dist: datasets (>=2.18.0,<3.0.0) Requires-
-Dist: instructor (>=0.6.7,<0.7.0) Requires-Dist: langchain (>=0.1.13,<0.2.0)
-Requires-Dist: openai (>=1.14.3,<2.0.0) Requires-Dist: tiktoken
-(>=0.6.0,<0.7.0) Requires-Dist: tqdm (>=4.66.2,<5.0.0) Requires-Dist: xmltodict
-(>=0.13.0,<0.14.0) Description-Content-Type: text/markdown # Financial Datasets
-Financial Datasets is an open-source Python library that allows developers to
-create synthetic financial datasets using Large Language Models (LLMs). With
-this library, you can generate realistic financial datasets based on SEC
-filings such as 10-Ks, 10-Qs, and other financial reports. [![Twitter Follow]
-(https://img.shields.io/twitter/follow/virattt?style=social)](https://
-twitter.com/virattt) ## Features - Generate synthetic financial datasets using
-LLMs - Supports various SEC filings (10-Ks, 10-Qs, etc.) - Easy integration
-with Python projects - Customizable data generation options ## Usage **Example
-code:** ```python import os from financial_datasets.generator import
-DatasetGenerator texts = ... # List of texts from SEC filing generator =
-DatasetGenerator( model="gpt-4-0125-preview", api_key=os.environ
-["OPENAI_API_KEY"], ) dataset = generator.generate_from_texts(texts,
+Dist: edgartools (>=2.16.1,<3.0.0) Requires-Dist: instructor (>=0.6.7,<0.7.0)
+Requires-Dist: langchain (>=0.1.13,<0.2.0) Requires-Dist: openai
+(>=1.14.3,<2.0.0) Requires-Dist: tiktoken (>=0.6.0,<0.7.0) Requires-Dist: tqdm
+(>=4.66.2,<5.0.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Description-
+Content-Type: text/markdown # Financial Datasets ð§ª Financial Datasets is an
+open-source Python library that allows developers to create synthetic financial
+datasets using Large Language Models (LLMs). With this library, you can
+generate realistic financial datasets based on SEC filings such as 10-Ks, 10-
+Qs, and other financial reports. [![Twitter Follow](https://img.shields.io/
+twitter/follow/virattt?style=social)](https://twitter.com/virattt) ## Features
+- Generate synthetic financial datasets using LLMs - Supports various SEC
+filings (10-Ks, 10-Qs, etc.) - Easy integration with Python projects -
+Customizable data generation options ## Usage **Example code:** ```python from
+financial_datasets.generator import DatasetGenerator texts = ... # List of
+texts from SEC filing generator = DatasetGenerator( model="gpt-4-0125-preview",
+api_key="YOUR_OPENAI_API_KEY", ) dataset = generator.generate_from_texts(texts,
 max_questions=100) ``` **Example generated dataset:** ```json [ { "question":
 "What was Airbnb's revenue in 2023?", "answer": "$9.9 billion", "context": "In
 2023, revenue increased by 18% to $9.9 billion compared to 2022, primarily due
 to a 14% increase in Nights and Experiences Booked of 54.5 million combined
 with higher average daily rates driving a 16% increase in Gross Booking Value
 of $10.0 billion." }, { "question": "By what percentage did Airbnb's net income
 increase in 2023 compared to the prior year?", "answer": "153%", "context":
 "Net income in 2023 increased by 153% to $4.8 billion, compared to the prior
 year, driven by our revenue growth, increased interest income, discipline in
 managing our cost structure, and the release of a portion of our valuation
 allowance on deferred tax assets of $2.9 billion." } ] ``` A full end-to-end
 code example can be found [here](https://colab.research.google.com/gist/
-virattt/953304288c8cd257156842d8f8d1062d/intro-financial-datasets.ipynb). ##
+virattt/f9b5a0ae82cc0caab57df5dedc2927c9/intro-financial-datasets.ipynb). ##
 Installation ### Using pip You can install the Financial Datasets library using
 pip: ``` pip install financial-datasets ``` ### Using Poetry If you prefer to
 use Poetry for dependency management, you can add Financial Datasets to your
 project: ``` poetry add financial-datasets ``` ### From the Repository If you
 want to install the library directly from the repository, follow these steps:
 1. Clone the repository: ``` git clone https://github.com/yourusername/
 financial-datasets.git ``` 2. Navigate to the project directory: ``` cd
```

