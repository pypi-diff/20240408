# Comparing `tmp/searegion_detection-0.0.1.tar.gz` & `tmp/searegion_detection-0.0.3.tar.gz`

## Comparing `searegion_detection-0.0.1.tar` & `searegion_detection-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 searegion_detection-0.0.1/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 searegion_detection-0.0.1/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 searegion_detection-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 searegion_detection-0.0.1/src/searegion_detection/__init__.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 searegion_detection-0.0.1/src/searegion_detection/pandaseavox.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 searegion_detection-0.0.1/src/searegion_detection/queryregion.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 searegion_detection-0.0.1/.gitignore
--rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 searegion_detection-0.0.1/LICENSE
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 searegion_detection-0.0.1/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 searegion_detection-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 searegion_detection-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 searegion_detection-0.0.3/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 searegion_detection-0.0.3/__init__.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 searegion_detection-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 searegion_detection-0.0.3/src/searegion_detection/__init__.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 searegion_detection-0.0.3/src/searegion_detection/pandaseavox.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 searegion_detection-0.0.3/src/searegion_detection/queryregion.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 searegion_detection-0.0.3/.gitignore
+-rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 searegion_detection-0.0.3/LICENSE
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 searegion_detection-0.0.3/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 searegion_detection-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 searegion_detection-0.0.3/PKG-INFO
```

### Comparing `searegion_detection-0.0.1/Makefile` & `searegion_detection-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `searegion_detection-0.0.1/src/searegion_detection/pandaseavox.py` & `searegion_detection-0.0.3/src/searegion_detection/pandaseavox.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 from copy import deepcopy
 from typing import Sequence
+from dataclasses import dataclass
 
 import numpy as np
 import pandas as pd
 from pandassta.df import Df, df_type_conversions
 from shapely.wkt import loads
 
-from .queryregion import (DbCredentials, build_points_query,
-                          build_query_points, connect)
+from .queryregion import DbCredentials, build_points_query, build_query_points, connect
 
 log = logging.getLogger(__name__)
 
 
+
 def seavox_to_df(response_seavox: Sequence[Sequence[str]]) -> pd.DataFrame:
     df = pd.DataFrame()
     df[[Df.REGION, Df.SUB_REGION]] = pd.DataFrame.from_records(response_seavox)
 
     return df
```

### Comparing `searegion_detection-0.0.1/src/searegion_detection/queryregion.py` & `searegion_detection-0.0.3/src/searegion_detection/queryregion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+from dataclasses import dataclass
 import logging
 import time
-from dataclasses import dataclass
 from typing import Sequence
 
 import psycopg2
 import psycopg2.extensions
 from shapely import Point, distance, intersects, set_srid
 from shapely.wkt import loads
 
-log = logging.getLogger(__name__)
-
 
 @dataclass
 class DbCredentials:
     database: str
     user: str
     host: str
     port: int
     passphrase: str
 
 
+# from services.df import seavox_to_df
+
+log = logging.getLogger(__name__)
+
 def connect(db_credentials: DbCredentials) -> psycopg2.extensions.connection:
     log.debug("Get connection seavox db")
     try:
         connection = psycopg2.connect(
             database=db_credentials.database,
             user=db_credentials.user,
             password=db_credentials.passphrase,
@@ -61,22 +63,24 @@
     q_out = ",".join(list_points)
     return q_out
 
 
 def main():
     t0 = time.time()
     points = [(3.0, 52), (2.9, 51.1), (89, 0.0), (52, 3.1254), (2, 2)] * 100
-    points_q = build_points_query([points[0]])
+    points_q = build_points_query(
+        [points[0]]
+        )
 
     db_credentials: DbCredentials = DbCredentials(
-        database="seavox_areas",
-        user="sevox",
-        host="localhost",
-        port=5432,
-        passphrase="ChangeMe",
+        database= "seavox_areas",
+        user= "sevox",
+        host= "localhost",
+        port= 5432,
+        passphrase="ChangeMe"
     )
 
     query_0 = build_query_points(
         table="seavox_sea_areas",
         points_query=points_q,
         select="region, sub_region, ST_AsText(geom)",
     )
```

### Comparing `searegion_detection-0.0.1/LICENSE` & `searegion_detection-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `searegion_detection-0.0.1/pyproject.toml` & `searegion_detection-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "searegion-detection"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
   { name="nvds" },
 ]
 description = "Package for searegion detection."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `searegion_detection-0.0.1/PKG-INFO` & `searegion_detection-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: searegion-detection
-Version: 0.0.1
+Version: 0.0.3
 Summary: Package for searegion detection.
 Project-URL: Homepage, https://github.com/nvdsteen/searegion-detection
 Project-URL: Issues, https://github.com/nvdsteen/searegion-detection/issues
 Author: nvds
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
-Requires-Dist: pandassta==0.0.1
+Requires-Dist: pandassta>=0.0.2
 Requires-Dist: psycopg2==2.9.9
 Requires-Dist: shapely==2.0.3
 Description-Content-Type: text/markdown
 
 # Searegion-detection
 
 package used for detecting searegions from coordinates using seavox database.
```

