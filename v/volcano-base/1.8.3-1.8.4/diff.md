# Comparing `tmp/volcano_base-1.8.3.tar.gz` & `tmp/volcano_base-1.8.4.tar.gz`

## Comparing `volcano_base-1.8.3.tar` & `volcano_base-1.8.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 volcano_base-1.8.3/.mise.local.toml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 volcano_base-1.8.3/.mise.toml
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 volcano_base-1.8.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-1.8.3/.release-please-manifest.json
--rw-r--r--   0        0        0    17941 2020-02-02 00:00:00.000000 volcano_base-1.8.3/CHANGELOG.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-1.8.3/release-please-config.json
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 volcano_base-1.8.3/requirements-dev.lock
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 volcano_base-1.8.3/requirements.lock
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 volcano_base-1.8.3/.github/dependabot.yml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-1.8.3/.github/release-please/release-please-config.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-1.8.3/.github/release-please/release-please-manifest.json
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 volcano_base-1.8.3/.github/workflows/release.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 volcano_base-1.8.3/src/volcano_base/__init__.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 volcano_base-1.8.3/src/volcano_base/config.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 volcano_base-1.8.3/src/volcano_base/down/__init__.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 volcano_base-1.8.3/src/volcano_base/down/cesm2.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 volcano_base-1.8.3/src/volcano_base/down/historic_so2.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 volcano_base-1.8.3/src/volcano_base/down/ob16.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 volcano_base-1.8.3/src/volcano_base/load/__init__.py
--rw-r--r--   0        0        0    22053 2020-02-02 00:00:00.000000 volcano_base-1.8.3/src/volcano_base/load/load_c2w_files.py
--rw-r--r--   0        0        0    31462 2020-02-02 00:00:00.000000 volcano_base-1.8.3/src/volcano_base/load/load_ob16.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 volcano_base-1.8.3/src/volcano_base/manipulate/__init__.py
--rw-r--r--   0        0        0    24352 2020-02-02 00:00:00.000000 volcano_base-1.8.3/src/volcano_base/manipulate/time_series.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 volcano_base-1.8.3/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 volcano_base-1.8.3/LICENSE
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 volcano_base-1.8.3/README.md
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 volcano_base-1.8.3/pyproject.toml
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 volcano_base-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.mise.local.toml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.mise.toml
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.release-please-manifest.json
+-rw-r--r--   0        0        0    18405 2020-02-02 00:00:00.000000 volcano_base-1.8.4/CHANGELOG.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-1.8.4/release-please-config.json
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 volcano_base-1.8.4/requirements-dev.lock
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 volcano_base-1.8.4/requirements.lock
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.github/release-please/release-please-config.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.github/release-please/release-please-manifest.json
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/__init__.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/config.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/down/__init__.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/down/cesm2.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/down/historic_so2.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/down/ob16.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/load/__init__.py
+-rw-r--r--   0        0        0    22142 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/load/load_c2w_files.py
+-rw-r--r--   0        0        0    31469 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/load/load_ob16.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/manipulate/__init__.py
+-rw-r--r--   0        0        0    24352 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/manipulate/time_series.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 volcano_base-1.8.4/LICENSE
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 volcano_base-1.8.4/README.md
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 volcano_base-1.8.4/pyproject.toml
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 volcano_base-1.8.4/PKG-INFO
```

### Comparing `volcano_base-1.8.3/.mise.toml` & `volcano_base-1.8.4/.mise.toml`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/.pre-commit-config.yaml` & `volcano_base-1.8.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/CHANGELOG.md` & `volcano_base-1.8.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
 
+## [1.8.4](https://github.com/engeir/volcano-base/compare/v1.8.3...v1.8.4) (2024-04-08)
+
+
+### Bug Fixes
+
+* **ob16:** scale colum SO2 so unit adjusts from kg/m2 to Tg (per Earth surface) ([7c82515](https://github.com/engeir/volcano-base/commit/7c8251584e8787d18bc964ead685e86efc5a3ef8))
+
+
+### Miscellaneous
+
+* **cesm2 load:** print path of where we look for files ([7e57d94](https://github.com/engeir/volcano-base/commit/7e57d947eb01b3367a7062b78f954a798be1c238))
+
 ## [1.8.3](https://github.com/engeir/volcano-base/compare/v1.8.2...v1.8.3) (2024-04-03)
 
 
 ### Miscellaneous
 
 * **cesm2 load:** do not create parent directories ([5e59dcd](https://github.com/engeir/volcano-base/commit/5e59dcdd78b069f70c525de05d1883f6f05baa09))
```

### Comparing `volcano_base-1.8.3/release-please-config.json` & `volcano_base-1.8.4/release-please-config.json`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/requirements-dev.lock` & `volcano_base-1.8.4/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/requirements.lock` & `volcano_base-1.8.4/requirements.lock`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/.github/release-please/release-please-config.json` & `volcano_base-1.8.4/.github/release-please/release-please-config.json`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/.github/workflows/release.yml` & `volcano_base-1.8.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/src/volcano_base/config.py` & `volcano_base-1.8.4/src/volcano_base/config.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/src/volcano_base/down/cesm2.py` & `volcano_base-1.8.4/src/volcano_base/down/cesm2.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/src/volcano_base/down/historic_so2.py` & `volcano_base-1.8.4/src/volcano_base/down/historic_so2.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/src/volcano_base/down/ob16.py` & `volcano_base-1.8.4/src/volcano_base/down/ob16.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/src/volcano_base/load/load_c2w_files.py` & `volcano_base-1.8.4/src/volcano_base/load/load_c2w_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 import volcano_base
 
 
 class CESM2FileNotFound(FileNotFoundError):
     """Raise an error if one of the CESM2 files are not found."""
 
     def __init__(self, *args: object) -> None:
-        if args:
-            msg = f'Cannot find the file "{args[0]}", which is a nescessary CESM2 file.'
-        else:
-            msg = "Cannot find the necessary CESM2 files."
-        self.message = f"{msg} Please run the `save_cesm_files` function within `down.cesm2` to see what files are missing."
+        file = volcano_base.config.DATA_PATH
+        msg = (
+            f'Cannot find the file "{args[0]}", which is a nescessary CESM2 file.'
+            if args
+            else "Cannot find the necessary CESM2 files."
+        )
+        self.message = f"{msg} I went looking in {file.resolve()}. Please run the `save_cesm_files` function within `down.cesm2` to see what files are missing."
         super().__init__(self.message)
 
 
 class FindFiles:
     """Find files that match a pre-defined regular expression.
 
     Parameters
```

### Comparing `volcano_base-1.8.3/src/volcano_base/load/load_ob16.py` & `volcano_base-1.8.4/src/volcano_base/load/load_ob16.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         if not (fn := volcano_base.config.DATA_PATH / "cesm-lme" / file).exists():
             print(f"Cannot find {fn.resolve()}")
             volcano_base.down.save_historical_so2(fn)
         ds = xr.open_dataset(fn)
         avgs_list = volcano_base.manipulate.mean_flatten([ds.colmass], dims=["lat"])
         avgs = avgs_list[0]
         # Scale so that the unit is now in Tg(SO2) (Otto-Bliesner et al. (2016)).
-        avgs = avgs / avgs.max() * 257.9 / 3 * 2
+        avgs *= 510e3  # From kg/m2 to Tg/Earth surface
         f_time = avgs.time.data
         f_time = f_time - f_time[0] + 501
         avgs = avgs.assign_coords(
             time=volcano_base.manipulate.float2dt(f_time, freq="MS")
             + datetime.timedelta(days=14)
         )
         self._so2 = avgs
```

### Comparing `volcano_base-1.8.3/src/volcano_base/manipulate/__init__.py` & `volcano_base-1.8.4/src/volcano_base/manipulate/__init__.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/src/volcano_base/manipulate/time_series.py` & `volcano_base-1.8.4/src/volcano_base/manipulate/time_series.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/.gitignore` & `volcano_base-1.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/LICENSE` & `volcano_base-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.3/README.md` & `volcano_base-1.8.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Core module for volcanic eruption simulation projects
 
-<sup>Latest version: v1.8.3</sup> <!-- x-release-please-version -->
+<sup>Latest version: v1.8.4</sup> <!-- x-release-please-version -->
 
 > [!WARNING]
 >
 > This README reflects the changes made to the main branch. For the most up to date
 > documentation about the version you are using, see the README at the relevant tag.
 
 This repository contains the core elements used across several independent volcanic
```

### Comparing `volcano_base-1.8.3/pyproject.toml` & `volcano_base-1.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "volcano-base"
-version = "1.8.3"
+version = "1.8.4"
 description = "Download, find and manipulate volcano and climate related time series"
 authors = [{ name = "engeir", email = "engeir@pm.me" }]
 license = "MIT"
 readme = "README.md"
 requires-python = ">= 3.12"
 dependencies = [
     "returns>=0.22.0",
```

### Comparing `volcano_base-1.8.3/PKG-INFO` & `volcano_base-1.8.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: volcano-base
-Version: 1.8.3
+Version: 1.8.4
 Summary: Download, find and manipulate volcano and climate related time series
 Author-email: engeir <engeir@pm.me>
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.12
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: cftime>=1.6.3
@@ -19,15 +19,15 @@
 Requires-Dist: rich>=13.7.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: xarray>=2024.1.1
 Description-Content-Type: text/markdown
 
 # Core module for volcanic eruption simulation projects
 
-<sup>Latest version: v1.8.3</sup> <!-- x-release-please-version -->
+<sup>Latest version: v1.8.4</sup> <!-- x-release-please-version -->
 
 > [!WARNING]
 >
 > This README reflects the changes made to the main branch. For the most up to date
 > documentation about the version you are using, see the README at the relevant tag.
 
 This repository contains the core elements used across several independent volcanic
```

