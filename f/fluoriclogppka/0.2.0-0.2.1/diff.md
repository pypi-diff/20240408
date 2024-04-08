# Comparing `tmp/fluoriclogppka-0.2.0.tar.gz` & `tmp/fluoriclogppka-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluoriclogppka-0.2.0.tar", last modified: Tue Mar 26 15:01:04 2024, max compression
+gzip compressed data, was "fluoriclogppka-0.2.1.tar", last modified: Mon Apr  8 13:03:34 2024, max compression
```

## Comparing `fluoriclogppka-0.2.0.tar` & `fluoriclogppka-0.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.989924 fluoriclogppka-0.2.0/
--rw-rw-rw-   0        0        0     1079 2024-03-05 16:24:49.000000 fluoriclogppka-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      120 2024-03-05 16:22:22.000000 fluoriclogppka-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      597 2024-03-26 15:01:03.990921 fluoriclogppka-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      635 2024-03-26 14:33:38.000000 fluoriclogppka-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.693544 fluoriclogppka-0.2.0/fluoriclogppka/
--rw-rw-rw-   0        0        0      281 2024-03-05 14:31:48.000000 fluoriclogppka-0.2.0/fluoriclogppka/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.722541 fluoriclogppka-0.2.0/fluoriclogppka/data/
--rw-rw-rw-   0        0        0    31365 2024-01-25 13:31:49.000000 fluoriclogppka-0.2.0/fluoriclogppka/data/pKa_Prediction_Starting_data_2024.01.25.csv
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.736548 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:27:18.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/__init__.py
--rw-rw-rw-   0        0        0     4341 2024-03-26 14:33:38.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/constants.py
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.745540 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/data_preparation/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:23:35.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/data_preparation/__init__.py
--rw-rw-rw-   0        0        0     4853 2024-03-26 14:36:16.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/data_preparation/smiles_to_features.py
--rw-rw-rw-   0        0        0     1391 2024-02-27 14:57:08.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.750544 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/inference/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:23:35.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/inference/__init__.py
--rw-rw-rw-   0        0        0     4223 2024-03-26 14:35:16.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/inference/inference.py
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.656541 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.658556 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.657543 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/logP/
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.875185 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/logP/all_molecules(without_angle_feature)_without_outliers/
--rw-rw-rw-   0        0        0 18512739 2024-02-08 20:47:01.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/logP/all_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_3_AutoML_2_20240208_214951
--rw-rw-rw-   0        0        0 15154680 2024-02-08 19:40:31.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/logP/all_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_5_AutoML_1_20240208_212954
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.660543 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.910186 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/acid_molecules(without_angle_feature)_without_outliers/
--rw-rw-rw-   0        0        0  1745159 2024-02-13 09:22:56.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/acid_molecules(without_angle_feature)_without_outliers/DeepLearning_grid_2_AutoML_4_20240213_102321_model_43
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.917186 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/amine_molecules(without_angle_feature)_without_outliers/
--rw-rw-rw-   0        0        0 18114821 2024-02-13 08:22:55.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/amine_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_5_AutoML_3_20240213_92029
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.987920 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:23:35.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/__init__.py
--rw-rw-rw-   0        0        0    47437 2024-02-28 09:51:32.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/features.py
--rw-rw-rw-   0        0        0     2740 2024-03-26 14:35:16.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/h2o_service.py
--rw-rw-rw-   0        0        0     3810 2024-03-26 14:38:23.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/molecule_2d_features_service.py
--rw-rw-rw-   0        0        0    44368 2024-03-26 14:39:52.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/molecule_3d_features_service.py
--rw-rw-rw-   0        0        0     2391 2024-02-28 09:50:08.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/mordred_features_service.py
--rw-rw-rw-   0        0        0     6057 2024-03-05 13:15:07.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/utils.py
--rw-rw-rw-   0        0        0     5960 2024-03-05 14:32:34.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/utils_logP.py
--rw-rw-rw-   0        0        0     3022 2024-03-05 14:32:30.000000 fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/utils_pKa.py
-drwxrwxrwx   0        0        0        0 2024-03-26 15:01:03.715541 fluoriclogppka-0.2.0/fluoriclogppka.egg-info/
--rw-rw-rw-   0        0        0      597 2024-03-26 15:00:59.000000 fluoriclogppka-0.2.0/fluoriclogppka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1754 2024-03-26 15:00:59.000000 fluoriclogppka-0.2.0/fluoriclogppka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 15:00:59.000000 fluoriclogppka-0.2.0/fluoriclogppka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      299 2024-03-26 15:00:59.000000 fluoriclogppka-0.2.0/fluoriclogppka.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-26 15:00:59.000000 fluoriclogppka-0.2.0/fluoriclogppka.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-26 15:01:04.001922 fluoriclogppka-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-03-26 14:57:38.000000 fluoriclogppka-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.405105 fluoriclogppka-0.2.1/
+-rw-rw-rw-   0        0        0     1083 2024-04-08 13:01:25.000000 fluoriclogppka-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      120 2024-03-05 16:22:22.000000 fluoriclogppka-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      597 2024-04-08 13:03:34.406105 fluoriclogppka-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      635 2024-03-26 14:33:38.000000 fluoriclogppka-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.212626 fluoriclogppka-0.2.1/fluoriclogppka/
+-rw-rw-rw-   0        0        0      281 2024-03-05 14:31:48.000000 fluoriclogppka-0.2.1/fluoriclogppka/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.226608 fluoriclogppka-0.2.1/fluoriclogppka/data/
+-rw-rw-rw-   0        0        0    31365 2024-01-25 13:31:49.000000 fluoriclogppka-0.2.1/fluoriclogppka/data/pKa_Prediction_Starting_data_2024.01.25.csv
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.231713 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:27:18.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/__init__.py
+-rw-rw-rw-   0        0        0     4396 2024-04-08 12:23:12.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.233713 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/data_preparation/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:23:35.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/data_preparation/__init__.py
+-rw-rw-rw-   0        0        0     4853 2024-04-08 12:25:45.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/data_preparation/smiles_to_features.py
+-rw-rw-rw-   0        0        0     1391 2024-02-27 14:57:08.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.236714 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/inference/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:23:35.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/inference/__init__.py
+-rw-rw-rw-   0        0        0     4223 2024-04-08 12:25:45.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/inference/inference.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.195756 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.196756 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.195756 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/logP/
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.283046 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/logP/all_molecules(without_angle_feature)_without_outliers/
+-rw-rw-rw-   0        0        0 18512739 2024-02-08 20:47:01.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/logP/all_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_3_AutoML_2_20240208_214951
+-rw-rw-rw-   0        0        0 15154680 2024-02-08 19:40:31.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/logP/all_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_5_AutoML_1_20240208_212954
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.197757 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.325037 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/acid_molecules(without_angle_feature)_without_outliers/
+-rw-rw-rw-   0        0        0  1745159 2024-02-13 09:22:56.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/acid_molecules(without_angle_feature)_without_outliers/DeepLearning_grid_2_AutoML_4_20240213_102321_model_43
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.334953 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/amine_molecules(without_angle_feature)_without_outliers/
+-rw-rw-rw-   0        0        0 18114821 2024-02-13 08:22:55.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/amine_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_5_AutoML_3_20240213_92029
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.403107 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:23:35.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/__init__.py
+-rw-rw-rw-   0        0        0    47437 2024-02-28 09:51:32.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/features.py
+-rw-rw-rw-   0        0        0     2740 2024-04-08 12:25:45.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/h2o_service.py
+-rw-rw-rw-   0        0        0     3810 2024-03-26 14:38:23.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/molecule_2d_features_service.py
+-rw-rw-rw-   0        0        0    44368 2024-04-08 12:25:45.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/molecule_3d_features_service.py
+-rw-rw-rw-   0        0        0     2391 2024-02-28 09:50:08.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/mordred_features_service.py
+-rw-rw-rw-   0        0        0     6057 2024-03-05 13:15:07.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/utils.py
+-rw-rw-rw-   0        0        0     5960 2024-03-05 14:32:34.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/utils_logP.py
+-rw-rw-rw-   0        0        0     3022 2024-03-05 14:32:30.000000 fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/utils_pKa.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:03:34.219608 fluoriclogppka-0.2.1/fluoriclogppka.egg-info/
+-rw-rw-rw-   0        0        0      597 2024-04-08 13:03:32.000000 fluoriclogppka-0.2.1/fluoriclogppka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1754 2024-04-08 13:03:32.000000 fluoriclogppka-0.2.1/fluoriclogppka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 13:03:32.000000 fluoriclogppka-0.2.1/fluoriclogppka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      299 2024-04-08 13:03:32.000000 fluoriclogppka-0.2.1/fluoriclogppka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 13:03:32.000000 fluoriclogppka-0.2.1/fluoriclogppka.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-08 13:03:34.409106 fluoriclogppka-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2024-04-08 13:01:33.000000 fluoriclogppka-0.2.1/setup.py
```

### Comparing `fluoriclogppka-0.2.0/LICENSE.txt` & `fluoriclogppka-0.2.1/LICENSE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT License
-Copyright (c) 2018 YOUR NAME
+Copyright (c) 2024 blackthorn.ai
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 The above copyright notice and this permission notice shall be included in all
```

### Comparing `fluoriclogppka-0.2.0/PKG-INFO` & `fluoriclogppka-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fluoriclogppka
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tool for pKa, logP prediction
 Home-page: https://github.com/blackthorn-ai/fluoricLogPpKa
-Download-URL: https://github.com/blackthorn-ai/fluoricLogPpKa/dist/fluoriclogppka-0.2.0.tar.gz
+Download-URL: https://github.com/blackthorn-ai/fluoricLogPpKa/dist/fluoriclogppka-0.2.1.tar.gz
 Author: Blackthorn.ai
 License: MIT
 Keywords: pKa,logP,tool
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fluoriclogppka-0.2.0/README.md` & `fluoriclogppka-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/data/pKa_Prediction_Starting_data_2024.01.25.csv` & `fluoriclogppka-0.2.1/fluoriclogppka/data/pKa_Prediction_Starting_data_2024.01.25.csv`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/constants.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import os
 from enum import Enum
+
 import numpy as np
 
 class Target(Enum):
     pKa = 'pKa'
     logP = 'logP'
 
 class Identificator(Enum):
@@ -12,24 +14,26 @@
 
 LOGP_FEATURES = ['f_freedom', 'PPSA5', 'mol_num_cycles', 'nFRing', 'nF', 'identificator',
                  'mol_weight', 'dipole_moment', 'nHRing', 'nO', 'PBF', 'nC', 'nARing',
                  'cis/trans', 'PNSA5', 'FPSA3', 'mol_volume', 'RPCS', 'GeomShapeIndex',
                  'WPSA5', 'TASA', 'f_to_fg', 'avg_atoms_in_cycle', 'nFHRing',
                  'chirality']
 
-LOGP_MODEL_PATH = r'fluoriclogppka\ml_part\models_weights\h2o_models\logP\all_molecules(without_angle_feature)_without_outliers\StackedEnsemble_BestOfFamily_3_AutoML_2_20240208_214951'
+MODELS_PATH = os.path.join('fluoriclogppka', 'ml_part', 'models_weights', 'h2o_models')
+
+LOGP_MODEL_PATH = os.path.join(MODELS_PATH, 'logP', 'all_molecules(without_angle_feature)_without_outliers', 'StackedEnsemble_BestOfFamily_3_AutoML_2_20240208_214951')
 
 PKA_FEATURES = ['RPCS', 'PBF', 'mol_weight', 'dipole_moment', 'PPSA5',
                 'avg_atoms_in_cycle', 'nHRing', 'cis/trans', 'FPSA3', 'nF', 'chirality',
                 'sasa', 'PNSA5', 'GeomShapeIndex', 'TASA', 'mol_num_cycles',
                 'f_freedom', 'nFRing', 'identificator', 'nO', 'nARing', 'nC', 'nFHRing',
                 'f_to_fg']
 
-PKA_AMINE_MODEL_PATH = r'fluoriclogppka\ml_part\models_weights\h2o_models\pKa\amine_molecules(without_angle_feature)_without_outliers\StackedEnsemble_BestOfFamily_5_AutoML_3_20240213_92029'
-PKA_ACID_MODEL_PATH = r'fluoriclogppka\ml_part\models_weights\h2o_models\pKa\acid_molecules(without_angle_feature)_without_outliers\DeepLearning_grid_2_AutoML_4_20240213_102321_model_43'
+PKA_AMINE_MODEL_PATH = os.path.join(MODELS_PATH, 'pKa', 'amine_molecules(without_angle_feature)_without_outliers', 'StackedEnsemble_BestOfFamily_5_AutoML_3_20240213_92029')
+PKA_ACID_MODEL_PATH = os.path.join(MODELS_PATH, 'pKa', 'acid_molecules(without_angle_feature)_without_outliers', 'DeepLearning_grid_2_AutoML_4_20240213_102321_model_43')
 
 FUNCTIONAL_GROUP_TO_SMILES = {
             "CF3": "CC(F)(F)F", 
             "CH2F": "CCF", 
             "gem-CF2": "C(F)(F)", 
             "CHF2": "CC(F)(F)",
             "CHF": "CF",
@@ -97,8 +101,8 @@
     "CCF2CCCCCOOH": ["FC(CCCCC(O)=O)(F)C", "FC1(F)CCCC1C(O)=O"],
     "CCF2CCCCCCOOH": ["FC(CCCCCC(O)=O)(F)C", "FC1(F)CCCCC1C(O)=O"],
     "CCFHCCOOH": ["FC(CC(O)=O)([H])C"],
     "CCFHCCCOOH": ["FC(CCC(O)=O)([H])C"],
     "CCFHCCCCOOH": ["FC(CCCC(O)=O)([H])C"],
     "CCFHCCCCCOOH": ["FC(CCCCC(O)=O)([H])C"],
     "CCFHCCCCCCOOH": ["FC(CCCCCC(O)=O)([H])C"]
-}
+}
```

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/data_preparation/smiles_to_features.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/data_preparation/smiles_to_features.py`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/exceptions.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/inference/inference.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/inference/inference.py`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/logP/all_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_3_AutoML_2_20240208_214951` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/logP/all_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_3_AutoML_2_20240208_214951`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/logP/all_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_5_AutoML_1_20240208_212954` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/logP/all_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_5_AutoML_1_20240208_212954`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/acid_molecules(without_angle_feature)_without_outliers/DeepLearning_grid_2_AutoML_4_20240213_102321_model_43` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/acid_molecules(without_angle_feature)_without_outliers/DeepLearning_grid_2_AutoML_4_20240213_102321_model_43`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/amine_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_5_AutoML_3_20240213_92029` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/models_weights/h2o_models/pKa/amine_molecules(without_angle_feature)_without_outliers/StackedEnsemble_BestOfFamily_5_AutoML_3_20240213_92029`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/features.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/features.py`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/h2o_service.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/h2o_service.py`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/molecule_2d_features_service.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/molecule_2d_features_service.py`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/molecule_3d_features_service.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/molecule_3d_features_service.py`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/mordred_features_service.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/mordred_features_service.py`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/utils.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/utils.py`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/utils_logP.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/utils_logP.py`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka/ml_part/services/utils_pKa.py` & `fluoriclogppka-0.2.1/fluoriclogppka/ml_part/services/utils_pKa.py`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka.egg-info/PKG-INFO` & `fluoriclogppka-0.2.1/fluoriclogppka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fluoriclogppka
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tool for pKa, logP prediction
 Home-page: https://github.com/blackthorn-ai/fluoricLogPpKa
-Download-URL: https://github.com/blackthorn-ai/fluoricLogPpKa/dist/fluoriclogppka-0.2.0.tar.gz
+Download-URL: https://github.com/blackthorn-ai/fluoricLogPpKa/dist/fluoriclogppka-0.2.1.tar.gz
 Author: Blackthorn.ai
 License: MIT
 Keywords: pKa,logP,tool
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fluoriclogppka-0.2.0/fluoriclogppka.egg-info/SOURCES.txt` & `fluoriclogppka-0.2.1/fluoriclogppka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluoriclogppka-0.2.0/setup.py` & `fluoriclogppka-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'fluoriclogppka',
   packages = find_packages(), 
   include_package_data = True,
 
-  version = '0.2.0',
+  version = '0.2.1',
   license = 'MIT',
   description = 'Tool for pKa, logP prediction',
   author = 'Blackthorn.ai',
   url = 'https://github.com/blackthorn-ai/fluoricLogPpKa',
-  download_url = 'https://github.com/blackthorn-ai/fluoricLogPpKa/dist/fluoriclogppka-0.2.0.tar.gz',
+  download_url = 'https://github.com/blackthorn-ai/fluoricLogPpKa/dist/fluoriclogppka-0.2.1.tar.gz',
   keywords = ['pKa', 'logP', 'tool'],
   
   install_requires=[ 
           'certifi==2024.2.2',
           'charset-normalizer==3.3.2',
           'future==1.0.0',
           'h2o==3.44.0.3',
```

