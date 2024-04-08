# Comparing `tmp/pycountries-1.0.0.tar.gz` & `tmp/pycountries-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycountries-1.0.0.tar", last modified: Wed Mar 27 19:57:49 2024, max compression
+gzip compressed data, was "pycountries-1.0.1.tar", last modified: Mon Apr  8 19:24:14 2024, max compression
```

## Comparing `pycountries-1.0.0.tar` & `pycountries-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:57:49.533182 pycountries-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-27 19:57:38.000000 pycountries-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-03-27 19:57:49.533182 pycountries-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-03-27 19:57:38.000000 pycountries-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-27 19:57:38.000000 pycountries-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:57:49.533182 pycountries-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-27 19:57:38.000000 pycountries-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:57:49.529182 pycountries-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:57:49.529182 pycountries-1.0.0/src/pycountries/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-27 19:57:38.000000 pycountries-1.0.0/src/pycountries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-27 19:57:38.000000 pycountries-1.0.0/src/pycountries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    47277 2024-03-27 19:57:38.000000 pycountries-1.0.0/src/pycountries/countries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30868 2024-03-27 19:57:38.000000 pycountries-1.0.0/src/pycountries/currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    83977 2024-03-27 19:57:38.000000 pycountries-1.0.0/src/pycountries/languages.py
--rw-r--r--   0 runner    (1001) docker     (127)    42776 2024-03-27 19:57:38.000000 pycountries-1.0.0/src/pycountries/phones.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:57:49.533182 pycountries-1.0.0/src/pycountries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-03-27 19:57:49.000000 pycountries-1.0.0/src/pycountries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-27 19:57:49.000000 pycountries-1.0.0/src/pycountries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:57:49.000000 pycountries-1.0.0/src/pycountries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-27 19:57:49.000000 pycountries-1.0.0/src/pycountries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-27 19:57:49.000000 pycountries-1.0.0/src/pycountries.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:57:49.533182 pycountries-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-27 19:57:38.000000 pycountries-1.0.0/tests/test_currencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:24:14.642955 pycountries-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 19:24:06.000000 pycountries-1.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-08 19:24:14.642955 pycountries-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-08 19:24:06.000000 pycountries-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-08 19:24:06.000000 pycountries-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:24:14.642955 pycountries-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 19:24:06.000000 pycountries-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:24:14.638955 pycountries-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:24:14.642955 pycountries-1.0.1/src/pycountries/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47277 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/countries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30868 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85082 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43057 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/phones.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:24:14.642955 pycountries-1.0.1/src/pycountries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-08 19:24:14.000000 pycountries-1.0.1/src/pycountries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-08 19:24:14.000000 pycountries-1.0.1/src/pycountries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:24:14.000000 pycountries-1.0.1/src/pycountries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 19:24:14.000000 pycountries-1.0.1/src/pycountries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 19:24:14.000000 pycountries-1.0.1/src/pycountries.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:24:14.642955 pycountries-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-08 19:24:06.000000 pycountries-1.0.1/tests/test_currencies.py
```

### Comparing `pycountries-1.0.0/LICENSE.md` & `pycountries-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.0/PKG-INFO` & `pycountries-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycountries
-Version: 1.0.0
+Version: 1.0.1
 Summary: List of existing countries and currencies
 Author-email: Ivan Koldakov <ivan@koldakov.com>
 Project-URL: Homepage, https://github.com/koldakov/pycountries
 Project-URL: Issues, https://github.com/koldakov/pycountries/issues
 Keywords: pydantic,fastapi,countries,currencies
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pycountries-1.0.0/README.md` & `pycountries-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.0/pyproject.toml` & `pycountries-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pycountries"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Ivan Koldakov", email="ivan@koldakov.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `pycountries-1.0.0/src/pycountries/__init__.py` & `pycountries-1.0.1/src/pycountries/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     WrongAmountDigitsNumberError,
     WrongAmountTypeError,
     ZeroAmountNotAllowedError,
 )
 from pycountries.languages import Language
 from pycountries.phones import Phone
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __author__ = "Ivan Koldakov"
 __all__ = [
     "AmountSpecialValuesNotAllowedError",
     "Country",
     "Currency",
     "Language",
     "NegativeAmountNotAllowedError",
```

### Comparing `pycountries-1.0.0/src/pycountries/_base.py` & `pycountries-1.0.1/src/pycountries/_base.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.0/src/pycountries/countries.py` & `pycountries-1.0.1/src/pycountries/countries.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.0/src/pycountries/currencies.py` & `pycountries-1.0.1/src/pycountries/currencies.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.0/src/pycountries/languages.py` & `pycountries-1.0.1/src/pycountries/languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,69 +1,103 @@
+from __future__ import annotations
+
+import sys
 from enum import Enum
 
 from pydantic import BaseModel, Field
 
 from pycountries._base import EnumTypeBase
 
 
-class LanguageUnit(BaseModel):
+class LanguageUnitBase(BaseModel):
     name: str = Field(
         description="Official Language name.",
         examples=[
             "English",
             "French",
             "Russian",
         ],
     )
-    alpha_2: str | None = Field(
-        default=None,
-        min_length=2,
-        max_length=2,
-        description="ISO 639-2 two-letter code to represent language.",
-        examples=[
-            "en",
-            "ru",
-        ],
-    )
     alpha_3: str = Field(
         min_length=3,
         max_length=3,
         description="ISO 639-2 three-letter code to represent language.",
         examples=[
             "eng",
             "fra",
             "rus",
         ],
     )
-    bibliographic: str | None = Field(
-        min_length=3,
-        max_length=3,
-        description="ISO 639-2 code designated specifically for bibliographic or library cataloging purposes. "
-        "Bibliographic code is used primarily in library systems and databases to categorize and "
-        "organize resources by language.",
-        examples=[
-            None,
-            "fre",
-            None,
-        ],
-    )
     terminology: str = Field(
         min_length=3,
         max_length=3,
         description="ISO 639-2 code refers to specific language code designated for terminology or "
         "specialized vocabulary purposes.",
         examples=[
             "eng",
             "fra",
             "rus",
         ],
     )
 
 
-def _get_compare_list(language: "Language") -> list[str]:
+if sys.version_info >= (3, 10):  # noqa: UP036
+
+    class LanguageUnit(LanguageUnitBase):
+        alpha_2: str | None = Field(
+            default=None,
+            min_length=2,
+            max_length=2,
+            description="ISO 639-2 two-letter code to represent language.",
+            examples=[
+                "en",
+                "ru",
+            ],
+        )
+        bibliographic: str | None = Field(
+            min_length=3,
+            max_length=3,
+            description="ISO 639-2 code designated specifically for bibliographic or library cataloging purposes. "
+            "Bibliographic code is used primarily in library systems and databases to categorize and "
+            "organize resources by language.",
+            examples=[
+                None,
+                "fre",
+                None,
+            ],
+        )
+else:
+    from typing import Optional
+
+    class LanguageUnit(LanguageUnitBase):
+        alpha_2: Optional[str] = Field(  # noqa: UP007
+            default=None,
+            min_length=2,
+            max_length=2,
+            description="ISO 639-2 two-letter code to represent language.",
+            examples=[
+                "en",
+                "ru",
+            ],
+        )
+        bibliographic: Optional[str] = Field(  # noqa: UP007
+            min_length=3,
+            max_length=3,
+            description="ISO 639-2 code designated specifically for bibliographic or library cataloging purposes. "
+            "Bibliographic code is used primarily in library systems and databases to categorize and "
+            "organize resources by language.",
+            examples=[
+                None,
+                "fre",
+                None,
+            ],
+        )
+
+
+def _get_compare_list(language: Language) -> list[str]:
     compare_list: list[str] = [
         language.alpha_3,
     ]
     if language.alpha_2 is not None:
         compare_list.append(language.alpha_2)
 
     return compare_list
```

### Comparing `pycountries-1.0.0/src/pycountries/phones.py` & `pycountries-1.0.1/src/pycountries/phones.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 from __future__ import annotations
 
+import sys
 from enum import Enum
 from functools import singledispatchmethod
 from typing import TYPE_CHECKING
 
 from pydantic import BaseModel, Field
 
 from pycountries._base import EnumTypeBase
 from pycountries.countries import Country
 
 if TYPE_CHECKING:
     from types import MappingProxyType
 
 
-class PhoneUnit(BaseModel):
+class PhoneUnitBase(BaseModel):
     country: Country
     calling_code: int = Field(
         description="International calling code",
     )
-    prefixes: list[int]
+    # prefixes: list[int]  # Abstract property
 
     def is_prefix_supported(self, prefix: int, /) -> bool:
         if not self.prefixes or prefix is None:
             return True
         return prefix in self.prefixes
 
 
+if sys.version_info >= (3, 10):  # noqa: UP036
+
+    class PhoneUnit(PhoneUnitBase):
+        prefixes: list[int]
+else:
+    from typing import List  # noqa: UP035
+
+    class PhoneUnit(PhoneUnitBase):
+        prefixes: List[int]  # noqa: UP006
+
+
 class _PhoneUnitNotFoundError(Exception):
     """Phone Unit Not Found Error"""
 
 
 class _PhoneEnumType(EnumTypeBase):
     @singledispatchmethod
     def _normalize_value(cls, value: str | int, /) -> int:  # noqa: N805
```

### Comparing `pycountries-1.0.0/src/pycountries.egg-info/PKG-INFO` & `pycountries-1.0.1/src/pycountries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycountries
-Version: 1.0.0
+Version: 1.0.1
 Summary: List of existing countries and currencies
 Author-email: Ivan Koldakov <ivan@koldakov.com>
 Project-URL: Homepage, https://github.com/koldakov/pycountries
 Project-URL: Issues, https://github.com/koldakov/pycountries/issues
 Keywords: pydantic,fastapi,countries,currencies
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pycountries-1.0.0/tests/test_currencies.py` & `pycountries-1.0.1/tests/test_currencies.py`

 * *Files identical despite different names*

