# Comparing `tmp/util_td-0.0.2.tar.gz` & `tmp/util_td-0.0.3.tar.gz`

## Comparing `util_td-0.0.2.tar` & `util_td-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 util_td-0.0.2/.git
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 util_td-0.0.2/README.en.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 util_td-0.0.2/__about__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 util_td-0.0.2/array.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 util_td-0.0.2/datetime_.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 util_td-0.0.2/dd.py
--rw-r--r--   0        0        0     8642 2020-02-02 00:00:00.000000 util_td-0.0.2/echart.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 util_td-0.0.2/encrypt.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 util_td-0.0.2/fs.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 util_td-0.0.2/log.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 util_td-0.0.2/os.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 util_td-0.0.2/security.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 util_td-0.0.2/vika.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 util_td-0.0.2/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 util_td-0.0.2/LICENSE
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 util_td-0.0.2/README.md
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 util_td-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 util_td-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 util_td-0.0.3/.git
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 util_td-0.0.3/README.en.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 util_td-0.0.3/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 util_td-0.0.3/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 util_td-0.0.3/array.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 util_td-0.0.3/datetime_.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 util_td-0.0.3/dd.py
+-rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 util_td-0.0.3/echart.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 util_td-0.0.3/encrypt.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 util_td-0.0.3/fs.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 util_td-0.0.3/log.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 util_td-0.0.3/os.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 util_td-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 util_td-0.0.3/security.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 util_td-0.0.3/vika.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 util_td-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 util_td-0.0.3/LICENSE
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 util_td-0.0.3/README.md
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 util_td-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 util_td-0.0.3/PKG-INFO
```

### Comparing `util_td-0.0.2/README.en.md` & `util_td-0.0.3/README.en.md`

 * *Files identical despite different names*

### Comparing `util_td-0.0.2/array.py` & `util_td-0.0.3/array.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,8 +25,12 @@
 		else:
 			filtered = list(filter(lambda x: getattr(x, field) == value, arr))
 	else:
 		filtered = list(filter(fn, arr))
 		
 	return filtered
 
-find_all = find_many
+find_all = find_many
+
+def find_closest(arr, target):
+    closest = min(arr, key=lambda x: abs(x - target))
+    return closest
```

### Comparing `util_td-0.0.2/dd.py` & `util_td-0.0.3/dd.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.2/echart.py` & `util_td-0.0.3/echart.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pyecharts import options as opts
 from pyecharts.charts import Kline, Line, Grid
 import os
 
-from .datetime_ import dt_to_str
+from .datetime import dt_to_str
 
 def line(bars_df, x, y, title='', bs_fields=[], extra=[], render_path='.'):
     html_path = render_path
 
 
     x_data = bars_df[x].tolist()
```

### Comparing `util_td-0.0.2/encrypt.py` & `util_td-0.0.3/encrypt.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.2/fs.py` & `util_td-0.0.3/fs.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.2/log.py` & `util_td-0.0.3/log.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.2/os.py` & `util_td-0.0.3/os.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.2/security.py` & `util_td-0.0.3/security.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.2/vika.py` & `util_td-0.0.3/vika.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.2/.gitignore` & `util_td-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `util_td-0.0.2/LICENSE` & `util_td-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `util_td-0.0.2/README.md` & `util_td-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `util_td-0.0.2/PKG-INFO` & `util_td-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: util_td
-Version: 0.0.2
+Version: 0.0.3
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: multitasking==0.0.11
 Requires-Dist: python-dateutil==2.9.*
 Description-Content-Type: text/markdown
```

