# Comparing `tmp/pyrtz-0.1.7.tar.gz` & `tmp/pyrtz-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz-0.1.7.tar", last modified: Thu Mar 10 22:32:58 2022, max compression
+gzip compressed data, was "pyrtz-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz-0.1.7.tar` & `pyrtz-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1799 2022-03-10 22:18:09.013152 pyrtz-0.1.7/.gitignore
--rw-r--r--   0        0        0    35149 2022-03-10 22:18:09.013152 pyrtz-0.1.7/LICENSE
--rw-r--r--   0        0        0      256 2022-03-10 22:18:09.013152 pyrtz-0.1.7/README.md
--rw-r--r--   0        0        0      818 2022-03-10 22:18:09.013152 pyrtz-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       52 2022-03-10 22:26:56.770300 pyrtz-0.1.7/pyrtz/__init__.py
--rw-r--r--   0        0        0     7200 2022-03-10 22:18:09.013152 pyrtz-0.1.7/pyrtz/annocp.py
--rw-r--r--   0        0        0     4360 2022-03-10 22:18:09.013152 pyrtz-0.1.7/pyrtz/asylum.py
--rw-r--r--   0        0        0    33922 2022-03-10 22:26:28.362265 pyrtz-0.1.7/pyrtz/curves.py
--rw-r--r--   0        0        0      715 2022-03-10 22:18:09.013152 pyrtz-0.1.7/pyrtz/utils.py
--rw-r--r--   0        0        0     1130 1970-01-01 00:00:00.000000 pyrtz-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1799 2024-04-08 16:53:53.833081 pyrtz-0.1.8/.gitignore
+-rw-r--r--   0        0        0    35149 2024-04-08 16:53:53.833081 pyrtz-0.1.8/LICENSE
+-rw-r--r--   0        0        0      256 2024-04-08 16:53:53.833081 pyrtz-0.1.8/README.md
+-rw-r--r--   0        0        0      822 2024-04-08 16:53:53.833081 pyrtz-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       52 2024-04-08 16:56:58.720035 pyrtz-0.1.8/pyrtz/__init__.py
+-rw-r--r--   0        0        0     7200 2024-04-08 16:53:53.833081 pyrtz-0.1.8/pyrtz/annocp.py
+-rw-r--r--   0        0        0     4361 2024-04-08 16:53:53.833081 pyrtz-0.1.8/pyrtz/asylum.py
+-rw-r--r--   0        0        0    33910 2024-04-08 16:53:53.833081 pyrtz-0.1.8/pyrtz/curves.py
+-rw-r--r--   0        0        0      715 2024-04-08 16:53:53.833081 pyrtz-0.1.8/pyrtz/utils.py
+-rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 pyrtz-0.1.8/PKG-INFO
```

### Comparing `pyrtz-0.1.7/.gitignore` & `pyrtz-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrtz-0.1.7/LICENSE` & `pyrtz-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz-0.1.7/pyproject.toml` & `pyrtz-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 	 'pandas >=1.0.5',
 	 'scipy >=1.4.1',
 	 'plotly >=5.1.0',
 	 'dash >=1.21.0',
 	 'dash_core_components >=1.17.1',
 	 'dash_html_components >=1.1.4',
 	 'PyPDF2 >=1.26.0',
-	 'igor >=0.3',
+	 'igor2 >=0.5.5',
 	 'kaleido >=0.2.1'
-]
+]
```

### Comparing `pyrtz-0.1.7/pyrtz/annocp.py` & `pyrtz-0.1.8/pyrtz/annocp.py`

 * *Files identical despite different names*

### Comparing `pyrtz-0.1.7/pyrtz/asylum.py` & `pyrtz-0.1.8/pyrtz/asylum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import igor.binarywave as bw
+import igor2.binarywave as bw
 import numpy as np
 import pandas as pd
 import pyrtz.curves
 import re
 import os
 
 def _get_notes(wave):
```

### Comparing `pyrtz-0.1.7/pyrtz/curves.py` & `pyrtz-0.1.8/pyrtz/curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -858,15 +858,15 @@
         filepath: The path where the fit report should be
         saved
 
         ---------------------Returns---------------------
 
         None'''
 
-        merger=pdf.PdfFileMerger()
+        merger=pdf.PdfMerger()
         for key in self:
             this_curve=self[key]
             if this_curve.stiff_fit==None:
                 raise Exception('Stiffness fit has not been performed, please run stiffness fit before attempting to export fit reports')
             title=''
             for label,ident in zip(self.ident_labels,key):
                 title=title+f'{label}{ident}'
@@ -889,15 +889,15 @@
         filepath: The path where the fit report should be
         saved
 
         ---------------------Returns---------------------
 
         None'''
 
-        merger=pdf.PdfFileMerger()
+        merger=pdf.PdfMerger()
         for key in self:
             this_curve=self[key]
             if this_curve.biexponential_fit==None:
                 raise Exception('Biexponential fit has not been performed, please run biexponential fit before attempting to export fit reports')
             title=''
             for label,ident in zip(self.ident_labels,key):
                 title=title+f'{label}{ident}'
@@ -920,15 +920,15 @@
         filepath: The path where the fit report should be
         saved
 
         ---------------------Returns---------------------
 
         None'''
 
-        merger=pdf.PdfFileMerger()
+        merger=pdf.PdfMerger()
         for key in self:
             this_curve=self[key]
             if this_curve.exponential_fit==None:
                 raise Exception('Biexponential fit has not been performed, please run biexponential fit before attempting to export fit reports')
             title=''
             for label,ident in zip(self.ident_labels,key):
                 title=title+f'{label}{ident}'
```

### Comparing `pyrtz-0.1.7/pyrtz/utils.py` & `pyrtz-0.1.8/pyrtz/utils.py`

 * *Files identical despite different names*

### Comparing `pyrtz-0.1.7/PKG-INFO` & `pyrtz-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtz
-Version: 0.1.7
+Version: 0.1.8
 Summary: Force spectroscopy in Python
 Home-page: https://github.com/nstone8/pyrtz
 Author: Nicholas Stone
 Author-email: stone.nicholas@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Requires-Dist: pandas >=1.0.5
 Requires-Dist: scipy >=1.4.1
 Requires-Dist: plotly >=5.1.0
 Requires-Dist: dash >=1.21.0
 Requires-Dist: dash_core_components >=1.17.1
 Requires-Dist: dash_html_components >=1.1.4
 Requires-Dist: PyPDF2 >=1.26.0
-Requires-Dist: igor >=0.3
+Requires-Dist: igor2 >=0.5.5
 Requires-Dist: kaleido >=0.2.1
 
 # pyrtz
 
 Analysis of AFM force curves in Python.
 
 Developed at the University of Iowa Institute for Vision Research https://ivr.uiowa.edu/
```

