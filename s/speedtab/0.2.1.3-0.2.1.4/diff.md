# Comparing `tmp/speedtab-0.2.1.3.tar.gz` & `tmp/speedtab-0.2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.2.1.3.tar", max compression
+gzip compressed data, was "speedtab-0.2.1.4.tar", max compression
```

## Comparing `speedtab-0.2.1.3.tar` & `speedtab-0.2.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2024-04-02 08:12:57.396526 speedtab-0.2.1.3/pyproject.toml
--rw-r--r--   0        0        0      382 2023-12-14 09:13:27.273500 speedtab-0.2.1.3/speedtab/__init__.py
--rw-r--r--   0        0        0    87055 2024-04-02 08:12:53.930932 speedtab-0.2.1.3/speedtab/client.py
--rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.1.3/speedtab/enums.py
--rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.1.3/speedtab/formats.py
--rw-r--r--   0        0        0      783 2024-04-02 08:13:03.600459 speedtab-0.2.1.3/setup.py
--rw-r--r--   0        0        0      808 2024-04-02 08:13:03.600459 speedtab-0.2.1.3/PKG-INFO
+-rw-r--r--   0        0        0      567 2024-04-08 13:10:37.767226 speedtab-0.2.1.4/pyproject.toml
+-rw-r--r--   0        0        0      382 2023-12-14 09:13:27.273500 speedtab-0.2.1.4/speedtab/__init__.py
+-rw-r--r--   0        0        0    87177 2024-04-08 13:13:51.329242 speedtab-0.2.1.4/speedtab/client.py
+-rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.1.4/speedtab/enums.py
+-rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.1.4/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2024-04-08 13:14:08.165881 speedtab-0.2.1.4/setup.py
+-rw-r--r--   0        0        0      808 2024-04-08 13:14:08.165881 speedtab-0.2.1.4/PKG-INFO
```

### Comparing `speedtab-0.2.1.3/pyproject.toml` & `speedtab-0.2.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.2.1.3"
+version = "0.2.1.4"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.2.1.3/speedtab/client.py` & `speedtab-0.2.1.4/speedtab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,21 +458,22 @@
 
 
 class Range:
     """A representation of a selected range in a Sheet. This class contains numerous methods for interaction with a sheet
     from formatting cells and inputting values to adding charts and changing cells' sizes.
     """
 
-    def __init__(self, sheet_id, _task_queue, work_zone, start_data_cell, base, data_cell):
+    def __init__(self, sheet_id, _task_queue, work_zone, start_data_cell, base, data_cell, data_cell_full):
         self.sheet_id = sheet_id
         self._task_queue = _task_queue
         self.work_zone = work_zone
         self.start_data_cell = start_data_cell
         self.base = base
         self.data_cell = data_cell
+        self.data_cell_full = data_cell_full
 
     def _increment_task(self):
         return len(self._task_queue)
 
     def add_chart(self,
                   columns,
                   target_axis: Union[AxisPosition, list] = AxisPosition.LEFT_AXIS,
@@ -1061,16 +1062,15 @@
         actual values set formatted_values to False.
 
         :param formated_values: Whether to save the formatting as in the column, defaults to True.
         :return: A list of lists containing the values from the sheet.
         """
         return (self.base.connect_v4.spreadsheets().values()
                 .get(spreadsheetId=self.base.spreadsheet_id,
-                     range=self.data_cell,
-                     # range='December!B1:1000',
+                     range=self.data_cell_full,
                      valueRenderOption='FORMATTED_VALUE' if formated_values else 'UNFORMATTED_VALUE').execute()
                 .get('values', []))
 
     def reset_size(self):
         """Resets the size of a cell.
 
         :return: A Spreadsheet object.
@@ -1388,21 +1388,22 @@
         self.sheet_name = sheet_name
         self.sheet_id = sheet_id
         self._task_queue = task_query
         self.sheets = sheets
         cells = parse_range(cells)
 
         self.start_data_cell = f'{sheet_name}!{col_num_to_string(cells[1])}{num_to_string(cells[0])}'
-        self.data_cell = self.start_data_cell + f':{col_num_to_string(cells[3])}{num_to_string(cells[2]) if cells[2] is not None else self.sheets.get(self.sheet_name).get("max_row")}'
+        self.data_cell = self.start_data_cell + f':{col_num_to_string(cells[3])}{num_to_string(cells[2]) if cells[2] is not None else ""}'
+        self.data_cell_full = self.data_cell + f'{self.sheets.get(self.sheet_name).get("max_row") if cells[2] is None else ""}'
         self.work_zone = dict([(key, val + SHIFT_DIM.get(key) if val is not None else val)
                                for key, val in zip(SHIFT_DIM.keys(), cells)]
                               + [('sheetId', self.sheet_id)])
 
         super().__init__(self.sheet_id, self._task_queue, self.work_zone, self.start_data_cell, self.base,
-                         self.data_cell)
+                         self.data_cell, self.data_cell_full)
 
     def cell_range(self, input_range):
         """Selects a cell range for an interaction.
 
         :param input_range: Either a string with Excel range (e.g. 'A1:B3'), or a tuple in a form
         (row_start, column_start, row_end, column_end). In the latter case 'A1:B3' can be implemented as (0, 0, 2, 1).
         :return: A Sheet object with a selected range.
```

### Comparing `speedtab-0.2.1.3/speedtab/enums.py` & `speedtab-0.2.1.4/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.3/speedtab/formats.py` & `speedtab-0.2.1.4/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.3/setup.py` & `speedtab-0.2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.2.1.3',
+    'version': '0.2.1.4',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.2.1.3/PKG-INFO` & `speedtab-0.2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.2.1.3
+Version: 0.2.1.4
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

