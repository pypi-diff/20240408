# Comparing `tmp/cesnet-datazoo-0.1.1.tar.gz` & `tmp/cesnet-datazoo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesnet-datazoo-0.1.1.tar", last modified: Tue Mar 19 14:29:17 2024, max compression
+gzip compressed data, was "cesnet-datazoo-0.1.2.tar", last modified: Mon Apr  8 09:41:04 2024, max compression
```

## Comparing `cesnet-datazoo-0.1.1.tar` & `cesnet-datazoo-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 14:29:17.688149 cesnet-datazoo-0.1.1/
--rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet-datazoo-0.1.1/LICENCE
--rw-rw-rw-   0        0        0    12573 2024-03-19 14:29:17.687151 cesnet-datazoo-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10994 2024-03-19 11:54:16.000000 cesnet-datazoo-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 14:29:17.647799 cesnet-datazoo-0.1.1/cesnet_datazoo/
--rw-rw-rw-   0        0        0        0 2023-09-04 15:14:00.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/__init__.py
--rw-rw-rw-   0        0        0    37635 2024-03-18 16:38:54.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/config.py
--rw-rw-rw-   0        0        0     1276 2024-03-05 13:52:13.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/constants.py
-drwxrwxrwx   0        0        0        0 2024-03-19 14:29:17.671883 cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/
--rw-rw-rw-   0        0        0      443 2023-10-09 14:50:14.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/__init__.py
--rw-rw-rw-   0        0        0    46546 2024-03-15 13:44:30.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/cesnet_dataset.py
--rw-rw-rw-   0        0        0     3617 2024-03-13 15:20:57.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/datasets.py
--rw-rw-rw-   0        0        0    29154 2024-03-13 15:20:40.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/datasets_constants.py
--rw-rw-rw-   0        0        0     1854 2024-03-14 10:53:21.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/loaders.py
-drwxrwxrwx   0        0        0        0 2024-03-19 14:29:17.673891 cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/metadata/
--rw-rw-rw-   0        0        0        0 2023-08-21 14:08:44.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/metadata/__init__.py
--rw-rw-rw-   0        0        0     1608 2024-03-13 16:30:28.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/metadata/dataset_metadata.py
--rw-rw-rw-   0        0        0     2175 2024-03-19 11:54:21.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/metadata/metadata.csv
--rw-rw-rw-   0        0        0    15137 2024-03-14 10:55:15.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/statistics.py
-drwxrwxrwx   0        0        0        0 2024-03-19 14:29:17.676890 cesnet-datazoo-0.1.1/cesnet_datazoo/metrics/
--rw-rw-rw-   0        0        0        0 2023-08-17 21:32:34.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/metrics/__init__.py
--rw-rw-rw-   0        0        0     4040 2023-10-30 20:24:25.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/metrics/classification_report.py
--rw-rw-rw-   0        0        0     1303 2024-03-13 15:46:01.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/metrics/provider_metrics.py
-drwxrwxrwx   0        0        0        0 2024-03-19 14:29:17.680912 cesnet-datazoo-0.1.1/cesnet_datazoo/pytables_data/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:24:29.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/pytables_data/__init__.py
--rw-rw-rw-   0        0        0     1411 2023-10-30 20:40:56.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/pytables_data/apps_split.py
--rw-rw-rw-   0        0        0     5083 2024-03-19 14:07:14.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/pytables_data/data_scalers.py
--rw-rw-rw-   0        0        0    12932 2024-03-13 11:13:30.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/pytables_data/indices_setup.py
--rw-rw-rw-   0        0        0    17599 2024-03-13 15:21:09.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/pytables_data/pytables_dataset.py
-drwxrwxrwx   0        0        0        0 2024-03-19 14:29:17.685136 cesnet-datazoo-0.1.1/cesnet_datazoo/utils/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:35:45.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/utils/__init__.py
--rw-rw-rw-   0        0        0     2540 2024-03-13 15:35:36.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/utils/class_info.py
--rw-rw-rw-   0        0        0     1441 2024-02-20 11:51:54.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/utils/download.py
--rw-rw-rw-   0        0        0      642 2023-09-01 13:43:06.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/utils/fileutils.py
--rw-rw-rw-   0        0        0      575 2023-09-26 08:58:11.000000 cesnet-datazoo-0.1.1/cesnet_datazoo/utils/random.py
-drwxrwxrwx   0        0        0        0 2024-03-19 14:29:17.685136 cesnet-datazoo-0.1.1/cesnet_datazoo.egg-info/
--rw-rw-rw-   0        0        0    12573 2024-03-19 14:29:17.000000 cesnet-datazoo-0.1.1/cesnet_datazoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2024-03-19 14:29:17.000000 cesnet-datazoo-0.1.1/cesnet_datazoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 14:29:17.000000 cesnet-datazoo-0.1.1/cesnet_datazoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      238 2024-03-19 14:29:17.000000 cesnet-datazoo-0.1.1/cesnet_datazoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-19 14:29:17.000000 cesnet-datazoo-0.1.1/cesnet_datazoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1792 2024-03-19 14:28:31.000000 cesnet-datazoo-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-19 14:29:17.688149 cesnet-datazoo-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.728378 cesnet-datazoo-0.1.2/
+-rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet-datazoo-0.1.2/LICENCE
+-rw-rw-rw-   0        0        0    12573 2024-04-08 09:41:04.728378 cesnet-datazoo-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10994 2024-03-19 11:54:16.000000 cesnet-datazoo-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.682206 cesnet-datazoo-0.1.2/cesnet_datazoo/
+-rw-rw-rw-   0        0        0        0 2023-09-04 15:14:00.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/__init__.py
+-rw-rw-rw-   0        0        0    38035 2024-04-05 08:44:24.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/config.py
+-rw-rw-rw-   0        0        0     1294 2024-03-26 11:19:49.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.707007 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/
+-rw-rw-rw-   0        0        0      443 2023-10-09 14:50:14.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/__init__.py
+-rw-rw-rw-   0        0        0    46458 2024-04-05 09:42:58.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/cesnet_dataset.py
+-rw-rw-rw-   0        0        0     3617 2024-03-13 15:20:57.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/datasets.py
+-rw-rw-rw-   0        0        0    29154 2024-03-13 15:20:40.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/datasets_constants.py
+-rw-rw-rw-   0        0        0     1854 2024-03-14 10:53:21.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/loaders.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.714183 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/
+-rw-rw-rw-   0        0        0        0 2023-08-21 14:08:44.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/__init__.py
+-rw-rw-rw-   0        0        0     1608 2024-03-13 16:30:28.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/dataset_metadata.py
+-rw-rw-rw-   0        0        0     2175 2024-03-19 11:54:21.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/metadata.csv
+-rw-rw-rw-   0        0        0    15137 2024-03-14 10:55:15.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/statistics.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.716532 cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/
+-rw-rw-rw-   0        0        0        0 2023-08-17 21:32:34.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/__init__.py
+-rw-rw-rw-   0        0        0     4040 2023-10-30 20:24:25.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/classification_report.py
+-rw-rw-rw-   0        0        0     1303 2024-03-13 15:46:01.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/provider_metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.720940 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:24:29.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/__init__.py
+-rw-rw-rw-   0        0        0     1411 2023-10-30 20:40:56.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/apps_split.py
+-rw-rw-rw-   0        0        0     5083 2024-03-19 14:07:14.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/data_scalers.py
+-rw-rw-rw-   0        0        0    13011 2024-03-26 09:58:57.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/indices_setup.py
+-rw-rw-rw-   0        0        0    17881 2024-04-05 09:43:19.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/pytables_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.725376 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:35:45.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/__init__.py
+-rw-rw-rw-   0        0        0     2462 2024-04-04 20:29:42.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/class_info.py
+-rw-rw-rw-   0        0        0     1441 2024-02-20 11:51:54.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/download.py
+-rw-rw-rw-   0        0        0      642 2023-09-01 13:43:06.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/fileutils.py
+-rw-rw-rw-   0        0        0      575 2023-09-26 08:58:11.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/random.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.726376 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/
+-rw-rw-rw-   0        0        0    12573 2024-04-08 09:41:04.000000 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2024-04-08 09:41:04.000000 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 09:41:04.000000 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      238 2024-04-08 09:41:04.000000 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 09:41:04.000000 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1792 2024-04-05 08:37:24.000000 cesnet-datazoo-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 09:41:04.729530 cesnet-datazoo-0.1.2/setup.cfg
```

### Comparing `cesnet-datazoo-0.1.1/LICENCE` & `cesnet-datazoo-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/PKG-INFO` & `cesnet-datazoo-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-datazoo
-Version: 0.1.1
+Version: 0.1.2
 Summary: A toolkit for large network traffic datasets
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-datazoo
 Project-URL: Documentation, https://cesnet.github.io/cesnet-datazoo/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-datazoo/issues
```

### Comparing `cesnet-datazoo-0.1.1/README.md` & `cesnet-datazoo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/config.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         flowstats_features_phist: Taken from `dataset.metadata.packet_histograms` if `use_packet_histograms` is true, otherwise an empty list.
         other_fields: Taken from `dataset.metadata.other_fields` if `return_other_fields` is true, otherwise an empty list.
 
     # Configuration options
 
     Attributes:
         need_train_set: Use to disable the train set. `Default: True`
-        need_val_set: Use to disable the validation set. When `need_train_set` is false, the validation set will also be disabled. `Default: True`
+        need_val_set: Use to disable the validation set. `Default: True`
         need_test_set: Use to disable the test set. `Default: True`
         train_period_name: Name of the train period. See [instructions][config.DatasetConfig--how-to-configure-train-validation-and-test-sets].
         train_dates: Dates used for creating a train set.
         train_dates_weigths: To use a non-uniform distribution of samples across train dates.
         val_approach: How a validation set should be created. Either split train data into train and validation or have a separate validation period. `Default: SPLIT_FROM_TRAIN`
         train_val_split_fraction: The fraction of validation samples when splitting from the train set. `Default: 0.2`
         val_period_name: Name of the validation period. See [instructions][config.DatasetConfig--how-to-configure-train-validation-and-test-sets].
@@ -157,15 +157,15 @@
         random_state: Fix all random processes performed during dataset initialization. `Default: 420`
         fold_id: To perform N-fold cross-validation, set this to `1..N`. Each fold will use the same configuration but a different random seed. `Default: 0`
         train_workers: Number of workers for loading train data. `0` means that the data will be loaded in the main process. `Default: 4`
         test_workers: Number of workers for loading test data. `0` means that the data will be loaded in the main process. `Default: 1`
         val_workers: Number of workers for loading validation data. `0` means that the data will be loaded in the main process. `Default: 1`
         batch_size: Number of samples per batch. `Default: 192`
         test_batch_size: Number of samples per batch for loading validation and test data. `Default: 2048`
-        preload_val: Whether to dump the validation set with `numpy.savez_compressed` and preload it in future runs. Useful when running a lot of experiments with the same dataset configuration. `Default: True`
+        preload_val: Whether to dump the validation set with `numpy.savez_compressed` and preload it in future runs. Useful when running a lot of experiments with the same dataset configuration. `Default: False`
         preload_test: Whether to dump the test set with `numpy.savez_compressed` and preload it in future runs. `Default: False`
         train_size: Size of the train set. See [instructions][config.DatasetConfig--how-to-configure-train-validation-and-test-sets]. `Default: all`
         val_known_size: Size of the validation set. See [instructions][config.DatasetConfig--how-to-configure-train-validation-and-test-sets]. `Default: all`
         test_known_size: Size of the test set. See [instructions][config.DatasetConfig--how-to-configure-train-validation-and-test-sets]. `Default: all`
         val_unknown_size: Size of the unknown classes validation set. Use for evaluation in the open-world setting. `Default: 0`
         test_unknown_size: Size of the unknown classes test set. Use for evaluation in the open-world setting. `Default: 0`
         train_dataloader_order: Whether to load train data in sequential or random order. `Default: RANDOM`
@@ -234,15 +234,15 @@
     random_state: int = 420
     fold_id: int = 0
     train_workers: int = 4
     test_workers: int = 1
     val_workers: int = 1
     batch_size: int = 192
     test_batch_size: int = 2048
-    preload_val: bool = True
+    preload_val: bool = False
     preload_test: bool = False
     train_size: int | Literal["all"] = "all"
     val_known_size: int | Literal["all"] = "all"
     test_known_size: int | Literal["all"] = "all"
     val_unknown_size: int | Literal["all"] = 0
     test_unknown_size: int | Literal["all"] = 0
     train_dataloader_order: DataLoaderOrder = DataLoaderOrder.RANDOM
@@ -264,15 +264,14 @@
         """
         self.data_root = dataset.data_root
         self.servicemap_path = dataset.servicemap_path
         self.database_filename = dataset.database_filename
         self.database_path = dataset.database_path
 
         if not self.need_train_set:
-            self.need_val_set = False
             if self.apps_selection != AppSelection.FIXED:
                 raise ValueError("Application selection has to be fixed when need_train_set is false")
             if (len(self.train_dates) > 0 or self.train_period_name != ""):
                 raise ValueError("train_dates and train_period_name cannot be specified when need_train_set is false")
         else:
             # Configure train dates
             if len(self.train_dates) > 0 and self.train_period_name == "":
@@ -295,25 +294,32 @@
                 if self.test_period_name not in dataset.time_periods:
                     raise ValueError(f"Unknown test_period_name {self.test_period_name}. Use time period available in dataset.time_periods")
                 self.test_dates = dataset.time_periods[self.test_period_name]
             if len(self.test_dates) == 0 and self.test_period_name == "":
                 self.test_period_name = dataset.default_test_period_name
                 self.test_dates = dataset.time_periods[dataset.default_test_period_name]
         # Configure val dates
-        if (not self.need_val_set or self.val_approach == ValidationApproach.SPLIT_FROM_TRAIN) and (len(self.val_dates) > 0 or self.val_period_name != ""):
-            raise ValueError("val_dates and val_period_name cannot be specified when need_val_set is false or the validation approach is split-from-train")
-        if self.val_approach == ValidationApproach.VALIDATION_DATES:
-            if len(self.val_dates) > 0 and self.val_period_name == "":
-                raise ValueError("val_period_name has to be specified when val_dates are set")
-            if len(self.val_dates) == 0 and self.val_period_name != "":
-                if self.val_period_name not in dataset.time_periods:
-                    raise ValueError(f"Unknown val_period_name {self.val_period_name}. Use time period available in dataset.time_periods")
-                self.val_dates = dataset.time_periods[self.val_period_name]
-            if len(self.val_dates) == 0 and self.val_period_name == "":
-                raise ValueError("val_period_name and val_dates (or val_period_name from dataset.time_periods) have to be specified when the validation approach is validation-dates")
+        if not self.need_val_set:
+            if len(self.val_dates) > 0 or self.val_period_name != "" or self.val_approach != ValidationApproach.SPLIT_FROM_TRAIN:
+                raise ValueError("val_dates, val_period_name, and val_approach cannot be specified when need_val_set is false")
+        else:
+            if self.val_approach == ValidationApproach.SPLIT_FROM_TRAIN:
+                if len(self.val_dates) > 0 or self.val_period_name != "":
+                    raise ValueError("val_dates and val_period_name cannot be specified when the validation approach is split-from-train")
+                if not self.need_train_set:
+                    raise ValueError("Cannot use the split-from-train validation approach when need_train_set is false. Either use the validation-dates approach or set need_val_set to false.")
+            elif self.val_approach == ValidationApproach.VALIDATION_DATES:
+                if len(self.val_dates) > 0 and self.val_period_name == "":
+                    raise ValueError("val_period_name has to be specified when val_dates are set")
+                if len(self.val_dates) == 0 and self.val_period_name != "":
+                    if self.val_period_name not in dataset.time_periods:
+                        raise ValueError(f"Unknown val_period_name {self.val_period_name}. Use time period available in dataset.time_periods")
+                    self.val_dates = dataset.time_periods[self.val_period_name]
+                if len(self.val_dates) == 0 and self.val_period_name == "":
+                    raise ValueError("val_period_name and val_dates (or val_period_name from dataset.time_periods) have to be specified when the validation approach is validation-dates")
         # Check if train, val, and test dates are available in the dataset
         bad_train_dates = [t for t in self.train_dates if t not in dataset.available_dates]
         bad_val_dates = [t for t in self.val_dates if t not in dataset.available_dates]
         bad_test_dates = [t for t in self.test_dates if t not in dataset.available_dates]
         if len(bad_train_dates) > 0:
             raise ValueError(f"Bad train dates {bad_train_dates}. Use dates available in dataset.available_dates (collection period {dataset.metadata.collection_period})" \
                             + (f". These dates are missing from the dataset collection period {dataset.metadata.missing_dates_in_collection_period}" if dataset.metadata.missing_dates_in_collection_period else ""))
@@ -322,20 +328,19 @@
                             + (f". These dates are missing from the dataset collection period {dataset.metadata.missing_dates_in_collection_period}" if dataset.metadata.missing_dates_in_collection_period else ""))
         if len(bad_test_dates) > 0:
             raise ValueError(f"Bad test dates {bad_test_dates}. Use dates available in dataset.available_dates (collection period {dataset.metadata.collection_period})" \
                             + (f". These dates are missing from the dataset collection period {dataset.metadata.missing_dates_in_collection_period}" if dataset.metadata.missing_dates_in_collection_period else ""))
         # Check time order of train, val, and test periods
         train_dates = [datetime.strptime(date_str, "%Y%m%d").date() for date_str in self.train_dates]
         test_dates = [datetime.strptime(date_str, "%Y%m%d").date() for date_str in self.test_dates]
-        if len(train_dates) > 0 and len(test_dates) > 0  and min(test_dates) <= max(train_dates):
+        if len(train_dates) > 0 and len(test_dates) > 0 and min(test_dates) <= max(train_dates):
             warnings.warn(f"Some test dates ({min(test_dates).strftime('%Y%m%d')}) are before or equal to the last train date ({max(train_dates).strftime('%Y%m%d')}). This might lead to improper evaluation and should be avoided.")
         if self.val_approach == ValidationApproach.VALIDATION_DATES:
-            # Train dates are guaranteed to be set
             val_dates = [datetime.strptime(date_str, "%Y%m%d").date() for date_str in self.val_dates]
-            if min(val_dates) <= max(train_dates):
+            if len(train_dates) > 0 and min(val_dates) <= max(train_dates):
                 warnings.warn(f"Some validation dates ({min(val_dates).strftime('%Y%m%d')}) are before or equal to the last train date ({max(train_dates).strftime('%Y%m%d')}). This might lead to improper evaluation and should be avoided.")
             if len(test_dates) > 0 and min(test_dates) <= max(val_dates):
                 warnings.warn(f"Some test dates ({min(test_dates).strftime('%Y%m%d')}) are before or equal to the last validation date ({max(val_dates).strftime('%Y%m%d')}). This might lead to improper evaluation and should be avoided.")
         # Configure features
         self.flowstats_features = dataset.metadata.flowstats_features
         self.flowstats_features_boolean = dataset.metadata.flowstats_features_boolean
         self.other_fields = dataset.metadata.other_fields if self.return_other_fields else []
@@ -471,15 +476,15 @@
         return feature_names
 
     def _get_train_tables_paths(self) -> list[str]:
         return list(map(lambda t: f"/flows/D{t}", self.train_dates))
 
     def _get_val_tables_paths(self) -> list[str]:
         if self.val_approach == ValidationApproach.SPLIT_FROM_TRAIN:
-            return list(map(lambda t: f"/flows/D{t}", self.train_dates))
+            return self._get_train_tables_paths()
         return list(map(lambda t: f"/flows/D{t}", self.val_dates))
 
     def _get_test_tables_paths(self) -> list[str]:
         return list(map(lambda t: f"/flows/D{t}", self.test_dates))
 
     def _get_train_data_hash(self) -> str:
         train_data_params = self._get_train_data_params()
```

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/constants.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # Features
 FLOWSTATS_TO_SCALE =  ["BYTES", "BYTES_REV", "PACKETS", "PACKETS_REV", "PPI_LEN", "PPI_ROUNDTRIPS", "PPI_DURATION", "DURATION"]
 FLOWSTATS_NO_CLIP = ["DURATION", "PPI_LEN", "PPI_ROUNDTRIPS", "PPI_DURATION"]
 SELECTED_TCP_FLAGS = ["FLAG_CWR", "FLAG_CWR_REV", "FLAG_ECE", "FLAG_ECE_REV", "FLAG_PSH_REV", "FLAG_RST", "FLAG_RST_REV", "FLAG_FIN", "FLAG_FIN_REV"]
 PHIST_BIN_COUNT = 8
 
 # Column names
+ID_COLUMN = "ID"
 APP_COLUMN = "APP"
 CATEGORY_COLUMN = "CATEGORY"
 PPI_COLUMN = "PPI"
 TLS_SNI_COLUMN = "TLS_SNI"
 QUIC_SNI_COLUMN = "QUIC_SNI"
 
 # Servicemap constants
```

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/cesnet_dataset.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/cesnet_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from cesnet_datazoo.pytables_data.apps_split import is_background_app
 from cesnet_datazoo.pytables_data.data_scalers import fit_scalers
 from cesnet_datazoo.pytables_data.indices_setup import (IndicesTuple, compute_known_app_counts,
                                                         compute_unknown_app_counts,
                                                         date_weight_sample_train_indices,
                                                         init_or_load_test_indices,
                                                         init_or_load_train_indices,
-                                                        init_or_load_val_indices,
+                                                        init_or_load_val_indices, no_indices,
                                                         subset_and_sort_indices)
 from cesnet_datazoo.pytables_data.pytables_dataset import PyTablesDataset, worker_init_fn
 from cesnet_datazoo.utils.class_info import ClassInfo, create_class_info
 from cesnet_datazoo.utils.download import resumable_download, simple_download
 from cesnet_datazoo.utils.random import RandomizedSection, get_fresh_random_generator
 
 DATAFRAME_SAMPLES_WARNING_THRESHOLD = 20_000_000
@@ -533,18 +533,18 @@
                     num_samples = dataset_config.train_size + dataset_config.val_known_size
                 else:
                     num_samples = dataset_config.train_size
                 if num_samples > len(train_indices):
                     raise ValueError(f"Requested number of samples for weight sampling ({num_samples}) is larger than the number of available train samples ({len(train_indices)})")
                 train_indices = date_weight_sample_train_indices(dataset_config=dataset_config, train_indices=train_indices, num_samples=num_samples)
         elif dataset_config.apps_selection == AppSelection.FIXED:
-            known_apps = dataset_config.apps_selection_fixed_known
-            unknown_apps = dataset_config.apps_selection_fixed_unknown
-            train_indices = np.zeros((0,3), dtype=np.int64)
-            train_unknown_indices = np.zeros((0,3), dtype=np.int64)
+            known_apps = sorted(dataset_config.apps_selection_fixed_known)
+            unknown_apps = sorted(dataset_config.apps_selection_fixed_unknown)
+            train_indices = no_indices()
+            train_unknown_indices = no_indices()
         else:
             raise ValueError("Either need train set or the fixed application selection")
         # Initialize validation set
         if dataset_config.need_val_set:
             if dataset_config.val_approach == ValidationApproach.VALIDATION_DATES:
                 val_known_indices, val_unknown_indices, val_data_path = init_or_load_val_indices(dataset_config=dataset_config,
                                                                                                  known_apps=known_apps,
@@ -573,27 +573,27 @@
                     if dataset_config.val_known_size != "all" and dataset_config.val_known_size > len(train_indices):
                         raise ValueError(f"Requested validation size ({dataset_config.val_known_size}) is larger than the number of available train samples ({len(train_indices)})")
                     train_indices, val_known_indices = train_test_split(train_indices,
                                                                         train_size=dataset_config.train_size if dataset_config.train_size != "all" else None,
                                                                         test_size=dataset_config.val_known_size if dataset_config.val_known_size != "all" else None,
                                                                         stratify=train_labels, shuffle=True, random_state=train_val_rng)
         else:
-            val_known_indices = np.zeros((0,3), dtype=np.int64)
-            val_unknown_indices = np.zeros((0,3), dtype=np.int64)
+            val_known_indices = no_indices()
+            val_unknown_indices = no_indices()
             val_data_path = None
         # Initialize test set
         if dataset_config.need_test_set:
             test_known_indices, test_unknown_indices, test_data_path = init_or_load_test_indices(dataset_config=dataset_config,
                                                                                                  known_apps=known_apps,
                                                                                                  unknown_apps=unknown_apps,
                                                                                                  tables_app_enum=self._tables_app_enum,
                                                                                                  disable_indices_cache=disable_indices_cache,)
         else:
-            test_known_indices = np.zeros((0,3), dtype=np.int64)
-            test_unknown_indices = np.zeros((0,3), dtype=np.int64)
+            test_known_indices = no_indices()
+            test_unknown_indices = no_indices()
             test_data_path = None
         # Fit scalers if needed
         if (dataset_config.ppi_transform is not None and dataset_config.ppi_transform.needs_fitting or
             dataset_config.flowstats_transform is not None and dataset_config.flowstats_transform.needs_fitting):
             if not dataset_config.need_train_set:
                 raise ValueError("Train set is needed to fit the scalers. Provide pre-fitted scalers.")
             fit_scalers(dataset_config=dataset_config, train_indices=train_indices)
@@ -632,15 +632,15 @@
                 flowstats_phist_transform=dataset_config.flowstats_phist_transform,
                 target_transform=encode_labels_with_unknown_fn,
                 return_tensors=dataset_config.return_tensors,)
         if dataset_config.need_val_set:
             assert val_data_path is not None
             val_dataset = PyTablesDataset(
                 database_path=dataset_config.database_path,
-                tables_paths=dataset_config._get_train_tables_paths(),
+                tables_paths=dataset_config._get_val_tables_paths(),
                 indices=dataset_indices.val_known_indices,
                 tables_app_enum=self._tables_app_enum,
                 tables_cat_enum=self._tables_cat_enum,
                 flowstats_features=dataset_config.flowstats_features,
                 flowstats_features_boolean=dataset_config.flowstats_features_boolean,
                 flowstats_features_phist=dataset_config.flowstats_features_phist,
                 other_fields=self.dataset_config.other_fields,
```

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/datasets.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/datasets_constants.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/datasets_constants.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/loaders.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/loaders.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/metadata/dataset_metadata.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/metadata/metadata.csv` & `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/metadata.csv`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/datasets/statistics.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/statistics.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/metrics/classification_report.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/classification_report.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/metrics/provider_metrics.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/provider_metrics.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/pytables_data/apps_split.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/apps_split.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/pytables_data/data_scalers.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/data_scalers.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/pytables_data/indices_setup.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/indices_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                                                                    tables_app_enum=tables_app_enum,
                                                                    rng=get_fresh_random_generator(dataset_config=dataset_config, section=RandomizedSection.INIT_VAL_INIDICES))
         if not disable_indices_cache:
             yaml_dump(dataclasses.asdict(val_data_params), os.path.join(val_data_path, TEST_DATA_PARAMS_FILE))
             np.save(os.path.join(val_data_path, "val_known_indices.npy"), val_known_indices)
             np.save(os.path.join(val_data_path, "val_unknown_indices.npy"), val_unknown_indices)
     else:
-        val_known_indices = np.load(os.path.join(val_data_path, "val_known_indices.npu"))
+        val_known_indices = np.load(os.path.join(val_data_path, "val_known_indices.npy"))
         val_unknown_indices = np.load(os.path.join(val_data_path, "val_unknown_indices.npy"))
     return val_known_indices, val_unknown_indices, val_data_path
 
 def init_or_load_test_indices(dataset_config: DatasetConfig, known_apps: list[str], unknown_apps: list[str], tables_app_enum: dict[int, str], disable_indices_cache: bool) -> tuple[np.ndarray, np.ndarray, str]:
     test_data_params, test_data_path = dataset_config._get_test_data_params_and_path(known_apps=known_apps, unknown_apps=unknown_apps)
     init_test_data(test_data_path)
     if not os.path.isfile(os.path.join(test_data_path, TEST_DATA_PARAMS_FILE)):
@@ -158,7 +158,10 @@
     os.makedirs(train_data_path, exist_ok=True)
     os.makedirs(os.path.join(train_data_path, "transforms"), exist_ok=True)
     os.makedirs(os.path.join(train_data_path, "preload"), exist_ok=True)
 
 def init_test_data(test_data_path: str):
     os.makedirs(test_data_path, exist_ok=True)
     os.makedirs(os.path.join(test_data_path, "preload"), exist_ok=True)
+
+def no_indices() -> np.ndarray:
+    return np.zeros((0,3), dtype=np.int64)
```

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/pytables_data/pytables_dataset.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/pytables_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 import torch
 from numpy.lib.recfunctions import structured_to_unstructured
 from torch.utils.data import Dataset
 from typing_extensions import assert_never
 
 from cesnet_datazoo.config import (AppSelection, MinTrainSamplesCheck, TestDataParams,
                                    TrainDataParams)
-from cesnet_datazoo.constants import APP_COLUMN, INDICES_INDEX_POS, INDICES_TABLE_POS, PPI_COLUMN
+from cesnet_datazoo.constants import (APP_COLUMN, INDICES_INDEX_POS, INDICES_TABLE_POS, PPI_COLUMN,
+                                      QUIC_SNI_COLUMN, TLS_SNI_COLUMN)
 from cesnet_datazoo.pytables_data.apps_split import (is_background_app,
                                                      split_apps_topx_with_provider_groups)
 
 log = logging.getLogger(__name__)
 
 
 class PyTablesDataset(Dataset):
@@ -62,14 +63,15 @@
         self.ppi_channels = ppi_channels
         self.ppi_transform = ppi_transform
         self.flowstats_transform = flowstats_transform
         self.flowstats_phist_transform = flowstats_phist_transform
         self.target_transform = target_transform
         self.return_tensors = return_tensors
         self.return_all_fields = return_all_fields
+        self.sni_column = TLS_SNI_COLUMN if TLS_SNI_COLUMN in self.other_fields else QUIC_SNI_COLUMN if QUIC_SNI_COLUMN in self.other_fields else None
 
         self.preload = preload
         self.preload_blob = preload_blob
 
     def __getitem__(self, batch_idx):
         # log.debug(f"worker {self.worker_id}: __getitem__")
         if self.preload:
@@ -175,15 +177,15 @@
     database, train_tables = load_database(database_path, tables_paths=train_data_params.train_tables_paths)
     inverted_tables_app_enum = {v: k for k, v in tables_app_enum.items()}
     all_app_labels = {}
     app_counts = pd.Series(dtype="int64")
     start_time = time.time()
     for i, table_path in enumerate(train_data_params.train_tables_paths):
         all_app_labels[i] = train_tables[i].read(field=APP_COLUMN)
-        log.info(f"Reading app column for train table {table_path} took {time.time() - start_time:.2f} seconds"); start_time = time.time()
+        log.info(f"Reading app column for table {table_path} took {time.time() - start_time:.2f} seconds"); start_time = time.time()
         app_counts = app_counts.add(pd.Series(all_app_labels[i]).value_counts(), fill_value=0)
     database.close()
     # Handle disabled apps and apps with less than min_samples_per_app samples
     if len(train_data_params.disabled_apps) > 0:
         log.info(f"Disabled applications in dataset config: {sorted(train_data_params.disabled_apps)}")
     disabled_apps_ids = [inverted_tables_app_enum[app] for app in train_data_params.disabled_apps]
     min_samples_apps_ids = set(app_counts[app_counts<train_data_params.min_train_samples_per_app].index.tolist())
@@ -219,40 +221,42 @@
                 unknown_apps = train_data_params.apps_selection_background_unknown
                 known_apps = [app for app in sorted_apps if not (is_background_app(app) or app in unknown_apps)]
         else: assert_never(train_data_params.apps_selection)
         log.info(f"Selected {len(known_apps)} known applications and {len(unknown_apps)} unknown applications")
     else:
         known_apps = train_data_params.apps_selection_fixed_known
         unknown_apps = train_data_params.apps_selection_fixed_unknown
+    known_apps = sorted(known_apps)
+    unknown_apps = sorted(unknown_apps)
     known_apps_ids = [inverted_tables_app_enum[app] for app in known_apps]
     unknown_apps_ids = [inverted_tables_app_enum[app] for app in unknown_apps]
 
     train_known_indices, train_unknown_indices = convert_dict_indices(base_indices=base_indices, base_labels=base_labels, known_apps_ids=known_apps_ids, unknown_apps_ids=unknown_apps_ids)
     rng.shuffle(train_known_indices)
     rng.shuffle(train_unknown_indices)
-    log.info(f"Processing train indices took {time.time() - start_time:.2f} seconds"); start_time = time.time()
+    log.info(f"Processing indices took {time.time() - start_time:.2f} seconds"); start_time = time.time()
     return train_known_indices, train_unknown_indices, known_apps, unknown_apps
 
 def init_test_indices(test_data_params: TestDataParams, database_path: str, tables_app_enum: dict[int, str], rng: np.random.RandomState) -> tuple[np.ndarray, np.ndarray]:
     database, test_tables = load_database(database_path, tables_paths=test_data_params.test_tables_paths)
     inverted_tables_app_enum = {v: k for k, v in tables_app_enum.items()}
     base_labels = {}
     base_indices = {}
     start_time = time.time()
     for i, table_path in enumerate(test_data_params.test_tables_paths):
         base_labels[i] = test_tables[i].read(field=APP_COLUMN)
-        log.info(f"Reading app column for test table {table_path} took {time.time() - start_time:.2f} seconds"); start_time = time.time()
+        log.info(f"Reading app column for table {table_path} took {time.time() - start_time:.2f} seconds"); start_time = time.time()
         base_indices[i] = np.arange(len(test_tables[i]))
     database.close()
     known_apps_ids = [inverted_tables_app_enum[app] for app in test_data_params.known_apps]
     unknown_apps_ids = [inverted_tables_app_enum[app] for app in test_data_params.unknown_apps]
     test_known_indices, test_unknown_indices = convert_dict_indices(base_indices=base_indices, base_labels=base_labels, known_apps_ids=known_apps_ids, unknown_apps_ids=unknown_apps_ids)
     rng.shuffle(test_known_indices)
     rng.shuffle(test_unknown_indices)
-    log.info(f"Processing test indices took {time.time() - start_time:.2f} seconds"); start_time = time.time()
+    log.info(f"Processing indices took {time.time() - start_time:.2f} seconds"); start_time = time.time()
     return test_known_indices, test_unknown_indices
 
 def load_database(database_path: str, tables_paths: Optional[list[str]] = None, mode: str = "r") -> tuple[tb.File, dict[int, Any]]: # dict[int, tb.Table]
     database = tb.open_file(database_path, mode=mode)
     if tables_paths is None:
         tables_paths = list(map(lambda x: x._v_pathname, iter(database.get_node(f"/flows"))))
     tables = {}
```

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/utils/class_info.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/utils/class_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,14 @@
     group_matrix: np.ndarray
     has_provider: dict[str, bool]
     provider_mapping: dict[str, str]
     provider_members: dict[str, list[str]]
     categories_mapping: dict[str, Optional[str]]
 
 def create_class_info(servicemap: Any, encoder: LabelEncoder, known_apps: list[str], unknown_apps: list[str]) -> ClassInfo:
-    known_apps = sorted(known_apps)
-    unknown_apps = sorted(unknown_apps)
     target_names_arr = encoder.classes_
     assert known_apps == list(target_names_arr[:-1])
     group_matrix = np.array([[a == b or
                 (a in servicemap.index and b in servicemap.index and
                 not pd.isnull(servicemap.loc[a, SERVICEMAP_PROVIDER_COLUMN]) and not pd.isnull(servicemap.loc[b, SERVICEMAP_PROVIDER_COLUMN]) and
                 servicemap.loc[a, SERVICEMAP_PROVIDER_COLUMN] == servicemap.loc[b, SERVICEMAP_PROVIDER_COLUMN])
                 for a in target_names_arr] for b in target_names_arr])
```

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/utils/download.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/utils/download.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/utils/fileutils.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo/utils/random.py` & `cesnet-datazoo-0.1.2/cesnet_datazoo/utils/random.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo.egg-info/PKG-INFO` & `cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-datazoo
-Version: 0.1.1
+Version: 0.1.2
 Summary: A toolkit for large network traffic datasets
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-datazoo
 Project-URL: Documentation, https://cesnet.github.io/cesnet-datazoo/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-datazoo/issues
```

### Comparing `cesnet-datazoo-0.1.1/cesnet_datazoo.egg-info/SOURCES.txt` & `cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.1/pyproject.toml` & `cesnet-datazoo-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cesnet-datazoo"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
 ]
 maintainers = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
```

