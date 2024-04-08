# Comparing `tmp/SQLDataModel-0.3.4.tar.gz` & `tmp/SQLDataModel-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLDataModel-0.3.4.tar", last modified: Fri Apr  5 20:08:36 2024, max compression
+gzip compressed data, was "SQLDataModel-0.3.5.tar", last modified: Mon Apr  8 16:56:06 2024, max compression
```

## Comparing `SQLDataModel-0.3.4.tar` & `SQLDataModel-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 20:08:36.399945 SQLDataModel-0.3.4/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.4/LICENSE
--rw-rw-rw-   0        0        0    27185 2024-04-05 20:08:36.391336 SQLDataModel-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.4/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 20:08:36.400946 SQLDataModel-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     2312 2024-04-05 20:07:12.000000 SQLDataModel-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:08:34.140985 SQLDataModel-0.3.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:08:35.503520 SQLDataModel-0.3.4/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.4/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.4/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.4/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   555539 2024-04-05 20:06:19.000000 SQLDataModel-0.3.4/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.4/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.4/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.4/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.4/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.4/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:08:36.304262 SQLDataModel-0.3.4/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.4/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.4/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-04-05 20:08:36.384334 SQLDataModel-0.3.4/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    27185 2024-04-05 20:08:33.000000 SQLDataModel-0.3.4/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-05 20:08:34.000000 SQLDataModel-0.3.4/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:08:33.000000 SQLDataModel-0.3.4/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 20:08:33.000000 SQLDataModel-0.3.4/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 20:08:36.320693 SQLDataModel-0.3.4/tests/
--rw-rw-rw-   0        0        0    48008 2024-04-05 19:51:59.000000 SQLDataModel-0.3.4/tests/test_Future.py
--rw-rw-rw-   0        0        0    48011 2024-04-05 19:52:16.000000 SQLDataModel-0.3.4/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:56:06.623130 SQLDataModel-0.3.5/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0    27185 2024-04-08 16:56:06.617119 SQLDataModel-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 16:56:06.624129 SQLDataModel-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2024-04-08 16:55:01.000000 SQLDataModel-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:56:05.278306 SQLDataModel-0.3.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:56:06.445195 SQLDataModel-0.3.5/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.5/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.5/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.5/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   558125 2024-04-08 16:25:58.000000 SQLDataModel-0.3.5/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.5/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.5/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.5/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.5/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.5/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:56:06.562421 SQLDataModel-0.3.5/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.5/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.5/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-04-08 16:56:06.612801 SQLDataModel-0.3.5/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    27185 2024-04-08 16:56:04.000000 SQLDataModel-0.3.5/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-08 16:56:05.000000 SQLDataModel-0.3.5/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:56:05.000000 SQLDataModel-0.3.5/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-08 16:56:05.000000 SQLDataModel-0.3.5/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 16:56:06.573421 SQLDataModel-0.3.5/tests/
+-rw-rw-rw-   0        0        0    48353 2024-04-08 16:22:48.000000 SQLDataModel-0.3.5/tests/test_Future.py
+-rw-rw-rw-   0        0        0    48356 2024-04-08 16:22:46.000000 SQLDataModel-0.3.5/tests/test_SQLDataModel.py
```

### Comparing `SQLDataModel-0.3.4/LICENSE` & `SQLDataModel-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.4/PKG-INFO` & `SQLDataModel-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.4
+Version: 0.3.5
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.4/README.md` & `SQLDataModel-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.4/setup.py` & `SQLDataModel-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.3.4',
+     version='0.3.5',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords='SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package',
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `SQLDataModel-0.3.4/src/SQLDataModel/ANSIColor.py` & `SQLDataModel-0.3.5/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.4/src/SQLDataModel/HTMLParser.py` & `SQLDataModel-0.3.5/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.4/src/SQLDataModel/JSONEncoder.py` & `SQLDataModel-0.3.5/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.4/src/SQLDataModel/SQLDataModel.py` & `SQLDataModel-0.3.5/src/SQLDataModel/SQLDataModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,15 @@
             │ Gerald │   30 │ M    │
             └────────┴──────┴──────┘
             [3 rows x 3 columns]
         ```
 
         Note:
             - If ``data`` is not provided, an empty model is created with headers, at least one of ``data``, ``headers`` or ``dtypes`` are required to instantiate the model.
-            - If ``headers`` are not provided, default headers will be generated using the the format `'col_0', ..., col_N` where N is the column count.
+            - If ``headers`` are not provided, default headers will be generated using the the format ``'0', '1', ..., N`` where ``N`` is the column count.
             - If ``dtypes`` is provided, it must be a dictionary with column names as keys and Python data types as string values, e.g., `{'first_name': 'str', 'weight': 'float'}`
             - If ``infer_types = True`` and ``dtypes`` are provided, the order will be resolved by first inferring the types, then overriding the inferred types for each ``{col:type}`` provided in the ``dtypes`` argument. If one is not provided, then the inferred type will be used as a fallback.
         """
         if data is None:
             if headers is None:
                 if dtypes is None:
                     raise ValueError(
@@ -377,15 +377,15 @@
                         ) from None
             for col in headers:
                 if "'" in col:
                     raise ValueError(
                         SQLDataModel.ErrorFormat(f"ValueError: invalid character in column '{col}', headers must be of type 'str' consisting of valid SQL column identifiers")
                     )
         else:
-            headers = list(dtypes.keys()) if dtypes is not None else [f"col_{x}" for x in range(len(data[0]))]
+            headers = list(dtypes.keys()) if dtypes is not None else [f"{x}" for x in range(len(data[0]))]
         self.sql_idx = "idx"
         """``str``: The index column name applied to the sqlite3 in-memory representation of the model. Default is ``'idx'``"""
         self.sql_model = "sdm"
         """``str``: The table name applied to the sqlite3 in-memory representation of the model. Default is ``'sdm'``"""
         self.display_max_rows = display_max_rows
         """``int``: The maximum number of rows to display. Default is 1,000 rows."""
         self.min_column_width = min_column_width
@@ -420,15 +420,15 @@
             headers_to_py_dtypes_dict = {self.headers[i]:type(data[0][i+dyn_idx_offset]).__name__ for i in range(self.column_count)}        
         if dtypes is not None:
             [(headers_to_py_dtypes_dict.__setitem__(col,dtype)) for col,dtype in dtypes.items() if col in self.headers and dtype in self.static_py_to_sql_map_dict]
         try:
             headers_with_sql_dtypes_str = ",".join(f'"{col}" {self.static_py_to_sql_map_dict[headers_to_py_dtypes_dict[col]]}' for col in self.headers)
         except KeyError as e:
             raise TypeError(
-                SQLDataModel.ErrorFormat(f"TypeError: invalid data type {e}, values in ``data`` must be a list of lists comprised of types 'str', 'int', 'float', 'bytes', 'datetime' or 'bool' ")
+                SQLDataModel.ErrorFormat(f"TypeError: invalid data type {e}, values in `data` must be a list of lists comprised of types 'str', 'int', 'float', 'bytes', 'datetime' or 'bool' ")
             ) from None
         sql_create_stmt = f"""create table if not exists "{self.sql_model}" ("{self.sql_idx}" INTEGER PRIMARY KEY,{headers_with_sql_dtypes_str})"""
         sql_insert_params = ",".join([SQLDataModel.sqlite_cast_type_format(dtype=headers_to_py_dtypes_dict[col], as_binding=True) for col in self.headers])        
         sql_insert_stmt = f"""insert into "{self.sql_model}" ({dyn_add_idx_insert}{','.join([f'"{col}"' for col in self.headers])}) values ({dyn_idx_bind}{sql_insert_params})"""
         self.sql_db_conn = sqlite3.connect(":memory:", uri=True, detect_types=sqlite3.PARSE_DECLTYPES)
         """``sqlite3.Connection``: The in-memory sqlite3 connection object in use by the model."""
         try:
@@ -2608,15 +2608,15 @@
             if not isinstance(data[0], dict):
                 raise TypeError(
                     SQLDataModel.ErrorFormat(f"TypeError: invalid type in list '{type(data[0].__name__)}', if ``data`` is of type 'list' its items must be of type 'dict' to use the `from_dict()` method")
                 )
             return cls.from_json(data)
         rowwise = True if all(isinstance(x, int) for x in data.keys()) else False
         if rowwise:
-            headers = ['idx',*[f'col_{i}' for i in range(len(data[next(iter(data))]))]] # get column count from first key value pair in provided dict
+            headers = ['idx',*[f'{i}' for i in range(len(data[next(iter(data))]))]] # get column count from first key value pair in provided dict
             return cls([tuple([k,*v]) for k,v in data.items()], headers, **kwargs)
         else:
             first_key_val = data[next(iter(data))]
             if isinstance(first_key_val, dict):
                 headers = list(data.keys())
                 data = [[data[col][val] for col in headers] for val in data.keys()]
             elif isinstance(first_key_val, (list,tuple)):
@@ -8762,14 +8762,71 @@
         ```    
         Note:
             - See related :meth:`SQLDataModel.head()` for the opposite, grabbing the top ``n_rows`` from the current model.
 
         """
         return self.execute_fetch(self._generate_unordered_sql_stmt(n_rows, ordering="desc"))
   
+    def transpose(self, infer_types:bool=True, include_headers:bool=False) -> SQLDataModel:
+        """
+        Transposes the model and returns as a new ``SQLDataModel``.
+
+        Parameters:
+            ``infer_types`` (bool, optional): If types should be inferred after the transposition. Defaults to True.
+            ``include_headers`` (bool, optional): If headers are included in the transposed data. Defaults to False.
+
+        Returns:
+            ``SQLDataModel``: The transposition of the model as a new SQLDataModel instance.
+
+        Example::
+
+            from SQLDataModel import SQLDataModel
+
+            # Create the model
+            sdm = SQLDataModel([('A1', 'A2'), ('B1', 'B2'), ('C1', 'C2')])
+
+            # Transpose it
+            sdm_transposed = sdm.transpose()
+
+            # View original
+            print(f"Original:\\n{sdm}")
+
+            # Along with transposed
+            print(f"Transposed:\\n{sdm_transposed}")
+
+        This will output the result of the transposition:
+
+        ```shell
+            Original:
+            ┌───┬─────┬─────┐
+            │   │ 0   │ 1   │
+            ├───┼─────┼─────┤
+            │ 0 │ A1  │ A2  │
+            │ 1 │ B1  │ B2  │
+            │ 2 │ C1  │ C2  │
+            └───┴─────┴─────┘
+            [3 rows x 2 columns]
+            
+            Transposed:
+            ┌───┬─────┬─────┬─────┐
+            │   │ 0   │ 1   │ 2   │
+            ├───┼─────┼─────┼─────┤
+            │ 0 │ A1  │ B1  │ C1  │
+            │ 1 │ A2  │ B2  │ C2  │
+            └───┴─────┴─────┴─────┘
+            [2 rows x 3 columns]            
+        ```
+
+        Note:
+            - When ``infer_types=False``, the first row of the transposed result will be used to set the ``dtypes`` of the new model. This is generally a poor choice considering the nature of transposing data.
+            - If ``include_headers=True``, the headers will be included as the first row in the transposed data.
+            - Running this method sequentially should return the original model, ``sdm == sdm.transpose().transpose()``
+        """
+        return type(self)(data=[row for row in zip(*self.data(include_headers=include_headers, index=False))], infer_types=infer_types, **self._get_display_args())
+
     def vstack(self, *other:SQLDataModel, inplace:bool=False) -> SQLDataModel:
         """
         Vertically stacks one or more ``SQLDataModel`` objects to the current model.
 
         Parameters:
             ``other`` (SQLDataModel or sequence of): The SQLDataModel objects to vertically stack.
             ``inplace`` (bool, optional): If True, performs the vertical stacking in-place, modifying the current model. Defaults to False, returning a new ``SQLDataModel``.
```

### Comparing `SQLDataModel-0.3.4/src/SQLDataModel/StandardDeviation.py` & `SQLDataModel-0.3.5/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.4/src/SQLDataModel/converters.py` & `SQLDataModel-0.3.5/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.4/src/SQLDataModel/demo.py` & `SQLDataModel-0.3.5/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.4/src/SQLDataModel/exceptions.py` & `SQLDataModel-0.3.5/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.4/src/SQLDataModel/extensions/str_utils.c` & `SQLDataModel-0.3.5/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.4/src/SQLDataModel.egg-info/PKG-INFO` & `SQLDataModel-0.3.5/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.4
+Version: 0.3.5
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.4/src/SQLDataModel.egg-info/SOURCES.txt` & `SQLDataModel-0.3.5/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.4/tests/test_Future.py` & `SQLDataModel-0.3.5/tests/test_Future.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,17 @@
     """Tests the `__setitem__()` method by using all possible type combinations `row, column` indexing and confirms the expected output."""
     grid_size = 10 # creates grid as (grid_size x grid_size)
     sdm = SQLDataModel([[f"F" for _ in range(grid_size)] for _ in range(grid_size)]) # create the grid canvas
     fill_char = 'X' # values to fill interior with
     test_corners = [('top left', 'top right'),('bottom left', 'bottom right')] # corner values
     test_indicies_and_values = [
         [(0), tuple([f'0,{i}' for i in range(sdm.column_count)])] # rowwise updates
-        ,['col_0', [(f'{i},0',) for i in range(sdm.row_count)]] # columnwise updates
+        ,['0', [(f'{i},0',) for i in range(sdm.row_count)]] # columnwise updates
         ,[(grid_size), tuple([f'{grid_size},{i}' for i in range(sdm.column_count)])] # new row
-        ,[f'col_{grid_size}', [(f'{i},{grid_size}',) for i in range(sdm.row_count + 1)]] # new column
+        ,[f'{grid_size}', [(f'{i},{grid_size}',) for i in range(sdm.row_count + 1)]] # new column
         ,[(slice(1,-1),slice(1,-1)), [tuple([fill_char for _ in range(sdm.column_count-1)]) for _ in range(sdm.row_count-1)]] # new interior values
         ,[(0,0), test_corners[0][0]] # top left
         ,[(0,-1), test_corners[0][-1]] # top right
         ,[(-1,0), test_corners[-1][0]] # bottom left
         ,[(-1,-1),test_corners[-1][-1]] # bottom right
     ]
     for t_pair in test_indicies_and_values:
@@ -761,8 +761,15 @@
     sdm_0['bytes'] = b'pad test'
     single_stack_test = sdm_0.vstack(sdm_1, inplace=False)
     output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
     data_0 = [tuple([*row, b'pad test']) for row in data_0]
     data_1 = [tuple([*row, None]) for row in data_1]
     expected_data, expected_headers = data_0 + data_1, [*headers_0, 'bytes']
     assert output_headers == expected_headers
-    assert output_data == expected_data    
+    assert output_data == expected_data    
+
+@pytest.mark.core
+def test_transpose():
+    num_rows, num_cols = 10, 5
+    input_data = [tuple(f"{i},{j}" for j in range(num_cols)) for i in range(num_rows)]
+    output_data = SQLDataModel(input_data).transpose(infer_types=True,include_headers=False).transpose(infer_types=True,include_headers=False).data()
+    assert output_data == input_data
```

### Comparing `SQLDataModel-0.3.4/tests/test_SQLDataModel.py` & `SQLDataModel-0.3.5/tests/test_SQLDataModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,17 +51,17 @@
     """Tests the `__setitem__()` method by using all possible type combinations `row, column` indexing and confirms the expected output."""
     grid_size = 10 # creates grid as (grid_size x grid_size)
     sdm = SQLDataModel([[f"F" for _ in range(grid_size)] for _ in range(grid_size)]) # create the grid canvas
     fill_char = 'X' # values to fill interior with
     test_corners = [('top left', 'top right'),('bottom left', 'bottom right')] # corner values
     test_indicies_and_values = [
         [(0), tuple([f'0,{i}' for i in range(sdm.column_count)])] # rowwise updates
-        ,['col_0', [(f'{i},0',) for i in range(sdm.row_count)]] # columnwise updates
+        ,['0', [(f'{i},0',) for i in range(sdm.row_count)]] # columnwise updates
         ,[(grid_size), tuple([f'{grid_size},{i}' for i in range(sdm.column_count)])] # new row
-        ,[f'col_{grid_size}', [(f'{i},{grid_size}',) for i in range(sdm.row_count + 1)]] # new column
+        ,[f'{grid_size}', [(f'{i},{grid_size}',) for i in range(sdm.row_count + 1)]] # new column
         ,[(slice(1,-1),slice(1,-1)), [tuple([fill_char for _ in range(sdm.column_count-1)]) for _ in range(sdm.row_count-1)]] # new interior values
         ,[(0,0), test_corners[0][0]] # top left
         ,[(0,-1), test_corners[0][-1]] # top right
         ,[(-1,0), test_corners[-1][0]] # bottom left
         ,[(-1,-1),test_corners[-1][-1]] # bottom right
     ]
     for t_pair in test_indicies_and_values:
@@ -761,8 +761,15 @@
     sdm_0['bytes'] = b'pad test'
     single_stack_test = sdm_0.vstack(sdm_1, inplace=False)
     output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
     data_0 = [tuple([*row, b'pad test']) for row in data_0]
     data_1 = [tuple([*row, None]) for row in data_1]
     expected_data, expected_headers = data_0 + data_1, [*headers_0, 'bytes']
     assert output_headers == expected_headers
-    assert output_data == expected_data    
+    assert output_data == expected_data    
+
+@pytest.mark.core
+def test_transpose():
+    num_rows, num_cols = 10, 5
+    input_data = [tuple(f"{i},{j}" for j in range(num_cols)) for i in range(num_rows)]
+    output_data = SQLDataModel(input_data).transpose(infer_types=True,include_headers=False).transpose(infer_types=True,include_headers=False).data()
+    assert output_data == input_data
```

