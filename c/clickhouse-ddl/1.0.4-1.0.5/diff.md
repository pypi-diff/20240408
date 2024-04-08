# Comparing `tmp/clickhouse_ddl-1.0.4.tar.gz` & `tmp/clickhouse_ddl-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse_ddl-1.0.4.tar", last modified: Mon Jul  3 14:51:17 2023, max compression
+gzip compressed data, was "clickhouse_ddl-1.0.5.tar", last modified: Mon Apr  8 09:31:19 2024, max compression
```

## Comparing `clickhouse_ddl-1.0.4.tar` & `clickhouse_ddl-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 14:51:17.056192 clickhouse_ddl-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-05-12 09:58:35.000000 clickhouse_ddl-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1718 2023-07-03 14:51:17.056192 clickhouse_ddl-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2023-05-12 11:55:34.000000 clickhouse_ddl-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 14:51:17.051192 clickhouse_ddl-1.0.4/clickhouse_ddl/
--rw-rw-rw-   0        0        0    21549 2023-07-03 14:50:42.000000 clickhouse_ddl-1.0.4/clickhouse_ddl/ClickHouseDDL.py
--rw-rw-rw-   0        0        0      392 2023-05-12 10:57:55.000000 clickhouse_ddl-1.0.4/clickhouse_ddl/Config.py
--rw-rw-rw-   0        0        0     1234 2023-05-12 10:01:56.000000 clickhouse_ddl-1.0.4/clickhouse_ddl/Function.py
--rw-rw-rw-   0        0        0        0 2023-05-12 10:02:23.000000 clickhouse_ddl-1.0.4/clickhouse_ddl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:51:17.055192 clickhouse_ddl-1.0.4/clickhouse_ddl.egg-info/
--rw-rw-rw-   0        0        0     1718 2023-07-03 14:51:16.000000 clickhouse_ddl-1.0.4/clickhouse_ddl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-07-03 14:51:16.000000 clickhouse_ddl-1.0.4/clickhouse_ddl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 14:51:16.000000 clickhouse_ddl-1.0.4/clickhouse_ddl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-03 14:51:16.000000 clickhouse_ddl-1.0.4/clickhouse_ddl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-03 14:51:16.000000 clickhouse_ddl-1.0.4/clickhouse_ddl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 14:51:17.056192 clickhouse_ddl-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      753 2023-07-03 14:51:11.000000 clickhouse_ddl-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:31:19.663657 clickhouse_ddl-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-05-12 09:58:35.000000 clickhouse_ddl-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1677 2024-04-08 09:31:19.663657 clickhouse_ddl-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2023-05-12 11:55:34.000000 clickhouse_ddl-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 09:31:19.658657 clickhouse_ddl-1.0.5/clickhouse_ddl/
+-rw-rw-rw-   0        0        0    21547 2024-04-08 09:22:11.000000 clickhouse_ddl-1.0.5/clickhouse_ddl/ClickHouseDDL.py
+-rw-rw-rw-   0        0        0      392 2023-05-12 10:57:55.000000 clickhouse_ddl-1.0.5/clickhouse_ddl/Config.py
+-rw-rw-rw-   0        0        0     1234 2023-05-12 10:01:56.000000 clickhouse_ddl-1.0.5/clickhouse_ddl/Function.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 10:02:23.000000 clickhouse_ddl-1.0.5/clickhouse_ddl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:31:19.662657 clickhouse_ddl-1.0.5/clickhouse_ddl.egg-info/
+-rw-rw-rw-   0        0        0     1677 2024-04-08 09:31:19.000000 clickhouse_ddl-1.0.5/clickhouse_ddl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-04-08 09:31:19.000000 clickhouse_ddl-1.0.5/clickhouse_ddl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 09:31:19.000000 clickhouse_ddl-1.0.5/clickhouse_ddl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-08 09:31:19.000000 clickhouse_ddl-1.0.5/clickhouse_ddl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 09:31:19.000000 clickhouse_ddl-1.0.5/clickhouse_ddl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 09:31:19.663657 clickhouse_ddl-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      753 2024-04-08 09:22:31.000000 clickhouse_ddl-1.0.5/setup.py
```

### Comparing `clickhouse_ddl-1.0.4/LICENSE` & `clickhouse_ddl-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse_ddl-1.0.4/PKG-INFO` & `clickhouse_ddl-1.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: clickhouse_ddl
-Version: 1.0.4
-Summary: Clickhouse metadata (DDL) grabber
-Home-page: https://github.com/ish1mura/clickhouse_ddl
-Author: ish1mura
-Author-email: ek.dummy@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ClickHouse DDL Parser
 
 # Description
 
 Clickhouse metadata (DDL) grabber
 
 # Dependencies
@@ -67,9 +52,7 @@
     ddl = ClickHouseDDL(path_result)
 ```
 
 # Links
 
 * [GitHub](https://github.com/ish1mura/clickhouse_ddl)
 * [PyPI](https://pypi.org/project/clickhouse-ddl/)
-
-
```

### Comparing `clickhouse_ddl-1.0.4/README.md` & `clickhouse_ddl-1.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: clickhouse_ddl
+Version: 1.0.5
+Summary: Clickhouse metadata (DDL) grabber
+Home-page: https://github.com/ish1mura/clickhouse_ddl
+Author: ish1mura
+Author-email: ek.dummy@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ClickHouse DDL Parser
 
 # Description
 
 Clickhouse metadata (DDL) grabber
 
 # Dependencies
```

### Comparing `clickhouse_ddl-1.0.4/clickhouse_ddl/ClickHouseDDL.py` & `clickhouse_ddl-1.0.5/clickhouse_ddl/ClickHouseDDL.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/local/bin/python
 # -*- coding: utf-8 -*-
 
-import os, re, json, shutil
+import os, re, json
 from multiprocessing import Pool
 from clickhouse_driver import Client
 from clickhouse_ddl.Config import Config
 from clickhouse_ddl.Function import Function
 
 RE_FLAGS = re.MULTILINE | re.IGNORECASE
 
@@ -241,29 +241,29 @@
             if is_mat:
                 start_text = f"({Config.NL}    `"
                 start_text_offset = 5
                 end_text = f") AS{Config.NL}"
             else:
                 start_text = f"CREATE VIEW {full_name}{Config.NL}({Config.NL}"
                 start_text_offset = 0
-                end_text = f") AS{Config.NL}("
+                end_text = f"){Config.NL}AS ("
 
             start_ind = ddl.find(start_text)-start_text_offset
             if start_ind < 0:
                 return ddl
             start_ind += len(start_text)-3
 
             end_idx = ddl.find(end_text, start_ind)
             if end_idx < 0:
                 return ddl
             end_idx += 1
 
             ddl = ddl.replace(ddl[start_ind:end_idx], "")
 
-            return ddl.replace(f"{Config.NL}(SELECT", f"({Config.NL}SELECT")
+            return ddl.replace(f"{Config.NL}AS (SELECT", f" AS({Config.NL}SELECT")
 
         self.Views = {}
         for view in self.GetData("""
             SELECT *
             FROM system.tables t
             WHERE
                 t.engine in ('View','MaterializedView') and
```

### Comparing `clickhouse_ddl-1.0.4/clickhouse_ddl/Function.py` & `clickhouse_ddl-1.0.5/clickhouse_ddl/Function.py`

 * *Files identical despite different names*

### Comparing `clickhouse_ddl-1.0.4/clickhouse_ddl.egg-info/PKG-INFO` & `clickhouse_ddl-1.0.5/clickhouse_ddl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: clickhouse-ddl
-Version: 1.0.4
+Version: 1.0.5
 Summary: Clickhouse metadata (DDL) grabber
 Home-page: https://github.com/ish1mura/clickhouse_ddl
 Author: ish1mura
 Author-email: ek.dummy@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ClickHouse DDL Parser
@@ -67,9 +65,7 @@
     ddl = ClickHouseDDL(path_result)
 ```
 
 # Links
 
 * [GitHub](https://github.com/ish1mura/clickhouse_ddl)
 * [PyPI](https://pypi.org/project/clickhouse-ddl/)
-
-
```

### Comparing `clickhouse_ddl-1.0.4/setup.py` & `clickhouse_ddl-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="clickhouse_ddl",
-    version="1.0.4",
+    version="1.0.5",
     author="ish1mura",
     author_email="ek.dummy@gmail.com",
     description="Clickhouse metadata (DDL) grabber",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ish1mura/clickhouse_ddl",
     packages=setuptools.find_packages(),
```

