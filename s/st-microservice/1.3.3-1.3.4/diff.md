# Comparing `tmp/st_microservice-1.3.3.tar.gz` & `tmp/st_microservice-1.3.4.tar.gz`

## Comparing `st_microservice-1.3.3.tar` & `st_microservice-1.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/__init__.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/auth_utils.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/backend_connector.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/base.graphql
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/celery_app.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/celery_utils.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/database.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/exceptions.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/filter_parser.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/general_utils.py
--rw-r--r--   0        0        0     9455 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/graphql_app.py
--rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/graphql_utils.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/models_utils.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/pypika_extentions.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/request_utils.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/starlette_backend.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/models_functions/__init__.py
--rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 st_microservice-1.3.3/src/st_microservice/models_functions/functions.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 st_microservice-1.3.3/.gitignore
--rw-r--r--   0        0        0    35182 2020-02-02 00:00:00.000000 st_microservice-1.3.3/LICENSE.txt
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 st_microservice-1.3.3/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 st_microservice-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 st_microservice-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/__init__.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/auth_utils.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/backend_connector.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/base.graphql
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/celery_app.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/celery_utils.py
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/database.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/exceptions.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/filter_parser.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/general_utils.py
+-rw-r--r--   0        0        0     9455 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/graphql_app.py
+-rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/graphql_utils.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/models_utils.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/pypika_extentions.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/request_utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/starlette_backend.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/models_functions/__init__.py
+-rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 st_microservice-1.3.4/src/st_microservice/models_functions/functions.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 st_microservice-1.3.4/.gitignore
+-rw-r--r--   0        0        0    35182 2020-02-02 00:00:00.000000 st_microservice-1.3.4/LICENSE.txt
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 st_microservice-1.3.4/README.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 st_microservice-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 st_microservice-1.3.4/PKG-INFO
```

### Comparing `st_microservice-1.3.3/src/st_microservice/auth_utils.py` & `st_microservice-1.3.4/src/st_microservice/auth_utils.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/backend_connector.py` & `st_microservice-1.3.4/src/st_microservice/backend_connector.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/base.graphql` & `st_microservice-1.3.4/src/st_microservice/base.graphql`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/celery_app.py` & `st_microservice-1.3.4/src/st_microservice/celery_app.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/celery_utils.py` & `st_microservice-1.3.4/src/st_microservice/celery_utils.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/database.py` & `st_microservice-1.3.4/src/st_microservice/database.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/filter_parser.py` & `st_microservice-1.3.4/src/st_microservice/filter_parser.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/graphql_app.py` & `st_microservice-1.3.4/src/st_microservice/graphql_app.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/graphql_utils.py` & `st_microservice-1.3.4/src/st_microservice/graphql_utils.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/models_utils.py` & `st_microservice-1.3.4/src/st_microservice/models_utils.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/pypika_extentions.py` & `st_microservice-1.3.4/src/st_microservice/pypika_extentions.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/request_utils.py` & `st_microservice-1.3.4/src/st_microservice/request_utils.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/starlette_backend.py` & `st_microservice-1.3.4/src/st_microservice/starlette_backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,21 @@
     # Allow origins from both HTTP or HTTPS, root or subdomains, any port
     root_domain_re = r'https?://(.*\.)?{}(:\d*)?'.format(root_domain.replace('.', r'\.'))
     print('Allowed Origins Regex:', root_domain_re)
 
     app = Starlette(
         routes=routes+[Route('/getuser', get_user, methods=['GET'])],
         middleware=[
-            Middleware(CORSMiddleware, allow_origin_regex=root_domain_re, allow_credentials=True, allow_methods=['*']),
+            Middleware(
+                CORSMiddleware,
+                allow_origin_regex=root_domain_re,
+                allow_credentials=True,
+                allow_methods=['*'],
+                allow_headers=['Authorization']
+            ),
             Middleware(AsyncDBMiddleware),
             Middleware(AuthenticationMiddleware, backend=authbackend, on_error=auth_error_handler)
         ],
         lifespan=lifespan,
         debug=debug,
     )
     app.router.redirect_slashes = False  # Ignore wrong type
```

### Comparing `st_microservice-1.3.3/src/st_microservice/models_functions/__init__.py` & `st_microservice-1.3.4/src/st_microservice/models_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/src/st_microservice/models_functions/functions.py` & `st_microservice-1.3.4/src/st_microservice/models_functions/functions.py`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/LICENSE.txt` & `st_microservice-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_microservice-1.3.3/pyproject.toml` & `st_microservice-1.3.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "st-microservice"
-version = "1.3.3"
+version = "1.3.4"
 authors = [
     {name = "Robert Trad", email = "roberttrad@gmail.com"}
 ]
 description = "Tools to build Microservice Backends"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "aiodataloader<1",
-    "ariadne==0.22.0",
+    "ariadne==0.23.0",
     "asyncpg<1",
     "gunicorn<22",
     "httpx<1",
-    "PyJWT>=2.1,<3",
+    "PyJWT<3",
     "pypika<1",
     "pyparsing<4",
     "starlette<1",
     "uvicorn<1",
     "websockets<13"
 ]
```

### Comparing `st_microservice-1.3.3/PKG-INFO` & `st_microservice-1.3.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: st-microservice
-Version: 1.3.3
+Version: 1.3.4
 Summary: Tools to build Microservice Backends
 Project-URL: Homepage, https://github.com/rouppart/ST-Microservice-Backend
 Author-email: Robert Trad <roberttrad@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Requires-Dist: aiodataloader<1
-Requires-Dist: ariadne==0.22.0
+Requires-Dist: ariadne==0.23.0
 Requires-Dist: asyncpg<1
 Requires-Dist: gunicorn<22
 Requires-Dist: httpx<1
-Requires-Dist: pyjwt<3,>=2.1
+Requires-Dist: pyjwt<3
 Requires-Dist: pyparsing<4
 Requires-Dist: pypika<1
 Requires-Dist: starlette<1
 Requires-Dist: uvicorn<1
 Requires-Dist: websockets<13
 Provides-Extra: celery
 Requires-Dist: celery; extra == 'celery'
```

