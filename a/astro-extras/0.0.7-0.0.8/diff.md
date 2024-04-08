# Comparing `tmp/astro_extras-0.0.7.tar.gz` & `tmp/astro_extras-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_extras-0.0.7.tar", last modified: Thu Apr  4 14:31:12 2024, max compression
+gzip compressed data, was "astro_extras-0.0.8.tar", last modified: Mon Apr  8 07:18:12 2024, max compression
```

## Comparing `astro_extras-0.0.7.tar` & `astro_extras-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-04 14:31:12.316142 astro_extras-0.0.7/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.0.7/LICENSE
--rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.0.7/MANIFEST.in
--rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-04 14:31:12.316142 astro_extras-0.0.7/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.0.7/README.md
--rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.0.7/pyproject.toml
--rw-rw-r--   0 kol       (1000) kol       (1000)      260 2024-03-11 13:15:33.000000 astro_extras-0.0.7/requirements.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-04-04 14:31:12.316142 astro_extras-0.0.7/setup.cfg
--rw-rw-r--   0 kol       (1000) kol       (1000)     1109 2024-04-04 13:35:07.000000 astro_extras-0.0.7/setup.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-04 14:31:12.300143 astro_extras-0.0.7/src/
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-04 14:31:12.300143 astro_extras-0.0.7/src/astro_extras/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1000 2024-04-04 13:35:21.000000 astro_extras-0.0.7/src/astro_extras/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-04 14:31:12.312142 astro_extras-0.0.7/src/astro_extras/hooks/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.7/src/astro_extras/hooks/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-04 14:31:12.312142 astro_extras-0.0.7/src/astro_extras/operators/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.7/src/astro_extras/operators/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3880 2023-10-26 14:10:20.000000 astro_extras-0.0.7/src/astro_extras/operators/direct.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    18057 2023-11-20 09:48:16.000000 astro_extras-0.0.7/src/astro_extras/operators/session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    22750 2024-04-04 11:59:53.000000 astro_extras-0.0.7/src/astro_extras/operators/table.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-04 14:31:12.312142 astro_extras-0.0.7/src/astro_extras/sensors/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.0.7/src/astro_extras/sensors/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5530 2024-04-02 07:34:37.000000 astro_extras-0.0.7/src/astro_extras/sensors/file.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-04 14:31:12.312142 astro_extras-0.0.7/src/astro_extras/utils/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.7/src/astro_extras/utils/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    10549 2023-11-17 15:24:02.000000 astro_extras-0.0.7/src/astro_extras/utils/data_compare.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.0.7/src/astro_extras/utils/datetime_local.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5378 2024-03-11 14:28:15.000000 astro_extras-0.0.7/src/astro_extras/utils/template.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1952 2024-03-28 14:14:29.000000 astro_extras-0.0.7/src/astro_extras/utils/utils.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-04 14:31:12.316142 astro_extras-0.0.7/src/astro_extras.egg-info/
--rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-04 14:31:12.000000 astro_extras-0.0.7/src/astro_extras.egg-info/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)      821 2024-04-04 14:31:12.000000 astro_extras-0.0.7/src/astro_extras.egg-info/SOURCES.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-04-04 14:31:12.000000 astro_extras-0.0.7/src/astro_extras.egg-info/dependency_links.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)      112 2024-04-04 14:31:12.000000 astro_extras-0.0.7/src/astro_extras.egg-info/requires.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-04-04 14:31:12.000000 astro_extras-0.0.7/src/astro_extras.egg-info/top_level.txt
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-04 14:31:12.312142 astro_extras-0.0.7/tests/
--rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.0.7/tests/test_session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     6158 2023-11-17 10:36:18.000000 astro_extras-0.0.7/tests/test_table.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.0.7/tests/test_templates.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-03-11 14:20:58.000000 astro_extras-0.0.7/tests/test_utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.487523 astro_extras-0.0.8/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.0.8/LICENSE
+-rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.0.8/MANIFEST.in
+-rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-08 07:18:12.487523 astro_extras-0.0.8/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.0.8/README.md
+-rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.0.8/pyproject.toml
+-rw-rw-r--   0 kol       (1000) kol       (1000)      260 2024-03-11 13:15:33.000000 astro_extras-0.0.8/requirements.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-04-08 07:18:12.487523 astro_extras-0.0.8/setup.cfg
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1109 2024-04-06 11:02:14.000000 astro_extras-0.0.8/setup.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.467523 astro_extras-0.0.8/src/
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.471523 astro_extras-0.0.8/src/astro_extras/
+-rw-rw-r--   0 kol       (1000) kol       (1000)      963 2024-04-06 11:01:44.000000 astro_extras-0.0.8/src/astro_extras/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.483523 astro_extras-0.0.8/src/astro_extras/hooks/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.8/src/astro_extras/hooks/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.483523 astro_extras-0.0.8/src/astro_extras/operators/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.8/src/astro_extras/operators/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.0.8/src/astro_extras/operators/direct.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    18057 2023-11-20 09:48:16.000000 astro_extras-0.0.8/src/astro_extras/operators/session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    24723 2024-04-06 11:01:05.000000 astro_extras-0.0.8/src/astro_extras/operators/table.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.483523 astro_extras-0.0.8/src/astro_extras/sensors/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.0.8/src/astro_extras/sensors/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.0.8/src/astro_extras/sensors/file.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.487523 astro_extras-0.0.8/src/astro_extras/utils/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.8/src/astro_extras/utils/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    10650 2024-04-06 10:39:43.000000 astro_extras-0.0.8/src/astro_extras/utils/data_compare.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.0.8/src/astro_extras/utils/datetime_local.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5378 2024-03-11 14:28:15.000000 astro_extras-0.0.8/src/astro_extras/utils/template.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     2029 2024-04-06 10:45:20.000000 astro_extras-0.0.8/src/astro_extras/utils/utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.487523 astro_extras-0.0.8/src/astro_extras.egg-info/
+-rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-08 07:18:12.000000 astro_extras-0.0.8/src/astro_extras.egg-info/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)      821 2024-04-08 07:18:12.000000 astro_extras-0.0.8/src/astro_extras.egg-info/SOURCES.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-04-08 07:18:12.000000 astro_extras-0.0.8/src/astro_extras.egg-info/dependency_links.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)      112 2024-04-08 07:18:12.000000 astro_extras-0.0.8/src/astro_extras.egg-info/requires.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-04-08 07:18:12.000000 astro_extras-0.0.8/src/astro_extras.egg-info/top_level.txt
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-08 07:18:12.487523 astro_extras-0.0.8/tests/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.0.8/tests/test_session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     6158 2023-11-17 10:36:18.000000 astro_extras-0.0.8/tests/test_table.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.0.8/tests/test_templates.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-03-11 14:20:58.000000 astro_extras-0.0.8/tests/test_utils.py
```

### Comparing `astro_extras-0.0.7/LICENSE` & `astro_extras-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.7/PKG-INFO` & `astro_extras-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.0.7
+Version: 0.0.8
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.0.7/README.md` & `astro_extras-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.7/setup.py` & `astro_extras-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="astro_extras",
-    version="0.0.7",
+    version="0.0.8",
     author="Kol",
     author_email="skolchin@gmail.com",
     description="Additional Astro SDK operators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/skolchin/astro-extras",
     classifiers=[
```

### Comparing `astro_extras-0.0.7/src/astro_extras/__init__.py` & `astro_extras-0.0.8/src/astro_extras/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Astro SDK Extras project
 # (c) kol, 2023-2024
 
-__version__ = '0.0.7'
+__version__ = '0.0.8'
 
 from .operators.session import (
     open_session, 
     close_session,
     ETLSession,
     get_current_session,
     get_session_period,
@@ -15,14 +15,15 @@
     load_table,
     save_table,
     declare_tables,
     transfer_table, 
     transfer_tables,
     update_timed_table, 
     update_timed_tables,
+    compare_tables,
 )
 from .operators.direct import (
     run_sql_template,
     run_sql_templates,
 )
 from .sensors.file import (
     FileChangedSensor
@@ -42,10 +43,8 @@
     datetime_to_local,
     datetime_to_utc,
     datetime_to_tz,
     datetime_to_naive,
     days_ago,
     months_ago
 )
-from .utils.data_compare import (
-    compare_datasets
-)
+
```

### Comparing `astro_extras-0.0.7/src/astro_extras/operators/direct.py` & `astro_extras-0.0.8/src/astro_extras/operators/direct.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from ..utils.template import get_template
 
 _logger = logging.getLogger('airflow.task')
 
 def run_sql_template(
     template: str,
     conn_id: str,
-    input_tables: Optional[Iterable[Table]] = None,
-    affected_tables: Optional[Iterable[Table]] = None,
+    input_tables: Iterable[Table] | None = None,
+    affected_tables: Iterable[Table] | None = None,
     **kwargs
 ) -> XComArg:
     """ Runs an SQL script from template file.
     
     SQL script is a single SQL statement or multiple statements 
     to do something good within a single database.
 
@@ -69,16 +69,16 @@
         return sql
 
     return _run_sql(template)
 
 def run_sql_templates(
     templates: Iterable[str],
     conn_id: str,
-    group_id: Optional[str] = None,
-    num_parallel: Optional[int] = 1,
+    group_id: str | None = None,
+    num_parallel: int = 1,
     **kwargs,
 ) -> TaskGroup:
     """ Runs SQL scripts from multiple template files wrapping them up
     in Airflow's `TaskGroup`. See `run_sql_template` for details.
 
     Args:
         templates: List of template names, which are to be base names of `.sql` files
```

### Comparing `astro_extras-0.0.7/src/astro_extras/operators/session.py` & `astro_extras-0.0.8/src/astro_extras/operators/session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.7/src/astro_extras/operators/table.py` & `astro_extras-0.0.8/src/astro_extras/operators/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # Astro SDK Extras project
 # (c) kol, 2023
 
 """ Table operations """
 
-import pandas as pd
 import logging
+import pandas as pd
 from sqlalchemy import text
-from airflow.hooks.base import BaseHook
-from airflow.models.xcom_arg import XComArg
+
 from airflow.models.dag import DagContext
-from airflow.operators.generic_transfer import GenericTransfer
 from airflow.utils.context import Context
+from airflow.models.xcom_arg import XComArg
 from airflow.utils.task_group import TaskGroup
 from airflow.exceptions import AirflowFailException
+from airflow.providers.common.sql.hooks.sql import DbApiHook
+from airflow.operators.generic_transfer import GenericTransfer
 
 from astro import sql as aql
 from astro.databases import create_database
 from astro.sql.table import BaseTable, Table
 from astro.databases.base import BaseDatabase
 from astro.airflow.datasets import kwargs_with_datasets
 
-from typing import Type, Union, Literal, Optional, Iterable, List
+from typing import Iterable, List
 
 from .session import ETLSession, ensure_session
 from ..utils.utils import ensure_table, schedule_ops, split_table_name
 from ..utils.template import get_template_file
 from ..utils.data_compare import compare_datasets, compare_timed_dict
 
 class TableTransfer(GenericTransfer):
@@ -39,15 +40,15 @@
     ui_color = "#b0f07c"
 
     def __init__(
         self,
         *,
         source_table: BaseTable,
         destination_table: BaseTable,
-        session: Optional[ETLSession] = None,
+        session: ETLSession | None = None,
         **kwargs,
     ) -> None:
 
         source_db = create_database(source_table.conn_id, source_table)
         dest_db = create_database(destination_table.conn_id, destination_table)
         sql = kwargs.pop('sql', self._get_sql(source_table, source_db, session))
 
@@ -62,15 +63,15 @@
         self.source: BaseTable = source_table
         self.source_table: str = source_db.get_table_qualified_name(self.source)
         self.destination: BaseTable = destination_table
         # self.destination_table is set by super().__init__()
         self.session: ETLSession = session
         self._pre_execute_called = False
 
-    def _get_sql(self, table: Table, db: BaseDatabase, session: ETLSession = None, suffix: str = None) -> str:
+    def _get_sql(self, table: BaseTable, db: BaseDatabase, session: ETLSession | None = None, suffix: str | None = None) -> str:
         """ Internal - get a sql statement or template for given table """
 
         if (sql_file := get_template_file(table.name, '.sql')):
             self.log.info(f'Using template file {sql_file}')
             return sql_file
 
         full_name = db.get_table_qualified_name(table) + (suffix or '')
@@ -80,14 +81,15 @@
         return 'select * from ' + full_name
 
     def _pre_execute(self, context: Context):
         """ Do all checks before execution """
         if self._pre_execute_called:
             return
         
+        assert 'dag_run' in context
         if context['dag_run'].conf.get('debug'):
             self.log.setLevel(logging.DEBUG)
             logging.getLogger('airflow.task').setLevel(logging.DEBUG)
 
         self.session = ensure_session(self.session, context)
         if self.session:
             if not self.source_conn_id:
@@ -121,47 +123,63 @@
     ui_color = "#8cbf62"
 
     def __init__(
         self,
         *,
         source_table: BaseTable,
         destination_table: BaseTable,
-        session: Optional[ETLSession] = None,
+        session: ETLSession | None = None,
         **kwargs,
     ) -> None:
 
         dest_db = create_database(destination_table.conn_id, destination_table)
         dest_sql = kwargs.pop('destination_sql', self._get_sql(destination_table, dest_db, suffix='_a'))
 
         super().__init__(source_table=source_table,
                          destination_table=destination_table,
                          session=session,
                          **kwargs)
 
         self.destination_sql: str = dest_sql
 
-    def _compare_datasets(self, stop_on_first_diff: bool) -> bool:
+    def _compare_datasets(self, stop_on_first_diff: bool, logger: logging.Logger | None = None) -> bool:
         """ Internal - compare source and target dictionaries """
 
-        src = BaseHook.get_hook(self.source_conn_id)
-        dest = BaseHook.get_hook(self.destination_conn_id)
+        logger = logger or self.log
 
-        self.log.info(f'Executing: {self.sql}')
+        src = DbApiHook.get_hook(self.source_conn_id)
+        dest = DbApiHook.get_hook(self.destination_conn_id)
+
+        logger.info(f'Executing: {self.sql}')
         df_src = src.get_pandas_df(self.sql)
-        self.log.info(f'Executing: {self.destination_sql}')
+        logger.info(f'Executing: {self.destination_sql}')
         df_trg = dest.get_pandas_df(self.destination_sql)
 
-        return compare_datasets(df_src, df_trg, stop_on_first_diff=stop_on_first_diff)
+        return compare_datasets(df_src, df_trg, stop_on_first_diff=stop_on_first_diff, logger=logger)
 
     def execute(self, context: Context):
         """ Execute operator """
         self._pre_execute(context)
         if not self._compare_datasets(stop_on_first_diff=True):
             return super().execute(context)
 
+class CompareTableOperator(ChangedTableTransfer):
+    """
+    Table comparsion operator to be used within `compare_table` function.
+    Compares source and target data and prints results to log.
+    """
+    ui_color = "#64bf62"
+
+    def execute(self, context: Context):
+        """ Execute operator """
+        logger = logging.getLogger(f'compare_tables_logger')
+        logger.setLevel(logging.DEBUG)
+        if not self._compare_datasets(stop_on_first_diff=True, logger=logger):
+            raise AirflowFailException(f'Differences detected')
+
 class TimedTableTransfer(TableTransfer):
     """
     Table transfer operator to be used within `update_timed_dict` function.
     Implements timed dictionary update behaviour.
     Requiures `xxx_a` view to exist both on source and target.
     """
 
@@ -170,15 +188,15 @@
     ui_color = "#597a3d"
 
     def __init__(
         self,
         *,
         source_table: BaseTable,
         destination_table: BaseTable,
-        session: Optional[ETLSession] = None,
+        session: ETLSession | None = None,
         **kwargs,
     ) -> None:
 
         source_db = create_database(source_table.conn_id, source_table)
         sql = kwargs.pop('sql', self._get_sql(source_table, source_db, session, suffix='_a'))
         dest_db = create_database(destination_table.conn_id, destination_table)
         dest_sql = kwargs.pop('destination_sql', self._get_sql(destination_table, dest_db, suffix='_a'))
@@ -194,16 +212,16 @@
     def execute(self, context: Context):
         """ Execute operator """
 
         # All the checks
         self._pre_execute(context)
 
         # Get source and target data
-        src = BaseHook.get_hook(self.source_conn_id)
-        dest = BaseHook.get_hook(self.destination_conn_id)
+        src = DbApiHook.get_hook(self.source_conn_id)
+        dest = DbApiHook.get_hook(self.destination_conn_id)
 
         self.log.info(f'Executing: {self.sql}')
         df_src = src.get_pandas_df(self.sql)
         self.log.info(f'Executing: {self.destination_sql}')
         df_trg = dest.get_pandas_df(self.destination_sql)
 
         # Get the deltas
@@ -222,18 +240,18 @@
                     self.log.info(f'Executing: {sql}')
                     conn.execute(text(sql))
 
             if df_opening is not None:
                 df_opening.to_sql(dest_table, conn, schema=dest_schema, index=False, if_exists='append')
 
 def load_table(
-        table: Union[str, BaseTable],
-        conn_id: Optional[str] = None,
-        session: Optional[ETLSession] = None,
-        sql: Optional[str] = None) -> XComArg:
+        table: str | BaseTable,
+        conn_id: str | None = None,
+        session: ETLSession | None = None,
+        sql: str | None = None) -> XComArg:
     """ Loads table into memory.
 
     This is a wrapper over Astro-SDK `run_raw_sql` to
     load data from given database table into XCom and make it available for 
     further processing.
 
     SQL templating is supported, e.g. if a template for given table was found, it
@@ -273,37 +291,37 @@
 
     if not isinstance(table, BaseTable):
         dag = DagContext.get_current_dag()
         @aql.run_raw_sql(handler=lambda result: result.fetchall(),
                         conn_id=conn_id,
                         task_id=f'load-{table}',
                         results_format='pandas_dataframe')
-        def _load_table_by_name(table: str, session: ETLSession):
+        def _load_table_by_name(table: str, session: ETLSession | None):
             sql_file = get_template_file(table, '.sql', dag=dag)
             return sql or sql_file or f'select * from {table}'
 
         return _load_table_by_name(table, session)
     else:
         dag = DagContext.get_current_dag()
         @aql.run_raw_sql(handler=lambda result: result.fetchall(),
                         conn_id=conn_id,
                         task_id=f'load-{table.name}',
                         results_format='pandas_dataframe')
-        def _load_table(table: Table, session: ETLSession):
+        def _load_table(table: BaseTable, session: ETLSession | None):
             sql_file = get_template_file(table.name, '.sql', dag=dag)
             return sql or sql_file or '''select * from {{table}}'''
 
         return _load_table(table, session)
 
 def save_table(
         data: XComArg,
-        table: Union[str, BaseTable],
-        conn_id: Optional[str] = None,
-        session: Optional[ETLSession] = None,
-        fail_if_not_exist: Optional[bool] = True) -> XComArg:
+        table: str | BaseTable,
+        conn_id: str | None = None,
+        session: ETLSession | None = None,
+        fail_if_not_exist: bool | None = True) -> XComArg:
     """ Saves a table into database """
 
     table = ensure_table(table, conn_id)
     task_id = f'save-{table.name}'
     conn_id = conn_id or table.conn_id
 
     @aql.dataframe(if_exists='append', conn_id=conn_id, task_id=task_id)
@@ -317,29 +335,29 @@
             data.insert(0, 'session_id', session.session_id)
         return data
 
     return _save_data(data, session, output_table=table)
 
 def declare_tables(
         table_names: Iterable[str],
-        conn_id: Optional[str] = None,
-        schema: Optional[str] = None,
-        database: Optional[str] = None,
-) -> List[Table]:
+        conn_id: str | None = None,
+        schema: str | None = None,
+        database: str | None = None,
+) -> List[BaseTable]:
     """ Convert list of string table names to list of `Table` objects """
 
     return [ensure_table(t, conn_id, schema, database) for t in table_names]
 
 def transfer_table(
-        source: Union[str, Table],
-        target: Union[str, Table, None] = None,
-        source_conn_id: Optional[str] = None,
-        destination_conn_id: Optional[str] = None,
-        session: Union[XComArg, ETLSession, None] = None,
-        changes_only: Optional[bool] = False,
+        source: str | BaseTable,
+        target: str | BaseTable | None = None,
+        source_conn_id: str | None = None,
+        destination_conn_id: str | None = None,
+        session: XComArg | ETLSession | None = None,
+        changes_only: bool | None = False,
         **kwargs) -> XComArg:
     
     """ Cross-database data transfer.
 
     This function implements cross-database geterogenous data transfer.
 
     It reads data from source table into memory and then sequentaly inserts 
@@ -390,15 +408,15 @@
             Used only with string target table name; for `Table` objects, `conn_id` field is used.
             If omitted and `session` argument is provided, `session.destination_conn_id` will be used.
 
         session:    `ETLSession` object. If set and no SQL template is defined,
             a `session_id` field will be automatically added to selection.
 
         changes_only:   If set to `True`, the operator will compare source and target
-            tables and transfer data only when they are different. Target data ara obtained
+            tables and transfer data only when they are different. Target data are obtained
             by runnning `destination_sql`. By default, this query will be built using 
             `<destination_table>_a` view to get actual data.
 
         kwargs:     Any parameters passed to underlying operator (e.g. `preoperator`, ...)
 
     Returns:
         `XComArg` object
@@ -417,41 +435,41 @@
 
         >>> with DAG(...) as dag, ETLSession('source_db', 'target_db') as sess:
         >>>     transfer_table('public.table_data', session=sess)
 
     """
 
     source_table = ensure_table(source, source_conn_id)
-    dest_table = ensure_table(target, destination_conn_id) or source_table
+    dest_table = ensure_table(target or source_table, destination_conn_id)
     op_cls = TableTransfer if not changes_only else ChangedTableTransfer
     op = op_cls(
         source_table=source_table,
         destination_table=dest_table,
         session=session,
         **kwargs_with_datasets(kwargs=kwargs, 
                                input_datasets=source_table, 
                                output_datasets=dest_table)
     )
     return XComArg(op)
 
 def transfer_tables(
-        source_tables: List[Union[str, Table]],
-        target_tables: Optional[List[Union[str, Table]]] = None,
-        source_conn_id: Optional[str] = None,
-        destination_conn_id: Optional[str] = None,
-        group_id: Optional[str] = None,
-        num_parallel: Optional[int] = 1,
-        session: Union[XComArg, ETLSession, None] = None,
-        changes_only: Optional[bool] = False,
+        source_tables: List[str | Table],
+        target_tables: List[str | Table] | None = None,
+        source_conn_id: str | None = None,
+        destination_conn_id: str | None = None,
+        group_id: str | None = None,
+        num_parallel: int = 1,
+        session: XComArg | ETLSession | None = None,
+        changes_only: bool | None = False,
         **kwargs) -> TaskGroup:
 
     """ Transfer multiple tables.
 
     Creates an Airflow task group consisting of `TableTransfer` operators 
-    for each table pair from `source_tables` and `target_tables` list.
+    for each table pair from `source_tables` and `target_tables` lists.
 
     See `transfer_table` for more information.
     """
 
     if target_tables and len(target_tables) != len(source_tables):
         raise AirflowFailException(f'Source and target tables list size must be equal')
 
@@ -471,20 +489,52 @@
                     kwargs=kwargs, 
                     input_datasets=source_table, 
                     output_datasets=dest_table))
             ops_list.append(op)
         schedule_ops(ops_list, num_parallel)
     return tg
 
+def compare_tables(
+        source_tables: List[str | Table],
+        target_tables: List[str | Table] | None = None,
+        source_conn_id: str | None = None,
+        destination_conn_id: str | None = None,
+        group_id: str | None = None,
+        num_parallel: int = 1,
+        **kwargs) -> TaskGroup:
+
+    """ Compares multiple tables.
+
+    Creates an Airflow task group consisting of `CompareTableTransfer` operators 
+    for each table pair from `source_tables` and `target_tables` lists.
+    Each operator will compare source and target table and fails if any differences
+    are detected among them.
+    """
+    if not target_tables or len(target_tables) != len(source_tables):
+        raise AirflowFailException(f'Source and target tables list size must be equal')
+
+    with TaskGroup(group_id or 'compare-tables', add_suffix_on_collision=True) as tg:
+        ops_list = []
+        for (source, target) in zip(source_tables, target_tables):
+            source_table = ensure_table(source, source_conn_id)
+            dest_table = ensure_table(target, destination_conn_id) or source_table
+            op = CompareTableOperator(
+                source_table=source_table, 
+                destination_table=dest_table, 
+                task_id=f'compare-{source_table.name}')
+            ops_list.append(op)
+        schedule_ops(ops_list, num_parallel)
+    return tg
+
 def update_timed_table(
-        source: Union[str, Table],
-        target: Union[str, Table, None] = None,
-        source_conn_id: Optional[str] = None,
-        destination_conn_id: Optional[str] = None,
-        session: Union[XComArg, ETLSession, None] = None,
+        source: str | BaseTable,
+        target: str | BaseTable | None = None,
+        source_conn_id: str | None = None,
+        destination_conn_id: str | None = None,
+        session: XComArg | ETLSession | None = None,
         **kwargs) -> XComArg:
     
     """ Updates timed dictionary table """
 
     source_table = ensure_table(source, source_conn_id)
     dest_table = ensure_table(target, destination_conn_id) or source_table
     op = TimedTableTransfer(
@@ -494,21 +544,21 @@
         **kwargs_with_datasets(kwargs=kwargs, 
                                input_datasets=source_table, 
                                output_datasets=dest_table)
     )
     return XComArg(op)
 
 def update_timed_tables(
-        source_tables: List[Union[str, Table]],
-        target_tables: Optional[List[Union[str, Table]]] = None,
-        source_conn_id: Optional[str] = None,
-        destination_conn_id: Optional[str] = None,
-        group_id: Optional[str] = None,
-        num_parallel: Optional[int] = 1,
-        session: Union[XComArg, ETLSession, None] = None,
+        source_tables: List[str | Table],
+        target_tables: List[str | Table] | None = None,
+        source_conn_id: str | None = None,
+        destination_conn_id: str | None = None,
+        group_id: str | None = None,
+        num_parallel: int = 1,
+        session: XComArg | ETLSession | None = None,
         **kwargs) -> TaskGroup:
 
     """ Updates multiple timed dictionary tables """
 
     if target_tables and len(target_tables) != len(source_tables):
         raise AirflowFailException(f'Source and target tables list size must be equal')
```

### Comparing `astro_extras-0.0.7/src/astro_extras/sensors/file.py` & `astro_extras-0.0.8/src/astro_extras/sensors/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,18 +90,21 @@
             await asyncio.sleep(self.poll_interval)
 
 class FileChangedSensor(FileSensor):
     """
     Extension of standard ``FileSensor`` which waits for a file to appear on a filesystem,
     and to be modified since last check.
 
-    :param fs_conn_id: reference to the File (path) connection id
-    :param filepath: file name to look after (wildcards/directories not allowed)
-    :param deferrable: triggers Airflow task deferral mode
-    :return    2-element tuple with file name and file modification time as isoformatted datetime
+    Args:
+        fs_conn_id: reference to the File (path) connection id
+        filepath: file name to look after (wildcards/directories not allowed)
+        deferrable: triggers Airflow task deferral mode
+
+    Returns:
+        2-element tuple with file name and file modification time as isoformatted string
     """
 
     def __init__(
             self,
             *,
             deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
             **kwargs,
```

### Comparing `astro_extras-0.0.7/src/astro_extras/utils/data_compare.py` & `astro_extras-0.0.8/src/astro_extras/utils/data_compare.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,19 @@
             if key in vals:
                 split_vals[suffix][shared_key] = vals[key]
     return split_vals['x'], split_vals['y']
 
 def _adjust_timestamps(df: pd.DataFrame, exclude_cols: Iterable):
     """ Internal: adjust timestamps to common TZ """
 
-    _logger = logging.getLogger('airflow.task')
+    logger = logging.getLogger('airflow.task')
     tz_cols = [col for col in df.columns if df[col].dtype == 'datetime64[ns]' and
                 col not in exclude_cols]
     if tz_cols:
-        _logger.debug(f'Converting TZ-unaware timestamp columns {tz_cols} to timezone {TIMEZONE.name}')
+        logger.debug(f'Converting TZ-unaware timestamp columns {tz_cols} to timezone {TIMEZONE.name}')
         for col in tz_cols:
             df[col] = df[col].map(lambda t: t.tz_localize(TIMEZONE.name))
 
     return df
 
 def _check_timestamp_types(df_a: pd.DataFrame, df_b: pd.DataFrame, exclude_cols: Iterable):
     """ Internal: check timestamp compatibility """
@@ -54,15 +54,16 @@
                                    f'{df_a.dtypes[col]} on source, {df_b.dtypes[col]} on target')
 
 def compare_datasets(
     df_src: pd.DataFrame, 
     df_trg: pd.DataFrame, 
     id_cols: Iterable = None, 
     exclude_cols: Iterable = None, 
-    stop_on_first_diff: bool = True) -> Union[bool, Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]]:
+    stop_on_first_diff: bool = True,
+    logger: logging.Logger = None) -> Union[bool, Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]]:
 
     """ Compare two dataframes by columns, their types and values.
 
     Args:
         df_src: Source dataframe
 
         df_trg: Target dataframe
@@ -71,73 +72,77 @@
             If empty, 1st column is considered to be ID
 
         exclude_cols: List of columns to be excluded from comparsion
 
         stop_on_first_diff: if `True`, any difference would stop the comparsion,
             otherwise it will continue and produce difference dataframes
 
+        logger: logger object (if `None`, `airflow.task` logger will be used)
+
     Returns:
-        If `stop_on_first_diff == True`, would return boolean flag whether do
-        the dataframes the same (`True`) or not (`False`).
+        If `stop_on_first_diff == True`, would return boolean flag whether
+        the dataframes are the same (`True`) or not (`False`).
 
-        Otherwise, will return 3 dataframes, for new, changed and 
-        deleted records from target. Any of them could be `None` meaning
-        no corresponding diff detected.
+        Otherwise, will return 3 dataframes for new, changed and 
+        deleted records. Any of them could be `None` meaning
+        no corresponding difference detected.
     """
 
+    logger = logger or logging.getLogger('airflow.task')
+
     orig_src_cols = list(df_src.columns)
     src_cols = df_src.columns.str.lower()
     trg_cols = df_trg.columns.str.lower()
     df_src.columns = src_cols
     df_trg.columns = trg_cols
-    _logger = logging.getLogger('airflow.task')
-    _logger.debug(f'Source cols: {src_cols}')
-    _logger.debug(f'Target cols: {trg_cols}')
+
+    logger.debug(f'Source cols: {src_cols}')
+    logger.debug(f'Target cols: {trg_cols}')
 
     if not exclude_cols:
         exclude_cols = []
     else:
         exclude_cols = [c.lower() for c in exclude_cols]
     exclude_cols.extend(['session_id', '_created', '_modified', '_deleted'])
-    _logger.debug(f'Excluded columns: {exclude_cols}')
+    logger.debug(f'Excluded columns: {exclude_cols}')
 
     if not id_cols:
         id_cols = [c for c in src_cols if c not in exclude_cols][:1]
     else:
         id_cols = [c.lower() for c in id_cols]
         diff_cols = set(id_cols).difference(src_cols)
         if diff_cols:
             raise AirflowFailException(f'ID columns missing from source dataset: {diff_cols}')
         diff_cols = set(id_cols).difference(trg_cols)
         if diff_cols:
             raise AirflowFailException(f'ID columns missing from target dataset: {diff_cols}')
-    _logger.debug(f'ID columns: {id_cols}')
+    logger.debug(f'ID columns: {id_cols}')
 
     diff_cols = set(src_cols).symmetric_difference(trg_cols).difference(exclude_cols)
     if diff_cols:
-        _logger.warning(f'Diff in columns detected: {diff_cols}.\n' + 
+        logger.warning(f'Diff in columns detected: {diff_cols}.\n' + 
                        'Operation will continue, but may result in incomplete data transfer or errors.\n' +
                        'Review the datasets and correct structure to avoid that.')
 
     if df_src.shape[0] != df_trg.shape[0] and stop_on_first_diff:
-        _logger.info('Number of records in source and target dataset is different')
+        logger.info('Number of records in source and target datasets is different')
         return False
 
     _check_timestamp_types(df_src, df_trg, exclude_cols)
 
     shared_cols = set(src_cols).intersection(trg_cols).difference(exclude_cols)
-    _logger.debug(f'Shared cols: {shared_cols}')
+    logger.debug(f'Shared cols: {shared_cols}')
 
     df_src.index.name = '__src_idx__'
     df_trg.index.name = '__trg_idx__'
     df_deleted = None
     df_merged = pd.merge(df_src.reset_index(), df_trg.reset_index(), how='outer', on=id_cols,
                             copy=False, indicator=True, sort=False)
     if df_merged['_merge'].eq('right_only').any():
-        _logger.info('Target dataset contains records not present on the source')
+        logger.info('Target dataset contains records not present on the source')
         if stop_on_first_diff:
             return False
 
         idx_list = df_merged[df_merged['_merge'] == 'right_only']['__trg_idx__']
         df_deleted = df_trg.iloc[idx_list]
         df_deleted.index.name = None
 
@@ -147,67 +152,67 @@
             yield d.pop('__src_idx__'), d.pop('__trg_idx__'), d
 
     new_idx, upd_idx = [], []
     for src_idx, trg_idx, vals in _iter_tuples():
         src_vals, trg_vals = _split_row(vals, id_cols, shared_cols)
         key_val = [src_vals[c] for c in id_cols]
 
-        _logger.debug(f'Src {src_idx}: {src_vals}')
-        _logger.debug(f'Trg {trg_idx}: {trg_vals}')
+        logger.debug(f'Src {src_idx}: {src_vals}')
+        logger.debug(f'Trg {trg_idx}: {trg_vals}')
 
         if not pd.isnull(vals.get('_deleted')) or vals.get('_merge') == 'right_only':
-            _logger.debug('Deleted record, skipping')
+            logger.debug('Deleted record, skipping')
             continue
         if pd.isnull(trg_idx):
             if stop_on_first_diff:
-                _logger.info(f'New record at {key_val}')
+                logger.info(f'New record at {key_val}')
                 return False
 
-            _logger.debug(f'New record at {key_val}')
+            logger.debug(f'New record at {key_val}')
             new_idx.append(src_idx)
         else:
             diff_values = {k: {'source': src_vals[k], 'target': trg_vals[k]} for k in shared_cols \
                 if not (pd.isnull(src_vals[k]) and pd.isnull(trg_vals[k])) \
                     and src_vals[k] != trg_vals[k]}
             if diff_values:
                 key_val = [src_vals[c] for c in id_cols]
                 if stop_on_first_diff:
-                    _logger.info(f'Diff at {id_cols}={key_val}: {diff_values}')
+                    logger.info(f'Diff at {id_cols}={key_val}: {diff_values}')
                     return False
                 
-                _logger.debug(f'Diff at {id_cols}={key_val}: {diff_values}')
+                logger.debug(f'Diff at {id_cols}={key_val}: {diff_values}')
                 upd_idx.append(src_idx)
 
     if stop_on_first_diff:
-        _logger.info(f'No differences detected')
+        logger.info(f'No differences detected')
         return True
 
     if not new_idx and not upd_idx and (df_deleted is None or df_deleted.empty):
-        _logger.info(f'No differences detected')
+        logger.info(f'No differences detected')
         return None, None, None
 
     if not new_idx:
         df_new = None
-        _logger.info(f'No new records on source')
+        logger.info(f'No new records on source')
     else:
         df_new = df_src.iloc[new_idx]
         df_new.index.name = None
         df_new.columns = orig_src_cols
-        _logger.info(f'{df_new.shape[0]} new records on source')
+        logger.info(f'{df_new.shape[0]} new records on source')
 
     if not upd_idx:
         df_upd = None
-        _logger.info(f'No modified records on source')
+        logger.info(f'No modified records on source')
     else:
         df_upd = df_src.iloc[upd_idx]
         df_upd.index.name = None
         df_upd.columns = orig_src_cols
-        _logger.info(f'{df_upd.shape[0]} modified records on source')
+        logger.info(f'{df_upd.shape[0]} modified records on source')
 
-    _logger.info(f'{df_deleted.shape[0] if df_deleted is not None else 0} records deleted on target')
+    logger.info(f'{df_deleted.shape[0] if df_deleted is not None else 0} records deleted on target')
 
     return df_new, df_upd, df_deleted
 
 
 def compare_timed_dict(df_src: pd.DataFrame, df_trg: pd.DataFrame) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """ Compares two datasets as if they are timed dictionary data. Returns dataframes with records to open and to close """
```

### Comparing `astro_extras-0.0.7/src/astro_extras/utils/datetime_local.py` & `astro_extras-0.0.8/src/astro_extras/utils/datetime_local.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.7/src/astro_extras/utils/template.py` & `astro_extras-0.0.8/src/astro_extras/utils/template.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.7/src/astro_extras/utils/utils.py` & `astro_extras-0.0.8/src/astro_extras/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,34 @@
         conn_id: Optional[str] = None, 
         schema: Optional[str] = None,
         database: Optional[str] = None) -> BaseTable:
     
     """ Ensure an object is a table """
     if table is None:
         return None
+    
     if isinstance(table, BaseTable):
         return table
-    if isinstance(table, str):
+    elif isinstance(table, str):
         schema_from_name, table = split_table_name(table)
         return Table(table, conn_id=conn_id, metadata=Metadata(schema=schema_from_name or schema, database=database))
-    
-    raise TypeError(f'Either str or BaseTable expected, {table.__class__.__name__} found')
+    else:
+        raise TypeError(f'Either str or BaseTable expected, {table.__class__.__name__} found')
 
 def schedule_ops(ops_list: List[BaseOperator], num_parallel: int = 1) -> List[BaseOperator]:
     """ Build parallel operator chains. Returns list of last operators in each chain. """
 
     if not ops_list:
         raise ValueError('Empty list')
     if len(ops_list) == 1:
         return ops_list[0]
     
+    if len(ops_list) == -1:
+        return ops_list
+    
     if num_parallel <= 1 or len(ops_list) <= num_parallel:
         _ = [a.set_downstream(b) for a, b in pairwise(ops_list)]
         return [ops_list[-1]]
 
     splits = list({k: [y[1] for y in g] \
         for k, g in groupby(enumerate(ops_list), lambda v: v[0] // (len(ops_list) // num_parallel))}.values())
     _ = [a.set_downstream(b) for g in splits for a, b in pairwise(g)]
```

### Comparing `astro_extras-0.0.7/src/astro_extras.egg-info/PKG-INFO` & `astro_extras-0.0.8/src/astro_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.0.7
+Version: 0.0.8
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.0.7/src/astro_extras.egg-info/SOURCES.txt` & `astro_extras-0.0.8/src/astro_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.7/tests/test_session.py` & `astro_extras-0.0.8/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.7/tests/test_table.py` & `astro_extras-0.0.8/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.7/tests/test_templates.py` & `astro_extras-0.0.8/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.7/tests/test_utils.py` & `astro_extras-0.0.8/tests/test_utils.py`

 * *Files identical despite different names*

