# Comparing `tmp/datamazing-4.1.2.tar.gz` & `tmp/datamazing-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-4.1.2.tar", max compression
+gzip compressed data, was "datamazing-4.2.0.tar", max compression
```

## Comparing `datamazing-4.1.2.tar` & `datamazing-4.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/__init__.py
--rw-r--r--   0        0        0      277 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/_conform.py
--rw-r--r--   0        0        0      645 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0      309 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/datacollection/__init__.py
--rw-r--r--   0        0        0     2199 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/io.py
--rw-r--r--   0        0        0      140 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      766 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     2711 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0     2384 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     8044 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0     2633 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/transformations/merging.py
--rw-r--r--   0        0        0     2145 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/transformations/reindexing.py
--rw-r--r--   0        0        0     6674 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      695 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pandas/types.py
--rw-r--r--   0        0        0      184 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pyspark/__init__.py
--rw-r--r--   0        0        0       92 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pyspark/testing/__init__.py
--rw-r--r--   0        0        0      295 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pyspark/testing/assertions.py
--rw-r--r--   0        0        0     2363 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pyspark/testing/data.py
--rw-r--r--   0        0        0        0 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pyspark/transformations/__init__.py
--rw-r--r--   0        0        0     3487 2024-03-20 13:52:17.880104 datamazing-4.1.2/datamazing/pyspark/transformations/grouping.py
--rw-r--r--   0        0        0      734 2024-03-20 13:52:17.880104 datamazing-4.1.2/pyproject.toml
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 datamazing-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-08 12:48:29.572371 datamazing-4.2.0/datamazing/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-08 12:48:29.572371 datamazing-4.2.0/datamazing/_conform.py
+-rw-r--r--   0        0        0      645 2024-04-08 12:48:29.572371 datamazing-4.2.0/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0     2199 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/io.py
+-rw-r--r--   0        0        0      140 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      766 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     2814 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0     2384 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     8044 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0     2633 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/transformations/merging.py
+-rw-r--r--   0        0        0     2145 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/transformations/reindexing.py
+-rw-r--r--   0        0        0     6674 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      695 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      184 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pyspark/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pyspark/testing/__init__.py
+-rw-r--r--   0        0        0      295 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pyspark/testing/assertions.py
+-rw-r--r--   0        0        0     2363 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pyspark/testing/data.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pyspark/transformations/__init__.py
+-rw-r--r--   0        0        0     3487 2024-04-08 12:48:29.576371 datamazing-4.2.0/datamazing/pyspark/transformations/grouping.py
+-rw-r--r--   0        0        0      734 2024-04-08 12:48:29.576371 datamazing-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 datamazing-4.2.0/PKG-INFO
```

### Comparing `datamazing-4.1.2/datamazing/pandas/__init__.py` & `datamazing-4.2.0/datamazing/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.1.2/datamazing/pandas/io.py` & `datamazing-4.2.0/datamazing/pandas/io.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.1.2/datamazing/pandas/testing/assertions.py` & `datamazing-4.2.0/datamazing/pandas/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.1.2/datamazing/pandas/testing/data.py` & `datamazing-4.2.0/datamazing/pandas/testing/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,11 +80,15 @@
             # filter to time interval
             is_after_start = df[self.time_column] >= time_interval.left
             is_before_end = df[self.time_column] <= time_interval.right
             is_in_interval = is_after_start & is_before_end
             df = df[is_in_interval]
 
         if filters:
-            df = df[(df[filters.keys()] == filters.values()).all(axis=1)]
+            for key, value in filters.items():
+                if not isinstance(value, list):
+                    value = [value]
+                df = df[df[key].isin(value)]
+
             df = df.reset_index(drop=True)
 
         return df
```

### Comparing `datamazing-4.1.2/datamazing/pandas/transformations/basic.py` & `datamazing-4.2.0/datamazing/pandas/transformations/basic.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.1.2/datamazing/pandas/transformations/grouping.py` & `datamazing-4.2.0/datamazing/pandas/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.1.2/datamazing/pandas/transformations/merging.py` & `datamazing-4.2.0/datamazing/pandas/transformations/merging.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.1.2/datamazing/pandas/transformations/reindexing.py` & `datamazing-4.2.0/datamazing/pandas/transformations/reindexing.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.1.2/datamazing/pandas/transformations/resampling.py` & `datamazing-4.2.0/datamazing/pandas/transformations/resampling.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.1.2/datamazing/pandas/types.py` & `datamazing-4.2.0/datamazing/pandas/types.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.1.2/datamazing/pyspark/testing/data.py` & `datamazing-4.2.0/datamazing/pyspark/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.1.2/datamazing/pyspark/transformations/grouping.py` & `datamazing-4.2.0/datamazing/pyspark/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.1.2/pyproject.toml` & `datamazing-4.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "4.1.2"
+version = "4.2.0"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

