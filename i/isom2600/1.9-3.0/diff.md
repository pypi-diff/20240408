# Comparing `tmp/isom2600-1.9.tar.gz` & `tmp/isom2600-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isom2600-1.9.tar", last modified: Fri Mar 15 23:43:49 2024, max compression
+gzip compressed data, was "isom2600-3.0.tar", last modified: Mon Apr  8 04:28:39 2024, max compression
```

## Comparing `isom2600-1.9.tar` & `isom2600-3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 23:43:49.833294 isom2600-1.9/
--rw-rw-rw-   0        0        0       85 2024-03-15 23:43:49.830945 isom2600-1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-15 23:43:49.823137 isom2600-1.9/isom2600/
--rw-rw-rw-   0        0        0       44 2024-03-15 15:35:38.000000 isom2600-1.9/isom2600/__init__.py
--rw-rw-rw-   0        0        0     2241 2024-03-15 23:43:37.000000 isom2600-1.9/isom2600/data.py
--rw-rw-rw-   0        0        0     2222 2024-03-15 15:38:21.000000 isom2600-1.9/isom2600/regression.py
-drwxrwxrwx   0        0        0        0 2024-03-15 23:43:49.828697 isom2600-1.9/isom2600.egg-info/
--rw-rw-rw-   0        0        0       85 2024-03-15 23:43:49.000000 isom2600-1.9/isom2600.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-03-15 23:43:49.000000 isom2600-1.9/isom2600.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 23:43:49.000000 isom2600-1.9/isom2600.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-15 23:43:49.000000 isom2600-1.9/isom2600.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-15 23:43:49.833294 isom2600-1.9/setup.cfg
--rw-rw-rw-   0        0        0      146 2024-03-15 23:43:45.000000 isom2600-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:28:39.586175 isom2600-3.0/
+-rw-rw-rw-   0        0        0       85 2024-04-08 04:28:39.583215 isom2600-3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-08 04:28:39.569193 isom2600-3.0/isom2600/
+-rw-rw-rw-   0        0        0       44 2024-03-15 15:35:38.000000 isom2600-3.0/isom2600/__init__.py
+-rw-rw-rw-   0        0        0     2335 2024-04-08 04:26:45.000000 isom2600-3.0/isom2600/data.py
+-rw-rw-rw-   0        0        0     2222 2024-03-15 15:38:21.000000 isom2600-3.0/isom2600/regression.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:28:39.580192 isom2600-3.0/isom2600.egg-info/
+-rw-rw-rw-   0        0        0       85 2024-04-08 04:28:39.000000 isom2600-3.0/isom2600.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-08 04:28:39.000000 isom2600-3.0/isom2600.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 04:28:39.000000 isom2600-3.0/isom2600.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 04:28:39.000000 isom2600-3.0/isom2600.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 04:28:39.587183 isom2600-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      146 2024-04-08 04:28:36.000000 isom2600-3.0/setup.py
```

### Comparing `isom2600-1.9/isom2600/data.py` & `isom2600-3.0/isom2600/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import pandas as pd
 import numpy as np
+import yfinance as yf
+def getStock(symbol):
+    return yf.download(symbol, progress=False)
 
 def energy(Clean=True):
     url = 'https://drive.google.com/file/d/1EpczybaLAzV053G8pG-kB38IXT7NC580/view?usp=sharing'
     data_path = 'https://drive.google.com/uc?export=download&id=' + url.split('/')[-2]
     df = pd.read_csv(data_path,index_col=0)
     if Clean==True:
         df.index=pd.to_datetime(df.index)
```

### Comparing `isom2600-1.9/isom2600/regression.py` & `isom2600-3.0/isom2600/regression.py`

 * *Files identical despite different names*

