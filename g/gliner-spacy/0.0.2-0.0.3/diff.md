# Comparing `tmp/gliner-spacy-0.0.2.tar.gz` & `tmp/gliner-spacy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-spacy-0.0.2.tar", last modified: Sat Mar 16 00:53:26 2024, max compression
+gzip compressed data, was "gliner-spacy-0.0.3.tar", last modified: Mon Apr  8 09:17:58 2024, max compression
```

## Comparing `gliner-spacy-0.0.2.tar` & `gliner-spacy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-03-16 00:53:26.128111 gliner-spacy-0.0.2/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2677 2024-03-16 00:53:26.128017 gliner-spacy-0.0.2/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1996 2024-03-16 00:30:40.000000 gliner-spacy-0.0.2/README.md
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-03-16 00:53:26.127295 gliner-spacy-0.0.2/gliner_spacy/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       27 2024-03-09 11:26:23.000000 gliner-spacy-0.0.2/gliner_spacy/__init__.py
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2543 2024-03-16 00:26:03.000000 gliner-spacy-0.0.2/gliner_spacy/pipeline.py
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-03-16 00:53:26.127878 gliner-spacy-0.0.2/gliner_spacy.egg-info/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2677 2024-03-16 00:53:26.000000 gliner-spacy-0.0.2/gliner_spacy.egg-info/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)      247 2024-03-16 00:53:26.000000 gliner-spacy-0.0.2/gliner_spacy.egg-info/SOURCES.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-03-16 00:53:26.000000 gliner-spacy-0.0.2/gliner_spacy.egg-info/dependency_links.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-03-16 00:53:26.000000 gliner-spacy-0.0.2/gliner_spacy.egg-info/requires.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-03-16 00:53:26.000000 gliner-spacy-0.0.2/gliner_spacy.egg-info/top_level.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-03-16 00:53:26.128140 gliner-spacy-0.0.2/setup.cfg
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1271 2024-03-16 00:52:54.000000 gliner-spacy-0.0.2/setup.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-08 09:17:58.054637 gliner-spacy-0.0.3/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3221 2024-04-08 09:17:58.054519 gliner-spacy-0.0.3/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     2540 2024-04-03 12:39:06.000000 gliner-spacy-0.0.3/README.md
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-08 09:17:58.053727 gliner-spacy-0.0.3/gliner_spacy/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       27 2024-03-09 11:26:23.000000 gliner-spacy-0.0.3/gliner_spacy/__init__.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     2943 2024-04-08 09:15:55.000000 gliner-spacy-0.0.3/gliner_spacy/pipeline.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-08 09:17:58.054344 gliner-spacy-0.0.3/gliner_spacy.egg-info/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3221 2024-04-08 09:17:57.000000 gliner-spacy-0.0.3/gliner_spacy.egg-info/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)      247 2024-04-08 09:17:58.000000 gliner-spacy-0.0.3/gliner_spacy.egg-info/SOURCES.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-04-08 09:17:58.000000 gliner-spacy-0.0.3/gliner_spacy.egg-info/dependency_links.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-08 09:17:58.000000 gliner-spacy-0.0.3/gliner_spacy.egg-info/requires.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-08 09:17:58.000000 gliner-spacy-0.0.3/gliner_spacy.egg-info/top_level.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-04-08 09:17:58.054689 gliner-spacy-0.0.3/setup.cfg
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1271 2024-04-08 09:17:56.000000 gliner-spacy-0.0.3/setup.py
```

### Comparing `gliner-spacy-0.0.2/PKG-INFO` & `gliner-spacy-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -59,14 +59,34 @@
 ### Expected Output
 
 ```
 Bill Gates person
 Microsoft organization
 ```
 
+## Example with Custom Configs
+
+```python
+import spacy
+from gliner_spacy.pipeline import GlinerSpacy
+
+custom_spacy_config = { "gliner_model": "urchade/gliner_multi",
+                            "chunk_size": 250,
+                            "labels": ["people","company","punctuation"],
+                            "style": "ent"}
+nlp = spacy.blank("en")
+nlp.add_pipe("gliner_spacy", config=custom_spacy_config)
+
+text = "This is a text about Bill Gates and Microsoft."
+doc = nlp(text)
+
+for ent in doc.ents:
+    print(ent.text, ent.label_)
+```
+
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
```

### Comparing `gliner-spacy-0.0.2/README.md` & `gliner-spacy-0.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -42,14 +42,34 @@
 ### Expected Output
 
 ```
 Bill Gates person
 Microsoft organization
 ```
 
+## Example with Custom Configs
+
+```python
+import spacy
+from gliner_spacy.pipeline import GlinerSpacy
+
+custom_spacy_config = { "gliner_model": "urchade/gliner_multi",
+                            "chunk_size": 250,
+                            "labels": ["people","company","punctuation"],
+                            "style": "ent"}
+nlp = spacy.blank("en")
+nlp.add_pipe("gliner_spacy", config=custom_spacy_config)
+
+text = "This is a text about Bill Gates and Microsoft."
+doc = nlp(text)
+
+for ent in doc.ents:
+    print(ent.text, ent.label_)
+```
+
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
```

### Comparing `gliner-spacy-0.0.2/gliner_spacy/pipeline.py` & `gliner-spacy-0.0.3/gliner_spacy/pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,35 +3,39 @@
 from spacy.language import Language
 
 
 DEFAULT_SPACY_CONFIG = {
         "gliner_model": "urchade/gliner_base",
         "chunk_size": 250,
         "labels": ["person", "organization"],
-        "style": "ent"
+        "style": "ent",
+        "threshold": .50
     }
 
 
 @Language.factory("gliner_spacy",
                   assigns=["doc.ents"],
                   default_config=DEFAULT_SPACY_CONFIG)
 class GlinerSpacy:
     def __init__(self,
                  nlp: Language,
                  name: str,
                  gliner_model: str,
                  chunk_size: int,
                  labels: list,
                  style: str,
+                 threshold: float
                  ):
+        
         self.nlp = nlp
         self.model = GLiNER.from_pretrained("urchade/gliner_base")
         self.labels = labels
         self.chunk_size = chunk_size
         self.style = style  # Store style as an instance variable
+        self.threshold = threshold
 
     def __call__(self, doc):
         # Tokenize the text
         chunks = []
         start = 0
         text = doc.text
         while start < len(text):
@@ -43,17 +47,21 @@
             start = end
 
         # Process each chunk and adjust entity indices
         all_entities = []
         offset = 0
         for chunk in chunks:
             if self.style == "span":
-                chunk_entities = self.model.predict_entities(chunk, self.labels, flat_ner=False)
+                chunk_entities = self.model.predict_entities(chunk, self.labels,
+                                                             flat_ner=False,
+                                                             threshold=self.threshold)
             else:
-                chunk_entities = self.model.predict_entities(chunk, self.labels, flat_ner=True)
+                chunk_entities = self.model.predict_entities(chunk, self.labels,
+                                                             flat_ner=True,
+                                                             threshold=self.threshold)
             for entity in chunk_entities:
                 all_entities.append({
                     'start': offset + entity['start'],
                     'end': offset + entity['end'],
                     'label': entity['label']
                 })
             offset += len(chunk)
```

### Comparing `gliner-spacy-0.0.2/gliner_spacy.egg-info/PKG-INFO` & `gliner-spacy-0.0.3/gliner_spacy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -59,14 +59,34 @@
 ### Expected Output
 
 ```
 Bill Gates person
 Microsoft organization
 ```
 
+## Example with Custom Configs
+
+```python
+import spacy
+from gliner_spacy.pipeline import GlinerSpacy
+
+custom_spacy_config = { "gliner_model": "urchade/gliner_multi",
+                            "chunk_size": 250,
+                            "labels": ["people","company","punctuation"],
+                            "style": "ent"}
+nlp = spacy.blank("en")
+nlp.add_pipe("gliner_spacy", config=custom_spacy_config)
+
+text = "This is a text about Bill Gates and Microsoft."
+doc = nlp(text)
+
+for ent in doc.ents:
+    print(ent.text, ent.label_)
+```
+
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
```

### Comparing `gliner-spacy-0.0.2/setup.py` & `gliner-spacy-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of your README file
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='gliner-spacy',  # Your package name
-    version='0.0.2',  # Initial version
+    version='0.0.3',  # Initial version
     author='William J. B. Mattingly',  # Your name
     description='A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities',  # Short description
     long_description=long_description,
     long_description_content_type='text/markdown',  # Ensures correct rendering on PyPI
     url='https://github.com/theirstory/gliner-spacy',  # Your repository URL
     packages=find_packages(),
     install_requires=[
```

