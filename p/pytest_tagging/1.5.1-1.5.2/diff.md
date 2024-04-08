# Comparing `tmp/pytest_tagging-1.5.1.tar.gz` & `tmp/pytest_tagging-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_tagging-1.5.1.tar", max compression
+gzip compressed data, was "pytest_tagging-1.5.2.tar", max compression
```

## Comparing `pytest_tagging-1.5.1.tar` & `pytest_tagging-1.5.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-04-07 20:19:01.447003 pytest_tagging-1.5.1/LICENSE
--rw-r--r--   0        0        0     2275 2024-04-07 20:19:01.447003 pytest_tagging-1.5.1/README.md
--rw-r--r--   0        0        0     1518 2024-04-07 20:19:01.447003 pytest_tagging-1.5.1/pyproject.toml
--rw-r--r--   0        0        0       70 2024-04-07 20:19:01.447003 pytest_tagging-1.5.1/pytest_tagging/__init__.py
--rw-r--r--   0        0        0       82 2024-04-07 20:19:01.447003 pytest_tagging-1.5.1/pytest_tagging/choices.py
--rw-r--r--   0        0        0     4259 2024-04-07 20:19:01.447003 pytest_tagging-1.5.1/pytest_tagging/plugin.py
--rw-r--r--   0        0        0     2762 2024-04-07 20:19:01.447003 pytest_tagging-1.5.1/pytest_tagging/selector.py
--rw-r--r--   0        0        0      959 2024-04-07 20:19:01.447003 pytest_tagging-1.5.1/pytest_tagging/utils.py
--rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 pytest_tagging-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-08 07:29:35.625097 pytest_tagging-1.5.2/LICENSE
+-rw-r--r--   0        0        0     2275 2024-04-08 07:29:35.625097 pytest_tagging-1.5.2/README.md
+-rw-r--r--   0        0        0     1518 2024-04-08 07:29:35.625097 pytest_tagging-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-04-08 07:29:35.625097 pytest_tagging-1.5.2/pytest_tagging/__init__.py
+-rw-r--r--   0        0        0       82 2024-04-08 07:29:35.625097 pytest_tagging-1.5.2/pytest_tagging/choices.py
+-rw-r--r--   0        0        0     4259 2024-04-08 07:29:35.625097 pytest_tagging-1.5.2/pytest_tagging/plugin.py
+-rw-r--r--   0        0        0     2753 2024-04-08 07:29:35.625097 pytest_tagging-1.5.2/pytest_tagging/selector.py
+-rw-r--r--   0        0        0      959 2024-04-08 07:29:35.625097 pytest_tagging-1.5.2/pytest_tagging/utils.py
+-rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 pytest_tagging-1.5.2/PKG-INFO
```

### Comparing `pytest_tagging-1.5.1/LICENSE` & `pytest_tagging-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_tagging-1.5.1/README.md` & `pytest_tagging-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_tagging-1.5.1/pyproject.toml` & `pytest_tagging-1.5.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest_tagging"
-version = "1.5.1"
+version = "1.5.2"
 description = "a pytest plugin to tag tests"
 authors = ["Sergio Castillo <s.cast.lara@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/scastlara/pytest-tagging"
 repository = "https://github.com/scastlara/pytest-tagging"
 
@@ -57,15 +57,15 @@
 
 [tool.coverage.report]
 source = "pytest_tagging"
 fail_under = 90
 exclude_lines = ["if TYPE_CHECKING:", "pragma: no cover"]
 
 [tool.commitizen]
-version = "1.5.1"
+version = "1.5.2"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytest_tagging-1.5.1/pytest_tagging/plugin.py` & `pytest_tagging-1.5.2/pytest_tagging/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_tagging-1.5.1/pytest_tagging/selector.py` & `pytest_tagging-1.5.2/pytest_tagging/selector.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,36 +33,36 @@
         return set(tags) or set()
 
     def get_items_to_run(self, tags_to_run, tags_to_exclude, items):
         """Given tags and the pytest items collected, return two sets of items:
         - Those that should be selected.
         - Those that should be deselected.
         """
-        selected_items = set()
-        deselected_items = set()
+        selected_items = []
+        deselected_items = []
         if is_tags_empty(self.config.tags) or (is_tags_option_provided(self.config.tags) and not tags_to_run):
             # No tags match the conditions to run
             # or we just passed an empty `--tags` options to see them all.
-            deselected_items.update(items)
+            deselected_items.extend(items)
         else:
             # Some tags were selected
             for item in items:
                 test_tags = get_tags_from_item(item)
                 # Excluding tags takes precendence ove any selection.
                 if test_tags & tags_to_exclude:
-                    deselected_items.add(item)
+                    deselected_items.append(item)
                 elif (
                     not is_tags_option_provided(self.config.tags)
                     or (self.config.operand is OperandChoices.OR and test_tags & tags_to_run)
                     or (self.config.operand is OperandChoices.AND and tags_to_run <= test_tags)
                 ):
-                    selected_items.add(item)
+                    selected_items.append(item)
                 else:
-                    deselected_items.add(item)
-        return list(selected_items), list(deselected_items)
+                    deselected_items.append(item)
+        return selected_items, deselected_items
 
 
 def get_tags_from_item(item) -> set[str]:
     return set(item.get_closest_marker("tags").args) if item.get_closest_marker("tags") else set()
 
 
 def is_tags_empty(tags: list[str] | None) -> bool:
```

### Comparing `pytest_tagging-1.5.1/pytest_tagging/utils.py` & `pytest_tagging-1.5.2/pytest_tagging/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_tagging-1.5.1/PKG-INFO` & `pytest_tagging-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_tagging
-Version: 1.5.1
+Version: 1.5.2
 Summary: a pytest plugin to tag tests
 Home-page: https://github.com/scastlara/pytest-tagging
 License: MIT
 Author: Sergio Castillo
 Author-email: s.cast.lara@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

