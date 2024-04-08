# Comparing `tmp/mapper_parser-0.0.1.tar.gz` & `tmp/mapper_parser-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapper_parser-0.0.1.tar", last modified: Fri Aug  4 08:07:34 2023, max compression
+gzip compressed data, was "mapper_parser-1.0.tar", last modified: Mon Apr  8 05:17:19 2024, max compression
```

## Comparing `mapper_parser-0.0.1.tar` & `mapper_parser-1.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 08:07:34.399967 mapper_parser-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-08-04 07:45:29.000000 mapper_parser-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2302 2023-08-04 08:07:34.398967 mapper_parser-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      507 2023-08-04 08:07:08.000000 mapper_parser-0.0.1/README.md
--rw-rw-rw-   0        0        0      644 2023-08-04 08:01:14.000000 mapper_parser-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-04 08:07:34.399967 mapper_parser-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-04 08:07:34.387967 mapper_parser-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-04 08:07:34.391966 mapper_parser-0.0.1/src/mapper_parser/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:21:11.000000 mapper_parser-0.0.1/src/mapper_parser/__init__.py
--rw-rw-rw-   0        0        0     4068 2023-08-04 07:35:26.000000 mapper_parser-0.0.1/src/mapper_parser/mapper_parser.py
-drwxrwxrwx   0        0        0        0 2023-08-04 08:07:34.396967 mapper_parser-0.0.1/src/mapper_parser.egg-info/
--rw-rw-rw-   0        0        0     2302 2023-08-04 08:07:34.000000 mapper_parser-0.0.1/src/mapper_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-08-04 08:07:34.000000 mapper_parser-0.0.1/src/mapper_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 08:07:34.000000 mapper_parser-0.0.1/src/mapper_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-04 08:07:34.000000 mapper_parser-0.0.1/src/mapper_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 05:17:19.795507 mapper_parser-1.0/
+-rw-rw-rw-   0        0        0     1016 2024-04-08 05:17:19.794507 mapper_parser-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2023-08-04 08:07:08.000000 mapper_parser-1.0/README.md
+-rw-rw-rw-   0        0        0      642 2024-04-08 05:16:59.000000 mapper_parser-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 05:17:19.795507 mapper_parser-1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 05:17:19.778506 mapper_parser-1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 05:17:19.783507 mapper_parser-1.0/src/mapper_parser/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:21:11.000000 mapper_parser-1.0/src/mapper_parser/__init__.py
+-rw-rw-rw-   0        0        0     4270 2024-04-08 05:16:00.000000 mapper_parser-1.0/src/mapper_parser/mapper_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-08 05:17:19.792509 mapper_parser-1.0/src/mapper_parser.egg-info/
+-rw-rw-rw-   0        0        0     1016 2024-04-08 05:17:19.000000 mapper_parser-1.0/src/mapper_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-04-08 05:17:19.000000 mapper_parser-1.0/src/mapper_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 05:17:19.000000 mapper_parser-1.0/src/mapper_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-08 05:17:19.000000 mapper_parser-1.0/src/mapper_parser.egg-info/top_level.txt
```

### Comparing `mapper_parser-0.0.1/pyproject.toml` & `mapper_parser-1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapper_parser"
-version = "0.0.1"
+version = "1.0"
 authors = [
   { name="Oliver Li", email="441640312@qq.com" },
 ]
 description = "Mybatis mapper xml file parser"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.0"
```

### Comparing `mapper_parser-0.0.1/src/mapper_parser/mapper_parser.py` & `mapper_parser-1.0/src/mapper_parser/mapper_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 import xml.etree.ElementTree as ET
-
+import re
 
 class Mapper(object):
     def __init__(self, namespace, result_maps, sqls, statements):
         self.namespace = namespace
         self.result_maps = result_maps
         self.sqls = sqls
         self.statements = statements
@@ -22,14 +22,22 @@
 class MapperStatement(MapperElement):
     def __init__(self, id, type, start_line, end_line, content, statement_tag, result_map, include_sql):
         super(MapperStatement, self).__init__(id, type, start_line, end_line, content)
         self.statement_tag = statement_tag
         self.result_map = result_map
         self.include_sql = include_sql
 
+def extract_value(string, tag):
+    pattern = tag + r'\s*=\s*"(\w+)"'
+    match = re.search(pattern, string)
+    if match:
+        value = match.group(1)
+        return value
+    else:
+        return None
 
 def parse(filepath):
     # 读取XML文件内容
     with open(filepath, "r", encoding="utf-8") as file:
         xml_content = file.read()
 
     # 解析XML文件
@@ -82,17 +90,17 @@
         end_line = 0
         result_map = None
         include_sql = None
         for i, line in enumerate(xml_content.splitlines(), start=1):
             if f'<{statement_element.tag} id="{statement_id}"' in line:
                 start_line = i
             if f'resultMap="' in line and start_line != 0:
-                result_map = line.split('resultMap="')[1].split('"')[0]
+                result_map = extract_value(line, 'resultMap')
             if line.strip().startswith('<include') and start_line != 0:
-                include_sql = line.split('refid="')[1].split('"')[0]
+                include_sql = extract_value(line, 'refid')
             if f'</{statement_element.tag}>' in line and start_line != 0:
                 end_line = i
                 break
         content = xml_content.splitlines()[start_line - 1: end_line]
         statement_info.append(MapperStatement(statement_id, 'statement', start_line, end_line, content, statement_element.tag, result_map, include_sql))
 
     return Mapper(namespace, result_map_info, sql_info, statement_info)
```

