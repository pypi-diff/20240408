# Comparing `tmp/burst2safe-0.1.0.tar.gz` & `tmp/burst2safe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burst2safe-0.1.0.tar", last modified: Wed Mar 27 20:41:25 2024, max compression
+gzip compressed data, was "burst2safe-0.2.0.tar", last modified: Mon Apr  8 14:38:46 2024, max compression
```

## Comparing `burst2safe-0.1.0.tar` & `burst2safe-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:41:25.202970 burst2safe-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:41:25.190970 burst2safe-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:41:25.190970 burst2safe-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.github/workflows/build-and-deploy-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.github/workflows/build-and-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.github/workflows/bump-version.yml
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.github/workflows/changelog-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.github/workflows/labeled-pr-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.github/workflows/release-checklist-comment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-27 20:41:15.000000 burst2safe-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-27 20:41:15.000000 burst2safe-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-27 20:41:15.000000 burst2safe-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-03-27 20:41:25.202970 burst2safe-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-03-27 20:41:15.000000 burst2safe-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-27 20:41:15.000000 burst2safe-0.1.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-27 20:41:15.000000 burst2safe-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 20:41:25.202970 burst2safe-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:41:25.190970 burst2safe-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:41:25.194970 burst2safe-0.1.0/src/burst2safe/
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/burst2safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:41:25.194970 burst2safe-0.1.0/src/burst2safe/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/data/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/data/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/data/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/data/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    60608 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/data/s1-object-types.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/product.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-03-27 20:41:15.000000 burst2safe-0.1.0/src/burst2safe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:41:25.202970 burst2safe-0.1.0/src/burst2safe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-03-27 20:41:25.000000 burst2safe-0.1.0/src/burst2safe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-27 20:41:25.000000 burst2safe-0.1.0/src/burst2safe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 20:41:25.000000 burst2safe-0.1.0/src/burst2safe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-27 20:41:25.000000 burst2safe-0.1.0/src/burst2safe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 20:41:24.000000 burst2safe-0.1.0/src/burst2safe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 20:41:25.000000 burst2safe-0.1.0/src/burst2safe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-27 20:41:25.000000 burst2safe-0.1.0/src/burst2safe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:41:25.194970 burst2safe-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-27 20:41:15.000000 burst2safe-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-03-27 20:41:15.000000 burst2safe-0.1.0/tests/test_burst2safe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:41:25.194970 burst2safe-0.1.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)  6011546 2024-03-27 20:41:15.000000 burst2safe-0.1.0/tests/test_data/S1A_IW_SLC__1SDV_20200604T022251_20200604T022318_032861_03CE65_7C85_VV.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:38:46.122131 burst2safe-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:38:46.106130 burst2safe-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:38:46.106130 burst2safe-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.github/workflows/build-and-deploy-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.github/workflows/build-and-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.github/workflows/bump-version.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.github/workflows/changelog-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.github/workflows/labeled-pr-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.github/workflows/release-checklist-comment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-08 14:38:41.000000 burst2safe-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-08 14:38:41.000000 burst2safe-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-08 14:38:41.000000 burst2safe-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-08 14:38:46.122131 burst2safe-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-08 14:38:41.000000 burst2safe-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 14:38:41.000000 burst2safe-0.2.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-08 14:38:41.000000 burst2safe-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:38:46.122131 burst2safe-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:38:46.102131 burst2safe-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:38:46.106130 burst2safe-0.2.0/src/burst2safe/
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/burst2safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:38:46.110131 burst2safe-0.2.0/src/burst2safe/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/data/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/data/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/data/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/data/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    60608 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/data/s1-object-types.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/swath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-08 14:38:41.000000 burst2safe-0.2.0/src/burst2safe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:38:46.118131 burst2safe-0.2.0/src/burst2safe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-08 14:38:46.000000 burst2safe-0.2.0/src/burst2safe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-08 14:38:46.000000 burst2safe-0.2.0/src/burst2safe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:38:46.000000 burst2safe-0.2.0/src/burst2safe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 14:38:46.000000 burst2safe-0.2.0/src/burst2safe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:38:45.000000 burst2safe-0.2.0/src/burst2safe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 14:38:46.000000 burst2safe-0.2.0/src/burst2safe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 14:38:46.000000 burst2safe-0.2.0/src/burst2safe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:38:46.114131 burst2safe-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_burst2safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:38:46.118131 burst2safe-0.2.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)  6011546 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_data/S1A_IW_SLC__1SDV_20200604T022251_20200604T022318_032861_03CE65_7C85_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36523 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_data/manifest_7C85.safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_swath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-08 14:38:41.000000 burst2safe-0.2.0/tests/test_utils.py
```

### Comparing `burst2safe-0.1.0/.github/workflows/build-and-deploy-test.yml` & `burst2safe-0.2.0/.github/workflows/build-and-deploy-test.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.1.0/.github/workflows/build-and-deploy.yml` & `burst2safe-0.2.0/.github/workflows/build-and-deploy.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.1.0/.github/workflows/static-analysis.yml` & `burst2safe-0.2.0/.github/workflows/static-analysis.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.1.0/.gitignore` & `burst2safe-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `burst2safe-0.1.0/LICENSE` & `burst2safe-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `burst2safe-0.1.0/PKG-INFO` & `burst2safe-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst2safe
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format
 Author-email: Forrest Williams <ffwilliams2@alaska.edu>
 Project-URL: Homepage, https://github.com/forrestfwilliams/burst2safe
 Project-URL: Bug Tracker, https://github.com/forrestfwilliams/burst2safe/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,14 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gdal
 Requires-Dist: numpy
 Requires-Dist: lxml
 Requires-Dist: asf_search
-Requires-Dist: crcmod
 Provides-Extra: develop
 Requires-Dist: pytest; extra == "develop"
 
 # burst2safe
 Utility for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format.
 
 **This is still a work in progress, and we recommend waiting until the release of version 1.0.0 for use in production environments!**
@@ -36,28 +35,40 @@
 ```
 
 Or conda:
 ```bash
 conda install -c conda-forge burst2safe
 ```
 
-Then provide a list of Sentinel-1 burst granule IDs to be merged into a SAFE file to the `burst2safe` CLI tool using the following structure:
+Then, run the `burst2safe` command line tool using the following structure:
+```bash
+burst2safe --orbit 32861 --bbox 53.57 27.54 53.78 27.60 --pols VV VH
+```
+Where:
 
+* `--orbit` is the absolute orbit number of the Sentinel-1 data.
+* `--bbox` is the bounding box of the area of interest in the format `minlon minlat maxlon maxlat`.
+* `--pols` is the polarization of the Sentinel-1 data. Options are `VV`, `VH`, `HV`, and `HH`.
+
+For more control over the burst group, you can also provide specific burst granule IDs to be merged into a SAFE file using the following structure:
 ```bash
-burst2safe S1_136231_IW2_20200604T022312_VV_7C85-BURST S1_136232_IW2_20200604T022315_VV_7C85-BURST
+burst2safe S1_136231_IW2_20200604T022312_VV_7C85-BURST S1_136232_IW2_20200604T022315_VV_7C85-BURST S1_136231_IW2_20200604T022312_VH_7C85-BURST S1_136232_IW2_20200604T022315_VH_7C85-BURST
 ```
-The output SAFE file will be created in the current directory.
+This search is equivalent to the previous search.
 To be eligible for processing, all burst granules must:
+
 1. Have the same acquisition mode
-1. Be in the same polarization
 1. Be from the same absolute orbit
 1. Be contiguous in time and space.
+1. Have the same footprint for all polarizations.
 
 The tool should raise an error if any of these conditions are not met.
 
+The output SAFE file will be created in the current directory.
+
 ## Strategy
 `burst2safe` combines and reformats individual bursts into a SAFE file following the procedure described in the [Sentinel-1 Product Specification Document](https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/document-library/-/asset_publisher/1dO7RF5fJMbd/content/sentinel-1-product-specification-from-ipf-360?_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId=4846613&_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_redirect=https%3A%2F%2Fsentinel.esa.int%2Fweb%2Fsentinel%2Fuser-guides%2Fsentinel-1-sar%2Fdocument-library%3Fp_p_id%3Dcom_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId%3D4846613%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_cur%3D0%26p_r_p_resetCur%3Dfalse)
 In this document, ESA describes how to create an Assembled Sentinel-1 Level 1 product from individual Sentinel-1 Level 1 SAFEs. We use this same strategy to combine ASF-extracted burst SLC products into a SAFE file that should be compatible with any SAR processor currently capable of using Sentinel-1 Level SAFEs. For in-depth technical details of the implementation, we refer you to the Sentinel-1 Product Specification document above. However, it is important to know that ESA recommends merging Sentinel-1 data/metadata components using three primary strategies:
 
 ### Include
 A given data/metadata component is the same for all data slices, and any value can be used (i.e., polarization).
 
@@ -116,8 +127,8 @@
 ## Contact Us
 Want to talk about `burst2safe`? We would love to hear from you!
 
 Found a bug? Want to request a feature?
 [open an issue](https://github.com/ASFHyP3/asf_tools/issues/new)
 
 General questions? Suggestions? Or just want to talk to the team?
-[chat with us on burst2safe's discussion page](https://github.com/forrestfwilliams/burst2safe/discussions) 
+[chat with us on burst2safe's discussion page](https://github.com/forrestfwilliams/burst2safe/discussions)
```

### Comparing `burst2safe-0.1.0/README.md` & `burst2safe-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,40 @@
 ```
 
 Or conda:
 ```bash
 conda install -c conda-forge burst2safe
 ```
 
-Then provide a list of Sentinel-1 burst granule IDs to be merged into a SAFE file to the `burst2safe` CLI tool using the following structure:
+Then, run the `burst2safe` command line tool using the following structure:
+```bash
+burst2safe --orbit 32861 --bbox 53.57 27.54 53.78 27.60 --pols VV VH
+```
+Where:
 
+* `--orbit` is the absolute orbit number of the Sentinel-1 data.
+* `--bbox` is the bounding box of the area of interest in the format `minlon minlat maxlon maxlat`.
+* `--pols` is the polarization of the Sentinel-1 data. Options are `VV`, `VH`, `HV`, and `HH`.
+
+For more control over the burst group, you can also provide specific burst granule IDs to be merged into a SAFE file using the following structure:
 ```bash
-burst2safe S1_136231_IW2_20200604T022312_VV_7C85-BURST S1_136232_IW2_20200604T022315_VV_7C85-BURST
+burst2safe S1_136231_IW2_20200604T022312_VV_7C85-BURST S1_136232_IW2_20200604T022315_VV_7C85-BURST S1_136231_IW2_20200604T022312_VH_7C85-BURST S1_136232_IW2_20200604T022315_VH_7C85-BURST
 ```
-The output SAFE file will be created in the current directory.
+This search is equivalent to the previous search.
 To be eligible for processing, all burst granules must:
+
 1. Have the same acquisition mode
-1. Be in the same polarization
 1. Be from the same absolute orbit
 1. Be contiguous in time and space.
+1. Have the same footprint for all polarizations.
 
 The tool should raise an error if any of these conditions are not met.
 
+The output SAFE file will be created in the current directory.
+
 ## Strategy
 `burst2safe` combines and reformats individual bursts into a SAFE file following the procedure described in the [Sentinel-1 Product Specification Document](https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/document-library/-/asset_publisher/1dO7RF5fJMbd/content/sentinel-1-product-specification-from-ipf-360?_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId=4846613&_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_redirect=https%3A%2F%2Fsentinel.esa.int%2Fweb%2Fsentinel%2Fuser-guides%2Fsentinel-1-sar%2Fdocument-library%3Fp_p_id%3Dcom_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId%3D4846613%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_cur%3D0%26p_r_p_resetCur%3Dfalse)
 In this document, ESA describes how to create an Assembled Sentinel-1 Level 1 product from individual Sentinel-1 Level 1 SAFEs. We use this same strategy to combine ASF-extracted burst SLC products into a SAFE file that should be compatible with any SAR processor currently capable of using Sentinel-1 Level SAFEs. For in-depth technical details of the implementation, we refer you to the Sentinel-1 Product Specification document above. However, it is important to know that ESA recommends merging Sentinel-1 data/metadata components using three primary strategies:
 
 ### Include
 A given data/metadata component is the same for all data slices, and any value can be used (i.e., polarization).
 
@@ -91,8 +103,8 @@
 ## Contact Us
 Want to talk about `burst2safe`? We would love to hear from you!
 
 Found a bug? Want to request a feature?
 [open an issue](https://github.com/ASFHyP3/asf_tools/issues/new)
 
 General questions? Suggestions? Or just want to talk to the team?
-[chat with us on burst2safe's discussion page](https://github.com/forrestfwilliams/burst2safe/discussions) 
+[chat with us on burst2safe's discussion page](https://github.com/forrestfwilliams/burst2safe/discussions)
```

### Comparing `burst2safe-0.1.0/pyproject.toml` & `burst2safe-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "gdal",
   "numpy",
   "lxml",
   "asf_search",
-  "crcmod",
 ]
 
 [project.urls]
 Homepage = "https://github.com/forrestfwilliams/burst2safe"
 "Bug Tracker" ="https://github.com/forrestfwilliams/burst2safe/issues"
 
 [project.scripts]
```

### Comparing `burst2safe-0.1.0/src/burst2safe/calibration.py` & `burst2safe-0.2.0/src/burst2safe/calibration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 from copy import deepcopy
 from typing import Iterable
 
 import lxml.etree as ET
 
-from burst2safe.base import Annotation, ListOfListElements
+from burst2safe.base import Annotation
 from burst2safe.utils import BurstInfo
 
 
 class Calibration(Annotation):
+    """Class representing a calibration XML."""
+
     def __init__(self, burst_infos: Iterable[BurstInfo], image_number: int):
+        """Create a calibration object.
+
+        Args:
+            burst_infos: List of BurstInfo objects.
+            image_number: Image number.
+        """
         super().__init__(burst_infos, 'calibration', image_number)
         self.calibration_information = None
         self.calibrattion_vector_list = None
 
     def create_calibration_information(self):
+        """Create the calibration information."""
         calibration_information = [calibration.find('calibrationInformation') for calibration in self.inputs][0]
         self.calibration_information = deepcopy(calibration_information)
 
     def create_calibration_vector_list(self):
-        cal_vectors = [cal.find('calibrationVectorList') for cal in self.inputs]
-        cal_vector_lol = ListOfListElements(cal_vectors, self.start_line, self.slc_lengths)
-        self.calibration_vector_list = cal_vector_lol.create_filtered_list([self.min_anx, self.max_anx])
+        """Create the calibration vector list."""
+        self.calibration_vector_list = self.merge_lists('calibrationVectorList')
 
     def assemble(self):
+        """Assemble the calibration object components."""
         self.create_ads_header()
         self.create_calibration_information()
         self.create_calibration_vector_list()
 
         calibration = ET.Element('calibration')
         calibration.append(self.ads_header)
         calibration.append(self.calibration_information)
```

### Comparing `burst2safe-0.1.0/src/burst2safe/data/s1-level-1-calibration.xsd` & `burst2safe-0.2.0/src/burst2safe/data/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.1.0/src/burst2safe/data/s1-level-1-noise.xsd` & `burst2safe-0.2.0/src/burst2safe/data/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.1.0/src/burst2safe/data/s1-level-1-product.xsd` & `burst2safe-0.2.0/src/burst2safe/data/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.1.0/src/burst2safe/data/s1-object-types.xsd` & `burst2safe-0.2.0/src/burst2safe/data/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.1.0/src/burst2safe/measurement.py` & `burst2safe-0.2.0/src/burst2safe/measurement.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,99 @@
 import hashlib
 from datetime import datetime
 from pathlib import Path
-from typing import Iterable
+from typing import Iterable, Tuple
 
-import lxml.etree as ET
 import numpy as np
 from osgeo import gdal, osr
 
-from burst2safe.product import Product
+from burst2safe.base import create_content_unit, create_data_object
+from burst2safe.product import GeoPoint
 from burst2safe.utils import BurstInfo, get_subxml_from_metadata
 
 
 class Measurement:
-    def __init__(self, burst_infos: Iterable[BurstInfo], product_obj: Product, image_number: int):
+    """Class representing a measurement GeoTIFF."""
+
+    def __init__(self, burst_infos: Iterable[BurstInfo], gcps: Iterable[GeoPoint], image_number: int):
+        """Initialize a Measurement object.
+
+        Args:
+            burst_infos: A list of BurstInfo objects
+            gcps: A list of GeoPoint objects
+            image_number: The image number of the measurement
+        """
         self.burst_infos = burst_infos
-        self.product = product_obj
+        self.gcps = gcps
         self.image_number = image_number
-        self.swath = burst_infos[0].swath
-        self.burst_length = burst_infos[0].length
-        self.burst_width = burst_infos[0].width
+
+        self.swath = self.burst_infos[0].swath
+        self.burst_length = self.burst_infos[0].length
+        self.burst_width = self.burst_infos[0].width
         self.total_width = self.burst_width
-        self.total_length = self.burst_length * len(burst_infos)
+        self.total_length = self.burst_length * len(self.burst_infos)
         self.data_mean = None
         self.data_std = None
+        self.size_bytes = None
+        self.md5 = None
 
     def get_data(self, band: int = 1) -> np.ndarray:
+        """Get the data from the measurement from ASF burst GeoTIFFs.
+
+        Args:
+            band: The GeoTIFF band to read
+
+        Returns:
+            The data from burst GeoTIFFs as a numpy array
+        """
         data = np.zeros((self.total_length, self.total_width), dtype=np.complex64)
         for i, burst_info in enumerate(self.burst_infos):
             ds = gdal.Open(str(burst_info.data_path))
             data[i * self.burst_length : (i + 1) * self.burst_length, :] = ds.GetRasterBand(band).ReadAsArray()
             ds = None
         return data
 
-    def add_metadata(self, ds):
-        gcps = self.product.gcps
-        gdal_gcps = [gdal.GCP(gcp.x, gcp.y, gcp.z, gcp.pixel, gcp.line) for gcp in gcps]
+    @staticmethod
+    def get_ipf_version(metadata_path: Path) -> str:
+        """Get the IPF version from the parent manifest file.
+
+        Returns:
+            The IPF version as a string
+        """
+        manifest = get_subxml_from_metadata(metadata_path, 'manifest')
+        version_xml = [elem for elem in manifest.findall('.//{*}software') if elem.get('name') == 'Sentinel-1 IPF'][0]
+        return version_xml.get('version')
+
+    def add_metadata(self, dataset: gdal.Dataset):
+        """Add metadata to an existing GDAL dataset.
+
+        Args:
+            dataset: The GDAL dataset to add metadata to
+        """
+        gdal_gcps = [gdal.GCP(gcp.x, gcp.y, gcp.z, gcp.pixel, gcp.line) for gcp in self.gcps]
         srs = osr.SpatialReference()
         srs.ImportFromEPSG(4326)
+        dataset.SetGCPs(gdal_gcps, srs.ExportToWkt())
 
-        manifest = get_subxml_from_metadata(self.burst_infos[0].metadata_path, 'manifest')[1]
-        software = 'Sentinel-1 IPF'
-        version_xml = [elem for elem in manifest.findall('.//{*}software') if elem.get('name') == software][0]
-        software_version = f'{software} {version_xml.get("version")}'
-
-        ds.SetGCPs(gdal_gcps, srs.ExportToWkt())
-        ds.SetMetadataItem('TIFFTAG_DATETIME', datetime.strftime(datetime.now(), '%Y:%m:%d %H:%M:%S'))
+        dataset.SetMetadataItem('TIFFTAG_DATETIME', datetime.strftime(datetime.now(), '%Y:%m:%d %H:%M:%S'))
         # TODO make sure A/B is being set correctly.
-        ds.SetMetadataItem('TIFFTAG_IMAGEDESCRIPTION', 'Sentinel-1A IW SLC L1')
-        ds.SetMetadataItem('TIFFTAG_IMAGEDESCRIPTION', 'Sentinel-1A IW SLC L1')
-        ds.SetMetadataItem('TIFFTAG_SOFTWARE', software_version)
+        dataset.SetMetadataItem('TIFFTAG_IMAGEDESCRIPTION', 'Sentinel-1A IW SLC L1')
+
+        version = self.get_ipf_version(self.burst_infos[0].metadata_path)
+        software_version = f'Sentinel-1 IPF {version}'
+        dataset.SetMetadataItem('TIFFTAG_SOFTWARE', software_version)
 
     def create_geotiff(self, out_path: Path, update_info=True):
+        """Create a GeoTIFF of SLC data from the constituent burst SLC GeoTIFFs.
+        Optionally update Measurment metadata.
+
+        Args:
+            out_path: The path to write the SLC GeoTIFF to
+            update_info: Whether to update the Measurement metadata
+        """
         mem_drv = gdal.GetDriverByName('MEM')
         mem_ds = mem_drv.Create('', self.total_width, self.total_length, 1, gdal.GDT_CInt16)
         data = self.get_data()
         band = mem_ds.GetRasterBand(1)
         band.WriteArray(data)
         band.SetNoDataValue(0)
         self.add_metadata(mem_ds)
@@ -65,41 +104,29 @@
             self.data_mean = np.mean(data[data != 0])
             self.data_std = np.std(data[data != 0])
             with open(self.path, 'rb') as f:
                 file_bytes = f.read()
                 self.size_bytes = len(file_bytes)
                 self.md5 = hashlib.md5(file_bytes).hexdigest()
 
-    def create_manifest_components(self):
-        unit_type = 'Measurement Data Unit'
-        mime_type = 'application/octet-stream'
+    def create_manifest_components(self) -> Tuple:
+        """Create the components of the SAFE manifest for the measurement file.
 
-        schema = '{urn:ccsds:schema:xfdu:1}'
-        rep_id = 's1Level1MeasurementSchema'
+        Returns:
+            A tuple of the content unit and data object for the measurement file
+        """
         simple_name = self.path.with_suffix('').name.replace('-', '')
-
-        content_unit = ET.Element(f'{schema}contentUnit')
-        content_unit.set('unitType', unit_type)
-        content_unit.set('repID', rep_id)
-        ET.SubElement(content_unit, 'dataObjectPointer', dataObjectID=simple_name)
+        rep_id = 's1Level1MeasurementSchema'
+        unit_type = 'Measurement Data Unit'
+        mime_type = 'application/octet-stream'
 
         safe_index = [i for i, x in enumerate(self.path.parts) if 'SAFE' in x][-1]
         safe_path = Path(*self.path.parts[: safe_index + 1])
         relative_path = self.path.relative_to(safe_path)
 
-        data_object = ET.Element('dataObject')
-        data_object.set('ID', simple_name)
-        data_object.set('repID', rep_id)
-        byte_stream = ET.SubElement(data_object, 'byteStream')
-        byte_stream.set('mimeType', mime_type)
-        byte_stream.set('size', str(self.size_bytes))
-        file_location = ET.SubElement(byte_stream, 'fileLocation')
-        file_location.set('locatorType', 'URL')
-        file_location.set('href', f'./{relative_path}')
-        checksum = ET.SubElement(byte_stream, 'checksum')
-        checksum.set('checksumName', 'MD5')
-        checksum.text = self.md5
-
+        content_unit = create_content_unit(simple_name, rep_id, unit_type)
+        data_object = create_data_object(simple_name, relative_path, rep_id, mime_type, self.size_bytes, self.md5)
         return content_unit, data_object
 
     def write(self, out_path):
+        """Write the measurement GeoTIFF to a file."""
         self.create_geotiff(out_path)
```

### Comparing `burst2safe-0.1.0/src/burst2safe/product.py` & `burst2safe-0.2.0/src/burst2safe/product.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,51 +8,65 @@
 
 from burst2safe.base import Annotation, ListOfListElements
 from burst2safe.utils import BurstInfo, flatten
 
 
 @dataclass
 class GeoPoint:
+    """A geolocation grid point."""
+
     x: float
     y: float
     z: float
     line: int
     pixel: int
 
 
 class Product(Annotation):
+    """Class representing a product XML."""
+
     def __init__(self, burst_infos: Iterable[BurstInfo], image_number: int):
+        """Create a Product object.
+
+        Args:
+            burst_infos: A list of BurstInfo objects
+            image_number: The image number
+        """
         super().__init__(burst_infos, 'product', image_number)
         self.qulatity_information = None
         self.general_annotation = None
         self.image_annotation = None
         self.doppler_centroid = None
         self.antenna_pattern = None
         self.swath_timing = None
         self.geolocation_grid = None
         self.coordinate_conversion = None
         self.swath_merging = None
         self.gcps = []
 
     def create_quality_information(self):
+        """Create the qualityInformation element."""
         quality_information = ET.Element('qualityInformation')
         quality_information.append(deepcopy(self.inputs[0].find('qualityInformation/productQualityIndex')))
 
         quality_datas = flatten([cal.findall('qualityInformation/qualityDataList/qualityData') for cal in self.inputs])
         quality_data_list = ET.Element('qualityDataList')
         quality_data_list.set('count', str(len(quality_datas)))
         for quality_data in quality_datas:
             quality_data_list.append(deepcopy(quality_data))
 
         quality_information.append(quality_data_list)
 
         self.quality_information = quality_information
 
     def create_general_annotation(self):
-        """The productInformation sub-record contains single value fields that
+        """Create the generalAnnotation element.
+
+        From product specification:
+        The productInformation sub-record contains single value fields that
         are merged and included. All other sub-records contain lists which are
         concatenated. Details are presented in Table 3-11."""
         general_annotation = ET.Element('generalAnnotation')
 
         product_information = deepcopy(self.inputs[0].find('generalAnnotation/productInformation'))
         # TODO: productInformation/platformHeading should be calculated more accurately
         product_information.find('platformHeading').text = ''
@@ -68,28 +82,31 @@
             'terrainHeightList',
             'azimuthFmRateList',
         ]
         for list_name in lists:
             list_elements = [prod.find(f'generalAnnotation/{list_name}') for prod in self.inputs]
             if list_name == 'replicaInformationList':
                 lol = ListOfListElements(list_elements, self.start_line, self.slc_lengths)
-                unique = lol.get_nonduplicate_elements()
+                unique = lol.get_unique_elements()
                 filtered = ET.Element('replicaInformationList')
                 filtered.set('count', str(len(unique)))
                 [filtered.append(element) for element in unique]
             else:
                 lol = ListOfListElements(list_elements, self.start_line, self.slc_lengths)
                 filtered = lol.create_filtered_list([self.min_anx, self.max_anx], buffer=timedelta(seconds=500))
 
             general_annotation.append(filtered)
 
         self.general_annotation = general_annotation
 
     def create_image_annotation(self):
-        """This DSR contains two records which contain only single value fields.
+        """Create the imageAnnotation element.
+
+        From product specification:
+        This DSR contains two records which contain only single value fields.
         The fields in the imageInformation record are included and merged
         and all the fields for the processingInformation record are included;
         except for the inputDimensionsList record, which is concatenated.
         Details are presented in Table 3-12."""
         image_annotation = ET.Element('imageAnnotation')
 
         image_information = deepcopy(self.inputs[0].find('imageAnnotation/imageInformation'))
@@ -125,44 +142,47 @@
         lol = ListOfListElements(list_elements, self.start_line, self.slc_lengths)
         filtered = lol.create_filtered_list([self.min_anx, self.max_anx])
         [dimensions_list.append(element) for element in filtered]
 
         image_annotation.append(processing_information)
         self.image_annotation = image_annotation
 
-    def update_data_stats(self, data_mean, data_std):
+    def update_data_stats(self, data_mean: np.complex64, data_std: np.complex64):
+        """Update the data statistics in the imageAnnotation element.
+
+        Args:
+            data_mean: The complex mean of the data.
+            data_std: The complex standard deviation of the data.
+        """
         base_path = 'imageInformation/imageStatistics/outputData'
         data_mean_re = f'{data_mean.real:.6e}'
         data_mean_im = f'{data_mean.imag:.6e}'
         data_std_re = f'{data_std.real:.6e}'
         data_std_im = f'{data_std.imag:.6e}'
 
         for elem in [self.image_annotation, self.xml.find('imageAnnotation')]:
             elem.find(f'{base_path}Mean/re').text = data_mean_re
             elem.find(f'{base_path}Mean/im').text = data_mean_im
             elem.find(f'{base_path}StdDev/re').text = data_std_re
             elem.find(f'{base_path}StdDev/im').text = data_std_im
 
     def create_doppler_centroid(self):
-        dc_lists = [prod.find('dopplerCentroid/dcEstimateList') for prod in self.inputs]
-        dc_lol = ListOfListElements(dc_lists, self.start_line, self.slc_lengths)
-        filtered = dc_lol.create_filtered_list([self.min_anx, self.max_anx])
+        """Create the dopplerCentroid element."""
         doppler_centroid = ET.Element('dopplerCentroid')
-        doppler_centroid.append(filtered)
+        doppler_centroid.append(self.merge_lists('dopplerCentroid/dcEstimateList'))
         self.doppler_centroid = doppler_centroid
 
     def create_antenna_pattern(self):
-        pattern_lists = [prod.find('antennaPattern/antennaPatternList') for prod in self.inputs]
-        pattern_lol = ListOfListElements(pattern_lists, self.start_line, self.slc_lengths)
-        filtered = pattern_lol.create_filtered_list([self.min_anx, self.max_anx])
+        """Create the antennaPattern element."""
         antenna_pattern = ET.Element('antennaPattern')
-        antenna_pattern.append(filtered)
+        antenna_pattern.append(self.merge_lists('antennaPattern/antennaPatternList'))
         self.antenna_pattern = antenna_pattern
 
     def create_swath_timing(self):
+        """Create the swathTiming element."""
         burst_lists = [prod.find('swathTiming/burstList') for prod in self.inputs]
         burst_lol = ListOfListElements(burst_lists, self.start_line, self.slc_lengths)
         filtered = burst_lol.create_filtered_list([self.min_anx, self.max_anx], buffer=timedelta(seconds=0.1))
 
         # TODO: This is needed since we always buffer backward AND forward
         if int(filtered.get('count')) > len(self.burst_infos):
             filtered.remove(filtered[-1])
@@ -174,46 +194,51 @@
 
         swath_timing = ET.Element('swathTiming')
         swath_timing.append(deepcopy(self.inputs[0].find('swathTiming/linesPerBurst')))
         swath_timing.append(deepcopy(self.inputs[0].find('swathTiming/samplesPerBurst')))
         swath_timing.append(filtered)
         self.swath_timing = swath_timing
 
-    def create_geolocation_grid(self):
-        grid_points = [prod.find('geolocationGrid/geolocationGridPointList') for prod in self.inputs]
-        grid_point_lol = ListOfListElements(grid_points, self.start_line, self.slc_lengths)
-        filtered = grid_point_lol.create_filtered_list([self.min_anx, self.max_anx], line_bounds=[0, self.total_lines])
-        geolocation_grid = ET.Element('geolocationGrid')
-        geolocation_grid.append(filtered)
-        self.geolocation_grid = geolocation_grid
-
-        gcp_xmls = geolocation_grid.find('geolocationGridPointList').findall('*')
+    def update_gcps(self):
+        """Update gcp attribute using the geolocationGridPointList."""
+        gcp_xmls = self.geolocation_grid.find('geolocationGridPointList').findall('*')
         for gcp_xml in gcp_xmls:
             gcp = GeoPoint(
                 float(gcp_xml.find('longitude').text),
                 float(gcp_xml.find('latitude').text),
                 float(gcp_xml.find('height').text),
                 int(gcp_xml.find('line').text),
                 int(gcp_xml.find('pixel').text),
             )
             self.gcps.append(gcp)
 
+    def create_geolocation_grid(self):
+        """Create the geolocationGrid element."""
+        geolocation_grid = ET.Element('geolocationGrid')
+        grid_list = self.merge_lists('geolocationGrid/geolocationGridPointList', line_bounds=[0, self.total_lines])
+        geolocation_grid.append(grid_list)
+        self.geolocation_grid = geolocation_grid
+        self.update_gcps()
+
     def create_coordinate_conversion(self):
+        """Create an empty coordinateConversion element."""
         coordinate_conversion = ET.Element('coordinateConversion')
         coordinate_conversion_list = ET.SubElement(coordinate_conversion, 'coordinateConversionList')
         coordinate_conversion_list.set('count', '0')
         self.coordinate_conversion = coordinate_conversion
 
     def create_swath_merging(self):
+        """Create an empty swathMerging element."""
         swath_merging = ET.Element('swathMerging')
         swath_merge_list = ET.SubElement(swath_merging, 'swathMergeList')
         swath_merge_list.set('count', '0')
         self.swath_merging = swath_merging
 
     def assemble(self):
+        """Assemble the product from its components."""
         self.create_ads_header()
         self.create_quality_information()
         self.create_general_annotation()
         self.create_image_annotation()
         self.create_doppler_centroid()
         self.create_antenna_pattern()
         self.create_swath_timing()
```

### Comparing `burst2safe-0.1.0/src/burst2safe/utils.py` & `burst2safe-0.2.0/src/burst2safe/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import warnings
+from binascii import crc_hqx
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from pathlib import Path
-from typing import Iterable, List, Optional
+from typing import Dict, Iterable, List, Optional
 
-import asf_search
-import crcmod
 import lxml.etree as ET
+from asf_search.Products.S1BurstProduct import S1BurstProduct
 from osgeo import gdal
 
 
 gdal.UseExceptions()
 warnings.filterwarnings('ignore')
 
 
@@ -50,36 +50,38 @@
         self.start_utc = start_utcs[self.burst_index]
 
         azimuth_time_interval = float(annotation.find('.//azimuthTimeInterval').text)
         burst_time_interval = timedelta(seconds=(self.length - 1) * azimuth_time_interval)
         self.stop_utc = self.start_utc + burst_time_interval
 
 
-def get_burst_info(granule: str, work_dir: Path) -> BurstInfo:
-    results = asf_search.search(product_list=[granule])
-    if len(results) == 0:
-        raise ValueError(f'ASF Search failed to find {granule}.')
-    if len(results) > 1:
-        raise ValueError(f'ASF Search found multiple results for {granule}.')
-    result = results[0]
-
-    burst_granule = result.properties['fileID']
-    slc_granule = result.umm['InputGranules'][0].split('-')[0]
-    swath = result.properties['burst']['subswath'].upper()
-    polarization = result.properties['polarization'].upper()
-    burst_id = int(result.properties['burst']['relativeBurstID'])
-    burst_index = int(result.properties['burst']['burstIndex'])
-    direction = result.properties['flightDirection'].upper()
-    absolute_orbit = int(result.properties['orbit'])
+def create_burst_info(product: S1BurstProduct, work_dir: Path) -> BurstInfo:
+    """Create a BurstInfo object given a granule.
+
+    Args:
+        product: A S1BurstProduct object
+        work_dir: The directory to save the data to.
+    """
+    slc_granule = product.umm['InputGranules'][0].split('-')[0]
+
+    burst_granule = product.properties['fileID']
+    direction = product.properties['flightDirection'].upper()
+    polarization = product.properties['polarization'].upper()
+    absolute_orbit = int(product.properties['orbit'])
+    data_url = product.properties['url']
+    metadata_url = product.properties['additionalUrls'][0]
+
+    swath = product.properties['burst']['subswath'].upper()
+    burst_id = int(product.properties['burst']['relativeBurstID'])
+    burst_index = int(product.properties['burst']['burstIndex'])
+
     date_format = '%Y%m%dT%H%M%S'
     burst_time_str = burst_granule.split('_')[3]
     burst_time = datetime.strptime(burst_time_str, date_format)
-    data_url = result.properties['url']
     data_path = work_dir / f'{burst_granule}.tiff'
-    metadata_url = result.properties['additionalUrls'][0]
     metadata_path = work_dir / f'{slc_granule}_{polarization}.xml'
 
     burst_info = BurstInfo(
         burst_granule,
         slc_granule,
         swath,
         polarization,
@@ -92,33 +94,42 @@
         data_path,
         metadata_url,
         metadata_path,
     )
     return burst_info
 
 
-def gather_burst_infos(granules: Iterable[str], work_dir: Path) -> List[BurstInfo]:
+def get_burst_infos(products: Iterable[S1BurstProduct], work_dir: Path) -> List[BurstInfo]:
     """Get burst information from ASF Search.
 
     Args:
-        granules: The burst granules to get information for.
+        products: A list of S1BurstProduct objects.
         save_dir: The directory to save the data to.
+
     Returns:
         A list of BurstInfo objects.
     """
     work_dir = optional_wd(work_dir)
     burst_info_list = []
-    for granule in granules:
-        burst_info = get_burst_info(granule, work_dir)
+    for product in products:
+        burst_info = create_burst_info(product, work_dir)
         burst_info_list.append(burst_info)
 
     return burst_info_list
 
 
-def sort_burst_infos(burst_info_list):
+def sort_burst_infos(burst_info_list: List[BurstInfo]) -> Dict:
+    """Sort BurstInfo objects by swath and polarization.
+
+    Args:
+        burst_info_list: List of BurstInfo objects.
+
+    Returns:
+        Dictionary of sorted BurstInfo objects. First key is swath, second key is polarization.
+    """
     burst_infos = {}
     for burst_info in burst_info_list:
         if burst_info.swath not in burst_infos:
             burst_infos[burst_info.swath] = {}
 
         if burst_info.polarization not in burst_infos[burst_info.swath]:
             burst_infos[burst_info.swath][burst_info.polarization] = []
@@ -129,34 +140,47 @@
     polarizations = list(burst_infos[swaths[0]].keys())
     for swath, polarization in zip(swaths, polarizations):
         burst_infos[swath][polarization] = sorted(burst_infos[swath][polarization], key=lambda x: x.burst_id)
 
     return burst_infos
 
 
-def optional_wd(wd: Optional[Path | str] = None) -> None:
-    """Return the working directory as a Path object"""
+def optional_wd(wd: Optional[Path | str] = None) -> Path:
+    """Return the working directory as a Path object
+
+    Args:
+        wd: Optional working directory as a Path or string
+
+    Returns:
+        Path to your input working directory or the current working directory.
+    """
     if wd is None:
         wd = Path.cwd()
     return Path(wd)
 
 
-def calculate_crc16(file_path: Path):
-    """Calculate the CRC16 checksum for a file."""
+def calculate_crc16(file_path: Path) -> str:
+    """Calculate the CRC16 checksum for a file.
+
+    Args:
+        file_path: Path to file to calculate checksum for
+
+    Returns:
+        CRC16 checksum as a hexadecimal string
+    """
     with open(file_path, 'rb') as f:
         data = f.read()
 
-    # TODO: this doesn't match the ESA checksum
-    crc16 = crcmod.predefined.mkPredefinedCrcFun('crc-16')
-    crc16_value = crc16(data)
-    crc16_hex = hex(crc16_value)[2:].zfill(4).upper()
-    return crc16_hex
+    crc = f'{crc_hqx(data, 0xffff):04X}'
+    return crc
 
 
-def get_subxml_from_metadata(metadata_path: str, xml_type: str, subswath: str = None, polarization: str = None):
+def get_subxml_from_metadata(
+    metadata_path: Path, xml_type: str, subswath: str = None, polarization: str = None
+) -> ET.Element:
     """Extract child xml info from ASF combined metadata file.
 
     Args:
         metadata_path: Path to metadata file
         xml_typ: Desired type of metadata to obtain (product, noise, calibration, or rfi)
         subswath: Desired subswath to obtain data for
         polarization: Desired polarization to obtain data for
@@ -164,17 +188,16 @@
     Returns:
         lxml Element for desired metadata
     """
     with open(metadata_path, 'r') as metadata_file:
         metadata = ET.parse(metadata_file).getroot()
 
     if xml_type == 'manifest':
-        name = 'manifest.safe'
         desired_metadata = metadata.find('manifest/{urn:ccsds:schema:xfdu:1}XFDU')
-        return name, desired_metadata
+        return desired_metadata
 
     possible_types = ['product', 'noise', 'calibration', 'rfi']
     if xml_type not in possible_types:
         raise ValueError(f'Metadata type {xml_type} not one of {" ".join(possible_types)}')
 
     if subswath is None or polarization is None:
         raise ValueError('subswath and polarization must be provided for non-manifest files')
@@ -187,13 +210,28 @@
         desired_metadata = None
     else:
         desired_metadata = correct_pol[0].find('content')
 
     return desired_metadata
 
 
-def flatten(list_of_lists: List[List]):
+def flatten(list_of_lists: List[List]) -> List:
+    """Flatten a list of lists."""
     return [item for sublist in list_of_lists for item in sublist]
 
 
-def drop_duplicates(input_list: List):
+def drop_duplicates(input_list: List) -> List:
+    """Drop duplicates from a list, while preserving order."""
     return list(dict.fromkeys(input_list))
+
+
+def set_text(element: ET.Element, text: str | int) -> None:
+    """Set the text of an element if it is not None.
+
+    Args:
+        element: The element to set the text of.
+        text: The text to set the element to.
+    """
+    if not isinstance(text, str) and not isinstance(text, int):
+        raise ValueError('Text must be a string or an integer.')
+
+    element.text = str(text)
```

### Comparing `burst2safe-0.1.0/src/burst2safe.egg-info/PKG-INFO` & `burst2safe-0.2.0/src/burst2safe.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst2safe
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format
 Author-email: Forrest Williams <ffwilliams2@alaska.edu>
 Project-URL: Homepage, https://github.com/forrestfwilliams/burst2safe
 Project-URL: Bug Tracker, https://github.com/forrestfwilliams/burst2safe/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,14 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gdal
 Requires-Dist: numpy
 Requires-Dist: lxml
 Requires-Dist: asf_search
-Requires-Dist: crcmod
 Provides-Extra: develop
 Requires-Dist: pytest; extra == "develop"
 
 # burst2safe
 Utility for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format.
 
 **This is still a work in progress, and we recommend waiting until the release of version 1.0.0 for use in production environments!**
@@ -36,28 +35,40 @@
 ```
 
 Or conda:
 ```bash
 conda install -c conda-forge burst2safe
 ```
 
-Then provide a list of Sentinel-1 burst granule IDs to be merged into a SAFE file to the `burst2safe` CLI tool using the following structure:
+Then, run the `burst2safe` command line tool using the following structure:
+```bash
+burst2safe --orbit 32861 --bbox 53.57 27.54 53.78 27.60 --pols VV VH
+```
+Where:
 
+* `--orbit` is the absolute orbit number of the Sentinel-1 data.
+* `--bbox` is the bounding box of the area of interest in the format `minlon minlat maxlon maxlat`.
+* `--pols` is the polarization of the Sentinel-1 data. Options are `VV`, `VH`, `HV`, and `HH`.
+
+For more control over the burst group, you can also provide specific burst granule IDs to be merged into a SAFE file using the following structure:
 ```bash
-burst2safe S1_136231_IW2_20200604T022312_VV_7C85-BURST S1_136232_IW2_20200604T022315_VV_7C85-BURST
+burst2safe S1_136231_IW2_20200604T022312_VV_7C85-BURST S1_136232_IW2_20200604T022315_VV_7C85-BURST S1_136231_IW2_20200604T022312_VH_7C85-BURST S1_136232_IW2_20200604T022315_VH_7C85-BURST
 ```
-The output SAFE file will be created in the current directory.
+This search is equivalent to the previous search.
 To be eligible for processing, all burst granules must:
+
 1. Have the same acquisition mode
-1. Be in the same polarization
 1. Be from the same absolute orbit
 1. Be contiguous in time and space.
+1. Have the same footprint for all polarizations.
 
 The tool should raise an error if any of these conditions are not met.
 
+The output SAFE file will be created in the current directory.
+
 ## Strategy
 `burst2safe` combines and reformats individual bursts into a SAFE file following the procedure described in the [Sentinel-1 Product Specification Document](https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/document-library/-/asset_publisher/1dO7RF5fJMbd/content/sentinel-1-product-specification-from-ipf-360?_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId=4846613&_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_redirect=https%3A%2F%2Fsentinel.esa.int%2Fweb%2Fsentinel%2Fuser-guides%2Fsentinel-1-sar%2Fdocument-library%3Fp_p_id%3Dcom_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId%3D4846613%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_cur%3D0%26p_r_p_resetCur%3Dfalse)
 In this document, ESA describes how to create an Assembled Sentinel-1 Level 1 product from individual Sentinel-1 Level 1 SAFEs. We use this same strategy to combine ASF-extracted burst SLC products into a SAFE file that should be compatible with any SAR processor currently capable of using Sentinel-1 Level SAFEs. For in-depth technical details of the implementation, we refer you to the Sentinel-1 Product Specification document above. However, it is important to know that ESA recommends merging Sentinel-1 data/metadata components using three primary strategies:
 
 ### Include
 A given data/metadata component is the same for all data slices, and any value can be used (i.e., polarization).
 
@@ -116,8 +127,8 @@
 ## Contact Us
 Want to talk about `burst2safe`? We would love to hear from you!
 
 Found a bug? Want to request a feature?
 [open an issue](https://github.com/ASFHyP3/asf_tools/issues/new)
 
 General questions? Suggestions? Or just want to talk to the team?
-[chat with us on burst2safe's discussion page](https://github.com/forrestfwilliams/burst2safe/discussions) 
+[chat with us on burst2safe's discussion page](https://github.com/forrestfwilliams/burst2safe/discussions)
```

### Comparing `burst2safe-0.1.0/src/burst2safe.egg-info/SOURCES.txt` & `burst2safe-0.2.0/src/burst2safe.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,27 +14,40 @@
 .github/workflows/pytest.yml
 .github/workflows/release-checklist-comment.yml
 .github/workflows/release.yml
 .github/workflows/static-analysis.yml
 src/burst2safe/base.py
 src/burst2safe/burst2safe.py
 src/burst2safe/calibration.py
+src/burst2safe/manifest.py
 src/burst2safe/measurement.py
 src/burst2safe/noise.py
 src/burst2safe/product.py
 src/burst2safe/safe.py
+src/burst2safe/swath.py
 src/burst2safe/utils.py
 src/burst2safe.egg-info/PKG-INFO
 src/burst2safe.egg-info/SOURCES.txt
 src/burst2safe.egg-info/dependency_links.txt
 src/burst2safe.egg-info/entry_points.txt
 src/burst2safe.egg-info/not-zip-safe
 src/burst2safe.egg-info/requires.txt
 src/burst2safe.egg-info/top_level.txt
 src/burst2safe/data/s1-level-1-calibration.xsd
 src/burst2safe/data/s1-level-1-measurement.xsd
 src/burst2safe/data/s1-level-1-noise.xsd
 src/burst2safe/data/s1-level-1-product.xsd
 src/burst2safe/data/s1-object-types.xsd
 tests/conftest.py
+tests/helpers.py
+tests/test_base.py
 tests/test_burst2safe.py
-tests/test_data/S1A_IW_SLC__1SDV_20200604T022251_20200604T022318_032861_03CE65_7C85_VV.xml
+tests/test_calibration.py
+tests/test_manifest.py
+tests/test_measurement.py
+tests/test_noise.py
+tests/test_product.py
+tests/test_safe.py
+tests/test_swath.py
+tests/test_utils.py
+tests/test_data/S1A_IW_SLC__1SDV_20200604T022251_20200604T022318_032861_03CE65_7C85_VV.xml
+tests/test_data/manifest_7C85.safe
```

### Comparing `burst2safe-0.1.0/tests/test_data/S1A_IW_SLC__1SDV_20200604T022251_20200604T022318_032861_03CE65_7C85_VV.xml` & `burst2safe-0.2.0/tests/test_data/S1A_IW_SLC__1SDV_20200604T022251_20200604T022318_032861_03CE65_7C85_VV.xml`

 * *Files identical despite different names*

