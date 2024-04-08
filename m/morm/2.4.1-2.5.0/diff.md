# Comparing `tmp/morm-2.4.1.tar.gz` & `tmp/morm-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morm-2.4.1.tar", last modified: Sun Apr  7 10:05:54 2024, max compression
+gzip compressed data, was "morm-2.5.0.tar", last modified: Mon Apr  8 11:45:12 2024, max compression
```

## Comparing `morm-2.4.1.tar` & `morm-2.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 10:05:54.789579 morm-2.4.1/
--rw-rw-r--   0 jahid     (1000) jahid     (1001)     1703 2018-09-27 12:35:40.000000 morm-2.4.1/LICENSE
--rw-r--r--   0 jahid     (1000) jahid     (1001)    19914 2024-04-07 10:05:54.789579 morm-2.4.1/PKG-INFO
--rw-r--r--   0 jahid     (1000) jahid     (1001)    19104 2024-04-06 16:41:31.000000 morm-2.4.1/README.md
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 10:05:54.786246 morm-2.4.1/morm/
--rw-r--r--   0 jahid     (1000) jahid     (1001)       50 2021-04-08 08:46:50.000000 morm-2.4.1/morm/__init__.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     3243 2023-09-06 05:38:51.000000 morm-2.4.1/morm/admin.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     2043 2024-04-06 16:27:25.000000 morm-2.4.1/morm/ctx.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    38299 2024-04-06 16:27:25.000000 morm-2.4.1/morm/db.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      636 2024-03-01 06:38:43.000000 morm-2.4.1/morm/dt.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      470 2021-04-08 08:46:50.000000 morm-2.4.1/morm/exceptions.py
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 10:05:54.786246 morm-2.4.1/morm/fields/
--rw-r--r--   0 jahid     (1000) jahid     (1001)       26 2021-04-08 08:46:50.000000 morm-2.4.1/morm/fields/__init__.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     2047 2024-03-17 13:56:43.000000 morm-2.4.1/morm/fields/common.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    25094 2024-04-06 17:48:27.000000 morm-2.4.1/morm/fields/field.py
--rwxr-xr-x   0 jahid     (1000) jahid     (1001)    24349 2024-04-06 16:48:50.000000 morm-2.4.1/morm/init_fap
--rw-r--r--   0 jahid     (1000) jahid     (1001)     2915 2021-04-08 08:46:50.000000 morm-2.4.1/morm/meta.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    22305 2024-03-01 06:38:43.000000 morm-2.4.1/morm/migration.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    24397 2024-04-06 16:48:50.000000 morm-2.4.1/morm/model.py
--rwxr-xr-x   0 jahid     (1000) jahid     (1001)       87 2021-03-16 13:12:06.000000 morm-2.4.1/morm/morm_admin
--rw-r--r--   0 jahid     (1000) jahid     (1001)     1162 2024-03-01 06:38:43.000000 morm-2.4.1/morm/pg_models.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      541 2024-03-01 06:38:43.000000 morm-2.4.1/morm/q.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     3533 2023-09-06 06:09:00.000000 morm-2.4.1/morm/utils.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)       89 2024-04-06 16:27:25.000000 morm-2.4.1/morm/version.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     2140 2024-03-01 06:38:43.000000 morm-2.4.1/morm/void.py
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 10:05:54.789579 morm-2.4.1/morm.egg-info/
--rw-r--r--   0 jahid     (1000) jahid     (1001)    19914 2024-04-07 10:05:54.000000 morm-2.4.1/morm.egg-info/PKG-INFO
--rw-r--r--   0 jahid     (1000) jahid     (1001)      678 2024-04-07 10:05:54.000000 morm-2.4.1/morm.egg-info/SOURCES.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-04-07 10:05:54.000000 morm-2.4.1/morm.egg-info/dependency_links.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)       44 2024-04-07 10:05:54.000000 morm-2.4.1/morm.egg-info/requires.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)        5 2024-04-07 10:05:54.000000 morm-2.4.1/morm.egg-info/top_level.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)       38 2024-04-07 10:05:54.789579 morm-2.4.1/setup.cfg
--rw-r--r--   0 jahid     (1000) jahid     (1001)     1614 2024-04-06 16:48:50.000000 morm-2.4.1/setup.py
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 10:05:54.789579 morm-2.4.1/tests/
--rw-r--r--   0 jahid     (1000) jahid     (1001)     9442 2021-07-21 14:32:19.000000 morm-2.4.1/tests/test_Migration.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      929 2021-07-21 15:06:51.000000 morm-2.4.1/tests/test_admin.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      357 2024-04-05 13:26:01.000000 morm-2.4.1/tests/test_datetime.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    15408 2024-03-07 08:51:29.000000 morm-2.4.1/tests/test_db.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     4648 2021-04-08 08:54:08.000000 morm-2.4.1/tests/test_field.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      335 2020-08-23 09:25:08.000000 morm-2.4.1/tests/test_meta.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    17616 2021-03-15 07:33:40.000000 morm-2.4.1/tests/test_model.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      293 2020-08-23 09:44:54.000000 morm-2.4.1/tests/test_package.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      295 2021-03-10 12:56:49.000000 morm-2.4.1/tests/test_q.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      749 2020-08-23 09:53:12.000000 morm-2.4.1/tests/test_types.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      962 2020-08-04 06:22:01.000000 morm-2.4.1/tests/testd.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-08 11:45:12.470189 morm-2.5.0/
+-rw-rw-r--   0 jahid     (1000) jahid     (1001)     1703 2018-09-27 12:35:40.000000 morm-2.5.0/LICENSE
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    21424 2024-04-08 11:45:12.470189 morm-2.5.0/PKG-INFO
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    20614 2024-04-08 11:45:02.000000 morm-2.5.0/README.md
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-08 11:45:12.470189 morm-2.5.0/morm/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       50 2021-04-08 08:46:50.000000 morm-2.5.0/morm/__init__.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     3243 2023-09-06 05:38:51.000000 morm-2.5.0/morm/admin.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     2043 2024-04-06 16:27:25.000000 morm-2.5.0/morm/ctx.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    38368 2024-04-08 11:45:02.000000 morm-2.5.0/morm/db.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      636 2024-03-01 06:38:43.000000 morm-2.5.0/morm/dt.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      470 2021-04-08 08:46:50.000000 morm-2.5.0/morm/exceptions.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-08 11:45:12.470189 morm-2.5.0/morm/fields/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       26 2021-04-08 08:46:50.000000 morm-2.5.0/morm/fields/__init__.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     2047 2024-03-17 13:56:43.000000 morm-2.5.0/morm/fields/common.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    25972 2024-04-08 11:45:02.000000 morm-2.5.0/morm/fields/field.py
+-rwxr-xr-x   0 jahid     (1000) jahid     (1001)    24349 2024-04-06 16:48:50.000000 morm-2.5.0/morm/init_fap
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     2915 2021-04-08 08:46:50.000000 morm-2.5.0/morm/meta.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    22305 2024-03-01 06:38:43.000000 morm-2.5.0/morm/migration.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    26835 2024-04-08 11:45:02.000000 morm-2.5.0/morm/model.py
+-rwxr-xr-x   0 jahid     (1000) jahid     (1001)       87 2021-03-16 13:12:06.000000 morm-2.5.0/morm/morm_admin
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     1162 2024-03-01 06:38:43.000000 morm-2.5.0/morm/pg_models.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      541 2024-03-01 06:38:43.000000 morm-2.5.0/morm/q.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     3533 2023-09-06 06:09:00.000000 morm-2.5.0/morm/utils.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       89 2024-04-08 11:45:02.000000 morm-2.5.0/morm/version.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     2140 2024-03-01 06:38:43.000000 morm-2.5.0/morm/void.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-08 11:45:12.470189 morm-2.5.0/morm.egg-info/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    21424 2024-04-08 11:45:12.000000 morm-2.5.0/morm.egg-info/PKG-INFO
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      678 2024-04-08 11:45:12.000000 morm-2.5.0/morm.egg-info/SOURCES.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-04-08 11:45:12.000000 morm-2.5.0/morm.egg-info/dependency_links.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       44 2024-04-08 11:45:12.000000 morm-2.5.0/morm.egg-info/requires.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        5 2024-04-08 11:45:12.000000 morm-2.5.0/morm.egg-info/top_level.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       38 2024-04-08 11:45:12.470189 morm-2.5.0/setup.cfg
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     1614 2024-04-06 16:48:50.000000 morm-2.5.0/setup.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-08 11:45:12.470189 morm-2.5.0/tests/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     9442 2021-07-21 14:32:19.000000 morm-2.5.0/tests/test_Migration.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      929 2021-07-21 15:06:51.000000 morm-2.5.0/tests/test_admin.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      357 2024-04-05 13:26:01.000000 morm-2.5.0/tests/test_datetime.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    15408 2024-03-07 08:51:29.000000 morm-2.5.0/tests/test_db.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     4648 2021-04-08 08:54:08.000000 morm-2.5.0/tests/test_field.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      335 2020-08-23 09:25:08.000000 morm-2.5.0/tests/test_meta.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    17616 2021-03-15 07:33:40.000000 morm-2.5.0/tests/test_model.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      293 2020-08-23 09:44:54.000000 morm-2.5.0/tests/test_package.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      295 2021-03-10 12:56:49.000000 morm-2.5.0/tests/test_q.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      749 2020-08-23 09:53:12.000000 morm-2.5.0/tests/test_types.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      962 2020-08-04 06:22:01.000000 morm-2.5.0/tests/testd.py
```

### Comparing `morm-2.4.1/LICENSE` & `morm-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/PKG-INFO` & `morm-2.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: morm
-Version: 2.4.1
-Summary: A minimal asynchronous database object relational mapper
-Home-page: https://github.com/neurobin/python-morm
-Author: Md. Jahidul Hamid
-Author-email: jahidulhamid@yahoo.com
-License: BSD
-Keywords: async,orm,postgresql
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: asyncpg
-Requires-Dist: nest_asyncio
-Requires-Dist: pydantic>=2.6.4
-Requires-Dist: orjson
-
 [![Build status image](https://travis-ci.org/neurobin/python-morm.svg?branch=release)](https://travis-ci.com/github/neurobin/python-morm) [![Coverage Status](https://coveralls.io/repos/github/neurobin/python-morm/badge.svg?branch=release)](https://coveralls.io/github/neurobin/python-morm?branch=release)
 
 A minimal asynchronous database object relational mapper that supports transaction, connection pool and migration.
 
 Currently supports *PostgreSQL* with `asyncpg`.
 
 # Install
@@ -346,14 +322,48 @@
     user6.age = 34
     await tdb.save(user6)
     user5 = await tdb(User).get(5)
     user5.age = 34
     await tdb.save(user5)
 ```
 
+# Indexing
+
+You can use the `index: Tuple[str] | str | None` parameter to define what type/s of indexing should be applied to the field. Examples:
+
+```python
+class User(Base):
+    parent_id = Field('integer', index='hash')
+    username = Field('varchar(65)', index='hash,btree') # two indexes
+    email = Field('varchar(255)', index=('hash', 'btree')) # tuple is allowed as well
+    perms = Field('integer[]', index='gin:gin__int_ops')
+```
+
+If you want to remove the indexing, Add a `-` minus sign to the specific index and then run migration. After that you can safely remove the index keyword, e.g:
+
+```bash
+--- parent_id = Field('integer', index='-hash')
+===$ ./mgr makemigrations
+===$ ./mgr migrate
+>>> parent_id = Field('integer', index='') # now you can remove the hash
+```
+
+# Field/Model grouping
+
+You can group your model fields, for example, you can define groups like `admin`, `mod`, `staff`, `normal` and make your model fields organized into these groups. This will enable you to implement complex field level organized access controls. You can say, that the `password` field belongs to the *admin* group, then `subscriptions` field to *mod* group and then `active_subscriptions` to *staff* group.
+
+```python
+class UserAdmin(Base):
+    class Meta:
+        groups = ('admin',) # this model belongs to the admin group
+    password = Field('varchar(100)', groups=('admin',))
+    subscriptions = Field('integer[]', groups=('mod',))
+    active_subscriptions = Field('integer[]', groups=('staff',))
+```
+
 # Migration
 
 **Migration is a new feature and only forward migrations are supported as of now.**
 
 You should have created the *_morm_config_.py* and *mgr.py* file with `morm_admin init`.
 
 List all the models that you want migration for in *mgr.py*. You will know how to edit it once you open it.
```

### Comparing `morm-2.4.1/README.md` & `morm-2.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: morm
+Version: 2.5.0
+Summary: A minimal asynchronous database object relational mapper
+Home-page: https://github.com/neurobin/python-morm
+Author: Md. Jahidul Hamid
+Author-email: jahidulhamid@yahoo.com
+License: BSD
+Keywords: async,orm,postgresql
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: asyncpg
+Requires-Dist: nest_asyncio
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: orjson
+
 [![Build status image](https://travis-ci.org/neurobin/python-morm.svg?branch=release)](https://travis-ci.com/github/neurobin/python-morm) [![Coverage Status](https://coveralls.io/repos/github/neurobin/python-morm/badge.svg?branch=release)](https://coveralls.io/github/neurobin/python-morm?branch=release)
 
 A minimal asynchronous database object relational mapper that supports transaction, connection pool and migration.
 
 Currently supports *PostgreSQL* with `asyncpg`.
 
 # Install
@@ -322,14 +346,48 @@
     user6.age = 34
     await tdb.save(user6)
     user5 = await tdb(User).get(5)
     user5.age = 34
     await tdb.save(user5)
 ```
 
+# Indexing
+
+You can use the `index: Tuple[str] | str | None` parameter to define what type/s of indexing should be applied to the field. Examples:
+
+```python
+class User(Base):
+    parent_id = Field('integer', index='hash')
+    username = Field('varchar(65)', index='hash,btree') # two indexes
+    email = Field('varchar(255)', index=('hash', 'btree')) # tuple is allowed as well
+    perms = Field('integer[]', index='gin:gin__int_ops')
+```
+
+If you want to remove the indexing, Add a `-` minus sign to the specific index and then run migration. After that you can safely remove the index keyword, e.g:
+
+```bash
+--- parent_id = Field('integer', index='-hash')
+===$ ./mgr makemigrations
+===$ ./mgr migrate
+>>> parent_id = Field('integer', index='') # now you can remove the hash
+```
+
+# Field/Model grouping
+
+You can group your model fields, for example, you can define groups like `admin`, `mod`, `staff`, `normal` and make your model fields organized into these groups. This will enable you to implement complex field level organized access controls. You can say, that the `password` field belongs to the *admin* group, then `subscriptions` field to *mod* group and then `active_subscriptions` to *staff* group.
+
+```python
+class UserAdmin(Base):
+    class Meta:
+        groups = ('admin',) # this model belongs to the admin group
+    password = Field('varchar(100)', groups=('admin',))
+    subscriptions = Field('integer[]', groups=('mod',))
+    active_subscriptions = Field('integer[]', groups=('staff',))
+```
+
 # Migration
 
 **Migration is a new feature and only forward migrations are supported as of now.**
 
 You should have created the *_morm_config_.py* and *mgr.py* file with `morm_admin init`.
 
 List all the models that you want migration for in *mgr.py*. You will know how to edit it once you open it.
```

### Comparing `morm-2.4.1/morm/admin.py` & `morm-2.5.0/morm/admin.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/morm/ctx.py` & `morm-2.5.0/morm/ctx.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/morm/db.py` & `morm-2.5.0/morm/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,18 +151,19 @@
     asyncpg.Connection
 
     Args:
         pool (Pool): A connection pool
         con (Connection): Connection. Defaults to None.
     """
 
-    def __init__(self, pool: Pool, con: Connection=None):
+    def __init__(self, pool: Pool, con: Connection=None, sudo=False):
         self._pool = pool
         self._con = con
         self.DATA_NO_CHANGE = 'DATA_NO_CHANGE_TRIGGERED'
+        self.sudo = sudo
 
     def corp(self) -> Union[asyncpg.pool.Pool, Connection]:
         """Return the connection if available, otherwise return a Pool.
 
         Note: The name reads 'c or p'
 
         Returns:
@@ -288,15 +289,15 @@
             mob (ModelBase): Model object
             reset (bool): Reset the value change counter. Defaults to False
 
         Returns:
             (str, list): query, args
         """
         data = mob.Meta._fields_
-        new_data_gen = mob.__class__._get_FieldValue_data_valid_(data, up=True, validate_all=True, mob=mob)
+        new_data_gen = mob.__class__._get_FieldValue_data_valid_(data, up=True, validate_all=True, mob=mob, sudo=self.sudo)
         columns = []
         values = []
         markers = []
         c = 0
         for n,v in new_data_gen:
             c += 1
             if reset:
@@ -325,15 +326,15 @@
             AttributeError: If primary key does not exists i.e if not updatable
 
         Returns:
             str, args: tuple of query, args
         """
         pkval = getattr(mob, mob.__class__._get_pk_()) #save method depends on it's AttributeError
         data = mob.Meta._fields_
-        new_data_gen = mob.__class__._get_FieldValue_data_valid_(data, up=True, mob=mob)
+        new_data_gen = mob.__class__._get_FieldValue_data_valid_(data, up=True, mob=mob, sudo=self.sudo)
         colval = []
         values = []
         c = 0
         for n,v in new_data_gen:
             if n == mob.__class__._get_pk_(): continue
             if v.value_change_count > 0:
                 c += 1
```

### Comparing `morm-2.4.1/morm/dt.py` & `morm-2.5.0/morm/dt.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/morm/fields/common.py` & `morm-2.5.0/morm/fields/common.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/morm/fields/field.py` & `morm-2.5.0/morm/fields/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -308,38 +308,45 @@
         unique (bool, optional): Whether the field is unique. Defaults to False.
         index (str, optional): Index type. Defaults to None. 'btree', 'hash', 'gin', 'gist', prepend with - to remove the index.
         choices (Tuple[Tuple[str, Any], ...], optional): choices tuple: (('Name of choice', 'value'), ...)
         help_text (str, optional):  help text to describe this field.
         validator (callable, optional): A callable that accepts exactly one argument. Validates the value in `clean` method. Defaults to always_valid.
         modifier (callable, optional): A callable that accepts exactly one argument. Modifies the value if validation fails when the `clean` method is called.. Defaults to nomodify.
         fallback (bool, optional): Whether invalid value should fallback to default value suppressing exception. (May hide bugs in your program)
+        sudo (bool, optional): Mark this field as requiring elevated permission (for something that you will implement in your app). Defaults to None.
+        groups (tuple, optional): Groups that this field belongs to. Defaults to ().
     """
     def __init__(self, sql_type: str,
                 max_length: Optional[int]=None, # added to sql_type e.g varchar(max_length)
                 max_digits: Optional[int]=None, # added to sql_type e.g numeric(max_digits, decimal_places)
                 decimal_places: Optional[int]=None, # added to sql_type e.g numeric(max_digits, decimal_places)
                 array_dimension: Tuple[int, ...] = (),
                 sql_onadd='',
                 sql_ondrop='',
                 sql_alter: Tuple[str, ...] = (),
                 sql_engine='postgresql',
                 default: Any=Void,
                 value: Any=Void,
                 unique=False,
-                index=None, # 'btree', 'hash', 'gin', 'gist', prepend with - to remove the index.
+                index: Tuple[str] | str | None=None, # 'btree', 'hash', 'gin', 'gist', prepend with - to remove the index. Can be a tuple or comma separated string to specify multiple indexes.
                 choices: Tuple[Tuple[str, Any], ...] = (),
                 help_text: str = '',
                 validator: Callable=always_valid,
                 validator_text: str = '',
                 modifier: Callable=nomodify,
-                fallback=False,): # if you add new param here, update __repr__ method
+                fallback=False,
+                sudo=None,
+                groups: Tuple[str, ...]=(),
+            ): # if you add new param here, update __repr__ method
         # Rules for using a variable name here as local variables go into the self._json_:
         # 1. Must precede with underscore if not in the parameter list
         # 2. Make sure to exclude unnecessary variables in the self._json_ like 'self' etc..
         _init_args = list(locals().keys())[1:] # this must be the first line here in __init__
+        self.sudo = sudo
+        self.groups = groups
         self.max_length = max_length
         self.max_digits = max_digits
         self.decimal_places = decimal_places
         self.validator_text = validator_text
         self.native_type, self.native_type_raw = sqlTypeToNative(sql_type, optional=default is not Void, containerType=None if not array_dimension else List)
         if max_length and self.native_type_raw is not str:
             raise ValueError(f"max_length is only valid for types that are string like, {sql_type} given.")
@@ -359,27 +366,34 @@
 
         self.sql_type = sql_type
         _unique_constraint = '__UNQ_{table}_{column}__'
         if unique:
             _sql_unique = 'ALTER TABLE "{table}" ADD CONSTRAINT "%s" UNIQUE ("{column}");' % (_unique_constraint,)
         else:
             _sql_unique = 'ALTER TABLE "{table}" DROP CONSTRAINT IF EXISTS "%s";' % (_unique_constraint,)
-        if index:
-            _idx_remove = True if index[0] == '-' else False
-            if _idx_remove:
-                index = index[1:]
-            if index not in ['btree', 'hash', 'gin', 'gist', 'spgist', 'brin']:
-                raise ValueError(f"Invalid index type: {index}")
-            _index_name = '__IDX_{table}_{column}_'+index+'__'
-            if not _idx_remove:
-                _sql_index = 'CREATE INDEX IF NOT EXISTS "%s" ON "{table}" USING %s ("{column}")' % (_index_name, index)
-            else:
-                _sql_index = 'DROP INDEX IF EXISTS "%s"' % (_index_name,)
         sql_alter = (_sql_unique, *sql_alter)
+        _sql_index = ''
         if index:
+            if isinstance(index, str):
+                index = index.split(',')
+            for idx in index:
+                _idx_remove = True if idx[0] == '-' else False
+                _idx_ops = ''
+                if ':' in idx:
+                    idx, _idx_ops = idx.split(':', 1)
+                if _idx_remove:
+                    idx = idx[1:]
+                if idx.lower() not in ['btree', 'hash', 'gin', 'gist', 'spgist', 'brin']:
+                    raise ValueError(f"Invalid index type: {idx}")
+                _index_name = '__IDX_{table}_{column}_'+idx+'__'
+                if not _idx_remove:
+                    _sql_index += 'CREATE INDEX IF NOT EXISTS "%s" ON "{table}" USING %s ("{column}" %s);' % (_index_name, idx, _idx_ops)
+                else:
+                    _sql_index += 'DROP INDEX IF EXISTS "%s";' % (_index_name,)
+        if _sql_index:
             sql_alter = (*sql_alter, _sql_index)
         # handle default
         if isinstance(default, (int, float, str, bool)) or is_sql_array(default):
             sql_alter = (*sql_alter, "ALTER TABLE \"{table}\" ALTER COLUMN \"{column}\" SET DEFAULT "+f"{sql_val(default, sql_type)}::{sql_type};")
         self.sql_conf = ColumnConfig(sql_type=sql_type, sql_onadd=sql_onadd, sql_ondrop=sql_ondrop, sql_alter=sql_alter, sql_engine=sql_engine)
         self.validator = validator
         self.modifier = modifier
@@ -407,15 +421,14 @@
             if callable(v):
                 v_src = inspect.getsource(v)
                 v_src = v_src.split('\n')[0].strip()+' ...'
                 self._json_[k] = v_src
             else:
                 self._json_[k] = 'Void' if v == Void else v
 
-
     def __eq__(self, other: 'Field') -> bool: # type: ignore
         return bool(other and self.sql_conf == other.sql_conf)
 
     def __repr__(self):
         reprs = []
         for k in self._json_['_init_args']:
             if k == 'sql_type': reprs.append(repr(self.sql_type))
@@ -429,14 +442,18 @@
                         reprs.append(f'{k}={k_src}')
                     else:
                         reprs.append(f'{k}={repr(self.__dict__[k])}')
                 except KeyError: pass
         body = ', '.join(reprs)
         return f'{self.__class__.__name__}({body})'
 
+
+    def check_sudo(self, sudo: bool) -> bool:
+        return False if self.sudo and not sudo else True
+
     def to_json(self):
         res = self._json_.copy()
         res['_name'] = self.name
         res['_repr'] = self.__repr__()
         del res['_init_args']
         return res
```

### Comparing `morm-2.4.1/morm/init_fap` & `morm-2.5.0/morm/init_fap`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/morm/meta.py` & `morm-2.5.0/morm/meta.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/morm/migration.py` & `morm-2.5.0/morm/migration.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/morm/model.py` & `morm-2.5.0/morm/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,24 +66,27 @@
                 # mutable values can be changed by other class meta change
                 if mutable:
                     meta_attrs[k] = copy.deepcopy(v)
                 else:
                     meta_attrs[k] = v
 
         _set_meta_attr('proxy', False)
+        _set_meta_attr('sudo', None)
+        _set_meta_attr('groups', ())
         _set_meta_attr('pk', 'id')
         _set_meta_attr('ordering', ())
         _set_meta_attr('fields_up', ())
         _set_meta_attr('fields_down', ())
         _set_meta_attr('exclude_fields_up', ())
         _set_meta_attr('exclude_fields_down', ())
         _set_meta_attr('exclude_values_up', {'':()}, mutable=True)
         _set_meta_attr('exclude_values_down', {'':()}, mutable=True)
         _set_meta_attr('ignore_init_exclude_error', True)
         _set_meta_attr('_field_defs_', {}, internal=True, mutable=True)
+        _set_meta_attr('_field_groups_', {}, internal=True, mutable=True)
 
         if meta_attrs['proxy']:
             #proxy model inherits everything
             try:
                 meta_attrs['db_table'] = BaseMeta.db_table #type: ignore
                 meta_attrs['abstract'] = BaseMeta.abstract #type: ignore
             except AttributeError:
@@ -102,15 +105,21 @@
             if isinstance(v, Field):
                 if n.startswith('_'):
                     raise AttributeError(f"Invalid field name '{n}' in model '{class_name}'. \
                         Field name must not start with underscore.")
                 if meta_attrs['proxy'] and n in attrs:
                     raise ValueError(f"Proxy model '{class_name}' can not define new field: {n}")
                 v.name = n
+                if meta_attrs['sudo'] is not None and v.sudo is None:
+                    v.sudo = meta_attrs['sudo']
                 # v.sql_conf.conf['table_name'] = meta_attrs['db_table'] # Field must not contain table_name, because it is void when model is abstract and it gets inherited.
+                for g in v.groups:
+                    gs = meta_attrs['_field_groups_'].setdefault(g, [])
+                    if n not in gs:
+                        gs.append(n)
                 meta_attrs['_field_defs_'][n] = v
             elif n in attrs:
                 new_attrs[n] = attrs[n]
 
         # we do this after finalizing meta_attr
         def _get_field_name(n: str) -> str:
             if n in meta_attrs['_field_defs_']:
@@ -220,14 +229,75 @@
             str: field name
         """
         if n in self.Meta._field_defs_:
             return n
         else:
             raise AttributeError(f"No such field `{n}` in model `{self.__name__}`")
 
+    def _check_sudo_(self, sudo: bool, n: str='') -> bool|List[str]:
+        """Check if the given sudo can get access to the field
+        Or return a list of fields that can be accessed with the given
+        value of sudo.
+        """
+        if n:
+            return self.Meta._field_defs_[self._check_field_name_(n)].check_sudo(sudo)
+        return [k for k, v in self.Meta._field_defs_.items() if v.check_sudo(sudo)]
+
+    def _sudo_fields_(self) -> Iterator[str]:
+        """Yield field names that require elevated access
+
+        Yields:
+            str: field name
+        """
+        for k, v in self.Meta._field_defs_.items():
+            if v.sudo:
+                yield k
+
+    def _groups_(self) -> Tuple[str]:
+        """Get groups that this model belongs to
+
+        Returns:
+            Tuple[str]: Tuple of group names
+        """
+        return tuple(self.Meta.groups)
+
+    def _group_fields_(self, g: str) -> Tuple[str]:
+        """Get field names of a group
+
+        Args:
+            g (str): group name
+
+        Returns:
+            Tuple[str]: Tuple of field names
+        """
+        return tuple(self.Meta._field_groups_.get(g, []))
+
+    def _field_groups_(self, n) -> Tuple[str]:
+        """Get groups of a field
+
+        Args:
+            n (str): field name
+
+        Returns:
+            Tuple[str]: List of group names
+        """
+        return tuple(self.Meta._field_defs_[self._check_field_name_(n)].groups)
+
+    def _check_group_(self, g: str, n: str) -> bool:
+        """Check if a field belongs to a group
+
+        Args:
+            g (str): group name
+            n (str): field name
+
+        Returns:
+            bool: True if field belongs to the group
+        """
+        return n in self._group_fields_(g)
+
     def _get_fields_(self, up=False) -> Iterator[str]:
         """Yields field names that pass include/exclude criteria
 
         Args:
             up (bool, optional): up criteria or down criteria. Defaults to False (down).
 
         Yields:
@@ -258,15 +328,15 @@
         fields = self._get_fields_(up)
         all_fields = self._get_all_fields_()
         for k in fields:
             res[k] = all_fields[k].to_json()
         return res
 
     def _pydantic_(self, up=False, suffix=None, include_validators=None):
-        '''Create a pydantic model from the model
+        '''Create a pydantic model from the morm model
 
         ### Parameters:
 
         up: bool
             Whether it's for up (data update) or down (data retrieval)
         suffix: str
             Suffix to append to the model name, default: _UP or _DOWN
@@ -295,15 +365,15 @@
             v._value = validator(v.value) # do not trigger the field validator
             # and do not increase the change count
         except AttributeError:
             pass
         return v
 
 
-    def _get_FieldValue_data_valid_(self, data: dict, up=False, validate_all=False, mob=None) -> Iterator[Tuple[str, Any]]:
+    def _get_FieldValue_data_valid_(self, data: dict, up=False, validate_all=False, mob=None, sudo=False) -> Iterator[Tuple[str, Any]]:
         """Yields valid key,value pairs from data.
 
         Validity is checked against include/exclude key/value criteria.
 
         Args:
             data (dict): data to be validated.
             up (bool, optional): whether up (data update) or down (data retrieval). Defaults to False.
@@ -324,14 +394,17 @@
             if validate_all: v = self._run_validations_(k, v, mob)
             if not self._is_valid_key_(k, fields, exclude_fields):
                 continue
             if not self._is_valid_value_(k, v.value, exclude_values):
                 continue
             if not validate_all: # run validations for to-be-changed fields only
                 v = self._run_validations_(k, v, mob)
+            # check sudo
+            if not v._field.check_sudo(sudo):
+                raise ValueError(f"Field {k} requires elevated access.")
             yield k, v
 
 
     # def _get_data_for_valid_values_(self, data, up=False, gen=False):
     #     if up:
     #         exclude_values = self.Meta.exclude_values_up
     #     else:
@@ -408,25 +481,28 @@
         # through the metaclasses __new__ methods and processed accordingly
         # to determine which one should be inherited and which one should not.
         pk = 'id'
         '''Primary key'''
         db_table = Void
         abstract = True
         proxy = False
+        sudo = None
+        groups = ()
         ordering = ()
         fields_up = ()
         fields_down = ()
         exclude_fields_up = ()
         exclude_fields_down = ()
         exclude_values_up = {'':()}
         exclude_values_down = {'':()}
         ignore_init_exclude_error = True
 
         #internal
         _field_defs_: Dict[str, Field]
+        _field_groups_: Dict[str, List[str]]
         _fields_: Dict[str, FieldValue]
         _fromdb_: List[str]
         _initializing_: bool = False
 
 
     def __init__(self, *args, **kwargs):
         class Meta:
```

### Comparing `morm-2.4.1/morm/pg_models.py` & `morm-2.5.0/morm/pg_models.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/morm/q.py` & `morm-2.5.0/morm/q.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/morm/utils.py` & `morm-2.5.0/morm/utils.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/morm/void.py` & `morm-2.5.0/morm/void.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/morm.egg-info/PKG-INFO` & `morm-2.5.0/morm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morm
-Version: 2.4.1
+Version: 2.5.0
 Summary: A minimal asynchronous database object relational mapper
 Home-page: https://github.com/neurobin/python-morm
 Author: Md. Jahidul Hamid
 Author-email: jahidulhamid@yahoo.com
 License: BSD
 Keywords: async,orm,postgresql
 Classifier: Development Status :: 5 - Production/Stable
@@ -346,14 +346,48 @@
     user6.age = 34
     await tdb.save(user6)
     user5 = await tdb(User).get(5)
     user5.age = 34
     await tdb.save(user5)
 ```
 
+# Indexing
+
+You can use the `index: Tuple[str] | str | None` parameter to define what type/s of indexing should be applied to the field. Examples:
+
+```python
+class User(Base):
+    parent_id = Field('integer', index='hash')
+    username = Field('varchar(65)', index='hash,btree') # two indexes
+    email = Field('varchar(255)', index=('hash', 'btree')) # tuple is allowed as well
+    perms = Field('integer[]', index='gin:gin__int_ops')
+```
+
+If you want to remove the indexing, Add a `-` minus sign to the specific index and then run migration. After that you can safely remove the index keyword, e.g:
+
+```bash
+--- parent_id = Field('integer', index='-hash')
+===$ ./mgr makemigrations
+===$ ./mgr migrate
+>>> parent_id = Field('integer', index='') # now you can remove the hash
+```
+
+# Field/Model grouping
+
+You can group your model fields, for example, you can define groups like `admin`, `mod`, `staff`, `normal` and make your model fields organized into these groups. This will enable you to implement complex field level organized access controls. You can say, that the `password` field belongs to the *admin* group, then `subscriptions` field to *mod* group and then `active_subscriptions` to *staff* group.
+
+```python
+class UserAdmin(Base):
+    class Meta:
+        groups = ('admin',) # this model belongs to the admin group
+    password = Field('varchar(100)', groups=('admin',))
+    subscriptions = Field('integer[]', groups=('mod',))
+    active_subscriptions = Field('integer[]', groups=('staff',))
+```
+
 # Migration
 
 **Migration is a new feature and only forward migrations are supported as of now.**
 
 You should have created the *_morm_config_.py* and *mgr.py* file with `morm_admin init`.
 
 List all the models that you want migration for in *mgr.py*. You will know how to edit it once you open it.
```

### Comparing `morm-2.4.1/morm.egg-info/SOURCES.txt` & `morm-2.5.0/morm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/setup.py` & `morm-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/tests/test_Migration.py` & `morm-2.5.0/tests/test_Migration.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/tests/test_admin.py` & `morm-2.5.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/tests/test_db.py` & `morm-2.5.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/tests/test_field.py` & `morm-2.5.0/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/tests/test_model.py` & `morm-2.5.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/tests/test_types.py` & `morm-2.5.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.1/tests/testd.py` & `morm-2.5.0/tests/testd.py`

 * *Files identical despite different names*

