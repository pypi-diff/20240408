# Comparing `tmp/hbv-1.3.1.tar.gz` & `tmp/hbv-1.4.0.tar.gz`

## Comparing `hbv-1.3.1.tar` & `hbv-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,16 @@
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 hbv-1.3.1/Dockerfile
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 hbv-1.3.1/MANIFEST.in
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 hbv-1.3.1/.idea/.gitignore
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 hbv-1.3.1/.idea/.name
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hbv-1.3.1/.idea/HBV BMI.iml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hbv-1.3.1/.idea/misc.xml
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 hbv-1.3.1/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hbv-1.3.1/.idea/vcs.xml
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 hbv-1.3.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hbv-1.3.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    36937 2020-02-02 00:00:00.000000 hbv-1.3.1/.ipynb_checkpoints/Forcing-checkpoint.txt
--rw-r--r--   0        0        0   524964 2020-02-02 00:00:00.000000 hbv-1.3.1/.ipynb_checkpoints/Forward model-checkpoint.ipynb
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 hbv-1.3.1/.ipynb_checkpoints/using BMI server-checkpoint.ipynb
--rw-r--r--   0        0        0    36937 2020-02-02 00:00:00.000000 hbv-1.3.1/docs/Forcing.txt
--rw-r--r--   0        0        0   524964 2020-02-02 00:00:00.000000 hbv-1.3.1/docs/Forward model.ipynb
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbv-1.3.1/docs/HBV_config.json
--rw-r--r--   0        0        0    43177 2020-02-02 00:00:00.000000 hbv-1.3.1/docs/HBV_forcing.nc
--rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 hbv-1.3.1/docs/Q_m_out_ref.txt
--rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 hbv-1.3.1/docs/model_layout.png
--rw-r--r--   0        0        0    19664 2020-02-02 00:00:00.000000 hbv-1.3.1/src/HBV/HBV_bmi.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hbv-1.3.1/src/HBV/__init__.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 hbv-1.3.1/src/HBV/utils.py
--rw-r--r--   0        0        0    16995 2020-02-02 00:00:00.000000 hbv-1.3.1/src/HBV/.ipynb_checkpoints/HBV_bmi-checkpoint.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 hbv-1.3.1/.gitignore
--rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 hbv-1.3.1/LICENSE.txt
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 hbv-1.3.1/README.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 hbv-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 hbv-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 hbv-1.4.0/Dockerfile
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hbv-1.4.0/MANIFEST.in
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hbv-1.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    36937 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/Forcing.txt
+-rw-r--r--   0        0        0   524964 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/Forward model.ipynb
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/HBV_config.json
+-rw-r--r--   0        0        0    43177 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/HBV_forcing.nc
+-rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/Q_m_out_ref.txt
+-rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 hbv-1.4.0/docs/model_layout.png
+-rw-r--r--   0        0        0    20165 2020-02-02 00:00:00.000000 hbv-1.4.0/src/HBV/HBV_bmi.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hbv-1.4.0/src/HBV/__init__.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 hbv-1.4.0/src/HBV/utils.py
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 hbv-1.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 hbv-1.4.0/README.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 hbv-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 hbv-1.4.0/PKG-INFO
```

### Comparing `hbv-1.3.1/Dockerfile` & `hbv-1.4.0/Dockerfile`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# Based on https://github.com/eWaterCycle/leakybucket-bmi/blob/main/Dockerfile
-# Base container for a BMI model written in Python
-#
-# Activates a default conda base environment with micromamba. While it may not
-# always be necessary, many hydrological models may at some point want to
-# install conda dependencies, which can be a struggle. This image should provide
-# a good starting point.
-#
-# For details on the base image, see
-# https://github.com/mamba-org/micromamba-docker
-#
-#
-# To build the image, run
-#
-#   docker build --tag hbv-np-grpc4bmi:v0.0.1 . 
-#
-# If you use podman, you may need to add `--format docker`
-#
-#   docker build --format docker --tag leakybucket-grpc4bmi:v0.0.1 .
-#
-# To talk to the model from outside the container, use grpc4bmi client
-#
-#   from grpc4bmi.bmi_client_docker import BmiClientDocker
-#   model = BmiClientDocker('leakybucket-grpc4bmi:v0.0.1', work_dir='/tmp', delay=1)
-#
-# To debug the container, you can override the grpc4bmi command
-#
-#   docker run --tty --interactive leakybucket-grpc4bmi:v0.0.1 bash
-#
-# This will spawn a new bash terminal running inside the docker container
-
-FROM mambaorg/micromamba:1.3.1
-MAINTAINER David Haasnoot daafips@gmail.com
-
-# Here you can point to the source repository of this Dockerfile:
-LABEL org.opencontainers.image.source="https://github.com/Daafip/HBV-bmi-numpy"
-
-# Install Python + additional conda-dependencies,
-# Here I added cartopy as an example
-RUN micromamba install -y -n base -c conda-forge python=3.10 cartopy git && \
-    micromamba clean --all --yes
-
-# Make sure the conda environment is activated for the remaining build
-# instructions below
-ARG MAMBA_DOCKERFILE_ACTIVATE=1  # (otherwise python will not be found)
-
-# Install HBV.HBV_bmi
-COPY . /opt/HBV
-RUN pip install /opt/HBV/
-
-RUN pip install grpc4bmi==0.4.0
-
-
-
-# Default command should be to run GRPC4BMI server
-# Don't override micromamba's entrypoint as that activates conda!
-# CMD run-bmi-server --name "HBV.HBV_bmi.HBV" --port 55555 --debug
-#ENTRYPOINT ["run-bmi-server", "--name", "HBV.HBV_bmi.HBV",--path,"/opt/mymodeldir"]
+# Based on https://github.com/eWaterCycle/leakybucket-bmi/blob/main/Dockerfile
+# Base container for a BMI model written in Python
+#
+# Activates a default conda base environment with micromamba. While it may not
+# always be necessary, many hydrological models may at some point want to
+# install conda dependencies, which can be a struggle. This image should provide
+# a good starting point.
+#
+# For details on the base image, see
+# https://github.com/mamba-org/micromamba-docker
+#
+#
+# To build the image, run
+#
+#   docker build --tag hbv-np-grpc4bmi:v0.0.1 . 
+#
+# If you use podman, you may need to add `--format docker`
+#
+#   docker build --format docker --tag leakybucket-grpc4bmi:v0.0.1 .
+#
+# To talk to the model from outside the container, use grpc4bmi client
+#
+#   from grpc4bmi.bmi_client_docker import BmiClientDocker
+#   model = BmiClientDocker('leakybucket-grpc4bmi:v0.0.1', work_dir='/tmp', delay=1)
+#
+# To debug the container, you can override the grpc4bmi command
+#
+#   docker run --tty --interactive leakybucket-grpc4bmi:v0.0.1 bash
+#
+# This will spawn a new bash terminal running inside the docker container
+
+FROM mambaorg/micromamba:1.3.1
+MAINTAINER David Haasnoot daafips@gmail.com
+
+# Here you can point to the source repository of this Dockerfile:
+LABEL org.opencontainers.image.source="https://github.com/Daafip/HBV-bmi"
+
+# Install Python + additional conda-dependencies,
+# Here I added cartopy as an example
+RUN micromamba install -y -n base -c conda-forge python=3.10 cartopy git && \
+    micromamba clean --all --yes
+
+# Make sure the conda environment is activated for the remaining build
+# instructions below
+ARG MAMBA_DOCKERFILE_ACTIVATE=1  # (otherwise python will not be found)
+
+# Install HBV.HBV_bmi
+COPY . /opt/HBV
+RUN pip install /opt/HBV/
+
+RUN pip install grpc4bmi==0.4.0
+
+
+
+# Default command should be to run GRPC4BMI server
+# Don't override micromamba's entrypoint as that activates conda!
+# CMD run-bmi-server --name "HBV.HBV_bmi.HBV" --port 55555 --debug
+#ENTRYPOINT ["run-bmi-server", "--name", "HBV.HBV_bmi.HBV",--path,"/opt/mymodeldir"]
 CMD run-bmi-server --name "HBV.HBV_bmi.HBV" --port 55555 --debug
```

### Comparing `hbv-1.3.1/.ipynb_checkpoints/Forcing-checkpoint.txt` & `hbv-1.4.0/docs/Forcing.txt`

 * *Files identical despite different names*

### Comparing `hbv-1.3.1/.ipynb_checkpoints/Forward model-checkpoint.ipynb` & `hbv-1.4.0/docs/Forward model.ipynb`

 * *Files identical despite different names*

### Comparing `hbv-1.3.1/docs/HBV_forcing.nc` & `hbv-1.4.0/docs/HBV_forcing.nc`

 * *Files identical despite different names*

### Comparing `hbv-1.3.1/docs/Q_m_out_ref.txt` & `hbv-1.4.0/docs/Q_m_out_ref.txt`

 * *Files identical despite different names*

### Comparing `hbv-1.3.1/docs/model_layout.png` & `hbv-1.4.0/docs/model_layout.png`

 * *Files identical despite different names*

### Comparing `hbv-1.3.1/src/HBV/HBV_bmi.py` & `hbv-1.4.0/src/HBV/HBV_bmi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,35 @@
 from bmipy import Bmi
 from typing import Any, Tuple
 from HBV import utils
 import numpy as np
 import warnings
 
+DICT_VAR_UNITS = {"Imax": "mm",
+                  "Ce": "-",
+                  "Sumax": "mm",
+                  "Beta": "-",
+                  "Pmax": "mm",
+                  "Tlag": "d",
+                  "Kf": "-",
+                  "Ks": "-",
+                  "FM": "mm/deg/d",
+                  "Si": "mm",
+                  "Su": "mm",
+                  "Sf": "mm",
+                  "Ss": "mm",
+                  "Sp": "mm",
+                  "M_dt": "mm/d",
+                  "Ei_dt": "mm/d",
+                  "Ea_dt": "mm/d",
+                  "Qs_dt": "mm/d",
+                  "Qf_dt": "mm/d",
+                  "Q_tot_dt": "mm/d",
+                  "Q": "mm/d"}
+
 
 class HBV(Bmi):
     """HBV model wrapped in a BMI interface."""
 
     def initialize(self, config_file: str) -> None:
         """"Based on LeakyBucketBMI simple implementation of HBV without snow component
             Requires atleast:
@@ -20,163 +42,127 @@
         """
         # open json files containing data
         self.config: dict[str, Any] = utils.read_config(config_file)
 
         # store forcing & obs
         self.P = utils.load_var(self.config["precipitation_file"], "pr")
 
-        # add Tas, Tmin and Tmax support for snow component ??!
         self.EP = utils.load_var(self.config["potential_evaporation_file"], "pev")
 
+        self.Tmean = utils.load_var(self.config["mean_temperature_file"], "tasmean")
+
         # set up times
-        self.Ts = self.P['time'].astype("datetime64[s]")
-        """:31: UserWarning: Converting non-nanosecond precision datetime values to nanosecond precision. 
-        This behavior can eventually be relaxed in xarray, as it is an artifact from pandas which is now beginning 
-        to support non-nanosecond precision values. 
-        This warning is caused by passing non-nanosecond np.datetime64 or np.timedelta64 values to the DataArray or 
-        Variable constructor; it can be silenced by converting the values to nanosecond precision ahead of time."""
-        self.end_timestep = len(self.Ts.values)
+        self.time = self.P['time'].astype("datetime64[s]")
+        self.end_timestep = len(self.time.values)
         self.current_timestep = 0
 
         # time step size in seconds (to be able to do unit conversions) - change here to days
         self.dt = (
-            self.Ts.values[1] - self.Ts.values[0]
-        ) / np.timedelta64(1, "s") / 24 / 3600
+                          self.time.values[1] - self.time.values[0]
+                  ) / np.timedelta64(1, "s") / 24 / 3600
 
         # define parameters 
         self.set_pars(np.array(self.config['parameters'].split(','), dtype=np.float64))
 
         # add memory vector for tlag & run weights function
         self.memory_vector_lag = self.set_empty_memory_vector_lag()
 
         # define storage & flow terms, flows 0, storages initialised 
-        s_in = np.array(self.config['initial_storage'].split(','),dtype=np.float64)
+        s_in = np.array(self.config['initial_storage'].split(','), dtype=np.float64)
         self.set_storage(s_in)
 
-        # set other flows for initial step 
-        self.Ei_dt     = 0       # interception evaporation
-        self.Ea_dt     = 0       # actual evaportation
-        self.Qs_dt     = 0       # slow flow
-        self.Qf_dt     = 0       # fast flow
-        self.Q_tot_dt  = 0       # total flow
-        self.Q       = 0       # Final model prediction
-
-        # stores the units for variables
-        self.dict_var_units = {
-                                "Imax":"mm",
-                                "Ce": "-",
-                                "Sumax": "mm",
-                                "Beta": "-",
-                                "Pmax": "mm",
-                                "Tlag": "d",
-                                "Kf": "-",
-                                "Ks": "-",
-                                "Si": "mm",
-                                "Su": "mm",
-                                "Sf": "mm",
-                                "Ss": "mm",
-                                "Ei_dt": "mm/d",
-                                "Ea_dt": "mm/d",
-                                "Qs_dt": "mm/d",
-                                "Qf_dt": "mm/d",
-                                "Q_tot_dt": "mm/d",
-                                "Q": "mm/d"}
-        # stores corresponding objects for variables
+        # set other flows for initial step
+        self.M_dt = 0  # snow melt
+        self.Ei_dt = 0  # interception evaporation
+        self.Ea_dt = 0  # actual evaportation
+        self.Qs_dt = 0  # slow flow
+        self.Qf_dt = 0  # fast flow
+        self.Q_tot_dt = 0  # total flow
+        self.Q = 0  # Final model prediction
 
-    def updating_dict_var_obj(self) -> None:
-        """Function which makes getting the objects more readable-  but adds more boiler plate.."""
-        self.dict_var_obj = {
-                             "Imax": self.I_max,
-                             "Ce": self.Ce,
-                             "Sumax": self.Su_max,
-                             "Beta": self.beta,
-                             "Pmax": self.P_max,
-                             "Tlag": self.T_lag,
-                             "Kf": self.Kf,
-                             "Ks": self.Ks,
-                             "Si": self.Si,
-                             "Su": self.Su,
-                             "Sf": self.Sf,
-                             "Ss": self.Ss,
-                             "Ei_dt": self.Ei_dt,
-                             "Ea_dt": self.Ei_dt,
-                             "Qs_dt": self.Qs_dt,
-                             "Qf_dt": self.Qf_dt,
-                             "Q_tot_dt": self.Q_tot_dt,
-                             "Q": self.Q,
-                             }
-    def updating_obj_from_dict_var(self) -> None:
-        """Function which inverts the dictionary above & sets objects correctly"""
-        param_names = ["Imax","Ce", "Sumax", "Beta", "Pmax", "Tlag", "Kf", "Ks"]
-        stor_names = ["Si", "Su", "Sf", "Ss"]
-        self.set_pars([self.dict_var_obj[par] for par in param_names])
-        self.set_storage([self.dict_var_obj[stor] for stor in stor_names])
+        # other constant for Snow:
+        self.Tt = -0.5  # Threshold temperature set for now. Can be between -1 to 1
 
     def set_pars(self, par) -> None:
-        self.I_max  = par[0]                # maximum interception
-        self.Ce     = par[1]                # Ea = Su / (sumax * Ce) * Ep
-        self.Su_max = par[2]                # ''
-        self.beta   = par[3]                # Cr = (su/sumax)**beta
-        self.P_max  = par[4]                # Qus = Pmax * (Su/Sumax)
-        self.T_lag  = self.set_tlag(par[5]) # used in triangular transfer function
-        self.Kf     = par[6]                # Qf=kf*sf
-        self.Ks     = par[7]                # Qs=Ks*
+        self.I_max = par[0]  # maximum interception
+        self.Ce = par[1]  # Ea = Su / (sumax * Ce) * Ep
+        self.Su_max = par[2]  # ''
+        self.beta = par[3]  # Cr = (su/sumax)**beta
+        self.P_max = par[4]  # Qus = Pmax * (Su/Sumax)
+        self.T_lag = self.set_tlag(par[5])  # used in triangular transfer function
+        self.Kf = par[6]  # Qf=kf*sf
+        self.Ks = par[7]  # Qs=Ks*
+        self.FM = par[8]  # degree day factor: Melt FM * (Tmean-Tt)
 
     def set_storage(self, stor) -> None:
-        self.Si = stor[0] # Interception storage
-        self.Su = stor[1] # Unsaturated Rootzone Storage
-        self.Sf = stor[2] # Fastflow storage
-        self.Ss = stor[3] # Groundwater storage
-
+        self.Si = stor[0]  # Interception storage
+        self.Su = stor[1]  # Unsaturated Rootzone Storage
+        self.Sf = stor[2]  # Fastflow storage
+        self.Ss = stor[3]  # Groundwater storage
+        self.Sp = stor[4]  # SnowPack storage
 
     def update(self) -> None:
         """ Updates model one timestep
 
         Old documentation:
             Function to run the update part of one timestep of the HBV model
-            par: array/list containing 8 parameters: Imax,  Ce,  Sumax, beta,  Pmax,  T_lag,   Kf,   Ks (floats)
-            s_in: array/list containing 4 storage terms which are input to the timestep: Si,  Su, Sf, Ss (floats)
-            storage_terms: list of arrays which store: Si, Su, Sf, Ss, Ei_dt, Ea_dt, Qs_dt_lst, Qf_dt_lst, Q_tot_dt
+            par: array/list containing 9 parameters: Imax,  Ce,  Sumax, beta,  Pmax,  T_lag,   Kf,   Ks, Fm (floats)
+            s_in: array/list containing 5 storage terms which are input to the timestep: Si,  Su, Sf, Ss,Sp (floats)
+            storage_terms: list of arrays which store: Si, Su, Sf, Ss,Sp, Ei_dt, Ea_dt, Qs_dt_lst, Qf_dt_lst, Q_tot_dt
             step_n - nth step which formard model takes: used to determin which Precipitaion & evaporation to use
         """
         if self.current_timestep < self.end_timestep:
-            self.P_dt  = self.P.isel(time=self.current_timestep).to_numpy() * self.dt
+            self.P_dt = self.P.isel(time=self.current_timestep).to_numpy() * self.dt
             self.Ep_dt = self.EP.isel(time=self.current_timestep).to_numpy() * self.dt
+            self.Tmean_i = self.Tmean.isel(time=self.current_timestep).to_numpy() * self.dt
+
+            # split P into rain and snow:
+            if self.Tmean_i < self.Tt:
+                self.Pr = 0  # if snowing, no rainfall
+                self.Ps = self.P_dt  # all precip goes into snow
+                self.M_dt = 0  # too cold to meld
+                self.Sp += self.Ps
+            else:
+                self.Pr = self.P_dt  # if not snowing, all rainfall
+                self.Ps = 0  # No snow
+                self.M_dt = min(self.Sp / self.dt, self.FM * (self.Tmean_i - self.Tt))  # melt factor * diff in temp
+                self.Sp -= self.M_dt  # remove melt from snowpack content
+                self.Pr += self.M_dt  # add it to `rainfall`: snow melt can also be intercepted
 
             # Interception Reservoir
-            if self.P_dt > 0:
+            if self.Pr > 0:
                 # if there is rain, no evap
-                self.Si    = self.Si + self.P_dt               # increase the storage
+                self.Si = self.Si + self.Pr  # increase the storage
                 self.Pe_dt = max((self.Si - self.I_max) / self.dt, 0)
-                self.Si    = self.Si - self.Pe_dt
-                self.Ei_dt = 0                          # if rainfall, evaporation = 0 as too moist
+                self.Si = self.Si - self.Pe_dt
+                self.Ei_dt = 0  # if rainfall, evaporation = 0 as too moist
             else:
                 # Evaporation only when there is no rainfall
-                self.Pe_dt = 0                      # nothing flows in so must be 0
-                self.Ei_dt = min(self.Ep_dt, self.Si / self.dt) # evaporation limited by storage
-                self.Si    = self.Si - self.Ei_dt
+                self.Pe_dt = 0  # nothing flows in so must be 0
+                self.Ei_dt = min(self.Ep_dt, self.Si / self.dt)  # evaporation limited by storage
+                self.Si = self.Si - self.Ei_dt
 
             # split flow into Unsaturated Reservoir and Fast flow
             if self.Pe_dt > 0:
-                cr       = (self.Su / self.Su_max)**self.beta
-                Qiu_dt   = (1 - cr ) * self.Pe_dt      # flux from Ir to Ur
-                self.Su  = self.Su + Qiu_dt
-                Quf_dt   = cr  * self.Pe_dt            # flux from Su to Sf
+                cr = (self.Su / self.Su_max) ** self.beta
+                Qiu_dt = (1 - cr) * self.Pe_dt  # flux from Ir to Ur
+                self.Su = self.Su + Qiu_dt
+                Quf_dt = cr * self.Pe_dt  # flux from Su to Sf
             else:
                 Quf_dt = 0
 
             # Transpiration
-            self.Ep_dt = max(0, self.Ep_dt - self.Ei_dt)        # Transpiration
-            self.Ea_dt = self.Ep_dt  * (self.Su / (self.Su_max * self.Ce))
-            self.Ea_dt = min(self.Su, self.Ea_dt)            # limited by water in soil
-            self.Su    = self.Su - self.Ea_dt
+            self.Ep_dt = max(0, self.Ep_dt - self.Ei_dt)  # Transpiration
+            self.Ea_dt = self.Ep_dt * (self.Su / (self.Su_max * self.Ce))
+            self.Ea_dt = min(self.Su, self.Ea_dt)  # limited by water in soil
+            self.Su = self.Su - self.Ea_dt
 
             # Percolation
-            Qus_dt = self.P_max * (self.Su / self.Su_max) * self.dt # Flux from Su to Ss
-            self.Su  = self.Su - Qus_dt
+            Qus_dt = self.P_max * (self.Su / self.Su_max) * self.dt  # Flux from Su to Ss
+            self.Su = self.Su - Qus_dt
 
             # Fast Reservoir
             self.Sf = self.Sf + Quf_dt
             self.Qf_dt = self.dt * self.Kf * self.Sf
             self.Sf = self.Sf - self.Qf_dt
 
             # Slow Reservoir
@@ -189,85 +175,125 @@
             # add time lag to the process - Qm is set here
             self.add_time_lag()
             # self.Q = self.Q_tot_dt
 
             # Advance the model time by one step
             self.current_timestep += 1
 
-    def Weigfun(self):
-        nmax=int(np.ceil(self.T_lag))
-        if nmax==1:
-            Weigths=float(1)
+    def updating_dict_var_obj(self) -> None:
+        """Function which makes getting the objects more readable-  but adds more boiler plate.."""
+        self.dict_var_obj = {
+                            "Imax": self.I_max,
+                            "Ce": self.Ce,
+                            "Sumax": self.Su_max,
+                            "Beta": self.beta,
+                            "Pmax": self.P_max,
+                            "Tlag": self.T_lag,
+                            "Kf": self.Kf,
+                            "Ks": self.Ks,
+                            "FM": self.FM,
+                            "Si": self.Si,
+                            "Su": self.Su,
+                            "Sf": self.Sf,
+                            "Ss": self.Ss,
+                            "Sp": self.Sp,
+                            "M_dt": self.M_dt,
+                            "Ei_dt": self.Ei_dt,
+                            "Ea_dt": self.Ea_dt,
+                            "Qs_dt": self.Qs_dt,
+                            "Qf_dt": self.Qf_dt,
+                            "Q_tot_dt": self.Q_tot_dt,
+                            "Q": self.Q,
+                            }
+
+    def updating_obj_from_dict_var(self) -> None:
+        """Function which inverts the dictionary above & sets objects correctly"""
+        param_names = ["Imax", "Ce", "Sumax", "Beta", "Pmax", "Tlag", "Kf", "Ks", "FM"]
+        stor_names = ["Si", "Su", "Sf", "Ss", "SP"]
+        self.set_pars([self.dict_var_obj[par] for par in param_names])
+        self.set_storage([self.dict_var_obj[stor] for stor in stor_names])
+
+    def weight_function(self):
+        """Generates weights for convolution using generates a weibull weight function"""
+
+        n_max = int(np.ceil(self.T_lag))
+        if n_max == 1:
+            weights = float(1)
         else:
-            Weigths=np.zeros(nmax)
-            th=self.T_lag/2
-            nh=int(np.floor(th))
-            for i in range(0,nh):
-                Weigths[i]=(float(i+1)-0.5)/th
-            i=nh
-
-            Weigths[i]=(1+(float(i+1)-1)/th)*(th-int(np.floor(th)))/2+(1+(self.T_lag-float(i+1))/th)*(int(np.floor(th))+1-th)/2
-            for i in range(nh+1, int(np.floor(self.T_lag))):
-                Weigths[i]=(self.T_lag-float(i+1)+.5)/th
+            weights = np.zeros(n_max)
+            th = self.T_lag / 2
+            nh = int(np.floor(th))
+            for i in range(0, nh):
+                weights[i] = (float(i + 1) - 0.5) / th
+            i = nh
+
+            weights[i] = (1 + (float(i + 1) - 1) / th) * (th - int(np.floor(th))) / 2 + (
+                        1 + (self.T_lag - float(i + 1)) / th) * (int(np.floor(th)) + 1 - th) / 2
+            for i in range(nh + 1, int(np.floor(self.T_lag))):
+                weights[i] = (self.T_lag - float(i + 1) + 0.5) / th
 
-            if self.T_lag>int(np.floor(self.T_lag)):
-                Weigths[int(np.floor(self.T_lag))]=(self.T_lag-int(np.floor(self.T_lag)))**2/(2*th)
+            if self.T_lag > int(np.floor(self.T_lag)):
+                weights[int(np.floor(self.T_lag))] = (self.T_lag - int(np.floor(self.T_lag))) ** 2 / (2 * th)
 
-            Weigths=Weigths/sum(Weigths)
+            weights = weights / sum(weights)
 
-        return Weigths
+        return weights
 
     def add_time_lag(self) -> None:
+        """Adds lag based on weights and discharge"""
         # with support for T_lag =0
         if len(self.memory_vector_lag) > 0:
             # Distribute current Q_tot_dt to memory vector
-            self.memory_vector_lag += self.weights*self.Q_tot_dt
+            self.memory_vector_lag += self.weights * self.Q_tot_dt
 
             # Extract the latest Qm
             self.Q = self.memory_vector_lag[0]
 
             # Make a forecast to the next time step
-            self.memory_vector_lag = np.roll(self.memory_vector_lag,-1)  # This cycles the array [1,2,3,4] becomes [2,3,4,1]
-            self.memory_vector_lag[-1] = 0                              # the next last entry becomes 0 (outside of convolution lag)
+            # This cycles the array [1,2,3,4] becomes [2,3,4,1]
+            self.memory_vector_lag = np.roll(self.memory_vector_lag, -1)
+            # the next last entry becomes 0 (outside of convolution lag)
+            self.memory_vector_lag[-1] = 0
 
     def set_empty_memory_vector_lag(self):
-        self.weights = self.Weigfun() # generates weights using a weibull weight function
+        self.weights = self.weight_function()
         return np.zeros(self.T_lag)
 
     def get_component_name(self) -> str:
         return "HBV"
 
     def get_value(self, var_name: str, dest: np.ndarray) -> np.ndarray:
         # first update the dictionary to match the current values of object
         self.updating_dict_var_obj()
         # handle the memory vector
         if var_name[:len("memory_vector")] == "memory_vector":
             if var_name == "memory_vector":
                 dest[:] = np.array(None)
                 message = "No action undertaken. Please use `set_value(f'memory_vector{n}',src)` where n is the index."
-                warnings.warn(message=message, type=SyntaxWarning)
+                warnings.warn(message, category=SyntaxWarning)
             else:
                 mem_index = int(var_name[len("memory_vector"):])
                 if mem_index < len(self.memory_vector_lag):
                     dest[:] = self.memory_vector_lag[mem_index]
                 else:
-                    raise IndexError(f'{mem_index} is out of range for memory vector size {len(self.memory_vector_lag)}')
+                    raise IndexError(
+                        f'{mem_index} is out of range for memory vector size {len(self.memory_vector_lag)}')
 
             return dest
         # otherwise return the variable from the dictionary
         elif var_name in self.dict_var_obj:
             dest[:] = np.array(self.dict_var_obj[var_name])
             return dest
         else:
             raise ValueError(f"Unknown variable {var_name}")
 
     def get_var_units(self, var_name: str) -> str:
         # look up table
-        if var_name in self.dict_var_units:
-            return self.dict_var_units[var_name]
+        if var_name in DICT_VAR_UNITS:
+            return DICT_VAR_UNITS[var_name]
         else:
             raise ValueError(f"Unknown variable {var_name}")
 
     def set_value(self, var_name: str, src: np.ndarray) -> None:
         # update the dict which maps variables to their current value
         self.updating_dict_var_obj()
         # handle two special case:
@@ -289,70 +315,71 @@
             # set new vector
             self.memory_vector_lag = new_memory_vector
 
         # 2. values in the memory vector must be set manually to work with DA
         elif var_name[:len("memory_vector")] == "memory_vector":
             if var_name == "memory_vector":
                 message = "No action undertaken. Please use `set_value(memory_vector{n},src)` where n is the index."
-                warnings.warn(message=message, type=SyntaxWarning)
+                warnings.warn(message=message, category=SyntaxWarning)
                 pass
             else:
                 mem_index = int(var_name[len("memory_vector"):])
                 if mem_index < len(self.memory_vector_lag):
                     self.memory_vector_lag[mem_index] = src[0]
                 else:
-                    raise IndexError(f'{mem_index} is out of range for memory vector size {len(self.memory_vector_lag)}')
+                    raise IndexError(
+                        f'{mem_index} is out of range for memory vector size {len(self.memory_vector_lag)}')
 
         # all other values can be set here
         elif var_name in self.dict_var_obj:
             self.dict_var_obj[var_name] = src[0]
             self.updating_obj_from_dict_var()
 
         else:
             raise ValueError(f"Unknown variable {var_name}")
 
     # this is a bad way, but oh well
     # first we set the new value in the dictionary
     # this doesn't update the obj...
     def get_output_var_names(self) -> Tuple[str]:
-        return tuple([str(key) for key in self.dict_var_units.keys()])
+        return tuple([str(key) for key in DICT_VAR_UNITS.keys()])
 
     # The BMI has to have some time-related functionality:
     def get_start_time(self) -> float:
         """Return end time in seconds since 1 january 1970."""
-        return get_unixtime(self.Ts.isel(time=0).values) # type: ignore
+        return get_unixtime(self.time.isel(time=0).values)  # type: ignore
 
     def get_end_time(self) -> float:
         """Return end time in seconds since 1 january 1970."""
-        return get_unixtime(self.Ts.isel(time=-1).values) # type: ignore
+        return get_unixtime(self.time.isel(time=-1).values)  # type: ignore
 
     def get_current_time(self) -> float:
         """Return current time in seconds since 1 january 1970."""
         # we get the timestep from the data, but the stopping condition requires it to go one beyond. 
-        return get_unixtime(self.Ts.isel(time=self.current_timestep).values) # type: ignore
+        return get_unixtime(self.time.isel(time=self.current_timestep).values)  # type: ignore
 
     def set_tlag(self, T_lag_in) -> int:
         """Ensures T_lag is an integer of at minimum 1"""
-        T_lag = max(1,int(round(T_lag_in,0)))
+        T_lag = max(1, int(round(T_lag_in, 0)))
         return T_lag
 
     def get_time_step(self) -> float:
-        if len(self.Ts) > 1:
-            return float((self.Ts.values[1] - self.Ts.values[0]) / np.timedelta64(1, "s"))
+        if len(self.time) > 1:
+            return float((self.time.values[1] - self.time.values[0]) / np.timedelta64(1, "s"))
         else:
             message = "No time series defined"
-            warnings.warn(message=message, type=ImportWarning)
+            warnings.warn(message=message, category=ImportWarning)
             return 0.0
 
     def get_time_units(self) -> str:
         return "seconds since 1970-01-01 00:00:00.0 +0000"
 
     # TODO implement setting different timestep?
     def get_value_at_indices(
-        self, name: str, dest: np.ndarray, inds: np.ndarray) -> np.ndarray:
+            self, name: str, dest: np.ndarray, inds: np.ndarray) -> np.ndarray:
         raise NotImplementedError()
 
     # TODO implement
     def set_value_at_indices(self, name: str, inds: np.ndarray, src: np.ndarray) -> None:
         raise NotImplementedError()
 
     def get_var_itemsize(self, name: str) -> int:
@@ -440,14 +467,14 @@
     def get_grid_face_edges(self, grid: int, face_edges: np.ndarray) -> np.ndarray:
         raise NotImplementedError()
 
     def get_grid_face_nodes(self, grid: int, face_nodes: np.ndarray) -> np.ndarray:
         raise NotImplementedError()
 
     def get_grid_nodes_per_face(
-        self, grid: int, nodes_per_face: np.ndarray) -> np.ndarray:
+            self, grid: int, nodes_per_face: np.ndarray) -> np.ndarray:
         raise NotImplementedError()
 
 
 def get_unixtime(Ts: np.datetime64) -> int:
     """Get unix timestamp (seconds since 1 january 1970) from a np.datetime64."""
-    return  np.datetime64(Ts).astype("datetime64[s]").astype("int")
+    return np.datetime64(Ts).astype("datetime64[s]").astype("int")
```

### Comparing `hbv-1.3.1/src/HBV/utils.py` & `hbv-1.4.0/src/HBV/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import xarray as xr
-from pathlib import Path
-import json
-
-
-def read_config(config_file: str) -> dict:
-    with open(config_file) as cfg:
-        config = json.load(cfg)
-    return config
-
-
-def load_var(ncfile: str | Path, varname: str) -> xr.DataArray:
-    """Load the precipitation data file generated by GenericLumpedForcing.
-
-
-    .. code-block:: python
-
-        from ewatercycle.base.forcing import GenericLumpedForcing
-
-        shape = Path("./src/ewatercycle/testing/data/Rhine/Rhine.shp")
-        cmip_dataset = {
-            "dataset": "EC-Earth3",
-            "project": "CMIP6",
-            "grid": "gr",
-            "exp": ["historical",],
-            "ensemble": "r6i1p1f1",
-        }
-
-        forcing = GenericLumpedForcing.generate(
-            dataset=cmip_dataset,
-            start_time="2000-01-01T00:00:00Z",
-            end_time="2001-01-01T00:00:00Z",
-            shape=shape.absolute(),
-        )
-
-        data = load_precip(forcing.directory / forcing.pr)
-    """
-    data = xr.open_dataset(ncfile)
-    assert "time" in data.dims
-    assert varname in data.data_vars
-    return data[varname]
+import xarray as xr
+from pathlib import Path
+import json
+
+
+def read_config(config_file: str) -> dict:
+    with open(config_file) as cfg:
+        config = json.load(cfg)
+    return config
+
+
+def load_var(ncfile: str | Path, varname: str) -> xr.DataArray:
+    """Load the precipitation data file generated by GenericLumpedForcing.
+
+
+    .. code-block:: python
+
+        from ewatercycle.base.forcing import GenericLumpedForcing
+
+        shape = Path("./src/ewatercycle/testing/data/Rhine/Rhine.shp")
+        cmip_dataset = {
+            "dataset": "EC-Earth3",
+            "project": "CMIP6",
+            "grid": "gr",
+            "exp": ["historical",],
+            "ensemble": "r6i1p1f1",
+        }
+
+        forcing = GenericLumpedForcing.generate(
+            dataset=cmip_dataset,
+            start_time="2000-01-01T00:00:00Z",
+            end_time="2001-01-01T00:00:00Z",
+            shape=shape.absolute(),
+        )
+
+        data = load_precip(forcing.directory / forcing.pr)
+    """
+    data = xr.open_dataset(ncfile)
+    assert "time" in data.dims
+    assert varname in data.data_vars
+    return data[varname]
```

### Comparing `hbv-1.3.1/LICENSE.txt` & `hbv-1.4.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-Apache License
-Version 2.0, January 2004
-http://www.apache.org/licenses/
-
-TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-1. Definitions.
-
-"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-
-"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-
-"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-
-"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-
-"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-
-"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-
-"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-
-"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-
-"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-
-"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-
-2. Grant of Copyright License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-
-3. Grant of Patent License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-
-4. Redistribution. You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-
-     (a) You must give any other recipients of the Work or Derivative Works a copy of this License; and
-
-     (b) You must cause any modified files to carry prominent notices stating that You changed the files; and
-
-     (c) You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-
-     (d) If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-
-     You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-
-5. Submission of Contributions. Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-
-6. Trademarks. This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-
-7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-
-8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-
-9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
-
-END OF TERMS AND CONDITIONS
-
-APPENDIX: How to apply the Apache License to your work.
-
-To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!)  The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
-
-Copyright [yyyy] [name of copyright owner]
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+Apache License
+Version 2.0, January 2004
+http://www.apache.org/licenses/
+
+TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+1. Definitions.
+
+"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
+
+"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
+
+"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
+
+"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
+
+"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
+
+"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
+
+"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
+
+"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
+
+"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
+
+"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
+
+2. Grant of Copyright License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
+
+3. Grant of Patent License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
+
+4. Redistribution. You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
+
+     (a) You must give any other recipients of the Work or Derivative Works a copy of this License; and
+
+     (b) You must cause any modified files to carry prominent notices stating that You changed the files; and
+
+     (c) You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
+
+     (d) If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
+
+     You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
+
+5. Submission of Contributions. Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
+
+6. Trademarks. This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
+
+7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
+
+8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
+
+9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
+
+END OF TERMS AND CONDITIONS
+
+APPENDIX: How to apply the Apache License to your work.
+
+To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!)  The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
+
+Copyright [yyyy] [name of copyright owner]
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `hbv-1.3.1/README.md` & `hbv-1.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -47,8 +47,12 @@
 - bug fix where wrong types were given, warning messages cleaned up and code attempted to be made more readable
 ### V1.2.0
 - pretty big issue with setting values fixed - won't affect most use but will cause issues for Data Assimilation
 - use opportunity to name all HBV packages/naming/images to 1.2.0 
 ### V1.3.0
 - Change `Q_m` to `Q` in order to better integrate data assimilation & just makes more sense. 
 ## v1.3.1
-- Fix bug in time indexing
+- Fix bug in time indexing
+## v1.3.2
+- typo in update updating_dict_var_obj: was getting values wrong 
+## V1.4.0
+- adding snow reservoir
```

### Comparing `hbv-1.3.1/pyproject.toml` & `hbv-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "HBV"
 description = "Dev version for a HBV hydrological model using BMI for eWaterCycle."
 readme = "README.md"
 license = "Apache-2.0"
-version = "1.3.1"
+version = "1.4.0"
 authors = [
   { name = "David Haasnoot", email = "davidhaasnoot@gmail.com" },
 ]
 
 # Include here only the dependencies for the BMI Model
 # This is used to run the BmiModel inside the container
 dependencies = [
```

### Comparing `hbv-1.3.1/PKG-INFO` & `hbv-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: HBV
-Version: 1.3.1
+Version: 1.4.0
 Summary: Dev version for a HBV hydrological model using BMI for eWaterCycle.
 Author-email: David Haasnoot <davidhaasnoot@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Requires-Dist: bmipy
 Requires-Dist: netcdf4
 Requires-Dist: numpy
@@ -61,8 +61,12 @@
 - bug fix where wrong types were given, warning messages cleaned up and code attempted to be made more readable
 ### V1.2.0
 - pretty big issue with setting values fixed - won't affect most use but will cause issues for Data Assimilation
 - use opportunity to name all HBV packages/naming/images to 1.2.0 
 ### V1.3.0
 - Change `Q_m` to `Q` in order to better integrate data assimilation & just makes more sense. 
 ## v1.3.1
-- Fix bug in time indexing
+- Fix bug in time indexing
+## v1.3.2
+- typo in update updating_dict_var_obj: was getting values wrong 
+## V1.4.0
+- adding snow reservoir
```

