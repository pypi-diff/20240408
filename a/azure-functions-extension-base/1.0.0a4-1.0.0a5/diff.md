# Comparing `tmp/azure-functions-extension-base-1.0.0a4.tar.gz` & `tmp/azure-functions-extension-base-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-functions-extension-base-1.0.0a4.tar", last modified: Thu Apr  4 23:33:01 2024, max compression
+gzip compressed data, was "azure-functions-extension-base-1.0.0a5.tar", last modified: Mon Apr  8 17:04:11 2024, max compression
```

## Comparing `azure-functions-extension-base-1.0.0a4.tar` & `azure-functions-extension-base-1.0.0a5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 23:33:01.404359 azure-functions-extension-base-1.0.0a4/
--rw-rw-rw-   0        0        0     1093 2024-03-13 21:50:44.000000 azure-functions-extension-base-1.0.0a4/LICENSE
--rw-rw-rw-   0        0        0       91 2024-03-13 21:50:44.000000 azure-functions-extension-base-1.0.0a4/MANIFEST.in
--rw-rw-rw-   0        0        0     1497 2024-04-04 23:33:01.401356 azure-functions-extension-base-1.0.0a4/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-03-27 17:03:54.000000 azure-functions-extension-base-1.0.0a4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 23:33:01.353758 azure-functions-extension-base-1.0.0a4/azure/
--rw-rw-rw-   0        0        0       66 2024-03-13 21:50:44.000000 azure-functions-extension-base-1.0.0a4/azure/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 23:33:01.356785 azure-functions-extension-base-1.0.0a4/azure/functions/
--rw-rw-rw-   0        0        0       66 2024-03-27 19:23:43.000000 azure-functions-extension-base-1.0.0a4/azure/functions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 23:33:01.359765 azure-functions-extension-base-1.0.0a4/azure/functions/extension/
--rw-rw-rw-   0        0        0       66 2024-03-13 21:50:44.000000 azure-functions-extension-base-1.0.0a4/azure/functions/extension/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 23:33:01.371763 azure-functions-extension-base-1.0.0a4/azure/functions/extension/base/
--rw-rw-rw-   0        0        0      856 2024-04-04 23:32:20.000000 azure-functions-extension-base-1.0.0a4/azure/functions/extension/base/__init__.py
--rw-rw-rw-   0        0        0     5773 2024-03-28 17:45:38.000000 azure-functions-extension-base-1.0.0a4/azure/functions/extension/base/meta.py
--rw-rw-rw-   0        0        0      296 2024-03-27 17:03:54.000000 azure-functions-extension-base-1.0.0a4/azure/functions/extension/base/sdkType.py
--rw-rw-rw-   0        0        0     8534 2024-03-28 17:41:27.000000 azure-functions-extension-base-1.0.0a4/azure/functions/extension/base/utils.py
--rw-rw-rw-   0        0        0     5010 2024-04-04 23:30:31.000000 azure-functions-extension-base-1.0.0a4/azure/functions/extension/base/web.py
-drwxrwxrwx   0        0        0        0 2024-04-04 23:33:01.398344 azure-functions-extension-base-1.0.0a4/azure_functions_extension_base.egg-info/
--rw-rw-rw-   0        0        0     1497 2024-04-04 23:33:01.000000 azure-functions-extension-base-1.0.0a4/azure_functions_extension_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2024-04-04 23:33:01.000000 azure-functions-extension-base-1.0.0a4/azure_functions_extension_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 23:33:01.000000 azure-functions-extension-base-1.0.0a4/azure_functions_extension_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-04 23:33:01.000000 azure-functions-extension-base-1.0.0a4/azure_functions_extension_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-04 23:33:01.000000 azure-functions-extension-base-1.0.0a4/azure_functions_extension_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1405 2024-03-25 18:09:04.000000 azure-functions-extension-base-1.0.0a4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 23:33:01.404359 azure-functions-extension-base-1.0.0a4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-04 23:33:01.396350 azure-functions-extension-base-1.0.0a4/tests/
--rw-rw-rw-   0        0        0      519 2024-03-28 17:41:27.000000 azure-functions-extension-base-1.0.0a4/tests/__init__.py
--rw-rw-rw-   0        0        0    11520 2024-04-04 23:26:52.000000 azure-functions-extension-base-1.0.0a4/tests/test_meta.py
--rw-rw-rw-   0        0        0      656 2024-03-28 17:41:27.000000 azure-functions-extension-base-1.0.0a4/tests/test_sdk_type.py
--rw-rw-rw-   0        0        0    11042 2024-03-28 17:41:27.000000 azure-functions-extension-base-1.0.0a4/tests/test_utils.py
--rw-rw-rw-   0        0        0    14668 2024-04-04 23:30:31.000000 azure-functions-extension-base-1.0.0a4/tests/test_web.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.705120 azure-functions-extension-base-1.0.0a5/
+-rw-rw-rw-   0        0        0     1093 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a5/LICENSE
+-rw-rw-rw-   0        0        0       91 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1497 2024-04-08 17:04:11.697897 azure-functions-extension-base-1.0.0a5/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-03-27 18:57:52.000000 azure-functions-extension-base-1.0.0a5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.514428 azure-functions-extension-base-1.0.0a5/azure/
+-rw-rw-rw-   0        0        0       66 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a5/azure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.529333 azure-functions-extension-base-1.0.0a5/azure/functions/
+-rw-rw-rw-   0        0        0       66 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a5/azure/functions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.547929 azure-functions-extension-base-1.0.0a5/azure/functions/extension/
+-rw-rw-rw-   0        0        0       66 2024-02-28 16:15:11.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.588046 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/
+-rw-rw-rw-   0        0        0      856 2024-04-08 17:02:01.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/__init__.py
+-rw-rw-rw-   0        0        0     5760 2024-04-08 17:01:50.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/meta.py
+-rw-rw-rw-   0        0        0      296 2024-03-27 18:57:52.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/sdkType.py
+-rw-rw-rw-   0        0        0     9064 2024-04-08 17:01:50.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/utils.py
+-rw-rw-rw-   0        0        0     5071 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/web.py
+drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.686770 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/
+-rw-rw-rw-   0        0        0     1497 2024-04-08 17:04:11.000000 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2024-04-08 17:04:11.000000 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 17:04:11.000000 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-08 17:04:11.000000 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-08 17:04:11.000000 azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1405 2024-03-27 14:46:39.000000 azure-functions-extension-base-1.0.0a5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 17:04:11.707260 azure-functions-extension-base-1.0.0a5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 17:04:11.678633 azure-functions-extension-base-1.0.0a5/tests/
+-rw-rw-rw-   0        0        0      519 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a5/tests/__init__.py
+-rw-rw-rw-   0        0        0    11527 2024-04-08 17:01:50.000000 azure-functions-extension-base-1.0.0a5/tests/test_meta.py
+-rw-rw-rw-   0        0        0      656 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a5/tests/test_sdk_type.py
+-rw-rw-rw-   0        0        0    12756 2024-04-08 17:01:50.000000 azure-functions-extension-base-1.0.0a5/tests/test_utils.py
+-rw-rw-rw-   0        0        0    15462 2024-04-03 21:21:10.000000 azure-functions-extension-base-1.0.0a5/tests/test_web.py
```

### Comparing `azure-functions-extension-base-1.0.0a4/LICENSE` & `azure-functions-extension-base-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a4/PKG-INFO` & `azure-functions-extension-base-1.0.0a5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-functions-extension-base
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Base Python worker extension for Azure Functions.
 Author-email: "Azure Functions team at Microsoft Corp." <azurefunctions@microsoft.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `azure-functions-extension-base-1.0.0a4/azure/functions/extension/base/__init__.py` & `azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
     "HttpV2FeatureChecker",
     "ResponseLabels",
     "WebServer",
     "WebApp",
     "RequestSynchronizer",
 ]
 
-__version__ = "1.0.0a4"
+__version__ = "1.0.0a5"
```

### Comparing `azure-functions-extension-base-1.0.0a4/azure/functions/extension/base/meta.py` & `azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         return cls
 
     @classmethod
     def get(cls, binding_name):
         return cls._bindings.get(binding_name)
 
     @classmethod
-    def get_raw_bindings(cls, indexed_function, input_types) -> List[str]:
+    def get_raw_bindings(cls, indexed_function, input_types):
         return utils.get_raw_bindings(indexed_function, input_types)
 
     @classmethod
     def check_supported_type(cls, subclass: type) -> bool:
         if subclass is not None and inspect.isclass(subclass):
             return issubclass(subclass, sdkType.SdkType)
         return False
```

### Comparing `azure-functions-extension-base-1.0.0a4/azure/functions/extension/base/utils.py` & `azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -156,45 +156,52 @@
     def data_type(self) -> Optional[int]:
         return self._data_type.value if self._data_type else None
 
     @property
     def direction(self) -> int:
         return self._direction.value
 
-    def get_dict_repr(binding, input_types) -> Dict:
+    def get_dict_repr(binding, input_types):
         """Build a dictionary of a particular binding. The keys are camel
         cased binding field names defined in `init_params` list and
         :class:`Binding` class. \n
         This method is invoked in function :meth:`get_raw_bindings` of class
         :class:`Function` to generate json dict for each binding.
 
-        :return: Dictionary representation of the binding.
+        :return: Dictionary representation of the binding. Tuple representation
+        of the binding in the format:
+        ((binding type, pytype), deferred bindings enabled)
         """
         params = list(dict.fromkeys(getattr(binding, "init_params", [])))
+        binding_info = {}
         for p in params:
             if p not in Binding.EXCLUDED_INIT_PARAMS:
                 binding._dict[to_camel_case(p)] = getattr(binding, p, None)
 
+        if input_types.get(binding.name) is not None:
+            pytype = input_types.get(binding.name).pytype
+        else:
+            pytype = None
         # Adding flag to signal to the host to send MBD object
         # 1. check if the binding is a supported type (blob, blobTrigger)
         # 2. check if the binding is an input binding
         # 3. check if the defined type is an SdkType
         if (
             binding.type in meta._ConverterMeta._bindings
             and binding.direction == 0
-            and meta._ConverterMeta.check_supported_type(
-                input_types.get(binding.name).pytype
-            )
+            and meta._ConverterMeta.check_supported_type(pytype)
         ):
             binding._dict["properties"] = {"SupportsDeferredBinding": True}
+            binding_info = {binding.name: {pytype: "True"}}
         # if it isn't, we set the flag to false
         else:
             binding._dict["properties"] = {"SupportsDeferredBinding": False}
+            binding_info = {binding.name: {pytype: "False"}}
 
-        return binding._dict
+        return binding._dict, binding_info
 
 
 def to_camel_case(snake_case_str: str):
     if snake_case_str is None or len(snake_case_str) == 0:
         raise ValueError(f"Please ensure arg name {snake_case_str} is not empty!")
 
     if not is_snake_case(snake_case_str) and not is_word(snake_case_str):
@@ -234,12 +241,15 @@
     >>> is_word('foo') # returns true
     :param input_string: String to test.
     :return: True for one word string, false otherwise.
     """
     return WORD_RE.match(input_string) is not None
 
 
-def get_raw_bindings(indexed_function, input_types) -> List[str]:
-    return [
-        json.dumps(Binding.get_dict_repr(b, input_types), cls=StringifyEnumJsonEncoder)
-        for b in indexed_function._bindings
-    ]
+def get_raw_bindings(indexed_function, input_types):
+    binding_dict_repr = []
+    bindings_logs = {}
+    for b in indexed_function._bindings:
+        dict_repr, logs = Binding.get_dict_repr(b, input_types)
+        binding_dict_repr.append(json.dumps(dict_repr, cls=StringifyEnumJsonEncoder))
+        bindings_logs.update(logs)
+    return binding_dict_repr, bindings_logs
```

### Comparing `azure-functions-extension-base-1.0.0a4/azure/functions/extension/base/web.py` & `azure-functions-extension-base-1.0.0a5/azure/functions/extension/base/web.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,25 +121,29 @@
             return cls._response_types is not None and any(
                 issubclass(pytype, response_type)
                 for response_type in cls._response_types.values()
             )
         return False
 
 
-class WebApp(metaclass=ModuleTrackerMeta):
+class ABCModuleTrackerMeta(abc.ABCMeta, ModuleTrackerMeta):
+    pass
+
+
+class WebApp(metaclass=ABCModuleTrackerMeta):
     @abstractmethod
     def route(self, func: Callable):
         raise NotImplementedError()
 
     @abstractmethod
     def get_app(self):
-        raise NotImplementedError()  # pragma: no cover
+        raise NotImplementedError()
 
 
-class WebServer(metaclass=ModuleTrackerMeta):
+class WebServer(metaclass=ABCModuleTrackerMeta):
     def __init__(self, hostname, port, web_app: WebApp):
         self.hostname = hostname
         self.port = port
         self.web_app = web_app.get_app()
 
     @abstractmethod
     async def serve(self):
```

### Comparing `azure-functions-extension-base-1.0.0a4/azure_functions_extension_base.egg-info/PKG-INFO` & `azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-functions-extension-base
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Base Python worker extension for Azure Functions.
 Author-email: "Azure Functions team at Microsoft Corp." <azurefunctions@microsoft.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `azure-functions-extension-base-1.0.0a4/azure_functions_extension_base.egg-info/SOURCES.txt` & `azure-functions-extension-base-1.0.0a5/azure_functions_extension_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a4/pyproject.toml` & `azure-functions-extension-base-1.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a4/tests/__init__.py` & `azure-functions-extension-base-1.0.0a5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a4/tests/test_meta.py` & `azure-functions-extension-base-1.0.0a5/tests/test_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         self.assertIsInstance(registry, type(meta._ConverterMeta))
         self.assertIsNone(registry.get("test"))
 
         class MockIndexedFunction:
             _bindings = {}
             _trigger = None
 
-        self.assertEqual(registry.get_raw_bindings(MockIndexedFunction, []), [])
+        self.assertEqual(registry.get_raw_bindings(MockIndexedFunction, []), ([], {}))
 
         self.assertFalse(registry.check_supported_type(None))
         self.assertFalse(registry.check_supported_type("hello"))
         self.assertTrue(registry.check_supported_type(sdkType.SdkType))
 
         self.assertFalse(registry.has_trigger_support(MockIndexedFunction))
 
@@ -189,15 +189,15 @@
         with self.assertRaises(ValueError):
             meta._BaseConverter._decode_typed_data(
                 datum_attempt_coerce, python_type=dict
             )
 
         # Case 7: attempt to coerce and pass
         datum_coerce_pass = meta.Datum(value=1, type="model_binding_data")
-        self.assertEqual(
+        self.assertEquals(
             meta._BaseConverter._decode_typed_data(datum_coerce_pass, python_type=str),
             "1",
         )
 
     def test_decode_trigger_metadata_field(self):
         datum_mbd = meta.Datum(value="{}", type="model_binding_data")
         mock_trigger_metadata = {"key": datum_mbd}
```

### Comparing `azure-functions-extension-base-1.0.0a4/tests/test_sdk_type.py` & `azure-functions-extension-base-1.0.0a5/tests/test_sdk_type.py`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-base-1.0.0a4/tests/test_utils.py` & `azure-functions-extension-base-1.0.0a5/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,25 +52,29 @@
                 binding_name="blobTrigger", pytype=sdkType.SdkType
             )
         }
 
         # Create test indexed_function
         mock_indexed_functions = MockFunction(bindings=[mock_blob])
 
-        dict_repr = utils.get_raw_bindings(mock_indexed_functions, mock_input_types)
+        dict_repr, logs = utils.get_raw_bindings(
+            mock_indexed_functions, mock_input_types
+        )
         self.assertEqual(
             dict_repr,
             [
                 '{"direction": "IN", '
                 '"dataType": null, "type": "blob", '
                 '"properties": '
                 '{"SupportsDeferredBinding": true}}'
             ],
         )
 
+        self.assertEqual(logs, {"client": {sdkType.SdkType: "True"}})
+
     def test_get_dict_repr_non_sdk(self):
         # Create mock blob
         meta._ConverterMeta._bindings = {"blob"}
 
         # Create test binding
         mock_blob = utils.Binding(
             name="blob",
@@ -83,24 +87,68 @@
         mock_input_types = {
             "blob": MockParamTypeInfo(binding_name="blobTrigger", pytype=bytes)
         }
 
         # Create test indexed_function
         mock_indexed_functions = MockFunction(bindings=[mock_blob])
 
-        dict_repr = utils.get_raw_bindings(mock_indexed_functions, mock_input_types)
+        dict_repr, logs = utils.get_raw_bindings(
+            mock_indexed_functions, mock_input_types
+        )
         self.assertEqual(
             dict_repr,
             [
                 '{"direction": "IN", '
                 '"dataType": null, "type": "blob", '
                 '"properties": '
                 '{"SupportsDeferredBinding": false}}'
             ],
         )
+        self.assertEqual(logs, {"blob": {bytes: "False"}})
+
+    def test_get_dict_repr_binding_name_none(self):
+        # Create mock blob
+        meta._ConverterMeta._bindings = {"blob"}
+
+        # Create test binding
+        mock_blob = utils.Binding(
+            name="blob",
+            direction=utils.BindingDirection.IN,
+            data_type=None,
+            type="blob",
+        )
+
+        mock_http = utils.Binding(
+            name="$return",
+            direction=utils.BindingDirection.OUT,
+            data_type=None,
+            type="httpResponse",
+        )
+
+        # Create test input_types dict
+        mock_input_types = {
+            "blob": MockParamTypeInfo(binding_name="blobTrigger", pytype=bytes)
+        }
+
+        # Create test indexed_function
+        mock_indexed_functions = MockFunction(bindings=[mock_blob, mock_http])
+
+        dict_repr, logs = utils.get_raw_bindings(
+            mock_indexed_functions, mock_input_types
+        )
+        self.assertEqual(
+            dict_repr,
+            [
+                '{"direction": "IN", "dataType": null, "type": "blob", '
+                '"properties": {"SupportsDeferredBinding": false}}',
+                '{"direction": "OUT", "dataType": null, "type": "httpResponse", '
+                '"properties": {"SupportsDeferredBinding": false}}',
+            ],
+        )
+        self.assertEqual(logs, {"$return": {None: "False"}, "blob": {bytes: "False"}})
 
     def test_get_dict_repr_init_params(self):
         # Create mock blob
         meta._ConverterMeta._bindings = {"blob"}
 
         # Create test binding
         mock_blob = MockInitParams(
@@ -117,24 +165,28 @@
                 binding_name="blobTrigger", pytype=sdkType.SdkType
             )
         }
 
         # Create test indexed_function
         mock_indexed_functions = MockFunction(bindings=[mock_blob])
 
-        dict_repr = utils.get_raw_bindings(mock_indexed_functions, mock_input_types)
+        dict_repr, logs = utils.get_raw_bindings(
+            mock_indexed_functions, mock_input_types
+        )
         self.assertEqual(
             dict_repr,
             [
                 '{"direction": "IN", "dataType": null, '
                 '"type": "blob", "test": null, "properties": '
                 '{"SupportsDeferredBinding": true}}'
             ],
         )
 
+        self.assertEqual(logs, {"client": {sdkType.SdkType: "True"}})
+
     def test_binding_data_type(self):
         mock_blob = utils.Binding(
             name="blob",
             direction=utils.BindingDirection.IN,
             data_type=None,
             type="blob",
         )
```

### Comparing `azure-functions-extension-base-1.0.0a4/tests/test_web.py` & `azure-functions-extension-base-1.0.0a5/tests/test_web.py`

 * *Files 5% similar despite different names*

```diff
@@ -350,26 +350,44 @@
 
         mock_web_app = MockWebApp()
         server = MockWebServer("localhost", 8080, mock_web_app)
         self.assertEqual(server.hostname, "localhost")
         self.assertEqual(server.port, 8080)
         self.assertEqual(server.web_app, "MockApp")
 
+    async def test_serve_method_raises_not_implemented_error(self):
+        # Create a mock WebApp instance
+        class MockWebApp(WebApp):
+            def route(self, func):
+                pass
+
+            def get_app(self):
+                pass
+
+        class MockWebServer(WebServer):
+            async def serve(self):
+                super().serve()
+
+        # Create a WebServer instance with the mock WebApp
+        server = MockWebServer("localhost", 8080, MockWebApp())
+
+        # Ensure that calling the serve method raises NotImplementedError
+        with self.assertRaises(NotImplementedError):
+            await server.serve()
 
-class TestHttpV2Enabled(unittest.TestCase):
-    def test_http_v2_enabled(self):
-        ModuleTrackerMeta._module = None
-
-        class MockClass(metaclass=ModuleTrackerMeta):
-            pass
-
-        MockClass()
 
+class TestHttpV2Enabled(unittest.TestCase):
+    @patch("azure.functions.extension.base.ModuleTrackerMeta.module_imported")
+    def test_http_v2_enabled(self, mock_module_imported):
+        mock_module_imported.return_value = True
         self.assertTrue(HttpV2FeatureChecker.http_v2_enabled())
 
+        mock_module_imported.return_value = False
+        self.assertFalse(HttpV2FeatureChecker.http_v2_enabled())
+
 
 class TestResponseLabels(unittest.TestCase):
     def test_enum_values(self):
         self.assertEqual(ResponseLabels.STANDARD.value, "standard")
         self.assertEqual(ResponseLabels.STREAMING.value, "streaming")
         self.assertEqual(ResponseLabels.FILE.value, "file")
         self.assertEqual(ResponseLabels.HTML.value, "html")
```

