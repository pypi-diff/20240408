# Comparing `tmp/eflips_ingest-1.0.1.tar.gz` & `tmp/eflips_ingest-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_ingest-1.0.1.tar", max compression
+gzip compressed data, was "eflips_ingest-1.0.2.tar", max compression
```

## Comparing `eflips_ingest-1.0.1.tar` & `eflips_ingest-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34143 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     7014 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/README.md
--rw-r--r--   0        0        0      207 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/__init__.py
--rw-r--r--   0        0        0     5811 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/base.py
--rw-r--r--   0        0        0    15422 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/dummy.py
--rw-r--r--   0        0        0        0 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/legacy/__init__.py
--rw-r--r--   0        0        0    63454 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/legacy/bvgxml.py
--rw-r--r--   0        0        0      383 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/legacy/xmldata/README.md
--rw-r--r--   0        0        0     1065 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/legacy/xmldata/__init__.py
--rw-r--r--   0        0        0    47033 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/legacy/xmldata/bvg_xml.py
--rw-r--r--   0        0        0     3049 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/util.py
--rw-r--r--   0        0        0     1120 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8056 1970-01-01 00:00:00.000000 eflips_ingest-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34143 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     7014 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/README.md
+-rw-r--r--   0        0        0      207 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/__init__.py
+-rw-r--r--   0        0        0     5979 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/base.py
+-rw-r--r--   0        0        0    15635 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/dummy.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/legacy/__init__.py
+-rw-r--r--   0        0        0    63454 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/legacy/bvgxml.py
+-rw-r--r--   0        0        0      383 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/legacy/xmldata/README.md
+-rw-r--r--   0        0        0     1065 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/legacy/xmldata/__init__.py
+-rw-r--r--   0        0        0    47033 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/legacy/xmldata/bvg_xml.py
+-rw-r--r--   0        0        0     3049 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/util.py
+-rw-r--r--   0        0        0     1120 2024-04-08 14:30:36.977329 eflips_ingest-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8056 1970-01-01 00:00:00.000000 eflips_ingest-1.0.2/PKG-INFO
```

### Comparing `eflips_ingest-1.0.1/LICENSE.md` & `eflips_ingest-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.1/README.md` & `eflips_ingest-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.1/eflips/ingest/base.py` & `eflips_ingest-1.0.2/eflips/ingest/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 class AbstractIngester(ABC):
     def __init__(self, database_url: str):
         """
         Constructor for the BaseIngester class.
 
         :param database_url: A string representing the URL of the database to ingest into. Must be of the form
                              postgresql://user:password@host:port/database. An url of the format
-                             postgis://user:password@host:port/database (django style) will be converted to the
-                             appropriate format.
+                             postgis://user:password@host:port/database (django style) will be converted to the4
         :return: None
         """
         if database_url.startswith("postgis://"):
             database_url = database_url.replace("postgis://", "postgresql://", 1)
         self.database_url = database_url
 
     @abstractmethod
@@ -70,14 +69,17 @@
         """
         Ingest the data into the database. In order for this method to be called, the :meth:`prepare` method must have
         returned a UUID, indicating that the preparation was successful.
 
         This method must call the progress_callback function periodically to update the progress of the ingestion
         process. The progress_callback function should accept a float value between 0 and 1.
 
+        The method should check if a scenario with the same UUID already exists in the database. If it does, it should
+        add the data to the existing scenario. If it does not, it should create a new scenario.
+
         :param uuid: A UUID representing the data to ingest.
         :return: Nothing. If unexpected errors occur, they should be raised as exceptions.
         """
         pass
 
     @property
     @abstractmethod
```

### Comparing `eflips_ingest-1.0.1/eflips/ingest/dummy.py` & `eflips_ingest-1.0.2/eflips/ingest/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,18 +162,22 @@
         with open(self.path_for_uuid(uuid) / "data.pkl", "rb") as f:
             params = pickle.load(f)
         assert isinstance(params, PrepareOptions)
 
         engine = create_engine(self.database_url)
 
         with Session(engine) as session:
-            scenario = Scenario(
-                name=params.name,
-            )
-            session.add(scenario)
+            scenario_or_none = session.query(Scenario).filter(Scenario.task_id == uuid).one_or_none()
+            if scenario_or_none:
+                scenario = scenario_or_none
+            else:
+                scenario = Scenario(
+                    name=params.name,
+                )
+                session.add(scenario)
 
             self._create_vehicle_types(scenario, session, params.bus_type)
             session.flush()  # To put the vehicle types into the database
 
             for i in range(params.depot_count):
                 depot = self._create_depot(scenario, session, i)
                 for j in range(params.line_count):
```

### Comparing `eflips_ingest-1.0.1/eflips/ingest/legacy/bvgxml.py` & `eflips_ingest-1.0.2/eflips/ingest/legacy/bvgxml.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.1/eflips/ingest/legacy/xmldata/__init__.py` & `eflips_ingest-1.0.2/eflips/ingest/legacy/xmldata/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.1/eflips/ingest/legacy/xmldata/bvg_xml.py` & `eflips_ingest-1.0.2/eflips/ingest/legacy/xmldata/bvg_xml.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.1/eflips/ingest/util.py` & `eflips_ingest-1.0.2/eflips/ingest/util.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.1/pyproject.toml` & `eflips_ingest-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-ingest"
-version = "1.0.1"
+version = "1.0.2"
 description = "A collection of import scripts for converting bus schedule data into the [eflips-model](https://github.com/mpm-tu-berlin/eflips-model) data format."
 authors = [
     "Ludger Heide <ludger.heide@lhtechnologies.de>"
 ]
 readme = "README.md"
 license = "AGPL-3.0-or-later"
 homepage = "https://github.com/mpm-tu-berlin/eflips-import"
```

### Comparing `eflips_ingest-1.0.1/PKG-INFO` & `eflips_ingest-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-ingest
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of import scripts for converting bus schedule data into the [eflips-model](https://github.com/mpm-tu-berlin/eflips-model) data format.
 Home-page: https://github.com/mpm-tu-berlin/eflips-import
 License: AGPL-3.0-or-later
 Author: Ludger Heide
 Author-email: ludger.heide@lhtechnologies.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

