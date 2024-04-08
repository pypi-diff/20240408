# Comparing `tmp/foamlib-0.2.4.tar.gz` & `tmp/foamlib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.2.4.tar", last modified: Wed Apr  3 13:00:57 2024, max compression
+gzip compressed data, was "foamlib-0.2.5.tar", last modified: Mon Apr  8 19:15:25 2024, max compression
```

## Comparing `foamlib-0.2.4.tar` & `foamlib-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:57.459715 foamlib-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-03 13:00:50.000000 foamlib-0.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-03 13:00:57.459715 foamlib-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-03 13:00:50.000000 foamlib-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:57.455715 foamlib-0.2.4/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:57.459715 foamlib-0.2.4/foamlib/_dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_dictionaries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_dictionaries/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_dictionaries/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_dictionaries/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:50.000000 foamlib-0.2.4/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:57.459715 foamlib-0.2.4/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-03 13:00:57.000000 foamlib-0.2.4/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-03 13:00:57.000000 foamlib-0.2.4/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:00:57.000000 foamlib-0.2.4/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-03 13:00:57.000000 foamlib-0.2.4/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 13:00:57.000000 foamlib-0.2.4/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-03 13:00:50.000000 foamlib-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:00:57.459715 foamlib-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:00:57.459715 foamlib-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_flange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_flange_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_pitz.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-03 13:00:50.000000 foamlib-0.2.4/tests/test_pitz_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:25.248138 foamlib-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-08 19:15:15.000000 foamlib-0.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-08 19:15:25.248138 foamlib-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-08 19:15:15.000000 foamlib-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:25.244138 foamlib-0.2.5/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21422 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:25.244138 foamlib-0.2.5/foamlib/_dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_dictionaries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_dictionaries/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_dictionaries/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_dictionaries/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:25.248138 foamlib-0.2.5/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-08 19:15:25.000000 foamlib-0.2.5/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 19:15:25.000000 foamlib-0.2.5/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:15:25.000000 foamlib-0.2.5/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-08 19:15:25.000000 foamlib-0.2.5/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 19:15:25.000000 foamlib-0.2.5/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-08 19:15:15.000000 foamlib-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:15:25.248138 foamlib-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:25.248138 foamlib-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_flange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_flange_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_pitz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_pitz_async.py
```

### Comparing `foamlib-0.2.4/LICENSE.txt` & `foamlib-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.4/PKG-INFO` & `foamlib-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -23,23 +23,22 @@
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aioshutil<2,>=1
 Requires-Dist: pyparsing<4,>=3
-Requires-Dist: typing-extensions<5,>=4
+Requires-Dist: typing-extensions<5,>=4; python_version < "3.11"
 Provides-Extra: lint
-Requires-Dist: mypy<2,>=1; extra == "lint"
-Requires-Dist: pytest<9,>=7; extra == "lint"
-Requires-Dist: pytest-asyncio<0.24,>=0.21; extra == "lint"
-Requires-Dist: numpy<2,>=1; extra == "lint"
-Requires-Dist: black; extra == "lint"
-Requires-Dist: flake8; extra == "lint"
-Requires-Dist: Flake8-pyproject; extra == "lint"
+Requires-Dist: ruff; extra == "lint"
+Provides-Extra: typing
+Requires-Dist: mypy<2,>=1; extra == "typing"
+Requires-Dist: pytest<9,>=7; extra == "typing"
+Requires-Dist: pytest-asyncio<0.24,>=0.21; extra == "typing"
+Requires-Dist: numpy<2,>=1; extra == "typing"
 Provides-Extra: test
 Requires-Dist: pytest<9,>=7; extra == "test"
 Requires-Dist: pytest-asyncio<0.24,>=0.21; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: numpy<2,>=1; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx<8,>=7; extra == "docs"
@@ -48,15 +47,15 @@
 
 # foamlib
 
 [![Documentation](https://img.shields.io/readthedocs/foamlib)](https://foamlib.readthedocs.io/)
 [![CI](https://github.com/gerlero/foamlib/actions/workflows/ci.yml/badge.svg)](https://github.com/gerlero/foamlib/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/gerlero/foamlib/branch/main/graph/badge.svg)](https://codecov.io/gh/gerlero/foamlib)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/foamlib)](https://pypi.org/project/foamlib/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/foamlib)](https://pypi.org/project/foamlib/)
 [![Docker image](https://img.shields.io/badge/docker%20image-gerlero%2Ffoamlib-informational)](https://hub.docker.com/r/gerlero/foamlib/)
 
 **foamlib** provides a simple, modern and ergonomic Python interface for interacting with [OpenFOAM](https://www.openfoam.com).
 
 It offers the following classes (among a few others):
```

### Comparing `foamlib-0.2.4/README.md` & `foamlib-0.2.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # foamlib
 
 [![Documentation](https://img.shields.io/readthedocs/foamlib)](https://foamlib.readthedocs.io/)
 [![CI](https://github.com/gerlero/foamlib/actions/workflows/ci.yml/badge.svg)](https://github.com/gerlero/foamlib/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/gerlero/foamlib/branch/main/graph/badge.svg)](https://codecov.io/gh/gerlero/foamlib)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/foamlib)](https://pypi.org/project/foamlib/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/foamlib)](https://pypi.org/project/foamlib/)
 [![Docker image](https://img.shields.io/badge/docker%20image-gerlero%2Ffoamlib-informational)](https://hub.docker.com/r/gerlero/foamlib/)
 
 **foamlib** provides a simple, modern and ergonomic Python interface for interacting with [OpenFOAM](https://www.openfoam.com).
 
 It offers the following classes (among a few others):
```

### Comparing `foamlib-0.2.4/foamlib/_cases.py` & `foamlib-0.2.5/foamlib/_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,38 @@
+import sys
 import os
 import asyncio
 import multiprocessing
 import shutil
 
 from pathlib import Path
 from contextlib import asynccontextmanager
 from typing import (
     Optional,
     Union,
-    Collection,
-    Mapping,
-    Set,
-    Sequence,
-    AsyncGenerator,
-    Callable,
-    Iterator,
     overload,
 )
 
+if sys.version_info >= (3, 9):
+    from collections.abc import (
+        Collection,
+        Mapping,
+        Set,
+        Sequence,
+        AsyncGenerator,
+        Callable,
+        Iterator,
+    )
+else:
+    from typing import Collection, Mapping, Sequence, AsyncGenerator, Callable, Iterator
+    from typing import AbstractSet as Set
+
 import aioshutil
 
-from ._subprocesses import run_process, run_process_async, CalledProcessError
+from ._util import is_sequence, run_process, run_process_async, CalledProcessError
 from ._dictionaries import FoamFile, FoamFieldFile
 
 
 class FoamCaseBase(Sequence["FoamCaseBase.TimeDirectory"]):
     def __init__(self, path: Union[Path, str]):
         self.path = Path(path).absolute()
         if not self.path.is_dir():
@@ -128,15 +136,15 @@
     def __len__(self) -> int:
         return len(self._times)
 
     def _clean_paths(self) -> Set[Path]:
         has_decompose_par_dict = (self.path / "system" / "decomposeParDict").is_file()
         has_block_mesh_dict = (self.path / "system" / "blockMeshDict").is_file()
 
-        paths: Set[Path] = set()
+        paths = set()
 
         for p in self.path.iterdir():
             if p.is_dir():
                 try:
                     t = float(p.name)
                 except ValueError:
                     pass
@@ -211,15 +219,15 @@
         env = os.environ.copy()
         env["PWD"] = str(self.path)
         return env
 
     def _parallel_cmd(
         self, cmd: Union[Sequence[Union[str, Path]], str, Path]
     ) -> Union[Sequence[Union[str, Path]], str]:
-        if isinstance(cmd, str) or not isinstance(cmd, Sequence):
+        if not is_sequence(cmd):
             return f"mpiexec -np {self._nprocessors} {cmd} -parallel"
         else:
             return [
                 "mpiexec",
                 "-np",
                 str(self._nprocessors),
                 cmd[0],
```

### Comparing `foamlib-0.2.4/foamlib/_dictionaries/_base.py` & `foamlib-0.2.5/foamlib/_dictionaries/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+import sys
+
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import Dict, NamedTuple, Optional, Sequence, Union
+from typing import Dict, NamedTuple, Optional, Union
+
+if sys.version_info >= (3, 9):
+    from collections.abc import Sequence
+else:
+    from typing import Sequence
 
 
 class FoamDictionaryBase:
     class DimensionSet(NamedTuple):
         mass: Union[int, float] = 0
         length: Union[int, float] = 0
         time: Union[int, float] = 0
```

### Comparing `foamlib-0.2.4/foamlib/_dictionaries/_files.py` & `foamlib-0.2.5/foamlib/_dictionaries/_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,38 @@
+import sys
+
 from pathlib import Path
 from typing import (
     Any,
-    Iterator,
-    Mapping,
-    MutableMapping,
     Optional,
-    Sequence,
     Tuple,
     Union,
     cast,
 )
 
-from typing_extensions import Self
+if sys.version_info >= (3, 9):
+    from collections.abc import Iterator, Mapping, MutableMapping, Sequence
+else:
+    from typing import Iterator, Mapping, MutableMapping, Sequence
 
-from ._base import FoamDictionaryBase
-from ._parsing import Parsed, as_dict, get_entry_locn, get_value, parse
-from ._serialization import serialize_entry
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
 
 try:
     import numpy as np
     from numpy.typing import NDArray
 except ModuleNotFoundError:
     pass
 
+from ._base import FoamDictionaryBase
+from ._parsing import Parsed, as_dict, get_entry_locn, get_value, parse
+from ._serialization import serialize_entry
+
 
 class _FoamFileBase:
     def __init__(self, path: Union[str, Path]) -> None:
         self.path = Path(path).absolute()
         if self.path.is_dir():
             raise IsADirectoryError(self.path)
         elif not self.path.is_file():
```

### Comparing `foamlib-0.2.4/foamlib/_dictionaries/_parsing.py` & `foamlib-0.2.5/foamlib/_dictionaries/_parsing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-from typing import Mapping, MutableMapping, Optional, Sequence, Tuple
+import sys
+
+from typing import Optional, Tuple
+
+if sys.version_info >= (3, 9):
+    from collections.abc import Mapping, MutableMapping, Sequence
+else:
+    from typing import Mapping, MutableMapping, Sequence
 
 from pyparsing import (
     Dict,
     Forward,
     Group,
     Keyword,
     LineEnd,
@@ -159,15 +166,14 @@
 
 def as_dict(parsed: Parsed) -> FoamDictionaryBase._Dict:
     """
     Return a nested dict representation of the file.
     """
     ret: FoamDictionaryBase._Dict = {}
     for keywords, (_, value, _) in parsed.items():
-
         r = ret
         for k in keywords[:-1]:
             assert isinstance(r, dict)
             v = r[k]
             assert isinstance(v, dict)
             r = v
```

### Comparing `foamlib-0.2.4/foamlib/_dictionaries/_serialization.py` & `foamlib-0.2.5/foamlib/_dictionaries/_serialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,39 @@
-from contextlib import suppress
-from typing import Any, Mapping, Sequence
+import sys
 
-from ._base import FoamDictionaryBase
+from contextlib import suppress
+from typing import Any
 
-try:
-    import numpy as np
-except ModuleNotFoundError:
-    numpy = False
+if sys.version_info >= (3, 9):
+    from collections.abc import Mapping
 else:
-    numpy = True
+    from typing import Mapping
 
-
-def _is_sequence(value: Any) -> bool:
-    return (
-        isinstance(value, Sequence)
-        and not isinstance(value, str)
-        or numpy
-        and isinstance(value, np.ndarray)
-    )
+from ._base import FoamDictionaryBase
+from .._util import is_sequence
 
 
 def _serialize_bool(value: Any) -> str:
     if value is True:
         return "yes"
     elif value is False:
         return "no"
     else:
         raise TypeError(f"Not a bool: {type(value)}")
 
 
 def _serialize_list(value: Any) -> str:
-    if _is_sequence(value):
+    if is_sequence(value):
         return f"({' '.join(_serialize_value(v) for v in value)})"
     else:
         raise TypeError(f"Not a valid sequence: {type(value)}")
 
 
 def _serialize_field(value: Any) -> str:
-    if _is_sequence(value):
+    if is_sequence(value):
         try:
             s = _serialize_list(value)
         except TypeError:
             raise TypeError(f"Not a valid field: {type(value)}") from None
         else:
             if len(value) < 10:
                 return f"uniform {s}"
@@ -60,15 +52,15 @@
                     )
                 return f"nonuniform List<{kind}> {len(value)}{s}"
     else:
         return f"uniform {value}"
 
 
 def _serialize_dimensions(value: Any) -> str:
-    if _is_sequence(value) and len(value) == 7:
+    if is_sequence(value) and len(value) == 7:
         return f"[{' '.join(str(v) for v in value)}]"
     else:
         raise TypeError(f"Not a valid dimension set: {type(value)}")
 
 
 def _serialize_dimensioned(value: Any) -> str:
     if isinstance(value, FoamDictionaryBase.Dimensioned):
```

### Comparing `foamlib-0.2.4/foamlib.egg-info/PKG-INFO` & `foamlib-0.2.5/foamlib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -23,23 +23,22 @@
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aioshutil<2,>=1
 Requires-Dist: pyparsing<4,>=3
-Requires-Dist: typing-extensions<5,>=4
+Requires-Dist: typing-extensions<5,>=4; python_version < "3.11"
 Provides-Extra: lint
-Requires-Dist: mypy<2,>=1; extra == "lint"
-Requires-Dist: pytest<9,>=7; extra == "lint"
-Requires-Dist: pytest-asyncio<0.24,>=0.21; extra == "lint"
-Requires-Dist: numpy<2,>=1; extra == "lint"
-Requires-Dist: black; extra == "lint"
-Requires-Dist: flake8; extra == "lint"
-Requires-Dist: Flake8-pyproject; extra == "lint"
+Requires-Dist: ruff; extra == "lint"
+Provides-Extra: typing
+Requires-Dist: mypy<2,>=1; extra == "typing"
+Requires-Dist: pytest<9,>=7; extra == "typing"
+Requires-Dist: pytest-asyncio<0.24,>=0.21; extra == "typing"
+Requires-Dist: numpy<2,>=1; extra == "typing"
 Provides-Extra: test
 Requires-Dist: pytest<9,>=7; extra == "test"
 Requires-Dist: pytest-asyncio<0.24,>=0.21; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: numpy<2,>=1; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx<8,>=7; extra == "docs"
@@ -48,15 +47,15 @@
 
 # foamlib
 
 [![Documentation](https://img.shields.io/readthedocs/foamlib)](https://foamlib.readthedocs.io/)
 [![CI](https://github.com/gerlero/foamlib/actions/workflows/ci.yml/badge.svg)](https://github.com/gerlero/foamlib/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/gerlero/foamlib/branch/main/graph/badge.svg)](https://codecov.io/gh/gerlero/foamlib)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/foamlib)](https://pypi.org/project/foamlib/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/foamlib)](https://pypi.org/project/foamlib/)
 [![Docker image](https://img.shields.io/badge/docker%20image-gerlero%2Ffoamlib-informational)](https://hub.docker.com/r/gerlero/foamlib/)
 
 **foamlib** provides a simple, modern and ergonomic Python interface for interacting with [OpenFOAM](https://www.openfoam.com).
 
 It offers the following classes (among a few others):
```

### Comparing `foamlib-0.2.4/foamlib.egg-info/SOURCES.txt` & `foamlib-0.2.5/foamlib.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE.txt
 README.md
 pyproject.toml
 foamlib/__init__.py
 foamlib/_cases.py
-foamlib/_subprocesses.py
+foamlib/_util.py
 foamlib/py.typed
 foamlib.egg-info/PKG-INFO
 foamlib.egg-info/SOURCES.txt
 foamlib.egg-info/dependency_links.txt
 foamlib.egg-info/requires.txt
 foamlib.egg-info/top_level.txt
 foamlib/_dictionaries/__init__.py
```

### Comparing `foamlib-0.2.4/pyproject.toml` & `foamlib-0.2.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -26,28 +26,26 @@
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 
 dependencies = [
     "aioshutil>=1,<2",
     "pyparsing>=3,<4",
-    "typing-extensions>=4,<5",
+    "typing-extensions>=4,<5; python_version<'3.11'",
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
-lint = [
+lint = ["ruff"]
+typing = [
     "mypy>=1,<2",
     "pytest>=7,<9",
     "pytest-asyncio>=0.21,<0.24",
     "numpy>=1,<2",
-    "black",
-    "flake8",
-    "Flake8-pyproject",
 ]
 test = [
     "pytest>=7,<9",
     "pytest-asyncio>=0.21,<0.24",
     "pytest-cov",
     "numpy>=1,<2",
 ]
@@ -70,26 +68,7 @@
 
 [tool.mypy]
 packages = [
     "foamlib",
     "tests",
 ]
 strict = true
-
-[tool.flake8]
-count = true
-ignore = [
-    "E203",  # whitespace before ':'
-    "E501",  # line too long
-    "E704",  # multiple statements on one line (def)
-    "F403",  # 'from foamlib import *' used; unable to detect undefined names
-    "F405",  # 'FoamDimensionSet' may be undefined, or defined from star imports: foamlib
-    "W503",  # line break before binary operator
-]
-exclude = [
-    ".git",
-    "__pycache__",
-    "docs/source/conf.py",
-    "build",
-    "dist",
-    "venv",
-]
```

### Comparing `foamlib-0.2.4/tests/test_dictionaries.py` & `foamlib-0.2.5/tests/test_dictionaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from pathlib import Path
 from typing import Sequence
 
 import numpy as np
 
-from foamlib import *
+from foamlib import FoamCase, FoamFile, FoamFieldFile
 from foamlib._dictionaries._parsing import _VALUE
 
 
 def test_parse_value() -> None:
     assert _VALUE.parse_string("1")[0] == 1
     assert _VALUE.parse_string("1.0")[0] == 1.0
     assert _VALUE.parse_string("1.0e-3")[0] == 1.0e-3
```

### Comparing `foamlib-0.2.4/tests/test_flange.py` & `foamlib-0.2.5/tests/test_flange.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.4/tests/test_flange_async.py` & `foamlib-0.2.5/tests/test_flange_async.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.4/tests/test_pitz.py` & `foamlib-0.2.5/tests/test_pitz.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.4/tests/test_pitz_async.py` & `foamlib-0.2.5/tests/test_pitz_async.py`

 * *Files identical despite different names*

