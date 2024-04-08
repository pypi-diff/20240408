# Comparing `tmp/idc-index-0.3.2.tar.gz` & `tmp/idc_index-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idc-index-0.3.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, last modified: Tue Mar 12 19:10:23 2024, max compression
```

## Comparing `idc-index-0.3.2.tar` & `idc_index-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,29 @@
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 idc-index-0.3.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 idc-index-0.3.2/.gitattributes
--rw-r--r--   0        0        0     2394 2022-11-09 12:37:21.000000 idc-index-0.3.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 idc-index-0.3.2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 idc-index-0.3.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1695 2022-11-09 12:37:21.000000 idc-index-0.3.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1517 2022-11-09 12:37:21.000000 idc-index-0.3.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 idc-index-0.3.2/.github/workflows/keep-alive.yaml
--rw-r--r--   0        0        0     2280 2022-11-09 12:37:21.000000 idc-index-0.3.2/.gitignore
--rw-r--r--   0        0        0     2358 2022-11-09 12:37:21.000000 idc-index-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 idc-index-0.3.2/.readthedocs.yaml
--rw-r--r--   0        0        0     2436 2022-11-09 12:37:21.000000 idc-index-0.3.2/CMakeLists.txt
--rw-r--r--   0        0        0     1077 2022-11-09 12:37:21.000000 idc-index-0.3.2/LICENSE
--rw-r--r--   0        0        0     4199 2022-11-09 12:37:21.000000 idc-index-0.3.2/README.md
--rw-r--r--   0        0        0      851 2022-11-09 12:37:21.000000 idc-index-0.3.2/docs/conf.py
--rw-r--r--   0        0        0      196 2022-11-09 12:37:21.000000 idc-index-0.3.2/docs/index.md
--rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 idc-index-0.3.2/idc_index/__init__.py
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 idc-index-0.3.2/idc_index/_version.py
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 idc-index-0.3.2/idc_index/_version.pyi
--rw-r--r--   0        0        0    25512 2022-11-09 12:37:21.000000 idc-index-0.3.2/idc_index/index.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 idc-index-0.3.2/idc_index/py.typed
--rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 idc-index-0.3.2/idc_index/s5cmd/__init__.py
--rw-r--r--   0        0        0     2742 2022-11-09 12:37:21.000000 idc-index-0.3.2/noxfile.py
--rw-r--r--   0        0        0     6484 2022-11-09 12:37:21.000000 idc-index-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1375 2022-11-09 12:37:21.000000 idc-index-0.3.2/queries/idc_index.sql
--rw-r--r--   0        0        0     2034 2022-11-09 12:37:21.000000 idc-index-0.3.2/s5cmdUrls.cmake
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 idc-index-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0     3595 2022-11-09 12:37:21.000000 idc-index-0.3.2/tests/idcindex.py
--rw-r--r--   0        0        0      413 2022-11-09 12:37:21.000000 idc-index-0.3.2/tests/study_manifest_aws.s5cmd
--rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 idc-index-0.3.2/tests/study_manifest_gcs.s5cmd
--rw-r--r--   0        0        0      175 2022-11-09 12:37:21.000000 idc-index-0.3.2/tests/test_package.py
--rw-r--r--   0        0        0     7409 2022-11-09 12:37:21.000000 idc-index-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-03-12 19:10:23.000000 idc_index-0.4.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-03-12 19:10:23.000000 idc_index-0.4.0/.gitattributes
+-rw-r--r--   0        0        0     2357 2024-03-12 19:10:23.000000 idc_index-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-03-12 19:10:23.000000 idc_index-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2024-03-12 19:10:23.000000 idc_index-0.4.0/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-03-12 19:10:23.000000 idc_index-0.4.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-03-12 19:10:23.000000 idc_index-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-03-12 19:10:23.000000 idc_index-0.4.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      847 2024-03-12 19:10:23.000000 idc_index-0.4.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1581 2024-03-12 19:10:23.000000 idc_index-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      355 2024-03-12 19:10:23.000000 idc_index-0.4.0/.github/workflows/keep-alive.yaml
+-rw-r--r--   0        0        0      851 2024-03-12 19:10:23.000000 idc_index-0.4.0/docs/conf.py
+-rw-r--r--   0        0        0      196 2024-03-12 19:10:23.000000 idc_index-0.4.0/docs/index.md
+-rw-r--r--   0        0        0      263 2024-03-12 19:10:23.000000 idc_index-0.4.0/idc_index/__init__.py
+-rw-r--r--   0        0        0      411 2024-03-12 19:10:23.000000 idc_index-0.4.0/idc_index/_version.py
+-rw-r--r--   0        0        0      118 2024-03-12 19:10:23.000000 idc_index-0.4.0/idc_index/_version.pyi
+-rw-r--r--   0        0        0    25055 2024-03-12 19:10:23.000000 idc_index-0.4.0/idc_index/index.py
+-rw-r--r--   0        0        0        0 2024-03-12 19:10:23.000000 idc_index-0.4.0/idc_index/py.typed
+-rw-r--r--   0        0        0     1383 2024-03-12 19:10:23.000000 idc_index-0.4.0/queries/idc_index.sql
+-rw-r--r--   0        0        0        0 2024-03-12 19:10:23.000000 idc_index-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3595 2024-03-12 19:10:23.000000 idc_index-0.4.0/tests/idcindex.py
+-rw-r--r--   0        0        0      413 2024-03-12 19:10:23.000000 idc_index-0.4.0/tests/study_manifest_aws.s5cmd
+-rw-r--r--   0        0        0      437 2024-03-12 19:10:23.000000 idc_index-0.4.0/tests/study_manifest_gcs.s5cmd
+-rw-r--r--   0        0        0      175 2024-03-12 19:10:23.000000 idc_index-0.4.0/tests/test_package.py
+-rw-r--r--   0        0        0     2265 2024-03-12 19:10:23.000000 idc_index-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1077 2024-03-12 19:10:23.000000 idc_index-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4290 2024-03-12 19:10:23.000000 idc_index-0.4.0/README.md
+-rw-r--r--   0        0        0     6138 2024-03-12 19:10:23.000000 idc_index-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7561 2024-03-12 19:10:23.000000 idc_index-0.4.0/PKG-INFO
```

### Comparing `idc-index-0.3.2/.github/CONTRIBUTING.md` & `idc_index-0.4.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc-index-0.3.2/.github/matchers/pylint.json` & `idc_index-0.4.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc-index-0.3.2/.github/workflows/ci.yml` & `idc_index-0.4.0/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -57,9 +57,11 @@
         run: python -m pip install .[test]
 
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20
 
-      - name: Upload coverage report
-        uses: codecov/codecov-action@v4.0.1
+#      - name: Upload coverage report
+#        uses: codecov/codecov-action@v4.1.0
+#        with:
+#          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `idc-index-0.3.2/.gitignore` & `idc_index-0.4.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -156,9 +156,8 @@
 Thumbs.db
 
 # Common editor files
 *~
 *.swp
 
 # idc-index
-*/s5cmd/s5cmd*
 */idc_index.csv.zip
```

### Comparing `idc-index-0.3.2/.pre-commit-config.yaml` & `idc_index-0.4.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     rev: "v3.1.0"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.1.15"
+    rev: "v0.2.2"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   #- repo: https://github.com/pre-commit/mirrors-mypy
   #  rev: "v1.8.0"
@@ -77,12 +77,12 @@
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: "v0.16"
     hooks:
       - id: validate-pyproject
         additional_dependencies: ["validate-pyproject-schema-store[all]"]
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: "0.27.3"
+    rev: "0.28.0"
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
```

### Comparing `idc-index-0.3.2/LICENSE` & `idc_index-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idc-index-0.3.2/README.md` & `idc_index-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 
 ## About
 
 `idc-index` is a Python package that enables query of the basic metadata and
 download of DICOM files hosted by the
 [NCI Imaging Data Commons (IDC)](https://imaging.datacommons.cancer.gov).
 
-## 👷‍♂️🚧 **WARNING**: this package is in its early development stages. Its functionality and API will change. Stay tuned for the updates and documentation, and please share your feedback about it by opening issues in this repository, or by starting a discussion in [IDC User forum](https://discourse.canceridc.dev/).🚧
+👷 🚧 This package is in its early development stages. Its functionality and API
+will change. Stay tuned for the updates and documentation, and please share your
+feedback about it by opening issues in this repository, or by starting a
+discussion in [IDC User forum](https://discourse.canceridc.dev/).🚧
 
 ## Usage
 
 There are no prerequisites - just install the package ...
 
 ```bash
 $ pip install idc-index
@@ -30,14 +33,16 @@
 PatientID/Study/Series as follows:
 
 ```python
 from idc_index import index
 
 client = index.IDCClient()
 
+all_collection_ids = client.get_collections()
+
 client.download_from_selection(collection_id="rider_pilot", downloadDir="/some/dir")
 ```
 
 ... or run queries against the "mini" index of Imaging Data Commons data!
 
 ```python
 from idc_index import index
@@ -74,15 +79,16 @@
 
 ## Resources
 
 - [Imaging Data Commons Portal](https://imaging.datacommons.cancer.gov/) can be
   used to explore the content of IDC from the web browser
 - [s5cmd](https://github.com/peak/s5cmd) is a highly efficient, open source,
   multi-platform S3 client that we use for downloading IDC data, which is hosted
-  in public AWS and GCS buckets
+  in public AWS and GCS buckets. Distributed on PyPI as
+  [s5cmd](https://pypi.org/project/s5cmd/).
 - [SlicerIDCBrowser](https://github.com/ImagingDataCommons/SlicerIDCBrowser) 3D
   Slicer extension that relies on `idc-index` for search and download of IDC
   data
 
 ## Acknowledgment
 
 This software is maintained by the IDC team, which has been funded in whole or
```

### Comparing `idc-index-0.3.2/docs/conf.py` & `idc_index-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc-index-0.3.2/idc_index/index.py` & `idc_index-0.4.0/idc_index/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,57 @@
 from __future__ import annotations
 
 import logging
 import os
 import re
 import shutil
 import subprocess
+import sys
 import tempfile
-import urllib.request
-from pathlib import Path
+
+if sys.version_info < (3, 10):
+    from importlib_metadata import distribution
+else:
+    from importlib.metadata import distribution
 
 import duckdb
+import idc_index_data
 import pandas as pd
 import psutil
 
-from ._version import version_tuple
-
 logger = logging.getLogger(__name__)
 
-idc_version = "v17"
-release_version = f"{version_tuple[0]}.{version_tuple[1]}.{version_tuple[2]}"
 aws_endpoint_url = "https://s3.amazonaws.com"
 gcp_endpoint_url = "https://storage.googleapis.com"
-latest_idc_index_csv_url = (
-    "https://github.com/ImagingDataCommons/idc-index/releases/download/"
-    + release_version
-    + "/idc_index.csv.zip"
-)
 
 
 class IDCClient:
     def __init__(self):
-        # If not found, download index file
-        current_dir = os.path.dirname(os.path.abspath(__file__))
-        file_path = os.path.join(current_dir, "idc_index.csv.zip")
-        if not os.path.exists(file_path):
-            logger.warning(
-                f"Index file not found. Downloading version {release_version} of the index file. This will take a minute or so."
-            )
-            urllib.request.urlretrieve(latest_idc_index_csv_url, file_path)
-            logger.warning(f"Index file v{release_version} downloaded.")
+        file_path = idc_index_data.IDC_INDEX_CSV_ARCHIVE_FILEPATH
 
         # Read index file
-        logger.debug(f"Reading index file v{release_version}")
+        logger.debug(f"Reading index file v{idc_index_data.__version__}")
         self.index = pd.read_csv(file_path, dtype=str, encoding="utf-8")
         self.index = self.index.astype(str).replace("nan", "")
         self.index["series_size_MB"] = self.index["series_size_MB"].astype(float)
         self.collection_summary = self.index.groupby("collection_id").agg(
             {"Modality": pd.Series.unique, "series_size_MB": "sum"}
         )
 
         # Lookup s5cmd
-        self.s5cmdPath = None
-
-        logger.debug("Checking if s5cmd is available in the package folder")
-        self.s5cmdPath = str(
-            next(Path(os.path.join(current_dir, "s5cmd")).glob("s5cmd*"), None)
-        )
+        self.s5cmdPath = shutil.which("s5cmd")
 
         if self.s5cmdPath is None:
-            logger.debug("Falling back to system s5cmd")
-            self.s5cmdPath = shutil.which("s5cmd")
+            # Workaround to support environment without a properly setup PATH
+            # See https://github.com/Slicer/Slicer/pull/7587
+            logger.debug("Falling back to looking up s5cmd along side the package")
+            for script in distribution("s5cmd").files:
+                if str(script).startswith("s5cmd/bin/s5cmd"):
+                    self.s5cmdPath = script.locate().resolve(strict=True)
+                    break
 
         if self.s5cmdPath is None:
             raise FileNotFoundError(
                 "s5cmd executable not found. Please install s5cmd from https://github.com/peak/s5cmd#installation"
             )
 
         self.s5cmdPath = str(self.s5cmdPath)
@@ -99,15 +87,15 @@
     @staticmethod
     def _filter_by_dicom_series_uid(df_index, dicom_series_uid):
         return IDCClient._filter_dataframe_by_id(
             "SeriesInstanceUID", df_index, dicom_series_uid
         )
 
     def get_idc_version(self):
-        return idc_version
+        return f"v{idc_index_data.__version__}"
 
     def get_collections(self):
         unique_collections = self.index["collection_id"].unique()
         return unique_collections.tolist()
 
     def get_series_size(self, seriesInstanceUID):
         resp = self.index[["SeriesInstanceUID"] == seriesInstanceUID][
```

### Comparing `idc-index-0.3.2/noxfile.py` & `idc_index-0.4.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc-index-0.3.2/pyproject.toml` & `idc_index-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
-requires = ["scikit-build-core"]
-build-backend = "scikit_build_core.build"
+requires = ["hatchling", "hatch-vcs"]
+build-backend = "hatchling.build"
 
 
 [project]
 name = "idc-index"
 authors = [
   { name = "Andrey Fedorov", email = "andrey.fedorov@gmail.com" },
   { name = "Vamsi Thiriveedhi", email = "vthiriveedhi@mgh.harvard.edu" },
@@ -28,22 +28,24 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
-  'duckdb;python_version<"3.12"',
-  'duckdb>0.9.2;python_version=="3.12"',
+  'duckdb>=0.10.0',
+  "idc-index-data",
   "pandas<2.2",
   "psutil",
+  "s5cmd",
 ]
 
 [project.optional-dependencies]
 test = [
+  "importlib_metadata>=2.0; python_version<'3.10'",
   "pytest >=6",
   "pytest-cov >=3",
 ]
 dev = [
   "pytest >=6",
   "pytest-cov >=3",
 ]
@@ -54,39 +56,25 @@
   "sphinx_autodoc_typehints",
   "furo>=2023.08.17",
 ]
 
 [project.urls]
 Homepage = "https://github.com/ImagingDataCommons/idc-index"
 "Bug Tracker" = "https://github.com/ImagingDataCommons/idc-index/issues"
-Discussions = "https://github.com/ImagingDataCommons/idc-index/discussions"
+Discussions = "https://discourse.canceridc.dev/"
 Changelog = "https://github.com/ImagingDataCommons/idc-index/releases"
 
-[project.scripts]
-s5cmd = "idc_index.s5cmd:s5cmd"
 
-
-[tool.scikit-build]
-minimum-version = "0.4"
-build-dir = "build/{wheel_tag}"
-metadata.version.provider = "scikit_build_core.metadata.setuptools_scm"
-sdist.include = ["idc_index/_version.py"]
-wheel.py-api = "py3"
-wheel.expand-macos-universal-tags = true
-
-
-[tool.setuptools_scm]
-version_scheme = "no-guess-dev"
-write_to = "idc_index/_version.py"
-
-
-[tool.cibuildwheel]
-test-command = "pytest {project}/tests"
-test-extras = ["test"]
-test-skip = ["*universal2:arm64"]
+[tool.hatch]
+version.source = "vcs"
+build.hooks.vcs.version-file = "idc_index/_version.py"
+
+[tool.hatch.envs.default]
+features = ["test"]
+scripts.test = "pytest {args}"
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = [
```

### Comparing `idc-index-0.3.2/queries/idc_index.sql` & `idc_index-0.4.0/queries/idc_index.sql`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,14 @@
   ANY_VALUE(SeriesNumber) AS SeriesNumber,
   COUNT(dicom_all.SOPInstanceUID) AS instanceCount,
   ANY_VALUE(license_short_name) as license_short_name,
   # download related attributes
   ANY_VALUE(CONCAT("s3://", aws_bucket, "/", crdc_series_uuid, "/*")) AS series_aws_url,
   ROUND(SUM(SAFE_CAST(instance_size AS float64))/1000000, 2) AS series_size_MB,
 FROM
-  bigquery-public-data.idc_v17.dicom_all AS dicom_all
+  bigquery-public-data.idc_current.dicom_all AS dicom_all
 JOIN
-  bigquery-public-data.idc_v17.dicom_metadata_curated AS dicom_curated
+  bigquery-public-data.idc_current.dicom_metadata_curated AS dicom_curated
 ON
   dicom_all.SOPInstanceUID = dicom_curated.SOPInstanceUID
 GROUP BY
   SeriesInstanceUID
```

### Comparing `idc-index-0.3.2/tests/idcindex.py` & `idc_index-0.4.0/tests/idcindex.py`

 * *Files identical despite different names*

### Comparing `idc-index-0.3.2/PKG-INFO` & `idc_index-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: idc-index
-Version: 0.3.2
+Version: 0.4.0
 Summary: Package to query and download data from an index of ImagingDataCommons
-Author-Email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
+Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
+Project-URL: Bug Tracker, https://github.com/ImagingDataCommons/idc-index/issues
+Project-URL: Discussions, https://discourse.canceridc.dev/
+Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
+Author-email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
 License: MIT License
         
         Copyright (c) 2023 Imaging Data Commons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
@@ -20,50 +24,49 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
-Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
-Project-URL: Bug tracker, https://github.com/ImagingDataCommons/idc-index/issues
-Project-URL: Discussions, https://github.com/ImagingDataCommons/idc-index/discussions
-Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
 Requires-Python: >=3.8
-Requires-Dist: duckdb; python_version < "3.12"
-Requires-Dist: duckdb>0.9.2; python_version == "3.12"
+Requires-Dist: duckdb>=0.10.0
+Requires-Dist: idc-index-data
 Requires-Dist: pandas<2.2
 Requires-Dist: psutil
-Requires-Dist: pytest>=6; extra == "test"
-Requires-Dist: pytest-cov>=3; extra == "test"
-Requires-Dist: pytest>=6; extra == "dev"
-Requires-Dist: pytest-cov>=3; extra == "dev"
-Requires-Dist: sphinx>=7.0; extra == "docs"
-Requires-Dist: myst_parser>=0.13; extra == "docs"
-Requires-Dist: sphinx_copybutton; extra == "docs"
-Requires-Dist: sphinx_autodoc_typehints; extra == "docs"
-Requires-Dist: furo>=2023.08.17; extra == "docs"
-Provides-Extra: test
+Requires-Dist: s5cmd
 Provides-Extra: dev
+Requires-Dist: pytest-cov>=3; extra == 'dev'
+Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
+Requires-Dist: furo>=2023.08.17; extra == 'docs'
+Requires-Dist: myst-parser>=0.13; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
+Requires-Dist: sphinx-copybutton; extra == 'docs'
+Requires-Dist: sphinx>=7.0; extra == 'docs'
+Provides-Extra: test
+Requires-Dist: importlib-metadata>=2.0; (python_version < '3.10') and extra == 'test'
+Requires-Dist: pytest-cov>=3; extra == 'test'
+Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
 # idc-index
 
 [![Actions Status][actions-badge]][actions-link]
 [![Documentation Status][rtd-badge]][rtd-link]
 
@@ -76,15 +79,18 @@
 
 ## About
 
 `idc-index` is a Python package that enables query of the basic metadata and
 download of DICOM files hosted by the
 [NCI Imaging Data Commons (IDC)](https://imaging.datacommons.cancer.gov).
 
-## 👷‍♂️🚧 **WARNING**: this package is in its early development stages. Its functionality and API will change. Stay tuned for the updates and documentation, and please share your feedback about it by opening issues in this repository, or by starting a discussion in [IDC User forum](https://discourse.canceridc.dev/).🚧
+👷 🚧 This package is in its early development stages. Its functionality and API
+will change. Stay tuned for the updates and documentation, and please share your
+feedback about it by opening issues in this repository, or by starting a
+discussion in [IDC User forum](https://discourse.canceridc.dev/).🚧
 
 ## Usage
 
 There are no prerequisites - just install the package ...
 
 ```bash
 $ pip install idc-index
@@ -94,14 +100,16 @@
 PatientID/Study/Series as follows:
 
 ```python
 from idc_index import index
 
 client = index.IDCClient()
 
+all_collection_ids = client.get_collections()
+
 client.download_from_selection(collection_id="rider_pilot", downloadDir="/some/dir")
 ```
 
 ... or run queries against the "mini" index of Imaging Data Commons data!
 
 ```python
 from idc_index import index
@@ -138,15 +146,16 @@
 
 ## Resources
 
 - [Imaging Data Commons Portal](https://imaging.datacommons.cancer.gov/) can be
   used to explore the content of IDC from the web browser
 - [s5cmd](https://github.com/peak/s5cmd) is a highly efficient, open source,
   multi-platform S3 client that we use for downloading IDC data, which is hosted
-  in public AWS and GCS buckets
+  in public AWS and GCS buckets. Distributed on PyPI as
+  [s5cmd](https://pypi.org/project/s5cmd/).
 - [SlicerIDCBrowser](https://github.com/ImagingDataCommons/SlicerIDCBrowser) 3D
   Slicer extension that relies on `idc-index` for search and download of IDC
   data
 
 ## Acknowledgment
 
 This software is maintained by the IDC team, which has been funded in whole or
```

