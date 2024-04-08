# Comparing `tmp/pytoughreact-1.0.3.tar.gz` & `tmp/pytoughreact-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytoughreact-1.0.3.tar", last modified: Mon Feb 26 06:03:15 2024, max compression
+gzip compressed data, was "pytoughreact-1.0.4.tar", last modified: Mon Apr  8 04:04:29 2024, max compression
```

## Comparing `pytoughreact-1.0.3.tar` & `pytoughreact-1.0.4.tar`

### file list

```diff
@@ -1,90 +1,79 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:15.346305 pytoughreact-1.0.3/
--rw-rw-rw-   0        0        0     1092 2023-10-24 18:20:51.000000 pytoughreact-1.0.3/LICENSE
--rw-rw-rw-   0        0        0    10842 2024-02-26 06:03:15.342317 pytoughreact-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8419 2023-10-24 18:20:51.000000 pytoughreact-1.0.3/README.md
--rw-rw-rw-   0        0        0     1991 2024-02-26 06:02:19.000000 pytoughreact-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-26 06:03:15.349296 pytoughreact-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3647 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:14.542039 pytoughreact-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:14.580008 pytoughreact-1.0.3/src/pytoughreact/
--rw-rw-rw-   0        0        0      781 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:14.625894 pytoughreact-1.0.3/src/pytoughreact/assembler/
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/assembler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:14.723626 pytoughreact-1.0.3/src/pytoughreact/chemical/
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/chemical/__init__.py
--rw-rw-rw-   0        0        0     7572 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/chemical/bio_process_description.py
--rw-rw-rw-   0        0        0    17331 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/chemical/biomass_composition.py
--rw-rw-rw-   0        0        0     2808 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/chemical/chemical_composition.py
--rw-rw-rw-   0        0        0     3273 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/chemical/kinetic_properties.py
--rw-rw-rw-   0        0        0     1513 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/chemical/mineral_composition.py
--rw-rw-rw-   0        0        0     5742 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/chemical/mineral_description.py
--rw-rw-rw-   0        0        0     1209 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/chemical/mineral_zone.py
--rw-rw-rw-   0        0        0     1390 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/chemical/perm_poro_zone.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:14.844493 pytoughreact-1.0.3/src/pytoughreact/constants/
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/constants/__init__.py
--rw-rw-rw-   0        0        0     1325 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/constants/cap_pressure_constants.py
--rw-rw-rw-   0        0        0    11023 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/constants/default_minerals.py
--rw-rw-rw-   0        0        0     3773 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/constants/defaults_constants.py
--rw-rw-rw-   0        0        0    21575 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/constants/format_specifications.py
--rw-rw-rw-   0        0        0     1422 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/constants/generalconstants.py
--rw-rw-rw-   0        0        0     1152 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/constants/grid_constants.py
--rw-rw-rw-   0        0        0     2958 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/constants/plotconstants.py
--rw-rw-rw-   0        0        0     1492 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/constants/reactionconstants.py
--rw-rw-rw-   0        0        0     1373 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/constants/rel_perm_constants.py
--rw-rw-rw-   0        0        0     2586 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/constants/sections.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:14.856407 pytoughreact-1.0.3/src/pytoughreact/exceptions/
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/exceptions/__init__.py
--rw-rw-rw-   0        0        0     4406 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/exceptions/custom_error.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:14.902727 pytoughreact-1.0.3/src/pytoughreact/model/
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/model/__init__.py
--rw-rw-rw-   0        0        0     5725 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/model/capillary_pressure.py
--rw-rw-rw-   0        0        0     2313 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/model/grid.py
--rw-rw-rw-   0        0        0     3448 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/model/physical_model.py
--rw-rw-rw-   0        0        0     4035 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/model/relative_permeability.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:14.915868 pytoughreact-1.0.3/src/pytoughreact/numerical/
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/numerical/__init__.py
--rw-rw-rw-   0        0        0     1497 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/numerical/physical_model_numericals.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:14.978286 pytoughreact-1.0.3/src/pytoughreact/plotting/
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/plotting/__init__.py
--rw-rw-rw-   0        0        0     5445 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/plotting/plot_multiple.py
--rw-rw-rw-   0        0        0    21511 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/plotting/plot_multiple_files_routine.py
--rw-rw-rw-   0        0        0    37224 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/plotting/plot_multiple_tough_routine.py
--rw-rw-rw-   0        0        0     7685 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/plotting/plot_single.py
--rw-rw-rw-   0        0        0    26598 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/plotting/plot_tough_routine.py
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/py.typed
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:15.121903 pytoughreact-1.0.3/src/pytoughreact/results/
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/results/__init__.py
--rw-rw-rw-   0        0        0     6864 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/results/multi_result_tough_3.py
--rw-rw-rw-   0        0        0     7946 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/results/multi_result_tough_react.py
--rw-rw-rw-   0        0        0     4180 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/results/result_multiple.py
--rw-rw-rw-   0        0        0     5405 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/results/result_single.py
--rw-rw-rw-   0        0        0    13427 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/results/result_tough_3.py
--rw-rw-rw-   0        0        0    31302 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/results/result_tough_react.py
--rw-rw-rw-   0        0        0     2096 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/results/simple_experiment_data.py
--rw-rw-rw-   0        0        0     2699 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/results/t2result.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:15.149829 pytoughreact-1.0.3/src/pytoughreact/utilities/
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/utilities/__init__.py
--rw-rw-rw-   0        0        0     6038 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/utilities/t2_tough_react_utilities.py
--rw-rw-rw-   0        0        0     8620 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/utilities/t2_utilities.py
--rw-rw-rw-   0        0        0       24 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/version.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:15.200693 pytoughreact-1.0.3/src/pytoughreact/wrapper/
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/wrapper/__init__.py
--rw-rw-rw-   0        0        0     2099 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/wrapper/react_data.py
--rw-rw-rw-   0        0        0     1883 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/wrapper/reactblock.py
--rw-rw-rw-   0        0        0     3639 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/wrapper/reactgrid.py
--rw-rw-rw-   0        0        0     1567 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/wrapper/reactzone.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:15.290454 pytoughreact-1.0.3/src/pytoughreact/writers/
--rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/writers/__init__.py
--rw-rw-rw-   0        0        0    38756 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/writers/bio_writing.py
--rw-rw-rw-   0        0        0    70906 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/writers/chemical_writing.py
--rw-rw-rw-   0        0        0    24789 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/writers/react_writing.py
--rw-rw-rw-   0        0        0    49782 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/src/pytoughreact/writers/solute_writing.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:15.339324 pytoughreact-1.0.3/src/pytoughreact.egg-info/
--rw-rw-rw-   0        0        0    10842 2024-02-26 06:03:14.000000 pytoughreact-1.0.3/src/pytoughreact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2959 2024-02-26 06:03:14.000000 pytoughreact-1.0.3/src/pytoughreact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 06:03:14.000000 pytoughreact-1.0.3/src/pytoughreact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-02-26 06:03:14.000000 pytoughreact-1.0.3/src/pytoughreact.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-02-26 06:03:14.000000 pytoughreact-1.0.3/src/pytoughreact.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:15.336344 pytoughreact-1.0.3/test/
--rw-rw-rw-   0        0        0     5514 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/test/test_pytoughreact_bio.py
--rw-rw-rw-   0        0        0    18716 2023-10-24 18:20:54.000000 pytoughreact-1.0.3/test/test_pytoughreact_react.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.435821 pytoughreact-1.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-10-24 18:20:51.000000 pytoughreact-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0    10284 2024-04-08 04:04:29.433829 pytoughreact-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9121 2024-04-08 03:03:50.000000 pytoughreact-1.0.4/README.md
+-rw-rw-rw-   0        0        0     1976 2024-04-08 03:46:55.000000 pytoughreact-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 04:04:29.436820 pytoughreact-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3647 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.274322 pytoughreact-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.295321 pytoughreact-1.0.4/src/pytoughreact/
+-rw-rw-rw-   0        0        0      781 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.338475 pytoughreact-1.0.4/src/pytoughreact/chemical/
+-rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/chemical/__init__.py
+-rw-rw-rw-   0        0        0    10286 2024-04-06 22:25:53.000000 pytoughreact-1.0.4/src/pytoughreact/chemical/bio_process_description.py
+-rw-rw-rw-   0        0        0    17330 2024-04-06 22:11:13.000000 pytoughreact-1.0.4/src/pytoughreact/chemical/biomass_composition.py
+-rw-rw-rw-   0        0        0     6564 2024-04-07 04:50:22.000000 pytoughreact-1.0.4/src/pytoughreact/chemical/chemical_composition.py
+-rw-rw-rw-   0        0        0     9485 2024-04-06 22:42:47.000000 pytoughreact-1.0.4/src/pytoughreact/chemical/kinetic_properties.py
+-rw-rw-rw-   0        0        0     2879 2024-04-06 23:02:02.000000 pytoughreact-1.0.4/src/pytoughreact/chemical/mineral_composition.py
+-rw-rw-rw-   0        0        0     6955 2024-04-06 22:50:12.000000 pytoughreact-1.0.4/src/pytoughreact/chemical/mineral_description.py
+-rw-rw-rw-   0        0        0     1432 2024-04-08 02:42:46.000000 pytoughreact-1.0.4/src/pytoughreact/chemical/mineral_zone.py
+-rw-rw-rw-   0        0        0     3342 2024-04-07 04:47:10.000000 pytoughreact-1.0.4/src/pytoughreact/chemical/perm_poro_zone.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.360090 pytoughreact-1.0.4/src/pytoughreact/constants/
+-rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/constants/__init__.py
+-rw-rw-rw-   0        0        0     1325 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/constants/cap_pressure_constants.py
+-rw-rw-rw-   0        0        0    11023 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/constants/default_minerals.py
+-rw-rw-rw-   0        0        0     3773 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/constants/defaults_constants.py
+-rw-rw-rw-   0        0        0    21575 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/constants/format_specifications.py
+-rw-rw-rw-   0        0        0     1422 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/constants/generalconstants.py
+-rw-rw-rw-   0        0        0     1152 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/constants/grid_constants.py
+-rw-rw-rw-   0        0        0     2974 2024-03-29 05:57:29.000000 pytoughreact-1.0.4/src/pytoughreact/constants/plotconstants.py
+-rw-rw-rw-   0        0        0     1492 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/constants/reactionconstants.py
+-rw-rw-rw-   0        0        0     1373 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/constants/rel_perm_constants.py
+-rw-rw-rw-   0        0        0     2586 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/constants/sections.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.363115 pytoughreact-1.0.4/src/pytoughreact/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     4432 2024-03-29 05:58:08.000000 pytoughreact-1.0.4/src/pytoughreact/exceptions/custom_error.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.375678 pytoughreact-1.0.4/src/pytoughreact/plotting/
+-rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/plotting/__init__.py
+-rw-rw-rw-   0        0        0     5756 2024-03-29 05:27:17.000000 pytoughreact-1.0.4/src/pytoughreact/plotting/plot_multiple.py
+-rw-rw-rw-   0        0        0    22879 2024-03-29 05:11:48.000000 pytoughreact-1.0.4/src/pytoughreact/plotting/plot_multiple_files_routine.py
+-rw-rw-rw-   0        0        0    40719 2024-04-08 02:16:45.000000 pytoughreact-1.0.4/src/pytoughreact/plotting/plot_multiple_tough_routine.py
+-rw-rw-rw-   0        0        0     8298 2024-03-29 05:04:44.000000 pytoughreact-1.0.4/src/pytoughreact/plotting/plot_single.py
+-rw-rw-rw-   0        0        0    28845 2024-04-08 02:16:59.000000 pytoughreact-1.0.4/src/pytoughreact/plotting/plot_tough_routine.py
+-rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.394967 pytoughreact-1.0.4/src/pytoughreact/results/
+-rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/results/__init__.py
+-rw-rw-rw-   0        0        0     9039 2024-04-07 23:25:18.000000 pytoughreact-1.0.4/src/pytoughreact/results/multi_result_tough_3.py
+-rw-rw-rw-   0        0        0    11581 2024-04-08 02:17:22.000000 pytoughreact-1.0.4/src/pytoughreact/results/multi_result_tough_react.py
+-rw-rw-rw-   0        0        0     5841 2024-04-07 22:39:53.000000 pytoughreact-1.0.4/src/pytoughreact/results/result_multiple.py
+-rw-rw-rw-   0        0        0     8573 2024-04-07 22:54:41.000000 pytoughreact-1.0.4/src/pytoughreact/results/result_single.py
+-rw-rw-rw-   0        0        0    22053 2024-04-08 03:00:10.000000 pytoughreact-1.0.4/src/pytoughreact/results/result_tough_3.py
+-rw-rw-rw-   0        0        0    14814 2024-04-08 01:28:22.000000 pytoughreact-1.0.4/src/pytoughreact/results/result_tough_react.py
+-rw-rw-rw-   0        0        0     3635 2024-04-08 01:08:27.000000 pytoughreact-1.0.4/src/pytoughreact/results/simple_experiment_data.py
+-rw-rw-rw-   0        0        0     4839 2024-04-08 01:05:28.000000 pytoughreact-1.0.4/src/pytoughreact/results/t2result.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.401912 pytoughreact-1.0.4/src/pytoughreact/utilities/
+-rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6064 2024-04-08 01:24:31.000000 pytoughreact-1.0.4/src/pytoughreact/utilities/t2_tough_react_utilities.py
+-rw-rw-rw-   0        0        0    11835 2024-04-08 01:47:56.000000 pytoughreact-1.0.4/src/pytoughreact/utilities/t2_utilities.py
+-rw-rw-rw-   0        0        0       24 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/version.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.412882 pytoughreact-1.0.4/src/pytoughreact/wrapper/
+-rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/wrapper/__init__.py
+-rw-rw-rw-   0        0        0     2487 2024-04-08 02:21:56.000000 pytoughreact-1.0.4/src/pytoughreact/wrapper/react_data.py
+-rw-rw-rw-   0        0        0     2875 2024-04-08 02:29:33.000000 pytoughreact-1.0.4/src/pytoughreact/wrapper/reactblock.py
+-rw-rw-rw-   0        0        0     4953 2024-04-08 02:37:39.000000 pytoughreact-1.0.4/src/pytoughreact/wrapper/reactgrid.py
+-rw-rw-rw-   0        0        0     2566 2024-04-08 02:48:17.000000 pytoughreact-1.0.4/src/pytoughreact/wrapper/reactzone.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.424850 pytoughreact-1.0.4/src/pytoughreact/writers/
+-rw-rw-rw-   0        0        0        0 2023-10-24 18:20:54.000000 pytoughreact-1.0.4/src/pytoughreact/writers/__init__.py
+-rw-rw-rw-   0        0        0    39238 2024-03-29 05:52:00.000000 pytoughreact-1.0.4/src/pytoughreact/writers/bio_writing.py
+-rw-rw-rw-   0        0        0    71873 2024-04-07 04:50:13.000000 pytoughreact-1.0.4/src/pytoughreact/writers/chemical_writing.py
+-rw-rw-rw-   0        0        0    24848 2024-03-29 05:44:14.000000 pytoughreact-1.0.4/src/pytoughreact/writers/react_writing.py
+-rw-rw-rw-   0        0        0    49900 2024-03-29 05:43:05.000000 pytoughreact-1.0.4/src/pytoughreact/writers/solute_writing.py
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.430834 pytoughreact-1.0.4/src/pytoughreact.egg-info/
+-rw-rw-rw-   0        0        0    10284 2024-04-08 04:04:29.000000 pytoughreact-1.0.4/src/pytoughreact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2625 2024-04-08 04:04:29.000000 pytoughreact-1.0.4/src/pytoughreact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 04:04:29.000000 pytoughreact-1.0.4/src/pytoughreact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-04-08 04:04:29.000000 pytoughreact-1.0.4/src/pytoughreact.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-08 04:04:29.000000 pytoughreact-1.0.4/src/pytoughreact.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 04:04:29.428842 pytoughreact-1.0.4/test/
+-rw-rw-rw-   0        0        0     5511 2024-04-06 22:25:47.000000 pytoughreact-1.0.4/test/test_pytoughreact_bio.py
+-rw-rw-rw-   0        0        0    18850 2024-04-07 03:43:58.000000 pytoughreact-1.0.4/test/test_pytoughreact_react.py
```

### Comparing `pytoughreact-1.0.3/LICENSE` & `pytoughreact-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytoughreact-1.0.3/PKG-INFO` & `pytoughreact-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,35 @@
 Metadata-Version: 2.1
 Name: pytoughreact
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Library for automating reaction simulations using TOUGHREACT, TMVOC and TMVOC-BIO
 Author-email: Temitope Ajayi <ajayi_temmy@yahoo.com>
 Maintainer-email: Temitope Ajayi <ajayi_temmy@yahoo.com>
 License: MIT License
-        
-        Copyright (c) 2023 Temitope Ajayi
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Project-URL: repository, https://github.com/temmy222/PyTOUGHREACT
 Keywords: biodegradation,reactive transport,automation,uncertainty quantification
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1
 Requires-Dist: scipy>=1
 Requires-Dist: vtk>=1
 Requires-Dist: matplotlib>=3
 Requires-Dist: pandas>=1
 Requires-Dist: PyTOUGH
+Requires-Dist: flake8
 
 # PyTOUGHREACT
 
 
 - [PyTOUGHREACT](#pytoughreact)
   - [Installation](#installation)
   - [Usage](#usage)
@@ -76,15 +56,22 @@
 
 The package can also be forked from this GitHub page and installation performed using
 
 ```bash
 python setup.py install  or py setup.py install
 ```
 
-Because pytoughreact requires PyTOUGH and PyTOUGH is not uploaded to PyPI, it is required to download the zip folder of PyTOUGH from the GitHub repository https://github.com/acroucher/PyTOUGH. Unzip the folder and place in your current working directory. Change directory into the PyTOUGH folder and run python setup.py install or pip install on the command line. With PyTOUGH installed, PyTOUGHREACT is ready to be used as a package.
+<!-- Because pytoughreact requires PyTOUGH and PyTOUGH is not uploaded to PyPI, it is required to download the zip folder of PyTOUGH from the GitHub repository https://github.com/acroucher/PyTOUGH. Unzip the folder and place in your current working directory. Change directory into the PyTOUGH folder and run python setup.py install or pip install on the command line. With PyTOUGH installed, PyTOUGHREACT is ready to be used as a package. -->
+
+Because pytoughreact requires PyTOUGH, this library also needs to be installed.
+PyTOUGH can be installed by running the command below
+
+```bash
+pip install PyTOUGH
+```
 
 ## Usage
 
 ```python
 import os
 from mulgrids import mulgrid
 from pytoughreact.writers.react_writing import t2react
@@ -226,20 +213,41 @@
 1. Clone the repo using preferred cloning method
 2. Install the library to enable you able to use the test example using
 
 ```python
 pip install -e .
 ```
 3. Modify the code 
-4. Run tests: Tests are conducted with pytest. Flake8 is also used to ensure code readability
+4. Tests are conducted with pytest and coverage reports are performed using pytest-cov. Install pytest and pytest-cov using the commands below
+   
+```python
+pip install pytest
+```
 
 ```python
+pip install pytest-cov
+```
+5. Run tests:  Run the below command from the root folder to run the tests
+   
+```python
 pytest
 ```
-5. Make a pull request after passing all tests
+
+6. Flake8 is also used to ensure code readability. Install flake8 using 
+   
+```python
+pip install flake8
+```
+and run flake8 using
+
+```python
+flake8 src
+```
+7. Make a pull request after passing all tests
+8. More information can be found in developer notes in the documentation - https://pytoughreact.readthedocs.io/en/master/developer.html 
 
 ## Documentation
 Documentation can be found here https://pytoughreact.readthedocs.io/en/latest/ 
 
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `pytoughreact-1.0.3/README.md` & `pytoughreact-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,22 @@
 
 The package can also be forked from this GitHub page and installation performed using
 
 ```bash
 python setup.py install  or py setup.py install
 ```
 
-Because pytoughreact requires PyTOUGH and PyTOUGH is not uploaded to PyPI, it is required to download the zip folder of PyTOUGH from the GitHub repository https://github.com/acroucher/PyTOUGH. Unzip the folder and place in your current working directory. Change directory into the PyTOUGH folder and run python setup.py install or pip install on the command line. With PyTOUGH installed, PyTOUGHREACT is ready to be used as a package.
+<!-- Because pytoughreact requires PyTOUGH and PyTOUGH is not uploaded to PyPI, it is required to download the zip folder of PyTOUGH from the GitHub repository https://github.com/acroucher/PyTOUGH. Unzip the folder and place in your current working directory. Change directory into the PyTOUGH folder and run python setup.py install or pip install on the command line. With PyTOUGH installed, PyTOUGHREACT is ready to be used as a package. -->
+
+Because pytoughreact requires PyTOUGH, this library also needs to be installed.
+PyTOUGH can be installed by running the command below
+
+```bash
+pip install PyTOUGH
+```
 
 ## Usage
 
 ```python
 import os
 from mulgrids import mulgrid
 from pytoughreact.writers.react_writing import t2react
@@ -177,20 +184,41 @@
 1. Clone the repo using preferred cloning method
 2. Install the library to enable you able to use the test example using
 
 ```python
 pip install -e .
 ```
 3. Modify the code 
-4. Run tests: Tests are conducted with pytest. Flake8 is also used to ensure code readability
+4. Tests are conducted with pytest and coverage reports are performed using pytest-cov. Install pytest and pytest-cov using the commands below
+   
+```python
+pip install pytest
+```
 
 ```python
+pip install pytest-cov
+```
+5. Run tests:  Run the below command from the root folder to run the tests
+   
+```python
 pytest
 ```
-5. Make a pull request after passing all tests
+
+6. Flake8 is also used to ensure code readability. Install flake8 using 
+   
+```python
+pip install flake8
+```
+and run flake8 using
+
+```python
+flake8 src
+```
+7. Make a pull request after passing all tests
+8. More information can be found in developer notes in the documentation - https://pytoughreact.readthedocs.io/en/master/developer.html 
 
 ## Documentation
 Documentation can be found here https://pytoughreact.readthedocs.io/en/latest/ 
 
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `pytoughreact-1.0.3/pyproject.toml` & `pytoughreact-1.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,117 +9,116 @@
 00000080: 696f 6e73 5d0d 0a61 6464 6f70 7473 203d  ions]..addopts =
 00000090: 2022 2d2d 636f 763d 7079 746f 7567 6872   "--cov=pytoughr
 000000a0: 6561 6374 220d 0a74 6573 7470 6174 6873  eact"..testpaths
 000000b0: 203d 205b 0d0a 2020 2020 2274 6573 7422   = [..    "test"
 000000c0: 2c0d 0a5d 0d0a 0d0a 5b70 726f 6a65 6374  ,..]....[project
 000000d0: 5d0d 0a6e 616d 6520 3d20 2270 7974 6f75  ]..name = "pytou
 000000e0: 6768 7265 6163 7422 0d0a 7665 7273 696f  ghreact"..versio
-000000f0: 6e20 3d20 2231 2e30 2e33 220d 0a64 6570  n = "1.0.3"..dep
+000000f0: 6e20 3d20 2231 2e30 2e34 220d 0a64 6570  n = "1.0.4"..dep
 00000100: 656e 6465 6e63 6965 7320 3d20 5b0d 0a20  endencies = [.. 
 00000110: 2022 6e75 6d70 793e 3d31 222c 0d0a 2020   "numpy>=1",..  
 00000120: 2273 6369 7079 3e3d 3122 2c0d 0a20 2022  "scipy>=1",..  "
 00000130: 7674 6b3e 3d31 222c 0d0a 2020 226d 6174  vtk>=1",..  "mat
 00000140: 706c 6f74 6c69 623e 3d33 222c 0d0a 2020  plotlib>=3",..  
 00000150: 2270 616e 6461 733e 3d31 222c 0d0a 2020  "pandas>=1",..  
-00000160: 2250 7954 4f55 4748 220d 0a5d 0d0a 0d0a  "PyTOUGH"..]....
-00000170: 636c 6173 7369 6669 6572 7320 3d20 5b0d  classifiers = [.
-00000180: 0a20 2022 5072 6f67 7261 6d6d 696e 6720  .  "Programming 
-00000190: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000001a0: 6f6e 203a 3a20 3222 2c0d 0a20 2022 5072  on :: 2",..  "Pr
-000001b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001d0: 3322 2c0d 0a20 2022 5072 6f67 7261 6d6d  3",..  "Programm
-000001e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001f0: 5079 7468 6f6e 203a 3a20 332e 3722 2c0d  Python :: 3.7",.
-00000200: 0a20 2022 5072 6f67 7261 6d6d 696e 6720  .  "Programming 
-00000210: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000220: 6f6e 203a 3a20 332e 3822 2c0d 0a20 2022  on :: 3.8",..  "
-00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000240: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000250: 3a20 332e 3922 2c0d 0a20 2020 2022 5072  : 3.9",..    "Pr
-00000260: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000270: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000280: 332e 3130 222c 0d0a 2020 2020 2250 726f  3.10",..    "Pro
-00000290: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002b0: 2e31 3122 2c0d 0a20 2022 4c69 6365 6e73  .11",..  "Licens
-000002c0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000002d0: 6420 3a3a 2047 4e55 204c 6573 7365 7220  d :: GNU Lesser 
-000002e0: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-000002f0: 6963 656e 7365 2076 3320 284c 4750 4c76  icense v3 (LGPLv
-00000300: 3329 222c 0d0a 2020 224f 7065 7261 7469  3)",..  "Operati
-00000310: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-00000320: 496e 6465 7065 6e64 656e 7422 0d0a 5d0d  Independent"..].
-00000330: 0a0d 0a72 6571 7569 7265 732d 7079 7468  ...requires-pyth
-00000340: 6f6e 203d 2022 3e3d 2033 2e37 220d 0a72  on = ">= 3.7"..r
-00000350: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
-00000360: 6d64 220d 0a61 7574 686f 7273 203d 205b  md"..authors = [
-00000370: 0d0a 2020 7b6e 616d 6520 3d20 2254 656d  ..  {name = "Tem
-00000380: 6974 6f70 6520 416a 6179 6922 2c20 656d  itope Ajayi", em
-00000390: 6169 6c20 3d20 2261 6a61 7969 5f74 656d  ail = "ajayi_tem
-000003a0: 6d79 4079 6168 6f6f 2e63 6f6d 227d 2c0d  my@yahoo.com"},.
-000003b0: 0a5d 0d0a 6d61 696e 7461 696e 6572 7320  .]..maintainers 
-000003c0: 3d20 5b0d 0a20 207b 6e61 6d65 203d 2022  = [..  {name = "
-000003d0: 5465 6d69 746f 7065 2041 6a61 7969 222c  Temitope Ajayi",
-000003e0: 2065 6d61 696c 203d 2022 616a 6179 695f   email = "ajayi_
-000003f0: 7465 6d6d 7940 7961 686f 6f2e 636f 6d22  temmy@yahoo.com"
-00000400: 7d0d 0a5d 0d0a 6465 7363 7269 7074 696f  }..]..descriptio
-00000410: 6e20 3d20 2250 7974 686f 6e20 4c69 6272  n = "Python Libr
-00000420: 6172 7920 666f 7220 6175 746f 6d61 7469  ary for automati
-00000430: 6e67 2072 6561 6374 696f 6e20 7369 6d75  ng reaction simu
-00000440: 6c61 7469 6f6e 7320 7573 696e 6720 544f  lations using TO
-00000450: 5547 4852 4541 4354 2c20 544d 564f 4320  UGHREACT, TMVOC 
-00000460: 616e 6420 544d 564f 432d 4249 4f22 0d0a  and TMVOC-BIO"..
-00000470: 6c69 6365 6e73 6520 3d20 7b66 696c 6520  license = {file 
-00000480: 3d20 224c 4943 454e 5345 227d 0d0a 6b65  = "LICENSE"}..ke
-00000490: 7977 6f72 6473 203d 205b 2262 696f 6465  ywords = ["biode
-000004a0: 6772 6164 6174 696f 6e22 2c20 2272 6561  gradation", "rea
-000004b0: 6374 6976 6520 7472 616e 7370 6f72 7422  ctive transport"
-000004c0: 2c20 2261 7574 6f6d 6174 696f 6e22 2c20  , "automation", 
-000004d0: 2275 6e63 6572 7461 696e 7479 2071 7561  "uncertainty qua
-000004e0: 6e74 6966 6963 6174 696f 6e22 5d0d 0a0d  ntification"]...
-000004f0: 0a5b 7072 6f6a 6563 742e 7572 6c73 5d0d  .[project.urls].
-00000500: 0a72 6570 6f73 6974 6f72 7920 3d20 2268  .repository = "h
-00000510: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000520: 6d2f 7465 6d6d 7932 3232 2f50 7954 4f55  m/temmy222/PyTOU
-00000530: 4748 5245 4143 5422 0d0a 0d0a 0d0a 5b74  GHREACT"......[t
-00000540: 6f6f 6c2e 636f 7665 7261 6765 2e68 746d  ool.coverage.htm
-00000550: 6c5d 0d0a 6469 7265 6374 6f72 7920 3d20  l]..directory = 
-00000560: 2263 6f76 6572 6167 655f 6874 6d6c 5f72  "coverage_html_r
-00000570: 6570 6f72 7422 0d0a 0d0a 5b74 6f6f 6c2e  eport"....[tool.
-00000580: 636f 7665 7261 6765 2e72 756e 5d0d 0a6f  coverage.run]..o
-00000590: 6d69 7420 3d20 5b0d 0a20 2020 2023 206f  mit = [..    # o
-000005a0: 6d69 7420 616e 7974 6869 6e67 2069 6e20  mit anything in 
-000005b0: 6120 2e6c 6f63 616c 2064 6972 6563 746f  a .local directo
-000005c0: 7279 2061 6e79 7768 6572 650d 0a20 2020  ry anywhere..   
-000005d0: 2022 2a2f 6d6f 6465 6c2f 2a22 2c0d 0a20   "*/model/*",.. 
-000005e0: 2020 2022 2a2f 636f 6e73 7461 6e74 732f     "*/constants/
-000005f0: 2a22 2c0d 0a20 2020 2022 2a2f 6578 6365  *",..    "*/exce
-00000600: 7074 696f 6e73 2f2a 222c 0d0a 2020 2020  ptions/*",..    
-00000610: 2320 6f6d 6974 2065 7665 7279 7468 696e  # omit everythin
-00000620: 6720 696e 202f 7573 720d 0a20 2020 2022  g in /usr..    "
-00000630: 2f75 7372 2f2a 222c 0d0a 2020 2020 2320  /usr/*",..    # 
-00000640: 6f6d 6974 2074 6869 7320 7369 6e67 6c65  omit this single
-00000650: 2066 696c 650d 0a20 2020 2022 7574 696c   file..    "util
-00000660: 732f 7469 7265 6669 7265 2e70 7922 2c0d  s/tirefire.py",.
-00000670: 0a20 2020 205d 0d0a 0d0a 5b74 6f6f 6c2e  .    ]....[tool.
-00000680: 6d79 7079 5d0d 0a6d 7970 795f 7061 7468  mypy]..mypy_path
-00000690: 203d 2022 7372 6322 0d0a 6368 6563 6b5f   = "src"..check_
-000006a0: 756e 7479 7065 645f 6465 6673 203d 2074  untyped_defs = t
-000006b0: 7275 650d 0a64 6973 616c 6c6f 775f 616e  rue..disallow_an
-000006c0: 795f 6765 6e65 7269 6373 203d 2074 7275  y_generics = tru
-000006d0: 650d 0a69 676e 6f72 655f 6d69 7373 696e  e..ignore_missin
-000006e0: 675f 696d 706f 7274 7320 3d20 7472 7565  g_imports = true
-000006f0: 0d0a 6e6f 5f69 6d70 6c69 6369 745f 6f70  ..no_implicit_op
-00000700: 7469 6f6e 616c 203d 2074 7275 650d 0a73  tional = true..s
-00000710: 686f 775f 6572 726f 725f 636f 6465 7320  how_error_codes 
-00000720: 3d20 7472 7565 0d0a 7374 7269 6374 5f65  = true..strict_e
-00000730: 7175 616c 6974 7920 3d20 7472 7565 0d0a  quality = true..
-00000740: 7761 726e 5f72 6564 756e 6461 6e74 5f63  warn_redundant_c
-00000750: 6173 7473 203d 2074 7275 650d 0a77 6172  asts = true..war
-00000760: 6e5f 7265 7475 726e 5f61 6e79 203d 2074  n_return_any = t
-00000770: 7275 650d 0a77 6172 6e5f 756e 7265 6163  rue..warn_unreac
-00000780: 6861 626c 6520 3d20 7472 7565 0d0a 7761  hable = true..wa
-00000790: 726e 5f75 6e75 7365 645f 636f 6e66 6967  rn_unused_config
-000007a0: 7320 3d20 7472 7565 0d0a 6e6f 5f69 6d70  s = true..no_imp
-000007b0: 6c69 6369 745f 7265 6578 706f 7274 203d  licit_reexport =
-000007c0: 2074 7275 650d 0a                         true..
+00000160: 2250 7954 4f55 4748 222c 0d0a 2020 2266  "PyTOUGH",..  "f
+00000170: 6c61 6b65 3822 0d0a 5d0d 0a0d 0a63 6c61  lake8"..]....cla
+00000180: 7373 6966 6965 7273 203d 205b 0d0a 2020  ssifiers = [..  
+00000190: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
+000001a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000001b0: 3a3a 2032 222c 0d0a 2020 2250 726f 6772  :: 2",..  "Progr
+000001c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 222c  :: Python :: 3",
+000001e0: 0d0a 2020 2250 726f 6772 616d 6d69 6e67  ..  "Programming
+000001f0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000200: 686f 6e20 3a3a 2033 2e37 222c 0d0a 2020  hon :: 3.7",..  
+00000210: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
+00000220: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000230: 3a3a 2033 2e38 222c 0d0a 2020 2250 726f  :: 3.8",..  "Pro
+00000240: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000250: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000260: 2e39 222c 0d0a 2020 2020 2250 726f 6772  .9",..    "Progr
+00000270: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000280: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000290: 3022 2c0d 0a20 2020 2022 5072 6f67 7261  0",..    "Progra
+000002a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000002b0: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
+000002c0: 222c 0d0a 2020 224c 6963 656e 7365 203a  ",..  "License :
+000002d0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+000002e0: 3a20 4d49 5420 4c69 6365 6e73 6522 2c0d  : MIT License",.
+000002f0: 0a20 2022 4f70 6572 6174 696e 6720 5379  .  "Operating Sy
+00000300: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00000310: 656e 6465 6e74 220d 0a5d 0d0a 0d0a 7265  endent"..]....re
+00000320: 7175 6972 6573 2d70 7974 686f 6e20 3d20  quires-python = 
+00000330: 223e 3d20 332e 3722 0d0a 7265 6164 6d65  ">= 3.7"..readme
+00000340: 203d 2022 5245 4144 4d45 2e6d 6422 0d0a   = "README.md"..
+00000350: 6175 7468 6f72 7320 3d20 5b0d 0a20 207b  authors = [..  {
+00000360: 6e61 6d65 203d 2022 5465 6d69 746f 7065  name = "Temitope
+00000370: 2041 6a61 7969 222c 2065 6d61 696c 203d   Ajayi", email =
+00000380: 2022 616a 6179 695f 7465 6d6d 7940 7961   "ajayi_temmy@ya
+00000390: 686f 6f2e 636f 6d22 7d2c 0d0a 5d0d 0a6d  hoo.com"},..]..m
+000003a0: 6169 6e74 6169 6e65 7273 203d 205b 0d0a  aintainers = [..
+000003b0: 2020 7b6e 616d 6520 3d20 2254 656d 6974    {name = "Temit
+000003c0: 6f70 6520 416a 6179 6922 2c20 656d 6169  ope Ajayi", emai
+000003d0: 6c20 3d20 2261 6a61 7969 5f74 656d 6d79  l = "ajayi_temmy
+000003e0: 4079 6168 6f6f 2e63 6f6d 227d 0d0a 5d0d  @yahoo.com"}..].
+000003f0: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
+00000400: 5079 7468 6f6e 204c 6962 7261 7279 2066  Python Library f
+00000410: 6f72 2061 7574 6f6d 6174 696e 6720 7265  or automating re
+00000420: 6163 7469 6f6e 2073 696d 756c 6174 696f  action simulatio
+00000430: 6e73 2075 7369 6e67 2054 4f55 4748 5245  ns using TOUGHRE
+00000440: 4143 542c 2054 4d56 4f43 2061 6e64 2054  ACT, TMVOC and T
+00000450: 4d56 4f43 2d42 494f 220d 0a6c 6963 656e  MVOC-BIO"..licen
+00000460: 7365 203d 207b 7465 7874 203d 2022 4d49  se = {text = "MI
+00000470: 5420 4c69 6365 6e73 6522 7d0d 0a6b 6579  T License"}..key
+00000480: 776f 7264 7320 3d20 5b22 6269 6f64 6567  words = ["biodeg
+00000490: 7261 6461 7469 6f6e 222c 2022 7265 6163  radation", "reac
+000004a0: 7469 7665 2074 7261 6e73 706f 7274 222c  tive transport",
+000004b0: 2022 6175 746f 6d61 7469 6f6e 222c 2022   "automation", "
+000004c0: 756e 6365 7274 6169 6e74 7920 7175 616e  uncertainty quan
+000004d0: 7469 6669 6361 7469 6f6e 225d 0d0a 0d0a  tification"]....
+000004e0: 5b70 726f 6a65 6374 2e75 726c 735d 0d0a  [project.urls]..
+000004f0: 7265 706f 7369 746f 7279 203d 2022 6874  repository = "ht
+00000500: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000510: 2f74 656d 6d79 3232 322f 5079 544f 5547  /temmy222/PyTOUG
+00000520: 4852 4541 4354 220d 0a0d 0a0d 0a0d 0a5b  HREACT"........[
+00000530: 746f 6f6c 2e63 6f76 6572 6167 652e 6874  tool.coverage.ht
+00000540: 6d6c 5d0d 0a64 6972 6563 746f 7279 203d  ml]..directory =
+00000550: 2022 636f 7665 7261 6765 5f68 746d 6c5f   "coverage_html_
+00000560: 7265 706f 7274 220d 0a0d 0a5b 746f 6f6c  report"....[tool
+00000570: 2e63 6f76 6572 6167 652e 7275 6e5d 0d0a  .coverage.run]..
+00000580: 6f6d 6974 203d 205b 0d0a 2020 2020 2320  omit = [..    # 
+00000590: 6f6d 6974 2061 6e79 7468 696e 6720 696e  omit anything in
+000005a0: 2061 202e 6c6f 6361 6c20 6469 7265 6374   a .local direct
+000005b0: 6f72 7920 616e 7977 6865 7265 0d0a 2020  ory anywhere..  
+000005c0: 2020 222a 2f6d 6f64 656c 2f2a 222c 0d0a    "*/model/*",..
+000005d0: 2020 2020 222a 2f63 6f6e 7374 616e 7473      "*/constants
+000005e0: 2f2a 222c 0d0a 2020 2020 222a 2f65 7863  /*",..    "*/exc
+000005f0: 6570 7469 6f6e 732f 2a22 2c0d 0a20 2020  eptions/*",..   
+00000600: 2023 206f 6d69 7420 6576 6572 7974 6869   # omit everythi
+00000610: 6e67 2069 6e20 2f75 7372 0d0a 2020 2020  ng in /usr..    
+00000620: 222f 7573 722f 2a22 2c0d 0a20 2020 2023  "/usr/*",..    #
+00000630: 206f 6d69 7420 7468 6973 2073 696e 676c   omit this singl
+00000640: 6520 6669 6c65 0d0a 2020 2020 2275 7469  e file..    "uti
+00000650: 6c73 2f74 6972 6566 6972 652e 7079 222c  ls/tirefire.py",
+00000660: 0d0a 2020 2020 5d0d 0a0d 0a5b 746f 6f6c  ..    ]....[tool
+00000670: 2e6d 7970 795d 0d0a 6d79 7079 5f70 6174  .mypy]..mypy_pat
+00000680: 6820 3d20 2273 7263 220d 0a63 6865 636b  h = "src"..check
+00000690: 5f75 6e74 7970 6564 5f64 6566 7320 3d20  _untyped_defs = 
+000006a0: 7472 7565 0d0a 6469 7361 6c6c 6f77 5f61  true..disallow_a
+000006b0: 6e79 5f67 656e 6572 6963 7320 3d20 7472  ny_generics = tr
+000006c0: 7565 0d0a 6967 6e6f 7265 5f6d 6973 7369  ue..ignore_missi
+000006d0: 6e67 5f69 6d70 6f72 7473 203d 2074 7275  ng_imports = tru
+000006e0: 650d 0a6e 6f5f 696d 706c 6963 6974 5f6f  e..no_implicit_o
+000006f0: 7074 696f 6e61 6c20 3d20 7472 7565 0d0a  ptional = true..
+00000700: 7368 6f77 5f65 7272 6f72 5f63 6f64 6573  show_error_codes
+00000710: 203d 2074 7275 650d 0a73 7472 6963 745f   = true..strict_
+00000720: 6571 7561 6c69 7479 203d 2074 7275 650d  equality = true.
+00000730: 0a77 6172 6e5f 7265 6475 6e64 616e 745f  .warn_redundant_
+00000740: 6361 7374 7320 3d20 7472 7565 0d0a 7761  casts = true..wa
+00000750: 726e 5f72 6574 7572 6e5f 616e 7920 3d20  rn_return_any = 
+00000760: 7472 7565 0d0a 7761 726e 5f75 6e72 6561  true..warn_unrea
+00000770: 6368 6162 6c65 203d 2074 7275 650d 0a77  chable = true..w
+00000780: 6172 6e5f 756e 7573 6564 5f63 6f6e 6669  arn_unused_confi
+00000790: 6773 203d 2074 7275 650d 0a6e 6f5f 696d  gs = true..no_im
+000007a0: 706c 6963 6974 5f72 6565 7870 6f72 7420  plicit_reexport 
+000007b0: 3d20 7472 7565 0d0a                      = true..
```

### Comparing `pytoughreact-1.0.3/setup.py` & `pytoughreact-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `pytoughreact-1.0.3/src/pytoughreact/__init__.py` & `pytoughreact-1.0.4/src/pytoughreact/__init__.py`

 * *Files identical despite different names*

### Comparing `pytoughreact-1.0.3/src/pytoughreact/chemical/bio_process_description.py` & `pytoughreact-1.0.4/src/pytoughreact/chemical/bio_process_description.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,14 +23,52 @@
 
 '''
 
 
 class BIODG(object):
     """Process specification"""
     def __init__(self, imonod, bfac, sw1, sw2, wea, wsub, processes, biomass, icflag=0):
+        """Initialization of Parameters
+
+        Parameters
+        -----------
+        imonod :  int
+            Selects between multiplicative and minimum Monod model for the substrate
+            degradation rate equation
+        bfac : float
+            Reduction factor criterion for local Newton-Raphson iteration in BIOREACT
+            subroutine to reduce substrate residual
+        sw1 : float
+            Lower limit of aqueous phase saturation considered in the saturation inhibition
+            function (if =0, the default value is 0.02)
+        sw2 : float
+            Upper limit of aqueous phase saturation considered in the saturation inhibition
+            function (SW1 < SW2 ≤ 1)
+        wea : float
+            Weighting factor for the linear interpolation of electron acceptor and nutrients
+            concentrations to be used in the substrate degradation rate equation (0 < WEA ≤
+            1). Default value is WEA = 0.5. WEA = 1 corresponds to using the concentration
+            evaluated at the end of the time step
+        wsub : float
+            weighting factor for the linear interpolation of substrate concentration to be used
+            in the substrate degradation rate equation (0 < WSUB ≤ 1). Default value is
+            WSUB = 0.5. WSUB=1 corresponds to using the concentration evaluated at the
+            end of the time step
+        processes: Process
+            List of Processes making use of this biodegradation configuration
+        biomass: Biomass
+            Biomass class list with all properties of the biomass
+        icflag: int
+            Selects how to consider the competitive and Haldane inhibition terms in the
+            Monod model
+
+        Returns
+        --------
+
+        """
         self.biomass = biomass
         self.icflag = icflag
         self.imonod = imonod
         self.processes = processes
         self.wsub = wsub
         self.wea = wea
         self.sw2 = sw2
@@ -45,15 +83,16 @@
         -----------
 
         Returns
         --------
         bio_numerical_parameters : list
             List of numerical parameters for biodegradation
         """
-        bio_numerical_parameters = [self.imonod, self.icflag, self.bfac, self.null, self.sw1, self.sw2, self.wea, self.wsub]
+        bio_numerical_parameters = [self.imonod, self.icflag, self.bfac, self.null, self.sw1, self.sw2,
+                                    self.wea, self.wsub]
         return bio_numerical_parameters
 
     def getNumberOfBiomasses(self):
         """ Function that gets the number of biomasses
 
         Parameters
         -----------
@@ -89,31 +128,48 @@
             if values[0][1] is not None:
                 print(keys[0].index)
 
 
 class Process(object):
     """Process specification"""
 
-    def __init__(self, biomass, numberOfComponents, mumax, yield_mass, enthalpy, totalComp=0, NumOfHaldane=0, NumOfNonCompetiting=0,
+    def __init__(self, biomass, numberOfComponents, mumax, yield_mass, enthalpy, totalComp=0,
+                 NumOfHaldane=0, NumOfNonCompetiting=0,
                  NumOfCompetiting=0, componentParams=None, gasParams=None, waterParams=None):
-        """ Initialization of Parameters
+        """Initialization of Parameters
 
         Parameters
         -----------
         biomass :  Biomass
-            This should be a Biomass class with all properties of the biomass
+            Biomass class with all properties of the biomass
         numberOfComponents : int
-            Number of Components present in the simulation
+            Number of mass components responsible for competitive inhibition in process
         mumax: float
             Maximum specific substrate degradation rate
+        yield_max: float
+            Yield coefficient for the growth of biomass due to the degradation of unit mass of
+            substrate in process IP (kg biomass / kg substrate)
+        enthalpy: float
+            Heat of reaction for the degradation of substrate in process (J/kg substrate)
+        totalComp: int
+            Number of mass components controlling the substrate degradation rate in process
+        NumOfHaldane: int
+            Number of mass components responsible for Haldane inhibition in process
+        NumOfNonCompetiting: int
+            Number of mass components responsible for non-competitive inhibition in process
+        componentParams : list
+            List of chemical components involved in the process
+        waterParams : list
+            List of water components involved in the process
+        gasParams : list
+            List of gas components involved in the process
 
         Returns
         --------
-        num_of_competiting : int
-            Number of Competiting species
+
         """
         self.enthalpy = enthalpy
         self.numberOfComponents = numberOfComponents
         self.yield_mass = yield_mass
         self.mumax = mumax
         self.biomass = biomass
         self.waterParams = waterParams
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/chemical/biomass_composition.py` & `pytoughreact-1.0.4/src/pytoughreact/chemical/biomass_composition.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             Non Competitive inhibition rate
         Kh: float
             Haldane inhibition rate
 
         Returns
         --------
         output : dict
-            Dicitionary of all parameters
+            Dictionary of all parameters
         process : Process
             Updated Process with new parameters
         """
         output = {self: [Uptake, Ks, Kc, Knc, Kh]}
         if Kc is not None:
             process.NumOfCompetiting += 1
         if Knc is not None:
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/chemical/mineral_composition.py` & `pytoughreact-1.0.4/src/pytoughreact/chemical/mineral_zone.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,22 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
 
-class MineralComp(object):
-    def __init__(self, mineral, init_volume_fraction, reaction_type, radius=None, reactive_surface_area=None, unit=None):
-        self.mineral = mineral
-        self.init_volume_fraction = init_volume_fraction
-        self.reaction_type = reaction_type
-        self.radius = radius
-        self.reactive_surface_area = reactive_surface_area
-        self.unit = unit
+class MineralZone(object):
+    def __init__(self, minerals):
+        """Initialization of Parameters
+
+        Parameters
+        -----------
+        minerals :  list[MineralComp]
+            List of all mineral compositions
+
+
+        Returns
+        --------
+
+        """
+        self.minerals = minerals
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/chemical/mineral_description.py` & `pytoughreact-1.0.4/src/pytoughreact/chemical/mineral_description.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,39 @@
 
 from copy import deepcopy
 from pytoughreact.constants.defaults_constants import DEFAULT_MINERAL_INCON
 
 
 class Mineral(object):
     def __init__(self, name, typeOfMineral, typeOfKC, indexSS, dryGridBlock):
+        """Initialization of Parameters
+
+        Parameters
+        -----------
+        name :  string
+            Name of the mineral phase,
+        typeOfMineral : int
+            Flag for the type of mineral: 0 for minerals at equilibrium, and 1 for those under kinetic
+            constraints
+        typeOfKC : int
+            Flag for the type of kinetic constraint: 1 for dissolution only, 2 for precipitation only, and 3
+            for both (mineral can either precipitate or dissolve
+        indexSS : int
+            Index for a solid solution mineral endmember. All endmembers for a specified phase are given the
+            same ISS value: ISS = 1 for each endmember of the first solid solution, ISS = 2 for each
+            endmember of the second solid solution
+        dryGridBlock : int
+            Flag to indicate that the mineral may precipitate in a dry grid block as a result of complete
+            evaporation (See user guide for more)
+
+
+        Returns
+        --------
+
+        """
         self.dryGridBlock = dryGridBlock
         self.indexSS = indexSS
         self.typeOfKC = typeOfKC
         self.typeOfMineral = typeOfMineral
         startIndex = name.find('\'')
         if startIndex >= 0:
             name = name.replace("'", "")
@@ -65,15 +90,16 @@
         Returns
         --------
         parameters : list
             List of parameters (rate constant, rate pH, activation energy) for dissolution
         """
         dissolution_data = self.dissolution[0]
         dissolution_data_list = [dissolution_data.rateConstant, dissolution_data.ratepH, dissolution_data.exponentN,
-                                 dissolution_data.exponentTheta, dissolution_data.activationEnergy, dissolution_data.coefA,
+                                 dissolution_data.exponentTheta, dissolution_data.activationEnergy,
+                                 dissolution_data.coefA,
                                  dissolution_data.coefB, dissolution_data.coefC]
         return dissolution_data_list
 
     def getComposition(self):
         return self.initial_composition
 
     def getPrecipitationParams(self):
@@ -84,17 +110,20 @@
 
         Returns
         --------
         parameters : list
             List of parameters (rate constant, rate pH, activation energy etc) for Precipitation
         """
         precipitation_data = self.precipitation[0]
-        precipitation_data_list = [precipitation_data.rateConstant, precipitation_data.ratepH, precipitation_data.exponentN,
-                                   precipitation_data.exponentTheta, precipitation_data.activationEnergy, precipitation_data.coefA,
-                                   precipitation_data.coefB, precipitation_data.coefC, precipitation_data.initVolumeFraction,
+        precipitation_data_list = [precipitation_data.rateConstant, precipitation_data.ratepH,
+                                   precipitation_data.exponentN,
+                                   precipitation_data.exponentTheta, precipitation_data.activationEnergy,
+                                   precipitation_data.coefA,
+                                   precipitation_data.coefB, precipitation_data.coefC,
+                                   precipitation_data.initVolumeFraction,
                                    precipitation_data.prepLawIndex]
         return precipitation_data_list
 
     def getPrecipitationParams2(self):
         """ Function that gets Precipitation parameters
 
         Parameters
@@ -102,15 +131,16 @@
 
         Returns
         --------
         parameters : list
             List of parameters () for Precipitation
         """
         precipitation_data_2 = self.precipitation[0]
-        precipitation_data_list_2 = [precipitation_data_2.logQKgap, precipitation_data_2.tempGap1, precipitation_data_2.tempGap2]
+        precipitation_data_list_2 = [precipitation_data_2.logQKgap, precipitation_data_2.tempGap1,
+                                     precipitation_data_2.tempGap2]
         return precipitation_data_list_2
 
     def getNumberOfpHDependence(self):
         """ Function that gets number of pH dependencies
 
         Parameters
         -----------
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/chemical/mineral_zone.py` & `pytoughreact-1.0.4/src/pytoughreact/constants/grid_constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,11 +19,9 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
-
-class MineralZone(object):
-    def __init__(self, minerals):
-        self.minerals = minerals
+GRID_NAME = 'GRID'
+CONNECTION = 'CONNE'
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/constants/cap_pressure_constants.py` & `pytoughreact-1.0.4/src/pytoughreact/constants/cap_pressure_constants.py`

 * *Files identical despite different names*

### Comparing `pytoughreact-1.0.3/src/pytoughreact/constants/default_minerals.py` & `pytoughreact-1.0.4/src/pytoughreact/constants/default_minerals.py`

 * *Files identical despite different names*

### Comparing `pytoughreact-1.0.3/src/pytoughreact/constants/defaults_constants.py` & `pytoughreact-1.0.4/src/pytoughreact/constants/defaults_constants.py`

 * *Files identical despite different names*

### Comparing `pytoughreact-1.0.3/src/pytoughreact/constants/format_specifications.py` & `pytoughreact-1.0.4/src/pytoughreact/constants/format_specifications.py`

 * *Files identical despite different names*

### Comparing `pytoughreact-1.0.3/src/pytoughreact/constants/generalconstants.py` & `pytoughreact-1.0.4/src/pytoughreact/constants/generalconstants.py`

 * *Files identical despite different names*

### Comparing `pytoughreact-1.0.3/src/pytoughreact/constants/grid_constants.py` & `pytoughreact-1.0.4/src/pytoughreact/constants/reactionconstants.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,9 +19,17 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
-GRID_NAME = 'GRID'
-CONNECTION = 'CONNE'
+TOBERMORITE_TOUGHREACT = 'tobermorite('
+TOBERMORITE_CONVERSION = 'Tobermorite'
+MONOSULFOALUMINATE_TOUGHREACT = 'monosulfoalu'
+MONOSULFOALUMINATE_CONVERSION = 'Monosulfoaluminate'
+KATOITE_TOUGHREACT = 'katoite'
+KATOITE_CONVERSION = 'Katoite'
+PH_TOUGHREACT = 'pH'
+C3FH6_TOUGHREACT = 'C3fh6'
+C3FH6_CONVERSION = 'C3FH6'
+CHANGE_IN_VOLUME_FRACTION = 'Change in volume fraction'
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/constants/plotconstants.py` & `pytoughreact-1.0.4/src/pytoughreact/constants/plotconstants.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 HORIZONTAL_ADDED = 'horizontal'
 VERTICAL_ADDED = 'vertical'
 DEPTH = 'depth'
 LAYER_FOR_LAYER = 'layer plot for layer'
 
 # Symbols
 COLOR_FORMAT = '--or'
-ALL_MARKERS = ["o", "v", "^", "<", ">", "1", "2", "3", "4", "8", "s", "p", "P", "*", "h", "H", "+", "x", "X", "D", "d", "|", "_"]
+ALL_MARKERS = ["o", "v", "^", "<", ">", "1", "2", "3", "4", "8", "s", "p", "P", "*",
+               "h", "H", "+", "x", "X", "D", "d", "|", "_"]
 ALL_COLORS = ['r', 'royalblue', 'g', 'k', 'c', 'm', 'y']
 X = 'x'
 Y = 'y'
 X_CAPS = 'X'
 Z_CAPS = 'Z'
 CARET_SYMBOL = '^'
 K_COLOR = 'k'
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/constants/rel_perm_constants.py` & `pytoughreact-1.0.4/src/pytoughreact/constants/rel_perm_constants.py`

 * *Files identical despite different names*

### Comparing `pytoughreact-1.0.3/src/pytoughreact/constants/sections.py` & `pytoughreact-1.0.4/src/pytoughreact/constants/sections.py`

 * *Files identical despite different names*

### Comparing `pytoughreact-1.0.3/src/pytoughreact/exceptions/custom_error.py` & `pytoughreact-1.0.4/src/pytoughreact/exceptions/custom_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 
 
 class RelativePermeabilityTypeError(Exception):
     """ Exception raised for wrong relative peremability inputs """
     def __init__(self, input_value, all_rel_perm_types):
         self.input_value = input_value
         self.all_rel_perm_types = all_rel_perm_types
-        self.message = '{0} is not one of the in-built relative permeability types. Please choose one of {1}'.format(self.input_value, self.all_rel_perm_types)
+        self.message = '{0} is not one of the in-built relative permeability types. \
+        Please choose one of {1}'.format(self.input_value, self.all_rel_perm_types)
         super().__init__(self.message)
 
 
 class NotFoundError(Exception):
     """ Exception raised when file is not found"""
     def __init__(self, input_value, directory):
         self.input_value = input_value
@@ -57,15 +58,16 @@
 
 
 class CapillaryPressureTypeError(Exception):
     """ Exception raised for wrong capillary pressure inputs """
     def __init__(self, input_value, all_cap_pres_types):
         self.input_value = input_value
         self.all_cap_pres_types = all_cap_pres_types
-        self.message = '{0} is not one of the in-built capillary pressure types. Please choose one of {1}'.format(self.input_value, self.all_cap_pres_types)
+        self.message = '{0} is not one of the in-built capillary pressure types. \
+            Please choose one of {1}'.format(self.input_value, self.all_cap_pres_types)
         super().__init__(self.message)
 
 
 class RestrictionError(Exception):
     def __init__(self, *args, condition_type):
         """ Exception raised for mathematical constraints of parameters """
         if condition_type == 'greater':
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/model/physical_model.py` & `pytoughreact-1.0.4/src/pytoughreact/wrapper/reactblock.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,77 +18,61 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
+from t2data import rocktype
+import numpy as np
 
-from t2data import mulgrid
-import t2data
-from pytoughreact.exceptions.custom_error import RequiredInputException
-from t2grids import t2grid
-from pytoughreact.numerical.physical_model_numericals import PhysicalNumericals
-import pytoughreact.constants.grid_constants as grid_constants
-from pytoughreact.model.relative_permeability import RelativePermeability
-
-
-class PhysicalModel(object):
-    def __init__(self, model_title) -> None:
-        self.data = t2data()
-        self.data.title = model_title
 
-    def createGrid(self, grid):
-        """ Creates Grid
+class t2block(object):
+    """Grid block"""
+    def __init__(self, name='     ', volume=1.0, blockrocktype=None, blockzone=None,
+                 centre=None, atmosphere=False, ahtx=None, pmx=None,
+                 nseq=None, nadd=None):
+        """ Initialization of parameters
 
         Parameters
         -----------
-        grid :  Grid
-            Grid object containing grid parameters
+        name : string
+            Name of the block
+        volume : float
+            Volume associated with the block
+        blockrocktype : rocktype
+            Rock type of the block
+        blockzone : t2zone
+            Zone the block is associated with
+        centre : float
+            Center of the block
+        atmosphere: boolean
+            If atmosphere present in block or not
+        ahtx: float
+            Interface area (m2) for linear heat exchange with semi-infinite confining
+            bed
+        pmx : float
+            Block-by-block permeability modification coefficient
+        nseq : int
+            Number of additional elements having the same volume and belonging to
+            the same reservoir domain
+        nadd : int
+            Increment between the code numbers of two successive elements
 
         Returns
         --------
-        geo : mulgrid
-            mulgrid parameter with all grid parameters
 
         """
-        if grid:
-            geo = mulgrid().rectangular(grid.x_dimension, grid.y_dimension, grid.z_dimension, grid.grid_top)
-            self.geo = geo
-        else:
-            raise RequiredInputException(grid_constants.GRID_NAME)
-        return geo
-
-    def convertGrid(self):
-        self.data.grid = t2grid().fromgeo(self.geo)
-
-    def storeGridData(self, file_name):
-        if self.geo:
-            self.geo.write(file_name)
-
-    def specifyGravity(self, gravity=9.81):
-        self.gravity = gravity
-
-    def initialConditions(self, temperature, pressure):
-        self.temperature = temperature
-        self.pressure = pressure
-
-    def defineNumericals(self):
-        numerical = PhysicalNumericals()
-        self.numerical = numerical
-
-    def relative_permeability(self, type_rel, parameters):
-        rel_perm_def = RelativePermeability(type_rel, parameters)
-        rel_perm = rel_perm_def.rel_perm_converter()
-        self.rel_perm = rel_perm
-
-    def domain_parameters(self, rock_type, perm, porosity, initial_pressure, initial_temp, density, conductivity=None, specific_heat=None):
-        self.density = density
-        self.initial_pressure = initial_pressure
-        self.initial_temp = initial_temp
-        self.specific_heat = specific_heat
-        self.conductivity = conductivity
-        assert isinstance(perm, dict)
-        self.perm = perm
-        self.poro = porosity
-        assert isinstance(rock_type, list)
-        self.rock_type = rock_type
+        self.zone = blockzone
+        if blockrocktype is None:
+            blockrocktype = rocktype()
+        self.name = name
+        self.volume = volume
+        self.rocktype = blockrocktype
+        if isinstance(centre, list):
+            centre = np.array(centre)
+        self.centre = centre
+        self.atmosphere = atmosphere
+        self.ahtx = ahtx
+        self.pmx = pmx
+        self.nseq, self.nadd = nseq, nadd
+        self.connection_name = set([])
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/plotting/plot_multiple.py` & `pytoughreact-1.0.4/src/pytoughreact/plotting/plot_multiple.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 
 '''
 
 from pytoughreact.plotting.plot_multiple_files_routine import PlotMultiFiles
 
 
 class PlotMultiple(object):
-    def __init__(self, simulator_type, file_locations, file_titles, props, **kwargs):
+    def __init__(self, simulator_type, file_locations, file_titles, props,
+                 **kwargs):
         """
         Class for processing multiple file results
 
         Parameters
         -----------
         file_locations :  list[str]
             specifies the location of the files on the syste
@@ -46,96 +47,107 @@
 
         x_slice value : int
             value at which the plot should be sliced at the  x axis
         per_file : boolean
             if the plot should be made per file and not per property
         tile : str
             title of each of the plots
-        
-        
+
+
         Returns
         --------
 
         """
         assert isinstance(file_locations, list)
         assert isinstance(file_titles, list)
         self.file_locations = file_locations
         self.file_titles = file_titles
         self.simulator_type = simulator_type
         self.props = props
         self.x_slice_value = kwargs.get('x_slice_value')
         self.per_file = kwargs.get('per_file')
         self.title = kwargs.get('title')
 
-    def plotTime(self, grid_block_number, legend, plot_kind='property', format_of_date='day'):
+    def plotTime(self, grid_block_number, legend, plot_kind='property',
+                 format_of_date='day'):
         """ Line Plots of a parameter in the results file as a function of time
 
         Parameters
         -----------
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
         legend: list[str]
             List of all legend values
         plot_kind: str
             if plot should be structured by property or file
-        
-        
+
+
         Returns
         --------
-        
+
         """
-        plottest = PlotMultiFiles(self.simulator_type, self.file_locations, self.file_titles, self.props,
-                                  x_slice_value=self.x_slice_value, per_file=self.per_file, title=self.title)
+        plottest = PlotMultiFiles(self.simulator_type, self.file_locations,
+                                  self.file_titles, self.props,
+                                  x_slice_value=self.x_slice_value,
+                                  per_file=self.per_file, title=self.title)
         if len(self.props) == 1:
             plottest.multiFileSinglePlot(grid_block_number, legend)
         else:
-            plottest.plotMultiElementMultiFile(grid_block_number, legend, format_of_date, plot_kind)
+            plottest.plotMultiElementMultiFile(grid_block_number, legend,
+                                               format_of_date, plot_kind)
 
-    def plotTimePerPanel(self, grid_block_number, panels, format_of_date='day'):
+    def plotTimePerPanel(self, grid_block_number, panels,
+                         format_of_date='day'):
         """ Plot Multiple plots in a panel
 
         Parameters
         -----------
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
         panels: list[str]
             List of all panels
-        
-        
+
+
         Returns
         --------
-        
+
         """
-        plottest = PlotMultiFiles(self.simulator_type, self.file_locations, self.file_titles, self.props,
-                                  x_slice_value=self.x_slice_value, per_file=self.per_file, title=self.title)
+        plottest = PlotMultiFiles(self.simulator_type, self.file_locations,
+                                  self.file_titles, self.props,
+                                  x_slice_value=self.x_slice_value,
+                                  per_file=self.per_file, title=self.title)
         plottest.plotMultiPerPanel(grid_block_number, panels, format_of_date)
 
-    def plotParamWithLayer(self, direction_x, direction_y, layer_num, time, legend):
+    def plotParamWithLayer(self, direction_x, direction_y, layer_num, time,
+                           legend):
         """ Plot of Parameter with Layer
 
         Parameters
         -----------
         direction_x :  str
-            The direction to be plotted on the x axis 
+            The direction to be plotted on the x axis
         direction_y :  str
             The direction to be plotted on the y axis
         legend :  list[str]
             List of legend values
         layer_num :  int
             The layer in the model to be plotted
         time : int
             the time at which the plot is to be made
-        
+
         Returns
         --------
-        
+
         """
-        plottest = PlotMultiFiles(self.simulator_type, self.file_locations, self.file_titles, self.props,
-                                  x_slice_value=self.x_slice_value, per_file=self.per_file, title=self.title)
+        plottest = PlotMultiFiles(self.simulator_type, self.file_locations,
+                                  self.file_titles, self.props,
+                                  x_slice_value=self.x_slice_value,
+                                  per_file=self.per_file, title=self.title)
         if len(self.props) == 1:
             pass
         else:
-            plottest.plotMultiFileDistance(direction_x, direction_y, time, layer_num, legend)
+            plottest.plotMultiFileDistance(direction_x, direction_y, time,
+                                           layer_num, legend)
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/plotting/plot_multiple_files_routine.py` & `pytoughreact-1.0.4/src/pytoughreact/plotting/plot_multiple_files_routine.py`

 * *Files 25% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 import pytoughreact.constants.plotconstants as pc
 import pytoughreact.constants.reactionconstants as rc
 
 from pytoughreact.utilities.t2_utilities import t2Utilities
 
 
 class PlotMultiFiles(object):
-    def __init__(self, simulator_type, file_locations, file_titles, props, **kwargs):
+    def __init__(self, simulator_type, file_locations, file_titles, props,
+                 **kwargs):
         """
         Class for processing multiple file results
 
         Parameters
         -----------
         file_locations :  list[str]
             specifies the location of the files on the syste
@@ -57,16 +58,16 @@
 
         x_slice value : int
             value at which the plot should be sliced at the  x axis
         per_file : boolean
             if the plot should be made per file and not per property
         tile : str
             title of each of the plots
-        
-        
+
+
         Returns
         --------
 
         """
         assert isinstance(file_locations, list)
         assert isinstance(file_titles, list)
         assert isinstance(props, list)
@@ -79,32 +80,39 @@
         self.per_file = kwargs.get(gc.PER_FILE)
         self.title = kwargs.get(gc.TITLE)
 
     def _validateInput(self):
         """ Validate Inputs
         """
         if self.simulator_type.lower() == gc.TOUGHREACT:
-            multi_tough = MultiResultReact(self.simulator_type, self.file_locations, self.file_titles, self.props,
+            multi_tough = MultiResultReact(self.simulator_type,
+                                           self.file_locations,
+                                           self.file_titles,
+                                           self.props,
                                            x_slice_value=self.x_slice_value)
         elif self.simulator_type.lower() == gc.TMVOC:
-            multi_tough = MultiResultTough3(self.simulator_type, self.file_locations, self.file_titles, self.props)
+            multi_tough = MultiResultTough3(self.simulator_type,
+                                            self.file_locations,
+                                            self.file_titles,
+                                            self.props)
         else:
-            print("Code only has capability for TOUGHREACT or TOUGH3 (by extension TMVOC)")
+            print("Code only has capability for TOUGHREACT or TOUGH3 \
+                  (by extension TMVOC)")
         return multi_tough
 
     def _plotRawSingle(self, data, legend):
         """ Plot of Single File
 
         Parameters
         -----------
         data :  pd.DataFrame
             data for plot
         legend :  list[str]
             List of legend values
-        
+
         Returns
         --------
         """
         prop_index = 0
         fig, axs = plt.subplots(1, 1)
         for i in range(0, len(data.columns), 2):
             x_data = data.iloc[:, i]
@@ -115,69 +123,73 @@
             axs.legend(legend, loc=pc.LOC_BEST)
             axs.ticklabel_format(useOffset=False)
         plt.setp(axs.get_xticklabels(), fontsize=14)
         plt.setp(axs.get_yticklabels(), fontsize=14)
         os.chdir(self.file_locations[0])
         plt.tight_layout()
         plt.show()
-        fig.savefig(self.props[0] + ' ' + pc.DIFFERENT_FILES_TAG + ' ' + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(self.props[0] + ' ' + pc.DIFFERENT_FILES_TAG + ' ' +
+                    pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
 
     def _plotRawMulti(self, data, legend):
         """ Plot of Multi File
 
         Parameters
         -----------
         data :  pd.DataFrame
             data for plot
         legend :  list[str]
             List of legend values
-        
+
         Returns
         --------
         """
-        
+
         fig = plt.figure()
         plot_counter = 1
         start_point = 0
         prop_index = 0
         initial_length = len(self.props) * 2
         for number in range(1, len(self.props)):
             axs = plt.subplot(3, 2, plot_counter)
             legend_index = 0
             for i in range(start_point, initial_length, 2):
                 x_data = data.iloc[:, i]
                 y_data = data.iloc[:, i + 1]
-                axs.plot(x_data, y_data, marker=pc.CARET_SYMBOL, label=legend[legend_index])
+                axs.plot(x_data, y_data, marker=pc.CARET_SYMBOL,
+                         label=legend[legend_index])
                 axs.set_xlabel(pc.X_LABEL_TIME_YEAR)
                 axs.set_ylabel(self.props[prop_index])
                 legend_index = legend_index + 1
             plot_counter = plot_counter + 1
             start_point = start_point + (len(self.props) * 2)
             initial_length = initial_length + (len(self.props) * 2)
             prop_index = prop_index + 1
         handles, labels = axs.get_legend_handles_labels()
         plt.setp(axs.get_xticklabels(), fontsize=14)
         plt.setp(axs.get_yticklabels(), fontsize=14)
-        plt.figlegend(handles, labels, loc=pc.LOC_LOWER_CENTER, ncol=5, labelspacing=0.)
+        plt.figlegend(handles, labels, loc=pc.LOC_LOWER_CENTER, ncol=5,
+                      labelspacing=0.)
         plt.show()
-        fig.savefig(self.props[0] + ' ' + pc.DIFFERENT_FILES_TAG + ' ' + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(self.props[0] + ' ' + pc.DIFFERENT_FILES_TAG + ' ' +
+                    pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
 
     def _setToughYLabel(self, value):
         """ Convert the value in tough results to understandable values
 
         Parameters
         -----------
         value :  str
             value to be converted (must be present in TOUGH data output)
-        
+
         Returns
         --------
         value :  str
             converted value
-        
+
         """
         if rc.TOBERMORITE_TOUGHREACT in value:
             value = rc.TOBERMORITE_CONVERSION
         elif rc.MONOSULFOALUMINATE_TOUGHREACT in value:
             value = rc.MONOSULFOALUMINATE_CONVERSION
         elif rc.KATOITE_TOUGHREACT in value:
             value = rc.KATOITE_CONVERSION
@@ -196,329 +208,363 @@
         -----------
         data :  pd.DataFrame
             data for plot
         legend :  list[str]
             List of legend values
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
+
         Returns
         --------
-        
+
         """
         fig = plt.figure(figsize=(10, 10))
         plot_counter = 1
         start_point = 0
         prop_index = 0
         markers = pc.ALL_MARKERS
         for number in range(1, len(self.props) + 1):
             if number == 4:
                 pass
-            axs = plt.subplot(math.ceil(len(self.props) / 2) + 1, 2, plot_counter)
+            axs = plt.subplot(math.ceil(len(self.props) / 2) + 1, 2,
+                              plot_counter)
             legend_index = 0
-            for i in range(start_point, len(data.columns), (len(self.props) * 2)):
+            for i in range(start_point, len(data.columns),
+                           (len(self.props) * 2)):
                 x_data = data.iloc[:, i]
                 y_data = data.iloc[:, i + 1]
-                axs.plot(x_data, y_data, marker=markers[legend_index], label=legend[legend_index])
-                axs.set_xlabel('Time ' + '(' + format_of_date + ')', fontsize=14)
-                axs.set_ylabel(self._setToughYLabel(self.props[prop_index]), fontsize=14)
+                axs.plot(x_data, y_data, marker=markers[legend_index],
+                         label=legend[legend_index])
+                axs.set_xlabel('Time ' + '(' + format_of_date + ')',
+                               fontsize=14)
+                axs.set_ylabel(self._setToughYLabel(self.props[prop_index]),
+                               fontsize=14)
                 axs.ticklabel_format(useOffset=False)
                 legend_index = legend_index + 1
             plot_counter = plot_counter + 1
             start_point = start_point + 2
             prop_index = prop_index + 1
             plt.setp(axs.get_xticklabels(), fontsize=14)
             plt.setp(axs.get_yticklabels(), fontsize=14)
         handles, labels = axs.get_legend_handles_labels()
         fig.tight_layout()
         if len(self.props) > 3:
-            plt.figlegend(handles, labels, loc=pc.LOC_LOWER_CENTER, ncol=4, labelspacing=0.)
+            plt.figlegend(handles, labels, loc=pc.LOC_LOWER_CENTER, ncol=4,
+                          labelspacing=0.)
         else:
-            plt.figlegend(handles, labels, loc=pc.LOC_LOWER_CENTER, ncol=4, labelspacing=0.)
+            plt.figlegend(handles, labels, loc=pc.LOC_LOWER_CENTER, ncol=4,
+                          labelspacing=0.)
         plt.show()
         os.chdir(self.file_locations[0])
-        fig.savefig(self.props[0] + ' ' + pc.DIFFERENT_FILES_TAG + ' ' + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(self.props[0] + ' ' + pc.DIFFERENT_FILES_TAG + ' ' +
+                    pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
 
     def _plotRawMultiFilePanel(self, data, panels, format_of_date):
         """ Plot of Multi File Per Panel
 
         Parameters
         -----------
         data :  pd.DataFrame
             data for plot
         panels :  int
             Number of panels
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
+
         Returns
         --------
-        
+
         """
         fig = plt.figure(figsize=(10, 8))
         start_point = 0
         # markers = pc.ALL_MARKERS
         fig, axs = plt.subplots(2, 2)
         number = 0
         length_of_prop = len(list(panels[number].values())[0][0])
         for i in range(0, len(panels)):
             x_data = data.iloc[:, start_point]
-            y_data = data.iloc[:, start_point + 1:start_point + length_of_prop + 1]
+            y_data = data.iloc[:, start_point + 1:start_point + length_of_prop
+                               + 1]
             number += 1
             start_point = start_point + length_of_prop + 1
             try:
                 length_of_prop = len(list(panels[number].values())[0][0])
             except IndexError:
                 pass
             if i == 0:
                 # marker = itertools.cycle((',', '+', '.', 'o', '*'))
                 axsa = axs[0, 0]
                 axsa.plot(x_data, y_data)
                 yLabel = list(panels[0].values())[0][2][0]
                 axsa.set_xlabel('Time ' + format_of_date, fontsize=12)
                 axsa.set_ylabel(yLabel, fontsize=12)
                 axsa.ticklabel_format(useOffset=False)
-                axsa.legend(list(panels[0].values())[0][1], fontsize=12, loc=pc.LOC_BEST, shadow=True, fancybox=True)
+                axsa.legend(list(panels[0].values())[0][1], fontsize=12,
+                            loc=pc.LOC_BEST, shadow=True, fancybox=True)
             elif i == 1:
                 axsa = axs[0, 1]
                 axsa.plot(x_data, y_data)
                 yLabel = list(panels[1].values())[0][2][0]
                 axsa.set_xlabel(pc.X_LABEL_TIME_YEAR, fontsize=12)
                 axsa.set_ylabel(yLabel, fontsize=12)
                 axsa.ticklabel_format(useOffset=False)
-                axsa.legend(list(panels[1].values())[0][1], fontsize=12, loc=pc.LOC_BEST, shadow=True, fancybox=True)
+                axsa.legend(list(panels[1].values())[0][1], fontsize=12,
+                            loc=pc.LOC_BEST, shadow=True, fancybox=True)
             elif i == 2:
                 axsa = axs[1, 0]
                 axsa.plot(x_data, y_data)
                 yLabel = list(panels[2].values())[0][2][0]
                 axsa.set_xlabel(pc.X_LABEL_TIME_YEAR, fontsize=12)
                 axsa.set_ylabel(yLabel, fontsize=12)
                 axsa.ticklabel_format(useOffset=False)
-                axsa.legend(list(panels[2].values())[0][1], fontsize=12, loc=pc.LOC_BEST, shadow=True, fancybox=True)
+                axsa.legend(list(panels[2].values())[0][1], fontsize=12,
+                            loc=pc.LOC_BEST, shadow=True, fancybox=True)
             elif i == 3:
                 axsa = axs[1, 1]
                 axsa.plot(x_data, y_data)
                 yLabel = list(panels[3].values())[0][2][0]
                 axsa.set_xlabel(pc.X_LABEL_TIME_YEAR, fontsize=12)
                 axsa.set_ylabel(yLabel, fontsize=12)
                 axsa.ticklabel_format(useOffset=False)
-                axsa.legend(list(panels[3].values())[0][1], fontsize=10, loc=pc.LOC_BEST, shadow=True, fancybox=True)
+                axsa.legend(list(panels[3].values())[0][1], fontsize=10,
+                            loc=pc.LOC_BEST, shadow=True, fancybox=True)
         fig.tight_layout()
         plt.show()
-        fig.savefig(list(panels[0].values())[0][0][0] + pc.MULTI_PLOTS_PER_PANEL + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(list(panels[0].values())[0][0][0] +
+                    pc.MULTI_PLOTS_PER_PANEL + pc.IMAGE_TYPE,
+                    bbox_inches=pc.TIGHT_BBOX, dpi=600)
 
     def _plotRawMultiFilePerFile(self, data, legend):
         """ Plot of Multi File Per File
 
         Parameters
         -----------
         data :  pd.DataFrame
             data for plot
         legend :  list[str]
             List of legend values
-        
+
         Returns
         --------
-        
+
         """
         fig = plt.figure(figsize=(10, 8))
         plot_counter = 1
         start_point = 0
         prop_index = 0
         markers = pc.ALL_MARKERS
         for number in range(1, len(self.props) + 1):
             axs = plt.subplot(3, 2, plot_counter)
             legend_index = 0
-            for i in range(start_point, len(data.columns), (len(self.props) * 2)):
+            for i in range(start_point, len(data.columns), (len(self.props)
+                                                            * 2)):
                 x_data = data.iloc[:, i]
                 y_data = data.iloc[:, i + 1]
                 if gc.POROSITY in data.columns[i]:
                     axs.plot(x_data, y_data, marker=markers[legend_index],
                              label=self._setToughYLabel(legend[legend_index]))
                     axs.set_xlabel(pc.X_LABEL_TIME_YEAR, fontsize=14)
                     if self.simulator_type.lower() == gc.TMVOC:
-                        axs.set_ylabel(self.modifier.param_label_full(self.props[prop_index]), fontsize=14)
+                        axs.set_ylabel(
+                            self.modifier.param_label_full(
+                                self.props[prop_index]), fontsize=14)
                     else:
-                        axs.set_ylabel(rc.CHANGE_IN_VOLUME_FRACTION, fontsize=14)
+                        axs.set_ylabel(rc.CHANGE_IN_VOLUME_FRACTION,
+                                       fontsize=14)
                 else:
                     axs.plot(x_data, y_data, marker=markers[legend_index],
                              label=self._setToughYLabel(legend[legend_index]))
                     axs.set_xlabel(pc.X_LABEL_TIME_YEAR, fontsize=14)
                     if self.simulator_type.lower() == gc.TMVOC:
-                        param_value = self.modifier.param_label_full(self.props[prop_index].upper())
+                        param_value = self.modifier.param_label_full(
+                            self.props[prop_index].upper())
                         axs.set_ylabel(param_value, fontsize=14)
                     else:
-                        axs.set_ylabel(rc.CHANGE_IN_VOLUME_FRACTION, fontsize=14)
+                        axs.set_ylabel(rc.CHANGE_IN_VOLUME_FRACTION,
+                                       fontsize=14)
                 axs.ticklabel_format(useOffset=False)
                 plt.setp(axs.get_xticklabels(), fontsize=14)
                 plt.setp(axs.get_yticklabels(), fontsize=14)
                 legend_index = legend_index + 1
             # axs.set_title(self.title[prop_index], fontsize='14')
             axs.set_title(self.props[prop_index], fontsize='14')
             plot_counter = plot_counter + 1
             start_point = start_point + 2
             prop_index = prop_index + 1
         handles, labels = axs.get_legend_handles_labels()
         # handles2, labels2 = ax2s.get_legend_handles_labels()
         # handles.append(handles2[0])
         # labels.append(labels2[0])
-        plt.figlegend(handles, labels, loc=pc.LOC_LOWER_CENTER, ncol=4, labelspacing=0.)
+        plt.figlegend(handles, labels, loc=pc.LOC_LOWER_CENTER, ncol=4,
+                      labelspacing=0.)
         fig.tight_layout()
         plt.show()
         os.chdir(self.file_locations[0])
-        fig.savefig(self.props[0] + ' ' + pc.DIFFERENT_FILES_TAG + ' ' + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(self.props[0] + ' ' + pc.DIFFERENT_FILES_TAG + ' '
+                    + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
 
     def multiFileSinglePlot(self, grid_block_number, legend):
         """ Plot of  Multiple Files with a single plot
 
         Parameters
         -----------
         grid_block_number :  int
-            The grid block number to be plotted 
+            The grid block number to be plotted
         legend :  list[str]
             List of legend values
-        
+
         Returns
         --------
-        
+
         """
         multi_tough = self._validateInput()
         data = multi_tough.retrieve_data_multi_timeseries(grid_block_number)
         try:
             with plt.style.context(pc.MY_STYLE):
                 self._plotRawSingle(data, legend)
         except Exception:
             with plt.style.context(pc.CLASSIC):
                 self._plotRawSingle(data, legend)
 
-    def _plotMultiElementMultiFilePerFile(self, grid_block_number, legend, format_of_date):
+    def _plotMultiElementMultiFilePerFile(self, grid_block_number, legend,
+                                          format_of_date):
         """ Plot of Multi Elements and Multiple Files for File only
 
         Parameters
         -----------
         grid_block_number :  int
-            The grid block number to be plotted 
+            The grid block number to be plotted
         legend :  list[str]
             List of legend values
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
+
         Returns
         --------
-        
+
         """
         multi_tough = self._validateInput()
-        data = multi_tough.getMultiElementData(grid_block_number, format_of_date)
+        data = multi_tough.getMultiElementData(grid_block_number,
+                                               format_of_date)
         try:
             with plt.style.context(pc.MY_STYLE):
                 self._plotRawMultiFilePerFile(data, legend)
         except Exception:
             with plt.style.context(pc.CLASSIC):
                 self._plotRawMultiFilePerFile(data, legend)
 
-    def _plotMultiElementMultiFilePerProp(self, grid_block_number, legend, format_of_date):
+    def _plotMultiElementMultiFilePerProp(self, grid_block_number, legend,
+                                          format_of_date):
         """ Plot of Multi Elements and Multiple Files for Property only
 
         Parameters
         -----------
         grid_block_number :  int
-            The grid block number to be plotted 
+            The grid block number to be plotted
         legend :  list[str]
             List of legend values
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
+
         Returns
         --------
-        
+
         """
         multi_tough = self._validateInput()
-        data = multi_tough.getMultiElementData(grid_block_number, format_of_date)
+        data = multi_tough.getMultiElementData(grid_block_number,
+                                               format_of_date)
         try:
             with plt.style.context(pc.MY_STYLE):
                 self._plotRawMultiFile(data, legend, format_of_date)
         except Exception:
             with plt.style.context(pc.CLASSIC):
                 self._plotRawMultiFile(data, legend, format_of_date)
 
-    def plotMultiElementMultiFile(self, grid_block_number, legend, format_of_date, plot_kind=pc.PROPERTY):
+    def plotMultiElementMultiFile(self, grid_block_number, legend,
+                                  format_of_date, plot_kind=pc.PROPERTY):
         """ Plot of Multi Elements and Multiple Files
 
         Parameters
         -----------
         grid_block_number :  int
-            The grid block number to be plotted 
+            The grid block number to be plotted
         legend :  list[str]
             List of legend values
         format_of_date: str
             The format of the date; could be minute, hour, day or year
         plot_kind: str
             The kind of plot to be used; could be 'property' or 'file'
-        
+
         Returns
         --------
-        
+
         """
         if plot_kind.lower() == pc.PROPERTY:
-            self._plotMultiElementMultiFilePerProp(grid_block_number, legend, format_of_date)
+            self._plotMultiElementMultiFilePerProp(grid_block_number, legend,
+                                                   format_of_date)
         elif plot_kind.lower() == pc.FILE:
-            self._plotMultiElementMultiFilePerFile(grid_block_number, legend, format_of_date)
+            self._plotMultiElementMultiFilePerFile(grid_block_number, legend,
+                                                   format_of_date)
         else:
             print('Plot kind can either be property or file')
 
-    def plotMultiPerPanel(self, grid_block_number, panels, format_of_date=pc.DAY):
+    def plotMultiPerPanel(self, grid_block_number, panels,
+                          format_of_date=pc.DAY):
         """ Plot of Multi Properties Per Panel
 
         Parameters
         -----------
         grid_block_number :  int
-            The grid block number to be plotted 
+            The grid block number to be plotted
         panels :  int
             Number of panels
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
+
         Returns
         --------
-        
+
         """
         multi_tough = self._validateInput()
-        data = multi_tough.getMultiElementDataPerPanel(grid_block_number, panels, format_of_date)
+        data = multi_tough.getMultiElementDataPerPanel(grid_block_number,
+                                                       panels, format_of_date)
         if self.x_slice_value is not None:
             stringo = panels[0]['panel1'][0][0] + 'time00'
             data = data[data[stringo] <= self.x_slice_value]
         try:
             with plt.style.context(pc.MY_STYLE):
                 self._plotRawMultiFilePanel(data, panels, format_of_date)
         except Exception:
             with plt.style.context(pc.CLASSIC):
                 self._plotRawMultiFilePanel(data, panels, format_of_date)
 
-    def plotMultiFileDistance(self, direction_x, direction_y, time, layer_num, legend):
+    def plotMultiFileDistance(self, direction_x, direction_y, time, layer_num,
+                              legend):
         """ Plot of Parameter with Distance for Multiple Files
 
         Parameters
         -----------
         direction_x :  str
-            The direction to be plotted on the x axis 
+            The direction to be plotted on the x axis
         direction_y :  str
             The direction to be plotted on the y axis
         legend :  list[str]
             List of legend values
         layer_num :  int
             The layer in the model to be plotted
         time : int
             the time at which the plot is to be made
-        
+
         Returns
         --------
-        
+
         """
         multi_tough = self._validateInput()
-        data = multi_tough.getMultiFileDistance(direction_x, direction_y, time, layer_num)
+        data = multi_tough.getMultiFileDistance(direction_x, direction_y, time,
+                                                layer_num)
         if self.per_file is True:
             try:
                 with plt.style.context(pc.MY_STYLE):
                     self._plotRawMultiFilePerFile(data, legend)
             except Exception:
                 with plt.style.context(pc.CLASSIC):
                     self._plotRawMultiFilePerFile(data, legend)
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/plotting/plot_multiple_tough_routine.py` & `pytoughreact-1.0.4/src/pytoughreact/plotting/plot_multiple_tough_routine.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
         generation : str
             generation file location
         restart_files : str
             restart file location
         experiment : str
             experimental file location
-        
-        
+
+
         Returns
         --------
 
         """
         self.filelocations = filelocations
         self.filetitles = filetitles
         self.simulatortype = simulatortype
@@ -72,24 +72,28 @@
         self.generation = kwargs.get(gc.GENERATION)
         self.args = kwargs.get(gc.RESTART_FILES)
         self.expt = kwargs.get(gc.EXPERIMENT)
         self.x_slice_value = kwargs.get(gc.X_SLICE_VALUE)
 
     def read_file(self):
         os.chdir(self.filelocations)
-        if self.simulatortype.lower() == gc.TMVOC or self.simulatortype.lower() == gc.TOUGH3:
-            fileReader = ResultTough3(self.simulatortype, self.filelocations, self.filetitles,
+        if (self.simulatortype.lower() == gc.TMVOC or
+                self.simulatortype.lower() == gc.TOUGH3):
+            fileReader = ResultTough3(self.simulatortype, self.filelocations,
+                                      self.filetitles,
                                       generation=self.generation)
         else:
-            fileReader = ResultReact(self.simulatortype, self.filelocations, self.filetitles)
+            fileReader = ResultReact(self.simulatortype, self.filelocations,
+                                     self.filetitles)
         return fileReader
 
     def read_file_multi(self, file, filetitle):
         os.chdir(file)
-        if self.simulatortype.lower() == gc.TMVOC or self.simulatortype.lower() == gc.TOUGH3:
+        if (self.simulatortype.lower() == gc.TMVOC or
+                self.simulatortype.lower() == gc.TOUGH3):
             fileReader = ResultTough3(self.simulatortype, file, filetitle)
         else:
             fileReader = ResultReact(self.simulatortype, file, filetitle)
         return fileReader
 
     def getRestartLocations(self):
         restart_files = list()
@@ -97,73 +101,86 @@
         restart_files = restart_files + self.args
         return restart_files
 
     def getRestartDataTime(self, format_of_date):
         locations = self.getRestartLocations()
         final_time = []
         for i in range(0, len(locations)):
-            if self.simulatortype.lower() == gc.TMVOC or self.simulatortype.lower() == gc.TOUGH3:
-                fileReader = ResultTough3(self.simulatortype, locations[i], self.filetitle)
+            if (self.simulatortype.lower() == gc.TMVOC or
+                    self.simulatortype.lower() == gc.TOUGH3):
+                fileReader = ResultTough3(self.simulatortype, locations[i],
+                                          self.filetitle)
             else:
-                fileReader = ResultReact(self.simulatortype, locations[i], self.filetitles)
+                fileReader = ResultReact(self.simulatortype, locations[i],
+                                         self.filetitles)
             if i == 0:
                 time_year = fileReader.convert_times(format_of_date)
                 final_time.append(time_year)
             else:
                 time_year = fileReader.convert_times(format_of_date)
                 time_year = time_year[1:]
                 final_time.append(time_year)
         final_time = list(itertools.chain.from_iterable(final_time))
         return final_time
 
     def getRestartDataElement(self, param, gridblocknumber):
         locations = self.getRestartLocations()
         final_result = []
         for i in range(0, len(locations)):
-            if self.simulatortype.lower() == gc.TMVOC or self.simulatortype.lower() == gc.TOUGH3:
-                fileReader = ResultTough3(self.simulatortype, locations[i], self.filetitles)
+            if (self.simulatortype.lower() == gc.TMVOC or
+                    self.simulatortype.lower() == gc.TOUGH3):
+                fileReader = ResultTough3(self.simulatortype, locations[i],
+                                          self.filetitles)
             else:
-                fileReader = ResultReact(self.simulatortype, locations[i], self.filetitles)
+                fileReader = ResultReact(self.simulatortype, locations[i],
+                                         self.filetitles)
             if i == 0:
-                result_array = fileReader.get_timeseries_data(param, gridblocknumber)
+                result_array = fileReader.get_timeseries_data(param,
+                                                              gridblocknumber)
                 final_result.append(result_array)
             else:
-                result_array = fileReader.get_timeseries_data(param, gridblocknumber)
+                result_array = fileReader.get_timeseries_data(param,
+                                                              gridblocknumber)
                 result_array = result_array[1:]
                 final_result.append(result_array)
         final_result = list(itertools.chain.from_iterable(final_result))
         return final_result
 
-    def _raw_multi_plot_restart_horizontal(self, param, format_of_date, gridblocknumber):
-        """ Line Plots of a multiple parameter in the results file as a function of time in horizontal orientation with restart
+    def _raw_multi_plot_restart_horizontal(self, param, format_of_date,
+                                           gridblocknumber):
+        """ Line Plots of a multiple parameter in the results file as a
+        function of time in horizontal orientation with restart
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
-        
+
+
         Returns
         --------
-        
+
         """
         time_year = self.getRestartDataTime(format_of_date)
         j = 0
         fig, axs = plt.subplots(len(param), sharex=False)
         for parameter in param:
-            result_array = self.getRestartDataElement(parameter, gridblocknumber)
+            result_array = self.getRestartDataElement(parameter,
+                                                      gridblocknumber)
             parameters = t2Utilities()
-            time_year, result_array = parameters.removeRepetiting(time_year, result_array)
+            time_year, result_array = parameters.remove_repetiting(time_year, result_array)
             axs[j].plot(time_year, result_array, marker=pc.CARET,
-                        label=self.modifier.param_label_full(parameter.upper()))
-            axs[j].set_ylabel(self.modifier.param_label_full(parameter.upper()), fontsize=12)
+                        label=self.modifier.param_label_full(
+                            parameter.upper()))
+            axs[j].set_ylabel(self.modifier.param_label_full(
+                parameter.upper()), fontsize=12)
             axs[j].spines[pc.BOTTOM].set_linewidth(1.5)
             axs[j].spines[pc.LEFT].set_linewidth(1.5)
             axs[j].spines[pc.TOP].set_linewidth(0)
             axs[j].spines[pc.RIGHT].set_linewidth(0)
             if format_of_date.lower() == pc.YEAR:
                 axs[j].set_xlabel(pc.X_LABEL_TIME_YEAR, fontsize=12)
             elif format_of_date.lower() == pc.DAY:
@@ -174,41 +191,47 @@
                 axs[j].set_xlabel(pc.X_LABEL_TIME_MINUTE, fontsize=12)
             axs[j].ticklabel_format(useOffset=False)
             plt.setp(axs[j].get_xticklabels(), fontsize=12)
             plt.setp(axs[j].get_yticklabels(), fontsize=12)
             j = j + 1
         plt.tight_layout()
         plt.show()
-        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX,
+                    dpi=600)
 
-    def _raw_multi_plot_restart_vertical(self, param, gridblocknumber, format_of_date):
-        """ Line Plots of a multiple parameter in the results file as a function of time in vertical orientation with restart
+    def _raw_multi_plot_restart_vertical(self, param, gridblocknumber,
+                                         format_of_date):
+        """ Line Plots of a multiple parameter in the results file as a
+        function of time in vertical orientation with restart
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
-        
+
+
         Returns
         --------
-        
+
         """
         time_year = self.getRestartDataTime(format_of_date)
         fig = plt.figure()
         for number in range(1, len(param) + 1):
             ax = fig.add_subplot(1, len(param), number)
-            result_array = self.getRestartDataElement(param[number - 1], gridblocknumber)
+            result_array = self.getRestartDataElement(param[number - 1],
+                                                      gridblocknumber)
             ax.plot(time_year, result_array, marker=pc.CARET_SYMBOL,
-                    label=self.modifier.param_label_full(param[number - 1].upper()))
-            ax.set_ylabel(self.modifier.param_label_full(param[number - 1].upper()), fontsize=12)
+                    label=self.modifier.param_label_full(
+                        param[number - 1].upper()))
+            ax.set_ylabel(self.modifier.param_label_full(
+                param[number - 1].upper()), fontsize=12)
             ax.spines[pc.BOTTOM].set_linewidth(1.5)
             ax.spines[pc.LEFT].set_linewidth(1.5)
             ax.spines[pc.TOP].set_linewidth(0)
             ax.spines[pc.RIGHT].set_linewidth(0)
             ax.ticklabel_format(useOffset=False)
             plt.setp(ax.get_xticklabels(), fontsize=12)
             plt.setp(ax.get_yticklabels(), fontsize=12)
@@ -219,102 +242,120 @@
                 ax.set_xlabel(pc.X_LABEL_TIME_DAY, fontsize=12)
             elif format_of_date.lower() == pc.HOUR:
                 ax.set_xlabel(pc.X_LABEL_TIME_HOUR, fontsize=12)
             elif format_of_date.lower() == pc.MINUTE:
                 ax.set_xlabel(pc.X_LABEL_TIME_MINUTE, fontsize=12)
         plt.tight_layout()
         plt.show()
-        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX,
+                    dpi=600)
 
-    def multi_time_plot_restart(self, param, gridblocknumber, format_of_date, style=pc.HORIZONTAL):
-        """ Line Plots of a multiple parameter in the results file as a function of time for restart files
+    def multi_time_plot_restart(self, param, gridblocknumber, format_of_date,
+                                style=pc.HORIZONTAL):
+        """ Line Plots of a multiple parameter in the results file as a
+        function of time for restart files
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
-        
-        
+
+
+
         Returns
         --------
-        
+
         """
         if style.lower() == pc.HORIZONTAL:
             if self.expt:
                 if isinstance(param, list) and len(param) < 3:
                     try:
                         with plt.style.context(pc.MY_STYLE):
-                            self._raw_multi_plot_restart_horizontal_with_expt(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_restart_horizontal_with_expt(
+                                param, format_of_date, gridblocknumber)
                     except Exception:
                         with plt.style.context(pc.CLASSIC):
-                            self._raw_multi_plot_restart_horizontal_with_expt(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_restart_horizontal_with_expt(
+                                param, format_of_date, gridblocknumber)
                 else:
                     raise ParameterLessThanThreeError()
             else:
                 if isinstance(param, list) and len(param) < 3:
                     try:
                         with plt.style.context(pc.MY_STYLE):
-                            self._raw_multi_plot_horizontal(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_horizontal(param,
+                                                            format_of_date,
+                                                            gridblocknumber)
                     except Exception:
                         with plt.style.context(pc.CLASSIC):
-                            self._raw_multi_plot_horizontal(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_horizontal(param,
+                                                            format_of_date,
+                                                            gridblocknumber)
                 else:
                     raise ParameterLessThanThreeError()
         elif style.lower() == pc.VERTICAL:
             if self.expt:
                 if isinstance(param, list) and len(param) < 3:
                     try:
                         with plt.style.context(pc.MY_STYLE):
-                            self._raw_multi_plot_vertical_with_expt(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_vertical_with_expt(
+                                param, format_of_date, gridblocknumber)
                     except Exception:
                         with plt.style.context(pc.CLASSIC):
-                            self._raw_multi_plot_vertical_with_expt(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_vertical_with_expt(
+                                param, format_of_date, gridblocknumber)
                 else:
                     raise ParameterLessThanThreeError()
             else:
                 if isinstance(param, list) and len(param) < 3:
                     try:
                         with plt.style.context(pc.MY_STYLE):
-                            self._raw_multi_plot_vertical(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_vertical(
+                                param, format_of_date, gridblocknumber)
                     except Exception:
                         with plt.style.context(pc.CLASSIC):
-                            self._raw_multi_plot_vertical(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_vertical(
+                                param, format_of_date, gridblocknumber)
                 else:
                     raise ParameterLessThanThreeError()
 
-    def _raw_multi_plot_horizontal(self, param, format_of_date, gridblocknumber):
-        """ Line Plots of a multiple parameter in the results file as a function of time in horizontal orientation
+    def _raw_multi_plot_horizontal(self, param, format_of_date,
+                                   gridblocknumber):
+        """ Line Plots of a multiple parameter in the results file as a
+        function of time in horizontal orientation
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
+
         Returns
         --------
-        
+
         """
         fileReader = self.read_file()
         time_year = fileReader.convert_times(format_of_date)
         j = 0
         fig, axs = plt.subplots(len(param), sharex=False)
         for parameter in param:
-            result_array = fileReader.get_timeseries_data(parameter, gridblocknumber)
+            result_array = fileReader.get_timeseries_data(parameter,
+                                                          gridblocknumber)
             axs[j].plot(time_year, result_array, marker=pc.CARET_SYMBOL,
-                        label=self.modifier.param_label_full(parameter.upper()))
-            axs[j].set_ylabel(self.modifier.param_label_full(parameter.upper()), fontsize=12)
+                        label=self.modifier.param_label_full(
+                            parameter.upper()))
+            axs[j].set_ylabel(self.modifier.param_label_full(
+                parameter.upper()), fontsize=12)
             axs[j].spines[pc.BOTTOM].set_linewidth(1.5)
             axs[j].spines[pc.LEFT].set_linewidth(1.5)
             axs[j].spines[pc.TOP].set_linewidth(0)
             axs[j].spines[pc.RIGHT].set_linewidth(0)
             if format_of_date.lower() == pc.YEAR:
                 axs[j].set_xlabel(pc.X_LABEL_TIME_YEAR, fontsize=12)
             elif format_of_date.lower() == pc.DAY:
@@ -325,52 +366,61 @@
                 axs[j].set_xlabel(pc.X_LABEL_TIME_MINUTE, fontsize=12)
             axs[j].ticklabel_format(useOffset=False)
             plt.setp(axs[j].get_xticklabels(), fontsize=12)
             plt.setp(axs[j].get_yticklabels(), fontsize=12)
             j = j + 1
         plt.tight_layout()
         plt.show()
-        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX,
+                    dpi=600)
 
-    def _raw_multi_plot_horizontal_with_expt(self, param, format_of_date, gridblocknumber, data_file='data_file.csv'):
-        """ Line Plots of a multiple parameter in the results file as a function of time in horizontal orientation with experiment
+    def _raw_multi_plot_horizontal_with_expt(self, param,
+                                             format_of_date, gridblocknumber,
+                                             data_file='data_file.csv'):
+        """ Line Plots of a multiple parameter in the results file as a
+        function of time in horizontal orientation with experiment
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
         data_file: str
             The name of the data file containing the experimental data
-        
-        
-        
+
+
+
         Returns
         --------
-        
+
         """
         fileReader = self.read_file()
         time_year = fileReader.convert_times(format_of_date)
         expt_test = Experiment(self.expt[0], data_file)
         time_year_expt = expt_test.get_times()
         j = 0
         fig, axs = plt.subplots(len(param), sharex=False)
         for parameter in param:
-            result_array = fileReader.get_timeseries_data(parameter, gridblocknumber)
+            result_array = fileReader.get_timeseries_data(parameter,
+                                                          gridblocknumber)
             result_array_expt = expt_test.get_timeseries_data(parameter)
-            axs[j].plot(time_year, result_array, marker=pc.CARET_SYMBOL, label=gc.SIMULATION)
+            axs[j].plot(time_year, result_array, marker=pc.CARET_SYMBOL,
+                        label=gc.SIMULATION)
             if max(result_array_expt) <= 0:
                 dy = 0.1 * abs(min(result_array_expt))
             else:
                 dy = 0.1 * abs(max(result_array_expt))
-            axs[j].errorbar(time_year_expt, result_array_expt, yerr=dy, fmt=pc.COLOR_FORMAT, color=pc.RED_SYMBOL, label=gc.EXPERIMENT)
-            axs[j].set_ylabel(self.modifier.param_label_full(parameter.upper()), fontsize=12)
+            axs[j].errorbar(time_year_expt, result_array_expt, yerr=dy,
+                            fmt=pc.COLOR_FORMAT, color=pc.RED_SYMBOL,
+                            label=gc.EXPERIMENT)
+            axs[j].set_ylabel(self.modifier.param_label_full(
+                parameter.upper()), fontsize=12)
             axs[j].spines[pc.BOTTOM].set_linewidth(1.5)
             axs[j].spines[pc.LEFT].set_linewidth(1.5)
             axs[j].spines[pc.TOP].set_linewidth(0)
             axs[j].spines[pc.RIGHT].set_linewidth(0)
             if format_of_date.lower() == pc.YEAR:
                 axs[j].set_xlabel(pc.X_LABEL_TIME_YEAR, fontsize=12)
             elif format_of_date.lower() == pc.DAY:
@@ -383,53 +433,65 @@
             axs[j].legend(loc=pc.LOC_BEST)
             plt.setp(axs[j].get_xticklabels(), fontsize=12)
             plt.setp(axs[j].get_yticklabels(), fontsize=12)
             j = j + 1
         plt.tight_layout()
         plt.show()
         os.chdir(self.filelocations)
-        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX,
+                    dpi=600)
 
-    def _raw_multi_plot_restart_horizontal_with_expt(self, param, format_of_date, gridblocknumber, data_file='data_file.csv'):
-        """ Line Plots of a multiple parameter in the results file as a function of time in horizontal orientation for restart files
+    def _raw_multi_plot_restart_horizontal_with_expt(self,
+                                                     param,
+                                                     format_of_date,
+                                                     gridblocknumber,
+                                                     data_file='data_file.csv'
+                                                     ):
+        """ Line Plots of a multiple parameter in the results file as a
+        function of time in horizontal orientation for restart files
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
         data_file: str
             The name of the data file containing the experimental data
-        
-        
-        
+
+
+
         Returns
         --------
-        
+
         """
         time_year = self.getRestartDataTime(format_of_date)
         j = 0
         fig, axs = plt.subplots(len(param), sharex=False)
         expt_test = Experiment(self.expt[0], data_file)
         time_year_expt = expt_test.get_times()
         for parameter in param:
-            result_array = self.getRestartDataElement(parameter, gridblocknumber)
+            result_array = self.getRestartDataElement(parameter,
+                                                      gridblocknumber)
             parameters = t2Utilities()
-            time_year, result_array = parameters.removeRepetiting(time_year, result_array)
+            time_year, result_array = parameters.remove_repetiting(time_year, result_array)
             result_array_expt = expt_test.get_timeseries_data(parameter)
-            axs[j].plot(time_year, result_array, marker=pc.CARET_SYMBOL, label=gc.SIMULATION)
+            axs[j].plot(time_year, result_array, marker=pc.CARET_SYMBOL,
+                        label=gc.SIMULATION)
             if max(result_array_expt) <= 0:
                 dy = 0.15 * abs(min(result_array_expt))
             else:
                 dy = 0.15 * abs(max(result_array_expt))
-            axs[j].errorbar(time_year_expt, result_array_expt, yerr=dy, fmt=pc.COLOR_FORMAT, color=pc.RED_SYMBOL, label=gc.EXPERIMENT)
-            axs[j].set_ylabel(self.modifier.param_label_full(parameter.upper()), fontsize=12)
+            axs[j].errorbar(time_year_expt, result_array_expt, yerr=dy,
+                            fmt=pc.COLOR_FORMAT, color=pc.RED_SYMBOL,
+                            label=gc.EXPERIMENT)
+            axs[j].set_ylabel(self.modifier.param_label_full(
+                parameter.upper()), fontsize=12)
             axs[j].spines[pc.BOTTOM].set_linewidth(1.5)
             axs[j].spines[pc.LEFT].set_linewidth(1.5)
             axs[j].spines[pc.TOP].set_linewidth(0)
             axs[j].spines[pc.RIGHT].set_linewidth(0)
             if format_of_date.lower() == pc.YEAR:
                 axs[j].set_xlabel(pc.X_LABEL_TIME_YEAR, fontsize=12)
             elif format_of_date.lower() == pc.DAY:
@@ -442,43 +504,48 @@
             plt.setp(axs[j].get_xticklabels(), fontsize=12)
             plt.setp(axs[j].get_yticklabels(), fontsize=12)
             axs[j].legend()
             j = j + 1
         plt.tight_layout()
         plt.show()
         os.chdir(self.filelocations)
-        fig.savefig(pc.MULTI_PLOT_EXPERIMENT_RESTART_LABEL, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(pc.MULTI_PLOT_EXPERIMENT_RESTART_LABEL,
+                    bbox_inches=pc.TIGHT_BBOX, dpi=600)
 
     def _raw_multi_plot_vertical(self, param, format_of_date, gridblocknumber):
-        """ Line Plots of a multiple parameter in the results file as a function of time in vertical orientation
+        """ Line Plots of a multiple parameter in the results file as a
+        function of time in vertical orientation
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
-        
+
+
         Returns
         --------
-        
+
         """
         fileReader = self.read_file()
         time_year = fileReader.convert_times(format_of_date)
         j = 0
         fig = plt.figure()
         for number in range(1, len(param) + 1):
             ax = fig.add_subplot(1, len(param), number)
-            result_array = fileReader.get_timeseries_data(param[number - 1], gridblocknumber)
+            result_array = fileReader.get_timeseries_data(param[number - 1],
+                                                          gridblocknumber)
             ax.plot(time_year, result_array, marker=pc.CARET_SYMBOL,
-                    label=self.modifier.param_label_full(param[number - 1].upper()))
-            ax.set_ylabel(self.modifier.param_label_full(param[number - 1].upper()), fontsize=12)
+                    label=self.modifier.param_label_full(
+                        param[number - 1].upper()))
+            ax.set_ylabel(self.modifier.param_label_full(
+                param[number - 1].upper()), fontsize=12)
             ax.spines[pc.BOTTOM].set_linewidth(1.5)
             ax.spines[pc.LEFT].set_linewidth(1.5)
             ax.spines[pc.TOP].set_linewidth(0)
             ax.spines[pc.RIGHT].set_linewidth(0)
             ax.ticklabel_format(useOffset=False)
             plt.setp(ax.get_xticklabels(), fontsize=12)
             plt.setp(ax.get_yticklabels(), fontsize=12)
@@ -489,49 +556,58 @@
             elif format_of_date.lower() == pc.HOUR:
                 ax.set_xlabel(pc.X_LABEL_TIME_HOUR, fontsize=12)
             elif format_of_date.lower() == pc.MIN:
                 ax.set_xlabel(pc.X_LABEL_TIME_MIN, fontsize=12)
             j = j + 1
         plt.tight_layout()
         plt.show()
-        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX,
+                    dpi=600)
 
-    def _raw_multi_plot_vertical_with_expt(self, param, format_of_date, grid_block_number, data_file='data_file.csv'):
-        """ Line Plots of a multiple parameter in the results file as a function of time in vertical orientation
+    def _raw_multi_plot_vertical_with_expt(self, param, format_of_date,
+                                           grid_block_number,
+                                           data_file='data_file.csv'):
+        """ Line Plots of a multiple parameter in the results file as a
+        function of time in vertical orientation
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
         data_file: str
             The name of the data file containing the experimental data
-        
-        
-        
+
+
+
         Returns
         --------
-        
+
         """
         fileReader = self.read_file()
         time_year = fileReader.convert_times(format_of_date)
         expt_test = Experiment(self.expt[0], data_file)
         time_year_expt = expt_test.get_times()
         j = 0
         fig = plt.figure()
         for number in range(1, len(param) + 1):
             ax = fig.add_subplot(1, len(param), number)
-            result_array_expt = expt_test.get_timeseries_data(param[number - 1])
-            result_array = fileReader.get_timeseries_data(param[number - 1], grid_block_number)
-            ax.plot(time_year, result_array, marker=pc.CARET, label=gc.SIMULATION)
-            ax.plot(time_year_expt, result_array_expt, '--', marker='o', color=pc.RED_COLOR, label=gc.EXPERIMENT)
-            ax.set_ylabel(self.modifier.param_label_full(param[number - 1].upper()), fontsize=12)
+            result_array_expt = expt_test.get_timeseries_data(
+                param[number - 1])
+            result_array = fileReader.get_timeseries_data(param[number - 1],
+                                                          grid_block_number)
+            ax.plot(time_year, result_array, marker=pc.CARET,
+                    label=gc.SIMULATION)
+            ax.plot(time_year_expt, result_array_expt, '--', marker='o',
+                    color=pc.RED_COLOR, label=gc.EXPERIMENT)
+            ax.set_ylabel(self.modifier.param_label_full(
+                param[number - 1].upper()), fontsize=12)
             ax.spines[pc.BOTTOM].set_linewidth(1.5)
             ax.spines[pc.LEFT].set_linewidth(1.5)
             ax.spines[pc.TOP].set_linewidth(0)
             ax.spines[pc.RIGHT].set_linewidth(0)
             ax.ticklabel_format(useOffset=False)
             plt.setp(ax.get_xticklabels(), fontsize=12)
             plt.setp(ax.get_yticklabels(), fontsize=12)
@@ -543,113 +619,126 @@
             elif format_of_date.lower() == pc.HOUR:
                 ax.set_xlabel(pc.X_LABEL_TIME_HOUR, fontsize=12)
             elif format_of_date.lower() == pc.MIN:
                 ax.set_xlabel(pc.X_LABEL_TIME_MIN, fontsize=12)
             j = j + 1
         plt.tight_layout()
         plt.show()
-        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(pc.MULTI_PLOT_DESCRIPTION_LABEL, bbox_inches=pc.TIGHT_BBOX,
+                    dpi=600)
 
-    def multi_time_plot(self, param, gridblocknumber, format_of_date, style=pc.HORIZONTAL):
-        """ Line Plots of a multiple parameter in the results file as a function of time
+    def multi_time_plot(self, param, gridblocknumber, format_of_date,
+                        style=pc.HORIZONTAL):
+        """ Line Plots of a multiple parameter in the results file as a
+        function of time
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or yeart
-        
-        
+
+
         Returns
         --------
-        
+
         """
         if style.lower() == pc.HORIZONTAL:
             if self.expt:
                 if isinstance(param, list) and len(param) < 3:
                     try:
                         with plt.style.context(pc.MY_STYLE):
-                            self._raw_multi_plot_horizontal_with_expt(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_horizontal_with_expt(
+                                param, format_of_date, gridblocknumber)
                     except Exception:
                         with plt.style.context(pc.CLASSIC):
-                            self._raw_multi_plot_horizontal_with_expt(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_horizontal_with_expt(
+                                param, format_of_date, gridblocknumber)
                 else:
                     raise ParameterLessThanThreeError()
             else:
                 if isinstance(param, list) and len(param) < 3:
                     try:
                         with plt.style.context(pc.MY_STYLE):
-                            self._raw_multi_plot_horizontal(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_horizontal(
+                                param, format_of_date, gridblocknumber)
                     except Exception:
                         with plt.style.context(pc.CLASSIC):
-                            self._raw_multi_plot_horizontal(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_horizontal(
+                                param, format_of_date, gridblocknumber)
                 else:
                     raise ParameterLessThanThreeError()
         elif style.lower() == pc.VERTICAL:
             if self.expt:
                 if isinstance(param, list) and len(param) < 3:
                     try:
                         with plt.style.context(pc.MY_STYLE):
-                            self._raw_multi_plot_vertical_with_expt(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_vertical_with_expt(
+                                param, format_of_date, gridblocknumber)
                     except Exception:
                         with plt.style.context(pc.CLASSIC):
-                            self._raw_multi_plot_vertical_with_expt(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_vertical_with_expt(
+                                param, format_of_date, gridblocknumber)
                 else:
                     raise ParameterLessThanThreeError()
             else:
                 if isinstance(param, list) and len(param) < 3:
                     try:
                         with plt.style.context(pc.MY_STYLE):
-                            self._raw_multi_plot_vertical(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_vertical(
+                                param, format_of_date, gridblocknumber)
                     except Exception:
                         with plt.style.context(pc.CLASSIC):
-                            self._raw_multi_plot_vertical(param, format_of_date, gridblocknumber)
+                            self._raw_multi_plot_vertical(
+                                param, format_of_date, gridblocknumber)
                 else:
                     raise ParameterLessThanThreeError()
 
     def _retrieve_multi_data(self, param, gridblocknumber):
         dataStorage = {}
         fileNames = []
         for parameter in param:
             fileNumber = 0
             for file in self.filelocations:
-                fileReader = self.read_file_multi(file, self.filetitles[fileNumber])
+                fileReader = self.read_file_multi(
+                    file, self.filetitles[fileNumber])
                 filename = parameter + str(fileNumber)
-                dataStorage[filename] = fileReader.get_timeseries_data(parameter, gridblocknumber)
+                dataStorage[filename] = fileReader.get_timeseries_data(
+                    parameter, gridblocknumber)
                 fileNames.append(filename)
                 fileNumber = fileNumber + 1
         return fileNames, dataStorage
 
     def _retrieve_multi_data_generation(self, param, format_of_date):
         """ Retrieve multi data for plotting
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
-        
+
+
         Returns
         --------
         data_table: pd.Dataframe
             returns the data in dataframe
-        
+
         """
         data_table = pd.DataFrame()
         fileReader = self.read_file()
         for i in range(len(param)):
             time_data_label = pc.TIME + str(i)
             result_data_label = pc.RESULT + str(i)
             time_data = fileReader.convert_times(format_of_date=format_of_date)
-            result_data = fileReader.getGenerationData(param[i])
+            result_data = fileReader.get_generation_data(param[i])
             data_table[time_data_label] = pd.Series(time_data)
             data_table[result_data_label] = pd.Series(result_data)
         return data_table
 
     def _slice_value(self, time, result):
         last_time = time[-1]
         last_result = result[-1]
@@ -659,78 +748,98 @@
         result_array = result_array[0:len(result_array) + 8:10]
         if len(time_array) > 10:
             return self._slice_value(time_array, result_array)
         time_array = np.append(time_array, last_time)
         result_array = np.append(result_array, last_result)
         return time_array, result_array
 
-    def plotMultiParamSinglePlot(self, param, gridblocknumber, format_of_date, labels=None):
+    def plotMultiParamSinglePlot(self, param, gridblocknumber, format_of_date,
+                                 labels=None):
         """ Line Multiple parameters in a single Plot
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
         labels: list[str]
             labels of the different plots in the chart
         Returns
         --------
-        
+
         """
         if self.generation is True:
             with plt.style.context(pc.CLASSIC):
                 fig, axs = plt.subplots(1, 1)
-                dataFile = self._retrieve_multi_data_generation(param, format_of_date)
+                dataFile = self._retrieve_multi_data_generation(param,
+                                                                format_of_date)
                 legend_index = 0
                 for i in range(0, len(dataFile.columns), 2):
                     if labels is None:
-                        axs.plot(dataFile.iloc[:, i], dataFile.iloc[:, i + 1], label=param[legend_index])
+                        axs.plot(dataFile.iloc[:, i], dataFile.iloc[:, i + 1],
+                                 label=param[legend_index])
                     else:
-                        axs.plot(dataFile.iloc[:, i], dataFile.iloc[:, i + 1], label=labels[legend_index])
-                    axs.set_xlabel(pc.TIME_CAPS + ' ' + pc.OPEN_BRACKET + format_of_date + pc.CLOSE_BRACKET, fontsize=14)
+                        axs.plot(dataFile.iloc[:, i], dataFile.iloc[:, i + 1],
+                                 label=labels[legend_index])
+                    axs.set_xlabel(pc.TIME_CAPS + ' ' + pc.OPEN_BRACKET +
+                                   format_of_date + pc.CLOSE_BRACKET,
+                                   fontsize=14)
                     axs.set_ylabel(pc.Mass_Fraction, fontsize=14)
                     legend_index += 1
                 plt.setp(axs.get_xticklabels(), fontsize=14)
                 plt.setp(axs.get_yticklabels(), fontsize=14)
                 plt.legend()
                 plt.tight_layout()
                 plt.show()
-                fig.savefig(pc.MULTIPLE_PARAM + ' ' + pc.VERSUS + ' ' + pc.TIME + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+                fig.savefig(pc.MULTIPLE_PARAM + ' ' + pc.VERSUS + ' ' +
+                            pc.TIME + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX,
+                            dpi=600)
         else:
             with plt.style.context(pc.CLASSIC):
                 fig, axs = plt.subplots(1, 1)
                 markers = pc.ALL_MARKERS
                 fileReader = self.read_file()
                 for i in range(0, len(param)):
                     time_year = fileReader.convert_times(format_of_date)
-                    result_array = fileReader.get_timeseries_data(param[i], gridblocknumber)
+                    result_array = fileReader.get_timeseries_data(
+                        param[i], gridblocknumber)
                     if len(time_year) > 50:
-                        time_year, result_array = self._slice_value(time_year, result_array)
+                        time_year, result_array = self._slice_value(
+                            time_year, result_array)
                     if labels is None:
-                        axs.plot(time_year, result_array, label=param[i], marker=markers[i])
+                        axs.plot(time_year, result_array, label=param[i],
+                                 marker=markers[i])
                     else:
-                        axs.plot(time_year, result_array, label=labels[i], marker=markers[i])
-                    axs.set_xlabel(pc.TIME_CAPS + ' ' + pc.OPEN_BRACKET + format_of_date + pc.CLOSE_BRACKET, fontsize=14)
+                        axs.plot(time_year, result_array, label=labels[i],
+                                 marker=markers[i])
+                    axs.set_xlabel(pc.TIME_CAPS + ' ' + pc.OPEN_BRACKET
+                                   + format_of_date + pc.CLOSE_BRACKET,
+                                   fontsize=14)
                     axs.set_ylabel(pc.MASS_FRACTION, fontsize=14)
-                    axs.ticklabel_format(useOffset=False, style=pc.PLAIN_STYLE, axis=pc.BOTH)
+                    axs.ticklabel_format(useOffset=False,
+                                         style=pc.PLAIN_STYLE, axis=pc.BOTH)
                 plt.setp(axs.get_xticklabels(), fontsize=14)
                 plt.setp(axs.get_yticklabels(), fontsize=14)
                 plt.legend(loc=pc.LOC_BEST)
                 plt.tight_layout()
                 plt.show()
                 plt.tick_params(axis=pc.X, which=pc.MAJOR, labelsize=3)
-                fig.savefig(param[0] + pc.MULTIPLE_PARAM_OUTPUT + ' ' + pc.VERSUS + ' ' + pc.TIME + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
-
-    def multi_param_multi_file_plot(self, param, gridblocknumber, labels, format_of_date=pc.YEAR, style=pc.HORIZONTAL,
+                fig.savefig(param[0] + pc.MULTIPLE_PARAM_OUTPUT
+                            + ' ' + pc.VERSUS + ' ' + pc.TIME + pc.IMAGE_TYPE,
+                            bbox_inches=pc.TIGHT_BBOX, dpi=600)
+
+    def multi_param_multi_file_plot(self, param, gridblocknumber, labels,
+                                    format_of_date=pc.YEAR,
+                                    style=pc.HORIZONTAL,
                                     width=12, height=8):
-        """ Line Plots of a multiple parameter in the results file as a function of time 
+        """ Line Plots of a multiple parameter in the results file as a
+        function of time
 
         Parameters
         -----------
         param :  list[str]
             The parameters to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
@@ -740,39 +849,44 @@
             Labels for the plots
         style : str
             orientation for multiple plots; could be horizontal or vertical
         width : int
             width of plot
         height : int
             height of plot
-        
-        
+
+
         Returns
         --------
-        
+
         """
         fig = plt.figure(figsize=(width, height))
-        fileReader = self.read_file_multi(self.filelocations[0], self.filetitles[0])
+        fileReader = self.read_file_multi(self.filelocations[0],
+                                          self.filetitles[0])
         time_year = fileReader.convert_times(format_of_date)
         lst, dictionary = self._retrieve_multi_data(param, gridblocknumber)
         colors = pc.ALL_COLORS
         markers = pc.ALL_MARKERS
         counter_2 = 0
         param_counter = 0
         subplot_i = 2
         k = 0
         subplot_j = 2
         fig, axs = plt.subplots(subplot_i, subplot_j)
         for number in range(subplot_i):
             for i in range(subplot_j):
                 for j in range(len(self.filelocations)):
-                    axs[number, i].plot(time_year, dictionary[lst[counter_2 + j]], label=labels[k], linewidth=2,
+                    axs[number, i].plot(time_year,
+                                        dictionary[lst[counter_2 + j]],
+                                        label=labels[k], linewidth=2,
                                         color=colors[j], marker=markers[j])
-                    axs[number, i].set_ylabel(self.modifier.strip_param(param[param_counter]))
-                    axs[number, i].set_title(self.modifier.param_label_full(param[param_counter].upper()))
+                    axs[number, i].set_ylabel(self.modifier.convert_parameter_name(
+                        param[param_counter]))
+                    axs[number, i].set_title(self.modifier.param_label_full(
+                        [param_counter].upper()))
                     axs[number, i].set_xlabel(pc.X_LABEL_TIME_YEAR)
                     axs[number, i].spines[pc.BOTTOM].set_linewidth(1.5)
                     axs[number, i].spines[pc.LEFT].set_linewidth(1.5)
                     axs[number, i].spines[pc.TOP].set_linewidth(0.0)
                     axs[number, i].spines[pc.RIGHT].set_linewidth(0.0)
                 counter_2 = counter_2 + len(self.filelocations)
                 param_counter = param_counter + 1
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/plotting/plot_single.py` & `pytoughreact-1.0.4/src/pytoughreact/plotting/plot_single.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,28 +41,29 @@
         self.simulatortype = simulatortype
         self.generation = kwargs.get(gc.GENERATION)
         self.full_args = kwargs.get(gc.RESTART_FILES)
         self.expt = kwargs.get(gc.EXPERIMENT)
         self.x_slice_value = kwargs.get(gc.X_SLICE_VALUE)
 
     def __repr__(self):
-        return 'Results from ' + self.filelocation + ' in ' + self.filetitle + ' for ' + self.simulatortype
+        return 'Results from ' + self.filelocation + ' in ' + self.filetitle \
+            + ' for ' + self.simulatortype
 
     def _validateFile(self):
         """ Validate File """
         if type(self.filelocation) != type(self.filetitle):
             print('Values can either be strings or lists')
 
     def _getSimulatorType(self):
         """ Get Simulator Type """
         return self.simulatortype
 
-    def plotTime(self, param, grid_block_number, format_of_date='year', labels=None, singlePlot=False, style='horizontal',
-                 width=12,
-                 height=8):
+    def plotTime(self, param, grid_block_number, format_of_date='year',
+                 labels=None, singlePlot=False, style='horizontal',
+                 width=12, height=8):
         """ General function for making line plot of parameter with time
 
         Parameters
         -----------
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         param :  str
@@ -76,106 +77,127 @@
         style : str
             orientation for multiple plots; could be horizontal or vertical
         width : int
             width of plot
         height : int
             height of plot
 
-        
+
         Returns
         --------
-        
+
         """
         if isinstance(param, str):
-            plottest = PlotTough(self.simulatortype, self.filelocation, self.filetitle, generation=self.generation,
+            plottest = PlotTough(self.simulatortype, self.filelocation,
+                                 self.filetitle, generation=self.generation,
                                  restart_files=self.full_args,
                                  experiment=self.expt)
             if self.full_args is None:
-                plottest.plotParamWithTime(param, grid_block_number, format_of_date)
+                plottest.plotParamWithTime(param, grid_block_number,
+                                           format_of_date)
             else:
-                plottest.plotParamWithTimeRestart(param, grid_block_number, format_of_date)
-        elif isinstance(param, list) and isinstance(self.filelocation, str) and singlePlot is False:
-            plottest = PlotMultiTough(self.simulatortype, self.filelocation, self.filetitle, generation=self.generation,
+                plottest.plotParamWithTimeRestart(param, grid_block_number,
+                                                  format_of_date)
+        elif (isinstance(param, list) and isinstance(self.filelocation, str)
+              and singlePlot is False):
+            plottest = PlotMultiTough(self.simulatortype, self.filelocation,
+                                      self.filetitle,
+                                      generation=self.generation,
                                       restart_files=self.full_args,
                                       experiment=self.expt)
             if self.full_args is None:
-                plottest.multi_time_plot(param, grid_block_number, format_of_date, style)
+                plottest.multi_time_plot(param, grid_block_number,
+                                         format_of_date, style)
             else:
-                plottest.multi_time_plot_restart(param, grid_block_number, format_of_date, style)
-        elif isinstance(param, list) and isinstance(self.filelocation, str) and singlePlot is True:
-            plottest = PlotMultiTough(self.simulatortype, self.filelocation, self.filetitle, generation=self.generation,
+                plottest.multi_time_plot_restart(param, grid_block_number,
+                                                 format_of_date, style)
+        elif (isinstance(param, list) and isinstance(self.filelocation, str)
+              and singlePlot is True):
+            plottest = PlotMultiTough(self.simulatortype, self.filelocation,
+                                      self.filetitle,
+                                      generation=self.generation,
                                       restart_files=self.full_args,
                                       experiment=self.expt,
                                       x_slice_value=self.x_slice_value)
             if self.full_args is None:
-                plottest.plotMultiParamSinglePlot(param, grid_block_number, format_of_date, labels)
+                plottest.plotMultiParamSinglePlot(param, grid_block_number,
+                                                  format_of_date, labels)
 
     def plotParamWithParam(self, param1, param2, gridblocknumber):
         """ Line Plot of two parameters in the results file
 
         Parameters
         -----------
         param1 :  str
             The parameter to be plotted on the x-axis
         param2 :  str
             The parameter to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
-        
+
         Returns
         --------
-        
+
         """
         """ Make Plot of parameter with parameter """
-        plottest = PlotTough(self.simulatortype, self.filelocation, self.filetitle)
+        plottest = PlotTough(self.simulatortype, self.filelocation,
+                             self.filetitle)
         plottest.plotParamWithParam(param1, param2, gridblocknumber)
 
-    def plotParamWithLayer(self, direction_x, direction_y, param, layer_num, time):
-        """ Make line plot of parameter at a particular time at a particular layer
+    def plotParamWithLayer(self, direction_x, direction_y, param, layer_num,
+                           time):
+        """ Make line plot of parameter at a particular time at a particular
+        layer
 
         Parameters
         -----------
         direction_x :  str
-            The direction to be plotted on the x axis 
+            The direction to be plotted on the x axis
         direction_y :  str
             The direction to be plotted on the y axis
         param :  str
             parameter to be plotted
         layer_num :  int
             layer number to be plotted
         time : int
             the time at which the plot is to be made
-        
+
         Returns
         --------
-        
-        """
-        plottest = PlotTough(self.simulatortype, self.filelocation, self.filetitle)
-        plottest.plotParamWithLayer(direction_x, direction_y, param, layer_num, time)
 
-    def plot2D(self, direction_x, direction_y, param, timer, grid_type='plain'):
-        """ Make 2D plot of parameter at a particular time across the whole domain
+        """
+        plottest = PlotTough(self.simulatortype, self.filelocation,
+                             self.filetitle)
+        plottest.plotParamWithLayer(direction_x, direction_y, param, layer_num,
+                                    time)
+
+    def plot2D(self, direction_x, direction_y, param, timer,
+               grid_type='plain'):
+        """ Make 2D plot of parameter at a particular time across the whole
+        domain
 
         Parameters
         -----------
         direction_x :  str
-            The direction to be plotted on the x axis 
+            The direction to be plotted on the x axis
         direction_y :  str
             The direction to be plotted on the y axis
         param :  str
             parameter to be plotted
         grid_type :  str
-            Specifies if plot should be gridded or not (options are 'plain' or 'grid')
+            Specifies if plot should be gridded or not (options are 'plain' or
+            'grid')
         timer : int
             the time at which the plot is to be made
-        
+
         Returns
         --------
-        
+
         """
-        plottest = PlotTough(self.simulatortype, self.filelocation, self.filetitle)
+        plottest = PlotTough(self.simulatortype, self.filelocation,
+                             self.filetitle)
         if grid_type == 'plain':
             plottest.plot2D_one(direction_x, direction_y, param, timer)
         elif grid_type == 'grid':
             plottest.plot2D_withgrid(direction_x, direction_y, param, timer)
         else:
             print('Type can either be plain or grid')
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/plotting/plot_tough_routine.py` & `pytoughreact-1.0.4/src/pytoughreact/plotting/plot_tough_routine.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 
         generation : str
             generation file location
         restart_files : str
             restart file location
         experiment : str
             experimental file location
-        
-        
+
+
         Returns
         --------
 
         """
         self.file_location = file_location
         os.chdir(self.file_location)
         self.filetitle = file_title
@@ -75,54 +75,60 @@
         self.modifier = t2Utilities()
         self.generation = kwargs.get(gc.GENERATION)
         self.args = kwargs.get(gc.RESTART_FILES)
         self.expt = kwargs.get(gc.EXPERIMENT)
 
     def _read_file(self):
         """ Read in the input files
-        
+
         """
-        if self.simulatortype.lower() == gc.TMVOC or self.simulatortype.lower() == gc.TOUGH3:
-            fileReader = ResultTough3(self.simulatortype, self.file_location, self.filetitle,
+        if (self.simulatortype.lower() == gc.TMVOC or
+                self.simulatortype.lower() == gc.TOUGH3):
+            fileReader = ResultTough3(self.simulatortype, self.file_location,
+                                      self.filetitle,
                                       generation=self.generation)
         else:
-            fileReader = ResultReact(self.simulatortype, self.file_location, self.filetitle)
+            fileReader = ResultReact(self.simulatortype, self.file_location,
+                                     self.filetitle)
         return fileReader
 
-    def _plotRaw(self, param, grid_block_number, format_of_date, restart=False):
+    def _plotRaw(self, param, grid_block_number,
+                 format_of_date, restart=False):
         """ Line Plots of a parameter in the results file as a function of time
 
         Parameters
         -----------
         param :  str
             The parameter to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
         restart: boolean
             If restart was performed in the simulation or not
-        
-        
+
+
         Returns
         --------
-        
+
         """
         parameters = t2Utilities()
         if restart is True:
             time_year = self._getRestartDataTime(format_of_date)
-            result_array = self._getRestartDataElement(param, grid_block_number)
-            time_year, result_array = parameters.removeRepetiting(time_year, result_array)
+            result_array = self._getRestartDataElement(param,
+                                                       grid_block_number)
+            time_year, result_array = parameters.remove_repetiting(time_year, result_array)
         else:
             fileReader = self._read_file()
             time_year = fileReader.convert_times(format_of_date)
             if self.generation is True:
-                result_array = fileReader.getGenerationData(param)
+                result_array = fileReader.get_generation_data(param)
             else:
-                result_array = fileReader.get_timeseries_data(param, grid_block_number)
+                result_array = fileReader.get_timeseries_data(
+                    param, grid_block_number)
         fig, axs = plt.subplots(1, 1)
         axs.plot(time_year, result_array, marker=pc.CARET_SYMBOL)
         if format_of_date.lower() == pc.YEAR:
             axs.set_xlabel(pc.X_LABEL_TIME_YEAR, fontsize=12)
         elif format_of_date.lower() == pc.DAY:
             axs.set_xlabel(pc.X_LABEL_TIME_DAY, fontsize=12)
         elif format_of_date.lower() == pc.HOUR:
@@ -135,79 +141,87 @@
         axs.spines[pc.TOP].set_linewidth(0)
         axs.spines[pc.RIGHT].set_linewidth(0)
         plt.setp(axs.get_xticklabels(), fontsize=12)
         plt.setp(axs.get_yticklabels(), fontsize=12)
         plt.tight_layout()
         plt.show()
         if restart is True:
-            fig.savefig(param + ' ' + pc.VERSUS + ' ' + pc.TIME + ' ' + pc.RESTART + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+            fig.savefig(param + ' ' + pc.VERSUS + ' ' + pc.TIME + ' '
+                        + pc.RESTART + pc.IMAGE_TYPE,
+                        bbox_inches=pc.TIGHT_BBOX, dpi=600)
         else:
-            fig.savefig(param + ' ' + pc.VERSUS + ' ' + pc.TIME + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+            fig.savefig(param + ' ' + pc.VERSUS + ' ' + pc.TIME
+                        + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
 
     def plotParamWithTime(self, param, grid_block_number, format_of_date):
         """ Line Plots of a parameter in the results file as a function of time
 
         Parameters
         -----------
         param :  str
             The parameter to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
+
         Returns
         --------
-        
+
         """
         if self.expt:
             try:
                 with plt.style.context(pc.MY_STYLE):
-                    self._plotRawWithExpt(param, grid_block_number, format_of_date)
+                    self._plotRawWithExpt(param, grid_block_number,
+                                          format_of_date)
             except Exception:
                 with plt.style.context(pc.CLASSIC):
-                    self._plotRawWithExpt(param, grid_block_number, format_of_date)
+                    self._plotRawWithExpt(param, grid_block_number,
+                                          format_of_date)
         else:
             try:
                 with plt.style.context(pc.MY_STYLE):
                     self._plotRaw(param, grid_block_number, format_of_date)
             except Exception:
                 with plt.style.context(pc.CLASSIC):
                     self._plotRaw(param, grid_block_number, format_of_date)
 
     def _getRestartLocations(self):
         """ Get Restart Locations
-        
+
         """
         restart_files = list()
         restart_files.append(self.file_location)
         restart_files = restart_files + self.args
         return restart_files
 
     def _getRestartDataTime(self, format_of_date):
         """ Get Restart Time Data
 
         Parameters
         -----------
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
+
         Returns
         --------
         restart_time : list
             restart time data in a list
-        
+
         """
         locations = self._getRestartLocations()
         restart_time = []
         for i in range(0, len(locations)):
-            if self.simulatortype.lower() == gc.TMVOC or self.simulatortype.lower() == gc.TOUGH3:
-                fileReader = ResultTough3(self.simulatortype, locations[i], self.filetitle)
+            if (self.simulatortype.lower() == gc.TMVOC or
+                    self.simulatortype.lower() == gc.TOUGH3):
+                fileReader = ResultTough3(self.simulatortype, locations[i],
+                                          self.filetitle)
             else:
-                fileReader = ResultReact(self.simulatortype, locations[i], self.filetitle)
+                fileReader = ResultReact(self.simulatortype, locations[i],
+                                         self.filetitle)
             if i == 0:
                 time_year = fileReader.convert_times(format_of_date)
                 restart_time.append(time_year)
             else:
                 time_year = fileReader.convert_times(format_of_date)
                 time_year = time_year[1:]
                 restart_time.append(time_year)
@@ -219,77 +233,90 @@
 
         Parameters
         -----------
         param :  str
             The parameter to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
-        
+
         Returns
         --------
         restart_result : list
             restart data in a list
-        
+
         """
         locations = self._getRestartLocations()
         restart_result = []
         for i in range(0, len(locations)):
-            if self.simulatortype.lower() == gc.TMVOC or self.simulatortype.lower() == gc.TOUGH3:
-                fileReader = ResultTough3(self.simulatortype, locations[i], self.filetitle)
+            if (self.simulatortype.lower() == gc.TMVOC or
+                    self.simulatortype.lower() == gc.TOUGH3):
+                fileReader = ResultTough3(self.simulatortype, locations[i],
+                                          self.filetitle)
             else:
-                fileReader = ResultReact(self.simulatortype, locations[i], self.filetitle)
+                fileReader = ResultReact(self.simulatortype, locations[i],
+                                         self.filetitle)
             if i == 0:
-                result_array = fileReader.get_timeseries_data(param, grid_block_number)
+                result_array = fileReader.get_timeseries_data(
+                    param, grid_block_number)
                 restart_result.append(result_array)
             else:
-                result_array = fileReader.get_timeseries_data(param, grid_block_number)
+                result_array = fileReader.get_timeseries_data(
+                    param, grid_block_number)
                 result_array = result_array[1:]
                 restart_result.append(result_array)
         restart_result = list(itertools.chain.from_iterable(restart_result))
         return restart_result
 
-    def _plotRawWithExpt(self, param, grid_block_number, format_of_date, restart=False, data_file='data_file.csv'):
-        """ Line Plots of a parameter in the results file as a function of time if restart and experiments was performed in the simulation
+    def _plotRawWithExpt(self, param, grid_block_number, format_of_date,
+                         restart=False, data_file='data_file.csv'):
+        """ Line Plots of a parameter in the results file as a function of
+        time if restart and experiments was performed in the simulation
 
         Parameters
         -----------
         param :  str
             The parameter to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
         restart: boolean
             If restart was performed in the simulation or not
         data_file: str
             Data containing the experimental result in csv format
-        
+
         Returns
         --------
-        
+
         """
         expt_test = Experiment(self.expt[0], data_file)
         time_year_expt = expt_test.get_times()
         result_array_expt = expt_test.get_timeseries_data(param)
         parameters = t2Utilities()
         if restart is True:
             time_year = self._getRestartDataTime(format_of_date)
-            result_array = self._getRestartDataElement(param, grid_block_number)
-            time_year, result_array = parameters.removeRepetiting(time_year, result_array)
+            result_array = self._getRestartDataElement(
+                param, grid_block_number)
+            time_year, result_array = parameters.remove_repetiting(
+                time_year, result_array)
         else:
             fileReader = self._read_file()
             time_year = fileReader.convert_times(format_of_date)
-            result_array = fileReader.get_timeseries_data(param, grid_block_number)
+            result_array = fileReader.get_timeseries_data(
+                param, grid_block_number)
         fig, axs = plt.subplots(1, 1)
         if max(result_array_expt) <= 0:
             dy = 0.15 * abs(min(result_array_expt))
         else:
             dy = 0.15 * abs(max(result_array_expt))
-        axs.plot(time_year, result_array, marker=pc.CARET_SYMBOL, label=gc.SIMULATION)
-        axs.errorbar(time_year_expt, result_array_expt, yerr=dy, fmt=pc.COLOR_FORMAT, color=pc.RED_SYMBOL, label=gc.EXPERIMENT)
+        axs.plot(time_year, result_array,
+                 marker=pc.CARET_SYMBOL, label=gc.SIMULATION)
+        axs.errorbar(time_year_expt, result_array_expt,
+                     yerr=dy, fmt=pc.COLOR_FORMAT, color=pc.RED_SYMBOL,
+                     label=gc.EXPERIMENT)
         if format_of_date.lower() == pc.YEAR:
             axs.set_xlabel(pc.X_LABEL_TIME_YEAR, fontsize=12)
         elif format_of_date.lower() == pc.DAY:
             axs.set_xlabel(pc.X_LABEL_TIME_DAY, fontsize=12)
         elif format_of_date.lower() == pc.HOUR:
             axs.set_xlabel(pc.X_LABEL_TIME_HOUR, fontsize=12)
         elif format_of_date.lower() == pc.MINUTE:
@@ -302,93 +329,116 @@
         plt.legend(loc=pc.LOC_BEST)
         plt.setp(axs.get_xticklabels(), fontsize=12)
         plt.setp(axs.get_yticklabels(), fontsize=12)
         plt.tight_layout()
         plt.show()
         if restart is True:
             os.chdir(self.file_location)
-            fig.savefig(param + ' ' + pc.VERSUS + ' ' + pc.TIME + ' ' + pc.RESTART + ' ' + pc.EXPERIMENT + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+            fig.savefig(param + ' ' + pc.VERSUS + ' ' + pc.TIME + ' '
+                        + pc.RESTART + ' ' + pc.EXPERIMENT + pc.IMAGE_TYPE,
+                        bbox_inches=pc.TIGHT_BBOX, dpi=600)
         else:
             os.chdir(self.file_location)
-            fig.savefig(param + ' ' + pc.VERSUS + ' ' + pc.TIME + ' ' + pc.EXPERIMENT + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
-
-    def plotParamWithTimeRestart(self, param, grid_block_number, format_of_date):
-        """ Line Plots of a parameter in the results file as a function of time if restart was performed in the simulation
+            fig.savefig(param + ' ' + pc.VERSUS + ' '
+                        + pc.TIME + ' ' + pc.EXPERIMENT + pc.IMAGE_TYPE,
+                        bbox_inches=pc.TIGHT_BBOX, dpi=600)
+
+    def plotParamWithTimeRestart(self, param, grid_block_number,
+                                 format_of_date):
+        """ Line Plots of a parameter in the results file as a function of
+        time if restart was performed in the simulation
 
         Parameters
         -----------
         param :  str
             The parameter to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
         format_of_date: str
             The format of the date; could be minute, hour, day or year
-        
+
         Returns
         --------
-        
+
         """
         if self.expt:
             try:
                 with plt.style.context(pc.MY_STYLE):
-                    self._plotRawWithExpt(param, grid_block_number, format_of_date, restart=True)
+                    self._plotRawWithExpt(param, grid_block_number,
+                                          format_of_date, restart=True)
             except Exception:
                 with plt.style.context(pc.CLASSIC):
-                    self._plotRawWithExpt(param, grid_block_number, format_of_date, restart=True)
+                    self._plotRawWithExpt(param, grid_block_number,
+                                          format_of_date, restart=True)
         else:
             try:
                 with plt.style.context(pc.MY_STYLE):
-                    self._plotRaw(param, grid_block_number, format_of_date, restart=True)
+                    self._plotRaw(param, grid_block_number,
+                                  format_of_date, restart=True)
             except Exception:
                 with plt.style.context(pc.CLASSIC):
-                    self._plotRaw(param, grid_block_number, format_of_date, restart=True)
+                    self._plotRaw(param, grid_block_number,
+                                  format_of_date, restart=True)
 
-    def _plotRawLayer(self, direction_x_axis, direction_y_axis, param, layer_num, time):
-        """ Line Plots to show the evolution of a particular parameter across a layer at a particular time
+    def _plotRawLayer(self, direction_x_axis, direction_y_axis,
+                      param, layer_num, time):
+        """ Line Plots to show the evolution of a particular parameter across
+        a layer at a particular time
 
         Parameters
         -----------
         direction_x_axis :  str
-            The direction to be plotted on the x axis 
+            The direction to be plotted on the x axis
         direction_y_axis :  str
             The direction to be plotted on the y axis
         param :  list[str]
             List of parameters
         layer_num :  int
             The layer in the model to be plotted
         time : int
             the time at which the plot is to be made
-        
+
         Returns
         --------
-        
+
         """
         fileReader = self._read_file()
         if len(param) == 1:
-            y_data = fileReader.getLayerData(direction_y_axis, layer_num, time, param[0])
+            y_data = fileReader.get_layer_data(direction_y_axis, layer_num,
+                                               time, param[0])
             x_data = fileReader.get_unique_coord_data(direction_x_axis, time)
             fig, axs = plt.subplots(1, 1)
             axs.plot(x_data, y_data, marker=pc.CARET_SYMBOL)
-            axs.set_xlabel(pc.DISTANCE_MSG + ' ' + direction_x_axis + ' ' + pc.DIRECTION + ' ' + pc.OPEN_BRACKET + pc.METER + pc.CLOSE_BRACKET)
+            axs.set_xlabel(pc.DISTANCE_MSG + ' ' + direction_x_axis
+                           + ' ' + pc.DIRECTION + ' ' + pc.OPEN_BRACKET
+                           + pc.METER + pc.CLOSE_BRACKET)
             axs.set_ylabel(self.modifier.param_label_full(param[0].upper()))
             plt.tight_layout()
             plt.show()
             os.chdir(self.file_location)
-            fig.savefig(param[0] + ' ' + pc.LAYER_FOR_LAYER + ' ' + str(layer_num) + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+            fig.savefig(param[0] + ' ' + pc.LAYER_FOR_LAYER
+                        + ' ' + str(layer_num) + pc.IMAGE_TYPE,
+                        bbox_inches=pc.TIGHT_BBOX, dpi=600)
         else:
             fig = plt.figure(figsize=(10, 8))
             plot_counter = 1
             start_point = 0
             x_data = fileReader.get_unique_coord_data(direction_x_axis, time)
             for _ in range(1, len(param) + 1):
-                axs = plt.subplot(math.ceil(len(param) / 2) + 1, 2, plot_counter)
-                y_data = fileReader.getLayerData(direction_y_axis, layer_num, time, param[start_point])
+                axs = plt.subplot(math.ceil(len(param) / 2) + 1, 2,
+                                  plot_counter)
+                y_data = fileReader.get_layer_data(direction_y_axis,
+                                                   layer_num, time, param[start_point])
                 axs.plot(x_data, y_data)
-                axs.set_xlabel(pc.DISTANCE_MSG + ' ' + direction_x_axis + ' ' + pc.DIRECTION + ' ' + pc.OPEN_BRACKET + pc.METER + pc.CLOSE_BRACKET, fontsize=14)
-                axs.set_ylabel(self.modifier.param_label_full(param[start_point].upper()), fontsize=14)
+                axs.set_xlabel(pc.DISTANCE_MSG + ' '
+                               + direction_x_axis + ' ' + pc.DIRECTION
+                               + ' ' + pc.OPEN_BRACKET + pc.METER
+                               + pc.CLOSE_BRACKET, fontsize=14)
+                axs.set_ylabel(self.modifier.param_label_full(
+                    param[start_point].upper()), fontsize=14)
                 plot_counter = plot_counter + 1
                 start_point = start_point + 1
                 plt.setp(axs.get_xticklabels(), fontsize=14)
                 plt.setp(axs.get_yticklabels(), fontsize=14)
             fig.tight_layout()
             plt.show()
 
@@ -399,155 +449,180 @@
         -----------
         param1 :  str
             The parameter to be plotted on the x-axis
         param2 :  str
             The parameter to be plotted on the y-axis
         grid_block_number : int
             the grid block in which its parameter evolution is to be observed.
-        
+
         Returns
         --------
-        
+
         """
         try:
             with plt.style.context(pc.MY_STYLE):
                 fileReader = self._read_file()
-                result_array_x = fileReader.get_timeseries_data(param1, grid_block_number)
-                result_array_y = fileReader.get_timeseries_data(param2, grid_block_number)
+                result_array_x = fileReader.get_timeseries_data(
+                    param1, grid_block_number)
+                result_array_y = fileReader.get_timeseries_data(
+                    param2, grid_block_number)
                 fig, axs = plt.subplots(1, 1)
-                axs.plot(result_array_x, result_array_y, marker=pc.CARET_SYMBOL)
+                axs.plot(result_array_x, result_array_y,
+                         marker=pc.CARET_SYMBOL)
                 axs.set_xlabel(self.modifier.param_label_full(param1.upper()))
                 axs.set_ylabel(self.modifier.param_label_full(param2.upper()))
                 plt.tight_layout()
                 plt.show()
-                fig.savefig(param2 + ' ' + pc.VERSUS + ' ' + param1 + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+                fig.savefig(param2 + ' ' + pc.VERSUS + ' '
+                            + param1 + pc.IMAGE_TYPE,
+                            bbox_inches=pc.TIGHT_BBOX, dpi=600)
         except Exception:
             with plt.style.context(pc.CLASSIC):
                 fileReader = self._read_file()
-                result_array_x = fileReader.get_timeseries_data(param1, grid_block_number)
-                result_array_y = fileReader.get_timeseries_data(param2, grid_block_number)
+                result_array_x = fileReader.get_timeseries_data(
+                    param1, grid_block_number)
+                result_array_y = fileReader.get_timeseries_data(
+                    param2, grid_block_number)
                 fig, axs = plt.subplots(1, 1)
-                axs.plot(result_array_x, result_array_y, marker=pc.CARET_SYMBOL)
+                axs.plot(result_array_x, result_array_y,
+                         marker=pc.CARET_SYMBOL)
                 axs.set_xlabel(self.modifier.param_label_full(param1.upper()))
                 axs.set_ylabel(self.modifier.param_label_full(param2.upper()))
                 plt.tight_layout()
                 plt.show()
-                fig.savefig(param2 + ' ' + pc.VERSUS + ' ' + param1 + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
-
-
-    def plotParamWithLayer(self, direction_x_axis, direction_y_axis, param, layer_num, time):
-        """ Line Plots to show the evolution of a particular parameter across a layer at a particular time
+                fig.savefig(param2 + ' ' + pc.VERSUS + ' '
+                            + param1 + pc.IMAGE_TYPE,
+                            bbox_inches=pc.TIGHT_BBOX, dpi=600)
+
+    def plotParamWithLayer(self, direction_x_axis, direction_y_axis,
+                           param, layer_num, time):
+        """ Line Plots to show the evolution of a particular parameter across
+        a layer at a particular time
 
         Parameters
         -----------
         direction_x_axis :  str
-            The direction to be plotted on the x axis 
+            The direction to be plotted on the x axis
         direction_y_axis :  str
             The direction to be plotted on the y axis
         param :  list[str]
             List of parameters
         layer_num :  int
             The layer in the model to be plotted
         time : int
             the time at which the plot is to be made
-        
+
         Returns
         --------
-        
+
         """
         try:
             with plt.style.context(pc.MY_STYLE):
-                self._plotRawLayer(direction_x_axis, direction_y_axis, param, layer_num, time)
+                self._plotRawLayer(direction_x_axis, direction_y_axis,
+                                   param, layer_num, time)
         except Exception:
             with plt.style.context(pc.CLASSIC):
-                self._plotRawLayer(direction_x_axis, direction_y_axis, param, layer_num, time)
+                self._plotRawLayer(direction_x_axis, direction_y_axis,
+                                   param, layer_num, time)
 
     def plot2D_one(self, direction_y_axis, direction_x_axis, param, timer):
-        """ 2D mesh plot (ungridded) to show the evolution of a particular parameter across a the entire domain at a particular time
+        """ 2D mesh plot (ungridded) to show the evolution of a particular
+        parameter across a the entire domain at a particular time
 
         Parameters
         -----------
         direction_x_axis :  str
-            The direction to be plotted on the x axis 
+            The direction to be plotted on the x axis
         direction_y_axis :  str
             The direction to be plotted on the y axis
         param :  str
             parameter to be plotted
         time : int
             the time at which the plot is to be made
-        
+
         Returns
         --------
-        
+
         """
         fileReader = self._read_file()
         fig, ax = plt.subplots(1, 1)
         X = fileReader.get_coord_data(direction_y_axis, timer)
         Z = fileReader.get_coord_data(direction_x_axis, timer)
         data = fileReader.get_element_data(timer, param)
         xi, yi = np.meshgrid(X, Z)
         data1 = griddata((X, Z), data, (xi, yi), method=pc.METHOD)
-        cs2 = plt.contourf(xi, yi, data1, 800, cmap=pc.CMAP_COLOR, vmin=min(data), vmax=max(data))
+        cs2 = plt.contourf(xi, yi, data1, 800, cmap=pc.CMAP_COLOR,
+                           vmin=min(data), vmax=max(data))
         vmin = min(data)
         if vmin < 1 or vmin > 1000:
-            cbar = fig.colorbar(cs2, pad=0.01, format=ticker.FuncFormatter(self.modifier.fmt))
+            cbar = fig.colorbar(cs2, pad=0.01,
+                                format=ticker.FuncFormatter(self.modifier.fmt))
         else:
             cbar = fig.colorbar(cs2, pad=0.01)
-        cbar.ax.set_ylabel(self.modifier.param_label_full(param.upper()), fontsize=12)
+        cbar.ax.set_ylabel(self.modifier.param_label_full(param.upper()),
+                           fontsize=12)
         ticklabs = cbar.ax.get_yticklabels()
         try:
             cbar.ax.set_yticklabels(ticklabs, fontsize=12)
         except ValueError:
             pass
-        plt.xlabel(pc.HORIZONTAL_ADDED.capitalize() + ' ' + pc.DISTANCE.capitalize() + pc.OPEN_BRACKET + pc.METER + pc.CLOSE_BRACKET, fontsize=12)
-        plt.ylabel(pc.VERTICAL_ADDED.capitalize() + ' ' + pc.DEPTH.capitalize() + pc.OPEN_BRACKET + pc.METER + pc.CLOSE_BRACKET, fontsize=12)
+        plt.xlabel(pc.HORIZONTAL_ADDED.capitalize() + ' '
+                   + pc.DISTANCE.capitalize() + pc.OPEN_BRACKET + pc.METER
+                   + pc.CLOSE_BRACKET, fontsize=12)
+        plt.ylabel(pc.VERTICAL_ADDED.capitalize()
+                   + ' ' + pc.DEPTH.capitalize() + pc.OPEN_BRACKET + pc.METER
+                   + pc.CLOSE_BRACKET, fontsize=12)
         plt.tick_params(axis=pc.X, labelsize=12)
         plt.tick_params(axis=pc.Y, labelsize=12)
         plt.tight_layout()
         plt.show()
-        fig.savefig('2D plain' + str(timer) + param + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig('2D plain' + str(timer) + param + pc.IMAGE_TYPE,
+                    bbox_inches=pc.TIGHT_BBOX, dpi=600)
 
-    def plot2D_withgrid(self, direction_y_axis, direction_x_axis, param, timer):
-        """ 2D mesh plot (gridded) to show the evolution of a particular parameter across a the entire domain at a particular time
+    def plot2D_withgrid(self, direction_y_axis, direction_x_axis,
+                        param, timer):
+        """ 2D mesh plot (gridded) to show the evolution of a particular
+        parameter across a the entire domain at a particular time
 
         Parameters
         -----------
         direction_x_axis :  str
-            The direction to be plotted on the x axis 
+            The direction to be plotted on the x axis
         direction_y_axis :  str
             The direction to be plotted on the y axis
         param :  str
             parameter to be plotted
         time : int
             the time at which the plot is to be made
-        
+
         Returns
         --------
-        
+
         """
         fileReader = self._read_file()
         X = fileReader.get_coord_data(direction_y_axis, timer)
         Z = fileReader.get_coord_data(direction_x_axis, timer)
         df = pd.DataFrame(index=range(len(X)))
         df[pc.X_CAPS] = X
         df[pc.Z_CAPS] = Z
-        Zvalues, Ztotal = self.modifier.getgridnumber(df, pc.Z_CAPS)
-        Xvalues, Xtotal = self.modifier.getgridnumber(df, pc.X_CAPS)
+        Zvalues, Ztotal = self.modifier.get_grid_number(df, pc.Z_CAPS)
+        Xvalues, Xtotal = self.modifier.get_grid_number(df, pc.X_CAPS)
         xi, yi = np.meshgrid(X, Z)
         orig_data = fileReader.get_element_data(timer, param)
         data = np.asarray(orig_data)
         data = data.reshape(Ztotal, Xtotal)
         if Ztotal > 5:
             height = 10
         else:
             height = 4
         fig, ax = plt.subplots(1, 1, figsize=(10, height))
         # data1 = griddata((X, Z), orig_data, (xi, yi), method=pc.METHOD)
         # extent = [min(X), max(X), min(Z), max(Z)]
-        cs2 = plt.imshow(np.reshape(data, newshape=(Ztotal, Xtotal)), cmap=pc.CMAP_COLOR, interpolation=pc.INTERPOLATION,
+        cs2 = plt.imshow(np.reshape(data, newshape=(Ztotal, Xtotal)),
+                         cmap=pc.CMAP_COLOR, interpolation=pc.INTERPOLATION,
                          aspect=pc.ASPECT)
         ax = plt.gca()
         slicer_X = len(Xvalues)
         slicer_Z = len(Zvalues)
         if slicer_Z < 10:
             slicer_Z = 1
         if slicer_X <= 10:
@@ -569,29 +644,40 @@
         tick_x = max(X) - min(X)
         tick_z = max(Z) - min(Z)
         x_tick = x_tick.astype(int)
         if max(X) < 1 or max(Z) < 1:
             magoosh = [Xvalues[i] for i in x_tick]
             magoosh = np.asarray(magoosh)
             ax.set_xticklabels(magoosh, fontsize=12)
-            ax.set_yticklabels(np.round(self.modifier.crange(min(Z_array), max(Z_array), tick_z / (num_tick_z - 1)), 4),
+            ax.set_yticklabels(np.round(self.modifier.crange(min(Z_array),
+                                                             max(Z_array),
+                                                             tick_z / (
+                                                                 num_tick_z -
+                                                                 1)), 4),
                                fontsize=12)
         else:
-            ax.set_xticklabels(np.round(self.modifier.crange(min(X), max(X), tick_x / (num_tick_x - 1)), 2), fontsize=12)
-            ax.set_yticklabels(np.round(self.modifier.crange(min(Z_array), max(Z_array), tick_z / (num_tick_z - 1)), 2),
-                               fontsize=12)
+            ax.set_xticklabels(np.round(self.modifier.crange(
+                min(X), max(X), tick_x / (num_tick_x - 1)), 2), fontsize=12)
+            ax.set_yticklabels(np.round(self.modifier.crange(
+                min(Z_array), max(Z_array), tick_z / (num_tick_z - 1)), 2),
+                fontsize=12)
         # Minor ticks
         ax.set_xticks(np.arange(-.5, Xtotal, 1), minor=True)
         ax.set_yticks(np.arange(-.5, Ztotal, 1), minor=True)
         # Gridlines based on minor ticks
         ax.grid(which='minor', color='k', linestyle='-', linewidth=1)
         cbar = fig.colorbar(cs2, ax=ax, pad=0.3, orientation=pc.HORIZONTAL)
         cbar.ax.set_title(param, fontsize=12)
         cbar.ax.tick_params(labelsize=12)
         cbar.ax.locator_params(nbins=5)
         cbar.ax.ticklabel_format(useOffset=False, style=pc.PLAIN_STYLE)
         plt.xticks(rotation=90)
-        plt.xlabel(pc.HORIZONTAL_ADDED.capitalize() + ' ' + pc.DISTANCE.capitalize() + ' ' + pc.OPEN_BRACKET + pc.METER + pc.CLOSE_BRACKET, fontsize=12)
-        plt.ylabel(pc.VERTICAL_ADDED.capitalize() + ' ' + pc.DEPTH.capitalize() + ' ' + pc.OPEN_BRACKET + pc.METER + pc.CLOSE_BRACKET, fontsize=12)
+        plt.xlabel(pc.HORIZONTAL_ADDED.capitalize() + ' '
+                   + pc.DISTANCE.capitalize() + ' ' + pc.OPEN_BRACKET
+                   + pc.METER + pc.CLOSE_BRACKET, fontsize=12)
+        plt.ylabel(pc.VERTICAL_ADDED.capitalize() + ' '
+                   + pc.DEPTH.capitalize() + ' ' + pc.OPEN_BRACKET
+                   + pc.METER + pc.CLOSE_BRACKET, fontsize=12)
         plt.tight_layout()
         plt.show()
-        fig.savefig(grc.GRID_NAME.capitalize() + str(timer) + param + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
+        fig.savefig(grc.GRID_NAME.capitalize() + str(timer) + param
+                    + pc.IMAGE_TYPE, bbox_inches=pc.TIGHT_BBOX, dpi=600)
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/results/multi_result_tough_3.py` & `pytoughreact-1.0.4/src/pytoughreact/results/multi_result_tough_3.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,33 @@
 import pandas as pd
 from pytoughreact.results.result_tough_3 import ResultTough3
 
 
 class MultiResultTough3(object):
     """ Class for retrieving results from multiple files for Tough3 and TMVOC """
     def __init__(self, simulator_type, file_location, file_title, prop):
+        """Initialization of Parameters
+
+        Parameters
+        -----------
+        simulator_type :  list[string]
+            List of type of simulator being run. Can either be 'tmvoc', 'toughreact' or 'tough3'.
+            Should be tough3 for this class
+        file_location : list[string]
+            List of location of results file on system
+        file_title : list[string]
+            List of title or name of the file. Example is 'kddconc.tec'
+        prop : string
+            Prperty to be plotted. Example could be 'portlandite'
+
+
+        Returns
+        --------
+
+        """
         assert isinstance(file_location, list)
         assert isinstance(file_title, list)
         assert isinstance(prop, list)
         self.file_location = file_location
         self.file_title = file_title
         self.simulator_type = simulator_type
         self.prop = prop
@@ -66,62 +85,116 @@
             time_data_label = 'time' + str(i)
             result_data_label = 'result' + str(i)
             data_table[time_data_label] = pd.Series(time_data)
             data_table[result_data_label] = pd.Series(result_data)
         return data_table
 
     def retrieve_data_multi_file_fixed_time(self, direction, time):
-        """ DataFrame to retrieve time and coordinate results from file """
+        """ DataFrame to retrieve time and coordinate results from file
+
+        Parameters
+        -----------
+        direction :  string
+            Direction of retrieval. Can be 'X', 'Y' or 'Z'
+        time : float
+            Time in which the data should be retrieved.
+
+        Returns
+        --------
+        data_table : pd.Dataframe
+            Dataframe with requested output
+        """
         data_table = pd.DataFrame()
         for i in range(0, len(self.file_location)):
             tough_data = ResultTough3(self.simulator_type, self.file_location[i], self.file_title[i])
             os.chdir(self.file_location[i])
             x_data = tough_data.get_coord_data(direction, time)
             result_data = tough_data.get_element_data(time, self.prop[i])
             x_data_label = 'x' + str(i)
             result_data_label = 'result' + str(i)
             data_table[x_data_label] = pd.Series(x_data)
             data_table[result_data_label] = pd.Series(result_data)
-            print(tough_data.getXDepthData(1, self.prop[i], time))
+            print(tough_data.get_x_depth_data(1, self.prop[i], time))
         return data_table
 
     def retrieve_data_multi_file_fixed_time_layer(self, direction, time, layer_num):
-        """ DataFrame to retrieve distance and results from file """
+        """ DataFrame to retrieve distance and results from file
+
+        Parameters
+        -----------
+        direction :  string
+            Direction of retrieval. Can be 'X', 'Y' or 'Z'
+        time : float
+            Time in which the data should be retrieved.
+        layer_num: int
+            Layer number in which to retrieve data
+
+        Returns
+        --------
+        data_table : pd.Dataframe
+            Dataframe with requested output
+        """
         data_table = pd.DataFrame()
         for i in range(0, len(self.file_location)):
             tough_data = ResultTough3(self.simulator_type, self.file_location[i], self.file_title[i])
             os.chdir(self.file_location[i])
             x_data = tough_data.get_coord_data(direction, time)
-            result_data = tough_data.getLayerData(direction, layer_num, time, self.prop[i])
+            result_data = tough_data.get_layer_data(direction, layer_num, time, self.prop[i])
             x_data_label = 'x' + str(i)
             result_data_label = 'result' + str(i)
             data_table[x_data_label] = pd.Series(x_data)
             data_table[result_data_label] = pd.Series(result_data)
         return data_table
 
     def getMultiElementData(self, grid_block_number, format_of_date):
-        """ DataFrame to retrieve multi element time and results from file """
+        """ DataFrame to retrieve multi element time and results from file
+
+        Parameters
+        -----------
+        grid_block_number :  int
+            The grid block number for which to retrieve the results
+        format_of_date : str
+            Provides information to the method on format of the date. For example. year, hour, min or seconds
+
+        Returns
+        --------
+        data_table : pd.Dataframe
+            Dataframe with requested output
+        """
         data_table = pd.DataFrame()
         pd.set_option('float_format', lambda x: '%.9f' % x)
-        # pd.set_option('display.chop_threshold', 0.00000001)
         for i in range(0, len(self.file_location)):
             for j in range(0, len(self.prop)):
                 os.chdir(self.file_location[i])
                 tough_data = ResultTough3(self.simulator_type, self.file_location[i], self.file_title[i])
                 result_data = tough_data.get_timeseries_data(self.prop[j], grid_block_number)
                 time_data = tough_data.convert_times(format_of_date)
                 time_data_label = self.prop[j] + 'time' + str(i) + str(j)
                 result_data_label = self.prop[j] + 'result' + str(i) + str(j)
                 data_table[time_data_label] = pd.Series(time_data)
                 data_table[result_data_label] = pd.Series(result_data)
-        # print(data_table.iloc[15][result_data_label])
         return data_table
 
     def getMultiElementDataPerPanel(self, grid_block_number, panels, format_of_date):
-        """ DataFrame to retrieve multi element time and results from file per panel """
+        """ DataFrame to retrieve multi element time and results from file per panel
+
+        Parameters
+        -----------
+        grid_block_number :  int
+            The grid block number for which to retrieve the results
+        panels: list[string]
+            Data to be retrieved for each of the panel in the canvas
+        format_of_date : str
+            Provides information to the method on format of the date. For example. year, hour, min or seconds
+
+        Returns
+        --------
+        data_table : pd.Dataframe
+            Dataframe with requested output
+        """
         data_table = pd.DataFrame()
         pd.set_option('float_format', lambda x: '%.9f' % x)
         for i in range(0, len(panels)):
             properties = list(panels[i].values())[0][0]
             os.chdir(self.file_location[i])
             tough_data = ResultTough3(self.simulator_type, self.file_location[i], self.file_title[i])
             time_data = tough_data.convert_times(format_of_date)
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/results/result_multiple.py` & `pytoughreact-1.0.4/src/pytoughreact/results/result_multiple.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,64 +25,117 @@
 
 from pytoughreact.plotting.plot_multiple_files_routine import PlotMultiFiles
 
 
 class FileReadMultiple(object):
     """
     Class for processing multiple file results
-    file_locations (list of strings) - specifies the location of the files on the system
-    file_titles (list of strings) - gives the title of the file e.g 'kdd.conc' or 'OUTPUT.csv
-    simulator_type (string) can either be toughreact, tmvoc or tough3
-    props (list of strings) -  are the properties to be plotted
-
-    **kwargs
-    x_slice value (integer) - if the plot should be sliced a the  x axis
-    per_file -  (boolean) - if the plot should be made per file and not per property
-    title (list of strings) - title of each of the plots
     """
 
     def __init__(self, simulator_type, file_locations, file_titles, props, **kwargs):
+        """Initialization of Parameters
+
+        Parameters
+        -----------
+        simulator_type :  string
+            List of type of simulator being run. Can either be 'tmvoc', 'toughreact' or 'tough3'.
+            Should be tough3 for this class
+        file_location : list[string]
+            List of location of results file on system
+        file_title : list[string]
+            List of title or name of the file. Example is 'kddconc.tec' or 'OUTPUT.csv'
+        prop : list[string]
+            Properties to be plotted. Example could be 'portlandite'
+        kwargs: dict
+            1) x_slice_value (integer) - if the plot should be sliced on the  x axis
+            2) per_file  (boolean) - if the plot should be made per file and not per property
+            3) title (list of strings) - title of each of the plots
+
+
+        Returns
+        --------
+
+        """
         assert isinstance(file_locations, list)
         assert isinstance(file_titles, list)
         self.file_locations = file_locations
         self.file_titles = file_titles
         self.simulator_type = simulator_type
         self.props = props
         self.x_slice_value = kwargs.get('x_slice_value')
         self.per_file = kwargs.get('per_file')
         self.title = kwargs.get('title')
 
     def plotTime(self, grid_block_number, legend, plot_kind='property', format_of_date='day'):
         # TODO write code to slice x axis
         # TODO write code to slice through domain
 
-        """
+        """ Plot selected parameter on y axis and time on x axis
+
+        Parameters
+        -----------
+        grid_block_number : int
+            The grid block number in mesh for which to retrieve the results
+        legend : list[string]
+            List of titles for the legend of the plot
+        plot_kind : string
+            If the plot should be made based on property or based on files
+        format_of_date : str
+            Provides information to the method on format of the date. For example. year, hour, min or seconds
+
+        Returns
+        --------
 
-        :param format_of_date:
-        :param grid_block_number: grid block number in mesh
-        :type grid_block_number: int
-        :param legend:
-        :type legend: list
-        :param plot_kind:
-        :type plot_kind: string
         """
         plottest = PlotMultiFiles(self.simulator_type, self.file_locations, self.file_titles, self.props,
                                   x_slice_value=self.x_slice_value, per_file=self.per_file, title=self.title)
         if len(self.props) == 1:
             plottest.multiFileSinglePlot(grid_block_number, legend)
         else:
             plottest.plotMultiElementMultiFile(grid_block_number, legend, format_of_date, plot_kind)
 
     def plotTimePerPanel(self, grid_block_number, panels, format_of_date='day'):
-        """ Plot Multiple plots in a panel """
+        """ Plot Multiple plots in a panel
+
+        Parameters
+        -----------
+        grid_block_number : int
+            The grid block number in mesh for which to retrieve the results
+        panels: list[string]
+            Data to be retrieved for each of the panel in the canvas
+        format_of_date : str
+            Provides information to the method on format of the date. For example. year, hour, min or seconds
+
+        Returns
+        --------
+
+        """
         plottest = PlotMultiFiles(self.simulator_type, self.file_locations, self.file_titles, self.props,
                                   x_slice_value=self.x_slice_value, per_file=self.per_file, title=self.title)
         plottest.plotMultiPerPanel(grid_block_number, panels, format_of_date)
 
     def plotParamWithLayer(self, directionX, directionY, layer_num, time, legend):
-        """ Plot of Parameter with Layer """
+        """ Plot of Parameter with Layer
+
+        Parameters
+        -----------
+        directionX :  string
+            Direction to be plotted on the X axis. Can be 'X', 'Y', 'Z'
+        directionY :  string
+            Direction to be plotted on the Y axis. Can be 'X', 'Y', 'Z'
+        layer_num: int
+            Layer number in which to retrieve data
+        time : float
+            Time in which the data should be retrieved.
+        legend : list[string]
+            List of titles for the legend of the plot
+
+        Returns
+        --------
+
+        """
         plottest = PlotMultiFiles(self.simulator_type, self.file_locations, self.file_titles, self.props,
                                   x_slice_value=self.x_slice_value, per_file=self.per_file, title=self.title)
         if len(self.props) == 1:
             pass
         else:
             plottest.plotMultiFileDistance(directionX, directionY, time, layer_num, legend)
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/results/result_single.py` & `pytoughreact-1.0.4/src/pytoughreact/results/t2result.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,88 +18,121 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
+
 import os
-from pytoughreact.plotting.plot_tough_routine import PlotTough
-from pytoughreact.plotting.plot_multiple_tough_routine import PlotMultiTough
-import pytoughreact.constants.generalconstants as gc
 
+from pytoughreact.results.result_tough_3 import ResultTough3
+from pytoughreact.results.result_tough_react import ResultReact
+
+
+class t2result(object):
+    def __init__(self, simulatortype, filetitle, filelocation=None, **kwargs):
+        """Initialization of Parameters
+
+        Parameters
+        -----------
+        simulator_type :  string
+            Type of simulator being run. Can either be 'tmvoc', 'toughreact' or 'tough3'.
+            Should be tough3 for this class
+        file_location : string
+            Location of results file on system
+        file_title : string
+            Title or name of the file. Example is 'kddconc.tec' or 'OUTPUT.csv'
+        kwargs: dict
+            1) generation (string) - if generation data exists in the results.
+
+
+        Returns
+        --------
 
-class FileReadSingle(object):
-    def __init__(self, simulatortype, filelocation, filetitle, **kwargs):
-        """
-        Class for processing single file results
-        :type simulatortype: object
         """
-        self.filelocation = filelocation
-        if isinstance(self.filelocation, str):
-            os.chdir(self.filelocation)
+        if filelocation is None:
+            # self.filelocation = os.path.dirname(os.path.realpath(__file__))
+            self.filelocation = os.getcwd()
+        else:
+            self.filelocation = filelocation
+        os.chdir(self.filelocation)
         self.filetitle = filetitle
         self.simulatortype = simulatortype
-        self.generation = kwargs.get(gc.GENERATION)
-        self.full_args = kwargs.get(gc.RESTART_FILES)
-        self.expt = kwargs.get(gc.EXPERIMENT)
-        self.x_slice_value = kwargs.get(gc.X_SLICE_VALUE)
-
-    def __repr__(self):
-        return 'Results from ' + self.filelocation + ' in ' + self.filetitle + ' for ' + self.simulatortype
-
-    def validateFile(self):
-        """ Validate File """
-        if type(self.filelocation) != type(self.filetitle):
-            print('Values can either be strings or lists')
-
-    def getSimulatorType(self):
-        """ Get Simulator Type """
-        return self.simulatortype
-
-    def plotTime(self, param, gridblocknumber, format_of_date='year', labels=None, singlePlot=False, style='horizontal',
-                 width=12,
-                 height=8):
-        """ Make Plot of parameter with time """
-        if isinstance(param, str):
-            plottest = PlotTough(self.simulatortype, self.filelocation, self.filetitle, generation=self.generation,
-                                 restart_files=self.full_args,
-                                 experiment=self.expt)
-            if self.full_args is None:
-                plottest.plotParamWithTime(param, gridblocknumber, format_of_date)
-            else:
-                plottest.plotParamWithTimeRestart(param, gridblocknumber, format_of_date)
-        elif isinstance(param, list) and isinstance(self.filelocation, str) and singlePlot is False:
-            plottest = PlotMultiTough(self.simulatortype, self.filelocation, self.filetitle, generation=self.generation,
-                                      restart_files=self.full_args,
-                                      experiment=self.expt)
-            if self.full_args is None:
-                plottest.multi_time_plot(param, gridblocknumber, format_of_date, style)
-            else:
-                plottest.multi_time_plot_restart(param, gridblocknumber, format_of_date, style)
-        elif isinstance(param, list) and isinstance(self.filelocation, str) and singlePlot is True:
-            plottest = PlotMultiTough(self.simulatortype, self.filelocation, self.filetitle, generation=self.generation,
-                                      restart_files=self.full_args,
-                                      experiment=self.expt,
-                                      x_slice_value=self.x_slice_value)
-            if self.full_args is None:
-                plottest.plotMultiParamSinglePlot(param, gridblocknumber, format_of_date, labels)
-
-    def plotParamWithParam(self, param1, param2, gridblocknumber):
-        """ Make Plot of parameter with parameter """
-        plottest = PlotTough(self.simulatortype, self.filelocation, self.filetitle)
-        plottest.plotParamWithParam(param1, param2, gridblocknumber)
-
-    def plotParamWithLayer(self, directionXAxis, directionYAxis, param, layer_num, time):
-        """ Make Plot of parameter with layer """
-        plottest = PlotTough(self.simulatortype, self.filelocation, self.filetitle)
-        plottest.plotParamWithLayer(directionXAxis, directionYAxis, param, layer_num, time)
-
-    def plot2D(self, direction1, direction2, param, timer, grid_type='plain'):
-        """ Make 2D plot either gridded or not gridded """
-        plottest = PlotTough(self.simulatortype, self.filelocation, self.filetitle)
-        if grid_type == 'plain':
-            plottest.plot2D_one(direction1, direction2, param, timer)
-        elif grid_type == 'grid':
-            plottest.plot2D_withgrid(direction1, direction2, param, timer)
+        self.generation = kwargs.get('generation')
+        self.file_as_list = []
+
+    def read_file(self):
+        """ Read file specified in file_location and file_title
+
+        Parameters
+        -----------
+
+
+        Returns
+        --------
+        resulting_class : ResultTough3 , ResultReact
+            Resulting class for further processing
+
+        """
+        if self.simulatortype.lower() == "tmvoc" or self.simulatortype.lower() == "tough3":
+            resulting_class = ResultTough3(self.simulatortype, self.filelocation, self.filetitle,
+                                           generation=self.generation)
         else:
-            print('Type can either be plain or grid')
+            resulting_class = ResultReact(self.simulatortype, self.filelocation, self.filetitle)
+        return resulting_class
+
+    def get_times(self, format_of_date='year'):
+        """ Get times stored for duration of the simulation
+
+        Parameters
+        -----------
+        format_of_date : str
+            Provides information to the method on format of the date. For example. year, hour, min or seconds
+
+        Returns
+        --------
+        processed_time_data : list
+            Time data directly from file without processing.
+        """
+        fileReader = self.read_file()
+        processed_time_data = fileReader.convert_times(format_of_date)
+        return processed_time_data
+
+    def get_time_series_data(self, param, gridblocknumber):
+        """ Get Time series data
+
+        Parameters
+        -----------
+        grid_block_number :  int
+            The grid block number for which to retrieve the results
+        param: string
+            Parameter to be derived from data
+
+        Returns
+        --------
+        final_timeseries_data : list
+            Time series data for particular parameter.
+
+        """
+        fileReader = self.read_file()
+        final_timeseries_data = fileReader.get_timeseries_data(param, gridblocknumber)
+        return final_timeseries_data
+
+    def get_grid_data(self, timer, param):
+        """ Get Data for grids
+
+        Parameters
+        -----------
+        timer : float
+            Time in which the data should be retrieved.
+        param: string
+            Parameter to be derive data
+
+        Returns
+        --------
+        final_element_data : list
+            Data for each of the elements.
+        """
+        fileReader = self.read_file()
+        final_element_data = fileReader.get_element_data(timer, param)
+        return final_element_data
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/results/result_tough_3.py` & `pytoughreact-1.0.4/src/pytoughreact/results/result_tough_react.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,339 +20,467 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
 import os
-import numpy as np
-import csv
-import collections
-import itertools
 from pytoughreact.utilities.t2_utilities import t2Utilities
+from pytoughreact.utilities.t2_tough_react_utilities import t2UtilitiesToughReact
+import t2listing
 
 
-class ResultTough3(object):
-    """ Class for processing results from Tough3 """
-    def __init__(self, simulatortype, filelocation, filetitle=None, **kwargs):
-        if filelocation is None:
-            self.filelocation = os.getcwd()
-        else:
-            self.filelocation = filelocation
-            os.chdir(self.filelocation)
+class ResultReact(object):
+    """ Class for processing results from TOUGHREACT """
+    def __init__(self, simulatortype, filelocation, filetitle):
+        """Initialization of Parameters
+
+        Parameters
+        -----------
+        simulator_type :  string
+            Type of simulator being run. Can either be 'tmvoc', 'toughreact' or 'tough3'.
+            Should be tough3 for this class
+        file_location : string
+            Location of results file on system
+        file_title : string
+            Title or name of the file. Example is 'kddconc.tec' or 'OUTPUT.csv'
+
+
+        Returns
+        --------
+
+        """
+        self.filelocation = filelocation
+        os.chdir(self.filelocation)
         self.filetitle = filetitle
         self.simulatortype = simulatortype
-        self.generation = kwargs.get('generation')
-        self.file_as_list = []
+        self.data = t2listing.toughreact_tecplot(self.filetitle, self.get_elements())
 
     def __repr__(self):
         return 'Results from ' + self.filelocation + ' in ' + self.filetitle + ' for ' + self.simulatortype
 
-    def read_file(self):
-        """ Read file """
-        os.chdir(self.filelocation)
-        with open(self.filetitle) as csv_file:
-            csv_reader = csv.reader(csv_file, delimiter=',', quotechar='"')
-            self.file_as_list = []
-            for row in csv_reader:
-                self.file_as_list.append(row)
-        return self.file_as_list
+    def get_parameters(self):
+        """ Get Parameters from file
+
+        Parameters
+        -----------
+
+
+        Returns
+        --------
+        output : list
+            Parameters returned as list
 
-    def get_times(self):
         """
-        get times stored for duration of the simulation
-        :return: a list of all times
+        return self.data.element.column_name
+
+    def get_elements(self):
+        """ Get elements from the simulation
+
+        Parameters
+        -----------
+
+
+        Returns
+        --------
+        grid_blocks : list
+            Elements present in the result file.
+
         """
-        self.read_file()
-        time = []
-        timeraw = []
-        if self.generation is True:
-            for i in range(1, len(self.file_as_list)):
-                timeraw.append(float(self.file_as_list[i][0]))
-        else:
-            for i in range(len(self.file_as_list)):
-                if len(self.file_as_list[i]) == 1:
-                    time.append(self.file_as_list[i])
-            for i in range(len(time)):
-                interim = time[i][0].split()
-                timeraw.append(float(interim[2]))
-        return timeraw
+        find_connection = t2UtilitiesToughReact(self.filelocation, 'CONNE')
+        find_connection.find_word()
+        find_connection.slice_off_line()
+        find_connection.write_to_file()
+        with open('test.txt') as f:
+            grid_blocks = f.read().splitlines()
+        return grid_blocks
+
+    def get_times(self):
+        """ Get times stored for duration of the simulation
+
+        Parameters
+        -----------
+
+
+        Returns
+        --------
+        unprocessed_time_data : list
+            Time data directly from file without processing.
+        """
+        time_data = self.data.times
+        unprocessed_time_data = list(time_data)
+        value = t2Utilities()
+        if len(unprocessed_time_data) > 15:
+            time_data = value.chop_list(unprocessed_time_data, 15)
+            return time_data
+        return unprocessed_time_data
 
     def convert_times(self, format_of_date):
+        """ Convert time to desirable format e.g day, month, year
+
+        Parameters
+        -----------
+        format_of_date : str
+            Provides information to the method on format of the date. For example. year, hour, min or seconds
+
+        Returns
+        --------
+        processed_time_data  : list
+            List of converted time
+
         """
-        convert time to desirable time e.g day, month, year
-        :param format_of_date: string of type 'day', 'month', 'year'
-        :return: a list of the time
-        """
-        intermediate = self.get_times()
-        utility_function = t2Utilities()
-        timeyear = utility_function.convert_times(intermediate, format_of_date)
-        return timeyear
-
-    def get_time_index(self):
-        """ Get Index of Time """
-        self.read_file()
-        indextime = []
-        for index, value in enumerate(self.file_as_list):
-            if len(self.file_as_list[index]) == 1:
-                indextime.append(index)
-        indextime.append(len(self.file_as_list))
-        return indextime
-
-    def getGenerationData(self, param):
-        """ Get Data from GENER file """
-        self.read_file()
-        resultarray = []
-        heading = []
-        heading_first = self.file_as_list[0]
-        heading_first_modify = []
-        for i in heading_first:
-            heading_first_modify.append(i.upper())
-        for i in range(len(heading_first_modify)):
-            heading.append(heading_first_modify[i].lstrip())
-        index_param = heading.index(param.upper())
-        for i in range(1, len(self.file_as_list)):
-            resultarray.append(float(self.file_as_list[i][index_param]))
-        return resultarray
+        get_times = self.get_times()
+        utility_class = t2Utilities()
+        processed_time_data = utility_class.convert_times(get_times, format_of_date)
+        return processed_time_data
+
+    def get_timeseries_data(self, param, grid_block_number):
+        """ Get Time series data
+
+        Parameters
+        -----------
+        grid_block_number :  int
+            The grid block number for which to retrieve the results
+        param: string
+            Parameter to be derived from data
+
+        Returns
+        --------
+        final_timeseries_data : list
+            Time series data for particular parameter.
 
-    def get_elements(self):
-        """ Get elements from the simulation """
-        self.read_file()
-        indextime = self.get_time_index()
-        temp_file = self.file_as_list[indextime[0] + 1:indextime[1]]
-        elements = []
-        for i in range(len(temp_file)):
-            elements.append(temp_file[i][0])
-        return elements
-
-    def getParameters(self):
-        """ Remove space from parameters """
-        self.read_file()
-        full_list = self.file_as_list[0]
-        for i in range(len(full_list)):
-            full_list[i] = full_list[i].replace(" ", "")
-        return full_list
-
-    def resultdict(self):
-        self.read_file()
-        resultdict = {}
-        tempdict = {}
-        indextime = self.get_time_index()
-        timeraw = self.get_times()
-        for i in range(len(indextime) - 1):
-            tempdict[i] = self.file_as_list[indextime[i] + 1:indextime[i + 1]]
-        for i in range(len(timeraw)):
-            resultdict[timeraw[i]] = tempdict[i]
-        return resultdict
-
-    def get_timeseries_data(self, param, gridblocknumber):
-        """ Get Time series data"""
-        self.read_file()
-        results = self.resultdict()
-        resultarray = []
-        heading = []
-        heading_first = self.file_as_list[0]
-        heading_first_modify = []
-        for i in heading_first:
-            heading_first_modify.append(i.upper())
-        for i in range(len(heading_first_modify)):
-            heading.append(heading_first_modify[i].lstrip())
-        index_param = heading.index(param.upper())
-        for k in results.keys():
-            resultarray.append(results[k][gridblocknumber][index_param].lstrip())
-        final_data = [float(x) for x in resultarray]
-        return final_data
+        """
+        os.chdir(self.filelocation)
+        grid = self.get_elements()[grid_block_number]
+        mf = self.data.history([(grid, param)])
+        final_timeseries_data = mf[1]
+        final_timeseries_data = list(final_timeseries_data)
+        value = t2Utilities()
+        if len(final_timeseries_data) > 15:
+            final_timeseries_data = value.chop_list(final_timeseries_data, 15)
+            return final_timeseries_data
+        return final_timeseries_data
 
     def get_element_data(self, time, param):
-        """ Get Data for elements """
-        self.read_file()
-        timeraw = self.get_times()
-        results = self.resultdict()
-        heading = []
-        heading_first = self.file_as_list[0]
-        heading_first_modify = []
-        for i in heading_first:
-            heading_first_modify.append(i.upper())
-        for i in range(len(heading_first_modify)):
-            heading.append(heading_first_modify[i].lstrip())
-        index_param = heading.index(param.upper())
-        if time < timeraw[0]:
-            time = timeraw[0]
-        elif time > timeraw[-1]:
-            time = timeraw[-1]
-        else:
-            absolute_difference_function = lambda list_value: abs(list_value - time)
-            time = min(timeraw, key=absolute_difference_function)
-        results_specific = results[time]
-        data = []
-        for i in range(len(results_specific)):
-            data.append(results_specific[i][index_param].lstrip())
-        final_data = [float(x) for x in data]
-        return final_data
-
-    def get_X_data(self, time):
-        """ Get X Axis Data """
-        return self.get_element_data(time, 'x')
-
-    def get_Y_data(self, time):
-        """ Get Y Axis Data """
-        return self.get_element_data(time, 'y')
-
-    def get_Z_data(self, time):
-        """ Get Z Axis Data """
-        return self.get_element_data(time, 'z')
+        """ Get Data for elements
 
-    def get_coord_data(self, direction, timer):
-        """ Get Coordinate Data """
-        if direction.lower() == 'x':
-            value = self.get_X_data(timer)
-        elif direction.lower() == 'y':
-            value = self.get_Y_data(timer)
-        elif direction.lower() == 'z':
-            value = self.get_Z_data(timer)
-        else:
-            print("coordinates can either be X, Y or Z")
-        return value
+        Parameters
+        -----------
+        time : float
+            Time in which the data should be retrieved.
+        param: string
+            Parameter to be derive data
+
+        Returns
+        --------
+        final_element_data : list
+            Data for each of the elements.
+        """
+        self.data.set_time(time)
+        final_element_data = self.data.element[param]
+        return final_element_data
+
+    def get_x_data(self, time):
+        """ Get X Axis Data
+
+        Parameters
+        -----------
+        time : float
+            Time in which the data should be retrieved.
+
+        Returns
+        --------
+        output : list
+            Data for the x axis.
+
+        """
+        return self.get_element_data(time, 'X(m)')
+
+    def get_y_data(self, time):
+        """ Get Y Axis Data
+
+        Parameters
+        -----------
+        time : float
+            Time in which the data should be retrieved.
+
+        Returns
+        --------
+        output : list
+            Data for the y axis.
 
-    def getUniqueXData(self, timer):
-        """ Get Unique X Axis Data """
-        ori_array = self.get_coord_data('x', timer)
+        """
+        return self.get_element_data(time, 'Y(m)')
+
+    def get_z_data(self, time):
+        """ Get Z Axis Data
+
+        Parameters
+        -----------
+        time : float
+            Time in which the data should be retrieved.
+
+        Returns
+        --------
+        output : list
+            Data for the z axis.
+
+        """
+        return self.get_element_data(time, 'Z(m)')
+
+    def get_unique_x_data(self, timer):
+        """ Get Unique X Axis Data
+
+        Parameters
+        -----------
+        timer : float
+            Time in which the data should be retrieved.
+
+        Returns
+        --------
+        unique_x_output_data : list
+            Unique data for the x axis.
+
+        """
+        original_array = self.get_coord_data('x', timer)
         indices_array = []
-        for i in range(0, len(ori_array)):
+        for i in range(0, len(original_array)):
             try:
-                if ori_array[i] > ori_array[i + 1]:
+                if original_array[i] > original_array[i + 1]:
                     indices_array.append(i)
                 else:
                     continue
             except Exception:
                 pass
-        output_data = ori_array[0:indices_array[0] + 1]
-        return output_data
+        if len(indices_array) > 0:
+            unique_x_output_data = original_array[0:indices_array[0] + 1]
+        else:
+            unique_x_output_data = original_array
+        return unique_x_output_data
+
+    def get_x_start_points(self, timer):
+        """ Get X Axis Start Point Data
 
-    def getXStartPoints(self, timer):
-        """ Get X Axis Start Point Data """
+        Parameters
+        -----------
+        timer : float
+            Time in which the data should be retrieved.
+
+        Returns
+        --------
+        indices_array : list
+            X Axis Start Point Data.
+
+        """
         original_array = self.get_coord_data('x', timer)
         indices_array = []
         for i in range(0, len(original_array)):
             try:
                 if original_array[i] > original_array[i + 1]:
                     indices_array.append(i)
                 else:
                     continue
             except Exception:
                 pass
-        # output_data = ori_array[0:indices_array[0] + 1]
         return indices_array
 
-    def getUniqueYData(self, timer):
-        """ Get Unique Y Axis Data """
-        ori_array = self.get_coord_data('y', timer)
-        output = list(set(ori_array))
+    def get_unique_y_data(self, timer):
+        """ Get Unique Y Axis Data
+
+        Parameters
+        -----------
+        timer : float
+            Time in which the data should be retrieved.
+
+        Returns
+        --------
+        unique_x_output_data : list
+            Unique data for the y axis.
+
+        """
+        original_array = self.get_coord_data('y', timer)
+        output = list(set(original_array))
         return output
 
-    def getUniqueZData(self, timer):
-        """ Get Unique Z Axis Data """
+    def get_unique_z_data(self, timer):
+        """ Get Unique Z Axis Data
+
+        Parameters
+        -----------
+        timer : float
+            Time in which the data should be retrieved.
+
+        Returns
+        --------
+        unique_x_output_data : list
+            Unique data for the z axis.
+
+        """
         ori_array = self.get_coord_data('z', timer)
         output = list(set(ori_array))
         return output
 
-    def getNumberOfLayers(self, direction):
-        """ Get Number of Layers """
+    def get_number_of_layers(self, direction):
+        """ Get Number of Layers
+
+        Parameters
+        -----------
+        direction : string
+            Direction to get data. Can be 'X', 'Y', 'Z'
+
+        Returns
+        --------
+        number_of_layers : int
+            Total number of layers.
+
+        """
         if direction.lower() == 'x':
-            array = self.getUniqueXData(0)
+            array = self.get_unique_x_data(0)
         elif direction.lower() == 'y':
-            array = self.getUniqueYData(0)
+            array = self.get_unique_y_data(0)
         elif direction.lower() == 'z':
-            array = self.getUniqueZData(0)
+            array = self.get_unique_z_data(0)
         else:
             print("coordinates can either be X, Y or Z")
-        number = len(array)
-        return number
+        number_of_layers = len(array)
+        return number_of_layers
+
+    def get_z_layer_data(self, layer_number, param, timer):
+        """ Get Z Layer Data
+
+        Parameters
+        -----------
+        timer : float
+            Time in which the data should be retrieved.
+        layer_num: int
+            Layer number in which to retrieve data
+        param: string
+            Parameter to be derive data
+
+        Returns
+        --------
+        z_layer_data_output : list
+            Data for the z direction.
 
-    def getZLayerData(self, layer_number, param, timer):
-        """ Get Z Layer Data """
-        x_start = self.getXStartPoints(timer)
+        """
+        x_start = self.get_x_start_points(timer)
         z_data = self.get_element_data(timer, param)
-        total_grid_in_z = self.getNumberOfLayers('z')
+        total_grid_in_z = self.get_number_of_layers('z')
         if layer_number > 1:
             begin_index = x_start[layer_number - 2] + 1
         else:
             begin_index = 0
         if layer_number < total_grid_in_z:
             end_index = x_start[layer_number - 1] + 1
         else:
             end_index = 50
-        output = z_data[begin_index:end_index]
-        return output
+        z_layer_data_output = z_data[begin_index:end_index]
+        return z_layer_data_output
+
+    def get_x_depth_data(self, line_number, param, timer):
+        """ Get X Axis And Depth Data
 
-    def getXDepthData(self, line_number, param, timer):
-        """ Get X Axis And Depth Data """
+        Parameters
+        -----------
+        timer : float
+            Time in which the data should be retrieved.
+        line_number: int
+            Line number to retrieve x depth data for
+        param: string
+            Parameter to be derive data
+
+        Returns
+        --------
+        x_depth_data_array : list
+            Data for the x depth.
+
+        """
         element_data = self.get_element_data(timer, param)
-        x_layers = self.getNumberOfLayers('x')
-        z_layers = self.getNumberOfLayers('z')
-        data_array = []
+        x_layers = self.get_number_of_layers('x')
+        z_layers = self.get_number_of_layers('z')
+        x_depth_data_array = []
         for i in range(0, z_layers):
-            data_array.append(element_data[line_number - 1])
+            x_depth_data_array.append(element_data[line_number - 1])
             line_number = line_number + x_layers
-        return data_array
+        return x_depth_data_array
+
+    def get_layer_data(self, direction, layer_number, timer, param):
+        """ Get Layer Data
 
-    def getLayerData(self, direction, layer_number, timer, param):
-        """ Get Layer Data """
-        number_of_layers = self.getNumberOfLayers(direction)
+        Parameters
+        -----------
+        direction : string
+            Direction to get data. Can be 'X', 'Y', 'Z'
+        timer : float
+            Time in which the data should be retrieved.
+        layer_num: int
+            Layer number in which to retrieve data
+        param: string
+            Parameter to be derive data
+
+        Returns
+        --------
+        layer_data_array : list
+            Data for the specified direction.
+
+        """
+        number_of_layers = self.get_number_of_layers(direction)
         if layer_number > number_of_layers:
             raise ValueError("The specified layer is more than the number of layers in the model")
         else:
             if direction.lower() == 'z':
-                data_array = self.getZLayerData(layer_number, param, timer)
+                layer_data_array = self.get_z_layer_data(layer_number, param, timer)
             elif direction.lower() == 'x':
-                data_array = self.getXDepthData(layer_number, param, timer)
-        return data_array
+                layer_data_array = self.get_x_depth_data(layer_number, param, timer)
+        return layer_data_array
 
-    def get_unique_coord_data(self, direction, timer):
-        """ Get Unique Coordinate Data """
+    def get_coord_data(self, direction, timer):
+        """ Get Coordinate Data
+
+        Parameters
+        -----------
+        direction : string
+            Direction to get data. Can be 'X', 'Y', 'Z'
+        timer : float
+            Time in which the data should be retrieved.
+
+        Returns
+        --------
+        coordinate_data : list
+            Data for the unique coordinate.
+
+        """
         if direction.lower() == 'x':
-            value = self.getUniqueXData(timer)
+            coordinate_data = self.get_x_data(timer)
         elif direction.lower() == 'y':
-            value = self.getUniqueYData(timer)
+            coordinate_data = self.get_y_data(timer)
         elif direction.lower() == 'z':
-            value = self.getUniqueZData(timer)
+            coordinate_data = self.get_z_data(timer)
         else:
             print("coordinates can either be X, Y or Z")
-        return value
+        return coordinate_data
+
+    def get_unique_coord_data(self, direction, timer):
+        """ Get Unique Coordinate Data
+
+        Parameters
+        -----------
+        direction : string
+            Direction to get data. Can be 'X', 'Y', 'Z'
+        timer : float
+            Time in which the data should be retrieved.
+
+        Returns
+        --------
+        unique_coordinate_data : list
+            Data for the unique coordinate.
 
-    def remove_non_increasing(self, seqA, seqB):
-        """ Remove Non Increasing Data """
-        monotone = self.check_strictly_increasing(seqA)
-        if not monotone:
-            index = self.duplicate_index(seqA)
-            if len(index) > 0:
-                seqA = self.del_index(seqA, index)
-            indexes1 = self.duplicate_index(seqB)
-            if len(seqA) != len(seqB):
-                if len(indexes1) > 0:
-                    seqB = self.del_index(seqB, indexes1)
-        return seqA, seqB
-
-    def check_strictly_increasing(self, sequence):
-        """ Check for only strictly increasing data """
-        dx = np.diff(sequence)
-        return np.all(dx > 0)
-
-    def del_index(self, my_list, indexes):
-        """ Delete index """
-        for index in sorted(indexes, reverse=True):
-            del my_list[index]
-        return my_list
-
-    def duplicate_index(self, sequence):
-        """ Duplicate index """
-        dicta = {}
-        indexes = []
-        dups = collections.defaultdict(list)
-        for i, e in enumerate(sequence):
-            dups[e].append(i)
-        for k, v in sorted(dups.items()):
-            if len(v) >= 2:
-                dicta[k] = v
-        for k, v in dicta.items():
-            indexes.append(v[1:])
-        return list(itertools.chain.from_iterable(indexes))
+        """
+        if direction.lower() == 'x':
+            unique_coordinate_data = self.get_unique_x_data(timer)
+        elif direction.lower() == 'y':
+            unique_coordinate_data = self.get_unique_y_data(timer)
+        elif direction.lower() == 'z':
+            unique_coordinate_data = self.get_unique_z_data(timer)
+        else:
+            print("coordinates can either be X, Y or Z")
+        return unique_coordinate_data
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/utilities/t2_tough_react_utilities.py` & `pytoughreact-1.0.4/src/pytoughreact/utilities/t2_tough_react_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,52 +30,58 @@
 
 class t2UtilitiesToughReact(object):
     # takes in file names as a list
     """
     This class prepares the output files from TOUGHREACT for plot visualizations and analysis
     """
 
-    def __init__(self, location, word, file2='MESH'):
-
-        """
+    def __init__(self, location, word, mesh_file_name='MESH'):
+        """ Initialization of Parameters
         An instance of this class takes in five parameters the last of which is optional;
 
-        location --> the current direction where the simulations have been carried out
-        destination ---> the directory containing PYTOUGH and its class which would be needed for
-        manipulations
-        filenames -> the result files to be transferred to the destination folder
-        word --> the word where the truncation in the MESH file is to begin. Typically this should be 'CONNE'
+        Parameters
+        -----------
+        location : string
+            The current file location where the simulations have been carried out
+        word : string
+            The word where the truncation in the MESH file is to begin. Typically this should be 'CONNE'
+        mesh_file_name : string
+            The name of the mesh file
+
+        Returns
+        --------
         """
 
         self.location = location
         self.word = word
-        self.file2 = file2
+        self.file2 = mesh_file_name
 
-    def copyfile(self, filename, destination):
+    def copy_file(self, filename, destination):
         """ This method copies single file from the location to the destination folder. it takes in a a single argument
 
         Parameters
         -----------
         filename : str
             the name of the file to be transferred
         destination : str
             the name of the file to receive it
 
         Returns
         --------
+
         """
         # copy specific file
         src_files = os.listdir(self.location)
         for file_name in src_files:
             if file_name == filename:
                 full_file_name = os.path.join(self.location, file_name)
                 if (os.path.isfile(full_file_name)):
                     shutil.copy(full_file_name, destination)
 
-    def copyallfiles(self, filenames):
+    def copy_all_files(self, filenames):
         """This method copies all files given in the instance of the class to the destination folder. It makes use
         of the copyfile() method in achieving this
 
         Parameters
         -----------
         filenames : list
             list of all filename
@@ -83,18 +89,18 @@
         Returns
         --------
 
         """
         # copy all files
         for i in range(0, len(filenames)):
             a = filenames[i]
-            self.copyfile(a)
+            self.copy_file(a)
         print('...copying files...')
 
-    def findword(self):
+    def find_word(self):
         """ This method finds the word where the truncation of the MESH file is to occur.
 
         Parameters
         -----------
 
         Returns
         --------
@@ -106,15 +112,15 @@
         with open(self.file2) as myFile:
             for num, line in enumerate(myFile, 1):
                 if self.word in line:
                     point1 = num
                     return point1
         myFile.close()
 
-    def sliceofffile(self):
+    def slice_off_file(self):
         """ This method slices off all parameters below the word stated in the instance of the class
 
         Parameters
         -----------
 
         Returns
         --------
@@ -128,22 +134,22 @@
         f.close()
         f = open("test.txt", "w+")
         f.close()
         f = open('test2.txt', 'r+')
         f.truncate(0)
         f.close()
         os.remove("test.txt")
-        point1 = self.findword()
+        point1 = self.find_word()
         with open("test2.txt", "w") as f1:
             with open(self.file2, "r") as text_file:
                 for line in itertools.islice(text_file, 1, point1 - 2):
                     f1.write(line)
         f1.close()
 
-    def sliceoffline(self):
+    def slice_off_line(self):
         """ This method slices off all grid parameter such as the volume, distance betweeen grids as stated in
         the TOUGHREACT flow.inp file
 
         The aim of the findword(), sliceofffile() and this method is to provide us with a list of all gridblocks
         in the simulation
 
         Parameters
@@ -151,38 +157,37 @@
 
         Returns
         --------
         output : list
             list of grids
 
         """
-        self.sliceofffile()
+        self.slice_off_file()
         with open('test2.txt') as thefile:
             lines = thefile.readlines()
             output = []
             for i in range(0, len(lines)):
                 a = lines[i]
                 b = a[0:5]
                 output.append(b)
 
         return output
-        thefile.close()
 
-    def writetofile(self):
+    def write_to_file(self):
         """ This method writes all gridblocks to a separate file called 'test.txt' for easy location and onward
         manipulations
 
-        The aim of the findword(), sliceofffile() and this method is to provide us with a list of all gridblocks
+        The aim of the find_word(), slice_off_file() and this method is to provide us with a list of all gridblocks
         in the simulation
 
         Parameters
         -----------
 
         Returns
         --------
 
         """
-        mesh = self.sliceoffline()
+        mesh = self.slice_off_line()
         with open("test.txt", "w") as f1:
             for item in mesh:
                 f1.write("%s\n" % item)
         f1.close()
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/utilities/t2_utilities.py` & `pytoughreact-1.0.4/src/pytoughreact/utilities/t2_utilities.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,71 +27,139 @@
 
 
 class t2Utilities(object):
     def __init__(self):
         pass
 
     def convert_times(self, arraylist, format_of_date):
-        """ Convert times to second/minute/hour/day/year """
-        intermediate = arraylist
-        timeyear = []
+        """ Convert times to second/minute/hour/day/year
+
+        Parameters
+        -----------
+        arraylist :  list
+            Array of the time to be converted
+        format_of_date : str
+            Provides information to the method on format of the date. For example. year, hour, min or seconds
+
+        Returns
+        --------
+        processed_time_data : list
+            Time data after conversion
+        """
+        processing_data_array = arraylist
+        processed_time_data = []
         if format_of_date.lower() == 'year':
-            for i in range(len(intermediate)):
-                timeyear.append(intermediate[i] / 3.154e+7)
+            for i in range(len(processing_data_array)):
+                processed_time_data.append(processing_data_array[i] / 3.154e+7)
         elif format_of_date.lower() == 'day':
-            for i in range(len(intermediate)):
-                timeyear.append(intermediate[i] / 86400)
+            for i in range(len(processing_data_array)):
+                processed_time_data.append(processing_data_array[i] / 86400)
         elif format_of_date.lower() == 'hour':
-            for i in range(len(intermediate)):
-                timeyear.append(intermediate[i] / 3600)
+            for i in range(len(processing_data_array)):
+                processed_time_data.append(processing_data_array[i] / 3600)
         elif format_of_date.lower() == 'minute':
-            for i in range(len(intermediate)):
-                timeyear.append(intermediate[i] / 60)
+            for i in range(len(processing_data_array)):
+                processed_time_data.append(processing_data_array[i] / 60)
         elif format_of_date.lower() == 'second':
-            for i in range(len(intermediate)):
-                timeyear.append(intermediate[i])
+            for i in range(len(processing_data_array)):
+                processed_time_data.append(processing_data_array[i])
         else:
             raise ValueError("format can either be year, day, hour, minute or second")
-        return timeyear
+        return processed_time_data
+
+    def chop_list(self, input_list, step_increase=3):
+        """ Reduce the length of the list
 
-    def choplist(self, liste, number=3):
-        """ Reduce the lsit size """
-        global finallist
-        if isinstance(liste, list):
-            if len(liste) > 100:
-                liste = liste[0:len(liste):number]
-                self.choplist(liste)
+        Parameters
+        -----------
+        input_list :  list[float]
+            List for which its size is to be reduced
+        step_increase : int
+            Step increase to used in the length reduction
+
+        Returns
+        --------
+        final_processed_list : list
+            List data after reduction
+        """
+        global final_processed_list
+        if isinstance(input_list, list):
+            if len(input_list) > 100:
+                input_list = input_list[0:len(input_list):step_increase]
+                self.chop_list(input_list)
             else:
-                finallist = liste[0:len(liste):number]
-        return finallist
+                final_processed_list = input_list[0:len(input_list):step_increase]
+        return final_processed_list
+
+    def trim_data_points(self, time_data, result_data, slice_value):
+        """ Trim the result output to avoid too many points on a graph
+
+        Parameters
+        -----------
+        time_data :  list[float]
+            Time data list
+        result_data :  list[float]
+            Result data list
+        slice_value : float
+            Number at which to trim the data
+
+        Returns
+        --------
+        time_data, result_data : list , list
+            List data after trimming
 
-    def cutdata(self, time_data, resultdata, slicevalue):
-        """ Cut the result output to avoid too many points on a graph """
+        """
         for i in range(len(time_data) - 1, 0, -1):
-            if time_data[i] > slicevalue:
+            if time_data[i] > slice_value:
                 del time_data[i]
-                del resultdata[i]
-        return time_data, resultdata
+                del result_data[i]
+        return time_data, result_data
+
+    def remove_repetiting(self, time_list, value_list):
+        """ Remove repetiting values
+
+        Parameters
+        -----------
+        time_list :  list[float]
+            Time data list
+        value_list :  list[float]
+            Result data list
+
+        Returns
+        --------
+        final_time_list, final_value_list : list , list
+            List data after removing repetiting values
 
-    def removeRepetiting(self, time_list, value_list):
-        """ Remove repetiting values """
+        """
         final_time_list = []
         final_value_list = []
         for i in range(0, len(time_list)):
             if time_list[i] not in final_time_list:
                 final_time_list.append(time_list[i])
                 final_value_list.append(value_list[i])
         for i in range(len(final_time_list) - 1, 0, -1):
             if final_time_list[i] - final_time_list[i - 1] < 1:
                 del final_time_list[i]
                 del final_value_list[i]
         return final_time_list, final_value_list
 
     def param_label_full(self, param):
-        """ Get Full Names of TOUGHREACT and TMVIO parameters """
+        """ Get Full Names of TOUGHREACT and TMVIO parameters to be embedded in graphs
+
+        Parameters
+        -----------
+        param: string
+            Parameter to be derived from data
+
+        Returns
+        --------
+        output : string
+            Full name of parameter
+
+        """
         dict_param = {'PRES': 'Pressure (Pa)', 'TEMP': 'Temperature ($^o C$)', 'SAT_G': 'Gas Saturation (-)',
                       'SAT_L': 'Liquid Saturation (-)',
                       'SAT_N': 'NAPL Saturation (-)', 'X_WATER_G': 'Water Mass Fraction in Gas (-)',
                       'X_AIR_G': 'Air Mass Fraction in Gas (-)',
                       'X_WATER_L': 'Water Mass Fraction in Liquid (-)', 'X_AIR_L': 'Air Mass Fraction in Liquid (-)',
                       'X_WATER_N': 'Water Mass Fraction in NAPL (-)',
                       'X_AIR_N': 'Air Mass Fraction in NAPL (-)', 'REL_G"': 'Relative Permeability of Gas (-)',
@@ -115,37 +183,76 @@
                       'POROSITY': 'Porosity', 'ETTRINGITE': 'Ettringite',
                       'X3_L_TOLUENE': 'Mass Fraction of Toluene', 'X2_L_O2': 'Mass Fraction Oxygen',
                       'X_P-XYLE_L': 'Mass Fraction of p-Xylene'
                       }
         return dict_param[param]
 
     def fmt(self, x, pos):
+        """ Format string
+
+        Parameters
+        -----------
+        x: string
+            String to be formatted
+
+        Returns
+        --------
+        output : string
+            String after formatting
+
+        """
         a, b = '{:.2e}'.format(x).split('e')
         b = int(b)
         return r'${} \times 10^{{{}}}$'.format(a, b)
 
     def get_number_of_grids(self, input_list):
-        """ Get number of grids in simulation """
-        output = set()
+        """ Get number of grids in simulation
+
+        Parameters
+        -----------
+        input_list: list
+            List to determine number of grids
+
+        Returns
+        --------
+        total_number_of_grids : int
+            Total number of grids
+
+        """
+        total_number_of_grids = set()
         for x in input_list:
-            output.add(x)
-        output = list(output)
-        return len(output)
-
-    def getgridnumber(self, df, direction):
-        """ Get Grid number """
-        X = df[direction]
+            total_number_of_grids.add(x)
+        total_number_of_grids = list(total_number_of_grids)
+        return len(total_number_of_grids)
+
+    def get_grid_number(self, data_frame, direction):
+        """ Get today number of grids in a particular direction
+
+        Parameters
+        -----------
+        data_frame: pd.Dataframe
+            Dataframe containing coordinate info
+        direction: string
+            Direction in which the get grid number
+
+        Returns
+        --------
+        grid_details : list
+            Grid information
+
+        """
+        X = data_frame[direction]
         d = {}
         for i in X:
             if i not in d:
                 d[i] = 1
             else:
                 d[i] += 1
-        m = list(d.keys())
-        return m, len(d)
+        grid_details = list(d.keys())
+        return grid_details, len(d)
 
     def cust_range(self, *args, rtol=1e-05, atol=1e-08, include=[True, False]):
         """
         Combines numpy.arange and numpy.isclose to mimic
         open, half-open and closed intervals.
         Avoids also floating point rounding errors as with
         >>> numpy.arange(1, 1.3, 0.1)
@@ -189,16 +296,28 @@
 
     def crange(self, *args, **kwargs):
         return self.cust_range(*args, **kwargs, include=[True, True])
 
     def orange(self, *args, **kwargs):
         return self.cust_range(*args, **kwargs, include=[True, False])
 
-    def strip_param(self, param):
-        """ Convert Parameters by stripping """
+    def convert_parameter_name(self, param):
+        """ Convert Parameters to conventional names
+
+        Parameters
+        -----------
+        param: string
+            Parameter to be derived from data
+
+        Returns
+        --------
+        converted_output : string
+            parameter after conversion
+
+        """
         if param.lower() == 'porosity':
-            output = 'Porosity'
+            converted_output = 'Porosity'
         elif param.startswith("t_"):
-            output = "Total Concentration (mol/L)"
+            converted_output = "Total Concentration (mol/L)"
         elif param.startswith("pH"):
-            output = 'pH'
-        return output
+            converted_output = 'pH'
+        return converted_output
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/wrapper/react_data.py` & `pytoughreact-1.0.4/src/pytoughreact/wrapper/react_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,29 @@
 from pytoughreact.wrapper.reactblock import t2block
 import numpy as np
 
 
 class react_data(t2data):
     """Class for parsing REACTION data file."""
     def __init__(self, filename, mode, read_function=default_read_function):
+        """ Initialization of parameters
+
+        Parameters
+        -----------
+        filename : string
+            File name of the reaction data file
+        mode : str
+            Mode in which to read the dat (read, write)
+        read_fuction : function
+            Function for processing the different spacing forms
+
+        Returns
+        --------
+
+        """
         super(t2data, self).__init__(filename='', meshfilename='',
                                      read_function=default_read_function)
 
     def read_blocks(self, infile):
         """ Reads grid blocks.
 
         Parameters
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/wrapper/reactgrid.py` & `pytoughreact-1.0.4/src/pytoughreact/wrapper/reactgrid.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,71 +27,141 @@
 from pytoughreact.wrapper.reactzone import t2zone
 from pytoughreact.wrapper.reactblock import t2block
 from t2data import rocktype
 
 
 class t2reactgrid(t2grid):
     def __init__(self):
+        """ Initialization of parameters
+
+        Parameters
+        -----------
+
+        Returns
+        --------
+
+        """
         self.empty()
         super().__init__()
 
     def get_num_zones(self):
+        """ Return number of zones in grid
+
+        Parameters
+        -----------
+
+        Returns
+        --------
+        output : int
+            Total number of zones in grid
+        """
         return len(self.zonelist)
     num_zones = property(get_num_zones)
 
     def fromgeo(self, geo, blockmap={}):
-        """Converts a MULgraph grid to a TOUGH2 grid. The blockmap parameter
+        """ Converts a MULgraph grid to a TOUGH2 grid. The blockmap parameter
         applies an optional mapping to the block names from the geometry.
+
+        Parameters
+        -----------
+        geo :  MULgraph
+            Dimension details of the grid
+        blockmap : dict
+            Applies an optional mapping to the block names from the geometry.
+
+        Returns
+        --------
+
         """
         self.empty()
         self.add_rocktype(rocktype())  # add default rock type
         self.add_blocks(geo, blockmap)
         self.add_connections(geo, blockmap)
         return self
 
     def __add__(self, other):
-        """Adds two grids together."""
-        result = t2reactgrid()
+        """ Adds two grids together
+
+        Parameters
+        -----------
+        other :  t2reactgrid
+            Grid to add to original grid
+
+        Returns
+        --------
+        resultant_grid : t2reactgrid
+            Grid after addition
+        """
+        resultant_grid = t2reactgrid()
         for grid in [self, other]:
             for rt in grid.rocktypelist:
-                result.add_rocktype(rt)
+                resultant_grid.add_rocktype(rt)
             for blk in grid.blocklist:
-                result.add_block(blk)
+                resultant_grid.add_block(blk)
             for con in grid.connectionlist:
-                result.add_connection(con)
-        return result
+                resultant_grid.add_connection(con)
+        return resultant_grid
 
     def empty(self):
-        """Empties a TOUGH2 grid"""
+        """ Empties a TOUGH2 grid
+
+        Parameters
+        -----------
+
+        Returns
+        --------
+
+        """
         self.rocktypelist = []
         self.blocklist = []
         self.connectionlist = []
         self.rocktype = {}
         self.block = {}
         self.connection = {}
         self.zone = {}
         self.zonelist = []
 
     def add_block(self, newblock=None):
-        """Adds a block to the grid"""
+        """ Adds a block to the grid
+
+        Parameters
+        -----------
+        newblock :  t2block
+            block to add to original react grid
+
+        Returns
+        --------
+
+        """
         if newblock is None:
             newblock = t2block()
         if newblock.name in self.block:
             i = self.blocklist.index(self.block[newblock.name])
             self.blocklist[i] = newblock
         else:
             self.blocklist.append(newblock)
         self.block[newblock.name] = newblock
 
     def add_zone(self, newzone=None):
-        """Adds a rock type to the grid.  Any existing rocktype of the same name is replaced."""
+        """ Adds a rock type to the grid.  Any existing rocktype of the same name is replaced.
+
+        Parameters
+        -----------
+        newzone :  t2zone
+            zone to add to original react grid
+
+        Returns
+        --------
+
+        """
         if newzone is None:
             newzone = t2zone()
         if newzone.name in self.zone:
             i = self.zonelist.index(self.zone[newzone.name])
             self.zonelist[i] = newzone
         else:
             self.zonelist.append(newzone)
         self.zone[newzone.name] = newzone
 
     def __repr__(self):
-        return str(self.num_rocktypes) + ' rock types; ' + str(self.num_zones) + ' zones; ' + str(self.num_blocks) + ' blocks; ' + str(self.num_connections) + ' connections'
+        return str(self.num_rocktypes) + ' rock types; ' + str(self.num_zones) + \
+            ' zones; ' + str(self.num_blocks) + ' blocks; ' + str(self.num_connections) + ' connections'
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/wrapper/reactzone.py` & `pytoughreact-1.0.4/src/pytoughreact/wrapper/reactzone.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,15 +21,42 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
 
 class t2zone(object):
-    def __init__(self, name='default', water=None, mineral=None, gas=None, permporo=None, adsorption=None, decay=None, cation=None):
+    def __init__(self, name='default', water=None, mineral=None, gas=None, permporo=None, adsorption=None,
+                 decay=None, cation=None):
+        """ Initialization of parameters
+
+        Parameters
+        -----------
+        name : string
+            Name of the zone
+        water : list[list[Water], list[Water]]
+            List of initial and boundary waters
+        mineral : MineralZone
+            Mineral composition present in the zone
+        gas : list[list[ReactGas], list[ReactGas]]
+            List of all initial and injected gases
+        permporo : PermPoroZone
+            Porosity Permeability relationship to be used in the zone
+        adsorption : list[list[Adsorb], list[Adsorb]]
+            List of all initial and injected adsorption zones (Not Implemented yet)
+        decay : list[list[Decay], list[Decay]]
+            List of all initial and injected decay zones (Not Implemented yet)
+        cation : list[list[Cation], list[Cation]]
+            List of all initial and injected cation zones (Not Implemented yet)
+
+
+        Returns
+        --------
+
+        """
         self.name = name
         self.cation = cation
         self.decay = decay
         self.adsorption = adsorption
         self.permporo = permporo
         self.water = water
         self.mineral_zone = mineral
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/writers/bio_writing.py` & `pytoughreact-1.0.4/src/pytoughreact/writers/bio_writing.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,38 +591,47 @@
         # for i in range(len(all_components)):
         #     dicta = {}
         #     dicta[all_components[i]] = []
         #     dicta_all.append(dicta)
         all_processes = []
         for i in range(len(process_details)):
             dicta_all = self.reset_bio_dicta(all_components)
-            process = Process(biomass=biomass_details[process_details[i][0][1] - 1], numberOfComponents=process_details[i][0][0],
+            process = Process(biomass=biomass_details[process_details[i][0][1] - 1],
+                              numberOfComponents=process_details[i][0][0],
                               mumax=process_details[i][0][2], yield_mass=process_details[i][0][3],
                               NumOfCompetiting=process_details[i][0][4], NumOfNonCompetiting=process_details[i][0][5],
                               NumOfHaldane=process_details[i][0][6], enthalpy=process_details[i][0][7])
             for j in range(len(all_components)):
                 dicta_all[j][all_components[j]].append(process_details[i][5][j])
                 for k in range(len(process_details[i][1])):
                     if process_details[i][1][k] == j + 1:
                         dicta_all[j][all_components[j]].append(process_details[i][1][k + 1])
                 if len(dicta_all[j][all_components[j]]) == 1:
                     all_components[j].addToProcess(process, dicta_all[j][all_components[j]][0])
                 elif len(dicta_all[j][all_components[j]]) == 2:
-                    all_components[j].addToProcess(process, dicta_all[j][all_components[j]][0], dicta_all[j][all_components[j]][1])
+                    all_components[j].addToProcess(process, dicta_all[j][all_components[j]][0],
+                                                   dicta_all[j][all_components[j]][1])
                 elif len(dicta_all[j][all_components[j]]) == 3:
-                    all_components[j].addToProcess(process, dicta_all[j][all_components[j]][0], dicta_all[j][all_components[j]][1],
+                    all_components[j].addToProcess(process, dicta_all[j][all_components[j]][0],
+                                                   dicta_all[j][all_components[j]][1],
                                                    dicta_all[j][all_components[j]][2])
                 elif len(dicta_all[j][all_components[j]]) == 4:
-                    all_components[j].addToProcess(process, dicta_all[j][all_components[j]][0], dicta_all[j][all_components[j]][1],
-                                                   dicta_all[j][all_components[j]][2], dicta_all[j][all_components[j]][3])
+                    all_components[j].addToProcess(process, dicta_all[j][all_components[j]][0],
+                                                   dicta_all[j][all_components[j]][1],
+                                                   dicta_all[j][all_components[j]][2],
+                                                   dicta_all[j][all_components[j]][3])
                 elif len(dicta_all[j][all_components[j]]) == 5:
-                    all_components[j].addToProcess(process, dicta_all[j][all_components[j]][0], dicta_all[j][all_components[j]][1],
-                                                   dicta_all[j][all_components[j]][2], dicta_all[j][all_components[j]][3], dicta_all[j][all_components[j]][4])
+                    all_components[j].addToProcess(process, dicta_all[j][all_components[j]][0],
+                                                   [j][all_components[j]][1],
+                                                   dicta_all[j][all_components[j]][2],
+                                                   dicta_all[j][all_components[j]][3],
+                                                   dicta_all[j][all_components[j]][4])
             all_processes.append(process)
-        biodegradation = BIODG(imonod=params[0], bfac=params[2], sw1=params[4], sw2=params[5], wea=params[6], wsub=params[7],
+        biodegradation = BIODG(imonod=params[0], bfac=params[2], sw1=params[4], sw2=params[5], wea=params[6],
+                               wsub=params[7],
                                processes=all_processes, biomass=biomass_details, icflag=params[1])
         self.biodg.append(biodegradation)
 
     def write_biodg(self, outfile):
         """ Writes Biodegradation Block
 
         Parameters
@@ -995,12 +1004,13 @@
                     mesh_sections = ['ELEME', 'CONNE']
         if self.type == 'AUTOUGH2':
             self.write_extra_precision(extra_precision, echo_extra_precision)
         outfile = t2bio_parser(self.filename, 'w')
         self.write_title(outfile)
         for keyword in self._sections:
             if (keyword not in mesh_sections) and \
-                    ((keyword not in self.extra_precision) or (keyword in self.extra_precision and self.echo_extra_precision)):
+                    ((keyword not in self.extra_precision) or (keyword in self.extra_precision and
+                                                               self.echo_extra_precision)):
                 self.write_fn[keyword](outfile)
         outfile.write(self.end_keyword + '\n')
         self.status = 'successful'
         outfile.close()
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/writers/chemical_writing.py` & `pytoughreact-1.0.4/src/pytoughreact/writers/chemical_writing.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,46 +91,50 @@
             liner = (line.split())
             precip_presence = int(liner[2])
             presence = any(c.isalpha() for c in liner[0])
             if presence is True:
                 mineral = Mineral(liner[0], int(liner[1]), int(liner[2]), int(liner[3]), int(liner[4]))
                 line = self.file.readline()
                 liner = (line.split())
-                read_dissolution = Dissolution(float(liner[0]), int(liner[1]), float(liner[2]), float(liner[3]), float(liner[4]),
+                read_dissolution = Dissolution(float(liner[0]), int(liner[1]), float(liner[2]),
+                                               float(liner[3]), float(liner[4]),
                                                float(liner[5]), float(liner[6]), float(liner[7]))
                 type_of_pH = liner[1]
                 if int(type_of_pH) == 0:
                     mineral.dissolution = [read_dissolution]
                 else:
                     line = self.file.readline()
                     liner = (line.split())
                     if liner[0].isnumeric():
                         number_of_ph = int(liner[0])
                         ph_deps = []
                         for i in range(number_of_ph):
                             line = self.file.readline()
                             liner = (line.split())
                             if type_of_pH == '2':
-                                ph_dep = pHDependenceType2(float(liner[0]), float(liner[1]), int(liner[2]), liner[3], float(liner[4]))
+                                ph_dep = pHDependenceType2(float(liner[0]), float(liner[1]), int(liner[2]),
+                                                           liner[3], float(liner[4]))
                             elif type_of_pH == '1':
-                                ph_dep = pHDependenceType1(float(liner[0]), int(liner[1]), float(liner[2]), int(liner[3]))
+                                ph_dep = pHDependenceType1(float(liner[0]), int(liner[1]),
+                                                           float(liner[2]), int(liner[3]))
                             ph_deps.append(ph_dep)
                         read_dissolution.pHDependence = ph_deps
                         mineral.dissolution = [read_dissolution]
                 presence = any(c.isalpha() for c in liner[0])
                 if precip_presence > 1:
                     line = self.file.readline()
                     liner = (line.split())
                     init_line = liner
                     line = self.file.readline()
                     liner = (line.split())
                     liner = init_line + liner
                     read_precipitation = Precipitation(float(liner[0]), int(liner[1]), float(liner[2]), float(liner[3]),
                                                        float(liner[4]), float(liner[5]), float(liner[6]),
-                                                       float(liner[7]), float(liner[8]), int(liner[9]), float(liner[10]),
+                                                       float(liner[7]), float(liner[8]), int(liner[9]),
+                                                       float(liner[10]),
                                                        float(liner[11]), float(liner[12]))
                     mineral.precipitation = [read_precipitation]
             all_lines.append(mineral)
             line = self.file.readline()
         return all_lines
 
     def get_param_values_gas(self):
@@ -498,15 +502,16 @@
         Parameters
         -----------
         primary_aqueous : list
             list of all primary aqueous species in the CHEMICAL.INP
 
         Returns
         --------
-        initial_waters_list, boundary_waters_list, initial_waters_mapping, boundary_waters_mapping : list, list, dict, dict
+        initial_waters_list, boundary_waters_list, initial_waters_mapping, boundary_waters_mapping :
+        list, list, dict, dict
             properties of the initial and boundary water
 
         """
         initial_waters_mapping = {}
         initial_waters_list = []
         boundary_waters_mapping = {}
         boundary_waters_list = []
@@ -525,15 +530,16 @@
             pressure = float(liner[2])
             line = self.file.readline()
             line = self.file.readline()
             all_comp = []
             while line.startswith("'*") is False:
                 liner = (line.split())
                 specie = self.find_primary_aqueous(primary_aqueous, liner[0])
-                all_comp.append(WaterComp(specie, int(liner[1]), float(liner[2]), float(liner[3]), liner[4], float(liner[5])))
+                all_comp.append(WaterComp(specie, int(liner[1]), float(liner[2]), float(liner[3]), liner[4],
+                                          float(liner[5])))
                 line = self.file.readline()
             line = self.file.readline()
             line = self.file.readline()
             liner = (line.split())
             water_composition = [Water(all_comp, temp, pressure)]
             # grid.zonelist[water_num -1].water = water_composition
             initial_waters_mapping[water_num] = water_composition
@@ -550,15 +556,16 @@
             pressure = float(liner[2])
             line = self.file.readline()
             line = self.file.readline()
             all_comp = []
             while line.startswith("'*") is False:
                 liner = (line.split())
                 specie = self.find_primary_aqueous(primary_aqueous, liner[0])
-                all_comp.append(WaterComp(specie, int(liner[1]), float(liner[2]), float(liner[3]), liner[4], float(liner[5])))
+                all_comp.append(WaterComp(specie, int(liner[1]), float(liner[2]), float(liner[3]), liner[4],
+                                          float(liner[5])))
                 line = self.file.readline()
             line = self.file.readline()
             line = self.file.readline()
             liner = (line.split())
             water_composition = [Water(all_comp, temp, pressure)]
             # grid.zonelist[water_num -1].water = water_composition
             boundary_waters_mapping[water_num] = water_composition
@@ -622,16 +629,18 @@
             while line.startswith("'*") is False:
                 liner = (line.split())
                 initial_mineral_value = liner
                 mineral_found = self.find_minerals(minerals, liner[0])
                 line = self.file.readline()
                 liner = (line.split())
                 initial_mineral_value = initial_mineral_value + liner
-                spec_mineral = MineralComp(mineral_found, float(initial_mineral_value[1]), int(initial_mineral_value[2]),
-                                           float(initial_mineral_value[3]), float(initial_mineral_value[4]), int(initial_mineral_value[5]))
+                spec_mineral = MineralComp(mineral_found, float(initial_mineral_value[1]),
+                                           int(initial_mineral_value[2]),
+                                           float(initial_mineral_value[3]), float(initial_mineral_value[4]),
+                                           int(initial_mineral_value[5]))
                 all_comp.append(spec_mineral)
                 line = self.file.readline()
             line = self.file.readline()
             liner = (line.split())
             # grid.zonelist[mineral_num -1].mineral_zone = MineralZone(all_comp)
             initial_minerals_mapping[mineral_num] = MineralZone(all_comp)
             initial_minerals_list.append(MineralZone(all_comp))
@@ -761,15 +770,16 @@
             line = self.file.readline()
             line = self.file.readline()
             all_comp = []
             while line.startswith("'*") is False:
                 liner = (line.split())
                 initial_perm_poro_value = liner
                 liner = (line.split())
-                spec_perm_poro = PermPoro(initial_perm_poro_value[0], initial_perm_poro_value[1], initial_perm_poro_value[2])
+                spec_perm_poro = PermPoro(initial_perm_poro_value[0], initial_perm_poro_value[1],
+                                          initial_perm_poro_value[2])
                 spec_perm_poro_zone = PermPoroZone([spec_perm_poro])
                 all_comp.append(spec_perm_poro_zone)
                 initial_perm_poro_mapping[perm_poro_num] = PermPoroZone(all_comp)
                 initial_perm_poro_list.append(PermPoroZone(all_comp))
                 line = self.file.readline()
             line = self.file.readline()
             liner = (line.split())
@@ -782,14 +792,29 @@
 
 
 class t2chemical(t2data):
     """
         Main class for structuring the writing , reading  of chemical parameters
     """
     def __init__(self, filename='', meshfilename='', t2reactgrid=None, path=None, read_function=default_read_function):
+        """Initialization of Parameters (Permeability Porosity)
+
+        Parameters
+        -----------
+        filename :  string
+            Name of file to be read from (optional)
+        meshfilename :  string
+            Name of mesh file to be read from (optional)
+        t2reactgrid : t2reactgrid
+            Grid object from t2react
+
+        Returns
+        --------
+
+        """
         self.t2grid = t2reactgrid
         self._sections = []
         self.title = ''
         self.primary_aqueous = []
         self.aqueous_kinetics = [-1]
         self.aqueous_complexes = [-1]
         self.minerals = []
@@ -1451,16 +1476,17 @@
 
         Returns
         --------
         components: self
             adds Initial and Boundary waters to grid
 
         """
-        initial_waters_list, boundary_waters_list, initial_waters_mapping, boundary_waters_mapping = infile.get_param_values_ib_waters(
-            self.primary_aqueous, self.t2grid)
+        initial_waters_list, boundary_waters_list, initial_waters_mapping, boundary_waters_mapping \
+            = infile.get_param_values_ib_waters(
+                self.primary_aqueous, self.t2grid)
         if len(initial_waters_list) == 0:
             self.__dict__['ib_waters'] = [-1]
         else:
             self.__dict__['waters'][0] = initial_waters_list
             if len(boundary_waters_list) > 0:
                 self.__dict__['waters'][1] = boundary_waters_list
             self.initial_waters_mapping = initial_waters_mapping
@@ -1532,27 +1558,29 @@
                 for i in range(len(boundary_water)):
                     outfile.write('# Index  Speciation T(C)  P(bar)  \n')
                     vals = [i + 1, boundary_water[i][0].temperature, boundary_water[i][0].pressure]
                     outfile.write_values(vals, 'water_comp1')
                     species = boundary_water[i][0].primary_species
                     outfile.write('#        icon       NRguess(molal)  ctot (molal)   \n')
                     for specie in species:
-                        vals = [specie.primary_species.NAME.strip(), specie.icon, specie.nrguess, specie.ctot, specie.nameq,
+                        vals = [specie.primary_species.NAME.strip(), specie.icon, specie.nrguess, specie.ctot,
+                                specie.nameq,
                                 specie.qksat]
                         outfile.write_values(vals, 'water_comp2')
                     outfile.write("'*'\n")
             except Exception:
                 for i in range(len(boundary_water)):
                     outfile.write('# Index  Speciation T(C)  P(bar)  \n')
                     vals = [i + 1, boundary_water[i].temperature, boundary_water[i].pressure]
                     outfile.write_values(vals, 'water_comp1')
                     species = boundary_water[i].primary_species
                     outfile.write('#        icon       NRguess(molal)  ctot (molal)   \n')
                     for specie in species:
-                        vals = [specie.primary_species.NAME.strip(), specie.icon, specie.nrguess, specie.ctot, specie.nameq,
+                        vals = [specie.primary_species.NAME.strip(), specie.icon, specie.nrguess, specie.ctot,
+                                specie.nameq,
                                 specie.qksat]
                         outfile.write_values(vals, 'water_comp2')
                     outfile.write("'*'\n")
 
     def getInitialWaterIndex(self):
         """ Get Initial Water Index
 
@@ -1751,15 +1779,16 @@
         for zone in self.mineral_zones:
             indexer = [index]
             outfile.write_values(indexer, 'mineral_zone1')
             outfile.write('# mineral         vol.frac\n')
             for mineralcomp in zone.minerals:
                 vals = [mineralcomp.mineral.name, mineralcomp.init_volume_fraction, mineralcomp.reaction_type]
                 outfile.write_values(vals, 'mineral_zone2')
-                if mineralcomp.radius is not None and mineralcomp.reactive_surface_area is not None and mineralcomp.unit is not None:
+                if (mineralcomp.radius is not None and mineralcomp.reactive_surface_area is not None and
+                        mineralcomp.unit is not None):
                     vals = [mineralcomp.radius, mineralcomp.reactive_surface_area, mineralcomp.unit]
                     outfile.write_values(vals, 'mineral_zone2.1')
             index += 1
             outfile.write("'*'\n")
 
     def read_ij_gas(self, infile):
         """ Read Initial and Injection Gas
@@ -1771,16 +1800,16 @@
 
         Returns
         --------
         components: self
             adds injection gas to grid
 
         """
-        initial_gas_list, injection_gas_list, initial_gas_mapping, injection_gas_mapping = infile.get_param_values_ij_gases(
-            self.gases)
+        initial_gas_list, injection_gas_list, initial_gas_mapping, injection_gas_mapping \
+            = infile.get_param_values_ij_gases(self.gases)
         if len(initial_gas_list) == 0:
             self.__dict__['ij_gas'] = [[], []]
         else:
             self.__dict__['ij_gas'][0] = initial_gas_list
             self.initial_gas_mapping = initial_gas_mapping
             if len(injection_gas_list) > 0:
                 self.__dict__['ij_gas'][1] = injection_gas_list
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/writers/react_writing.py` & `pytoughreact-1.0.4/src/pytoughreact/writers/react_writing.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
-from pytoughreact.constants.format_specifications import t2react_format_specification, t2react_extra_precision_format_specification
+from pytoughreact.constants.format_specifications import t2react_format_specification, \
+    t2react_extra_precision_format_specification
 from pytoughreact.constants.defaults_constants import DEFAULT_REACT as default_react
 from pytoughreact.constants.defaults_constants import DEFAULT_PARAMETERS as default_parameters
 from pytoughreact.constants.sections import t2react_sections
 from fixed_format_file import default_read_function, fixed_format_file
 from pytoughreact.wrapper.reactgrid import t2reactgrid
 from pytoughreact.wrapper.reactblock import t2block
 from pytoughreact.exceptions.custom_error import NotFoundError
@@ -636,11 +637,12 @@
                     self.write_binary_meshfiles()
                     mesh_sections = ['ELEME', 'CONNE']
         if self.type == 'AUTOUGH2':
             self.write_extra_precision(extra_precision, echo_extra_precision)
         outfile = t2react_parser(self.filename, 'w')
         self.write_title(outfile)
         for keyword in self._sections:
-            if (keyword not in mesh_sections) and ((keyword not in self.extra_precision) or (keyword in self.extra_precision and self.echo_extra_precision)):
+            if (keyword not in mesh_sections) and ((keyword not in self.extra_precision) or
+                                                   (keyword in self.extra_precision and self.echo_extra_precision)):
                 self.write_fn[keyword](outfile)
         outfile.write(self.end_keyword + '\n')
         outfile.close()
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact/writers/solute_writing.py` & `pytoughreact-1.0.4/src/pytoughreact/writers/solute_writing.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 import os
 import sys
 from fixed_format_file import default_read_function, fixed_format_file
 from t2data import t2data
 from pytoughreact.constants.format_specifications import t2solute_format_specification
 from pytoughreact.constants.sections import t2solute_sections
 from pytoughreact.constants.defaults_constants import (DEFAULT_OPTIONS, DEFAULT_CONSTRAINTS, DEFAULT_READIO,
-                                                       DEFAULT_WEIGHT_DIFFUSION, DEFAULT_TOLERANCE, DEFAULT_PRINTOUT, DEFAULT_ZONE)
+                                                       DEFAULT_WEIGHT_DIFFUSION, DEFAULT_TOLERANCE, DEFAULT_PRINTOUT,
+                                                       DEFAULT_ZONE)
 from pytoughreact.exceptions.custom_error import ReactiveOptionsError, RequiredInputException, ReactiveConstraintsError
 from copy import deepcopy
 
 
 class t2solute_parser(fixed_format_file):
     """Class for parsing SOLUTE.INP data file."""
 
@@ -333,15 +334,16 @@
 
 
 class t2solute(t2data):
     """
         Main class for structuring the writing , reading  of solute parameters
     """
     def __init__(self, filename='', meshfilename='', options=None, chemical_zones=None, constraints=None, readio=None,
-                 weight_diffusion=None, tolerance=None, printout=None, t2chemical=None, read_function=default_read_function):
+                 weight_diffusion=None, tolerance=None, printout=None, t2chemical=None,
+                 read_function=default_read_function):
         super().__init__(filename, meshfilename, read_function)
         self.t2chemical = t2chemical
         self._sections = []
         if self.t2chemical is not None:
             self.title = self.t2chemical.title
         else:
             self.title = 'Reactive Transport'
@@ -456,15 +458,16 @@
                     initial_gas_zone = self.getZoneValue(self.initial_gas_index, initial_gas)
                     boundary_water_zone = self.getZoneValue(self.boundary_water_index, boundary_water)
                     injection_gas_zone = self.getZoneValue(self.injection_gas_index, injection_gas)
                 except ValueError:
                     boundary_water_zone = 1
                     injection_gas_zone = 1
                     initial_gas_zone = 1
-                appender = [block.name, 0, 0, initial_water_zone, boundary_water_zone, mineral_zone, initial_gas_zone, 0, 0,
+                appender = [block.name, 0, 0, initial_water_zone, boundary_water_zone, mineral_zone, initial_gas_zone,
+                            0, 0,
                             perm_poro_zone, 0, injection_gas_zone]
                 output.append(appender)
                 viewer.append(block)
             return output
         except Exception:
             return output
 
@@ -1168,15 +1171,16 @@
         Returns
         --------
 
         """
         # TODO find out why leaving a space doesnt run
         if self.aqueous_species[0] == -1:
             outfile.write("\n")
-            # outfile.write('# Individual aqueous species for which to output concentrations in time and plot files:' + ' \n tr' )
+            # outfile.write('# Individual aqueous species for which to output concentrations in time and plot files:'
+            # + ' \n tr' )
             outfile.write(
                 '# Individual aqueous species for which to output concentrations in time and plot files:' + '\n')
 
     def read_adsorption_species(self, infile):
         """Reads Adsorption species for which to output concentrations in time and plot files"""
         pass
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact.egg-info/PKG-INFO` & `pytoughreact-1.0.4/src/pytoughreact.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,35 @@
 Metadata-Version: 2.1
 Name: pytoughreact
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Library for automating reaction simulations using TOUGHREACT, TMVOC and TMVOC-BIO
 Author-email: Temitope Ajayi <ajayi_temmy@yahoo.com>
 Maintainer-email: Temitope Ajayi <ajayi_temmy@yahoo.com>
 License: MIT License
-        
-        Copyright (c) 2023 Temitope Ajayi
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Project-URL: repository, https://github.com/temmy222/PyTOUGHREACT
 Keywords: biodegradation,reactive transport,automation,uncertainty quantification
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1
 Requires-Dist: scipy>=1
 Requires-Dist: vtk>=1
 Requires-Dist: matplotlib>=3
 Requires-Dist: pandas>=1
 Requires-Dist: PyTOUGH
+Requires-Dist: flake8
 
 # PyTOUGHREACT
 
 
 - [PyTOUGHREACT](#pytoughreact)
   - [Installation](#installation)
   - [Usage](#usage)
@@ -76,15 +56,22 @@
 
 The package can also be forked from this GitHub page and installation performed using
 
 ```bash
 python setup.py install  or py setup.py install
 ```
 
-Because pytoughreact requires PyTOUGH and PyTOUGH is not uploaded to PyPI, it is required to download the zip folder of PyTOUGH from the GitHub repository https://github.com/acroucher/PyTOUGH. Unzip the folder and place in your current working directory. Change directory into the PyTOUGH folder and run python setup.py install or pip install on the command line. With PyTOUGH installed, PyTOUGHREACT is ready to be used as a package.
+<!-- Because pytoughreact requires PyTOUGH and PyTOUGH is not uploaded to PyPI, it is required to download the zip folder of PyTOUGH from the GitHub repository https://github.com/acroucher/PyTOUGH. Unzip the folder and place in your current working directory. Change directory into the PyTOUGH folder and run python setup.py install or pip install on the command line. With PyTOUGH installed, PyTOUGHREACT is ready to be used as a package. -->
+
+Because pytoughreact requires PyTOUGH, this library also needs to be installed.
+PyTOUGH can be installed by running the command below
+
+```bash
+pip install PyTOUGH
+```
 
 ## Usage
 
 ```python
 import os
 from mulgrids import mulgrid
 from pytoughreact.writers.react_writing import t2react
@@ -226,20 +213,41 @@
 1. Clone the repo using preferred cloning method
 2. Install the library to enable you able to use the test example using
 
 ```python
 pip install -e .
 ```
 3. Modify the code 
-4. Run tests: Tests are conducted with pytest. Flake8 is also used to ensure code readability
+4. Tests are conducted with pytest and coverage reports are performed using pytest-cov. Install pytest and pytest-cov using the commands below
+   
+```python
+pip install pytest
+```
 
 ```python
+pip install pytest-cov
+```
+5. Run tests:  Run the below command from the root folder to run the tests
+   
+```python
 pytest
 ```
-5. Make a pull request after passing all tests
+
+6. Flake8 is also used to ensure code readability. Install flake8 using 
+   
+```python
+pip install flake8
+```
+and run flake8 using
+
+```python
+flake8 src
+```
+7. Make a pull request after passing all tests
+8. More information can be found in developer notes in the documentation - https://pytoughreact.readthedocs.io/en/master/developer.html 
 
 ## Documentation
 Documentation can be found here https://pytoughreact.readthedocs.io/en/latest/ 
 
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `pytoughreact-1.0.3/src/pytoughreact.egg-info/SOURCES.txt` & `pytoughreact-1.0.4/src/pytoughreact.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 src/pytoughreact/py.typed
 src/pytoughreact/version.py
 src/pytoughreact.egg-info/PKG-INFO
 src/pytoughreact.egg-info/SOURCES.txt
 src/pytoughreact.egg-info/dependency_links.txt
 src/pytoughreact.egg-info/requires.txt
 src/pytoughreact.egg-info/top_level.txt
-src/pytoughreact/assembler/__init__.py
 src/pytoughreact/chemical/__init__.py
 src/pytoughreact/chemical/bio_process_description.py
 src/pytoughreact/chemical/biomass_composition.py
 src/pytoughreact/chemical/chemical_composition.py
 src/pytoughreact/chemical/kinetic_properties.py
 src/pytoughreact/chemical/mineral_composition.py
 src/pytoughreact/chemical/mineral_description.py
@@ -29,21 +28,14 @@
 src/pytoughreact/constants/grid_constants.py
 src/pytoughreact/constants/plotconstants.py
 src/pytoughreact/constants/reactionconstants.py
 src/pytoughreact/constants/rel_perm_constants.py
 src/pytoughreact/constants/sections.py
 src/pytoughreact/exceptions/__init__.py
 src/pytoughreact/exceptions/custom_error.py
-src/pytoughreact/model/__init__.py
-src/pytoughreact/model/capillary_pressure.py
-src/pytoughreact/model/grid.py
-src/pytoughreact/model/physical_model.py
-src/pytoughreact/model/relative_permeability.py
-src/pytoughreact/numerical/__init__.py
-src/pytoughreact/numerical/physical_model_numericals.py
 src/pytoughreact/plotting/__init__.py
 src/pytoughreact/plotting/plot_multiple.py
 src/pytoughreact/plotting/plot_multiple_files_routine.py
 src/pytoughreact/plotting/plot_multiple_tough_routine.py
 src/pytoughreact/plotting/plot_single.py
 src/pytoughreact/plotting/plot_tough_routine.py
 src/pytoughreact/results/__init__.py
```

### Comparing `pytoughreact-1.0.3/test/test_pytoughreact_bio.py` & `pytoughreact-1.0.4/test/test_pytoughreact_bio.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                         bio.add_generator(gen)
                     else:
                         gen = t2generator(name=well + str(i), block=bio.grid.blocklist[i].name, type=component,
                                           ltab=len(duration), itab=str(3), time=duration, rate=rate, enthalpy=energy)
                         bio.add_generator(gen)
                     j = j + 1
 
-        # ____________________________________RUN SIMULATION_______________________________________________________________
+        # ____________________________________RUN SIMULATION____________________________________________________________
         bio.write('INFILE', runlocation=os.getcwd())
         # bio.run(simulator='tmvoc', runlocation='')
         return bio
 
     def set_up_read(self):
         bio_read = t2bio()
         bio_read.read('INFILE')
```

### Comparing `pytoughreact-1.0.3/test/test_pytoughreact_react.py` & `pytoughreact-1.0.4/test/test_pytoughreact_react.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 from mulgrids import mulgrid
 from pytoughreact.chemical.kinetic_properties import pHDependenceType2, Dissolution, Precipitation
 from pytoughreact.chemical.mineral_description import Mineral
 from pytoughreact.chemical.chemical_composition import PrimarySpecies, WaterComp, Water, ReactGas
 from pytoughreact.chemical.mineral_composition import MineralComp
 from pytoughreact.chemical.mineral_zone import MineralZone
 from pytoughreact.chemical.perm_poro_zone import PermPoro, PermPoroZone
@@ -11,15 +12,14 @@
 from pytoughreact.writers.chemical_writing import t2chemical
 from pytoughreact.wrapper.reactzone import t2zone
 from pytoughreact.wrapper.reactgrid import t2reactgrid
 from pytoughreact.results.t2result import t2result
 from t2data import rocktype
 
 
-
 class ReactTestCase():
     def get_specific_mineral(self, mineral_name):
 
         calcite_ph = pHDependenceType2(5.0119e-01, 14.4, 1, 'h+', 1.0)
         dissolution_calcite = Dissolution(1.5488e-06, 2, 1, 1, 23.5, 0, 0, 0)
         dissolution_calcite.pHDependence = [calcite_ph]
         precipitation_calcite = Precipitation(1.5488e-06, 0, 1, 1, 23.5, 0, 0, 0, 1.0E-5, 0, 0, 0, 0)
@@ -294,15 +294,16 @@
         al_comp1 = WaterComp(al, 1, 1E-10, 9.96E-5)
         fe_comp1 = WaterComp(fe, 1, 1E-10, 9.7E-9)
         hs_comp1 = WaterComp(hs, 1, 1E-10, 1E-10)
 
         initial_water_zone1 = Water([h2o_comp1, h_comp1, na_comp1, cl_comp1, hco3_comp1, ca_comp1, so4_comp1, mg_comp1,
                                      h4sio4_comp1, al_comp1, fe_comp1, hs_comp1], 25, 200)
 
-        mineral_list = ['c3fh6', 'tobermorite', 'calcite', 'csh', 'portlandite', 'ettringite', 'katoite', 'hydrotalcite']
+        mineral_list = ['c3fh6', 'tobermorite', 'calcite', 'csh', 'portlandite', 'ettringite', 'katoite',
+                        'hydrotalcite']
         all_minerals = self.get_kinetics_minerals(mineral_list)
 
         c3fh6_zone1 = MineralComp(self.get_specific_mineral(mineral_list[0]), 0.1, 0, 0.0E-00, 20000.0, 0)
         tobermorite_zone1 = MineralComp(self.get_specific_mineral(mineral_list[1]), 0.05, 0, 0.0E-00, 20000.0, 0)
         calcite_zone1 = MineralComp(self.get_specific_mineral(mineral_list[2]), 0.4, 1, 0.0E-00, 260.0, 0)
         csh_zone1 = MineralComp(self.get_specific_mineral(mineral_list[3]), 0.1, 1, 0.0E-00, 20000.0, 0)
         portlandite_zone1 = MineralComp(self.get_specific_mineral(mineral_list[4]), 0.1, 1, 0.0E-00, 1540.0, 0)
@@ -314,15 +315,16 @@
         # ijgas = [[initial_co2], []]
 
         permporo = PermPoro(1, 0, 0)
         permporozone = PermPoroZone([permporo])
 
         zone1.water = [[initial_water_zone1], []]
         zone1.gas = [[initial_co2], []]
-        mineral_zone1 = MineralZone([c3fh6_zone1, tobermorite_zone1, calcite_zone1, csh_zone1, portlandite_zone1, ettringite_zone1,
+        mineral_zone1 = MineralZone([c3fh6_zone1, tobermorite_zone1, calcite_zone1, csh_zone1, portlandite_zone1,
+                                     ettringite_zone1,
                                      katoite_zone1, hydrotalcite_zone1])
         zone1.mineral_zone = mineral_zone1
         zone1.permporo = permporozone
 
         writeChemical = t2chemical(t2reactgrid=react.grid)
         writeChemical.minerals = all_minerals
         writeChemical.title = 'Automating Tough react'
@@ -362,14 +364,15 @@
     write_output = test_case.set_up_read()
     result = write_output.status
     assert result == 'successful'
 
 
 def test_result_first():
     FILE_PATH = os.path.abspath(os.curdir)
+    FILE_PATH = os.path.dirname(os.path.realpath(__file__))
     results = t2result('toughreact', 'kdd_conc.tec', FILE_PATH)
     time = results.get_times()
     parameter_result = results.get_time_series_data('pH', 0)
     time_length = len(time)
     parameter_result_length = len(parameter_result)
     assert time_length == parameter_result_length
```

