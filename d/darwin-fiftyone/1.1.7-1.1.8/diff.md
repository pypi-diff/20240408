# Comparing `tmp/darwin-fiftyone-1.1.7.tar.gz` & `tmp/darwin-fiftyone-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darwin-fiftyone-1.1.7.tar", last modified: Wed Mar 20 18:38:27 2024, max compression
+gzip compressed data, was "darwin-fiftyone-1.1.8.tar", last modified: Mon Apr  8 15:49:23 2024, max compression
```

## Comparing `darwin-fiftyone-1.1.7.tar` & `darwin-fiftyone-1.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:38:27.638790 darwin-fiftyone-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-20 18:38:22.000000 darwin-fiftyone-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-20 18:38:27.638790 darwin-fiftyone-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-20 18:38:22.000000 darwin-fiftyone-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:38:27.634790 darwin-fiftyone-1.1.7/darwin_fiftyone/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-20 18:38:22.000000 darwin-fiftyone-1.1.7/darwin_fiftyone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63486 2024-03-20 18:38:22.000000 darwin-fiftyone-1.1.7/darwin_fiftyone/darwin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:38:27.638790 darwin-fiftyone-1.1.7/darwin_fiftyone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-20 18:38:27.000000 darwin-fiftyone-1.1.7/darwin_fiftyone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-20 18:38:27.000000 darwin-fiftyone-1.1.7/darwin_fiftyone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 18:38:27.000000 darwin-fiftyone-1.1.7/darwin_fiftyone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-20 18:38:27.000000 darwin-fiftyone-1.1.7/darwin_fiftyone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 18:38:27.000000 darwin-fiftyone-1.1.7/darwin_fiftyone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 18:38:27.638790 darwin-fiftyone-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-20 18:38:22.000000 darwin-fiftyone-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:49:23.983510 darwin-fiftyone-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 15:49:19.000000 darwin-fiftyone-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-08 15:49:23.983510 darwin-fiftyone-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-08 15:49:19.000000 darwin-fiftyone-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:49:23.983510 darwin-fiftyone-1.1.8/darwin_fiftyone/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 15:49:19.000000 darwin-fiftyone-1.1.8/darwin_fiftyone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64771 2024-04-08 15:49:19.000000 darwin-fiftyone-1.1.8/darwin_fiftyone/darwin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:49:23.983510 darwin-fiftyone-1.1.8/darwin_fiftyone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-08 15:49:23.000000 darwin-fiftyone-1.1.8/darwin_fiftyone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 15:49:23.000000 darwin-fiftyone-1.1.8/darwin_fiftyone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:49:23.000000 darwin-fiftyone-1.1.8/darwin_fiftyone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 15:49:23.000000 darwin-fiftyone-1.1.8/darwin_fiftyone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 15:49:23.000000 darwin-fiftyone-1.1.8/darwin_fiftyone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:49:23.983510 darwin-fiftyone-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 15:49:19.000000 darwin-fiftyone-1.1.8/setup.py
```

### Comparing `darwin-fiftyone-1.1.7/LICENSE` & `darwin-fiftyone-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `darwin-fiftyone-1.1.7/PKG-INFO` & `darwin-fiftyone-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darwin-fiftyone
-Version: 1.1.7
+Version: 1.1.8
 Summary: Integration between V7 Darwin and Voxel51
 Home-page: https://github.com/v7labs/darwin_fiftyone
 Author: Simon Edwardsson & Mark Cox-Smith
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: darwin-py
 Requires-Dist: fiftyone
```

### Comparing `darwin-fiftyone-1.1.7/README.md` & `darwin-fiftyone-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `darwin-fiftyone-1.1.7/darwin_fiftyone/darwin.py` & `darwin-fiftyone-1.1.8/darwin_fiftyone/darwin.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,26 +39,28 @@
         media_field="filepath",
         api_key=None,
         dataset_slug=None,
         atts=None,
         external_storage=None,
         base_url = "https://darwin.v7labs.com/api/v2/teams",
         item_name_annotation=False,
+        custom_filename_sample_id_map={},
         **kwargs,
     ):
         super().__init__(
             name=name, label_schema=label_schema, media_field=media_field, **kwargs
         )
 
         self.dataset_slug = dataset_slug
         self.atts = atts
         self.external_storage = external_storage
         self.base_url = base_url
         self._api_key = api_key
         self.item_name_annotation = item_name_annotation
+        self.custom_filename_sample_id_map = custom_filename_sample_id_map
 
     @property
     def api_key(self):
         return self._api_key
 
     @api_key.setter
     def api_key(self, value):
@@ -91,14 +93,15 @@
         ]
 
     @property
     def supported_attr_types(self):
         return [
             "text",
             "select",
+            "radio"
         ]
 
     @property
     def supports_keyframes(self):
         return True
 
     @property
@@ -173,28 +176,28 @@
         """
         logger.info('upload anns')
         
         label_schema = backend.config.label_schema
         media_field = backend.config.media_field
         external_storage = backend.config.external_storage
         base_url = backend.config.base_url
+        custom_filename_sample_id_map = backend.config.custom_filename_sample_id_map
 
         logger.debug(f'label_schema: {str(label_schema)}')
 
         assert label_schema, "Voxel51 label_schema must be provided"
 
         if backend.config.dataset_slug is None:
             backend.config.dataset_slug = f"voxel51-{uuid.uuid4().hex}"
 
         try:
             dataset = self._client.get_remote_dataset(backend.config.dataset_slug)
         except darwin.exceptions.NotFound:
             dataset = self._client.create_dataset(backend.config.dataset_slug)
 
-        # External Storage Logic
         if external_storage:
             result = _register_items(
                 samples,
                 backend.config.api_key,
                 dataset.slug,
                 dataset.team,
                 external_storage,
@@ -205,24 +208,37 @@
             logger.info("Paths to upload",samples.values(media_field))
             result = dataset.push(files_to_upload=samples.values(media_field))
 
         filename_sample_id_map = {
             Path(sample[media_field]).name: sample.id for sample in samples
         }
 
-        if external_storage:
+        voxel_file_list = [k for k in filename_sample_id_map.keys()]
+        darwin_dataset_items = _list_items(backend.config.api_key, dataset.dataset_id, dataset.team,base_url)
+        annotation_run_items = [item for item in darwin_dataset_items if item["name"] in voxel_file_list]
+
+        if external_storage and custom_filename_sample_id_map == {}:
             item_sample_map = {
                 item.get("id"): {
                     "filename": item.get("name"),
                     "sample_id": filename_sample_id_map[item.get("name")],
                 }
-                for item in _list_items(
-                    backend.config.api_key, dataset.dataset_id, dataset.team,base_url
-                )
+                for item in annotation_run_items
             }
+
+        #Can be used to handle the duplicate name issue
+        elif external_storage and custom_filename_sample_id_map:
+            item_sample_map = {
+                item.get("id"): {
+                    "filename": item.get("name"),
+                    "sample_id": custom_filename_sample_id_map[item.get("id")],
+                }
+                for item in annotation_run_items
+            }
+
         else:
             item_sample_map = {
                 item.dataset_item_id: {
                     "filename": item.filename,
                     "sample_id": filename_sample_id_map[item.filename],
                 }
                 for item in result.blocked_items + result.pending_items
@@ -326,15 +342,14 @@
         -------
         list
             A list of Darwin annotations.
         """
         
         annotation_label = annotation.label
 
-        #Item name class setting
         if backend.config.item_name_annotation and annotation.label in ["Item","item","ITEM"]:
             external_path = sample.filepath
             path_list = external_path.split("/")
             sample_name = path_list[-1]
             annotation_label = sample_name
 
         darwin_annotation = _v7_basic_annotation(
@@ -566,15 +581,15 @@
             list
             A list of properties extracted from the label schema.
         """
         if "type" in class_schema["attributes"][prop]:
             if class_schema["attributes"][prop]["type"] == "select":
                 select_type = "single_select"
             elif class_schema["attributes"][prop]["type"] == "radio":
-                logger.info("Radio attribute not supported in V7 Darwin. Switching to single select property.")
+                logger.info("Radio attribute not supported in V7 Darwin. Converting to single select property.")
                 select_type = "single_select"
             else:
                 select_type = "multi_select"
         else:
             logger.info("No type found for property, defaulting to single_select")
             select_type = "single_select"
 
@@ -592,15 +607,15 @@
             "property_values": []
         }
 
         for val in vals:
             val_dict = {
                     "type": "string",
                     "color": "rgba(58,23,197,1.0)",
-                    "value": val
+                    "value": str(val)
                 }
             payload["property_values"].append(val_dict)
         
         assert payload["property_values"], "Please ensure that all select attributes have a list of possible values in your label schema"
         return payload
 
 
@@ -857,15 +872,15 @@
                         continue
                     sample_id = item_sample_map[item_id]["sample_id"]
                     width = data["item"]["slots"][0]["width"]
                     height = data["item"]["slots"][0]["height"]
                     item_name = data["item"]["name"]
 
                     is_darwin_video = False
-                    #Detects if video
+
                     if data["item"]["slots"][0]["type"] == "video":
                         is_darwin_video = True
                         frame_count = data["item"]["slots"][0]["frame_count"]
                         frame_dict = {}
                         for frame_number in range(1,frame_count+2):
                             frame_dict.update({frame_number: {}})
 
@@ -934,14 +949,21 @@
                             if "instance_id" in frame_annotation:
                                 darwin_attributes["darwin_instance_id"] = frame_annotation["instance_id"]["value"]
 
                             #Adding text support
                             if "text" in frame_annotation:
                                  darwin_attributes["Text"] = frame_annotation["text"]["text"]
 
+                            #Add in/out view or occluded here
+                            if "hidden_areas" in annotation:
+                                darwin_attributes["occluded"] = "False"
+                                for hidden_area in annotation["hidden_areas"]:
+                                    if hidden_area[0] <= int(frame_number) <= hidden_area[1]:
+                                        darwin_attributes["occluded"] = "True"
+
                             if "inference" in frame_annotation:
                                 confidence = frame_annotation["inference"]["confidence"] if "confidence" in frame_annotation["inference"] else None
 
                             voxel_annotation = None
                             if "polygon" in frame_annotation and label_type in ["polygons", "polylines"]:
                                 if len(frame_annotation["polygon"]["paths"]) == 1:
                                     logger.info(f"Processing simple polygons")
@@ -992,15 +1014,15 @@
                                     width,
                                     attributes=darwin_attributes,
                                 )
 
                             #Ignores non matching annotation types with label_type 
                             if not voxel_annotation:
                                 continue
-
+                                    
                             #Adding confidence score
                             if confidence:
                                 voxel_annotation.confidence = confidence
 
                             #Adding direct attributes
                             if direct_attribute:
                                 for key,val in direct_attribute_dict.items():
@@ -1392,24 +1414,22 @@
 # Registering External Storage Items
 def _register_items(samples, api_key, dataset_slug, team_slug, external_storage, base_url):
     """
     Registers external storage items in Darwin
 
     Only readwrite currently supported
     """
-
     logger.info("item registration started")
 
     headers = {
         "Content-Type": "application/json",
         "Accept": "application/json",
         "Authorization": f"ApiKey {api_key}",
     }
 
-    items = []
     item_list = []
 
     for sample in samples:
         external_path = sample.filepath
         path_list = external_path.split("/")
         name = path_list[-1]
         item_list.append(name)
@@ -1422,33 +1442,35 @@
                     "slot_name": "0",
                     "storage_key": new_path,
                     "file_name": name,
                 }
             ],
             "name": name,
         }
-        items.append(temp_dict)
 
-    payload = {
-        "items": items,
-        "dataset_slug": dataset_slug,
-        "storage_slug": external_storage,
-    }
+        payload = {
+            "items": [temp_dict],
+            "dataset_slug": dataset_slug,
+            "storage_slug": external_storage,
+        }
 
-    response = requests.post(
-        f"{base_url}/{team_slug}/items/register_existing",
-        headers=headers,
-        json=payload,
-    )
+        response = requests.post(
+            f"{base_url}/{team_slug}/items/register_existing",
+            headers=headers,
+            json=payload,
+        )
+
+        if response.ok:
+            logger.info(f"Item registration complete for {name}")
+
+        else:
+            logger.error(f"Item {name} registration failed with status code {response.status_code}. Skipping item registration")
+    
+    return item_list
 
-    if response.ok:
-        logger.info("Item registration complete")
-        return item_list
-    else:
-        raise requests.exceptions.HTTPError(f"POST request failed with status code {response.status_code}.")
 
 
 def _v7_basic_annotation(
     label,
     annotators: list = [],
     reviewers: list = [],
     confidence=None,
@@ -1625,8 +1647,8 @@
     "instances": "segmentation",
     "polygons": "polylines",
     "polygon": "polylines",
     "polyline": "polylines",
     "polylines": "polylines",
     "keypoint": "keypoints",
     "keypoints": "keypoints",
-}
+}
```

### Comparing `darwin-fiftyone-1.1.7/darwin_fiftyone.egg-info/PKG-INFO` & `darwin-fiftyone-1.1.8/darwin_fiftyone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darwin-fiftyone
-Version: 1.1.7
+Version: 1.1.8
 Summary: Integration between V7 Darwin and Voxel51
 Home-page: https://github.com/v7labs/darwin_fiftyone
 Author: Simon Edwardsson & Mark Cox-Smith
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: darwin-py
 Requires-Dist: fiftyone
```

