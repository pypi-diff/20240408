# Comparing `tmp/smadi-0.2.7.tar.gz` & `tmp/smadi-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smadi-0.2.7.tar", last modified: Wed Apr  3 19:59:57 2024, max compression
+gzip compressed data, was "smadi-0.2.8.tar", last modified: Sun Apr  7 23:28:40 2024, max compression
```

## Comparing `smadi-0.2.7.tar` & `smadi-0.2.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.561693 smadi-0.2.7/
--rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-0.2.7/.coveragerc
--rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-0.2.7/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-0.2.7/.readthedocs.yml
--rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-0.2.7/AUTHORS.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      128 2024-03-30 14:53:43.000000 smadi-0.2.7/CHANGELOG.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-0.2.7/CONTRIBUTING.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-0.2.7/LICENSE.txt
--rw-r--r--   0 m294      (1000) m294      (1000)     2224 2024-04-03 19:59:57.561693 smadi-0.2.7/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)      806 2024-04-03 19:20:09.000000 smadi-0.2.7/README.rst
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.557692 smadi-0.2.7/docs/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/Makefile
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.557692 smadi-0.2.7/docs/_static/
--rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/_static/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/authors.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/changelog.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     9748 2024-04-03 19:56:03.000000 smadi-0.2.7/docs/conf.py
--rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/contributing.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/index.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/license.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/readme.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      233 2024-03-30 14:53:43.000000 smadi-0.2.7/docs/requirements.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-0.2.7/pyproject.toml
--rw-rw-r--   0 m294      (1000) m294      (1000)      301 2024-04-03 02:37:06.000000 smadi-0.2.7/requirements.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)     1492 2024-04-03 19:59:57.561693 smadi-0.2.7/setup.cfg
--rw-rw-r--   0 m294      (1000) m294      (1000)      836 2024-04-03 19:59:48.000000 smadi-0.2.7/setup.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.549692 smadi-0.2.7/src/
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.557692 smadi-0.2.7/src/smadi/
--rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-0.2.7/src/smadi/__init__.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    19649 2024-04-01 23:41:33.000000 smadi-0.2.7/src/smadi/anomaly_detectors.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    15629 2024-04-03 14:11:17.000000 smadi-0.2.7/src/smadi/climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     3482 2024-04-02 14:59:26.000000 smadi-0.2.7/src/smadi/data_reader.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     8740 2024-04-03 14:10:41.000000 smadi-0.2.7/src/smadi/indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     5213 2024-04-03 02:37:06.000000 smadi-0.2.7/src/smadi/map.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     1813 2024-04-01 23:41:33.000000 smadi-0.2.7/src/smadi/metadata.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     7713 2024-04-03 14:17:09.000000 smadi-0.2.7/src/smadi/plot.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     8624 2024-04-03 14:16:38.000000 smadi-0.2.7/src/smadi/preprocess.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     4882 2024-04-03 14:50:02.000000 smadi-0.2.7/src/smadi/utils.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    16724 2024-04-03 19:54:00.000000 smadi-0.2.7/src/smadi/workflow.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.561693 smadi-0.2.7/src/smadi.egg-info/
--rw-r--r--   0 m294      (1000) m294      (1000)     2224 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)      915 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/SOURCES.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/dependency_links.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)       44 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/entry_points.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/not-zip-safe
--rw-rw-r--   0 m294      (1000) m294      (1000)      327 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/requires.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-04-03 19:59:57.000000 smadi-0.2.7/src/smadi.egg-info/top_level.txt
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-03 19:59:57.561693 smadi-0.2.7/tests/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-0.2.7/tests/conftest.py
--rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-0.2.7/tests/data_sample.csv
--rw-rw-r--   0 m294      (1000) m294      (1000)    20031 2024-03-30 14:58:36.000000 smadi-0.2.7/tests/test_climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-0.2.7/tests/test_indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-0.2.7/tox.ini
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.951335 smadi-0.2.8/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-0.2.8/.coveragerc
+-rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-0.2.8/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-0.2.8/.readthedocs.yml
+-rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-0.2.8/AUTHORS.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      128 2024-03-30 14:53:43.000000 smadi-0.2.8/CHANGELOG.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-0.2.8/CONTRIBUTING.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-0.2.8/LICENSE.txt
+-rw-r--r--   0 m294      (1000) m294      (1000)     6981 2024-04-07 23:28:40.951335 smadi-0.2.8/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)     5563 2024-04-07 23:28:23.000000 smadi-0.2.8/README.rst
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.947335 smadi-0.2.8/docs/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/Makefile
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.947335 smadi-0.2.8/docs/_static/
+-rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/_static/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/authors.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/changelog.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     9748 2024-04-03 20:04:41.000000 smadi-0.2.8/docs/conf.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/contributing.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/index.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/license.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/readme.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      231 2024-04-03 20:04:36.000000 smadi-0.2.8/docs/requirements.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-0.2.8/pyproject.toml
+-rw-rw-r--   0 m294      (1000) m294      (1000)      301 2024-04-03 02:37:06.000000 smadi-0.2.8/requirements.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1492 2024-04-07 23:28:40.955335 smadi-0.2.8/setup.cfg
+-rw-rw-r--   0 m294      (1000) m294      (1000)      836 2024-04-07 23:20:59.000000 smadi-0.2.8/setup.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.943334 smadi-0.2.8/src/
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.951335 smadi-0.2.8/src/smadi/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-0.2.8/src/smadi/__init__.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    18006 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/anomaly_detectors.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    15636 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     3482 2024-04-02 14:59:26.000000 smadi-0.2.8/src/smadi/data_reader.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     8809 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     5419 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/map.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2871 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/metadata.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     7809 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/plot.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     8624 2024-04-03 14:16:38.000000 smadi-0.2.8/src/smadi/preprocess.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     4882 2024-04-03 14:50:02.000000 smadi-0.2.8/src/smadi/utils.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    18957 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/workflow.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.951335 smadi-0.2.8/src/smadi.egg-info/
+-rw-r--r--   0 m294      (1000) m294      (1000)     6981 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)      915 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/SOURCES.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/dependency_links.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)       44 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/entry_points.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/not-zip-safe
+-rw-rw-r--   0 m294      (1000) m294      (1000)      327 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/requires.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/top_level.txt
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.951335 smadi-0.2.8/tests/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-0.2.8/tests/conftest.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-0.2.8/tests/data_sample.csv
+-rw-rw-r--   0 m294      (1000) m294      (1000)    20031 2024-03-30 14:58:36.000000 smadi-0.2.8/tests/test_climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-0.2.8/tests/test_indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-0.2.8/tox.ini
```

### Comparing `smadi-0.2.7/.coveragerc` & `smadi-0.2.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/.gitignore` & `smadi-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/.readthedocs.yml` & `smadi-0.2.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/CONTRIBUTING.rst` & `smadi-0.2.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/LICENSE.txt` & `smadi-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/docs/Makefile` & `smadi-0.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/docs/conf.py` & `smadi-0.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/docs/index.rst` & `smadi-0.2.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/setup.cfg` & `smadi-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/setup.py` & `smadi-0.2.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
         setup(
-            version="0.2.7",
+            version="0.2.8",
             entry_points={
                 "console_scripts": [
                     "run = smadi.workflow:main",
                 ]
             },
         )
```

### Comparing `smadi-0.2.7/src/smadi/__init__.py` & `smadi-0.2.8/src/smadi/__init__.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/src/smadi/anomaly_detectors.py` & `smadi-0.2.8/src/smadi/anomaly_detectors.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,66 +138,14 @@
 
         """
         self.clim_df = self._preprocess().copy()
 
         return filter_df(self.clim_df, **kwargs)
 
 
-class AbsoluteAnomaly(AnomalyDetector):
-    """
-    A class for detecting anomalies in time series data based on the absolute deviation value from the climate normal.
-
-    SMA = x - ref
-
-        where:
-        x: the average value of the variable in the time series data. It can be any of the following:
-        Daily average, weekly average, monthly average, etc.
-        ref: the long-term mean (μ) or median (η) of the variable(the climate normal).
-
-    """
-
-    def __init__(
-        self,
-        df: pd.DataFrame,
-        variable: str,
-        fillna: bool = False,
-        fillna_window_size: int = None,
-        smoothing=False,
-        smooth_window_size=None,
-        timespan: List[str] = None,
-        time_step: str = "month",
-        normal_metrics: List[str] = ["mean"],
-    ):
-        super().__init__(
-            df,
-            variable,
-            fillna,
-            fillna_window_size,
-            smoothing,
-            smooth_window_size,
-            timespan,
-            time_step,
-            normal_metrics,
-        )
-
-    def _preprocess(self, **kwargs) -> pd.DataFrame:
-        super()._preprocess(**kwargs)
-        return self.clim_df
-
-    def detect_anomaly(self, **kwargs) -> pd.DataFrame:
-        super().detect_anomaly(**kwargs)
-
-        for metric in self.normal_metrics:
-            self.clim_df[f"abs-{metric}"] = (
-                self.clim_df[f"{self.var}-avg"] - self.clim_df[f"norm-{metric}"]
-            )
-
-        return filter_df(self.clim_df, **kwargs)
-
-
 class ZScore(AnomalyDetector):
     """
     A class for detecting anomalies in time series data based on the Z-Score method.
 
     z_score = (x - μ) / σ
 
         where:
@@ -670,12 +618,7 @@
     from pathlib import Path
     from smadi.data_reader import extract_obs_ts
 
     ascat_path = Path("/home/m294/VSA/Code/datasets")
 
     po = 4854801
     sm_ts = extract_obs_ts(po, ascat_path, obs_type="sm", read_bulk=False)
-    df = AbsoluteAnomaly(
-        sm_ts, "sm", time_step="month", normal_metrics=["mean", "median"]
-    ).detect_anomaly()
-
-    print(df)
```

### Comparing `smadi-0.2.7/src/smadi/climatology.py` & `smadi-0.2.8/src/smadi/climatology.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,15 +447,15 @@
     ):
         """
         Initializes the Climatology class.
         """
         self.time_step = time_step
         self.normal_metrics = normal_metrics
         self.valid_time_steps = ["month", "dekad", "week", "day", "bimonth"]
-        self.valid_metrics = ["mean", "median", "min", "max"]
+        self.valid_metrics = ["mean", "median", "min", "max", "std"]
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
```

### Comparing `smadi-0.2.7/src/smadi/data_reader.py` & `smadi-0.2.8/src/smadi/data_reader.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/src/smadi/indicators.py` & `smadi-0.2.8/src/smadi/indicators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from scipy.stats import gaussian_kde
 from scipy.stats import norm, beta, gamma
+from scipy.stats import percentileofscore
 
 
 def zscore(obs, mean=None, std=None):
     """
     Computes the standardized z-score of the time series data.
 
     Parameters:
@@ -261,15 +262,15 @@
 def para_dis(obs, dist="beta"):
     """
     Compute the anomalies in time series data based on fitting the observed data to a parametric distribution.
 
     parameters:
     -----------
 
-    obs: sequence-like object
+    obs: pd.Series or np.ndarray or sequence-like object
         The observed time series data.
 
     dist: str, optional
         The distribution to fit the observed data to. Supported values: 'beta', 'gamma'
     """
 
     obs = np.asarray(obs)
```

### Comparing `smadi-0.2.7/src/smadi/map.py` & `smadi-0.2.8/src/smadi/map.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     -----------
 
     method: str
         The method name for which the thresholds are to be set. Supported methods are:
         'zscore', 'smapi', 'smdi', 'smca', 'smad', 'smci', 'smds', 'essmi', 'beta', 'gamma'
     """
 
-    if method in ["beta", "gamma", "essmi", "zscore", "smad"]:
-        return indicators_thresholds["zscore"]
-    else:
+    if method in indicators_thresholds.keys():
         return indicators_thresholds[method]
+    else:
+        return None
 
 
 def set_extent(df, x="lon", y="lat", buffer=2):
     """
     Set the extent for the map based on the provided dataframe and buffer.
 
     parameters:
@@ -59,156 +59,154 @@
         The data column name for which the bins and labels are to be set.
     """
     method = colm.split("(")[0]
     if "-" in method:
         method = method.split("-")[0]
 
     thrsholds = set_thresholds(method)
+    if not thrsholds:
+        return None
     bins = [val[1] for val in thrsholds.values()]
     labels = [key for key in thrsholds.keys()]
     labels.insert(0, labels[0])
     bins.insert(0, next(iter(thrsholds.values()))[0])
 
     return bins, labels
 
 
-def plot_anomaly_map(
-    df,
-    colm,
+def plot_anomaly_maps(
+    figsize=(25, 20),
+    ax_rows=1,
+    ax_cols=1,
+    df=None,
     x="lon",
     y="lat",
+    df_colms=None,
     crs=4326,
-    set_extent_to=True,
-    extent=None,
-    figsize=(7, 7),
-    title="SM Anomaly",
-    bins=None,
-    labels=None,
-    add_gridlines=True,
-    g_kwargs={
-        "d": (2, 2),
-        "ec": "grey",
-        "ls": "--",
-        "lw": 0.01,
+    figure_title="",
+    figure_title_kwargs={
+        "x": 0.5,
+        "y": 0.95,
+        "fontsize": 15,
+        "ha": "center",
+        "va": "center",
+        "fontweight": "bold",
     },
-    vmin=None,
-    vmax=None,
-    add_colorbar=True,
+    maps_titles=None,
+    maps_titles_kwargs={"pad": 20, "fontsize": 12, "fontweight": "bold"},
+    add_features=True,
+    frame_line_width=1,
     cmap="RdYlBu",
+    add_gridlines=False,
     cb_kwargs={
         "pos": 0.4,
-        "labelsize": 7,
+        "labelsize": 0.5,
         "tick_lines": "center",
         "show_values": False,
     },
 ):
-    """
-    Plot the anomaly map for the selected column from the dataframe.
-
-    parameters:
-    -----------
-
-    df: pd.DataFrame
-        The dataframe containing the data.
-
-    colm: str
-        The column name for the data to be plotted.
-
-    x: str
-        The column name for the x-axis.
-
-    y: str
-        The column name for the y-axis.
-
-    crs: int
-        The coordinate reference system for the map.
-
-    set_extent_to: bool
-        Whether to set the map to a specific extent.
-
-    extent: tuple
-        The extent to set the map to. if None, the extent is calculated based on the data.
-
-    figsize: tuple
-        The figure size for the map.
-
-    title: str
-        The title for the map.
-
-    bins: list
-        The bins for the color classification.
-
-    labels: list
-        The labels for the bins of the color classification.
-
-    add_gridlines: bool
-        Whether to add gridlines to the map.
-
-    g_kwargs: dict
-        The gridlines keyword arguments. This includes the linestyle, linewidth, edgecolor, and distance between gridlines.
-
-    vmin: float
-        The minimum value for the color classification.
-
-    vmax: float
-        The maximum value for the color classification.
-
-    cmap: str
-        The colormap for the map.
+    m = eomaps.Maps(ax=(ax_rows, ax_cols, 1), figsize=figsize)
+    figure_title_kwargs["s"] = figure_title
+    m.text(**figure_title_kwargs)
+
+    for i, colm in enumerate(df_colms):
+        ax_index = i + 1
+        if i == 0:
+            m = m
+        else:
+            m = m.new_map(ax=(ax_rows, ax_cols, ax_index), figsize=(7, 7))
+        m.ax.set_title(maps_titles[i], **maps_titles_kwargs)
+        m.set_shape.rectangles(radius=0.05)
+        if add_features:
+            m.add_feature.preset.coastline(lw=0.6)
+            m.add_feature.preset.countries(lw=0.4, ls="--")
+            m.add_feature.preset.ocean()
+            m.add_feature.preset.land()
+
+        m.set_frame(linewidth=frame_line_width)
+        m.set_data(data=df, parameter=colm, x=x, y=y, crs=crs)
+
+        if add_gridlines:
+            g = m.add_gridlines(
+                d=(2, 2),
+                ec="grey",
+                ls="--",
+                lw=0.01,
+            )
+            g.add_labels(fontsize=8)
+        clss = set_bins(colm)
+        bins = clss[0] if clss else [0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100]
+        labels = (
+            clss[1]
+            if clss
+            else [
+                "0-10",
+                "10-20",
+                "20-30",
+                "30-40",
+                "40-50",
+                "50-60",
+                "60-70",
+                "70-80",
+                "80-90",
+                "90-100",
+            ]
+        )
+        vmin = clss[0][0] if clss else df[colm].min()
+        vmax = clss[0][-1] if clss else df[colm].max()
 
-    add_colorbar: bool
-        Whether to add a colorbar to the map.
+        m.set_classify.UserDefined(bins=bins)
 
-    cb_kwargs: dict
-        The colorbar keyword arguments. This includes the position, label size, tick lines, and whether to show values.
+        if colm.split("(")[0] == "smds":
+            cmap = cmap + "_r"
+        m.plot_map(vmin=vmin, vmax=vmax, cmap=cmap, lw=1.5)
+        cb = m.add_colorbar(
+            label=False, spacing="uniform", pos=0.4, orientation="vertical"
+        )
+        cb.set_hist_size(0.8)
+        cb.tick_params(rotation=0, labelsize=10, pad=5)
 
+        if clss:
+            bins, labels = clss
+            cb.set_bin_labels(
+                bins=bins,
+                names=labels,
+                tick_lines=cb_kwargs["tick_lines"],
+                show_values=cb_kwargs["show_values"],
+            )
 
-    """
+    m.show()
 
-    # Initialize map object
-    m = eomaps.Maps(figsize=figsize, frameon=True, crs=crs)
-    m.ax.set_title(title, pad=20, linespacing=1.5)
-    m.set_shape.rectangles(radius=0.05)
-    m.set_frame(linewidth=0.5)
-
-    # Set data and parameter
-    m.set_data(data=df, parameter=colm, x=x, y=y, crs=crs)
-
-    # Set extent
-    if set_extent_to:
-        extent = set_extent(df, x=x, y=y) if extent is None else extent
-        m.ax.set_extent(extent, eomaps.Maps.CRS.PlateCarree())
-
-    # Set bins and labels
-    if bins is None and labels is None:
-        bins, labels = set_bins(colm)
-
-    # Set classification
-    m.set_classify.UserDefined(bins=bins)
-    # Add gridlines
-    if add_gridlines:
-        g = m.add_gridlines(**g_kwargs)
-        g.add_labels(fontsize=8)
-
-    # Set vmin and vmax based on the thresholds min and max
-    vmin = bins[0] if vmin is None else vmin
-    vmax = bins[-1] if vmax is None else vmax
-
-    # Plot map
-    cmap = cmap + "_r" if colm.split("(")[0] == "smds" else cmap
-    m.plot_map(vmin=vmin, vmax=vmax, cmap=cmap, lw=1.5)
 
-    # Add colorbar
+if __name__ == "__main__":
+    import pandas as pd
 
-    if add_colorbar:
-        cb = m.add_colorbar(
-            pos=cb_kwargs["pos"],
-        )
-        cb.tick_params(labelsize=cb_kwargs["labelsize"])
-        cb.set_bin_labels(
-            bins=bins,
-            names=labels,
-            tick_lines=cb_kwargs["tick_lines"],
-            show_values=cb_kwargs["show_values"],
-        )
+    df = pd.read_csv("test1.csv")
+    df.dropna(inplace=True)
 
-    m.show()
+    parameters = [
+        "sm-avg(2021-7)",
+        "norm-mean(2021-7)",
+        "abs-mean(2021-7)",
+        "abs-median(2021-7)",
+        "zscore(2021-7)",
+        "smad(2021-7)",
+    ]
+    titles = [
+        "SSM Average ",
+        "Climatology",
+        "Absolute Anomaly- Mean",
+        "Absolute Anomaly- Median",
+        "Z-Score",
+        "SMAD",
+    ]
+    plot_anomaly_maps(
+        figsize=(25, 20),
+        ax_cols=3,
+        ax_rows=2,
+        df=df,
+        df_colms=parameters,
+        figure_title="ASCAT SSM Anomaly Maps for Germany, July 2021",
+        maps_titles=titles,
+        add_gridlines=False,
+        add_features=True,
+    )
```

### Comparing `smadi-0.2.7/src/smadi/plot.py` & `smadi-0.2.8/src/smadi/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import matplotlib
 import matplotlib.pyplot as plt
 
 
 from smadi.anomaly_detectors import *
 from smadi.metadata import indicators_thresholds
+from smadi.map import set_thresholds
 
 
 def get_plot_options(**kwargs):
     """
     Set the basic plot options based on the provided kwargs for the plot.
 
     parameters:
@@ -55,15 +56,15 @@
     plt.ylabel(plot_params["ylabel"])
 
     # Add legend if specified
     if plot_params["legend"]:
         if plot_params["legend_labels"] is not None:
             plt.legend(plot_params["legend_labels"])
         else:
-            plt.legend()
+            plt.legend(loc="lower left")
 
     # Show plot
     plt.grid(plot_params["grid"])
     plt.tight_layout()
     if plot_params["savefig"] is not None:
         plt.savefig(plot_params["savefig"])
     plt.show()
@@ -99,14 +100,15 @@
 
     thresholds: dict
         The dictionary containing the thresholds for each category of the anomaly method.
 
     x_axis: list
         The x-axis values for the plot.
     """
+    thresholds = set_thresholds(thresholds)
     for key, value in thresholds.items():
         alpha = (
             int(key.split("-")[1]) * 0.2
             if key.startswith("D") or key.startswith("W")
             else 0.1
         )
         color = (
@@ -131,15 +133,15 @@
         The dictionary containing the column names and their respective matplotlib plot options.
 
     thresholds: str
         The name of the anomaly method to use its thresholds.
     """
 
     results = []
-    anomaly_thresholds = indicators_thresholds[thresholds]
+    anomaly_thresholds = set_thresholds(thresholds)
 
     if len(columns) > 2:
         raise ValueError("The number of columns should not exceed 2.")
 
     for colm, _ in columns.items():
         category_counter = {}
         for key, value in anomaly_thresholds.items():
@@ -165,15 +167,16 @@
 
     anomaly_method: str
         The name of the anomaly method to use its thresholds.
 
     """
     for i, result in enumerate(results):
         for key, value in result.items():
-            y = indicators_thresholds[anomaly_method][key][1]
+            thresholds = set_thresholds(anomaly_method)
+            y = thresholds[key][1]
             x = x_axis[0] if i == 0 else x_axis[-1]
             halignment = "right" if i == 0 else "left"
             plt.text(
                 x=x,
                 y=y,
                 s=f"{key}:{value}",
                 fontsize=10,
@@ -219,15 +222,15 @@
 
     # Set values for kwargs based on provided values
     plot_params = get_plot_options(**kwargs)
     plt.figure(figsize=plot_params["figsize"])
     plot_colmns(df, x_axis, colmns)
 
     if plot_hbars:
-        draw_hbars(indicators_thresholds[thresholds], x_axis)
+        draw_hbars(thresholds, x_axis)
     if plot_categories:
         results = clss_counter(df, colmns, thresholds)
         plot_categories_count(x_axis, results, thresholds)
 
     plot_figure(plot_params)
```

### Comparing `smadi-0.2.7/src/smadi/preprocess.py` & `smadi-0.2.8/src/smadi/preprocess.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/src/smadi/utils.py` & `smadi-0.2.8/src/smadi/utils.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/src/smadi/workflow.py` & `smadi-0.2.8/src/smadi/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,27 +26,27 @@
 
 
 def setup_argument_parser() -> ArgumentParser:
     """
     Setup argument parser for SMADI workflow execution.
     """
     parser = ArgumentParser(
-        description="Run the SMADI workflow for anomaly detection in ASCAT data"
+        description="Run the SMADI workflow for anomaly detection on ASCAT data"
     )
 
     # Required arguments
     parser.add_argument(
         "data_path", metavar="data_path", type=str, help="Path to the ASCAT data"
     )
     parser.add_argument(
         "aoi",
         metavar="aoi",
         type=str,
         help="Country name or bounding box coordinates\
-        in the tuple 'lon_min, lon_max , lat_min, lat_max'",
+        in str format 'lon_min, lon_max , lat_min, lat_max'",
     )
     parser.add_argument(
         "time_step",
         metavar="time_step",
         type=str,
         default="month",
         choices=["month", "dekad", "week", "bimonth", "day"],
@@ -148,15 +148,24 @@
         "--smooth_size", type=int, default=31, help="Smoothing window size"
     )
     parser.add_argument(
         "--workers",
         metavar="workers",
         type=int,
         default=None,
-        help="The number of workers to use for multiprocessing",
+        help="The number of workers to determine the degree of concurrent processing in a multiprocessing setup",
+    )
+
+    parser.add_argument(
+        "--addi_retrive",
+        metavar="addi_retrive",
+        type=str,
+        nargs="*",
+        default=None,
+        help="Additional parameters to retrieve from the anomaly dataframe. Supported values: 'var', 'norm' , 'abs'",
     )
     parser.add_argument(
         "--save_to",
         type=str,
         default=None,
         help="Save the output to a file to the given path",
     )
@@ -194,14 +203,15 @@
         "timespan": args.timespan,
         "year": args.year,
         "month": args.month,
         "dekad": args.dekad,
         "week": args.week,
         "bimonth": args.bimonth,
         "day": args.day,
+        "addi_retrive": args.addi_retrive,
         "save_to": args.save_to,
     }
     return parsed_args
 
 
 # Create a logger
 logger = create_logger("workflow-logger")
@@ -371,14 +381,55 @@
         if method not in _Detectors.keys():
             raise ValueError(
                 f"Anomaly method '{method}' is not supported."
                 f"Supported methods are one of the following: {tuple(_Detectors.keys())}"
             )
 
 
+def addi_retrival(
+    addi_retrive: list = ["var", "norm", "abs"],
+    results: pd.DataFrame = None,
+    anomaly: pd.DataFrame = None,
+    variable: str = None,
+    date_str: str = None,
+):
+    """
+    Validate and retrieve additional parameters from the anomaly dataframe.
+    """
+
+    if addi_retrive is not None:
+
+        # if not all(value in ["var", "norm"] for value in addi_retrive):
+        #     raise ValueError(
+        #         "The additional retrieval parameters must be one of the following: 'var', 'norm'"
+        #     )
+
+        if "var" in addi_retrive:
+            results[f"{variable}-avg" + f"({date_str})"] = anomaly[
+                f"{variable}-avg"
+            ].values
+        if "norm" in addi_retrive:
+            if "norm-mean" in anomaly.columns:
+                results["norm-mean" + f"({date_str})"] = anomaly["norm-mean"].values
+            if "norm-median" in anomaly.columns:
+                results["norm-median" + f"({date_str})"] = anomaly["norm-median"].values
+
+        if "abs" in addi_retrive:
+            if "norm-mean" in anomaly.columns:
+                results["abs-mean" + f"({date_str})"] = (
+                    anomaly[f"{variable}-avg"].values - anomaly["norm-mean"].values
+                )
+            if "norm-median" in anomaly.columns:
+                results["abs-median" + f"({date_str})"] = (
+                    anomaly[f"{variable}-avg"].values - anomaly["norm-median"].values
+                )
+
+    return results
+
+
 @log_exception(logger)
 def single_po_run(
     gpi: int,
     methods: str = ["zscore"],
     variable: str = "sm",
     time_step: str = "month",
     fillna: bool = False,
@@ -388,14 +439,15 @@
     year: Union[int, List[int]] = None,
     month: Union[int, List[int]] = None,
     dekad: Union[int, List[int]] = None,
     week: Union[int, List[int]] = None,
     bimonth: Union[int, List[int]] = None,
     day: Union[int, List[int]] = None,
     timespan: List[str] = None,
+    addi_retrive: list = ["var", "norm"],
 ) -> Tuple[int, Dict[str, float]]:
     """
     Run the anomaly detection workflow for a single grid point index.
     """
 
     # Load the time series for the given gpi
     global ascat_obj
@@ -434,15 +486,23 @@
 
         try:
             for date_param in date_params:
                 anomaly = _Detectors[method](**anomaly_params).detect_anomaly(
                     **date_param
                 )
                 date_str = f"-".join(str(value) for value in date_param.values())
-                results[method + f"({date_str})"] = anomaly[method].values[0]
+                results[method + f"({date_str})"] = anomaly[method].values
+
+                results = addi_retrival(
+                    addi_retrive=addi_retrive,
+                    results=results,
+                    anomaly=anomaly,
+                    variable=variable,
+                    date_str=date_str,
+                )
 
         except AttributeError as e:
             return None
 
     return (gpi, results)
 
 
@@ -474,29 +534,29 @@
     year: List[int] = None,
     month: List[int] = None,
     dekad: List[int] = None,
     week: List[int] = None,
     bimonth: List[int] = None,
     day: List[int] = None,
     workers: int = None,
+    addi_retrive: list = ["anomaly"],
 ) -> pd.DataFrame:
     """
     Run the anomaly detection workflow for multiple grid point indices with multiprocessing support.
     """
-    logger.info("\nWorkflow started....\n")
+    logger.info("Workflow started....\n")
     logger.info(f"Loading grid points for {aoi}....")
 
     if isinstance(aoi, str):
         pointlist = load_gpis_by_country(aoi)
     else:
         pointlist = get_gpis_from_bbox(aoi)
 
     logger.info(f"Grid points loaded successfully for {aoi}\n")
     logger.info(f"\n\n{pointlist.head()}")
-    pointlist = pointlist[:10]
     pre_compute = partial(
         single_po_run,
         methods=methods,
         variable=variable,
         time_step=time_step,
         fillna=fillna,
         fillna_window_size=fillna_window_size,
@@ -505,14 +565,15 @@
         year=year,
         month=month,
         dekad=dekad,
         week=week,
         bimonth=bimonth,
         day=day,
         timespan=timespan,
+        addi_retrive=addi_retrive,
     )
 
     logger.info(f"Running the anomaly detection workflow for {aoi}....\n")
 
     logger.info("Workflow parameters:\n")
     logger.info(f"    Anomaly detection methods: {', '.join(methods)}")
     logger.info(f"    Variable: {variable}")
@@ -575,23 +636,24 @@
         dekad=args["dekad"],
         timespan=args["timespan"],
         fillna=args["fillna"],
         fillna_window_size=args["fillna_size"],
         smoothing=args["smoothing"],
         smooth_window_size=args["smooth_size"],
         workers=args["workers"],
+        addi_retrive=args["addi_retrive"],
     )
 
     logger.info(f"\n\n {df}")
 
     if args["save_to"]:
         try:
             df.to_csv(args["save_to"])
-            print(f"Saving the output data frame to {args['save_to']}....")
-            print("Output saved successfully")
+            logger.info(f"Saving the output data frame to {args['save_to']}....")
+            logger.info("Output saved successfully")
 
         except ArgumentError as e:
             parser.error(str(e))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `smadi-0.2.7/src/smadi.egg-info/SOURCES.txt` & `smadi-0.2.8/src/smadi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/tests/conftest.py` & `smadi-0.2.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/tests/data_sample.csv` & `smadi-0.2.8/tests/data_sample.csv`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/tests/test_climatology.py` & `smadi-0.2.8/tests/test_climatology.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/tests/test_indicators.py` & `smadi-0.2.8/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.7/tox.ini` & `smadi-0.2.8/tox.ini`

 * *Files identical despite different names*

