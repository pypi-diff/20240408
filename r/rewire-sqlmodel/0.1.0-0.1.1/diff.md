# Comparing `tmp/rewire-sqlmodel-0.1.0.tar.gz` & `tmp/rewire-sqlmodel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewire-sqlmodel-0.1.0.tar", last modified: Fri Apr  5 21:10:22 2024, max compression
+gzip compressed data, was "rewire-sqlmodel-0.1.1.tar", last modified: Mon Apr  8 17:49:56 2024, max compression
```

## Comparing `rewire-sqlmodel-0.1.0.tar` & `rewire-sqlmodel-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.022064 rewire-sqlmodel-0.1.0/
--rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2131 2024-04-05 21:10:22.022064 rewire-sqlmodel-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.1.0/README.md
--rw-rw-rw-   0        0        0      812 2024-04-05 20:57:56.000000 rewire-sqlmodel-0.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.010847 rewire-sqlmodel-0.1.0/rewire_sqlmodel/
--rw-rw-rw-   0        0        0    15704 2024-04-05 21:08:47.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.018063 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/
--rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_merge_dev.py
--rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_migrations.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.019062 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_template/
--rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_template/env.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.020062 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_template/versions/
--rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
--rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/fastapi.py
--rw-rw-rw-   0        0        0     2485 2024-02-04 08:52:32.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel/tests.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:10:22.021062 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/
--rw-rw-rw-   0        0        0     2131 2024-04-05 21:10:21.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-05 21:10:22.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 21:10:21.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-05 21:10:21.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-05 21:10:21.000000 rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 21:10:22.022064 rewire-sqlmodel-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 17:49:56.334565 rewire-sqlmodel-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2131 2024-04-08 17:49:56.333565 rewire-sqlmodel-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.1.1/README.md
+-rw-rw-rw-   0        0        0      812 2024-04-08 17:49:39.000000 rewire-sqlmodel-0.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-08 17:49:56.317498 rewire-sqlmodel-0.1.1/rewire_sqlmodel/
+-rw-rw-rw-   0        0        0    15704 2024-04-05 21:08:47.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:49:56.330562 rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/
+-rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/alembic_merge_dev.py
+-rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/alembic_migrations.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:49:56.331565 rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/alembic_template/
+-rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/alembic_template/env.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:49:56.332563 rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/alembic_template/versions/
+-rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
+-rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/fastapi.py
+-rw-rw-rw-   0        0        0     2446 2024-04-08 17:48:46.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:49:56.332563 rewire-sqlmodel-0.1.1/rewire_sqlmodel.egg-info/
+-rw-rw-rw-   0        0        0     2131 2024-04-08 17:49:56.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-08 17:49:56.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 17:49:56.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-08 17:49:56.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-08 17:49:56.000000 rewire-sqlmodel-0.1.1/rewire_sqlmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 17:49:56.334565 rewire-sqlmodel-0.1.1/setup.cfg
```

### Comparing `rewire-sqlmodel-0.1.0/LICENSE` & `rewire-sqlmodel-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.1.0/PKG-INFO` & `rewire-sqlmodel-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.1.0
+Version: 0.1.1
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rewire-sqlmodel-0.1.0/pyproject.toml` & `rewire-sqlmodel-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rewire-sqlmodel"
-version = "0.1.0"
+version = "0.1.1"
 description = "Integration of rewire and sqlmodel"
 readme = "README.md"
 authors = [{ name = "Ivan Vozhakov", email = "gou177@bk.ru" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rewire-sqlmodel-0.1.0/rewire_sqlmodel/__init__.py` & `rewire-sqlmodel-0.1.1/rewire_sqlmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_merge_dev.py` & `rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/alembic_merge_dev.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_migrations.py` & `rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/alembic_migrations.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/alembic_template/env.py` & `rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/alembic_template/env.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.1.0/rewire_sqlmodel/ext/fastapi.py` & `rewire-sqlmodel-0.1.1/rewire_sqlmodel/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.1.0/rewire_sqlmodel/tests.py` & `rewire-sqlmodel-0.1.1/rewire_sqlmodel/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,13 @@
                 await (
                     DependenciesModule.get()
                     .add(plugin)
                     .rebuild(inplace=True)
                     .add(TemporalDBModule.get().dependencies())
                     .solve()
                 )
-                try:
+                async with LifecycleModule.get().use_running():
                     return await cb(*args, **kwargs)
-                finally:
-                    await LifecycleModule.get().stop()
 
         return wrapped
 
     return wrapper
```

### Comparing `rewire-sqlmodel-0.1.0/rewire_sqlmodel.egg-info/PKG-INFO` & `rewire-sqlmodel-0.1.1/rewire_sqlmodel.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.1.0
+Version: 0.1.1
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

