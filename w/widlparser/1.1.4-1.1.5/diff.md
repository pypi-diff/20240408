# Comparing `tmp/widlparser-1.1.4.tar.gz` & `tmp/widlparser-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widlparser-1.1.4.tar", last modified: Tue Dec 19 20:35:34 2023, max compression
+gzip compressed data, was "widlparser-1.1.5.tar", last modified: Mon Apr  8 18:57:40 2024, max compression
```

## Comparing `widlparser-1.1.4.tar` & `widlparser-1.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 20:35:34.790611 widlparser-1.1.4/
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-12-19 20:33:35.000000 widlparser-1.1.4/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-12-19 20:33:35.000000 widlparser-1.1.4/.git-blame-ignore-revs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 20:35:34.774611 widlparser-1.1.4/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 20:35:34.782611 widlparser-1.1.4/.github/workflows/
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-12-19 20:33:35.000000 widlparser-1.1.4/.github/workflows/test.yml
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-12-19 20:33:35.000000 widlparser-1.1.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-12-19 20:33:35.000000 widlparser-1.1.4/.gitlab-ci.env
--rw-rw-rw-   0 root         (0) root         (0)      315 2023-12-19 20:33:35.000000 widlparser-1.1.4/.gitlab-ci.yaml
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-12-19 20:33:35.000000 widlparser-1.1.4/.yamllint.yaml
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-12-19 20:33:35.000000 widlparser-1.1.4/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    14224 2023-12-19 20:35:34.790611 widlparser-1.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12399 2023-12-19 20:33:35.000000 widlparser-1.1.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-12-19 20:33:35.000000 widlparser-1.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-19 20:35:34.790611 widlparser-1.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    58224 2023-12-19 20:33:35.000000 widlparser-1.1.4/test-expected.txt
--rwxrwxrwx   0 root         (0) root         (0)    12557 2023-12-19 20:35:32.000000 widlparser-1.1.4/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 20:35:34.786610 widlparser-1.1.4/widlparser/
--rw-rw-rw-   0 root         (0) root         (0)     3412 2023-12-19 20:33:35.000000 widlparser-1.1.4/widlparser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    72886 2023-12-19 20:33:35.000000 widlparser-1.1.4/widlparser/constructs.py
--rw-rw-rw-   0 root         (0) root         (0)    11191 2023-12-19 20:33:35.000000 widlparser-1.1.4/widlparser/markup.py
--rw-rw-rw-   0 root         (0) root         (0)    11119 2023-12-19 20:33:35.000000 widlparser-1.1.4/widlparser/parser.py
--rw-rw-rw-   0 root         (0) root         (0)    86549 2023-12-19 20:33:35.000000 widlparser-1.1.4/widlparser/productions.py
--rw-rw-rw-   0 root         (0) root         (0)     3768 2023-12-19 20:33:35.000000 widlparser-1.1.4/widlparser/protocols.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-12-19 20:33:35.000000 widlparser-1.1.4/widlparser/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    11449 2023-12-19 20:33:35.000000 widlparser-1.1.4/widlparser/tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 20:35:34.790611 widlparser-1.1.4/widlparser.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14224 2023-12-19 20:35:34.000000 widlparser-1.1.4/widlparser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      567 2023-12-19 20:35:34.000000 widlparser-1.1.4/widlparser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-19 20:35:34.000000 widlparser-1.1.4/widlparser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      366 2023-12-19 20:35:34.000000 widlparser-1.1.4/widlparser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-12-19 20:35:34.000000 widlparser-1.1.4/widlparser.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-12-19 20:33:35.000000 widlparser-1.1.4/widlparser.sublime-project
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 18:57:40.768077 widlparser-1.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-04-08 18:52:23.000000 widlparser-1.1.5/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      125 2024-04-08 18:52:23.000000 widlparser-1.1.5/.git-blame-ignore-revs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 18:57:40.748077 widlparser-1.1.5/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 18:57:40.756076 widlparser-1.1.5/.github/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)      427 2024-04-08 18:52:23.000000 widlparser-1.1.5/.github/workflows/test.yml
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-08 18:52:23.000000 widlparser-1.1.5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-08 18:52:23.000000 widlparser-1.1.5/.gitlab-ci.env
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-04-08 18:52:23.000000 widlparser-1.1.5/.gitlab-ci.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-04-08 18:52:23.000000 widlparser-1.1.5/.yamllint.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      539 2024-04-08 18:52:23.000000 widlparser-1.1.5/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    14224 2024-04-08 18:57:40.768077 widlparser-1.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12399 2024-04-08 18:52:23.000000 widlparser-1.1.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2024-04-08 18:52:23.000000 widlparser-1.1.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 18:57:40.768077 widlparser-1.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    58224 2024-04-08 18:52:23.000000 widlparser-1.1.5/test-expected.txt
+-rwxrwxrwx   0 root         (0) root         (0)    12557 2024-04-08 18:57:37.000000 widlparser-1.1.5/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 18:57:40.760077 widlparser-1.1.5/widlparser/
+-rw-rw-rw-   0 root         (0) root         (0)     3412 2024-04-08 18:52:23.000000 widlparser-1.1.5/widlparser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    72886 2024-04-08 18:52:23.000000 widlparser-1.1.5/widlparser/constructs.py
+-rw-rw-rw-   0 root         (0) root         (0)    11191 2024-04-08 18:52:23.000000 widlparser-1.1.5/widlparser/markup.py
+-rw-rw-rw-   0 root         (0) root         (0)    11119 2024-04-08 18:52:23.000000 widlparser-1.1.5/widlparser/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    86565 2024-04-08 18:52:23.000000 widlparser-1.1.5/widlparser/productions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3768 2024-04-08 18:52:23.000000 widlparser-1.1.5/widlparser/protocols.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-08 18:52:23.000000 widlparser-1.1.5/widlparser/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    11465 2024-04-08 18:52:23.000000 widlparser-1.1.5/widlparser/tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 18:57:40.764077 widlparser-1.1.5/widlparser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14224 2024-04-08 18:57:40.000000 widlparser-1.1.5/widlparser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      567 2024-04-08 18:57:40.000000 widlparser-1.1.5/widlparser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 18:57:40.000000 widlparser-1.1.5/widlparser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      366 2024-04-08 18:57:40.000000 widlparser-1.1.5/widlparser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-08 18:57:40.000000 widlparser-1.1.5/widlparser.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-08 18:52:23.000000 widlparser-1.1.5/widlparser.sublime-project
```

### Comparing `widlparser-1.1.4/CONTRIBUTING.md` & `widlparser-1.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `widlparser-1.1.4/PKG-INFO` & `widlparser-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widlparser
-Version: 1.1.4
+Version: 1.1.5
 Summary: WebIDL Parser
 Author-email: Peter Linss <pypi@linss.com>
 License: MIT Licence
 Project-URL: homepage, https://gitlab.linss.com/open-source/python/widlparser
 Keywords: config
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `widlparser-1.1.4/README.md` & `widlparser-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `widlparser-1.1.4/pyproject.toml` & `widlparser-1.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `widlparser-1.1.4/test-expected.txt` & `widlparser-1.1.5/test-expected.txt`

 * *Files identical despite different names*

### Comparing `widlparser-1.1.4/test.py` & `widlparser-1.1.5/test.py`

 * *Files identical despite different names*

### Comparing `widlparser-1.1.4/widlparser/__init__.py` & `widlparser-1.1.5/widlparser/__init__.py`

 * *Files identical despite different names*

### Comparing `widlparser-1.1.4/widlparser/constructs.py` & `widlparser-1.1.5/widlparser/constructs.py`

 * *Files identical despite different names*

### Comparing `widlparser-1.1.4/widlparser/markup.py` & `widlparser-1.1.5/widlparser/markup.py`

 * *Files identical despite different names*

### Comparing `widlparser-1.1.4/widlparser/parser.py` & `widlparser-1.1.5/widlparser/parser.py`

 * *Files identical despite different names*

### Comparing `widlparser-1.1.4/widlparser/productions.py` & `widlparser-1.1.5/widlparser/productions.py`

 * *Files 0% similar despite different names*

```diff
@@ -934,15 +934,15 @@
 	| "object" [TypeSuffix] | "Error" TypeSuffix | "Promise" "<" Type ">" [Null] | BufferRelatedType [Null]
 	| "FrozenArray" "<" TypeWithExtendedAttributes ">" [Null] | "ObservableArray" "<" TypeWithExtendedAttributes ">" [Null]
 	| "record" "<" StringType "," TypeWithExtendedAttributes ">"
 	"""
 
 	BUFFER_RELATED_TYPES = frozenset(['ArrayBuffer', 'DataView', 'Int8Array', 'Int16Array', 'Int32Array',
 	                                  'Uint8Array', 'Uint16Array', 'Uint32Array', 'Uint8ClampedArray',
-	                                  'Float32Array', 'Float64Array'])
+	                                  'Float16Array', 'Float32Array', 'Float64Array'])
 	STRING_TYPES = frozenset(['ByteString', 'DOMString', 'USVString'])
 	OBJECT_TYPES = frozenset(['object', 'Error'])
 
 	type: (PrimitiveType | TypeIdentifier | TypeWithExtendedAttributes | Type | Symbol)
 	type_name: (str | None)
 	sequence: (Symbol | None)
 	promise: (Symbol | None)
```

### Comparing `widlparser-1.1.4/widlparser/protocols.py` & `widlparser-1.1.5/widlparser/protocols.py`

 * *Files identical despite different names*

### Comparing `widlparser-1.1.4/widlparser/tokenizer.py` & `widlparser-1.1.5/widlparser/tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 class Tokenizer(object):
 	"""Consume a string and convert to tokens."""
 
 	SYMBOL_IDENTS = frozenset((
 		'any', 'async', 'attribute', 'ArrayBuffer', 'bigint', 'boolean', 'byte', 'ByteString', 'callback', 'const', 'constructor', 'creator', 'DataView',
 		'deleter', 'dictionary', 'DOMString', 'double', 'enum', 'Error', 'false', 'float',
-		'Float32Array', 'Float64Array', 'FrozenArray', 'getter', 'implements', 'includes', 'Infinity', '-Infinity', 'inherit', 'Int8Array',
+		'Float16Array', 'Float32Array', 'Float64Array', 'FrozenArray', 'getter', 'implements', 'includes', 'Infinity', '-Infinity', 'inherit', 'Int8Array',
 		'Int16Array', 'Int32Array', 'interface', 'iterable', 'legacycaller', 'legacyiterable', 'long', 'maplike', 'mixin',
 		'namespace', 'NaN', 'null', 'object', 'ObservableArray', 'octet', 'optional', 'or', 'partial', 'Promise', 'readonly', 'record', 'required',
 		'sequence', 'setlike', 'setter', 'short', 'static', 'stringifier', 'true', 'typedef',
 		'Uint8Array', 'Uint16Array', 'Uint32Array', 'Uint8ClampedArray', 'undefined', 'unrestricted', 'unsigned', 'USVString'))
 
 	ui: (UserInterface | None)
 	tokens: deque[Token]
```

### Comparing `widlparser-1.1.4/widlparser.egg-info/PKG-INFO` & `widlparser-1.1.5/widlparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widlparser
-Version: 1.1.4
+Version: 1.1.5
 Summary: WebIDL Parser
 Author-email: Peter Linss <pypi@linss.com>
 License: MIT Licence
 Project-URL: homepage, https://gitlab.linss.com/open-source/python/widlparser
 Keywords: config
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `widlparser-1.1.4/widlparser.egg-info/SOURCES.txt` & `widlparser-1.1.5/widlparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

