# Comparing `tmp/setuptools-git-versioning-1.9.2.tar.gz` & `tmp/setuptools-git-versioning-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-git-versioning-1.9.2.tar", last modified: Mon Mar 21 15:50:20 2022, max compression
+gzip compressed data, was "setuptools-git-versioning-2.0.0.tar", last modified: Mon Apr  8 20:15:10 2024, max compression
```

## Comparing `setuptools-git-versioning-1.9.2.tar` & `setuptools-git-versioning-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:50:20.456611 setuptools-git-versioning-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4627 2022-03-21 15:50:20.456611 setuptools-git-versioning-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3367 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-03-21 15:50:20.460611 setuptools-git-versioning-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2485 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:50:20.456611 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4627 2022-03-21 15:50:19.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-03-21 15:50:20.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 15:50:19.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-03-21 15:50:19.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 15:50:19.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-21 15:50:19.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-03-21 15:50:20.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13105 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:15:10.953364 setuptools-git-versioning-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-08 20:15:00.000000 setuptools-git-versioning-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 20:15:00.000000 setuptools-git-versioning-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-08 20:15:10.953364 setuptools-git-versioning-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-08 20:15:00.000000 setuptools-git-versioning-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-08 20:15:00.000000 setuptools-git-versioning-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-08 20:15:10.953364 setuptools-git-versioning-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-08 20:15:10.000000 setuptools-git-versioning-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:15:10.953364 setuptools-git-versioning-2.0.0/setuptools_git_versioning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-08 20:15:10.000000 setuptools-git-versioning-2.0.0/setuptools_git_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-08 20:15:10.000000 setuptools-git-versioning-2.0.0/setuptools_git_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:15:10.000000 setuptools-git-versioning-2.0.0/setuptools_git_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 20:15:10.000000 setuptools-git-versioning-2.0.0/setuptools_git_versioning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:15:10.000000 setuptools-git-versioning-2.0.0/setuptools_git_versioning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 20:15:10.000000 setuptools-git-versioning-2.0.0/setuptools_git_versioning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 20:15:10.000000 setuptools-git-versioning-2.0.0/setuptools_git_versioning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23356 2024-04-08 20:15:00.000000 setuptools-git-versioning-2.0.0/setuptools_git_versioning.py
```

### Comparing `setuptools-git-versioning-1.9.2/LICENSE` & `setuptools-git-versioning-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-git-versioning-1.9.2/PKG-INFO` & `setuptools-git-versioning-2.0.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: setuptools-git-versioning
-Version: 1.9.2
-Summary: Use git repo data for building a version number according PEP-440
-Home-page: https://setuptools-git-versioning.readthedocs.io
-Author: dolfinus
-Author-email: martinov.m.s.8@gmail.com
-License: MIT
-Project-URL: Documentation, https://setuptools-git-versioning.readthedocs.io
-Project-URL: Source, https://github.com/dolfinus/setuptools-git-versioning
-Project-URL: CI/CD, https://github.com/dolfinus/setuptools-git-versioning/actions
-Project-URL: Coverage, https://app.codecov.io/gh/dolfinus/setuptools-git-versioning
-Project-URL: Tracker, https://github.com/dolfinus/setuptools-git-versioning/issues
-Keywords: setuptools git version-control
-Platform: UNKNOWN
-Classifier: Framework :: Setuptools Plugin
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 *************************
 setuptools-git-versioning
 *************************
 
 |status| |PyPI| |PyPI License| |PyPI Python Version|
 |ReadTheDocs| |Build| |Coverage| |pre-commit.ci|
 
@@ -64,25 +36,27 @@
 
 - Templates for *tag*, *dev* and *dirty* versions are separated
 
 - Templates support a lot of substitutions including git and environment information
 
 - Well-documented
 
-
-See `difference <https://setuptools-git-versioning.readthedocs.io/en/latest/differences.html>`_
+See `comparison <https://setuptools-git-versioning.readthedocs.io/en/stable/comparison.html>`_
 between ``setuptools-git-versioning`` and other tools.
 
 **Limitations:**
 
 - Currently the only supported VCS is *Git*
 
-- Only git v2 is supported
+- Only Git v2 is supported
 
-- Currently does not support exporting version to file for runtime use
+- Only Setuptools build backend is supported (no Poetry & others)
+
+- Currently does not support automatic exporting of package version to a file for runtime use
+  (but you can use ``setuptools-git-versioning > file`` redirect instead)
 
 .. documentation
 
 Documentation
 --------------
 
 See https://setuptools-git-versioning.readthedocs.io/en/stable/
@@ -98,36 +72,69 @@
 
 Install
 ------------
 
 ``pyproject.toml``
 ~~~~~~~~~~~~~~~~~~
 
-Just add ``setuptools-git-versioning`` to ``build-sytem`` part of your ``pyproject.toml``
+Just add ``setuptools-git-versioning`` to ``build-sytem`` section of your ``pyproject.toml``,
+add a section ``tool.setuptools-git-versioning`` with config options, and mark the project
+``version`` as dynamic.
 
 .. code:: toml
 
     [build-system]
-    requires = [ "setuptools>=41", "wheel", "setuptools-git-versioning", ]
+    requires = [ "setuptools>=41", "wheel", "setuptools-git-versioning>=2.0,<3", ]
     build-backend = "setuptools.build_meta"
 
     [tool.setuptools-git-versioning]
     enabled = true
 
+    [project]
+    dynamic = ["version"]
+
+And check the package version generated (see `command help <https://setuptools-git-versioning.readthedocs.io/en/stable/command.html>`_):
+
+.. code:: bash
+
+    $ python -m setuptools_git_versioning
+    0.0.1
+
+    # or
+
+    $ setuptools-git-versioning
+    0.0.1
+
 ``setup.py``
-~~~~~~~~~~~~~~
+~~~~~~~~~~~~
 
-Just add ``setuptools-git-versioning`` to ``setup_requires`` part of your ``setup.py``
+Just add ``setuptools-git-versioning`` to ``setup_requires`` argument of ``setuptools.setup`` function call,
+and then add new argument ``setuptools_git_versioning`` with config options:
 
 .. code:: python
 
     import setuptools
 
     setuptools.setup(
         ...,
         setuptools_git_versioning={
             "enabled": True,
         },
-        setup_requires=["setuptools-git-versioning"],
+        setup_requires=["setuptools-git-versioning>=2.0,<3"],
     )
 
+And check the package version generated (see `command help <https://setuptools-git-versioning.readthedocs.io/en/stable/command.html>`_):
+
+.. code:: bash
+
+    $ python setup.py --version
+    0.0.1
+
+    # or
+
+    $ python -m setuptools_git_versioning
+    0.0.1
+
+    # or
 
+    $ setuptools-git-versioning
+    0.0.1
```

### Comparing `setuptools-git-versioning-1.9.2/setup.py` & `setuptools-git-versioning-2.0.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,48 @@
-import os
-from setuptools import setup, find_packages
-from setuptools_git_versioning import version_from_git
+from __future__ import annotations
 
-HERE = os.path.dirname(os.path.abspath(__file__))
+from pathlib import Path
 
+from setuptools import find_packages, setup
 
-def parse_requirements(file_content):
-    lines = file_content.splitlines()
-    return [line.strip() for line in lines if line and not line.startswith("#")]
 
 
-with open(os.path.join(HERE, "README.rst")) as f:
-    long_description = f.read()
+def parse_requirements(file: Path) -> list[str]:
+    lines = file.read_text().splitlines()
+    return [line.rstrip() for line in lines if line and not line.startswith("#")]
 
-with open(os.path.join(HERE, "requirements.txt")) as f:
-    requirements = parse_requirements(f.read())
+
+here = Path(__file__).parent.resolve()
+requirements = parse_requirements(here / "requirements.txt")
+long_description = here.joinpath("README.rst").read_text()
 
 setup(
     name="setuptools-git-versioning",
-    version=version_from_git(),
+    # +local version is not allowed in PyPI
+    # https://github.com/pypa/pypi-legacy/issues/731#issuecomment-345461596
+    version='2.0.0',
     author="dolfinus",
     author_email="martinov.m.s.8@gmail.com",
     description="Use git repo data for building a version number according PEP-440",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://setuptools-git-versioning.readthedocs.io",
-    keywords="setuptools git version-control",
+    keywords=["setuptools", "git", "versioning", "pep-440"],
     packages=find_packages(exclude=["docs", "tests", "docs.*", "tests.*"]),
     classifiers=[
         "Framework :: Setuptools Plugin",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     project_urls={
         "Documentation": "https://setuptools-git-versioning.readthedocs.io",
         "Source": "https://github.com/dolfinus/setuptools-git-versioning",
         "CI/CD": "https://github.com/dolfinus/setuptools-git-versioning/actions",
@@ -48,17 +51,17 @@
     },
     python_requires=">=3.7",
     py_modules=["setuptools_git_versioning"],
     install_requires=requirements,
     setup_requires=requirements,
     entry_points={
         "distutils.setup_keywords": [
-            "version_config = setuptools_git_versioning:parse_config",
             "setuptools_git_versioning = setuptools_git_versioning:parse_config",
         ],
         "setuptools.finalize_distribution_options": [
             "setuptools_git_versioning = setuptools_git_versioning:infer_version",
         ],
+        "console_scripts": ["setuptools-git-versioning=setuptools_git_versioning:__main__"],
     },
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/PKG-INFO` & `setuptools-git-versioning-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: setuptools-git-versioning
-Version: 1.9.2
+Version: 2.0.0
 Summary: Use git repo data for building a version number according PEP-440
 Home-page: https://setuptools-git-versioning.readthedocs.io
 Author: dolfinus
 Author-email: martinov.m.s.8@gmail.com
 License: MIT
 Project-URL: Documentation, https://setuptools-git-versioning.readthedocs.io
 Project-URL: Source, https://github.com/dolfinus/setuptools-git-versioning
 Project-URL: CI/CD, https://github.com/dolfinus/setuptools-git-versioning/actions
 Project-URL: Coverage, https://app.codecov.io/gh/dolfinus/setuptools-git-versioning
 Project-URL: Tracker, https://github.com/dolfinus/setuptools-git-versioning/issues
-Keywords: setuptools git version-control
-Platform: UNKNOWN
+Keywords: setuptools,git,versioning,pep-440
 Classifier: Framework :: Setuptools Plugin
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: packaging
+Requires-Dist: setuptools
+Requires-Dist: toml>=0.10.2; python_version < "3.11"
 
 *************************
 setuptools-git-versioning
 *************************
 
 |status| |PyPI| |PyPI License| |PyPI Python Version|
 |ReadTheDocs| |Build| |Coverage| |pre-commit.ci|
@@ -64,25 +68,27 @@
 
 - Templates for *tag*, *dev* and *dirty* versions are separated
 
 - Templates support a lot of substitutions including git and environment information
 
 - Well-documented
 
-
-See `difference <https://setuptools-git-versioning.readthedocs.io/en/latest/differences.html>`_
+See `comparison <https://setuptools-git-versioning.readthedocs.io/en/stable/comparison.html>`_
 between ``setuptools-git-versioning`` and other tools.
 
 **Limitations:**
 
 - Currently the only supported VCS is *Git*
 
-- Only git v2 is supported
+- Only Git v2 is supported
+
+- Only Setuptools build backend is supported (no Poetry & others)
 
-- Currently does not support exporting version to file for runtime use
+- Currently does not support automatic exporting of package version to a file for runtime use
+  (but you can use ``setuptools-git-versioning > file`` redirect instead)
 
 .. documentation
 
 Documentation
 --------------
 
 See https://setuptools-git-versioning.readthedocs.io/en/stable/
@@ -98,36 +104,69 @@
 
 Install
 ------------
 
 ``pyproject.toml``
 ~~~~~~~~~~~~~~~~~~
 
-Just add ``setuptools-git-versioning`` to ``build-sytem`` part of your ``pyproject.toml``
+Just add ``setuptools-git-versioning`` to ``build-sytem`` section of your ``pyproject.toml``,
+add a section ``tool.setuptools-git-versioning`` with config options, and mark the project
+``version`` as dynamic.
 
 .. code:: toml
 
     [build-system]
-    requires = [ "setuptools>=41", "wheel", "setuptools-git-versioning", ]
+    requires = [ "setuptools>=41", "wheel", "setuptools-git-versioning>=2.0,<3", ]
     build-backend = "setuptools.build_meta"
 
     [tool.setuptools-git-versioning]
     enabled = true
 
+    [project]
+    dynamic = ["version"]
+
+And check the package version generated (see `command help <https://setuptools-git-versioning.readthedocs.io/en/stable/command.html>`_):
+
+.. code:: bash
+
+    $ python -m setuptools_git_versioning
+    0.0.1
+
+    # or
+
+    $ setuptools-git-versioning
+    0.0.1
+
 ``setup.py``
-~~~~~~~~~~~~~~
+~~~~~~~~~~~~
 
-Just add ``setuptools-git-versioning`` to ``setup_requires`` part of your ``setup.py``
+Just add ``setuptools-git-versioning`` to ``setup_requires`` argument of ``setuptools.setup`` function call,
+and then add new argument ``setuptools_git_versioning`` with config options:
 
 .. code:: python
 
     import setuptools
 
     setuptools.setup(
         ...,
         setuptools_git_versioning={
             "enabled": True,
         },
-        setup_requires=["setuptools-git-versioning"],
+        setup_requires=["setuptools-git-versioning>=2.0,<3"],
     )
 
+And check the package version generated (see `command help <https://setuptools-git-versioning.readthedocs.io/en/stable/command.html>`_):
+
+.. code:: bash
+
+    $ python setup.py --version
+    0.0.1
+
+    # or
+
+    $ python -m setuptools_git_versioning
+    0.0.1
+
+    # or
 
+    $ setuptools-git-versioning
+    0.0.1
```

