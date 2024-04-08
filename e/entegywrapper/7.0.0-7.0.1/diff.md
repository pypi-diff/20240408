# Comparing `tmp/entegywrapper-7.0.0.tar.gz` & `tmp/entegywrapper-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entegywrapper-7.0.0.tar", max compression
+gzip compressed data, was "entegywrapper-7.0.1.tar", max compression
```

## Comparing `entegywrapper-7.0.0.tar` & `entegywrapper-7.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2739 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/README.md
--rw-r--r--   0        0        0     8497 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/attendance_tracking/__init__.py
--rw-r--r--   0        0        0     5790 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/attendance_tracking/attendance_tracking.py
--rw-r--r--   0        0        0        0 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/content/__init__.py
--rw-r--r--   0        0        0    11946 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/content/categories.py
--rw-r--r--   0        0        0    11413 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/content/content.py
--rw-r--r--   0        0        0     3236 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/content/documents.py
--rw-r--r--   0        0        0     6928 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/content/multi_link.py
--rw-r--r--   0        0        0      716 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/errors.py
--rw-r--r--   0        0        0        0 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/notification/__init__.py
--rw-r--r--   0        0        0     5749 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/notification/notification.py
--rw-r--r--   0        0        0        0 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/plugins/__init__.py
--rw-r--r--   0        0        0     1323 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/plugins/ext_auth.py
--rw-r--r--   0        0        0        0 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/points/__init__.py
--rw-r--r--   0        0        0     4729 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/points/point_management.py
--rw-r--r--   0        0        0        0 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/profiles/__init__.py
--rw-r--r--   0        0        0     4286 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/profiles/profile_custom.py
--rw-r--r--   0        0        0    11869 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/profiles/profile_links.py
--rw-r--r--   0        0        0     2354 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/profiles/profile_payments.py
--rw-r--r--   0        0        0     6126 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/profiles/profile_types.py
--rw-r--r--   0        0        0    16279 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/profiles/profiles.py
--rw-r--r--   0        0        0        0 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/schemas/__init__.py
--rw-r--r--   0        0        0      236 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/schemas/attendance_tracking.py
--rw-r--r--   0        0        0     6626 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/schemas/content.py
--rw-r--r--   0        0        0      286 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/schemas/lead_capture.py
--rw-r--r--   0        0        0      334 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/schemas/page_settings.py
--rw-r--r--   0        0        0     1260 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/schemas/points.py
--rw-r--r--   0        0        0     4717 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/schemas/profile.py
--rw-r--r--   0        0        0     2068 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/schemas/project.py
--rw-r--r--   0        0        0      329 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/entegywrapper/schemas/schedule.py
--rw-r--r--   0        0        0      920 2024-03-25 05:15:50.051010 entegywrapper-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 entegywrapper-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2739 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/README.md
+-rw-r--r--   0        0        0     8497 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/attendance_tracking/__init__.py
+-rw-r--r--   0        0        0     5790 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/attendance_tracking/attendance_tracking.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/content/__init__.py
+-rw-r--r--   0        0        0    12219 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/content/categories.py
+-rw-r--r--   0        0        0    11413 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/content/content.py
+-rw-r--r--   0        0        0     3276 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/content/documents.py
+-rw-r--r--   0        0        0     6983 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/content/multi_link.py
+-rw-r--r--   0        0        0      716 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/errors.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/notification/__init__.py
+-rw-r--r--   0        0        0     5749 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/notification/notification.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/plugins/__init__.py
+-rw-r--r--   0        0        0     1323 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/plugins/ext_auth.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/points/__init__.py
+-rw-r--r--   0        0        0     4729 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/points/point_management.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/profiles/__init__.py
+-rw-r--r--   0        0        0     4286 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/profiles/profile_custom.py
+-rw-r--r--   0        0        0    11869 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/profiles/profile_links.py
+-rw-r--r--   0        0        0     2354 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/profiles/profile_payments.py
+-rw-r--r--   0        0        0     6126 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/profiles/profile_types.py
+-rw-r--r--   0        0        0    16279 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/profiles/profiles.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/schemas/__init__.py
+-rw-r--r--   0        0        0      236 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/schemas/attendance_tracking.py
+-rw-r--r--   0        0        0     6754 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/schemas/content.py
+-rw-r--r--   0        0        0      286 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/schemas/lead_capture.py
+-rw-r--r--   0        0        0      334 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/schemas/page_settings.py
+-rw-r--r--   0        0        0     1260 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/schemas/points.py
+-rw-r--r--   0        0        0     4717 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/schemas/profile.py
+-rw-r--r--   0        0        0     2068 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/schemas/project.py
+-rw-r--r--   0        0        0      329 2024-04-08 06:49:28.322022 entegywrapper-7.0.1/entegywrapper/schemas/schedule.py
+-rw-r--r--   0        0        0      920 2024-04-08 06:49:28.326022 entegywrapper-7.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 entegywrapper-7.0.1/PKG-INFO
```

### Comparing `entegywrapper-7.0.0/README.md` & `entegywrapper-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/__init__.py` & `entegywrapper-7.0.1/entegywrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/attendance_tracking/attendance_tracking.py` & `entegywrapper-7.0.1/entegywrapper/attendance_tracking/attendance_tracking.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/content/categories.py` & `entegywrapper-7.0.1/entegywrapper/content/categories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Optional
 
 from entegywrapper.errors import EntegyFailedRequestError
-from entegywrapper.schemas.content import Category, TemplateType
+from entegywrapper.schemas.content import Category, ContentCreate, TemplateType
 
 if TYPE_CHECKING:
     from entegywrapper import EntegyAPI
 
 
 def available_categories(
     self: EntegyAPI,
@@ -34,15 +34,15 @@
 
         `EntegyFailedRequestError`: if the API request fails
 
     Returns
     -------
         `list[Category]`: the available categories
     """
-    data = {"templateType": template_type}
+    data: dict[str, Any] = {"templateType": template_type}
 
     if module_id is not None:
         data["moduleId"] = module_id
     elif external_reference is not None:
         data["externalReference"] = external_reference
     else:
         raise ValueError("Please specify an identifier")
@@ -162,15 +162,15 @@
     else:
         raise ValueError("Please specify an identifier")
 
     response = self.post(self.api_endpoint + "/v2/Categories/Deselect", data=data)
 
     match response["response"]:
         case 200:
-            return
+            return True
         case 401:
             raise EntegyFailedRequestError("Missing Id")
         case 402:
             raise EntegyFailedRequestError("templateType doesn't support categories")
         case 404:
             raise EntegyFailedRequestError("Category doesn't exist")
         case 405:
@@ -178,43 +178,48 @@
         case 406:
             raise EntegyFailedRequestError("No categories to unselect")
         case _:
             raise EntegyFailedRequestError(
                 f"{response['response']}: {response.get('message', 'Unknown error')}"
             )
 
+    return False
+
 
 def create_categories(
     self: EntegyAPI,
     template_type: TemplateType,
-    categories: list[Category],
+    categories: list[Category] | list[ContentCreate],
     *,
     module_id: Optional[int] = None,
     external_reference: Optional[str] = None,
 ):
     """
     Creates categories under a root page.
 
     Parameters
     ----------
         `template_type` (`TemplateType`): the templateType of the page holding the categories
 
-        `categories` (`list[Category]`): the categories to create
+        `categories` (`list[Category | ContentCreate]]`): the categories to create
 
         `module_id` (`int`, optional): the moduleId of the page holding the categories; defaults to `None`
 
         `external_reference` (`str`, optional): the externalReference of the page holding the categories; defaults to `None`
 
     Raises
     ------
         `ValueError`: if no identifier is specified
 
         `EntegyFailedRequestError`: if the API request fails
     """
-    data = {"templateType": template_type, "categories": categories}
+    data = {
+        "templateType": template_type,
+        "categories": [category.model_dump() for category in categories],
+    }
 
     if module_id is not None:
         data["moduleId"] = module_id
     elif external_reference is not None:
         data["externalReference"] = external_reference
     else:
         raise ValueError("Please specify an identifier")
@@ -258,15 +263,15 @@
 
     Raises
     ------
         `ValueError`: if no identifier is specified
 
         `EntegyFailedRequestError`: if the API request fails
     """
-    data = {"categories": categories}
+    data = {"categories": [category.model_dump() for category in categories]}
 
     if module_id is not None:
         data["moduleId"] = module_id
     elif external_reference is not None:
         data["externalReference"] = external_reference
     else:
         raise ValueError("Please specify an identifier")
@@ -308,15 +313,15 @@
 
     Raises
     ------
         `ValueError`: if no identifier is specified
 
         `EntegyFailedRequestError`: if the API request fails
     """
-    data = {"name": name}
+    data: dict[str, Any] = {"name": name}
 
     if module_id is not None:
         data["moduleId"] = module_id
     elif external_reference is not None:
         data["externalReference"] = external_reference
     else:
         raise ValueError("Please specify an identifier")
@@ -359,24 +364,27 @@
 
     Raises
     ------
         `ValueError`: if no identifier is specified
 
         `EntegyFailedRequestError`: if the API request fails
     """
-    data = {"templateType": template_type, "categories": categories}
+    data = {
+        "templateType": template_type,
+        "categories": [category.model_dump() for category in categories],
+    }
 
     if module_id is not None:
         data["moduleId"] = module_id
     elif external_reference is not None:
         data["externalReference"] = external_reference
     else:
         raise ValueError("Please specify an identifier")
 
-    response = self.delete(self.api_endpoint + "/v2/Categories/Delete", data=data)
+    response = self.post(self.api_endpoint + "/v2/Categories/Delete", data=data)
 
     match response["response"]:
         case 200:
             return
         case 401:
             raise EntegyFailedRequestError("Missing Id")
         case 404:
```

### Comparing `entegywrapper-7.0.0/entegywrapper/content/content.py` & `entegywrapper-7.0.1/entegywrapper/content/content.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/content/documents.py` & `entegywrapper-7.0.1/entegywrapper/content/documents.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ------
         `ValueError`: if no identifier is specified
 
         `EntegyFailedRequestError`: if the API request fails
     """
     data = {
         "templateType": template_type,
-        "fileDocuments": file_documents,
+        "fileDocuments": [document.model_dump() for document in file_documents],
     }
 
     if module_id is not None:
         data["moduleId"] = module_id
     elif external_reference is not None:
         data["externalReference"] = external_reference
     else:
```

### Comparing `entegywrapper-7.0.0/entegywrapper/content/multi_link.py` & `entegywrapper-7.0.1/entegywrapper/content/multi_link.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,18 @@
 
     Raises
     ------
         `ValueError`: if no identifier is specified
 
         `EntegyFailedRequestError`: if the API request fails
     """
-    data = {"templateType": template_type, "multiLinks": multi_links}
+    data = {
+        "templateType": template_type,
+        "multiLinks": [link.model_dump() for link in multi_links],
+    }
 
     if module_id is not None:
         data["moduleId"] = module_id
     elif external_reference is not None:
         data["externalReference"] = external_reference
     else:
         raise ValueError("Please specify an identifier")
```

### Comparing `entegywrapper-7.0.0/entegywrapper/errors.py` & `entegywrapper-7.0.1/entegywrapper/errors.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/notification/notification.py` & `entegywrapper-7.0.1/entegywrapper/notification/notification.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/plugins/ext_auth.py` & `entegywrapper-7.0.1/entegywrapper/plugins/ext_auth.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/points/point_management.py` & `entegywrapper-7.0.1/entegywrapper/points/point_management.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/profiles/profile_custom.py` & `entegywrapper-7.0.1/entegywrapper/profiles/profile_custom.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/profiles/profile_links.py` & `entegywrapper-7.0.1/entegywrapper/profiles/profile_links.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/profiles/profile_payments.py` & `entegywrapper-7.0.1/entegywrapper/profiles/profile_payments.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/profiles/profile_types.py` & `entegywrapper-7.0.1/entegywrapper/profiles/profile_types.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/profiles/profiles.py` & `entegywrapper-7.0.1/entegywrapper/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/schemas/content.py` & `entegywrapper-7.0.1/entegywrapper/schemas/content.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,37 +131,37 @@
     icon: Icon
     fileUrl: str
     type: str
 
 
 class Link(BaseModel):
     templateType: TemplateType
-    moduleId: int
+    moduleId: Optional[int] = None  # Optional when creating, not optional when retrieving.
     externalReference: str
 
 
 class NamedLink(Link):
     name: str
 
 
 class Category(BaseModel):
-    moduleId: Optional[int]
     externalReference: str
-    name: Optional[str] = None
+    name: str
+    moduleId: Optional[int] = None  # Optional when creating, not optional when retrieving.
     childCategories: list["Category"] = []
 
 
 class Content(BaseModel):
     name: str
     templateType: TemplateType
     externalReference: str
     mainImage: str
     strings: dict[str, str]
     contentType: Optional[str] = None
-    moduleId: Optional[int]  # Optional when creating, not optional when retrieving.
+    moduleId: Optional[int] = None  # Optional when creating, not optional when retrieving.
     pageSettings: Optional[dict[PageSetting, bool]] = None
     sortOrder: Optional[int] = None
     documents: Optional[list[Document]] = None
     links: Optional[list[Link]] = None
     multiLinks: Optional[list[NamedLink]] = None
     selectedCategories: Optional[list[Category]] = None
     children: Optional[list[Content]] = None
```

### Comparing `entegywrapper-7.0.0/entegywrapper/schemas/points.py` & `entegywrapper-7.0.1/entegywrapper/schemas/points.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/schemas/profile.py` & `entegywrapper-7.0.1/entegywrapper/schemas/profile.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/entegywrapper/schemas/project.py` & `entegywrapper-7.0.1/entegywrapper/schemas/project.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.0.0/pyproject.toml` & `entegywrapper-7.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core>=1.0.0a5"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "entegywrapper"
-version = "7.0.0"
+version = "7.0.1"
 requires-python = ">=3.10"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.poetry]
 name = "entegywrapper"
-version = "7.0.0"
+version = "7.0.1"
 description = "Python SDK for the Entegy API"
 authors = [
     "Situ Development <developer@situ.com.au>",
     "William Sawyer <william@situ.com.au>",
     "Nathan Thomas <nathan@situ.com.au>",
 ]
 readme = "README.md"
```

### Comparing `entegywrapper-7.0.0/PKG-INFO` & `entegywrapper-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entegywrapper
-Version: 7.0.0
+Version: 7.0.1
 Summary: Python SDK for the Entegy API
 Home-page: https://github.com/SituDevelopment/entegy-sdk-python
 Author: Situ Development
 Author-email: developer@situ.com.au
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

