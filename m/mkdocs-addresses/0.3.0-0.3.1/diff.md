# Comparing `tmp/mkdocs_addresses-0.3.0.tar.gz` & `tmp/mkdocs_addresses-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_addresses-0.3.0.tar", max compression
+gzip compressed data, was "mkdocs_addresses-0.3.1.tar", max compression
```

## Comparing `mkdocs_addresses-0.3.0.tar` & `mkdocs_addresses-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0   303056 2024-04-07 13:02:30.042002 mkdocs_addresses-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     6870 2024-04-07 13:19:35.416233 mkdocs_addresses-0.3.0/README.md
--rw-r--r--   0        0        0      141 2024-04-07 13:02:30.158005 mkdocs_addresses-0.3.0/mkdocs_addresses/__init__.py
--rw-r--r--   0        0        0       22 2024-04-07 13:27:46.314691 mkdocs_addresses-0.3.0/mkdocs_addresses/__version__.py
--rw-r--r--   0        0        0    12859 2024-04-07 13:02:30.158005 mkdocs_addresses-0.3.0/mkdocs_addresses/addresses_checker.py
--rw-r--r--   0        0        0    35160 2024-04-07 13:02:30.178006 mkdocs_addresses-0.3.0/mkdocs_addresses/addresses_plugin.py
--rw-r--r--   0        0        0     1826 2024-04-07 13:02:30.242007 mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/__init__.py
--rw-r--r--   0        0        0     3851 2024-04-07 13:02:30.278009 mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/_base_handler.py
--rw-r--r--   0        0        0     1273 2024-04-07 13:02:30.278009 mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/_no_completion_handler.py
--rw-r--r--   0        0        0     4173 2024-04-07 13:02:30.290009 mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/_vsc_handlers.py
--rw-r--r--   0        0        0    24827 2024-04-07 13:02:30.290009 mkdocs_addresses-0.3.0/mkdocs_addresses/config_plugin.py
--rw-r--r--   0        0        0     4482 2023-09-21 08:35:25.358662 mkdocs_addresses-0.3.0/mkdocs_addresses/exceptions.py
--rw-r--r--   0        0        0     8074 2024-04-07 13:02:30.298009 mkdocs_addresses-0.3.0/mkdocs_addresses/logger.py
--rw-r--r--   0        0        0        0 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.0/mkdocs_addresses/other_plugins_handling/__init__.py
--rw-r--r--   0        0        0     1663 2024-04-07 13:02:30.310009 mkdocs_addresses-0.3.0/mkdocs_addresses/other_plugins_handling/autorefs.py
--rw-r--r--   0        0        0     1897 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.0/mkdocs_addresses/path_manager.py
--rw-r--r--   0        0        0     5260 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.0/mkdocs_addresses/soup_excluding_codes.py
--rw-r--r--   0        0        0      692 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/__init__.py
--rw-r--r--   0        0        0     1965 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/files_tracker.py
--rw-r--r--   0        0        0    17190 2024-04-07 13:27:46.270689 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/static_handler.py
--rw-r--r--   0        0        0     2525 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py
--rw-r--r--   0        0        0     5805 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_data_pages.py
--rw-r--r--   0        0        0     2228 2023-09-20 13:11:14.914470 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_errors_counter.py
--rw-r--r--   0        0        0     5628 2024-04-07 13:02:30.342010 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_references.py
--rw-r--r--   0        0        0      712 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/types_aliases.py
--rw-r--r--   0        0        0      492 2024-04-07 13:02:30.342010 mkdocs_addresses-0.3.0/mkdocs_addresses/toolbox.py
--rw-r--r--   0        0        0     2013 2024-04-07 13:22:55.886145 mkdocs_addresses-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8327 1970-01-01 00:00:00.000000 mkdocs_addresses-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0   303056 2024-04-07 13:02:30.042002 mkdocs_addresses-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     6870 2024-04-07 13:19:35.416233 mkdocs_addresses-0.3.1/README.md
+-rw-r--r--   0        0        0      141 2024-04-07 13:02:30.158005 mkdocs_addresses-0.3.1/mkdocs_addresses/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-08 15:15:46.388646 mkdocs_addresses-0.3.1/mkdocs_addresses/__version__.py
+-rw-r--r--   0        0        0    12859 2024-04-07 13:02:30.158005 mkdocs_addresses-0.3.1/mkdocs_addresses/addresses_checker.py
+-rw-r--r--   0        0        0    35160 2024-04-07 13:02:30.178006 mkdocs_addresses-0.3.1/mkdocs_addresses/addresses_plugin.py
+-rw-r--r--   0        0        0     1826 2024-04-07 13:02:30.242007 mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/__init__.py
+-rw-r--r--   0        0        0     3851 2024-04-07 13:02:30.278009 mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_base_handler.py
+-rw-r--r--   0        0        0     1273 2024-04-07 13:02:30.278009 mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_no_completion_handler.py
+-rw-r--r--   0        0        0     4173 2024-04-07 13:02:30.290009 mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_vsc_handlers.py
+-rw-r--r--   0        0        0    25225 2024-04-08 15:13:31.968454 mkdocs_addresses-0.3.1/mkdocs_addresses/config_plugin.py
+-rw-r--r--   0        0        0     4482 2023-09-21 08:35:25.358662 mkdocs_addresses-0.3.1/mkdocs_addresses/exceptions.py
+-rw-r--r--   0        0        0     8074 2024-04-07 13:02:30.298009 mkdocs_addresses-0.3.1/mkdocs_addresses/logger.py
+-rw-r--r--   0        0        0        0 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.1/mkdocs_addresses/other_plugins_handling/__init__.py
+-rw-r--r--   0        0        0     1663 2024-04-07 13:02:30.310009 mkdocs_addresses-0.3.1/mkdocs_addresses/other_plugins_handling/autorefs.py
+-rw-r--r--   0        0        0     1897 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.1/mkdocs_addresses/path_manager.py
+-rw-r--r--   0        0        0     5260 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.1/mkdocs_addresses/soup_excluding_codes.py
+-rw-r--r--   0        0        0      692 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/__init__.py
+-rw-r--r--   0        0        0     1965 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/files_tracker.py
+-rw-r--r--   0        0        0    17190 2024-04-08 15:15:46.344645 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/static_handler.py
+-rw-r--r--   0        0        0     2525 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py
+-rw-r--r--   0        0        0     5805 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_data_pages.py
+-rw-r--r--   0        0        0     2228 2023-09-20 13:11:14.914470 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_errors_counter.py
+-rw-r--r--   0        0        0     5628 2024-04-07 13:02:30.342010 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_references.py
+-rw-r--r--   0        0        0      712 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/types_aliases.py
+-rw-r--r--   0        0        0      492 2024-04-07 13:02:30.342010 mkdocs_addresses-0.3.1/mkdocs_addresses/toolbox.py
+-rw-r--r--   0        0        0     2013 2024-04-08 15:15:46.340645 mkdocs_addresses-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8327 1970-01-01 00:00:00.000000 mkdocs_addresses-0.3.1/PKG-INFO
```

### Comparing `mkdocs_addresses-0.3.0/LICENSE.md` & `mkdocs_addresses-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/README.md` & `mkdocs_addresses-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/addresses_checker.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/addresses_checker.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/addresses_plugin.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/addresses_plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/__init__.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/_base_handler.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_base_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/_no_completion_handler.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_no_completion_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/_vsc_handlers.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_vsc_handlers.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/config_plugin.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/config_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,30 +450,36 @@
     more_verbose = C.Type(bool, default=PluginOptions.more_verbose)
 
     plugin_off = C.Type(bool, default=PluginOptions.plugin_off)
 
     strict_anchor_check = C.Type(bool, default=PluginOptions.strict_anchor_check)
 
     # LEGACY:
-    use_vsc = C.Type(bool, default=PluginOptions.use_vsc)
+    use_vsc = C.Optional(C.Choice((True,False,None), default=PluginOptions.use_vsc))
 
     verify_only = C.ListOfItems(C.File(exists=True), default=PluginOptions.verify_only)
 
-
+#TypeError: AddressAddressesConfig.use_vsc: Setting 'required' is unsupported in class-based configs. All values are required, or can be wrapped into config_options.Optional
 
     #----------------------------------------------
+    def _validate(self):
+        return super()._validate()
+
+    def _pre_validate(self):
+        return super()._pre_validate()
 
+    def _post_validate(self):
+        return super()._post_validate()
 
 
     def validate_and_process(self, config:MkDocsConfig):
         """ Performs the basic, then extras validations on each property, and also apply the
             post conversions to the data structures that need it.
             Add on the fly the needed fields from the mkdocs config.
         """
-
         # Enforce no unexpected option name (because this is boring AF...)
         # Enforce no unexpected option name (because this is boring AF...)
         if 'plugins' in config and 'mkdocs-addresses' in config.plugins:
             settings = set(config.plugins['mkdocs-addresses'].config)
             base_settings = set(dir(config.plugins['mkdocs-addresses'].__class__.mro()[1]))
             user_settings = settings - base_settings
         else:
```

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/exceptions.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/exceptions.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/logger.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/logger.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/other_plugins_handling/autorefs.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/other_plugins_handling/autorefs.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/path_manager.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/path_manager.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/soup_excluding_codes.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/soup_excluding_codes.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/__init__.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/files_tracker.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/files_tracker.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/static_handler.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/static_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_data_pages.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_data_pages.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_errors_counter.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_errors_counter.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_references.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_references.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/types_aliases.py` & `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/types_aliases.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.0/pyproject.toml` & `mkdocs_addresses-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-addresses"
-version = "0.3.0"
+version = "0.3.1"
 description = "Mkdocs automatic paths/addresses building - auto-completion support (VSC)"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/frederic-zinelli/mkdocs-addresses"
 homepage = "http://frederic-zinelli.gitlab.io/mkdocs-addresses/"
 exclude = ["mkdocs_addresses/_test_data_extraction.py"]
 keywords = [
```

### Comparing `mkdocs_addresses-0.3.0/PKG-INFO` & `mkdocs_addresses-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-addresses
-Version: 0.3.0
+Version: 0.3.1
 Summary: Mkdocs automatic paths/addresses building - auto-completion support (VSC)
 Home-page: http://frederic-zinelli.gitlab.io/mkdocs-addresses/
 Keywords: mkdocs,mkdocs-plugin,links,autocompletion
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Plugins
```

