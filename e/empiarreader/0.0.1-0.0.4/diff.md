# Comparing `tmp/empiarreader-0.0.1.tar.gz` & `tmp/empiarreader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empiarreader-0.0.1.tar", max compression
+gzip compressed data, was "empiarreader-0.0.4.tar", max compression
```

## Comparing `empiarreader-0.0.1.tar` & `empiarreader-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,14 @@
--rw-r--r--   0        0        0     1533 2023-06-02 10:55:49.533814 empiarreader-0.0.1/LICENSE
--rw-r--r--   0        0        0      768 2023-06-02 10:55:49.535437 empiarreader-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      158 2023-06-02 10:55:49.535779 empiarreader-0.0.1/src/empiarreader/__init__.py
--rw-r--r--   0        0        0     5428 2023-06-02 10:55:49.535983 empiarreader-0.0.1/src/empiarreader/empiar.py
--rw-r--r--   0        0        0     2710 2023-06-02 10:55:49.536162 empiarreader-0.0.1/src/empiarreader/mrcsource.py
--rw-r--r--   0        0        0     1838 2023-06-02 10:55:49.536359 empiarreader-0.0.1/src/empiarreader/starsource.py
--rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 empiarreader-0.0.1/setup.py
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 empiarreader-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1533 2023-05-18 11:07:30.325791 empiarreader-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5608 2024-04-08 13:47:25.654343 empiarreader-0.0.4/README.md
+-rw-r--r--   0        0        0     1383 2024-04-08 13:47:25.654343 empiarreader-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      242 2023-08-23 08:23:07.897607 empiarreader-0.0.4/src/empiarreader/__init__.py
+-rw-r--r--   0        0        0     1260 2024-01-16 15:43:56.940158 empiarreader-0.0.4/src/empiarreader/cli.py
+-rw-r--r--   0        0        0        0 2023-08-23 08:23:07.897607 empiarreader-0.0.4/src/empiarreader/empiar/__init__.py
+-rw-r--r--   0        0        0     6937 2024-01-16 15:43:56.940158 empiarreader-0.0.4/src/empiarreader/empiar/empiar.py
+-rw-r--r--   0        0        0        0 2023-08-23 08:23:07.897607 empiarreader-0.0.4/src/empiarreader/intake_source/__init__.py
+-rw-r--r--   0        0        0     2777 2024-01-16 15:43:56.940158 empiarreader-0.0.4/src/empiarreader/intake_source/mrcsource.py
+-rw-r--r--   0        0        0     1913 2024-01-16 15:43:56.940158 empiarreader-0.0.4/src/empiarreader/intake_source/starsource.py
+-rw-r--r--   0        0        0        0 2023-08-23 08:23:07.897607 empiarreader-0.0.4/src/empiarreader/utilities/__init__.py
+-rw-r--r--   0        0        0     3582 2024-01-16 15:43:56.940158 empiarreader-0.0.4/src/empiarreader/utilities/download.py
+-rw-r--r--   0        0        0     4104 2024-01-16 15:43:56.940158 empiarreader-0.0.4/src/empiarreader/utilities/search.py
+-rw-r--r--   0        0        0     7055 1970-01-01 00:00:00.000000 empiarreader-0.0.4/PKG-INFO
```

### Comparing `empiarreader-0.0.1/LICENSE` & `empiarreader-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `empiarreader-0.0.1/src/empiarreader/empiar.py` & `empiarreader-0.0.4/src/empiarreader/empiar/empiar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 import re
 
 import requests
+import fnmatch
 
 from urllib.parse import urlparse
 from pathlib import Path
 from intake.source.base import Schema, DataSource
 from intake.catalog.base import Catalog
 from intake.catalog.local import LocalCatalogEntry
 from bs4 import BeautifulSoup
 
-from .mrcsource import MrcSource
-from .starsource import StarSource
+from empiarreader.intake_source.mrcsource import MrcSource
+from empiarreader.intake_source.starsource import StarSource
 
 
 class EmpiarCatalog(Catalog):
+    """Catalog for the EMPIAR entries
+
+    Args:
+        empiar_index: Index for the dataset in the archive.
+    """
+
     name = "empiar_catalog"
 
     _empiar_url_api_base = "https://www.ebi.ac.uk/empiar/api"
 
     def __init__(self, empiar_index, metadata=None, **kwargs):
         self.empiar_index = empiar_index
 
         super().__init__(name=self.name, metadata=metadata, **kwargs)
 
     @classmethod
     def fetch_entry_data(cls, empiar_index):
+        """Requests the data from the entry according to the EMPIAR index."""
         req = requests.get(f"{cls._empiar_url_api_base}/entry/{empiar_index}")
         entry_data = list(req.json().values())[0]
         return entry_data
 
     def _load(self):
+        """Loads the dataset metadata after fetching the online information."""
         entry_data = self.fetch_entry_data(self.empiar_index)
 
         imagesets = entry_data["imagesets"]
 
         # TODO load other metadata
 
         for imageset in imagesets:
@@ -47,14 +56,30 @@
                     "directory": imageset["directory"],
                     "imageset_metadata": imageset,
                 },
             )
 
 
 class EmpiarSource(DataSource):
+    """General EMPIAR intake driver, as DataSource.
+
+    Args:
+        empiar_index: EMPIAR entry number
+        directory: directory for the relevant files, within the EMPIAR entry
+        driver: type of intake driver needed for the data (mrc, starfile or ...
+                any image)
+        filename: [Optional] Name for a specific file to download
+        regexp: [Optional] Name for a specific file type to download
+        imageset_metadata: [Optional] Metadata relative to the specific ...
+                            imageset needed
+        metadata: [Optional] Metadata relative to the entry
+        storage_options: [Optional] Option to save the data, or cache
+
+    """
+
     name = "empiar"
     container = "xarray"
     version = "0.0.1"
     partition_access = True
 
     _empiar_url_ftp_over_https_base = (
         "https://ftp.ebi.ac.uk/empiar/world_availability"
@@ -67,35 +92,40 @@
     }
 
     def __init__(
         self,
         empiar_index,
         directory,
         driver=None,
-        filename_regexp=None,
+        filename=None,
+        regexp=False,
         imageset_metadata=None,
         metadata=None,
         storage_options=None,
     ):
         super().__init__(metadata=metadata)
 
         self.empiar_index = empiar_index
         self.directory = directory
-        self.image_url_regexp = (
-            re.compile(filename_regexp) if filename_regexp else None
-        )
+        self.image_url_regexp = None
+        if filename and regexp:
+            self.image_url_regexp = re.compile(filename)
+        elif filename:
+            self.image_url_regexp = re.compile(fnmatch.translate(filename))
+
         self.imageset_metadata = imageset_metadata
 
         self._driver = driver
 
         self._image_urls = None
         self._datasource = None
 
     @property
     def data_directory_url(self):
+        """Retrieve the current selected data directory for the dataset."""
         return (
             f"{self._empiar_url_ftp_over_https_base}/"
             + f"{self.empiar_index}/{self.directory}"
         )
 
     def _parse_data_dir(self, data_dir_url):
         soup = BeautifulSoup(requests.get(data_dir_url).text, "html.parser")
@@ -171,20 +201,26 @@
 
         if self._datasource is None:
             self._datasource = self._driver(urlpath=self._image_urls)
 
         return self._schema
 
     def read(self):
+        """Reads the DataSource according to the metadata."""
         self._load_metadata()
 
         return self._datasource.read()
 
     def read_partition(self, i):
+        """ " Reads an individual element of the dataset.
+
+        Args:
+            i (int): Position of the element in the dataset"""
         self._load_metadata()
 
         return self._datasource.read_partition(i)
 
     def to_dask(self):
+        """Lazily read the DataSource according to the metadata, using Dask."""
         self._load_metadata()
 
         return self._datasource.to_dask()
```

### Comparing `empiarreader-0.0.1/src/empiarreader/mrcsource.py` & `empiarreader-0.0.4/src/empiarreader/intake_source/mrcsource.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 from intake.source.base import DataSource, Schema
 
 from fsspec.core import open_files
 
 
 class MrcSource(DataSource):
-    """Simple MRCfile intake driver"""
+    """Intake driver for mrcfiles as DataSource.
+
+    Args:
+        urlpath: URL for the mrcfile.
+    """
 
     container = "xarray"
     name = "mrc"
     version = "0.0.1"
     partition_access = True
 
     def __init__(self, urlpath, metadata=None):
```

### Comparing `empiarreader-0.0.1/src/empiarreader/starsource.py` & `empiarreader-0.0.4/src/empiarreader/intake_source/starsource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import intake
 import starfile
 from fsspec.core import open_files
 
 
 class StarSource(intake.source.base.DataSource):
-    """Starfile intake driver"""
+    """Intake driver for starfiles as DataSource.
+
+    Args:
+        urlpath: URL for the starfile.
+    """
 
     container = "xarray"
     name = "starfile"
     version = "0.0.1"
     partition_access = True
 
     def __init__(self, urlpath, metadata=None):
```

