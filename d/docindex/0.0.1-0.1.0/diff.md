# Comparing `tmp/docindex-0.0.1.tar.gz` & `tmp/docindex-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docindex-0.0.1.tar", last modified: Sat Apr  6 09:21:41 2024, max compression
+gzip compressed data, was "docindex-0.1.0.tar", last modified: Mon Apr  8 13:14:16 2024, max compression
```

## Comparing `docindex-0.0.1.tar` & `docindex-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:21:40.998644 docindex-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-06 09:21:40.998644 docindex-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 09:21:35.000000 docindex-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 09:21:35.000000 docindex-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-06 09:21:40.998644 docindex-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:21:40.994644 docindex-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:21:40.994644 docindex-0.0.1/src/_openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 09:21:35.000000 docindex-0.0.1/src/_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-06 09:21:35.000000 docindex-0.0.1/src/_openai/doc_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-06 09:21:35.000000 docindex-0.0.1/src/_openai/index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:21:40.998644 docindex-0.0.1/src/docindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-06 09:21:40.000000 docindex-0.0.1/src/docindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-06 09:21:40.000000 docindex-0.0.1/src/docindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:21:40.000000 docindex-0.0.1/src/docindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-06 09:21:40.000000 docindex-0.0.1/src/docindex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 09:21:40.000000 docindex-0.0.1/src/docindex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:16.001561 docindex-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-08 13:14:11.000000 docindex-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-08 13:14:16.001561 docindex-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-08 13:14:11.000000 docindex-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 13:14:11.000000 docindex-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-08 13:14:16.001561 docindex-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:15.997561 docindex-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:16.001561 docindex-0.1.0/src/_google/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_google/doc_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_google/docindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_google/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:16.001561 docindex-0.1.0/src/_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_openai/doc_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_openai/doc_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_openai/docindex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:16.001561 docindex-0.1.0/src/docindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-08 13:14:15.000000 docindex-0.1.0/src/docindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-08 13:14:15.000000 docindex-0.1.0/src/docindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:14:15.000000 docindex-0.1.0/src/docindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 13:14:15.000000 docindex-0.1.0/src/docindex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 13:14:15.000000 docindex-0.1.0/src/docindex.egg-info/top_level.txt
```

### Comparing `docindex-0.0.1/setup.cfg` & `docindex-0.1.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = docindex
 author = Kevin Kibe
-version = 0.0.1
+version = 0.1.0
 author_email = keviinkibe@gmail.com
 description = A package for fast indexing of multiple documents and their metadata on Pinecone.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/docindex
 license = MIT
 
@@ -16,14 +16,15 @@
 	pinecone-client==3.2.2
 	tiktoken==0.6.0
 	pypdf==4.1.0
 	unstructured==0.12.6
 	langchain-community==0.0.31
 	langchain==0.1.14
 	langchain-openai==0.1.1
+	langchain-google-genai==1.0.1
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `docindex-0.0.1/src/_openai/index.py` & `docindex-0.1.0/src/_google/docindex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from pinecone import Pinecone
 from tqdm.auto import tqdm
 from uuid import uuid4
 from langchain_community.document_loaders import PyPDFLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
-from langchain_openai import OpenAIEmbeddings
+from langchain_google_genai import GoogleGenerativeAIEmbeddings
 import tiktoken
 from typing import List
-from .doc_model import Page
+from _openai.doc_model import Page
 
 
-class OpenaiPineconeIndexer:
+class GooglePineconeIndexer:
     """
-    Class for indexing documents to Pinecone using OpenAI embeddings.
+    Class for indexing documents to Pinecone using GoogleGenerativeAIEmbeddings embeddings.
     """
     def __init__(
         self,
         index_name: str,
         pinecone_api_key: str,
         environment: str,
-        openai_api_key: str
+        google_api_key: str
     ) -> None:
         """
-        Initialize the OpenAIPineconeIndexer object.
+        Initialize the GoogleGenerativeAIEmbeddings object.
 
         Args:
             index_name (str): Name of the Pinecone index.
             pinecone_api_key (str): Pinecone API key.
             environment (str): Environment for Pinecone service.
-            openai_api_key (str): OpenAI API key.
+            google_api_key (str): Google API key.
         """
         self.pc = Pinecone(api_key=pinecone_api_key, environment=environment)
         self.index = self.pc.Index(index_name)
-        self.openai_api_key = openai_api_key
+        self.google_api_key = google_api_key
         self.tokenizer = tiktoken.get_encoding('p50k_base')
 
 
     def load_pdf(self, pdf_url) -> List:
         """
         Load and split a PDF document into pages.
 
@@ -61,53 +61,47 @@
         """
         tokens = self.tokenizer.encode(
             text,
             disallowed_special=()
         )
         return len(tokens)
     
-    def embed(self) -> OpenAIEmbeddings:
+    def embed(self) -> GoogleGenerativeAIEmbeddings:
         """
-        Initialize OpenAIEmbeddings object.
+        Initialize GoogleGenerativeAIEmbeddings object.
 
         Returns:
-            OpenAIEmbeddings: OpenAIEmbeddings object.
+            GoogleGenerativeAIEmbeddings: GoogleGenerativeAIEmbeddings object.
         """
-        return OpenAIEmbeddings(
-            openai_api_key=self.openai_api_key
-        )
-
-    def text_splitter(self) -> RecursiveCharacterTextSplitter:
-        """
-        Initialize RecursiveCharacterTextSplitter object.
+        return GoogleGenerativeAIEmbeddings(
+            model="models/embedding-001", 
+            google_api_key=self.google_api_key
+            )
 
-        Returns:
-            RecursiveCharacterTextSplitter: RecursiveCharacterTextSplitter object.
-        """
-        return RecursiveCharacterTextSplitter(
-            chunk_size=400,
-            chunk_overlap=20,
-            length_function=self.tiktoken_len,
-            separators=["\n\n", "\n", " ", ""]
-        )
     
-    def upsert_documents(self, documents: List[Page], batch_limit: int) -> None:
+    def upsert_documents(self, documents: List[Page], batch_limit: int, chunk_size: int = 256) -> None:
         """
         Upsert documents into the Pinecone index.
 
         Args:
             documents (List[Page]): List of documents to upsert.
             batch_limit (int): Maximum batch size for upsert operation.
+            chunks_size(int): size of texts per chunk.
 
         Returns:
             None
         """
         texts = []
         metadatas = []
-        text_splitter = self.text_splitter()  
+        text_splitter = RecursiveCharacterTextSplitter(
+            chunk_size=int(chunk_size),
+            chunk_overlap=20,
+            length_function=self.tiktoken_len,
+            separators=["\n\n", "\n", " ", ""]
+        )
         embed = self.embed()  
         for i, record in enumerate(tqdm(documents)):
             metadata = {
                 'content': record.page_content,
                 'source': record.page,
                 'title': record.source
             }
@@ -121,21 +115,22 @@
                 ids = [str(uuid4()) for _ in range(len(texts))]
                 embeds = embed.embed_documents(texts)  
                 self.index.upsert(vectors=zip(ids, embeds, metadatas), async_req=True)
                 texts = []
                 metadatas = []
 
 
-    def index_documents(self, urls: List[str], batch_limit: int) -> None:
+    def index_documents(self, urls: List[str], batch_limit: int, chunk_size: int = 256) -> None:
         """
         Process a list of URLs and upsert documents to a Pinecone index.
 
         Args:
             urls (List[str]): List of URLs to process.
             batch_limit (int): Batch limit for upserting documents.
+            chunks_size(int): size of texts per chunk.
 
         Returns:
             None
         """
         for url in tqdm(urls, desc="Processing URLs"):
             print(f"Processing URL: {url}")
             pages = self.load_pdf(url)
@@ -147,10 +142,10 @@
                     page=page.metadata['page'],
                     source=page.metadata['source']
                 )
                 for page in pages
             ]
 
             print(f"Upserting {len(pages_data)} pages to the Pinecone index...")
-            self.upsert_documents(pages_data, batch_limit)  
+            self.upsert_documents(pages_data, batch_limit, chunk_size)  
             print("Finished upserting documents for this URL.")
         print("Indexing complete.")
```

