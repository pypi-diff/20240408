# Comparing `tmp/django-ws-scoring-0.1.8.tar.gz` & `tmp/django-ws-scoring-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ws-scoring-0.1.8.tar", last modified: Thu Mar 21 08:13:44 2024, max compression
+gzip compressed data, was "django-ws-scoring-0.2.0.tar", last modified: Mon Apr  8 09:54:52 2024, max compression
```

## Comparing `django-ws-scoring-0.1.8.tar` & `django-ws-scoring-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:13:44.760259 django-ws-scoring-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-21 08:13:19.000000 django-ws-scoring-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-21 08:13:19.000000 django-ws-scoring-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-21 08:13:44.760259 django-ws-scoring-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-03-21 08:13:19.000000 django-ws-scoring-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:13:44.760259 django-ws-scoring-0.1.8/django_ws_scoring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-21 08:13:44.000000 django-ws-scoring-0.1.8/django_ws_scoring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-21 08:13:44.000000 django-ws-scoring-0.1.8/django_ws_scoring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 08:13:44.000000 django-ws-scoring-0.1.8/django_ws_scoring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-21 08:13:44.000000 django-ws-scoring-0.1.8/django_ws_scoring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-21 08:13:44.000000 django-ws-scoring-0.1.8/django_ws_scoring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-21 08:13:19.000000 django-ws-scoring-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-21 08:13:44.764259 django-ws-scoring-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-21 08:13:19.000000 django-ws-scoring-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:13:44.760259 django-ws-scoring-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-03-21 08:13:19.000000 django-ws-scoring-0.1.8/tests/test_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:13:44.760259 django-ws-scoring-0.1.8/ws_scoring/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 08:13:19.000000 django-ws-scoring-0.1.8/ws_scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-03-21 08:13:19.000000 django-ws-scoring-0.1.8/ws_scoring/module_ws_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:54:52.611773 django-ws-scoring-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 09:54:23.000000 django-ws-scoring-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 09:54:23.000000 django-ws-scoring-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-08 09:54:52.611773 django-ws-scoring-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-08 09:54:23.000000 django-ws-scoring-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:54:52.611773 django-ws-scoring-0.2.0/django_ws_scoring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-08 09:54:52.000000 django-ws-scoring-0.2.0/django_ws_scoring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-08 09:54:52.000000 django-ws-scoring-0.2.0/django_ws_scoring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:54:52.000000 django-ws-scoring-0.2.0/django_ws_scoring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 09:54:52.000000 django-ws-scoring-0.2.0/django_ws_scoring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 09:54:52.000000 django-ws-scoring-0.2.0/django_ws_scoring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 09:54:23.000000 django-ws-scoring-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-08 09:54:52.611773 django-ws-scoring-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 09:54:23.000000 django-ws-scoring-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:54:52.611773 django-ws-scoring-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-08 09:54:23.000000 django-ws-scoring-0.2.0/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:54:52.611773 django-ws-scoring-0.2.0/ws_scoring/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:54:23.000000 django-ws-scoring-0.2.0/ws_scoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-08 09:54:23.000000 django-ws-scoring-0.2.0/ws_scoring/module_ws_scoring.py
```

### Comparing `django-ws-scoring-0.1.8/LICENSE` & `django-ws-scoring-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ws-scoring-0.1.8/PKG-INFO` & `django-ws-scoring-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ws-scoring
-Version: 0.1.8
+Version: 0.2.0
 Summary: A light weight scoring system for a Django Queryset based on past User Input.
 Home-page: https://github.com/windschatten-it/django-ws-scoring
 Author: windschatten.it
 Author-email: niklas@windschatten.it
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `django-ws-scoring-0.1.8/README.rst` & `django-ws-scoring-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-ws-scoring-0.1.8/django_ws_scoring.egg-info/PKG-INFO` & `django-ws-scoring-0.2.0/django_ws_scoring.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ws-scoring
-Version: 0.1.8
+Version: 0.2.0
 Summary: A light weight scoring system for a Django Queryset based on past User Input.
 Home-page: https://github.com/windschatten-it/django-ws-scoring
 Author: windschatten.it
 Author-email: niklas@windschatten.it
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `django-ws-scoring-0.1.8/setup.cfg` & `django-ws-scoring-0.2.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-ws-scoring
-version = 0.1.8
+version = 0.2.0
 description = A light weight scoring system for a Django Queryset based on past User Input.
 url = https://github.com/windschatten-it/django-ws-scoring
 author = windschatten.it
 author_email = niklas@windschatten.it
 license = MIT
 zip_safe = False
 long_description = file: README.rst
```

### Comparing `django-ws-scoring-0.1.8/tests/test_module.py` & `django-ws-scoring-0.2.0/tests/test_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,18 +72,14 @@
 
         processed_df = self.manipulator.preprocess_user_history()
         self.assertFalse(processed_df.empty)
 
         # Check for correct group assignment based on 'created_at'
         self.assertTrue(all(processed_df['group'].notnull()))
 
-        # Ensure that rows with 'None' values are handled as expected
-        self.assertTrue(all(processed_df['keyword_frequency_weight'] >= 0))
-        self.assertTrue(all(processed_df['location_frequency_weight'] >= 0))
-
         # Check if 'weight_factor' is assigned correctly
         self.assertIn('weight_factor', processed_df.columns)
 
     @patch('ws_scoring.module_ws_scoring.read_frame')
     def test_get_scores_map(self, mock_read_frame):
         # Mock the read_frame call to return a DataFrame for the job details
         # since preprocess_user_history will process the self.user_history_data
```

### Comparing `django-ws-scoring-0.1.8/ws_scoring/module_ws_scoring.py` & `django-ws-scoring-0.2.0/ws_scoring/module_ws_scoring.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pandas as pd
 from django.db.models import When, Value, Case, DecimalField
+from django.utils import timezone
 from django_pandas.io import read_frame
 
 
 class ManipulateQuerySet:
     def __init__(self, queryset, user_history, field_weight_dict):
         self.queryset = queryset
         self.user_history = user_history
@@ -34,41 +35,45 @@
         user_history_df['group'] = pd.cut(
             user_history_df['days_diff'],
             bins=[-np.inf, 7, 31, np.inf],
             labels=['group1', 'group2', 'group3'],
             right=False
         )
 
-        # Calculate frequency weights independently
-        valid_keyword_searches = user_history_df['keyword_search'][user_history_df['keyword_search'].notnull()
-                                                                   & (user_history_df['keyword_search'] != '')]
-        valid_location_searches = user_history_df['location_search'][user_history_df['location_search'].notnull()
-                                                                   & (user_history_df['location_search'] != '')]
-        keyword_frequency = valid_keyword_searches.value_counts()
-        location_frequency = valid_location_searches.value_counts()
-
-        # Map the frequencies back to the original dataframe
-        user_history_df['keyword_frequency_weight'] = user_history_df['keyword_search'].map(keyword_frequency).fillna(0)
-        user_history_df['location_frequency_weight'] = user_history_df['location_search'].map(
-            location_frequency).fillna(0)
-
-        # Calculate a combined frequency weight by summing keyword and location frequency weights
-        user_history_df['total_weight'] = user_history_df['keyword_frequency_weight'] + user_history_df[
-            'location_frequency_weight']
-        # user_history_df['total_weight'] = user_history_df['frequency_weight']  # Adjust this calculation as needed
+        group2_df = user_history_df[user_history_df['group'] == 'group2']
+        group3_df = user_history_df[user_history_df['group'] == 'group3']
+        group2_df = group2_df.head(3)
+        group3_df = group3_df.head(1)
+        group2_3_df = pd.concat([group2_df, group3_df])
+
+        group2_3_df = group2_3_df.drop_duplicates(subset=['keyword_search'], keep='first')
+        group2_3_df = group2_3_df.drop_duplicates(subset=['location_search'], keep='first')
 
         # Filter and select rows based on group assignment
-        group1_df = user_history_df[user_history_df['group'] == 'group1']
-        group2_df = user_history_df[user_history_df['group'] == 'group2'].sort_values(by='total_weight',
-                                                                                      ascending=False).head(3)
-        group3_df = user_history_df[user_history_df['group'] == 'group3'].sort_values(by='total_weight',
-                                                                                      ascending=False).head(1)
+        group1_df = user_history_df[user_history_df['group'] == 'group1'].head(50)
+
+        # Deduplicate for keyword_search, retaining the first occurrence
+        group1_keywords = group1_df.drop_duplicates(subset=['keyword_search'], keep='first') \
+            .loc[group1_df['keyword_search'] != ''].assign(location_search='')
+
+        # Deduplicate for location_search, retaining the first occurrence
+        group1_locations = group1_df.drop_duplicates(subset=['location_search'], keep='first') \
+            .loc[group1_df['location_search'] != ''].assign(keyword_search='')
+
+        group1_kldb = group1_df[group1_df['kldb'].notna()]
+
+        # Deduplicate for location_search, retaining the first occurrence
+        group1_kldb = group1_kldb.drop_duplicates(subset=['kldb'], keep='first')
+
+        # Combine the distinct keyword and location searches, filling empty values to avoid losing rows
+        group1_df_combined = pd.concat([group1_keywords, group1_locations, group1_kldb], ignore_index=True) \
+            .drop_duplicates(subset=['keyword_search', 'location_search', 'kldb'], keep='first')
 
         # Concatenate the selected rows from each group
-        final_df = pd.concat([group1_df, group2_df, group3_df])
+        final_df = pd.concat([group1_df_combined, group2_3_df])
 
         # Sort the final_df by 'created_at' in descending order to ensure it's in the correct order
         # This step is crucial if the concatenation disrupts the order you're expecting for applying the weight factor
         final_df = final_df.sort_values(by='created_at', ascending=False)
 
         # Apply a depreciating factor to each row in final_df
         starting_weight = 1.0
@@ -78,14 +83,18 @@
         num_rows = len(final_df)
 
         # Generate a list of depreciating factors for each row
         depreciating_factors = [starting_weight * (depreciation_rate ** i) for i in range(num_rows)]
 
         # Assign the generated depreciating factors to a new column 'weight_factor' in final_df
         final_df['weight_factor'] = depreciating_factors
+
+        final_df.loc[final_df['group'] == 'group2', 'weight_factor'] *= 0.1
+        final_df.loc[final_df['group'] == 'group3', 'weight_factor'] *= 0.01
+
         # Now, final_df includes a 'weight_factor' column with depreciating values for each row, ready to return
         return final_df
 
     def get_scores_map(self):
         # Preprocess user history first
         user_history_df = self.preprocess_user_history()
         # Convert queryset to DataFrame
```

