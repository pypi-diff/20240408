# Comparing `tmp/types-qrcode-7.4.0.20240106.tar.gz` & `tmp/types-qrcode-7.4.0.20240408.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-qrcode-7.4.0.20240106.tar", last modified: Sat Jan  6 02:21:49 2024, max compression
+gzip compressed data, was "types-qrcode-7.4.0.20240408.tar", last modified: Mon Apr  8 02:17:07 2024, max compression
```

## Comparing `types-qrcode-7.4.0.20240106.tar` & `types-qrcode-7.4.0.20240408.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:21:49.747838 types-qrcode-7.4.0.20240106/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-01-06 02:21:49.000000 types-qrcode-7.4.0.20240106/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-06 02:21:49.000000 types-qrcode-7.4.0.20240106/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-06 02:21:49.747838 types-qrcode-7.4.0.20240106/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:21:49.743838 types-qrcode-7.4.0.20240106/qrcode-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/LUT.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-06 02:21:49.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/console_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:21:49.743838 types-qrcode-7.4.0.20240106/qrcode-stubs/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/pil.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/pure.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/styledpil.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:21:49.743838 types-qrcode-7.4.0.20240106/qrcode-stubs/image/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/styles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/styles/colormasks.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:21:49.743838 types-qrcode-7.4.0.20240106/qrcode-stubs/image/styles/moduledrawers/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/styles/moduledrawers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/styles/moduledrawers/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/styles/moduledrawers/pil.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/styles/moduledrawers/svg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/image/svg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/release.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-01-06 02:18:46.000000 types-qrcode-7.4.0.20240106/qrcode-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 02:21:49.747838 types-qrcode-7.4.0.20240106/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-01-06 02:21:49.000000 types-qrcode-7.4.0.20240106/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:21:49.747838 types-qrcode-7.4.0.20240106/types_qrcode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-06 02:21:49.000000 types-qrcode-7.4.0.20240106/types_qrcode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-06 02:21:49.000000 types-qrcode-7.4.0.20240106/types_qrcode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 02:21:49.000000 types-qrcode-7.4.0.20240106/types_qrcode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-06 02:21:49.000000 types-qrcode-7.4.0.20240106/types_qrcode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:17:07.806906 types-qrcode-7.4.0.20240408/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-08 02:17:07.000000 types-qrcode-7.4.0.20240408/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 02:17:07.000000 types-qrcode-7.4.0.20240408/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-08 02:17:07.806906 types-qrcode-7.4.0.20240408/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:17:07.802906 types-qrcode-7.4.0.20240408/qrcode-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/LUT.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 02:17:07.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/console_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:17:07.806906 types-qrcode-7.4.0.20240408/qrcode-stubs/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/pil.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/pure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/styledpil.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:17:07.806906 types-qrcode-7.4.0.20240408/qrcode-stubs/image/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/styles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/styles/colormasks.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:17:07.806906 types-qrcode-7.4.0.20240408/qrcode-stubs/image/styles/moduledrawers/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/styles/moduledrawers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/styles/moduledrawers/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/styles/moduledrawers/pil.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/styles/moduledrawers/svg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/image/svg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:17:07.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/release.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-08 02:16:43.000000 types-qrcode-7.4.0.20240408/qrcode-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 02:17:07.806906 types-qrcode-7.4.0.20240408/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-08 02:17:07.000000 types-qrcode-7.4.0.20240408/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:17:07.806906 types-qrcode-7.4.0.20240408/types_qrcode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-08 02:17:07.000000 types-qrcode-7.4.0.20240408/types_qrcode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-08 02:17:07.000000 types-qrcode-7.4.0.20240408/types_qrcode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 02:17:07.000000 types-qrcode-7.4.0.20240408/types_qrcode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 02:17:07.000000 types-qrcode-7.4.0.20240408/types_qrcode.egg-info/top_level.txt
```

### Comparing `types-qrcode-7.4.0.20240106/PKG-INFO` & `types-qrcode-7.4.0.20240408/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-qrcode
-Version: 7.4.0.20240106
+Version: 7.4.0.20240408
 Summary: Typing stubs for qrcode
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/qrcode.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-qrcode` aims to provide accurate annotations
 for `qrcode==7.4.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/qrcode. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `1d33abb91749cfa070fbc1482f186ff6b2ecbbbb` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
```

### Comparing `types-qrcode-7.4.0.20240106/qrcode-stubs/base.pyi` & `types-qrcode-7.4.0.20240408/qrcode-stubs/base.pyi`

 * *Files identical despite different names*

### Comparing `types-qrcode-7.4.0.20240106/qrcode-stubs/image/base.pyi` & `types-qrcode-7.4.0.20240408/qrcode-stubs/image/base.pyi`

 * *Files identical despite different names*

### Comparing `types-qrcode-7.4.0.20240106/qrcode-stubs/image/pure.pyi` & `types-qrcode-7.4.0.20240408/qrcode-stubs/image/pure.pyi`

 * *Files identical despite different names*

### Comparing `types-qrcode-7.4.0.20240106/qrcode-stubs/image/styledpil.pyi` & `types-qrcode-7.4.0.20240408/qrcode-stubs/image/styledpil.pyi`

 * *Files identical despite different names*

### Comparing `types-qrcode-7.4.0.20240106/qrcode-stubs/image/styles/colormasks.pyi` & `types-qrcode-7.4.0.20240408/qrcode-stubs/image/styles/colormasks.pyi`

 * *Files identical despite different names*

### Comparing `types-qrcode-7.4.0.20240106/qrcode-stubs/image/styles/moduledrawers/pil.pyi` & `types-qrcode-7.4.0.20240408/qrcode-stubs/image/styles/moduledrawers/pil.pyi`

 * *Files identical despite different names*

### Comparing `types-qrcode-7.4.0.20240106/qrcode-stubs/image/styles/moduledrawers/svg.pyi` & `types-qrcode-7.4.0.20240408/qrcode-stubs/image/styles/moduledrawers/svg.pyi`

 * *Files identical despite different names*

### Comparing `types-qrcode-7.4.0.20240106/qrcode-stubs/image/svg.pyi` & `types-qrcode-7.4.0.20240408/qrcode-stubs/image/svg.pyi`

 * *Files identical despite different names*

### Comparing `types-qrcode-7.4.0.20240106/qrcode-stubs/util.pyi` & `types-qrcode-7.4.0.20240408/qrcode-stubs/util.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from _typeshed import Incomplete
-from collections.abc import Generator
+from collections.abc import Callable, Generator
+from typing import Final, Literal, overload
+from typing_extensions import TypeAlias
 
 from qrcode.base import RSBlock as RSBlock
 
-MODE_NUMBER: Incomplete
-MODE_ALPHA_NUM: Incomplete
-MODE_8BIT_BYTE: Incomplete
-MODE_KANJI: Incomplete
+_MaskPattern: TypeAlias = Literal[0, 1, 2, 3, 4, 5, 6, 7]
+
+MODE_NUMBER: Final = 1
+MODE_ALPHA_NUM: Final = 2
+MODE_8BIT_BYTE: Final = 4
+MODE_KANJI: Final = 8
+
 MODE_SIZE_SMALL: Incomplete
 MODE_SIZE_MEDIUM: Incomplete
 MODE_SIZE_LARGE: Incomplete
+
 ALPHA_NUM: bytes
 RE_ALPHA_NUM: Incomplete
 NUMBER_LENGTH: Incomplete
 PATTERN_POSITION_TABLE: Incomplete
 G15: Incomplete
 G18: Incomplete
 G15_MASK: Incomplete
@@ -21,29 +27,34 @@
 PAD1: int
 BIT_LIMIT_TABLE: Incomplete
 
 def BCH_type_info(data): ...
 def BCH_type_number(data): ...
 def BCH_digit(data): ...
 def pattern_position(version): ...
-def mask_func(pattern): ...
+def mask_func(pattern: _MaskPattern) -> Callable[[int, int], bool]: ...
 def mode_sizes_for_version(version): ...
 def length_in_bits(mode, version): ...
 def check_version(version) -> None: ...
 def lost_point(modules): ...
-def optimal_data_chunks(data, minimum: int = 4) -> Generator[Incomplete, None, None]: ...
-def to_bytestring(data): ...
-def optimal_mode(data): ...
+def optimal_data_chunks(data: str | bytes, minimum: int = 4) -> Generator[QRData, None, None]: ...
+def to_bytestring(data: str | bytes) -> bytes: ...
+def optimal_mode(data) -> Literal[1, 2, 4]: ...
 
 class QRData:
-    mode: Incomplete
-    data: Incomplete
-    def __init__(self, data, mode: Incomplete | None = None, check_data: bool = True) -> None: ...
+    mode: Literal[1, 2, 4]
+    data: bytes
+    @overload
+    def __init__(self, data: bytes | str, mode: Literal[1, 2, 4] | None = None, check_data: Literal[True] = True) -> None: ...
+    @overload
+    def __init__(self, data: bytes, mode: Literal[1, 2, 4] | None = None, *, check_data: Literal[False]) -> None: ...
+    @overload
+    def __init__(self, data: bytes, mode: Literal[1, 2, 4] | None, check_data: Literal[False]) -> None: ...
     def __len__(self) -> int: ...
-    def write(self, buffer) -> None: ...
+    def write(self, buffer: BitBuffer) -> None: ...
 
 class BitBuffer:
     buffer: Incomplete
     length: int
     def __init__(self) -> None: ...
     def get(self, index): ...
     def put(self, num, length) -> None: ...
```

### Comparing `types-qrcode-7.4.0.20240106/setup.py` & `types-qrcode-7.4.0.20240408/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-qrcode` aims to provide accurate annotations
 for `qrcode==7.4.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/qrcode. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `1d33abb91749cfa070fbc1482f186ff6b2ecbbbb` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="7.4.0.20240106",
+      version="7.4.0.20240408",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/qrcode.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['qrcode-stubs'],
-      package_data={'qrcode-stubs': ['LUT.pyi', '__init__.pyi', 'base.pyi', 'console_scripts.pyi', 'constants.pyi', 'exceptions.pyi', 'image/__init__.pyi', 'image/base.pyi', 'image/pil.pyi', 'image/pure.pyi', 'image/styledpil.pyi', 'image/styles/__init__.pyi', 'image/styles/colormasks.pyi', 'image/styles/moduledrawers/__init__.pyi', 'image/styles/moduledrawers/base.pyi', 'image/styles/moduledrawers/pil.pyi', 'image/styles/moduledrawers/svg.pyi', 'image/svg.pyi', 'main.pyi', 'release.pyi', 'util.pyi', 'METADATA.toml']},
+      package_data={'qrcode-stubs': ['LUT.pyi', '__init__.pyi', 'base.pyi', 'console_scripts.pyi', 'constants.pyi', 'exceptions.pyi', 'image/__init__.pyi', 'image/base.pyi', 'image/pil.pyi', 'image/pure.pyi', 'image/styledpil.pyi', 'image/styles/__init__.pyi', 'image/styles/colormasks.pyi', 'image/styles/moduledrawers/__init__.pyi', 'image/styles/moduledrawers/base.pyi', 'image/styles/moduledrawers/pil.pyi', 'image/styles/moduledrawers/svg.pyi', 'image/svg.pyi', 'main.pyi', 'release.pyi', 'util.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-qrcode-7.4.0.20240106/types_qrcode.egg-info/PKG-INFO` & `types-qrcode-7.4.0.20240408/types_qrcode.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-qrcode
-Version: 7.4.0.20240106
+Version: 7.4.0.20240408
 Summary: Typing stubs for qrcode
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/qrcode.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-qrcode` aims to provide accurate annotations
 for `qrcode==7.4.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/qrcode. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `1d33abb91749cfa070fbc1482f186ff6b2ecbbbb` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
```

### Comparing `types-qrcode-7.4.0.20240106/types_qrcode.egg-info/SOURCES.txt` & `types-qrcode-7.4.0.20240408/types_qrcode.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 qrcode-stubs/METADATA.toml
 qrcode-stubs/__init__.pyi
 qrcode-stubs/base.pyi
 qrcode-stubs/console_scripts.pyi
 qrcode-stubs/constants.pyi
 qrcode-stubs/exceptions.pyi
 qrcode-stubs/main.pyi
+qrcode-stubs/py.typed
 qrcode-stubs/release.pyi
 qrcode-stubs/util.pyi
 qrcode-stubs/image/__init__.pyi
 qrcode-stubs/image/base.pyi
 qrcode-stubs/image/pil.pyi
 qrcode-stubs/image/pure.pyi
 qrcode-stubs/image/styledpil.pyi
```

