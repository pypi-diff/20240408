# Comparing `tmp/salure_helpers_datev-1.0.4.tar.gz` & `tmp/salure_helpers_datev-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_datev-1.0.4.tar", last modified: Tue Mar 19 13:03:16 2024, max compression
+gzip compressed data, was "dist/salure_helpers_datev-1.0.5.tar", last modified: Mon Apr  8 15:23:57 2024, max compression
```

## Comparing `salure_helpers_datev-1.0.4.tar` & `salure_helpers_datev-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      259 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/salure_helpers/datev/
--rw-rw-rw-   0 root         (0) root         (0)      231 2024-03-19 13:02:55.000000 salure_helpers_datev-1.0.4/salure_helpers/datev/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30522 2024-03-19 13:02:55.000000 salure_helpers_datev-1.0.4/salure_helpers/datev/datev.py
--rw-rw-rw-   0 root         (0) root         (0)    83546 2024-03-19 13:02:55.000000 salure_helpers_datev-1.0.4/salure_helpers/datev/datev_lodas.py
--rw-rw-rw-   0 root         (0) root         (0)    32802 2024-03-19 13:02:55.000000 salure_helpers_datev-1.0.4/salure_helpers/datev/datev_lodas_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     5621 2024-03-19 13:02:55.000000 salure_helpers_datev-1.0.4/salure_helpers/datev/datev_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/salure_helpers_datev.egg-info/
--rw-r--r--   0 root         (0) root         (0)      259 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/salure_helpers_datev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      451 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/salure_helpers_datev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/salure_helpers_datev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/salure_helpers_datev.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       81 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/salure_helpers_datev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/salure_helpers_datev.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 13:03:16.000000 salure_helpers_datev-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-03-19 13:02:55.000000 salure_helpers_datev-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      259 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30522 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/datev.py
+-rw-rw-rw-   0 root         (0) root         (0)    83624 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/datev_lodas.py
+-rw-rw-rw-   0 root         (0) root         (0)    32802 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/datev_lodas_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     5621 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/datev_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      259 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/setup.py
```

### Comparing `salure_helpers_datev-1.0.4/salure_helpers/datev/datev.py` & `salure_helpers_datev-1.0.5/salure_helpers/datev/datev.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_datev-1.0.4/salure_helpers/datev/datev_lodas.py` & `salure_helpers_datev-1.0.5/salure_helpers/datev/datev_lodas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1214,15 +1214,17 @@
                 f"{row['booking_date'] if 'booking_date' in row.keys() else ''};"
                 f"{row['value'] if 'value' in row.keys() else ''};"
                 f"{row['declaration_type'] if 'declaration_type' in row.keys() else ''};"
                 f"{row['costcenter'] if 'costcenter' in row.keys() else ''};"
                 f"{row['wage_component'] if 'wage_component' in row.keys() else ''};"
                 f"{row['wage_factor'] if 'wage_factor' in row.keys() else ''};\n"
             )
-            return template_description, body
+            body.append(formatted_string)
+
+        return template_description, body
 
     @staticmethod
     def employee_vwl(df: pd.DataFrame,
                      use_alternative_employee_number: bool = False):
         """
         TECHNICAL NAME              DESCRIPTION Lodas               DESCRIPTION English                 INTERFACE VALUE        DEID (values)
         pnr_betriebliche#psd        Betriebliche Personalnummer     Alternative employee ID             employee_id
@@ -1246,15 +1248,17 @@
                 f"1300;"
                 f"{row['employee_id']};"
                 f"{row['vwl_saving_formation'] if 'vwl_saving_formation' in row.keys() else ''};"
                 f"{row['vwl_wage_component'] if 'vwl_wage_component' in row.keys() else ''};"
                 f"{row['vwl_amount'] if 'vwl_amount' in row.keys() else ''};"
                 f"{row['vwl_direct_debit'] if 'vwl_direct_debit' in row.keys() else ''};\n"
             )
-            return template_description, body
+            body.append(formatted_string)
+
+        return template_description, body
 
     @staticmethod
     def _replace_invalid_characters(input_string):
         return input_string.replace('\xdf', 'ss')
 
     def _replace_in_list(self, string_list):
         return [self._replace_invalid_characters(s) for s in string_list]
```

### Comparing `salure_helpers_datev-1.0.4/salure_helpers/datev/datev_lodas_mapping.py` & `salure_helpers_datev-1.0.5/salure_helpers/datev/datev_lodas_mapping.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_datev-1.0.4/salure_helpers/datev/datev_mapping.py` & `salure_helpers_datev-1.0.5/salure_helpers/datev/datev_mapping.py`

 * *Files identical despite different names*

