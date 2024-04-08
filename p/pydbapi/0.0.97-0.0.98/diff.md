# Comparing `tmp/pydbapi-0.0.97.tar.gz` & `tmp/pydbapi-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbapi-0.0.97.tar", last modified: Fri Nov 18 07:18:57 2022, max compression
+gzip compressed data, was "pydbapi-0.0.98.tar", last modified: Fri Nov 18 07:46:19 2022, max compression
```

## Comparing `pydbapi-0.0.97.tar` & `pydbapi-0.0.98.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:18:57.121241 pydbapi-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-11-18 07:18:40.000000 pydbapi-0.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7742 2022-11-18 07:18:57.121241 pydbapi-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7384 2022-11-18 07:18:40.000000 pydbapi-0.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:18:57.121241 pydbapi-0.0.97/pydbapi/
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:18:57.121241 pydbapi-0.0.97/pydbapi/api/
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6657 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/api/mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/api/redshift.py
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/api/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/api/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (121)     9036 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/api/trino.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:18:57.121241 pydbapi-0.0.97/pydbapi/col/
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/col/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/col/colmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:18:57.121241 pydbapi-0.0.97/pydbapi/conf/
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/conf/myhandlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:18:57.121241 pydbapi-0.0.97/pydbapi/db/
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9147 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/db/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/db/fileexec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:18:57.121241 pydbapi-0.0.97/pydbapi/sql/
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5392 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/sql/compile.py
--rw-r--r--   0 runner    (1001) docker     (121)     7049 2022-11-18 07:18:40.000000 pydbapi-0.0.97/pydbapi/sql/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:18:57.121241 pydbapi-0.0.97/pydbapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7742 2022-11-18 07:18:57.000000 pydbapi-0.0.97/pydbapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-11-18 07:18:57.000000 pydbapi-0.0.97/pydbapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 07:18:57.000000 pydbapi-0.0.97/pydbapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-18 07:18:57.000000 pydbapi-0.0.97/pydbapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-18 07:18:57.000000 pydbapi-0.0.97/pydbapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-18 07:18:57.121241 pydbapi-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-11-18 07:18:40.000000 pydbapi-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:46:19.235724 pydbapi-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-11-18 07:46:04.000000 pydbapi-0.0.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7742 2022-11-18 07:46:19.235724 pydbapi-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7384 2022-11-18 07:46:04.000000 pydbapi-0.0.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:46:19.235724 pydbapi-0.0.98/pydbapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:46:19.235724 pydbapi-0.0.98/pydbapi/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6657 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/api/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/api/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/api/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/api/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9171 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/api/trino.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:46:19.235724 pydbapi-0.0.98/pydbapi/col/
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/col/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3944 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/col/colmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:46:19.235724 pydbapi-0.0.98/pydbapi/conf/
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/conf/myhandlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:46:19.235724 pydbapi-0.0.98/pydbapi/db/
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9147 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/db/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/db/fileexec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:46:19.235724 pydbapi-0.0.98/pydbapi/sql/
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5392 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/sql/compile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7049 2022-11-18 07:46:04.000000 pydbapi-0.0.98/pydbapi/sql/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 07:46:19.235724 pydbapi-0.0.98/pydbapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7742 2022-11-18 07:46:19.000000 pydbapi-0.0.98/pydbapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-11-18 07:46:19.000000 pydbapi-0.0.98/pydbapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 07:46:19.000000 pydbapi-0.0.98/pydbapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-18 07:46:19.000000 pydbapi-0.0.98/pydbapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-18 07:46:19.000000 pydbapi-0.0.98/pydbapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-18 07:46:19.235724 pydbapi-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-11-18 07:46:04.000000 pydbapi-0.0.98/setup.py
```

### Comparing `pydbapi-0.0.97/LICENSE` & `pydbapi-0.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/PKG-INFO` & `pydbapi-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbapi
-Version: 0.0.97
+Version: 0.0.98
 Summary: A simple database API
 Home-page: https://pypi.org/project/pydbapi/
 Author: longfengpili
 Author-email: 398745129@qq.com
 Project-URL: Documentation, https://github.com/longfengpili/pydbapi/blob/master/README.md
 Project-URL: Source, https://github.com/longfengpili/pydbapi
 Keywords: dbapi,sqlite3,redshift,snowflake
```

### Comparing `pydbapi-0.0.97/README.md` & `pydbapi-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/__init__.py` & `pydbapi-0.0.98/pydbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/api/__init__.py` & `pydbapi-0.0.98/pydbapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/api/mysql.py` & `pydbapi-0.0.98/pydbapi/api/mysql.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/api/redshift.py` & `pydbapi-0.0.98/pydbapi/api/redshift.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/api/snowflake.py` & `pydbapi-0.0.98/pydbapi/api/snowflake.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/api/sqlite.py` & `pydbapi-0.0.98/pydbapi/api/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/api/trino.py` & `pydbapi-0.0.98/pydbapi/api/trino.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: longfengpili
 # @Date:   2022-11-14 14:17:02
 # @Last Modified by:   longfengpili
-# @Last Modified time: 2022-11-18 15:06:03
+# @Last Modified time: 2022-11-18 15:44:22
 
 
 import re
 import tqdm
 import pandas as pd
 import threading
 
@@ -36,20 +36,24 @@
         coltype = partition.coltype
         if not coltype.startswith('varchar'):
             raise TypeError(f"{partition} only support varchar !")
         partition = f"with (partitioned_by = ARRAY['{partition.newname}'])"
         return partition
 
     def create(self, columns, partition=None):
-        sql = self.create_nonindex(columns)
-
         if partition:
             partition_key = columns.get_column_by_name(partition)
-            partition = self.create_partition(partition_key)
-            sql = sql.replace(';', f'\n{partition};')
+            columns = columns.remove(partition)
+            columns = columns.append(partition_key)
+            partition_sql = self.create_partition(partition_key)
+
+        sql = self.create_nonindex(columns)
+
+        if partition_sql:
+            sql = sql.replace(';', f'\n{partition_sql};')
 
         return sql
 
 
 class TrinoDB(DBMixin, DBFileExec):
     _instance_lock = threading.Lock()
```

### Comparing `pydbapi-0.0.97/pydbapi/col/colmodel.py` & `pydbapi-0.0.98/pydbapi/col/colmodel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # @Author: chunyang.xu
 # @Email:  398745129@qq.com
 # @Date:   2020-11-30 16:28:21
-# @Last Modified time: 2022-11-14 19:08:24
+# @Last Modified time: 2022-11-18 15:40:35
 # @github: https://github.com/longfengpili
 
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 
 class ColumnModel(object):
@@ -60,19 +60,27 @@
         return self.columns[key]
 
     def __contains__(self, name):
         col = self.get_column_by_name(name)
         isin = True if col else False
         return isin
 
-    def append(self, column):
+    def append(self, column: ColumnModel):
         columns = list(self.columns)
         columns.append(column)
         return ColumnsModel(*columns)
 
+    def remove(self, remove_column: str):
+        new_columns = []
+        columns = list(self.columns)
+        for column in columns:
+            if column.newname != remove_column:
+                new_columns.append(column)
+        return ColumnsModel(*new_columns)
+
     @property
     def func_cols(self):
         func_cols = [col for col in self.columns if col.func]
         return func_cols
 
     @property
     def nonfunc_cols(self):
```

### Comparing `pydbapi-0.0.97/pydbapi/conf/myhandlers.py` & `pydbapi-0.0.98/pydbapi/conf/myhandlers.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/conf/settings.py` & `pydbapi-0.0.98/pydbapi/conf/settings.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/db/base.py` & `pydbapi-0.0.98/pydbapi/db/base.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/db/fileexec.py` & `pydbapi-0.0.98/pydbapi/db/fileexec.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/sql/compile.py` & `pydbapi-0.0.98/pydbapi/sql/compile.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi/sql/parse.py` & `pydbapi-0.0.98/pydbapi/sql/parse.py`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/pydbapi.egg-info/PKG-INFO` & `pydbapi-0.0.98/pydbapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbapi
-Version: 0.0.97
+Version: 0.0.98
 Summary: A simple database API
 Home-page: https://pypi.org/project/pydbapi/
 Author: longfengpili
 Author-email: 398745129@qq.com
 Project-URL: Documentation, https://github.com/longfengpili/pydbapi/blob/master/README.md
 Project-URL: Source, https://github.com/longfengpili/pydbapi
 Keywords: dbapi,sqlite3,redshift,snowflake
```

### Comparing `pydbapi-0.0.97/pydbapi.egg-info/SOURCES.txt` & `pydbapi-0.0.98/pydbapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydbapi-0.0.97/setup.py` & `pydbapi-0.0.98/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # @Author: chunyang.xu
 # @Email:  398745129@qq.com
 # @Date:   2020-06-09 16:46:54
-# @Last Modified time: 2022-11-18 15:06:28
+# @Last Modified time: 2022-11-18 15:44:48
 # @github: https://github.com/longfengpili
 
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 import os
 import sys
 import shutil
 import setuptools
 
-VERSION = '0.0.97'
+VERSION = '0.0.98'
 PROJECT_NAME = 'pydbapi'
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 with open('./requirements.txt', 'r', encoding='utf-8') as f:
     requires = f.readlines()
```

