# Comparing `tmp/rewire-sqlmodel-0.2.0.tar.gz` & `tmp/rewire-sqlmodel-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewire-sqlmodel-0.2.0.tar", last modified: Mon Apr  8 18:07:49 2024, max compression
+gzip compressed data, was "rewire-sqlmodel-0.2.1.tar", last modified: Mon Apr  8 19:56:30 2024, max compression
```

## Comparing `rewire-sqlmodel-0.2.0.tar` & `rewire-sqlmodel-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 18:07:49.994747 rewire-sqlmodel-0.2.0/
--rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2131 2024-04-08 18:07:49.993403 rewire-sqlmodel-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.2.0/README.md
--rw-rw-rw-   0        0        0      812 2024-04-08 18:07:35.000000 rewire-sqlmodel-0.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-08 18:07:49.980861 rewire-sqlmodel-0.2.0/rewire_sqlmodel/
--rw-rw-rw-   0        0        0    15704 2024-04-05 21:08:47.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:07:49.990399 rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/
--rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/alembic_merge_dev.py
--rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/alembic_migrations.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:07:49.991402 rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/alembic_template/
--rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/alembic_template/env.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:07:49.992400 rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/alembic_template/versions/
--rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
--rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/fastapi.py
--rw-rw-rw-   0        0        0     2582 2024-04-08 18:06:38.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel/tests.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:07:49.992400 rewire-sqlmodel-0.2.0/rewire_sqlmodel.egg-info/
--rw-rw-rw-   0        0        0     2131 2024-04-08 18:07:49.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-08 18:07:49.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 18:07:49.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-08 18:07:49.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-08 18:07:49.000000 rewire-sqlmodel-0.2.0/rewire_sqlmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 18:07:49.994747 rewire-sqlmodel-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.949284 rewire-sqlmodel-0.2.1/
+-rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2131 2024-04-08 19:56:30.948123 rewire-sqlmodel-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.2.1/README.md
+-rw-rw-rw-   0        0        0      812 2024-04-08 19:56:23.000000 rewire-sqlmodel-0.2.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.910680 rewire-sqlmodel-0.2.1/rewire_sqlmodel/
+-rw-rw-rw-   0        0        0    15505 2024-04-08 19:56:15.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.936657 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/
+-rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_merge_dev.py
+-rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_migrations.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.941164 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_template/
+-rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_template/env.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.945168 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_template/versions/
+-rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
+-rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/fastapi.py
+-rw-rw-rw-   0        0        0     2582 2024-04-08 18:06:38.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.947116 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/
+-rw-rw-rw-   0        0        0     2131 2024-04-08 19:56:30.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-08 19:56:30.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 19:56:30.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-08 19:56:30.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-08 19:56:30.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 19:56:30.949284 rewire-sqlmodel-0.2.1/setup.cfg
```

### Comparing `rewire-sqlmodel-0.2.0/LICENSE` & `rewire-sqlmodel-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.0/PKG-INFO` & `rewire-sqlmodel-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.2.0
+Version: 0.2.1
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rewire-sqlmodel-0.2.0/pyproject.toml` & `rewire-sqlmodel-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rewire-sqlmodel"
-version = "0.2.0"
+version = "0.2.1"
 description = "Integration of rewire and sqlmodel"
 readme = "README.md"
 authors = [{ name = "Ivan Vozhakov", email = "gou177@bk.ru" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rewire-sqlmodel-0.2.0/rewire_sqlmodel/__init__.py` & `rewire-sqlmodel-0.2.1/rewire_sqlmodel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,33 +146,31 @@
 
         cache_ok = True
 
         def __init__(self, type: Type = None, *args, **kwargs) -> None:
             super().__init__(*args, **kwargs)
             self._type = type
 
-        def load_dialect_impl(self, dialect):
-            if id(dialect) not in dialect_patched:
-                dialect._json_serializer = self.type_adapter.dump_json  # type: ignore
-                dialect_patched.add(id(dialect))
-            return super().load_dialect_impl(dialect)
-
-        def process_bind_param(self, value, dialect):
-            if isinstance(value, BaseModel):
-                return dict(value._iter(to_dict=True))
+        def bind_processor(self, dialect):
+            json = JSON()
 
-            return value
+            def test(a):
+                return self.type_adapter.dump_json(a)
 
-        @memoized_property
-        def type_adapter(self):
-            return TypeAdapter(self._type)
+            return json._make_bind_processor(
+                json._str_impl.bind_processor(dialect), test
+            )
 
         def process_result_value(self, value, dialect):
             return self.type_adapter.validate_python(value)
 
+        @memoized_property
+        def type_adapter(self):
+            return TypeAdapter(self._type)
+
         def copy(self, *a, **kw):
             return type(self)(self._type, *a, **kw)
 
     if not TYPE_CHECKING:
 
         class BigInt(int):
             pass
```

### Comparing `rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/alembic_merge_dev.py` & `rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_merge_dev.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/alembic_migrations.py` & `rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_migrations.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/alembic_template/env.py` & `rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_template/env.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.0/rewire_sqlmodel/ext/fastapi.py` & `rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.0/rewire_sqlmodel/tests.py` & `rewire-sqlmodel-0.2.1/rewire_sqlmodel/tests.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.0/rewire_sqlmodel.egg-info/PKG-INFO` & `rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.2.0
+Version: 0.2.1
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

