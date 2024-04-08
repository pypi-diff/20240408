# Comparing `tmp/matplotlib_visual-0.9.1.tar.gz` & `tmp/matplotlib_visual-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib_visual-0.9.1.tar", last modified: Mon Apr  8 13:14:58 2024, max compression
+gzip compressed data, was "matplotlib_visual-0.9.2.tar", last modified: Mon Apr  8 13:59:36 2024, max compression
```

## Comparing `matplotlib_visual-0.9.1.tar` & `matplotlib_visual-0.9.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-08 13:14:58.299340 matplotlib_visual-0.9.1/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)    35149 2024-01-30 14:32:10.000000 matplotlib_visual-0.9.1/LICENSE
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-04-08 13:14:58.298340 matplotlib_visual-0.9.1/PKG-INFO
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1753 2024-03-29 07:11:10.000000 matplotlib_visual-0.9.1/README.md
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-08 13:14:58.294340 matplotlib_visual-0.9.1/matplotlib_visual/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 14:35:01.000000 matplotlib_visual-0.9.1/matplotlib_visual/__init__.py
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-08 13:14:58.297340 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 15:02:02.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/__init__.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      568 2024-03-29 07:18:38.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/god.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-02-04 07:14:39.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir1.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      624 2024-02-04 07:15:04.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir2.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      540 2024-02-04 07:15:26.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir3.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      687 2024-02-04 07:16:22.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir4.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 14:59:27.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir5.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     3301 2024-03-13 15:24:02.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir5full.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1225 2024-03-13 15:05:07.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir6.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-03-13 15:10:30.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir7.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 15:03:11.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir8.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1627 2024-04-08 13:09:48.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml10.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1145 2024-04-08 13:13:22.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml11a.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      879 2024-04-08 13:13:05.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml11b.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1047 2024-04-08 13:12:53.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml2.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1814 2024-04-08 13:06:20.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml3.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1303 2024-02-04 07:27:56.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml4.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1153 2024-04-08 13:12:07.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml5.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     2967 2024-04-08 13:11:46.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml6.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      742 2024-03-25 16:15:35.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml7.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1195 2024-03-25 16:15:45.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml8.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1089 2024-04-08 13:09:25.000000 matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml9.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      769 2024-04-07 12:13:26.000000 matplotlib_visual-0.9.1/matplotlib_visual/graph.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      252 2024-03-16 13:23:06.000000 matplotlib_visual-0.9.1/matplotlib_visual/models.py
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-08 13:14:58.298340 matplotlib_visual-0.9.1/matplotlib_visual.egg-info/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-04-08 13:14:58.000000 matplotlib_visual-0.9.1/matplotlib_visual.egg-info/PKG-INFO
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1147 2024-04-08 13:14:58.000000 matplotlib_visual-0.9.1/matplotlib_visual.egg-info/SOURCES.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        1 2024-04-08 13:14:58.000000 matplotlib_visual-0.9.1/matplotlib_visual.egg-info/dependency_links.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       18 2024-04-08 13:14:58.000000 matplotlib_visual-0.9.1/matplotlib_visual.egg-info/top_level.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       38 2024-04-08 13:14:58.299340 matplotlib_visual-0.9.1/setup.cfg
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      333 2024-04-08 13:14:08.000000 matplotlib_visual-0.9.1/setup.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-08 13:59:36.490960 matplotlib_visual-0.9.2/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)    35149 2024-01-30 14:32:10.000000 matplotlib_visual-0.9.2/LICENSE
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-04-08 13:59:36.489960 matplotlib_visual-0.9.2/PKG-INFO
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1753 2024-03-29 07:11:10.000000 matplotlib_visual-0.9.2/README.md
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-08 13:59:36.486960 matplotlib_visual-0.9.2/matplotlib_visual/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 14:35:01.000000 matplotlib_visual-0.9.2/matplotlib_visual/__init__.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-08 13:59:36.489960 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 15:02:02.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/__init__.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      568 2024-03-29 07:18:38.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/god.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-02-04 07:14:39.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir1.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      624 2024-02-04 07:15:04.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir2.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      540 2024-02-04 07:15:26.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir3.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      687 2024-02-04 07:16:22.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir4.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 14:59:27.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir5.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     3301 2024-03-13 15:24:02.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir5full.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1225 2024-03-13 15:05:07.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir6.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-03-13 15:10:30.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir7.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 15:03:11.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir8.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1627 2024-04-08 13:09:48.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml10.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1145 2024-04-08 13:13:22.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml11a.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      879 2024-04-08 13:13:05.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml11b.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1047 2024-04-08 13:12:53.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml2.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1814 2024-04-08 13:06:20.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml3.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1303 2024-02-04 07:27:56.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml4.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1153 2024-04-08 13:12:07.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml5.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     2967 2024-04-08 13:11:46.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml6.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      742 2024-03-25 16:15:35.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml7.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1195 2024-03-25 16:15:45.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml8.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1089 2024-04-08 13:09:25.000000 matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml9.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      769 2024-04-08 13:57:55.000000 matplotlib_visual-0.9.2/matplotlib_visual/graph.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      252 2024-04-08 13:57:54.000000 matplotlib_visual-0.9.2/matplotlib_visual/models.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      376 2024-04-08 13:57:53.000000 matplotlib_visual-0.9.2/matplotlib_visual/piechart.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-08 13:59:36.489960 matplotlib_visual-0.9.2/matplotlib_visual.egg-info/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-04-08 13:59:36.000000 matplotlib_visual-0.9.2/matplotlib_visual.egg-info/PKG-INFO
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1177 2024-04-08 13:59:36.000000 matplotlib_visual-0.9.2/matplotlib_visual.egg-info/SOURCES.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        1 2024-04-08 13:59:36.000000 matplotlib_visual-0.9.2/matplotlib_visual.egg-info/dependency_links.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       18 2024-04-08 13:59:36.000000 matplotlib_visual-0.9.2/matplotlib_visual.egg-info/top_level.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       38 2024-04-08 13:59:36.490960 matplotlib_visual-0.9.2/setup.cfg
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      333 2024-04-08 13:58:25.000000 matplotlib_visual-0.9.2/setup.py
```

### Comparing `matplotlib_visual-0.9.1/LICENSE` & `matplotlib_visual-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/README.md` & `matplotlib_visual-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/god.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/god.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir1.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir1.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir2.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir2.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir3.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir3.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir4.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir4.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir5.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir5.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir5full.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir5full.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir6.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir6.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir7.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir7.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ir8.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ir8.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml10.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml10.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml11a.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml11a.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml11b.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml11b.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml2.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml2.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml3.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml3.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml4.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml4.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml5.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml5.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml6.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml6.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml7.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml7.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml8.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml8.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/code_snippets/ml9.py` & `matplotlib_visual-0.9.2/matplotlib_visual/code_snippets/ml9.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual/graph.py` & `matplotlib_visual-0.9.2/matplotlib_visual/graph.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.1/matplotlib_visual.egg-info/SOURCES.txt` & `matplotlib_visual-0.9.2/matplotlib_visual.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 matplotlib_visual/__init__.py
 matplotlib_visual/graph.py
 matplotlib_visual/models.py
+matplotlib_visual/piechart.py
 matplotlib_visual.egg-info/PKG-INFO
 matplotlib_visual.egg-info/SOURCES.txt
 matplotlib_visual.egg-info/dependency_links.txt
 matplotlib_visual.egg-info/top_level.txt
 matplotlib_visual/code_snippets/__init__.py
 matplotlib_visual/code_snippets/god.py
 matplotlib_visual/code_snippets/ir1.py
```

