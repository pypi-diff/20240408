# Comparing `tmp/fosslight_android-4.1.16.tar.gz` & `tmp/fosslight_android-4.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fosslight_android-4.1.16.tar", last modified: Mon Nov  6 07:46:06 2023, max compression
+gzip compressed data, was "fosslight_android-4.1.17.tar", last modified: Mon Apr  8 04:33:54 2024, max compression
```

## Comparing `fosslight_android-4.1.16.tar` & `fosslight_android-4.1.17.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 07:46:06.221113 fosslight_android-4.1.16/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-11-06 07:46:06.221113 fosslight_android-4.1.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 07:46:06.221113 fosslight_android-4.1.16/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1557 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 07:46:06.213113 fosslight_android-4.1.16/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 07:46:06.217113 fosslight_android-4.1.16/src/fosslight_android/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/_binary_db_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/_src_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/_write_excel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    33530 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/android_binary_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12695 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/check_notice_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/check_package_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 07:46:06.221113 fosslight_android-4.1.16/src/fosslight_android/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   146753 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/resources/aosp_repository.json
--rw-r--r--   0 runner    (1001) docker     (127)      953 2023-11-06 07:45:50.000000 fosslight_android-4.1.16/src/fosslight_android/resources/module_license.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 07:46:06.221113 fosslight_android-4.1.16/src/fosslight_android.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-11-06 07:46:05.000000 fosslight_android-4.1.16/src/fosslight_android.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      821 2023-11-06 07:46:06.000000 fosslight_android-4.1.16/src/fosslight_android.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 07:46:05.000000 fosslight_android-4.1.16/src/fosslight_android.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-06 07:46:05.000000 fosslight_android-4.1.16/src/fosslight_android.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-11-06 07:46:05.000000 fosslight_android-4.1.16/src/fosslight_android.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-06 07:46:05.000000 fosslight_android-4.1.16/src/fosslight_android.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1557 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:54.457349 fosslight_android-4.1.17/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/src/fosslight_android/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_binary_db_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_src_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_write_excel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33530 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/android_binary_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/check_notice_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/check_package_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/src/fosslight_android/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   146753 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/resources/aosp_repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/resources/module_license.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/src/fosslight_android.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/top_level.txt
```

### Comparing `fosslight_android-4.1.16/LICENSE` & `fosslight_android-4.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.16/PKG-INFO` & `fosslight_android-4.1.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_android
-Version: 4.1.16
+Version: 4.1.17
 Summary: FOSSLight Android Scanner
 Home-page: https://github.com/fosslight/fosslight_android_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_android_scanner
 Description: <!--
         # SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

### Comparing `fosslight_android-4.1.16/README.md` & `fosslight_android-4.1.17/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.16/setup.py` & `fosslight_android-4.1.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open('requirements.txt', 'r', 'utf-8') as f:
     required = f.read().splitlines()
 
 
 if __name__ == "__main__":
     setup(
         name='fosslight_android',
-        version='4.1.16',
+        version='4.1.17',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Android Scanner',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_android-4.1.16/src/fosslight_android/_binary_db_controller.py` & `fosslight_android-4.1.17/src/fosslight_android/_binary_db_controller.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.16/src/fosslight_android/_common.py` & `fosslight_android-4.1.17/src/fosslight_android/_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,23 +131,24 @@
             need_check = "O"
         else:
             need_check = ""
         print_items_txt.append(f"{self.bin_name}\t{source_path}\t{self.notice}\t"
                                f"{oss_name}\t{self.oss_version}\t{self.license}\t{need_check}\t{comment}\t{self.tlsh}\t{self.checksum}")
         repo_link = self.download_location if self.is_new_bin else ""
         print_items_excel.append([self.bin_name, source_path, self.notice, oss_name,
-                                  self.oss_version, self.license, repo_link, repo_link, '', '', '', comment, need_check])
+                                  self.oss_version, self.license, repo_link, repo_link, '', '', '', comment,
+                                  need_check, self.tlsh, self.checksum])
 
         if self.additional_oss_items is not None:
             for item in self.additional_oss_items:
                 print_items_txt.append(f"{self.bin_name}\t{source_path}\t{self.notice}\t{item}"
                                        f"\t{need_check}\t{comment}\t{self.tlsh}\t{self.checksum}")
                 excel_item = [self.bin_name, source_path, self.notice]
                 excel_item.extend(item.split('\t'))
-                excel_item.extend(['', '', '', '', '', comment, need_check])
+                excel_item.extend(['', '', '', '', '', comment, need_check, self.tlsh, self.checksum])
                 print_items_excel.append(excel_item)
         return print_items_txt, print_items_excel
 
 
 def check_empty_column(license, oss_name, directory):
     empty_columns = []
     license_to_notice = True
```

### Comparing `fosslight_android-4.1.16/src/fosslight_android/_help.py` & `fosslight_android-4.1.17/src/fosslight_android/_help.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.16/src/fosslight_android/_src_analysis.py` & `fosslight_android-4.1.17/src/fosslight_android/_src_analysis.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.16/src/fosslight_android/_util.py` & `fosslight_android-4.1.17/src/fosslight_android/_util.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.16/src/fosslight_android/_write_excel.py` & `fosslight_android-4.1.17/src/fosslight_android/_write_excel.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 # SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
 # SPDX-License-Identifier: Apache-2.0
 import sys
 import xlsxwriter
 import logging
 from fosslight_util.write_txt import write_txt_file
 from fosslight_util.constant import LOGGER_NAME
+from fosslight_util.write_excel import hide_column
 
 logger = logging.getLogger(LOGGER_NAME)
+HIDDEN_HEADER = ['TLSH', 'SHA1']
 
 
 def write_result_to_excel(out_file_name, row_list):
     header_row = ['ID', 'Binary Name', 'Source Code Path', 'NOTICE.html', 'OSS Name', 'OSS Version', 'License',
                   'Download Location', 'Homepage',
                   'Copyright Text',
-                  'License Text', 'Exclude', 'Comment', 'Need Check']
+                  'License Text', 'Exclude', 'Comment', 'Need Check', 'TLSH', 'SHA1']
     sheet_name = "BIN (Android)"
     try:
         workbook = xlsxwriter.Workbook(out_file_name)
         worksheet = create_worksheet(workbook, sheet_name, header_row)
         write_result_to_sheet(worksheet, row_list)
+        hide_column(worksheet, header_row, HIDDEN_HEADER)
         workbook.close()
     except Exception as ex:
         print('* Error :' + str(ex))
 
 
 def write_result_to_sheet(worksheet, list_to_print):
     row = 1
```

### Comparing `fosslight_android-4.1.16/src/fosslight_android/android_binary_analysis.py` & `fosslight_android-4.1.17/src/fosslight_android/android_binary_analysis.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.16/src/fosslight_android/check_notice_file.py` & `fosslight_android-4.1.17/src/fosslight_android/check_notice_file.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.16/src/fosslight_android/check_package_file.py` & `fosslight_android-4.1.17/src/fosslight_android/check_package_file.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.16/src/fosslight_android/resources/aosp_repository.json` & `fosslight_android-4.1.17/src/fosslight_android/resources/aosp_repository.json`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.16/src/fosslight_android/resources/module_license.json` & `fosslight_android-4.1.17/src/fosslight_android/resources/module_license.json`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.16/src/fosslight_android.egg-info/PKG-INFO` & `fosslight_android-4.1.17/src/fosslight_android.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-android
-Version: 4.1.16
+Version: 4.1.17
 Summary: FOSSLight Android Scanner
 Home-page: https://github.com/fosslight/fosslight_android_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_android_scanner
 Description: <!--
         # SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

### Comparing `fosslight_android-4.1.16/src/fosslight_android.egg-info/SOURCES.txt` & `fosslight_android-4.1.17/src/fosslight_android.egg-info/SOURCES.txt`

 * *Files identical despite different names*

