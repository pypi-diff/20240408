# Comparing `tmp/shmessy-1.2.9.tar.gz` & `tmp/shmessy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shmessy-1.2.9.tar", max compression
+gzip compressed data, was "shmessy-1.3.0.tar", max compression
```

## Comparing `shmessy-1.2.9.tar` & `shmessy-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1073 2024-02-23 08:05:24.091698 shmessy-1.2.9/LICENSE
--rw-r--r--   0        0        0     5670 2024-02-23 08:05:24.091698 shmessy-1.2.9/README.md
--rw-r--r--   0        0        0      856 2024-02-23 08:05:53.591556 shmessy-1.2.9/pyproject.toml
--rw-r--r--   0        0        0     5706 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/__init__.py
--rw-r--r--   0        0        0     2023 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/exceptions.py
--rw-r--r--   0        0        0      395 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/schema.py
--rw-r--r--   0        0        0        0 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types/__init__.py
--rw-r--r--   0        0        0     1037 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types/base.py
--rw-r--r--   0        0        0     2226 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types/boolean.py
--rw-r--r--   0        0        0     2460 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types/date.py
--rw-r--r--   0        0        0     2870 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types/datetime_.py
--rw-r--r--   0        0        0     1016 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types/email.py
--rw-r--r--   0        0        0     1260 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types/float.py
--rw-r--r--   0        0        0     1256 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types/integer.py
--rw-r--r--   0        0        0     1272 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types/ipv4_address.py
--rw-r--r--   0        0        0     1018 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types/string.py
--rw-r--r--   0        0        0     3174 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types/unix_timestamp.py
--rw-r--r--   0        0        0     6451 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/types_handler.py
--rw-r--r--   0        0        0     1761 2024-02-23 08:05:24.095698 shmessy-1.2.9/src/shmessy/utils.py
--rw-r--r--   0        0        0     6354 1970-01-01 00:00:00.000000 shmessy-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-08 17:24:49.873855 shmessy-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5669 2024-04-08 17:24:49.873855 shmessy-1.3.0/README.md
+-rw-r--r--   0        0        0      856 2024-04-08 17:25:19.726321 shmessy-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5701 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/__init__.py
+-rw-r--r--   0        0        0     2023 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/exceptions.py
+-rw-r--r--   0        0        0      395 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/schema.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/base.py
+-rw-r--r--   0        0        0     2226 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/boolean.py
+-rw-r--r--   0        0        0     2493 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/date.py
+-rw-r--r--   0        0        0     2929 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/datetime_.py
+-rw-r--r--   0        0        0     1016 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/email.py
+-rw-r--r--   0        0        0     1550 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/float.py
+-rw-r--r--   0        0        0     1256 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/integer.py
+-rw-r--r--   0        0        0     1272 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/ipv4_address.py
+-rw-r--r--   0        0        0      991 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/string.py
+-rw-r--r--   0        0        0     3188 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/unix_timestamp.py
+-rw-r--r--   0        0        0     7381 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types_handler.py
+-rw-r--r--   0        0        0     1848 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/utils.py
+-rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 shmessy-1.3.0/PKG-INFO
```

### Comparing `shmessy-1.2.9/LICENSE` & `shmessy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shmessy-1.2.9/README.md` & `shmessy-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 ### Constructor
 ```python
 shmessy = Shmessy(
     sample_size: Optional[int] = 1000,
     reader_encoding: Optional[str] = "UTF-8",
     locale_formatter: Optional[str] = "en_US",
     use_random_sample: Optional[bool] = True,
-    ignore_virtual_types: Optional[bool] = False,
+    types_to_ignore: Optional[List[str]] = None,
     max_columns_num: Optional[int] = 500
 )
 ```
 
 ### read_csv
 ```python
 shmessy.read_csv(
```

### Comparing `shmessy-1.2.9/pyproject.toml` & `shmessy-1.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shmessy"
-version = "v1.2.9"
+version = "v1.3.0"
 description = "If your data is messy - Use Shmessy!"
 readme = "README.md"
 authors = ["Ohad Mata <ohadmata@gmail.com>"]
 homepage = "https://github.com/ohadmata/shmessy"
 repository = "https://github.com/ohadmata/shmessy"
 packages = [
     { include = "shmessy", from = "src" },
```

### Comparing `shmessy-1.2.9/src/shmessy/__init__.py` & `shmessy-1.3.0/src/shmessy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import csv
 import locale
 import logging
 import time
-from typing import BinaryIO, Optional, TextIO, Union
+from typing import BinaryIO, List, Optional, TextIO, Union
 
 import pandas as pd
 from pandas import DataFrame
 
 from .exceptions import TooManyColumnException, exception_router
 from .schema import ShmessySchema
 from .types_handler import TypesHandler
@@ -24,18 +24,18 @@
 class Shmessy:
     def __init__(
         self,
         sample_size: Optional[int] = 1000,
         reader_encoding: Optional[str] = "UTF-8",
         locale_formatter: Optional[str] = "en_US",
         use_random_sample: Optional[bool] = True,
-        ignore_virtual_types: Optional[bool] = False,
+        types_to_ignore: Optional[List[str]] = None,
         max_columns_num: Optional[int] = 500,
     ) -> None:
-        self.__types_handler = TypesHandler(ignore_virtual_types=ignore_virtual_types)
+        self.__types_handler = TypesHandler(types_to_ignore=types_to_ignore)
         self.__sample_size = sample_size
         self.__reader_encoding = reader_encoding
         self.__locale_formatter = locale_formatter
         self.__use_random_sample = use_random_sample
         self.__max_columns_num = max_columns_num
 
         self.__inferred_schema: Optional[ShmessySchema] = None
```

### Comparing `shmessy-1.2.9/src/shmessy/exceptions.py` & `shmessy-1.3.0/src/shmessy/exceptions.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.2.9/src/shmessy/types/base.py` & `shmessy-1.3.0/src/shmessy/types/base.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.2.9/src/shmessy/types/boolean.py` & `shmessy-1.3.0/src/shmessy/types/boolean.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.2.9/src/shmessy/types/date.py` & `shmessy-1.3.0/src/shmessy/types/date.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         "%d/%m/%Y",  # 01/12/2022
         "%d-%m-%Y",  # 01-12-2022
         "%d.%m.%Y",  # 01.12.2022
         "%d/%b/%Y",  # 01/Mar/2022
         "%d-%b-%Y",  # 01-Mar-2022
         "%Y-%m",  # 2022-07
         "%d %b %Y",  # 13 Jan 2023
+        "%d %b %y",  # 04 Jul 96
     ]
 
     def validate(self, data: ndarray) -> Optional[InferredField]:
         for pattern in self.patterns:
             valid_pattern = True
             at_least_single_not_nan_value = False
             for value in data:
```

### Comparing `shmessy-1.2.9/src/shmessy/types/datetime_.py` & `shmessy-1.3.0/src/shmessy/types/datetime_.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         "%Y-%m-%dT%H:%M:%SZ",  # 2022-12-30T00:00:00Z
         "%Y-%m-%dT%H:%M:%S.%f",  # 2022-12-30T00:00:00.000
         "%Y-%m-%d %H:%M:%S.%fZ",  # 2022-12-30 00:00:00.000Z
         "%Y-%m-%d %H:%M:%S.%f",  # 2022-12-30 00:00:00.000
         "%Y-%m-%dT%H:%M:%S.%fZ",  # 2022-12-30T00:00:00.000Z
         "%Y-%m-%dT%H:%M:%S",  # 2022-12-30T00:00:00
         "%d/%m/%Y %H:%M",  # 30/12/2022 00:00
+        "%Y-%m-%d %H:%M:%S %Z",  # 2020-09-24 11:57:27 UTC
     ]
 
     def validate(self, data: ndarray) -> Optional[InferredField]:
         if data.dtype.type == np.dtype("datetime64"):
             return InferredField(inferred_type=self.name)
 
         for pattern in self.patterns:
```

### Comparing `shmessy-1.2.9/src/shmessy/types/email.py` & `shmessy-1.3.0/src/shmessy/types/email.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.2.9/src/shmessy/types/float.py` & `shmessy-1.3.0/src/shmessy/types/integer.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from ..schema import InferredField
 from .base import BaseType
 
 logger = logging.getLogger(__name__)
 
 
-class FloatType(BaseType):
-    weight = 8
+class IntegerType(BaseType):
+    weight = 7
 
     def validate(self, data: ndarray) -> Optional[InferredField]:
         for value in data:
             try:
                 self.cast_value(value)
             except Exception:  # noqa
                 logger.debug(f"Cannot cast the value '{value}' to {self.name}")
@@ -28,16 +28,16 @@
     @property
     def prefer_column_casting(self) -> bool:
         return True
 
     def cast_column(self, column: Series, inferred_field: InferredField) -> Series:
         if is_numeric_dtype(column):
             return column
-        return to_numeric(column.apply(locale.atof))
+        return to_numeric(column.apply(locale.atoi))
 
     def cast_value(self, value: Any, pattern: Optional[Any] = None) -> Optional[Any]:
         if isinstance(value, str):
-            return float(locale.atof(value))
-        return float(value)
+            return int(locale.atoi(value))
+        return int(value)
 
     def ignore_cast_for_types(self) -> Tuple[Any]:
-        return (np.dtype("float64"),)
+        return (np.dtype("int64"),)
```

### Comparing `shmessy-1.2.9/src/shmessy/types/integer.py` & `shmessy-1.3.0/src/shmessy/types/ipv4_address.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-import locale
 import logging
 from typing import Any, Optional, Tuple
 
 import numpy as np
 from numpy import ndarray
-from pandas import Series, to_numeric
-from pandas.api.types import is_numeric_dtype
+from pandas import Series
+from pydantic import BaseModel
+from pydantic.networks import IPv4Address  # noqa
 
 from ..schema import InferredField
 from .base import BaseType
 
 logger = logging.getLogger(__name__)
 
 
-class IntegerType(BaseType):
-    weight = 7
+class Model(BaseModel):
+    ip: IPv4Address
+
+
+class IPv4Type(BaseType):
+    weight = 6
 
     def validate(self, data: ndarray) -> Optional[InferredField]:
         for value in data:
             try:
-                self.cast_value(value)
-            except Exception:  # noqa
+                if not isinstance(value, str):
+                    logger.debug(
+                        f"Value '{value}' is not string, cannot cast to {self.name}"
+                    )
+                    return None
+                Model(ip=value)
+            except ValueError:
                 logger.debug(f"Cannot cast the value '{value}' to {self.name}")
                 return None
         return InferredField(inferred_type=self.name)
 
-    @property
-    def prefer_column_casting(self) -> bool:
-        return True
-
     def cast_column(self, column: Series, inferred_field: InferredField) -> Series:
-        if is_numeric_dtype(column):
-            return column
-        return to_numeric(column.apply(locale.atoi))
+        raise NotImplementedError()
 
     def cast_value(self, value: Any, pattern: Optional[Any] = None) -> Optional[Any]:
-        if isinstance(value, str):
-            return int(locale.atoi(value))
-        return int(value)
+        return str(value)
 
     def ignore_cast_for_types(self) -> Tuple[Any]:
-        return (np.dtype("int64"),)
+        return (np.dtype("O"),)
```

### Comparing `shmessy-1.2.9/src/shmessy/types/ipv4_address.py` & `shmessy-1.3.0/src/shmessy/types/float.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,49 @@
+import locale
 import logging
 from typing import Any, Optional, Tuple
 
 import numpy as np
 from numpy import ndarray
-from pandas import Series
-from pydantic import BaseModel
-from pydantic.networks import IPv4Address  # noqa
+from pandas import Series, to_numeric
+from pandas.api.types import is_numeric_dtype
 
 from ..schema import InferredField
 from .base import BaseType
 
 logger = logging.getLogger(__name__)
 
 
-class Model(BaseModel):
-    ip: IPv4Address
-
-
-class IPv4Type(BaseType):
-    weight = 6
+class FloatType(BaseType):
+    weight = 8
 
     def validate(self, data: ndarray) -> Optional[InferredField]:
+        at_least_single_not_empty_value: bool = False
         for value in data:
             try:
-                if not isinstance(value, str):
-                    logger.debug(
-                        f"Value '{value}' is not string, cannot cast to {self.name}"
-                    )
-                    return None
-                Model(ip=value)
-            except ValueError:
+                self.cast_value(value)
+                if not at_least_single_not_empty_value and not self.is_empty_value(
+                    value
+                ):
+                    at_least_single_not_empty_value = True
+            except Exception:  # noqa
                 logger.debug(f"Cannot cast the value '{value}' to {self.name}")
                 return None
-        return InferredField(inferred_type=self.name)
+        if at_least_single_not_empty_value:
+            return InferredField(inferred_type=self.name)
+
+    @property
+    def prefer_column_casting(self) -> bool:
+        return True
 
     def cast_column(self, column: Series, inferred_field: InferredField) -> Series:
-        raise NotImplementedError()
+        if is_numeric_dtype(column):
+            return column
+        return to_numeric(column.apply(locale.atof))
 
     def cast_value(self, value: Any, pattern: Optional[Any] = None) -> Optional[Any]:
-        return str(value)
+        if isinstance(value, str):
+            return float(locale.atof(value))
+        return float(value)
 
     def ignore_cast_for_types(self) -> Tuple[Any]:
-        return (np.dtype("O"),)
+        return (np.dtype("float64"),)
```

### Comparing `shmessy-1.2.9/src/shmessy/types/string.py` & `shmessy-1.3.0/src/shmessy/types/string.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 from typing import Any, Optional, Tuple
 
-import numpy as np
 from numpy import ndarray
 from pandas import Series
 
 from ..schema import InferredField
 from .base import BaseType
 
 logger = logging.getLogger(__name__)
@@ -24,14 +23,14 @@
         return InferredField(inferred_type=self.name)
 
     @property
     def prefer_column_casting(self) -> bool:
         return True
 
     def cast_column(self, column: Series, inferred_field: InferredField) -> Series:
-        raise column.apply(lambda x: str(x))
+        return column.apply(lambda x: str(x))
 
     def cast_value(self, value: Any, pattern: Optional[Any] = None) -> Optional[Any]:
         return str(value)
 
     def ignore_cast_for_types(self) -> Tuple[Any]:
-        return (np.dtype("O"),)
+        return tuple()
```

### Comparing `shmessy-1.2.9/src/shmessy/types/unix_timestamp.py` & `shmessy-1.3.0/src/shmessy/types/unix_timestamp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from datetime import datetime
+from datetime import datetime, time
 from enum import Enum
 from typing import Any, Optional, Tuple
 
 import numpy as np
 from numpy import ndarray
 from pandas import Series, to_datetime
 
@@ -47,15 +47,15 @@
         if selected_resolution == TimestampResolution.NANOSECONDS:
             return int(int(value) / 1000 / 1000)
 
     def _is_valid_unix_timestamp(self, value: Any) -> bool:
         if self.is_empty_value(value):
             return True
 
-        if self.is_empty_value(value) or isinstance(value, datetime):
+        if self.is_empty_value(value) or isinstance(value, (datetime, time)):
             return False
 
         if not self.resolution:
             self.resolution = self._unix_timestamp_resolution(int(value))
 
         if self.resolution:
             parsed_value = datetime.utcfromtimestamp(
```

### Comparing `shmessy-1.2.9/src/shmessy/types_handler.py` & `shmessy-1.3.0/src/shmessy/types_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type
 
-from numpy import ndarray
+from numpy import nan, ndarray
 from numpy.dtypes import (
     BoolDType,
     DateTime64DType,
     Float16DType,
     Float32DType,
     Float64DType,
     Int8DType,
@@ -35,42 +35,48 @@
 logger = logging.getLogger(__name__)
 
 
 class TypesHandler:
     PACKAGE_NAME: str = "shmessy"
     TYPES_DIR: str = "types"
 
-    def __init__(self, ignore_virtual_types: bool):
-        self.__types = self._discover_types(ignore_virtual_types=ignore_virtual_types)
+    def __init__(self, types_to_ignore: List[str]):
+        self.__types = self._discover_types(types_to_ignore=types_to_ignore)
         self.__types_as_dict: Dict[str, BaseType] = self._types_as_dict(self.__types)
 
     @classmethod
     def _types_as_dict(cls, __types: List[BaseType]) -> Dict[str, BaseType]:
         res = {}
         for type_ in __types:
             res[type_.name] = type_
         return res
 
     @classmethod
-    def _discover_types(cls, ignore_virtual_types: bool) -> List[BaseType]:
+    def _discover_types(cls, types_to_ignore: List[str]) -> List[BaseType]:
+        filtered_types = []
+        types_to_ignore = (
+            [x.lower() for x in types_to_ignore] if types_to_ignore else []
+        )
         types = [
             BooleanType(),
             DatetimeType(),
             DateType(),
             FloatType(),
             IntegerType(),
             StringType(),
             UnixTimestampType(),
+            IPv4Type(),
+            EmailType(),
         ]
-        if not ignore_virtual_types:
-            types += [
-                IPv4Type(),
-                EmailType(),
-            ]
-        return sorted(types, key=lambda x: x.weight)
+
+        for _type in types:
+            if _type.name.lower() not in types_to_ignore:
+                filtered_types.append(_type)
+
+        return sorted(filtered_types, key=lambda x: x.weight)
 
     @staticmethod
     def _extract_bad_value(column: Series, func: Callable) -> Tuple[int, Any]:
         for idx, row in enumerate(column):
             try:
                 func(row)  # noqa
             except Exception:  # noqa
@@ -83,34 +89,52 @@
     def _cast_with_fallback_to_null(
         value: Any, inferred_pattern: Any, type_: BaseType
     ) -> Any:
         try:
             return type_.cast_value(value, inferred_pattern)
         except Exception as e:
             logger.debug(e)
-            return None
+            return nan
 
     def _fix_column(
         self,
         column: Series,
         inferred_field: InferredField,
         type_: BaseType,
         fallback_to_null: Optional[bool] = False,
     ) -> Series:
         try:
             if column.dtype.type in type_.ignore_cast_for_types():
                 return column
+            if type_.prefer_column_casting:
+                try:
+                    return type_.cast_column(column, inferred_field)
+                except Exception as e:  # noqa
+                    logger.debug(f"Cannot cast column to type: {type_}. Error: {e}")
+
+                    if fallback_to_null:
+                        logger.debug(
+                            f"Trying to cast column to type: {type_} using FallbackToNull"
+                        )
+                        return column.apply(
+                            lambda x: self._cast_with_fallback_to_null(
+                                x, inferred_field.inferred_pattern, type_
+                            )
+                        )
+
             if fallback_to_null:
+                logger.debug(
+                    f"Trying to cast column to type: {type_} using FallbackToNull"
+                )
                 return column.apply(
                     lambda x: self._cast_with_fallback_to_null(
                         x, inferred_field.inferred_pattern, type_
                     )
                 )
-            if type_.prefer_column_casting:
-                return type_.cast_column(column, inferred_field)
+
             return column.apply(
                 lambda x: type_.cast_value(x, inferred_field.inferred_pattern)
             )
         except Exception as e:
             logger.debug(f"Couldn't cast column to type {type_.name}: {e}")
             try:
                 line_number, bad_value = self._extract_bad_value(
```

### Comparing `shmessy-1.2.9/src/shmessy/utils.py` & `shmessy-1.3.0/src/shmessy/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,11 +47,13 @@
     # sample = "".join(filepath_or_buffer.readlines(sample_size))
     # There is an issue with readlines(x) that reads the whole data instead of X first rows
 
     sample = ""
     for idx, line in enumerate(filepath_or_buffer):
         if idx > sample_size:
             break
+        if not isinstance(line, str):
+            line = line.decode(encoding)  # noqa
         sample += line
 
     filepath_or_buffer.seek(0)
     return sample
```

### Comparing `shmessy-1.2.9/PKG-INFO` & `shmessy-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shmessy
-Version: 1.2.9
+Version: 1.3.0
 Summary: If your data is messy - Use Shmessy!
 Home-page: https://github.com/ohadmata/shmessy
 Author: Ohad Mata
 Author-email: ohadmata@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -143,15 +143,15 @@
 ### Constructor
 ```python
 shmessy = Shmessy(
     sample_size: Optional[int] = 1000,
     reader_encoding: Optional[str] = "UTF-8",
     locale_formatter: Optional[str] = "en_US",
     use_random_sample: Optional[bool] = True,
-    ignore_virtual_types: Optional[bool] = False,
+    types_to_ignore: Optional[List[str]] = None,
     max_columns_num: Optional[int] = 500
 )
 ```
 
 ### read_csv
 ```python
 shmessy.read_csv(
```

