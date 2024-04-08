# Comparing `tmp/wiliot-api-4.8.0.tar.gz` & `tmp/wiliot-api-4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-api-4.8.0.tar", last modified: Fri Apr  5 05:17:05 2024, max compression
+gzip compressed data, was "wiliot-api-4.8.1.tar", last modified: Mon Apr  8 11:06:06 2024, max compression
```

## Comparing `wiliot-api-4.8.0.tar` & `wiliot-api-4.8.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)    11137 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10631 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     9514 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1685 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.940864 wiliot-api-4.8.0/wiliot_api/
--rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13768 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.940864 wiliot-api-4.8.0/wiliot_api/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/edge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20455 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/edge/edge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.940864 wiliot-api-4.8.0/wiliot_api/edge/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/edge/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5799 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/edge/examples/edge_api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.940864 wiliot-api-4.8.0/wiliot_api/manufacturing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/manufacturing/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/wiliot_api/manufacturing/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/manufacturing/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/manufacturing/examples/mannufacturing_api.py
--rw-rw-rw-   0 root         (0) root         (0)    23403 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/manufacturing/manufacturing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/wiliot_api/platform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/platform/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/wiliot_api/platform/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/platform/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5899 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/platform/examples/platform_api.py
--rw-rw-rw-   0 root         (0) root         (0)    52224 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/platform/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/platform/platform_models.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/wiliot_api/security/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/security/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7096 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/security/security.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/wiliot_api/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6184 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.940864 wiliot-api-4.8.0/wiliot_api.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    11137 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)    11225 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10719 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     9514 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.631605 wiliot-api-4.8.1/wiliot_api/
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13768 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/edge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20455 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/edge/edge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/edge/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/edge/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/edge/examples/edge_api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/manufacturing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/manufacturing/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/manufacturing/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/manufacturing/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/manufacturing/examples/mannufacturing_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    23403 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/manufacturing/manufacturing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/platform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/platform/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/platform/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/platform/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/platform/examples/platform_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    52463 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/platform/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/platform/platform_models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7096 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/security/security.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6184 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.631605 wiliot-api-4.8.1/wiliot_api.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    11225 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/top_level.txt
```

### Comparing `wiliot-api-4.8.0/LICENSE` & `wiliot-api-4.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/PKG-INFO` & `wiliot-api-4.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.8.0
+Version: 4.8.1
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -38,14 +38,18 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.1:
+
+* Fixed a bug in setting multiple key value pairs in a single call
+
 ### Version 4.8.0:
 
 * Added support for new labels (key:value pairs for platform entities)
 
 ### Version 4.7.1:
 
 * Added option to upload testers data to cloud
```

### Comparing `wiliot-api-4.8.0/README.md` & `wiliot-api-4.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.1:
+
+* Fixed a bug in setting multiple key value pairs in a single call
+
 ### Version 4.8.0:
 
 * Added support for new labels (key:value pairs for platform entities)
 
 ### Version 4.7.1:
 
 * Added option to upload testers data to cloud
```

### Comparing `wiliot-api-4.8.0/bitbucket-pipelines.yml` & `wiliot-api-4.8.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/setup.py` & `wiliot-api-4.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/wiliot_api/__init__.py` & `wiliot-api-4.8.1/wiliot_api/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/wiliot_api/api_client.py` & `wiliot-api-4.8.1/wiliot_api/api_client.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/wiliot_api/edge/edge.py` & `wiliot-api-4.8.1/wiliot_api/edge/edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/wiliot_api/edge/examples/edge_api.py` & `wiliot-api-4.8.1/wiliot_api/edge/examples/edge_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/wiliot_api/manufacturing/examples/mannufacturing_api.py` & `wiliot-api-4.8.1/wiliot_api/manufacturing/examples/mannufacturing_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/wiliot_api/manufacturing/manufacturing.py` & `wiliot-api-4.8.1/wiliot_api/manufacturing/manufacturing.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/wiliot_api/platform/examples/platform_api.py` & `wiliot-api-4.8.1/wiliot_api/platform/examples/platform_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/wiliot_api/platform/platform.py` & `wiliot-api-4.8.1/wiliot_api/platform/platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1132,60 +1132,65 @@
         :param entity_type: EntityType - Required - the entity type of the entity to add the key value pair to
         :param entity_ids: List - Required - a list of entity IDs to add the key value pairs to
         :param keys_values: Dictionary - Required - A dictionary of key and values to add to the specified entities
         :param overwrite_existing: Boolean - Optional - If True any existing association to the requested labels will not be overwritten
         :return: Boolean - True if successful, False otherwise
         """
         # For each key value pair in the keys_value dictionary - create the label if it doesn't already exist
+        key_ids_and_values = {}
         for key, value in keys_values.items():
             try:
                 res = self._create_labels(entity_type=entity_type, keys=[key])
                 # Since we're only trying to create a single label - a success means we were able to
                 label_id = res['data'][0]['id']
+                key_ids_and_values[label_id] = value
             except WiliotCloudError as wce:
                 # Check if the error is that the label already exists
                 if wce.args[0].get('data', {}).get('failedLabels', [{}])[0].get('reason', '').find('exist') != -1:
                     label_id = wce.args[0]['data']['failedLabels'][0].get('labelId', None)
+                    key_ids_and_values[label_id] = value
                 else:
                     print(f"Failed to create label {key} for entity type {entity_type} due to: {wce.args[0]}. Will not create a key-value pair")
                     continue
-            # Once we have a label ID - new or existing - associate a new value for a specific entity
-            try:
-                res = self._associate_labels_to_entities(entity_type=entity_type,
-                                                         entity_ids=entity_ids,
-                                                         label_values=[{"labelId": label_id, "value": value}])
-                if res['status_code'] == 200:
-                    return True
-                elif res['status_code'] == 207:
-                    # Partial success
-                    if overwrite_existing:
-                        for entity in res['data']:
-                            if entity['status'].lower() != 'success':
-                                for label in entity['failedLabels']:
-                                    if label['reason'].find('exist') != -1:
-                                        # If there is already a value associated with this label for this entity - update it
-                                        self._update_label_value_for_entities(entity_type=entity_type,
-                                                                              entity_ids=[entity['entityId']],
-                                                                              label_values=[{'labelId': label['labelId'], 'value': value}])
-                                        return True
-                else:
-                    return False
-
-            except WiliotCloudError as wce:
-                # If asked to overwrite - examine the results
+        # Once we have a label ID - new or existing - associate a new value for a specific entity
+        try:
+            res = self._associate_labels_to_entities(entity_type=entity_type,
+                                                     entity_ids=entity_ids,
+                                                     label_values=[{'labelId': key,
+                                                                    'value': value} for key, value in key_ids_and_values.items()])
+            if res['status_code'] == 200:
+                return True
+            elif res['status_code'] == 207:
+                # Partial success
                 if overwrite_existing:
-                    for entity in wce.args[0]['data']:
-                        for label in entity.get('failedLabels'):
-                            if label.get('reason').find('exists') != -1:
-                                self._update_label_value_for_entities(entity_type=entity_type,
-                                                                      entity_ids=[entity['entityId']],
-                                                                      label_values=[{'labelId': label['labelId'], 'value': value}])
-                                return True
-                else:
-                    raise
+                    for entity in res['data']:
+                        if entity['status'].lower() != 'success':
+                            for label in entity['failedLabels']:
+                                if label['reason'].find('exist') != -1:
+                                    # If there is already a value associated with this label for this entity - update it
+                                    self._update_label_value_for_entities(entity_type=entity_type,
+                                                                          entity_ids=[entity['entityId']],
+                                                                          label_values=[{'labelId': key,
+                                                                                         'value': value} for key, value in key_ids_and_values.items()])
+                                    return True
+            else:
+                return False
+
+        except WiliotCloudError as wce:
+            # If asked to overwrite - examine the results
+            if overwrite_existing:
+                for entity in wce.args[0]['data']:
+                    for label in entity.get('failedLabels'):
+                        if label.get('reason').find('exists') != -1:
+                            self._update_label_value_for_entities(entity_type=entity_type,
+                                                                  entity_ids=[entity['entityId']],
+                                                                  label_values=[{'labelId': label['labelId'], 'value': value}])
+                            return True
+            else:
+                raise
 
     def get_entity_keys_values(self, entity_type: EntityType, entity_id: str, key: str=None):
         """
         Get all key value pairs for an entity
         :param entity_type: EntityType - Required - the entity type of the entity to add the key value pair to
         :param entity_id: String - Required - the ID of the entity to query
         :param key: String - Optional - filter only values for the provided key
```

### Comparing `wiliot-api-4.8.0/wiliot_api/platform/platform_models.py` & `wiliot-api-4.8.1/wiliot_api/platform/platform_models.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/wiliot_api/security/security.py` & `wiliot-api-4.8.1/wiliot_api/security/security.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/wiliot_api/utils/get_version.py` & `wiliot-api-4.8.1/wiliot_api/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.0/wiliot_api.egg-info/PKG-INFO` & `wiliot-api-4.8.1/wiliot_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.8.0
+Version: 4.8.1
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -38,14 +38,18 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.1:
+
+* Fixed a bug in setting multiple key value pairs in a single call
+
 ### Version 4.8.0:
 
 * Added support for new labels (key:value pairs for platform entities)
 
 ### Version 4.7.1:
 
 * Added option to upload testers data to cloud
```

### Comparing `wiliot-api-4.8.0/wiliot_api.egg-info/SOURCES.txt` & `wiliot-api-4.8.1/wiliot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

