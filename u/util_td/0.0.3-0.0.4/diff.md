# Comparing `tmp/util_td-0.0.3.tar.gz` & `tmp/util_td-0.0.4.tar.gz`

## Comparing `util_td-0.0.3.tar` & `util_td-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 util_td-0.0.3/.git
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 util_td-0.0.3/README.en.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 util_td-0.0.3/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 util_td-0.0.3/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 util_td-0.0.3/array.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 util_td-0.0.3/datetime_.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 util_td-0.0.3/dd.py
--rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 util_td-0.0.3/echart.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 util_td-0.0.3/encrypt.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 util_td-0.0.3/fs.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 util_td-0.0.3/log.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 util_td-0.0.3/os.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 util_td-0.0.3/requirements.txt
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 util_td-0.0.3/security.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 util_td-0.0.3/vika.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 util_td-0.0.3/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 util_td-0.0.3/LICENSE
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 util_td-0.0.3/README.md
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 util_td-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 util_td-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 util_td-0.0.4/.git
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 util_td-0.0.4/README.en.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 util_td-0.0.4/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 util_td-0.0.4/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 util_td-0.0.4/array.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 util_td-0.0.4/datetime_.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 util_td-0.0.4/dd.py
+-rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 util_td-0.0.4/echart.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 util_td-0.0.4/encrypt.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 util_td-0.0.4/fs.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 util_td-0.0.4/log.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 util_td-0.0.4/os.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 util_td-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 util_td-0.0.4/security.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 util_td-0.0.4/vika.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 util_td-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 util_td-0.0.4/LICENSE
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 util_td-0.0.4/README.md
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 util_td-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 util_td-0.0.4/PKG-INFO
```

### Comparing `util_td-0.0.3/README.en.md` & `util_td-0.0.4/README.en.md`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/array.py` & `util_td-0.0.4/array.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/datetime_.py` & `util_td-0.0.4/datetime_.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/dd.py` & `util_td-0.0.4/dd.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/echart.py` & `util_td-0.0.4/echart.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/encrypt.py` & `util_td-0.0.4/encrypt.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/fs.py` & `util_td-0.0.4/fs.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/log.py` & `util_td-0.0.4/log.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/os.py` & `util_td-0.0.4/os.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/security.py` & `util_td-0.0.4/security.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/vika.py` & `util_td-0.0.4/vika.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/.gitignore` & `util_td-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/LICENSE` & `util_td-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/README.md` & `util_td-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `util_td-0.0.3/PKG-INFO` & `util_td-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.3
 Name: util_td
-Version: 0.0.3
+Version: 0.0.4
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: multitasking==0.0.11
 Requires-Dist: python-dateutil==2.9.*
+Requires-Dist: vika==1.3.1
 Description-Content-Type: text/markdown
 
 # util_py
 
 #### 介绍
 python的常用工具库，例如logger和文件读写等
```

