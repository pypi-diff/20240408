# Comparing `tmp/social_interaction_cloud-1.2.2.tar.gz` & `tmp/social_interaction_cloud-1.2.3.tar.gz`

## Comparing `social_interaction_cloud-1.2.2.tar` & `social_interaction_cloud-1.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.2/src/social_interaction_cloud/__init__.py
--rw-r--r--   0        0        0    41181 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.2/src/social_interaction_cloud/abstract_connector.py
--rw-r--r--   0        0        0    44886 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.2/src/social_interaction_cloud/basic_connector.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.2/src/social_interaction_cloud/choregraphe_to_json.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.2/src/social_interaction_cloud/detection_result_pb2.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.2/src/social_interaction_cloud/tracking_result_pb2.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.2/LICENSE
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.2/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.3/src/social_interaction_cloud/__init__.py
+-rw-r--r--   0        0        0    41181 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.3/src/social_interaction_cloud/abstract_connector.py
+-rw-r--r--   0        0        0    44859 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.3/src/social_interaction_cloud/basic_connector.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.3/src/social_interaction_cloud/choregraphe_to_json.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.3/src/social_interaction_cloud/detection_result_pb2.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.3/src/social_interaction_cloud/tracking_result_pb2.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.3/LICENSE
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.3/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.3/PKG-INFO
```

### Comparing `social_interaction_cloud-1.2.2/src/social_interaction_cloud/abstract_connector.py` & `social_interaction_cloud-1.2.3/src/social_interaction_cloud/abstract_connector.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.2/src/social_interaction_cloud/basic_connector.py` & `social_interaction_cloud-1.2.3/src/social_interaction_cloud/basic_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,22 +676,22 @@
     def set_memory_session(self, interactant_id: str, session_id: str, callback: callable = None,
                            sync: bool = True, load: bool = False):
         self.__process_action(super(BasicSICConnector, self).set_memory_session, interactant_id, session_id,
                               callback=callback, event='SessionSet', sync=sync, load=load)
 
     def set_memory_entry(self, interactant_id: str, entry_type: str, entry_data: dict,
                          callback: callable = None, sync: bool = True, load: bool = False) -> None:
-        self.__process_action(super(BasicSICConnector, self).set_memory_session, interactant_id, entry_type, entry_data,
+        self.__process_action(super(BasicSICConnector, self).set_memory_entry, interactant_id, entry_type, entry_data,
                               callback=callback, event='MemoryEntryStored', sync=sync, load=load,
                               listener_type=ListenerType.MEMORY)
 
     def get_memory_entry(self, interactant_id: str, entry_type: str, entry_id: str,
                          callback: callable = None, sync: bool = True, load: bool = False) -> None:
         self.__process_action(super(BasicSICConnector, self).get_memory_entry, interactant_id, entry_type, entry_id,
-                              callback=callback, event=f'Entry_{entry_type}_{entry_id}', sync=sync, load=load,
+                              callback=callback, event='Entry', sync=sync, load=load,
                               listener_type=ListenerType.MEMORY)
 
     def get_memory_entries(self, interactant_id: str, entry_type: str, callback: callable = None,
                            sync: bool = True, load: bool = False):
         self.__process_action(super(BasicSICConnector, self).get_memory_entries, interactant_id, entry_type,
                               callback=callback, event=f'Entries_{entry_type}', sync=sync, load=load,
                               listener_type=ListenerType.MEMORY)
```

### Comparing `social_interaction_cloud-1.2.2/src/social_interaction_cloud/choregraphe_to_json.py` & `social_interaction_cloud-1.2.3/src/social_interaction_cloud/choregraphe_to_json.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.2/src/social_interaction_cloud/detection_result_pb2.py` & `social_interaction_cloud-1.2.3/src/social_interaction_cloud/detection_result_pb2.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.2/src/social_interaction_cloud/tracking_result_pb2.py` & `social_interaction_cloud-1.2.3/src/social_interaction_cloud/tracking_result_pb2.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.2/LICENSE` & `social_interaction_cloud-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.2/pyproject.toml` & `social_interaction_cloud-1.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "social_interaction_cloud"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Mike Ligthart", email="m.e.u.ligthart@vu.nl" },
 ]
 description = "Connector to the Social Interaction Cloud"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `social_interaction_cloud-1.2.2/PKG-INFO` & `social_interaction_cloud-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: social_interaction_cloud
-Version: 1.2.2
+Version: 1.2.3
 Summary: Connector to the Social Interaction Cloud
 Project-URL: Source, https://bitbucket.org/socialroboticshub/connectors/src/master/python/sic/
 Project-URL: Wiki, https://socialrobotics.atlassian.net/wiki/spaces/CBSR/overview
 Author-email: Mike Ligthart <m.e.u.ligthart@vu.nl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

