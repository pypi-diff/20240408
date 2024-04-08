# Comparing `tmp/titanq-0.7.1.tar.gz` & `tmp/titanq-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanq-0.7.1.tar", last modified: Thu Apr  4 15:01:57 2024, max compression
+gzip compressed data, was "titanq-0.8.0.tar", last modified: Mon Apr  8 13:59:00 2024, max compression
```

## Comparing `titanq-0.7.1.tar` & `titanq-0.8.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-04 15:01:57.539907 titanq-0.7.1/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-04-01 13:41:38.000000 titanq-0.7.1/LICENSE.txt
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-04 15:01:57.539907 titanq-0.7.1/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     5011 2024-04-01 18:11:59.000000 titanq-0.7.1/README.md
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1243 2024-04-04 15:00:54.000000 titanq-0.7.1/pyproject.toml
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-04-01 13:41:38.000000 titanq-0.7.1/requirements.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-04 15:01:57.539907 titanq-0.7.1/setup.cfg
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-04 15:01:57.535907 titanq-0.7.1/tests/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     6756 2024-04-02 15:31:47.000000 titanq-0.7.1/tests/test_client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    23136 2024-04-04 15:00:54.000000 titanq-0.7.1/tests/test_model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2849 2024-04-02 15:31:47.000000 titanq-0.7.1/tests/test_numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      736 2024-04-01 18:11:59.000000 titanq-0.7.1/tests/test_optimize_response.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      427 2024-04-02 15:31:47.000000 titanq-0.7.1/tests/test_variable.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-04 15:01:57.535907 titanq-0.7.1/titanq/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-04-01 13:41:38.000000 titanq-0.7.1/titanq/__init__.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-04 15:01:57.539907 titanq-0.7.1/titanq/_client/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      127 2024-04-02 15:31:47.000000 titanq-0.7.1/titanq/_client/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-04-02 13:51:42.000000 titanq-0.7.1/titanq/_client/client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3844 2024-04-02 15:31:47.000000 titanq-0.7.1/titanq/_client/model.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-04 15:01:57.539907 titanq-0.7.1/titanq/_model/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-04-01 18:11:59.000000 titanq-0.7.1/titanq/_model/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     5162 2024-04-04 15:00:54.000000 titanq-0.7.1/titanq/_model/constraints.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      894 2024-04-02 15:31:47.000000 titanq-0.7.1/titanq/_model/errors.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1837 2024-04-02 15:31:47.000000 titanq-0.7.1/titanq/_model/manifest.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    27041 2024-04-02 15:31:47.000000 titanq-0.7.1/titanq/_model/model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2752 2024-04-02 15:31:47.000000 titanq-0.7.1/titanq/_model/numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1986 2024-04-01 13:41:38.000000 titanq-0.7.1/titanq/_model/objective.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3942 2024-04-01 13:41:38.000000 titanq-0.7.1/titanq/_model/optimize_response.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1541 2024-04-02 15:31:47.000000 titanq-0.7.1/titanq/_model/variable.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-04 15:01:57.539907 titanq-0.7.1/titanq/_storage/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-04-01 13:41:38.000000 titanq-0.7.1/titanq/_storage/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     4284 2024-04-04 15:00:54.000000 titanq-0.7.1/titanq/_storage/managed_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     6173 2024-04-02 15:31:47.000000 titanq-0.7.1/titanq/_storage/s3_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3919 2024-04-02 15:31:47.000000 titanq-0.7.1/titanq/_storage/storage_client.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-04 15:01:57.539907 titanq-0.7.1/titanq.egg-info/
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-04 15:01:57.000000 titanq-0.7.1/titanq.egg-info/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      789 2024-04-04 15:01:57.000000 titanq-0.7.1/titanq.egg-info/SOURCES.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-04 15:01:57.000000 titanq-0.7.1/titanq.egg-info/dependency_links.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-04 15:01:57.000000 titanq-0.7.1/titanq.egg-info/requires.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-04 15:01:57.000000 titanq-0.7.1/titanq.egg-info/top_level.txt
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.821948 titanq-0.8.0/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-04-01 13:41:38.000000 titanq-0.8.0/LICENSE.txt
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-08 13:59:00.821948 titanq-0.8.0/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5011 2024-04-01 18:11:59.000000 titanq-0.8.0/README.md
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1243 2024-04-08 13:21:32.000000 titanq-0.8.0/pyproject.toml
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-04-01 13:41:38.000000 titanq-0.8.0/requirements.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-08 13:59:00.821948 titanq-0.8.0/setup.cfg
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.817948 titanq-0.8.0/tests/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6756 2024-04-02 15:31:47.000000 titanq-0.8.0/tests/test_client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    25419 2024-04-08 13:39:25.000000 titanq-0.8.0/tests/test_model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2849 2024-04-02 15:31:47.000000 titanq-0.8.0/tests/test_numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1405 2024-04-05 13:48:53.000000 titanq-0.8.0/tests/test_optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      940 2024-04-05 13:48:53.000000 titanq-0.8.0/tests/test_variable.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.817948 titanq-0.8.0/titanq/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-04-01 13:41:38.000000 titanq-0.8.0/titanq/__init__.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.817948 titanq-0.8.0/titanq/_client/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      127 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_client/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-04-02 13:51:42.000000 titanq-0.8.0/titanq/_client/client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3844 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_client/model.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.817948 titanq-0.8.0/titanq/_model/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-04-01 18:11:59.000000 titanq-0.8.0/titanq/_model/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5393 2024-04-08 13:21:32.000000 titanq-0.8.0/titanq/_model/constraints.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      984 2024-04-05 13:48:53.000000 titanq-0.8.0/titanq/_model/errors.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1837 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_model/manifest.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    28359 2024-04-05 18:58:59.000000 titanq-0.8.0/titanq/_model/model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2752 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_model/numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1986 2024-04-01 13:41:38.000000 titanq-0.8.0/titanq/_model/objective.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     4721 2024-04-05 13:48:53.000000 titanq-0.8.0/titanq/_model/optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2766 2024-04-05 13:48:53.000000 titanq-0.8.0/titanq/_model/variable.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2645 2024-04-05 13:48:53.000000 titanq-0.8.0/titanq/_model/variable_list.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.821948 titanq-0.8.0/titanq/_storage/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-04-01 13:41:38.000000 titanq-0.8.0/titanq/_storage/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     4283 2024-04-05 13:48:53.000000 titanq-0.8.0/titanq/_storage/managed_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6173 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_storage/s3_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3919 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_storage/storage_client.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.821948 titanq-0.8.0/titanq.egg-info/
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-08 13:59:00.000000 titanq-0.8.0/titanq.egg-info/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      820 2024-04-08 13:59:00.000000 titanq-0.8.0/titanq.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-08 13:59:00.000000 titanq-0.8.0/titanq.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-08 13:59:00.000000 titanq-0.8.0/titanq.egg-info/requires.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-08 13:59:00.000000 titanq-0.8.0/titanq.egg-info/top_level.txt
```

### Comparing `titanq-0.7.1/LICENSE.txt` & `titanq-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/PKG-INFO` & `titanq-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.7.1
+Version: 0.8.0
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
```

### Comparing `titanq-0.7.1/README.md` & `titanq-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/pyproject.toml` & `titanq-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "titanq"
 description = "The TitanQ SDK for python"
 dynamic = ["dependencies"]
 readme = { file = "README.md", content-type = "text/markdown" }
-version = "0.7.1"
+version = "0.8.0"
 license = { text = "Apache 2.0" }
 keywords = ["titan", "titanq", "optimization", "platform", "infinity", "infinityq"]
 requires-python = ">= 3.9"
 maintainers = [
     { name = "InfinityQ", email = "support@infinityq.tech" }
 ]
 classifiers = [
```

### Comparing `titanq-0.7.1/tests/test_client.py` & `titanq-0.8.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/tests/test_model.py` & `titanq-0.8.0/tests/test_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,21 +99,14 @@
     if error:
         with pytest.raises(error):
             model_s3_client.add_variable_vector(name, size, vtype)
     else:
         model_s3_client.add_variable_vector(name, size, vtype)
 
 
-def test_multiple_variable(model_s3_client):
-    model_s3_client.add_variable_vector('x', 1, Vtype.BINARY)
-
-    with pytest.raises(errors.MaximumVariableLimitError):
-        model_s3_client.add_variable_vector('y', 2, Vtype.BINARY)
-
-
 @pytest.mark.parametrize("weights_shape, bias_shape, objective, error", [
     ((10, 10), (10,), Target.MINIMIZE, None),
     ((11, 10), (10,), Target.MINIMIZE, ValueError),
     ((10, 11), (10,), Target.MINIMIZE, ValueError),
     ((11, 11), (10,), Target.MINIMIZE, ValueError),
     ((10, 10, 10), (10,), Target.MINIMIZE, ValueError),
     ((10,), (10,), Target.MINIMIZE, ValueError),
@@ -261,15 +254,15 @@
             model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
     else:
         model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
 
 
 @pytest.mark.parametrize("vtype", [
     (Vtype.BINARY),
-    (Vtype.BIPOLAR)
+    (Vtype.BIPOLAR),
 ])
 def test_vtype_sent(model_s3_client, mock_titanq_client, vtype):
     model = model_s3_client
     mock_client = mock_titanq_client
 
     # optimize using sdk
     weights = np.random.rand(10, 10).astype(np.float32)
@@ -404,25 +397,50 @@
     np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[-3.45, -3.45]], dtype=np.float32))
 
     model_s3_client.add_equality_constraint(np.array([14, 0], dtype=np.float32), 0)
     np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1.05, -1.1], [14, 0]], dtype=np.float32))
     np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[-3.45, -3.45], [0, 0]], dtype=np.float32))
 
 
+@pytest.mark.parametrize("method, kwargs", [
+    ("add_set_partitioning_constraints_matrix", { "constraint_mask": np.array([[0,1]])}),
+    ("add_set_partitioning_constraint",         { "constraint_mask": np.array([0,1])}),
+    ("add_cardinality_constraints_matrix",      { "constraint_mask": np.array([[0,1]]),                   "cardinalities": np.array([1])}),
+    ("add_cardinality_constraint",              { "constraint_mask": np.array([0,1]),                     "cardinality": 1 }),
+    ("add_equality_constraints_matrix",         { "constraint_mask": np.array([[0,1]], dtype=np.float32), "limit": np.array([1], dtype=np.float32) }),
+    ("add_equality_constraint",                 { "constraint_mask": np.array([0,1], dtype=np.float32),   "limit": 1 }),
+    ("add_inequality_constraints_matrix",       { "constraint_mask": np.array([[0,1]], dtype=np.float32), "constraint_bounds": np.array([[-50, np.nan]], dtype=np.float32)}),
+    ("add_inequality_constraint",               { "constraint_mask": np.array([0,1], dtype=np.float32),   "constraint_bounds": np.array([-50, np.nan], dtype=np.float32)}),
+])
+def test_constraint_weights_and_bounds_float_32_output(model_s3_client, method, kwargs):
+    model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
+
+    constraint_function = getattr(model_s3_client, method)
+    constraint_function(**kwargs)
+
+    assert model_s3_client._constraints.bounds().dtype == np.float32
+
+
 def test_add_equality_constraint_matrix(model_s3_client):
     model_s3_client.add_variable_vector('x', 4, Vtype.BINARY)
 
     model_s3_client.add_equality_constraints_matrix(np.array([[-3.51, 0, 0, 0], [10, 0, 0, 0]], dtype=np.float32), np.array([2, 10], dtype=np.float32))
     np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[-3.51, 0, 0, 0], [10, 0, 0, 0]], dtype=np.float32))
     np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[2, 2], [10, 10]], dtype=np.float32))
 
     model_s3_client.add_equality_constraints_matrix(np.array([[0, 5, 0, 0], [0, 0, -5, 0]], dtype=np.float32), np.array([-1, 1], dtype=np.float32))
     np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[-3.51, 0, 0, 0], [10, 0, 0, 0], [0, 5, 0, 0], [0, 0, -5, 0]], dtype=np.float32))
     np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[2, 2], [10, 10], [-1, -1], [1, 1]], dtype=np.float32))
 
+    with pytest.raises(ValueError):
+        model_s3_client.add_equality_constraints_matrix(np.array([[1, 2, 3, 4]], dtype=np.float32), np.array([[10, 10]], dtype=np.float32))
+
+    with pytest.raises(ValueError):
+        model_s3_client.add_equality_constraints_matrix(np.array([[1, 2, 3, 4]], dtype=np.float32), np.array([10], dtype=np.int32))
+
 
 def test_equality_constraint_override_variable_types(model_s3_client, mock_titanq_client):
     weights = np.random.rand(2, 2).astype(np.float32)
     bias = np.random.rand(2).astype(np.float32)
 
     model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
     model_s3_client.set_objective_matrices(weights, bias)
@@ -440,22 +458,30 @@
     np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1.05, -1.1]], dtype=np.float32))
     np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[np.nan, -3.45]], dtype=np.float32))
 
     model_s3_client.add_inequality_constraint(np.array([14, 0], dtype=np.float32), np.array([-0.09, 0], dtype=np.float32))
     np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1.05, -1.1], [14, 0]], dtype=np.float32))
     np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[np.nan, -3.45], [-0.09, 0]], dtype=np.float32))
 
+    model_s3_client.add_inequality_constraint(np.array([76, -4.8], dtype=np.float32), np.array([None, -8], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[1.05, -1.1], [14, 0], [76, -4.8]], dtype=np.float32))
+    np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[np.nan, -3.45], [-0.09, 0], [None, -8]], dtype=np.float32))
 
 def test_add_inequality_constraint_matrix(model_s3_client):
     model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
     model_s3_client.add_inequality_constraints_matrix(np.array([[-3.51, 0], [10, 0]], dtype=np.float32), np.array([[8, 9], [np.nan, 100_000]], dtype=np.float32))
 
     np.testing.assert_equal(model_s3_client._constraints.weights(), np.array([[-3.51, 0], [10, 0]], dtype=np.float32))
     np.testing.assert_equal(model_s3_client._constraints.bounds(), np.array([[8, 9], [np.nan, 100_000]], dtype=np.float32))
 
+    with pytest.raises(ValueError):
+        model_s3_client.add_equality_constraints_matrix(np.array([[1, 2]], dtype=np.float32), np.array([[np.nan, 10]], dtype=np.float32))
+
+    with pytest.raises(ValueError):
+        model_s3_client.add_equality_constraints_matrix(np.array([[1, 2]], dtype=np.float32), np.array([np.nan, 10], dtype=np.int32))
 
 def test_inequality_constraint_override_variable_types(model_s3_client, mock_titanq_client):
     weights = np.random.rand(2, 2).astype(np.float32)
     bias = np.random.rand(2).astype(np.float32)
 
     model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
     model_s3_client.set_objective_matrices(weights, bias)
```

### Comparing `titanq-0.7.1/tests/test_numpy_util.py` & `titanq-0.8.0/tests/test_numpy_util.py`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/titanq/__init__.py` & `titanq-0.8.0/titanq/__init__.py`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/titanq/_client/client.py` & `titanq-0.8.0/titanq/_client/client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/titanq/_client/model.py` & `titanq-0.8.0/titanq/_client/model.py`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/titanq/_model/constraints.py` & `titanq-0.8.0/titanq/_model/constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,28 @@
 from .numpy_util import convert_to_float32
 
 log = logging.getLogger("TitanQ")
 
 MAX_CONSTRAINTS_COUNT = 16_000
 
 class Constraints:
-    def __init__(self, variable_size: int) -> None:
-        self._variable_size = variable_size
+    def __init__(self) -> None:
+        self._variable_size = 0
         self._constraint_weights = None
         self._constraint_bounds = None
 
 
+    def is_empty(self) -> bool :
+        return self._constraint_bounds is None and self._constraint_weights is None
+
+
+    def augment_size(self, size: int):
+        self._variable_size += size
+
+
     def add_constraint(self, constraint_weights: np.ndarray, constraint_bounds: np.ndarray):
         """
         Add a constraint to the existing ones
 
         :param constraint_weights: constraint_weights to append to the existing ones.
         :param constraint_bounds: constraint_bounds to append to the existing ones.
 
@@ -36,14 +44,16 @@
             raise MaximumConstraintLimitError(
                 "Cannot add additional constraints. The limit of constraints have been reached. " \
                 f"Number of constraints: {self._constraints_rows()} while {self._constraints_rows() + constraint_weights.shape[0]} is trying to be added."
             )
 
         # API only takes np.float32
         constraint_weights = convert_to_float32(constraint_weights)
+        constraint_bounds = convert_to_float32(constraint_bounds)
+
         self._append_constraint_weights(constraint_weights)
         self._append_constraint_bounds(constraint_bounds)
 
 
     def weights(self):
         """
         :return: The weights constraints.
```

### Comparing `titanq-0.7.1/titanq/_model/errors.py` & `titanq-0.8.0/titanq/_model/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 class TitanQError(Exception):
     """Base TitanQ error"""
 
-class MaximumVariableLimitError(TitanQError):
-    """Variable already defined in the model"""
-
 class MissingVariableError(TitanQError):
     """Variable has not already been registered"""
 
+class VariableAlreadyExist(TitanQError):
+    """Variable with the same name already exist"""
+
 class MissingObjectiveError(TitanQError):
     """Objective has not already been registered"""
 
 class MaximumConstraintLimitError(TitanQError):
     """The number of constraints is bigger than the number of variables"""
 
 class ConstraintSizeError(TitanQError):
     """The constraint size does not match"""
 
+class ConstraintAlreadySetError(TitanQError):
+    """A constraint has already been set"""
+
 class ObjectiveAlreadySetError(TitanQError):
     """An objective has already been set"""
 
 class OptimizeError(TitanQError):
     """Error occur during optimization"""
 
 class ServerError(TitanQError):
```

### Comparing `titanq-0.7.1/titanq/_model/manifest.py` & `titanq-0.8.0/titanq/_model/manifest.py`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/titanq/_model/model.py` & `titanq-0.8.0/titanq/_model/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 import logging
 import numpy as np
 import zipfile
 from typing import Any, Dict, List, Tuple
 
 from .constraints import Constraints
 from .errors import (
-    MaximumVariableLimitError,
+    ConstraintAlreadySetError,
     MissingVariableError,
     MissingObjectiveError,
     ObjectiveAlreadySetError,
     OptimizeError
 )
 from .objective import Objective, Target
 from .optimize_response import OptimizeResponse
 from .manifest import Manifest
-from .variable import VariableVector, Vtype
+from .variable import BinaryVariableVector, BipolarVariableVector, IntegerVariableVector, Vtype
 from .._client import api_model, Client
 from .._storage import ManagedStorage, StorageClient
 from .numpy_util import (
     is_ndarray_binary,
     is_upperbound_bigger_equal_lowerbound,
     ndarray_contains_nan_inf,
     reshape_to_2d,
     validate_cardinalities
 )
+from .variable_list import VariableVectorList
 
 log = logging.getLogger("TitanQ")
 
 _TITANQ_BASE_URL = "https://titanq.infinityq.io"
 
 
 class Model:
@@ -71,28 +72,28 @@
                 bucket_name="{insert bucket name here}"
             )
         )
 
         # managed Storage (Up to 10k variables only)
         model = Model(api_key="{insert API key here}")
         """
-        self._variables: VariableVector = None
+        self._variables = VariableVectorList()
         self._objective: Objective = None
-        self._constraints: Constraints = None
+        self._constraints = Constraints()
         self._titanq_client = Client(api_key, base_server_url)
         self._manifest: Manifest = Manifest()
 
         # the user chose a managed storage or left it as default
         if storage_client is None:
             storage_client = ManagedStorage(self._titanq_client)
 
         self._storage_client = storage_client
 
 
-    def add_variable_vector(self, name='', size=1, vtype=Vtype.BINARY):
+    def add_variable_vector(self, name='', size=1, vtype=Vtype.BINARY, variable_bounds: List[Tuple[int, int]]=[]):
         """
         Add a vector of variable to the model. Only a single vector of variables can be set.
         Calling this method again will override the current vector of variables
 
         :param name: The name given to this variable vector.
         :param size: The size of the vector.
         :param vtype: Type of the variables inside the vector.
@@ -108,22 +109,43 @@
         from titanq import Model, Vtype
 
         # set up model
         ...
 
         model.add_variable_vector('x', size, Vtype.BINARY)
         """
-        if self._variables is not None:
-            raise MaximumVariableLimitError("Cannot add additional variable without busting the maximum number of variable (1).")
+        # validation
+        if not self._constraints.is_empty():
+            raise ConstraintAlreadySetError("Cannot add additional variable once constraints have been defined")
 
-        log.debug(f"add variable name='{name}'.")
+        if self._objective is not None:
+            raise ObjectiveAlreadySetError("Cannot add additional variable once objective have been defined")
+
+        # create the Variable vector
+        if vtype is Vtype.BINARY:
+            if variable_bounds:
+                raise ValueError("variable_bounds is not supported with Vtype.BINARY")
+            variables = BinaryVariableVector(name, size)
+
+        elif vtype is Vtype.BIPOLAR:
+            if variable_bounds:
+                raise ValueError("variable_bounds is not supported with Vtype.BIPOLAR")
+            variables = BipolarVariableVector(name, size)
+
+        elif vtype is Vtype.INTEGER:
+            variables = IntegerVariableVector(name, size, variable_bounds)
 
-        self._variables = VariableVector(name, size, vtype)
+        else:
+            raise NotImplementedError(f"Unsupported variable type: {vtype}")
+
+        self._variables.add(variables)
+        self._constraints.augment_size(size)
+
+        log.debug(f"add variable name='{name}', type={str(vtype)}, size={size}.")
 
-        self._constraints = Constraints(size)
 
 
     def set_objective_matrices(self, weights: np.ndarray, bias: np.ndarray, target=Target.MINIMIZE):
         """
         Set the objective matrices for the model.
 
         :param weights: The quadratic objective matrix, **this matrix needs to be symmetrical**
@@ -160,23 +182,23 @@
 
         # set up model
         ...
 
         model.set_objective_matrices(weights, bias, Target.MINIMIZE)
         """
 
-        if self._variables is None:
+        if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set objective before adding a variable to the model.")
 
         if self._objective is not None:
             raise ObjectiveAlreadySetError("An objective has already have been set for this model.")
 
         log.debug(f"set objective matrix and bias vector.")
 
-        self._objective = Objective(self._variables.size(), weights, bias, target)
+        self._objective = Objective(self._variables.total_variable_size(), weights, bias, target)
 
 
     def set_constraints_matrices(self, constraint_weights: np.ndarray, constraint_bounds: np.ndarray):
         """
         Set the constraints matrices for the model.
 
         :param constraint_weights: The constraint_weights matrix of shape (M, N) where M the number of constraints and N is the number of variables
@@ -185,15 +207,15 @@
         :param constraint_bounds: The constraint_bounds vector of shape (M,2) where M is the number of constraints
         :type constraint_bounds:  a NumPy 1-D ndarray (must be float32)
 
         :raise MissingVariableError: If no variable have been added to the model.
         :raise ValueError: If the constraint_weights shape or the constraint_bounds shape does not fit the expected shape of this model.
         :raise ValueError: If the constraint_weights or constraint_bounds data type is not f32.
         """
-        if self._variables is None:
+        if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
         log.debug(f"set weights constraints matrix and bias constraints vector.")
         self._constraints.set_constraint_matrices(constraint_weights, constraint_bounds)
 
 
     def add_set_partitioning_constraints_matrix(self, constraint_mask: np.ndarray):
@@ -217,15 +239,15 @@
 
         # set up model
         ...
 
         constraint_mask = np.array([[1, 1, 1, 0, 1], [1, 1, 1, 1, 0]])
         model.add_set_partitioning_constraints_matrix(constraint_mask)
         """
-        if self._variables is None:
+        if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
         if constraint_mask.ndim == 1:
             raise ValueError(
                 "Cannot use add_set_partitioning_constraints_matrix() function with a vector, " \
                 "please use add_set_partitioning_constraint() insead")
 
@@ -296,15 +318,15 @@
         # set up model
         ...
 
         constraint_mask = np.array([[1, 1, 1, 0, 1], [1, 1, 1, 1, 0]])
         cardinalities = np.array([3, 2])
         model.add_cardinality_constraints_matrix(constraint_mask, cardinalities)
         """
-        if self._variables is None:
+        if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
         if constraint_mask.ndim == 1:
             raise ValueError(
                 "Cannot use add_cardinality_constraints_matrix() function with a vector, " \
                 "please use add_cardinality_constraint() insead")
 
@@ -374,36 +396,42 @@
     def add_equality_constraints_matrix(self, constraint_mask: np.ndarray, limit: np.ndarray) -> None:
         """
         Adds an equality constraint matrix to the model.
 
         :param constraint_mask: The constraint_mask vector of shape (M, N) where M the number of constraints and N is the number of variables.
         :type constraint_mask: A NumPy 2-D dense ndarray (float32)
         :param limit: The limit vector of shape (M,) where M is the number of constraints
-        :type limit: A NumPy 1-D array
+        :type limit: A NumPy 1-D array (float32)
 
         :raise MissingVariableError: If no variable have been added to the model.
-        :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
+        :raises MaximumConstraintLimitError: The number of constraint exceed the limit.
         :raise ValueError: If the constraint_mask shape does not fit the expected shape of this model.
         :raise ValueError: If the constraint_mask or limit contains irregular format ('NaN' or 'inf')
         """
-        if self._variables is None:
+        if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
+        if constraint_mask.dtype != np.float32 or limit.dtype != np.float32:
+            raise ValueError(f"Input parameters must be float32, got Constraint mask: {constraint_mask.dtype}, Limit: {limit.dtype}")
+
         if constraint_mask.ndim == 1:
             raise ValueError(
                 "Cannot use add_equality_constraint_matrix() function with a vector, " \
                 "please use add_equality_constraint() insead")
 
         if ndarray_contains_nan_inf(constraint_mask):
             raise ValueError("Constraint mask contains NaN  or inf values")
 
+        if limit.ndim != 1:
+            raise ValueError("Limit must be a NumPy 1-D array")
+
         if ndarray_contains_nan_inf(limit):
             raise ValueError("Limit contains NaN or inf values")
 
-        if self._variables.vtype() == Vtype.BIPOLAR:
+        if self._variables.has_variable_of_type(Vtype.BIPOLAR):
             raise ValueError("Cannot add equality constraint with variable vector set to 'bipolar'")
 
         self._constraints.add_constraint(
             constraint_weights=constraint_mask,
             constraint_bounds=np.repeat(limit, 2).reshape(-1, 2)
         )
         self._manifest.activate_equality_constraint()
@@ -441,17 +469,20 @@
 
         :raise MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
         :raise ValueError: If the constraint_mask shape does not fit the expected shape of this model.
         :raise ValueError: A lowerbound is equal or higher than its given upperbound
         :raise ValueError: If the constraint_mask contains irregular format ('NaN' or 'inf')
         """
-        if self._variables is None:
+        if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
+        if constraint_mask.dtype != np.float32 or constraint_bounds.dtype != np.float32:
+            raise ValueError(f"Input parameters must be float32, got Constraint mask: {constraint_mask.dtype}, Limit: {constraint_bounds.dtype}")
+
         if constraint_mask.ndim == 1:
             raise ValueError(
                 "Cannot use add_inequality_constraint_matrix() function with a vector, " \
                 "please use add_inequality_constraint() insead")
 
         if ndarray_contains_nan_inf(constraint_mask):
             raise ValueError("Constraint mask contains NaN  or inf values.")
@@ -526,23 +557,23 @@
         # print values
         print("-" * 15, "+", "-" * 26, sep="")
         print("Ising energy   | Result vector")
         print("-" * 15, "+", "-" * 26, sep="")
         for ising_energy, result_vector in response.result_items():
             print(f"{ising_energy: <14f} | {result_vector}")
         """
-        if self._variables is None:
+        if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot optimize before adding a variable to the model.")
 
         if self._objective is None:
             raise MissingObjectiveError("Cannot optimize before adding an objective to the model.")
 
         result, metrics = self._solve(beta, coupling_mult, timeout_in_secs, num_chains, num_engines, normalized)
 
-        return OptimizeResponse(self._variables.name(), result, metrics)
+        return OptimizeResponse(self._variables, result, metrics)
 
     def _solve(self,
             beta: List[float],
             coupling_mult: float,
             timeout_in_secs: float,
             num_chains: int,
             num_engines: int,
@@ -561,29 +592,29 @@
         """
         with self._storage_client.temp_files_manager(
             self._objective.bias(),
             self._objective.weights(),
             self._constraints.bounds() if self._constraints else None,
             self._constraints.weights() if self._constraints else None,
             # variables bounds is only sent if variable is set to binary
-            self._variables.create_variable_bounds() if self._variables.vtype() != Vtype.BIPOLAR else None
+            self._variables.variable_bounds() if not self._variables.has_variable_of_type(Vtype.BIPOLAR) else None
         ) as temp_files:
 
             # api request
             request = api_model.SolveRequest(
                 input=temp_files.input(),
                 output=temp_files.output(),
                 parameters=api_model.Parameters(
                     beta=beta,
                     coupling_mult=coupling_mult,
                     num_chains=num_chains,
                     num_engines=num_engines,
                     normalized=normalized,
                     timeout_in_secs=timeout_in_secs,
-                    variable_types=self._get_variable_types()
+                    variable_types=self._variables.get_variable_types_str(self._manifest.has_equality_constraint(), self._manifest.has_inequality_constraint())
                 )
             )
 
             # adding manifest flags to the request
             request.input.manifest = api_model.Manifest(
                 has_set_partitioning_constraint=self._manifest.has_set_partitioning_constraint(),
                 has_cardinality_constraint=self._manifest.has_cardinality_constraint(),
@@ -606,18 +637,7 @@
                     except KeyError as e:
                         raise OptimizeError(
                             "Unexpected error in the solver, please contact InfinityQ support for more help" \
                             f" and provide the following computation id {solve_response.computation_id}") from e
 
         log.debug("Optimization completed")
         return np.load(io.BytesIO(result_content)), json.loads(metrics_content)
-
-
-    def _get_variable_types(self):
-        """
-        Will return the variables types based on the manifest
-        if equality or inequality -> 'bbbbbbb...'
-        if not 'binary' or 'bipolar'
-        """
-        if self._manifest.has_equality_constraint() or self._manifest.has_inequality_constraint():
-            return self._variables.variable_types_as_list()
-        return str(self._variables.vtype())
```

### Comparing `titanq-0.7.1/titanq/_model/numpy_util.py` & `titanq-0.8.0/titanq/_model/numpy_util.py`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/titanq/_model/objective.py` & `titanq-0.8.0/titanq/_model/objective.py`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/titanq/_model/optimize_response.py` & `titanq-0.8.0/titanq/_model/optimize_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,50 @@
 import logging
 from typing import Any, Dict, List, Tuple, Union
 import uuid
 import warnings
 
 import numpy as np
 
+from .variable_list import VariableVectorList
+
 log = logging.getLogger('TitanQ')
 
 class OptimizeResponse:
     """
     Object containing Optimization response and all its metrics.
     """
-    def __init__(self, var_name: str, result_array: np.ndarray, metrics: Dict[str, Any]) -> None:
-        self._var_name = var_name
-        self._result_vector = result_array
+    def __init__(self, variable_list: VariableVectorList, result_array: np.ndarray, metrics: Dict[str, Any]) -> None:
+        self._result_by_variable: Dict[str, np.ndarray] = {}
+        start_index = 0
+
+        # extract all the result for each given variable
+        # The result array is a 2d array where each line is a different result of the same problem
+        for variable_vector in  variable_list:
+
+            result_for_this_variable = []
+            last_index = start_index + variable_vector.size()
+
+            for full_result in result_array:
+                result_extracted = full_result[start_index: last_index]
+                result_for_this_variable.append(result_extracted)
+
+            self._result_by_variable[variable_vector.name()] = np.array(result_for_this_variable)
+            start_index = last_index
+
         self._metrics = metrics
+        self._all_results = result_array
 
 
     def __getattr__(self, attr: str):
-        # if attribute is the _var_name
-        if attr == self._var_name:
-            return self.result_vector()
+        # if attribute is the name of a variable
+        try:
+            return self._result_by_variable[attr]
+        except KeyError:
+            pass
 
         # This is to keep compatibility with older version of SDK
         if attr == "ising_energy":
             try:
                 return self.__getattr__("solutions_objective_value")
             except (AttributeError, KeyError):
                 pass
@@ -55,26 +75,26 @@
             raise AttributeError(attr)
 
 
     def result_vector(self) -> np.ndarray:
         """
         :return: The result vector of this optimization.
         """
-        return self._result_vector
+        return self._all_results
 
 
     def result_items(self) -> List[Tuple[int, np.ndarray]]:
         """
         ex. [(-10000, [0, 1, 1, 0]), (-20000, [1, 0, 1, 0]), ...]
 
         :return: list of tuples containing the solutions objective value and it's corresponding result vector
         """
 
         solutions_objective_value = self.ising_energy
-        return [(solutions_objective_value[i], self._result_vector[i]) for i in range(len(self._result_vector))]
+        return [(solutions_objective_value[i], self._all_results[i]) for i in range(len(self._all_results))]
 
 
     def computation_metrics(self, key: str = None) -> Any:
         """
         :return: All computation metrics if no key is given of the specific metrics with the associated key if one is provided.
 
         :raise KeyError: The given key does not exist
```

### Comparing `titanq-0.7.1/titanq/_model/variable.py` & `titanq-0.8.0/titanq/_model/variable.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,107 @@
+import abc
 import enum
+from typing import List, Tuple
 import numpy as np
+from numpy._typing import NDArray
 
 class Vtype(str, enum.Enum):
     BINARY = 'binary'
     BIPOLAR = 'bipolar'
+    INTEGER = 'integer'
 
     def __str__(self) -> str:
         return str(self.value)
 
-class VariableVector:
+class VariableVector(abc.ABC):
     """
     Object That represent a vector of variable to be optimized.
     """
-    def __init__(self, name='', size=1, vtype=Vtype.BINARY) -> None:
+    def __init__(self, name: str, size: int) -> None:
         if size < 1:
             raise ValueError("Variable vector size cannot be less than 1")
 
         self._name = name
         self._size = size
-        self._vtype = vtype
 
 
     def size(self) -> int:
         """
         :return: size of this vector.
         """
         return self._size
 
-    def vtype(self) -> Vtype:
-        """
-        :return: Type of variable in the vector.
-        """
-        return self._vtype
 
     def name(self) -> str:
         """
         :return: Name of this variable vector.
         """
         return self._name
 
+
+    @abc.abstractmethod
+    def vtype(self) -> Vtype:
+        """
+        :return: Type of variable in the vector.
+        """
+
+
+    @abc.abstractmethod
     def variable_types_as_list(self) -> str:
         """
-        :return: Generate a string of 'b' depending on the variable size
+        :return: Generate a string of 'b' or 'i' depending on the variable type
         """
-        if self._vtype == Vtype.BIPOLAR:
-            raise ValueError("Cannot set variable types as a list for 'bipolar' type")
 
-        return "".join(['b' for _ in range(self._size)])
 
-    def create_variable_bounds(self):
+    @abc.abstractmethod
+    def variable_bounds(self) -> NDArray:
         """
-        :return: Generate a string of 'b' depending on the variable size
+        :return: The variable bounds associated to this variable vector
         """
-        if self._vtype == Vtype.BIPOLAR:
-            raise ValueError("Cannot set variable types as a list for 'bipolar' type")
 
-        return np.tile(np.array([0,1]), (self._size, 1))
+
+class BinaryVariableVector(VariableVector):
+    def vtype(self) -> Vtype:
+        return Vtype.BINARY
+
+
+    def variable_types_as_list(self) -> str:
+        return "b" * self.size()
+
+
+    def variable_bounds(self) -> NDArray:
+        return np.tile(np.array([0,1], dtype=np.float32), (self._size, 1))
+
+
+# This class violate the Liskov Substitution Principle because it raise error in some of
+# the method it need to implement. This is somewhat fine for now but should be fix soon.
+class BipolarVariableVector(VariableVector):
+    def vtype(self) -> Vtype:
+        return Vtype.BIPOLAR
+
+    def variable_types_as_list(self) -> str:
+        raise ValueError("Cannot set variable types as a list for 'bipolar' variable type")
+
+    def variable_bounds(self) -> NDArray:
+        raise ValueError("Cannot define variable bounds for 'bipolar' variable type")
+
+
+class IntegerVariableVector(VariableVector):
+    def __init__(self, name: str, size: int, variable_bounds: List[Tuple[int, int]]) -> None:
+        super().__init__(name, size)
+
+        if len(variable_bounds) != self.size():
+            raise ValueError("variable_bounds need to be the same length as variable size")
+
+        self._variable_bounds = np.array(variable_bounds, dtype=np.float32)
+
+
+    def vtype(self) -> Vtype:
+        return Vtype.INTEGER
+
+
+    def variable_types_as_list(self) -> str:
+        return "i" * self.size()
+
+
+    def variable_bounds(self) -> NDArray:
+        return self._variable_bounds
```

### Comparing `titanq-0.7.1/titanq/_storage/managed_storage.py` & `titanq-0.8.0/titanq/_storage/managed_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from .storage_client import StorageClient
 from .._client.client import Client
 from .._model.errors import ConnectionError
 
 log = logging.getLogger("TitanQ")
 
 
-
 class ManagedStorage(StorageClient):
     def __init__(self, titanq_client: Client):
         """
         Initiate the managed storage client for handling the temporary files.
 
         :titanq_client: titanq_client to be used to fetch temporary URL's
         """
```

### Comparing `titanq-0.7.1/titanq/_storage/s3_storage.py` & `titanq-0.8.0/titanq/_storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/titanq/_storage/storage_client.py` & `titanq-0.8.0/titanq/_storage/storage_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.7.1/titanq.egg-info/PKG-INFO` & `titanq-0.8.0/titanq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.7.1
+Version: 0.8.0
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
```

### Comparing `titanq-0.7.1/titanq.egg-info/SOURCES.txt` & `titanq-0.8.0/titanq.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,11 +21,12 @@
 titanq/_model/errors.py
 titanq/_model/manifest.py
 titanq/_model/model.py
 titanq/_model/numpy_util.py
 titanq/_model/objective.py
 titanq/_model/optimize_response.py
 titanq/_model/variable.py
+titanq/_model/variable_list.py
 titanq/_storage/__init__.py
 titanq/_storage/managed_storage.py
 titanq/_storage/s3_storage.py
 titanq/_storage/storage_client.py
```

