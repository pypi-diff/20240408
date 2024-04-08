# Comparing `tmp/lasertram-0.0.8.tar.gz` & `tmp/lasertram-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasertram-0.0.8.tar", last modified: Wed Oct 25 23:57:26 2023, max compression
+gzip compressed data, was "lasertram-0.0.9.tar", last modified: Fri Oct 27 00:52:26 2023, max compression
```

## Comparing `lasertram-0.0.8.tar` & `lasertram-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 23:57:26.385955 lasertram-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-10-25 23:57:10.000000 lasertram-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-10-25 23:57:26.385955 lasertram-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-10-25 23:57:10.000000 lasertram-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 23:57:26.381955 lasertram-0.0.8/lasertram/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 23:57:10.000000 lasertram-0.0.8/lasertram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44782 2023-10-25 23:57:10.000000 lasertram-0.0.8/lasertram/lasertram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 23:57:26.385955 lasertram-0.0.8/lasertram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-10-25 23:57:26.000000 lasertram-0.0.8/lasertram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-10-25 23:57:26.000000 lasertram-0.0.8/lasertram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 23:57:26.000000 lasertram-0.0.8/lasertram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-10-25 23:57:26.000000 lasertram-0.0.8/lasertram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-25 23:57:26.000000 lasertram-0.0.8/lasertram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-25 23:57:10.000000 lasertram-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-10-25 23:57:26.385955 lasertram-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 23:57:26.385955 lasertram-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2023-10-25 23:57:10.000000 lasertram-0.0.8/tests/test_lasertram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 00:52:26.044353 lasertram-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-10-27 00:52:13.000000 lasertram-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-10-27 00:52:26.044353 lasertram-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2023-10-27 00:52:13.000000 lasertram-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 00:52:26.040353 lasertram-0.0.9/lasertram/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 00:52:13.000000 lasertram-0.0.9/lasertram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44536 2023-10-27 00:52:13.000000 lasertram-0.0.9/lasertram/lasertram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 00:52:26.044353 lasertram-0.0.9/lasertram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-10-27 00:52:26.000000 lasertram-0.0.9/lasertram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2023-10-27 00:52:26.000000 lasertram-0.0.9/lasertram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 00:52:26.000000 lasertram-0.0.9/lasertram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-10-27 00:52:26.000000 lasertram-0.0.9/lasertram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-27 00:52:26.000000 lasertram-0.0.9/lasertram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-27 00:52:13.000000 lasertram-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2023-10-27 00:52:26.044353 lasertram-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 00:52:26.044353 lasertram-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    33094 2023-10-27 00:52:13.000000 lasertram-0.0.9/tests/test_lasertram.py
```

### Comparing `lasertram-0.0.8/LICENSE` & `lasertram-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lasertram-0.0.8/PKG-INFO` & `lasertram-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasertram
-Version: 0.0.8
+Version: 0.0.9
 Summary: For processing LA-ICP-MS data
 Home-page: https://github.com/jlubbersgeo/lasertram
 Author: Jordan Lubbers
 Author-email: jelubber@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lasertram-0.0.8/README.md` & `lasertram-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lasertram-0.0.8/lasertram/lasertram.py` & `lasertram-0.0.9/lasertram/lasertram.py`

 * *Files 3% similar despite different names*

```diff
@@ -480,15 +480,15 @@
         where each row represents data for a standard reference material.
         The first column should be named "Standard". All other columns are
         for different elemental concentrations.Standard names must be exact
         names found in GEOREM: http://georem.mpch-mainz.gwdg.de/sample_query_pref.asp
         """
 
         self.standards_data = df.set_index("Standard")
-        self.database_standards = self.standards_data.index.unique()
+        self.database_standards = self.standards_data.index.unique().to_list()
         # Get a list of all of the elements supported in the published standard datasheet
         # Get a second list for the same elements but their corresponding uncertainty columns
         self.standard_elements = [
             analyte
             for analyte in self.standards_data.columns.tolist()
             if not ("_std" in analyte)
         ]
@@ -499,19 +499,22 @@
     def get_data(self, df):
         """load in output from `LaserTRAM` for calculation of concentrations
 
         Args:
             df (pandas DataFrame): a 2D pandas DataFrame representing numerous concatenated calls to `LaserTRAM.make_output_report()`
 
         """
+        # check if first row is nan (output from GUI does this).
+        # If so, remove it
+        df = df[df.iloc[:, 0].isna() == False]
 
         data = df.set_index("Spot")
         data.insert(loc=1, column="index", value=np.arange(1, len(data) + 1))
 
-        self.spots = data.index.unique().tolist()
+        self.spots = data.index.unique().dropna().tolist()
 
         # Check for potential calibration standards. This will let us know what our options
         # are for choosing calibration standards by looking for spots that have the same string
         # as the standard spreadsheet
 
         stds_column = [
             [std for std in self.database_standards if std in spot]
@@ -570,15 +573,15 @@
     def set_calibration_standard(self, std):
         """Assign which standard reference material will be the calibration
         standard for calculating concentrations.
 
         Args:
             std (str): name of standard reference material (e.g., `NIST-612`,`BCR-2G`)
         """
-        self.calibration_standard = std
+        self.calibration_std = std
 
         self.calibration_std_data = self.data.loc[std, :]
         # Calibration standard information
         # mean
         self.calibration_std_means = self.calibration_std_data.loc[
             :, self.analytes
         ].mean()
@@ -628,34 +631,34 @@
                 ).astype(np.float64)
                 # x = np.cumsum(np.diff(x))
                 # x = np.insert(x, 0, 0).astype(np.float64)
 
             else:
                 x = self.calibration_std_data["index"]
 
-            y = self.calibration_std_data[self.analytes[j]].astype("float64")
+            y = self.calibration_std_data.loc[:, self.analytes[j]].astype("float64")
 
             X = sm.add_constant(x)
             # Note the difference in argument order
             model = sm.OLS(y, X).fit()
             # now generate predictions
             ypred = model.predict(X)
 
             # calc rmse
             RMSE = rmse(y, ypred)
 
             calib_std_rmses.append(RMSE)
 
             if model.params.shape[0] < 2:
-                calib_std_slopes.append(model.params[0])
+                calib_std_slopes.append(model.params.loc["x1"])
                 calib_std_intercepts.append(0)
 
             else:
-                calib_std_slopes.append(model.params[1])
-                calib_std_intercepts.append(model.params[0])
+                calib_std_slopes.append(model.params.loc["x1"])
+                calib_std_intercepts.append(model.params.loc["const"])
 
             # new stuff
             # confidence limit 99%
 
             # f value stuff
 
             fvalue = model.fvalue
@@ -667,15 +670,15 @@
             if (f_pvalue < pval) and (fvalue > fcrit):
                 drift = "True"
                 drift_check.append(drift)
             else:
                 drift = "False"
                 drift_check.append(drift)
 
-        self.calibration_standard_stats = pd.DataFrame(
+        self.calibration_std_stats = pd.DataFrame(
             {
                 "drift_correct": drift_check,
                 "f_pval": f_pvals,
                 "f_value": f_vals,
                 "f_crit_value": f_crits,
                 "rmse": calib_std_rmses,
                 "slope": calib_std_slopes,
@@ -702,26 +705,26 @@
             nomass = re.split("(\d+)", self.analytes[i])[2]
             # make it a list
             myanalytes_nomass.append(nomass)
 
             # if our element is in the list of standard elements take the ratio
             if nomass in self.standard_elements:
                 std_conc_ratios.append(
-                    self.standards_data.loc[self.calibration_standard, nomass]
+                    self.standards_data.loc[self.calibration_std, nomass]
                     / self.standards_data.loc[
-                        self.calibration_standard,
+                        self.calibration_std,
                         re.split(
                             "(\d+)", self.calibration_std_data["norm"].unique()[0]
                         )[2],
                     ]
                 )
 
         # make our list an array for easier math going forward
         # std_conc_ratios = pd.DataFrame(np.array(std_conc_ratios)[np.newaxis,:],columns = myanalytes)
-        self.calibration_standard_conc_ratios = np.array(std_conc_ratios)
+        self.calibration_std_conc_ratios = np.array(std_conc_ratios)
 
     def set_internal_standard_concentrations(
         self,
         spots=None,
         concentrations=None,
         uncertainties=None,
     ):
@@ -738,16 +741,16 @@
             uncertainties (array-like): values representing the internal standard relative uncertainty in percent. Must be the same shape as `spots`.
         """
         if spots is None:
             spots = (self.data["Spot"],)
             concentrations = (np.full(self.data["Spot"].shape[0], 10),)
             uncertainties = (np.full(self.data["Spot"].shape[0], 1),)
 
-        self.data["internal_std_comp"] = 10
-        self.data["internal_std_rel_unc"] = 1
+        self.data["internal_std_comp"] = 10.0
+        self.data["internal_std_rel_unc"] = 1.0
         df = self.data.reset_index().set_index("Spot")
 
         for spot, concentration, uncertainty in zip(
             spots, concentrations, uncertainties
         ):
             df.loc[spot, "internal_std_comp"] = concentration
             df.loc[spot, "internal_std_rel_unc"] = uncertainty
@@ -760,41 +763,41 @@
         Calculates the concentration and uncertainty of all spots in the experiment
         using the user specified calibration standard and internal standard
         concentrations/uncertainties.
 
         """
 
         secondary_standards = self.potential_calibration_standards.copy()
-        secondary_standards.remove(self.calibration_standard)
+        secondary_standards.remove(self.calibration_std)
         self.secondary_standards = secondary_standards
         secondary_standards_concentrations_list = []
         unknown_concentrations_list = []
 
         for sample in secondary_standards:
             Cn_u = self.standards_data.loc[
                 sample,
                 re.split(
                     "(\d+)",
                     self.calibration_std_data["norm"].unique()[0],
                 )[2],
             ]
-            Cin_std = self.calibration_standard_conc_ratios
-            Ni_std = self.calibration_standard_stats["mean"][self.analytes]
+            Cin_std = self.calibration_std_conc_ratios
+            Ni_std = self.calibration_std_stats["mean"][self.analytes]
             Ni_u = self.data.loc[sample, self.analytes]
 
             concentrations = Cn_u * (Cin_std / Ni_std) * Ni_u
 
             drift_concentrations_list = []
 
             for j, analyte, slope, intercept, drift in zip(
                 range(len(self.analytes)),
                 self.analytes,
-                self.calibration_standard_stats["slope"],
-                self.calibration_standard_stats["intercept"],
-                self.calibration_standard_stats["drift_correct"],
+                self.calibration_std_stats["slope"],
+                self.calibration_std_stats["intercept"],
+                self.calibration_std_stats["drift_correct"],
             ):
                 if "True" in drift:
                     if "timestamp" in self.data.columns.tolist():
                         frac = (
                             slope
                             * np.array(
                                 [
@@ -846,30 +849,30 @@
 
         ###############################
         for sample in self.samples_nostandards:
             Cn_u = oxide_to_ppm(
                 self.data.loc[sample, "internal_std_comp"],
                 self.data.loc[sample, "norm"].unique()[0],
             ).to_numpy()
-            Cin_std = self.calibration_standard_conc_ratios
-            Ni_std = self.calibration_standard_stats["mean"][self.analytes].to_numpy()
+            Cin_std = self.calibration_std_conc_ratios
+            Ni_std = self.calibration_std_stats["mean"][self.analytes].to_numpy()
             Ni_u = self.data.loc[sample, self.analytes].to_numpy()
 
             concentrations = pd.DataFrame(
                 Cn_u[:, np.newaxis] * (Cin_std / Ni_std) * Ni_u, columns=self.analytes
             )
 
             drift_concentrations_list = []
 
             for j, analyte, slope, intercept, drift in zip(
                 range(len(self.analytes)),
                 self.analytes,
-                self.calibration_standard_stats["slope"],
-                self.calibration_standard_stats["intercept"],
-                self.calibration_standard_stats["drift_correct"],
+                self.calibration_std_stats["slope"],
+                self.calibration_std_stats["intercept"],
+                self.calibration_std_stats["drift_correct"],
             ):
                 if "True" in drift:
                     if "timestamp" in self.data.columns.tolist():
                         frac = (
                             slope
                             * np.array(
                                 [
@@ -972,23 +975,23 @@
         myuncertainties = [analyte + "_se" for analyte in self.analytes]
         srm_rel_uncertainties_list = []
         unk_rel_uncertainties_list = []
         # use RMSE of regression for elements where drift correction is applied rather than the standard error
         # of the mean of all the calibration standard normalized ratios
         rse_i_std = []
         for analyte in self.analytes:
-            if "True" in self.calibration_standard_stats.loc[analyte, "drift_correct"]:
+            if "True" in self.calibration_std_stats.loc[analyte, "drift_correct"]:
                 rse_i_std.append(
                     100
-                    * self.calibration_standard_stats.loc[analyte, "rmse"]
-                    / self.calibration_standard_stats.loc[analyte, "mean"]
+                    * self.calibration_std_stats.loc[analyte, "rmse"]
+                    / self.calibration_std_stats.loc[analyte, "mean"]
                 )
             else:
                 rse_i_std.append(
-                    self.calibration_standard_stats.loc[analyte, "percent_std_err"]
+                    self.calibration_std_stats.loc[analyte, "percent_std_err"]
                 )
 
         rse_i_std = np.array(rse_i_std)
 
         for sample in self.secondary_standards:
             # concentration of internal standard in unknown uncertainties
             int_std_element = re.split(
@@ -997,36 +1000,32 @@
             t1 = (
                 self.standards_data.loc[sample, f"{int_std_element}_std"]
                 / self.standards_data.loc[sample, f"{int_std_element}"]
             ) ** 2
 
             # concentration of internal standard in calibration standard uncertainties
             t2 = (
-                self.standards_data.loc[
-                    self.calibration_standard, f"{int_std_element}_std"
-                ]
-                / self.standards_data.loc[
-                    self.calibration_standard, f"{int_std_element}"
-                ]
+                self.standards_data.loc[self.calibration_std, f"{int_std_element}_std"]
+                / self.standards_data.loc[self.calibration_std, f"{int_std_element}"]
             ) ** 2
 
             # concentration of each analyte in calibration standard uncertainties
             std_conc_stds = []
             for i in range(len(self.analytes)):
                 # strip the atomic number from our analyte data
                 nomass = re.split("(\d+)", self.analytes[i])[2]
 
                 # if our element is in the list of standard elements take the ratio
                 if nomass in self.standard_elements:
                     std_conc_stds.append(
                         (
                             self.standards_data.loc[
-                                self.calibration_standard, f"{nomass}_std"
+                                self.calibration_std, f"{nomass}_std"
                             ]
-                            / self.standards_data.loc[self.calibration_standard, nomass]
+                            / self.standards_data.loc[self.calibration_std, nomass]
                         )
                         ** 2
                     )
 
             std_conc_stds = np.array(std_conc_stds)
 
             # Overall uncertainties
@@ -1069,36 +1068,32 @@
             # concentration of internal standard in unknown uncertainties
             t1 = (self.data.loc[sample, "internal_std_rel_unc"] / 100) ** 2
             t1 = np.array(t1)
             t1 = t1[:, np.newaxis]
 
             # concentration of internal standard in calibration standard uncertainties
             t2 = (
-                self.standards_data.loc[
-                    self.calibration_standard, f"{int_std_element}_std"
-                ]
-                / self.standards_data.loc[
-                    self.calibration_standard, f"{int_std_element}"
-                ]
+                self.standards_data.loc[self.calibration_std, f"{int_std_element}_std"]
+                / self.standards_data.loc[self.calibration_std, f"{int_std_element}"]
             ) ** 2
 
             # concentration of each analyte in calibration standard uncertainties
             std_conc_stds = []
             for i in range(len(self.analytes)):
                 # strip the atomic number from our analyte data
                 nomass = re.split("(\d+)", self.analytes[i])[2]
 
                 # if our element is in the list of standard elements take the ratio
                 if nomass in self.standard_elements:
                     std_conc_stds.append(
                         (
                             self.standards_data.loc[
-                                self.calibration_standard, f"{nomass}_std"
+                                self.calibration_std, f"{nomass}_std"
                             ]
-                            / self.standards_data.loc[self.calibration_standard, nomass]
+                            / self.standards_data.loc[self.calibration_std, nomass]
                         )
                         ** 2
                     )
 
             std_conc_stds = np.array(std_conc_stds)
 
             # Overall uncertainties
@@ -1115,27 +1110,24 @@
                     ).astype(np.float64)
                 )
             )
             rel_uncertainty.columns = myuncertainties
             unk_rel_uncertainties_list.append(rel_uncertainty)
 
         unk_rel_uncertainties = pd.concat(unk_rel_uncertainties_list)
-        overall_uncertainties = (
-            unk_rel_uncertainties.values
-            * self.unknown_concentrations.loc[:, self.analytes].values
-        )
-        srm_uncertainties = pd.DataFrame(
+
+        unknown_uncertainties = pd.DataFrame(
             unk_rel_uncertainties.values
             * self.unknown_concentrations.loc[:, self.analytes].values,
             columns=myuncertainties,
             index=self.unknown_concentrations.index,
         )
 
         self.unknown_concentrations = pd.concat(
-            [self.unknown_concentrations, srm_uncertainties], axis="columns"
+            [self.unknown_concentrations, unknown_uncertainties], axis="columns"
         )
 
     # make an accuracy checking function
     # need to use analytes no mass to check SRM vals
     def get_secondary_standard_accuracies(self):
         """
         calculate the accuracy of each secondary standard where accuracy is 100 * measured / accepted value
```

### Comparing `lasertram-0.0.8/lasertram.egg-info/PKG-INFO` & `lasertram-0.0.9/lasertram.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasertram
-Version: 0.0.8
+Version: 0.0.9
 Summary: For processing LA-ICP-MS data
 Home-page: https://github.com/jlubbersgeo/lasertram
 Author: Jordan Lubbers
 Author-email: jelubber@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lasertram-0.0.8/setup.cfg` & `lasertram-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lasertram
-version = 0.0.8
+version = 0.0.9
 author = Jordan Lubbers
 author_email = jelubber@gmail.com
 description = For processing LA-ICP-MS data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jlubbersgeo/lasertram
 classifiers =
```

