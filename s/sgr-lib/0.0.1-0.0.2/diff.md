# Comparing `tmp/sgr-lib-0.0.1.tar.gz` & `tmp/sgr-lib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgr-lib-0.0.1.tar", last modified: Fri Oct 13 12:39:51 2023, max compression
+gzip compressed data, was "sgr-lib-0.0.2.tar", last modified: Mon Apr  8 15:42:27 2024, max compression
```

## Comparing `sgr-lib-0.0.1.tar` & `sgr-lib-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-10-13 12:39:51.980245 sgr-lib-0.0.1/
--rw-rw-rw-   0        0        0     1553 2022-08-22 07:27:32.000000 sgr-lib-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      577 2023-10-13 12:39:51.978240 sgr-lib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2289 2022-11-16 14:17:42.000000 sgr-lib-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-10-13 12:39:51.980245 sgr-lib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-10-13 12:38:32.000000 sgr-lib-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-13 12:39:51.817369 sgr-lib-0.0.1/sgr_lib.egg-info/
--rw-rw-rw-   0        0        0      577 2023-10-13 12:39:51.000000 sgr-lib-0.0.1/sgr_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1816 2023-10-13 12:39:51.000000 sgr-lib-0.0.1/sgr_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-13 12:39:51.000000 sgr-lib-0.0.1/sgr_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-10-13 12:39:51.000000 sgr-lib-0.0.1/sgr_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-10-13 12:39:51.000000 sgr-lib-0.0.1/sgr_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-13 12:39:51.875046 sgr-lib-0.0.1/sgr_library/
--rw-rw-rw-   0        0        0      326 2023-10-12 22:36:30.000000 sgr-lib-0.0.1/sgr_library/__init__.py
--rw-rw-rw-   0        0        0     4881 2023-10-12 21:37:27.000000 sgr-lib-0.0.1/sgr_library/auxiliary_functions.py
-drwxrwxrwx   0        0        0        0 2023-10-13 12:39:51.877962 sgr-lib-0.0.1/sgr_library/data_classes/
--rw-rw-rw-   0        0        0      184 2023-10-12 22:36:34.000000 sgr-lib-0.0.1/sgr_library/data_classes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-13 12:39:51.893644 sgr-lib-0.0.1/sgr_library/data_classes/communicator/
--rw-rw-rw-   0        0        0      632 2023-10-12 22:36:46.000000 sgr-lib-0.0.1/sgr_library/data_classes/communicator/__init__.py
--rw-rw-rw-   0        0        0     1594 2023-10-12 22:37:48.000000 sgr-lib-0.0.1/sgr_library/data_classes/communicator/communicator_frame.py
--rw-rw-rw-   0        0        0     7950 2023-10-12 22:37:59.000000 sgr-lib-0.0.1/sgr_library/data_classes/communicator/communicator_types.py
-drwxrwxrwx   0        0        0        0 2023-10-13 12:39:51.899553 sgr-lib-0.0.1/sgr_library/data_classes/functional_profile/
--rw-rw-rw-   0        0        0      309 2023-10-12 22:38:06.000000 sgr-lib-0.0.1/sgr_library/data_classes/functional_profile/__init__.py
--rw-rw-rw-   0        0        0     6742 2023-10-12 22:38:14.000000 sgr-lib-0.0.1/sgr_library/data_classes/functional_profile/functional_profile_frame.py
-drwxrwxrwx   0        0        0        0 2023-10-13 12:39:51.937963 sgr-lib-0.0.1/sgr_library/data_classes/generic/
--rw-rw-rw-   0        0        0     2789 2023-10-12 22:38:32.000000 sgr-lib-0.0.1/sgr_library/data_classes/generic/__init__.py
--rw-rw-rw-   0        0        0     4338 2023-09-26 07:27:46.000000 sgr-lib-0.0.1/sgr_library/data_classes/generic/base_type_functional_profile_category.py
--rw-rw-rw-   0        0        0     7569 2023-09-26 07:27:46.000000 sgr-lib-0.0.1/sgr_library/data_classes/generic/base_type_functional_profile_type.py
--rw-rw-rw-   0        0        0     1181 2023-09-26 07:27:46.000000 sgr-lib-0.0.1/sgr_library/data_classes/generic/base_type_level_of_operation_type.py
--rw-rw-rw-   0        0        0    47398 2023-10-12 22:38:43.000000 sgr-lib-0.0.1/sgr_library/data_classes/generic/base_types.py
--rw-rw-rw-   0        0        0     4023 2023-10-12 22:38:49.000000 sgr-lib-0.0.1/sgr_library/data_classes/generic/data_point.py
--rw-rw-rw-   0        0        0     2899 2023-10-12 22:38:55.000000 sgr-lib-0.0.1/sgr_library/data_classes/generic/functional_profile.py
--rw-rw-rw-   0        0        0     2040 2023-10-12 22:43:00.000000 sgr-lib-0.0.1/sgr_library/data_classes/generic/sgr_serial_int_capability.py
-drwxrwxrwx   0        0        0        0 2023-10-13 12:39:51.974221 sgr-lib-0.0.1/sgr_library/data_classes/product/
--rw-rw-rw-   0        0        0     3359 2023-10-12 22:39:08.000000 sgr-lib-0.0.1/sgr_library/data_classes/product/__init__.py
--rw-rw-rw-   0        0        0     3072 2023-10-12 22:39:17.000000 sgr-lib-0.0.1/sgr_library/data_classes/product/contact_interface.py
--rw-rw-rw-   0        0        0     1916 2023-10-12 22:39:22.000000 sgr-lib-0.0.1/sgr_library/data_classes/product/generic_interface.py
--rw-rw-rw-   0        0        0     4290 2023-10-12 22:39:26.000000 sgr-lib-0.0.1/sgr_library/data_classes/product/modbus_interface.py
--rw-rw-rw-   0        0        0    27584 2023-10-12 22:39:35.000000 sgr-lib-0.0.1/sgr_library/data_classes/product/modbus_types.py
--rw-rw-rw-   0        0        0     8690 2023-10-12 22:39:44.000000 sgr-lib-0.0.1/sgr_library/data_classes/product/product.py
--rw-rw-rw-   0        0        0     2743 2023-10-12 22:39:49.000000 sgr-lib-0.0.1/sgr_library/data_classes/product/rest_api_interface.py
--rw-rw-rw-   0        0        0     7297 2023-09-26 07:27:46.000000 sgr-lib-0.0.1/sgr_library/data_classes/product/rest_api_types.py
--rw-rw-rw-   0        0        0      728 2023-10-12 14:24:45.000000 sgr-lib-0.0.1/sgr_library/exceptions.py
--rw-rw-rw-   0        0        0     1691 2023-10-13 12:18:38.000000 sgr-lib-0.0.1/sgr_library/generic_interface.py
--rw-rw-rw-   0        0        0     2940 2023-10-13 11:42:55.000000 sgr-lib-0.0.1/sgr_library/modbusRTU_client.py
--rw-rw-rw-   0        0        0     3007 2023-10-13 11:42:38.000000 sgr-lib-0.0.1/sgr_library/modbusRTU_client_async.py
--rw-rw-rw-   0        0        0     8719 2023-10-13 11:48:25.000000 sgr-lib-0.0.1/sgr_library/modbusRTU_interface.py
--rw-rw-rw-   0        0        0    10677 2023-10-12 21:29:05.000000 sgr-lib-0.0.1/sgr_library/modbusRTU_interface_async.py
--rw-rw-rw-   0        0        0     5148 2023-10-13 11:50:01.000000 sgr-lib-0.0.1/sgr_library/modbus_client.py
--rw-rw-rw-   0        0        0    12034 2023-10-13 12:18:59.000000 sgr-lib-0.0.1/sgr_library/modbus_interface.py
--rw-rw-rw-   0        0        0     4024 2022-10-04 09:21:14.000000 sgr-lib-0.0.1/sgr_library/payload_decoder.py
--rw-rw-rw-   0        0        0      499 2023-03-27 12:26:51.000000 sgr-lib-0.0.1/sgr_library/resource_errors.py
--rw-rw-rw-   0        0        0     9172 2023-10-13 11:48:38.000000 sgr-lib-0.0.1/sgr_library/restapi_client_async.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:42:27.679685 sgr-lib-0.0.2/
+-rw-rw-rw-   0        0        0     1553 2024-03-04 14:32:22.000000 sgr-lib-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0      153 2024-04-08 15:42:27.677688 sgr-lib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2677 2024-03-04 14:32:22.000000 sgr-lib-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 15:42:27.680688 sgr-lib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      528 2024-04-08 15:42:09.000000 sgr-lib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:42:27.533603 sgr-lib-0.0.2/sgr_lib.egg-info/
+-rw-rw-rw-   0        0        0      153 2024-04-08 15:42:27.000000 sgr-lib-0.0.2/sgr_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2180 2024-04-08 15:42:27.000000 sgr-lib-0.0.2/sgr_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 15:42:27.000000 sgr-lib-0.0.2/sgr_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-08 15:42:27.000000 sgr-lib-0.0.2/sgr_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 15:42:27.571610 sgr-lib-0.0.2/sgr_library/
+-rw-rw-rw-   0        0        0      393 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:42:27.588134 sgr-lib-0.0.2/sgr_library/api/
+-rw-rw-rw-   0        0        0      625 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/api/__init__.py
+-rw-rw-rw-   0        0        0      764 2024-03-13 15:32:36.000000 sgr-lib-0.0.2/sgr_library/api/configuration_parameter.py
+-rw-rw-rw-   0        0        0     2616 2024-04-03 14:34:57.000000 sgr-lib-0.0.2/sgr_library/api/data_point_api.py
+-rw-rw-rw-   0        0        0      215 2024-03-04 14:32:22.000000 sgr-lib-0.0.2/sgr_library/api/data_types.py
+-rw-rw-rw-   0        0        0     2091 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/api/device_api.py
+-rw-rw-rw-   0        0        0      918 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/api/function_profile_api.py
+-rw-rw-rw-   0        0        0      571 2024-03-04 14:32:22.000000 sgr-lib-0.0.2/sgr_library/api/sub_set_units.py
+-rw-rw-rw-   0        0        0     4745 2024-04-03 14:34:57.000000 sgr-lib-0.0.2/sgr_library/auxiliary_functions.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:42:27.595137 sgr-lib-0.0.2/sgr_library/converters/
+-rw-rw-rw-   0        0        0      102 2024-03-04 14:32:22.000000 sgr-lib-0.0.2/sgr_library/converters/__init__.py
+-rw-rw-rw-   0        0        0     4516 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/converters/converter.py
+-rw-rw-rw-   0        0        0     1639 2024-04-03 14:34:57.000000 sgr-lib-0.0.2/sgr_library/converters/resolver.py
+-rw-rw-rw-   0        0        0      728 2023-10-12 14:24:45.000000 sgr-lib-0.0.2/sgr_library/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:42:27.598133 sgr-lib-0.0.2/sgr_library/generated/
+-rw-rw-rw-   0        0        0      224 2024-03-22 22:42:14.000000 sgr-lib-0.0.2/sgr_library/generated/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:42:27.607133 sgr-lib-0.0.2/sgr_library/generated/communicator/
+-rw-rw-rw-   0        0        0      626 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/communicator/__init__.py
+-rw-rw-rw-   0        0        0     1991 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/communicator/communicator_frame.py
+-rw-rw-rw-   0        0        0     7989 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/communicator/communicator_types.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:42:27.612133 sgr-lib-0.0.2/sgr_library/generated/functional_profile/
+-rw-rw-rw-   0        0        0      306 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/functional_profile/__init__.py
+-rw-rw-rw-   0        0        0     7144 2024-03-13 15:32:36.000000 sgr-lib-0.0.2/sgr_library/generated/functional_profile/functional_profile_frame.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:42:27.643134 sgr-lib-0.0.2/sgr_library/generated/generic/
+-rw-rw-rw-   0        0        0     3337 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/generic/__init__.py
+-rw-rw-rw-   0        0        0     4320 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/generic/base_type_functional_profile_category.py
+-rw-rw-rw-   0        0        0     1181 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/generic/base_type_level_of_operation_type.py
+-rw-rw-rw-   0        0        0    36145 2024-03-13 15:32:36.000000 sgr-lib-0.0.2/sgr_library/generated/generic/base_types.py
+-rw-rw-rw-   0        0        0     4792 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/generic/data_point.py
+-rw-rw-rw-   0        0        0     2923 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/generic/functional_profile.py
+-rw-rw-rw-   0        0        0     2474 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/generic/generic_attribute.py
+-rw-rw-rw-   0        0        0     2040 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/generic/sgr_serial_int_capability.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:42:27.666139 sgr-lib-0.0.2/sgr_library/generated/product/
+-rw-rw-rw-   0        0        0     3508 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/product/__init__.py
+-rw-rw-rw-   0        0        0     3066 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/product/contact_interface.py
+-rw-rw-rw-   0        0        0     1910 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/product/generic_interface.py
+-rw-rw-rw-   0        0        0     4250 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/product/modbus_interface.py
+-rw-rw-rw-   0        0        0    24266 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/product/modbus_types.py
+-rw-rw-rw-   0        0        0    10835 2024-03-13 15:32:36.000000 sgr-lib-0.0.2/sgr_library/generated/product/product.py
+-rw-rw-rw-   0        0        0     2703 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/product/rest_api_interface.py
+-rw-rw-rw-   0        0        0     8688 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generated/product/rest_api_types.py
+-rw-rw-rw-   0        0        0     4703 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/generic_interface.py
+-rw-rw-rw-   0        0        0     2940 2023-10-13 11:42:55.000000 sgr-lib-0.0.2/sgr_library/modbusRTU_client.py
+-rw-rw-rw-   0        0        0     3538 2024-04-04 17:46:28.000000 sgr-lib-0.0.2/sgr_library/modbusRTU_client_async.py
+-rw-rw-rw-   0        0        0     8977 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/modbusRTU_interface.py
+-rw-rw-rw-   0        0        0    13991 2024-04-03 14:34:57.000000 sgr-lib-0.0.2/sgr_library/modbusRTU_interface_async.py
+-rw-rw-rw-   0        0        0     5148 2024-02-12 17:18:17.000000 sgr-lib-0.0.2/sgr_library/modbus_client.py
+-rw-rw-rw-   0        0        0    15489 2024-03-13 15:32:36.000000 sgr-lib-0.0.2/sgr_library/modbus_interface.py
+-rw-rw-rw-   0        0        0     4046 2024-04-03 14:34:57.000000 sgr-lib-0.0.2/sgr_library/payload_decoder.py
+-rw-rw-rw-   0        0        0      499 2023-03-27 12:26:51.000000 sgr-lib-0.0.2/sgr_library/resource_errors.py
+-rw-rw-rw-   0        0        0    11015 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/restapi_client_async.py
+-rw-rw-rw-   0        0        0     1796 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/sgr_device.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:42:27.674686 sgr-lib-0.0.2/sgr_library/validators/
+-rw-rw-rw-   0        0        0      105 2024-03-04 14:32:22.000000 sgr-lib-0.0.2/sgr_library/validators/__init__.py
+-rw-rw-rw-   0        0        0     1338 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/validators/resolver.py
+-rw-rw-rw-   0        0        0     2432 2024-03-12 08:07:54.000000 sgr-lib-0.0.2/sgr_library/validators/validator.py
```

### Comparing `sgr-lib-0.0.1/LICENSE.md` & `sgr-lib-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sgr-lib-0.0.1/README.md` & `sgr-lib-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 # INDEX
 
 1) How to use
-2) Pip installation for developers
+2) Pip installation
 3) Directory structure
 
 ## 1) How to use
 
 - getval(<fp_name>, <dp_name>) from **generic_interface.py** module (Implemented in restapi and modbus)
 - setval(<fp_name>, <dp_name>, <value>) from **generic_interface.py** module (Only implemented for modbus)
 	
 generic_interface.py has a script with an example on how to use these functions.
 
 - For the xsdata documentation and the library documentation please go to sgr_library folder in this directory. There you will find the specific the documentation.
 - For EXAMPLES on how to use the library, you will also find them in the sgr_library file, as 'examples'.
 
-## 2) Pip Instalation
+## 2.1) Pip Installation
+
+Install our libray by running the command:
+
+		pip install sgr-lib
+
+Then import the library as follows (Please watch "example_generic.py" in our examples file for more clarity):
+
+		from sgr_library.generic_interface import GenericInterface
+
+## 2.2) DEVELOPER Pip Installation
 
 ### Pip Install from local repository (developer).
 0) Create virtual enviroment:
 
 		py -m venv venv
 		venv\Scripts\activate
     
@@ -29,30 +39,31 @@
     	pip install -e C:\path\to\file\
 	
 	EXAMPLE: pip install -e C:\Users\admin\Desktop\SGrPython   
 
 
 ### DEPRECATED Pip Install from pypi testing server (user).
 
-I uploaded the library as "sgr-demo-v0.0.4" for now.
+Uploaded the library as "sgr-demo-v0.0.4" for now.
 You can download it with the following command.
 
     pip install --index-url https://test.pypi.org/simple/ sgr-demo-v0.0.4
     
     
 ## 3) Directory
 
-- sgr_library: Is the folder which will be installed with the pip install command. In there 
+- sgr_library: Is the folder which will be installed with the pip install command.
+
+- examples: This folder contains files on how to use the library. Please go to "example_generic.py" to have a basic example.
 
 - xml_files: Contains sample xml files for users to modify or use as example.
 
 - xsd_files: Contains the SGr xsd files structure, from which the dataclasses in "sgr_library" directory were generated. 
 You don't have to do this, since the classes come included in the pip install, but in case you want to change something, you can generate classes with the following command:
 
 		xsdata --package data_classes xsd_files/SGrIncluder.xsd
 	
 - setup.py: The script that is executed when installing the library with pip.
-
 	
 - requirements.txt: required libraries are included in the setup of the file, but in case these fail, install from requierements.txt file.
 	
 		pip install -r requirements.txt
```

### Comparing `sgr-lib-0.0.1/sgr_lib.egg-info/SOURCES.txt` & `sgr-lib-0.0.2/sgr_lib.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 LICENSE.md
 README.md
 setup.py
 sgr_lib.egg-info/PKG-INFO
 sgr_lib.egg-info/SOURCES.txt
 sgr_lib.egg-info/dependency_links.txt
-sgr_lib.egg-info/requires.txt
 sgr_lib.egg-info/top_level.txt
 sgr_library/__init__.py
 sgr_library/auxiliary_functions.py
 sgr_library/exceptions.py
 sgr_library/generic_interface.py
 sgr_library/modbusRTU_client.py
 sgr_library/modbusRTU_client_async.py
 sgr_library/modbusRTU_interface.py
 sgr_library/modbusRTU_interface_async.py
 sgr_library/modbus_client.py
 sgr_library/modbus_interface.py
 sgr_library/payload_decoder.py
 sgr_library/resource_errors.py
 sgr_library/restapi_client_async.py
-sgr_library/data_classes/__init__.py
-sgr_library/data_classes/communicator/__init__.py
-sgr_library/data_classes/communicator/communicator_frame.py
-sgr_library/data_classes/communicator/communicator_types.py
-sgr_library/data_classes/functional_profile/__init__.py
-sgr_library/data_classes/functional_profile/functional_profile_frame.py
-sgr_library/data_classes/generic/__init__.py
-sgr_library/data_classes/generic/base_type_functional_profile_category.py
-sgr_library/data_classes/generic/base_type_functional_profile_type.py
-sgr_library/data_classes/generic/base_type_level_of_operation_type.py
-sgr_library/data_classes/generic/base_types.py
-sgr_library/data_classes/generic/data_point.py
-sgr_library/data_classes/generic/functional_profile.py
-sgr_library/data_classes/generic/sgr_serial_int_capability.py
-sgr_library/data_classes/product/__init__.py
-sgr_library/data_classes/product/contact_interface.py
-sgr_library/data_classes/product/generic_interface.py
-sgr_library/data_classes/product/modbus_interface.py
-sgr_library/data_classes/product/modbus_types.py
-sgr_library/data_classes/product/product.py
-sgr_library/data_classes/product/rest_api_interface.py
-sgr_library/data_classes/product/rest_api_types.py
+sgr_library/sgr_device.py
+sgr_library/api/__init__.py
+sgr_library/api/configuration_parameter.py
+sgr_library/api/data_point_api.py
+sgr_library/api/data_types.py
+sgr_library/api/device_api.py
+sgr_library/api/function_profile_api.py
+sgr_library/api/sub_set_units.py
+sgr_library/converters/__init__.py
+sgr_library/converters/converter.py
+sgr_library/converters/resolver.py
+sgr_library/generated/__init__.py
+sgr_library/generated/communicator/__init__.py
+sgr_library/generated/communicator/communicator_frame.py
+sgr_library/generated/communicator/communicator_types.py
+sgr_library/generated/functional_profile/__init__.py
+sgr_library/generated/functional_profile/functional_profile_frame.py
+sgr_library/generated/generic/__init__.py
+sgr_library/generated/generic/base_type_functional_profile_category.py
+sgr_library/generated/generic/base_type_level_of_operation_type.py
+sgr_library/generated/generic/base_types.py
+sgr_library/generated/generic/data_point.py
+sgr_library/generated/generic/functional_profile.py
+sgr_library/generated/generic/generic_attribute.py
+sgr_library/generated/generic/sgr_serial_int_capability.py
+sgr_library/generated/product/__init__.py
+sgr_library/generated/product/contact_interface.py
+sgr_library/generated/product/generic_interface.py
+sgr_library/generated/product/modbus_interface.py
+sgr_library/generated/product/modbus_types.py
+sgr_library/generated/product/product.py
+sgr_library/generated/product/rest_api_interface.py
+sgr_library/generated/product/rest_api_types.py
+sgr_library/validators/__init__.py
+sgr_library/validators/resolver.py
+sgr_library/validators/validator.py
```

### Comparing `sgr-lib-0.0.1/sgr_library/auxiliary_functions.py` & `sgr-lib-0.0.2/sgr_library/auxiliary_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from pymodbus.constants import Endian
-
-from sgr_library.data_classes.product import DeviceFrame
-
-from sgr_library.exceptions import DataPointException, FunctionalProfileException, InvalidEndianType
-
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.parsers import XmlParser
 
+from sgr_library.generated.product import DeviceFrame, BitOrder, ModbusDataPoint
+from sgr_library.exceptions import DataPointException, FunctionalProfileException
+
 
 # TODO error handling
-def get_protocol(xml_file:str) -> str:
+def get_protocol(xml_file: str) -> str:
     """
     Searches for protocol type in xml file
     :return: protocol type string
     """
     parser = XmlParser(context=XmlContext())
     root = parser.parse(xml_file, DeviceFrame)
 
@@ -28,88 +26,94 @@
     elif generic:
         return "generic"
     elif contact:
         return "contact"
     else:
         return "error"
 
+
 # TODO make this one so that it is generic.
-def find_dp(root, fp_name: str, dp_name: str):
+def find_dp(root, fp_name: str, dp_name: str) -> ModbusDataPoint:
     """
     Searches the datapoint in the root element.
     :param root: The root element created with the xsdata parser
     :param fp_name: The name of the funcitonal profile in which the datapoint resides
     :param dp_name: The name of the datapoint
     :returns: The datapoint element found in root, if not, returns None.
     """
+    for fp in root.interface_list.modbus_interface.functional_profile_list.functional_profile_list_element:
+        for dp in fp.data_point_list.data_point_list_element:
+            if fp.functional_profile.functional_profile_name == fp_name and dp.data_point.data_point_name:
+                return dp
+    raise DataPointException(f"Datapoint {dp_name} not found in functional profile {fp_name}.")
+    # raise FunctionalProfileException(f"Functional profile {fp_name} not found in XML file.")
 
-    fp = next(filter(lambda x: x.functional_profile.functional_profile_name == fp_name, root.interface_list.modbus_interface.functional_profile_list.functional_profile_list_element), None)
-    if fp:
-        dp = next(filter(lambda x: x.data_point.data_point_name == dp_name, fp.data_point_list.data_point_list_element), None)
-        if dp:
-            print(dp)
-        raise DataPointException(f"Datapoint {dp_name} not found in functional profile {fp_name}.")
-    raise FunctionalProfileException(f"Functional profile {fp_name} not found in XML file.")
 
 def get_modbusInterfaceSelection(xml_file: str) -> str:
     try:
         parser = XmlParser(context=XmlContext())
         root = parser.parse(xml_file, DeviceFrame)
         interface_selection = root.interface_list.modbus_interface.modbus_interface_description.modbus_interface_selection.value
         if interface_selection not in ['RTU', 'TCPIP', 'UDPIP', 'RTU-ASCII', 'TCPIP-ASCII', 'UDPIP-ASCII']:
             raise ValueError('Invalid Modbus interface selection found.')
         return interface_selection
     except Exception as e:
         raise ValueError(f"Error parsing XML file or extracting Modbus interface selection: {e}")
 
+
 def get_address(root) -> str:
     try:
         return str(root.interface_list.modbus_interface.modbus_interface_description.modbus_tcp.address)
     except AttributeError:
         raise ValueError("IP address not found in XML file.")
 
+
 def get_port(root) -> int:
     try:
         return int(root.interface_list.modbus_interface.modbus_interface_description.modbus_tcp.port)
     except (AttributeError, ValueError):
         raise ValueError("Port not found or invalid in XML file.")
 
+
 def get_slave(root) -> int:
     try:
         return int(root.interface_list.modbus_interface.modbus_interface_description.modbus_tcp.slave_id)
     except (AttributeError, ValueError):
         raise ValueError("Slave ID not found or invalid in XML file.")
 
+
 def get_slave_rtu(root) -> int:
     try:
         return int(root.interface_list.modbus_interface.modbus_interface_description.modbus_rtu.slave_addr)
     except (AttributeError, ValueError):
         raise ValueError("RTU Slave ID not found or invalid in XML file.")
 
+
 def get_endian(root) -> str:
     try:
-        endian_str = str(root.interface_list.modbus_interface.modbus_interface_description.bit_order.value)
-        if endian_str == "BigEndian":
-            return Endian.Big
-        elif endian_str == "LittleEndian":
-            return Endian.Little
-        else:
-            raise InvalidEndianType(f'received invalid endian type: "{endian_str}"')
+        match root.interface_list.modbus_interface.modbus_interface_description.bit_order:
+            case BitOrder.BIG_ENDIAN:
+                return Endian.BIG
+            case _:
+                return Endian.LITTLE
     except AttributeError:
         raise ValueError("Endian type not found in XML file.")
 
+
 def get_baudrate(root) -> int:
     try:
-        return int(root.interface_list.modbus_interface.modbus_interface_description.modbus_rtu.baud_rate_selected.value)
+        return int(
+            root.interface_list.modbus_interface.modbus_interface_description.modbus_rtu.baud_rate_selected.value)
     except (AttributeError, ValueError):
         raise ValueError("Baudrate not found or invalid in XML file.")
 
+
 def get_parity(root) -> str:
     try:
-        parity_string = str(root.interface_list.modbus_interface.modbus_interface_description.modbus_rtu.parity_selected.value)
+        parity_string = str(
+            root.interface_list.modbus_interface.modbus_interface_description.modbus_rtu.parity_selected.value)
         if parity_string == "EVEN":
             return "E"
         else:
             raise NotImplementedError(f'Parity type "{parity_string}" not supported.')
     except AttributeError:
         raise ValueError("Parity type not found in XML file.")
-
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/communicator/__init__.py` & `sgr-lib-0.0.2/sgr_library/generated/communicator/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from sgr_library.data_classes.communicator.communicator_frame import (
+from sgr_library.generated.communicator.communicator_frame import (
     CommunicatorFrame1,
     CommunicatorFunctionalProfile,
     CommunicatorFrame,
 )
-from sgr_library.data_classes.communicator.communicator_types import (
+from sgr_library.generated.communicator.communicator_types import (
     CommunicatorBase,
     CommunicatorCategory,
     CommunicatorInformation,
     CommunicatorTransportService,
     TransportServices,
 )
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/communicator/communicator_frame.py` & `sgr-lib-0.0.2/sgr_library/generated/product/generic_interface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,67 @@
 from dataclasses import dataclass, field
-from typing import List
-from sgr_library.data_classes.communicator.communicator_types import CommunicatorBase
-from sgr_library.data_classes.generic.data_point import DataPointBase
-from sgr_library.data_classes.generic.functional_profile import FunctionalProfileBase
+from typing import List, Optional
+from sgr_library.generated.generic.data_point import DataPointBase
+from sgr_library.generated.generic.functional_profile import FunctionalProfileBase
 
 __NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
 
 
 @dataclass
-class CommunicatorFunctionalProfile(FunctionalProfileBase):
+class GenericDataPointList:
     """
-    Extends the base functional profile type with generic data points.
+    List of data points.
     """
     data_point_list_element: List[DataPointBase] = field(
         default_factory=list,
         metadata={
             "name": "dataPointListElement",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "min_occurs": 1,
         }
     )
 
 
 @dataclass
-class CommunicatorFrame1(CommunicatorBase):
+class GenericFunctionalProfile(FunctionalProfileBase):
+    data_point_list: Optional[GenericDataPointList] = field(
+        default=None,
+        metadata={
+            "name": "dataPointList",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+
+
+@dataclass
+class GenericFunctionalProfileList:
     """
-    Data type definition for a Communicator Description.
+    List of functional profiles.
     """
-    class Meta:
-        name = "CommunicatorFrame"
-
-    functional_profile_list_element: List[CommunicatorFunctionalProfile] = field(
+    functional_profile_list_element: List[GenericFunctionalProfile] = field(
         default_factory=list,
         metadata={
             "name": "functionalProfileListElement",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "min_occurs": 1,
         }
     )
 
 
 @dataclass
-class CommunicatorFrame(CommunicatorFrame1):
+class GenericInterface:
     """
-    RPT Root Point for Communicator.
+    Container for a device without supported transport service.
     """
-    class Meta:
-        name = "communicatorFrame"
-        namespace = "http://www.smartgridready.com/ns/V0/"
+    functional_profile_list: Optional[GenericFunctionalProfileList] = field(
+        default=None,
+        metadata={
+            "name": "functionalProfileList",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/communicator/communicator_types.py` & `sgr-lib-0.0.2/sgr_library/generated/communicator/communicator_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import List, Optional
-from sgr_library.data_classes.generic.base_type_level_of_operation_type import LevelOfOperation
-from sgr_library.data_classes.generic.base_types import (
+from sgr_library.generated.generic.base_type_level_of_operation_type import LevelOfOperation
+from sgr_library.generated.generic.base_types import (
     AlternativeNames,
-    GenericAttributes,
+    GenericAttributeListFunctionalProfile,
     LegibleDescription,
     ReleaseNotes,
 )
-from sgr_library.data_classes.product.modbus_types import ModbusInterfaceSelection
-from sgr_library.data_classes.product.rest_api_types import RestApiInterfaceSelection
+from sgr_library.generated.product.modbus_types import ModbusInterfaceSelection
+from sgr_library.generated.product.rest_api_types import RestApiInterfaceSelection
 
 __NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
 
 
 class CommunicatorCategory(Enum):
     """
     Communicator types, a growing list of supported Communicators.
@@ -183,15 +183,15 @@
         manufacturer
     :ivar manufacturer_name: Name of the Manufacturer or OEM
     :ivar release_notes:
     :ivar specification_owner_identification: the identifier as
         enumeration indicates that the manufacturer is related with the
         organisation and that this declaration is generated by himself
     :ivar communicator_information:
-    :ivar generic_attributes:
+    :ivar generic_attribute_list:
     """
     communicator_name: Optional[str] = field(
         default=None,
         metadata={
             "name": "communicatorName",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
@@ -230,15 +230,15 @@
         metadata={
             "name": "communicatorInformation",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
-    generic_attributes: Optional[GenericAttributes] = field(
+    generic_attribute_list: Optional[GenericAttributeListFunctionalProfile] = field(
         default=None,
         metadata={
-            "name": "genericAttributes",
+            "name": "genericAttributeList",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/functional_profile/functional_profile_frame.py` & `sgr-lib-0.0.2/sgr_library/generated/functional_profile/functional_profile_frame.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from dataclasses import dataclass, field
 from typing import List, Optional
-from sgr_library.data_classes.generic.base_types import (
+from sgr_library.generated.generic.base_types import (
     AlternativeNames,
-    DataDirection,
+    DataDirectionFunctionalProfile,
     DataTypeFunctionalProfile,
     FunctionalProfileIdentification,
-    GenericAttributes,
+    GenericAttributeListFunctionalProfile,
     LegibleDescription,
     PresenceLevel,
     ReleaseNotes,
+    RequestParam,
     Units,
 )
 
 __NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
 
 
 @dataclass
@@ -25,18 +26,18 @@
         metadata={
             "name": "dataPoint",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
-    generic_attributes: Optional[GenericAttributes] = field(
+    generic_attribute_list: Optional[GenericAttributeListFunctionalProfile] = field(
         default=None,
         metadata={
-            "name": "genericAttributes",
+            "name": "genericAttributeList",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
 
     @dataclass
     class DataPoint:
@@ -46,14 +47,15 @@
         :ivar data_point_name: Bezeichnung des Datenpunktes:
             «Schlagwort», welches die Bedeutung identifiziert. Diese
             Bezeichnung gilt neben der Indexnummer als Definition für
             den SmartGridready Namespace für die maschinenlesbaren
             Daten.
         :ivar data_direction:
         :ivar presence_level:
+        :ivar request_params:
         :ivar data_type:
         :ivar unit:
         :ivar array_length:
         :ivar alternative_names:
         :ivar legible_description: Published and printable information
             related to this datapoint
         """
@@ -62,15 +64,15 @@
             metadata={
                 "name": "dataPointName",
                 "type": "Element",
                 "namespace": "http://www.smartgridready.com/ns/V0/",
                 "required": True,
             }
         )
-        data_direction: Optional[DataDirection] = field(
+        data_direction: Optional[DataDirectionFunctionalProfile] = field(
             default=None,
             metadata={
                 "name": "dataDirection",
                 "type": "Element",
                 "namespace": "http://www.smartgridready.com/ns/V0/",
                 "required": True,
             }
@@ -80,14 +82,22 @@
             metadata={
                 "name": "presenceLevel",
                 "type": "Element",
                 "namespace": "http://www.smartgridready.com/ns/V0/",
                 "required": True,
             }
         )
+        request_params: Optional[RequestParam] = field(
+            default=None,
+            metadata={
+                "name": "requestParams",
+                "type": "Element",
+                "namespace": "http://www.smartgridready.com/ns/V0/",
+            }
+        )
         data_type: Optional[DataTypeFunctionalProfile] = field(
             default=None,
             metadata={
                 "name": "dataType",
                 "type": "Element",
                 "namespace": "http://www.smartgridready.com/ns/V0/",
                 "required": True,
@@ -163,27 +173,26 @@
         default=None,
         metadata={
             "name": "functionalProfile",
             "type": "Element",
             "required": True,
         }
     )
-    generic_attributes: List[GenericAttributes] = field(
-        default_factory=list,
+    generic_attribute_list: Optional[GenericAttributeListFunctionalProfile] = field(
+        default=None,
         metadata={
-            "name": "genericAttributes",
+            "name": "genericAttributeList",
             "type": "Element",
         }
     )
     data_point_list: Optional[FunctionalProfileDataPointList] = field(
         default=None,
         metadata={
             "name": "dataPointList",
             "type": "Element",
-            "required": True,
         }
     )
 
     @dataclass
     class FunctionalProfile:
         """
         Functional profile element.
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/generic/__init__.py` & `sgr-lib-0.0.2/sgr_library/generated/generic/functional_profile.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,93 @@
-from sgr_library.data_classes.generic.base_type_functional_profile_category import FunctionalProfileCategory
-from sgr_library.data_classes.generic.base_type_functional_profile_type import FunctionalProfileType
-from sgr_library.data_classes.generic.base_type_level_of_operation_type import LevelOfOperation
-from sgr_library.data_classes.generic.base_types import (
+from dataclasses import dataclass, field
+from typing import List, Optional
+from sgr_library.generated.generic.base_types import (
     AlternativeNames,
-    BitmapEntryFunctionalProfile,
-    BitmapEntryProduct,
-    BitmapFunctionalProfile,
-    BitmapProduct,
-    ChangeLog,
-    DataDirection,
-    DataTypeFunctionalProfile,
-    DataTypeProduct,
-    DeviceCategory,
-    EmptyType,
-    EnumType,
-    EnumEntry,
-    EnumMapFunctionalProfile,
-    EnumMapProduct,
-    FlexAssistance,
     FunctionalProfileIdentification,
-    GenericAttributes,
-    Language,
+    GenericAttributeListProduct,
     LegibleDescription,
-    MeasuredValueSource,
-    MeasuredValueType,
-    ObligLvlType,
-    PowerSource,
-    PresenceLevel,
-    ReleaseNotes,
-    ReleaseState,
-    SgcpserviceType,
-    ScalingFactor,
-    SmoothTransition,
-    StabilityFallback,
-    Units,
-    VersionNumber,
-    EnumEntryProductRecord,
-    EnumEntryRecordFunctionalProfile,
-)
-from sgr_library.data_classes.generic.data_point import (
-    DataPointBase,
-    DataPointDescription,
-)
-from sgr_library.data_classes.generic.functional_profile import (
-    FunctionalProfileBase,
-    FunctionalProfileDescription,
-)
-from sgr_library.data_classes.generic.sgr_serial_int_capability import (
-    BaudRate,
-    ByteLength,
-    Parity,
-    SerialInterfaceCapability,
-    StopBitLength,
 )
 
-__all__ = [
-    "FunctionalProfileCategory",
-    "FunctionalProfileType",
-    "LevelOfOperation",
-    "AlternativeNames",
-    "BitmapEntryFunctionalProfile",
-    "BitmapEntryProduct",
-    "BitmapFunctionalProfile",
-    "BitmapProduct",
-    "ChangeLog",
-    "DataDirection",
-    "DataTypeFunctionalProfile",
-    "DataTypeProduct",
-    "DeviceCategory",
-    "EmptyType",
-    "EnumType",
-    "EnumEntry",
-    "EnumMapFunctionalProfile",
-    "EnumMapProduct",
-    "FlexAssistance",
-    "FunctionalProfileIdentification",
-    "GenericAttributes",
-    "Language",
-    "LegibleDescription",
-    "MeasuredValueSource",
-    "MeasuredValueType",
-    "ObligLvlType",
-    "PowerSource",
-    "PresenceLevel",
-    "ReleaseNotes",
-    "ReleaseState",
-    "SgcpserviceType",
-    "ScalingFactor",
-    "SmoothTransition",
-    "StabilityFallback",
-    "Units",
-    "VersionNumber",
-    "EnumEntryProductRecord",
-    "EnumEntryRecordFunctionalProfile",
-    "DataPointBase",
-    "DataPointDescription",
-    "FunctionalProfileBase",
-    "FunctionalProfileDescription",
-    "BaudRate",
-    "ByteLength",
-    "Parity",
-    "SerialInterfaceCapability",
-    "StopBitLength",
-]
+__NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
+
+
+@dataclass
+class FunctionalProfileDescription:
+    """
+    Functional profile properties.
+
+    :ivar functional_profile_name:
+    :ivar functional_profile_identification:
+    :ivar alternative_names:
+    :ivar legible_description: Published and printable information
+        related to this functional profile
+    :ivar programmer_hints: additional device-specific implementation
+        hints for this functional profile
+    """
+    functional_profile_name: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "functionalProfileName",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+    functional_profile_identification: Optional[FunctionalProfileIdentification] = field(
+        default=None,
+        metadata={
+            "name": "functionalProfileIdentification",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+    alternative_names: Optional[AlternativeNames] = field(
+        default=None,
+        metadata={
+            "name": "alternativeNames",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+    legible_description: List[LegibleDescription] = field(
+        default_factory=list,
+        metadata={
+            "name": "legibleDescription",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "max_occurs": 4,
+        }
+    )
+    programmer_hints: List[LegibleDescription] = field(
+        default_factory=list,
+        metadata={
+            "name": "programmerHints",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "max_occurs": 4,
+        }
+    )
+
+
+@dataclass
+class FunctionalProfileBase:
+    """
+    Functional profile element.
+    """
+    functional_profile: Optional[FunctionalProfileDescription] = field(
+        default=None,
+        metadata={
+            "name": "functionalProfile",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+    generic_attribute_list: Optional[GenericAttributeListProduct] = field(
+        default=None,
+        metadata={
+            "name": "genericAttributeList",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/generic/base_type_functional_profile_category.py` & `sgr-lib-0.0.2/sgr_library/generated/generic/base_type_functional_profile_category.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     :cvar DHWCIRCUIT: 4: WarmWasserHeizung
     :cvar DHWSTORAGE: 5: WarmWasserSpeicher
     :cvar DISHWASHER: 6: Geschirrspülmaschine
     :cvar DRYER: 7: Trockner
     :cvar ELECTRICAL_IMMERSION_HEATER: 8: elTauchSieder
     :cvar FAN: 9: Ventilator
     :cvar GAS_HEATING_APPLIANCE: 10: GasWärmeAnwendung
-    :cvar NON_SPECIFIC: 11: allgemein verwendbar
+    :cvar METERING: 11: allgemein verwendbar
     :cvar HEATING_BUFFER_STORAGE: 12: WaermeBufferSpeicher
     :cvar HEATING_CIRCUIT: 13: Heizkreis
     :cvar HEATING_OBJECT: 14: Heizungsobjekt
     :cvar HEATING_ZONE: 15: Heizzone
     :cvar HEAT_PUMP_CONTROL: 16: WärmePumpenAnwendung
     :cvar HEAT_SINK_CIRCUIT: 17: KuehlKoerperSchaltung
     :cvar HEAT_SOURCE_CIRCUIT: 18: WärmekörperSchaltung
@@ -36,42 +36,41 @@
     :cvar SOLAR_THERMAL_CIRCUIT: SolarWarmwasserKreislauf
     :cvar SUB_METER_ELECTRICITY: 30: SubMeter Elektrisch
     :cvar TEMPERATURE_SENSOR: 31: Temperatursensor
     :cvar WASHER: 32: Waschmaschine
     :cvar BATTERY_SYSTEM: 33: Batteriesystem
     :cvar ELECTRICITY_GENERATION_SYSTEM: 34: Generator Elektrisch
     :cvar ELECTRICITY_STORAGE_SYSTEM: 35: ElektroSpeicher System
-    :cvar SGCP: 31: GridConnectionPoint Nachbarschaft
-    :cvar HOUSEHOLD: 327: Haushalt
+    :cvar SGCP: 36: GridConnectionPoint Nachbarschaft
+    :cvar HOUSEHOLD: 37: Haushalt
     :cvar PVSYSTEM: 38: PV System
     :cvar EV: 39: Elektromobil
     :cvar EVSE: 40: Ladestationscontroller für Elektrofahrzeug
     :cvar CHARGING_OUTLET: 41: Ladestation
     :cvar CEM: 42: Energiemanager für Endverbraucher
     :cvar ACTUATOR: 43:allgemein fuer Aktor
     :cvar SENSOR: 44: allgemein fuer Messdatenaufnahme
     :cvar CONTROLLER: 45:Steuergeraet
     :cvar ENV_CONDITION: 46:Umweltbedingungen
     :cvar FLEX_BUILDING_CAMPUS: 47: Gebäude und Campus.elektrische
         Flexibilität
-    :cvar R48: 48: Reserve
-    :cvar R49: 49: Reserve
+    :cvar DYNAMIC_TARIFF: 49: Dynamic Tariff
     :cvar R50: 50: Reserve
     """
     BATTERY = "Battery"
     COMPRESSOR = "Compressor"
     DEVICE_INFORMATION = "DeviceInformation"
     DHWCIRCUIT = "DHWCircuit"
     DHWSTORAGE = "DHWStorage"
     DISHWASHER = "Dishwasher"
     DRYER = "Dryer"
     ELECTRICAL_IMMERSION_HEATER = "ElectricalImmersionHeater"
     FAN = "Fan"
     GAS_HEATING_APPLIANCE = "GasHeatingAppliance"
-    NON_SPECIFIC = "NonSpecific"
+    METERING = "Metering"
     HEATING_BUFFER_STORAGE = "HeatingBufferStorage"
     HEATING_CIRCUIT = "HeatingCircuit"
     HEATING_OBJECT = "HeatingObject"
     HEATING_ZONE = "HeatingZone"
     HEAT_PUMP_CONTROL = "HeatPumpControl"
     HEAT_SINK_CIRCUIT = "HeatSinkCircuit"
     HEAT_SOURCE_CIRCUIT = "HeatSourceCircuit"
@@ -100,10 +99,9 @@
     CHARGING_OUTLET = "ChargingOutlet"
     CEM = "CEM"
     ACTUATOR = "Actuator"
     SENSOR = "Sensor"
     CONTROLLER = "Controller"
     ENV_CONDITION = "EnvCondition"
     FLEX_BUILDING_CAMPUS = "FlexBuildingCampus"
-    R48 = "R48"
-    R49 = "R49"
+    DYNAMIC_TARIFF = "DynamicTariff"
     R50 = "R50"
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/generic/base_type_level_of_operation_type.py` & `sgr-lib-0.0.2/sgr_library/generated/generic/base_type_level_of_operation_type.py`

 * *Files identical despite different names*

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/generic/base_types.py` & `sgr-lib-0.0.2/sgr_library/generated/generic/base_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 from dataclasses import dataclass, field
-from decimal import Decimal
 from enum import Enum
 from typing import List, Optional
 from xsdata.models.datatype import XmlDate
-from sgr_library.data_classes.generic.base_type_functional_profile_category import FunctionalProfileCategory
-from sgr_library.data_classes.generic.base_type_functional_profile_type import FunctionalProfileType
-from sgr_library.data_classes.generic.base_type_level_of_operation_type import LevelOfOperation
+from sgr_library.generated.generic.base_type_functional_profile_category import FunctionalProfileCategory
+from sgr_library.generated.generic.base_type_level_of_operation_type import LevelOfOperation
 
 __NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
 
 
 @dataclass
 class AlternativeNames:
     """a name list for EEBUS, IEC6850,, SAREF4ENER etc.
 
-    Used to support onology naming.
+    Used to support ontology naming.
 
+    :ivar s_lv1_name: Currently not used. Reserved for the future to
+        secure legacy compatibility one we start renaming in future SGr
+        label versions
     :ivar work_name: work name for temporary use
     :ivar manuf_name: manufacturers may use an internal wording
-    :ivar iec61850_name: IEC 61850 termonoligy place to add the 61850
-        abreviatuions
-    :ivar saref_name: SAREF for ENER termonoligy place to add the SAREF
-        abreviations (https://saref.etsi.org)
+    :ivar iec61850_name: IEC 61850 terminology place to add the 61850
+        abbreviatuions
+    :ivar saref_name: SAREF for ENER terminology place to add the SAREF
+        abbreviations (https://saref.etsi.org)
     :ivar eebus_name: EEBUS for terminology place to add the EEBUS
-        abreviations
+        abbreviations
     :ivar sun_spec_name: sSUNSPEC for terminology place to add the
-        www.sunspec.org abreviations
+        www.sunspec.org abbreviations
     :ivar hp_bwp_name: bwp (German Heat Pump Association) for
         terminology place to add the bwp naming for HVAC
     :ivar en17609_name: EN17609 terminology place to add the EU17609
         abbreviations
     """
+    s_lv1_name: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "sLV1Name",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
     work_name: Optional[str] = field(
         default=None,
         metadata={
             "name": "workName",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
@@ -186,19 +195,29 @@
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
 
 
-class DataDirection(Enum):
+class DataDirectionFunctionalProfile(Enum):
+    """
+    Read/write direction with read (R), write (W), read-write (RW)
+    """
+    R = "R"
+    W = "W"
+    RW = "RW"
+
+
+class DataDirectionProduct(Enum):
     """
     Read/write direction with read (R), write (W), read-write (RW), read-write
-    with persistent storage (RWP)
+    with persistent storage (RWP), or constant (C)
     """
+    C = "C"
     R = "R"
     W = "W"
     RW = "RW"
     RWP = "RWP"
 
 
 class DeviceCategory(Enum):
@@ -243,14 +262,15 @@
     :cvar ELECTRICITY_STORAGE_SYSTEM:
     :cvar SGCP: EEBUS: GridConnectionPointOfPremises
     :cvar HOUSEHOLD:
     :cvar PVSYSTEM:
     :cvar EV:
     :cvar EVSE:
     :cvar CHARGING_STATION: EEBUS: ChargingOutlet
+    :cvar ACTUATOR:
     :cvar CEM:
     """
     BATTERY = "Battery"
     COMPRESSOR = "Compressor"
     DEVICE_INFORMATION = "DeviceInformation"
     DHWCIRCUIT = "DHWCircuit"
     DHWSTORAGE = "DHWStorage"
@@ -286,22 +306,27 @@
     ELECTRICITY_STORAGE_SYSTEM = "ElectricityStorageSystem"
     SGCP = "SGCP"
     HOUSEHOLD = "Household"
     PVSYSTEM = "PVSystem"
     EV = "EV"
     EVSE = "EVSE"
     CHARGING_STATION = "ChargingStation"
+    ACTUATOR = "Actuator"
     CEM = "CEM"
 
 
 @dataclass
 class EmptyType:
     pass
 
 
+class EmptyValue(Enum):
+    VALUE = ""
+
+
 @dataclass
 class EnumEntry:
     """
     Maps a device specific ordinal to its literal.
     """
     literal: Optional[str] = field(
         default=None,
@@ -324,66 +349,98 @@
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
 
 
+@dataclass
+class EnumEntryProductRecord:
+    literal: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+    ordinal: Optional[int] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+    description: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+
+
+@dataclass
+class EnumEntryRecordFunctionalProfile:
+    literal: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+    description: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+
+
+@dataclass
+class GenericAttributeFunctionalProfile:
+    name: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+
+
 class Language(Enum):
     """this is the identification of the language for information to be
     published.
 
     So far en, de, fr and it is possible
     """
     DE = "de"
     EN = "en"
     FR = "fr"
     IT = "it"
 
 
-class MeasuredValueSource(Enum):
-    """
-    E0003.
-    """
-    MEASURED_VALUE = "measuredValue"
-    CALCULATED_VALUE = "calculatedValue"
-    EMPIRICAL_VALUE = "empiricalValue"
-
-
-class MeasuredValueType(Enum):
-    VALUE = "value"
-    MIN = "min"
-    MAX = "max"
-    AVERAGE = "average"
-    STD_DEV = "stdDev"
-
-
-class ObligLvlType(Enum):
-    """E0014: Obligation level of a reaction / function. SHALL: action is required
-    SHOULD: action is strongly recommended MAY: action is permitted"""
-    OL_SHALL = "OL_SHALL"
-    OL_SHOULD = "OL_SHOULD"
-    OL_MAY = "OL_MAY"
-
-
 class PowerSource(Enum):
     """
     E0004.
     """
     UNKNOWN = "unknown"
     MAINS1_PHASE = "mains1Phase"
     MAINS3_PHASE = "mains3Phase"
     BATTERY = "battery"
     DC = "dc"
 
 
 class PresenceLevel(Enum):
     """
-    Indicates wheter the element is mandatory (M), recommended (R, at least one
-    of the R elements mus be present), or optional (O, can be ommitted)
+    Indicates whether the element is mandatory (M), recommended (R, at least
+    one of the R elements must be present), or optional (O, can be omitted)
     """
     M = "M"
     R = "R"
     O = "O"
 
 
 class ReleaseState(Enum):
@@ -392,28 +449,18 @@
     """
     DRAFT = "Draft"
     REVIEW = "Review"
     PUBLISHED = "Published"
     REVOKED = "Revoked"
 
 
-class SgcpserviceType(Enum):
-    """E0013: Assistance type of a reaction / function. This Attribute indicates the
-    type of Flexibility Entity of the operation NET servicable: Operation for the benefit of a
-    distribution network operator (DSO) SYS servicable: Operation of the total system operators
-    (TSO) ENER servicable: Operation for energy optimization"""
-    AT_NET_SERVICEABLE = "AT_NetServiceable"
-    AT_SYS_SERVICEABLE = "AT_SysServiceable"
-    AT_ENER_SERVICEABLE = "AT_EnerServiceable"
-
-
 @dataclass
 class ScalingFactor:
     """scaled_value = value * multiplicator * 10^powerof10 This type is used for to
-    convert intereger datapoint values into floats only"""
+    convert integer datapoint values into floats only"""
     multiplicator: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
@@ -424,301 +471,54 @@
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
 
 
-@dataclass
-class SmoothTransition:
-    """
-    The time behavior of a transition from a power adjustment (positive as well
-    as negative) can be determined by several time values, so that this starts
-    with a random time delay, changes via a ramp and an expiry time with return
-    to the initial value.
-
-    :ivar win_tms: indicates a time window in seconds in which the new
-        operating mode is started randomly. The time window begins with
-        the start command of the operating mode. The value 0 means
-        immediate
-    :ivar rvrt_tms: determines how long the operating mode should be
-        active in seconds. When the time has elapsed, the operating mode
-        is automatically terminated. If rvrtTms = 0 (standard value),
-        the operating mode remains active until a new command is
-        received.
-    :ivar rmp_tms: specifies how quickly the changes should be made in
-        seconds. The corresponding value is gradually changed from the
-        old to the new value in the specified time.
-    """
-    win_tms: Optional[int] = field(
-        default=None,
-        metadata={
-            "name": "winTms",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-        }
-    )
-    rvrt_tms: Optional[int] = field(
-        default=None,
-        metadata={
-            "name": "rvrtTms",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-        }
-    )
-    rmp_tms: Optional[int] = field(
-        default=None,
-        metadata={
-            "name": "rmpTms",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-        }
-    )
-
-
-@dataclass
-class StabilityFallback:
-    """A consumer or a generating system receives the permit for a load change
-    for a certain period of time.
-
-    This time is always set to 0 each time a confirmation message is
-    received (HeartBeat).
-
-    :ivar max_receive_time: Time in seconds. If the device does not
-        recieve any communication within this specified time the device
-        automatically initiates the fallback. 0 indicates no fallback
-        will be performed.
-    :ivar init_value: Value of the reference variable at the start of
-        the process cycle. Unit: inherited
-    :ivar fallback_value: Value of the reference variable in the event
-        of a communication failure . Unit:inherited
-    """
-    max_receive_time: Optional[float] = field(
-        default=None,
-        metadata={
-            "name": "maxReceiveTime",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
-        }
-    )
-    init_value: Optional[Decimal] = field(
-        default=None,
-        metadata={
-            "name": "initValue",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
-        }
-    )
-    fallback_value: Optional[Decimal] = field(
-        default=None,
-        metadata={
-            "name": "fallbackValue",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
-        }
-    )
-
-
 class Units(Enum):
-    AMPERE_SQUARE_METERS = "AMPERE_SQUARE_METERS"
     AMPERES = "AMPERES"
-    AMPERES_PER_METER = "AMPERES_PER_METER"
-    AMPERES_PER_SQUARE_METER = "AMPERES_PER_SQUARE_METER"
     BARS = "BARS"
-    BTUS = "BTUS"
-    BTUS_PER_HOUR = "BTUS_PER_HOUR"
-    BTUS_PER_POUND = "BTUS_PER_POUND"
-    BTUS_PER_POUND_DRY_AIR = "BTUS_PER_POUND_DRY_AIR"
-    CANDELAS = "CANDELAS"
-    CANDELAS_PER_SQUARE_METER = "CANDELAS_PER_SQUARE_METER"
-    CENTIMETERS = "CENTIMETERS"
-    CENTIMETERS_OF_MERCURY = "CENTIMETERS_OF_MERCURY"
-    CENTIMETERS_OF_WATER = "CENTIMETERS_OF_WATER"
-    CUBIC_FEET = "CUBIC_FEET"
-    CUBIC_FEET_PER_MINUTE = "CUBIC_FEET_PER_MINUTE"
-    CUBIC_FEET_PER_SECOND = "CUBIC_FEET_PER_SECOND"
     CUBIC_METERS = "CUBIC_METERS"
-    CUBIC_METERS_PER_HOUR = "CUBIC_METERS_PER_HOUR"
-    CUBIC_METERS_PER_MINUTE = "CUBIC_METERS_PER_MINUTE"
     CUBIC_METERS_PER_SECOND = "CUBIC_METERS_PER_SECOND"
-    CURRENCY1 = "CURRENCY1"
-    CURRENCY10 = "CURRENCY10"
-    CURRENCY2 = "CURRENCY2"
-    CURRENCY3 = "CURRENCY3"
-    CURRENCY4 = "CURRENCY4"
-    CURRENCY5 = "CURRENCY5"
-    CURRENCY6 = "CURRENCY6"
-    CURRENCY7 = "CURRENCY7"
-    CURRENCY8 = "CURRENCY8"
-    CURRENCY9 = "CURRENCY9"
-    CYCLES_PER_HOUR = "CYCLES_PER_HOUR"
-    CYCLES_PER_MINUTE = "CYCLES_PER_MINUTE"
-    DAYS = "DAYS"
-    DEGREE_DAYS_CELSIUS = "DEGREE_DAYS_CELSIUS"
-    DEGREE_DAYS_FAHRENHEIT = "DEGREE_DAYS_FAHRENHEIT"
-    DEGREES_ANGULAR = "DEGREES_ANGULAR"
     DEGREES_CELSIUS = "DEGREES_CELSIUS"
-    DEGREES_CELSIUS_PER_HOUR = "DEGREES_CELSIUS_PER_HOUR"
-    DEGREES_CELSIUS_PER_MINUTE = "DEGREES_CELSIUS_PER_MINUTE"
-    DEGREES_FAHRENHEIT = "DEGREES_FAHRENHEIT"
-    DEGREES_FAHRENHEIT_PER_HOUR = "DEGREES_FAHRENHEIT_PER_HOUR"
-    DEGREES_FAHRENHEIT_PER_MINUTE = "DEGREES_FAHRENHEIT_PER_MINUTE"
-    DEGREES_KELVIN = "DEGREES_KELVIN"
-    DEGREES_KELVIN_PER_HOUR = "DEGREES_KELVIN_PER_HOUR"
-    DEGREES_KELVIN_PER_MINUTE = "DEGREES_KELVIN_PER_MINUTE"
     DEGREES_PHASE = "DEGREES_PHASE"
-    DELTA_DEGREES_FAHRENHEIT = "DELTA_DEGREES_FAHRENHEIT"
-    DELTA_DEGREES_KELVIN = "DELTA_DEGREES_KELVIN"
-    FARADS = "FARADS"
-    FEET = "FEET"
-    FEET_PER_MINUTE = "FEET_PER_MINUTE"
-    FEET_PER_SECOND = "FEET_PER_SECOND"
-    FOOT_CANDLES = "FOOT_CANDLES"
-    GIGAJOULES = "GIGAJOULES"
-    GRAMS_OF_WATER_PER_KILOGRAM_DRY_AIR = "GRAMS_OF_WATER_PER_KILOGRAM_DRY_AIR"
-    GRAMS_PER_MINUTE = "GRAMS_PER_MINUTE"
-    GRAMS_PER_SECOND = "GRAMS_PER_SECOND"
-    HECTOPASCALS = "HECTOPASCALS"
-    HENRYS = "HENRYS"
     HERTZ = "HERTZ"
-    HORSEPOWER = "HORSEPOWER"
     HOURS = "HOURS"
-    HUNDREDTHS_SECONDS = "HUNDREDTHS_SECONDS"
-    IMPERIAL_GALLONS = "IMPERIAL_GALLONS"
-    IMPERIAL_GALLONS_PER_MINUTE = "IMPERIAL_GALLONS_PER_MINUTE"
-    INCHES = "INCHES"
-    INCHES_OF_MERCURY = "INCHES_OF_MERCURY"
-    INCHES_OF_WATER = "INCHES_OF_WATER"
-    JOULE_SECONDS = "JOULE_SECONDS"
     JOULES = "JOULES"
-    JOULES_PER_DEGREE_KELVIN = "JOULES_PER_DEGREE_KELVIN"
-    JOULES_PER_KILOGRAM_DEGREE_KELVIN = "JOULES_PER_KILOGRAM_DEGREE_KELVIN"
-    JOULES_PER_KILOGRAM_DRY_AIR = "JOULES_PER_KILOGRAM_DRY_AIR"
-    KILO_BTUS = "KILO_BTUS"
-    KILO_BTUS_PER_HOUR = "KILO_BTUS_PER_HOUR"
     KILOGRAMS = "KILOGRAMS"
-    KILOGRAMS_PER_CUBIC_METER = "KILOGRAMS_PER_CUBIC_METER"
-    KILOGRAMS_PER_HOUR = "KILOGRAMS_PER_HOUR"
-    KILOGRAMS_PER_MINUTE = "KILOGRAMS_PER_MINUTE"
-    KILOGRAMS_PER_SECOND = "KILOGRAMS_PER_SECOND"
-    KILOHERTZ = "KILOHERTZ"
-    KILOOHMS = "KILOOHMS"
-    KILOJOULES = "KILOJOULES"
-    KILOJOULES_PER_DEGREE_KELVIN = "KILOJOULES_PER_DEGREE_KELVIN"
-    KILOJOULES_PER_KILOGRAM = "KILOJOULES_PER_KILOGRAM"
-    KILOJOULES_PER_KILOGRAM_DRY_AIR = "KILOJOULES_PER_KILOGRAM_DRY_AIR"
-    KILOMETERS_PER_HOUR = "KILOMETERS_PER_HOUR"
-    KILOPASCALS = "KILOPASCALS"
     KILOVOLT_AMPERES = "KILOVOLT_AMPERES"
     KILOVOLT_AMPERE_HOURS = "KILOVOLT_AMPERE_HOURS"
     KILOVOLT_AMPERES_REACTIVE = "KILOVOLT_AMPERES_REACTIVE"
     KILOVOLT_AMPERES_REACTIVE_HOURS = "KILOVOLT_AMPERES_REACTIVE_HOURS"
-    KILOVOLTS = "KILOVOLTS"
     KILOWATT_HOURS = "KILOWATT_HOURS"
     KILOWATTS = "KILOWATTS"
-    KW_HOURS_PER_SQUARE_FOOT = "KW_HOURS_PER_SQUARE_FOOT"
-    KW_HOURS_PER_SQUARE_METER = "KW_HOURS_PER_SQUARE_METER"
-    LITERS = "LITERS"
-    LITERS_PER_HOUR = "LITERS_PER_HOUR"
-    LITERS_PER_MINUTE = "LITERS_PER_MINUTE"
-    LITERS_PER_SECOND = "LITERS_PER_SECOND"
-    LUMENS = "LUMENS"
-    LUXES = "LUXES"
-    MEGA_BTUS = "MEGA_BTUS"
-    MEGAHERTZ = "MEGAHERTZ"
-    MEGAJOULES = "MEGAJOULES"
-    MEGAJOULES_PER_DEGREE_KELVIN = "MEGAJOULES_PER_DEGREE_KELVIN"
-    MEGAJOULES_PER_KILOGRAM_DRY_AIR = "MEGAJOULES_PER_KILOGRAM_DRY_AIR"
-    MEGAJOULES_PER_SQUARE_FOOT = "MEGAJOULES_PER_SQUARE_FOOT"
-    MEGAJOULES_PER_SQUARE_METER = "MEGAJOULES_PER_SQUARE_METER"
-    MEGAVOLT_AMPERES = "MEGAVOLT_AMPERES"
-    MEGAVOLT_AMPERES_REACTIVE = "MEGAVOLT_AMPERES_REACTIVE"
-    MEGAVOLTS = "MEGAVOLTS"
     MEGAWATT_HOURS = "MEGAWATT_HOURS"
-    MEGAWATTS = "MEGAWATTS"
-    MEGOHMS = "MEGOHMS"
     METERS = "METERS"
-    METERS_PER_HOUR = "METERS_PER_HOUR"
-    METERS_PER_MINUTE = "METERS_PER_MINUTE"
     METERS_PER_SECOND = "METERS_PER_SECOND"
     METERS_PER_SECOND_PER_SECOND = "METERS_PER_SECOND_PER_SECOND"
-    MILES_PER_HOUR = "MILES_PER_HOUR"
-    MILLIAMPERES = "MILLIAMPERES"
-    MILLIBARS = "MILLIBARS"
-    MILLIMETERS = "MILLIMETERS"
-    MILLIMETERS_OF_MERCURY = "MILLIMETERS_OF_MERCURY"
-    MILLIMETERS_PER_MINUTE = "MILLIMETERS_PER_MINUTE"
-    MILLIMETERS_PER_SECOND = "MILLIMETERS_PER_SECOND"
-    MILLIOHMS = "MILLIOHMS"
-    MILLISECONDS = "MILLISECONDS"
-    MILLIVOLTS = "MILLIVOLTS"
-    MILLIWATTS = "MILLIWATTS"
     MINUTES = "MINUTES"
-    MONTHS = "MONTHS"
-    NEWTON = "NEWTON"
-    NEWTON_METERS = "NEWTON_METERS"
-    NEWTON_SECONDS = "NEWTON_SECONDS"
-    NEWTONS_PER_METER = "NEWTONS_PER_METER"
     NO_UNITS = "NO_UNITS"
-    OHM_METERS = "OHM_METERS"
     OHMS = "OHMS"
-    PARTS_PER_BILLION = "PARTS_PER_BILLION"
     PARTS_PER_MILLION = "PARTS_PER_MILLION"
     PASCALS = "PASCALS"
     PER_HOUR = "PER_HOUR"
-    PER_MINUTE = "PER_MINUTE"
-    PER_SECOND = "PER_SECOND"
     PERCENT = "PERCENT"
-    PERCENT_OBSCURATION_PER_FOOT = "PERCENT_OBSCURATION_PER_FOOT"
-    PERCENT_OBSCURATION_PER_METER = "PERCENT_OBSCURATION_PER_METER"
-    PERCENT_PER_SECOND = "PERCENT_PER_SECOND"
     PERCENT_RELATIVE_HUMIDITY = "PERCENT_RELATIVE_HUMIDITY"
-    POUNDS_FORCE_PER_SQUARE_INCH = "POUNDS_FORCE_PER_SQUARE_INCH"
-    POUNDS_MASS = "POUNDS_MASS"
-    POUNDS_MASS_PER_HOUR = "POUNDS_MASS_PER_HOUR"
-    POUNDS_MASS_PER_MINUTE = "POUNDS_MASS_PER_MINUTE"
-    POUNDS_MASS_PER_SECOND = "POUNDS_MASS_PER_SECOND"
     POWER_FACTOR = "POWER_FACTOR"
-    PSI_PER_DEGREE_FAHRENHEIT = "PSI_PER_DEGREE_FAHRENHEIT"
     RADIANS = "RADIANS"
     RADIANS_PER_SECOND = "RADIANS_PER_SECOND"
     REVOLUTIONS_PER_MINUTE = "REVOLUTIONS_PER_MINUTE"
     SECONDS = "SECONDS"
-    SIEMENS = "SIEMENS"
-    SIEMENS_PER_METER = "SIEMENS_PER_METER"
-    SQUARE_CENTIMETERS = "SQUARE_CENTIMETERS"
-    SQUARE_FEET = "SQUARE_FEET"
-    SQUARE_INCHES = "SQUARE_INCHES"
     SQUARE_METERS = "SQUARE_METERS"
-    SQUARE_METERS_PER_NEWTON = "SQUARE_METERS_PER_NEWTON"
-    TESLAS = "TESLAS"
-    THERMS = "THERMS"
-    TON_HOURS = "TON_HOURS"
-    TONS = "TONS"
-    TONS_PER_HOUR = "TONS_PER_HOUR"
-    TONS_REFRIGERATION = "TONS_REFRIGERATION"
-    US_GALLONS = "US_GALLONS"
-    US_GALLONS_PER_MINUTE = "US_GALLONS_PER_MINUTE"
     VOLT_AMPERES = "VOLT_AMPERES"
     VOLT_AMPERES_REACTIVE = "VOLT_AMPERES_REACTIVE"
     VOLTS = "VOLTS"
-    VOLTS_PER_DEGREE_KELVIN = "VOLTS_PER_DEGREE_KELVIN"
-    VOLTS_PER_METER = "VOLTS_PER_METER"
     WATT_HOURS = "WATT_HOURS"
     WATTS = "WATTS"
-    WATTS_PER_METER_PER_DEGREE_KELVIN = "WATTS_PER_METER_PER_DEGREE_KELVIN"
-    WATTS_PER_SQUARE_FOOT = "WATTS_PER_SQUARE_FOOT"
-    WATTS_PER_SQUARE_METER = "WATTS_PER_SQUARE_METER"
-    WATTS_PER_SQUARE_METER_DEGREE_KELVIN = "WATTS_PER_SQUARE_METER_DEGREE_KELVIN"
-    WEBERS = "WEBERS"
-    WEEKS = "WEEKS"
-    YEARS = "YEARS"
     NONE = "NONE"
 
 
 @dataclass
 class VersionNumber:
     """
     a three digit version mumber system.
@@ -749,77 +549,25 @@
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
 
 
 @dataclass
-class EnumEntryProductRecord:
-    class Meta:
-        name = "enumEntryProductRecord"
-
-    literal: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
-        }
-    )
-    ordinal: Optional[int] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-        }
-    )
-    description: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-        }
-    )
-
-
-@dataclass
-class EnumEntryRecordFunctionalProfile:
-    class Meta:
-        name = "enumEntryRecordFunctionalProfile"
-
-    literal: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
-        }
-    )
-    description: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-        }
-    )
-
-
-@dataclass
 class BitmapFunctionalProfile:
     """bitmap for status bits.
 
     Maps device-specific bit patterns (as hex mask) to literals.
     """
     bitmap_entry: List[BitmapEntryFunctionalProfile] = field(
         default_factory=list,
         metadata={
             "name": "bitmapEntry",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "min_occurs": 1,
         }
     )
 
 
 @dataclass
 class BitmapProduct:
     """bitmap for status bits.
@@ -873,15 +621,14 @@
 class EnumMapFunctionalProfile:
     enum_entry: List[EnumEntryRecordFunctionalProfile] = field(
         default_factory=list,
         metadata={
             "name": "enumEntry",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "min_occurs": 1,
         }
     )
     hex_mask: Optional[bytes] = field(
         default=None,
         metadata={
             "name": "hexMask",
             "type": "Element",
@@ -910,54 +657,34 @@
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "format": "base16",
         }
     )
 
 
 @dataclass
-class FlexAssistance:
-    assists: Optional[SgcpserviceType] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
-        }
-    )
-    obliged_to: Optional[ObligLvlType] = field(
-        default=None,
-        metadata={
-            "name": "obligedTo",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
-        }
-    )
-
-
-@dataclass
 class FunctionalProfileIdentification:
     """
     Specification of design source 0 means: specified by SmartGridready, the
-    Porfilenumber follows the SmargGirdready scheme &gt;0 means: specfied by
-    manufacturer hhhh, the Profilenumber followos a manufacturors scheme.
+    Profile number follows the SmargGirdready scheme &gt;0 means: specified by
+    manufacturer hhhh, the Profile number follows a manufacturers scheme.
 
     :ivar specification_owner_identification:
-    :ivar functional_profile_category: The Profile Identfication
-        identiofis the main profile classes. The enumeration text is
+    :ivar functional_profile_category: The Profile Identification
+        identifies the main profile classes. The enumeration text is
         also documented with numbers being referenced in the profile
         number hhhh.nnnn.uuuu.ss.VV.vv as nnnn
     :ivar functional_profile_type:
     :ivar level_of_operation: levelOfOperation defines a controls
-        complexity level m) for read-only monitoring dat points level 1)
-        single contact 2) 2 or more contacts /state controlled interface
-        3) statical defined characteristics tables 4) dynamic realtime
-        control combined with statical defined characteristics tables 5)
-        dynamic realtime control combined with dynamic changeable
-        characteristics tables 6) prognosis based systems
+        complexity level m) for read-only monitoring data points level
+        1) single contact 2) 2 or more contacts /state controlled
+        interface 3) statistical defined characteristics tables 4)
+        dynamic real-time control combined with statistical defined
+        characteristics tables 5) dynamic real-time control combined
+        with dynamic changeable characteristics tables 6) prediction
+        based systems
     :ivar version_number:
     """
     specification_owner_identification: Optional[str] = field(
         default=None,
         metadata={
             "name": "specificationOwnerIdentification",
             "type": "Element",
@@ -970,15 +697,15 @@
         metadata={
             "name": "functionalProfileCategory",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
-    functional_profile_type: Optional[FunctionalProfileType] = field(
+    functional_profile_type: Optional[str] = field(
         default=None,
         metadata={
             "name": "functionalProfileType",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
@@ -1000,23 +727,72 @@
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
 
 
 @dataclass
+class GenericAttributeListFunctionalProfile:
+    generic_attribute_list_element: List[GenericAttributeFunctionalProfile] = field(
+        default_factory=list,
+        metadata={
+            "name": "genericAttributeListElement",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "min_occurs": 1,
+        }
+    )
+
+
+@dataclass
+class JsonElemFunctionalProfile:
+    class Meta:
+        name = "JSonElemFunctionalProfile"
+
+    key: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+    date: Optional[EmptyValue] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+    string: Optional[EmptyValue] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+    number: Optional[EmptyValue] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+
+
+@dataclass
 class LegibleDescription:
     """This element us used to extend the definitions with legible text
-    elements: a short understandbale explanation of the items addressed.
+    elements: a short understandable explanation of the items addressed.
 
     These elements are used for printed and published information
 
     :ivar text_element: information to be published
     :ivar language: language identifier de, en, fr, it
-    :ivar uri: optional URI pointong towards additional information
+    :ivar uri: optional URI pointing towards additional information
     """
     text_element: Optional[str] = field(
         default=None,
         metadata={
             "name": "textElement",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
@@ -1069,28 +845,35 @@
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
 
 
 @dataclass
-class DataTypeFunctionalProfile:
-    """Generic high-level data types.
+class DataTypeProduct:
+    """Generic high-devel data types.
 
     Implementations of this XSD map these types into native data types
-    in their programming language (java, python, golang, ...)
+    in their programming language (java, python, go lang, ...)
     """
-    enum: Optional[EnumMapFunctionalProfile] = field(
+    enum: Optional[EnumMapProduct] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    bitmap: Optional[BitmapFunctionalProfile] = field(
+    bitmap: Optional[BitmapProduct] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+    json: Optional[EmptyValue] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
     boolean: Optional[EmptyType] = field(
@@ -1188,306 +971,295 @@
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
 
 
 @dataclass
-class DataTypeProduct:
-    """Generic high-ldevel data types.
+class JsonArrayOutputFunctionalProfile:
+    class Meta:
+        name = "JSonArrayOutputFunctionalProfile"
 
-    Implementations of this XSD map these types into native data types
-    in their programming language (java, python, golang, ...)
-    """
-    enum: Optional[EnumMapProduct] = field(
+    name: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    bitmap: Optional[BitmapProduct] = field(
-        default=None,
+    array: List["JsonArrayOutputFunctionalProfile"] = field(
+        default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
+            "sequential": True,
         }
     )
-    boolean: Optional[EmptyType] = field(
-        default=None,
+    elem: List[JsonElemFunctionalProfile] = field(
+        default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
+            "sequential": True,
         }
     )
-    int8: Optional[EmptyType] = field(
-        default=None,
+
+
+@dataclass
+class RequestParam:
+    param: List[JsonElemFunctionalProfile] = field(
+        default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
+            "min_occurs": 1,
         }
     )
-    int16: Optional[EmptyType] = field(
+
+
+@dataclass
+class GenericAttributeProductEnd:
+    name: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
         }
     )
-    int32: Optional[EmptyType] = field(
+    data_type: Optional[DataTypeProduct] = field(
         default=None,
         metadata={
+            "name": "dataType",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    int64: Optional[EmptyType] = field(
+    value: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    int8_u: Optional[EmptyType] = field(
+    unit: Optional[Units] = field(
         default=None,
         metadata={
-            "name": "int8U",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    int16_u: Optional[EmptyType] = field(
-        default=None,
+
+
+@dataclass
+class JsonOutputFunctionalProfile:
+    class Meta:
+        name = "JSonOutputFunctionalProfile"
+
+    array: List[JsonArrayOutputFunctionalProfile] = field(
+        default_factory=list,
         metadata={
-            "name": "int16U",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    int32_u: Optional[EmptyType] = field(
-        default=None,
+    elem: List[JsonElemFunctionalProfile] = field(
+        default_factory=list,
         metadata={
-            "name": "int32U",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    int64_u: Optional[EmptyType] = field(
+
+
+@dataclass
+class DataTypeFunctionalProfile:
+    """Generic high-level data types.
+
+    Implementations of this XSD map these types into native data types
+    in their programming language (java, python, golang, ...)
+    """
+    enum: Optional[EnumMapFunctionalProfile] = field(
         default=None,
         metadata={
-            "name": "int64U",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    float32: Optional[EmptyType] = field(
+    bitmap: Optional[BitmapFunctionalProfile] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    float64: Optional[EmptyType] = field(
+    json: Optional[JsonOutputFunctionalProfile] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    date_time: Optional[EmptyType] = field(
+    boolean: Optional[EmptyType] = field(
         default=None,
         metadata={
-            "name": "dateTime",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    string: Optional[EmptyType] = field(
+    int8: Optional[EmptyType] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-
-
-@dataclass
-class GenericAttributes:
-    """these attributes are defined for the generic interface for the
-    application programmer.
-
-    An attribute can be aligned to either a device, a functional Profile
-    or a datapoint
-
-    :ivar max_val: upper range limit. Unit:inherited
-    :ivar min_val: lower range limit. Unit:inherited
-    :ivar special_quality_requirement: indicates quality requirements
-        fullfilled like formal certifications
-    :ivar precision_percent: the precisionPercent of a measurement,
-        calculation result or result of a controls process
-    :ivar stability_fallback: A consumer or a generating system receives
-        the permit for a load change for a certain period of time. This
-        time is always set to 0 each time a confirmation message is
-        received (HeartBeat).
-    :ivar smooth_transition: The time behavior of a transition from a
-        power adjustment (positive as well as negative) can be
-        determined by several time values, so that this starts with a
-        random time delay, changes via a ramp and an expiry time with
-        return to the initial value.
-    :ivar max_latency_time_ms: Maximum time in milliseconds from
-        capturing of measured value until ready at the product interface
-        (i.e. analog-digital conversion time)
-    :ivar measured_value_type: MeasValueType: type of measurement.
-        Possbile values are "value", "min", max", "average", "stdDev"
-    :ivar measured_value_source: Value source kind related to SGr level
-        6 applications. Potential values are measuredValue,
-        calculatedValue, empiricalValue
-    :ivar sample_rate_hz: SampleRate in Hertz
-    :ivar curtailment:
-    :ivar min_load:
-    :ivar max_lock_time_minutes:
-    :ivar min_run_time_minutes:
-    :ivar value_by_time_table_minutes:
-    :ivar flex_assistance: Systems with more than One communicator need
-        a definition of the priority of the commands / demands for a
-        flexibility requirement. This element defines the kind of a such
-        a command (servicable for net (DSO), energy or system (TNO)) and
-        its priority (SHALL / SHOULD / MAY)
-    :ivar unit_conversion_multiplicator:
-    """
-    max_val: Optional[Decimal] = field(
+    int16: Optional[EmptyType] = field(
         default=None,
         metadata={
-            "name": "maxVal",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    min_val: Optional[Decimal] = field(
+    int32: Optional[EmptyType] = field(
         default=None,
         metadata={
-            "name": "minVal",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    special_quality_requirement: Optional[str] = field(
+    int64: Optional[EmptyType] = field(
         default=None,
         metadata={
-            "name": "specialQualityRequirement",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    precision_percent: Optional[Decimal] = field(
+    int8_u: Optional[EmptyType] = field(
         default=None,
         metadata={
-            "name": "precisionPercent",
+            "name": "int8U",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "min_inclusive": Decimal("0.001"),
-            "max_inclusive": Decimal("15"),
         }
     )
-    stability_fallback: Optional[StabilityFallback] = field(
+    int16_u: Optional[EmptyType] = field(
         default=None,
         metadata={
-            "name": "stabilityFallback",
+            "name": "int16U",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    smooth_transition: Optional[SmoothTransition] = field(
+    int32_u: Optional[EmptyType] = field(
         default=None,
         metadata={
-            "name": "smoothTransition",
+            "name": "int32U",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    max_latency_time_ms: Optional[int] = field(
+    int64_u: Optional[EmptyType] = field(
         default=None,
         metadata={
-            "name": "maxLatencyTimeMs",
+            "name": "int64U",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    measured_value_type: Optional[MeasuredValueType] = field(
+    float32: Optional[EmptyType] = field(
         default=None,
         metadata={
-            "name": "measuredValueType",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    measured_value_source: Optional[MeasuredValueSource] = field(
+    float64: Optional[EmptyType] = field(
         default=None,
         metadata={
-            "name": "measuredValueSource",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    sample_rate_hz: Optional[int] = field(
+    date_time: Optional[EmptyType] = field(
         default=None,
         metadata={
-            "name": "sampleRateHz",
+            "name": "dateTime",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    curtailment: Optional[float] = field(
+    string: Optional[EmptyType] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    min_load: Optional[float] = field(
-        default=None,
+
+
+@dataclass
+class GenericAttributeListProductEnd:
+    generic_attribute_list_element: List[GenericAttributeProductEnd] = field(
+        default_factory=list,
         metadata={
-            "name": "minLoad",
+            "name": "genericAttributeListElement",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
+            "min_occurs": 1,
         }
     )
-    max_lock_time_minutes: Optional[float] = field(
+
+
+@dataclass
+class GenericAttributeProduct:
+    name: Optional[str] = field(
         default=None,
         metadata={
-            "name": "maxLockTimeMinutes",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
         }
     )
-    min_run_time_minutes: Optional[float] = field(
+    data_type: Optional[DataTypeProduct] = field(
         default=None,
         metadata={
-            "name": "minRunTimeMinutes",
+            "name": "dataType",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    value_by_time_table_minutes: Optional[float] = field(
+    value: Optional[str] = field(
         default=None,
         metadata={
-            "name": "valueByTimeTableMinutes",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    flex_assistance: Optional[FlexAssistance] = field(
+    unit: Optional[Units] = field(
         default=None,
         metadata={
-            "name": "flexAssistance",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    unit_conversion_multiplicator: Optional[float] = field(
+    generic_attribute_list: Optional[GenericAttributeListProductEnd] = field(
         default=None,
         metadata={
-            "name": "unitConversionMultiplicator",
+            "name": "genericAttributeList",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
+
+
+@dataclass
+class GenericAttributeListProduct:
+    generic_attribute_list_element: List[GenericAttributeProduct] = field(
+        default_factory=list,
+        metadata={
+            "name": "genericAttributeListElement",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "min_occurs": 1,
+        }
+    )
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/generic/data_point.py` & `sgr-lib-0.0.2/sgr_library/generated/generic/data_point.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from dataclasses import dataclass, field
 from typing import List, Optional
-from sgr_library.data_classes.generic.base_types import (
+from sgr_library.generated.generic.base_types import (
     AlternativeNames,
-    DataDirection,
+    DataDirectionProduct,
     DataTypeProduct,
-    GenericAttributes,
+    GenericAttributeListProduct,
     LegibleDescription,
-    PresenceLevel,
     Units,
 )
 
 __NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
 
 
 @dataclass
 class DataPointDescription:
     """
     Generic data point properties.
 
     :ivar data_point_name: Name of the data point (unique on functional
         profile)
     :ivar data_direction:
-    :ivar presence_level:
     :ivar data_type:
+    :ivar value:
     :ivar unit:
     :ivar array_length: Optional, if present the data point is an array
         of specified length
+    :ivar minimum_value:
+    :ivar maximum_value:
+    :ivar unit_conversion_multiplicator:
     :ivar alternative_names:
     :ivar legible_description: Published and printable information
         related to this data point
     :ivar programmer_hints: additional device-specific implementation
         hints for this data point
     """
     data_point_name: Optional[str] = field(
@@ -37,39 +39,37 @@
         metadata={
             "name": "dataPointName",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
-    data_direction: Optional[DataDirection] = field(
+    data_direction: Optional[DataDirectionProduct] = field(
         default=None,
         metadata={
             "name": "dataDirection",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
-    presence_level: Optional[PresenceLevel] = field(
+    data_type: Optional[DataTypeProduct] = field(
         default=None,
         metadata={
-            "name": "presenceLevel",
+            "name": "dataType",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
-    data_type: Optional[DataTypeProduct] = field(
+    value: Optional[str] = field(
         default=None,
         metadata={
-            "name": "dataType",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
         }
     )
     unit: Optional[Units] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
@@ -80,14 +80,38 @@
         default=None,
         metadata={
             "name": "arrayLength",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
+    minimum_value: Optional[float] = field(
+        default=None,
+        metadata={
+            "name": "minimumValue",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+    maximum_value: Optional[float] = field(
+        default=None,
+        metadata={
+            "name": "maximumValue",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+    unit_conversion_multiplicator: Optional[float] = field(
+        default=None,
+        metadata={
+            "name": "unitConversionMultiplicator",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
     alternative_names: Optional[AlternativeNames] = field(
         default=None,
         metadata={
             "name": "alternativeNames",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
@@ -122,15 +146,15 @@
         metadata={
             "name": "dataPoint",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
-    generic_attributes: Optional[GenericAttributes] = field(
+    generic_attribute_list: Optional[GenericAttributeListProduct] = field(
         default=None,
         metadata={
-            "name": "genericAttributes",
+            "name": "genericAttributeList",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/generic/functional_profile.py` & `sgr-lib-0.0.2/sgr_library/generated/generic/generic_attribute.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,93 +1,95 @@
 from dataclasses import dataclass, field
 from typing import List, Optional
-from sgr_library.data_classes.generic.base_types import (
-    AlternativeNames,
-    FunctionalProfileIdentification,
-    GenericAttributes,
+from sgr_library.generated.generic.base_types import (
+    DataTypeFunctionalProfile,
     LegibleDescription,
+    Units,
 )
 
 __NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
 
 
 @dataclass
-class FunctionalProfileDescription:
-    """
-    Functional profile properties.
-
-    :ivar functional_profile_name:
-    :ivar functional_profile_identification:
-    :ivar alternative_names:
-    :ivar legible_description: Published and printable information
-        related to this functional profile
-    :ivar programmer_hints: additional device-specific implementation
-        hints for this functional profile
-    """
-    functional_profile_name: Optional[str] = field(
+class GenericAttributeListElement:
+    name: Optional[str] = field(
         default=None,
         metadata={
-            "name": "functionalProfileName",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
         }
     )
-    functional_profile_identification: Optional[FunctionalProfileIdentification] = field(
+    data_type: Optional[DataTypeFunctionalProfile] = field(
         default=None,
         metadata={
-            "name": "functionalProfileIdentification",
+            "name": "dataType",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
-    alternative_names: Optional[AlternativeNames] = field(
+    unit: Optional[Units] = field(
         default=None,
         metadata={
-            "name": "alternativeNames",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-        }
-    )
-    legible_description: List[LegibleDescription] = field(
-        default_factory=list,
-        metadata={
-            "name": "legibleDescription",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "max_occurs": 4,
+            "required": True,
         }
     )
-    programmer_hints: List[LegibleDescription] = field(
+
+
+@dataclass
+class GenericAttributeList:
+    generic_attribute_list_element: List[GenericAttributeListElement] = field(
         default_factory=list,
         metadata={
-            "name": "programmerHints",
+            "name": "genericAttributeListElement",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "max_occurs": 4,
+            "min_occurs": 1,
         }
     )
 
 
 @dataclass
-class FunctionalProfileBase:
+class GenericAttributeFrame:
     """
-    Functional profile element.
+    Generic Attribute.
     """
-    functional_profile: Optional[FunctionalProfileDescription] = field(
+    class Meta:
+        namespace = "http://www.smartgridready.com/ns/V0/"
+
+    name: Optional[str] = field(
         default=None,
         metadata={
-            "name": "functionalProfile",
             "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
         }
     )
-    generic_attributes: Optional[GenericAttributes] = field(
+    generic_attribute_list: Optional[GenericAttributeList] = field(
         default=None,
         metadata={
-            "name": "genericAttributes",
+            "name": "genericAttributeList",
             "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+    data_type: Optional[DataTypeFunctionalProfile] = field(
+        default=None,
+        metadata={
+            "name": "dataType",
+            "type": "Element",
+        }
+    )
+    unit: Optional[Units] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    legible_description: List[LegibleDescription] = field(
+        default_factory=list,
+        metadata={
+            "name": "legibleDescription",
+            "type": "Element",
+            "max_occurs": 4,
         }
     )
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/generic/sgr_serial_int_capability.py` & `sgr-lib-0.0.2/sgr_library/generated/generic/sgr_serial_int_capability.py`

 * *Files identical despite different names*

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/product/__init__.py` & `sgr-lib-0.0.2/sgr_library/generated/product/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,66 @@
-from sgr_library.data_classes.product.contact_interface import (
+from sgr_library.generated.product.contact_interface import (
     ContactFunctionalProfile,
     ContactFunctionalProfileList,
     ContactInterface,
     ContactInterfaceDescription,
     ContactsDataPointList,
 )
-from sgr_library.data_classes.product.generic_interface import (
+from sgr_library.generated.product.generic_interface import (
     GenericDataPointList,
     GenericFunctionalProfile,
     GenericFunctionalProfileList,
     GenericInterface,
 )
-from sgr_library.data_classes.product.modbus_interface import (
+from sgr_library.generated.product.modbus_interface import (
     ModbusDataPoint,
     ModbusDataPointList,
     ModbusFunctionalProfile,
     ModbusFunctionalProfileList,
     ModbusInterface,
 )
-from sgr_library.data_classes.product.modbus_types import (
+from sgr_library.generated.product.modbus_types import (
     AccessProtectionEnabled,
     BitOrder,
     MasterFunctionsSupported,
     MasterFunctionsSupportedList,
     ModbusAttributes,
-    ModbusBitmapMapper,
-    ModbusBooleanMapper,
+    ModbusBoolean,
     ModbusDataPointConfiguration,
     ModbusDataType,
-    ModbusEnumMapper,
     ModbusExceptionCode,
     ModbusInterfaceDescription,
     ModbusInterfaceSelection,
     ModbusLayer6Deviation,
     ModbusRtu,
     ModbusTcp,
     RegisterType,
     TimeSyncBlockNotification,
 )
-from sgr_library.data_classes.product.product import (
+from sgr_library.generated.product.product import (
+    ConfigurationDescription,
+    ConfigurationList,
+    ConfigurationListElement,
     DeviceFrame,
     DeviceInformation,
     InterfaceList,
 )
-from sgr_library.data_classes.product.rest_api_interface import (
+from sgr_library.generated.product.rest_api_interface import (
     RestApiDataPoint,
     RestApiDataPointList,
     RestApiFunctionalProfile,
     RestApiFunctionalProfileList,
     RestApiInterface,
 )
-from sgr_library.data_classes.product.rest_api_types import (
+from sgr_library.generated.product.rest_api_types import (
     HeaderEntry,
     HeaderList,
     HttpMethod,
+    JmespathMapping,
+    JmespathMappingRecord,
     ResponseQuery,
     ResponseQueryType,
     RestApiAuthenticationMethod,
     RestApiBasic,
     RestApiBearer,
     RestApiDataPointConfiguration,
     RestApiDataType,
@@ -82,38 +85,41 @@
     "ModbusFunctionalProfileList",
     "ModbusInterface",
     "AccessProtectionEnabled",
     "BitOrder",
     "MasterFunctionsSupported",
     "MasterFunctionsSupportedList",
     "ModbusAttributes",
-    "ModbusBitmapMapper",
-    "ModbusBooleanMapper",
+    "ModbusBoolean",
     "ModbusDataPointConfiguration",
     "ModbusDataType",
-    "ModbusEnumMapper",
     "ModbusExceptionCode",
     "ModbusInterfaceDescription",
     "ModbusInterfaceSelection",
     "ModbusLayer6Deviation",
     "ModbusRtu",
     "ModbusTcp",
     "RegisterType",
     "TimeSyncBlockNotification",
+    "ConfigurationDescription",
+    "ConfigurationList",
+    "ConfigurationListElement",
     "DeviceFrame",
     "DeviceInformation",
     "InterfaceList",
     "RestApiDataPoint",
     "RestApiDataPointList",
     "RestApiFunctionalProfile",
     "RestApiFunctionalProfileList",
     "RestApiInterface",
     "HeaderEntry",
     "HeaderList",
     "HttpMethod",
+    "JmespathMapping",
+    "JmespathMappingRecord",
     "ResponseQuery",
     "ResponseQueryType",
     "RestApiAuthenticationMethod",
     "RestApiBasic",
     "RestApiBearer",
     "RestApiDataPointConfiguration",
     "RestApiDataType",
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/product/contact_interface.py` & `sgr-lib-0.0.2/sgr_library/generated/product/contact_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass, field
 from typing import List, Optional
-from sgr_library.data_classes.generic.data_point import DataPointBase
-from sgr_library.data_classes.generic.functional_profile import FunctionalProfileBase
+from sgr_library.generated.generic.data_point import DataPointBase
+from sgr_library.generated.generic.functional_profile import FunctionalProfileBase
 
 __NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
 
 
 @dataclass
 class ContactInterfaceDescription:
     """
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/product/generic_interface.py` & `sgr-lib-0.0.2/sgr_library/generated/communicator/communicator_frame.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,61 @@
 from dataclasses import dataclass, field
 from typing import List, Optional
-from sgr_library.data_classes.generic.data_point import DataPointBase
-from sgr_library.data_classes.generic.functional_profile import FunctionalProfileBase
+from sgr_library.generated.communicator.communicator_types import CommunicatorBase
+from sgr_library.generated.generic.base_types import GenericAttributeListFunctionalProfile
+from sgr_library.generated.generic.data_point import DataPointBase
+from sgr_library.generated.generic.functional_profile import FunctionalProfileDescription
 
 __NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
 
 
 @dataclass
-class GenericDataPointList:
+class CommunicatorFunctionalProfile(FunctionalProfileDescription):
     """
-    List of data points.
+    Extends the base functional profile type with generic data points.
     """
-    data_point_list_element: List[DataPointBase] = field(
-        default_factory=list,
+    generic_attribute_list: Optional[GenericAttributeListFunctionalProfile] = field(
+        default=None,
         metadata={
-            "name": "dataPointListElement",
+            "name": "genericAttributeList",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "min_occurs": 1,
         }
     )
-
-
-@dataclass
-class GenericFunctionalProfile(FunctionalProfileBase):
-    data_point_list: Optional[GenericDataPointList] = field(
-        default=None,
+    data_point_list_element: List[DataPointBase] = field(
+        default_factory=list,
         metadata={
-            "name": "dataPointList",
+            "name": "dataPointListElement",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
+            "min_occurs": 1,
         }
     )
 
 
 @dataclass
-class GenericFunctionalProfileList:
+class CommunicatorFrame1(CommunicatorBase):
     """
-    List of functional profiles.
+    Data type definition for a Communicator Description.
     """
-    functional_profile_list_element: List[GenericFunctionalProfile] = field(
+    class Meta:
+        name = "CommunicatorFrame"
+
+    functional_profile_list_element: List[CommunicatorFunctionalProfile] = field(
         default_factory=list,
         metadata={
             "name": "functionalProfileListElement",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "min_occurs": 1,
         }
     )
 
 
 @dataclass
-class GenericInterface:
+class CommunicatorFrame(CommunicatorFrame1):
     """
-    Container for a device without supported transport service.
+    RPT Root Point for Communicator.
     """
-    functional_profile_list: Optional[GenericFunctionalProfileList] = field(
-        default=None,
-        metadata={
-            "name": "functionalProfileList",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
-        }
-    )
+    class Meta:
+        name = "communicatorFrame"
+        namespace = "http://www.smartgridready.com/ns/V0/"
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/product/modbus_interface.py` & `sgr-lib-0.0.2/sgr_library/generated/product/modbus_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from typing import List, Optional
-from sgr_library.data_classes.generic.data_point import DataPointBase
-from sgr_library.data_classes.generic.functional_profile import FunctionalProfileBase
-from sgr_library.data_classes.product.modbus_types import (
+from sgr_library.generated.generic.data_point import DataPointBase
+from sgr_library.generated.generic.functional_profile import FunctionalProfileBase
+from sgr_library.generated.product.modbus_types import (
     ModbusAttributes,
     ModbusDataPointConfiguration,
     ModbusInterfaceDescription,
     TimeSyncBlockNotification,
 )
 
 __NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
@@ -22,15 +22,14 @@
     """
     modbus_data_point_configuration: Optional[ModbusDataPointConfiguration] = field(
         default=None,
         metadata={
             "name": "modbusDataPointConfiguration",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
         }
     )
     block_cache_identification: Optional[str] = field(
         default=None,
         metadata={
             "name": "blockCacheIdentification",
             "type": "Element",
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/product/modbus_types.py` & `sgr-lib-0.0.2/sgr_library/generated/product/modbus_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import List, Optional
-from sgr_library.data_classes.generic.base_types import (
+from sgr_library.generated.generic.base_types import (
     BitmapProduct,
     EmptyType,
     EnumType,
     ScalingFactor,
 )
-from sgr_library.data_classes.generic.sgr_serial_int_capability import (
+from sgr_library.generated.generic.sgr_serial_int_capability import (
     BaudRate,
     ByteLength,
     Parity,
     SerialInterfaceCapability,
     StopBitLength,
 )
 
@@ -91,93 +91,32 @@
     GET_COM_EVENT_COUNTER = "GetComEventCounter"
     GET_COM_EVENT_LOG = "GetComEventLog"
     REPORT_SLAVE_ID = "ReportSlaveID"
     READ_DEVICE_IDENTIFICATION = "ReadDeviceIdentification"
 
 
 @dataclass
-class ModbusBitmapMapper:
-    """Bitmaps typically define operation modes or parallel active states.
-
-    Devices use different control schemes, SmartGridrady defines a
-    commmon information model for interoperable behaviour. At interface
-    class level, Bitmaps may use different binary values.
+class ModbusBoolean:
     """
-    modbus_bit_mapper: List[int] = field(
-        default_factory=list,
-        metadata={
-            "name": "modbusBitMapper",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "min_occurs": 1,
-        }
-    )
-    generic_bit_mapper: List[int] = field(
-        default_factory=list,
-        metadata={
-            "name": "genericBitMapper",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "min_occurs": 1,
-        }
-    )
-
-
-@dataclass
-class ModbusBooleanMapper:
-    """Booleans at modbus level may be true if 1, 0, 0xff, -1 , all but not a
-    certain value .
-
-    isPositiveLogic is true if a number must contain a specific value to
-    be valid isPositiveLogic is false if a number must contain any but
-    NOT a specific value to be valid
+    Modbus specific boolean definition.
     """
-    is_positive_logic: Optional[bool] = field(
+    true_value: Optional[int] = field(
         default=None,
         metadata={
-            "name": "isPositiveLogic",
+            "name": "trueValue",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
         }
     )
-    value: Optional[int] = field(
+    false_value: Optional[int] = field(
         default=None,
         metadata={
+            "name": "falseValue",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
-        }
-    )
-
-
-@dataclass
-class ModbusEnumMapper:
-    """Enumerations typically define operation modes or singlular states.
-
-    Devices use different control schemes, SmartGridrady defines a
-    commmon information model for interoperable behaviour. At interface
-    class level, enums may use different binary values.
-    """
-    modbus_enum_mapper: List[int] = field(
-        default_factory=list,
-        metadata={
-            "name": "modbusEnumMapper",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "min_occurs": 1,
-        }
-    )
-    gen_enum_mapper: List[int] = field(
-        default_factory=list,
-        metadata={
-            "name": "genEnumMapper",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-            "min_occurs": 1,
         }
     )
 
 
 class ModbusExceptionCode(Enum):
     """
     Type of the Modbus Exceptions sent by Slave (Server) responses.
@@ -242,24 +181,17 @@
 
     :cvar VALUE_2_REG_BASE1000_L2_H: 2 Registers show a combined value,
         as example in kWh and MWh beginning with lower range @ lower
         address
     :cvar VALUE_2_REG_BASE1000_H2_L: 2 Registers show a combined value,
         as example in kWh and MWh beginning with lower range @ higher
         address
-    :cvar SGREADY_ENUM2_IO_H2_L: 2 Registers combine SGready IO1 and IO2
-        into the sgreadyStateLv2 enum beginning with IO1 @ higher
-        address
-    :cvar SGREADY_ENUM2_IO_L2_H: 2 Registers combine SGready IO1 and IO2
-        into the sgreadyStateLv2 enum beginning with IO1 @ lower address
     """
     VALUE_2_REG_BASE1000_L2_H = "2RegBase1000_L2H"
     VALUE_2_REG_BASE1000_H2_L = "2RegBase1000_H2L"
-    SGREADY_ENUM2_IO_H2_L = "SGReadyEnum2IO_H2L"
-    SGREADY_ENUM2_IO_L2_H = "SGReadyEnum2IO_L2H"
 
 
 @dataclass
 class ModbusTcp:
     """Modbus IP address:Specific P elements for Modbus over IP protocol.
 
     This definition is partially inherited from 61850-80-5's
@@ -276,15 +208,15 @@
     )
     address: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "required": True,
-            "pattern": r"\d+\.\d+\.\d+\.\d+",
+            "pattern": r"\d+\.\d+\.\d+\.\d+|\{\{.*\}\}",
         }
     )
     slave_id: Optional[int] = field(
         default=None,
         metadata={
             "name": "slaveId",
             "type": "Element",
@@ -363,15 +295,15 @@
 
 
 @dataclass
 class ModbusDataType:
     """
     Modbus specific data types.
     """
-    boolean: Optional[EmptyType] = field(
+    boolean: Optional[ModbusBoolean] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
     int8: Optional[EmptyType] = field(
@@ -610,17 +542,14 @@
         +10) generic value = dataPoint * 10^p note: Sunspec uses sunssf
         usually as Modbus Register with dynamic values check attribute
         "timeAlignedNotification"
     :ivar polling_latency_ms: The time for a master slave communication
         cycle in ms
     :ivar access_protection:
     :ivar layer6_deviation:
-    :ivar iop_enum_mapper:
-    :ivar iop_bitmap_mapper:
-    :ivar iop_boolean_mapper:
     """
     scaling_factor: Optional[ScalingFactor] = field(
         default=None,
         metadata={
             "name": "scalingFactor",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
@@ -661,38 +590,14 @@
         default=None,
         metadata={
             "name": "layer6Deviation",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    iop_enum_mapper: Optional[ModbusEnumMapper] = field(
-        default=None,
-        metadata={
-            "name": "iopEnumMapper",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-        }
-    )
-    iop_bitmap_mapper: Optional[ModbusBitmapMapper] = field(
-        default=None,
-        metadata={
-            "name": "iopBitmapMapper",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-        }
-    )
-    iop_boolean_mapper: Optional[ModbusBooleanMapper] = field(
-        default=None,
-        metadata={
-            "name": "iopBooleanMapper",
-            "type": "Element",
-            "namespace": "http://www.smartgridready.com/ns/V0/",
-        }
-    )
 
 
 @dataclass
 class ModbusDataPointConfiguration:
     """
     Detailed configuration for modbus data point.
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/product/product.py` & `sgr-lib-0.0.2/sgr_library/generated/product/product.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 from dataclasses import dataclass, field
 from typing import List, Optional
-from sgr_library.data_classes.generic.base_type_level_of_operation_type import LevelOfOperation
-from sgr_library.data_classes.generic.base_types import (
+from sgr_library.generated.generic.base_type_level_of_operation_type import LevelOfOperation
+from sgr_library.generated.generic.base_types import (
     AlternativeNames,
+    DataTypeProduct,
     DeviceCategory,
-    GenericAttributes,
+    GenericAttributeListProduct,
     LegibleDescription,
     PowerSource,
     ReleaseNotes,
+    VersionNumber,
 )
-from sgr_library.data_classes.product.contact_interface import ContactInterface
-from sgr_library.data_classes.product.modbus_interface import ModbusInterface
-from sgr_library.data_classes.product.rest_api_interface import RestApiInterface
+from sgr_library.generated.product.contact_interface import ContactInterface
+from sgr_library.generated.product.generic_interface import GenericInterface
+from sgr_library.generated.product.modbus_interface import ModbusInterface
+from sgr_library.generated.product.rest_api_interface import RestApiInterface
 
 __NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
 
 
 @dataclass
+class ConfigurationDescription(LegibleDescription):
+    label: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+
+
+@dataclass
 class DeviceInformation:
     """
     :ivar alternative_names:
     :ivar legible_description: Published and printable information
         related to this product
     :ivar device_category:
     :ivar is_local_control: Value "false" means "is cloud control
@@ -30,21 +44,22 @@
     :ivar software_revision: software version information for this
         product declaration
     :ivar hardware_revision: hardware version information for this
         product declaration
     :ivar brand_name: branding information
     :ivar power_source: power supply type
     :ivar nominal_power: nominal Power of the device (installation)
-    :ivar manufacturer_specification_identification: manufacurers
+    :ivar manufacturer_specification_identification: manufacturers
         specification identifier
     :ivar manufacturer_label: manufacturers label of the device
     :ivar general_remarks: author of this sheet may add remarks / non
         disclaimer statements
     :ivar level_of_operation: defines the SGr Label Level 1...6 of the
         highest level functional profile of this device
+    :ivar version_number:
     :ivar programmer_hints: additional device-specific implementation
         hints for this device
     """
     alternative_names: Optional[AlternativeNames] = field(
         default=None,
         metadata={
             "name": "alternativeNames",
@@ -147,14 +162,22 @@
         default=None,
         metadata={
             "name": "levelOfOperation",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
+    version_number: Optional[VersionNumber] = field(
+        default=None,
+        metadata={
+            "name": "versionNumber",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
     programmer_hints: List[LegibleDescription] = field(
         default_factory=list,
         metadata={
             "name": "programmerHints",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
             "max_occurs": 4,
@@ -187,35 +210,79 @@
         default=None,
         metadata={
             "name": "contactInterface",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
-    generic_interface: Optional[str] = field(
+    generic_interface: Optional[GenericInterface] = field(
         default=None,
         metadata={
             "name": "genericInterface",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
 
 
 @dataclass
+class ConfigurationListElement:
+    name: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+    data_type: Optional[DataTypeProduct] = field(
+        default=None,
+        metadata={
+            "name": "dataType",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+    configuration_description: List[ConfigurationDescription] = field(
+        default_factory=list,
+        metadata={
+            "name": "configurationDescription",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "max_occurs": 4,
+        }
+    )
+
+
+@dataclass
+class ConfigurationList:
+    configuration_list_element: List[ConfigurationListElement] = field(
+        default_factory=list,
+        metadata={
+            "name": "configurationListElement",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "min_occurs": 1,
+        }
+    )
+
+
+@dataclass
 class DeviceFrame:
     """
     Product declaration.
 
     :ivar device_name: Device Name in the context of the manufacturer
     :ivar manufacturer_name: Name of the Manufacturer or OEM
     :ivar specification_owner_identification:
     :ivar release_notes:
     :ivar device_information:
-    :ivar generic_attributes:
+    :ivar configuration_list:
+    :ivar generic_attribute_list:
     :ivar interface_list:
     """
     class Meta:
         namespace = "http://www.smartgridready.com/ns/V0/"
 
     device_name: Optional[str] = field(
         default=None,
@@ -252,18 +319,25 @@
         default=None,
         metadata={
             "name": "deviceInformation",
             "type": "Element",
             "required": True,
         }
     )
-    generic_attributes: Optional[GenericAttributes] = field(
+    configuration_list: Optional[ConfigurationList] = field(
+        default=None,
+        metadata={
+            "name": "configurationList",
+            "type": "Element",
+        }
+    )
+    generic_attribute_list: Optional[GenericAttributeListProduct] = field(
         default=None,
         metadata={
-            "name": "genericAttributes",
+            "name": "genericAttributeList",
             "type": "Element",
         }
     )
     interface_list: Optional[InterfaceList] = field(
         default=None,
         metadata={
             "name": "interfaceList",
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/product/rest_api_interface.py` & `sgr-lib-0.0.2/sgr_library/generated/product/rest_api_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from typing import List, Optional
-from sgr_library.data_classes.generic.data_point import DataPointBase
-from sgr_library.data_classes.generic.functional_profile import FunctionalProfileBase
-from sgr_library.data_classes.product.rest_api_types import (
+from sgr_library.generated.generic.data_point import DataPointBase
+from sgr_library.generated.generic.functional_profile import FunctionalProfileBase
+from sgr_library.generated.product.rest_api_types import (
     RestApiDataPointConfiguration,
     RestApiInterfaceDescription,
 )
 
 __NAMESPACE__ = "http://www.smartgridready.com/ns/V0/"
 
 
@@ -14,15 +14,14 @@
 class RestApiDataPoint(DataPointBase):
     rest_api_data_point_configuration: Optional[RestApiDataPointConfiguration] = field(
         default=None,
         metadata={
             "name": "restApiDataPointConfiguration",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
         }
     )
 
 
 @dataclass
 class RestApiDataPointList:
     """
```

### Comparing `sgr-lib-0.0.1/sgr_library/data_classes/product/rest_api_types.py` & `sgr-lib-0.0.2/sgr_library/generated/product/rest_api_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,18 +30,50 @@
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
     PATCH = "PATCH"
     DELETE = "DELETE"
 
 
+@dataclass
+class JmespathMappingRecord:
+    class Meta:
+        name = "JMESPathMappingRecord"
+
+    from_value: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "from",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+    to: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "required": True,
+        }
+    )
+    name: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+        }
+    )
+
+
 class ResponseQueryType(Enum):
     JMESPATH_EXPRESSION = "JMESPathExpression"
     XPATH_EXPRESSION = "XPathExpression"
     REGULAR_EXPRESSION = "RegularExpression"
+    JMESPATH_MAPPING = "JMESPathMapping"
 
 
 class RestApiAuthenticationMethod(Enum):
     NO_SECURITY_SCHEME = "NoSecurityScheme"
     BEARER_SECURITY_SCHEME = "BearerSecurityScheme"
     API_KEY_SECURITY_SCHEME = "ApiKeySecurityScheme"
     BASIC_SECURITY_SCHEME = "BasicSecurityScheme"
@@ -106,14 +138,29 @@
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
 
 
 @dataclass
+class JmespathMapping:
+    class Meta:
+        name = "JMESPathMapping"
+
+    mapping: List[JmespathMappingRecord] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
+            "min_occurs": 1,
+        }
+    )
+
+
+@dataclass
 class ResponseQuery:
     query_type: Optional[ResponseQueryType] = field(
         default=None,
         metadata={
             "name": "queryType",
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
@@ -121,15 +168,22 @@
         }
     )
     query: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.smartgridready.com/ns/V0/",
-            "required": True,
+        }
+    )
+    jmes_path_mappings: Optional[JmespathMapping] = field(
+        default=None,
+        metadata={
+            "name": "jmesPathMappings",
+            "type": "Element",
+            "namespace": "http://www.smartgridready.com/ns/V0/",
         }
     )
 
 
 @dataclass
 class RestApiServiceCall:
     request_header: Optional[HeaderList] = field(
```

### Comparing `sgr-lib-0.0.1/sgr_library/exceptions.py` & `sgr-lib-0.0.2/sgr_library/exceptions.py`

 * *Files identical despite different names*

### Comparing `sgr-lib-0.0.1/sgr_library/modbusRTU_client.py` & `sgr-lib-0.0.2/sgr_library/modbusRTU_client.py`

 * *Files identical despite different names*

### Comparing `sgr-lib-0.0.1/sgr_library/modbusRTU_client_async.py` & `sgr-lib-0.0.2/sgr_library/modbusRTU_client_async.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,85 @@
-import asyncio
-
-from sgr_library.payload_decoder import PayloadDecoder, PayloadBuilder
-from pymodbus.constants import Endian
-from pymodbus.client import AsyncModbusSerialClient, ModbusSerialClient
-
-# In this case establishes a connection with the localhost server that is running the simulation.
-
-class SGrModbusRTUClient:
-
-    def __init__(self, port: str, parity: str, baudrate: int, client=None):
-        """
-        Creates client
-        :param ip: The host to connect to (default 127.0.0.1)
-        :param port: The modbus port to connect to (default 502)
-        """
-        if client is not None:
-            self.client = client
-        else:
-            self.client = AsyncModbusSerialClient(method="rtu", port=port, parity=parity, baudrate=baudrate) #changed source: https://stackoverflow.com/questions/58773476/why-do-i-get-pymodbus-modbusioexception-on-20-of-attempts
-
-            connected = self.client.connect() #TODO a wrapper that opens and closes connection when function is excecuted?
-            if connected:
-                print("Connected to ModbusRTU ond Port: " + port)
-
-    #not changed
-    async def value_decoder(self, addr: int, size: int, data_type: str, register_type: str, slave_id: int, order: Endian) -> float:
-        """
-        Reads register and decodes the value.
-        :param addr: The address to read from and decode
-        :param size: The number of registers to read
-        :param data_type: The modbus type to decode
-        :returns: Decoded float
-        """
-        if register_type == "HoldRegister": #Todo im Modbus_client ist "HoldingRegister" angeben, ist das falsch?
-            reg = await self.client.read_holding_registers(addr, count=size, slave=slave_id)
-            #print(reg.registers)
-        else:
-            reg = await self.client.read_input_registers(addr, count=size, slave=slave_id)
-        decoder = PayloadDecoder.fromRegisters(reg.registers, byteorder=order, wordorder=order)
-        
-        if not reg.isError():
-            return decoder.decode(data_type, 0)
-    #not changed
-    async def value_encoder(self, addr: int, value: float, data_type: str, slave_id: int, order: Endian):
-        """
-        Encodes value to be set on the register address
-        :param addr: The address to read from and decode
-        :param value: The value to be written on the register
-        :param data_type: The modbus type to decode
-        """
-        builder = PayloadBuilder(byteorder=order, wordorder=order)
-        builder.encode(value, data_type, rounding="floor")
-        await self.client.write_registers(address=addr, values=builder.to_registers(), unit=slave_id)
-
-if __name__ == "__main__":
-
-    async def run():
-        MyClient = SGrModbusRTUClient("COM5", "E", 19200)
-
-        connected = await MyClient.client.connect()
-
-        a = await MyClient.value_decoder(0x5B14,2,"int32","HoldRegister",slave_id=1, order=Endian.Big)
-        print (f"Der Wert ist: {a}")
-        await MyClient.client.close()
-
-    asyncio.run(run())
-
+import asyncio
+
+from pymodbus.client import AsyncModbusSerialClient
+from pymodbus.constants import Endian
+
+from sgr_library.payload_decoder import PayloadDecoder, PayloadBuilder, RoundingScheme
+
+
+# In this case establishes a connection with the localhost server that is running the simulation.
+
+class SGrModbusRTUClient:
+
+    def __init__(self, port: str, parity: str, baudrate: int, client=None):
+        """
+        Creates client
+        :param ip: The host to connect to (default 127.0.0.1)
+        :param port: The modbus port to connect to (default 502)
+        """
+        self._port = port
+        self._semaphore = asyncio.Semaphore(1)
+        if client is not None:
+            self.client = client
+        else:
+            self.client = AsyncModbusSerialClient(
+                method="rtu",
+                port=port,
+                parity=parity,
+                baudrate=baudrate,
+            )  # changed source: https://stackoverflow.com/questions/58773476/why-do-i-get-pymodbus-modbusioexception-on-20-of-attempts
+
+            # connected = self.client.connect() #TODO a wrapper that opens and closes connection when function is excecuted?
+            # if connected:
+            #     print("Connected to ModbusRTU ond Port: " + port)
+
+    async def connect(self):
+        await self.client.connect()
+        print("Connected to ModbusRTU ond Port: " + self._port)
+
+    # not changed
+    async def value_decoder(self, addr: int, size: int, data_type: str, register_type: str, slave_id: int,
+                            order: Endian) -> float:
+        """
+        Reads register and decodes the value.
+        :param addr: The address to read from and decode
+        :param size: The number of registers to read
+        :param data_type: The modbus type to decode
+        :returns: Decoded float
+        """
+        async with self._semaphore:
+            if register_type == "HoldRegister":  # Todo im Modbus_client ist "HoldingRegister" angeben, ist das falsch?
+                reg = await self.client.read_holding_registers(addr, count=size, slave=slave_id)
+                # print(reg.registers)
+            else:
+                reg = await self.client.read_input_registers(addr, count=size, slave=slave_id)
+            decoder = PayloadDecoder.fromRegisters(reg.registers, byteorder=order, wordorder=order)
+
+            if not reg.isError():
+                return decoder.decode(data_type, 0)
+
+    # not changed
+    async def value_encoder(self, addr: int, value: float, data_type: str, slave_id: int, order: Endian):
+        """
+        Encodes value to be set on the register address
+        :param addr: The address to read from and decode
+        :param value: The value to be written on the register
+        :param data_type: The modbus type to decode
+        """
+        async with self._semaphore:
+            builder = PayloadBuilder(byteorder=order, wordorder=order)
+            builder.encode(value, data_type, rounding=RoundingScheme.floor)
+            await self.client.write_registers(address=addr, values=builder.to_registers(), unit=slave_id)
+
+
+if __name__ == "__main__":
+    async def run():
+        MyClient = SGrModbusRTUClient("COM5", "E", 19200)
+
+        connected = await MyClient.client.connect()
+
+        a = await MyClient.value_decoder(0x5B14, 2, "int32", "HoldRegister", slave_id=1, order=Endian.BIG)
+        print(f"Der Wert ist: {a}")
+        await MyClient.client.close()
+
+
+    asyncio.run(run())
```

### Comparing `sgr-lib-0.0.1/sgr_library/modbus_client.py` & `sgr-lib-0.0.2/sgr_library/modbus_client.py`

 * *Files identical despite different names*

### Comparing `sgr-lib-0.0.1/sgr_library/modbus_interface.py` & `sgr-lib-0.0.2/sgr_library/modbusRTU_interface_async.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,309 +1,346 @@
+import logging
+import os
+from dataclasses import dataclass
+from typing import Optional, Tuple, Dict, Any, Iterable
+from pymodbus.constants import Endian
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.context import XmlContext
 import time
-from sgr_library.exceptions import DataPointException, FunctionalProfileException, DataProcessingError, DeviceInformationError, InvalidEndianType
-from pymodbus.exceptions import ConnectionException
-from aiohttp import ClientError
-
-#from sgr_library.data_classes.ei_modbus import SgrModbusDeviceFrame
-#from sgr_library.data_classes.ei_modbus.sgr_modbus_eidevice_frame import SgrModbusDataPointType
-
-from sgr_library.data_classes.product import DeviceFrame
-from sgr_library.auxiliary_functions import get_address, get_endian, get_port, get_slave
-
-from sgr_library.modbus_client import SGrModbusClient
-# from auxiliary_functions import find_dp
-import asyncio
 
-import logging
+from sgr_library.api import BaseSGrInterface, DeviceInformation, FunctionProfile, DataPointProtocol, DataPoint, \
+    build_configurations_parameters, ConfigurationParameter
+from sgr_library.auxiliary_functions import find_dp
+from sgr_library.converters import build_converter
+from sgr_library.generated.generic import Parity, DataDirectionProduct
+
+# from sgr_library.data_classes.ei_modbus import SgrModbusDeviceDescriptionType
+from sgr_library.generated.product import DeviceFrame, ModbusDataPoint, ModbusFunctionalProfile
+
+from sgr_library.modbusRTU_client_async import SGrModbusRTUClient
+from sgr_library.validators import build_validator
+
+
+def get_port(root) -> str:
+    """
+    :param root: The root element created with the xsdata parser
+    :returns: string with port from xml file.
+    """
+    return (str(root.modbus_interface_desc.trsp_srv_modbus_tcpout_of_box.port))
+    # return(str(root.modbus_interface_desc.trspSrvModbusRTUoutOfBox.port)) #TODO Port datapoint for RTU in XML is not existing
+
+
+def get_slave(root) -> int:
+    """
+    returns the selected slave address
+    """
+    return root.interface_list.modbus_interface.modbus_interface_description.modbus_rtu.slave_addr
+
+
+def get_endian(root) -> Endian:
+    return Endian.BIG
+
+
+def get_baudrate(root) -> int:
+    """
+    returns the selected baudrate. Implemented for Even
+    """
+    return root.interface_list.modbus_interface.modbus_interface_description.modbus_rtu.baud_rate_selected.value
+
+
+def get_parity(root) -> str:
+    """
+    returns the parity. Implemented for Even
+    """
+    parity = root.interface_list.modbus_interface.modbus_interface_description.modbus_rtu.parity_selected
+    match parity:
+        case Parity.EVEN:
+            return 'E'
+        case _:
+            raise NotImplementedError
+
+
+def build_modbus_rtu_data_point(data_point: ModbusDataPoint, function_profile: ModbusFunctionalProfile,
+                                interface: 'SgrModbusRtuInterface') -> DataPoint:
+    protocol = ModBusRTUDataPoint(data_point, function_profile, interface)
+    converter = build_converter(data_point.data_point.unit)
+    validator = build_validator(data_point.data_point.data_type)
+    return DataPoint(protocol, converter, validator)
+
+
+class ModBusRTUDataPoint(DataPointProtocol):
+
+    def __init__(self, modbus_api_dp: ModbusDataPoint, modbus_api_fp: ModbusFunctionalProfile,
+                 interface: 'SgrModbusRtuInterface'):
+        self._dp = modbus_api_dp
+        self._fp = modbus_api_fp
+        self._interface = interface
+
+    async def write(self, data: Any):
+        return await self._interface.setval(self.name()[0], self.name()[1], data)
+
+    async def read(self) -> Any:
+        return await self._interface.getval(self.name()[0], self.name()[1])
+
+    def name(self) -> tuple[str, str]:
+        return self._fp.functional_profile.functional_profile_name, self._dp.data_point.data_point_name
+
+    def direction(self) -> DataDirectionProduct:
+        return self._dp.data_point.data_direction
 
-logging.basicConfig(level=logging.ERROR)
-logger = logging.getLogger(__name__)
 
-class SgrModbusInterface: 
+class ModBusRTUFunctionProfile(FunctionProfile):
 
-    def __init__(self, xml_file: str) -> None:
+    def __init__(self, modbus_api_fp: ModbusFunctionalProfile, interface: 'SgrModbusRtuInterface'):
+        self._fp = modbus_api_fp
+        self._interface = interface
+        dps = [build_modbus_rtu_data_point(dp, self._fp, self._interface) for dp in
+               self._fp.data_point_list.data_point_list_element]
+        self._data_points = {dp.name(): dp for dp in dps}
+
+    def name(self) -> str:
+        return self._fp.functional_profile.functional_profile_name
+
+    def get_data_points(self) -> dict[tuple[str, str], DataPoint]:
+        return self._data_points
+
+
+class SgrModbusRtuInterface(BaseSGrInterface):
+    # a global Modbus client
+    globalModbusRTUClient = None
+
+    def __init__(self, frame: DeviceFrame) -> None:
         """
         Creates a connection from xml file data.
         Parses the xml file with xsdata library.
         :param xml_file: Name of the xml file to parse
         """
-        print('I Have been created!')
-        self.parser = XmlParser(context=XmlContext())
-        self.root = self.parser.parse(xml_file, DeviceFrame)
-        self.ip = get_address(self.root)
-        self.port = get_port(self.root)
-        self.client = SGrModbusClient(self.ip, self.port)
+        self.root = frame
+        # self.root = parser.parse(interface_file, SgrModbusDeviceDescriptionType)
+        self.port = os.getenv("SGR_RTU_PORT")  # get_port(self.root) #TODO überlegungen machen wo Port untergebracht wird
+        self._configurations_params = build_configurations_parameters(frame.configuration_list)
+        self.baudrate = get_baudrate(self.root)
+        self.parity = get_parity(self.root)
         self.slave_id = get_slave(self.root)
         self.byte_order = get_endian(self.root)
-        # A dictionary where we cash the value of the datapoint. With name, value, timestamp and alive_time? ;)
-        self.cash_dict = {}
-        
-    async def connect(self):
-        try:
-            await self.client.client.connect()
-            logger.info("Connected successfully.")
-        except ConnectionException as e:
-            logger.error(f"ConnectionException: Failed to connect: {e}")
-        except TimeoutError as e:
-            logger.error(f"TimeoutError: Connection timed out: {e}")
-        except Exception as e:
-            logger.exception(f"An unexpected error occurred during the connection: {e}")
+        fps = [ModBusRTUFunctionProfile(profile, self) for profile in
+               self.root.interface_list.modbus_interface.functional_profile_list.functional_profile_list_element]
+        self._function_profiles = {fp.name(): fp for fp in fps}
+        self._device_information = DeviceInformation(
+            name=frame.device_name,
+            manufacture=frame.manufacturer_name,
+            software_revision=frame.device_information.software_revision,
+            hardware_revision=frame.device_information.hardware_revision,
+            device_category=frame.device_information.device_category,
+            is_local=frame.device_information.is_local_control
+        )
 
+    def get_pymodbus_client(self):
+        """
+        returns the pymodbus client object
+        """
+        return self.client.client
+
+    # TODO
+    def get_dp_attribute(self, datapoint: str, attribute: str):
+        """
+        Searches for a specific attribute in the datapoint via a key.
+        :param attribute"address", "size", "bitrank", "data_type", "register_type", "unit", "multiplicator", "power_of", "name"
+        :returns: The chosen attribute.
+        """
+        # TODO
+        ...
 
-    async def getval(self, fp_name, dp_name) -> float:
+    # TODO assign multiple dispatch to the function.
+    '''def getval(self, fp_name: str, dp_name: str) -> float:
+        """
+        Reads datapoint value.
+        :param fp_name: The name of the funcitonal profile in which the datapoint resides.
+        :param dp_name: The name of the datapoint.
+        :returns: The current decoded value in the datapoint register.
+        """
+        dp = find_dp(self.root, fp_name, dp_name)
+        address = self.get_address(dp)
+        size = self.get_size(dp)
+        data_type = self.get_datatype(dp)
+        reg_type = self.get_register_type(dp)
+        return self.client.value_decoder(address, size, data_type, reg_type)'''
+
+    # getval with multiple dispatching
+    async def getval(self, *parameter) -> float:
         """
         Reads datapoint value.
 
         :dp: The already obtained datapoint object
 
         2 parameters alternative:
         :param fp_name: The name of the functional profile in which the datapoint resides.
         :param dp_name: The name of the datapoint.
 
         :returns: The current decoded value in the datapoint register.
         """
-            
-        try:
-            dp = self.find_dp(self.root, fp_name, dp_name)
-        except DataPointException as e:
-            logger.error(e)
-            return float('nan')
-        except FunctionalProfileException as e:
-            logger.warning(e)
-            return float('nan')
-
-        try:
-            address = self.get_address(dp)
-            size = self.get_size(dp)
-            data_type = self.get_datatype(dp)
-            reg_type = self.get_register_type(dp)
-            slave_id = self.slave_id
-            order = self.byte_order
-            answer = await self.client.value_decoder(address, size, data_type, reg_type, slave_id, order)
-            return answer
-        except ClientError as e:
-            logger.exception(e)
-            return float('nan')
-
-
-    # TODO under construction
-    async def getval_block(self, fp_name: str, dp_name: str):
-        try:
-            dp = self.find_dp(self.root, fp_name, dp_name)
-        except DataPointException as e:
-            logger.error(f"DataPointException: {e}")
-            return None
-        except FunctionalProfileException as e:
-            logger.warning(f"FunctionalProfileException: {e}")
-            return None
-
-        try:
-            address = self.get_address(dp)
-            size = self.get_size(dp)
-            data_type = self.get_datatype(dp)
-            reg_type = self.get_register_type(dp)
-            slave_id = self.slave_id
-            order = self.byte_order
-            answer = await self.client.mult_value_decoder(address, size, data_type, reg_type, slave_id, order)
-            return answer
-        except ClientError as e:
-            logger.exception(f"ClientError: Failed to retrieve value block {e}")
-            return None
-        except Exception as e:
-            logger.exception(f"An unexpected error occurred: {e}")
-            return None
-
+        if len(parameter) == 2:
+            dp = find_dp(self.root, parameter[0], parameter[1])
+        else:
+            dp = parameter[0]
+        address = self.get_address(dp)
+        size = self.get_size(dp)
+        data_type = self.get_datatype(dp)
+        reg_type = self.get_register_type(dp)
+        slave_id = self.slave_id
+        order = self.byte_order
+
+        logging.debug(
+            f"getVal() with address: {address}, size: {size}, data_type:{data_type}, slave_id: {slave_id}, order: {order}")  # for debugging
+        return await self.client.value_decoder(address, size, data_type, reg_type, slave_id, order)
 
     async def setval(self, fp_name: str, dp_name: str, value: float) -> None:
-        try:
-            dp = self.find_dp(self.root, fp_name, dp_name)
-        except DataPointException as e:
-            logger.error(f"DataPointException: {e}")
-            return
-        except FunctionalProfileException as e:
-            logger.warning(f"FunctionalProfileException: {e}")
-            return
-
-        try:
-            address = self.get_address(dp)
-            data_type = self.get_datatype(dp)
-            slave_id = self.slave_id
-            order = self.byte_order
-            await self.client.value_encoder(address, value, data_type, slave_id, order)
-            logger.info(f"Value {value} has been set for {dp_name} in {fp_name}")
-        except ClientError as e:
-            logger.exception(f"ClientError: Failed to set value {e}")
-        except ValueError as e:
-            logger.error(f"ValueError: Invalid value or datatype {e}")
-        except Exception as e:
-            logger.exception(f"An unexpected error occurred: {e}")
-    
-    
+        """
+        Writes datapoint value.
+        :param fp_name: The name of the funcitonal profile in which the datapoint resides.
+        :param dp_name: The name of the datapoint.
+        :param value: The value that is to be written on the datapoint.
+        """
+        dp: ModbusDataPoint = find_dp(self.root, fp_name, dp_name)
+        address = self.get_address(dp)
+        data_type = self.get_datatype(dp)
+        slave_id = self.slave_id
+        order = self.byte_order
+        await self.client.value_encoder(address, value, data_type, slave_id, order)
+
     def get_device_profile(self):
-        try:
-            brand_name = self.root.device_information.brand_name
-            nominal_power = self.root.device_information.nominal_power
-            level_of_operation = self.root.device_information.legible_description
-            
-            if None in [brand_name, nominal_power, level_of_operation]:
-                raise DeviceInformationError("Incomplete device information")
-            
-            logger.info(f"Brand Name: {brand_name}")
-            logger.info(f"Nominal Power: {nominal_power}")
-            logger.info(f"Level of Operation: {level_of_operation}")
-
-            return self.root.device_information
-            
-        except AttributeError as e:
-            logger.error(f"AttributeError: {e}")
-            return None
-        except DeviceInformationError as e:
-            logger.error(f"DeviceInformationError: {e}")
-            return None
+        return (self.root.device_profile)
 
-    def get_register_type(self, dp) -> str:
+    def get_register_type(self, dp: ModbusDataPoint) -> str:
         """
         Returns register type E.g. "HoldRegister"
         :param fp_name: The name of the functional profile
         :param dp_name: The name of the data point.
-        :returns: The type of the register 
+        :returns: The type of the register
         """
-        try:
-            register_type = dp.modbus_data_point_configuration.register_type.value
-            if register_type is None:
-                raise DataProcessingError("Register type is None")
-            return register_type
-        except AttributeError as e:
-            logger.error(f"AttributeError: {e}")
-            return None
-
-    def get_datatype(self, dp) -> str:
-        try:
-            datatype = dp.modbus_data_point_configuration.modbus_data_type.__dict__
-            for key in datatype:
-                if datatype[key] is not None:
-                    return key
-            raise DataProcessingError('data_type not available')
-        except AttributeError as e:
-            logger.error(f"AttributeError: {e}")
-            return None
-    
-    def get_bit_rank(self, dp):
-        try:
-            bitrank = dp.modbus_data_point_configuration.bit_rank
-            if bitrank is None:
-                raise DataProcessingError("Bit rank is None")
-            return bitrank
-        except AttributeError as e:
-            logger.error(f"AttributeError: {e}")
-            return None
-
-    def get_address(self, dp):
-        try:
-            address = dp.modbus_data_point_configuration.address
-            if address is None:
-                raise DataProcessingError("Address is None")
-            return address
-        except AttributeError as e:
-            logger.error(f"AttributeError: {e}")
-            return None
-
-
-    def get_size(self, dp):
-        try:
-            size = dp.modbus_data_point_configuration.number_of_registers
-            if size is None:
-                raise DataProcessingError("Size is None")
-            return size
-        except AttributeError as e:
-            logger.error(f"AttributeError: {e}")
-            return None
-
-    def get_multiplicator(self, dp):
-        try:
-            multiplicator = dp.modbus_attributes.scaling_factor.multiplicator
-            if multiplicator is None:
-                raise DataProcessingError("Multiplicator is None")
-            return multiplicator
-        except AttributeError as e:
-            logger.error(f"AttributeError: {e}")
-            return None
-
-    def get_power_10(self, dp):
-        try:
-            power_10 = dp.modbus_attributes.scaling_factor.powerof10
-            if power_10 is None:
-                raise DataProcessingError("Power of 10 is None")
-            return power_10
-        except AttributeError as e:
-            logger.error(f"AttributeError: {e}")
-            return None
-
-    def get_unit(self, dp):
-        try:
-            unit = dp.data_point.unit.value
-            if unit is None:
-                raise DataProcessingError("Unit is None")
-            return unit
-        except AttributeError as e:
-            logger.error(f"AttributeError: {e}")
-            return None
-
-    def get_name(self, dp):
-        try:
-            name = dp.data_point.data_point_name
-            if name is None:
-                raise DataProcessingError("Name is None")
-            return name
-        except AttributeError as e:
-            logger.error(f"AttributeError: {e}")
-            return None
+        return dp.modbus_data_point_configuration.register_type.value.__str__()
+
+    def get_datatype(self, dp: ModbusDataPoint) -> str:
+        datatype = dp.modbus_data_point_configuration.modbus_data_type.__dict__
+        for key in datatype:
+            if datatype[key] is not None:
+                return key
+
+    def get_bit_rank(self, dp: ModbusDataPoint):
+        return dp.modbus_data_point_configuration.bit_rank
+
+    def get_address(self, dp: ModbusDataPoint):
+        return dp.modbus_data_point_configuration.address
+
+    def get_size(self, dp: ModbusDataPoint):
+        return dp.modbus_data_point_configuration.number_of_registers
+
+    def get_multiplicator(self, dp: ModbusDataPoint) -> int:
+        return dp.modbus_attributes.scaling_factor.multiplicator
+
+    def get_power_10(self, dp: ModbusDataPoint) -> int:
+        return dp.modbus_attributes.scaling_factor.powerof10
+
+    def get_unit(self, dp: ModbusDataPoint):
+        return dp.data_point.unit.value
+
+    def get_name(self, dp: ModbusDataPoint):
+        return dp.data_point.data_point_name
+
+    """
+    def find_dp(self, fp_name: str, dp_name: str) -> SgrModbusDataPointType:
+        
+        Searches the datapoint in the root element.
+        :param root: The root element created with the xsdata parser
+        :param fp_name: The name of the funcitonal profile in which the datapoint resides
+        :param dp_name: The name of the datapoint
+        :returns: The datapoint element found in root, if not, returns None.
+        
+        for fp in self.root.fp_list_element:
+                if fp_name == fp.functional_profile.profile_name:
+                    #Secondly we filter the datpoint name
+                    for dp in fp.dp_list_element:
+                        if dp_name == dp.data_point[0].datapoint_name:
+                            return dp
+        return None
+    """
 
-    def find_dp(self, root, fp_name: str, dp_name: str):
+    def configuration_parameter(self) -> list[ConfigurationParameter]:
+        return self._configurations_params
+
+    async def connect(self):
+        # check if there already exists a ModbusRTUClient for the communication over ModbusRTU
+        if SgrModbusRtuInterface.globalModbusRTUClient is None:
+            self.client = SGrModbusRTUClient(str(self.port), str(self.parity), int(self.baudrate))
+            SgrModbusRtuInterface.globalModbusRTUClient = self.client
+        else:
+            self.client = SgrModbusRtuInterface.globalModbusRTUClient
+
+        if self.client:
+            connected = await self.client.connect()
+            if connected:
+                print("Connected to ModbusRTU on Port: " + self.port)
+
+    def get_function_profiles(self) -> dict[str, FunctionProfile]:
+        return self._function_profiles
+
+    def device_information(self) -> DeviceInformation:
+        return self._device_information
+
+    def find_dp(self, fp_name: str, dp_name: str):
         """
         Searches the datapoint in the root element.
         :param root: The root element created with the xsdata parser
         :param fp_name: The name of the funcitonal profile in which the datapoint resides
         :param dp_name: The name of the datapoint
         :returns: The datapoint element found in root, if not, returns None.
         """
-        fp = next(filter(lambda x: x.functional_profile.functional_profile_name == fp_name, root.interface_list.modbus_interface.functional_profile_list.functional_profile_list_element), None)
+        fp = next(filter(lambda x: x.functional_profile.profile_name == fp_name, self.root.fp_list_element), None)
         if fp:
-            dp = next(filter(lambda x: x.data_point.data_point_name == dp_name, fp.data_point_list.data_point_list_element), None)
+            dp = next(filter(lambda x: x.data_point.datapoint_name == dp_name, fp.dp_list_element), None)
             if dp:
                 return dp
-            raise DataPointException(f"Datapoint {dp_name} not found in functional profile {fp_name}.")
-        raise FunctionalProfileException(f"Functional profile {fp_name} not found in XML file.")
 
-    # TODO a getval for L1, L2 and L3 at the same time
+    def get_device_name(self) -> str:
+        """
+        returns the s_LV1_Name of the device
+        """
+        return self.root.device_profile.dev_name_list.s_lv1_name
 
-    #TODO
-    def get_dp_attribute(self, datapoint: str, attribute: str):
+    def get_modbusInterfaceSelection(self) -> str:
         """
-        Searches for a specific attribute in the datapoint via a key.
-        :param attribute"address", "size", "bitrank", "data_type", "register_type", "unit", "multiplicator", "power_of", "name"
-        :returns: The chosen attribute.
+        Returns selected Modbus Interface in XML file
         """
-        #TODO
-        ...
+        return (self.root.modbus_interface_desc.modbus_interface_selection.value)
 
-async def test_loop():
-    while True:
-        print('start')
-        interface_file = 'abb_terra_01.xml'
-        sgr_modbus = SgrModbusInterface(interface_file)
-        await sgr_modbus.client.client.connect()
-        getval = await sgr_modbus.getval('CurrentAC', 'CurrentACL1')
-        print(getval)
-        await asyncio.sleep(10)
+    def get_manufacturer(self):
+        """
+        returns the manufacturer name of the device
+        """
+        # TODO it could also be root.device_information.alternative_names.manuf_name
+        return self.root.manufacturer_name
+
+    def set_slave_id(self, slave_id: int):
+        """
+        changes the slave id for the instance
+        """
+        self.slave_id = slave_id
+
+    # TODO a getval for L1, L2 and L3 at the same time
 
 
 if __name__ == "__main__":
     starting_time = time.time()
     print('start')
-    try:
-        asyncio.run(test_loop())
-    except KeyboardInterrupt:
-        print("done")
+    interface_file = '../xml_files/SGr_04_0016_xxxx_ABBMeterV0.2.1.xml'
+    a = SgrModbusRtuInterface(interface_file)
+    print('ActivePowerACtot :', a.getval('ActivePowerAC', 'ActivePowerACtot'))
+    # Power = a.client.value_decoder(0x5B14,2,"int32","HoldingRegister",1,Endian.Big)
+    # print(str(Power*0.01) + "W")
+
+    # a.setval('ActiveEnerBalanceAC', 'ActiveImportAC', 9000)
+
+    dp = find_dp(a.root, 'ActiveEnerBalanceAC', 'ActiveImportAC')
+    print("ActiveImportAC :", a.getval(dp))
 
+    a.client.client.close()
+    print("print finished")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sgr-lib-0.0.1/sgr_library/payload_decoder.py` & `sgr-lib-0.0.2/sgr_library/payload_decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """
 SGr Payload Builder
 ------------------------
 
 An adapted payload decoder and payload builder to use with the pymodbus library.
 """
 from pymodbus.payload import BinaryPayloadDecoder, BinaryPayloadBuilder
-from numpy import ceil, floor, rint
 from enum import Enum
+from math import ceil, floor
 
 
 class RoundingScheme(Enum):
     floor = 'floor'
     ceil = 'ceil'
     near = 'Near'
 
+
 def round_to_int(value: float, scheme: RoundingScheme) -> int:
     if scheme == RoundingScheme.floor:
-        return int(floor(value))
+        return floor(value)
     elif scheme == RoundingScheme.ceil:
-        return int(ceil(value))
+        return ceil(value)
     elif scheme == RoundingScheme.near:
-        return int(rint(value))
+        return round(value)
     else:
         print(
             'tried rounding with a invalid scheme (%s) using floor instead', scheme
         )
         return int(floor(value))
 
 
@@ -54,19 +55,20 @@
         elif modbus_type == 'int64_u':
             return self.decode_64bit_uint()
         elif modbus_type == 'float16':
             return self.decode_16bit_float()
         elif modbus_type == 'float32':
             return self.decode_32bit_float()
         elif modbus_type == 'float64':
-            return self.decode_32bit_float()
+            return self.decode_64bit_float()
         elif modbus_type == 'string':
             return self.decode_string(byte_count)
         else:
-            pass
+            raise ValueError('Unknown modbus type "%s"', modbus_type)
+
 
 class PayloadBuilder(BinaryPayloadBuilder):
     def __init__(self, *args, **kwarg):
         super().__init__(*args, **kwarg)
 
     def encode(self, value: float, modbus_type: str, rounding: RoundingScheme):
         """
@@ -95,14 +97,7 @@
             self.add_32bit_float(round_to_int(value, rounding))
         elif modbus_type == 'float64':
             self.add_64bit_float(round_to_int(value, rounding))
         elif modbus_type == 'string':
             self.add_string(round_to_int(value, rounding))
         else:
             print('Unknown modbus type "%s"', modbus_type)
-
-
-
-
-
-
-
```

