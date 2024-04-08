# Comparing `tmp/rectanglepy-0.1.0.tar.gz` & `tmp/rectanglepy-0.1.2.tar.gz`

## Comparing `rectanglepy-0.1.0.tar` & `rectanglepy-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.bumpversion.cfg
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.cruft.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.editorconfig
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/changelog.md
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/conf.py
--rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/contributing.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/index.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/make.bat
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/docs/notebooks/example.ipynb
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/src/rectanglepy/__init__.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/src/rectanglepy/rectangle.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/src/rectanglepy/data/hao1_annotations_small.csv
--rw-r--r--   0        0        0  2694169 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/src/rectanglepy/data/hao1_counts_small.csv
--rw-r--r--   0        0        0    91148 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/src/rectanglepy/data/small_fino_bulks.csv
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/src/rectanglepy/pp/__init__.py
--rw-r--r--   0        0        0    19253 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/src/rectanglepy/pp/create_signature.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/src/rectanglepy/pp/rectangle_signature.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/src/rectanglepy/tl/__init__.py
--rw-r--r--   0        0        0    14808 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/src/rectanglepy/tl/deconvolution.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/tests/test_pp.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/tests/test_rectangle.py
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/tests/test_tl.py
--rw-r--r--   0        0        0    28466 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/tests/data/TIL10_signature.txt
--rw-r--r--   0        0        0   132044 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/tests/data/bulk_small.csv
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/tests/data/cell_annotations_small.txt
--rw-r--r--   0        0        0  2201267 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/tests/data/quanTIseq_SimRNAseq_mixture_smaller.csv
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/tests/data/quanTIseq_SimRNAseq_read_fractions_small.txt
--rw-r--r--   0        0        0   274597 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/tests/data/sc_object_small.csv
--rw-r--r--   0        0        0   312634 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/tests/data/signature_hao1.csv
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/LICENSE
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/README.md
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 rectanglepy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.bumpversion.cfg
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.cruft.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.editorconfig
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/changelog.md
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/conf.py
+-rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/contributing.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/index.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/docs/notebooks/example.ipynb
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/src/rectanglepy/__init__.py
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/src/rectanglepy/rectangle.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/src/rectanglepy/data/hao1_annotations_small.zip
+-rw-r--r--   0        0        0  1423449 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/src/rectanglepy/data/hao1_counts_small.zip
+-rw-r--r--   0        0        0   296709 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/src/rectanglepy/data/small_fino_bulks.zip
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/src/rectanglepy/pp/__init__.py
+-rw-r--r--   0        0        0    19135 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/src/rectanglepy/pp/create_signature.py
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/src/rectanglepy/pp/rectangle_signature.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/src/rectanglepy/tl/__init__.py
+-rw-r--r--   0        0        0    14808 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/src/rectanglepy/tl/deconvolution.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/tests/test_pp.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/tests/test_rectangle.py
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/tests/test_tl.py
+-rw-r--r--   0        0        0    28466 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/tests/data/TIL10_signature.txt
+-rw-r--r--   0        0        0   132044 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/tests/data/bulk_small.csv
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/tests/data/cell_annotations_small.txt
+-rw-r--r--   0        0        0  2201267 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/tests/data/quanTIseq_SimRNAseq_mixture_smaller.csv
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/tests/data/quanTIseq_SimRNAseq_read_fractions_small.txt
+-rw-r--r--   0        0        0   274597 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/tests/data/sc_object_small.csv
+-rw-r--r--   0        0        0   312634 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/tests/data/signature_hao1.csv
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/README.md
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 rectanglepy-0.1.2/PKG-INFO
```

### Comparing `rectanglepy-0.1.0/.cruft.json` & `rectanglepy-0.1.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/.pre-commit-config.yaml` & `rectanglepy-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/.github/workflows/build.yaml` & `rectanglepy-0.1.2/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/.github/workflows/release.yaml` & `rectanglepy-0.1.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/.github/workflows/test.yaml` & `rectanglepy-0.1.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/docs/Makefile` & `rectanglepy-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/docs/conf.py` & `rectanglepy-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/docs/contributing.md` & `rectanglepy-0.1.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/docs/make.bat` & `rectanglepy-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/docs/references.bib` & `rectanglepy-0.1.2/docs/references.bib`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/docs/_templates/autosummary/class.rst` & `rectanglepy-0.1.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/docs/extensions/typed_returns.py` & `rectanglepy-0.1.2/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/docs/notebooks/example.ipynb` & `rectanglepy-0.1.2/docs/notebooks/example.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949318910256411%*

 * *Differences: {"'cells'": "{2: {'execution_count': 1, 'metadata': {'ExecuteTime': {'end_time': "*

 * *            "'2024-03-25T16:12:40.629887Z', 'start_time': '2024-03-25T16:12:39.074585Z'}}}, 4: "*

 * *            "{'execution_count': 2, 'metadata': {'ExecuteTime': {'end_time': "*

 * *            "'2024-03-25T16:12:41.282874Z', 'start_time': '2024-03-25T16:12:40.630684Z'}}}, 5: "*

 * *            "{'execution_count': 3, 'outputs': {0: {'data': {'text/plain': '                       "*

 * *            'MIR1302-2HG  AL627309.1  AL627309.4  AC114 […]*

```diff
@@ -12,19 +12,19 @@
             "metadata": {
                 "collapsed": false
             },
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 1,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-03-07T18:31:49.115245Z",
-                    "start_time": "2024-03-07T18:31:49.092165Z"
+                    "end_time": "2024-03-25T16:12:40.629887Z",
+                    "start_time": "2024-03-25T16:12:39.074585Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import rectanglepy as rectangle\n",
                 "from anndata import AnnData"
             ]
@@ -36,92 +36,92 @@
             },
             "source": [
                 "## Load tutorial data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 2,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-03-07T18:31:49.161373Z",
-                    "start_time": "2024-03-07T18:31:49.120483Z"
+                    "end_time": "2024-03-25T16:12:41.282874Z",
+                    "start_time": "2024-03-25T16:12:40.630684Z"
                 }
             },
             "outputs": [],
             "source": [
                 "sc_counts, annotations, bulks  = rectangle.load_tutorial_data()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-03-07T18:31:49.162499Z",
-                    "start_time": "2024-03-07T18:31:49.160216Z"
+                    "end_time": "2024-03-25T16:12:41.300170Z",
+                    "start_time": "2024-03-25T16:12:41.284686Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>NOC2L</th>\n      <th>HES4</th>\n      <th>ISG15</th>\n      <th>SDF4</th>\n      <th>B3GALT6</th>\n      <th>UBE2J2</th>\n      <th>INTS11</th>\n      <th>AURKAIP1</th>\n      <th>CCNL2</th>\n      <th>MRPL20</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>E2L4_GATGCTACAGGCACAA</th>\n      <td>0</td>\n      <td>11</td>\n      <td>7</td>\n      <td>0</td>\n      <td>2</td>\n      <td>1</td>\n      <td>2</td>\n      <td>5</td>\n      <td>0</td>\n      <td>0</td>\n    </tr>\n    <tr>\n      <th>L3_AACGTCACATCAGCAT</th>\n      <td>0</td>\n      <td>0</td>\n      <td>1</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>1</td>\n      <td>1</td>\n      <td>0</td>\n      <td>1</td>\n    </tr>\n    <tr>\n      <th>L3_GGAATGGGTCTAACGT</th>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>2</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>1</td>\n      <td>0</td>\n      <td>3</td>\n    </tr>\n    <tr>\n      <th>E2L7_GTCATTTAGGCCTTCG</th>\n      <td>2</td>\n      <td>1</td>\n      <td>1</td>\n      <td>2</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>1</td>\n      <td>0</td>\n      <td>0</td>\n    </tr>\n    <tr>\n      <th>E2L6_CCCTTAGCATTGACCA</th>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>1</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>1</td>\n      <td>2</td>\n      <td>1</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
-                        "text/plain": "                       NOC2L  HES4  ISG15  SDF4  B3GALT6  UBE2J2  INTS11   \nE2L4_GATGCTACAGGCACAA      0    11      7     0        2       1       2  \\\nL3_AACGTCACATCAGCAT        0     0      1     0        0       0       1   \nL3_GGAATGGGTCTAACGT        0     0      0     2        0       0       0   \nE2L7_GTCATTTAGGCCTTCG      2     1      1     2        0       0       0   \nE2L6_CCCTTAGCATTGACCA      0     0      0     1        0       0       0   \n\n                       AURKAIP1  CCNL2  MRPL20  \nE2L4_GATGCTACAGGCACAA         5      0       0  \nL3_AACGTCACATCAGCAT           1      0       1  \nL3_GGAATGGGTCTAACGT           1      0       3  \nE2L7_GTCATTTAGGCCTTCG         1      0       0  \nE2L6_CCCTTAGCATTGACCA         1      2       1  "
+                        "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>MIR1302-2HG</th>\n      <th>AL627309.1</th>\n      <th>AL627309.4</th>\n      <th>AC114498.1</th>\n      <th>AL669831.5</th>\n      <th>FAM41C</th>\n      <th>AL645608.5</th>\n      <th>NOC2L</th>\n      <th>PERM1</th>\n      <th>ISG15</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>E2L4_GATGCTACAGGCACAA</th>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>7</td>\n    </tr>\n    <tr>\n      <th>L5_AACAACCAGGAACTAT</th>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>1</td>\n    </tr>\n    <tr>\n      <th>L5_TCCTTCTGTACTCCGG</th>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n    </tr>\n    <tr>\n      <th>L2_GCCCGAACACGTATAC</th>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>2</td>\n    </tr>\n    <tr>\n      <th>E2L2_ATGCATGTCACACCCT</th>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>1</td>\n      <td>0</td>\n      <td>0</td>\n      <td>0</td>\n      <td>1</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
+                        "text/plain": "                       MIR1302-2HG  AL627309.1  AL627309.4  AC114498.1   \nE2L4_GATGCTACAGGCACAA            0           0           0           0  \\\nL5_AACAACCAGGAACTAT              0           0           0           0   \nL5_TCCTTCTGTACTCCGG              0           0           0           0   \nL2_GCCCGAACACGTATAC              0           0           0           0   \nE2L2_ATGCATGTCACACCCT            0           0           0           0   \n\n                       AL669831.5  FAM41C  AL645608.5  NOC2L  PERM1  ISG15  \nE2L4_GATGCTACAGGCACAA           0       0           0      0      0      7  \nL5_AACAACCAGGAACTAT             0       0           0      0      0      1  \nL5_TCCTTCTGTACTCCGG             0       0           0      0      0      0  \nL2_GCCCGAACACGTATAC             0       0           0      0      0      2  \nE2L2_ATGCATGTCACACCCT           0       1           0      0      0      1  "
                     },
-                    "execution_count": 13,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "sc_counts.iloc[:, :10].head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 4,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-03-07T18:31:49.169641Z",
-                    "start_time": "2024-03-07T18:31:49.164684Z"
+                    "end_time": "2024-03-25T16:12:41.982618Z",
+                    "start_time": "2024-03-25T16:12:41.979126Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "E2L4_GATGCTACAGGCACAA    Monocytes\nL3_AACGTCACATCAGCAT      Monocytes\nL3_GGAATGGGTCTAACGT      Monocytes\nE2L7_GTCATTTAGGCCTTCG    Monocytes\nE2L6_CCCTTAGCATTGACCA    Monocytes\nName: 0, dtype: object"
+                        "text/plain": "E2L4_GATGCTACAGGCACAA    Monocytes\nL5_AACAACCAGGAACTAT      Monocytes\nL5_TCCTTCTGTACTCCGG      Monocytes\nL2_GCCCGAACACGTATAC      Monocytes\nE2L2_ATGCATGTCACACCCT    Monocytes\nName: 0, dtype: object"
                     },
-                    "execution_count": 14,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "annotations.head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 5,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-03-07T18:31:49.177705Z",
-                    "start_time": "2024-03-07T18:31:49.173852Z"
+                    "end_time": "2024-03-25T16:12:43.131140Z",
+                    "start_time": "2024-03-25T16:12:43.127235Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>SNORA52</th>\n      <th>SNORA53</th>\n      <th>SNORA54</th>\n      <th>SNORA55</th>\n      <th>SNORA56</th>\n      <th>SNORA57</th>\n      <th>SNORA59B</th>\n      <th>SNORA5A</th>\n      <th>SNORA5B</th>\n      <th>SNORA5C</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>pbmc_1</th>\n      <td>2.02120</td>\n      <td>0.426412</td>\n      <td>0.0</td>\n      <td>0.585614</td>\n      <td>0.00000</td>\n      <td>2.060440</td>\n      <td>0.666746</td>\n      <td>1.84082</td>\n      <td>0.000000</td>\n      <td>2.53766</td>\n    </tr>\n    <tr>\n      <th>pbmc_10</th>\n      <td>1.15102</td>\n      <td>0.000000</td>\n      <td>0.0</td>\n      <td>1.185750</td>\n      <td>1.15618</td>\n      <td>0.325934</td>\n      <td>0.379692</td>\n      <td>2.01894</td>\n      <td>0.884945</td>\n      <td>1.70451</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
-                        "text/plain": "         SNORA52   SNORA53  SNORA54   SNORA55  SNORA56   SNORA57  SNORA59B   \npbmc_1   2.02120  0.426412      0.0  0.585614  0.00000  2.060440  0.666746  \\\npbmc_10  1.15102  0.000000      0.0  1.185750  1.15618  0.325934  0.379692   \n\n         SNORA5A   SNORA5B  SNORA5C  \npbmc_1   1.84082  0.000000  2.53766  \npbmc_10  2.01894  0.884945  1.70451  "
+                        "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>UBE2Q2P2</th>\n      <th>SSX9</th>\n      <th>CXorf67</th>\n      <th>EFCAB8</th>\n      <th>SPATA31B1P</th>\n      <th>SDR16C6P</th>\n      <th>GTPBP6</th>\n      <th>EFCAB12</th>\n      <th>A1BG</th>\n      <th>A1CF</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>pbmc_1</th>\n      <td>0.000000</td>\n      <td>0.0</td>\n      <td>0.118865</td>\n      <td>0.00000</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>57.280197</td>\n      <td>0.252188</td>\n      <td>10.863071</td>\n      <td>0.0</td>\n    </tr>\n    <tr>\n      <th>pbmc_10</th>\n      <td>0.081115</td>\n      <td>0.0</td>\n      <td>0.086782</td>\n      <td>0.00000</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>72.275326</td>\n      <td>0.095742</td>\n      <td>14.785649</td>\n      <td>0.0</td>\n    </tr>\n    <tr>\n      <th>pbmc_12</th>\n      <td>0.000000</td>\n      <td>0.0</td>\n      <td>0.188464</td>\n      <td>0.03157</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>50.997427</td>\n      <td>0.100608</td>\n      <td>7.492537</td>\n      <td>0.0</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
+                        "text/plain": "         UBE2Q2P2  SSX9   CXorf67   EFCAB8  SPATA31B1P  SDR16C6P     GTPBP6   \npbmc_1   0.000000   0.0  0.118865  0.00000         0.0       0.0  57.280197  \\\npbmc_10  0.081115   0.0  0.086782  0.00000         0.0       0.0  72.275326   \npbmc_12  0.000000   0.0  0.188464  0.03157         0.0       0.0  50.997427   \n\n          EFCAB12       A1BG  A1CF  \npbmc_1   0.252188  10.863071   0.0  \npbmc_10  0.095742  14.785649   0.0  \npbmc_12  0.100608   7.492537   0.0  "
                     },
-                    "execution_count": 15,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "bulks.iloc[:, :10].head()"
             ]
@@ -131,19 +131,19 @@
             "metadata": {},
             "source": [
                 "### Convert to AnnData object"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 7,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-03-07T18:31:49.181062Z",
-                    "start_time": "2024-03-07T18:31:49.178366Z"
+                    "end_time": "2024-03-25T16:15:38.118620Z",
+                    "start_time": "2024-03-25T16:15:38.098633Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "sc_adata = AnnData(sc_counts, obs=annotations.to_frame(name=\"cell_type\"))"
             ]
@@ -166,44 +166,44 @@
             "outputs": [],
             "source": [
                 "estimations, signature_result = rectangle.rectangle(sc_adata, bulks)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 9,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-03-07T18:32:46.333109Z",
-                    "start_time": "2024-03-07T18:32:46.329466Z"
+                    "end_time": "2024-03-25T16:18:17.737030Z",
+                    "start_time": "2024-03-25T16:18:17.731946Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>B cells</th>\n      <th>Monocytes</th>\n      <th>NK cells</th>\n      <th>Plasma cells</th>\n      <th>T cells CD4 conv</th>\n      <th>T cells CD8</th>\n      <th>Tregs</th>\n      <th>mDC</th>\n      <th>pDC</th>\n      <th>Unknown</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>pbmc_1</th>\n      <td>-1.653677e-18</td>\n      <td>0.105667</td>\n      <td>0.029340</td>\n      <td>0.008662</td>\n      <td>3.723346e-01</td>\n      <td>5.698229e-02</td>\n      <td>1.376688e-02</td>\n      <td>0.164630</td>\n      <td>0.248618</td>\n      <td>0.0</td>\n    </tr>\n    <tr>\n      <th>pbmc_10</th>\n      <td>1.641017e-17</td>\n      <td>0.242756</td>\n      <td>0.061698</td>\n      <td>0.001183</td>\n      <td>2.935494e-16</td>\n      <td>3.265707e-17</td>\n      <td>-3.973413e-17</td>\n      <td>0.278038</td>\n      <td>0.416326</td>\n      <td>0.0</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
-                        "text/plain": "              B cells  Monocytes  NK cells  Plasma cells  T cells CD4 conv   \npbmc_1  -1.653677e-18   0.105667  0.029340      0.008662      3.723346e-01  \\\npbmc_10  1.641017e-17   0.242756  0.061698      0.001183      2.935494e-16   \n\n          T cells CD8         Tregs       mDC       pDC  Unknown  \npbmc_1   5.698229e-02  1.376688e-02  0.164630  0.248618      0.0  \npbmc_10  3.265707e-17 -3.973413e-17  0.278038  0.416326      0.0  "
+                        "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>B cells</th>\n      <th>ILC</th>\n      <th>Monocytes</th>\n      <th>NK cells</th>\n      <th>Plasma cells</th>\n      <th>Platelet</th>\n      <th>T cells CD4 conv</th>\n      <th>T cells CD8</th>\n      <th>Tregs</th>\n      <th>mDC</th>\n      <th>pDC</th>\n      <th>Unknown</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>pbmc_1</th>\n      <td>0.075919</td>\n      <td>0.001291</td>\n      <td>0.279064</td>\n      <td>0.046658</td>\n      <td>0.010834</td>\n      <td>0.008950</td>\n      <td>0.139600</td>\n      <td>0.268706</td>\n      <td>0.069930</td>\n      <td>0.017415</td>\n      <td>0.001971</td>\n      <td>0.079661</td>\n    </tr>\n    <tr>\n      <th>pbmc_10</th>\n      <td>0.093986</td>\n      <td>0.003410</td>\n      <td>0.316445</td>\n      <td>0.033528</td>\n      <td>0.002279</td>\n      <td>0.036153</td>\n      <td>0.243435</td>\n      <td>0.146063</td>\n      <td>0.011599</td>\n      <td>0.032518</td>\n      <td>0.005273</td>\n      <td>0.075309</td>\n    </tr>\n    <tr>\n      <th>pbmc_12</th>\n      <td>0.060533</td>\n      <td>0.017572</td>\n      <td>0.251589</td>\n      <td>0.114043</td>\n      <td>0.002038</td>\n      <td>0.027041</td>\n      <td>0.119488</td>\n      <td>0.325029</td>\n      <td>0.024586</td>\n      <td>0.027099</td>\n      <td>0.004422</td>\n      <td>0.026560</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
+                        "text/plain": "          B cells       ILC  Monocytes  NK cells  Plasma cells  Platelet   \npbmc_1   0.075919  0.001291   0.279064  0.046658      0.010834  0.008950  \\\npbmc_10  0.093986  0.003410   0.316445  0.033528      0.002279  0.036153   \npbmc_12  0.060533  0.017572   0.251589  0.114043      0.002038  0.027041   \n\n         T cells CD4 conv  T cells CD8     Tregs       mDC       pDC   Unknown  \npbmc_1           0.139600     0.268706  0.069930  0.017415  0.001971  0.079661  \npbmc_10          0.243435     0.146063  0.011599  0.032518  0.005273  0.075309  \npbmc_12          0.119488     0.325029  0.024586  0.027099  0.004422  0.026560  "
                     },
-                    "execution_count": 18,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "estimations"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "signature_result is a [`RectangleSignatureResult`](../generated/rectanglepy.pp.RectangleSignatureResult.rst) object"
+                "signature_result is a [`RectangleSignatureResult`](../generated/rectanglepy.pp.RectangleSignatureResult.rst) object. Results of estimations vary slightly from machine to machine (due to difference in theunderlying linear algebra packages)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
```

### Comparing `rectanglepy-0.1.0/src/rectanglepy/rectangle.py` & `rectanglepy-0.1.2/src/rectanglepy/rectangle.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,17 +101,17 @@
 def load_tutorial_data() -> tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]:
     """Loads the single-cell count data, annotations, and bulk data from the tutorial.
 
     Returns
     -------
     The single-cell count data, annotations, and bulk data.
     """
-    with resource_stream(__name__, "data/hao1_annotations_small.csv") as annotations_file:
-        annotations = pd.read_csv(annotations_file, index_col=0)["0"]
+    with resource_stream(__name__, "data/hao1_annotations_small.zip") as annotations_file:
+        annotations = pd.read_csv(annotations_file, index_col=0, compression="zip")["0"]
 
-    with resource_stream(__name__, "data/hao1_counts_small.csv") as counts_file:
-        sc_counts = pd.read_csv(counts_file, index_col=0).astype("int")
+    with resource_stream(__name__, "data/hao1_counts_small.zip") as counts_file:
+        sc_counts = pd.read_csv(counts_file, index_col=0, compression="zip").astype("int")
 
-    with resource_stream(__name__, "data/small_fino_bulks.csv") as bulks_file:
-        bulks = pd.read_csv(bulks_file, index_col=0)
+    with resource_stream(__name__, "data/small_fino_bulks.zip") as bulks_file:
+        bulks = pd.read_csv(bulks_file, index_col=0, compression="zip")
 
     return sc_counts.T, annotations, bulks.T
```

### Comparing `rectanglepy-0.1.0/src/rectanglepy/pp/create_signature.py` & `rectanglepy-0.1.2/src/rectanglepy/pp/create_signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,16 +138,14 @@
     for i, cell_type in enumerate(countsig.columns):
         logger.info(f"Running DE analysis for {cell_type}")
         condition = np.zeros(len(countsig.columns))
         condition[i] = 1
         clinical_df = pd.DataFrame({"condition": condition}, index=countsig.columns)
         dds = DeseqDataSet(counts=count_df, metadata=clinical_df, design_factors="condition", quiet=True, n_cpus=n_cpus)
         dds.deseq2()
-        dds.varm["LFC"] = dds.varm["LFC"].round(4)
-        dds.varm["dispersions"] = dds.varm["dispersions"].round(3)
 
         stat_res = DeseqStats(dds, n_cpus=n_cpus, quiet=True)
         stat_res.summary(quiet=True)
         stat_res.lfc_shrink()
         results[cell_type] = stat_res.results_df
 
     return results
```

### Comparing `rectanglepy-0.1.0/src/rectanglepy/pp/rectangle_signature.py` & `rectanglepy-0.1.2/src/rectanglepy/pp/rectangle_signature.py`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/src/rectanglepy/tl/deconvolution.py` & `rectanglepy-0.1.2/src/rectanglepy/tl/deconvolution.py`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/tests/test_pp.py` & `rectanglepy-0.1.2/tests/test_pp.py`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/tests/test_rectangle.py` & `rectanglepy-0.1.2/tests/test_rectangle.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,23 +12,23 @@
     assert isinstance(bulks, pd.DataFrame)
 
 
 def test_rectangle():
     sc_data, annotations, bulks = rectanglepy.load_tutorial_data()
     sc_data_adata = AnnData(sc_data, obs=annotations.to_frame(name="cell_type"))
 
-    result = rectanglepy.rectangle(sc_data_adata, bulks, optimize_cutoffs=False, p=0.1, lfc=0.5)
+    result = rectanglepy.rectangle(sc_data_adata, bulks)
 
     assert isinstance(result[0], pd.DataFrame)
     assert isinstance(result[1], RectangleSignatureResult)
 
 
 def test_rectangle_consensus():
     sc_data, annotations, bulks = rectanglepy.load_tutorial_data()
     sc_data_adata = AnnData(sc_data, obs=annotations.to_frame(name="cell_type"))
 
     result = rectanglepy.rectangle(
-        sc_data_adata, bulks, optimize_cutoffs=False, p=0.5, lfc=0.0, consensus_runs=2, sample_size=9
+        sc_data_adata, bulks, optimize_cutoffs=False, p=0.5, lfc=0.0, consensus_runs=2, sample_size=50
     )
 
     assert isinstance(result[0], pd.DataFrame)
     assert isinstance(result[1], RectangleSignatureResult)
```

### Comparing `rectanglepy-0.1.0/tests/test_tl.py` & `rectanglepy-0.1.2/tests/test_tl.py`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/tests/data/TIL10_signature.txt` & `rectanglepy-0.1.2/tests/data/TIL10_signature.txt`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/tests/data/bulk_small.csv` & `rectanglepy-0.1.2/tests/data/bulk_small.csv`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/tests/data/quanTIseq_SimRNAseq_mixture_smaller.csv` & `rectanglepy-0.1.2/tests/data/quanTIseq_SimRNAseq_mixture_smaller.csv`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/tests/data/quanTIseq_SimRNAseq_read_fractions_small.txt` & `rectanglepy-0.1.2/tests/data/quanTIseq_SimRNAseq_read_fractions_small.txt`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/tests/data/sc_object_small.csv` & `rectanglepy-0.1.2/tests/data/sc_object_small.csv`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/tests/data/signature_hao1.csv` & `rectanglepy-0.1.2/tests/data/signature_hao1.csv`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/LICENSE` & `rectanglepy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.0/README.md` & `rectanglepy-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 ## Citation
 
 > t.b.a
 
 [scverse-discourse]: https://discourse.scverse.org/
 [issue-tracker]: https://github.com/ComputationalBiomedicineGroup/Rectangle/issues
-[changelog]: https://Rectanglepy.readthedocs.io/latest/changelog.html
+[changelog]: https://rectanglepy.readthedocs.io/changelog.html
 [link-docs]: https://Rectanglepy.readthedocs.io
 [link-api]: https://rectanglepy.readthedocs.io/api.html
```

### Comparing `rectanglepy-0.1.0/pyproject.toml` & `rectanglepy-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "rectanglepy"
-version = "0.1.0"
+version = "0.1.2"
 description = "Hierarchical deconvolution of bulk  transcriptomics"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 authors = [
     {name = "Bernhard Eder"},
 ]
```

### Comparing `rectanglepy-0.1.0/PKG-INFO` & `rectanglepy-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rectanglepy
-Version: 0.1.0
+Version: 0.1.2
 Summary: Hierarchical deconvolution of bulk  transcriptomics
 Project-URL: Documentation, https://rectanglepy.readthedocs.io/
 Project-URL: Source, https://github.com/ComputationalBiomedicineGroup/Rectangle
 Project-URL: Home-page, https://github.com/ComputationalBiomedicineGroup/Rectangle
 Author: Bernhard Eder
 Maintainer-email: Bernhard Eder <Bernhard.Eder@student.uibk.ac.at>
 License: MIT License
@@ -93,10 +93,10 @@
 
 ## Citation
 
 > t.b.a
 
 [scverse-discourse]: https://discourse.scverse.org/
 [issue-tracker]: https://github.com/ComputationalBiomedicineGroup/Rectangle/issues
-[changelog]: https://Rectanglepy.readthedocs.io/latest/changelog.html
+[changelog]: https://rectanglepy.readthedocs.io/changelog.html
 [link-docs]: https://Rectanglepy.readthedocs.io
 [link-api]: https://rectanglepy.readthedocs.io/api.html
```

