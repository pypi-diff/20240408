# Comparing `tmp/pylearningstandards-0.1.0.tar.gz` & `tmp/pylearningstandards-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylearningstandards-0.1.0.tar", max compression
+gzip compressed data, was "pylearningstandards-0.2.0.tar", max compression
```

## Comparing `pylearningstandards-0.1.0.tar` & `pylearningstandards-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-02 21:28:52.185732 pylearningstandards-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 21:28:26.555732 pylearningstandards-0.1.0/py_learning_standards/__init__.py
--rw-r--r--   0        0        0      331 2024-04-02 21:27:55.165732 pylearningstandards-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 pylearningstandards-0.1.0/setup.py
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 pylearningstandards-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1812 2024-02-16 21:19:55.487949 pylearningstandards-0.2.0/LICENSE
+-rw-r--r--   0        0        0      920 2024-02-16 21:19:55.487949 pylearningstandards-0.2.0/LICENSE_HEADER
+-rw-r--r--   0        0        0        0 2024-04-02 21:28:52.185732 pylearningstandards-0.2.0/README.md
+-rw-r--r--   0        0        0     3569 2024-04-08 20:44:59.275731 pylearningstandards-0.2.0/py_learning_standards/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-08 20:47:11.585732 pylearningstandards-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 pylearningstandards-0.2.0/setup.py
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 pylearningstandards-0.2.0/PKG-INFO
```

### Comparing `pylearningstandards-0.1.0/setup.py` & `pylearningstandards-0.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 
 packages = \
 ['py_learning_standards']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['dataclass-wizard>=0.22.3,<0.23.0', 'pyld>=2.0.4,<3.0.0']
+
 setup_kwargs = {
     'name': 'pylearningstandards',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': '',
     'author': 'Daniel Auerbach',
     'author_email': 'auerbach@ict.usc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
+    'install_requires': install_requires,
+    'python_requires': '>=3.8.4,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

