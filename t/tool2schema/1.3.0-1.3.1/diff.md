# Comparing `tmp/tool2schema-1.3.0.tar.gz` & `tmp/tool2schema-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool2schema-1.3.0.tar", max compression
+gzip compressed data, was "tool2schema-1.3.1.tar", max compression
```

## Comparing `tool2schema-1.3.0.tar` & `tool2schema-1.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11338 2024-03-25 16:36:49.668442 tool2schema-1.3.0/LICENSE
--rw-r--r--   0        0        0     6688 2024-03-25 16:36:49.668442 tool2schema-1.3.0/README.md
--rw-r--r--   0        0        0      734 2024-03-25 16:37:05.740627 tool2schema-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      310 2024-03-25 16:37:05.736627 tool2schema-1.3.0/tool2schema/__init__.py
--rw-r--r--   0        0        0     2986 2024-03-25 16:36:49.668442 tool2schema-1.3.0/tool2schema/config.py
--rw-r--r--   0        0        0     3865 2024-03-25 16:36:49.668442 tool2schema-1.3.0/tool2schema/parameter_schema.py
--rw-r--r--   0        0        0    12906 2024-03-25 16:36:49.668442 tool2schema-1.3.0/tool2schema/schema.py
--rw-r--r--   0        0        0     9311 2024-03-25 16:36:49.668442 tool2schema-1.3.0/tool2schema/type_schema.py
--rw-r--r--   0        0        0     7421 1970-01-01 00:00:00.000000 tool2schema-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-04-08 18:08:45.965268 tool2schema-1.3.1/LICENSE
+-rw-r--r--   0        0        0     6780 2024-04-08 18:08:45.965268 tool2schema-1.3.1/README.md
+-rw-r--r--   0        0        0      734 2024-04-08 18:09:22.897307 tool2schema-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-04-08 18:09:22.897307 tool2schema-1.3.1/tool2schema/__init__.py
+-rw-r--r--   0        0        0     2986 2024-04-08 18:08:45.969268 tool2schema-1.3.1/tool2schema/config.py
+-rw-r--r--   0        0        0     3865 2024-04-08 18:08:45.969268 tool2schema-1.3.1/tool2schema/parameter_schema.py
+-rw-r--r--   0        0        0    12911 2024-04-08 18:08:45.969268 tool2schema-1.3.1/tool2schema/schema.py
+-rw-r--r--   0        0        0     9311 2024-04-08 18:08:45.969268 tool2schema-1.3.1/tool2schema/type_schema.py
+-rw-r--r--   0        0        0     7513 1970-01-01 00:00:00.000000 tool2schema-1.3.1/PKG-INFO
```

### Comparing `tool2schema-1.3.0/LICENSE` & `tool2schema-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tool2schema-1.3.0/README.md` & `tool2schema-1.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # tool2schema
 
 [![Check Code](https://github.com/cadifyai/tool2schema/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/cadifyai/tool2schema/actions/workflows/python-package.yml)
+[![Downloads](https://static.pepy.tech/badge/tool2schema)](https://pepy.tech/project/tool2schema)
 
 A library to convert Python functions to schemas supported by the OpenAI API.
 
 Inspired by [janekb04/py2gpt](https://github.com/janekb04/py2gpt) and [fastai/lm-hackers](https://github.com/fastai/lm-hackers).
 
 ## Why tool2schema?
 
@@ -110,15 +111,15 @@
 - `bool`
 - `list`
 
 Any other parameter types will be listed as `object` in the schema.
 
 ### Enumerations
 
-If you want to limit the possible values of a parameter, you can use a `typing.Literal` type hint or a 
+If you want to limit the possible values of a parameter, you can use a `typing.Literal` type hint or a
 subclass of `enum.Enum`. For example, using `typing.Literal`:
 
 ```python
 import typing
 
 
 @GPTEnabled
@@ -150,20 +151,20 @@
     :param a: First parameter
     :param b: Second parameter
     """
     # Function code here...
 ```
 
 In the case of `Enum` subclasses, note that the schema will include the enumeration names rather than the values.
-In the example above, the schema will include `["YES", "NO"]` rather than `[0, 1]`. 
+In the example above, the schema will include `["YES", "NO"]` rather than `[0, 1]`.
 
-The `@GPTEnabled` decorator also allows to invoke the function using the name of the enum member rather than an 
+The `@GPTEnabled` decorator also allows to invoke the function using the name of the enum member rather than an
 instance of the class. For example, you may invoke `my_function(1, MyEnum.YES)` as `my_function(1, "YES")`.
 
-If the enumeration values are not known at the time of defining the function, 
+If the enumeration values are not known at the time of defining the function,
 you can add them later using the `add_enum` method.
 
 ```python
 @GPTEnabled
 def my_function(a: int, b: str,):
     """
     Example function description.
@@ -214,17 +215,17 @@
 def my_function(a: int, b: str, c: float):
     # Function code here...
 ```
 
 The available settings are:
 - `ignore_parameters`: A list of parameter names to exclude from the schema (defaults to `[]`).
 - `ignore_all_parameters`: A boolean value indicating whether to exclude all parameters from the schema
-  (defaults to `False`). When set to true, all other parameter-related settings (`ignore_parameters` and 
+  (defaults to `False`). When set to true, all other parameter-related settings (`ignore_parameters` and
   `ignore_parameter_descriptions`) will be ignored.
-- `ignore_function_description`: A boolean value indicating whether to exclude the function description from 
+- `ignore_function_description`: A boolean value indicating whether to exclude the function description from
   the schema (defaults to `False`).
 - `ignore_parameter_descriptions`: A boolean value indicating whether to exclude all parameter descriptions
   from the schema (defaults to `False`).
 
 It is also possible to specify the settings globally, so that they apply to all functions
 unless explicitly overridden. It can be done by editing the global configuration as follows:
```

### Comparing `tool2schema-1.3.0/pyproject.toml` & `tool2schema-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 line_length = 100
 
 [tool.coverage.run]
 source = ["tool2schema"]
 
 [tool.poetry]
 name = "tool2schema"
-version = "v1.3.0"
+version = "v1.3.1"
 description = "A library to generate function schemas for use in the OpenAI API."
 authors = ["Angus Stewart <siliconlad@protonmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository="https://github.com/cadifyai/tool2schema"
 keywords=["openai", "llm"]
```

### Comparing `tool2schema-1.3.0/tool2schema/config.py` & `tool2schema-1.3.1/tool2schema/config.py`

 * *Files identical despite different names*

### Comparing `tool2schema-1.3.0/tool2schema/parameter_schema.py` & `tool2schema-1.3.1/tool2schema/parameter_schema.py`

 * *Files identical despite different names*

### Comparing `tool2schema-1.3.0/tool2schema/schema.py` & `tool2schema-1.3.1/tool2schema/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import functools
 import inspect
 import json
 import re
 from enum import Enum
 from inspect import Parameter
 from types import ModuleType
-from typing import Callable, Optional
+from typing import Any, Callable, Optional
 
 import tool2schema
 from tool2schema.config import Config
 from tool2schema.parameter_schema import ParameterSchema
 
 
 class SchemaType(Enum):
@@ -83,15 +83,15 @@
 
 
 def LoadGPTEnabled(
     module: ModuleType,
     function: dict,
     validate: bool = True,
     ignore_hallucinations: bool = True,
-) -> Optional[tuple[Callable, dict]]:
+) -> tuple[Callable, dict[str, Any]]:
     """
     Given a function dictionary containing the name of a function and the arguments to pass to it,
     retrieve the corresponding function among those with the `GPTEnabled` decorator defined in
     `module`. When `validate` is true, validate the arguments and raise `ParseException` if the
     arguments are not valid (see more information below).
 
     :param module: The module where the function is defined
```

### Comparing `tool2schema-1.3.0/tool2schema/type_schema.py` & `tool2schema-1.3.1/tool2schema/type_schema.py`

 * *Files identical despite different names*

### Comparing `tool2schema-1.3.0/PKG-INFO` & `tool2schema-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tool2schema
-Version: 1.3.0
+Version: 1.3.1
 Summary: A library to generate function schemas for use in the OpenAI API.
 Home-page: https://github.com/cadifyai/tool2schema
 License: Apache-2.0
 Keywords: openai,llm
 Author: Angus Stewart
 Author-email: siliconlad@protonmail.com
 Requires-Python: >=3.9,<4.0
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/cadifyai/tool2schema
 Description-Content-Type: text/markdown
 
 # tool2schema
 
 [![Check Code](https://github.com/cadifyai/tool2schema/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/cadifyai/tool2schema/actions/workflows/python-package.yml)
+[![Downloads](https://static.pepy.tech/badge/tool2schema)](https://pepy.tech/project/tool2schema)
 
 A library to convert Python functions to schemas supported by the OpenAI API.
 
 Inspired by [janekb04/py2gpt](https://github.com/janekb04/py2gpt) and [fastai/lm-hackers](https://github.com/fastai/lm-hackers).
 
 ## Why tool2schema?
 
@@ -129,15 +130,15 @@
 - `bool`
 - `list`
 
 Any other parameter types will be listed as `object` in the schema.
 
 ### Enumerations
 
-If you want to limit the possible values of a parameter, you can use a `typing.Literal` type hint or a 
+If you want to limit the possible values of a parameter, you can use a `typing.Literal` type hint or a
 subclass of `enum.Enum`. For example, using `typing.Literal`:
 
 ```python
 import typing
 
 
 @GPTEnabled
@@ -169,20 +170,20 @@
     :param a: First parameter
     :param b: Second parameter
     """
     # Function code here...
 ```
 
 In the case of `Enum` subclasses, note that the schema will include the enumeration names rather than the values.
-In the example above, the schema will include `["YES", "NO"]` rather than `[0, 1]`. 
+In the example above, the schema will include `["YES", "NO"]` rather than `[0, 1]`.
 
-The `@GPTEnabled` decorator also allows to invoke the function using the name of the enum member rather than an 
+The `@GPTEnabled` decorator also allows to invoke the function using the name of the enum member rather than an
 instance of the class. For example, you may invoke `my_function(1, MyEnum.YES)` as `my_function(1, "YES")`.
 
-If the enumeration values are not known at the time of defining the function, 
+If the enumeration values are not known at the time of defining the function,
 you can add them later using the `add_enum` method.
 
 ```python
 @GPTEnabled
 def my_function(a: int, b: str,):
     """
     Example function description.
@@ -233,17 +234,17 @@
 def my_function(a: int, b: str, c: float):
     # Function code here...
 ```
 
 The available settings are:
 - `ignore_parameters`: A list of parameter names to exclude from the schema (defaults to `[]`).
 - `ignore_all_parameters`: A boolean value indicating whether to exclude all parameters from the schema
-  (defaults to `False`). When set to true, all other parameter-related settings (`ignore_parameters` and 
+  (defaults to `False`). When set to true, all other parameter-related settings (`ignore_parameters` and
   `ignore_parameter_descriptions`) will be ignored.
-- `ignore_function_description`: A boolean value indicating whether to exclude the function description from 
+- `ignore_function_description`: A boolean value indicating whether to exclude the function description from
   the schema (defaults to `False`).
 - `ignore_parameter_descriptions`: A boolean value indicating whether to exclude all parameter descriptions
   from the schema (defaults to `False`).
 
 It is also possible to specify the settings globally, so that they apply to all functions
 unless explicitly overridden. It can be done by editing the global configuration as follows:
```

