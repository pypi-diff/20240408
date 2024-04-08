# Comparing `tmp/invrs_opt-0.5.0.tar.gz` & `tmp/invrs_opt-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invrs_opt-0.5.0.tar", last modified: Fri Mar 29 20:12:21 2024, max compression
+gzip compressed data, was "invrs_opt-0.5.1.tar", last modified: Mon Apr  8 14:16:13 2024, max compression
```

## Comparing `invrs_opt-0.5.0.tar` & `invrs_opt-0.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:12:21.392063 invrs_opt-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-29 20:12:21.392063 invrs_opt-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 20:12:21.392063 invrs_opt-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:12:21.388063 invrs_opt-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:12:21.388063 invrs_opt-0.5.0/src/invrs_opt/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/src/invrs_opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/src/invrs_opt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:12:21.388063 invrs_opt-0.5.0/src/invrs_opt/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/src/invrs_opt/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/src/invrs_opt/experimental/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/src/invrs_opt/experimental/labels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:12:21.388063 invrs_opt-0.5.0/src/invrs_opt/lbfgsb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/src/invrs_opt/lbfgsb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27896 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/src/invrs_opt/lbfgsb/lbfgsb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/src/invrs_opt/lbfgsb/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/src/invrs_opt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:12:21.392063 invrs_opt-0.5.0/src/invrs_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-29 20:12:21.000000 invrs_opt-0.5.0/src/invrs_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-29 20:12:21.000000 invrs_opt-0.5.0/src/invrs_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 20:12:21.000000 invrs_opt-0.5.0/src/invrs_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-29 20:12:21.000000 invrs_opt-0.5.0/src/invrs_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-29 20:12:21.000000 invrs_opt-0.5.0/src/invrs_opt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:12:21.388063 invrs_opt-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-03-29 20:12:07.000000 invrs_opt-0.5.0/tests/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.868456 invrs_opt-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.868456 invrs_opt-0.5.1/src/invrs_opt/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/src/invrs_opt/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/experimental/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/experimental/labels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/src/invrs_opt/lbfgsb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/lbfgsb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27892 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/lbfgsb/lbfgsb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/lbfgsb/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/src/invrs_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 14:16:13.000000 invrs_opt-0.5.1/src/invrs_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-08 14:16:13.000000 invrs_opt-0.5.1/src/invrs_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:16:13.000000 invrs_opt-0.5.1/src/invrs_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 14:16:13.000000 invrs_opt-0.5.1/src/invrs_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 14:16:13.000000 invrs_opt-0.5.1/src/invrs_opt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/tests/test_algos.py
```

### Comparing `invrs_opt-0.5.0/LICENSE` & `invrs_opt-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.0/PKG-INFO` & `invrs_opt-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invrs_opt
-Version: 0.5.0
+Version: 0.5.1
 Summary: Algorithms for inverse design
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 The INVRS-IO authors.
         
@@ -45,15 +45,15 @@
 Provides-Extra: dev
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # invrs-opt - Optimization algorithms for inverse design
-`v0.5.0`
+`v0.5.1`
 
 ## Overview
 
 The `invrs-opt` package defines an optimizer API intended for topology optimization, inverse design, or AI-guided design. It (currently) implements the L-BFGS-B optimization algorithm along with some variants. The API is intended to be general so that new algorithms can be accommodated, and is inspired by the functional optimizer approach used in jax. Example usage is as follows:
 
 ```python
 initial_params = ...
```

### Comparing `invrs_opt-0.5.0/README.md` & `invrs_opt-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # invrs-opt - Optimization algorithms for inverse design
-`v0.5.0`
+`v0.5.1`
 
 ## Overview
 
 The `invrs-opt` package defines an optimizer API intended for topology optimization, inverse design, or AI-guided design. It (currently) implements the L-BFGS-B optimization algorithm along with some variants. The API is intended to be general so that new algorithms can be accommodated, and is inspired by the functional optimizer approach used in jax. Example usage is as follows:
 
 ```python
 initial_params = ...
```

### Comparing `invrs_opt-0.5.0/pyproject.toml` & `invrs_opt-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "invrs_opt"
-version = "v0.5.0"
+version = "v0.5.1"
 description = "Algorithms for inverse design"
 keywords = ["topology", "optimization", "jax", "inverse design"]
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 
 authors = [
```

### Comparing `invrs_opt-0.5.0/src/invrs_opt/base.py` & `invrs_opt-0.5.1/src/invrs_opt/base.py`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.0/src/invrs_opt/experimental/client.py` & `invrs_opt-0.5.1/src/invrs_opt/experimental/client.py`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.0/src/invrs_opt/experimental/labels.py` & `invrs_opt-0.5.1/src/invrs_opt/experimental/labels.py`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.0/src/invrs_opt/lbfgsb/lbfgsb.py` & `invrs_opt-0.5.1/src/invrs_opt/lbfgsb/lbfgsb.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,16 +284,16 @@
             flat_latent_grad: PyTree,
             value: jnp.ndarray,
             jax_lbfgsb_state: JaxLbfgsbDict,
         ) -> Tuple[PyTree, JaxLbfgsbDict]:
             assert onp.size(value) == 1
             scipy_lbfgsb_state = ScipyLbfgsbState.from_jax(jax_lbfgsb_state)
             scipy_lbfgsb_state.update(
-                grad=onp.asarray(flat_latent_grad, dtype=onp.float64),
-                value=onp.asarray(value, dtype=onp.float64),
+                grad=onp.array(flat_latent_grad, dtype=onp.float64),
+                value=onp.array(value, dtype=onp.float64),
             )
             flat_latent_params = jnp.asarray(scipy_lbfgsb_state.x)
             return flat_latent_params, scipy_lbfgsb_state.to_jax()
 
         _, latent_params, jax_lbfgsb_state = state
         _, vjp_fn = jax.vjp(transform_fn, latent_params)
         (latent_grad,) = vjp_fn(grad)
```

### Comparing `invrs_opt-0.5.0/src/invrs_opt/lbfgsb/transform.py` & `invrs_opt-0.5.1/src/invrs_opt/lbfgsb/transform.py`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.0/src/invrs_opt.egg-info/PKG-INFO` & `invrs_opt-0.5.1/src/invrs_opt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invrs_opt
-Version: 0.5.0
+Version: 0.5.1
 Summary: Algorithms for inverse design
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 The INVRS-IO authors.
         
@@ -45,15 +45,15 @@
 Provides-Extra: dev
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # invrs-opt - Optimization algorithms for inverse design
-`v0.5.0`
+`v0.5.1`
 
 ## Overview
 
 The `invrs-opt` package defines an optimizer API intended for topology optimization, inverse design, or AI-guided design. It (currently) implements the L-BFGS-B optimization algorithm along with some variants. The API is intended to be general so that new algorithms can be accommodated, and is inspired by the functional optimizer approach used in jax. Example usage is as follows:
 
 ```python
 initial_params = ...
```

### Comparing `invrs_opt-0.5.0/src/invrs_opt.egg-info/SOURCES.txt` & `invrs_opt-0.5.1/src/invrs_opt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.0/tests/test_algos.py` & `invrs_opt-0.5.1/tests/test_algos.py`

 * *Files identical despite different names*

