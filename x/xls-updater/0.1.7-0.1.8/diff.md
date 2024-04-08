# Comparing `tmp/xls_updater-0.1.7.tar.gz` & `tmp/xls_updater-0.1.8.tar.gz`

## Comparing `xls_updater-0.1.7.tar` & `xls_updater-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.pylintrc
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 xls_updater-0.1.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 xls_updater-0.1.7/Makefile
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 xls_updater-0.1.7/requirements-dev.txt
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 xls_updater-0.1.7/requirements-test.txt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 xls_updater-0.1.7/requirements.txt
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/actions/prepare-environment/action.yaml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/black.yml
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/isort.yml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/mypy.yml
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/validation.yaml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/test_app.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/test_big.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/test_cli.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/test_samples.py
--rw-r--r--   0        0        0    30208 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/samples/sample1.xls
--rw-r--r--   0        0        0    39424 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/samples/sample2.xls
--rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/samples/sample3.xls
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xls_updater-0.1.7/xls_updater/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xls_updater-0.1.7/xls_updater/__main__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 xls_updater-0.1.7/xls_updater/app.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 xls_updater-0.1.7/xls_updater/cli.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.gitignore
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 xls_updater-0.1.7/README.md
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 xls_updater-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 xls_updater-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.pylintrc
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 xls_updater-0.1.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 xls_updater-0.1.8/Makefile
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 xls_updater-0.1.8/requirements-dev.txt
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 xls_updater-0.1.8/requirements-test.txt
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/actions/prepare-environment/action.yaml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/black.yml
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/isort.yml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/validation.yaml
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/test_app.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/test_big.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/test_cli.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/test_samples.py
+-rw-r--r--   0        0        0    30208 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/samples/sample1.xls
+-rw-r--r--   0        0        0    39424 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/samples/sample2.xls
+-rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/samples/sample3.xls
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xls_updater-0.1.8/xls_updater/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xls_updater-0.1.8/xls_updater/__main__.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 xls_updater-0.1.8/xls_updater/app.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 xls_updater-0.1.8/xls_updater/cli.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 xls_updater-0.1.8/README.md
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 xls_updater-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 xls_updater-0.1.8/PKG-INFO
```

### Comparing `xls_updater-0.1.7/.pre-commit-config.yaml` & `xls_updater-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/.pylintrc` & `xls_updater-0.1.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/CONTRIBUTING.md` & `xls_updater-0.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/Makefile` & `xls_updater-0.1.8/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 SHELL=/bin/bash
 
 run:
 	python3 xls_updater/app.py
 
 setup:
-	python3 -m pip install .
+	python3 -m pip install '.[dev, test, release]'
 
 setup-dev:
 	python3 -m pip install --editable '.[dev]'
 
 setup-test:
 	python3 -m pip install --editable '.[test]'
 
+setup-relase:
+	python3 -m pip install --editable '.[release]'
+
 pip-clean:
 	python3 -m pip uninstall -y -r <(pip freeze)
 
 clean:
 	rm -rf **/__pycache__ .pytest_cache/ dist/ .mypy_cache/ .coverage *.egg-info build
 
 check-black:
@@ -45,18 +48,9 @@
 tests: | pytest coverage
 
 check-mypy:
 	python3 -m mypy -p xls_updater
 
 compile:
 	python3 -m pip install --upgrade pip-tools
-	python3 -m piptools compile -o requirements.txt pyproject.toml
 	python3 -m piptools compile -o requirements-dev.txt --extra dev pyproject.toml
 	python3 -m piptools compile -o requirements-test.txt --extra test pyproject.toml
-
-build:
-	python3 -m pip install --upgrade build
-	python3 -m build
-
-publish:
-	python3 -m pip install --upgrade twine
-	python3 -m twine upload dist/*
```

### Comparing `xls_updater-0.1.7/requirements-dev.txt` & `xls_updater-0.1.8/requirements-dev.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-about-time==4.2.1         # via alive-progress
-alive-progress==3.1.5     # via xls-updater (pyproject.toml)
 astroid==3.0.1            # via pylint
 black==23.10.1            # via xls-updater (pyproject.toml)
 cfgv==3.4.0               # via pre-commit
 click==8.1.7              # via black, xls-updater (pyproject.toml)
 dill==0.3.7               # via pylint
 distlib==0.3.7            # via virtualenv
 et-xmlfile==1.1.0         # via openpyxl
 filelock==3.12.4          # via virtualenv
-grapheme==0.6.0           # via alive-progress
 identify==2.5.30          # via pre-commit
 isort==5.12.0             # via pylint, xls-updater (pyproject.toml)
 mccabe==0.7.0             # via pylint
 mypy==1.8.0               # via xls-updater (pyproject.toml)
 mypy-extensions==1.0.0    # via black, mypy
 nodeenv==1.8.0            # via pre-commit
 openpyxl==3.1.2           # via xls-updater (pyproject.toml)
@@ -20,13 +17,14 @@
 pathspec==0.11.2          # via black
 platformdirs==3.11.0      # via black, pylint, virtualenv
 pre-commit==3.5.0         # via xls-updater (pyproject.toml)
 pylint==3.0.2             # via xls-updater (pyproject.toml)
 pyyaml==6.0.1             # via pre-commit
 tomli==2.0.1              # via black, mypy, pylint
 tomlkit==0.12.1           # via pylint
+tqdm==4.66.2              # via xls-updater (pyproject.toml)
 typing-extensions==4.9.0  # via astroid, black, mypy
 virtualenv==20.24.6       # via pre-commit
 xlrd==2.0.1               # via xls-updater (pyproject.toml)
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `xls_updater-0.1.7/requirements-test.txt` & `xls_updater-0.1.8/requirements-test.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-about-time==4.2.1         # via alive-progress
-alive-progress==3.1.5     # via xls-updater (pyproject.toml)
 click==8.1.7              # via xls-updater (pyproject.toml)
 coverage==7.4.4           # via pytest-cov
 et-xmlfile==1.1.0         # via openpyxl
 exceptiongroup==1.2.0     # via pytest
-grapheme==0.6.0           # via alive-progress
 humanize==4.9.0           # via xls-updater (pyproject.toml)
 iniconfig==2.0.0          # via pytest
 numpy==1.26.4             # via pandas, pyarrow
 openpyxl==3.1.2           # via xls-updater (pyproject.toml)
 packaging==24.0           # via pytest
 pandas==2.2.1             # via xls-updater (pyproject.toml)
 pluggy==1.4.0             # via pytest
@@ -16,10 +13,11 @@
 pytest==8.1.1             # via pytest-cov, pytest-mock, xls-updater (pyproject.toml)
 pytest-cov==5.0.0         # via xls-updater (pyproject.toml)
 pytest-mock==3.14.0       # via xls-updater (pyproject.toml)
 python-dateutil==2.9.0.post0  # via pandas
 pytz==2024.1              # via pandas
 six==1.16.0               # via python-dateutil
 tomli==2.0.1              # via coverage, pytest
+tqdm==4.66.2              # via xls-updater (pyproject.toml)
 tzdata==2024.1            # via pandas
 xlrd==2.0.1               # via xls-updater (pyproject.toml)
 xlwt==1.3.0               # via xls-updater (pyproject.toml)
```

### Comparing `xls_updater-0.1.7/.github/workflows/coverage.yml` & `xls_updater-0.1.8/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/.github/workflows/publish.yml` & `xls_updater-0.1.8/.github/workflows/publish.yml`

 * *Files 5% similar despite different names*

```diff
@@ -39,22 +39,26 @@
 
       - name: Checkout
         uses: actions/checkout@v4
         with:
           ref: ${{ github.ref }}
           fetch-depth: 0
 
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          python -m pip install '.[release]'
+
       - name: Bump Version
         id: bump_version
         env:
           BUMP_TYPE: ${{ github.event.inputs.bump_type }}
         run: |
-          python -m pip install semvergit
           echo "Bumping type: ${{ env.BUMP_TYPE }}"
-          new_version=$(semvergit -t ${{ env.BUMP_TYPE }} -v)
+          new_version=$(python -m semvergit -t ${{ env.BUMP_TYPE }} -v)
           echo "new_version=$new_version" >> $GITHUB_OUTPUT
 
       - name: Create Github Release
         if: ${{ github.event.inputs.release == 'true' }}
         id: create_release
         uses: softprops/action-gh-release@v1
         env:
@@ -63,16 +67,16 @@
           tag_name: ${{ steps.bump_version.outputs.new_version }}
           release_name: ${{ steps.bump_version.outputs.new_version }}
           body: New Release ${{ steps.bump_version.outputs.new_version }}
 
       - name: Build Package
         if: ${{ github.event.inputs.publish == 'true' }}
         run: |
-          make build
+          python -m build
 
       - name: Publish To PyPI
         if: ${{ github.event.inputs.publish == 'true' }}
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
           TWINE_USERNAME: ${{ secrets.PYPI_API_USER }}
         run: |
-          make publish
+          python -m twine upload dist/*
```

### Comparing `xls_updater-0.1.7/.github/workflows/pytest.yml` & `xls_updater-0.1.8/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/.github/workflows/validation.yaml` & `xls_updater-0.1.8/.github/workflows/validation.yaml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/tests/test_app.py` & `xls_updater-0.1.8/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/tests/test_big.py` & `xls_updater-0.1.8/tests/test_big.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/tests/test_cli.py` & `xls_updater-0.1.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/tests/test_samples.py` & `xls_updater-0.1.8/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/tests/samples/sample1.xls` & `xls_updater-0.1.8/tests/samples/sample1.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/tests/samples/sample2.xls` & `xls_updater-0.1.8/tests/samples/sample2.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/tests/samples/sample3.xls` & `xls_updater-0.1.8/tests/samples/sample3.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/xls_updater/app.py` & `xls_updater-0.1.8/xls_updater/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module to convert xls to newer xlsx."""
 
 import pathlib
 
 import xlrd
-from alive_progress import alive_bar
 from openpyxl.workbook import Workbook
+from tqdm import tqdm
 
 
 def convert_xls_to_xlsx(src_file_path: pathlib.Path) -> None:
     """Function converting the given xls file to the newer xlsx format."""
     dst_file_path = src_file_path.with_suffix(".xlsx")
     book_xls = xlrd.open_workbook(src_file_path)
     book_xlsx = Workbook()
@@ -16,22 +16,22 @@
     sheet_names = book_xls.sheet_names()
 
     total_cells = 0
     for sheet_name in sheet_names:
         sheet_xls = book_xls.sheet_by_name(sheet_name)
         total_cells += sheet_xls.nrows * sheet_xls.ncols
 
-    with alive_bar(total_cells, title="Converting xls to xlsx", monitor=False, stats="{eta}") as progress_bar:
+    with tqdm(total=total_cells, desc="Converting xls to xlsx") as progress_bar:
         for sheet_index, sheet_name in enumerate(sheet_names):
             sheet_xls = book_xls.sheet_by_name(sheet_name)
             if sheet_index == 0:
                 sheet_xlsx = book_xlsx.active
                 sheet_xlsx.title = sheet_name
             else:
                 sheet_xlsx = book_xlsx.create_sheet(title=sheet_name)
 
             for row in range(0, sheet_xls.nrows):
                 for col in range(0, sheet_xls.ncols):
                     sheet_xlsx.cell(row=row + 1, column=col + 1).value = sheet_xls.cell_value(row, col)
-                    progress_bar()  # pylint: disable=not-callable
+                    progress_bar.update(1)
 
     book_xlsx.save(dst_file_path)
```

### Comparing `xls_updater-0.1.7/.gitignore` & `xls_updater-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/README.md` & `xls_updater-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.7/pyproject.toml` & `xls_updater-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Topic :: Office/Business :: Financial :: Spreadsheet",
     "Topic :: File Formats",
 ]
 dependencies = [
     "click==8.1.7",
     "openpyxl==3.1.2",
     "xlrd==2.0.1",
-    "alive_progress==3.1.5"
+    "tqdm==4.66.2"
 ]
 [project.optional-dependencies]
 dev = [
     "black",
     "isort",
     "pylint",
     "pre-commit",
@@ -44,14 +44,19 @@
     "pyarrow==15.*",
     "humanize",
     "pandas==2.*",
     "pytest",
     "pytest-cov",
     "pytest_mock",
 ]
+release = [
+    "semvergit",
+    "build",
+    "twine",
+]
 
 [project.scripts]
 xls-updater = "xls_updater.cli:cli"
 
 [project.urls]
 homepage = "https://github.com/Tranquility2/xls_updater"
 repository = "https://github.com/Tranquility2/xls_updater"
```

### Comparing `xls_updater-0.1.7/PKG-INFO` & `xls_updater-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.3
 Name: xls-updater
-Version: 0.1.7
+Version: 0.1.8
 Summary: Convert legacy xls data to newer xlsx format.
 Project-URL: homepage, https://github.com/Tranquility2/xls_updater
 Project-URL: repository, https://github.com/Tranquility2/xls_updater
 Author-email: Roy Moore <roy@moore.co.il>
 Keywords: converter,excel,fileformat,spreadsheet,xls,xlsx
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: File Formats
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Requires-Python: >=3.10
-Requires-Dist: alive-progress==3.1.5
 Requires-Dist: click==8.1.7
 Requires-Dist: openpyxl==3.1.2
+Requires-Dist: tqdm==4.66.2
 Requires-Dist: xlrd==2.0.1
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
+Provides-Extra: release
+Requires-Dist: build; extra == 'release'
+Requires-Dist: semvergit; extra == 'release'
+Requires-Dist: twine; extra == 'release'
 Provides-Extra: test
 Requires-Dist: humanize; extra == 'test'
 Requires-Dist: pandas==2.*; extra == 'test'
 Requires-Dist: pyarrow==15.*; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-mock; extra == 'test'
```

