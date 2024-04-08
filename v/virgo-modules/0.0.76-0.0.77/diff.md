# Comparing `tmp/virgo_modules-0.0.76.tar.gz` & `tmp/virgo_modules-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.76.tar", last modified: Fri Apr  5 14:59:35 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.77.tar", last modified: Mon Apr  8 18:00:08 2024, max compression
```

## Comparing `virgo_modules-0.0.76.tar` & `virgo_modules-0.0.77.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 14:59:35.871625 virgo_modules-0.0.76/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.76/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-04-05 14:59:35.869624 virgo_modules-0.0.76/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.76/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 14:59:35.872624 virgo_modules-0.0.76/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-04-05 14:59:05.000000 virgo_modules-0.0.76/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:59:35.780584 virgo_modules-0.0.76/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-04-05 14:59:35.802730 virgo_modules-0.0.76/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:59:35.863631 virgo_modules-0.0.76/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    64053 2024-04-04 18:20:37.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   142521 2024-04-03 15:42:01.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:59:35.824246 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-04-05 14:59:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-04-05 14:59:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 14:59:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-04-05 14:59:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 14:59:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 18:00:08.665646 virgo_modules-0.0.77/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.77/LICENSE
+-rw-rw-rw-   0        0        0      859 2024-04-08 18:00:08.662644 virgo_modules-0.0.77/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.77/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 18:00:08.665646 virgo_modules-0.0.77/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-08 17:58:53.000000 virgo_modules-0.0.77/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:00:08.581644 virgo_modules-0.0.77/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:00:08.606644 virgo_modules-0.0.77/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:00:08.659650 virgo_modules-0.0.77/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    64053 2024-04-04 18:20:37.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   142729 2024-04-08 17:58:53.000000 virgo_modules-0.0.77/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:00:08.628644 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0      859 2024-04-08 18:00:07.000000 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-04-08 18:00:07.000000 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 18:00:07.000000 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-04-08 18:00:07.000000 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-08 18:00:07.000000 virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.76/LICENSE` & `virgo_modules-0.0.77/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.76/setup.py` & `virgo_modules-0.0.77/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.76",
+    version="0.0.77",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.76/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.77/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.76/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.77/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.76/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.77/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.76/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.77/virgo_app/virgo_modules/src/re_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.76/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.77/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -2730,19 +2730,19 @@
             np.where(
                 df[low_signal] == 1,
                 'down',
                 None
             )
         )
         df = df[~df.signal_type.isna()]
-        # df['Date'] = df.index
         df['lag_Date'] = df['Date'].shift(1)
+        df['lag_signal_type'] = df['signal_type'].shift(1)
         df['span'] = (pd.to_datetime(df['Date']) - pd.to_datetime(df['lag_Date'])).dt.days - 1
-        df['break'] = np.where(df['span'] > 3, 1, 0)
-        df['break'] = np.where(df['span'].isna(), 1, df['break'])
+        df['break'] = np.where((df['span'] > 3) & (df['lag_signal_type'] == df['signal_type']), 1, 0)
+        df['break'] = np.where((df['lag_signal_type'] != df['signal_type']), 1, df['break'])
 
         df['chain_id'] = df.sort_values(['Date']).groupby(['break']).cumcount() + 1
         df['chain_id'] = np.where(df['break'] == 1, df['chain_id'], np.nan )
         df['chain_id'] = df['chain_id'].fillna(method = 'ffill')
 
         df['internal_rn'] = df.sort_values(['Date']).groupby(['chain_id']).cumcount() + 1
         df['inv_internal_rn'] = df.sort_values(['Date'],ascending = False).groupby(['chain_id']).cumcount() + 1
@@ -2857,19 +2857,19 @@
                     np.where(
                         df2[low_signal] == 1,
                         'down',
                         None
                     )
                 )
         df2 = df2[~df2.signal_type.isna()]
-        # df2['Date_'] = df2.index
         df2['lag_Date'] = df2['Date'].shift(1)
+        df2['lag_signal_type'] = df2['signal_type'].shift(1)
         df2['span'] = (pd.to_datetime(df2['Date']) - pd.to_datetime(df2['lag_Date'])).dt.days - 1
-        df2['break'] = np.where(df2['span'] > 3, 1, 0)
-        df2['break'] = np.where(df2['span'].isna(), 1, df2['break'])
+        df2['break'] = np.where((df2['span'] > 3) & (df2['lag_signal_type'] == df2['signal_type']), 1, 0)
+        df2['break'] = np.where((df2['lag_signal_type'] != df2['signal_type']), 1, df2['break'])
 
         df2['chain_id'] = df2.sort_values(['Date']).groupby(['break']).cumcount() + 1
         df2['chain_id'] = np.where(df2['break'] == 1, df2['chain_id'], np.nan )
         df2['chain_id'] = df2['chain_id'].fillna(method = 'ffill')
 
         df2['internal_rn'] = df2.sort_values(['Date']).groupby(['chain_id']).cumcount() + 1
         df2['inv_internal_rn'] = df2.sort_values(['Date'],ascending = False).groupby(['chain_id']).cumcount() + 1
```

### Comparing `virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.77/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

