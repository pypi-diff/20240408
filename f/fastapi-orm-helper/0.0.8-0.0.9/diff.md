# Comparing `tmp/fastapi_orm_helper-0.0.8.tar.gz` & `tmp/fastapi_orm_helper-0.0.9.tar.gz`

## Comparing `fastapi_orm_helper-0.0.8.tar` & `fastapi_orm_helper-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/build_and_publish.sh
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/build_and_test.sh
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/requirements.txt
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/tox.ini
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/fastapi_orm_helper/__init__.py
--rw-r--r--   0        0        0    13444 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/fastapi_orm_helper/base_repository.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/fastapi_orm_helper/dependencies/pagination.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/fastapi_orm_helper/entity_mappers/entity_mapper.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/fastapi_orm_helper/entity_mappers/entity_reverse_mapper.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/fastapi_orm_helper/enums/join_type_enum.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/fastapi_orm_helper/helpers/deep_pluck.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/fastapi_orm_helper/helpers/join.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/LICENSE
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/build_and_publish.sh
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/build_and_test.sh
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/tox.ini
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/fastapi_orm_helper/__init__.py
+-rw-r--r--   0        0        0    13444 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/fastapi_orm_helper/base_repository.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/fastapi_orm_helper/dependencies/pagination.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/fastapi_orm_helper/entity_mappers/entity_mapper.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/fastapi_orm_helper/entity_mappers/entity_reverse_mapper.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/fastapi_orm_helper/enums/join_type_enum.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/fastapi_orm_helper/helpers/deep_pluck.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/fastapi_orm_helper/helpers/join.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/LICENSE
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 fastapi_orm_helper-0.0.9/PKG-INFO
```

### Comparing `fastapi_orm_helper-0.0.8/.github/workflows/publish.yaml` & `fastapi_orm_helper-0.0.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_orm_helper-0.0.8/fastapi_orm_helper/base_repository.py` & `fastapi_orm_helper-0.0.9/fastapi_orm_helper/base_repository.py`

 * *Files identical despite different names*

### Comparing `fastapi_orm_helper-0.0.8/fastapi_orm_helper/entity_mappers/entity_mapper.py` & `fastapi_orm_helper-0.0.9/fastapi_orm_helper/entity_mappers/entity_mapper.py`

 * *Files identical despite different names*

### Comparing `fastapi_orm_helper-0.0.8/fastapi_orm_helper/entity_mappers/entity_reverse_mapper.py` & `fastapi_orm_helper-0.0.9/fastapi_orm_helper/entity_mappers/entity_reverse_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         for mapper in self.mappers:
             if '*' in mapper['entity_id_key']:
                 for item in self.data:
                     keys = mapper['entity_id_key'].split('.*.')
                     new_data = item
                     for index, key in enumerate(keys):
                         if index == len(keys) - 1:
-                            self.set_value_to_objects(entities, new_data, key, mapper['reverse_id'], mapper['map_key'])
+                            self.set_value_to_objects(entities, new_data, key, mapper['reverse_id'], mapper['map_key'], mapper['is_mapped_data_list'])
                             break
                         new_data = get(new_data, key)
                         if new_data is None:
                             break
             else:
                 self.set_value_to_objects(
                     entities, self.data, mapper['entity_id_key'], mapper['reverse_id'], mapper['map_key'], mapper['is_mapped_data_list']
```

### Comparing `fastapi_orm_helper-0.0.8/.gitignore` & `fastapi_orm_helper-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_orm_helper-0.0.8/LICENSE` & `fastapi_orm_helper-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_orm_helper-0.0.8/pyproject.toml` & `fastapi_orm_helper-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_orm_helper"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Dzung Nguyen", email="dung@megatron-solutions.com" },
 ]
 description = "FastAPI ORM Helper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fastapi_orm_helper-0.0.8/PKG-INFO` & `fastapi_orm_helper-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_orm_helper
-Version: 0.0.8
+Version: 0.0.9
 Summary: FastAPI ORM Helper
 Project-URL: Homepage, https://github.com/megatron-global/fastapi-orm-helper
 Project-URL: Bug Tracker, https://github.com/megatron-global/fastapi-orm-helper/issues
 Author-email: Dzung Nguyen <dung@megatron-solutions.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

