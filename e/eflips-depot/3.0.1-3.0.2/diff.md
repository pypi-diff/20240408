# Comparing `tmp/eflips_depot-3.0.1.tar.gz` & `tmp/eflips_depot-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_depot-3.0.1.tar", max compression
+gzip compressed data, was "eflips_depot-3.0.2.tar", max compression
```

## Comparing `eflips_depot-3.0.1.tar` & `eflips_depot-3.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    34143 2023-09-12 12:04:52.313847 eflips_depot-3.0.1/LICENSE.md
--rw-r--r--   0        0        0     4923 2024-01-30 11:53:09.584369 eflips_depot-3.0.1/README.md
--rw-r--r--   0        0        0     6148 2023-10-25 16:23:56.817889 eflips_depot-3.0.1/eflips/depot/.DS_Store
--rw-r--r--   0        0        0     1556 2023-09-18 10:32:47.648700 eflips_depot-3.0.1/eflips/depot/__init__.py
--rw-r--r--   0        0        0    48272 2024-03-20 16:50:59.634702 eflips_depot-3.0.1/eflips/depot/api/__init__.py
--rw-r--r--   0        0        0     9147 2024-01-15 12:09:04.913191 eflips_depot-3.0.1/eflips/depot/api/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    42910 2024-03-20 16:52:43.351740 eflips_depot-3.0.1/eflips/depot/api/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5375 2024-03-19 13:55:55.791236 eflips_depot-3.0.1/eflips/depot/api/defaults/default_settings.json
--rw-r--r--   0        0        0        0 2024-03-20 16:37:13.222393 eflips_depot-3.0.1/eflips/depot/api/private/__init__.py
--rw-r--r--   0        0        0      186 2024-03-20 16:42:14.644098 eflips_depot-3.0.1/eflips/depot/api/private/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    16582 2024-03-20 16:52:43.354244 eflips_depot-3.0.1/eflips/depot/api/private/__pycache__/depot.cpython-312.pyc
--rw-r--r--   0        0        0     8963 2024-03-18 17:23:57.413115 eflips_depot-3.0.1/eflips/depot/api/private/__pycache__/depot_layout.cpython-312.pyc
--rw-r--r--   0        0        0    15908 2024-03-20 16:42:14.649900 eflips_depot-3.0.1/eflips/depot/api/private/__pycache__/util.cpython-312.pyc
--rw-r--r--   0        0        0    16594 2024-03-20 16:50:59.635201 eflips_depot-3.0.1/eflips/depot/api/private/depot.py
--rw-r--r--   0        0        0    15261 2024-03-20 16:37:13.222833 eflips_depot-3.0.1/eflips/depot/api/private/util.py
--rw-r--r--   0        0        0    35678 2024-03-19 13:55:55.792840 eflips_depot-3.0.1/eflips/depot/configuration.py
--rw-r--r--   0        0        0   105566 2024-03-20 16:50:59.635993 eflips_depot-3.0.1/eflips/depot/depot.py
--rw-r--r--   0        0        0   140842 2024-03-19 13:55:55.793916 eflips_depot-3.0.1/eflips/depot/evaluation.py
--rw-r--r--   0        0        0    15522 2023-09-18 10:44:13.224151 eflips_depot-3.0.1/eflips/depot/filters.py
--rw-r--r--   0        0        0     5569 2023-09-12 07:17:14.199982 eflips_depot-3.0.1/eflips/depot/input_epex_power_price.py
--rw-r--r--   0        0        0        0 2023-07-04 10:37:34.116338 eflips_depot-3.0.1/eflips/depot/layout_opt/__init__.py
--rw-r--r--   0        0        0      197 2023-07-04 13:45:08.435464 eflips_depot-3.0.1/eflips/depot/layout_opt/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      185 2024-01-15 16:09:16.741928 eflips_depot-3.0.1/eflips/depot/layout_opt/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    35672 2023-07-04 14:28:06.446062 eflips_depot-3.0.1/eflips/depot/layout_opt/__pycache__/evaluation.cpython-311.pyc
--rw-r--r--   0        0        0    83908 2023-07-04 14:28:06.127266 eflips_depot-3.0.1/eflips/depot/layout_opt/__pycache__/packing.cpython-311.pyc
--rw-r--r--   0        0        0     1378 2023-07-04 14:27:45.921545 eflips_depot-3.0.1/eflips/depot/layout_opt/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     5898 2023-07-04 14:28:06.443416 eflips_depot-3.0.1/eflips/depot/layout_opt/__pycache__/util.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-07-04 10:37:34.116399 eflips_depot-3.0.1/eflips/depot/layout_opt/doc/__init__.py
--rw-r--r--   0        0        0    22330 2023-07-04 10:37:34.116540 eflips_depot-3.0.1/eflips/depot/layout_opt/doc/direct_details.pdf
--rw-r--r--   0        0        0    24855 2023-11-27 13:13:21.354478 eflips_depot-3.0.1/eflips/depot/layout_opt/evaluation.py
--rw-r--r--   0        0        0      594 2023-09-12 07:17:14.200220 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__init__.py
--rw-r--r--   0        0        0     1114 2023-07-04 14:28:06.119012 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1871 2023-07-04 14:28:06.119582 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/crossover.cpython-311.pyc
--rw-r--r--   0        0        0    10041 2023-07-04 14:29:58.881420 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/fitness_c_urfd.cpython-311.pyc
--rw-r--r--   0        0        0     8052 2023-07-04 14:28:06.442624 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/fitness_util.cpython-311.pyc
--rw-r--r--   0        0        0    21433 2023-07-04 14:28:06.122179 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/init.cpython-311.pyc
--rw-r--r--   0        0        0    14402 2023-07-04 14:28:06.120785 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/mutation.cpython-311.pyc
--rw-r--r--   0        0        0     1057 2023-07-04 10:37:34.116782 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/crossover.py
--rw-r--r--   0        0        0     8230 2024-03-19 13:55:55.794538 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py
--rw-r--r--   0        0        0     7027 2024-03-19 13:55:55.794746 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/fitness_util.py
--rw-r--r--   0        0        0    14707 2023-09-18 10:44:13.136159 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/init.py
--rw-r--r--   0        0        0    12238 2023-09-18 10:44:13.095315 eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/mutation.py
--rw-r--r--   0        0        0     9821 2023-11-27 13:13:21.355200 eflips_depot-3.0.1/eflips/depot/layout_opt/optimize_c_urfd.py
--rw-r--r--   0        0        0    56989 2023-11-27 13:13:21.355852 eflips_depot-3.0.1/eflips/depot/layout_opt/packing.py
--rw-r--r--   0        0        0      810 2023-09-12 07:17:14.201273 eflips_depot-3.0.1/eflips/depot/layout_opt/settings.py
--rw-r--r--   0        0        0     9736 2023-09-18 10:44:13.156260 eflips_depot-3.0.1/eflips/depot/layout_opt/template_creation.py
--rw-r--r--   0        0        0     3780 2023-09-18 10:44:13.048607 eflips_depot-3.0.1/eflips/depot/layout_opt/util.py
--rw-r--r--   0        0        0     2509 2023-10-26 12:56:09.063373 eflips_depot-3.0.1/eflips/depot/plots.py
--rw-r--r--   0        0        0    58757 2024-03-20 16:56:56.764032 eflips_depot-3.0.1/eflips/depot/processes.py
--rw-r--r--   0        0        0    16648 2023-09-18 10:44:12.914701 eflips_depot-3.0.1/eflips/depot/rating.py
--rw-r--r--   0        0        0    13568 2024-01-15 15:15:16.955650 eflips_depot-3.0.1/eflips/depot/resources.py
--rw-r--r--   0        0        0     2527 2023-09-24 11:00:36.366976 eflips_depot-3.0.1/eflips/depot/settings_config.py
--rw-r--r--   0        0        0     9375 2023-10-09 12:48:51.301551 eflips_depot-3.0.1/eflips/depot/simple_vehicle.py
--rw-r--r--   0        0        0    10676 2024-03-20 16:37:13.224092 eflips_depot-3.0.1/eflips/depot/simulation.py
--rw-r--r--   0        0        0    54311 2023-11-27 13:13:21.357629 eflips_depot-3.0.1/eflips/depot/smart_charging.py
--rw-r--r--   0        0        0    22338 2023-11-13 11:10:33.262925 eflips_depot-3.0.1/eflips/depot/standalone.py
--rw-r--r--   0        0        0     7097 2023-09-18 10:44:13.235715 eflips_depot-3.0.1/eflips/depot/validation.py
--rw-r--r--   0        0        0     1084 2024-03-20 16:57:57.153859 eflips_depot-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     5648 1970-01-01 00:00:00.000000 eflips_depot-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34143 2023-09-12 12:04:52.313847 eflips_depot-3.0.2/LICENSE.md
+-rw-r--r--   0        0        0     4923 2024-01-30 11:53:09.584369 eflips_depot-3.0.2/README.md
+-rw-r--r--   0        0        0     6148 2023-10-25 16:23:56.817889 eflips_depot-3.0.2/eflips/depot/.DS_Store
+-rw-r--r--   0        0        0     1556 2023-09-18 10:32:47.648700 eflips_depot-3.0.2/eflips/depot/__init__.py
+-rw-r--r--   0        0        0    48272 2024-04-08 08:44:07.631762 eflips_depot-3.0.2/eflips/depot/api/__init__.py
+-rw-r--r--   0        0        0     9147 2024-01-15 12:09:04.913191 eflips_depot-3.0.2/eflips/depot/api/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    42910 2024-03-20 16:52:43.351740 eflips_depot-3.0.2/eflips/depot/api/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5375 2024-03-19 13:55:55.791236 eflips_depot-3.0.2/eflips/depot/api/defaults/default_settings.json
+-rw-r--r--   0        0        0        0 2024-03-20 16:37:13.222393 eflips_depot-3.0.2/eflips/depot/api/private/__init__.py
+-rw-r--r--   0        0        0      186 2024-03-20 16:42:14.644098 eflips_depot-3.0.2/eflips/depot/api/private/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    16582 2024-03-20 16:52:43.354244 eflips_depot-3.0.2/eflips/depot/api/private/__pycache__/depot.cpython-312.pyc
+-rw-r--r--   0        0        0     8963 2024-03-18 17:23:57.413115 eflips_depot-3.0.2/eflips/depot/api/private/__pycache__/depot_layout.cpython-312.pyc
+-rw-r--r--   0        0        0    15908 2024-03-20 16:42:14.649900 eflips_depot-3.0.2/eflips/depot/api/private/__pycache__/util.cpython-312.pyc
+-rw-r--r--   0        0        0    16594 2024-04-08 08:44:07.632141 eflips_depot-3.0.2/eflips/depot/api/private/depot.py
+-rw-r--r--   0        0        0    15261 2024-03-20 16:37:13.222833 eflips_depot-3.0.2/eflips/depot/api/private/util.py
+-rw-r--r--   0        0        0    35678 2024-03-19 13:55:55.792840 eflips_depot-3.0.2/eflips/depot/configuration.py
+-rw-r--r--   0        0        0   105566 2024-04-08 08:44:07.632864 eflips_depot-3.0.2/eflips/depot/depot.py
+-rw-r--r--   0        0        0   140842 2024-03-19 13:55:55.793916 eflips_depot-3.0.2/eflips/depot/evaluation.py
+-rw-r--r--   0        0        0    15522 2023-09-18 10:44:13.224151 eflips_depot-3.0.2/eflips/depot/filters.py
+-rw-r--r--   0        0        0     5569 2023-09-12 07:17:14.199982 eflips_depot-3.0.2/eflips/depot/input_epex_power_price.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:37:34.116338 eflips_depot-3.0.2/eflips/depot/layout_opt/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-04 13:45:08.435464 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      185 2024-01-15 16:09:16.741928 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    35672 2023-07-04 14:28:06.446062 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/evaluation.cpython-311.pyc
+-rw-r--r--   0        0        0    83908 2023-07-04 14:28:06.127266 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/packing.cpython-311.pyc
+-rw-r--r--   0        0        0     1378 2023-07-04 14:27:45.921545 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0     5898 2023-07-04 14:28:06.443416 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/util.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-07-04 10:37:34.116399 eflips_depot-3.0.2/eflips/depot/layout_opt/doc/__init__.py
+-rw-r--r--   0        0        0    22330 2023-07-04 10:37:34.116540 eflips_depot-3.0.2/eflips/depot/layout_opt/doc/direct_details.pdf
+-rw-r--r--   0        0        0    24855 2023-11-27 13:13:21.354478 eflips_depot-3.0.2/eflips/depot/layout_opt/evaluation.py
+-rw-r--r--   0        0        0      594 2023-09-12 07:17:14.200220 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__init__.py
+-rw-r--r--   0        0        0     1114 2023-07-04 14:28:06.119012 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1871 2023-07-04 14:28:06.119582 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/crossover.cpython-311.pyc
+-rw-r--r--   0        0        0    10041 2023-07-04 14:29:58.881420 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/fitness_c_urfd.cpython-311.pyc
+-rw-r--r--   0        0        0     8052 2023-07-04 14:28:06.442624 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/fitness_util.cpython-311.pyc
+-rw-r--r--   0        0        0    21433 2023-07-04 14:28:06.122179 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/init.cpython-311.pyc
+-rw-r--r--   0        0        0    14402 2023-07-04 14:28:06.120785 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/mutation.cpython-311.pyc
+-rw-r--r--   0        0        0     1057 2023-07-04 10:37:34.116782 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/crossover.py
+-rw-r--r--   0        0        0     8230 2024-03-19 13:55:55.794538 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py
+-rw-r--r--   0        0        0     7027 2024-03-19 13:55:55.794746 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/fitness_util.py
+-rw-r--r--   0        0        0    14707 2023-09-18 10:44:13.136159 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/init.py
+-rw-r--r--   0        0        0    12238 2023-09-18 10:44:13.095315 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/mutation.py
+-rw-r--r--   0        0        0     9821 2023-11-27 13:13:21.355200 eflips_depot-3.0.2/eflips/depot/layout_opt/optimize_c_urfd.py
+-rw-r--r--   0        0        0    56989 2023-11-27 13:13:21.355852 eflips_depot-3.0.2/eflips/depot/layout_opt/packing.py
+-rw-r--r--   0        0        0      810 2023-09-12 07:17:14.201273 eflips_depot-3.0.2/eflips/depot/layout_opt/settings.py
+-rw-r--r--   0        0        0     9736 2023-09-18 10:44:13.156260 eflips_depot-3.0.2/eflips/depot/layout_opt/template_creation.py
+-rw-r--r--   0        0        0     3780 2023-09-18 10:44:13.048607 eflips_depot-3.0.2/eflips/depot/layout_opt/util.py
+-rw-r--r--   0        0        0     2509 2023-10-26 12:56:09.063373 eflips_depot-3.0.2/eflips/depot/plots.py
+-rw-r--r--   0        0        0    58757 2024-04-08 08:44:07.633396 eflips_depot-3.0.2/eflips/depot/processes.py
+-rw-r--r--   0        0        0    16648 2023-09-18 10:44:12.914701 eflips_depot-3.0.2/eflips/depot/rating.py
+-rw-r--r--   0        0        0    13568 2024-01-15 15:15:16.955650 eflips_depot-3.0.2/eflips/depot/resources.py
+-rw-r--r--   0        0        0     2527 2023-09-24 11:00:36.366976 eflips_depot-3.0.2/eflips/depot/settings_config.py
+-rw-r--r--   0        0        0     9375 2023-10-09 12:48:51.301551 eflips_depot-3.0.2/eflips/depot/simple_vehicle.py
+-rw-r--r--   0        0        0    10676 2024-03-20 16:37:13.224092 eflips_depot-3.0.2/eflips/depot/simulation.py
+-rw-r--r--   0        0        0    54311 2023-11-27 13:13:21.357629 eflips_depot-3.0.2/eflips/depot/smart_charging.py
+-rw-r--r--   0        0        0    22338 2023-11-13 11:10:33.262925 eflips_depot-3.0.2/eflips/depot/standalone.py
+-rw-r--r--   0        0        0     7097 2023-09-18 10:44:13.235715 eflips_depot-3.0.2/eflips/depot/validation.py
+-rw-r--r--   0        0        0     1084 2024-04-08 08:50:00.210743 eflips_depot-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5648 1970-01-01 00:00:00.000000 eflips_depot-3.0.2/PKG-INFO
```

### Comparing `eflips_depot-3.0.1/LICENSE.md` & `eflips_depot-3.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/README.md` & `eflips_depot-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/.DS_Store` & `eflips_depot-3.0.2/eflips/depot/.DS_Store`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/__init__.py` & `eflips_depot-3.0.2/eflips/depot/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/api/__init__.py` & `eflips_depot-3.0.2/eflips/depot/api/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/api/__pycache__/__init__.cpython-311.pyc` & `eflips_depot-3.0.2/eflips/depot/api/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/api/__pycache__/__init__.cpython-312.pyc` & `eflips_depot-3.0.2/eflips/depot/api/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/api/defaults/default_settings.json` & `eflips_depot-3.0.2/eflips/depot/api/defaults/default_settings.json`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/api/private/__pycache__/depot.cpython-312.pyc` & `eflips_depot-3.0.2/eflips/depot/api/private/__pycache__/depot.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/api/private/__pycache__/depot_layout.cpython-312.pyc` & `eflips_depot-3.0.2/eflips/depot/api/private/__pycache__/depot_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/api/private/__pycache__/util.cpython-312.pyc` & `eflips_depot-3.0.2/eflips/depot/api/private/__pycache__/util.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/api/private/depot.py` & `eflips_depot-3.0.2/eflips/depot/api/private/depot.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/api/private/util.py` & `eflips_depot-3.0.2/eflips/depot/api/private/util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/configuration.py` & `eflips_depot-3.0.2/eflips/depot/configuration.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/depot.py` & `eflips_depot-3.0.2/eflips/depot/depot.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/evaluation.py` & `eflips_depot-3.0.2/eflips/depot/evaluation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/filters.py` & `eflips_depot-3.0.2/eflips/depot/filters.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/input_epex_power_price.py` & `eflips_depot-3.0.2/eflips/depot/input_epex_power_price.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/__pycache__/evaluation.cpython-311.pyc` & `eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/evaluation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/__pycache__/packing.cpython-311.pyc` & `eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/packing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/__pycache__/settings.cpython-311.pyc` & `eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/__pycache__/util.cpython-311.pyc` & `eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/doc/direct_details.pdf` & `eflips_depot-3.0.2/eflips/depot/layout_opt/doc/direct_details.pdf`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/evaluation.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/evaluation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__init__.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/__init__.cpython-311.pyc` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/crossover.cpython-311.pyc` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/crossover.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/fitness_c_urfd.cpython-311.pyc` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/fitness_c_urfd.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/fitness_util.cpython-311.pyc` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/fitness_util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/init.cpython-311.pyc` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/init.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/__pycache__/mutation.cpython-311.pyc` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/mutation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/crossover.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/crossover.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/fitness_util.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/fitness_util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/init.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/init.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/opt_tools/mutation.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/mutation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/optimize_c_urfd.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/optimize_c_urfd.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/packing.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/packing.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/settings.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/settings.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/template_creation.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/template_creation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/layout_opt/util.py` & `eflips_depot-3.0.2/eflips/depot/layout_opt/util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/plots.py` & `eflips_depot-3.0.2/eflips/depot/plots.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/processes.py` & `eflips_depot-3.0.2/eflips/depot/processes.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/rating.py` & `eflips_depot-3.0.2/eflips/depot/rating.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/resources.py` & `eflips_depot-3.0.2/eflips/depot/resources.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/settings_config.py` & `eflips_depot-3.0.2/eflips/depot/settings_config.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/simple_vehicle.py` & `eflips_depot-3.0.2/eflips/depot/simple_vehicle.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/simulation.py` & `eflips_depot-3.0.2/eflips/depot/simulation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/smart_charging.py` & `eflips_depot-3.0.2/eflips/depot/smart_charging.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/standalone.py` & `eflips_depot-3.0.2/eflips/depot/standalone.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/eflips/depot/validation.py` & `eflips_depot-3.0.2/eflips/depot/validation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.1/pyproject.toml` & `eflips_depot-3.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-depot"
-version = "3.0.1"
+version = "3.0.2"
 description = "Depot Simulation for eFLIPS"
 authors = ["Enrico Lauth <enrico.lauth@tu-berlin.de>",
     "Ludger Heide <ludger.heide@tu-berlin.de",
     "Shuyao Guo <shuyao.guo@tu-berlin.de"]
 license = "AGPLv3"
 readme = "README.md"
 packages = [{ include = "eflips/depot" }]
```

### Comparing `eflips_depot-3.0.1/PKG-INFO` & `eflips_depot-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-depot
-Version: 3.0.1
+Version: 3.0.2
 Summary: Depot Simulation for eFLIPS
 License: AGPLv3
 Author: Enrico Lauth
 Author-email: enrico.lauth@tu-berlin.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

