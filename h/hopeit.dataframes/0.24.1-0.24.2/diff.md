# Comparing `tmp/hopeit.dataframes-0.24.1.tar.gz` & `tmp/hopeit.dataframes-0.24.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopeit.dataframes-0.24.1.tar", last modified: Wed Mar 20 22:14:01 2024, max compression
+gzip compressed data, was "hopeit.dataframes-0.24.2.tar", last modified: Mon Apr  8 14:34:04 2024, max compression
```

## Comparing `hopeit.dataframes-0.24.1.tar` & `hopeit.dataframes-0.24.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:14:01.577205 hopeit.dataframes-0.24.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-20 22:14:01.577205 hopeit.dataframes-0.24.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 22:14:01.577205 hopeit.dataframes-0.24.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:14:01.573205 hopeit.dataframes-0.24.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:14:01.573205 hopeit.dataframes-0.24.1/src/hopeit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:14:01.577205 hopeit.dataframes-0.24.1/src/hopeit/dataframes/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/src/hopeit/dataframes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/src/hopeit/dataframes/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/src/hopeit/dataframes/dataframeobject.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/src/hopeit/dataframes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:14:01.577205 hopeit.dataframes-0.24.1/src/hopeit/dataframes/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/src/hopeit/dataframes/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/src/hopeit/dataframes/serialization/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/src/hopeit/dataframes/serialization/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/src/hopeit/dataframes/serialization/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:14:01.577205 hopeit.dataframes-0.24.1/src/hopeit/dataframes/setup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/src/hopeit/dataframes/setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-20 22:06:29.000000 hopeit.dataframes-0.24.1/src/hopeit/dataframes/setup/dataframes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:14:01.577205 hopeit.dataframes-0.24.1/src/hopeit.dataframes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-20 22:14:01.000000 hopeit.dataframes-0.24.1/src/hopeit.dataframes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-20 22:14:01.000000 hopeit.dataframes-0.24.1/src/hopeit.dataframes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 22:14:01.000000 hopeit.dataframes-0.24.1/src/hopeit.dataframes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-20 22:14:01.000000 hopeit.dataframes-0.24.1/src/hopeit.dataframes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-20 22:14:01.000000 hopeit.dataframes-0.24.1/src/hopeit.dataframes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:34:04.715750 hopeit.dataframes-0.24.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-08 14:34:04.711750 hopeit.dataframes-0.24.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:34:04.715750 hopeit.dataframes-0.24.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:34:04.707750 hopeit.dataframes-0.24.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:34:04.707750 hopeit.dataframes-0.24.2/src/hopeit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:34:04.711750 hopeit.dataframes-0.24.2/src/hopeit/dataframes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/src/hopeit/dataframes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/src/hopeit/dataframes/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/src/hopeit/dataframes/dataframeobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/src/hopeit/dataframes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:34:04.711750 hopeit.dataframes-0.24.2/src/hopeit/dataframes/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/src/hopeit/dataframes/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/src/hopeit/dataframes/serialization/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/src/hopeit/dataframes/serialization/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/src/hopeit/dataframes/serialization/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:34:04.711750 hopeit.dataframes-0.24.2/src/hopeit/dataframes/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/src/hopeit/dataframes/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-08 14:26:28.000000 hopeit.dataframes-0.24.2/src/hopeit/dataframes/setup/dataframes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:34:04.711750 hopeit.dataframes-0.24.2/src/hopeit.dataframes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-08 14:34:04.000000 hopeit.dataframes-0.24.2/src/hopeit.dataframes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-08 14:34:04.000000 hopeit.dataframes-0.24.2/src/hopeit.dataframes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:34:04.000000 hopeit.dataframes-0.24.2/src/hopeit.dataframes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-08 14:34:04.000000 hopeit.dataframes-0.24.2/src/hopeit.dataframes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 14:34:04.000000 hopeit.dataframes-0.24.2/src/hopeit.dataframes.egg-info/top_level.txt
```

### Comparing `hopeit.dataframes-0.24.1/PKG-INFO` & `hopeit.dataframes-0.24.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.dataframes
-Version: 0.24.1
+Version: 0.24.2
 Summary: Hopeit Engine Dataframes Toolkit
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
@@ -22,15 +22,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: hopeit.engine[fs-storage]==0.24.1
+Requires-Dist: hopeit.engine[fs-storage]==0.24.2
 Requires-Dist: pandas
 Requires-Dist: numpy
 Provides-Extra: pyarrow
 Requires-Dist: pyarrow; extra == "pyarrow"
 
 # hopeit.engine dataframes plugin
```

### Comparing `hopeit.dataframes-0.24.1/README.md` & `hopeit.dataframes-0.24.2/README.md`

 * *Files identical despite different names*

### Comparing `hopeit.dataframes-0.24.1/setup.py` & `hopeit.dataframes-0.24.2/setup.py`

 * *Files identical despite different names*

### Comparing `hopeit.dataframes-0.24.1/src/hopeit/dataframes/__init__.py` & `hopeit.dataframes-0.24.2/src/hopeit/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `hopeit.dataframes-0.24.1/src/hopeit/dataframes/dataframe.py` & `hopeit.dataframes-0.24.2/src/hopeit/dataframes/dataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,17 +77,18 @@
         self.__df = pd.DataFrame()
         raise NotImplementedError  # must use @dataframe decorator  # pragma: no cover
 
     @staticmethod
     def __init_from_series__(
         self, **series: pd.Series
     ):  # pylint: disable=bad-staticmethod-argument
-        if self.__data_object__["validate"]:
-            series = self._coerce_datatypes(series)
         df = pd.DataFrame(series)
+        df.index.name = None  # Removes index name to avoid colisions with series name
+        if self.__data_object__["validate"]:
+            df = pd.DataFrame(self._coerce_datatypes(df))
         setattr(self, "__df", df[self.__dataframe__.columns])
 
     @classmethod
     def _from_df(cls, df: pd.DataFrame, **series: Any) -> DataFrameT:
         df = df if cls.__data_object__["unsafe"] else pd.DataFrame(df)
         obj = cls(**{**df._series, **series})  # pylint: disable=protected-access
         return obj  # type: ignore
@@ -167,17 +168,17 @@
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name in self.__dataframe__.columns:
             self.__df[name] = value
         else:
             object.__setattr__(self, name, value)
 
-    def _coerce_datatypes(self, series: Dict[str, pd.Series]) -> Dict[str, pd.Series]:
+    def _coerce_datatypes(self, df: pd.DataFrame) -> Dict[str, pd.Series]:
         return {
-            name: self.DATATYPE_MAPPING[field.type](series[name])  # type: ignore
+            name: self.DATATYPE_MAPPING[field.type](df[name])  # type: ignore
             for name, field in self.__dataframe__.fields.items()
         }
 
 
 def dataframe(
     decorated_class=None,
     unsafe: bool = False,
```

### Comparing `hopeit.dataframes-0.24.1/src/hopeit/dataframes/dataframeobject.py` & `hopeit.dataframes-0.24.2/src/hopeit/dataframes/dataframeobject.py`

 * *Files identical despite different names*

### Comparing `hopeit.dataframes-0.24.1/src/hopeit/dataframes/serialization/dataset.py` & `hopeit.dataframes-0.24.2/src/hopeit/dataframes/serialization/dataset.py`

 * *Files identical despite different names*

### Comparing `hopeit.dataframes-0.24.1/src/hopeit/dataframes/serialization/files.py` & `hopeit.dataframes-0.24.2/src/hopeit/dataframes/serialization/files.py`

 * *Files identical despite different names*

### Comparing `hopeit.dataframes-0.24.1/src/hopeit/dataframes/setup/dataframes.py` & `hopeit.dataframes-0.24.2/src/hopeit/dataframes/setup/dataframes.py`

 * *Files identical despite different names*

### Comparing `hopeit.dataframes-0.24.1/src/hopeit.dataframes.egg-info/PKG-INFO` & `hopeit.dataframes-0.24.2/src/hopeit.dataframes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.dataframes
-Version: 0.24.1
+Version: 0.24.2
 Summary: Hopeit Engine Dataframes Toolkit
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
@@ -22,15 +22,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: hopeit.engine[fs-storage]==0.24.1
+Requires-Dist: hopeit.engine[fs-storage]==0.24.2
 Requires-Dist: pandas
 Requires-Dist: numpy
 Provides-Extra: pyarrow
 Requires-Dist: pyarrow; extra == "pyarrow"
 
 # hopeit.engine dataframes plugin
```

### Comparing `hopeit.dataframes-0.24.1/src/hopeit.dataframes.egg-info/SOURCES.txt` & `hopeit.dataframes-0.24.2/src/hopeit.dataframes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

