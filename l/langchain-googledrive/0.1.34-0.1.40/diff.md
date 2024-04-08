# Comparing `tmp/langchain_googledrive-0.1.34.tar.gz` & `tmp/langchain_googledrive-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_googledrive-0.1.34.tar", max compression
+gzip compressed data, was "langchain_googledrive-0.1.40.tar", max compression
```

## Comparing `langchain_googledrive-0.1.34.tar` & `langchain_googledrive-0.1.40.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-09-29 15:31:57.756473 langchain_googledrive-0.1.34/LICENSE.txt
--rw-r--r--   0        0        0     1391 2024-03-12 07:53:57.458994 langchain_googledrive-0.1.34/README.md
--rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.34/langchain_googledrive/__init__.py
--rw-r--r--   0        0        0       84 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.34/langchain_googledrive/document_loaders/__init__.py
--rw-r--r--   0        0        0    13362 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.34/langchain_googledrive/document_loaders/google_drive.py
--rw-r--r--   0        0        0       90 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.34/langchain_googledrive/retrievers/__init__.py
--rw-r--r--   0        0        0     2214 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.34/langchain_googledrive/retrievers/google_drive.py
--rw-r--r--   0        0        0       97 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.34/langchain_googledrive/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.34/langchain_googledrive/tools/google_drive/__init__.py
--rw-r--r--   0        0        0     1183 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.34/langchain_googledrive/tools/google_drive/tool.py
--rw-r--r--   0        0        0      109 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.34/langchain_googledrive/utilities/__init__.py
--rw-r--r--   0        0        0    77821 2024-03-19 17:18:10.572131 langchain_googledrive-0.1.34/langchain_googledrive/utilities/google_drive.py
--rw-r--r--   0        0        0     3399 2024-03-19 17:23:21.113431 langchain_googledrive-0.1.34/pyproject.toml
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 langchain_googledrive-0.1.34/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-09-29 15:31:57.756473 langchain_googledrive-0.1.40/LICENSE.txt
+-rw-r--r--   0        0        0     1391 2024-03-12 07:53:57.458994 langchain_googledrive-0.1.40/README.md
+-rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/__init__.py
+-rw-r--r--   0        0        0       84 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/document_loaders/__init__.py
+-rw-r--r--   0        0        0    13362 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.40/langchain_googledrive/document_loaders/google_drive.py
+-rw-r--r--   0        0        0       90 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/retrievers/__init__.py
+-rw-r--r--   0        0        0     2214 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.40/langchain_googledrive/retrievers/google_drive.py
+-rw-r--r--   0        0        0       97 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/tools/google_drive/__init__.py
+-rw-r--r--   0        0        0     1183 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.40/langchain_googledrive/tools/google_drive/tool.py
+-rw-r--r--   0        0        0      109 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/utilities/__init__.py
+-rw-r--r--   0        0        0    77959 2024-04-08 10:52:09.662282 langchain_googledrive-0.1.40/langchain_googledrive/utilities/google_drive.py
+-rw-r--r--   0        0        0     3399 2024-03-19 17:23:21.113431 langchain_googledrive-0.1.40/pyproject.toml
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 langchain_googledrive-0.1.40/PKG-INFO
```

### Comparing `langchain_googledrive-0.1.34/LICENSE.txt` & `langchain_googledrive-0.1.40/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.34/README.md` & `langchain_googledrive-0.1.40/README.md`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.34/langchain_googledrive/document_loaders/google_drive.py` & `langchain_googledrive-0.1.40/langchain_googledrive/document_loaders/google_drive.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.34/langchain_googledrive/retrievers/google_drive.py` & `langchain_googledrive-0.1.40/langchain_googledrive/retrievers/google_drive.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.34/langchain_googledrive/tools/google_drive/tool.py` & `langchain_googledrive-0.1.40/langchain_googledrive/tools/google_drive/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.34/langchain_googledrive/utilities/google_drive.py` & `langchain_googledrive-0.1.40/langchain_googledrive/utilities/google_drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,14 +233,15 @@
             UnstructuredHTMLLoader,
             UnstructuredImageLoader,
             UnstructuredMarkdownLoader,
             UnstructuredODTLoader,
             UnstructuredPDFLoader,
             UnstructuredPowerPointLoader,
             UnstructuredWordDocumentLoader,
+            UnstructuredExcelLoader,
         )
 
         try:
             import detectron2  # noqa: F401 , type: ignore
             import pdf2image  # type: ignore
             import pytesseract  # type: ignore
 
@@ -271,15 +272,15 @@
 
             mime_types_mapping.update(
                 {
                     "application/epub+zip": UnstructuredEPubLoader,
                 }
             )
         except ImportError:
-            logger.info("Ignore Epub for GDrive (no module named 'pypandoc'")
+            logger.info("Ignore Epub for GDrive (no module named 'pypandoc')")
 
         try:
             import pdf2image  # noqa: F401, F811
             import pytesseract  # noqa: F401, F811
 
             mime_types_mapping.update(
                 {
@@ -288,31 +289,33 @@
                         partial(UnstructuredPDFLoader, strategy=strategy, mode=mode),
                     ),
                 }
             )
         except ImportError:
             logger.info(
                 "Ignore PDF for GDrive (no module named 'pdf2image' "
-                "and 'pytesseract'"
+                "and 'pytesseract')"
             )
 
         mime_types_mapping.update(
             {
                 "text/html": UnstructuredHTMLLoader,
                 "text/markdown": UnstructuredMarkdownLoader,
                 "application/vnd.openxmlformats-officedocument."
                 "presentationml.presentation": cast(
                     TYPE_LOAD, partial(UnstructuredPowerPointLoader, mode=mode)
                 ),  # PPTX
                 "application/vnd.openxmlformats-officedocument."
                 "wordprocessingml.document": cast(
                     TYPE_LOAD, partial(UnstructuredWordDocumentLoader, mode=mode)
                 ),  # DOCX
-                # "application/vnd.openxmlformats-officedocument.
-                # spreadsheetml.sheet": # XLSX
+                "application/vnd.openxmlformats-officedocument."
+                "spreadsheetml.sheet": cast(
+                    TYPE_LOAD, partial(UnstructuredExcelLoader, mode=mode)
+                ),  # XLSX
                 "application/vnd.oasis.opendocument.text": UnstructuredODTLoader,
             }
         )
     except ImportError:
         logger.info(
             "Ignore Unstructure*Loader for GDrive "
             "(no module `unstructured[local-inference]`)"
```

### Comparing `langchain_googledrive-0.1.34/pyproject.toml` & `langchain_googledrive-0.1.40/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.34/PKG-INFO` & `langchain_googledrive-0.1.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-googledrive
-Version: 0.1.34
+Version: 0.1.40
 Summary: This is a temporary project while I wait for my langchain [pull-request](https://github.com/hwchase17/langchain/pull/5135) to be validated.
 Home-page: https://www.github.com/pprados/langchain-googledrive
 License: Apache 2.0
 Author: Philippe PRADOS
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

