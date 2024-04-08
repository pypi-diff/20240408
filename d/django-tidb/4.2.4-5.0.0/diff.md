# Comparing `tmp/django-tidb-4.2.4.tar.gz` & `tmp/django-tidb-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tidb-4.2.4.tar", last modified: Sun Apr  7 06:32:21 2024, max compression
+gzip compressed data, was "django-tidb-5.0.0.tar", last modified: Mon Apr  8 11:11:02 2024, max compression
```

## Comparing `django-tidb-4.2.4.tar` & `django-tidb-5.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:32:21.771673 django-tidb-4.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-04-07 06:32:17.000000 django-tidb-4.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-04-07 06:32:21.771673 django-tidb-4.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-07 06:32:17.000000 django-tidb-4.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:32:21.767673 django-tidb-4.2.4/django_tidb/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:32:21.771673 django-tidb-4.2.4/django_tidb/fields/
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/fields/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9238 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:32:21.771673 django-tidb-4.2.4/django_tidb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-04-07 06:32:21.000000 django-tidb-4.2.4/django_tidb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-07 06:32:21.000000 django-tidb-4.2.4/django_tidb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:32:21.000000 django-tidb-4.2.4/django_tidb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 06:32:21.000000 django-tidb-4.2.4/django_tidb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 06:32:21.000000 django-tidb-4.2.4/django_tidb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-07 06:32:17.000000 django-tidb-4.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:32:21.771673 django-tidb-4.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:11:02.763212 django-tidb-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-04-08 11:10:55.000000 django-tidb-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-08 11:11:02.763212 django-tidb-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-08 11:10:55.000000 django-tidb-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:11:02.759212 django-tidb-5.0.0/django_tidb/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 11:10:55.000000 django-tidb-5.0.0/django_tidb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-08 11:10:55.000000 django-tidb-5.0.0/django_tidb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17772 2024-04-08 11:10:55.000000 django-tidb-5.0.0/django_tidb/features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:11:02.763212 django-tidb-5.0.0/django_tidb/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-08 11:10:55.000000 django-tidb-5.0.0/django_tidb/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-08 11:10:55.000000 django-tidb-5.0.0/django_tidb/fields/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-08 11:10:55.000000 django-tidb-5.0.0/django_tidb/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-08 11:10:55.000000 django-tidb-5.0.0/django_tidb/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-08 11:10:55.000000 django-tidb-5.0.0/django_tidb/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-08 11:10:55.000000 django-tidb-5.0.0/django_tidb/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-08 11:10:55.000000 django-tidb-5.0.0/django_tidb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:11:02.763212 django-tidb-5.0.0/django_tidb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-08 11:11:02.000000 django-tidb-5.0.0/django_tidb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-08 11:11:02.000000 django-tidb-5.0.0/django_tidb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:11:02.000000 django-tidb-5.0.0/django_tidb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 11:11:02.000000 django-tidb-5.0.0/django_tidb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 11:11:02.000000 django-tidb-5.0.0/django_tidb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-08 11:10:55.000000 django-tidb-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:11:02.763212 django-tidb-5.0.0/setup.cfg
```

### Comparing `django-tidb-4.2.4/LICENSE` & `django-tidb-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.4/PKG-INFO` & `django-tidb-5.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: django-tidb
-Version: 4.2.4
+Version: 5.0.0
 Summary: Django backend for TiDB
 Author-email: Xiang Zhang <zhangxiang02@pingcap.com>, Di Wang <wangdi@pingcap.com>
 Project-URL: Homepage, https://github.com/pingcap/tidb
 Project-URL: Bug Reports, https://github.com/pingcap/django-tidb/issues
 Project-URL: Source, https://github.com/pingcap/django-tidb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: vector
 Requires-Dist: numpy~=1.0; extra == "vector"
 
 # TiDB dialect for Django
 
@@ -62,14 +61,15 @@
 
 To install django-tidb, you need to select the version that corresponds with your Django version. Please refer to the table below for guidance:
 
 > The minor release number of Django doesn't correspond to the minor release number of django-tidb. Use the latest minor release of each.
 
 |django|django-tidb|install command|
 |:----:|:---------:|:-------------:|
+|v5.0.x|v5.0.x|`pip install 'django-tidb>=5.0.0,<5.1.0'`|
 |v4.2.x|v4.2.x|`pip install 'django-tidb>=4.2.0,<4.3.0'`|
 |v4.1.x|v4.1.x|`pip install 'django-tidb>=4.1.0,<4.2.0'`|
 |v3.2.x|v3.2.x|`pip install 'django-tidb>=3.2.0,<3.3.0'`|
 
 ## Usage
 
 Set `'ENGINE': 'django_tidb'` in your settings to this:
@@ -209,16 +209,16 @@
 
 ```python
 Test.objects.alias(distance=CosineDistance('embedding', [3, 1, 2])).filter(distance__lt=5)
 ```
 
 ## Supported versions
 
-- TiDB 4.0 and newer
-- Django 3.2, 4.1 and 4.2
+- TiDB 5.0 and newer
+- Django 3.2, 4.1, 4.2 and 5.0
 - Python 3.6 and newer(must match Django's Python version requirement)
 
 ## Test
 
 create your virtualenv with:
 
 ```bash
@@ -234,14 +234,14 @@
 $ DJANGO_VERSION=3.2.12 python run_testing_worker.py
 ```
 
 ## Migrate from previous versions
 
 Releases on PyPi before 3.0.0 are published from repository https://github.com/blacktear23/django_tidb. This repository is a new implementation and released under versions from 3.0.0. No backwards compatibility is ensured. The most significant points are:
 
-- Only Django 3.2 and 4.0 are tested and supported.
 - Engine name is `django_tidb` instead of `django_tidb.tidb`.
 
 ## Known issues
 
 - TiDB before v6.6.0 does not support FOREIGN KEY constraints([#18209](https://github.com/pingcap/tidb/issues/18209)).
 - TiDB before v6.2.0 does not support SAVEPOINT([#6840](https://github.com/pingcap/tidb/issues/6840)).
+- TiDB has limited support for default value expressions, please refer to the [documentation](https://docs.pingcap.com/tidb/dev/data-type-default-values#specify-expressions-as-default-values).
```

### Comparing `django-tidb-4.2.4/README.md` & `django-tidb-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 To install django-tidb, you need to select the version that corresponds with your Django version. Please refer to the table below for guidance:
 
 > The minor release number of Django doesn't correspond to the minor release number of django-tidb. Use the latest minor release of each.
 
 |django|django-tidb|install command|
 |:----:|:---------:|:-------------:|
+|v5.0.x|v5.0.x|`pip install 'django-tidb>=5.0.0,<5.1.0'`|
 |v4.2.x|v4.2.x|`pip install 'django-tidb>=4.2.0,<4.3.0'`|
 |v4.1.x|v4.1.x|`pip install 'django-tidb>=4.1.0,<4.2.0'`|
 |v3.2.x|v3.2.x|`pip install 'django-tidb>=3.2.0,<3.3.0'`|
 
 ## Usage
 
 Set `'ENGINE': 'django_tidb'` in your settings to this:
@@ -184,16 +185,16 @@
 
 ```python
 Test.objects.alias(distance=CosineDistance('embedding', [3, 1, 2])).filter(distance__lt=5)
 ```
 
 ## Supported versions
 
-- TiDB 4.0 and newer
-- Django 3.2, 4.1 and 4.2
+- TiDB 5.0 and newer
+- Django 3.2, 4.1, 4.2 and 5.0
 - Python 3.6 and newer(must match Django's Python version requirement)
 
 ## Test
 
 create your virtualenv with:
 
 ```bash
@@ -209,14 +210,14 @@
 $ DJANGO_VERSION=3.2.12 python run_testing_worker.py
 ```
 
 ## Migrate from previous versions
 
 Releases on PyPi before 3.0.0 are published from repository https://github.com/blacktear23/django_tidb. This repository is a new implementation and released under versions from 3.0.0. No backwards compatibility is ensured. The most significant points are:
 
-- Only Django 3.2 and 4.0 are tested and supported.
 - Engine name is `django_tidb` instead of `django_tidb.tidb`.
 
 ## Known issues
 
 - TiDB before v6.6.0 does not support FOREIGN KEY constraints([#18209](https://github.com/pingcap/tidb/issues/18209)).
 - TiDB before v6.2.0 does not support SAVEPOINT([#6840](https://github.com/pingcap/tidb/issues/6840)).
+- TiDB has limited support for default value expressions, please refer to the [documentation](https://docs.pingcap.com/tidb/dev/data-type-default-values#specify-expressions-as-default-values).
```

### Comparing `django-tidb-4.2.4/django_tidb/__init__.py` & `django-tidb-5.0.0/django_tidb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # limitations under the License.
 
 # Check Django compatibility before other imports which may fail if the
 # wrong version of Django is installed.
 
 from .patch import monkey_patch
 
-__version__ = "4.2.4"
+__version__ = "5.0.0"
 
 
 monkey_patch()
```

### Comparing `django-tidb-4.2.4/django_tidb/base.py` & `django-tidb-5.0.0/django_tidb/base.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.4/django_tidb/features.py` & `django-tidb-5.0.0/django_tidb/features.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,30 +17,32 @@
     DatabaseFeatures as MysqlDatabaseFeatures,
 )
 from django.utils.functional import cached_property
 
 
 class DatabaseFeatures(MysqlDatabaseFeatures):
     has_select_for_update = True
+    has_native_uuid_field = False
     atomic_transactions = False
     supports_atomic_references_rename = False
     can_clone_databases = False
     can_rollback_ddl = False
     # Unsupported add column and foreign key in single statement
     # https://github.com/pingcap/tidb/issues/45474
     can_create_inline_fk = False
     order_by_nulls_first = True
     create_test_procedure_without_params_sql = None
     create_test_procedure_with_int_param_sql = None
     test_collations = {
         "ci": "utf8mb4_general_ci",
         "non_default": "utf8mb4_bin",
+        "virtual": "utf8mb4_general_ci",
     }
 
-    minimum_database_version = (4,)
+    minimum_database_version = (5,)
 
     @cached_property
     def supports_foreign_keys(self):
         if self.connection.tidb_version >= (6, 6, 0):
             return True
         return False
 
@@ -71,14 +73,16 @@
 
     @cached_property
     def django_test_skips(self):
         skips = {
             "This doesn't work on MySQL.": {
                 "db_functions.comparison.test_greatest.GreatestTests.test_coalesce_workaround",
                 "db_functions.comparison.test_least.LeastTests.test_coalesce_workaround",
+                # UPDATE ... ORDER BY syntax on MySQL/MariaDB does not support ordering by related fields
+                "update.tests.AdvancedTests.test_update_ordered_by_m2m_annotation_desc",
             },
             "MySQL doesn't support functional indexes on a function that "
             "returns JSON": {
                 "schema.tests.SchemaTests.test_func_index_json_key_transform",
             },
             "MySQL supports multiplying and dividing DurationFields by a "
             "scalar value but it's not implemented (#25287).": {
@@ -131,14 +135,15 @@
                 "schema.tests.SchemaTests.test_alter_primary_key_the_same_name",
                 "schema.tests.SchemaTests.test_autofield_to_o2o",
                 "update.tests.AdvancedTests.test_update_ordered_by_inline_m2m_annotation",
                 "update.tests.AdvancedTests.test_update_ordered_by_m2m_annotation",
                 # IntegrityError not raised
                 "constraints.tests.CheckConstraintTests.test_database_constraint",
                 "constraints.tests.CheckConstraintTests.test_database_constraint_unicode",
+                # Result of function ROUND(x, d) is different from MySQL
                 # https://github.com/pingcap/tidb/issues/26993
                 "db_functions.math.test_round.RoundTests.test_integer_with_negative_precision",
                 "db_functions.text.test_chr.ChrTests.test_transform",
                 "db_functions.text.test_chr.ChrTests.test_non_ascii",
                 "db_functions.text.test_chr.ChrTests.test_basic",
                 "db_functions.comparison.test_collate.CollateTests.test_collate_filter_ci",
                 # Unsupported modifying collation of column from 'utf8mb4_general_ci' to 'utf8mb4_bin'
@@ -156,16 +161,35 @@
                 "migrations.test_operations.OperationTests.test_add_constraint_percent_escaping",
                 "migrations.test_operations.OperationTests.test_add_or_constraint",
                 "migrations.test_operations.OperationTests.test_create_model_with_constraint",
                 "migrations.test_operations.OperationTests.test_remove_constraint",
                 "migrations.test_operations.OperationTests.test_alter_field_pk_mti_and_fk_to_base",
                 "migrations.test_operations.OperationTests.test_alter_field_pk_mti_fk",
                 "migrations.test_operations.OperationTests.test_create_model_with_boolean_expression_in_check_constraint",
+                # Unsupported adding a stored generated column through ALTER TABLE
+                "migrations.test_operations.OperationTests.test_add_field_after_generated_field",
+                "migrations.test_operations.OperationTests.test_add_generated_field_stored",
+                "migrations.test_operations.OperationTests.test_invalid_generated_field_changes_stored",
+                "migrations.test_operations.OperationTests.test_invalid_generated_field_persistency_change",
+                "migrations.test_operations.OperationTests.test_remove_generated_field_stored",
+                "schema.tests.SchemaTests.test_add_generated_field_contains",
+                # Failed to modify column's default value when has expression index
+                # https://github.com/pingcap/tidb/issues/52355
+                "migrations.test_operations.OperationTests.test_alter_field_with_func_index",
+                # TiDB has limited support for default value expressions
+                # https://docs.pingcap.com/tidb/dev/data-type-default-values#specify-expressions-as-default-values
+                "migrations.test_operations.OperationTests.test_add_field_database_default_function",
+                "schema.tests.SchemaTests.test_add_text_field_with_db_default",
+                "schema.tests.SchemaTests.test_db_default_equivalent_sql_noop",
+                "schema.tests.SchemaTests.test_db_default_output_field_resolving",
                 # about Pessimistic/Optimistic Transaction Model
                 "select_for_update.tests.SelectForUpdateTests.test_raw_lock_not_available",
+                # Wrong referenced_table_schema in information_schema.key_column_usage
+                # https://github.com/pingcap/tidb/issues/52350
+                "backends.mysql.test_introspection.TestCrossDatabaseRelations.test_omit_cross_database_relations",
             },
         }
         if self.connection.tidb_version < (5,):
             skips.update(
                 {
                     "tidb4": {
                         # Unsupported modify column
@@ -265,14 +289,20 @@
         operator.attrgetter("supports_over_clause")
     )
 
     @cached_property
     def supports_column_check_constraints(self):
         return True
 
+    @cached_property
+    def supports_expression_defaults(self):
+        # TiDB has limited support for default value expressions
+        # https://docs.pingcap.com/tidb/dev/data-type-default-values#specify-expressions-as-default-values
+        return True
+
     supports_table_check_constraints = property(
         operator.attrgetter("supports_column_check_constraints")
     )
 
     @cached_property
     def can_introspect_check_constraints(self):
         return False
```

### Comparing `django-tidb-4.2.4/django_tidb/fields/__init__.py` & `django-tidb-5.0.0/django_tidb/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.4/django_tidb/fields/vector.py` & `django-tidb-5.0.0/django_tidb/fields/vector.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.4/django_tidb/introspection.py` & `django-tidb-5.0.0/django_tidb/introspection.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     DatabaseIntrospection as MysqlDatabaseIntrospection,
 )
 from django.db.models import Index
 from django.utils.datastructures import OrderedSet
 
 FieldInfo = namedtuple(
     "FieldInfo",
-    BaseFieldInfo._fields + ("extra", "is_unsigned", "has_json_constraint", "comment"),
+    BaseFieldInfo._fields
+    + ("extra", "is_unsigned", "has_json_constraint", "comment", "data_type"),
 )
 InfoLine = namedtuple(
     "InfoLine",
     "col_name data_type max_len num_prec num_scale extra column_default "
     "collation is_unsigned comment",
 )
 
@@ -111,14 +112,15 @@
                     line[6],
                     info.column_default,
                     info.collation,
                     info.extra,
                     info.is_unsigned,
                     line[0] in json_constraints,
                     info.comment,
+                    info.data_type,
                 )
             )
         return fields
 
     def get_constraints(self, cursor, table_name):
         """
         Retrieve any constraints or keys (unique, pk, fk, check, index) across
```

### Comparing `django-tidb-4.2.4/django_tidb/operations.py` & `django-tidb-5.0.0/django_tidb/operations.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.4/django_tidb/patch.py` & `django-tidb-5.0.0/django_tidb/patch.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.4/django_tidb/schema.py` & `django-tidb-5.0.0/django_tidb/schema.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.4/django_tidb/version.py` & `django-tidb-5.0.0/django_tidb/version.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.4/django_tidb.egg-info/PKG-INFO` & `django-tidb-5.0.0/django_tidb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: django-tidb
-Version: 4.2.4
+Version: 5.0.0
 Summary: Django backend for TiDB
 Author-email: Xiang Zhang <zhangxiang02@pingcap.com>, Di Wang <wangdi@pingcap.com>
 Project-URL: Homepage, https://github.com/pingcap/tidb
 Project-URL: Bug Reports, https://github.com/pingcap/django-tidb/issues
 Project-URL: Source, https://github.com/pingcap/django-tidb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: vector
 Requires-Dist: numpy~=1.0; extra == "vector"
 
 # TiDB dialect for Django
 
@@ -62,14 +61,15 @@
 
 To install django-tidb, you need to select the version that corresponds with your Django version. Please refer to the table below for guidance:
 
 > The minor release number of Django doesn't correspond to the minor release number of django-tidb. Use the latest minor release of each.
 
 |django|django-tidb|install command|
 |:----:|:---------:|:-------------:|
+|v5.0.x|v5.0.x|`pip install 'django-tidb>=5.0.0,<5.1.0'`|
 |v4.2.x|v4.2.x|`pip install 'django-tidb>=4.2.0,<4.3.0'`|
 |v4.1.x|v4.1.x|`pip install 'django-tidb>=4.1.0,<4.2.0'`|
 |v3.2.x|v3.2.x|`pip install 'django-tidb>=3.2.0,<3.3.0'`|
 
 ## Usage
 
 Set `'ENGINE': 'django_tidb'` in your settings to this:
@@ -209,16 +209,16 @@
 
 ```python
 Test.objects.alias(distance=CosineDistance('embedding', [3, 1, 2])).filter(distance__lt=5)
 ```
 
 ## Supported versions
 
-- TiDB 4.0 and newer
-- Django 3.2, 4.1 and 4.2
+- TiDB 5.0 and newer
+- Django 3.2, 4.1, 4.2 and 5.0
 - Python 3.6 and newer(must match Django's Python version requirement)
 
 ## Test
 
 create your virtualenv with:
 
 ```bash
@@ -234,14 +234,14 @@
 $ DJANGO_VERSION=3.2.12 python run_testing_worker.py
 ```
 
 ## Migrate from previous versions
 
 Releases on PyPi before 3.0.0 are published from repository https://github.com/blacktear23/django_tidb. This repository is a new implementation and released under versions from 3.0.0. No backwards compatibility is ensured. The most significant points are:
 
-- Only Django 3.2 and 4.0 are tested and supported.
 - Engine name is `django_tidb` instead of `django_tidb.tidb`.
 
 ## Known issues
 
 - TiDB before v6.6.0 does not support FOREIGN KEY constraints([#18209](https://github.com/pingcap/tidb/issues/18209)).
 - TiDB before v6.2.0 does not support SAVEPOINT([#6840](https://github.com/pingcap/tidb/issues/6840)).
+- TiDB has limited support for default value expressions, please refer to the [documentation](https://docs.pingcap.com/tidb/dev/data-type-default-values#specify-expressions-as-default-values).
```

### Comparing `django-tidb-4.2.4/pyproject.toml` & `django-tidb-5.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,26 @@
 name = "django-tidb"
 authors = [
   { name="Xiang Zhang", email="zhangxiang02@pingcap.com" },
   { name="Di Wang", email="wangdi@pingcap.com" }
 ]
 description = "Django backend for TiDB"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Django",
-    "Framework :: Django :: 4.2",
+    "Framework :: Django :: 5.0",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12"
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/pingcap/tidb"
 "Bug Reports" = "https://github.com/pingcap/django-tidb/issues"
 "Source" = "https://github.com/pingcap/django-tidb"
```

