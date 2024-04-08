# Comparing `tmp/sgr_demo_v0.0.4-0.0.8.tar.gz` & `tmp/sgr_demo_v0.0.4-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgr_demo_v0.0.4-0.0.8.tar", last modified: Thu Oct 12 22:03:03 2023, max compression
+gzip compressed data, was "sgr_demo_v0.0.4-0.0.9.tar", last modified: Thu Oct 12 22:06:43 2023, max compression
```

## Comparing `sgr_demo_v0.0.4-0.0.8.tar` & `sgr_demo_v0.0.4-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-10-12 22:03:03.705445 sgr_demo_v0.0.4-0.0.8/
--rw-rw-rw-   0        0        0     1553 2022-08-22 07:27:32.000000 sgr_demo_v0.0.4-0.0.8/LICENSE.md
--rw-rw-rw-   0        0        0      582 2023-10-12 22:03:03.702440 sgr_demo_v0.0.4-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2289 2022-11-16 14:17:42.000000 sgr_demo_v0.0.4-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-10-12 22:03:03.706443 sgr_demo_v0.0.4-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-10-12 22:03:01.000000 sgr_demo_v0.0.4-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-12 22:03:03.625705 sgr_demo_v0.0.4-0.0.8/sgr_demo_v0.0.4.egg-info/
--rw-rw-rw-   0        0        0      582 2023-10-12 22:03:03.000000 sgr_demo_v0.0.4-0.0.8/sgr_demo_v0.0.4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1856 2023-10-12 22:03:03.000000 sgr_demo_v0.0.4-0.0.8/sgr_demo_v0.0.4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-12 22:03:03.000000 sgr_demo_v0.0.4-0.0.8/sgr_demo_v0.0.4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-10-12 22:03:03.000000 sgr_demo_v0.0.4-0.0.8/sgr_demo_v0.0.4.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-10-12 22:03:03.000000 sgr_demo_v0.0.4-0.0.8/sgr_demo_v0.0.4.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-12 22:03:03.653828 sgr_demo_v0.0.4-0.0.8/sgr_library/
--rw-rw-rw-   0        0        0      297 2023-10-12 22:02:51.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/__init__.py
--rw-rw-rw-   0        0        0     4881 2023-10-12 21:37:27.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/auxiliary_functions.py
-drwxrwxrwx   0        0        0        0 2023-10-12 22:03:03.655835 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/
--rw-rw-rw-   0        0        0      172 2023-10-12 22:01:51.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-12 22:03:03.662034 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/communicator/
--rw-rw-rw-   0        0        0      608 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/communicator/__init__.py
--rw-rw-rw-   0        0        0     1558 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/communicator/communicator_frame.py
--rw-rw-rw-   0        0        0     7902 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/communicator/communicator_types.py
-drwxrwxrwx   0        0        0        0 2023-10-12 22:03:03.667031 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/functional_profile/
--rw-rw-rw-   0        0        0      297 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/functional_profile/__init__.py
--rw-rw-rw-   0        0        0     6730 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/functional_profile/functional_profile_frame.py
-drwxrwxrwx   0        0        0        0 2023-10-12 22:03:03.678564 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/
--rw-rw-rw-   0        0        0     2705 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/__init__.py
--rw-rw-rw-   0        0        0     4338 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/base_type_functional_profile_category.py
--rw-rw-rw-   0        0        0     7569 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/base_type_functional_profile_type.py
--rw-rw-rw-   0        0        0     1181 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/base_type_level_of_operation_type.py
--rw-rw-rw-   0        0        0    47362 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/base_types.py
--rw-rw-rw-   0        0        0     4011 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/data_point.py
--rw-rw-rw-   0        0        0     2887 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/functional_profile.py
--rw-rw-rw-   0        0        0     2040 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/sgr_serial_int_capability.py
-drwxrwxrwx   0        0        0        0 2023-10-12 22:03:03.698487 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/
--rw-rw-rw-   0        0        0     3275 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/__init__.py
--rw-rw-rw-   0        0        0     3048 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/contact_interface.py
--rw-rw-rw-   0        0        0     1892 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/generic_interface.py
--rw-rw-rw-   0        0        0     4254 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/modbus_interface.py
--rw-rw-rw-   0        0        0    27560 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/modbus_types.py
--rw-rw-rw-   0        0        0     8630 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/product.py
--rw-rw-rw-   0        0        0     2707 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/rest_api_interface.py
--rw-rw-rw-   0        0        0     7297 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/rest_api_types.py
--rw-rw-rw-   0        0        0      728 2023-10-12 14:24:45.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/exceptions.py
--rw-rw-rw-   0        0        0     3556 2023-10-12 21:31:53.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/generic_interface.py
--rw-rw-rw-   0        0        0     3218 2023-10-12 17:15:51.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/modbusRTU_client.py
--rw-rw-rw-   0        0        0     3591 2023-10-12 17:15:51.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/modbusRTU_client_async.py
--rw-rw-rw-   0        0        0     8721 2023-10-12 19:27:13.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/modbusRTU_interface.py
--rw-rw-rw-   0        0        0    10677 2023-10-12 21:29:05.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/modbusRTU_interface_async.py
--rw-rw-rw-   0        0        0     5097 2023-10-12 21:36:10.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/modbus_client.py
--rw-rw-rw-   0        0        0    12077 2023-10-12 21:37:49.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/modbus_interface.py
--rw-rw-rw-   0        0        0     4024 2022-10-04 09:21:14.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/payload_decoder.py
--rw-rw-rw-   0        0        0      499 2023-03-27 12:26:51.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/resource_errors.py
--rw-rw-rw-   0        0        0     8605 2023-10-12 19:31:24.000000 sgr_demo_v0.0.4-0.0.8/sgr_library/restapi_client_async.py
+drwxrwxrwx   0        0        0        0 2023-10-12 22:06:43.678182 sgr_demo_v0.0.4-0.0.9/
+-rw-rw-rw-   0        0        0     1553 2022-08-22 07:27:32.000000 sgr_demo_v0.0.4-0.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0      582 2023-10-12 22:06:43.677181 sgr_demo_v0.0.4-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2289 2022-11-16 14:17:42.000000 sgr_demo_v0.0.4-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-10-12 22:06:43.679182 sgr_demo_v0.0.4-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-10-12 22:06:41.000000 sgr_demo_v0.0.4-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-12 22:06:43.607500 sgr_demo_v0.0.4-0.0.9/sgr_demo_v0.0.4.egg-info/
+-rw-rw-rw-   0        0        0      582 2023-10-12 22:06:43.000000 sgr_demo_v0.0.4-0.0.9/sgr_demo_v0.0.4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1856 2023-10-12 22:06:43.000000 sgr_demo_v0.0.4-0.0.9/sgr_demo_v0.0.4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-12 22:06:43.000000 sgr_demo_v0.0.4-0.0.9/sgr_demo_v0.0.4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-10-12 22:06:43.000000 sgr_demo_v0.0.4-0.0.9/sgr_demo_v0.0.4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-10-12 22:06:43.000000 sgr_demo_v0.0.4-0.0.9/sgr_demo_v0.0.4.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-10-12 22:06:43.629344 sgr_demo_v0.0.4-0.0.9/sgr_library/
+-rw-rw-rw-   0        0        0      316 2023-10-12 22:06:06.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/__init__.py
+-rw-rw-rw-   0        0        0     4881 2023-10-12 21:37:27.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/auxiliary_functions.py
+drwxrwxrwx   0        0        0        0 2023-10-12 22:06:43.636378 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/
+-rw-rw-rw-   0        0        0      161 2023-10-12 22:05:50.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-12 22:06:43.644348 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/communicator/
+-rw-rw-rw-   0        0        0      608 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/communicator/__init__.py
+-rw-rw-rw-   0        0        0     1558 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/communicator/communicator_frame.py
+-rw-rw-rw-   0        0        0     7902 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/communicator/communicator_types.py
+drwxrwxrwx   0        0        0        0 2023-10-12 22:06:43.646831 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/functional_profile/
+-rw-rw-rw-   0        0        0      297 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/functional_profile/__init__.py
+-rw-rw-rw-   0        0        0     6730 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/functional_profile/functional_profile_frame.py
+drwxrwxrwx   0        0        0        0 2023-10-12 22:06:43.663185 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/
+-rw-rw-rw-   0        0        0     2705 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/__init__.py
+-rw-rw-rw-   0        0        0     4338 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/base_type_functional_profile_category.py
+-rw-rw-rw-   0        0        0     7569 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/base_type_functional_profile_type.py
+-rw-rw-rw-   0        0        0     1181 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/base_type_level_of_operation_type.py
+-rw-rw-rw-   0        0        0    47362 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/base_types.py
+-rw-rw-rw-   0        0        0     4011 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/data_point.py
+-rw-rw-rw-   0        0        0     2887 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/functional_profile.py
+-rw-rw-rw-   0        0        0     2040 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/sgr_serial_int_capability.py
+drwxrwxrwx   0        0        0        0 2023-10-12 22:06:43.676180 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/
+-rw-rw-rw-   0        0        0     3275 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/__init__.py
+-rw-rw-rw-   0        0        0     3048 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/contact_interface.py
+-rw-rw-rw-   0        0        0     1892 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/generic_interface.py
+-rw-rw-rw-   0        0        0     4254 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/modbus_interface.py
+-rw-rw-rw-   0        0        0    27560 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/modbus_types.py
+-rw-rw-rw-   0        0        0     8630 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/product.py
+-rw-rw-rw-   0        0        0     2707 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/rest_api_interface.py
+-rw-rw-rw-   0        0        0     7297 2023-09-26 07:27:46.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/rest_api_types.py
+-rw-rw-rw-   0        0        0      728 2023-10-12 14:24:45.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/exceptions.py
+-rw-rw-rw-   0        0        0     3556 2023-10-12 21:31:53.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/generic_interface.py
+-rw-rw-rw-   0        0        0     3218 2023-10-12 17:15:51.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/modbusRTU_client.py
+-rw-rw-rw-   0        0        0     3591 2023-10-12 17:15:51.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/modbusRTU_client_async.py
+-rw-rw-rw-   0        0        0     8721 2023-10-12 19:27:13.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/modbusRTU_interface.py
+-rw-rw-rw-   0        0        0    10677 2023-10-12 21:29:05.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/modbusRTU_interface_async.py
+-rw-rw-rw-   0        0        0     5097 2023-10-12 21:36:10.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/modbus_client.py
+-rw-rw-rw-   0        0        0    12077 2023-10-12 21:37:49.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/modbus_interface.py
+-rw-rw-rw-   0        0        0     4024 2022-10-04 09:21:14.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/payload_decoder.py
+-rw-rw-rw-   0        0        0      499 2023-03-27 12:26:51.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/resource_errors.py
+-rw-rw-rw-   0        0        0     8605 2023-10-12 19:31:24.000000 sgr_demo_v0.0.4-0.0.9/sgr_library/restapi_client_async.py
```

### Comparing `sgr_demo_v0.0.4-0.0.8/LICENSE.md` & `sgr_demo_v0.0.4-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/PKG-INFO` & `sgr_demo_v0.0.4-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgr_demo_v0.0.4
-Version: 0.0.8
+Version: 0.0.9
 Summary: SGr demo
 Home-page: UNKNOWN
 Author: zupeuc(CLEMAP)
 Author-email: <daniel@clemap.ch>
 License: UNKNOWN
 Keywords: python,SGr
 Platform: UNKNOWN
```

### Comparing `sgr_demo_v0.0.4-0.0.8/README.md` & `sgr_demo_v0.0.4-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/setup.py` & `sgr_demo_v0.0.4-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'SGr demo'
 
 # Setting up
 setup(
     name="sgr_demo_v0.0.4",
     version=VERSION,
     author="zupeuc(CLEMAP)",
```

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_demo_v0.0.4.egg-info/PKG-INFO` & `sgr_demo_v0.0.4-0.0.9/sgr_demo_v0.0.4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgr-demo-v0.0.4
-Version: 0.0.8
+Version: 0.0.9
 Summary: SGr demo
 Home-page: UNKNOWN
 Author: zupeuc(CLEMAP)
 Author-email: <daniel@clemap.ch>
 License: UNKNOWN
 Keywords: python,SGr
 Platform: UNKNOWN
```

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_demo_v0.0.4.egg-info/SOURCES.txt` & `sgr_demo_v0.0.4-0.0.9/sgr_demo_v0.0.4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/auxiliary_functions.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/communicator/__init__.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/communicator/__init__.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/communicator/communicator_frame.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/communicator/communicator_frame.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/communicator/communicator_types.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/communicator/communicator_types.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/functional_profile/functional_profile_frame.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/functional_profile/functional_profile_frame.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/__init__.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/base_type_functional_profile_category.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/base_type_functional_profile_category.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/base_type_functional_profile_type.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/base_type_functional_profile_type.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/base_type_level_of_operation_type.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/base_type_level_of_operation_type.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/base_types.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/base_types.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/data_point.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/data_point.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/functional_profile.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/functional_profile.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/generic/sgr_serial_int_capability.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/generic/sgr_serial_int_capability.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/__init__.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/__init__.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/contact_interface.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/contact_interface.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/generic_interface.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/generic_interface.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/modbus_interface.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/modbus_interface.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/modbus_types.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/modbus_types.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/product.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/product.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/rest_api_interface.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/rest_api_interface.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/data_classes/product/rest_api_types.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/data_classes/product/rest_api_types.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/exceptions.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/exceptions.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/generic_interface.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/generic_interface.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/modbusRTU_client.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/modbusRTU_client.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/modbusRTU_client_async.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/modbusRTU_client_async.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/modbusRTU_interface.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/modbusRTU_interface.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/modbusRTU_interface_async.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/modbusRTU_interface_async.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/modbus_client.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/modbus_client.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/modbus_interface.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/modbus_interface.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/payload_decoder.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/payload_decoder.py`

 * *Files identical despite different names*

### Comparing `sgr_demo_v0.0.4-0.0.8/sgr_library/restapi_client_async.py` & `sgr_demo_v0.0.4-0.0.9/sgr_library/restapi_client_async.py`

 * *Files identical despite different names*

