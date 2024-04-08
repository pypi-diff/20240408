# Comparing `tmp/ewatercycle_hbv-1.6.1.tar.gz` & `tmp/ewatercycle_hbv-1.7.0.tar.gz`

## Comparing `ewatercycle_hbv-1.6.1.tar` & `ewatercycle_hbv-1.7.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/CHANGELOG.md
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/plugin_guide.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/.idea/.gitignore
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/.idea/ewatercycle-hbv-numpy.iml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/.idea/misc.xml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/docs/Makefile
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/docs/conf.py
--rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/docs/example_model_run_HBV.ipynb
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/docs/make.bat
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/docs/model.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/docs/requirements.txt
--rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/docs/_images/model_layout.png
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/docs/_static/README.rst
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/src/ewatercycle_HBV/__init__.py
--rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/src/ewatercycle_HBV/forcing.py
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/src/ewatercycle_HBV/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/tests/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/tests/test_forcing.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/tests/test_model.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/LICENSE.txt
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/README.md
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/plugin_guide.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/.idea/.gitignore
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/.idea/ewatercycle-hbv-numpy.iml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/docs/Makefile
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/docs/conf.py
+-rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/docs/example_model_run_HBV.ipynb
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/docs/make.bat
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/docs/model.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/docs/requirements.txt
+-rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/docs/_images/model_layout.png
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/docs/_static/README.rst
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/src/ewatercycle_HBV/__init__.py
+-rw-r--r--   0        0        0    15185 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/src/ewatercycle_HBV/forcing.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/src/ewatercycle_HBV/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/tests/test_forcing.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/tests/test_model.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/README.md
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.0/PKG-INFO
```

### Comparing `ewatercycle_hbv-1.6.1/CHANGELOG.md` & `ewatercycle_hbv-1.7.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,8 +31,10 @@
 #### 1.5.1
 - fix bug/implementation error with time indexing, docker image version 1.3.1
 #### 1.5.2
 - typo in bmi implementation: docker image 1.3.2
 ### 1.6.0
   - now compatible with ewatercycle V2.1 `LumpedMakkinkForcing` which generates evaporation from era5/CMIP.
 #### 1.6.1
-  - bug fix occuring when loading makkink data
+  - bug fix occuring when loading makkink data
+### 1.7.0
+  - new version of HBV bmi which adds snow
```

### Comparing `ewatercycle_hbv-1.6.1/plugin_guide.md` & `ewatercycle_hbv-1.7.0/plugin_guide.md`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/.github/workflows/python-publish.yml` & `ewatercycle_hbv-1.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/.github/workflows/test.yml` & `ewatercycle_hbv-1.7.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/docs/Makefile` & `ewatercycle_hbv-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/docs/conf.py` & `ewatercycle_hbv-1.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/docs/example_model_run_HBV.ipynb` & `ewatercycle_hbv-1.7.0/docs/example_model_run_HBV.ipynb`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/docs/index.rst` & `ewatercycle_hbv-1.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/docs/make.bat` & `ewatercycle_hbv-1.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/docs/model.rst` & `ewatercycle_hbv-1.7.0/docs/model.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/docs/_images/model_layout.png` & `ewatercycle_hbv-1.7.0/docs/_images/model_layout.png`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/docs/_static/README.rst` & `ewatercycle_hbv-1.7.0/docs/_static/README.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/src/ewatercycle_HBV/forcing.py` & `ewatercycle_hbv-1.7.0/src/ewatercycle_HBV/forcing.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 import xarray as xr
 import numpy as np
 
 from ewatercycle.base.forcing import DefaultForcing
 
 
 RENAME_CAMELS = {'total_precipitation_sum':'pr',
-                      'potential_evaporation_sum':'pev',
-                      'streamflow':'Q'}
+                 'potential_evaporation_sum':'pev',
+                 'streamflow':'Q',
+                 'temperature_2m_min':'tasmin',
+                 'temperature_2m_max':'tasmax',
+                 }
 
-REQUIRED_PARAMS = ["pr", "pev"]
+REQUIRED_PARAMS = ["pr", "pev", "tasmean"]
 class HBVForcing(DefaultForcing):
     """Container for HBV forcing data.
 
     Args:
         camels_file: .txt file that contains CAMELS forcing from https://hess.copernicus.org/articles/21/5293/2017/
         pr: Path to a NetCDF (.nc) file containing precipitation - ensure yourself that these already match start_time & end time
         pev: Path to a NetCDF (.nc) file containing potential evaporation
@@ -67,14 +70,15 @@
     """
 
     # either a forcing file is supplied
     camels_file: Optional[str] = ".txt"
     # or pr and pev are supplied seperately - can also be the same dataset
     pr: Optional[str] = ".nc"
     pev: Optional[str] = ".nc"
+    tasmean: Optional[str] = ".nc"
     alpha: Optional[float] = 1.26 # varies per catchment, mostly 1.26?
     test_data_bool: bool = False # allows to use self.from_test_txt()
 
     def camels_txt_defined(self):
         """test whether user defined forcing file, used converting text forcing file to netcdf"""
         if len(self.camels_file) > 4:
             return True
@@ -107,24 +111,29 @@
         fn = self.directory / self.camels_file
         forcing = np.loadtxt(fn, delimiter="	")
         names = ["year", "month", "day", "pr","Q", "pev"]
         df_in = pd.DataFrame(forcing, columns=names)
         df_in.index = df_in.apply(lambda x: pd.Timestamp(f'{int(x.year)}-{int(x.month)}-{int(x.day)}'), axis=1)
         df_in = df_in.drop(columns=["year", "month", "day"])
         df_in.index.name = "time"
+        # test data has no snow but let's add in synthetic temperatures to ensure there's no snow:
+        df_in['tasmean'] = 25
+
         # TODO use netcdf-cf conventions
         ds = xr.Dataset(data_vars=df_in,
                         attrs={
                             "title": "HBV forcing data",
                             "history": "Created by ewatercycle_HBV.forcing.HBVForcing.to_xarray()",
                                 },
                         )
         ds, ds_name = self.crop_ds(ds, "test")
         self.pev = ds_name
         self.pr = ds_name
+        self.tasmean = ds_name
+
         return ds
 
     def from_camels_txt(self) -> xr.Dataset:
         """Load forcing data from a txt file into an xarray dataset.
 
         Requirements:
             Must be in the same format as the CAMELS dataset:
@@ -179,15 +188,16 @@
                         'tmax': 'tasmax',
                         'tmin': 'tasmin'}
         df.rename(columns=rename_dict2, inplace=True)
 
         # add attributes
         attrs = {"title": "HBV forcing data",
                  "history": "Created by ewatercycle_HBV.forcing.HBVForcing.from_camels_txt()",
-                 "units": "daylight(s), precipitation(mm/day), mean radiation(W/m2), snow water equivalen(mm), temperature max(C), temperature min(C), vapour pressure(Pa)", }
+                 "units": "daylight(s), precipitation(mm/day), mean radiation(W/m2), snow water equivalen(mm), temperature max(C), temperature min(C), temperature mean(c),vapour pressure(Pa)",
+                 }
 
         # add the data lines with catchment characteristics to the description
         attrs.update(data)
 
         ds = xr.Dataset(data_vars=df,
                         attrs=attrs,
                         )
@@ -196,53 +206,62 @@
                              ds["tasmin"].values,
                              ds["tasmax"].values,
                              ds["time.dayofyear"].values,
                              self.alpha,
                              ds.attrs['elevation(m)'],
                              ds.attrs['lat']
                              )
+        ds['tasmean'] = (ds["tasmin"] + ds["tasmax"]) / 2
         ds, ds_name= self.crop_ds(ds, "CAMELS")
         self.pev = ds_name
         self.pr = ds_name
+        self.tasmean = ds_name
         return ds
 
     def from_external_source(self):
         """Runs checks on externally provided forcing"""
         if None in [self.directory, self.pr, self.pev]:
             self.file_not_found_error()
 
         # often same file
-        if self.pr == self.pev:
+        if self.pr == self.pev == self.tasmean:
             ds = xr.open_dataset(self.directory / self.pr)
 
+            # make compatile with CARAVAN data style:
             if sum([key in ds.data_vars for key in RENAME_CAMELS.keys()]) == len(RENAME_CAMELS):
                 ds = ds.rename(RENAME_CAMELS)
                 ds = ds.rename_dims({'date': 'time'})
                 ds = ds.rename({'date': 'time'})
+                ds['tasmean'] = (ds["tasmin"] + ds["tasmax"]) / 2
 
             ds, ds_name = self.crop_ds(ds, "external")
             self.pev = ds_name
             self.pr = ds_name
+            self.tasmean = ds_name
             return ds
 
         else:
             # but can also seperate
             ds_pr = xr.open_dataset(self.directory / self.pr)
             ds_pev = xr.open_dataset(self.directory / self.pev)
-            combined_data_vars = list(ds_pr.data_vars) + list(ds_pev.data_vars)
+            ds_tasmean = xr.open_dataset(self.directory / self.tasmean)
+            combined_data_vars = list(ds_pr.data_vars) + list(ds_pev.data_vars) + list(ds_tasmean.data_vars)
             if sum([param in combined_data_vars for param in REQUIRED_PARAMS]) != len(REQUIRED_PARAMS):
                 raise UserWarning(f"Supplied NetCDF files must contain {REQUIRED_PARAMS} respectively")
 
             ds_pr, ds_name_pr = self.crop_ds(ds_pr, "external")
             self.pr = ds_name_pr
 
             ds_pev, ds_name_pev = self.crop_ds(ds_pev, "external")
             self.pev = ds_name_pev
 
-            return ds_pr, ds_pev
+            ds_tasmean, ds_name_tasmean = self.crop_ds(ds_tasmean, "external")
+            self.tasmean = ds_name_tasmean
+
+            return ds_pr, ds_pev, ds_tasmean
 
     def crop_ds(self, ds: xr.Dataset, name: str):
         start = np.datetime64(self.start_time)
         end = np.datetime64(self.end_time)
         ds = ds.isel(time=(ds['time'].values >= start) & (ds['time'].values <= end))
 
         time = str(datetime.now())[:-10].replace(":", "_")
```

### Comparing `ewatercycle_hbv-1.6.1/src/ewatercycle_HBV/model.py` & `ewatercycle_hbv-1.7.0/src/ewatercycle_HBV/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
     forcing: LumpedMakkinkForcing|HBVForcing|GenericLumpedForcing  # The model requires forcing.
     parameter_set: None  # The model has no parameter set.
 
     _config: dict = {
         "precipitation_file": "",
         "potential_evaporation_file": "",
+        "mean_temperature_file": "",
         "parameters": "",
         "initial_storage": "",
                         }
 
     def _make_cfg_file(self, **kwargs) -> Path:
         """Write model configuration file."""
 
@@ -64,14 +65,17 @@
             self._config["precipitation_file"] = str(
                 self.forcing.directory / self.forcing.pr
             )
 
             self._config["potential_evaporation_file"] = str(
                 self.forcing.directory / self.forcing.pev
             )
+            self._config["mean_temperature_file"] = str(
+                self.forcing.directory / self.forcing.tasmean)
+
 
         elif type(self.forcing).__name__ == 'GenericLumpedForcing':
                 raise UserWarning("Generic Lumped Forcing does not provide potential evaporation, which this model needs")
 
         elif type(self.forcing).__name__ == 'LumpedMakkinkForcing':
             temporary_pev_file = self.forcing.directory / self.forcing.filenames['evspsblpot'].replace('evspsblpot',
                                                                                                        'pev_mm')
@@ -91,31 +95,35 @@
                 attributes = ds['pr'].attrs
                 attributes['units'] = 'mm'
                 ds['pr'] = ds['pr'] * 86400
                 ds['pr'].attrs = attributes
                 ds.to_netcdf(temporary_pr_file)
                 ds.close()
 
+            temporary_tasmean_file = self.forcing.directory / self.forcing.filenames['tas'].replace('tas', 'tasmean')
+            if not temporary_tasmean_file.is_file():
+                ds = xr.open_dataset(self.forcing.directory / self.forcing.filenames['tas'])
+                attributes = ds['tas'].attrs
+                ds['tasmean'] = ds['tas']
+                if ds['tasmean'].mean().values > 200: # adjust for kelvin units
+                    ds['tasmean'] -= 273.15
+                ds['tasmean'].attrs = attributes
+                ds.to_netcdf(temporary_tasmean_file)
+                ds.close()
+
             self._config["precipitation_file"] = str(
                 temporary_pr_file
             )
             self._config["potential_evaporation_file"] = str(
                 temporary_pev_file
             )
 
-        ## possibly add later for snow?
-        # self._config["temperature_file"] = str(
-        #     self.forcing.directory / self.forcing.tas
-        # )
-        # self._config["temperature_min_file"] = str(
-        #     self.forcing.directory / self.forcing.tasmin
-        # )
-        # self._config["temperature_max_file"] = str(
-        #     self.forcing.directory / self.forcing.tasmax
-        # )
+            self._config["mean_temperature_file"] = str(
+                temporary_tasmean_file
+            )
 
         for kwarg in kwargs:  # Write any kwargs to the config. - doesn't overwrite config?
             self._config[kwarg] = kwargs[kwarg]
 
         config_file = self._cfg_dir / "HBV_config.json"
 
         with config_file.open(mode="w") as f:
@@ -149,27 +157,30 @@
             T_lag (d): is the lag time between water falling and reaching the river.
 
             Kf (-): the fast flow is modelled as a linear reservoir thus a fraction
                     of the volume stored leaves to the river 𝑄𝑓=𝐾𝑓∗𝑆𝑓
 
             Ks (−): Similarly the slow flow is also modelled as 𝑄𝑆=𝐾𝑠∗𝑆𝑆.
 
+            FM (mm/deg/d): Melt Factor: mm of melt per deg per day
+
         """
         pars: dict[str, Any] = dict(zip(HBV_PARAMS, self._config["parameters"].split(',')))
         return pars.items()
 
     @property
     def states(self) -> ItemsView[str, Any]:
         """List the (initial!) states for this model.
 
         Exposed HBV states:
             Si (mm): Interception storage, water stored in leaves
             Su (mm): Unsaturated rootzone storage, water stored accessible to plants
             Sf (mm): Fastflow storage, moving Fast through the soil - preferential flow paths, upper level
             Ss (mm): Groundwater storage, moving Slowly through the soil - deeper grounds water.
+            Sp (mm): SnowPack Storage, amount of snow stored
 
         """
         pars: dict[str, Any] = dict(zip(HBV_STATES, self._config["initial_storage"].split(',')))
         return pars.items()
 
 
     def finalize(self) -> None:
@@ -203,19 +214,19 @@
                 self.unlink()
 
         elif type(self.forcing).__name__ == 'LumpedMakkinkForcing':
             # we created a temporary file so let's unlink that
             self.unlink()
 
     def unlink(self):
-        for file in ["potential_evaporation_file", "precipitation_file"]:
+        for file in ["potential_evaporation_file", "precipitation_file","mean_temperature_file"]:
             path = self.forcing.directory / self._config[file]
             if path.is_file():  # often both with be the same, e.g. with camels data.
                 path.unlink()
             else:
                 pass
 
 class HBV(ContainerizedModel, HBVMethods):
     """The HBV eWaterCycle model, with the Container Registry docker image."""
     bmi_image: ContainerImage = ContainerImage(
-        "ghcr.io/daafip/hbv-bmi-grpc4bmi:v1.3.2"
+        "ghcr.io/daafip/hbv-bmi-grpc4bmi:v1.4.0"
     )
```

### Comparing `ewatercycle_hbv-1.6.1/.gitignore` & `ewatercycle_hbv-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/LICENSE.txt` & `ewatercycle_hbv-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/README.md` & `ewatercycle_hbv-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.6.1/pyproject.toml` & `ewatercycle_hbv-1.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = "src/ewatercycle_HBV/__init__.py"
 
 [project]
 name = "ewatercycle-HBV"
 description = "Implementation of HBV for eWaterCycle"
 readme = "README.md"
 license = "Apache-2.0"
-version = "1.6.1"
+version = "1.7.0"
 authors = [
   { name = "David Haasnoot", email = "davidhaasnoot@gmail.com" },
 ]
 keywords = ["ewatercycle", "hydrology"]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
```

### Comparing `ewatercycle_hbv-1.6.1/PKG-INFO` & `ewatercycle_hbv-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ewatercycle-HBV
-Version: 1.6.1
+Version: 1.7.0
 Summary: Implementation of HBV for eWaterCycle
 Project-URL: homepage, https://github.com/Daafip/ewatercycle-hbv
 Author-email: David Haasnoot <davidhaasnoot@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Keywords: ewatercycle,hydrology
 Classifier: Intended Audience :: Developers
```

