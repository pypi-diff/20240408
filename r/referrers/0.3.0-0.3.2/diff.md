# Comparing `tmp/referrers-0.3.0.tar.gz` & `tmp/referrers-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "referrers-0.3.0.tar", max compression
+gzip compressed data, was "referrers-0.3.2.tar", max compression
```

## Comparing `referrers-0.3.0.tar` & `referrers-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-03-27 21:43:39.382657 referrers-0.3.0/LICENSE
--rw-r--r--   0        0        0     6825 2024-03-27 21:43:39.382657 referrers-0.3.0/README.md
--rw-r--r--   0        0        0      372 2024-03-27 21:43:39.382657 referrers-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      130 2024-03-27 21:43:39.382657 referrers-0.3.0/src/referrers/__init__.py
--rw-r--r--   0        0        0    37144 2024-03-27 21:43:39.382657 referrers-0.3.0/src/referrers/impl.py
--rw-r--r--   0        0        0     7358 1970-01-01 00:00:00.000000 referrers-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 21:18:50.216968 referrers-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6887 2024-04-08 21:18:50.216968 referrers-0.3.2/README.md
+-rw-r--r--   0        0        0      372 2024-04-08 21:18:50.216968 referrers-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-04-08 21:18:50.216968 referrers-0.3.2/src/referrers/__init__.py
+-rw-r--r--   0        0        0    37144 2024-04-08 21:18:50.216968 referrers-0.3.2/src/referrers/impl.py
+-rw-r--r--   0        0        0     7420 1970-01-01 00:00:00.000000 referrers-0.3.2/PKG-INFO
```

### Comparing `referrers-0.3.0/LICENSE` & `referrers-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `referrers-0.3.0/README.md` & `referrers-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,53 @@
+Metadata-Version: 2.1
+Name: referrers
+Version: 0.3.2
+Summary: Finds the graph of referrers for a Python object
+Author: Neil Ferguson
+Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: networkx (>=3.1.0)
+Description-Content-Type: text/markdown
+
 # Referrers
 
 Referrers is a Python package that helps to answer the question **"what is holding
 a reference to this object?"**, which is useful for debugging memory leaks and other
 issues. It tries to assign a meaningful name to each reference to an object and
 returns a graph of referrers (including indirect referrers).
 
-As a simple example, here is the graph of referrers for an instance of a Python `list`:
+For example, this code:
+
+```python
+import referrers
+
+def my_function():
+    a = [2, 4]
+    d = dict(a=a)
+    print(referrers.get_referrer_graph(a))
+
+my_function()
+```
+
+Will produce output like:
 
 ```plaintext
-╙── list instance (id=4514970240)
-    └─╼ ParentClass.member_variable (instance attribute) (id=4513308624)
-        └─╼ my_func.local_variable (local) (id=4513308624)
+╙── list instance (id=4346564736)
+    ├─╼ dict[a] (id=4347073728)
+    │   └─╼ my_function.d (local) (id=4347073728)
+    └─╼ my_function.a (local) (id=4346564736)
 ```
 
-In this case the list instance is referenced by a member variable of `ParentClass`, which
-is in turn referenced by a local variable in the `my_func` function. For the code to produce
-this graph see "Basic Example" below.
+In this case the list instance is referenced directly by a local variable called `a`, and also
+via a dictionary, which is in turn referenced by a local variable called `d`.
 
 Note: this package is experimental and may not work in all cases. It may also be inefficient
 in certain cases, and should not be used in performance-critical code.
 
 ## Installation
 
 Install using pip:
@@ -224,7 +252,8 @@
 
 my_function()
 ```
 
 ## Source
 
 See [https://github.com/nfergu/referrers](https://github.com/nfergu/referrers) for the Github repo.
+
```

### Comparing `referrers-0.3.0/src/referrers/impl.py` & `referrers-0.3.2/src/referrers/impl.py`

 * *Files identical despite different names*

### Comparing `referrers-0.3.0/PKG-INFO` & `referrers-0.3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-Metadata-Version: 2.1
-Name: referrers
-Version: 0.3.0
-Summary: Finds the graph of referrers for a Python object
-Author: Neil Ferguson
-Requires-Python: >=3.8
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: networkx (>=3.1.0)
-Description-Content-Type: text/markdown
-
 # Referrers
 
 Referrers is a Python package that helps to answer the question **"what is holding
 a reference to this object?"**, which is useful for debugging memory leaks and other
 issues. It tries to assign a meaningful name to each reference to an object and
 returns a graph of referrers (including indirect referrers).
 
-As a simple example, here is the graph of referrers for an instance of a Python `list`:
+For example, this code:
+
+```python
+import referrers
+
+def my_function():
+    a = [2, 4]
+    d = dict(a=a)
+    print(referrers.get_referrer_graph(a))
+
+my_function()
+```
+
+Will produce output like:
 
 ```plaintext
-╙── list instance (id=4514970240)
-    └─╼ ParentClass.member_variable (instance attribute) (id=4513308624)
-        └─╼ my_func.local_variable (local) (id=4513308624)
+╙── list instance (id=4346564736)
+    ├─╼ dict[a] (id=4347073728)
+    │   └─╼ my_function.d (local) (id=4347073728)
+    └─╼ my_function.a (local) (id=4346564736)
 ```
 
-In this case the list instance is referenced by a member variable of `ParentClass`, which
-is in turn referenced by a local variable in the `my_func` function. For the code to produce
-this graph see "Basic Example" below.
+In this case the list instance is referenced directly by a local variable called `a`, and also
+via a dictionary, which is in turn referenced by a local variable called `d`.
 
 Note: this package is experimental and may not work in all cases. It may also be inefficient
 in certain cases, and should not be used in performance-critical code.
 
 ## Installation
 
 Install using pip:
@@ -239,8 +237,7 @@
 
 my_function()
 ```
 
 ## Source
 
 See [https://github.com/nfergu/referrers](https://github.com/nfergu/referrers) for the Github repo.
-
```

