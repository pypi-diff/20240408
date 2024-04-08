# Comparing `tmp/polars_qt-0.1.1.tar.gz` & `tmp/polars_qt-0.1.2.tar.gz`

## Comparing `polars_qt-0.1.1.tar` & `polars_qt-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 polars_qt-0.1.1/Cargo.toml
--rw-r--r--   0     1001      127     3533 2024-04-04 14:52:55.000000 polars_qt-0.1.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127       74 2024-04-04 14:52:55.000000 polars_qt-0.1.1/.gitignore
--rw-r--r--   0     1001      127        8 2024-04-04 14:52:55.000000 polars_qt-0.1.1/.python-version
--rw-r--r--   0     1001      127      601 2024-04-04 14:52:55.000000 polars_qt-0.1.1/Makefile
--rw-r--r--   0     1001      127     1448 2024-04-04 14:52:55.000000 polars_qt-0.1.1/README.md
--rw-r--r--   0     1001      127       37 2024-04-04 14:52:55.000000 polars_qt-0.1.1/polars_qt/__init__.py
--rw-r--r--   0     1001      127      960 2024-04-04 14:52:55.000000 polars_qt-0.1.1/polars_qt/funcs.py
--rw-r--r--   0     1001      127      437 2024-04-04 14:52:55.000000 polars_qt-0.1.1/polars_qt/qt.py
--rw-r--r--   0     1001      127     2597 2024-04-04 14:52:55.000000 polars_qt-0.1.1/polars_qt/utils.py
--rw-r--r--   0     1001      127       34 2024-04-04 14:52:55.000000 polars_qt-0.1.1/requirements.txt
--rw-r--r--   0     1001      127       42 2024-04-04 14:52:55.000000 polars_qt-0.1.1/rust-toolchain.toml
--rw-r--r--   0     1001      127      473 2024-04-04 14:52:55.000000 polars_qt-0.1.1/src/if_then.rs
--rw-r--r--   0     1001      127      237 2024-04-04 14:52:55.000000 polars_qt-0.1.1/src/lib.rs
--rw-r--r--   0     1001      127     3250 2024-04-04 14:52:55.000000 polars_qt-0.1.1/src/rolling_rank.rs
--rw-r--r--   0     1001      127      837 2024-04-04 14:52:55.000000 polars_qt-0.1.1/tests/test_if_then.py
--rw-r--r--   0     1001      127      587 2024-04-04 14:52:55.000000 polars_qt-0.1.1/tests/test_rolling_rank.py
--rw-r--r--   0     1001      127    33830 2024-04-04 14:53:07.000000 polars_qt-0.1.1/Cargo.lock
--rw-r--r--   0     1001      127      550 2024-04-04 14:52:55.000000 polars_qt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 polars_qt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 polars_qt-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      127     3716 2024-04-08 06:47:06.000000 polars_qt-0.1.2/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      100 2024-04-08 06:47:06.000000 polars_qt-0.1.2/.gitignore
+-rw-r--r--   0     1001      127        8 2024-04-08 06:47:06.000000 polars_qt-0.1.2/.python-version
+-rw-r--r--   0     1001      127      541 2024-04-08 06:47:06.000000 polars_qt-0.1.2/Makefile
+-rw-r--r--   0     1001      127     1786 2024-04-08 06:47:06.000000 polars_qt-0.1.2/README.md
+-rw-r--r--   0     1001      127       38 2024-04-08 06:47:06.000000 polars_qt-0.1.2/polars_qt/__init__.py
+-rw-r--r--   0     1001      127     2893 2024-04-08 06:47:06.000000 polars_qt-0.1.2/polars_qt/funcs.py
+-rw-r--r--   0     1001      127     1408 2024-04-08 06:47:06.000000 polars_qt-0.1.2/polars_qt/qt.py
+-rw-r--r--   0     1001      127     2567 2024-04-08 06:47:06.000000 polars_qt-0.1.2/polars_qt/utils.py
+-rw-r--r--   0     1001      127       34 2024-04-08 06:47:06.000000 polars_qt-0.1.2/requirements.txt
+-rw-r--r--   0     1001      127       42 2024-04-08 06:47:06.000000 polars_qt-0.1.2/rust-toolchain.toml
+-rw-r--r--   0     1001      127    13255 2024-04-08 06:47:06.000000 polars_qt-0.1.2/src/equity.rs
+-rw-r--r--   0     1001      127      649 2024-04-08 06:47:06.000000 polars_qt-0.1.2/src/if_then.rs
+-rw-r--r--   0     1001      127      276 2024-04-08 06:47:06.000000 polars_qt-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      127     3250 2024-04-08 06:47:06.000000 polars_qt-0.1.2/src/rolling_rank.rs
+-rw-r--r--   0     1001      127     1375 2024-04-08 06:47:06.000000 polars_qt-0.1.2/tests/test_equity.py
+-rw-r--r--   0     1001      127      867 2024-04-08 06:47:06.000000 polars_qt-0.1.2/tests/test_if_then.py
+-rw-r--r--   0     1001      127      662 2024-04-08 06:47:06.000000 polars_qt-0.1.2/tests/test_rolling_rank.py
+-rw-r--r--   0     1001      127    33830 2024-04-08 06:47:21.000000 polars_qt-0.1.2/Cargo.lock
+-rw-r--r--   0     1001      127     1726 2024-04-08 06:47:06.000000 polars_qt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.2/PKG-INFO
```

### Comparing `polars_qt-0.1.1/.github/workflows/publish_to_pypi.yml` & `polars_qt-0.1.2/.github/workflows/publish_to_pypi.yml`

 * *Files 10% similar despite different names*

```diff
@@ -38,20 +38,23 @@
           python-version: ${{ matrix.python-version }}
           
 
       - name: Set up Rust
         run: rustup show
       - uses: mozilla-actions/sccache-action@v0.0.3
       - run: make .venv
-      - run: make pre-commit
-      - run: make install
-      - run: make test
+      - run: |
+          source .venv/bin/activate
+          make pre-commit
+          make install
+          make test
 
   linux:
     runs-on: ubuntu-latest
+    if: "startsWith(github.ref, 'refs/tags/')"
     strategy:
       matrix:
         target: [x86_64, x86]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
@@ -69,14 +72,15 @@
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   windows:
     runs-on: windows-latest
+    if: "startsWith(github.ref, 'refs/tags/')"
     strategy:
       matrix:
         target: [x64]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
@@ -96,14 +100,15 @@
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   macos:
     runs-on: macos-latest
+    if: "startsWith(github.ref, 'refs/tags/')"
     strategy:
       matrix:
         target: [x86_64, aarch64]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
```

### Comparing `polars_qt-0.1.1/polars_qt/utils.py` & `polars_qt-0.1.2/polars_qt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import re
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Sequence
 
 import polars as pl
 
 if TYPE_CHECKING:
-    from pathlib import Path
-
     from polars.type_aliases import IntoExpr, PolarsDataType
 
 
 def parse_into_expr(
     expr: IntoExpr,
     *,
     str_as_lit: bool = False,
@@ -77,22 +75,22 @@
         args=args,
         plugin_path=lib,
         function_name=symbol,
         kwargs=kwargs,
         is_elementwise=is_elementwise,
     )
 
+
 def parse_version(version: Sequence[str | int]) -> tuple[int, ...]:
     # Simple version parser; split into a tuple of ints for comparison.
     # vendored from Polars
     if isinstance(version, str):
         version = version.split(".")
     return tuple(int(re.sub(r"\D", "", str(v))) for v in version)
 
 
-
 if parse_version(pl.__version__) < parse_version("0.20.16"):
     from polars.utils.udfs import _get_shared_lib_location
 
     lib: str | Path = _get_shared_lib_location(__file__)
 else:
     lib = Path(__file__).parent
```

### Comparing `polars_qt-0.1.1/src/rolling_rank.rs` & `polars_qt-0.1.2/src/rolling_rank.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.1/tests/test_rolling_rank.py` & `polars_qt-0.1.2/tests/test_rolling_rank.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import polars as pl
-import polars_qt as pq
 from polars.testing import assert_series_equal
 
+import polars_qt as pq
+
+
 def test_rolling_rank():
-    df = pl.DataFrame({
-        'a': [5.2, 4.1, 6.3, None, 10, 4, 5],
-    })
+    df = pl.DataFrame(
+        {
+            "a": [5.2, 4.1, 6.3, None, 10, 4, 5],
+        }
+    )
     df = df.with_columns(
-        pq.rolling_rank(pl.col('a'), 4, min_periods=1, pct=True).alias('a_rank'),
-        pl.col('a').qt.rolling_rank(4, pct=False, rev=True).alias('a_rank2')
+        pq.rolling_rank(pl.col("a"), 4, min_periods=1, pct=True).alias("a_rank"),
+        pl.col("a").qt.rolling_rank(4, pct=False, rev=True).alias("a_rank2"),
+    )
+    assert_series_equal(
+        df["a_rank"],
+        pl.Series([1, 0.5, 1.0, None, 1.0, 1 / 3, 2 / 3]),
+        check_names=False,
+    )
+    assert_series_equal(
+        df["a_rank2"], pl.Series([None, 2.0, 1, None, 1, 3, 2]), check_names=False
     )
-    assert_series_equal(df['a_rank'], pl.Series([1, 0.5, 1.0, None, 1.0, 1/3, 2/3]), check_names=False)
-    assert_series_equal(df['a_rank2'], pl.Series([None, 2., 1, None, 1, 3, 2]), check_names=False)
```

### Comparing `polars_qt-0.1.1/Cargo.lock` & `polars_qt-0.1.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -193,17 +193,17 @@
 name = "foreign_vec"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "a06fddc2749e0528d2813f95e050e87e52c8cbbae56223b9babf73b3e53b0cc6"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -631,15 +631,15 @@
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-qt"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "polars",
  "pyo3",
  "pyo3-polars",
  "serde",
 ]
 
@@ -903,17 +903,17 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
```

### Comparing `polars_qt-0.1.1/PKG-INFO` & `polars_qt-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-Metadata-Version: 2.3
-Name: polars-qt
-Version: 0.1.1
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: polars >=0.20.16
-Author-email: Teamon9161 <teamon9161@163.com>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-
 # polars_qt
+[![PyPI](https://img.shields.io/pypi/v/polars_qt)](https://pypi.org/project/polars_qt)
 
-Add a qt namespace for polars.
+Useful Quant expressions for polars implemented by polars plugin.
 
 Currently :
 
-* a rolling_rank function 
+* Rolling_rank expression
 
-* A if-then expression.
+* If-Then expression.
 
+* Calculate return of future using strategy signal
 
 
 ### rolling_rank
 
 ```python
 import polars as pl
 import polars_qt as pq
@@ -72,7 +63,14 @@
 │ 5   │
 │ 4   │
 │ 4   │
 └─────┘
 ```
 
 
+
+适用于金融量化领域的polars表达式扩展，使用polars plugin实现。
+
+目前支持：
+* 滚动排序
+* if_then表达式
+* 利用策略信号回测收益
```

