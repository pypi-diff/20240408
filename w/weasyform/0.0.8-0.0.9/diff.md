# Comparing `tmp/weasyform-0.0.8.tar.gz` & `tmp/weasyform-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weasyform-0.0.8.tar", last modified: Sun Apr  7 06:57:02 2024, max compression
+gzip compressed data, was "weasyform-0.0.9.tar", last modified: Mon Apr  8 12:56:07 2024, max compression
```

## Comparing `weasyform-0.0.8.tar` & `weasyform-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sadam     (1000) users      (100)        0 2024-04-07 06:57:02.335121 weasyform-0.0.8/
--rw-r--r--   0 sadam     (1000) users      (100)     1134 2024-04-07 06:57:02.335121 weasyform-0.0.8/PKG-INFO
--rw-r--r--   0 sadam     (1000) users      (100)      126 2022-03-13 18:55:31.000000 weasyform-0.0.8/README.md
--rw-r--r--   0 sadam     (1000) users      (100)       38 2024-04-07 06:57:02.335121 weasyform-0.0.8/setup.cfg
--rw-r--r--   0 sadam     (1000) users      (100)     1386 2024-04-07 06:53:45.000000 weasyform-0.0.8/setup.py
--rw-r--r--   0 sadam     (1000) users      (100)     1203 2024-04-06 22:23:31.000000 weasyform-0.0.8/test.py
-drwxr-xr-x   0 sadam     (1000) users      (100)        0 2024-04-07 06:57:02.335121 weasyform-0.0.8/weasyform/
--rw-r--r--   0 sadam     (1000) users      (100)     6203 2024-04-06 22:22:56.000000 weasyform-0.0.8/weasyform/FormFinisher.py
--rw-r--r--   0 sadam     (1000) users      (100)        0 2024-04-06 22:04:54.000000 weasyform-0.0.8/weasyform/__init__.py
-drwxr-xr-x   0 sadam     (1000) users      (100)        0 2024-04-07 06:57:02.335121 weasyform-0.0.8/weasyform.egg-info/
--rw-r--r--   0 sadam     (1000) users      (100)     1134 2024-04-07 06:57:02.000000 weasyform-0.0.8/weasyform.egg-info/PKG-INFO
--rw-r--r--   0 sadam     (1000) users      (100)      238 2024-04-07 06:57:02.000000 weasyform-0.0.8/weasyform.egg-info/SOURCES.txt
--rw-r--r--   0 sadam     (1000) users      (100)        1 2024-04-07 06:57:02.000000 weasyform-0.0.8/weasyform.egg-info/dependency_links.txt
--rw-r--r--   0 sadam     (1000) users      (100)       17 2024-04-07 06:57:02.000000 weasyform-0.0.8/weasyform.egg-info/requires.txt
--rw-r--r--   0 sadam     (1000) users      (100)       10 2024-04-07 06:57:02.000000 weasyform-0.0.8/weasyform.egg-info/top_level.txt
+drwxr-xr-x   0 sadam     (1000) users      (100)        0 2024-04-08 12:56:07.943717 weasyform-0.0.9/
+-rw-r--r--   0 sadam     (1000) users      (100)     1134 2024-04-08 12:56:07.943717 weasyform-0.0.9/PKG-INFO
+-rw-r--r--   0 sadam     (1000) users      (100)      126 2022-03-13 18:55:31.000000 weasyform-0.0.9/README.md
+-rw-r--r--   0 sadam     (1000) users      (100)       38 2024-04-08 12:56:07.943717 weasyform-0.0.9/setup.cfg
+-rw-r--r--   0 sadam     (1000) users      (100)     1386 2024-04-08 12:54:40.000000 weasyform-0.0.9/setup.py
+-rw-r--r--   0 sadam     (1000) users      (100)     1203 2024-04-06 22:23:31.000000 weasyform-0.0.9/test.py
+drwxr-xr-x   0 sadam     (1000) users      (100)        0 2024-04-08 12:56:07.940384 weasyform-0.0.9/weasyform/
+-rw-r--r--   0 sadam     (1000) users      (100)     6202 2024-04-08 12:49:49.000000 weasyform-0.0.9/weasyform/FormFinisher.py
+-rw-r--r--   0 sadam     (1000) users      (100)        0 2024-04-06 22:04:54.000000 weasyform-0.0.9/weasyform/__init__.py
+drwxr-xr-x   0 sadam     (1000) users      (100)        0 2024-04-08 12:56:07.943717 weasyform-0.0.9/weasyform.egg-info/
+-rw-r--r--   0 sadam     (1000) users      (100)     1134 2024-04-08 12:56:07.000000 weasyform-0.0.9/weasyform.egg-info/PKG-INFO
+-rw-r--r--   0 sadam     (1000) users      (100)      238 2024-04-08 12:56:07.000000 weasyform-0.0.9/weasyform.egg-info/SOURCES.txt
+-rw-r--r--   0 sadam     (1000) users      (100)        1 2024-04-08 12:56:07.000000 weasyform-0.0.9/weasyform.egg-info/dependency_links.txt
+-rw-r--r--   0 sadam     (1000) users      (100)       17 2024-04-08 12:56:07.000000 weasyform-0.0.9/weasyform.egg-info/requires.txt
+-rw-r--r--   0 sadam     (1000) users      (100)       10 2024-04-08 12:56:07.000000 weasyform-0.0.9/weasyform.egg-info/top_level.txt
```

### Comparing `weasyform-0.0.8/PKG-INFO` & `weasyform-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weasyform
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple form support for WeasyPrint
 Home-page: https://github.com/Salamek/weasyform
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: BSD
 Project-URL: Release notes, https://github.com/Salamek/weasyform/releases
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `weasyform-0.0.8/setup.py` & `weasyform-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_readme() -> str:
     with open('README.md', 'r', encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='weasyform',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(exclude=['tests', 'tests.*']),
     install_requires=[
         'WeasyPrint>=61.0'
     ],
 
     url='https://github.com/Salamek/weasyform',
     license='BSD',
```

### Comparing `weasyform-0.0.8/test.py` & `weasyform-0.0.9/test.py`

 * *Files identical despite different names*

### Comparing `weasyform-0.0.8/weasyform/FormFinisher.py` & `weasyform-0.0.9/weasyform/FormFinisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             signature_field['AP'] = ap_dict
 
     def override_field(self, pdf: pydyf.PDF, input_name: str):
         found_element = self._find_form_field(pdf, input_name)
         if not found_element:
             raise ValueError('Input with name {} not found'.format(input_name))
         found_element['FT'] = '/Sig'
-        found_element['F'] = 132,
+        found_element['F'] = 132
         found_element['T'] = pydyf.String(input_name)  #!FIXME we have to override name since weasyprint doublepacks T in pydyf.String -> pydyf.String
         if self.inject_empty_cryptographic_signature:
             found_element['V'] = self._append_empty_cryptographic_signature(pdf).reference
         else:
             del found_element['V']  # Remove V (value) since it is set to pydyf.String and that may break signing in some pdf readers???
         del found_element['DA']  # Remove DA whoever it is lol
```

### Comparing `weasyform-0.0.8/weasyform.egg-info/PKG-INFO` & `weasyform-0.0.9/weasyform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weasyform
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple form support for WeasyPrint
 Home-page: https://github.com/Salamek/weasyform
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: BSD
 Project-URL: Release notes, https://github.com/Salamek/weasyform/releases
 Classifier: Development Status :: 5 - Production/Stable
```

