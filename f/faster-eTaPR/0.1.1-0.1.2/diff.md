# Comparing `tmp/faster_etapr-0.1.1.tar.gz` & `tmp/faster_etapr-0.1.2.tar.gz`

## Comparing `faster_etapr-0.1.1.tar` & `faster_etapr-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/CHANGELOG.rst
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/benchmark.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/py.typed
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/tox.ini
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/changelog/.gitignore
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/changelog/README.rst
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/changelog/towncrier_template.rst
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/docs/Makefile
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/docs/make.bat
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/docs/source/conf.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/docs/source/index.rst
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0        0        0   112044 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/docs/source/img/motivation.png
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/docs/source/pages/changelog.rst
--rw-r--r--   0        0        0    13114 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/docs/source/pages/motivation.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/docs/source/pages/readme.rst
--rw-r--r--   0        0        0   112044 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/img/motivation.png
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/src/faster_etapr/__init__.py
--rw-r--r--   0        0        0    33389 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/src/faster_etapr/etapr.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/src/faster_etapr/types.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/src/faster_etapr/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/tests/test_etapr.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/tests/test_utils.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/.gitignore
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/LICENSE
--rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/README.rst
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 faster_etapr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/CHANGELOG.rst
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/benchmark.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/py.typed
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/tox.ini
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/changelog/.gitignore
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/changelog/README.rst
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/changelog/towncrier_template.rst
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/docs/source/conf.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/docs/source/index.rst
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0   112044 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/docs/source/img/motivation.png
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/docs/source/pages/changelog.rst
+-rw-r--r--   0        0        0    13114 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/docs/source/pages/motivation.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/docs/source/pages/readme.rst
+-rw-r--r--   0        0        0   112044 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/img/motivation.png
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/src/faster_etapr/__init__.py
+-rw-r--r--   0        0        0    33388 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/src/faster_etapr/etapr.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/src/faster_etapr/types.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/src/faster_etapr/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/tests/test_etapr.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/.gitignore
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/README.rst
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8006 2020-02-02 00:00:00.000000 faster_etapr-0.1.2/PKG-INFO
```

### Comparing `faster_etapr-0.1.1/.pre-commit-config.yaml` & `faster_etapr-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/.readthedocs.yaml` & `faster_etapr-0.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/benchmark.py` & `faster_etapr-0.1.2/benchmark.py`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/tox.ini` & `faster_etapr-0.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/.github/workflows/python-package.yml` & `faster_etapr-0.1.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/.github/workflows/python-publish.yml` & `faster_etapr-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/changelog/README.rst` & `faster_etapr-0.1.2/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/changelog/towncrier_template.rst` & `faster_etapr-0.1.2/changelog/towncrier_template.rst`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/docs/Makefile` & `faster_etapr-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/docs/make.bat` & `faster_etapr-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/docs/source/conf.py` & `faster_etapr-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/docs/source/_templates/custom-class-template.rst` & `faster_etapr-0.1.2/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/docs/source/_templates/custom-module-template.rst` & `faster_etapr-0.1.2/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/docs/source/img/motivation.png` & `faster_etapr-0.1.2/docs/source/img/motivation.png`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/docs/source/pages/motivation.rst` & `faster_etapr-0.1.2/docs/source/pages/motivation.rst`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/img/motivation.png` & `faster_etapr-0.1.2/img/motivation.png`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/src/faster_etapr/etapr.py` & `faster_etapr-0.1.2/src/faster_etapr/etapr.py`

 * *Files 0% similar despite different names*

```diff
@@ -695,15 +695,15 @@
           - ``point_adjust/recall``: point-adjusted recall
           - ``point_adjust/precision``: point-adjusted precision
           - ``point_adjust/f1``: point-adjusted f1
 
     Example:
 
         >>> import faster_etapr
-        >>> faster_etapr.evaluate_from_ranges(
+        >>> faster_etapr.evaluate_from_preds(
         ...     y_hat=[0, 1, 0, 1, 1, 0, 0, 1, 1, 1, 0, 1, 1, 1, 0, 0, 0],
         ...     y=    [0, 1, 1, 0, 0, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 0, 1],
         ...     theta_p=0.5,
         ...     theta_r=0.1,
         ... )
         {
             'eta/recall': 0.3875,
```

### Comparing `faster_etapr-0.1.1/src/faster_etapr/types.py` & `faster_etapr-0.1.2/src/faster_etapr/types.py`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/src/faster_etapr/utils.py` & `faster_etapr-0.1.2/src/faster_etapr/utils.py`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/tests/test_etapr.py` & `faster_etapr-0.1.2/tests/test_etapr.py`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/tests/test_utils.py` & `faster_etapr-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/.gitignore` & `faster_etapr-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/LICENSE` & `faster_etapr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `faster_etapr-0.1.1/README.rst` & `faster_etapr-0.1.2/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     uv pip install faster-etapr
 
 Now, you run your evaluation in python:
 
 .. code::
 
     import faster_etapr
-    faster_etapr.evaluate_from_ranges(
+    faster_etapr.evaluate_from_preds(
         y_hat=[0, 1, 0, 1, 1, 0, 0, 1, 1, 1, 0, 1, 1, 1, 0, 0, 0],
         y=    [0, 1, 1, 0, 0, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 0, 1],
         theta_p=0.5,
         theta_r=0.1,
     )
     {
         'eta/recall': 0.3875,
@@ -130,7 +130,31 @@
 +---------+-----------+--------------+--------+
 | 10 000  | 35.8264   | 0.1810       | ~198x  |
 +---------+-----------+--------------+--------+
 | 20 000  | 148.2670  | 0.6547       | ~226x  |
 +---------+-----------+--------------+--------+
 | 100 000 | too long  | 55.04712     |        |
 +---------+-----------+--------------+--------+
+
+Citation
+--------
+
+If you use eTaPR, please cite the original author/paper:
+
+.. code::
+
+    @inproceedings{10.1145/3477314.3507024,
+    author = {Hwang, Won-Seok and Yun, Jeong-Han and Kim, Jonguk and Min, Byung Gil},
+    title = {"Do You Know Existing Accuracy Metrics Overrate Time-Series Anomaly Detections?"},
+    year = {2022},
+    isbn = {9781450387132},
+    publisher = {Association for Computing Machinery},
+    address = {New York, NY, USA},
+    url = {https://doi.org/10.1145/3477314.3507024},
+    doi = {10.1145/3477314.3507024},
+    booktitle = {Proceedings of the 37th ACM/SIGAPP Symposium on Applied Computing},
+    pages = {403–412},
+    numpages = {10},
+    keywords = {accuracy metric, anomaly detection, precision, recall, time-series},
+    location = {Virtual Event},
+    series = {SAC '22}
+    }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `faster_etapr-0.1.1/pyproject.toml` & `faster_etapr-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     "ipykernel>=6.29.3",
     "etapr-pkg @ git+https://github.com/GPla/eTaPR",
     "mypy>=1.9.0",
     "pytest-mock>=3.14.0",
     "tox>=4.14.2",
     "uv>=0.1.24",
     "pytest-cov>=5.0.0",
+    "towncrier>=23.11.0",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/faster_etapr"]
@@ -100,19 +101,19 @@
 convention = "google"
 
 [tool.ruff.lint.isort]
 force-single-line = true
 
 [tool.towncrier]
     package_dir="src"
-    package = "etapr"
+    package = "faster_etapr"
     filename = "CHANGELOG.rst"
     directory = "changelog"
     template = "changelog/towncrier_template.rst"
-    issue_format = "`#{issue} <https://github.com/saurf4ng/eTaPR/issues/{issue}>`__"
+    issue_format = "`#{issue} <https://github.com/GPla/faster-eTaPR/issues/{issue}>`__"
     title_format = "{version} ({project_date})"
     underlines=["-", "-", "^"]
 
     [[tool.towncrier.type]]
         directory = "change"
         name = "Changes"
         showcontent = true
```

### Comparing `faster_etapr-0.1.1/PKG-INFO` & `faster_etapr-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faster-eTaPR
-Version: 0.1.1
+Version: 0.1.2
 Dynamic: Summary
 Project-URL: Documentation, https://faster-etapr.readthedocs.io
 Project-URL: Source, https://github.com/GPla/faster-eTaPR
 Author-email: Gorden Platz <36087062+GPla@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: anomaly,detection,etapr,evaluation,learning,machine,metrics,performance,point-adjust
@@ -99,15 +99,15 @@
     uv pip install faster-etapr
 
 Now, you run your evaluation in python:
 
 .. code::
 
     import faster_etapr
-    faster_etapr.evaluate_from_ranges(
+    faster_etapr.evaluate_from_preds(
         y_hat=[0, 1, 0, 1, 1, 0, 0, 1, 1, 1, 0, 1, 1, 1, 0, 0, 0],
         y=    [0, 1, 1, 0, 0, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 0, 1],
         theta_p=0.5,
         theta_r=0.1,
     )
     {
         'eta/recall': 0.3875,
@@ -164,7 +164,31 @@
 +---------+-----------+--------------+--------+
 | 10 000  | 35.8264   | 0.1810       | ~198x  |
 +---------+-----------+--------------+--------+
 | 20 000  | 148.2670  | 0.6547       | ~226x  |
 +---------+-----------+--------------+--------+
 | 100 000 | too long  | 55.04712     |        |
 +---------+-----------+--------------+--------+
+
+Citation
+--------
+
+If you use eTaPR, please cite the original author/paper:
+
+.. code::
+
+    @inproceedings{10.1145/3477314.3507024,
+    author = {Hwang, Won-Seok and Yun, Jeong-Han and Kim, Jonguk and Min, Byung Gil},
+    title = {"Do You Know Existing Accuracy Metrics Overrate Time-Series Anomaly Detections?"},
+    year = {2022},
+    isbn = {9781450387132},
+    publisher = {Association for Computing Machinery},
+    address = {New York, NY, USA},
+    url = {https://doi.org/10.1145/3477314.3507024},
+    doi = {10.1145/3477314.3507024},
+    booktitle = {Proceedings of the 37th ACM/SIGAPP Symposium on Applied Computing},
+    pages = {403–412},
+    numpages = {10},
+    keywords = {accuracy metric, anomaly detection, precision, recall, time-series},
+    location = {Virtual Event},
+    series = {SAC '22}
+    }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

