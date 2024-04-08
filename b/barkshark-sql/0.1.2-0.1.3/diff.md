# Comparing `tmp/barkshark-sql-0.1.2.tar.gz` & `tmp/barkshark-sql-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barkshark-sql-0.1.2.tar", last modified: Mon Apr  1 18:31:47 2024, max compression
+gzip compressed data, was "barkshark-sql-0.1.3.tar", last modified: Mon Apr  8 19:54:16 2024, max compression
```

## Comparing `barkshark-sql-0.1.2.tar` & `barkshark-sql-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 18:31:47.994035 barkshark-sql-0.1.2/
--rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2022-11-19 10:00:01.000000 barkshark-sql-0.1.2/LICENSE.md
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2214 2024-04-01 18:31:47.994035 barkshark-sql-0.1.2/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      538 2024-03-10 22:34:07.000000 barkshark-sql-0.1.2/README.md
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 18:31:47.994035 barkshark-sql-0.1.2/barkshark_sql.egg-info/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2214 2024-04-01 18:31:47.000000 barkshark-sql-0.1.2/barkshark_sql.egg-info/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      389 2024-04-01 18:31:47.000000 barkshark-sql-0.1.2/barkshark_sql.egg-info/SOURCES.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-01 18:31:47.000000 barkshark-sql-0.1.2/barkshark_sql.egg-info/dependency_links.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)      178 2024-04-01 18:31:47.000000 barkshark-sql-0.1.2/barkshark_sql.egg-info/requires.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        5 2024-04-01 18:31:47.000000 barkshark-sql-0.1.2/barkshark_sql.egg-info/top_level.txt
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 18:31:47.994035 barkshark-sql-0.1.2/bsql/
--rw-r--r--   0 zoey      (1000) zoey      (1000)      528 2024-04-01 17:36:29.000000 barkshark-sql-0.1.2/bsql/__init__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     4706 2024-04-01 17:44:06.000000 barkshark-sql-0.1.2/bsql/backends.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)    18891 2024-04-01 17:47:15.000000 barkshark-sql-0.1.2/bsql/database.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1112 2024-02-19 17:31:54.000000 barkshark-sql-0.1.2/bsql/enums.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     3569 2024-04-01 17:48:22.000000 barkshark-sql-0.1.2/bsql/misc.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-10 22:38:06.000000 barkshark-sql-0.1.2/bsql/py.typed
--rw-r--r--   0 zoey      (1000) zoey      (1000)     7123 2024-04-01 17:48:47.000000 barkshark-sql-0.1.2/bsql/statement.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     7732 2024-04-01 17:49:07.000000 barkshark-sql-0.1.2/bsql/table.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2089 2024-04-01 18:22:58.000000 barkshark-sql-0.1.2/pyproject.toml
--rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-01 18:31:47.994035 barkshark-sql-0.1.2/setup.cfg
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 18:31:47.994035 barkshark-sql-0.1.2/tests/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1880 2024-04-01 18:22:11.000000 barkshark-sql-0.1.2/tests/test_statements.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)      654 2024-04-01 18:22:18.000000 barkshark-sql-0.1.2/tests/test_tables.py
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2022-11-19 10:00:01.000000 barkshark-sql-0.1.3/LICENSE.md
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2214 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      538 2024-03-10 22:34:07.000000 barkshark-sql-0.1.3/README.md
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/barkshark_sql.egg-info/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2214 2024-04-08 19:54:16.000000 barkshark-sql-0.1.3/barkshark_sql.egg-info/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      389 2024-04-08 19:54:16.000000 barkshark-sql-0.1.3/barkshark_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-08 19:54:16.000000 barkshark-sql-0.1.3/barkshark_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      178 2024-04-08 19:54:16.000000 barkshark-sql-0.1.3/barkshark_sql.egg-info/requires.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        5 2024-04-08 19:54:16.000000 barkshark-sql-0.1.3/barkshark_sql.egg-info/top_level.txt
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/bsql/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      538 2024-04-08 19:32:15.000000 barkshark-sql-0.1.3/bsql/__init__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     5365 2024-04-08 18:47:11.000000 barkshark-sql-0.1.3/bsql/backends.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    18977 2024-04-02 20:23:43.000000 barkshark-sql-0.1.3/bsql/database.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1178 2024-04-02 20:23:36.000000 barkshark-sql-0.1.3/bsql/enums.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     4174 2024-04-08 18:44:46.000000 barkshark-sql-0.1.3/bsql/misc.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-10 22:38:06.000000 barkshark-sql-0.1.3/bsql/py.typed
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     7209 2024-04-02 20:23:25.000000 barkshark-sql-0.1.3/bsql/statement.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     7732 2024-04-01 17:49:07.000000 barkshark-sql-0.1.3/bsql/table.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2089 2024-04-01 18:22:58.000000 barkshark-sql-0.1.3/pyproject.toml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/setup.cfg
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/tests/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1880 2024-04-01 18:22:11.000000 barkshark-sql-0.1.3/tests/test_statements.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      654 2024-04-01 18:22:18.000000 barkshark-sql-0.1.3/tests/test_tables.py
```

### Comparing `barkshark-sql-0.1.2/LICENSE.md` & `barkshark-sql-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.2/PKG-INFO` & `barkshark-sql-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barkshark-sql
-Version: 0.1.2
+Version: 0.1.3
 Summary: Connection pool and query builder for dbapi 2.0 database drivers
 Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/bsql
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/bsql/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/barkshark-sql
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/bsql
```

### Comparing `barkshark-sql-0.1.2/README.md` & `barkshark-sql-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.2/barkshark_sql.egg-info/PKG-INFO` & `barkshark-sql-0.1.3/barkshark_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barkshark-sql
-Version: 0.1.2
+Version: 0.1.3
 Summary: Connection pool and query builder for dbapi 2.0 database drivers
 Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/bsql
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/bsql/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/barkshark-sql
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/bsql
```

### Comparing `barkshark-sql-0.1.2/bsql/__init__.py` & `barkshark-sql-0.1.3/bsql/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 __software__ = "Barkshark SQL"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __author__ = "Zoey Mae"
 __homepage__ = "https://git.barkshark.xyz/barkshark/bsql"
 
 from .backends import Backend, PG8000, Sqlite3
 from .database import Connection, Cursor, Database
 from .enums import BackendType, Comparison, OrderDirection, StrEnum
 from .table import Tables, Table, Column
 from .statement import Statement, Select, Insert, Update, Delete, Where, OrderBy
 
 from .misc import (
 	ColumnDescription,
 	ConnectionProto,
 	CursorProto,
 	Row,
-	StatementParsingError
+	StatementParsingError,
+	boolean
 )
```

### Comparing `barkshark-sql-0.1.2/bsql/backends.py` & `barkshark-sql-0.1.3/bsql/backends.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
+import json
 import typing
 
 from abc import ABC, abstractmethod
 from datetime import datetime, timezone
 from importlib import import_module
 from pathlib import Path
 
 from .enums import BackendType
-from .misc import ClassProperty
+from .misc import ClassProperty, boolean
 
 if typing.TYPE_CHECKING:
 	from collections.abc import Iterable
 	from typing import Any
 	from types import ModuleType
 	from .database import Connection, Database
 	from .misc import ConnectionProto
@@ -112,14 +113,29 @@
 class Sqlite3(Backend):
 	"Supports connecting to sqlite databases with the :mod:`sqlite3` module."
 
 	module_name = "sqlite3"
 	backend_type = BackendType.SQLITE
 
 
+	def __init__(self) -> None:
+		self.module.register_adapter(datetime, lambda v: v.timestamp())
+		self.module.register_adapter(dict, json.dumps)
+		self.module.register_adapter(list, json.dumps)
+		self.module.register_adapter(tuple, json.dumps)
+		self.module.register_adapter(set, json.dumps)
+		self.module.register_adapter(bool, lambda v: boolean(v.decode("utf-8")))
+
+		self.module.register_converter("timestamp", Sqlite3.deserialize_timestamp)
+		self.module.register_converter("datetime", Sqlite3.deserialize_timestamp)
+		self.module.register_converter("json", json.loads)
+		self.module.register_converter("boolean", lambda v: True if v == b"1" else False)
+		self.module.register_converter("real", float)
+		self.module.register_converter("integer", int)
+
 	@staticmethod
 	def deserialize_timestamp(raw_value: bytes) -> datetime:
 		"""
 			Method used to serialize ``TIMESTMAP`` and ``DATETIME`` column values.
 		"""
 
 		value = raw_value.decode("utf-8")
@@ -128,26 +144,23 @@
 			return datetime.fromtimestamp(float(value), tz = timezone.utc)
 
 		except ValueError:
 			return datetime.fromisoformat(value)
 
 
 	def get_connection(self, database: Database) -> Any:
-		mod = self.module
-		mod.register_converter("timestamp", Sqlite3.deserialize_timestamp)
-		mod.register_converter("datetime", Sqlite3.deserialize_timestamp)
-
 		options = database.arguments.copy()
 
 		if "check_same_thread" not in options:
 			options["check_same_thread"] = False
 
-		return mod.connect(
+		return self.module.connect(
 			database.database,
-			detect_types = mod.PARSE_DECLTYPES,
+			detect_types = self.module.PARSE_DECLTYPES,
+			# autocommit = False,
 			**options
 		)
 
 
 	def get_databases(self, conn: Connection) -> Iterable[str]:
 		return tuple([])
```

### Comparing `barkshark-sql-0.1.2/bsql/database.py` & `barkshark-sql-0.1.3/bsql/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,24 @@
 from .misc import ColumnDescription, Row, StatementParsingError
 from .statement import Statement, Select, Insert, Update, Delete
 from .table import Tables
 
 if typing.TYPE_CHECKING:
 	from collections.abc import Generator, Iterable, Iterator
 	from types import TracebackType
-	from typing import Any, Self
+	from typing import Any
 	from .enums import BackendType
 	from .misc import ConnectionProto, CursorProto
 
+	try:
+		from typing import Self
+
+	except ImportError:
+		from typing_extensions import Self
+
 
 TRANS_QUERIES = (
 	"alter",
 	"begin",
 	"create",
 	"delete",
 	"drop",
```

### Comparing `barkshark-sql-0.1.2/bsql/enums.py` & `barkshark-sql-0.1.3/bsql/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
 import typing
 
 from enum import Enum
 
 if typing.TYPE_CHECKING:
-	from typing import Self
+	try:
+		from typing import Self
+
+	except ImportError:
+		from typing_extensions import Self
 
 
 class StrEnum(str, Enum):
 	"Base class for :class:`str`-based enums"
 
 	def __new__(cls: type[Self], value: str) -> Self:
 		return str.__new__(cls, value)
```

### Comparing `barkshark-sql-0.1.2/bsql/misc.py` & `barkshark-sql-0.1.3/bsql/misc.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,45 @@
 
 if typing.TYPE_CHECKING:
 	from collections.abc import Callable, Iterable
 	from typing import Any
 	from .database import Cursor
 
 
+def boolean(value: Any) -> bool:
+	"""
+		Convert any object into a boolean
+
+		:param value: The object to convert
+	"""
+
+	if isinstance(value, str):
+		if value.lower() in {'on', 'y', 'yes', 'true', 'enable', 'enabled', '1'}:
+			return True
+
+		if value.lower() in {'off', 'n', 'no', 'false', 'disable', 'disabled', '0'}:
+			return False
+
+		raise TypeError(f'Cannot parse string "{value}" as a boolean')
+
+	if isinstance(value, int):
+		if value == 1:
+			return True
+
+		if value == 0:
+			return False
+
+		raise ValueError('Integer value must be 1 or 0')
+
+	if value is None:
+		return False
+
+	return bool(value)
+
+
 class ClassProperty:
 	def __init__(self, func_get: Callable, func_set: Callable | None = None):
 		self.func_get = func_get
 		self.func_set = func_set
 
 
 	def __get__(self, obj: object, cls: type[object]) -> Any:
```

### Comparing `barkshark-sql-0.1.2/bsql/statement.py` & `barkshark-sql-0.1.3/bsql/statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 import typing
 
 from dataclasses import dataclass
 
 from .enums import Comparison, OrderDirection
 
 if typing.TYPE_CHECKING:
-	from typing import Any, Self
+	from typing import Any
 	from .enums import BackendType
 
+	try:
+		from typing import Self
+
+	except ImportError:
+		from typing_extensions import Self
+
 
 @dataclass()
 class Where:
 	"Represents a single comparison in a ``WHERE`` block"
 
 	key: str
 	"Column to compare the data to"
```

### Comparing `barkshark-sql-0.1.2/bsql/table.py` & `barkshark-sql-0.1.3/bsql/table.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.2/pyproject.toml` & `barkshark-sql-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.2/tests/test_statements.py` & `barkshark-sql-0.1.3/tests/test_statements.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.2/tests/test_tables.py` & `barkshark-sql-0.1.3/tests/test_tables.py`

 * *Files identical despite different names*

