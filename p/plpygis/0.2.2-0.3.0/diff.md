# Comparing `tmp/plpygis-0.2.2.tar.gz` & `tmp/plpygis-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plpygis-0.2.2.tar", last modified: Fri Mar  8 11:07:36 2024, max compression
+gzip compressed data, was "plpygis-0.3.0.tar", last modified: Mon Apr  8 19:26:07 2024, max compression
```

## Comparing `plpygis-0.2.2.tar` & `plpygis-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-03-08 11:07:36.454035 plpygis-0.2.2/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-03-08 11:07:36.447367 plpygis-0.2.2/.github/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-03-08 11:07:36.450701 plpygis-0.2.2/.github/workflows/
--rw-r--r--   0 ben       (1000) ben       (1000)      590 2024-03-08 10:22:13.000000 plpygis-0.2.2/.github/workflows/pythonpackage.yml
--rw-r--r--   0 ben       (1000) ben       (1000)     1172 2024-03-08 10:22:13.000000 plpygis-0.2.2/.gitignore
--rw-r--r--   0 ben       (1000) ben       (1000)      813 2024-03-08 10:57:50.000000 plpygis-0.2.2/CHANGELOG.md
--rw-r--r--   0 ben       (1000) ben       (1000)    35142 2024-03-08 10:22:13.000000 plpygis-0.2.2/LICENSE
--rw-r--r--   0 ben       (1000) ben       (1000)      102 2024-03-08 10:22:13.000000 plpygis-0.2.2/MANIFEST.in
--rw-r--r--   0 ben       (1000) ben       (1000)      203 2024-03-08 10:22:13.000000 plpygis-0.2.2/Makefile
--rw-r--r--   0 ben       (1000) ben       (1000)     2335 2024-03-08 11:07:36.454035 plpygis-0.2.2/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)     1860 2024-03-08 10:22:13.000000 plpygis-0.2.2/README.rst
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-03-08 11:07:36.450701 plpygis-0.2.2/doc/
--rw-r--r--   0 ben       (1000) ben       (1000)      610 2024-03-08 10:22:13.000000 plpygis-0.2.2/doc/Makefile
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-03-08 11:07:36.450701 plpygis-0.2.2/doc/source/
--rw-r--r--   0 ben       (1000) ben       (1000)     4912 2024-03-08 10:22:13.000000 plpygis-0.2.2/doc/source/conf.py
--rw-r--r--   0 ben       (1000) ben       (1000)     8289 2024-03-08 10:22:13.000000 plpygis-0.2.2/doc/source/examples.rst
--rw-r--r--   0 ben       (1000) ben       (1000)      678 2024-03-08 10:22:13.000000 plpygis-0.2.2/doc/source/index.rst
--rw-r--r--   0 ben       (1000) ben       (1000)     1380 2024-03-08 10:22:13.000000 plpygis-0.2.2/doc/source/installation.rst
--rw-r--r--   0 ben       (1000) ben       (1000)      240 2024-03-08 10:22:13.000000 plpygis-0.2.2/doc/source/plpygis.rst
--rw-r--r--   0 ben       (1000) ben       (1000)     9484 2024-03-08 10:22:13.000000 plpygis-0.2.2/doc/source/plpython.rst
--rw-r--r--   0 ben       (1000) ben       (1000)     8323 2024-03-08 10:22:13.000000 plpygis-0.2.2/doc/source/subclasses.rst
--rw-r--r--   0 ben       (1000) ben       (1000)     3918 2024-03-08 10:22:13.000000 plpygis-0.2.2/doc/source/usage.rst
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-03-08 11:07:36.450701 plpygis-0.2.2/plpygis/
--rw-r--r--   0 ben       (1000) ben       (1000)      156 2024-03-08 10:22:13.000000 plpygis-0.2.2/plpygis/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)       22 2024-03-08 11:06:44.000000 plpygis-0.2.2/plpygis/_version.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1233 2024-03-08 10:22:13.000000 plpygis-0.2.2/plpygis/exceptions.py
--rw-r--r--   0 ben       (1000) ben       (1000)    31041 2024-03-08 11:02:23.000000 plpygis-0.2.2/plpygis/geometry.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2676 2024-03-08 10:22:13.000000 plpygis-0.2.2/plpygis/hex.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-03-08 11:07:36.450701 plpygis-0.2.2/plpygis.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)     2335 2024-03-08 11:07:36.000000 plpygis-0.2.2/plpygis.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)      701 2024-03-08 11:07:36.000000 plpygis-0.2.2/plpygis.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        1 2024-03-08 11:07:36.000000 plpygis-0.2.2/plpygis.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       34 2024-03-08 11:07:36.000000 plpygis-0.2.2/plpygis.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        8 2024-03-08 11:07:36.000000 plpygis-0.2.2/plpygis.egg-info/top_level.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       28 2024-03-08 10:22:13.000000 plpygis-0.2.2/requirements-test.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       32 2024-03-08 11:03:58.000000 plpygis-0.2.2/requirements.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       38 2024-03-08 11:07:36.454035 plpygis-0.2.2/setup.cfg
--rw-r--r--   0 ben       (1000) ben       (1000)      750 2024-03-08 11:04:02.000000 plpygis-0.2.2/setup.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-03-08 11:07:36.450701 plpygis-0.2.2/test/
--rw-r--r--   0 ben       (1000) ben       (1000)       23 2024-03-08 10:22:13.000000 plpygis-0.2.2/test/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)       56 2024-03-08 10:22:13.000000 plpygis-0.2.2/test/__main__.py
--rw-r--r--   0 ben       (1000) ben       (1000)      180 2024-03-08 10:22:13.000000 plpygis-0.2.2/test/multipoint.shp
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-03-08 11:07:36.450701 plpygis-0.2.2/test/plpygis/
--rw-r--r--   0 ben       (1000) ben       (1000)      252 2024-03-08 10:22:13.000000 plpygis-0.2.2/test/plpygis/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)    21966 2024-03-08 10:22:13.000000 plpygis-0.2.2/test/plpygis/geometry.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.497663 plpygis-0.3.0/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.490996 plpygis-0.3.0/.github/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.490996 plpygis-0.3.0/.github/workflows/
+-rw-r--r--   0 ben       (1000) ben       (1000)      606 2024-03-08 17:37:46.000000 plpygis-0.3.0/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     1172 2024-03-08 10:22:13.000000 plpygis-0.3.0/.gitignore
+-rw-r--r--   0 ben       (1000) ben       (1000)      828 2024-04-08 19:20:38.000000 plpygis-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 ben       (1000) ben       (1000)     1107 2024-04-08 19:23:50.000000 plpygis-0.3.0/CHANGELOG.md
+-rw-r--r--   0 ben       (1000) ben       (1000)    35142 2024-03-08 10:22:13.000000 plpygis-0.3.0/LICENSE
+-rw-r--r--   0 ben       (1000) ben       (1000)      102 2024-03-08 10:22:13.000000 plpygis-0.3.0/MANIFEST.in
+-rw-r--r--   0 ben       (1000) ben       (1000)      203 2024-03-08 10:22:13.000000 plpygis-0.3.0/Makefile
+-rw-r--r--   0 ben       (1000) ben       (1000)     2335 2024-04-08 19:26:07.494330 plpygis-0.3.0/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)     1860 2024-03-08 10:22:13.000000 plpygis-0.3.0/README.rst
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.490996 plpygis-0.3.0/doc/
+-rw-r--r--   0 ben       (1000) ben       (1000)      610 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/Makefile
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.494330 plpygis-0.3.0/doc/source/
+-rw-r--r--   0 ben       (1000) ben       (1000)     4903 2024-04-08 19:14:37.000000 plpygis-0.3.0/doc/source/conf.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     8289 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/source/examples.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)      678 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/source/index.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)     1395 2024-04-03 07:00:40.000000 plpygis-0.3.0/doc/source/installation.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)      240 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/source/plpygis.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)     9484 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/source/plpython.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)     8671 2024-04-08 19:14:37.000000 plpygis-0.3.0/doc/source/subclasses.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)     3918 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/source/usage.rst
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.494330 plpygis-0.3.0/plpygis/
+-rw-r--r--   0 ben       (1000) ben       (1000)      156 2024-03-08 10:22:13.000000 plpygis-0.3.0/plpygis/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)       22 2024-04-08 19:14:37.000000 plpygis-0.3.0/plpygis/_version.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1233 2024-03-08 10:22:13.000000 plpygis-0.3.0/plpygis/exceptions.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    30983 2024-04-08 19:14:37.000000 plpygis-0.3.0/plpygis/geometry.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2676 2024-03-08 10:22:13.000000 plpygis-0.3.0/plpygis/hex.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.494330 plpygis-0.3.0/plpygis.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2335 2024-04-08 19:26:07.000000 plpygis-0.3.0/plpygis.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)      719 2024-04-08 19:26:07.000000 plpygis-0.3.0/plpygis.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2024-04-08 19:26:07.000000 plpygis-0.3.0/plpygis.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       34 2024-04-08 19:26:07.000000 plpygis-0.3.0/plpygis.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        8 2024-04-08 19:26:07.000000 plpygis-0.3.0/plpygis.egg-info/top_level.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       28 2024-03-08 11:17:40.000000 plpygis-0.3.0/requirements-test.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       32 2024-03-08 11:03:58.000000 plpygis-0.3.0/requirements.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       38 2024-04-08 19:26:07.497663 plpygis-0.3.0/setup.cfg
+-rw-r--r--   0 ben       (1000) ben       (1000)      750 2024-03-08 11:04:02.000000 plpygis-0.3.0/setup.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.494330 plpygis-0.3.0/test/
+-rw-r--r--   0 ben       (1000) ben       (1000)       23 2024-03-08 10:22:13.000000 plpygis-0.3.0/test/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)       56 2024-03-08 10:22:13.000000 plpygis-0.3.0/test/__main__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      180 2024-03-08 10:22:13.000000 plpygis-0.3.0/test/multipoint.shp
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.494330 plpygis-0.3.0/test/plpygis/
+-rw-r--r--   0 ben       (1000) ben       (1000)      252 2024-03-08 10:22:13.000000 plpygis-0.3.0/test/plpygis/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    22629 2024-04-08 19:14:37.000000 plpygis-0.3.0/test/plpygis/geometry.py
```

### Comparing `plpygis-0.2.2/.github/workflows/pythonpackage.yml` & `plpygis-0.3.0/.github/workflows/pythonpackage.yml`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `plpygis-0.2.2/.gitignore` & `plpygis-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `plpygis-0.2.2/CHANGELOG.md` & `plpygis-0.3.0/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## [0.3.0] - 2024-04-08
+
+- fixed: prevent invalid EWKB creation for multigeometries with SRIDs
+
 ## [0.2.2] - 2024-03-08
 
 - changed: support Shapely 2.x
 - fixed: conform to SPDX licence standard
 
 ## [0.2.1] - 2023-03-11
 
@@ -17,12 +21,15 @@
 - removed: dependency on nose for testing
 
 ## [0.1.0] - 2018-02-14
 ## [0.0.3] - 2018-01-21
 ## [0.0.2] - 2017-08-06
 ## [0.0.1] - 2017-07-30
 
+[0.3.0]: https://github.com/bosth/plpygis/compare/v0.2.2...v0.3.0
+[0.2.2]: https://github.com/bosth/plpygis/compare/v0.2.1...v0.2.2
+[0.2.1]: https://github.com/bosth/plpygis/compare/v0.2.0...v0.2.1
 [0.2.0]: https://github.com/bosth/plpygis/compare/v0.1.0...v0.2.0
 [0.1.0]: https://github.com/bosth/plpygis/compare/v0.0.3...v0.1.0
 [0.0.3]: https://github.com/bosth/plpygis/compare/v0.0.2...v0.0.3
 [0.0.2]: https://github.com/bosth/plpygis/compare/v0.0.1...v0.0.2
 [0.0.1]: https://github.com/bosth/plpygis/releases/tag/v0.0.1
```

### Comparing `plpygis-0.2.2/LICENSE` & `plpygis-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plpygis-0.2.2/PKG-INFO` & `plpygis-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plpygis
-Version: 0.2.2
+Version: 0.3.0
 Summary: PostGIS Python tools
 Home-page: https://github.com/bosth/plpygis
 Author: Benjamin Trigona-Harany
 Author-email: plpygis@jaxartes.net
 License: GPL-3.0-only
 Keywords: gis geospatial postgis postgresql plpython
 Platform: any
```

### Comparing `plpygis-0.2.2/README.rst` & `plpygis-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `plpygis-0.2.2/doc/Makefile` & `plpygis-0.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `plpygis-0.2.2/doc/source/conf.py` & `plpygis-0.3.0/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -95,15 +95,15 @@
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = []
 
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'plpygisdoc'
```

### Comparing `plpygis-0.2.2/doc/source/examples.rst` & `plpygis-0.3.0/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `plpygis-0.2.2/doc/source/index.rst` & `plpygis-0.3.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `plpygis-0.2.2/doc/source/installation.rst` & `plpygis-0.3.0/doc/source/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Installation
 ============
 
 Requirements
 ------------
 
-``plpygis`` has no dependencies beyond an installation of Python 2.7.x or 3.6.x. Additionally, ``plpygis`` can use `Shapely <https://github.com/Toblerity/Shapely>`_ (version 1.6 or greater) if available. Without it, conversion to and from Shapely geometries will be impossible.
+``plpygis`` has no dependencies beyond an installation of Python 3 (Python 2 should also work). Additionally, ``plpygis`` can use `Shapely <https://github.com/Toblerity/Shapely>`_ (version 2.0 or greater) if available. Without it, conversion to and from Shapely geometries will be impossible.
 
 Python Package Index
 --------------------
 
 ``plpygis`` may be installed from PyPI.
 
 .. code-block:: console
```

### Comparing `plpygis-0.2.2/doc/source/plpython.rst` & `plpygis-0.3.0/doc/source/plpython.rst`

 * *Files identical despite different names*

### Comparing `plpygis-0.2.2/doc/source/subclasses.rst` & `plpygis-0.3.0/doc/source/subclasses.rst`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,27 @@
 
 An SRID may be added at creation time with an optional ``SRID`` parameter:
 
 .. code-block:: python
 
     >>> point = Point((0, 0), srid=4326)
 
-``plpygis`` will detect conflicts when multigeometries or collections are created with mixed SRIDs.
+When creating a multigeometry with an SRID, each geometry must have the same SRID or no SRID.
+
+.. code-block:: python
+
+    >>> p1 = Point((0, 0), srid=4326)
+    >>> p2 = Point((1, 1), srid=4326)
+    >>> mp = MultiPoint([p1, p2], srid=4326)
+
+    >>> p3 = Point((0, 0))
+    >>> p4 = Point((1, 1))
+    >>> mp = MultiPoint([p3, p4], srid=4326)
+
+``plpygis`` will not allow the creation of a multigeometry with no SRID if any of the geometries have one.
 
 .. warning::
 
     Changing the SRID of an instance that is part of another geometry (such as a :class:`Point <plpygis.geometry.Point>` that is a vertex in a :class:`LineString <plpygis.geometry.LineString>` or a vertex in the linear ring of a :class:`Polygon <plpygis.geometry.Polygon>`) will *not* be detected. When converted to a WKB or Shapely instance, only the SRID of the "parent" geometry will be used.
 
 Dimensionality
 --------------
```

### Comparing `plpygis-0.2.2/doc/source/usage.rst` & `plpygis-0.3.0/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `plpygis-0.2.2/plpygis/exceptions.py` & `plpygis-0.3.0/plpygis/exceptions.py`

 * *Files identical despite different names*

### Comparing `plpygis-0.2.2/plpygis/geometry.py` & `plpygis-0.3.0/plpygis/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,19 +378,19 @@
                 self._dimz = geometry.dimz
             elif self._dimz != geometry.dimz:
                 raise DimensionalityError("Mixed dimensionality in MultiGeometry")
             if self._dimm is None:
                 self._dimm = geometry.dimm
             elif self._dimm != geometry.dimm:
                 raise DimensionalityError("Mixed dimensionality in MultiGeometry")
-            if self.srid is None:
-                if geometry._srid is not None:
-                    self._srid = geometry.srid
-            elif self.srid != geometry.srid and geometry.srid is not None:
-                raise SridError("Mixed SRIDs in MultiGeometry")
+            if geometry._srid is not None:
+                if self._srid != geometry._srid:
+                    raise SridError("Geometry can not be different from SRID in MultiGeometry")
+                else:
+                    geometry._srid = None
 
     def _to_geojson_coordinates(self, dimz):
         coordinates = [g._to_geojson_coordinates(dimz=dimz) for g in self.geometries]
         return coordinates
 
     @staticmethod
     def _read_wkb(reader, dimz, dimm):
@@ -863,15 +863,16 @@
     objects.
 
         >>> p1 = Point((0, 0, 0))
         >>> p2 = Point((1, 1, 0))
         >>> MultiPoint([p1, p2])
         <MultiPoint: 'geometry(MultiPointZ)'>
 
-    The dimensionality of all geometries in the collection must be identical.
+    The SRID and dimensionality of all geometries in the collection must be
+    identical.
     """
 
     _LWGEOMTYPE = 4
     __slots__ = ["_points"]
 
     def __init__(self, points=None, srid=None):
         if self._wkb:
@@ -908,15 +909,16 @@
     ``LineString`` objects.
 
         >>> l1 = LineString([(1, 1, 0), (2, 2, 0)], dimm=True)
         >>> l2 = LineString([(0, 0, 0), (0, 1, 0)], dimm=True)
         >>> MultiLineString([l1, l2])
         <MultiLineString: 'geometry(MultiLineStringM)'>
 
-    The dimensionality of all geometries in the collection must be identical.
+    The SRID and dimensionality of all geometries in the collection must be
+    identical.
     """
 
     _LWGEOMTYPE = 5
     __slots__ = ["_linestrings"]
 
     def __init__(self, linestrings=None, srid=None):
         if self._wkb:
@@ -948,32 +950,31 @@
 class MultiPolygon(_MultiGeometry):
     """
     A representation of a PostGIS MultiPolygon.
 
     ``MultiPolygon`` objects can be created directly from a list of ``Polygon``
     objects.
 
-        >>> p1 = Polygon([[(0, 0), (1, 0), (1, 1), (0, 1), (0, 0)]], srid=4326)
-        >>> p2 = Polygon([[(2, 2), (3, 2), (3, 3), (2, 3), (2, 2)]], srid=4326)
-        >>> MultiPolygon([p1, p2])
+        >>> p1 = Polygon([[(0, 0), (1, 0), (1, 1), (0, 1), (0, 0)]])
+        >>> p2 = Polygon([[(2, 2), (3, 2), (3, 3), (2, 3), (2, 2)]])
+        >>> MultiPolygon([p1, p2], srid=4326)
         <MultiPolygon: 'geometry(MultiPolygon,4326)'>
 
-    The dimensionality of all geometries in the collection must be identical.
+    The SRID and dimensionality of all geometries in the collection must be
+    identical.
     """
 
     _LWGEOMTYPE = 6
     __slots__ = ["__polygons__"]
 
-    def __init__(self, polygons=None, srid=None, dimz=False, dimm=False):
+    def __init__(self, polygons=None, srid=None):
         if self._wkb:
             self._polygons = None
         else:
             self._srid = srid
-            self._dimz = dimz
-            self._dimm = dimm
             self._polygons = polygons
             self._set_multi_metadata()
 
     @property
     def polygons(self):
         """
         List of all component polygons.
@@ -1000,15 +1001,16 @@
     geometries, including other collections.
 
         >>> p = Point((0, 0, 0))
         >>> l = LineString([(1, 1, 0), (2, 2, 0)])
         >>> GeometryCollection([p, l])
         <GeometryCollection: 'geometry(GeometryCollectionZ)'>
 
-    The dimensionality of all geometries in the collection must be identical.
+    The SRID and dimensionality of all geometries in the collection must be
+    identical.
     """
 
     _LWGEOMTYPE = 7
     __slots__ = ["_geometries"]
 
     def __init__(self, geometries=None, srid=None, dimz=False, dimm=False):
         if self._wkb:
```

### Comparing `plpygis-0.2.2/plpygis/hex.py` & `plpygis-0.3.0/plpygis/hex.py`

 * *Files identical despite different names*

### Comparing `plpygis-0.2.2/plpygis.egg-info/PKG-INFO` & `plpygis-0.3.0/plpygis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plpygis
-Version: 0.2.2
+Version: 0.3.0
 Summary: PostGIS Python tools
 Home-page: https://github.com/bosth/plpygis
 Author: Benjamin Trigona-Harany
 Author-email: plpygis@jaxartes.net
 License: GPL-3.0-only
 Keywords: gis geospatial postgis postgresql plpython
 Platform: any
```

### Comparing `plpygis-0.2.2/plpygis.egg-info/SOURCES.txt` & `plpygis-0.3.0/plpygis.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.readthedocs.yaml
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 requirements-test.txt
 requirements.txt
```

### Comparing `plpygis-0.2.2/setup.py` & `plpygis-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `plpygis-0.2.2/test/plpygis/geometry.py` & `plpygis-0.3.0/test/plpygis/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 geojson_gc = {"type":"GeometryCollection","geometries":[{"type":"Point","coordinates":[10,0]},{"type":"LineString","coordinates":[[11,0],[12,1]]}]}
 wkb_ln = "0102000000050000000000000040BE40409D640199EB373F400000000080AC3E40BF244710FD1939400000000000503940D2A6484BEB41374000000000801D3740248729C89C832A400000000000833340940338EFAFBB2C40"
 wkb_pg = "010300000002000000060000000000000000003440000000000080414000000000000024400000000000003E40000000000000244000000000000024400000000000003E4000000000000014400000000000804640000000000000344000000000000034400000000000804140040000000000000000003E40000000000000344000000000000034400000000000002E40000000000000344000000000000039400000000000003E400000000000003440"
 wkb_mpt = "010400008002000000010100008000000000000059400000000000006940000000000000000001010000800000000000000000000000000000F03F0000000000000000"
 wkb_mln = "010500004002000000010200004002000000000000000000000000000000000000000000000000004940000000000000F03F000000000000F03F0000000000003940010200004002000000000000000000F0BF000000000000F0BF000000000000F03F2DB29DEFA7C60140ED0DBE3099AA0A400000000000388F40"
 wkb_mpg = "01060000000200000001030000000100000004000000000000000000444000000000000044400000000000003440000000000080464000000000008046400000000000003E4000000000000044400000000000004440010300000002000000060000000000000000003440000000000080414000000000000024400000000000003E40000000000000244000000000000024400000000000003E4000000000000014400000000000804640000000000000344000000000000034400000000000804140040000000000000000003E40000000000000344000000000000034400000000000002E40000000000000344000000000000039400000000000003E400000000000003440"
 wkb_gc = "0107000000020000000101000000000000000000000000000000000000000102000000020000000000000000000000000000000000F03F000000000000F03F000000000000F03F"
+wkb_mpt_srid = "0104000020e8030000020000000101000000000000000000000000000000000000000101000000000000000000f03f000000000000f03f"
 
 class GeometryTestCase(unittest.TestCase):
     def test_missing_ewkb(self):
         """
         missing EWKB
         """
         self.assertRaises(WkbError, Geometry, None, None)
@@ -255,14 +256,29 @@
         geom.dimz = True
         geom.dimm = True
         self.assertEqual(geom.dimz, True)
         self.assertEqual(geom.dimm, True)
         geom.srid = geom.srid # clear cached WKB
         self.assertNotEqual(geom.__str__().lower(), wkb.lower())
 
+    def test_multigeometry_srid(self):
+        p1 = Point((0, 0), srid=1000)
+        p2 = Point((1, 1), srid=1000)
+        mp = MultiPoint([p1, p2], srid=1000)
+        self.assertEqual(mp.wkb, wkb_mpt_srid)
+
+    def test_multigeometry_srid_exception(self):
+        p1 = Point((0, 0), srid=1000)
+        p2 = Point((1, 1), srid=1000)
+        self.assertRaises(SridError, MultiPoint, [p1, p2])
+
+        p1 = Point((0, 0), srid=1000)
+        p2 = Point((1, 1), srid=1000)
+        self.assertRaises(SridError, MultiPoint, [p1, p2], 4326)
+
     def test_translate_geojson_pt(self):
         """
         load and dump GeoJSON point
         """
         geom = Geometry.from_geojson(geojson_pt)
         self.assertEqual(geom.srid, 4326)
         self.assertEqual(Point, type(geom))
```

