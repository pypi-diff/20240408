# Comparing `tmp/df_qc_tools-0.0.1.tar.gz` & `tmp/df_qc_tools-0.0.2.tar.gz`

## Comparing `df_qc_tools-0.0.1.tar` & `df_qc_tools-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/requirements.txt
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/requirements.txt_old
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/src/df_qc_tools/__init__.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/src/df_qc_tools/config.py
--rw-r--r--   0        0        0    19983 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/src/df_qc_tools/qc.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/src/df_qc_tools/qualityflags.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/tests/test_config.py
--rw-r--r--   0        0        0    29601 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/tests/test_qc.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/tests/conf/conf_base.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/tests/resources/data_velocity_acc.csv
--rw-r--r--   0        0        0  1417615 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/tests/resources/df_outliers.csv
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/.gitignore
--rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/README.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 df_qc_tools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/src/df_qc_tools/__init__.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/src/df_qc_tools/config.py
+-rw-r--r--   0        0        0    19983 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/src/df_qc_tools/qc.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/src/df_qc_tools/qualityflags.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/tests/test_config.py
+-rw-r--r--   0        0        0    29601 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/tests/test_qc.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/tests/conf/conf_base.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/tests/resources/data_velocity_acc.csv
+-rw-r--r--   0        0        0  1417615 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/tests/resources/df_outliers.csv
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/.gitignore
+-rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/LICENSE
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/README.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/PKG-INFO
```

### Comparing `df_qc_tools-0.0.1/Makefile` & `df_qc_tools-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.1/src/df_qc_tools/config.py` & `df_qc_tools-0.0.2/src/df_qc_tools/config.py`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.1/src/df_qc_tools/qc.py` & `df_qc_tools-0.0.2/src/df_qc_tools/qc.py`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.1/tests/test_config.py` & `df_qc_tools-0.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.1/tests/test_qc.py` & `df_qc_tools-0.0.2/tests/test_qc.py`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.1/tests/resources/data_velocity_acc.csv` & `df_qc_tools-0.0.2/tests/resources/data_velocity_acc.csv`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.1/tests/resources/df_outliers.csv` & `df_qc_tools-0.0.2/tests/resources/df_outliers.csv`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.1/LICENSE` & `df_qc_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.1/pyproject.toml` & `df_qc_tools-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "df-qc-tools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="nvds" },
 ]
 description = "Package for easy datarequests from sensortings"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `df_qc_tools-0.0.1/PKG-INFO` & `df_qc_tools-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: df-qc-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for easy datarequests from sensortings
 Project-URL: Homepage, https://github.com/nvdsteen/pandassta
 Project-URL: Issues, https://github.com/nvdsteen/pandassta/issues
 Author: nvds
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -12,13 +12,18 @@
 Requires-Python: >=3.11
 Requires-Dist: geopandas==0.14.3
 Requires-Dist: geopy==2.4.1
 Requires-Dist: hydra-core==1.3.2
 Requires-Dist: numpy==1.26.4
 Requires-Dist: omegaconf==2.3.0
 Requires-Dist: pandas==2.2.1
-Requires-Dist: pandassta==0.0.1
+Requires-Dist: pandassta>=0.0.2
 Requires-Dist: pytest==8.1.1
 Requires-Dist: scipy==1.12.0
-Requires-Dist: searegion-detection==0.0.1
+Requires-Dist: searegion-detection>=0.0.2
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: xarray==2024.2.0
+Description-Content-Type: text/markdown
+
+# df-qc-tools
+
+Tools to perform basic quality checks on observations stored in a pandas dataframe.
```

