# Comparing `tmp/yaml-to-markdown-0.1.1712531157.tar.gz` & `tmp/yaml-to-markdown-0.1.1712543251.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-to-markdown-0.1.1712531157.tar", last modified: Sun Apr  7 23:05:57 2024, max compression
+gzip compressed data, was "yaml-to-markdown-0.1.1712543251.tar", last modified: Mon Apr  8 02:27:31 2024, max compression
```

## Comparing `yaml-to-markdown-0.1.1712531157.tar` & `yaml-to-markdown-0.1.1712543251.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:05:57.538582 yaml-to-markdown-0.1.1712531157/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 23:04:59.000000 yaml-to-markdown-0.1.1712531157/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-07 23:05:57.538582 yaml-to-markdown-0.1.1712531157/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-07 23:04:59.000000 yaml-to-markdown-0.1.1712531157/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-07 23:05:57.538582 yaml-to-markdown-0.1.1712531157/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-07 23:04:59.000000 yaml-to-markdown-0.1.1712531157/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:05:57.534582 yaml-to-markdown-0.1.1712531157/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:05:57.534582 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:04:59.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-07 23:04:59.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-07 23:04:59.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/convert_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-07 23:04:59.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/md_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-07 23:04:59.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/md_converter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-07 23:04:59.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 23:04:59.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:05:57.538582 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-07 23:05:57.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-07 23:05:57.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:05:57.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 23:05:57.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-07 23:05:57.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-07 23:05:57.000000 yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:27:31.660256 yaml-to-markdown-0.1.1712543251/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-08 02:27:31.660256 yaml-to-markdown-0.1.1712543251/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 02:27:31.660256 yaml-to-markdown-0.1.1712543251/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:27:31.656256 yaml-to-markdown-0.1.1712543251/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:27:31.656256 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/convert_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/md_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/md_converter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 02:26:24.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:27:31.660256 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 02:27:31.000000 yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/top_level.txt
```

### Comparing `yaml-to-markdown-0.1.1712531157/LICENSE` & `yaml-to-markdown-0.1.1712543251/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712531157/PKG-INFO` & `yaml-to-markdown-0.1.1712543251/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-to-markdown
-Version: 0.1.1712531157
+Version: 0.1.1712543251
 Summary: Converts a YAML/JSON file or python Dict/List to a Markdown file
 Home-page: https://anevis.github.io/yaml-to-markdown/
 Author: anevis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
@@ -75,12 +75,12 @@
 
 #### Convert a YAML file to Markdown:
 ```bash
 yaml-to-markdown --output-file output.md --yaml-file test.yaml
 ```
 
 ## Developer Guide
-Please see the [DEVELOPER.md](https://anevis.github.io/yaml-to-markdown/docs/DEVELOPER.md) file for more information on how to contribute to this project.
+Please see the [DEVELOPER.md](https://anevis.github.io/yaml-to-markdown/docs/DEVELOPER.html) file for more information on how to contribute to this project.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](https://anevis.github.io/yaml-to-markdown/LICENSE) file for details.
```

### Comparing `yaml-to-markdown-0.1.1712531157/README.md` & `yaml-to-markdown-0.1.1712543251/README.md`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712531157/setup.py` & `yaml-to-markdown-0.1.1712543251/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ts = calendar.timegm(gmt)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 long_description = long_description.replace(
     "](", "](https://anevis.github.io/yaml-to-markdown/"
-)
+).replace(".md)", ".html)")
 
 with open("requirements.txt", "r") as req_file:
     raw_requirements = req_file.readlines()
 
 requirements: List[str] = []
 for req in raw_requirements:
     if req.strip() == "# Dev dependencies":
```

### Comparing `yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/convert.py` & `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/convert.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/convert_test.py` & `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/convert_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from unittest.mock import mock_open, patch, Mock
 
 import pytest
 
 from yaml_to_markdown.convert import convert
 
 _JSON_DATA = '{"key": "value"}'
+_OUTPUT_FILE_NAME = "output.md"
 
 
 def test_convert_with_no_file() -> None:
     # Execute
     with pytest.raises(
         RuntimeError, match="One of yaml_file or json_file is required."
     ):
@@ -18,26 +19,26 @@
 
 @patch("io.open", new_callable=mock_open(read_data=_JSON_DATA))
 def test_convert_with_json_data(mock_open_file: Mock) -> None:
     # Prepare
     mock_open_file.return_value.__enter__.return_value = StringIO(_JSON_DATA)
 
     # Execute
-    convert(output_file="output.md", json_file="test.json")
+    convert(output_file=_OUTPUT_FILE_NAME, json_file="test.json")
 
     # Assert
     mock_open_file.assert_any_call("test.json", "r", encoding="utf-8")
-    mock_open_file.assert_any_call("output.md", "w", encoding="utf-8")
+    mock_open_file.assert_any_call(_OUTPUT_FILE_NAME, "w", encoding="utf-8")
 
 
 @patch("io.open", new_callable=mock_open())
 def test_convert_with_yaml_data(mock_open_file: Mock) -> None:
     # Prepare
     data = "key: value"
     mock_open_file.return_value.__enter__.return_value = StringIO(data)
 
     # Execute
-    convert(output_file="output.md", yaml_file="test.yaml")
+    convert(output_file=_OUTPUT_FILE_NAME, yaml_file="test.yaml")
 
     # Assert
     mock_open_file.assert_any_call("test.yaml", "r", encoding="utf-8")
-    mock_open_file.assert_any_call("output.md", "w", encoding="utf-8")
+    mock_open_file.assert_any_call(_OUTPUT_FILE_NAME, "w", encoding="utf-8")
```

### Comparing `yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/md_converter.py` & `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/md_converter.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown/md_converter_test.py` & `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown/md_converter_test.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown.egg-info/PKG-INFO` & `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-to-markdown
-Version: 0.1.1712531157
+Version: 0.1.1712543251
 Summary: Converts a YAML/JSON file or python Dict/List to a Markdown file
 Home-page: https://anevis.github.io/yaml-to-markdown/
 Author: anevis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
@@ -75,12 +75,12 @@
 
 #### Convert a YAML file to Markdown:
 ```bash
 yaml-to-markdown --output-file output.md --yaml-file test.yaml
 ```
 
 ## Developer Guide
-Please see the [DEVELOPER.md](https://anevis.github.io/yaml-to-markdown/docs/DEVELOPER.md) file for more information on how to contribute to this project.
+Please see the [DEVELOPER.md](https://anevis.github.io/yaml-to-markdown/docs/DEVELOPER.html) file for more information on how to contribute to this project.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](https://anevis.github.io/yaml-to-markdown/LICENSE) file for details.
```

### Comparing `yaml-to-markdown-0.1.1712531157/src/yaml_to_markdown.egg-info/SOURCES.txt` & `yaml-to-markdown-0.1.1712543251/src/yaml_to_markdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

