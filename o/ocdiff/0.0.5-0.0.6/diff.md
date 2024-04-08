# Comparing `tmp/ocdiff-0.0.5.tar.gz` & `tmp/ocdiff-0.0.6.tar.gz`

## Comparing `ocdiff-0.0.5.tar` & `ocdiff-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 ocdiff-0.0.5/Cargo.toml
--rw-r--r--   0      501       20     2237 2024-04-08 10:14:46.000000 ocdiff-0.0.5/.github/workflows/ci.yml
--rw-r--r--   0      501       20     3097 2024-04-08 10:14:46.000000 ocdiff-0.0.5/.gitignore
--rw-r--r--   0      501       20     1071 2024-04-08 10:14:46.000000 ocdiff-0.0.5/LICENSE
--rw-r--r--   0      501       20      551 2024-04-08 10:14:46.000000 ocdiff-0.0.5/README.md
--rw-r--r--   0      501       20      139 2024-04-08 10:14:46.000000 ocdiff-0.0.5/python/ocdiff/__init__.py
--rw-r--r--   0      501       20      152 2024-04-08 10:14:46.000000 ocdiff-0.0.5/python/ocdiff/__init__.pyi
--rw-r--r--   0      501       20     1505 2024-04-08 10:14:46.000000 ocdiff-0.0.5/python/ocdiff/helpers.py
--rw-r--r--   0      501       20     8914 2024-04-08 10:14:46.000000 ocdiff-0.0.5/src/lib.rs
--rw-r--r--   0      501       20      788 2024-04-08 10:14:46.000000 ocdiff-0.0.5/tests/a.json
--rw-r--r--   0      501       20      737 2024-04-08 10:14:46.000000 ocdiff-0.0.5/tests/b.json
--rw-r--r--   0      501       20     4398 2024-04-08 10:14:46.000000 ocdiff-0.0.5/tests/expected.html
--rw-r--r--   0      501       20      369 2024-04-08 10:14:46.000000 ocdiff-0.0.5/tests/test_ocdiff.py
--rw-r--r--   0      501       20     8716 2024-04-08 10:14:46.000000 ocdiff-0.0.5/Cargo.lock
--rw-r--r--   0      501       20     1283 2024-04-08 10:14:46.000000 ocdiff-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 ocdiff-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 ocdiff-0.0.6/Cargo.toml
+-rw-r--r--   0      501       20     2728 2024-04-08 10:26:05.000000 ocdiff-0.0.6/.github/workflows/ci.yml
+-rw-r--r--   0      501       20     3097 2024-04-08 10:26:05.000000 ocdiff-0.0.6/.gitignore
+-rw-r--r--   0      501       20     1071 2024-04-08 10:26:05.000000 ocdiff-0.0.6/LICENSE
+-rw-r--r--   0      501       20      551 2024-04-08 10:26:05.000000 ocdiff-0.0.6/README.md
+-rw-r--r--   0      501       20      139 2024-04-08 10:26:05.000000 ocdiff-0.0.6/python/ocdiff/__init__.py
+-rw-r--r--   0      501       20      152 2024-04-08 10:26:05.000000 ocdiff-0.0.6/python/ocdiff/__init__.pyi
+-rw-r--r--   0      501       20     1505 2024-04-08 10:26:05.000000 ocdiff-0.0.6/python/ocdiff/helpers.py
+-rw-r--r--   0      501       20     8914 2024-04-08 10:26:05.000000 ocdiff-0.0.6/src/lib.rs
+-rw-r--r--   0      501       20      788 2024-04-08 10:26:05.000000 ocdiff-0.0.6/tests/a.json
+-rw-r--r--   0      501       20      737 2024-04-08 10:26:05.000000 ocdiff-0.0.6/tests/b.json
+-rw-r--r--   0      501       20     4398 2024-04-08 10:26:05.000000 ocdiff-0.0.6/tests/expected.html
+-rw-r--r--   0      501       20      369 2024-04-08 10:26:05.000000 ocdiff-0.0.6/tests/test_ocdiff.py
+-rw-r--r--   0      501       20     8716 2024-04-08 10:26:05.000000 ocdiff-0.0.6/Cargo.lock
+-rw-r--r--   0      501       20     1283 2024-04-08 10:26:05.000000 ocdiff-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 ocdiff-0.0.6/PKG-INFO
```

### Comparing `ocdiff-0.0.5/.github/workflows/ci.yml` & `ocdiff-0.0.6/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
   build:
     name: build py${{ matrix.python-version }} on ${{ matrix.platform || matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os:
           - macos
+          - linux
+          - windows
         python-version:
           - '3.11'
         include:
           - os: ubuntu
             platform: linux
           - os: windows
             ls: dir
@@ -41,16 +43,15 @@
           toolchain: 1.74.0
           profile: minimal
           default: true
           override: true
 
       - name: install python dependencies
         run: |
-          pip install twine
-          pip install -U build
+          pip install build twine
 
       - name: build ${{ matrix.platform || matrix.os }} binaries
         run: python -m build
         env:
           CIBW_BUILD: '${{ matrix.cibw-version }}-*'
           CIBW_SKIP: '*-win32'
           CIBW_PLATFORM: ${{ matrix.platform || matrix.os }}
@@ -60,14 +61,27 @@
             rustup show
           CIBW_BEFORE_BUILD_LINUX: >
             curl https://sh.rustup.rs -sSf | sh -s -- --profile=minimal -y &&
             rustup show
           CIBW_TEST_COMMAND: "pytest {project}/tests"
           CIBW_TEST_EXTRAS: test
 
+      - name: build windows 32bit binaries
+        if: matrix.os == 'windows'
+        run: python -m build
+        env:
+          CIBW_BUILD: '${{ matrix.cibw-version }}-win32'
+          CIBW_PLATFORM: windows
+          CIBW_ENVIRONMENT: 'PATH="$UserProfile\.cargo\bin;$PATH"'
+          CIBW_BEFORE_BUILD: >
+            rustup default stable-i686-pc-windows-msvc &&
+            rustup show
+          CIBW_TEST_COMMAND: "pytest {project}/tests"
+          CIBW_TEST_EXTRAS: test
+
       # - name: Upload to github releases
       #   if: startsWith(github.ref, 'refs/tags/')
       #   uses: svenstaro/upload-release-action@v2
       #   with:
       #     repo_token: ${{ secrets.GITHUB_TOKEN }}
       #     file: dist/*.whl
       #     file_glob: true
```

### Comparing `ocdiff-0.0.5/.gitignore` & `ocdiff-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.5/LICENSE` & `ocdiff-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.5/README.md` & `ocdiff-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.5/python/ocdiff/helpers.py` & `ocdiff-0.0.6/python/ocdiff/helpers.py`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.5/src/lib.rs` & `ocdiff-0.0.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.5/tests/a.json` & `ocdiff-0.0.6/tests/a.json`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.5/tests/b.json` & `ocdiff-0.0.6/tests/b.json`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.5/tests/expected.html` & `ocdiff-0.0.6/tests/expected.html`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.5/Cargo.lock` & `ocdiff-0.0.6/Cargo.lock`

 * *Files identical despite different names*

### Comparing `ocdiff-0.0.5/pyproject.toml` & `ocdiff-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ocdiff"
-version = "0.0.5"
+version = "0.0.6"
 description = "difftastic Python wrapper"
 readme = "README.md"
 requires-python = ">=3.11"
 license = { file = "LICENSE" }
 keywords = ["diff"]
 authors = [{ name = "Oliver Russell", email = "ojhrussell@gmail.com" }]
 maintainers = [{ name = "Oliver Russell", email = "ojhrussell@gmail.com" }]
```

### Comparing `ocdiff-0.0.5/PKG-INFO` & `ocdiff-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ocdiff
-Version: 0.0.5
+Version: 0.0.6
 Classifier: Programming Language :: Python
 Requires-Dist: maturin ==1.4.0 ; extra == 'dev'
 Requires-Dist: pytest ==7.* ; extra == 'dev'
 Requires-Dist: mypy ==1.6.* ; extra == 'dev'
 Requires-Dist: pip ==24.0 ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
```

