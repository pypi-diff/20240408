# Comparing `tmp/SOMcreator-1.6.8.tar.gz` & `tmp/SOMcreator-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SOMcreator-1.6.8.tar", last modified: Thu Feb 22 12:34:37 2024, max compression
+gzip compressed data, was "SOMcreator-1.6.9.tar", last modified: Fri Mar  1 07:43:59 2024, max compression
```

## Comparing `SOMcreator-1.6.8.tar` & `SOMcreator-1.6.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.869413 SOMcreator-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-22 12:34:37.869413 SOMcreator-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 12:34:37.869413 SOMcreator-1.6.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.853413 SOMcreator-1.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.857413 SOMcreator-1.6.8/src/SOMcreator/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.861413 SOMcreator-1.6.8/src/SOMcreator/Template/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/Template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.861413 SOMcreator-1.6.8/src/SOMcreator/Template/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/Template/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/Template/bookmark_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/Template/fast_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/Template/ifc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.861413 SOMcreator-1.6.8/src/SOMcreator/Template/js_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/Template/js_templates/start_check_start.js
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/Template/js_templates/start_koordinaten.js
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/Template/mapping_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/Template/template.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/Template/untested_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38909 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.861413 SOMcreator-1.6.8/src/SOMcreator/constants/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/constants/ifc_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/constants/json_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/constants/log_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/constants/value_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.861413 SOMcreator-1.6.8/src/SOMcreator/external_software/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.861413 SOMcreator-1.6.8/src/SOMcreator/external_software/IDS/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/IDS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/IDS/ids_xsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/IDS/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/IDS/xml_xsd.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/allplan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.865413 SOMcreator-1.6.8/src/SOMcreator/external_software/bim_collab_zoom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/bim_collab_zoom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/bim_collab_zoom/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/bim_collab_zoom/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/bim_collab_zoom/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/bim_collab_zoom/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/card1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.865413 SOMcreator-1.6.8/src/SOMcreator/external_software/desite/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/desite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/desite/attribute_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/desite/bill_of_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/desite/bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/desite/building_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    19687 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/desite/modelcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)    21973 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/revit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/external_software/vestra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.865413 SOMcreator-1.6.8/src/SOMcreator/filehandling/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/filehandling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/filehandling/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/filehandling/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/filehandling/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/filehandling/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/filehandling/inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/filehandling/obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/filehandling/predefined_pset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/filehandling/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/filehandling/property_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/filehandling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.865413 SOMcreator-1.6.8/src/SOMcreator/ifc_modification/
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/ifc_modification/grouping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.869413 SOMcreator-1.6.8/src/SOMcreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-02-22 12:34:30.000000 SOMcreator-1.6.8/src/SOMcreator/tools/merge_projects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:34:37.869413 SOMcreator-1.6.8/src/SOMcreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-22 12:34:37.000000 SOMcreator-1.6.8/src/SOMcreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-02-22 12:34:37.000000 SOMcreator-1.6.8/src/SOMcreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 12:34:37.000000 SOMcreator-1.6.8/src/SOMcreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-22 12:34:37.000000 SOMcreator-1.6.8/src/SOMcreator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-22 12:34:37.000000 SOMcreator-1.6.8/src/SOMcreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-22 12:34:37.000000 SOMcreator-1.6.8/src/SOMcreator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.219555 SOMcreator-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-01 07:43:59.219555 SOMcreator-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 07:43:59.219555 SOMcreator-1.6.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.207556 SOMcreator-1.6.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.207556 SOMcreator-1.6.9/src/SOMcreator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/Template/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/Template/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/bookmark_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/fast_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/ifc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/Template/js_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/js_templates/start_check_start.js
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/js_templates/start_koordinaten.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/mapping_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/untested_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39045 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/constants/ifc_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/constants/json_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/constants/log_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/constants/value_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/external_software/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/ids_xsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/xml_xsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/allplan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.215556 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/card1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.215556 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/attribute_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/bill_of_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/building_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19687 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/modelcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21973 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/revit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/vestra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.215556 SOMcreator-1.6.9/src/SOMcreator/filehandling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/predefined_pset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/property_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.215556 SOMcreator-1.6.9/src/SOMcreator/ifc_modification/
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/ifc_modification/grouping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.219555 SOMcreator-1.6.9/src/SOMcreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/tools/merge_projects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.219555 SOMcreator-1.6.9/src/SOMcreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/top_level.txt
```

### Comparing `SOMcreator-1.6.8/LICENSE` & `SOMcreator-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/PKG-INFO` & `SOMcreator-1.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.6.8
+Version: 1.6.9
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.6.8/pyproject.toml` & `SOMcreator-1.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/Template/fast_template.txt` & `SOMcreator-1.6.9/src/SOMcreator/Template/fast_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/Template/ifc.json` & `SOMcreator-1.6.9/src/SOMcreator/Template/ifc.json`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/Template/js_templates/start_check_start.js` & `SOMcreator-1.6.9/src/SOMcreator/Template/js_templates/start_check_start.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/Template/js_templates/start_koordinaten.js` & `SOMcreator-1.6.9/src/SOMcreator/Template/js_templates/start_koordinaten.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/Template/mapping_template.txt` & `SOMcreator-1.6.9/src/SOMcreator/Template/mapping_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/Template/template.txt` & `SOMcreator-1.6.9/src/SOMcreator/Template/template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/Template/untested_template.txt` & `SOMcreator-1.6.9/src/SOMcreator/Template/untested_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/classes.py` & `SOMcreator-1.6.9/src/SOMcreator/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Iterator, Union
 from uuid import uuid4
 
 import copy as cp
 from anytree import AnyNode
 
 from . import filehandling
-from .constants import value_constants, json_constants
+from .constants import value_constants
 from dataclasses import dataclass, field
 
 
 # Add child to Parent leads to reverse
 
 def filter_by_filter_dict(func):
     """decorator function that filters list output of function by project phase and use_case"""
@@ -509,14 +509,15 @@
     def add_child(self, child: PropertySet | Object | Attribute | Aggregation) -> None:
         self._children.add(child)
         child.parent = self
 
     def remove_child(self, child: PropertySet | Object | Attribute | Aggregation | Hirarchy) -> None:
         if child in self._children:
             self._children.remove(child)
+            child.remove_parent()
 
     def delete(self, recursive: bool = False) -> None:
         logging.info(f"Delete {self.__class__.__name__} {self.name} (recursive: {recursive})")
         if self.parent is not None:
             self.parent.remove_child(self)
 
         if self in self._registry:
@@ -787,14 +788,20 @@
         :return:
         """
         if parent is None:
             self.remove_parent()
             return
         self._parent = parent
 
+    def remove_child(self, child: PropertySet) -> None:
+        super().remove_child(child)
+        child.remove_parent()
+        for attribute in [a for a in child.attributes if a.parent]:
+            attribute.parent.remove_child(attribute)
+
     def change_parent(self, new_parent: PropertySet) -> None:
         for attribute in self.attributes:
             if attribute.parent.property_set == self._parent:
                 self.remove_attribute(attribute)
         self.parent = new_parent
 
     def delete(self, recursive: bool = False, override_ident_deletion=False) -> None:
@@ -1097,18 +1104,14 @@
     def set_parent(self, value, connection_type):
         if self.parent is not None and value != self.parent:
             return False
         self._parent = value
         self._parent_connection = connection_type
         return True
 
-    def remove_child(self, value: Aggregation):
-        if value in self._children:
-            self._children.remove(value)
-
     def add_child(self, child: Aggregation, connection_type: int = value_constants.AGGREGATION) -> bool:
         """returns if adding child is allowed"""
 
         def loop_parents(element, search_value):
             if element.parent is None:
                 return True
             if element.parent.object == search_value:
```

### Comparing `SOMcreator-1.6.8/src/SOMcreator/constants/ifc_datatypes.py` & `SOMcreator-1.6.9/src/SOMcreator/constants/ifc_datatypes.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/constants/value_constants.py` & `SOMcreator-1.6.9/src/SOMcreator/constants/value_constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/IDS/ids_xsd.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/ids_xsd.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/IDS/main.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/main.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/IDS/xml_xsd.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/xml_xsd.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/allplan.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/allplan.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/bim_collab_zoom/condition.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/condition.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/bim_collab_zoom/constants.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/bim_collab_zoom/rule.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/rule.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/card1.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/card1.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/desite/__init__.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/__init__.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/desite/attribute_json.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/attribute_json.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/desite/bill_of_quantities.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/bill_of_quantities.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/desite/bookmarks.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/bookmarks.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/desite/building_structure.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/building_structure.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/desite/modelcheck.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/modelcheck.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/excel.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/excel.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/revit.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/revit.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/external_software/vestra.py` & `SOMcreator-1.6.9/src/SOMcreator/external_software/vestra.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/filehandling/__init__.py` & `SOMcreator-1.6.9/src/SOMcreator/filehandling/__init__.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/filehandling/aggregation.py` & `SOMcreator-1.6.9/src/SOMcreator/filehandling/aggregation.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/filehandling/attribute.py` & `SOMcreator-1.6.9/src/SOMcreator/filehandling/attribute.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/filehandling/constants.py` & `SOMcreator-1.6.9/src/SOMcreator/filehandling/constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/filehandling/core.py` & `SOMcreator-1.6.9/src/SOMcreator/filehandling/core.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/filehandling/inheritance.py` & `SOMcreator-1.6.9/src/SOMcreator/filehandling/inheritance.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/filehandling/obj.py` & `SOMcreator-1.6.9/src/SOMcreator/filehandling/obj.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/filehandling/predefined_pset.py` & `SOMcreator-1.6.9/src/SOMcreator/filehandling/predefined_pset.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/filehandling/project.py` & `SOMcreator-1.6.9/src/SOMcreator/filehandling/project.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/filehandling/property_set.py` & `SOMcreator-1.6.9/src/SOMcreator/filehandling/property_set.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/filehandling/typing.py` & `SOMcreator-1.6.9/src/SOMcreator/filehandling/typing.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/ifc_modification/grouping.py` & `SOMcreator-1.6.9/src/SOMcreator/ifc_modification/grouping.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator/tools/merge_projects.py` & `SOMcreator-1.6.9/src/SOMcreator/tools/merge_projects.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.8/src/SOMcreator.egg-info/PKG-INFO` & `SOMcreator-1.6.9/src/SOMcreator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.6.8
+Version: 1.6.9
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.6.8/src/SOMcreator.egg-info/SOURCES.txt` & `SOMcreator-1.6.9/src/SOMcreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

