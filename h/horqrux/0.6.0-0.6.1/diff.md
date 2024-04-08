# Comparing `tmp/horqrux-0.6.0.tar.gz` & `tmp/horqrux-0.6.1.tar.gz`

## Comparing `horqrux-0.6.0.tar` & `horqrux-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 horqrux-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 horqrux-0.6.0/README.md
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 horqrux-0.6.0/mkdocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 horqrux-0.6.0/setup.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 horqrux-0.6.0/.github/workflows/run-tests-and-mypy.yml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 horqrux-0.6.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 horqrux-0.6.0/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0     6458 2020-02-02 00:00:00.000000 horqrux-0.6.0/docs/index.md
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 horqrux-0.6.0/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 horqrux-0.6.0/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 horqrux-0.6.0/horqrux/__init__.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 horqrux-0.6.0/horqrux/abstract.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 horqrux-0.6.0/horqrux/adjoint.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 horqrux-0.6.0/horqrux/analog.py
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 horqrux-0.6.0/horqrux/apply.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 horqrux-0.6.0/horqrux/matrices.py
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 horqrux-0.6.0/horqrux/parametric.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 horqrux-0.6.0/horqrux/primitive.py
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 horqrux-0.6.0/horqrux/utils.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 horqrux-0.6.0/tests/test_adjoint.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 horqrux-0.6.0/tests/test_analog.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 horqrux-0.6.0/tests/test_gates.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 horqrux-0.6.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 horqrux-0.6.0/LICENSE
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 horqrux-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 horqrux-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 horqrux-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 horqrux-0.6.1/README.md
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 horqrux-0.6.1/mkdocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 horqrux-0.6.1/setup.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 horqrux-0.6.1/.github/workflows/run-tests-and-mypy.yml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 horqrux-0.6.1/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 horqrux-0.6.1/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0    13456 2020-02-02 00:00:00.000000 horqrux-0.6.1/docs/index.md
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 horqrux-0.6.1/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 horqrux-0.6.1/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/adjoint.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/analog.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/apply.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/matrices.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/parametric.py
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/primitive.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/utils.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 horqrux-0.6.1/tests/test_adjoint.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 horqrux-0.6.1/tests/test_analog.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 horqrux-0.6.1/tests/test_gates.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 horqrux-0.6.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 horqrux-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 horqrux-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 horqrux-0.6.1/PKG-INFO
```

### Comparing `horqrux-0.6.0/.pre-commit-config.yaml` & `horqrux-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/mkdocs.yml` & `horqrux-0.6.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/.github/workflows/run-tests-and-mypy.yml` & `horqrux-0.6.1/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/docs/CODE_OF_CONDUCT.md` & `horqrux-0.6.1/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/docs/CONTRIBUTING.md` & `horqrux-0.6.1/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/horqrux/abstract.py` & `horqrux-0.6.1/horqrux/parametric.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,30 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Any, Iterable, Tuple
 
-import numpy as np
+import jax.numpy as jnp
 from jax import Array
 from jax.tree_util import register_pytree_node_class
 
 from .matrices import OPERATIONS_DICT
+from .primitive import Primitive
 from .utils import (
     ControlQubits,
     QubitSupport,
     TargetQubits,
-    _dagger,
     _jacobian,
     _unitary,
     is_controlled,
-    none_like,
 )
 
 
 @register_pytree_node_class
 @dataclass
-class Primitive:
-    """Primitive gate class which stores information about generators target and control qubits
-    of a particular quantum operator."""
-
-    generator_name: str
-    target: QubitSupport
-    control: QubitSupport
-
-    @staticmethod
-    def parse_idx(
-        idx: Tuple,
-    ) -> Tuple:
-        if isinstance(idx, (int, np.int64)):
-            return ((idx,),)
-        elif isinstance(idx, tuple):
-            return (idx,)
-        else:
-            return (idx.astype(int),)
-
-    def __post_init__(self) -> None:
-        self.target = Primitive.parse_idx(self.target)
-        if self.control is None:
-            self.control = none_like(self.target)
-        else:
-            self.control = Primitive.parse_idx(self.control)
-
-    def __iter__(self) -> Iterable:
-        return iter((self.generator_name, self.target, self.control))
-
-    def tree_flatten(self) -> Tuple[Tuple, Tuple[str, TargetQubits, ControlQubits]]:
-        children = ()
-        aux_data = (self.generator_name, self.target[0], self.control[0])
-        return (children, aux_data)
-
-    @classmethod
-    def tree_unflatten(cls, aux_data: Any, children: Any) -> Any:
-        return cls(*children, *aux_data)
-
-    def unitary(self, values: dict[str, float] = dict()) -> Array:
-        return OPERATIONS_DICT[self.generator_name]
-
-    def dagger(self, values: dict[str, float] = dict()) -> Array:
-        return _dagger(self.unitary(values))
-
-    @property
-    def name(self) -> str:
-        return "C" + self.generator_name if is_controlled(self.control) else self.generator_name
-
-    def __repr__(self) -> str:
-        return self.name + f"(target={self.target[0]}, control={self.control[0]})"
-
-
-@register_pytree_node_class
-@dataclass
 class Parametric(Primitive):
     """Extension of the Primitive class adding the option to pass a parameter."""
 
     generator_name: str
     target: QubitSupport
     control: QubitSupport
     param: str | float = ""
@@ -123,7 +68,81 @@
         base_name = "R" + self.generator_name
         return "C" + base_name if is_controlled(self.control) else base_name
 
     def __repr__(self) -> str:
         return (
             self.name + f"(target={self.target[0]}, control={self.control[0]}, param={self.param})"
         )
+
+
+def RX(param: float | str, target: TargetQubits, control: ControlQubits = (None,)) -> Parametric:
+    """RX gate.
+
+    Arguments:
+        param: Parameter denoting the Rotational angle.
+        target: Tuple of target qubits denoted as ints.
+        control: Optional tuple of control qubits denoted as ints.
+
+    Returns:
+        Parametric: A Parametric gate object.
+    """
+    return Parametric("X", target, control, param)
+
+
+def RY(param: float | str, target: TargetQubits, control: ControlQubits = (None,)) -> Parametric:
+    """RY gate.
+
+    Arguments:
+        param: Parameter denoting the Rotational angle.
+        target: Tuple of target qubits denoted as ints.
+        control: Optional tuple of control qubits denoted as ints.
+
+    Returns:
+        Parametric: A Parametric gate object.
+    """
+    return Parametric("Y", target, control, param)
+
+
+def RZ(param: float | str, target: TargetQubits, control: ControlQubits = (None,)) -> Parametric:
+    """RZ gate.
+
+    Arguments:
+        param: Parameter denoting the Rotational angle.
+        target: Tuple of target qubits denoted as ints.
+        control: Optional tuple of control qubits denoted as ints.
+
+    Returns:
+        Parametric: A Parametric gate object.
+    """
+    return Parametric("Z", target, control, param)
+
+
+class _PHASE(Parametric):
+    def unitary(self, values: dict[str, float] = dict()) -> Array:
+        u = jnp.eye(2, 2, dtype=jnp.complex128)
+        u = u.at[(1, 1)].set(jnp.exp(1.0j * self.parse_values(values)))
+        return u
+
+    def jacobian(self, values: dict[str, float] = dict()) -> Array:
+        jac = jnp.zeros((2, 2), dtype=jnp.complex128)
+        jac = jac.at[(1, 1)].set(1j * jnp.exp(1.0j * self.parse_values(values)))
+        return jac
+
+    @property
+    def name(self) -> str:
+        base_name = "PHASE"
+        return "C" + base_name if is_controlled(self.control) else base_name
+
+
+def PHASE(param: float, target: TargetQubits, control: ControlQubits = (None,)) -> Parametric:
+    """Phase gate.
+
+    Arguments:
+        param: Parameter denoting the Rotational angle.
+        target: Tuple of target qubits denoted as ints.
+        control: Optional tuple of control qubits denoted as ints.
+
+    Returns:
+        Parametric: A Parametric gate object.
+    """
+
+    return _PHASE("I", target, control, param)
```

### Comparing `horqrux-0.6.0/horqrux/adjoint.py` & `horqrux-0.6.1/horqrux/adjoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 from typing import Tuple
 
 from jax import Array, custom_vjp
 from jax.numpy import real as jnpreal
 
-from horqrux.abstract import Parametric, Primitive
 from horqrux.apply import apply_gate
+from horqrux.parametric import Parametric
+from horqrux.primitive import Primitive
 from horqrux.utils import OperationType, inner
 
 
 def expectation(
     state: Array, gates: list[Primitive], observable: list[Primitive], values: dict[str, float]
 ) -> Array:
     out_state = apply_gate(state, gates, values, OperationType.UNITARY)
```

### Comparing `horqrux-0.6.0/horqrux/analog.py` & `horqrux-0.6.1/horqrux/analog.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dataclasses import dataclass
 
 from jax import Array
 from jax.scipy.linalg import expm
 from jax.tree_util import register_pytree_node_class
 
-from .abstract import Primitive, QubitSupport
+from .primitive import Primitive, QubitSupport
 
 
 @register_pytree_node_class
 @dataclass
 class _HamiltonianEvolution(Primitive):
     """
     A slim wrapper class which evolves a 'hamiltonian'
```

### Comparing `horqrux-0.6.0/horqrux/apply.py` & `horqrux-0.6.1/horqrux/apply.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from operator import add
 from typing import Iterable, Tuple
 
 import jax.numpy as jnp
 import numpy as np
 from jax import Array
 
-from horqrux.abstract import Primitive
+from horqrux.primitive import Primitive
 
 from .utils import OperationType, State, _controlled, is_controlled
 
 
 def apply_operator(
     state: State,
     operator: Array,
```

### Comparing `horqrux-0.6.0/horqrux/matrices.py` & `horqrux-0.6.1/horqrux/matrices.py`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/horqrux/utils.py` & `horqrux-0.6.1/horqrux/utils.py`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/tests/test_adjoint.py` & `horqrux-0.6.1/tests/test_adjoint.py`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/tests/test_analog.py` & `horqrux-0.6.1/tests/test_analog.py`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/tests/test_gates.py` & `horqrux-0.6.1/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/.gitignore` & `horqrux-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/LICENSE` & `horqrux-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.0/pyproject.toml` & `horqrux-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 authors = [
     { name = "Gert-Jan Both" , email = "gert-jan.both@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
 ]
 requires-python = ">=3.8,<3.13"
 license = {text = "Apache 2.0"}
 
-version = "0.6.0"
+version = "0.6.1"
 
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `horqrux-0.6.0/PKG-INFO` & `horqrux-0.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: horqrux
-Version: 0.6.0
+Version: 0.6.1
 Summary: Jax-based quantum state vector simulator.
 Author-email: Gert-Jan Both <gert-jan.both@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>
 License: Apache 2.0
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

