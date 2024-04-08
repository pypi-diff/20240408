# Comparing `tmp/sgen-1.0.1.tar.gz` & `tmp/sgen-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgen-1.0.1.tar", last modified: Mon Jan  8 17:54:10 2024, max compression
+gzip compressed data, was "sgen-1.0.2.tar", last modified: Mon Apr  8 08:25:53 2024, max compression
```

## Comparing `sgen-1.0.1.tar` & `sgen-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 verner     (501) staff       (20)        0 2024-01-08 17:54:10.855218 sgen-1.0.1/
--rw-r--r--   0 verner     (501) staff       (20)     2339 2024-01-08 17:54:10.854689 sgen-1.0.1/PKG-INFO
--rw-r--r--   0 verner     (501) staff       (20)     1576 2024-01-08 17:32:05.000000 sgen-1.0.1/README.rst
--rw-r--r--   0 verner     (501) staff       (20)       86 2024-01-08 17:10:48.000000 sgen-1.0.1/pyproject.toml
--rw-r--r--   0 verner     (501) staff       (20)       38 2024-01-08 17:54:10.855381 sgen-1.0.1/setup.cfg
--rw-r--r--   0 verner     (501) staff       (20)     1664 2024-01-08 17:32:32.000000 sgen-1.0.1/setup.py
-drwxr-xr-x   0 verner     (501) staff       (20)        0 2024-01-08 17:54:10.822946 sgen-1.0.1/src/
-drwxr-xr-x   0 verner     (501) staff       (20)        0 2024-01-08 17:54:10.830711 sgen-1.0.1/src/sgen/
--rw-r--r--   0 verner     (501) staff       (20)      266 2024-01-08 17:47:41.000000 sgen-1.0.1/src/sgen/__init__.py
--rw-r--r--   0 verner     (501) staff       (20)      485 2024-01-06 23:07:56.000000 sgen-1.0.1/src/sgen/base.py
--rw-r--r--   0 verner     (501) staff       (20)      199 2024-01-08 17:03:22.000000 sgen-1.0.1/src/sgen/dto.py
--rw-r--r--   0 verner     (501) staff       (20)    13603 2024-01-08 17:03:00.000000 sgen-1.0.1/src/sgen/fields.py
--rw-r--r--   0 verner     (501) staff       (20)     2675 2024-01-08 17:03:00.000000 sgen-1.0.1/src/sgen/sgen.py
--rw-r--r--   0 verner     (501) staff       (20)      780 2024-01-08 14:36:26.000000 sgen-1.0.1/src/sgen/utils.py
--rw-r--r--   0 verner     (501) staff       (20)     7642 2024-01-08 17:46:22.000000 sgen-1.0.1/src/sgen/validate.py
-drwxr-xr-x   0 verner     (501) staff       (20)        0 2024-01-08 17:54:10.853316 sgen-1.0.1/src/sgen.egg-info/
--rw-r--r--   0 verner     (501) staff       (20)     2339 2024-01-08 17:54:10.000000 sgen-1.0.1/src/sgen.egg-info/PKG-INFO
--rw-r--r--   0 verner     (501) staff       (20)      843 2024-01-08 17:54:10.000000 sgen-1.0.1/src/sgen.egg-info/SOURCES.txt
--rw-r--r--   0 verner     (501) staff       (20)        1 2024-01-08 17:54:10.000000 sgen-1.0.1/src/sgen.egg-info/dependency_links.txt
--rw-r--r--   0 verner     (501) staff       (20)        1 2024-01-08 17:34:57.000000 sgen-1.0.1/src/sgen.egg-info/not-zip-safe
--rw-r--r--   0 verner     (501) staff       (20)       93 2024-01-08 17:54:10.000000 sgen-1.0.1/src/sgen.egg-info/requires.txt
--rw-r--r--   0 verner     (501) staff       (20)        5 2024-01-08 17:54:10.000000 sgen-1.0.1/src/sgen.egg-info/top_level.txt
-drwxr-xr-x   0 verner     (501) staff       (20)        0 2024-01-08 17:54:10.851680 sgen-1.0.1/tests/
--rw-r--r--   0 verner     (501) staff       (20)     3052 2024-01-06 13:55:59.000000 sgen-1.0.1/tests/test_boolean_negative.py
--rw-r--r--   0 verner     (501) staff       (20)     3354 2024-01-06 13:55:59.000000 sgen-1.0.1/tests/test_boolean_positive.py
--rw-r--r--   0 verner     (501) staff       (20)     4139 2024-01-06 13:32:15.000000 sgen-1.0.1/tests/test_collection_negative.py
--rw-r--r--   0 verner     (501) staff       (20)     1595 2024-01-06 13:32:15.000000 sgen-1.0.1/tests/test_collection_positive.py
--rw-r--r--   0 verner     (501) staff       (20)     4473 2024-01-08 11:27:58.000000 sgen-1.0.1/tests/test_date_negative.py
--rw-r--r--   0 verner     (501) staff       (20)     4541 2024-01-08 11:28:48.000000 sgen-1.0.1/tests/test_date_positive.py
--rw-r--r--   0 verner     (501) staff       (20)     4547 2024-01-08 11:25:46.000000 sgen-1.0.1/tests/test_datetime_negative.py
--rw-r--r--   0 verner     (501) staff       (20)     4633 2024-01-08 11:27:58.000000 sgen-1.0.1/tests/test_datetime_positive.py
--rw-r--r--   0 verner     (501) staff       (20)     4373 2024-01-06 13:55:59.000000 sgen-1.0.1/tests/test_float_negative.py
--rw-r--r--   0 verner     (501) staff       (20)     4446 2024-01-06 13:55:59.000000 sgen-1.0.1/tests/test_float_positive.py
--rw-r--r--   0 verner     (501) staff       (20)     4379 2024-01-06 13:55:59.000000 sgen-1.0.1/tests/test_integer_negative.py
--rw-r--r--   0 verner     (501) staff       (20)     4454 2024-01-06 13:55:59.000000 sgen-1.0.1/tests/test_integet_positive.py
--rw-r--r--   0 verner     (501) staff       (20)     1383 2024-01-06 13:26:00.000000 sgen-1.0.1/tests/test_nested_negative.py
--rw-r--r--   0 verner     (501) staff       (20)     1927 2024-01-06 13:26:00.000000 sgen-1.0.1/tests/test_nested_positive.py
--rw-r--r--   0 verner     (501) staff       (20)     4497 2024-01-06 13:55:59.000000 sgen-1.0.1/tests/test_string_negative.py
--rw-r--r--   0 verner     (501) staff       (20)     4590 2024-01-06 13:55:59.000000 sgen-1.0.1/tests/test_string_positive.py
+drwxr-xr-x   0 verner     (501) staff       (20)        0 2024-04-08 08:25:53.365447 sgen-1.0.2/
+-rw-r--r--   0 verner     (501) staff       (20)     2339 2024-04-08 08:25:53.364438 sgen-1.0.2/PKG-INFO
+-rw-r--r--   0 verner     (501) staff       (20)     1576 2024-04-05 16:05:22.000000 sgen-1.0.2/README.rst
+-rw-r--r--   0 verner     (501) staff       (20)       86 2024-04-05 16:05:22.000000 sgen-1.0.2/pyproject.toml
+-rw-r--r--   0 verner     (501) staff       (20)       38 2024-04-08 08:25:53.365660 sgen-1.0.2/setup.cfg
+-rw-r--r--   0 verner     (501) staff       (20)     1614 2024-04-08 06:18:33.000000 sgen-1.0.2/setup.py
+drwxr-xr-x   0 verner     (501) staff       (20)        0 2024-04-08 08:25:53.340362 sgen-1.0.2/sgen/
+-rw-r--r--   0 verner     (501) staff       (20)      266 2024-04-08 08:25:46.000000 sgen-1.0.2/sgen/__init__.py
+-rw-r--r--   0 verner     (501) staff       (20)      485 2024-04-05 16:05:22.000000 sgen-1.0.2/sgen/base.py
+-rw-r--r--   0 verner     (501) staff       (20)      199 2024-04-05 16:05:22.000000 sgen-1.0.2/sgen/dto.py
+-rw-r--r--   0 verner     (501) staff       (20)    11964 2024-04-08 07:19:08.000000 sgen-1.0.2/sgen/fields.py
+-rw-r--r--   0 verner     (501) staff       (20)     2449 2024-04-08 08:21:47.000000 sgen-1.0.2/sgen/sgen.py
+-rw-r--r--   0 verner     (501) staff       (20)      886 2024-04-08 06:40:42.000000 sgen-1.0.2/sgen/utils.py
+-rw-r--r--   0 verner     (501) staff       (20)     7642 2024-04-07 07:28:48.000000 sgen-1.0.2/sgen/validate.py
+drwxr-xr-x   0 verner     (501) staff       (20)        0 2024-04-08 08:25:53.362550 sgen-1.0.2/sgen.egg-info/
+-rw-r--r--   0 verner     (501) staff       (20)     2339 2024-04-08 08:25:53.000000 sgen-1.0.2/sgen.egg-info/PKG-INFO
+-rw-r--r--   0 verner     (501) staff       (20)      791 2024-04-08 08:25:53.000000 sgen-1.0.2/sgen.egg-info/SOURCES.txt
+-rw-r--r--   0 verner     (501) staff       (20)        1 2024-04-08 08:25:53.000000 sgen-1.0.2/sgen.egg-info/dependency_links.txt
+-rw-r--r--   0 verner     (501) staff       (20)        1 2024-04-08 06:03:28.000000 sgen-1.0.2/sgen.egg-info/not-zip-safe
+-rw-r--r--   0 verner     (501) staff       (20)       93 2024-04-08 08:25:53.000000 sgen-1.0.2/sgen.egg-info/requires.txt
+-rw-r--r--   0 verner     (501) staff       (20)        5 2024-04-08 08:25:53.000000 sgen-1.0.2/sgen.egg-info/top_level.txt
+drwxr-xr-x   0 verner     (501) staff       (20)        0 2024-04-08 08:25:53.361307 sgen-1.0.2/tests/
+-rw-r--r--   0 verner     (501) staff       (20)     3166 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_boolean_negative.py
+-rw-r--r--   0 verner     (501) staff       (20)     3435 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_boolean_positive.py
+-rw-r--r--   0 verner     (501) staff       (20)     4172 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_collection_negative.py
+-rw-r--r--   0 verner     (501) staff       (20)     1628 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_collection_positive.py
+-rw-r--r--   0 verner     (501) staff       (20)     4838 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_date_negative.py
+-rw-r--r--   0 verner     (501) staff       (20)     4857 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_date_positive.py
+-rw-r--r--   0 verner     (501) staff       (20)     4917 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_datetime_negative.py
+-rw-r--r--   0 verner     (501) staff       (20)     5009 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_datetime_positive.py
+-rw-r--r--   0 verner     (501) staff       (20)     4398 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_float_negative.py
+-rw-r--r--   0 verner     (501) staff       (20)     4484 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_float_positive.py
+-rw-r--r--   0 verner     (501) staff       (20)     4414 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_integer_negative.py
+-rw-r--r--   0 verner     (501) staff       (20)     4497 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_integer_positive.py
+-rw-r--r--   0 verner     (501) staff       (20)     1165 2024-04-08 06:27:42.000000 sgen-1.0.2/tests/test_nested_negative.py
+-rw-r--r--   0 verner     (501) staff       (20)     1989 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_nested_positive.py
+-rw-r--r--   0 verner     (501) staff       (20)     4581 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_string_negative.py
+-rw-r--r--   0 verner     (501) staff       (20)     4680 2024-04-08 05:00:03.000000 sgen-1.0.2/tests/test_string_positive.py
```

### Comparing `sgen-1.0.1/PKG-INFO` & `sgen-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgen
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generating test data structures
 Home-page: https://github.com/Apels1nA/sgen/
 Author: Ilya Verner
 License: MIT
 Project-URL: Repo, https://github.com/Apels1nA/sgen
 Project-URL: Docs, https://sgen.readthedocs.io/en/latest/index.html
 Project-URL: Changelog, https://sgen.readthedocs.io/en/latest/changelog.html
```

### Comparing `sgen-1.0.1/README.rst` & `sgen-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `sgen-1.0.1/setup.py` & `sgen-1.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 import re
+
 from setuptools import setup, find_packages
 
+
 EXTRAS_REQUIRE = {
     "tests": ["pytest"],
     "docs": [
         "sphinx==7.2.6",
         "sphinx-issues==3.0.1",
         "alabaster==0.7.13",
     ],
 }
 
 
-def find_version(fname):
-    """Attempts to find the version number in the file names fname.
+def find_version(file_name):
+    """
+    Attempts to find the version number in the file names file_name.
     Raises RuntimeError if not found.
     """
-    version = ""
-    with open(fname) as fp:
-        reg = re.compile(r'__version__ = [\'"]([^\'"]*)[\'"]')
-        for line in fp:
-            m = reg.match(line)
-            if m:
-                version = m.group(1)
-                break
-    if not version:
+
+    pattern = re.compile(r'__version__ = \"\d+\.\d+\.\d+\"')
+
+    with open(file_name) as file:
+        lines = ' '.join(map(str.strip, file.readlines()))
+
+    matches = re.findall(pattern, lines)
+
+    if not matches:
         raise RuntimeError("Cannot find version information")
-    return version
+
+    return matches[0].split('"')[-2]
 
 
-def read(fname):
-    with open(fname) as fp:
+def read(file_name):
+    with open(file_name) as fp:
         content = fp.read()
     return content
 
 
 setup(
     name="sgen",
-    version=find_version("src/sgen/__init__.py"),
-    description=(
-        "Generating test data structures"
-    ),
+    version=find_version("sgen/__init__.py"),
+    description="Generating test data structures",
     long_description=read("README.rst"),
     author="Ilya Verner",
     url="https://github.com/Apels1nA/sgen/",
-    packages=find_packages("src"),
-    package_dir={"": "src"},
+    package_dir={"sgen": "sgen"},
     install_requires=["packaging>=17.0"],
     extras_require=EXTRAS_REQUIRE,
     license="MIT",
     zip_safe=False,
     keywords=[
         "generate",
         "data",
```

### Comparing `sgen-1.0.1/src/sgen/fields.py` & `sgen-1.0.2/sgen/fields.py`

 * *Files 25% similar despite different names*

```diff
@@ -50,50 +50,84 @@
 
         self.positive_data_from = positive_data_from
         self.negative_data_from = negative_data_from
         self.default = default
         self.allow_none = allow_none
         self.required = required
         self.values = ValuesStorage()
+        self.inner_values = []  # Only for Collections
 
     def positive(self):
         self.values = ValuesStorage()
+
         if self.positive_data_from is not None:
-            self._register(list(self.positive_data_from()))
+            yield from self.positive_data_from()
             return
 
         for validator in self.validators:
-            if not isinstance(self, Collection):
+            if isinstance(self, Collection):
+                self.inner_values = list(self.data_type.positive())
+                values = validator.positive(self)
+                for value in values:
+                    self._register(value)
+            else:
                 self._register(validator.positive(self))
 
         if self.allow_none:
             self._register(None)
 
         if self.default is not None:
             self._register(self.default)
 
         if not self.required:
             self._register(Missing())
 
+        if self.positive_data_from is None and not self.validators:
+            self.set_positive_values()
+
+        yield from self.values
+
     def negative(self):
         self.values = ValuesStorage()
+
         if self.negative_data_from is not None:
-            self._register(list(self.negative_data_from()))
+            yield from self.negative_data_from()
             return
 
         for validator in self.validators:
-            if not isinstance(self, Collection):
+            if isinstance(self, Collection):
+                self.inner_values = list(self.data_type.positive())
+                values = validator.negative(self)
+                for value in values:
+                    self._register(value)
+
+                self.inner_values = list(self.data_type.negative())
+                values = validator.positive(self)
+                for value in values:
+                    self._register(value)
+            else:
                 self._register(validator.negative(self))
 
         if not self.allow_none:
             self._register(None)
 
         if self.required:
             self._register(Missing())
 
+        if self.positive_data_from is None:
+            self.set_negative_values()
+
+        yield from self.values
+
+    def set_positive_values(self):
+        raise NotImplementedError('Implement this method in your data type')
+
+    def set_negative_values(self):
+        raise NotImplementedError('Implement this method in your data type')
+
     def generate(self, length):
         """Implement this method for the Length validator to work correctly"""
 
         raise NotImplemented(
             "To allow the Length validator to work with iterable data types"
             "you need to implement the generate method, which will return a collection of length length"
         )
@@ -103,15 +137,15 @@
 
         raise NotImplemented(
             "To allow the Range validator to work with numeric data types"
             "you need to implement a get_step method that will return the step for a numeric data type"
         )
 
     def get_other_value(self, value: Any):
-        """Реализуйте этот метод для корректной работы валидаторов Equal, OneOf и NoneOf"""
+        """Implement this method for the Equal, OneOf и NoneOf validators to work correctly"""
 
         raise NotImplemented(
             "For the Equal, OneOf and NoneOf validators to work, you need"
             "implement the get_other_value method, which will return a value not equal to value"
         )
 
     def _register(self, for_register: Union[Any, List[Any]]):
@@ -125,232 +159,155 @@
             if for_register not in self.values:
                 self.values.append(for_register)
 
 
 class String(Field):
     """String representation"""
 
-    def positive(self) -> List[Union[None, Missing, str]]:
-        super().positive()
-
-        if self.positive_data_from is not None:
-            return self.values
-
-        if not self.validators:
-            self._register(self.generate(length=randint(1, 10)))
-
-        return self.values
-
-    def negative(self) -> List[Union[None, Missing, str, int]]:
-        super().negative()
-
-        if self.negative_data_from is not None:
-            return self.values
+    def set_positive_values(self) -> None:
+        self._register(self.generate(length=randint(1, 10)))
 
+    def set_negative_values(self) -> None:
         self._register(randint(-100, 100))
 
-        return self.values
-
     def generate(self, length: int):
         """
         Generates a string of the specified length.
 
         :param length: String length.
         :return: String.
         """
 
         return ''.join(choice(ascii_letters) for _ in range(length))
 
     def get_other_value(self, value: Optional[str]) -> str:
+        """Returns an object of type str and not equal to value"""
+
         if value is None:
             return 'not_comparable'
         return 'not_' + value
 
 
 class Integer(Field):
     """Integer representation"""
 
     def __init__(self, step: int = 1, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.step = step
 
-    def positive(self) -> List[Union[None, Missing, int]]:
-        super().positive()
-
-        if self.positive_data_from is not None:
-            return self.values
-
-        if not self.validators:
-            self._register(randint(-100, 100))
-
-        return self.values
-
-    def negative(self) -> List[Union[None, Missing, int, str]]:
-        super().negative()
-
-        if self.negative_data_from is not None:
-            return self.values
+    def set_positive_values(self) -> None:
+        self._register(randint(-100, 100))
 
+    def set_negative_values(self) -> None:
         self._register(
             ''.join(choice(ascii_letters) for _ in range(randint(5, 10)))
         )
 
-        return self.values
-
     def get_step(self):
         return self.step
 
     def get_other_value(self, value: Optional[int]) -> int:
+        """Returns an object of type int and not equal to value"""
+
         if value is None:
             return randint(10, 100000)
         return value + randint(10, 100000)
 
 
 class Float(Field):
     """Floating point representation"""
 
     def __init__(self, step: float = 0.01, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.step = step
 
-    def positive(self) -> List[Union[None, Missing, float]]:
-        super().positive()
-
-        if self.positive_data_from is not None:
-            return self.values
-
-        if not self.validators:
-            self._register(randint(-10000, 10000) / 100)
-
-        return self.values
-
-    def negative(self) -> List[Union[None, Missing, float, str]]:
-        super().negative()
-
-        if self.negative_data_from is not None:
-            return self.values
+    def set_positive_values(self) -> None:
+        self._register(randint(-10000, 10000) / 100)
 
+    def set_negative_values(self) -> None:
         self._register(
             ''.join(choice(ascii_letters) for _ in range(randint(5, 10)))
         )
 
-        return self.values
-
     def get_step(self):
         return self.step
 
     def get_other_value(self, value: Optional[float]) -> float:
+        """Returns an object of type float and not equal to value"""
+
         if value is None:
             return randint(1000000, 100000000) / 100
         return value + randint(1000000, 100000000) / 100
 
 
 class Boolean(Field):
     """Boolean type representation"""
 
-    def positive(self) -> List[Union[None, Missing, bool]]:
-        super().positive()
-
-        if self.positive_data_from is not None:
-            return self.values
-
-        if not self.validators:
-            self._register([True, False])
-
-        return self.values
-
-    def negative(self) -> List[Union[None, Missing, bool, str]]:
-        super().negative()
-
-        if self.negative_data_from is not None:
-            return self.values
+    def set_positive_values(self) -> None:
+        self._register([True, False])
 
+    def set_negative_values(self) -> None:
         self._register(
             ''.join(choice(ascii_letters) for _ in range(randint(5, 10)))
         )
 
-        return self.values
-
     def get_other_value(self, value: Optional[bool]) -> bool:
+        """Returns an object of type bool and not equal to value"""
+
         if value is None:
             return True
         return not value
 
 
 class DateTime(Field):
     """Datetime type representation"""
 
     def __init__(self, step: timedelta = timedelta(days=1), *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.step = step
 
-    def positive(self) -> List[Union[None, Missing, datetime]]:
-        super().positive()
-
-        if self.positive_data_from is not None:
-            return self.values
-
-        if not self.validators:
-            self._register(datetime.now())
-
-        return self.values
-
-    def negative(self) -> List[Union[None, Missing, datetime, str]]:
-        super().negative()
-
-        if self.negative_data_from is not None:
-            return self.values
+    def set_positive_values(self) -> None:
+        self._register(datetime.now())
 
+    def set_negative_values(self) -> None:
         self._register('not_datetime')
 
-        return self.values
-
     def get_step(self) -> timedelta:
         return self.step
 
     def get_other_value(self, value: Optional[datetime]) -> datetime:
+        """Returns an object of type datetime and not equal to value"""
+
         if value is None:
             return datetime.now()
         return value + timedelta(days=randint(1, 365), minutes=randint(1, 60))
 
 
 class Date(Field):
     """Date type representation"""
 
     def __init__(self, step: timedelta = timedelta(days=1), *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.step = step
 
-    def positive(self) -> List[Union[None, Missing, date]]:
-        super().positive()
-
-        if self.positive_data_from is not None:
-            return self.values
-
-        if not self.validators:
-            self._register(datetime.now().date())
-
-        return self.values
-
-    def negative(self) -> List[Union[None, Missing, date, str]]:
-        super().negative()
-
-        if self.negative_data_from is not None:
-            return self.values
+    def set_positive_values(self) -> None:
+        self._register(datetime.now().date())
 
+    def set_negative_values(self) -> None:
         self._register('not_date')
 
-        return self.values
-
     def get_step(self):
         return self.step
 
     def get_other_value(self, value: date) -> date:
+        """Returns an object of type date and not equal to value"""
+
         if value is None:
             return datetime.now().date()
+
         return value + timedelta(days=randint(1, 365))
 
 
 class Collection(Field):
     """List view"""
 
     def __init__(self, data_type: Union[FieldABC, 'SGen'], *args, **kwargs):
@@ -358,15 +315,14 @@
         Initializes the collection by adding a new data_type parameter to it
 
         :param data_type: Collection data type
         """
 
         super().__init__(*args, **kwargs)
         self.data_type = data_type
-        self.inner_values = []
 
     def _register(self, for_register: Union[Any, List[Any]]):
         """
         Adds a new value/values to the field's list of values if it is not already present
         Additionally, it clears lists of the Missing value, since doing this at the SGen class level is inconvenient
 
         :param for_register: Adds a value or list of logged values
@@ -378,63 +334,35 @@
                 for value in for_register
                 if list(filter(lambda item: not isinstance(item, Missing), value)) or not self.validators
             ])
         else:
             if for_register not in self.values:
                 self.values.append(for_register)
 
-    def positive(self) -> List[Any]:
-        super().positive()
-
-        if self.positive_data_from is not None:
-            return self.values
-
+    def set_positive_values(self) -> None:
         self.inner_values = self.data_type.positive()
 
-        for validator in self.validators:
-            values = validator.positive(self)
-            for value in values:
-                self._register(value)
-
-        if not self.validators:
-            for value in self.inner_values:
-                self._register([[value for _ in range(randint(1, 5))]])
-        return self.values
-
-    def negative(self) -> List[Any]:
-        super().negative()
-
-        if self.negative_data_from is not None:
-            return self.values
-
-        self.inner_values = self.data_type.positive()
-        for validator in self.validators:
-            values = validator.negative(self)
-            for value in values:
-                self._register(value)
+        for value in self.inner_values:
+            self._register([[value for _ in range(randint(1, 5))]])
 
+    def set_negative_values(self) -> None:
         self.inner_values = self.data_type.negative()
-        for validator in self.validators:
-            values = validator.positive(self)
-            for value in values:
-                self._register(value)
-
-        if not self.validators:
-            for value in self.inner_values:
-                self._register([[value for _ in range(randint(1, 5))]])
 
-        return self.values
+        for value in self.inner_values:
+            self._register([[value for _ in range(randint(1, 5))]])
 
     def generate(self, length: int) -> List[Any]:
         return [
             [allowed_value for _ in range(length)]
             for allowed_value in self.inner_values
         ]
 
     def get_other_value(self, value: list) -> list:
+        """Returns an object of type list and not equal to value"""
+
         if value is None:
             return [self.data_type.get_other_value(value=value)]
         return value * 2
 
 
 class Nested(Field):
     """Entity View"""
@@ -445,24 +373,12 @@
 
         :param data_type: Schema data type
         """
 
         super().__init__(*args, **kwargs)
         self.data_type = data_type
 
-    def positive(self):
-        super().positive()
-
-        if self.positive_data_from is not None:
-            return self.values
-
-        for structure in self.data_type.positive():
-            yield structure
-
-    def negative(self):
-        super().negative()
-
-        if self.negative_data_from is not None:
-            return self.values
+    def set_positive_values(self) -> None:
+        self._register(list(self.data_type.positive()))
 
-        for structure in self.data_type.negative():
-            yield structure
+    def set_negative_values(self) -> None:
+        self._register(list(self.data_type.negative()))
```

### Comparing `sgen-1.0.1/src/sgen/sgen.py` & `sgen-1.0.2/sgen/sgen.py`

 * *Files 15% similar despite different names*

```diff
@@ -79,13 +79,7 @@
                 fields.append(p_gen)
 
             for dataset in self._generate(fields=fields):
                 yield dict(filter(
                     lambda field_value: not isinstance(field_value[1], Missing),
                     dataset
                 ))
-
-        for dataset in self._generate(fields=self.fields(is_positive=False)):
-            yield dict(filter(
-                lambda field_value: not isinstance(field_value[1], Missing),
-                dataset
-            ))
```

### Comparing `sgen-1.0.1/src/sgen/utils.py` & `sgen-1.0.2/sgen/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from inspect import isgeneratorfunction, isgenerator
 
 
 class Missing:
     """Represents an instance of a missing field"""
 
+    is_missing = True
+
     def __repr__(self):
         return "<sgen.missing>"
 
 
 class ValuesStorage(list):
-    """Represents storage for field values"""
+    """
+    Represents storage for field values
+
+    :note: Implemented because True in [1] -> True, but should be False
+    """
 
     def __contains__(self, item):
         present = list(filter(
             lambda value: type(value) == type(item) and value == item,
             self
         ))
```

### Comparing `sgen-1.0.1/src/sgen/validate.py` & `sgen-1.0.2/sgen/validate.py`

 * *Files identical despite different names*

### Comparing `sgen-1.0.1/src/sgen.egg-info/PKG-INFO` & `sgen-1.0.2/sgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgen
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generating test data structures
 Home-page: https://github.com/Apels1nA/sgen/
 Author: Ilya Verner
 License: MIT
 Project-URL: Repo, https://github.com/Apels1nA/sgen
 Project-URL: Docs, https://sgen.readthedocs.io/en/latest/index.html
 Project-URL: Changelog, https://sgen.readthedocs.io/en/latest/changelog.html
```

### Comparing `sgen-1.0.1/src/sgen.egg-info/SOURCES.txt` & `sgen-1.0.2/sgen.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 README.rst
 pyproject.toml
 setup.py
-src/sgen/__init__.py
-src/sgen/base.py
-src/sgen/dto.py
-src/sgen/fields.py
-src/sgen/sgen.py
-src/sgen/utils.py
-src/sgen/validate.py
-src/sgen.egg-info/PKG-INFO
-src/sgen.egg-info/SOURCES.txt
-src/sgen.egg-info/dependency_links.txt
-src/sgen.egg-info/not-zip-safe
-src/sgen.egg-info/requires.txt
-src/sgen.egg-info/top_level.txt
+sgen/__init__.py
+sgen/base.py
+sgen/dto.py
+sgen/fields.py
+sgen/sgen.py
+sgen/utils.py
+sgen/validate.py
+sgen.egg-info/PKG-INFO
+sgen.egg-info/SOURCES.txt
+sgen.egg-info/dependency_links.txt
+sgen.egg-info/not-zip-safe
+sgen.egg-info/requires.txt
+sgen.egg-info/top_level.txt
 tests/test_boolean_negative.py
 tests/test_boolean_positive.py
 tests/test_collection_negative.py
 tests/test_collection_positive.py
 tests/test_date_negative.py
 tests/test_date_positive.py
 tests/test_datetime_negative.py
 tests/test_datetime_positive.py
 tests/test_float_negative.py
 tests/test_float_positive.py
 tests/test_integer_negative.py
-tests/test_integet_positive.py
+tests/test_integer_positive.py
 tests/test_nested_negative.py
 tests/test_nested_positive.py
 tests/test_string_negative.py
 tests/test_string_positive.py
```

### Comparing `sgen-1.0.1/tests/test_boolean_negative.py` & `sgen-1.0.2/tests/test_boolean_negative.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 from tests import has_data_type, Unique
-from fields import Boolean
-from utils import Missing
-from validate import Equal, OneOf
+from sgen.fields import Boolean
+from sgen.utils import Missing
+from sgen.validate import Equal, OneOf
 
 
 def test_boolean():
     field = Boolean()
 
-    negative_values = field.negative()
+    negative_values = list(field.negative())
 
     assert len(negative_values) == 1
     assert not isinstance(negative_values[0], bool)
 
 
 def test_allow_none():
     field = Boolean(allow_none=False)
 
-    assert None in field.negative()
+    assert None in list(field.negative())
 
 
 def test_required():
     field = Boolean(required=True)
 
-    assert has_data_type(field.negative(), Missing)
+    negative_values = list(field.negative())
+
+    assert has_data_type(negative_values, Missing)
 
 
 def test_negative_data_from():
     def negative_data_from():
         return 'a', -88.17, None
 
     field = Boolean(negative_data_from=negative_data_from)
 
-    assert field.negative() == list(negative_data_from())
+    assert list(field.negative()) == list(negative_data_from())
 
 
 # ===================================================
 # Тесты на взаимодействие типа Boolean с валидаторами
 # ===================================================
 
 
 def test_equal():
     comparable = Unique()
 
     field = Boolean(
         validate=Equal(comparable=comparable)
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert comparable not in field_values
     assert None not in field_values
     assert has_data_type(field_values, str)
 
 
 def test_equal_allow_none_and_required():
@@ -58,15 +60,15 @@
 
     field = Boolean(
         validate=Equal(comparable=comparable),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert comparable not in field_values
     assert None in field_values
     assert has_data_type(field_values, str)
     assert has_data_type(field_values, Missing)
 
 
@@ -76,28 +78,28 @@
 
     field = Boolean(
         validate=Equal(comparable=comparable),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert default not in field_values
     assert None in field_values
 
 
 def test_one_of():
     choices = [Unique(), Unique(), Unique()]
 
     field = Boolean(
         validate=OneOf(choices=choices),
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     for value in choices:
         assert value not in field_values
 
     assert None not in field_values
     assert has_data_type(field_values, str)
     assert not has_data_type(field_values, Missing)
@@ -108,15 +110,15 @@
 
     field = Boolean(
         validate=OneOf(choices=choices),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     for value in choices:
         assert value not in field_values
 
     assert None in field_values
     assert has_data_type(field_values, str)
     assert has_data_type(field_values, Missing)
@@ -128,11 +130,11 @@
 
     field = Boolean(
         validate=OneOf(choices=choices),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert default not in field_values
     assert None in field_values
```

### Comparing `sgen-1.0.1/tests/test_boolean_positive.py` & `sgen-1.0.2/tests/test_boolean_positive.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from tests import has_data_type, Unique
-from fields import Boolean
-from utils import Missing
-from validate import Equal, OneOf
+from sgen.fields import Boolean
+from sgen.utils import Missing
+from sgen.validate import Equal, OneOf
 
 
 def test_boolean():
     field = Boolean()
 
-    positive_values = field.positive()
+    positive_values = list(field.positive())
 
     assert len(positive_values) == 4
 
     has_true = False
     has_false = False
     for value in positive_values:
         if isinstance(value, bool) and value:
@@ -24,51 +24,51 @@
     assert has_data_type(positive_values, type(None))
     assert has_data_type(positive_values, Missing)
 
 
 def test_allow_none():
     field = Boolean(allow_none=False)
 
-    assert None not in field.positive()
+    assert None not in list(field.positive())
 
 
 def test_required():
     fields = Boolean(required=True)
 
-    assert not has_data_type(fields.positive(), Missing)
+    assert not has_data_type(list(fields.positive()), Missing)
 
 
 def test_default():
     field = Boolean(default=False)
 
-    assert False in field.positive()
+    assert False in list(field.positive())
 
 
 def test_positive_data_from():
     def positive_data_generator():
         return 0, 1, False, True
 
     field = Boolean(positive_data_from=positive_data_generator)
 
-    assert field.positive() == list(positive_data_generator())
+    assert list(field.positive()) == list(positive_data_generator())
 
 
 # ===================================================
 # Тесты на взаимодействие типа Boolean с валидаторами
 # ===================================================
 
 
 def test_equal():
     comparable = Unique()
 
     field = Boolean(
         validate=Equal(comparable=comparable)
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert comparable in field_values
     assert None in field_values
     assert has_data_type(field_values, Missing)
 
 
 def test_equal_allow_none_required():
@@ -76,15 +76,15 @@
 
     field = Boolean(
         validate=Equal(comparable=comparable),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert comparable in field_values
     assert None not in field_values
     assert not has_data_type(field_values, Missing)
 
 
 def test_equal_default():
@@ -93,28 +93,28 @@
 
     field = Boolean(
         validate=Equal(comparable=comparable),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert default in field_values
     assert None not in field_values
 
 
 def test_one_of():
     choices = [Unique(), Unique(), Unique()]
 
     field = Boolean(
         validate=OneOf(choices=choices),
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     for value in choices:
         assert value in field_values
 
     assert None in field_values
     assert has_data_type(field_values, Missing)
 
@@ -124,15 +124,15 @@
 
     field = Boolean(
         validate=OneOf(choices=choices),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     for value in choices:
         assert value in field_values
 
     assert None not in field_values
     assert not has_data_type(field_values, Missing)
 
@@ -143,11 +143,11 @@
 
     field = Boolean(
         validate=OneOf(choices=choices),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert default in field_values
     assert None not in field_values
```

### Comparing `sgen-1.0.1/tests/test_collection_negative.py` & `sgen-1.0.2/tests/test_collection_negative.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from fields import (
+from sgen.fields import (
     Collection,
     String,
     Float,
     Boolean,
     Integer,
 )
-from validate import Length
+from sgen.validate import Length
 from tests import Unique, has_data_type
-from utils import Missing
+from sgen.utils import Missing
 
 DATA_TYPES = [
     # [Тип поля, представляемый им тип, противоположный тип]
     [String, str, int],
     [Integer, int, str],
     [Float, float, str],
     [Boolean, bool, str],
 ]
 
 
 def test_simple():
     for type_ in DATA_TYPES:
         field = Collection(data_type=type_[0]())
 
-        field_values = field.negative()
+        field_values = list(field.negative())
 
         assert None not in field_values
         assert not has_data_type(field_values, Missing)
         assert has_data_type(field_values, list)
 
         for value in field_values:
             if isinstance(value, list):
@@ -53,15 +53,15 @@
                 min=min_,
                 max=max_,
             ),
             allow_none=False,
             required=True,
         )
 
-        field_values = field.negative()
+        field_values = list(field.negative())
 
         assert None in field_values
         assert has_data_type(field_values, Missing)
         assert has_data_type(field_values, list)
 
         has_lower = False
         has_min = False
@@ -105,15 +105,15 @@
                 min_inclusive=False,
                 max_inclusive=False,
             ),
             allow_none=False,
             required=True,
         )
 
-        field_values = field.negative()
+        field_values = list(field.negative())
 
         has_lower = False
         has_min = False
         has_max = False
         has_biggest = False
         has_positive_len_but_wrong_type_min = False
         has_positive_len_but_wrong_type_max = False
```

### Comparing `sgen-1.0.1/tests/test_collection_positive.py` & `sgen-1.0.2/tests/test_collection_positive.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from fields import (
+from sgen.fields import (
     Collection,
     String,
     Float,
     Boolean,
     Integer,
 )
-from validate import Length
+from sgen.validate import Length
 from tests import Unique, has_data_type
-from utils import Missing
+from sgen.utils import Missing
 
 DATA_TYPES = [
     [String, str],
     [Integer, int],
     [Float, float],
     [Boolean, bool],
 ]
 
 
 def test_simple():
     for type_ in DATA_TYPES:
         field = Collection(data_type=type_[0]())
 
-        field_values = field.positive()
+        field_values = list(field.positive())
 
         assert None in field_values
         assert has_data_type(field_values, Missing)
         assert has_data_type(field_values, list)
 
         for value in field_values:
             if isinstance(value, list):
@@ -33,15 +33,15 @@
                     has_data_type(value, type_[1]) or
                     not value or
                     None in value
                 )
 
         default = Unique()
         field = Collection(data_type=type_[0](), default=default)
-        assert default in field.positive()
+        assert default in list(field.positive())
 
 
 def test_length_validator():
     min_ = 100
     max_ = 200
 
     for type_ in DATA_TYPES:
@@ -51,15 +51,15 @@
                 min=min_,
                 max=max_,
             ),
             allow_none=False,
             required=True,
         )
 
-        field_values = field.positive()
+        field_values = list(field.positive())
 
         assert None not in field_values
         assert not has_data_type(field_values, Missing)
         assert has_data_type(field_values, list)
 
         for value in field_values:
             if isinstance(value, list):
```

### Comparing `sgen-1.0.1/tests/test_date_negative.py` & `sgen-1.0.2/tests/test_float_negative.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,207 +1,205 @@
-from datetime import datetime, date
+from tests import has_data_type
+from sgen.fields import Float
+from sgen.utils import Missing
+from sgen.validate import Range, Equal, OneOf
 
-from tests import has_data_type, Unique
-from fields import Date
-from utils import Missing
-from validate import Range, Equal, OneOf
 
+def test_float():
+    field = Float()
 
-def test_date():
-    field = Date()
-
-    negative_values = field.negative()
+    negative_values = list(field.negative())
 
     assert len(negative_values) == 1
-    assert not isinstance(negative_values[0], date)
+    assert not isinstance(negative_values[0], float)
 
 
 def test_allow_none():
-    field = Date(allow_none=False)
+    field = Float(allow_none=False)
 
-    assert None in field.negative()
+    assert None in list(field.negative())
 
 
 def test_required():
-    field = Date(required=True)
+    field = Float(required=True)
 
-    assert has_data_type(field.negative(), Missing)
+    assert has_data_type(list(field.negative()), Missing)
 
 
 def test_negative_data_from():
     def negative_data_from():
-        return None, Missing
+        return 'a', 333.44, None, Missing
 
-    field = Date(negative_data_from=negative_data_from)
+    field = Float(negative_data_from=negative_data_from)
 
-    assert field.negative() == list(negative_data_from())
+    assert list(field.negative()) == list(negative_data_from())
 
 
 # =================================================
 # Тесты на взаимодействие типа Float с валидаторами
 # =================================================
 
 
 def test_range():
-    min_ = date(2022, 1, 1)
-    max_ = date(2023, 1, 1)
+    min_ = -673.94
+    max_ = 98.01
 
-    field = Date(
+    field = Float(
         validate=Range(
             min=min_, max=max_
         )
     )
 
-    negative_data = field.negative()
+    negative_data = list(field.negative())
 
-    assert min_ - field.get_step() in negative_data
-    assert max_ + field.get_step() in negative_data
+    assert min_ - 0.01 in negative_data
+    assert max_ + 0.01 in negative_data
 
 
 def test_range_inclusive():
-    min_ = date(2022, 1, 1)
-    max_ = date(2023, 1, 1)
+    min_ = -673.94
+    max_ = 98.01
 
-    field = Date(
+    field = Float(
         validate=Range(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         required=True,
     )
 
-    negative_data = field.negative()
+    negative_data = list(field.negative())
 
     assert min_ in negative_data
     assert max_ in negative_data
     assert None in negative_data
     assert has_data_type(negative_data, Missing)
 
 
 def test_range_default():
-    min_ = datetime(2022, 1, 1)
-    max_ = datetime(2023, 1, 1)
-    default = Unique()
+    min_ = -673.94
+    max_ = 98.01
+    default = 55.19
 
-    field = Date(
+    field = Float(
         validate=Range(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         default=default,
     )
 
-    negative_data = field.negative()
+    negative_data = list(field.negative())
 
     assert min_ in negative_data
     assert max_ in negative_data
     assert None in negative_data
     assert default not in negative_data
 
 
 def test_equal():
-    comparable = Unique()
+    comparable = 55.19
 
-    field = Date(
+    field = Float(
         validate=Equal(comparable=comparable)
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert comparable not in field_values
     assert None not in field_values
     assert has_data_type(field_values, str)
 
 
 def test_equal_allow_none_required():
-    comparable = Unique()
+    comparable = 55.19
 
-    field = Date(
+    field = Float(
         validate=Equal(comparable=comparable),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert comparable not in field_values
     assert None in field_values
     assert has_data_type(field_values, str)
     assert has_data_type(field_values, Missing)
 
 
 def test_equal_default():
-    comparable = Unique()
-    default = Unique()
+    comparable = 55.19
+    default = -87.009
 
-    field = Date(
+    field = Float(
         validate=Equal(comparable=comparable),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert None in field_values
     assert default not in field_values
 
 
 def test_one_of():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [1.1, 2.2, 3.3]
 
-    field = Date(
+    field = Float(
         validate=OneOf(choices=choices),
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     for value in choices:
         assert value not in field_values
 
     assert None not in field_values
     assert has_data_type(field_values, str)
     assert not has_data_type(field_values, Missing)
 
 
 def test_one_of_allow_none_required():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [1.1, 2.2, 3.3]
 
-    field = Date(
+    field = Float(
         validate=OneOf(choices=choices),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     for value in choices:
         assert value not in field_values
 
     assert None in field_values
     assert has_data_type(field_values, str)
     assert has_data_type(field_values, Missing)
 
 
 def test_one_of_default():
-    choices = [Unique(), Unique(), Unique()]
-    default = Unique()
+    choices = [1.1, 2.2, 3.3]
+    default = 55.087
 
-    field = Date(
+    field = Float(
         validate=OneOf(choices=choices),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     for value in choices:
         assert value not in field_values
 
     assert has_data_type(field_values, str)
     assert None in field_values
     assert default not in field_values
```

### Comparing `sgen-1.0.1/tests/test_date_positive.py` & `sgen-1.0.2/tests/test_datetime_positive.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,213 +1,225 @@
-from datetime import date
+from datetime import datetime
 
-from tests import has_data_type, Unique
-from fields import Date
-from utils import Missing
-from validate import Range, Equal, OneOf
+from tests import has_data_type
+from sgen.fields import DateTime
+from sgen.utils import Missing
+from sgen.validate import Range, Equal, OneOf
 
 
-def test_date():
-    field = Date()
+def test_datetime():
+    field = DateTime()
 
-    positive_values = field.positive()
+    positive_values = list(field.positive())
 
     assert len(positive_values) == 3
 
-    assert has_data_type(positive_values, date)
+    assert has_data_type(positive_values, datetime)
     assert has_data_type(positive_values, type(None))
     assert has_data_type(positive_values, Missing)
 
 
 def test_allow_none():
-    field = Date(allow_none=False)
+    field = DateTime(allow_none=False)
 
-    assert None not in field.positive()
+    assert None not in list(field.positive())
 
 
 def test_required():
-    field = Date(required=True)
+    field = DateTime(required=True)
 
-    assert not has_data_type(field.positive(), Missing)
+    assert not has_data_type(list(field.positive()), Missing)
 
 
 def test_default():
     default = 1.23456789
-    field = Date(default=default)
+    field = DateTime(default=default)
 
-    assert default in field.positive()
+    assert default in list(field.positive())
 
 
 def test_positive_data_from():
     def positive_data_generator():
         return 1.0, -9999.9999
 
-    field = Date(positive_data_from=positive_data_generator)
+    field = DateTime(positive_data_from=positive_data_generator)
 
-    assert field.positive() == list(positive_data_generator())
+    assert list(field.positive()) == list(positive_data_generator())
 
 
 # =================================================
-# Тесты на взаимодействие типа Date с валидаторами
+# Тесты на взаимодействие типа DateTime с валидаторами
 # =================================================
 
 
 def test_range():
     min_ = -999.74
     max_ = 998.39
 
-    field = Date(
+    field = DateTime(
         validate=Range(
             min=min_, max=max_
         )
     )
 
-    positive_data = field.positive()
+    positive_data = list(field.positive())
 
     assert min_ in positive_data
     assert max_ in positive_data
 
 
 def test_range_inclusive():
-    min_ = date(2022, 1, 1)
-    max_ = date(2023, 1, 1)
+    min_ = datetime(2022, 1, 1)
+    max_ = datetime(2023, 1, 1)
 
-    field = Date(
+    field = DateTime(
         validate=Range(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         required=True,
     )
 
-    positive_data = field.positive()
+    positive_data = list(field.positive())
 
     assert min_ + field.get_step() in positive_data
     assert max_ - field.get_step() in positive_data
     assert None not in positive_data
     assert not has_data_type(positive_data, Missing)
 
 
 def test_range_default():
-    min_ = date(2022, 1, 1)
-    max_ = date(2023, 1, 1)
-    default = Unique()
+    min_ = datetime(2022, 1, 1)
+    max_ = datetime(2023, 1, 1)
+    default = datetime(1996, 12, 3)
 
-    field = Date(
+    field = DateTime(
         validate=Range(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         default=default,
     )
 
-    positive_data = field.positive()
+    positive_data = list(field.positive())
 
     assert min_ + field.get_step() in positive_data
     assert max_ - field.get_step() in positive_data
     assert None not in positive_data
     assert default in positive_data
 
 
 def test_equal():
-    comparable = Unique()
+    comparable = datetime(1996, 12, 3)
 
-    field = Date(
+    field = DateTime(
         validate=Equal(comparable=comparable)
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert comparable in field_values
     assert None in field_values
     assert has_data_type(field_values, Missing)
 
 
 def test_equal_allow_none_required():
-    comparable = Unique()
+    comparable = datetime(1996, 12, 3)
 
-    field = Date(
+    field = DateTime(
         validate=Equal(comparable=comparable),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert comparable in field_values
     assert None not in field_values
     assert not has_data_type(field_values, Missing)
 
 
 def test_equal_default():
-    comparable = Unique()
-    default = Unique()
+    comparable = datetime(1996, 12, 3)
+    default = datetime(2000, 12, 3)
 
-    field = Date(
+    field = DateTime(
         validate=Equal(comparable=comparable),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert default in field_values
     assert None not in field_values
 
 
 def test_one_of():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [
+        datetime(1996, 12, 3),
+        datetime(2000, 12, 3),
+        datetime(2002, 12, 3)
+    ]
 
-    field = Date(
+    field = DateTime(
         validate=OneOf(choices=choices),
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     for value in choices:
         assert value in field_values
 
     assert None in field_values
     assert has_data_type(field_values, Missing)
 
 
 def test_one_of_allow_none_required():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [
+        datetime(1996, 12, 3),
+        datetime(2000, 12, 3),
+        datetime(2002, 12, 3)
+    ]
 
-    field = Date(
+    field = DateTime(
         validate=OneOf(choices=choices),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     for value in choices:
         assert value in field_values
 
     assert None not in field_values
     assert not has_data_type(field_values, Missing)
 
 
 def test_one_of_default():
-    choices = [Unique(), Unique(), Unique()]
-    default = Unique()
+    choices = [
+        datetime(1996, 12, 3),
+        datetime(2000, 12, 3),
+        datetime(2002, 12, 3)
+    ]
+    default = datetime(1991, 12, 3)
 
-    field = Date(
+    field = DateTime(
         validate=OneOf(choices=choices),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     for value in choices:
         assert value in field_values
 
     assert None not in field_values
     assert default in field_values
```

### Comparing `sgen-1.0.1/tests/test_datetime_negative.py` & `sgen-1.0.2/tests/test_datetime_negative.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from datetime import datetime
 
-from tests import has_data_type, Unique
-from fields import DateTime
-from utils import Missing
-from validate import Range, Equal, OneOf
+from tests import has_data_type
+from sgen.fields import DateTime
+from sgen.utils import Missing
+from sgen.validate import Range, Equal, OneOf
 
 
 def test_datetime():
     field = DateTime()
 
-    negative_values = field.negative()
+    negative_values = list(field.negative())
 
     assert len(negative_values) == 1
     assert not isinstance(negative_values[0], datetime)
 
 
 def test_allow_none():
     field = DateTime(allow_none=False)
 
-    assert None in field.negative()
+    assert None in list(field.negative())
 
 
 def test_required():
     field = DateTime(required=True)
 
-    assert has_data_type(field.negative(), Missing)
+    assert has_data_type(list(field.negative()), Missing)
 
 
 def test_negative_data_from():
     def negative_data_from():
         return None, Missing
 
     field = DateTime(negative_data_from=negative_data_from)
 
-    assert field.negative() == list(negative_data_from())
+    assert list(field.negative()) == list(negative_data_from())
 
 
 # =================================================
 # Тесты на взаимодействие типа Float с валидаторами
 # =================================================
 
 
@@ -47,15 +47,15 @@
 
     field = DateTime(
         validate=Range(
             min=min_, max=max_
         )
     )
 
-    negative_data = field.negative()
+    negative_data = list(field.negative())
 
     assert min_ - field.get_step() in negative_data
     assert max_ + field.get_step() in negative_data
 
 
 def test_range_inclusive():
     min_ = datetime(2022, 1, 1)
@@ -68,140 +68,152 @@
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         required=True,
     )
 
-    negative_data = field.negative()
+    negative_data = list(field.negative())
 
     assert min_ in negative_data
     assert max_ in negative_data
     assert None in negative_data
     assert has_data_type(negative_data, Missing)
 
 
 def test_range_default():
     min_ = datetime(2022, 1, 1)
     max_ = datetime(2023, 1, 1)
-    default = Unique()
+    default = datetime(1996, 12, 3)
 
     field = DateTime(
         validate=Range(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         default=default,
     )
 
-    negative_data = field.negative()
+    negative_data = list(field.negative())
 
     assert min_ in negative_data
     assert max_ in negative_data
     assert None in negative_data
     assert default not in negative_data
 
 
 def test_equal():
-    comparable = Unique()
+    comparable = datetime(1996, 12, 3)
 
     field = DateTime(
         validate=Equal(comparable=comparable)
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert comparable not in field_values
     assert None not in field_values
     assert has_data_type(field_values, str)
 
 
 def test_equal_allow_none_required():
-    comparable = Unique()
+    comparable = datetime(1996, 12, 3)
 
     field = DateTime(
         validate=Equal(comparable=comparable),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert comparable not in field_values
     assert None in field_values
     assert has_data_type(field_values, str)
     assert has_data_type(field_values, Missing)
 
 
 def test_equal_default():
-    comparable = Unique()
-    default = Unique()
+    comparable = datetime(1996, 12, 3)
+    default = datetime(2000, 12, 3)
 
     field = DateTime(
         validate=Equal(comparable=comparable),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert None in field_values
     assert default not in field_values
 
 
 def test_one_of():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [
+        datetime(1996, 12, 3),
+        datetime(2000, 12, 3),
+        datetime(2002, 12, 3)
+    ]
 
     field = DateTime(
         validate=OneOf(choices=choices),
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     for value in choices:
         assert value not in field_values
 
     assert None not in field_values
     assert has_data_type(field_values, str)
     assert not has_data_type(field_values, Missing)
 
 
 def test_one_of_allow_none_required():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [
+        datetime(1996, 12, 3),
+        datetime(2000, 12, 3),
+        datetime(2002, 12, 3)
+    ]
 
     field = DateTime(
         validate=OneOf(choices=choices),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     for value in choices:
         assert value not in field_values
 
     assert None in field_values
     assert has_data_type(field_values, str)
     assert has_data_type(field_values, Missing)
 
 
 def test_one_of_default():
-    choices = [Unique(), Unique(), Unique()]
-    default = Unique()
+    choices = [
+        datetime(1996, 12, 3),
+        datetime(2000, 12, 3),
+        datetime(2002, 12, 3)
+    ]
+    default = datetime(1991, 12, 3)
 
     field = DateTime(
         validate=OneOf(choices=choices),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     for value in choices:
         assert value not in field_values
 
     assert has_data_type(field_values, str)
     assert None in field_values
     assert default not in field_values
```

### Comparing `sgen-1.0.1/tests/test_datetime_positive.py` & `sgen-1.0.2/tests/test_date_positive.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,213 +1,225 @@
-from datetime import datetime
+from datetime import date
 
-from tests import has_data_type, Unique
-from fields import DateTime
-from utils import Missing
-from validate import Range, Equal, OneOf
+from tests import has_data_type
+from sgen.fields import Date
+from sgen.utils import Missing
+from sgen.validate import Range, Equal, OneOf
 
 
-def test_datetime():
-    field = DateTime()
+def test_date():
+    field = Date()
 
-    positive_values = field.positive()
+    positive_values = list(field.positive())
 
     assert len(positive_values) == 3
 
-    assert has_data_type(positive_values, datetime)
+    assert has_data_type(positive_values, date)
     assert has_data_type(positive_values, type(None))
     assert has_data_type(positive_values, Missing)
 
 
 def test_allow_none():
-    field = DateTime(allow_none=False)
+    field = Date(allow_none=False)
 
-    assert None not in field.positive()
+    assert None not in list(field.positive())
 
 
 def test_required():
-    field = DateTime(required=True)
+    field = Date(required=True)
 
-    assert not has_data_type(field.positive(), Missing)
+    assert not has_data_type(list(field.positive()), Missing)
 
 
 def test_default():
     default = 1.23456789
-    field = DateTime(default=default)
+    field = Date(default=default)
 
-    assert default in field.positive()
+    assert default in list(field.positive())
 
 
 def test_positive_data_from():
     def positive_data_generator():
         return 1.0, -9999.9999
 
-    field = DateTime(positive_data_from=positive_data_generator)
+    field = Date(positive_data_from=positive_data_generator)
 
-    assert field.positive() == list(positive_data_generator())
+    assert list(field.positive()) == list(positive_data_generator())
 
 
 # =================================================
-# Тесты на взаимодействие типа DateTime с валидаторами
+# Тесты на взаимодействие типа Date с валидаторами
 # =================================================
 
 
 def test_range():
     min_ = -999.74
     max_ = 998.39
 
-    field = DateTime(
+    field = Date(
         validate=Range(
             min=min_, max=max_
         )
     )
 
-    positive_data = field.positive()
+    positive_data = list(field.positive())
 
     assert min_ in positive_data
     assert max_ in positive_data
 
 
 def test_range_inclusive():
-    min_ = datetime(2022, 1, 1)
-    max_ = datetime(2023, 1, 1)
+    min_ = date(2022, 1, 1)
+    max_ = date(2023, 1, 1)
 
-    field = DateTime(
+    field = Date(
         validate=Range(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         required=True,
     )
 
-    positive_data = field.positive()
+    positive_data = list(field.positive())
 
     assert min_ + field.get_step() in positive_data
     assert max_ - field.get_step() in positive_data
     assert None not in positive_data
     assert not has_data_type(positive_data, Missing)
 
 
 def test_range_default():
-    min_ = datetime(2022, 1, 1)
-    max_ = datetime(2023, 1, 1)
-    default = Unique()
+    min_ = date(2022, 1, 1)
+    max_ = date(2023, 1, 1)
+    default = date(1996, 12, 3)
 
-    field = DateTime(
+    field = Date(
         validate=Range(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         default=default,
     )
 
-    positive_data = field.positive()
+    positive_data = list(field.positive())
 
     assert min_ + field.get_step() in positive_data
     assert max_ - field.get_step() in positive_data
     assert None not in positive_data
     assert default in positive_data
 
 
 def test_equal():
-    comparable = Unique()
+    comparable = date(1996, 12, 3)
 
-    field = DateTime(
+    field = Date(
         validate=Equal(comparable=comparable)
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert comparable in field_values
     assert None in field_values
     assert has_data_type(field_values, Missing)
 
 
 def test_equal_allow_none_required():
-    comparable = Unique()
+    comparable = date(1996, 12, 3)
 
-    field = DateTime(
+    field = Date(
         validate=Equal(comparable=comparable),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert comparable in field_values
     assert None not in field_values
     assert not has_data_type(field_values, Missing)
 
 
 def test_equal_default():
-    comparable = Unique()
-    default = Unique()
+    comparable = date(1996, 12, 3)
+    default = date(2000, 12, 3)
 
-    field = DateTime(
+    field = Date(
         validate=Equal(comparable=comparable),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert default in field_values
     assert None not in field_values
 
 
 def test_one_of():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [
+        date(1996, 12, 3),
+        date(2000, 12, 3),
+        date(2002, 12, 3)
+    ]
 
-    field = DateTime(
+    field = Date(
         validate=OneOf(choices=choices),
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     for value in choices:
         assert value in field_values
 
     assert None in field_values
     assert has_data_type(field_values, Missing)
 
 
 def test_one_of_allow_none_required():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [
+        date(1996, 12, 3),
+        date(2000, 12, 3),
+        date(2002, 12, 3)
+    ]
 
-    field = DateTime(
+    field = Date(
         validate=OneOf(choices=choices),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     for value in choices:
         assert value in field_values
 
     assert None not in field_values
     assert not has_data_type(field_values, Missing)
 
 
 def test_one_of_default():
-    choices = [Unique(), Unique(), Unique()]
-    default = Unique()
+    choices = [
+        date(1996, 12, 3),
+        date(2000, 12, 3),
+        date(2002, 12, 3)
+    ]
+    default = date(1991, 12, 3)
 
-    field = DateTime(
+    field = Date(
         validate=OneOf(choices=choices),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     for value in choices:
         assert value in field_values
 
     assert None not in field_values
     assert default in field_values
```

### Comparing `sgen-1.0.1/tests/test_float_negative.py` & `sgen-1.0.2/tests/test_string_positive.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,205 +1,214 @@
+from uuid import uuid4
+
 from tests import has_data_type, Unique
-from fields import Float
-from utils import Missing
-from validate import Range, Equal, OneOf
+from sgen.fields import String
+from sgen.utils import Missing
+from sgen.validate import Length, Equal, OneOf
 
 
-def test_float():
-    field = Float()
+def test_string():
+    field = String()
 
-    negative_values = field.negative()
+    positive_values = list(field.positive())
 
-    assert len(negative_values) == 1
-    assert not isinstance(negative_values[0], float)
+    assert len(positive_values) == 3
 
+    assert has_data_type(positive_values, str)
+    assert has_data_type(positive_values, type(None))
+    assert has_data_type(positive_values, Missing)
 
-def test_allow_none():
-    field = Float(allow_none=False)
 
-    assert None in field.negative()
+def test_not_allow_none():
+    field = String(allow_none=False)
 
+    positive_values = list(field.positive())
 
-def test_required():
-    field = Float(required=True)
+    assert None not in positive_values
 
-    assert has_data_type(field.negative(), Missing)
 
+def test_default():
+    default = uuid4().hex
+    field = String(default=default)
 
-def test_negative_data_from():
-    def negative_data_from():
-        return 'a', 333.44, None, Missing
+    assert default in list(field.positive())
 
-    field = Float(negative_data_from=negative_data_from)
 
-    assert field.negative() == list(negative_data_from())
+def test_required():
+    field = String(required=True)
 
+    assert not has_data_type(list(field.positive()), Missing)
 
-# =================================================
-# Тесты на взаимодействие типа Float с валидаторами
-# =================================================
 
+def test_positive_data_from():
+    def positive_data_generator():
+        return 'a', '1', None, Missing
 
-def test_range():
-    min_ = -673.94
-    max_ = 98.01
+    field = String(positive_data_from=positive_data_generator)
+
+    assert list(field.positive()) == list(positive_data_generator())
 
-    field = Float(
-        validate=Range(
-            min=min_, max=max_
-        )
-    )
 
-    negative_data = field.negative()
+# ==================================================
+# Тесты на взаимодействие типа String с валидаторами
+# ==================================================
 
-    assert min_ - 0.01 in negative_data
-    assert max_ + 0.01 in negative_data
 
+def test_length():
+    min_ = 999
+    max_ = 1111
 
-def test_range_inclusive():
-    min_ = -673.94
-    max_ = 98.01
+    field = String(validate=Length(min=min_, max=max_))
 
-    field = Float(
-        validate=Range(
+    for value in list(field.positive()):
+        if isinstance(value, str):
+            assert len(value) in [min_, max_]
+
+
+def test_length_allow_none_required():
+    min_ = 999
+    max_ = 1111
+
+    field = String(
+        validate=Length(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         required=True,
     )
 
-    negative_data = field.negative()
+    field_values = list(field.positive())
 
-    assert min_ in negative_data
-    assert max_ in negative_data
-    assert None in negative_data
-    assert has_data_type(negative_data, Missing)
+    for value in field_values:
+        if isinstance(value, str):
+            assert len(value) in [min_ + 1, max_ - 1]
+
+    assert None not in field_values
+    assert not has_data_type(field_values, Missing)
 
 
-def test_range_default():
-    min_ = -673.94
-    max_ = 98.01
+def test_length_default():
+    min_ = 999
+    max_ = 1111
     default = Unique()
 
-    field = Float(
-        validate=Range(
+    field = String(
+        validate=Length(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         default=default,
     )
 
-    negative_data = field.negative()
+    field_values = list(field.positive())
 
-    assert min_ in negative_data
-    assert max_ in negative_data
-    assert None in negative_data
-    assert default not in negative_data
+    for value in field_values:
+        if isinstance(value, str):
+            assert len(value) in [min_ + 1, max_ - 1]
+
+    assert None not in field_values
+    assert default in field_values
 
 
 def test_equal():
-    comparable = Unique()
+    comparable = 'str_text'
 
-    field = Float(
+    field = String(
         validate=Equal(comparable=comparable)
     )
 
-    field_values = field.negative()
+    field_values = list(field.positive())
 
-    assert comparable not in field_values
-    assert None not in field_values
-    assert has_data_type(field_values, str)
+    assert comparable in field_values
+    assert None in field_values
+    assert has_data_type(field_values, Missing)
 
 
 def test_equal_allow_none_required():
-    comparable = Unique()
+    comparable = 'str_text'
 
-    field = Float(
+    field = String(
         validate=Equal(comparable=comparable),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.negative()
+    field_values = list(field.positive())
 
-    assert comparable not in field_values
-    assert None in field_values
-    assert has_data_type(field_values, str)
-    assert has_data_type(field_values, Missing)
+    assert comparable in field_values
+    assert None not in field_values
+    assert not has_data_type(field_values, Missing)
 
 
 def test_equal_default():
-    comparable = Unique()
-    default = Unique()
+    comparable = 'str_text'
+    default = 'str_text_def'
 
-    field = Float(
+    field = String(
         validate=Equal(comparable=comparable),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.negative()
+    field_values = list(field.positive())
 
-    assert None in field_values
-    assert default not in field_values
+    assert default in field_values
+    assert None not in field_values
 
 
 def test_one_of():
-    choices = [Unique(), Unique(), Unique()]
+    choices = ['a_1', 'a_2', 'a_3']
 
-    field = Float(
+    field = String(
         validate=OneOf(choices=choices),
     )
 
-    field_values = field.negative()
+    field_values = list(field.positive())
 
     for value in choices:
-        assert value not in field_values
+        assert value in field_values
 
-    assert None not in field_values
-    assert has_data_type(field_values, str)
-    assert not has_data_type(field_values, Missing)
+    assert None in field_values
+    assert has_data_type(field_values, Missing)
 
 
 def test_one_of_allow_none_required():
-    choices = [Unique(), Unique(), Unique()]
+    choices = ['a_1', 'a_2', 'a_3']
 
-    field = Float(
+    field = String(
         validate=OneOf(choices=choices),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.negative()
+    field_values = list(field.positive())
 
     for value in choices:
-        assert value not in field_values
+        assert value in field_values
 
-    assert None in field_values
-    assert has_data_type(field_values, str)
-    assert has_data_type(field_values, Missing)
+    assert None not in field_values
+    assert not has_data_type(field_values, Missing)
 
 
 def test_one_of_default():
-    choices = [Unique(), Unique(), Unique()]
-    default = Unique()
+    choices = ['a_1', 'a_2', 'a_3']
+    default = 'str_text_def'
 
-    field = Float(
+    field = String(
         validate=OneOf(choices=choices),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.negative()
+    field_values = list(field.positive())
 
     for value in choices:
-        assert value not in field_values
+        assert value in field_values
 
-    assert has_data_type(field_values, str)
-    assert None in field_values
-    assert default not in field_values
+    assert None not in field_values
+    assert default in field_values
```

### Comparing `sgen-1.0.1/tests/test_float_positive.py` & `sgen-1.0.2/tests/test_float_positive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from tests import has_data_type, Unique
-from fields import Float
-from utils import Missing
-from validate import Range, Equal, OneOf
+from tests import has_data_type
+from sgen.fields import Float
+from sgen.utils import Missing
+from sgen.validate import Range, Equal, OneOf
 
 
 def test_float():
     field = Float()
 
-    positive_values = field.positive()
+    positive_values = list(field.positive())
 
     assert len(positive_values) == 3
 
     assert has_data_type(positive_values, float)
     assert has_data_type(positive_values, type(None))
     assert has_data_type(positive_values, Missing)
 
 
 def test_allow_none():
     field = Float(allow_none=False)
 
-    assert None not in field.positive()
+    assert None not in list(field.positive())
 
 
 def test_required():
     field = Float(required=True)
 
-    assert not has_data_type(field.positive(), Missing)
+    assert not has_data_type(list(field.positive()), Missing)
 
 
 def test_default():
     default = 1.23456789
     field = Float(default=default)
 
-    assert default in field.positive()
+    assert default in list(field.positive())
 
 
 def test_positive_data_from():
     def positive_data_generator():
         return 1.0, -9999.9999
 
     field = Float(positive_data_from=positive_data_generator)
 
-    assert field.positive() == list(positive_data_generator())
+    assert list(field.positive()) == list(positive_data_generator())
 
 
 # =================================================
 # Тесты на взаимодействие типа Float с валидаторами
 # =================================================
 
 
@@ -55,15 +55,15 @@
 
     field = Float(
         validate=Range(
             min=min_, max=max_
         )
     )
 
-    positive_data = field.positive()
+    positive_data = list(field.positive())
 
     assert min_ in positive_data
     assert max_ in positive_data
 
 
 def test_range_inclusive():
     min_ = -999.74
@@ -76,136 +76,136 @@
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         required=True,
     )
 
-    positive_data = field.positive()
+    positive_data = list(field.positive())
 
     assert min_ + 0.01 in positive_data
     assert max_ - 0.01 in positive_data
     assert None not in positive_data
     assert not has_data_type(positive_data, Missing)
 
 
 def test_range_default():
     min_ = -999.74
     max_ = 998.39
-    default = Unique()
+    default = 38.1678
 
     field = Float(
         validate=Range(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         default=default,
     )
 
-    positive_data = field.positive()
+    positive_data = list(field.positive())
 
     assert min_ + 0.01 in positive_data
     assert max_ - 0.01 in positive_data
     assert None not in positive_data
     assert default in positive_data
 
 
 def test_equal():
-    comparable = Unique()
+    comparable = 38.1678
 
     field = Float(
         validate=Equal(comparable=comparable)
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert comparable in field_values
     assert None in field_values
     assert has_data_type(field_values, Missing)
 
 
 def test_equal_allow_none_required():
-    comparable = Unique()
+    comparable = 38.1678
 
     field = Float(
         validate=Equal(comparable=comparable),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert comparable in field_values
     assert None not in field_values
     assert not has_data_type(field_values, Missing)
 
 
 def test_equal_default():
-    comparable = Unique()
-    default = Unique()
+    comparable = 38.1678
+    default = 16.16
 
     field = Float(
         validate=Equal(comparable=comparable),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     assert default in field_values
     assert None not in field_values
 
 
 def test_one_of():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [1.1, 2.2, 3.3]
 
     field = Float(
         validate=OneOf(choices=choices),
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     for value in choices:
         assert value in field_values
 
     assert None in field_values
     assert has_data_type(field_values, Missing)
 
 
 def test_one_of_allow_none_required():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [1.1, 2.2, 3.3]
 
     field = Float(
         validate=OneOf(choices=choices),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     for value in choices:
         assert value in field_values
 
     assert None not in field_values
     assert not has_data_type(field_values, Missing)
 
 
 def test_one_of_default():
-    choices = [Unique(), Unique(), Unique()]
-    default = Unique()
+    choices = [1.1, 2.2, 3.3]
+    default = 38.1678
 
     field = Float(
         validate=OneOf(choices=choices),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.positive()
+    field_values = list(field.positive())
 
     for value in choices:
         assert value in field_values
 
     assert None not in field_values
     assert default in field_values
```

### Comparing `sgen-1.0.1/tests/test_integer_negative.py` & `sgen-1.0.2/tests/test_date_negative.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,205 +1,222 @@
-from tests import has_data_type, Unique
-from fields import Integer
-from validate import Range, Equal, OneOf
-from utils import Missing
+from datetime import datetime, date
 
+from tests import has_data_type
+from sgen.fields import Date
+from sgen.utils import Missing
+from sgen.validate import Range, Equal, OneOf
 
-def test_int():
-    field = Integer()
 
-    negative_values = field.negative()
+def test_date():
+    field = Date()
+
+    negative_values = list(field.negative())
 
     assert len(negative_values) == 1
-    assert not isinstance(negative_values[0], int)
+    assert not isinstance(negative_values[0], date)
 
 
 def test_allow_none():
-    field = Integer(allow_none=False)
+    field = Date(allow_none=False)
 
-    assert None in field.negative()
+    assert None in list(field.negative())
 
 
 def test_required():
-    field = Integer(required=True)
+    field = Date(required=True)
+
+    # src.sgen.utils.Missing
+    # sgen.utils.Missing
 
-    assert has_data_type(field.negative(), Missing)
+    assert has_data_type(list(field.negative()), Missing)
 
 
 def test_negative_data_from():
     def negative_data_from():
-        return 'a', 666, None, Missing
+        return None, Missing
 
-    field = Integer(negative_data_from=negative_data_from)
+    field = Date(negative_data_from=negative_data_from)
 
-    assert field.negative() == list(negative_data_from())
+    assert list(field.negative()) == list(negative_data_from())
 
 
-# ===================================================
-# Тесты на взаимодействие типа Integer с валидаторами
-# ===================================================
+# =================================================
+# Тесты на взаимодействие типа Float с валидаторами
+# =================================================
 
 
 def test_range():
-    min_ = -998
-    max_ = 649
+    min_ = date(2022, 1, 1)
+    max_ = date(2023, 1, 1)
 
-    field = Integer(
+    field = Date(
         validate=Range(
             min=min_, max=max_
         )
     )
 
-    negative_data = field.negative()
+    negative_data = list(field.negative())
 
-    assert min_ - 1 in negative_data
-    assert max_ + 1 in negative_data
+    assert min_ - field.get_step() in negative_data
+    assert max_ + field.get_step() in negative_data
 
 
 def test_range_inclusive():
-    min_ = -998
-    max_ = 649
+    min_ = date(2022, 1, 1)
+    max_ = date(2023, 1, 1)
 
-    field = Integer(
+    field = Date(
         validate=Range(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         required=True,
     )
 
-    negative_data = field.negative()
+    negative_data = list(field.negative())
 
     assert min_ in negative_data
     assert max_ in negative_data
     assert None in negative_data
     assert has_data_type(negative_data, Missing)
 
 
 def test_range_default():
-    min_ = -998
-    max_ = 649
-    default = Unique()
+    min_ = datetime(2022, 1, 1)
+    max_ = datetime(2023, 1, 1)
+    default = date(1996, 12, 3)
 
-    field = Integer(
+    field = Date(
         validate=Range(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         default=default,
     )
 
-    negative_data = field.negative()
+    negative_data = list(field.negative())
 
     assert min_ in negative_data
     assert max_ in negative_data
     assert None in negative_data
     assert default not in negative_data
 
 
 def test_equal():
-    comparable = Unique()
+    comparable = date(1996, 12, 3)
 
-    field = Integer(
+    field = Date(
         validate=Equal(comparable=comparable)
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert comparable not in field_values
     assert None not in field_values
     assert has_data_type(field_values, str)
 
 
 def test_equal_allow_none_required():
-    comparable = Unique()
+    comparable = date(1996, 12, 3)
 
-    field = Integer(
+    field = Date(
         validate=Equal(comparable=comparable),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     assert comparable not in field_values
     assert None in field_values
     assert has_data_type(field_values, str)
     assert has_data_type(field_values, Missing)
 
 
 def test_equal_default():
-    comparable = Unique()
-    default = Unique()
+    comparable = date(1996, 12, 3)
+    default = date(2000, 12, 3)
 
-    field = Integer(
+    field = Date(
         validate=Equal(comparable=comparable),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
-    assert default not in field_values
     assert None in field_values
+    assert default not in field_values
 
 
 def test_one_of():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [
+        date(1996, 12, 3),
+        date(2000, 12, 3),
+        date(2002, 12, 3)
+    ]
 
-    field = Integer(
+    field = Date(
         validate=OneOf(choices=choices),
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     for value in choices:
         assert value not in field_values
 
     assert None not in field_values
     assert has_data_type(field_values, str)
     assert not has_data_type(field_values, Missing)
 
 
 def test_one_of_allow_none_required():
-    choices = [Unique(), Unique(), Unique()]
+    choices = [
+        date(1996, 12, 3),
+        date(2000, 12, 3),
+        date(2002, 12, 3)
+    ]
 
-    field = Integer(
+    field = Date(
         validate=OneOf(choices=choices),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     for value in choices:
         assert value not in field_values
 
     assert None in field_values
     assert has_data_type(field_values, str)
     assert has_data_type(field_values, Missing)
 
 
 def test_one_of_default():
-    choices = [Unique(), Unique(), Unique()]
-    default = Unique()
+    choices = [
+        date(1996, 12, 3),
+        date(2000, 12, 3),
+        date(2002, 12, 3)
+    ]
+    default = date(1992, 12, 3)
 
-    field = Integer(
+    field = Date(
         validate=OneOf(choices=choices),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.negative()
+    field_values = list(field.negative())
 
     for value in choices:
         assert value not in field_values
 
-    assert None in field_values
     assert has_data_type(field_values, str)
+    assert None in field_values
     assert default not in field_values
```

### Comparing `sgen-1.0.1/tests/test_integet_positive.py` & `sgen-1.0.2/tests/test_string_negative.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,208 +1,205 @@
 from tests import has_data_type, Unique
-from fields import Integer
-from validate import Range, Equal, OneOf
-from utils import Missing
+from sgen.fields import String
+from sgen.utils import Missing
+from sgen.validate import Length, Equal, OneOf
 
 
-def test_integer():
-    field = Integer()
+def test_string():
+    field = String()
 
-    positive_values = field.positive()
+    negative_values = list(field.negative())
 
-    assert len(positive_values) == 3
+    assert len(negative_values) == 1
+    assert isinstance(negative_values[0], int)
 
-    assert has_data_type(positive_values, int)
-    assert has_data_type(positive_values, type(None))
-    assert has_data_type(positive_values, Missing)
 
+def test_not_allow_none():
+    field = String(allow_none=False)
 
-def test_allow_none():
-    field = Integer(allow_none=False)
-
-    assert None not in field.positive()
+    assert None in list(field.negative())
 
 
 def test_required():
-    field = Integer(required=True)
-
-    assert not has_data_type(field.positive(), Missing)
+    field = String(required=True)
 
+    assert has_data_type(list(field.negative()), Missing)
 
-def test_default():
-    default = -9999
-    field = Integer(default=default)
 
-    assert default in field.positive()
+def test_negative_data_from():
+    def negative_data_from():
+        return 'a', 666, None, Missing
 
+    field = String(negative_data_from=negative_data_from)
 
-def test_positive_data_from():
-    def positive_data_generator():
-        return 1, None, -999
+    assert list(field.negative()) == list(negative_data_from())
 
-    field = Integer(positive_data_from=positive_data_generator)
 
-    assert field.positive() == list(positive_data_generator())
+# ==================================================
+# Тесты на взаимодействие типа String с валидаторами
+# ==================================================
 
 
-# ===================================================
-# Тесты на взаимодействие типа Integer с валидаторами
-# ===================================================
+def test_length():
+    min_ = 999
+    max_ = 1111
 
+    field = String(validate=Length(min=min_, max=max_))
 
-def test_range():
-    min_ = -999
-    max_ = 998
-    field = Integer(
-        validate=Range(
-            min=min_, max=max_
-        )
-    )
-    positive_data = field.positive()
-    assert min_ in positive_data
-    assert max_ in positive_data
+    for value in list(field.negative()):
+        if isinstance(value, str):
+            assert len(value) in [min_ - 1, max_ + 1]
 
 
-def test_range_allow_none_required():
-    min_ = -999
-    max_ = 998
+def test_length_allow_none_required():
+    min_ = 999
+    max_ = 1111
 
-    field = Integer(
-        validate=Range(
+    field = String(
+        validate=Length(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         required=True,
     )
 
-    positive_data = field.positive()
+    field_values = list(field.negative())
+
+    for value in field_values:
+        if isinstance(value, str):
+            assert len(value) in [min_, max_]
 
-    assert min_ + 1 in positive_data
-    assert max_ - 1 in positive_data
-    assert None not in positive_data
-    assert not has_data_type(positive_data, Missing)
+    assert None in field_values
+    assert has_data_type(field_values, Missing)
 
 
-def test_range_inclusive():
-    min_ = -999
-    max_ = 998
+def test_length_default():
+    min_ = 999
+    max_ = 1111
     default = Unique()
 
-    field = Integer(
-        validate=Range(
+    field = String(
+        validate=Length(
             min=min_,
             max=max_,
             min_inclusive=False,
             max_inclusive=False,
         ),
         allow_none=False,
         default=default,
     )
 
-    positive_data = field.positive()
+    field_values = list(field.negative())
 
-    assert min_ + 1 in positive_data
-    assert max_ - 1 in positive_data
-    assert None not in positive_data
-    assert default in positive_data
+    for value in field_values:
+        if isinstance(value, str):
+            assert len(value) in [min_, max_]
+
+    assert None in field_values
+    assert default not in field_values
 
 
 def test_equal():
-    comparable = Unique()
+    comparable = 'str_text'
 
-    field = Integer(
+    field = String(
         validate=Equal(comparable=comparable)
     )
 
-    field_values = field.positive()
+    field_values = list(field.negative())
 
-    assert comparable in field_values
-    assert None in field_values
-    assert has_data_type(field_values, Missing)
+    assert comparable not in field_values
+    assert None not in field_values
+    assert has_data_type(field_values, int)
 
 
 def test_equal_allow_none_required():
-    comparable = Unique()
+    comparable = 'str_text'
 
-    field = Integer(
+    field = String(
         validate=Equal(comparable=comparable),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.positive()
+    field_values = list(field.negative())
 
-    assert comparable in field_values
-    assert None not in field_values
-    assert not has_data_type(field_values, Missing)
+    assert comparable not in field_values
+    assert None in field_values
+    assert has_data_type(field_values, int)
+    assert has_data_type(field_values, type(None))
+    assert has_data_type(field_values, Missing)
 
 
 def test_equal_default():
-    comparable = Unique()
-    default = Unique()
+    comparable = 'str_text'
+    default = 'str_text_def'
 
-    field = Integer(
+    field = String(
         validate=Equal(comparable=comparable),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.positive()
+    field_values = list(field.negative())
 
-    assert default in field_values
-    assert None not in field_values
+    assert default not in field_values
+    assert None in field_values
 
 
 def test_one_of():
-    choices = [Unique(), Unique(), Unique()]
+    choices = ['a_1', 'a_2', 'a_3']
 
-    field = Integer(
+    field = String(
         validate=OneOf(choices=choices),
     )
 
-    field_values = field.positive()
+    field_values = list(field.negative())
 
     for value in choices:
-        assert value in field_values
+        assert value not in field_values
 
-    assert None in field_values
-    assert has_data_type(field_values, Missing)
+    assert None not in field_values
+    assert has_data_type(field_values, int)
+    assert not has_data_type(field_values, Missing)
 
 
 def test_one_of_allow_none_required():
-    choices = [Unique(), Unique(), Unique()]
+    choices = ['a_1', 'a_2', 'a_3']
 
-    field = Integer(
+    field = String(
         validate=OneOf(choices=choices),
         allow_none=False,
         required=True,
     )
 
-    field_values = field.positive()
+    field_values = list(field.negative())
 
     for value in choices:
-        assert value in field_values
+        assert value not in field_values
 
-    assert None not in field_values
-    assert not has_data_type(field_values, Missing)
+    assert None in field_values
+    assert has_data_type(field_values, int)
+    assert has_data_type(field_values, Missing)
 
 
 def test_one_of_default():
-    choices = [Unique(), Unique(), Unique()]
-    default = Unique()
+    choices = ['a_1', 'a_2', 'a_3']
+    default = 'str_text_def'
 
-    field = Integer(
+    field = String(
         validate=OneOf(choices=choices),
         allow_none=False,
         default=default,
     )
 
-    field_values = field.positive()
+    field_values = list(field.negative())
 
     for value in choices:
-        assert value in field_values
+        assert value not in field_values
 
-    assert None not in field_values
-    assert default in field_values
+    assert None in field_values
+    assert has_data_type(field_values, int)
+    assert default not in field_values
```

### Comparing `sgen-1.0.1/tests/test_nested_negative.py` & `sgen-1.0.2/tests/test_nested_negative.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from fields import (
+from sgen.fields import (
     Nested,
     String,
     Integer,
     Float,
     Boolean,
     Collection
 )
-from validate import (
+from sgen.validate import (
     Range,
-    Length,
     OneOf,
     NoneOf,
-    Equal,
 )
 from sgen import SGen
 
 
 def test_nested_simple():
     class Test(SGen):
         name = String()
@@ -23,33 +21,29 @@
         balance = Float()
         is_admin = Boolean()
 
     field = Nested(Test())
 
     datasets_from_sgen = list(field.negative())
 
-    assert len(datasets_from_sgen) == 136
+    assert len(datasets_from_sgen) == 135
 
 
 def test_nested_with_validators():
-    field_name = String(allow_none=False, default='Aboba', validate=Length(min=10, max=40))
     field_age = Integer(validate=Range(min=18, min_inclusive=False))
     field_balance = Float(allow_none=False, required=True, validate=OneOf(choices=[1, 2, 3, 4, 5]))
     field_is_admin = Boolean(required=True)
     field_keys = Collection(data_type=Integer(), allow_none=False, required=True)
     field_address = String(validate=NoneOf(invalid_values=['Pepega street']))
-    field_car = String(validate=Equal(comparable='Jaguar XF'))
 
     class Test(SGen):
-        name = field_name
         age = field_age
         balance = field_balance
         is_admin = field_is_admin
         keys = field_keys
         address = field_address
-        car = field_car
 
     field = Nested(Test())
 
-    datasets_from_sgen = list(field.positive())
+    datasets_from_sgen = list(field.negative())
 
-    assert len(datasets_from_sgen) == 4860
+    assert len(datasets_from_sgen) == 1863
```

### Comparing `sgen-1.0.1/tests/test_nested_positive.py` & `sgen-1.0.2/tests/test_nested_positive.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from itertools import product
 
-from fields import (
+from sgen.fields import (
     Nested,
     String,
     Integer,
     Float,
     Boolean,
     Collection
 )
-from validate import (
+from sgen.validate import (
     Range,
     Length,
     OneOf,
     NoneOf,
     Equal,
 )
 from sgen import SGen
@@ -31,15 +31,15 @@
     datasets_from_system_library = list(product(
         String().positive(),
         Integer().positive(),
         Float().positive(),
         Boolean().positive(),
     ))
 
-    assert len(datasets_from_sgen) == len(datasets_from_system_library)
+    assert len(datasets_from_sgen) == len(datasets_from_system_library) + 2  # 2 = none + missing
 
 
 def test_nested_with_validators():
     field_name = String(allow_none=False, default='Aboba', validate=Length(min=10, max=40))
     field_age = Integer(validate=Range(min=18, min_inclusive=False))
     field_balance = Float(allow_none=False, required=True, validate=OneOf(choices=[1, 2, 3, 4, 5]))
     field_is_admin = Boolean(required=True)
@@ -65,8 +65,8 @@
         field_balance.positive(),
         field_is_admin.positive(),
         field_keys.positive(),
         field_address.positive(),
         field_car.positive(),
     ))
 
-    assert len(datasets_from_sgen) == len(datasets_from_system_library)
+    assert len(datasets_from_sgen) == len(datasets_from_system_library) + 2  # 2 = none + missing
```

