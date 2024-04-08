# Comparing `tmp/hbv-1.4.0.tar.gz` & `tmp/hbv-1.4.1.tar.gz`

## Comparing `hbv-1.4.0.tar` & `hbv-1.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 hbv-1.4.0/Dockerfile
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hbv-1.4.0/MANIFEST.in
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hbv-1.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    36937 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/Forcing.txt
--rw-r--r--   0        0        0   524964 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/Forward model.ipynb
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/HBV_config.json
--rw-r--r--   0        0        0    43177 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/HBV_forcing.nc
--rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/Q_m_out_ref.txt
--rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/model_layout.png
--rw-r--r--   0        0        0    20165 2020-02-02 00:00:00.000000 hbv-1.4.0/src/HBV/HBV_bmi.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hbv-1.4.0/src/HBV/__init__.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 hbv-1.4.0/src/HBV/utils.py
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 hbv-1.4.0/LICENSE.txt
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 hbv-1.4.0/README.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 hbv-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 hbv-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 hbv-1.4.1/Dockerfile
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hbv-1.4.1/MANIFEST.in
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hbv-1.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    36937 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/Forcing.txt
+-rw-r--r--   0        0        0   525026 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/Forward model.ipynb
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/HBV_config.json
+-rw-r--r--   0        0        0    43177 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/HBV_forcing.nc
+-rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/Q_m_out_ref.txt
+-rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/model_layout.png
+-rw-r--r--   0        0        0    20165 2020-02-02 00:00:00.000000 hbv-1.4.1/src/HBV/HBV_bmi.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hbv-1.4.1/src/HBV/__init__.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 hbv-1.4.1/src/HBV/utils.py
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 hbv-1.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 hbv-1.4.1/README.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 hbv-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 hbv-1.4.1/PKG-INFO
```

### Comparing `hbv-1.4.0/Dockerfile` & `hbv-1.4.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `hbv-1.4.0/.github/workflows/python-publish.yml` & `hbv-1.4.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hbv-1.4.0/docs/Forcing.txt` & `hbv-1.4.1/docs/Forcing.txt`

 * *Files identical despite different names*

### Comparing `hbv-1.4.0/docs/Forward model.ipynb` & `hbv-1.4.1/docs/Forward model.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999683277027027%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'Shows how model is implemented step by step **without** "*

 * *            "a BMI<br>\\n'), (2, '**And now snow models as implemented in 1.4.0.**')], delete: "*

 * *            '[1]}}}'}*

```diff
@@ -2,15 +2,16 @@
     "cells": [
         {
             "cell_type": "markdown",
             "id": "1cd4a22b-283b-42b5-9b41-c6839654d253",
             "metadata": {},
             "source": [
                 "# NOTEBOOK FOR REFERENCE ONLY!\n",
-                "Shows how model is implemented step by step **without** a BMI"
+                "Shows how model is implemented step by step **without** a BMI<br>\n",
+                "**And now snow models as implemented in 1.4.0.**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "48595997-9cae-43b9-94d5-319c6ee5d4c2",
             "metadata": {},
```

### Comparing `hbv-1.4.0/docs/HBV_forcing.nc` & `hbv-1.4.1/docs/HBV_forcing.nc`

 * *Files identical despite different names*

### Comparing `hbv-1.4.0/docs/Q_m_out_ref.txt` & `hbv-1.4.1/docs/Q_m_out_ref.txt`

 * *Files identical despite different names*

### Comparing `hbv-1.4.0/docs/model_layout.png` & `hbv-1.4.1/docs/model_layout.png`

 * *Files identical despite different names*

### Comparing `hbv-1.4.0/src/HBV/HBV_bmi.py` & `hbv-1.4.1/src/HBV/HBV_bmi.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                             "Q_tot_dt": self.Q_tot_dt,
                             "Q": self.Q,
                             }
 
     def updating_obj_from_dict_var(self) -> None:
         """Function which inverts the dictionary above & sets objects correctly"""
         param_names = ["Imax", "Ce", "Sumax", "Beta", "Pmax", "Tlag", "Kf", "Ks", "FM"]
-        stor_names = ["Si", "Su", "Sf", "Ss", "SP"]
+        stor_names = ["Si", "Su", "Sf", "Ss", "Sp"]
         self.set_pars([self.dict_var_obj[par] for par in param_names])
         self.set_storage([self.dict_var_obj[stor] for stor in stor_names])
 
     def weight_function(self):
         """Generates weights for convolution using generates a weibull weight function"""
 
         n_max = int(np.ceil(self.T_lag))
```

### Comparing `hbv-1.4.0/src/HBV/utils.py` & `hbv-1.4.1/src/HBV/utils.py`

 * *Files identical despite different names*

### Comparing `hbv-1.4.0/LICENSE.txt` & `hbv-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hbv-1.4.0/README.md` & `hbv-1.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Basic Model Interface (BMI) HBV model intended for use with [eWaterCycle](https://github.com/eWaterCycle). See said repo for installation instructions. 
 
 HBV (Hydrologiska Byråns Vattenbalansavdelning) is a conceptual hydrological model. For more information on its history, see this [paper](https://hess.copernicus.org/articles/26/1371/2022/).
 
 This current implementation is _without_ a snow reservoir, as shown below.
 (_Image from the course ENVM1502 - river basin Hydrology (Markus Hrachowitz)._) 
-![model_layout.png](https://raw.githubusercontent.com/Daafip/HBV-bmi/main/model_layout.png)
+![model_layout.png](https://raw.githubusercontent.com/Daafip/HBV-bmi/main/docs/model_layout.png)
 
 Actual eWatercycle model wrapper can be found on [GitHub](https://github.com/Daafip/ewatercycle-hbv) with accompanying [documentation](https://ewatercycle-hbv.readthedocs.io/en/latest/)
 
 Feel free to fork/duplicate this repo and publish your own (better) version.
 
 
 ## separate use
@@ -44,15 +44,17 @@
 - added support for updating memory vector on the fly for Data assimilation.
 #### V1.1.1
 - bug fix in `T_lag` value: can now only be set an integer larger than 1: otherwise makes no physical sense
 - bug fix where wrong types were given, warning messages cleaned up and code attempted to be made more readable
 ### V1.2.0
 - pretty big issue with setting values fixed - won't affect most use but will cause issues for Data Assimilation
 - use opportunity to name all HBV packages/naming/images to 1.2.0 
-### V1.3.0
+## V1.3.0
 - Change `Q_m` to `Q` in order to better integrate data assimilation & just makes more sense. 
-## v1.3.1
+### v1.3.1
 - Fix bug in time indexing
-## v1.3.2
+### v1.3.2
 - typo in update updating_dict_var_obj: was getting values wrong 
 ## V1.4.0
-- adding snow reservoir
+- adding snow reservoir
+### V1.4.1
+- bug fix in naming of values
```

### Comparing `hbv-1.4.0/pyproject.toml` & `hbv-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "HBV"
 description = "Dev version for a HBV hydrological model using BMI for eWaterCycle."
 readme = "README.md"
 license = "Apache-2.0"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name = "David Haasnoot", email = "davidhaasnoot@gmail.com" },
 ]
 
 # Include here only the dependencies for the BMI Model
 # This is used to run the BmiModel inside the container
 dependencies = [
```

### Comparing `hbv-1.4.0/PKG-INFO` & `hbv-1.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: HBV
-Version: 1.4.0
+Version: 1.4.1
 Summary: Dev version for a HBV hydrological model using BMI for eWaterCycle.
 Author-email: David Haasnoot <davidhaasnoot@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Requires-Dist: bmipy
 Requires-Dist: netcdf4
 Requires-Dist: numpy
@@ -18,15 +18,15 @@
 
 Basic Model Interface (BMI) HBV model intended for use with [eWaterCycle](https://github.com/eWaterCycle). See said repo for installation instructions. 
 
 HBV (Hydrologiska Byråns Vattenbalansavdelning) is a conceptual hydrological model. For more information on its history, see this [paper](https://hess.copernicus.org/articles/26/1371/2022/).
 
 This current implementation is _without_ a snow reservoir, as shown below.
 (_Image from the course ENVM1502 - river basin Hydrology (Markus Hrachowitz)._) 
-![model_layout.png](https://raw.githubusercontent.com/Daafip/HBV-bmi/main/model_layout.png)
+![model_layout.png](https://raw.githubusercontent.com/Daafip/HBV-bmi/main/docs/model_layout.png)
 
 Actual eWatercycle model wrapper can be found on [GitHub](https://github.com/Daafip/ewatercycle-hbv) with accompanying [documentation](https://ewatercycle-hbv.readthedocs.io/en/latest/)
 
 Feel free to fork/duplicate this repo and publish your own (better) version.
 
 
 ## separate use
@@ -58,15 +58,17 @@
 - added support for updating memory vector on the fly for Data assimilation.
 #### V1.1.1
 - bug fix in `T_lag` value: can now only be set an integer larger than 1: otherwise makes no physical sense
 - bug fix where wrong types were given, warning messages cleaned up and code attempted to be made more readable
 ### V1.2.0
 - pretty big issue with setting values fixed - won't affect most use but will cause issues for Data Assimilation
 - use opportunity to name all HBV packages/naming/images to 1.2.0 
-### V1.3.0
+## V1.3.0
 - Change `Q_m` to `Q` in order to better integrate data assimilation & just makes more sense. 
-## v1.3.1
+### v1.3.1
 - Fix bug in time indexing
-## v1.3.2
+### v1.3.2
 - typo in update updating_dict_var_obj: was getting values wrong 
 ## V1.4.0
-- adding snow reservoir
+- adding snow reservoir
+### V1.4.1
+- bug fix in naming of values
```

