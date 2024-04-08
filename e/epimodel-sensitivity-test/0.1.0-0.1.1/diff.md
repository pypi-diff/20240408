# Comparing `tmp/epimodel_sensitivity_test-0.1.0.tar.gz` & `tmp/epimodel_sensitivity_test-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epimodel_sensitivity_test-0.1.0.tar", last modified: Sat Apr  6 21:27:37 2024, max compression
+gzip compressed data, was "epimodel_sensitivity_test-0.1.1.tar", last modified: Mon Apr  8 18:33:30 2024, max compression
```

## Comparing `epimodel_sensitivity_test-0.1.0.tar` & `epimodel_sensitivity_test-0.1.1.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.378243 epimodel_sensitivity_test-0.1.0/
--rw-rw-rw-   0        0        0     2153 2024-04-06 21:27:37.378243 epimodel_sensitivity_test-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1698 2024-04-05 10:47:20.000000 epimodel_sensitivity_test-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.268886 epimodel_sensitivity_test-0.1.0/epimodel_sensitivity_test.egg-info/
--rw-rw-rw-   0        0        0     2153 2024-04-06 21:27:37.000000 epimodel_sensitivity_test-0.1.0/epimodel_sensitivity_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1763 2024-04-06 21:27:37.000000 epimodel_sensitivity_test-0.1.0/epimodel_sensitivity_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 21:27:37.000000 epimodel_sensitivity_test-0.1.0/epimodel_sensitivity_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-06 21:27:37.000000 epimodel_sensitivity_test-0.1.0/epimodel_sensitivity_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-06 21:27:37.000000 epimodel_sensitivity_test-0.1.0/epimodel_sensitivity_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.268886 epimodel_sensitivity_test-0.1.0/examples/
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.284501 epimodel_sensitivity_test-0.1.0/examples/SEIHR_2_age_group/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/SEIHR_2_age_group/__init__.py
--rw-rw-rw-   0        0        0      962 2024-04-05 13:00:08.000000 epimodel_sensitivity_test-0.1.0/examples/SEIHR_2_age_group/seihr_2_ag_main.py
--rw-rw-rw-   0        0        0     1698 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/SEIHR_2_age_group/simulation_seihr.py
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.284501 epimodel_sensitivity_test-0.1.0/examples/SEIR_no_age_groups/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/SEIR_no_age_groups/__init__.py
--rw-rw-rw-   0        0        0      691 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/SEIR_no_age_groups/model_seir.py
--rw-rw-rw-   0        0        0     1006 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/SEIR_no_age_groups/sampler_seir.py
--rw-rw-rw-   0        0        0      714 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/SEIR_no_age_groups/seir_no_ag_main.py
--rw-rw-rw-   0        0        0     1350 2024-04-05 15:31:35.000000 epimodel_sensitivity_test-0.1.0/examples/SEIR_no_age_groups/simulation_seir.py
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.300115 epimodel_sensitivity_test-0.1.0/examples/contact_sensitivity/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/contact_sensitivity/__init__.py
--rw-rw-rw-   0        0        0      406 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/contact_sensitivity/contact_main.py
--rw-rw-rw-   0        0        0      562 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/contact_sensitivity/sampler_contact.py
--rw-rw-rw-   0        0        0     3171 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/contact_sensitivity/sensitivity_model_contact.py
--rw-rw-rw-   0        0        0     3768 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/contact_sensitivity/simulation_contact.py
--rw-rw-rw-   0        0        0      397 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/test.py
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.315741 epimodel_sensitivity_test-0.1.0/examples/utils/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/utils/__init__.py
--rw-rw-rw-   0        0        0     3456 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/utils/dataloader_16_ag.py
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.331364 epimodel_sensitivity_test-0.1.0/examples/vaccinated_sensitivity/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/vaccinated_sensitivity/__init__.py
--rw-rw-rw-   0        0        0     2771 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/vaccinated_sensitivity/sampler_vaccinated.py
--rw-rw-rw-   0        0        0     1112 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py
--rw-rw-rw-   0        0        0     3688 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/vaccinated_sensitivity/simulation_vacc.py
--rw-rw-rw-   0        0        0      428 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/examples/vaccinated_sensitivity/vaccinated_main.py
--rw-rw-rw-   0        0        0       42 2024-04-06 21:27:37.378243 epimodel_sensitivity_test-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      811 2024-04-06 21:27:21.000000 epimodel_sensitivity_test-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.331364 epimodel_sensitivity_test-0.1.0/src/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.0/src/__init__.py
--rw-rw-rw-   0        0        0      517 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/src/dataloader.py
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.346990 epimodel_sensitivity_test-0.1.0/src/model/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.0/src/model/__init__.py
--rw-rw-rw-   0        0        0     1205 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/src/model/epidemic_model.py
--rw-rw-rw-   0        0        0    10205 2024-04-05 22:37:32.000000 epimodel_sensitivity_test-0.1.0/src/model/matrix_generator.py
--rw-rw-rw-   0        0        0     3963 2024-04-05 10:30:29.000000 epimodel_sensitivity_test-0.1.0/src/model/model_base.py
--rw-rw-rw-   0        0        0     4707 2024-04-05 16:11:25.000000 epimodel_sensitivity_test-0.1.0/src/model/r0.py
--rw-rw-rw-   0        0        0     5440 2024-04-06 17:24:37.000000 epimodel_sensitivity_test-0.1.0/src/plotter.py
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.362631 epimodel_sensitivity_test-0.1.0/src/sensitivity/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.0/src/sensitivity/__init__.py
--rw-rw-rw-   0        0        0     1137 2024-04-04 14:22:44.000000 epimodel_sensitivity_test-0.1.0/src/sensitivity/prcc.py
--rw-rw-rw-   0        0        0     4608 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/src/sensitivity/sampler_base.py
--rw-rw-rw-   0        0        0     4734 2024-04-05 19:32:24.000000 epimodel_sensitivity_test-0.1.0/src/sensitivity/sensitivity_model_base.py
-drwxrwxrwx   0        0        0        0 2024-04-06 21:27:37.362631 epimodel_sensitivity_test-0.1.0/src/sensitivity/target_calc/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/src/sensitivity/target_calc/__init__.py
--rw-rw-rw-   0        0        0      896 2024-04-05 12:26:45.000000 epimodel_sensitivity_test-0.1.0/src/sensitivity/target_calc/final_size_calc.py
--rw-rw-rw-   0        0        0     1183 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/src/sensitivity/target_calc/output_generator.py
--rw-rw-rw-   0        0        0      913 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/src/sensitivity/target_calc/peak_calc.py
--rw-rw-rw-   0        0        0     3373 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/src/sensitivity/target_calc/target_calc_base.py
--rw-rw-rw-   0        0        0     7804 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.0/src/simulation_base.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:30.153453 epimodel_sensitivity_test-0.1.1/
+-rw-rw-rw-   0        0        0     2153 2024-04-08 18:33:30.153453 epimodel_sensitivity_test-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2024-04-05 10:47:20.000000 epimodel_sensitivity_test-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:29.819688 epimodel_sensitivity_test-0.1.1/epimodel_sensitivity_test.egg-info/
+-rw-rw-rw-   0        0        0     2153 2024-04-08 18:33:29.000000 epimodel_sensitivity_test-0.1.1/epimodel_sensitivity_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1887 2024-04-08 18:33:29.000000 epimodel_sensitivity_test-0.1.1/epimodel_sensitivity_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 18:33:29.000000 epimodel_sensitivity_test-0.1.1/epimodel_sensitivity_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-08 18:33:29.000000 epimodel_sensitivity_test-0.1.1/epimodel_sensitivity_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-08 18:33:29.000000 epimodel_sensitivity_test-0.1.1/epimodel_sensitivity_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:29.819688 epimodel_sensitivity_test-0.1.1/examples/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:29.836466 epimodel_sensitivity_test-0.1.1/examples/SEIHR_2_age_group/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/SEIHR_2_age_group/__init__.py
+-rw-rw-rw-   0        0        0      962 2024-04-05 13:00:08.000000 epimodel_sensitivity_test-0.1.1/examples/SEIHR_2_age_group/seihr_2_ag_main.py
+-rw-rw-rw-   0        0        0     1698 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/SEIHR_2_age_group/simulation_seihr.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:29.853144 epimodel_sensitivity_test-0.1.1/examples/SEIR_no_age_groups/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/SEIR_no_age_groups/__init__.py
+-rw-rw-rw-   0        0        0      691 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/SEIR_no_age_groups/model_seir.py
+-rw-rw-rw-   0        0        0      332 2024-04-08 13:30:52.000000 epimodel_sensitivity_test-0.1.1/examples/SEIR_no_age_groups/sampler_seir.py
+-rw-rw-rw-   0        0        0      714 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/SEIR_no_age_groups/seir_no_ag_main.py
+-rw-rw-rw-   0        0        0     1350 2024-04-05 15:31:35.000000 epimodel_sensitivity_test-0.1.1/examples/SEIR_no_age_groups/simulation_seir.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:29.869690 epimodel_sensitivity_test-0.1.1/examples/contact_sensitivity/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/contact_sensitivity/__init__.py
+-rw-rw-rw-   0        0        0      406 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/contact_sensitivity/contact_main.py
+-rw-rw-rw-   0        0        0      562 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/contact_sensitivity/sampler_contact.py
+-rw-rw-rw-   0        0        0     3171 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/contact_sensitivity/sensitivity_model_contact.py
+-rw-rw-rw-   0        0        0     3768 2024-04-08 14:28:40.000000 epimodel_sensitivity_test-0.1.1/examples/contact_sensitivity/simulation_contact.py
+-rw-rw-rw-   0        0        0      397 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/test.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:29.886309 epimodel_sensitivity_test-0.1.1/examples/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/utils/__init__.py
+-rw-rw-rw-   0        0        0     3456 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/utils/dataloader_16_ag.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:29.986281 epimodel_sensitivity_test-0.1.1/examples/vaccinated_sensitivity/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/vaccinated_sensitivity/__init__.py
+-rw-rw-rw-   0        0        0     2771 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/vaccinated_sensitivity/sampler_vaccinated.py
+-rw-rw-rw-   0        0        0     1112 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py
+-rw-rw-rw-   0        0        0     3688 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/vaccinated_sensitivity/simulation_vacc.py
+-rw-rw-rw-   0        0        0      428 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/examples/vaccinated_sensitivity/vaccinated_main.py
+-rw-rw-rw-   0        0        0       42 2024-04-08 18:33:30.161746 epimodel_sensitivity_test-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      868 2024-04-08 13:16:41.000000 epimodel_sensitivity_test-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:30.036286 epimodel_sensitivity_test-0.1.1/src/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.1/src/__init__.py
+-rw-rw-rw-   0        0        0      517 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/src/dataloader.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:30.052992 epimodel_sensitivity_test-0.1.1/src/model/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.1/src/model/__init__.py
+-rw-rw-rw-   0        0        0     1205 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/src/model/epidemic_model.py
+-rw-rw-rw-   0        0        0    10205 2024-04-05 22:37:32.000000 epimodel_sensitivity_test-0.1.1/src/model/matrix_generator.py
+-rw-rw-rw-   0        0        0     3963 2024-04-05 10:30:29.000000 epimodel_sensitivity_test-0.1.1/src/model/model_base.py
+-rw-rw-rw-   0        0        0     4707 2024-04-05 16:11:25.000000 epimodel_sensitivity_test-0.1.1/src/model/r0.py
+-rw-rw-rw-   0        0        0     5440 2024-04-06 17:24:37.000000 epimodel_sensitivity_test-0.1.1/src/plotter.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:30.086169 epimodel_sensitivity_test-0.1.1/src/sensitivity/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.1/src/sensitivity/__init__.py
+-rw-rw-rw-   0        0        0     1137 2024-04-04 14:22:44.000000 epimodel_sensitivity_test-0.1.1/src/sensitivity/prcc.py
+-rw-rw-rw-   0        0        0     4593 2024-04-08 14:28:40.000000 epimodel_sensitivity_test-0.1.1/src/sensitivity/sampler_base.py
+-rw-rw-rw-   0        0        0     4893 2024-04-08 14:52:25.000000 epimodel_sensitivity_test-0.1.1/src/sensitivity/sensitivity_model_base.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:30.086169 epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/__init__.py
+-rw-rw-rw-   0        0        0     1479 2024-04-08 13:26:57.000000 epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/output_generator.py
+-rw-rw-rw-   0        0        0     1608 2024-04-08 14:34:22.000000 epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/r0calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:33:30.153453 epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/sol_based/
+-rw-rw-rw-   0        0        0        0 2024-04-07 15:24:44.000000 epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/sol_based/__init__.py
+-rw-rw-rw-   0        0        0      906 2024-04-07 15:33:11.000000 epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/sol_based/final_size_calc.py
+-rw-rw-rw-   0        0        0      923 2024-04-07 15:33:11.000000 epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/sol_based/peak_calc.py
+-rw-rw-rw-   0        0        0     3373 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/sol_based/target_calc_base.py
+-rw-rw-rw-   0        0        0     8381 2024-04-08 14:28:40.000000 epimodel_sensitivity_test-0.1.1/src/simulation_base.py
```

### Comparing `epimodel_sensitivity_test-0.1.0/PKG-INFO` & `epimodel_sensitivity_test-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epimodel_sensitivity_test
-Version: 0.1.0
+Version: 0.1.1
 Summary: Efficient sensitivity analysis and evaluation of epidemiological models
 Home-page: https://github.com/KKol21/epimodel_sensitivity
 Author: Kolos Kovács
 Author-email: kovkol21@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `epimodel_sensitivity_test-0.1.0/README.md` & `epimodel_sensitivity_test-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/epimodel_sensitivity_test.egg-info/PKG-INFO` & `epimodel_sensitivity_test-0.1.1/epimodel_sensitivity_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epimodel-sensitivity-test
-Version: 0.1.0
+Version: 0.1.1
 Summary: Efficient sensitivity analysis and evaluation of epidemiological models
 Home-page: https://github.com/KKol21/epimodel_sensitivity
 Author: Kolos Kovács
 Author-email: kovkol21@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `epimodel_sensitivity_test-0.1.0/epimodel_sensitivity_test.egg-info/SOURCES.txt` & `epimodel_sensitivity_test-0.1.1/epimodel_sensitivity_test.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -37,11 +37,13 @@
 src/model/model_base.py
 src/model/r0.py
 src/sensitivity/__init__.py
 src/sensitivity/prcc.py
 src/sensitivity/sampler_base.py
 src/sensitivity/sensitivity_model_base.py
 src/sensitivity/target_calc/__init__.py
-src/sensitivity/target_calc/final_size_calc.py
 src/sensitivity/target_calc/output_generator.py
-src/sensitivity/target_calc/peak_calc.py
-src/sensitivity/target_calc/target_calc_base.py
+src/sensitivity/target_calc/r0calculator.py
+src/sensitivity/target_calc/sol_based/__init__.py
+src/sensitivity/target_calc/sol_based/final_size_calc.py
+src/sensitivity/target_calc/sol_based/peak_calc.py
+src/sensitivity/target_calc/sol_based/target_calc_base.py
```

### Comparing `epimodel_sensitivity_test-0.1.0/examples/SEIHR_2_age_group/seihr_2_ag_main.py` & `epimodel_sensitivity_test-0.1.1/examples/SEIHR_2_age_group/seihr_2_ag_main.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/examples/SEIHR_2_age_group/simulation_seihr.py` & `epimodel_sensitivity_test-0.1.1/examples/SEIHR_2_age_group/simulation_seihr.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/examples/SEIR_no_age_groups/model_seir.py` & `epimodel_sensitivity_test-0.1.1/examples/SEIR_no_age_groups/model_seir.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/examples/SEIR_no_age_groups/seir_no_ag_main.py` & `epimodel_sensitivity_test-0.1.1/examples/SEIR_no_age_groups/seir_no_ag_main.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/examples/SEIR_no_age_groups/simulation_seir.py` & `epimodel_sensitivity_test-0.1.1/examples/SEIR_no_age_groups/simulation_seir.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/examples/contact_sensitivity/sampler_contact.py` & `epimodel_sensitivity_test-0.1.1/examples/contact_sensitivity/sampler_contact.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/examples/contact_sensitivity/sensitivity_model_contact.py` & `epimodel_sensitivity_test-0.1.1/examples/contact_sensitivity/sensitivity_model_contact.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/examples/contact_sensitivity/simulation_contact.py` & `epimodel_sensitivity_test-0.1.1/examples/contact_sensitivity/simulation_contact.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/examples/utils/dataloader_16_ag.py` & `epimodel_sensitivity_test-0.1.1/examples/utils/dataloader_16_ag.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/examples/vaccinated_sensitivity/sampler_vaccinated.py` & `epimodel_sensitivity_test-0.1.1/examples/vaccinated_sensitivity/sampler_vaccinated.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py` & `epimodel_sensitivity_test-0.1.1/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/examples/vaccinated_sensitivity/simulation_vacc.py` & `epimodel_sensitivity_test-0.1.1/examples/vaccinated_sensitivity/simulation_vacc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/setup.py` & `epimodel_sensitivity_test-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='epimodel_sensitivity_test',
-    version='0.1.0',
+    version='0.1.1',
     author='Kolos Kovács',
     author_email='kovkol21@gmail.com',
     description='Efficient sensitivity analysis and evaluation of epidemiological models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/KKol21/epimodel_sensitivity',
     packages=find_packages(),
+    package_data={
+        '': ['*.json', '*.xls']},
     install_requires=[
         "smt~=1.3.0",
         "tqdm==4.51.0",
         "xlrd==1.2.0",
         "torch~=2.0.0",
         "torchode~=0.1.8",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-)
+)
```

### Comparing `epimodel_sensitivity_test-0.1.0/src/dataloader.py` & `epimodel_sensitivity_test-0.1.1/src/dataloader.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/src/model/epidemic_model.py` & `epimodel_sensitivity_test-0.1.1/src/model/epidemic_model.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/src/model/matrix_generator.py` & `epimodel_sensitivity_test-0.1.1/src/model/matrix_generator.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/src/model/model_base.py` & `epimodel_sensitivity_test-0.1.1/src/model/model_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/src/model/r0.py` & `epimodel_sensitivity_test-0.1.1/src/model/r0.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/src/plotter.py` & `epimodel_sensitivity_test-0.1.1/src/plotter.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/src/sensitivity/prcc.py` & `epimodel_sensitivity_test-0.1.1/src/sensitivity/prcc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/src/sensitivity/sampler_base.py` & `epimodel_sensitivity_test-0.1.1/src/sensitivity/sampler_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,14 @@
     def save_output(self, output, output_name: str, filename: str):
         folder_name = self.sim_obj.folder_name
         os.makedirs(folder_name, exist_ok=True)
 
         dirname = os.path.join(folder_name, output_name)
         filename = os.path.join(dirname, f"{output_name}_{filename}")
         os.makedirs(dirname, exist_ok=True)
-        np.savetxt(fname=filename + ".csv", X=output, delimiter=";")
+        np.savetxt(fname=filename + ".csv", X=output)
 
 
 def create_latin_table(n_of_samples, lower, upper):
     bounds = np.array([lower, upper]).T
     sampling = LHS(xlimits=bounds)
     return sampling(n_of_samples)
```

### Comparing `epimodel_sensitivity_test-0.1.0/src/sensitivity/sensitivity_model_base.py` & `epimodel_sensitivity_test-0.1.1/src/sensitivity/sensitivity_model_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,18 @@
     for param, bound in sampled_params_boundaries.items():
         param_dim = len(bound[0]) if isinstance(bound[0], list) else 1
         params_col_idx[param] = last_idx if param_dim == 1 else slice(last_idx, last_idx + param_dim)
         last_idx += param_dim
     return params_col_idx
 
 
+def get_lhs_dict(params: list, lhs_table: torch.Tensor, params_col_idx: dict) -> dict:
+    return {param: lhs_table[:, params_col_idx[param]] for param in params}
+
+
 class SensitivityModelBase(EpidemicModelBase, ABC):
     def __init__(self, sim_obj):
         super().__init__(data=sim_obj.data, **sim_obj.model_struct)
         self.sim_obj = sim_obj
         self.test = sim_obj.test
         self.sim_state = None
 
@@ -89,23 +93,21 @@
         trans_params = [trans["param"] for trans in self.trans_data]
         linear_params = [param for param in spb
                          if param in trans_params + distr_params]
         # Params in T_1
         susc_params = [param for tms_rule in self.tms_rules for param in tms_rule["source"]["params"]]
         transmission_params_left = [param for param in spb if param in susc_params]
         # Params in T_2
-        inf_params = [param for tms_rule in self.tms_rules
-                      for param in tms_rule["infection"]["actors-params"].values()]
+        actor_params = [param for tms_rule in self.tms_rules
+                        for param in tms_rule["infection"]["actors-params"].values()]
+        inf_params = actor_params + [param for tms_rule in self.tms_rules
+                                     for param in tms_rule["infection"]["infection_params"]]
         transmission_params_right = [param for param in spb if param in inf_params] + ["beta"]
 
-        params_col_idx = get_params_col_idx(sampled_params_boundaries=spb)
-
-        def get_lhs_dict(params, lhs_table):
-            return {param: lhs_table[:, params_col_idx[param]] for param in params}
+        pci = get_params_col_idx(sampled_params_boundaries=spb)
 
-        tpl_lhs = get_lhs_dict(transmission_params_left, samples)
-        tpr_lhs = get_lhs_dict(transmission_params_right, samples)
-        tpl_lhs.update(**tpr_lhs) # TODO: This is not the proper way, but it works until new transmission rules are added
-        lp_lhs = get_lhs_dict(linear_params, samples)
-        self.A = self.get_matrix_from_lhs(tpl_lhs, "A") if len(tpl_lhs) > 0 else self.A
-        self.T = self.get_matrix_from_lhs(tpr_lhs, "T") if len(tpr_lhs) > 0 else self.T
-        self.B = self.get_matrix_from_lhs(lp_lhs, "B") if len(lp_lhs) > 0 else self.B
+        tpl_lhs = get_lhs_dict(transmission_params_left, samples, pci)
+        tpr_lhs = get_lhs_dict(transmission_params_right, samples, pci)
+        lp_lhs = get_lhs_dict(linear_params, samples, pci)
+        self.A = self.get_matrix_from_lhs(tpl_lhs, "A") if len(tpl_lhs) > 0 else self.matrix_generator.get_A()
+        self.T = self.get_matrix_from_lhs(tpr_lhs, "T") if len(tpr_lhs) > 0 else self.matrix_generator.get_T()
+        self.B = self.get_matrix_from_lhs(lp_lhs, "B") if len(lp_lhs) > 0 else self.matrix_generator.get_B()
```

### Comparing `epimodel_sensitivity_test-0.1.0/src/sensitivity/target_calc/final_size_calc.py` & `epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/sol_based/final_size_calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 
 from src.sensitivity.sensitivity_model_base import SensitivityModelBase
-from src.sensitivity.target_calc.target_calc_base import TargetCalcBase
+from src.sensitivity.target_calc.sol_based.target_calc_base import TargetCalcBase
 
 
 class FinalSizeCalculator(TargetCalcBase):
     def __init__(self, model: SensitivityModelBase):
         super().__init__(model)
 
     def metric(self, sol, comp: str):
```

### Comparing `epimodel_sensitivity_test-0.1.0/src/sensitivity/target_calc/output_generator.py` & `epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/output_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import numpy as np
 import torch
 
-from src.sensitivity.target_calc.final_size_calc import FinalSizeCalculator
-from src.sensitivity.target_calc.peak_calc import PeakCalculator
+from src.sensitivity.target_calc.sol_based.final_size_calc import FinalSizeCalculator
+from src.sensitivity.target_calc.sol_based.peak_calc import PeakCalculator
+from src.sensitivity.target_calc.r0calculator import R0Calculator
 
 
 class OutputGenerator:
     def __init__(self, sim_obj, variable_params):
         self.batch_size = sim_obj.batch_size
         self.sim_obj = sim_obj
         self.variable_params = variable_params
 
     def get_output(self, lhs_table: np.ndarray) -> dict:
         lhs = torch.from_numpy(lhs_table).float().to(self.sim_obj.device)
         results = {}
         for target in self.sim_obj.target_vars:
-            results[target] = self.calculate_target(lhs, target)
+            if target == "r0":
+                r0calc = R0Calculator(self.sim_obj)
+                results[target] = r0calc.get_output(lhs_table=lhs)
+            else:
+                results[target] = self.calculate_target(lhs_table=lhs, target_var=target)
         return results
 
     def calculate_target(self, lhs_table: torch.Tensor, target_var: str) -> torch.Tensor:
         if target_var.split('_')[1] == "sup":
-            target_calculator = FinalSizeCalculator(self.sim_obj.model)
+            target_calculator = FinalSizeCalculator(model=self.sim_obj.model)
         else:
-            target_calculator = PeakCalculator(self.sim_obj.model)
+            target_calculator = PeakCalculator(model=self.sim_obj.model)
         return target_calculator.get_output(lhs_table=lhs_table,
                                             batch_size=self.batch_size,
                                             target_var=target_var)
```

### Comparing `epimodel_sensitivity_test-0.1.0/src/sensitivity/target_calc/peak_calc.py` & `epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/sol_based/peak_calc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from src.sensitivity.target_calc.target_calc_base import TargetCalcBase
+from src.sensitivity.target_calc.sol_based.target_calc_base import TargetCalcBase
 
 
 class PeakCalculator(TargetCalcBase):
     def __init__(self, model):
         super().__init__(model)
 
     def stopping_condition(self, **kwargs):
```

### Comparing `epimodel_sensitivity_test-0.1.0/src/sensitivity/target_calc/target_calc_base.py` & `epimodel_sensitivity_test-0.1.1/src/sensitivity/target_calc/sol_based/target_calc_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.0/src/simulation_base.py` & `epimodel_sensitivity_test-0.1.1/src/simulation_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -128,30 +128,44 @@
         Calculates PRCC (Partial Rank Correlation Coefficient) values from saved LHS tables and simulation results.
 
         This method reads the saved LHS tables and simulation results for each parameter combination and calculates
         the PRCC values. The PRCC values are saved in separate files in the 'sens_data_"folder_name"/prcc' directory.
 
         """
         folder_name = self.folder_name
-        os.makedirs(f"{folder_name}/prcc", exist_ok=True)
-        filename_without_target = filename[:filename[:filename.rfind("_")].rfind("_")]
-        lhs_table = np.loadtxt(f'{folder_name}/lhs/lhs_{filename_without_target}.csv', delimiter=';')
-        sim_output = np.loadtxt(f'{folder_name}/simulations/simulations_{filename}.csv', delimiter=';')
+        os.makedirs(os.path.join(folder_name, "prcc"), exist_ok=True)
+        if "r0" == filename[-2:]:  # remove _r0
+            filename_without_target = filename[:-3]
+        else:  # remove _comp_sup / _comp_max
+            filename_without_target = filename[:filename[:filename.rfind("_")].rfind("_")]
+        lhs_path = os.path.join(folder_name, f"lhs/lhs_{filename_without_target}.csv")
+        output_path = os.path.join(folder_name, f"simulations/simulations_{filename}.csv")
+        lhs_table = np.loadtxt(lhs_path)
+        sim_output = np.loadtxt(output_path)
 
         prcc = get_prcc_values(np.c_[lhs_table, sim_output.T])
-        np.savetxt(fname=f'{folder_name}/prcc/prcc_{filename}.csv', X=prcc)
+
+        prcc_path = os.path.join(folder_name, f"prcc/prcc_{filename}.csv")
+        np.savetxt(fname=prcc_path, X=prcc)
 
     def calculate_p_values(self, filename, significance=0.05):
-        os.makedirs(self.folder_name + '/p_values', exist_ok=True)
-        prcc = np.loadtxt(fname=f'{self.folder_name}/prcc/prcc_{filename}.csv')
+        p_values_dir = os.path.join(self.folder_name, 'p_values')
+        os.makedirs(p_values_dir, exist_ok=True)
+
+        prcc_path = os.path.join(self.folder_name, f"prcc/prcc_{filename}.csv")
+        prcc = np.loadtxt(fname=prcc_path)
+
         t = prcc * np.sqrt((self.n_samples - 2 - self.n_age) / (1 - prcc ** 2))
         # p-value for 2-sided test
         dof = self.n_samples - 2 - self.n_age
         p_values = 2 * (1 - ss.t.cdf(x=abs(t), df=dof))
-        np.savetxt(fname=f'{self.folder_name}/p_values/p_values_{filename}.csv', X=p_values)
+
+        p_values_path = os.path.join(self.folder_name, f"p_values/p_values_{filename}.csv")
+        np.savetxt(fname=p_values_path, X=p_values)
+
         is_first = True
         if len(p_values) < 30:
             for idx, p_val in enumerate(p_values):
                 if p_val > significance:
                     if is_first:
                         print("\nInsignificant p-values in ", filename, " case: \n")
                         is_first = False
@@ -179,17 +193,22 @@
             for param, idx in pci.items():
                 param_label = get_aged_param_labels(param) if isinstance(spb[param][0], list) else param
                 if isinstance(param_label, list):
                     labels += param_label
                 else:
                     labels.append(param_label)
 
-        os.makedirs(f'{self.folder_name}/prcc_plots', exist_ok=True)
-        prcc = np.loadtxt(fname=f'{self.folder_name}/prcc/prcc_{filename}.csv')
-        p_val = np.loadtxt(fname=f'{self.folder_name}/p_values/p_values_{filename}.csv')
+        prcc_plots_dir = os.path.join(self.folder_name, "prcc_plots")
+        os.makedirs(prcc_plots_dir, exist_ok=True)
+
+        prcc_file = os.path.join(self.folder_name, f"prcc/prcc_{filename}.csv")
+        prcc = np.loadtxt(fname=prcc_file)
+
+        p_values_file = os.path.join(self.folder_name, f"p_values/p_values_{filename}.csv")
+        p_val = np.loadtxt(fname=p_values_file)
 
         generate_tornado_plot(sim_obj=self,
                               labels=labels,
                               prcc=prcc,
                               p_val=p_val,
                               filename=filename)
```

