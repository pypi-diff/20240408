# Comparing `tmp/spswarehouse-0.6.2.tar.gz` & `tmp/spswarehouse-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spswarehouse-0.6.2.tar", last modified: Wed Apr  3 17:48:11 2024, max compression
+gzip compressed data, was "spswarehouse-0.6.3.tar", last modified: Mon Apr  8 20:14:56 2024, max compression
```

## Comparing `spswarehouse-0.6.2.tar` & `spswarehouse-0.6.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.439124 spswarehouse-0.6.2/
--rw-rw-rw-   0        0        0    35823 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/LICENSE
--rw-rw-rw-   0        0        0      448 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     8200 2024-04-03 17:48:11.436160 spswarehouse-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     7815 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 17:48:11.440298 spswarehouse-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      744 2024-04-03 17:19:19.000000 spswarehouse-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.059018 spswarehouse-0.6.2/spswarehouse/
--rw-rw-rw-   0        0        0      582 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.234994 spswarehouse-0.6.2/spswarehouse/calpads/
--rw-rw-rw-   0        0        0        0 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/calpads/__init__.py
--rw-rw-rw-   0        0        0    40824 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/calpads/calpads.py
--rw-rw-rw-   0        0        0     6136 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/calpads/calpads_config.py
--rw-rw-rw-   0        0        0     1187 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/credentials.py.template
-drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.302831 spswarehouse-0.6.2/spswarehouse/general/
--rw-rw-rw-   0        0        0        0 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/general/__init__.py
--rw-rw-rw-   0        0        0      730 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/general/os.py
--rw-rw-rw-   0        0        0    14021 2024-04-03 17:13:50.000000 spswarehouse-0.6.2/spswarehouse/general/selenium.py
--rw-rw-rw-   0        0        0     2347 2024-04-03 17:47:17.000000 spswarehouse-0.6.2/spswarehouse/googledrive.py
--rw-rw-rw-   0        0        0     2044 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/googlesheets.py
--rw-rw-rw-   0        0        0     2078 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/googleslides.py
--rw-rw-rw-   0        0        0    35075 2024-04-03 17:14:06.000000 spswarehouse-0.6.2/spswarehouse/magic_spreadsheet.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.424368 spswarehouse-0.6.2/spswarehouse/powerschool/
--rw-rw-rw-   0        0        0        0 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/powerschool/__init__.py
--rw-rw-rw-   0        0        0    36921 2024-04-03 17:16:40.000000 spswarehouse-0.6.2/spswarehouse/powerschool/powerschool.py
--rw-rw-rw-   0        0        0    35449 2024-04-03 17:14:06.000000 spswarehouse-0.6.2/spswarehouse/powerschool/powerschool_calpads.py
--rw-rw-rw-   0        0        0     4122 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/powerschool/student_passwords.py
--rw-rw-rw-   0        0        0      357 2024-04-03 17:14:06.000000 spswarehouse-0.6.2/spswarehouse/requirements.txt
--rw-rw-rw-   0        0        0     1269 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/table_names.py
--rw-rw-rw-   0        0        0     8313 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/table_utils.py
--rw-rw-rw-   0        0        0     4812 2023-11-02 22:29:50.000000 spswarehouse-0.6.2/spswarehouse/warehouse.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:48:11.153958 spswarehouse-0.6.2/spswarehouse.egg-info/
--rw-rw-rw-   0        0        0     8200 2024-04-03 17:48:09.000000 spswarehouse-0.6.2/spswarehouse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-04-03 17:48:10.000000 spswarehouse-0.6.2/spswarehouse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 17:48:09.000000 spswarehouse-0.6.2/spswarehouse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-03 17:48:09.000000 spswarehouse-0.6.2/spswarehouse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 20:14:56.895064 spswarehouse-0.6.3/
+-rw-rw-rw-   0        0        0    35823 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0      448 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     8200 2024-04-08 20:14:56.890356 spswarehouse-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7815 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 20:14:56.896185 spswarehouse-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      744 2024-04-08 19:48:22.000000 spswarehouse-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:14:56.733152 spswarehouse-0.6.3/spswarehouse/
+-rw-rw-rw-   0        0        0      582 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:14:56.823384 spswarehouse-0.6.3/spswarehouse/calpads/
+-rw-rw-rw-   0        0        0        0 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/calpads/__init__.py
+-rw-rw-rw-   0        0        0    40824 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/calpads/calpads.py
+-rw-rw-rw-   0        0        0     6136 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/calpads/calpads_config.py
+-rw-rw-rw-   0        0        0     1187 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/credentials.py.template
+drwxrwxrwx   0        0        0        0 2024-04-08 20:14:56.849639 spswarehouse-0.6.3/spswarehouse/general/
+-rw-rw-rw-   0        0        0        0 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/general/__init__.py
+-rw-rw-rw-   0        0        0      730 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/general/os.py
+-rw-rw-rw-   0        0        0    14683 2024-04-05 22:45:19.000000 spswarehouse-0.6.3/spswarehouse/general/selenium.py
+-rw-rw-rw-   0        0        0     2347 2024-04-08 19:48:01.000000 spswarehouse-0.6.3/spswarehouse/googledrive.py
+-rw-rw-rw-   0        0        0     2044 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/googlesheets.py
+-rw-rw-rw-   0        0        0     2078 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/googleslides.py
+-rw-rw-rw-   0        0        0    35075 2024-04-08 19:48:01.000000 spswarehouse-0.6.3/spswarehouse/magic_spreadsheet.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:14:56.884414 spswarehouse-0.6.3/spswarehouse/powerschool/
+-rw-rw-rw-   0        0        0        0 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/powerschool/__init__.py
+-rw-rw-rw-   0        0        0    36921 2024-04-08 19:48:01.000000 spswarehouse-0.6.3/spswarehouse/powerschool/powerschool.py
+-rw-rw-rw-   0        0        0    35449 2024-04-08 19:48:01.000000 spswarehouse-0.6.3/spswarehouse/powerschool/powerschool_calpads.py
+-rw-rw-rw-   0        0        0     4122 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/powerschool/student_passwords.py
+-rw-rw-rw-   0        0        0      357 2024-04-08 19:48:01.000000 spswarehouse-0.6.3/spswarehouse/requirements.txt
+-rw-rw-rw-   0        0        0     1269 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/table_names.py
+-rw-rw-rw-   0        0        0     8313 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/table_utils.py
+-rw-rw-rw-   0        0        0     4812 2023-11-02 22:29:50.000000 spswarehouse-0.6.3/spswarehouse/warehouse.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:14:56.781564 spswarehouse-0.6.3/spswarehouse.egg-info/
+-rw-rw-rw-   0        0        0     8200 2024-04-08 20:14:55.000000 spswarehouse-0.6.3/spswarehouse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-04-08 20:14:56.000000 spswarehouse-0.6.3/spswarehouse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 20:14:55.000000 spswarehouse-0.6.3/spswarehouse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-08 20:14:55.000000 spswarehouse-0.6.3/spswarehouse.egg-info/top_level.txt
```

### Comparing `spswarehouse-0.6.2/LICENSE` & `spswarehouse-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/PKG-INFO` & `spswarehouse-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.6.2
+Version: 0.6.3
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.6.2/README.md` & `spswarehouse-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/setup.py` & `spswarehouse-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spswarehouse",
-    version="0.6.2",
+    version="0.6.3",
     author="Summit Public Schools; Harry Li Consulting, LLC",
     author_email="warehouse@summitps.org",
     description="Summit Public Schools Snowflake warehouse",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SummitPublicSchools/spswarehouse",
     packages=setuptools.find_packages(),
```

### Comparing `spswarehouse-0.6.2/spswarehouse/__init__.py` & `spswarehouse-0.6.3/spswarehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/calpads/calpads.py` & `spswarehouse-0.6.3/spswarehouse/calpads/calpads.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/calpads/calpads_config.py` & `spswarehouse-0.6.3/spswarehouse/calpads/calpads_config.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/credentials.py.template` & `spswarehouse-0.6.3/spswarehouse/credentials.py.template`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/general/os.py` & `spswarehouse-0.6.3/spswarehouse/general/os.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/general/selenium.py` & `spswarehouse-0.6.3/spswarehouse/general/selenium.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,14 +104,22 @@
 def get_element_by_xpath(driver, xpath: str, wait_time_in_seconds=30):
     """
     Waits for an element by XPATH and returns it.
     """
     elem = WebDriverWait(driver, wait_time_in_seconds).until(EC.presence_of_element_located((By.XPATH, xpath)))
     return elem
 
+def get_element_by_class_name(driver, class_name: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by class_name and returns it.
+    """
+    elem = WebDriverWait(driver, wait_time_in_seconds).until(EC.presence_of_element_located((By.CLASS_NAME, class_name)))
+
+    return elem
+
 def get_multiple_elements_by_class_name(driver, class_name: str, wait_time_in_seconds=30):
     """
     Waits for an element by class name, then retrieves the full list of elements with that class name.
     """
     _wait_for_element_to_be_present_and_return_it(driver, By.CLASS_NAME, class_name, wait_time_in_seconds)
 
     # Pause to give all elements with that class_name time to load
@@ -155,14 +163,22 @@
     """
     Waits for an element by name, clears it, and types in the input.
     """
     elem =  _wait_for_element_to_be_present_and_return_it(driver, By.NAME, element_name, wait_time_in_seconds)
     elem.clear()
     elem.send_keys(input_to_type)
 
+def type_in_element_by_xpath(driver, element_xpath: str, input_to_type: str, wait_time_in_seconds=30):
+    """
+    Waits for an element by XPATH, clears it, and types in the input.
+    """
+    elem =  _wait_for_element_to_be_present_and_return_it(driver, By.XPATH, element_xpath, wait_time_in_seconds)
+    elem.clear()
+    elem.send_keys(input_to_type)
+
 
 ### Wait for Element
     
 def wait_for_element_containing_specific_text(driver, expected_element_text, wait_time_in_seconds=30):
     """
     Waits for an element containing the specific text. Will crash if it does not 
     appear in the time allotted (default = 30 seconds).
```

### Comparing `spswarehouse-0.6.2/spswarehouse/googledrive.py` & `spswarehouse-0.6.3/spswarehouse/googledrive.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/googlesheets.py` & `spswarehouse-0.6.3/spswarehouse/googlesheets.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/googleslides.py` & `spswarehouse-0.6.3/spswarehouse/googleslides.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/magic_spreadsheet.py` & `spswarehouse-0.6.3/spswarehouse/magic_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/powerschool/powerschool.py` & `spswarehouse-0.6.3/spswarehouse/powerschool/powerschool.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/powerschool/powerschool_calpads.py` & `spswarehouse-0.6.3/spswarehouse/powerschool/powerschool_calpads.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/powerschool/student_passwords.py` & `spswarehouse-0.6.3/spswarehouse/powerschool/student_passwords.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/table_names.py` & `spswarehouse-0.6.3/spswarehouse/table_names.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/table_utils.py` & `spswarehouse-0.6.3/spswarehouse/table_utils.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse/warehouse.py` & `spswarehouse-0.6.3/spswarehouse/warehouse.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.6.2/spswarehouse.egg-info/PKG-INFO` & `spswarehouse-0.6.3/spswarehouse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.6.2
+Version: 0.6.3
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.6.2/spswarehouse.egg-info/SOURCES.txt` & `spswarehouse-0.6.3/spswarehouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

