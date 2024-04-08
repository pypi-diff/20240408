# Comparing `tmp/rewire-sqlmodel-0.2.1.tar.gz` & `tmp/rewire-sqlmodel-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewire-sqlmodel-0.2.1.tar", last modified: Mon Apr  8 19:56:30 2024, max compression
+gzip compressed data, was "rewire-sqlmodel-0.2.2.tar", last modified: Mon Apr  8 20:08:22 2024, max compression
```

## Comparing `rewire-sqlmodel-0.2.1.tar` & `rewire-sqlmodel-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.949284 rewire-sqlmodel-0.2.1/
--rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2131 2024-04-08 19:56:30.948123 rewire-sqlmodel-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.2.1/README.md
--rw-rw-rw-   0        0        0      812 2024-04-08 19:56:23.000000 rewire-sqlmodel-0.2.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.910680 rewire-sqlmodel-0.2.1/rewire_sqlmodel/
--rw-rw-rw-   0        0        0    15505 2024-04-08 19:56:15.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.936657 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/
--rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_merge_dev.py
--rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_migrations.py
-drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.941164 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_template/
--rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_template/env.py
-drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.945168 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_template/versions/
--rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
--rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/fastapi.py
--rw-rw-rw-   0        0        0     2582 2024-04-08 18:06:38.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel/tests.py
-drwxrwxrwx   0        0        0        0 2024-04-08 19:56:30.947116 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/
--rw-rw-rw-   0        0        0     2131 2024-04-08 19:56:30.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-08 19:56:30.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 19:56:30.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-08 19:56:30.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-08 19:56:30.000000 rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 19:56:30.949284 rewire-sqlmodel-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 20:08:22.393827 rewire-sqlmodel-0.2.2/
+-rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2131 2024-04-08 20:08:22.393827 rewire-sqlmodel-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.2.2/README.md
+-rw-rw-rw-   0        0        0      812 2024-04-08 20:08:14.000000 rewire-sqlmodel-0.2.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-08 20:08:22.379591 rewire-sqlmodel-0.2.2/rewire_sqlmodel/
+-rw-rw-rw-   0        0        0    15837 2024-04-08 20:07:38.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:08:22.390155 rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/
+-rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/alembic_merge_dev.py
+-rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/alembic_migrations.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:08:22.390155 rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/alembic_template/
+-rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/alembic_template/env.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:08:22.391821 rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/alembic_template/versions/
+-rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
+-rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/fastapi.py
+-rw-rw-rw-   0        0        0     2582 2024-04-08 18:06:38.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:08:22.392824 rewire-sqlmodel-0.2.2/rewire_sqlmodel.egg-info/
+-rw-rw-rw-   0        0        0     2131 2024-04-08 20:08:22.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-08 20:08:22.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 20:08:22.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-08 20:08:22.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-08 20:08:22.000000 rewire-sqlmodel-0.2.2/rewire_sqlmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 20:08:22.394828 rewire-sqlmodel-0.2.2/setup.cfg
```

### Comparing `rewire-sqlmodel-0.2.1/LICENSE` & `rewire-sqlmodel-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.1/PKG-INFO` & `rewire-sqlmodel-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.2.1
+Version: 0.2.2
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rewire-sqlmodel-0.2.1/pyproject.toml` & `rewire-sqlmodel-0.2.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rewire-sqlmodel"
-version = "0.2.1"
+version = "0.2.2"
 description = "Integration of rewire and sqlmodel"
 readme = "README.md"
 authors = [{ name = "Ivan Vozhakov", email = "gou177@bk.ru" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rewire-sqlmodel-0.2.1/rewire_sqlmodel/__init__.py` & `rewire-sqlmodel-0.2.2/rewire_sqlmodel/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,46 +219,53 @@
 
 tx_lock = anyio.Lock()
 
 session_context = Context[AsyncSession]()
 
 
 class ContextSession:
+    ctx = CTX()
     session: AsyncSession | None = None
     commit_hooks: list[Callable[[], Awaitable]]
     rollback_hooks: list[Callable[[], Awaitable]]
 
     async def __aenter__(self):
+        if (root := self.ctx.get(None)) is not None:
+            return root
         if self.session is not None:
             self.context = session_context.use(self.session)
             self.context.__enter__()
+            self.self_context = self.ctx.use()
+            self.self_context.__enter__()
             return self
         lazy = LazySession.ctx.get(None)
         if lazy is not None:
             self.context = None
             session = await lazy.start()
             return session
         await self.start()
         assert self.session is not None
         self.context = session_context.use(self.session)
         self.context.__enter__()
+        self.self_context = self.ctx.use()
+        self.self_context.__enter__()
         return self
 
     async def start(self):
         self.session = Dependencies.ctx.get().resolve(AsyncSessionmaker)()
         self.commit_hooks = []
         self.rollback_hooks = []
 
     async def __aexit__(self, exc_type, exc_value, trace):
         if not self.context:
             return
+        self.self_context.__exit__(exc_type, exc_value, trace)
         self.context.__exit__(exc_type, exc_value, trace)
         if self.session is None:
             return
-
         if not exc_type:
             try:
                 await self.session.commit()
             finally:
                 await self.session.__aexit__(exc_type, exc_value, trace)
             for hook in self.commit_hooks:
                 await hook()
```

### Comparing `rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_merge_dev.py` & `rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/alembic_merge_dev.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_migrations.py` & `rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/alembic_migrations.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/alembic_template/env.py` & `rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/alembic_template/env.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.1/rewire_sqlmodel/ext/fastapi.py` & `rewire-sqlmodel-0.2.2/rewire_sqlmodel/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.1/rewire_sqlmodel/tests.py` & `rewire-sqlmodel-0.2.2/rewire_sqlmodel/tests.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.1/rewire_sqlmodel.egg-info/PKG-INFO` & `rewire-sqlmodel-0.2.2/rewire_sqlmodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.2.1
+Version: 0.2.2
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

