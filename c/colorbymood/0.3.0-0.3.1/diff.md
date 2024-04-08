# Comparing `tmp/colorbymood-0.3.0.tar.gz` & `tmp/colorbymood-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorbymood-0.3.0.tar", max compression
+gzip compressed data, was "colorbymood-0.3.1.tar", max compression
```

## Comparing `colorbymood-0.3.0.tar` & `colorbymood-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       18 2023-12-13 10:59:39.168901 colorbymood-0.3.0/README.md
--rw-r--r--   0        0        0      285 2023-12-13 10:59:39.168901 colorbymood-0.3.0/colorbymood/__init__.py
--rw-r--r--   0        0        0      991 2023-12-13 10:59:39.168901 colorbymood-0.3.0/colorbymood/cli.py
--rw-r--r--   0        0        0     1643 2023-12-13 10:59:39.168901 colorbymood-0.3.0/colorbymood/click_utils.py
--rw-r--r--   0        0        0     1809 2023-12-13 10:59:39.168901 colorbymood-0.3.0/colorbymood/color.py
--rw-r--r--   0        0        0      491 2023-12-13 10:59:39.168901 colorbymood-0.3.0/colorbymood/color.yaml
--rw-r--r--   0        0        0     1061 2023-12-13 10:59:39.168901 colorbymood-0.3.0/colorbymood/frequency.yaml
--rw-r--r--   0        0        0      536 2023-12-13 10:59:39.168901 colorbymood-0.3.0/colorbymood/io.py
--rw-r--r--   0        0        0     2429 2023-12-13 10:59:39.168901 colorbymood-0.3.0/colorbymood/window.py
--rw-r--r--   0        0        0      631 2023-12-13 10:59:39.168901 colorbymood-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 colorbymood-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-04-08 20:14:49.155957 colorbymood-0.3.1/README.md
+-rw-r--r--   0        0        0      286 2024-04-08 20:14:49.155957 colorbymood-0.3.1/colorbymood/__init__.py
+-rw-r--r--   0        0        0      992 2024-04-08 20:14:49.155957 colorbymood-0.3.1/colorbymood/cli.py
+-rw-r--r--   0        0        0     1644 2024-04-08 20:14:49.155957 colorbymood-0.3.1/colorbymood/click_utils.py
+-rw-r--r--   0        0        0     1810 2024-04-08 20:14:49.155957 colorbymood-0.3.1/colorbymood/color.py
+-rw-r--r--   0        0        0      491 2024-04-08 20:14:49.155957 colorbymood-0.3.1/colorbymood/color.yaml
+-rw-r--r--   0        0        0     1061 2024-04-08 20:14:49.155957 colorbymood-0.3.1/colorbymood/frequency.yaml
+-rw-r--r--   0        0        0      537 2024-04-08 20:14:49.155957 colorbymood-0.3.1/colorbymood/io.py
+-rw-r--r--   0        0        0     2430 2024-04-08 20:14:49.155957 colorbymood-0.3.1/colorbymood/window.py
+-rw-r--r--   0        0        0     1274 2024-04-08 20:14:49.159957 colorbymood-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 colorbymood-0.3.1/PKG-INFO
```

### Comparing `colorbymood-0.3.0/colorbymood/cli.py` & `colorbymood-0.3.1/colorbymood/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 entry point to the colorbymood program.
 """
+
 import sys
 
 import click
 from PyQt6.QtWidgets import QApplication  # pylint: disable=E0611
 
 import colorbymood
 from colorbymood import Window, hex_from_dict
```

### Comparing `colorbymood-0.3.0/colorbymood/click_utils.py` & `colorbymood-0.3.1/colorbymood/click_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """handles the addition of command line arguments to the script."""
+
 from typing import Any, Callable
 
 import click
 
 from colorbymood.color import get_colors_from_yaml, get_frequency_from_yaml
```

### Comparing `colorbymood-0.3.0/colorbymood/color.py` & `colorbymood-0.3.1/colorbymood/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """handles import and conversion of color values."""
+
 import random
 from colorsys import hls_to_rgb
 from typing import Union
 
 from matplotlib.colors import rgb2hex
 
 from colorbymood.io import load_dicts_from_yaml
```

### Comparing `colorbymood-0.3.0/colorbymood/frequency.yaml` & `colorbymood-0.3.1/colorbymood/frequency.yaml`

 * *Files identical despite different names*

### Comparing `colorbymood-0.3.0/colorbymood/io.py` & `colorbymood-0.3.1/colorbymood/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """reading yaml files."""
+
 from os.path import dirname
 from typing import Any
 
 from yaml import Loader, load  # pylint: disable=E0401
 
 
 def load_dicts_from_yaml(filename: str) -> dict[str, Any]:
```

### Comparing `colorbymood-0.3.0/colorbymood/window.py` & `colorbymood-0.3.1/colorbymood/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains class for gui window with flashing background."""
+
 from PyQt6.QtCore import QEasingCurve  # pylint: disable=E0611
 from PyQt6.QtCore import QPropertyAnimation
 from PyQt6.QtWidgets import QMainWindow  # pylint: disable=E0611
 
 from colorbymood.color import (  # type: ignore pylint: disable=E0611
     create_random_interims,
     get_frequency_from_yaml,
```

### Comparing `colorbymood-0.3.0/PKG-INFO` & `colorbymood-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorbymood
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Niels Maedern
 Author-email: maedern@student.ethz.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

