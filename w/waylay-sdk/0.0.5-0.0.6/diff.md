# Comparing `tmp/waylay-sdk-0.0.5.tar.gz` & `tmp/waylay-sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay-sdk-0.0.5.tar", last modified: Thu Mar 28 14:02:37 2024, max compression
+gzip compressed data, was "waylay-sdk-0.0.6.tar", last modified: Mon Apr  8 08:05:16 2024, max compression
```

## Comparing `waylay-sdk-0.0.5.tar` & `waylay-sdk-0.0.6.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 14:02:37.724906 waylay-sdk-0.0.5/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      746 2024-03-26 14:02:35.000000 waylay-sdk-0.0.5/LICENSE.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     9390 2024-03-28 14:02:37.723931 waylay-sdk-0.0.5/PKG-INFO
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     7018 2024-03-28 11:04:55.000000 waylay-sdk-0.0.5/README.md
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1663 2024-03-28 13:41:35.000000 waylay-sdk-0.0.5/pyproject.toml
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       38 2024-03-28 14:02:37.724990 waylay-sdk-0.0.5/setup.cfg
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 14:02:37.654880 waylay-sdk-0.0.5/src/
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 14:02:37.653888 waylay-sdk-0.0.5/src/waylay/
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 14:02:37.661114 waylay-sdk-0.0.5/src/waylay/sdk/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      754 2024-03-28 08:55:26.000000 waylay-sdk-0.0.5/src/waylay/sdk/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       60 2024-03-28 11:04:55.000000 waylay-sdk-0.0.5/src/waylay/sdk/_version.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 14:02:37.695606 waylay-sdk-0.0.5/src/waylay/sdk/api/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      661 2024-03-21 16:22:46.000000 waylay-sdk-0.0.5/src/waylay/sdk/api/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     5970 2024-03-26 14:02:35.000000 waylay-sdk-0.0.5/src/waylay/sdk/api/_models.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4423 2024-03-28 08:55:26.000000 waylay-sdk-0.0.5/src/waylay/sdk/api/client.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2298 2024-03-15 11:31:35.000000 waylay-sdk-0.0.5/src/waylay/sdk/api/exceptions.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2299 2024-03-21 16:22:46.000000 waylay-sdk-0.0.5/src/waylay/sdk/api/http.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    10842 2024-03-28 08:55:26.000000 waylay-sdk-0.0.5/src/waylay/sdk/api/serialization.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 14:02:37.701710 waylay-sdk-0.0.5/src/waylay/sdk/auth/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      523 2024-03-15 11:31:35.000000 waylay-sdk-0.0.5/src/waylay/sdk/auth/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      882 2024-03-08 11:24:03.000000 waylay-sdk-0.0.5/src/waylay/sdk/auth/exceptions.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     5972 2024-03-08 11:24:03.000000 waylay-sdk-0.0.5/src/waylay/sdk/auth/interactive.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    11539 2024-03-08 11:24:03.000000 waylay-sdk-0.0.5/src/waylay/sdk/auth/model.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      832 2024-03-08 11:24:03.000000 waylay-sdk-0.0.5/src/waylay/sdk/auth/parse.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4243 2024-03-08 11:24:03.000000 waylay-sdk-0.0.5/src/waylay/sdk/auth/provider.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1796 2024-03-28 11:04:55.000000 waylay-sdk-0.0.5/src/waylay/sdk/client.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 14:02:37.708324 waylay-sdk-0.0.5/src/waylay/sdk/config/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      341 2024-03-15 11:31:35.000000 waylay-sdk-0.0.5/src/waylay/sdk/config/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     3106 2024-03-21 16:22:46.000000 waylay-sdk-0.0.5/src/waylay/sdk/config/client.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    13667 2024-03-08 11:24:03.000000 waylay-sdk-0.0.5/src/waylay/sdk/config/model.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2809 2024-03-15 11:31:35.000000 waylay-sdk-0.0.5/src/waylay/sdk/exceptions.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 14:02:37.714947 waylay-sdk-0.0.5/src/waylay/sdk/plugin/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      229 2024-03-15 11:31:35.000000 waylay-sdk-0.0.5/src/waylay/sdk/plugin/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4401 2024-03-21 16:22:46.000000 waylay-sdk-0.0.5/src/waylay/sdk/plugin/base.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2373 2024-03-21 16:22:46.000000 waylay-sdk-0.0.5/src/waylay/sdk/plugin/client.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      177 2024-03-08 11:24:03.000000 waylay-sdk-0.0.5/src/waylay/sdk/plugin/loader.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2480 2024-03-28 11:04:55.000000 waylay-sdk-0.0.5/src/waylay/sdk/plugin/type_stubs.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       80 2024-02-13 14:44:08.000000 waylay-sdk-0.0.5/src/waylay/sdk/py.typed
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-03-28 14:02:37.722211 waylay-sdk-0.0.5/src/waylay_sdk.egg-info/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     9390 2024-03-28 14:02:37.000000 waylay-sdk-0.0.5/src/waylay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1036 2024-03-28 14:02:37.000000 waylay-sdk-0.0.5/src/waylay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-03-28 14:02:37.000000 waylay-sdk-0.0.5/src/waylay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       64 2024-03-28 14:02:37.000000 waylay-sdk-0.0.5/src/waylay_sdk.egg-info/entry_points.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      441 2024-03-28 14:02:37.000000 waylay-sdk-0.0.5/src/waylay_sdk.egg-info/requires.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        7 2024-03-28 14:02:37.000000 waylay-sdk-0.0.5/src/waylay_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.766450 waylay-sdk-0.0.6/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      746 2024-03-26 14:02:35.000000 waylay-sdk-0.0.6/LICENSE.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     9390 2024-04-08 08:05:16.763467 waylay-sdk-0.0.6/PKG-INFO
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     7018 2024-03-28 11:04:55.000000 waylay-sdk-0.0.6/README.md
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1663 2024-04-08 08:03:16.000000 waylay-sdk-0.0.6/pyproject.toml
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       38 2024-04-08 08:05:16.766523 waylay-sdk-0.0.6/setup.cfg
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.711405 waylay-sdk-0.0.6/src/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.710230 waylay-sdk-0.0.6/src/waylay/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.715760 waylay-sdk-0.0.6/src/waylay/sdk/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      754 2024-03-28 08:55:26.000000 waylay-sdk-0.0.6/src/waylay/sdk/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       60 2024-04-08 08:03:17.000000 waylay-sdk-0.0.6/src/waylay/sdk/_version.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.719756 waylay-sdk-0.0.6/src/waylay/sdk/api/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      661 2024-03-21 16:22:46.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     6130 2024-04-08 08:02:45.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/_models.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     4423 2024-03-28 08:55:26.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/client.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2298 2024-03-15 11:31:35.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/exceptions.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2299 2024-03-21 16:22:46.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/http.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)    10842 2024-03-29 09:16:21.000000 waylay-sdk-0.0.6/src/waylay/sdk/api/serialization.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.736117 waylay-sdk-0.0.6/src/waylay/sdk/auth/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      523 2024-03-15 11:31:35.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      882 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/exceptions.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     5972 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/interactive.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)    11539 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/model.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      832 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/parse.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     4243 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/auth/provider.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1880 2024-04-08 08:02:45.000000 waylay-sdk-0.0.6/src/waylay/sdk/client.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.739325 waylay-sdk-0.0.6/src/waylay/sdk/config/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      341 2024-03-15 11:31:35.000000 waylay-sdk-0.0.6/src/waylay/sdk/config/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     3106 2024-03-21 16:22:46.000000 waylay-sdk-0.0.6/src/waylay/sdk/config/client.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)    13667 2024-03-08 11:24:03.000000 waylay-sdk-0.0.6/src/waylay/sdk/config/model.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2809 2024-03-15 11:31:35.000000 waylay-sdk-0.0.6/src/waylay/sdk/exceptions.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.748324 waylay-sdk-0.0.6/src/waylay/sdk/plugin/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      229 2024-03-15 11:31:35.000000 waylay-sdk-0.0.6/src/waylay/sdk/plugin/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     4401 2024-03-21 16:22:46.000000 waylay-sdk-0.0.6/src/waylay/sdk/plugin/base.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2373 2024-03-21 16:22:46.000000 waylay-sdk-0.0.6/src/waylay/sdk/plugin/client.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      206 2024-04-08 08:02:45.000000 waylay-sdk-0.0.6/src/waylay/sdk/plugin/loader.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2480 2024-03-28 11:04:55.000000 waylay-sdk-0.0.6/src/waylay/sdk/plugin/type_stubs.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       80 2024-02-13 14:44:08.000000 waylay-sdk-0.0.6/src/waylay/sdk/py.typed
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.748875 waylay-sdk-0.0.6/src/waylay/sdk/services/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     4887 2024-04-08 08:02:45.000000 waylay-sdk-0.0.6/src/waylay/sdk/services/gateway.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-08 08:05:16.761854 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     9390 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1071 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       64 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      441 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/requires.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        7 2024-04-08 08:05:16.000000 waylay-sdk-0.0.6/src/waylay_sdk.egg-info/top_level.txt
```

### Comparing `waylay-sdk-0.0.5/LICENSE.txt` & `waylay-sdk-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/PKG-INFO` & `waylay-sdk-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2020, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice
```

### Comparing `waylay-sdk-0.0.5/README.md` & `waylay-sdk-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/pyproject.toml` & `waylay-sdk-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk"
-version = "0.0.5"
+version = "0.0.6"
 description = "Waylay Python SDK."
 requires-python = ">=3.9"
 keywords = ["waylay", "sdk"]
 readme = "README.md"
 authors = [{name = "Waylay", email = "info@waylay.io"}]
 license={file = "LICENSE.txt"}
 dependencies = [
```

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/__init__.py` & `waylay-sdk-0.0.6/src/waylay/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/api/__init__.py` & `waylay-sdk-0.0.6/src/waylay/sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/api/_models.py` & `waylay-sdk-0.0.6/src/waylay/sdk/api/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,21 +64,25 @@
             context = info.context or {}
             if context.get("skip_validation", False):
                 model = cls.model_construct(**value)
                 if not model.model_fields_set:
                     raise
                 for field_name in model.model_fields_set:
                     field_value = getattr(model, field_name)
-                    cls.__pydantic_validator__.validate_assignment(
-                        model,
-                        field_name,
-                        field_value,
-                        strict=(info.config or {}).get("strict"),
-                        context=context,
-                    )
+                    strict = (info.config or {}).get("strict")
+                    try:
+                        cls.__pydantic_validator__.validate_assignment(
+                            model,
+                            field_name,
+                            field_value,
+                            strict=strict,
+                            context=context,
+                        )
+                    except BaseException:
+                        pass
                 return model
             else:
                 raise
 
     @field_validator("*", mode="wrap")
     def _field_validator(
         cls, value: Any, handler: ValidatorFunctionWrapHandler, info: ValidationInfo
```

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/api/client.py` & `waylay-sdk-0.0.6/src/waylay/sdk/api/client.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/api/exceptions.py` & `waylay-sdk-0.0.6/src/waylay/sdk/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/api/http.py` & `waylay-sdk-0.0.6/src/waylay/sdk/api/http.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/api/serialization.py` & `waylay-sdk-0.0.6/src/waylay/sdk/api/serialization.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/auth/__init__.py` & `waylay-sdk-0.0.6/src/waylay/sdk/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/auth/exceptions.py` & `waylay-sdk-0.0.6/src/waylay/sdk/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/auth/interactive.py` & `waylay-sdk-0.0.6/src/waylay/sdk/auth/interactive.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/auth/model.py` & `waylay-sdk-0.0.6/src/waylay/sdk/auth/model.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/auth/parse.py` & `waylay-sdk-0.0.6/src/waylay/sdk/auth/parse.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/auth/provider.py` & `waylay-sdk-0.0.6/src/waylay/sdk/auth/provider.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/client.py` & `waylay-sdk-0.0.6/src/waylay/sdk/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """REST client for the Waylay Platform."""
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
 
+from waylay.sdk.services.gateway import GatewayService
+
 from .plugin.client import WithServicesAndTools
 from .config.client import WaylayConfig, WithConfig, HttpClientOptions
 from .api import ApiClient
 from .api.http import AsyncClient
 
 
 if TYPE_CHECKING:
@@ -19,14 +21,15 @@
         StorageService,
     )
 
 
 class WaylayClient(WithConfig, WithServicesAndTools):
     """REST client for the Waylay Platform."""
 
+    gateway: GatewayService
     alarms: "AlarmsService"
     data: "DataService"
     registry: "RegistryService"
     resources: "ResourcesService"
     rules: "RulesService"
     storage: "StorageService"
```

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/config/client.py` & `waylay-sdk-0.0.6/src/waylay/sdk/config/client.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/config/model.py` & `waylay-sdk-0.0.6/src/waylay/sdk/config/model.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/exceptions.py` & `waylay-sdk-0.0.6/src/waylay/sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/plugin/base.py` & `waylay-sdk-0.0.6/src/waylay/sdk/plugin/base.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/plugin/client.py` & `waylay-sdk-0.0.6/src/waylay/sdk/plugin/client.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay/sdk/plugin/type_stubs.py` & `waylay-sdk-0.0.6/src/waylay/sdk/plugin/type_stubs.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-0.0.5/src/waylay_sdk.egg-info/PKG-INFO` & `waylay-sdk-0.0.6/src/waylay_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2020, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice
```

### Comparing `waylay-sdk-0.0.5/src/waylay_sdk.egg-info/SOURCES.txt` & `waylay-sdk-0.0.6/src/waylay_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,13 +22,14 @@
 src/waylay/sdk/config/client.py
 src/waylay/sdk/config/model.py
 src/waylay/sdk/plugin/__init__.py
 src/waylay/sdk/plugin/base.py
 src/waylay/sdk/plugin/client.py
 src/waylay/sdk/plugin/loader.py
 src/waylay/sdk/plugin/type_stubs.py
+src/waylay/sdk/services/gateway.py
 src/waylay_sdk.egg-info/PKG-INFO
 src/waylay_sdk.egg-info/SOURCES.txt
 src/waylay_sdk.egg-info/dependency_links.txt
 src/waylay_sdk.egg-info/entry_points.txt
 src/waylay_sdk.egg-info/requires.txt
 src/waylay_sdk.egg-info/top_level.txt
```

