# Comparing `tmp/sigstore-2.1.3.tar.gz` & `tmp/sigstore-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigstore-2.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigstore-2.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigstore-2.1.3.tar` & `sigstore-2.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11358 2024-03-19 17:26:50.821714 sigstore-2.1.3/LICENSE
--rw-r--r--   0        0        0    20630 2024-03-19 17:26:50.821714 sigstore-2.1.3/README.md
--rw-r--r--   0        0        0     3939 2024-03-19 17:26:50.821714 sigstore-2.1.3/pyproject.toml
--rw-r--r--   0        0        0      955 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/__init__.py
--rw-r--r--   0        0        0      726 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/__main__.py
--rw-r--r--   0        0        0    35844 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_cli.py
--rw-r--r--   0        0        0      738 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/__init__.py
--rw-r--r--   0        0        0      774 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/ctfe.py
--rw-r--r--   0        0        0      883 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/fulcio/__init__.py
--rw-r--r--   0        0        0    12112 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/fulcio/client.py
--rw-r--r--   0        0        0     3891 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/keyring.py
--rw-r--r--   0        0        0     4544 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/merkle.py
--rw-r--r--   0        0        0      653 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/oidc/__init__.py
--rw-r--r--   0        0        0    15958 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/oidc/oauth.py
--rw-r--r--   0        0        0      748 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/rekor/__init__.py
--rw-r--r--   0        0        0     7235 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/rekor/checkpoint.py
--rw-r--r--   0        0        0     8026 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/rekor/client.py
--rw-r--r--   0        0        0     9884 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/sct.py
--rw-r--r--   0        0        0     1729 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/set.py
--rw-r--r--   0        0        0     9403 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_internal/tuf.py
--rw-r--r--   0        0        0     1247 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_store/__init__.py
--rw-r--r--   0        0        0     6388 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_store/prod/root.json
--rw-r--r--   0        0        0     4567 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_store/prod/trusted_root.json
--rw-r--r--   0        0        0     1876 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_store/staging/root.json
--rw-r--r--   0        0        0     4521 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_store/staging/trusted_root.json
--rw-r--r--   0        0        0    10225 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/_utils.py
--rw-r--r--   0        0        0     3247 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/errors.py
--rw-r--r--   0        0        0    15939 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/oidc.py
--rw-r--r--   0        0        0    13258 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/sign.py
--rw-r--r--   0        0        0     5519 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/transparency.py
--rw-r--r--   0        0        0     1932 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/verify/__init__.py
--rw-r--r--   0        0        0    18223 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/verify/models.py
--rw-r--r--   0        0        0     9824 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/verify/policy.py
--rw-r--r--   0        0        0    11484 2024-03-19 17:26:50.825714 sigstore-2.1.3/sigstore/verify/verifier.py
--rw-r--r--   0        0        0    22793 1970-01-01 00:00:00.000000 sigstore-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-08 14:27:08.179680 sigstore-2.1.5/LICENSE
+-rw-r--r--   0        0        0    20630 2024-04-08 14:27:08.179680 sigstore-2.1.5/README.md
+-rw-r--r--   0        0        0     3948 2024-04-08 14:27:08.179680 sigstore-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0      955 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/__init__.py
+-rw-r--r--   0        0        0      726 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/__main__.py
+-rw-r--r--   0        0        0    35844 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_cli.py
+-rw-r--r--   0        0        0      738 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/__init__.py
+-rw-r--r--   0        0        0      774 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/ctfe.py
+-rw-r--r--   0        0        0      883 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/fulcio/__init__.py
+-rw-r--r--   0        0        0    12112 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/fulcio/client.py
+-rw-r--r--   0        0        0     3891 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/keyring.py
+-rw-r--r--   0        0        0     4544 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/merkle.py
+-rw-r--r--   0        0        0      653 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/oidc/__init__.py
+-rw-r--r--   0        0        0    15958 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/oidc/oauth.py
+-rw-r--r--   0        0        0      748 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/rekor/__init__.py
+-rw-r--r--   0        0        0     7235 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/rekor/checkpoint.py
+-rw-r--r--   0        0        0     8026 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/rekor/client.py
+-rw-r--r--   0        0        0     9884 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/sct.py
+-rw-r--r--   0        0        0     1729 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/set.py
+-rw-r--r--   0        0        0     9403 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_internal/tuf.py
+-rw-r--r--   0        0        0     1247 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_store/__init__.py
+-rw-r--r--   0        0        0     6388 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_store/prod/root.json
+-rw-r--r--   0        0        0     4567 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_store/prod/trusted_root.json
+-rw-r--r--   0        0        0     1876 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_store/staging/root.json
+-rw-r--r--   0        0        0     4521 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_store/staging/trusted_root.json
+-rw-r--r--   0        0        0    10225 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/_utils.py
+-rw-r--r--   0        0        0     3247 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/errors.py
+-rw-r--r--   0        0        0    15939 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/oidc.py
+-rw-r--r--   0        0        0    13258 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/sign.py
+-rw-r--r--   0        0        0     5519 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/transparency.py
+-rw-r--r--   0        0        0     1932 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/verify/__init__.py
+-rw-r--r--   0        0        0    18223 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/verify/models.py
+-rw-r--r--   0        0        0     9824 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/verify/policy.py
+-rw-r--r--   0        0        0    11484 2024-04-08 14:27:08.179680 sigstore-2.1.5/sigstore/verify/verifier.py
+-rw-r--r--   0        0        0    22802 1970-01-01 00:00:00.000000 sigstore-2.1.5/PKG-INFO
```

### Comparing `sigstore-2.1.3/LICENSE` & `sigstore-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/README.md` & `sigstore-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/pyproject.toml` & `sigstore-2.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   "id >= 1.1.0",
   "importlib_resources ~= 5.7; python_version < '3.11'",
   "pydantic >= 2,< 3",
   "pyjwt >= 2.1",
   "pyOpenSSL >= 23.0.0",
   "requests",
   "rich ~= 13.0",
-  "securesystemslib",
+  "securesystemslib < 0.32.0",
   "sigstore-protobuf-specs >= 0.2.2, < 0.4",
   # NOTE(ww): Under active development, so strictly pinned.
   "sigstore-rekor-types == 0.0.11",
   "tuf >= 2.1,< 4.0",
 ]
 requires-python = ">=3.8"
```

### Comparing `sigstore-2.1.3/sigstore/__init__.py` & `sigstore-2.1.5/sigstore/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 Otherwise, here are some quick starting points:
 
 * `sigstore.verify`: verifying of Sigstore signatures,
   including flexible policy control
 * `sigstore.sign`: creation of Sigstore signatures
 """
 
-__version__ = "2.1.3"
+__version__ = "2.1.5"
```

### Comparing `sigstore-2.1.3/sigstore/__main__.py` & `sigstore-2.1.5/sigstore/__main__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_cli.py` & `sigstore-2.1.5/sigstore/_cli.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/__init__.py` & `sigstore-2.1.5/sigstore/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/ctfe.py` & `sigstore-2.1.5/sigstore/_internal/ctfe.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/fulcio/__init__.py` & `sigstore-2.1.5/sigstore/_internal/fulcio/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/fulcio/client.py` & `sigstore-2.1.5/sigstore/_internal/fulcio/client.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/keyring.py` & `sigstore-2.1.5/sigstore/_internal/keyring.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/merkle.py` & `sigstore-2.1.5/sigstore/_internal/merkle.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/oidc/__init__.py` & `sigstore-2.1.5/sigstore/_internal/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/oidc/oauth.py` & `sigstore-2.1.5/sigstore/_internal/oidc/oauth.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/rekor/__init__.py` & `sigstore-2.1.5/sigstore/_internal/rekor/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/rekor/checkpoint.py` & `sigstore-2.1.5/sigstore/_internal/rekor/checkpoint.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/rekor/client.py` & `sigstore-2.1.5/sigstore/_internal/rekor/client.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/sct.py` & `sigstore-2.1.5/sigstore/_internal/sct.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/set.py` & `sigstore-2.1.5/sigstore/_internal/set.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_internal/tuf.py` & `sigstore-2.1.5/sigstore/_internal/tuf.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_store/__init__.py` & `sigstore-2.1.5/sigstore/_store/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_store/prod/root.json` & `sigstore-2.1.5/sigstore/_store/prod/root.json`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_store/prod/trusted_root.json` & `sigstore-2.1.5/sigstore/_store/prod/trusted_root.json`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_store/staging/root.json` & `sigstore-2.1.5/sigstore/_store/staging/root.json`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_store/staging/trusted_root.json` & `sigstore-2.1.5/sigstore/_store/staging/trusted_root.json`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/_utils.py` & `sigstore-2.1.5/sigstore/_utils.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/errors.py` & `sigstore-2.1.5/sigstore/errors.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/oidc.py` & `sigstore-2.1.5/sigstore/oidc.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/sign.py` & `sigstore-2.1.5/sigstore/sign.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/transparency.py` & `sigstore-2.1.5/sigstore/transparency.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/verify/__init__.py` & `sigstore-2.1.5/sigstore/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/verify/models.py` & `sigstore-2.1.5/sigstore/verify/models.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/verify/policy.py` & `sigstore-2.1.5/sigstore/verify/policy.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/sigstore/verify/verifier.py` & `sigstore-2.1.5/sigstore/verify/verifier.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.1.3/PKG-INFO` & `sigstore-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigstore
-Version: 2.1.3
+Version: 2.1.5
 Summary: A tool for signing Python package distributions
 Author-email: Sigstore Authors <sigstore-dev@googlegroups.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 Requires-Dist: id >= 1.1.0
 Requires-Dist: importlib_resources ~= 5.7; python_version < '3.11'
 Requires-Dist: pydantic >= 2,< 3
 Requires-Dist: pyjwt >= 2.1
 Requires-Dist: pyOpenSSL >= 23.0.0
 Requires-Dist: requests
 Requires-Dist: rich ~= 13.0
-Requires-Dist: securesystemslib
+Requires-Dist: securesystemslib < 0.32.0
 Requires-Dist: sigstore-protobuf-specs >= 0.2.2, < 0.4
 Requires-Dist: sigstore-rekor-types == 0.0.11
 Requires-Dist: tuf >= 2.1,< 4.0
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: bump >= 1.3.2 ; extra == "dev"
 Requires-Dist: sigstore[doc,test,lint] ; extra == "dev"
 Requires-Dist: pdoc ; extra == "doc"
```

