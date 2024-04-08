# Comparing `tmp/gliderpy-0.2.1.tar.gz` & `tmp/gliderpy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliderpy-0.2.1.tar", last modified: Thu Feb  1 14:40:30 2024, max compression
+gzip compressed data, was "gliderpy-0.2.2.tar", last modified: Mon Apr  8 19:25:42 2024, max compression
```

## Comparing `gliderpy-0.2.1.tar` & `gliderpy-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 14:40:30.002682 gliderpy-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 14:40:29.998682 gliderpy-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-01 14:40:19.000000 gliderpy-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 14:40:30.002682 gliderpy-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-01 14:40:19.000000 gliderpy-0.2.1/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-02-01 14:40:19.000000 gliderpy-0.2.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-01 14:40:19.000000 gliderpy-0.2.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-01 14:40:19.000000 gliderpy-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-01 14:40:19.000000 gliderpy-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-01 14:40:19.000000 gliderpy-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-01 14:40:30.002682 gliderpy-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-01 14:40:19.000000 gliderpy-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 14:40:30.002682 gliderpy-0.2.1/gliderpy/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-01 14:40:19.000000 gliderpy-0.2.1/gliderpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-02-01 14:40:19.000000 gliderpy-0.2.1/gliderpy/fetchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-01 14:40:19.000000 gliderpy-0.2.1/gliderpy/plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-02-01 14:40:19.000000 gliderpy-0.2.1/gliderpy/servers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 14:40:30.002682 gliderpy-0.2.1/gliderpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-01 14:40:29.000000 gliderpy-0.2.1/gliderpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-02-01 14:40:19.000000 gliderpy-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-01 14:40:19.000000 gliderpy-0.2.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-01 14:40:19.000000 gliderpy-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 14:40:30.002682 gliderpy-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:25:42.290128 gliderpy-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:25:42.286128 gliderpy-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 19:25:36.000000 gliderpy-0.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:25:42.290128 gliderpy-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-08 19:25:36.000000 gliderpy-0.2.2/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-08 19:25:36.000000 gliderpy-0.2.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-08 19:25:36.000000 gliderpy-0.2.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-08 19:25:36.000000 gliderpy-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-08 19:25:36.000000 gliderpy-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-08 19:25:36.000000 gliderpy-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-08 19:25:42.290128 gliderpy-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-08 19:25:36.000000 gliderpy-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:25:42.290128 gliderpy-0.2.2/gliderpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 19:25:36.000000 gliderpy-0.2.2/gliderpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-04-08 19:25:36.000000 gliderpy-0.2.2/gliderpy/fetchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-08 19:25:36.000000 gliderpy-0.2.2/gliderpy/plotters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-08 19:25:36.000000 gliderpy-0.2.2/gliderpy/servers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:25:42.290128 gliderpy-0.2.2/gliderpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 19:25:42.000000 gliderpy-0.2.2/gliderpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-08 19:25:36.000000 gliderpy-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 19:25:36.000000 gliderpy-0.2.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 19:25:36.000000 gliderpy-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:25:42.290128 gliderpy-0.2.2/setup.cfg
```

### Comparing `gliderpy-0.2.1/.github/workflows/deploy-docs.yml` & `gliderpy-0.2.2/.github/workflows/deploy-docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -44,11 +44,11 @@
         mv notebooks/*output.ipynb docs/source/
         pushd docs
         make clean html linkcheck
         popd
 
     - name: Deploy
       if: success() && github.event_name == 'release'
-      uses: peaceiris/actions-gh-pages@v3
+      uses: peaceiris/actions-gh-pages@v4
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
         publish_dir: docs/build/html
```

### Comparing `gliderpy-0.2.1/.github/workflows/pypi.yml` & `gliderpy-0.2.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `gliderpy-0.2.1/.github/workflows/tests.yml` & `gliderpy-0.2.2/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     branches: [main]
 
 jobs:
   run:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.10", "3.11", "3.12"]
         os: [windows-latest, ubuntu-latest, macos-latest]
       fail-fast: false
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Setup Micromamba ${{ matrix.python-version }}
```

### Comparing `gliderpy-0.2.1/.pre-commit-config.yaml` & `gliderpy-0.2.2/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
     - id: trailing-whitespace
     - id: check-ast
     - id: debug-statements
     - id: end-of-file-fixer
     - id: check-docstring-first
     - id: check-added-large-files
       exclude_types: [yaml]
     - id: requirements-txt-fixer
     - id: file-contents-sorter
       files: requirements-dev.txt
 
-- repo: https://github.com/psf/black
-  rev: 24.1.1
-  hooks:
-  - id: black
-    language_version: python3
-
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.8.0
+  rev: v1.9.0
   hooks:
   - id: mypy
     exclude: docs/source/conf.py
     entry: bash -c 'exec env CONDA_PREFIX="$(python -c "import sys; print(sys.executable)")"'
     args: ["--ignore-missing-imports", "--python-executable=CONDA_PREFIX"]
 
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.9
   hooks:
     - id: blackdoc
 
 - repo: https://github.com/econchick/interrogate
-  rev: 237be78f9c6135fc1a620d211cdfdc5d3885082b
+  rev: 1.7.0
   hooks:
     - id: interrogate
       exclude: ^(docs|tests)
       args: [--config=pyproject.toml]
 
 - repo: https://github.com/codespell-project/codespell
   rev: v2.2.6
@@ -52,17 +46,35 @@
 
 - repo: https://github.com/asottile/add-trailing-comma
   rev: v3.1.0
   hooks:
     - id: add-trailing-comma
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.1.15
+  rev: v0.3.5
   hooks:
     - id: ruff
+      args: ["--fix", "--show-fixes"]
+    - id: ruff-format
+
+- repo: https://github.com/nbQA-dev/nbQA
+  rev: 1.8.5
+  hooks:
+    - id: nbqa-check-ast
+    - id: nbqa-black
+    - id: nbqa-ruff
+      args: [
+        --fix,
+        --config=ruff.toml,
+        ]
+
+- repo: https://github.com/bdice/nb-strip-paths
+  rev: v0.1.0
+  hooks:
+    - id: nb-strip-paths
 
 - repo: https://github.com/tox-dev/pyproject-fmt
   rev: 1.7.0
   hooks:
     - id: pyproject-fmt
 
 ci:
```

### Comparing `gliderpy-0.2.1/LICENSE.txt` & `gliderpy-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gliderpy-0.2.1/PKG-INFO` & `gliderpy-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliderpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Glider Data Fetcher
 Maintainer: Lindsay Abrams, Filipe Fernandes
 Maintainer-email: Callum Rollo <c.rollo@outlook.com>
 License: Copyright 2017 Filipe Fernandes and contributors
         
         
         Redistribution and use in source and binary forms,
@@ -33,20 +33,18 @@
         STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY
         WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: documentation, https://ioos.github.io/gliderpy
 Project-URL: homepage, https://github.com/ioos/gliderpy
 Project-URL: repository, https://github.com/ioos/gliderpy
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: erddapy
 Requires-Dist: httpx
 Requires-Dist: pandas
 Requires-Dist: xarray
```

### Comparing `gliderpy-0.2.1/README.md` & `gliderpy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gliderpy-0.2.1/gliderpy/fetchers.py` & `gliderpy-0.2.2/gliderpy/fetchers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,126 +1,140 @@
-"""
-Helper methods to fetch glider data from multiple ERDDAP serves
-
-"""
+"""Helper methods to fetch glider data from multiple ERDDAP serves."""
 
+import datetime
 import functools
 from copy import copy
-from typing import Optional
+from numbers import Number
 
 import httpx
 import pandas as pd
 from erddapy import ERDDAP
-from erddapy.erddapy import urlopen
+from erddapy.core.url import urlopen
 
 from gliderpy.servers import (
     server_parameter_rename,
     server_vars,
 )
 
-OptionalStr = Optional[str]
+OptionalBool = bool | None
+OptionalDF = pd.DataFrame | None
+OptionalDict = dict | None
+OptionalList = list[str] | tuple[str] | None
+OptionalStr = str | None
+OptionalNum = Number | None
+# Should we add more or datetime.datetime catches all?
+OptionalDateTime = datetime.datetime | str
 
 # Defaults to the IOOS glider DAC.
 _server = "https://gliders.ioos.us/erddap"
 
 
 @functools.lru_cache(maxsize=128)
-def _to_pandas_multiple(glider_grab):
-    """Thin wrapper to cache the results when multiple datasets are requested."""
+def _to_pandas_multiple(glider_grab: "GliderDataFetcher") -> pd.DataFrame:
+    """Thin wrapper to cache results when multiple datasets are requested."""
     df_all = {}
     glider_grab_copy = copy(glider_grab)
     for dataset_id in glider_grab_copy.datasets["Dataset ID"]:
         glider_grab_copy.fetcher.dataset_id = dataset_id
-        df = glider_grab_copy.fetcher.to_pandas()
+        glider_df = glider_grab_copy.fetcher.to_pandas()
         dataset_url = glider_grab_copy.fetcher.get_download_url().split("?")[0]
-        df = standardise_df(df, dataset_url)
-        df_all.update({dataset_id: df})
+        glider_df = standardise_df(glider_df, dataset_url)
+        df_all.update({dataset_id: glider_df})
     return df_all
 
 
-def standardise_df(df, dataset_url):
-    """
-    Standardise variable names in a dataset and add column for url
-    """
-    df.columns = df.columns.str.lower()
-    df = df.set_index("time (utc)")
-    df = df.rename(columns=server_parameter_rename)
-    df.index = pd.to_datetime(df.index)
-    # We need to sort b/c of the non-sequential submission of files due to the nature of glider data transmission.
-    df = df.sort_index()
-    df["dataset_url"] = dataset_url
-    return df
+def standardise_df(glider_df: pd.DataFrame, dataset_url: str) -> pd.DataFrame:
+    """Standardise variable names in a dataset and add column for URL."""
+    glider_df.columns = glider_df.columns.str.lower()
+    glider_df = glider_df.set_index("time (utc)")
+    glider_df = glider_df.rename(columns=server_parameter_rename)
+    glider_df.index = pd.to_datetime(
+        glider_df.index,
+        format="%Y-%m-%dT%H:%M:%SZ",
+    )
+    # We need to sort b/c of the non-sequential submission of files due to
+    # the nature of glider data transmission.
+    glider_df = glider_df.sort_index()
+    glider_df["dataset_url"] = dataset_url
+    return glider_df
 
 
 class GliderDataFetcher:
-    """
+    """Instantiate the glider fetcher.
+
     Args:
+    ----
         server: A glider ERDDAP server URL.
 
     Attributes:
+    ----------
         dataset_id: A dataset unique id.
         constraints: Download constraints, defaults same as query.
 
     """
 
-    def __init__(self, server=_server):
+    def __init__(
+        self: "GliderDataFetcher",
+        server: OptionalStr = _server,
+    ) -> None:
+        """Instantiate main class attributes."""
         self.server = server
         self.fetcher = ERDDAP(
             server=server,
             protocol="tabledap",
         )
         self.fetcher.variables = server_vars[server]
         self.fetcher.dataset_id: OptionalStr = None
-        self.datasets: Optional = None
+        self.datasets: OptionalDF = None
 
-    def to_pandas(self):
-        """
-        Fetches data from the server and reads into a pandas dataframe
+    def to_pandas(self: "GliderDataFetcher") -> pd.DataFrame:
+        """Return data from the server as a pandas dataframe.
 
-        :return: pandas dataframe with datetime UTC as index, multiple dataset_ids dataframes are stored in a dictionary
+        :return: pandas a dataframe with datetime UTC as index,
+                 multiple dataset_ids dataframes are stored in a dictionary
         """
         if self.fetcher.dataset_id:
-            df = self.fetcher.to_pandas()
+            glider_df = self.fetcher.to_pandas()
         elif not self.fetcher.dataset_id and self.datasets is not None:
-            df_all = _to_pandas_multiple(self)
-            # We need to reset to avoid fetching a single dataset_id when making multiple requests.
+            glider_df = _to_pandas_multiple(self)
+            # We need to reset to avoid fetching a single dataset_id when
+            # making multiple requests.
             self.fetcher.dataset_id = None
-            return df_all
+            return glider_df
         else:
-            raise ValueError(
-                f"Must provide a {self.fetcher.dataset_id} or `query` terms to download data.",
-            )
+            msg = "Must provide a dataset_id or query terms to download data."
+            raise ValueError(msg)
 
         # Standardize variable names for the single dataset_id.
         dataset_url = self.fetcher.get_download_url().split("?")[0]
-        df = standardise_df(df, dataset_url)
-        return df
+        return standardise_df(glider_df, dataset_url)
 
-    def query(
-        self,
-        min_lat=None,
-        max_lat=None,
-        min_lon=None,
-        max_lon=None,
-        min_time=None,
-        max_time=None,
-        delayed=False,
-    ):
-        """
-        Takes user supplied geographical and time constraints and adds them to the query
+    def query(  # noqa: PLR0913
+        self: "GliderDataFetcher",
+        *,
+        min_lat: OptionalNum = None,
+        max_lat: OptionalNum = None,
+        min_lon: OptionalNum = None,
+        max_lon: OptionalNum = None,
+        min_time: OptionalDateTime = None,
+        max_time: OptionalDateTime = None,
+        delayed: OptionalBool = False,
+    ) -> pd.DataFrame:
+        """Add user supplied geographical and time constraints to the query.
 
         :param min_lat: southernmost lat
         :param max_lat: northermost lat
         :param min_lon: westernmost lon (-180 to +180)
         :param max_lon: easternmost lon (-180 to +180)
         :param min_time: start time, can be datetime object or string
         :param max_time: end time, can be datetime object or string
         :return: search query with argument constraints applied
         """
-        # FIXME: The time constrain could be better implemented by just dropping it instead.
+        # NB: The time constrain could be better implemented by just
+        # dropping it instead.
         min_time = min_time if min_time else "1970-01-01"
         max_time = max_time if max_time else "2038-01-19"
         min_lat = min_lat if min_lat else -90.0
         max_lat = max_lat if max_lat else 90.0
         min_lon = min_lon if min_lon else -180.0
         max_lon = max_lon if max_lon else 180.0
 
@@ -128,64 +142,83 @@
             "time>=": min_time,
             "time<=": max_time,
             "latitude>=": min_lat,
             "latitude<=": max_lat,
             "longitude>=": min_lon,
             "longitude<=": max_lon,
         }
-        if not self.datasets:
+        if self.datasets is None:
             url = self.fetcher.get_search_url(
                 search_for="glider",
                 response="csv",
                 min_lat=min_lat,
                 max_lat=max_lat,
                 min_lon=min_lon,
                 max_lon=max_lon,
                 min_time=min_time,
                 max_time=max_time,
             )
             self.query_url = url
             try:
                 data = urlopen(url)
             except httpx.HTTPError as err:
-                raise Exception(
-                    f"Error, no datasets found in supplied range. Try relaxing your constraints: {self.fetcher.constraints}",
-                ) from err
-                return None
-            df = pd.read_csv(data)[["Title", "Institution", "Dataset ID"]]
+                msg = (
+                    "Error, no datasets found in supplied range. "
+                    f"Try relaxing the constraints: {self.fetcher.constraints}"
+                )
+                err.message = f"{err.message}\n{msg}"
+                raise
+
+            cols = ["Title", "Institution", "Dataset ID"]
+            datasets = pd.read_csv(data)[cols]
             if not delayed:
-                df = df.loc[~df["Dataset ID"].str.endswith("delayed")]
+                datasets = datasets.loc[
+                    ~datasets["Dataset ID"].str.endswith("delayed")
+                ]
                 info_urls = [
-                    self.fetcher.get_info_url(dataset_id=dataset_id, response="html")
-                    for dataset_id in df["Dataset ID"]
+                    self.fetcher.get_info_url(
+                        dataset_id=dataset_id,
+                        response="html",
+                    )
+                    for dataset_id in datasets["Dataset ID"]
                 ]
-                df["info_url"] = info_urls
-            self.datasets = df
+                datasets["info_url"] = info_urls
+            self.datasets = datasets
         return self.datasets
 
 
 class DatasetList:
     """Build a glider dataset ids list.
 
 
-    Attributes:
+    Attributes
+    ----------
         e: an ERDDAP server instance
-        TODO: search_terms: A list of terms to search the server for. Multiple terms will be combined as "AND."
+        TODO -> search_terms: A list of terms to search the server for.
+                Multiple terms will be combined as "AND."
 
     """
 
-    def __init__(self, server=_server):
+    def __init__(self: "DatasetList", server: OptionalStr = _server) -> None:
+        """Instantiate main class attributes.
+
+        Attributes
+        ----------
+          server: the server URL.
+          protocol: ERDDAP's protocol (tabledap/griddap)
+
+        """
         self.e = ERDDAP(
             server=server,
             protocol="tabledap",
         )
 
-    def get_ids(self):
+    def get_ids(self: "DatasetList") -> list:
         """Return the allDatasets list for the glider server."""
         if self.e.server == "https://gliders.ioos.us/erddap":
             self.e.dataset_id = "allDatasets"
             dataset_ids = self.e.to_pandas()["datasetID"].to_list()
             dataset_ids.remove("allDatasets")
             self.dataset_ids = dataset_ids
             return self.dataset_ids
-        else:
-            raise ValueError(f"The {self.e.server} does not supported this operation.")
+        msg = f"The {self.e.server} does not supported this operation."
+        raise ValueError(msg)
```

### Comparing `gliderpy-0.2.1/gliderpy/plotters.py` & `gliderpy-0.2.2/gliderpy/plotters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,57 @@
-"""
-Some convenience functions to help visualize glider data.
-"""
+"""Some convenience functions to help visualize glider data."""
+
+from __future__ import annotations
 
 import warnings
+from typing import TYPE_CHECKING
 
 try:
     import cartopy.crs as ccrs
     import matplotlib.dates as mdates
     import matplotlib.pyplot as plt
-except ModuleNotFoundError as err:
+except ModuleNotFoundError:
     warnings.warn(
         "gliderpy requires matplotlib and cartopy for plotting.",
         stacklevel=1,
     )
-    raise err
+    raise
 
 
-def plot_track(df):
-    """
-    Plots a track of glider path coloured by temperature
+if TYPE_CHECKING:
+    import pandas as pd
+
+
+def plot_track(df: pd.DataFrame) -> tuple(plt.Figure, plt.Axes):
+    """Plot a track of glider path coloured by temperature.
+
     :return: figures, axes
     """
-
     x = df["longitude (degrees_east)"]
     y = df["latitude (degrees_north)"]
     dx, dy = 2, 4
 
     fig, ax = plt.subplots(
         figsize=(9, 9),
         subplot_kw={"projection": ccrs.PlateCarree()},
     )
     ax.scatter(x, y, c=None, s=25, alpha=0.25, edgecolor="none")
     ax.coastlines("10m")
     ax.set_extent([x.min() - dx, x.max() + dx, y.min() - dy, y.max() + dy])
     return fig, ax
 
 
-def plot_transect(df, var, **kw):
-    """
-    Makes a scatter plot of depth vs time coloured by a user defined variable
+def plot_transect(
+    df: pd.DataFrame,
+    var: str,
+    **kw: dict,
+) -> tuple(plt.Figure, plt.Axes):
+    """Make a scatter plot of depth vs time coloured by a user defined
+    variable.
+
     :param var: variable to colour the scatter plot
     :return: figure, axes
     """
     cmap = kw.get("cmap", None)
 
     fig, ax = plt.subplots(figsize=(17, 2))
     cs = ax.scatter(
```

### Comparing `gliderpy-0.2.1/gliderpy/servers.py` & `gliderpy-0.2.2/gliderpy/servers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-"""
-Server names and aliases that point to an ERDDAP instance
-
-"""
+"""Server names and aliases that point to an ERDDAP instance."""
 
 server_vars = {
     "https://gliders.ioos.us/erddap": [
         "latitude",
         "longitude",
         "pressure",
         "profile_id",
```

### Comparing `gliderpy-0.2.1/pyproject.toml` & `gliderpy-0.2.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -12,19 +12,17 @@
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 maintainers = [
     {name = "Callum Rollo", email = "c.rollo@outlook.com"},
     {name = "Lindsay Abrams"},
     {name = "Filipe Fernandes"},
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "dependencies",
   "version",
@@ -43,41 +41,14 @@
 readme = {file = "README.md", content-type = "text/markdown"}
 
 [tool.setuptools_scm]
 write_to = "gliderpy/_version.py"
 write_to_template = "__version__ = '{version}'"
 tag_regex = "^(?P<prefix>v)?(?P<version>[^\\+]+)(?P<suffix>.*)?$"
 
-[tool.ruff]
-select = [
-    "A", # flake8-builtins
-    "B", # flake8-bugbear
-    "C4", # flake8-comprehensions
-    "F", # flakes
-    "I", # import sorting
-    "T20", # flake8-print
-    "UP", # upgrade
-    "ERA",  # flake8-eradicate/eradicate (remove commented out code)
-    "PIE",  # flake8-pie (misc lints)
-    "SIM",  # flake8-simplify (reduce code complexity)
-    "TID",  # flake8-tidy-imports
-    "TCH",  # flake8-type-checking
-    "N",  # pep8-naming
-    "RUF",  # Ruff-specific rules
-]
-target-version = "py38"
-line-length = 79
-
-[tool.ruff.per-file-ignores]
-"docs/source/conf.py" = [
-  "E402",
-  "A001",
-  "ERA001",
-]
-
 [tool.check-manifest]
 ignore = [
   "*.yml",
   "*.yaml",
   ".coveragerc",
   "docs",
   "docs/*",
```

