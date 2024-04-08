# Comparing `tmp/python_odisi-0.3.0.tar.gz` & `tmp/python_odisi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_odisi-0.3.0.tar", max compression
+gzip compressed data, was "python_odisi-0.4.0.tar", max compression
```

## Comparing `python_odisi-0.3.0.tar` & `python_odisi-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1079 2023-12-05 16:25:50.713442 python_odisi-0.3.0/LICENSE
--rw-r--r--   0        0        0     3393 2023-12-06 16:46:57.209454 python_odisi-0.3.0/README.md
--rw-r--r--   0        0        0       70 2023-11-28 18:27:53.276395 python_odisi-0.3.0/odisi/__init__.py
--rw-r--r--   0        0        0    11037 2023-12-06 16:36:18.843669 python_odisi-0.3.0/odisi/odisi.py
--rw-r--r--   0        0        0     5067 2023-12-05 17:00:16.089271 python_odisi-0.3.0/odisi/reader.py
--rw-r--r--   0        0        0      151 2023-12-04 13:25:09.093084 python_odisi-0.3.0/odisi/utils.py
--rw-r--r--   0        0        0      766 2023-12-06 16:46:34.973670 python_odisi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 python_odisi-0.3.0/setup.py
--rw-r--r--   0        0        0     4111 1970-01-01 00:00:00.000000 python_odisi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-12-05 16:25:50.713442 python_odisi-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3590 2023-12-06 16:51:01.143081 python_odisi-0.4.0/README.md
+-rw-r--r--   0        0        0       70 2023-11-28 18:27:53.276395 python_odisi-0.4.0/odisi/__init__.py
+-rw-r--r--   0        0        0    11310 2024-04-08 10:19:31.366965 python_odisi-0.4.0/odisi/odisi.py
+-rw-r--r--   0        0        0     5067 2023-12-08 14:49:50.707736 python_odisi-0.4.0/odisi/reader.py
+-rw-r--r--   0        0        0      151 2023-12-04 13:25:09.093084 python_odisi-0.4.0/odisi/utils.py
+-rw-r--r--   0        0        0      766 2024-04-08 11:36:53.207667 python_odisi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4465 1970-01-01 00:00:00.000000 python_odisi-0.4.0/setup.py
+-rw-r--r--   0        0        0     4308 1970-01-01 00:00:00.000000 python_odisi-0.4.0/PKG-INFO
```

### Comparing `python_odisi-0.3.0/LICENSE` & `python_odisi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_odisi-0.3.0/README.md` & `python_odisi-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,22 @@
 import polars as pl
 
 load = pl.read_csv("load_data.csv")
 # Assume that the timestamp is in the column 'time'
 d.interpolate(load.select(pl.col("time")), clip=True)
 ```
 
+### Export segment data
+
+The data of all segments can be exported to individual csv-files with the following code:
+
+```python
+d.export_segments_csv(prefix="my_experiment", path="data_folder")
+```
+
 ## Tests
 
 The package includes a test suite which should be run with pytest:
 
 ```bash
 poetry run pytest
 ```
```

### Comparing `python_odisi-0.3.0/odisi/odisi.py` & `python_odisi-0.4.0/odisi/odisi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import pdb
+from datetime import timedelta
 
 import numpy as np
 import polars as pl
 from numpy.typing import NDArray
 
 from odisi.utils import timedelta_sec
 
 
 class OdisiResult:
-
     """Contains the data from the experiment.
 
     Attributes
     ----------
     data : obj:`DataFrame`
         A dataframe with the data of the experiment.
     x : ArrayLike
@@ -68,16 +67,27 @@
     def gages(self) -> list[str]:
         return list(self._gages.keys())
 
     @property
     def segments(self) -> list[str]:
         return list(self._segments.keys())
 
+    def shift_time(self, t: timedelta):
+        """Shift the datetime information by `t`.
+
+        Parameters
+        ----------
+        t : timedelta
+            Time shifted.
+
+        """
+        self._data = self._data.with_columns(pl.col("time") + t)
+
     def gage(self, label: str, with_time: bool = False) -> pl.DataFrame:
-        """Get data corresponding to the given gauge.
+        """Get data corresponding to the given gage.
 
         Parameters
         ----------
         label : str
             The label of the gage.
         with_time : bool
             Whether a column with the time should also be returned in the dataframe.
@@ -328,15 +338,14 @@
             di, xi = self.segment(si, with_time=with_time)
             di.write_csv(f"{path}/{prefix}_{si}_data.csv")
             df_x = pl.DataFrame({"x": xi})
             df_x.write_csv(f"{path}/{prefix}_{si}_x.csv")
 
 
 class OdisiGagesResult(OdisiResult):
-
     """Docstring ."""
 
     def __init__(
         self,
         data,
         x,
         gages: dict[str, int],
```

### Comparing `python_odisi-0.3.0/odisi/reader.py` & `python_odisi-0.4.0/odisi/reader.py`

 * *Files identical despite different names*

### Comparing `python_odisi-0.3.0/pyproject.toml` & `python_odisi-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-odisi"
-version = "0.3.0"
+version = "0.4.0"
 description = "Import and post-process data generated by the Luna ODiSI System"
 authors = ["Cristóbal Tapia Camú <crtapia@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/cristobaltapia/python-odisi"
 repository = "https://github.com/cristobaltapia/python-odisi"
 packages = [{ include = "odisi" }]
 license = "MIT"
```

### Comparing `python_odisi-0.3.0/setup.py` & `python_odisi-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.26.2,<2.0.0', 'polars>=0.19.17,<0.20.0']
 
 setup_kwargs = {
     'name': 'python-odisi',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Import and post-process data generated by the Luna ODiSI System',
-    'long_description': '# Python reader for exported ODiSI data\n\n## Description\n\nThis python package defines a reader and helper methods to handle data exported from the Luna ODiSI 6000 optical measuring system.\nIt allows for an easier retrieval of data corresponding to each segment, as well as the possibility to interpolate the results based on additional measurements, such as experimental load.\nDoing this manually requires some amount of python code, which can be avoided by using this package.\n\n## Installation\n\nInstall as usual:\n\n```bash\npip install python-odisi\n```\n\n## Usage\n\n### Retrieve data from a \\*.tsv file\n\nThe library can be used to read files in the following manner:\n\n```python\nfrom odisi import read_tsv\n\nd = read_tsv("data_gages.tsv")\n\n# List all gages\ngages = d.gages\n# List all segments\nsegments = d.segments\n# Get the data for a specific gage, e.g. with the label \'A\'\nd_gage = d.gage("A")\n# Get the data for a specific segment, e.g. with the label \'Seg-1\'\nd_seg, x_seg = d.segment("Seg-1")\n```\n\n### Interpolation of data\n\nThe package allows to easily interpolate an external signal (e.g. the load during the test).\nFor this, two strategies can be followed:\n\n#### 1. Interpolate the data from the sensors using the timestamps from the external signal\n\n```python\nimport polars as pl\n\nload = pl.read_csv("load_data.csv")\n# Assume that the timestamp is in the column \'time\'\nd.interpolate(load.select(pl.col("time")))\n```\n\nThen you should be able to plot your data against the measured load:\n\n```python\nimport matplotlib.pyplot as plt\n\nd_gage = d.gage("A")\n# Assume that the load data is in column \'load\'\na_load = load.select(pl.col("load")).to_series()\n\nplt.plot(d_gage, a_load)\n```\n\n#### 2. Interpolate the data from the external signal to match the timestamp from the sensor data\n\n```python\nimport polars as pl\n\nload = pl.read_csv("load_data.csv")\n# Assume that the timestamp is in the column \'time\'\nnew_load = d.interpolate_signal(data=load, time="time")\n```\n\nThen you should be able to plot your data against the measured load:\n\n```python\nimport matplotlib.pyplot as plt\n\nd_gage = d.gage("A")\n# Assume that the load data is in column \'load\'\na_load = new_load.select(pl.col("load")).to_series()\n\nplt.plot(d_gage, a_load)\n```\n\nIn both cases it is assumed that the timestamps from both files are synchronized, i.e. that both measuring computers have synchronized clocks.\n\n### Clip data during interpolation\n\nIt is probable that the measurements from both data sources (ODiSI and additional system) were started at different times.\nThis produces some annoyances during the processing of the data due to the mismatch in datapoints.\nTo remedy this, the option `clip=True` can be passed to both interpolation methods (`interpolate(...)` and `interpolate_signal(...)`), which will clip the data to the common time interval between both signals.\n\n```python\nimport polars as pl\n\nload = pl.read_csv("load_data.csv")\n# Assume that the timestamp is in the column \'time\'\nd.interpolate(load.select(pl.col("time")), clip=True)\n```\n\n## Tests\n\nThe package includes a test suite which should be run with pytest:\n\n```bash\npoetry run pytest\n```\n\n## Citation\n\n```bib\n@software{Tapia_2023,\n    author = {Tapia Camú, Cristóbal},\n    title = {{python-odisi: Import data generated by the Luna ODiSI System}},\n    url = {https://github.com/cristobaltapia/python-odisi},\n    version = {v0.3},\n    year = {2023},\n}\n```\n',
+    'long_description': '# Python reader for exported ODiSI data\n\n## Description\n\nThis python package defines a reader and helper methods to handle data exported from the Luna ODiSI 6000 optical measuring system.\nIt allows for an easier retrieval of data corresponding to each segment, as well as the possibility to interpolate the results based on additional measurements, such as experimental load.\nDoing this manually requires some amount of python code, which can be avoided by using this package.\n\n## Installation\n\nInstall as usual:\n\n```bash\npip install python-odisi\n```\n\n## Usage\n\n### Retrieve data from a \\*.tsv file\n\nThe library can be used to read files in the following manner:\n\n```python\nfrom odisi import read_tsv\n\nd = read_tsv("data_gages.tsv")\n\n# List all gages\ngages = d.gages\n# List all segments\nsegments = d.segments\n# Get the data for a specific gage, e.g. with the label \'A\'\nd_gage = d.gage("A")\n# Get the data for a specific segment, e.g. with the label \'Seg-1\'\nd_seg, x_seg = d.segment("Seg-1")\n```\n\n### Interpolation of data\n\nThe package allows to easily interpolate an external signal (e.g. the load during the test).\nFor this, two strategies can be followed:\n\n#### 1. Interpolate the data from the sensors using the timestamps from the external signal\n\n```python\nimport polars as pl\n\nload = pl.read_csv("load_data.csv")\n# Assume that the timestamp is in the column \'time\'\nd.interpolate(load.select(pl.col("time")))\n```\n\nThen you should be able to plot your data against the measured load:\n\n```python\nimport matplotlib.pyplot as plt\n\nd_gage = d.gage("A")\n# Assume that the load data is in column \'load\'\na_load = load.select(pl.col("load")).to_series()\n\nplt.plot(d_gage, a_load)\n```\n\n#### 2. Interpolate the data from the external signal to match the timestamp from the sensor data\n\n```python\nimport polars as pl\n\nload = pl.read_csv("load_data.csv")\n# Assume that the timestamp is in the column \'time\'\nnew_load = d.interpolate_signal(data=load, time="time")\n```\n\nThen you should be able to plot your data against the measured load:\n\n```python\nimport matplotlib.pyplot as plt\n\nd_gage = d.gage("A")\n# Assume that the load data is in column \'load\'\na_load = new_load.select(pl.col("load")).to_series()\n\nplt.plot(d_gage, a_load)\n```\n\nIn both cases it is assumed that the timestamps from both files are synchronized, i.e. that both measuring computers have synchronized clocks.\n\n### Clip data during interpolation\n\nIt is probable that the measurements from both data sources (ODiSI and additional system) were started at different times.\nThis produces some annoyances during the processing of the data due to the mismatch in datapoints.\nTo remedy this, the option `clip=True` can be passed to both interpolation methods (`interpolate(...)` and `interpolate_signal(...)`), which will clip the data to the common time interval between both signals.\n\n```python\nimport polars as pl\n\nload = pl.read_csv("load_data.csv")\n# Assume that the timestamp is in the column \'time\'\nd.interpolate(load.select(pl.col("time")), clip=True)\n```\n\n### Export segment data\n\nThe data of all segments can be exported to individual csv-files with the following code:\n\n```python\nd.export_segments_csv(prefix="my_experiment", path="data_folder")\n```\n\n## Tests\n\nThe package includes a test suite which should be run with pytest:\n\n```bash\npoetry run pytest\n```\n\n## Citation\n\n```bib\n@software{Tapia_2023,\n    author = {Tapia Camú, Cristóbal},\n    title = {{python-odisi: Import data generated by the Luna ODiSI System}},\n    url = {https://github.com/cristobaltapia/python-odisi},\n    version = {v0.3},\n    year = {2023},\n}\n```\n',
     'author': 'Cristóbal Tapia Camú',
     'author_email': 'crtapia@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cristobaltapia/python-odisi',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `python_odisi-0.3.0/PKG-INFO` & `python_odisi-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-odisi
-Version: 0.3.0
+Version: 0.4.0
 Summary: Import and post-process data generated by the Luna ODiSI System
 Home-page: https://github.com/cristobaltapia/python-odisi
 License: MIT
 Keywords: odisi,reader,import
 Author: Cristóbal Tapia Camú
 Author-email: crtapia@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -115,14 +115,22 @@
 import polars as pl
 
 load = pl.read_csv("load_data.csv")
 # Assume that the timestamp is in the column 'time'
 d.interpolate(load.select(pl.col("time")), clip=True)
 ```
 
+### Export segment data
+
+The data of all segments can be exported to individual csv-files with the following code:
+
+```python
+d.export_segments_csv(prefix="my_experiment", path="data_folder")
+```
+
 ## Tests
 
 The package includes a test suite which should be run with pytest:
 
 ```bash
 poetry run pytest
 ```
```

