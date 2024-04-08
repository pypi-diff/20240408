# Comparing `tmp/DrissionRecorder-3.4.13.tar.gz` & `tmp/DrissionRecorder-3.4.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DrissionRecorder-3.4.13.tar", last modified: Sat Apr  6 15:10:27 2024, max compression
+gzip compressed data, was "DrissionRecorder-3.4.14.tar", last modified: Mon Apr  8 12:13:10 2024, max compression
```

## Comparing `DrissionRecorder-3.4.13.tar` & `DrissionRecorder-3.4.14.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 15:10:27.672838 DrissionRecorder-3.4.13/
-drwxrwxrwx   0        0        0        0 2024-04-06 15:10:27.631317 DrissionRecorder-3.4.13/DrissionRecorder/
--rw-rw-rw-   0        0        0      164 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/__init__.py
--rw-rw-rw-   0        0        0     6240 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/base.py
--rw-rw-rw-   0        0        0     1954 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/base.pyi
--rw-rw-rw-   0        0        0     1818 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/byte_recorder.py
--rw-rw-rw-   0        0        0      536 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/byte_recorder.pyi
--rw-rw-rw-   0        0        0     6538 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/db_recorder.py
--rw-rw-rw-   0        0        0      992 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/db_recorder.pyi
--rw-rw-rw-   0        0        0    23153 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/filler.py
--rw-rw-rw-   0        0        0     3287 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/filler.pyi
--rw-rw-rw-   0        0        0     7078 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/recorder.py
--rw-rw-rw-   0        0        0      988 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/recorder.pyi
--rw-rw-rw-   0        0        0    14182 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/setter.py
--rw-rw-rw-   0        0        0     3118 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/setter.pyI
-drwxrwxrwx   0        0        0        0 2024-04-06 15:10:27.657208 DrissionRecorder-3.4.13/DrissionRecorder/style/
--rw-rw-rw-   0        0        0       77 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/style/__init__.py
--rw-rw-rw-   0        0        0    28558 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/style/cell_style.py
--rw-rw-rw-   0        0        0    15846 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/tools.py
--rw-rw-rw-   0        0        0     1935 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/tools.pyi
-drwxrwxrwx   0        0        0        0 2024-04-06 15:10:27.657208 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/
--rw-rw-rw-   0        0        0     4512 2024-04-06 15:10:27.000000 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2024-04-06 15:10:27.000000 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 15:10:27.000000 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 15:10:27.000000 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-06 15:10:27.000000 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/LICENSE
--rw-rw-rw-   0        0        0       30 2024-04-06 15:07:18.000000 DrissionRecorder-3.4.13/MANIFEST.in
--rw-rw-rw-   0        0        0     4512 2024-04-06 15:10:27.672838 DrissionRecorder-3.4.13/PKG-INFO
--rw-rw-rw-   0        0        0     4000 2024-04-06 15:07:18.000000 DrissionRecorder-3.4.13/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 15:10:27.672838 DrissionRecorder-3.4.13/setup.cfg
--rw-rw-rw-   0        0        0      921 2024-04-06 15:07:18.000000 DrissionRecorder-3.4.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:13:10.621431 DrissionRecorder-3.4.14/
+drwxrwxrwx   0        0        0        0 2024-04-08 12:13:10.589209 DrissionRecorder-3.4.14/DrissionRecorder/
+-rw-rw-rw-   0        0        0      164 2024-04-08 12:10:43.000000 DrissionRecorder-3.4.14/DrissionRecorder/__init__.py
+-rw-rw-rw-   0        0        0     6240 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/base.py
+-rw-rw-rw-   0        0        0     1954 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/base.pyi
+-rw-rw-rw-   0        0        0     1818 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/byte_recorder.py
+-rw-rw-rw-   0        0        0      536 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/byte_recorder.pyi
+-rw-rw-rw-   0        0        0     6538 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/db_recorder.py
+-rw-rw-rw-   0        0        0      992 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/db_recorder.pyi
+-rw-rw-rw-   0        0        0    23642 2024-04-08 12:09:10.000000 DrissionRecorder-3.4.14/DrissionRecorder/filler.py
+-rw-rw-rw-   0        0        0     3287 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/filler.pyi
+-rw-rw-rw-   0        0        0     7078 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/recorder.py
+-rw-rw-rw-   0        0        0      988 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/recorder.pyi
+-rw-rw-rw-   0        0        0    14182 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/setter.py
+-rw-rw-rw-   0        0        0     3118 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/setter.pyI
+drwxrwxrwx   0        0        0        0 2024-04-08 12:13:10.608494 DrissionRecorder-3.4.14/DrissionRecorder/style/
+-rw-rw-rw-   0        0        0       77 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/style/__init__.py
+-rw-rw-rw-   0        0        0    28558 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/style/cell_style.py
+-rw-rw-rw-   0        0        0    15846 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/tools.py
+-rw-rw-rw-   0        0        0     1935 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/DrissionRecorder/tools.pyi
+drwxrwxrwx   0        0        0        0 2024-04-08 12:13:10.604926 DrissionRecorder-3.4.14/DrissionRecorder.egg-info/
+-rw-rw-rw-   0        0        0     4512 2024-04-08 12:13:10.000000 DrissionRecorder-3.4.14/DrissionRecorder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      745 2024-04-08 12:13:10.000000 DrissionRecorder-3.4.14/DrissionRecorder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 12:13:10.000000 DrissionRecorder-3.4.14/DrissionRecorder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 12:13:10.000000 DrissionRecorder-3.4.14/DrissionRecorder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-08 12:13:10.000000 DrissionRecorder-3.4.14/DrissionRecorder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/LICENSE
+-rw-rw-rw-   0        0        0       30 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/MANIFEST.in
+-rw-rw-rw-   0        0        0     4512 2024-04-08 12:13:10.620433 DrissionRecorder-3.4.14/PKG-INFO
+-rw-rw-rw-   0        0        0     4000 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 12:13:10.621431 DrissionRecorder-3.4.14/setup.cfg
+-rw-rw-rw-   0        0        0      921 2024-04-08 10:49:37.000000 DrissionRecorder-3.4.14/setup.py
```

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/base.py` & `DrissionRecorder-3.4.14/DrissionRecorder/base.py`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/base.pyi` & `DrissionRecorder-3.4.14/DrissionRecorder/base.pyi`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/byte_recorder.py` & `DrissionRecorder-3.4.14/DrissionRecorder/byte_recorder.py`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/byte_recorder.pyi` & `DrissionRecorder-3.4.14/DrissionRecorder/byte_recorder.pyi`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/db_recorder.py` & `DrissionRecorder-3.4.14/DrissionRecorder/db_recorder.py`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/db_recorder.pyi` & `DrissionRecorder-3.4.14/DrissionRecorder/db_recorder.pyi`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/filler.py` & `DrissionRecorder-3.4.14/DrissionRecorder/filler.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,15 @@
             get_css_head(self, True)
 
         with open(self.path, 'r', encoding=self.encoding) as f:
             reader = csv_reader(f, delimiter=self.delimiter, quotechar=self.quote_char)
             lines = list(reader)
             lines_count = len(lines)
 
+            head_len = len(self._head) if self._fit_head else None
             for i in self._data:
                 if i[0] == 'set_link':
                     coord = parse_coord(i[1][0], self.data_col)
                     now_data = (f'=HYPERLINK("{i[1][1]}","{i[1][2] or i[1][1]}")',)
 
                 elif i[0] == 'set_img':
                     continue
@@ -278,30 +279,34 @@
                     coord = i[0]
                     now_data = i[1]
 
                 row, col = get_usable_coord_int(coord, lines_count, len(lines[0]) if lines_count else 1)
                 now_data = (now_data,) if not isinstance(now_data[0], (list, tuple, dict)) else now_data
 
                 for r, data in enumerate(now_data, row):
-                    if isinstance(data, dict):
-                        if self._fit_head and self._head:
-                            data = ok_list([data.get(h, None) for h in self._head])
-                            col = 1
-                        else:
-                            data = ok_list(data.values())
-
                     for _ in range(r - lines_count):  # 若行数不够，填充行数
                         lines.append([])
                         lines_count += 1
-
                     row_num = r - 1
 
+                    if isinstance(data, dict):
+                        if self._fit_head and self._head:
+                            # 若列数不够，填充空列
+                            lines[row_num].extend([None] * (head_len - len(lines[row_num])))
+                            for k, h in enumerate(self._head):
+                                if h in data:
+                                    lines[row_num][k] = data[h]
+                            lines[row_num] = ok_list(lines[row_num])
+                            continue
+
+                        else:
+                            data = ok_list(data.values())
+
                     # 若列数不够，填充空列
                     lines[row_num].extend([None] * (col - len(lines[row_num]) + len(data) - 1))
-
                     for k, j in enumerate(data):  # 填充数据
                         lines[row_num][col + k - 1] = process_content(j)
 
             writer = csv_writer(open(self.path, 'w', encoding=self.encoding, newline=''), delimiter=self.delimiter,
                                 quotechar=self.quote_char)
             writer.writerows(lines)
 
@@ -488,16 +493,18 @@
 
     row, col = get_usable_coord(data[0], max_row, ws)
     now_data = (data[1],) if not isinstance(data[1][0], (list, tuple, dict)) else data[1]
 
     if head:  # 自动匹配表头
         for r, i in enumerate(now_data, row):
             if isinstance(i, dict):
-                i = [i.get(h, None) for h in head]
-                col = 1
+                for k, h in enumerate(head, 1):
+                    if h in i:
+                        ws.cell(r, k).value = process_content(i[h], True)
+                continue
 
             for key, j in enumerate(i):
                 ws.cell(r, col + key).value = process_content(j, True)
 
     else:
         for r, i in enumerate(now_data, row):
             if isinstance(i, dict):
```

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/filler.pyi` & `DrissionRecorder-3.4.14/DrissionRecorder/filler.pyi`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/recorder.py` & `DrissionRecorder-3.4.14/DrissionRecorder/recorder.py`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/recorder.pyi` & `DrissionRecorder-3.4.14/DrissionRecorder/recorder.pyi`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/setter.py` & `DrissionRecorder-3.4.14/DrissionRecorder/setter.py`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/setter.pyI` & `DrissionRecorder-3.4.14/DrissionRecorder/setter.pyI`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/style/cell_style.py` & `DrissionRecorder-3.4.14/DrissionRecorder/style/cell_style.py`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/tools.py` & `DrissionRecorder-3.4.14/DrissionRecorder/tools.py`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder/tools.pyi` & `DrissionRecorder-3.4.14/DrissionRecorder/tools.pyi`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder.egg-info/PKG-INFO` & `DrissionRecorder-3.4.14/DrissionRecorder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DrissionRecorder
-Version: 3.4.13
+Version: 3.4.14
 Summary: 用于记录数据的模块。
 Home-page: https://gitee.com/g1879/DrissionRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DrissionRecorder
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DrissionRecorder-3.4.13/DrissionRecorder.egg-info/SOURCES.txt` & `DrissionRecorder-3.4.14/DrissionRecorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/LICENSE` & `DrissionRecorder-3.4.14/LICENSE`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/PKG-INFO` & `DrissionRecorder-3.4.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DrissionRecorder
-Version: 3.4.13
+Version: 3.4.14
 Summary: 用于记录数据的模块。
 Home-page: https://gitee.com/g1879/DrissionRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DrissionRecorder
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DrissionRecorder-3.4.13/README.md` & `DrissionRecorder-3.4.14/README.md`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.13/setup.py` & `DrissionRecorder-3.4.14/setup.py`

 * *Files identical despite different names*

