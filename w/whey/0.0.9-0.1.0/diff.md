# Comparing `tmp/whey-0.0.9.tar.gz` & `tmp/whey-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whey-0.0.9.tar", last modified: Tue Apr  6 09:47:08 2021, max compression
+gzip compressed data, was "whey-0.1.0.tar", last modified: Mon Apr  8 21:45:33 2024, max compression
```

## Comparing `whey-0.0.9.tar` & `whey-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 09:47:08.739432 whey-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-04-06 09:46:38.000000 whey-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-04-06 09:46:38.000000 whey-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8410 2021-04-06 09:47:08.739432 whey-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5570 2021-04-06 09:46:38.000000 whey-0.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      788 2021-04-06 09:46:38.000000 whey-0.0.9/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2021-04-06 09:46:38.000000 whey-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-04-06 09:46:38.000000 whey-0.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1717 2021-04-06 09:47:08.739432 whey-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      655 2021-04-06 09:46:38.000000 whey-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 09:47:08.735432 whey-0.0.9/whey/
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2021-04-06 09:46:38.000000 whey-0.0.9/whey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3358 2021-04-06 09:46:38.000000 whey-0.0.9/whey/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21561 2021-04-06 09:46:38.000000 whey-0.0.9/whey/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 09:47:08.739432 whey-0.0.9/whey/config/
--rw-r--r--   0 runner    (1001) docker     (121)     3497 2021-04-06 09:46:38.000000 whey-0.0.9/whey/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17073 2021-04-06 09:46:38.000000 whey-0.0.9/whey/config/pep621.py
--rw-r--r--   0 runner    (1001) docker     (121)    12588 2021-04-06 09:46:38.000000 whey-0.0.9/whey/config/whey.py
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2021-04-06 09:46:38.000000 whey-0.0.9/whey/foreman.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-06 09:46:38.000000 whey-0.0.9/whey/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 09:47:08.739432 whey-0.0.9/whey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8410 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      439 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      244 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:33.356426 whey-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 21:45:04.000000 whey-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 21:45:04.000000 whey-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-08 21:45:33.356426 whey-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-08 21:45:04.000000 whey-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 21:45:04.000000 whey-0.1.0/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-08 21:45:04.000000 whey-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 21:45:04.000000 whey-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-08 21:45:33.356426 whey-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-08 21:45:04.000000 whey-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:33.352426 whey-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    43090 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_builder_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21136 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28981 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_foreman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_pep517_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:33.352426 whey-0.1.0/whey/
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-08 21:45:04.000000 whey-0.1.0/whey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-08 21:45:04.000000 whey-0.1.0/whey/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-08 21:45:04.000000 whey-0.1.0/whey/_editable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-08 21:45:04.000000 whey-0.1.0/whey/additional_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27105 2024-04-08 21:45:04.000000 whey-0.1.0/whey/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:33.356426 whey-0.1.0/whey/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-08 21:45:04.000000 whey-0.1.0/whey/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-08 21:45:04.000000 whey-0.1.0/whey/config/pep621.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12864 2024-04-08 21:45:04.000000 whey-0.1.0/whey/config/whey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-08 21:45:04.000000 whey-0.1.0/whey/foreman.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:04.000000 whey-0.1.0/whey/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-08 21:45:04.000000 whey-0.1.0/whey/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:33.356426 whey-0.1.0/whey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/top_level.txt
```

### Comparing `whey-0.0.9/LICENSE` & `whey-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whey-0.0.9/README.rst` & `whey-0.1.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 * handles type hint files
   (`py.typed <https://www.python.org/dev/peps/pep-0561/>`_ and ``*.pyi`` stubs).
 * is distributed under the `MIT License <https://choosealicense.com/licenses/mit/>`_.
 * `is the liquid remaining after milk has been curdled and strained <https://en.wikipedia.org/wiki/Whey>`_.
   It is a byproduct of the manufacture of cheese and has several commercial uses.
 
 
+See `the documentation`_ for configuration_ and usage_ information.
+
+.. _the documentation: https://whey.readthedocs.io/en/latest/
+.. _configuration: https://whey.readthedocs.io/en/latest/configuration.html
+.. _usage: https://whey.readthedocs.io/en/latest/configuration.html
+
 .. start shields
 
 .. list-table::
 	:stub-columns: 1
 	:widths: 10 90
 
 	* - Docs
@@ -66,16 +72,16 @@
 	:target: https://github.com/repo-helper/whey/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/whey/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/whey/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://requires.io/github/repo-helper/whey/requirements.svg?branch=master
-	:target: https://requires.io/github/repo-helper/whey/requirements/?branch=master
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/whey/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/whey/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/whey/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/whey?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/whey?logo=codefactor
@@ -94,38 +100,38 @@
 	:target: https://pypi.org/project/whey/
 	:alt: PyPI - Supported Implementations
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/whey
 	:target: https://pypi.org/project/whey/
 	:alt: PyPI - Wheel
 
-.. |conda-version| image:: https://img.shields.io/conda/v/domdfcoding/whey?logo=anaconda
-	:target: https://anaconda.org/domdfcoding/whey
+.. |conda-version| image:: https://img.shields.io/conda/v/conda-forge/whey?logo=anaconda
+	:target: https://anaconda.org/conda-forge/whey
 	:alt: Conda - Package Version
 
-.. |conda-platform| image:: https://img.shields.io/conda/pn/domdfcoding/whey?label=conda%7Cplatform
-	:target: https://anaconda.org/domdfcoding/whey
+.. |conda-platform| image:: https://img.shields.io/conda/pn/conda-forge/whey?label=conda%7Cplatform
+	:target: https://anaconda.org/conda-forge/whey
 	:alt: Conda - Platform
 
 .. |license| image:: https://img.shields.io/github/license/repo-helper/whey
 	:target: https://github.com/repo-helper/whey/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/whey
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.0.9
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.1.0
 	:target: https://github.com/repo-helper/whey/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/whey
 	:target: https://github.com/repo-helper/whey/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2021
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/whey
 	:target: https://pypi.org/project/whey/
 	:alt: PyPI - Downloads
 
 .. end shields
@@ -141,21 +147,27 @@
 
 .. code-block:: bash
 
 	$ python -m pip install whey
 
 To install with ``conda``:
 
-	* First add the required channels
+.. code-block:: bash
+
+	$ conda install -c conda-forge whey
 
-	.. code-block:: bash
+.. end installation
+
+``whey`` also has an optional README validation feature, which checks the README will render correctly on PyPI.
+This requires that the ``readme`` extra is installed:
 
-		$ conda config --add channels http://conda.anaconda.org/conda-forge
-		$ conda config --add channels http://conda.anaconda.org/domdfcoding
+.. code-block:: bash
 
-	* Then install
+	$ python -m pip install whey[readme]
 
-	.. code-block:: bash
+and in ``pyproject.toml``:
 
-		$ conda install whey
+.. code-block:: TOML
 
-.. end installation
+	[build-system]
+	requires = [ "whey[readme]",]
+	build-backend = "whey"
```

### Comparing `whey-0.0.9/setup.py` & `whey-0.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 repo_root = pathlib.Path(__file__).parent
 install_requires = (repo_root / "requirements.txt").read_text(encoding="UTF-8").split('\n')
 
 setup(
 		description="A simple Python wheel builder for simple projects.",
 		extras_require=extras_require,
 		install_requires=install_requires,
+		name="whey",
 		py_modules=[],
-		version=__version__,
 		)
 
 shutil.rmtree("whey.egg-info", ignore_errors=True)
```

### Comparing `whey-0.0.9/whey/builder.py` & `whey-0.1.0/whey/builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,42 +23,47 @@
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
-import configparser
+import datetime
 import os
 import pathlib
-import posixpath
 import re
 import shutil
+import sys
 import tarfile
+import zipfile
 from abc import ABC, abstractmethod
 from email.headerregistry import Address
-from email.message import EmailMessage
 from functools import partial
-from io import StringIO
-from typing import Any, Dict, Iterator, Mapping, Optional
-from zipfile import ZipFile
+from posixpath import join as posixpath_join
+from typing import TYPE_CHECKING, Any, Dict, Iterator, Mapping, Optional
+from warnings import warn as warnings_warn
 
 # 3rd party
 import click
 import dom_toml
-from consolekit.terminal_colours import Fore, resolve_color_default
+import handy_archives
+from consolekit.terminal_colours import ColourTrilean, Fore, resolve_color_default
+from dist_meta import entry_points, metadata, wheel
+from dist_meta.metadata_mapping import MetadataMapping
 from domdf_python_tools.paths import PathPlus, sort_paths, traverse_to_file
-from domdf_python_tools.stringlist import StringList
 from domdf_python_tools.typing import PathLike
 from domdf_python_tools.words import word_join
-from first import first
+from pyproject_parser import PyProjectTomlEncoder
 from shippinglabel.checksum import get_record_entry
 from shippinglabel.requirements import ComparableRequirement, combine_requirements
 
-__all__ = ["AbstractBuilder", "SDistBuilder", "WheelBuilder"]
+# this package
+from whey import additional_files
+
+__all__ = ("AbstractBuilder", "SDistBuilder", "WheelBuilder")
 
 archive_name_sub_re = re.compile(
 		r"[^\w\d.]+",
 		re.UNICODE,
 		)
 
 
@@ -66,35 +71,48 @@
 	"""
 	Abstract base class for builders of Python distributions using metadata read from ``pyproject.toml``.
 
 	:param project_dir: The project to build the distribution for.
 	:param build_dir: The (temporary) build directory.
 	:default build_dir: :file:`{<project_dir>}/build/`
 	:param out_dir: The output directory.
-	:default out_dir: :file:`{<project_dir>}/dist`
+	:default out_dir: :file:`{<project_dir>}/dist/`
 	:param verbose: Whether to enable verbose output.
 	:param colour: Whether to use coloured output.
+
+	.. autosummary-widths:: 1/2
+
+	.. autoclasssumm:: AbstractBuilder
+		:autosummary-sections: Attributes
+
+	.. latex:clearpage::
+
+	.. autosummary-widths:: 7/16
+
+	.. autoclasssumm:: AbstractBuilder
+		:autosummary-sections: Methods
 	"""
 
 	def __init__(
 			self,
 			project_dir: PathPlus,
 			config: Mapping[str, Any],
 			build_dir: Optional[PathLike] = None,
 			out_dir: Optional[PathLike] = None,
-			*,
+			*args,
 			verbose: bool = False,
-			colour: bool = None,
+			colour: ColourTrilean = None,
+			**kwargs,
 			):
 
 		# Walk up the tree until a "pyproject.toml" file is found.
 		#: The pyproject.toml directory
 		self.project_dir: PathPlus = traverse_to_file(PathPlus(project_dir), "pyproject.toml")
 
-		#: Configuration parsed from "pyproject.toml".
+		#: Configuration parsed from ``pyproject.toml``.
 		self.config: Dict[str, Any] = dict(config)
 
 		#: The archive name, without the tag
 		self.archive_name = archive_name_sub_re.sub(
 				'_',
 				self.config["name"],
 				) + f"-{self.config['version']}"
@@ -127,14 +145,22 @@
 	def default_out_dir(self) -> PathPlus:  # pragma: no cover
 		"""
 		Provides a default for the ``out_dir`` argument.
 		"""
 
 		return self.project_dir / "dist"
 
+	@property
+	def code_directory(self) -> str:
+		"""
+		The directory containing the code in the build directory.
+		"""
+
+		return self.config["source-dir"]
+
 	def clear_build_dir(self) -> None:
 		"""
 		Clear the build directory of any residue from previous builds.
 		"""
 
 		if self.build_dir.is_dir():
 			shutil.rmtree(self.build_dir)
@@ -145,15 +171,20 @@
 		"""
 		Iterate over the files in the source directory.
 		"""
 
 		pkgdir = self.project_dir / self.config["source-dir"] / self.config["package"]
 
 		if not pkgdir.is_dir():
-			raise FileNotFoundError(f"Package directory '{self.config['package']}' not found.")
+			message = f"Package directory {self.config['package']!r} not found"
+
+			if self.config["source-dir"]:
+				raise FileNotFoundError(f"{message} in {self.config['source-dir']!r}.")
+			else:
+				raise FileNotFoundError(f"{message}.")
 
 		found_file = False
 
 		for py_pattern in {"**/*.py", "**/*.pyi", "**/*.pyx", "**/py.typed"}:
 			for py_file in pkgdir.rglob(py_pattern):
 				if "__pycache__" not in py_file.parts:
 					found_file = True
@@ -164,109 +195,104 @@
 
 	def copy_source(self) -> None:
 		"""
 		Copy source files into the build directory.
 		"""
 
 		for py_file in self.iter_source_files():
-			target = self.build_dir / py_file.relative_to(self.project_dir / self.config["source-dir"])
+			target = self.build_dir / py_file.relative_to(self.project_dir / self.code_directory)
 			target.parent.maybe_make(parents=True)
 			target.write_clean(py_file.read_text())
+			shutil.copystat(py_file, target)  # pylint: disable=dotted-import-in-loop
 			self.report_copied(py_file, target)
 
+	def _echo_if_v(self, *args, **kwargs) -> None:
+		if self.verbose:
+			self._echo(*args, **kwargs)
+
 	def report_copied(self, source: pathlib.Path, target: pathlib.Path) -> None:
 		"""
 		Report that a file has been copied into the build directory.
 
 		The format is::
 
 			Copying {source} -> {target.relative_to(self.build_dir)}
 
+		.. latex:vspace:: -5px
+
 		:param source: The source file
 		:param target: The file in the build directory.
 		"""
 
-		if self.verbose:
-			self._echo(f"Copying {source.resolve().as_posix()} -> {target.relative_to(self.build_dir).as_posix()}")
+		self._echo_if_v(
+				f"Copying {source.resolve().as_posix()} -> {target.relative_to(self.build_dir).as_posix()}"
+				)
 
 	def report_removed(self, removed_file: pathlib.Path) -> None:
 		"""
-		Report that a file has been removed from the build directory.
+		Reports the removal of a file from the build directory.
 
 		The format is::
 
 			Removing {removed_file.relative_to(self.build_dir)}
 
+		.. latex:vspace:: -5px
+
 		:param removed_file:
 		"""
 
-		if self.verbose:
-			self._echo(f"Removing {removed_file.relative_to(self.build_dir).as_posix()}")
+		self._echo_if_v(f"Removing {removed_file.relative_to(self.build_dir).as_posix()}")
 
 	def report_written(self, written_file: pathlib.Path) -> None:
 		"""
 		Report that a file has been written to the build directory.
 
 		The format is::
 
 			Writing {written_file.relative_to(self.build_dir)}
 
+		.. latex:vspace:: -5px
+
 		:param written_file:
 		"""
 
-		if self.verbose:
-			self._echo(f"Writing {written_file.relative_to(self.build_dir).as_posix()}")
+		self._echo_if_v(f"Writing {written_file.relative_to(self.build_dir).as_posix()}")
 
-	def copy_additional_files(self) -> None:  # pylint: disable=useless-return
+	def copy_additional_files(self) -> None:
 		"""
 		Copy additional files to the build directory, as specified in the ``additional-files`` key.
 		"""
 
 		self.parse_additional_files(*self.config["additional-files"])
 
-	def parse_additional_files(self, *entries: str) -> None:  # pylint: disable=useless-return
+	def parse_additional_files(self, *entries: additional_files.AdditionalFilesEntry) -> None:  # pylint: disable=useless-return
 		r"""
-		Copy additional files to the build directory,
-		by parsing `MANIFEST.in <https://packaging.python.org/guides/using-manifest-in/>`_-style entries.
+		Copy additional files to the build directory, by parsing `MANIFEST.in`_-style entries.
+
+		.. _MANIFEST.in: https://packaging.python.org/guides/using-manifest-in/
 
 		:param \*entries:
-		"""  # noqa: D400
+		"""
 
-		def copy_file(filename):
-			target = self.build_dir / filename.relative_to(self.project_dir)
-			target.parent.maybe_make(parents=True)
-			shutil.copy2(src=filename, dst=target)
-			self.report_copied(filename, target)
+		# this package
+		from whey import additional_files
 
 		for entry in entries:
-			parts = entry.split(' ')
-
-			if parts[0] == "include":
-				for include_pat in parts[1:]:
-					for include_file in sorted(self.project_dir.glob(include_pat)):
-						if include_file.is_file():
-							copy_file(filename=include_file)
-
-			elif parts[0] == "exclude":
-				for exclude_pat in parts[1:]:
-					for exclude_file in sorted(self.build_dir.glob(exclude_pat)):
-						if exclude_file.is_file():
-							exclude_file.unlink()
-							self.report_removed(exclude_file)
-
-			elif parts[0] == "recursive-include":
-				for include_file in sort_paths(*(self.project_dir / parts[1]).rglob(parts[2])):
-					if include_file.is_file():
-						copy_file(filename=include_file)
-
-			elif parts[0] == "recursive-exclude":
-				for exclude_file in sort_paths(*(self.build_dir / parts[1]).rglob(parts[2])):
-					if exclude_file.is_file():
-						exclude_file.unlink()
-						self.report_removed(exclude_file)
+			if isinstance(entry, (additional_files.Include, additional_files.RecursiveInclude)):
+				for include_file in entry.iter_files(self.project_dir):
+					target = self.build_dir / include_file.relative_to(self.project_dir / self.code_directory)
+					target.parent.maybe_make(parents=True)
+					shutil.copy2(src=include_file, dst=target)
+					self.report_copied(include_file, target)
+			elif isinstance(entry, (additional_files.Exclude, additional_files.RecursiveExclude)):
+				for exclude_file in entry.iter_files(self.build_dir):
+					exclude_file.unlink()
+					self.report_removed(exclude_file)
+			else:  # pragma: no cover
+				warnings_warn(f"Unsupported command in 'additional-files': {entry}")
 
 		#
 		# elif parts[0] == "global-include":
 		# 	for include_pat in parts[1:]:
 		# 		for include_file in self.project_dir.rglob(include_pat):
 		# 			if include_file.is_file():
 		# 				copy_file(filename=include_file)
@@ -288,47 +314,40 @@
 		# elif parts[0] == "prune":
 		# 	for prune_dir in self.project_dir.rglob(parts[1]):
 		# 		for prune_file in prune_dir.rglob("*.*"):
 		# 			if prune_file.is_file():
 		# 				prune_file.unlink()
 		# 				self.report_removed(exclude_file)
 
+		# pylint: enable=loop-invariant-statement
 		return
 
-	def write_license(self, dest_dir: PathPlus):
+	def write_license(self, dest_dir: PathPlus, dest_filename: str = "LICENSE") -> None:
 		"""
 		Write the ``LICENSE`` file.
 
-		:param dest_dir: The directory to write the files into.
+		:param dest_dir: The directory to write the file into.
+		:param dest_filename: The name of the file to write in ``dest_dir``.
 		"""
 
-		if "license" in self.config:
-			target = dest_dir / "LICENSE"
+		if self.config.get("license", None) is not None:
+			target = dest_dir / dest_filename
 			target.parent.maybe_make(parents=True)
-			target.write_clean(self.config["license"])
+			target.write_clean(self.config["license"].text)
 			self.report_written(target)
 
-	def write_metadata(self, metadata_file: PathPlus):
+	def parse_authors(self) -> Dict[str, str]:
 		"""
-		Write `Core Metadata <https://packaging.python.org/specifications/core-metadata>`_
-		to the given file.
+		Parse the :tconf:`project.authors` and :tconf:`~project.maintainers` fields into :core-meta:`Author`,
+		:core-meta:`Maintainer-Email` etc.
 
-		:param metadata_file:
-		"""  # noqa: D400
-
-		metadata = EmailMessage()
+		:return: A mapping of field names to values.
 
-		# TODO: metadata 2.2
-		# Need to translate pep621 dynamic into core metadata field names
-		metadata["Metadata-Version"] = "2.1"
-		metadata["Name"] = self.config["name"]
-		metadata["Version"] = str(self.config["version"])
-
-		if self.config["description"] is not None:
-			metadata["Summary"] = self.config["description"]
+			Possible field names are ``Author``, ``Author-Email``, ``Maintainer``, and ``Maintainer-Email``.
+		"""  # noqa: D400
 
 		author = []
 		author_email = []
 		maintainer = []
 		maintainer_email = []
 
 		for entry in self.config["authors"]:
@@ -338,91 +357,132 @@
 			elif entry["email"]:
 				author_email.append(entry["email"])
 			elif entry["name"]:
 				author.append(entry["name"])
 
 		for entry in self.config["maintainers"]:
 			if entry["name"] and entry["email"]:
-				maintainer_email.append("{name} <{email}>".format_map(entry))
+				address = Address(entry["name"], addr_spec=entry["email"])
+				author_email.append(str(address))
 			elif entry["email"]:
 				maintainer_email.append(entry["email"])
 			elif entry["name"]:
 				maintainer.append(entry["name"])
 
 		# TODO: I'm not quite sure how PEP 621 expects a name for one author and the email for another to be handled.
 
+		output = {}
+
 		if author_email:
-			metadata["Author-email"] = ", ".join(author_email)
+			output["Author-email"] = ", ".join(author_email)
 		elif author:
-			metadata["Author"] = word_join(author)
+			output["Author"] = word_join(author)
 
 		if maintainer_email:
-			metadata["Author-email"] = ", ".join(maintainer_email)
+			output["Maintainer-email"] = ", ".join(maintainer_email)
 		elif maintainer:
-			metadata["Author"] = word_join(maintainer)
+			output["Maintainer"] = word_join(maintainer)
 
-		if self.config["license-key"] is not None:
-			metadata["License"] = self.config["license-key"]
+		return output
+
+	def get_metadata_map(self) -> MetadataMapping:
+		"""
+		Generate the content of the ``METADATA`` / ``PKG-INFO`` file.
+		"""
+
+		metadata_mapping = MetadataMapping()
+
+		metadata_mapping["Metadata-Version"] = "2.2"
+		metadata_mapping["Name"] = self.config["name"]
+		metadata_mapping["Version"] = str(self.config["version"])
+
+		def add_not_none(key: str, field: str) -> None:
+			if self.config[key] is not None:
+				metadata_mapping[field] = self.config[key]
+
+		def add_multiple(key: str, field: str) -> None:
+			for value in self.config[key]:
+				metadata_mapping[field] = str(value)  # pylint: disable=loop-invariant-statement
+
+		add_multiple("dynamic", "Dynamic")
+		metadata_mapping.update(self.parse_authors())
+
+		add_not_none("description", "Summary")
+		add_not_none("license-key", "License")
+
+		add_multiple("classifiers", "Classifier")
+		add_multiple("dependencies", "Requires-Dist")
 
 		if self.config["keywords"]:
-			metadata["Keywords"] = ','.join(self.config["keywords"])
+			metadata_mapping["Keywords"] = ','.join(self.config["keywords"])
 
+		seen_hp = False
+
+		# pylint: disable=loop-invariant-statement
 		for category, url in self.config["urls"].items():
-			if category.lower() in {"homepage", "home page"}:
-				metadata["Home-page"] = url
+			if category.lower() in {"homepage", "home page"} and not seen_hp:
+				metadata_mapping["Home-page"] = url
+				seen_hp = True
 			else:
-				metadata["Project-URL"] = f"{category}, {url}"
+				metadata_mapping["Project-URL"] = f"{category}, {url}"
 
 		for platform in (self.config.get("platforms", None) or ()):
-			metadata["Platform"] = platform
-
-		for classifier in self.config["classifiers"]:
-			metadata["Classifier"] = classifier
+			metadata_mapping["Platform"] = platform
 
 		if self.config["requires-python"]:
-			metadata["Requires-Python"] = str(self.config["requires-python"])
-
-		for requirement in self.config["dependencies"]:
-			metadata["Requires-Dist"] = str(requirement)
+			metadata_mapping["Requires-Python"] = str(self.config["requires-python"])
 
 		for extra, requirements in self.config["optional-dependencies"].items():
-			metadata["Provides-Extra"] = extra
+			metadata_mapping["Provides-Extra"] = extra
 			for requirement in requirements:
-				metadata["Requires-Dist"] = f"{requirement!s} ; extra == {extra!r}"
+				requirement = ComparableRequirement(str(requirement))
+
+				if requirement.marker:
+					requirement.marker = f"({requirement.marker!s}) and extra == {extra!r}"
+				else:
+					requirement.marker = f"extra == {extra!r}"
+
+				metadata_mapping["Requires-Dist"] = str(requirement)
+
+		# pylint: enable=loop-invariant-statement
 
 		# TODO:
 		#  https://packaging.python.org/specifications/core-metadata/#requires-external-multiple-use
 		#  https://packaging.python.org/specifications/core-metadata/#provides-dist-multiple-use
 		#  https://packaging.python.org/specifications/core-metadata/#obsoletes-dist-multiple-use
 
-		if self.config["readme"] is None:
-			description = ''
-		else:
-			metadata["Description-Content-Type"] = self.config["readme"]["content-type"]
-			description = self.config["readme"]["text"]
+		if self.config["readme"] is not None:
+			metadata_mapping["Description"] = self.config["readme"].text
+			metadata_mapping["Description-Content-Type"] = self.config["readme"].content_type
+
+		return metadata_mapping
 
-		metadata_file.write_lines([
-				# TODO: https://github.com/python/typeshed/issues/5094
-				metadata.as_string(maxheaderlen=2048, policy=metadata.policy.clone(utf8=True)),  # type: ignore
-				description,
-				])
+	def write_metadata(self, metadata_file: PathPlus, metadata_mapping: MetadataMapping) -> None:
+		"""
+		Write `Core Metadata`_ to the given file.
+
+		.. _Core Metadata: https://packaging.python.org/specifications/core-metadata
+
+		:param metadata_file:
+		"""
 
+		metadata_file.write_clean(metadata.dumps(metadata_mapping))
 		self.report_written(metadata_file)
 
-	def call_additional_hooks(self):
+	def call_additional_hooks(self) -> None:
 		"""
 		Subclasses may call this method to give *their* subclasses an opportunity to run custom code.
 
 		For example, the wheel builder calls this as the final step before adding files to the archive,
 		giving an opportunity for subclasses of :class:`~.WheelBuilder` to include additional steps
 		without having to override the entire :meth:`~.WheelBuilder.build_wheel` method.
 		"""
 
 	@abstractmethod
-	def build(self):
+	def build(self) -> str:
 		"""
 		Build the distribution.
 
 		:returns: The filename of the created archive.
 		"""
 
 		raise NotImplementedError
@@ -444,33 +504,42 @@
 	def default_build_dir(self) -> PathPlus:  # pragma: no cover
 		"""
 		Provides a default for the ``build_dir`` argument.
 		"""
 
 		return self.project_dir / "build" / "sdist"
 
+	@property
+	def code_directory(self) -> str:
+		"""
+		The directory containing the code in the build and project directories.
+		"""
+
+		return ''
+
 	def create_sdist_archive(self) -> str:
 		"""
 		Create the sdist archive.
 
 		:return: The filename of the created archive.
 		"""
 
 		self.out_dir.maybe_make(parents=True)
 
 		sdist_filename = self.out_dir / f"{self.archive_name}.tar.gz"
 		with tarfile.open(sdist_filename, mode="w:gz", format=tarfile.PAX_FORMAT) as sdist_archive:
 			for file in self.build_dir.rglob('*'):
 				if file.is_file():
-					sdist_archive.add(str(file), arcname=file.relative_to(self.build_dir).as_posix())
+					arcname = posixpath_join(self.archive_name, file.relative_to(self.build_dir).as_posix())
+					sdist_archive.add(str(file), arcname=arcname)
 
 		self._echo(Fore.GREEN(f"Source distribution created at {sdist_filename.resolve().as_posix()}"))
 		return os.path.basename(sdist_filename)
 
-	def write_pyproject_toml(self):
+	def write_pyproject_toml(self) -> None:
 		"""
 		Write the ``pyproject.toml`` file.
 		"""
 
 		# Copy pyproject.toml
 		pp_toml = dom_toml.load(self.project_dir / "pyproject.toml")
 
@@ -498,17 +567,17 @@
 		# Make "requires-python" static
 		if "requires-python" in dynamic:
 			dynamic.remove("requires-python")
 
 			pp_toml["project"]["requires-python"] = str(self.config["requires-python"])
 
 		# Set the new value for "dynamic"
-		pp_toml["project"]["dynamic"] = dynamic
+		pp_toml["project"]["dynamic"] = sorted(dynamic)
 
-		dom_toml.dump(pp_toml, self.build_dir / "pyproject.toml", encoder=dom_toml.TomlEncoder)
+		dom_toml.dump(pp_toml, self.build_dir / "pyproject.toml", encoder=PyProjectTomlEncoder)
 		self.report_copied(self.project_dir / "pyproject.toml", self.build_dir / "pyproject.toml")
 
 	def build_sdist(self) -> str:
 		"""
 		Build the source distribution.
 
 		:return: The filename of the created archive.
@@ -528,36 +597,36 @@
 			source = self.project_dir / filename
 			if source.is_file():
 				dest = self.build_dir / filename
 				dest.write_clean(source.read_text())
 				self.report_copied(source, dest)
 
 		self.write_readme()
-		self.write_metadata(self.build_dir / "PKG-INFO")
+		self.write_metadata(self.build_dir / "PKG-INFO", self.get_metadata_map())
 		self.call_additional_hooks()
 
 		return self.create_sdist_archive()
 
-	def write_readme(self):
+	def write_readme(self) -> None:
 		"""
 		Write the ``README.*`` file.
 		"""
 
 		if self.config["readme"] is None:
 			return
 
-		if self.config["readme"]["content-type"] == "text/x-rst":
+		if self.config["readme"].content_type == "text/x-rst":
 			target = self.build_dir / "README.rst"
-		elif self.config["readme"]["content-type"] == "text/markdown":
+		elif self.config["readme"].content_type == "text/markdown":
 			target = self.build_dir / "README.md"
 		else:
 			target = self.build_dir / "README"
 
 		target.parent.maybe_make(parents=True)
-		target.write_clean(self.config["readme"]["text"])
+		target.write_clean(self.config["readme"].text)
 		self.report_written(target)
 
 	build = build_sdist
 
 
 class WheelBuilder(AbstractBuilder):
 	"""
@@ -565,14 +634,18 @@
 
 	:param project_dir: The project to build the distribution for.
 	:param build_dir: The (temporary) build directory.
 	:default build_dir: :file:`{<project_dir>}/build/wheel`
 	:param out_dir: The output directory.
 	:default out_dir: :file:`{<project_dir>}/dist`
 	:param verbose: Enable verbose output.
+
+	.. autosummary-widths:: 11/32
+
+	.. latex:vspace:: -10px
 	"""
 
 	@property
 	def default_build_dir(self) -> PathPlus:  # pragma: no cover
 		"""
 		Provides a default for the ``build_dir`` argument.
 		"""
@@ -593,103 +666,179 @@
 	def tag(self) -> str:
 		"""
 		The tag for the wheel.
 		"""
 
 		return "py3-none-any"
 
+	@property
+	def generator(self) -> str:
+		"""
+		The value for the ``Generator`` field in ``*.dist-info/WHEEL``.
+		"""
+
+		# this package
+		from whey import __version__
+
+		return f"whey ({__version__})"
+
 	def write_entry_points(self) -> None:
 		"""
 		Write the list of entry points to the wheel, as specified in
 		``[project.scripts]``, ``[project.gui-scripts]`` and ``[project.entry-points]``
 		"""  # noqa: D400
 
-		buf = StringList()
-		if self.config["scripts"]:
-			buf.append("[console_scripts]")
+		ep_dict = {}
 
-			for name, func in self.config["scripts"].items():
-				buf.append(f"{name} = {func}")
+		if self.config["scripts"]:
+			ep_dict["console_scripts"] = self.config["scripts"]
 
 		if self.config["gui-scripts"]:
-			buf.append("[gui_scripts]")
-
-			for name, func in self.config["gui-scripts"].items():
-				buf.append(f"{name} = {func}")
+			ep_dict["gui_scripts"] = self.config["gui-scripts"]
 
-		for group, entry_points in self.config["entry-points"].items():
-
-			buf.append(f"[{group}]")
-
-			for name, func in entry_points.items():
-				buf.append(f"{name} = {func}")
-
-		cfg_parser = configparser.ConfigParser()
-		cfg_parser.optionxform = str  # type: ignore  # preserve case
-		cfg_parser.read_string(str(buf))
-		cfg_io = StringIO()
-		cfg_parser.write(cfg_io)
+		ep_dict.update(self.config["entry-points"])
 
 		entry_points_file = self.dist_info / "entry_points.txt"
-		entry_points_file.write_clean(cfg_io.getvalue())
+		entry_points.dump(ep_dict, entry_points_file)
 		self.report_written(entry_points_file)
 
 	def write_wheel(self) -> None:
 		"""
 		Write the metadata to the ``WHEEL`` file.
 		"""
 
-		# this package
-		from whey import __version__
+		wheel_file = self.dist_info / "WHEEL"
 
-		wheel = EmailMessage()
-		wheel["Wheel-Version"] = "1.0"
-		wheel["Generator"] = f"whey ({__version__})"
-		wheel["Root-Is-Purelib"] = "true"
-		wheel["Tag"] = self.tag
+		wheel_file.write_clean(
+				wheel.dumps({
+						"Wheel-Version": "1.0",
+						"Generator": self.generator,
+						"Root-Is-Purelib": True,
+						"Tag": [self.tag],
+						})
+				)
 
-		wheel_file = self.dist_info / "WHEEL"
-		wheel_file.write_clean(str(wheel))
 		self.report_written(wheel_file)
 
+	@staticmethod
+	def get_source_epoch() -> Optional[datetime.datetime]:
+		"""
+		Returns the parsed value of the :envvar:`SOURCE_DATE_EPOCH` environment variable, or :py:obj:`None` if unset.
+
+		See https://reproducible-builds.org/specs/source-date-epoch/ for the specification.
+
+		:raises ValueError: if the value is in an invalid format.
+		"""
+
+		# If SOURCE_DATE_EPOCH is set (e.g. by Debian), it's used for timestamps inside the wheel.
+		epoch: Optional[str] = os.environ.get("SOURCE_DATE_EPOCH")
+		if epoch is None:
+			return None
+		elif epoch.isdigit() and sys.version_info >= (3, 11):
+			return datetime.datetime.fromtimestamp(int(epoch), datetime.UTC)  # type: ignore[attr-defined]
+		elif epoch.isdigit():
+			return datetime.datetime.utcfromtimestamp(int(epoch))
+		else:
+			raise ValueError(f"'SOURCE_DATE_EPOCH' must be an integer with no fractional component, not {epoch!r}")
+
 	def create_wheel_archive(self) -> str:
 		"""
 		Create the wheel archive.
 
 		:return: The filename of the created archive.
 		"""
 
 		wheel_filename = self.out_dir / f"{self.archive_name}-{self.tag}.whl"
 		self.out_dir.maybe_make(parents=True)
 
-		with ZipFile(wheel_filename, mode='w') as wheel_archive:
+		mtime = self.get_source_epoch()
+
+		non_record_filenames = []
+		record_filenames = []
+
+		for file in self.build_dir.rglob('*'):
+			if not file.is_file():
+				continue
+			if "RECORD" in file.name and self.dist_info.name in file.parts:
+				record_filenames.append(file)
+				continue
+
+			non_record_filenames.append(file)
+
+		record_filenames = sort_paths(*record_filenames, self.dist_info / "RECORD")
+
+		# Perhaps LZMA support in the future
+		with handy_archives.ZipFile(wheel_filename, mode='w', compression=zipfile.ZIP_DEFLATED) as wheel_archive:
 			with (self.dist_info / "RECORD").open('w') as fp:
-				for file in self.build_dir.rglob('*'):
-					if "RECORD" in file.name and self.dist_info.name in file.parts:
-						continue
-					if not file.is_file():
-						continue
-
-					fp.write(get_record_entry(file, relative_to=self.build_dir))
-					fp.write('\n')
-					wheel_archive.write(file, arcname=file.relative_to(self.build_dir))
-
-				for file in self.dist_info.rglob("RECORD*"):
-					if file.is_file():
-						fp.write(f"{file.relative_to(self.build_dir).as_posix()},,\n")
+				for file in sort_paths(*non_record_filenames):  # pylint: disable=loop-invariant-statement
 
-			for file in self.dist_info.rglob("RECORD*"):
-				if file.is_file():
-					wheel_archive.write(file, arcname=file.relative_to(self.build_dir))
-					self.report_written(file)
+					fp.write(f"{get_record_entry(file, relative_to=self.build_dir)}\n")
+
+					wheel_archive.write_file(
+							file,
+							arcname=file.relative_to(self.build_dir),
+							mtime=mtime,
+							)
+
+				for file in record_filenames:
+					fp.write(f"{file.relative_to(self.build_dir).as_posix()},,\n")
+
+			for file in record_filenames:
+				wheel_archive.write_file(
+						file,
+						arcname=file.relative_to(self.build_dir),
+						mtime=mtime,
+						)
+				self.report_written(file)
 
 		self._echo(Fore.GREEN(f"Wheel created at {wheel_filename.resolve().as_posix()}"))
 
 		return wheel_filename.name
 
+	def create_editables_files(self) -> Iterator[ComparableRequirement]:
+		"""
+		Generate files with `editables`_ for use in a :pep:`660` wheel.
+
+		.. _editables: https://pypi.org/project/editables/
+
+		.. extras-require:: editable
+			:scope: method
+			:pyproject:
+
+		:returns: An iterator of additional runtime requirements which should be added to the wheel's ``METADATA`` file.
+		"""
+
+		# this package
+		from whey._editable import EditableProject
+
+		pkgdir = self.project_dir / self.config["source-dir"] / self.config["package"]
+
+		if not pkgdir.is_dir():
+			message = f"Package directory {self.config['package']!r} not found"
+
+			if self.config["source-dir"]:
+				raise FileNotFoundError(f"{message} in {self.config['source-dir']!r}.")
+			else:
+				raise FileNotFoundError(f"{message}.")
+
+		my_project = EditableProject(
+				self.config["name"].replace('-', '_'),
+				pkgdir.parent,
+				)
+
+		my_project.map_or_add_to_path(self.config["package"], pkgdir)
+
+		for name, content in my_project.files():
+			target = self.build_dir / name
+			target.parent.maybe_make(parents=True)
+			target.write_clean(content)
+			self.report_written(target)
+
+		yield from map(ComparableRequirement, my_project.dependencies())
+
 	def build_wheel(self) -> str:
 		"""
 		Build the binary wheel distribution.
 
 		:return: The filename of the created archive.
 		"""
 
@@ -698,18 +847,60 @@
 
 		self.build_dir.maybe_make(parents=True)
 
 		self.copy_source()
 		self.copy_additional_files()
 		self.write_license(self.dist_info)
 		self.write_entry_points()
-		self.write_metadata(self.dist_info / "METADATA")
+		self.write_metadata(self.dist_info / "METADATA", self.get_metadata_map())
 		self.write_wheel()
 		self.call_additional_hooks()
 
-		top_level = first(posixpath.split(self.config["package"]), default=self.config["package"])
-		(self.dist_info / "top_level.txt").write_clean(top_level)
-		self.report_written(self.dist_info / "top_level.txt")
-
 		return self.create_wheel_archive()
 
 	build = build_wheel
+
+	def build_editable(self) -> str:
+		"""
+		Build an editable wheel.
+
+		An "editable" wheel uses the wheel format not for distribution but as ephemeral communication
+		between the build system and the front end.
+		This avoids having the build backend install anything directly.
+		This wheel must not be exposed to end users, nor cached, nor distributed.
+
+		You should use a different ``build_dir`` and ``out_dir`` to those used for standard wheel builds.
+
+		The default implementation of this method does not call
+		:meth:`~.AbstractBuilder.copy_source` or :meth:`~.AbstractBuilder.copy_additional_files`.
+
+		.. extras-require:: editable
+			:scope: method
+			:pyproject:
+
+		:return: The filename of the created archive.
+		"""
+
+		if self.build_dir.is_dir():
+			shutil.rmtree(self.build_dir)
+
+		self.build_dir.maybe_make(parents=True)
+
+		extra_deps = self.create_editables_files()
+		self.write_license(self.dist_info)
+		self.write_entry_points()
+
+		metadata = self.get_metadata_map()
+
+		for dep in extra_deps:
+			if not any(dep.name in req for req in metadata.get_all("Requires-Dist", ())):
+				# Additional runtime requirement for editable wheels.
+				metadata["Requires-Dist"] = str(dep)
+
+		# Prevents uploading to PyPI, which you shouldn't do with an editable wheel.
+		metadata["Classifier"] = "Private :: Do Not Upload"
+
+		self.write_metadata(self.dist_info / "METADATA", metadata)
+		self.write_wheel()
+		self.call_additional_hooks()
+
+		return self.create_wheel_archive()
```

### Comparing `whey-0.0.9/whey/config/__init__.py` & `whey-0.1.0/whey/config/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,81 +23,111 @@
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
+import re
 from typing import Any, Dict
 
 # 3rd party
 import dom_toml
+import dom_toml.decoder
 from dom_toml.parser import BadConfigError
 from domdf_python_tools.iterative import natmin
 from domdf_python_tools.paths import PathPlus, in_directory
 from domdf_python_tools.typing import PathLike
+from packaging.requirements import InvalidRequirement
 from packaging.specifiers import Specifier
 from shippinglabel.requirements import combine_requirements, read_requirements
 
 # this package
-from whey.config.pep621 import PEP621Parser, read_readme
-from whey.config.whey import WheyParser, backfill_classifiers, get_default_builders
+from whey.config.pep621 import PEP621Parser
+from whey.config.whey import WheyParser, backfill_classifiers
 
-__all__ = [
-		"BadConfigError",
+__all__ = (
 		"PEP621Parser",
 		"WheyParser",
 		"backfill_classifiers",
 		"load_toml",
-		"read_readme",
-		]
+		)
+
+_name_to_package_re = re.compile("-(?!stubs)")
+
+
+def _get_default_package(name: str) -> str:
+	return _name_to_package_re.sub('_', name.split('.', 1)[0])
 
 
 def load_toml(filename: PathLike) -> Dict[str, Any]:  # TODO: TypedDict
 	"""
 	Load the ``whey`` configuration mapping from the given TOML file.
 
 	:param filename:
 	"""
 
 	filename = PathPlus(filename)
 
 	project_dir = filename.parent
-	config = dom_toml.load(filename)
+	config = dom_toml.load(filename, decoder=dom_toml.decoder.TomlPureDecoder)
 
 	parsed_config = {}
 	tool_table = config.get("tool", {})
 
 	with in_directory(project_dir):
 
 		parsed_config.update(WheyParser().parse(tool_table.get("whey", {}), set_defaults=True))
 
 		if "project" in config:
 			parsed_config.update(PEP621Parser().parse(config["project"], set_defaults=True))
 		else:
 			raise KeyError(f"'project' table not found in '{filename!s}'")
 
+		if parsed_config.get("readme", None) is not None:
+			parsed_config["readme"] = parsed_config["readme"].resolve()
+
+		if parsed_config.get("license", None) is not None:
+			parsed_config["license"] = parsed_config["license"].resolve()
+
 	# set defaults
-	parsed_config.setdefault("package", config["project"]["name"].split('.', 1)[0])
+	parsed_config.setdefault("package", _get_default_package(config["project"]["name"]))
 
 	dynamic_fields = parsed_config.get("dynamic", [])
 
 	if "classifiers" in dynamic_fields:
+		dynamic_fields.remove("classifiers")
 		parsed_config["classifiers"] = backfill_classifiers(parsed_config)
 
-	if "requires-python" in dynamic_fields and parsed_config["python-versions"]:
-		parsed_config["requires-python"] = Specifier(f">={natmin(parsed_config['python-versions'])}")
+	if "requires-python" in dynamic_fields:
+		if parsed_config["python-versions"]:
+			dynamic_fields.remove("requires-python")
+			parsed_config["requires-python"] = Specifier(f">={natmin(parsed_config['python-versions'])}")
+		else:
+			raise BadConfigError(
+					"'requires-python' was listed in 'project.dynamic', "
+					"but whey cannot determine the minimum supported Python version. \n"
+					"Set 'tool.whey.python-versions' to a list of supported Python versions to fix this."
+					)
 
 	if "dependencies" in dynamic_fields:
+		dynamic_fields.remove("dependencies")
+
 		if (project_dir / "requirements.txt").is_file():
-			dependencies = read_requirements(project_dir / "requirements.txt", include_invalid=True)[0]
+			dependencies, comments, invalid = read_requirements(project_dir / "requirements.txt", include_invalid=True)
+
+			for bad_string in invalid:
+				raise InvalidRequirement(bad_string)
+
 			parsed_config["dependencies"] = sorted(combine_requirements(dependencies))
 		else:
 			raise BadConfigError(
 					"'project.dependencies' was listed as a dynamic field "
 					"but no 'requirements.txt' file was found."
 					)
 
+	parsed_config["dynamic"] = dynamic_fields
+
 	if "base-classifiers" in parsed_config:
 		del parsed_config["base-classifiers"]
 
 	return parsed_config
```

### Comparing `whey-0.0.9/whey/config/whey.py` & `whey-0.1.0/whey/config/whey.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,27 +23,33 @@
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
-import itertools
-from typing import Dict, Iterable, List, Set, Type
+from typing import Dict, List, Set, Type, cast
 
 # 3rd party
+import dist_meta.entry_points
 from dom_toml.parser import TOML_TYPES, AbstractConfigParser, BadConfigError
-from domdf_python_tools.compat import importlib_metadata
 from natsort import natsorted
 from shippinglabel.classifiers import validate_classifiers
 
 # this package
+from whey import additional_files
 from whey.builder import AbstractBuilder, SDistBuilder, WheelBuilder
 
-__all__ = ["WheyParser", "backfill_classifiers", "get_default_builders", "get_entry_points"]
+__all__ = (
+		"WheyParser",
+		"backfill_classifiers",
+		"get_default_builders",
+		"get_entry_points",
+		"license_lookup",
+		)
 
 #: Mapping of license short codes to license names used in trove classifiers.
 license_lookup = {
 		"Apache-2.0": "Apache Software License",
 		"BSD": "BSD License",
 		"BSD-2-Clause": "BSD License",
 		"BSD-3-Clause": "BSD License",
@@ -91,14 +97,16 @@
 
 	return {"sdist": SDistBuilder, "binary": WheelBuilder, "wheel": WheelBuilder}
 
 
 class WheyParser(AbstractConfigParser):
 	"""
 	Parser for the ``[tool.whey]`` table from ``pyproject.toml``.
+
+	.. autosummary-widths:: 1/2
 	"""
 
 	defaults = {
 			"source-dir": '.',
 			"license-key": None,
 			"platforms": None,
 			"python-versions": None,
@@ -110,15 +118,15 @@
 			"builders": get_default_builders,
 			}
 
 	def parse_package(self, config: Dict[str, TOML_TYPES]) -> str:
 		"""
 		Parse the ``package`` key, giving the name of the importable package.
 
-		This defaults to `project.name <https://www.python.org/dev/peps/pep-0621/#name>`_ if unspecified.
+		This defaults to :pep621:`project.name <name>` if unspecified.
 
 		:param config: The unparsed TOML config for the ``[tool.whey]`` table.
 		"""
 
 		package = config["package"]
 
 		self.assert_type(package, str, ["tool", "whey", "package"])
@@ -149,29 +157,37 @@
 
 		license_key = config["license-key"]
 
 		self.assert_type(license_key, str, ["tool", "whey", "license-key"])
 
 		return license_key
 
-	def parse_additional_files(self, config: Dict[str, TOML_TYPES]) -> List[str]:
+	def parse_additional_files(self, config: Dict[str, TOML_TYPES]) -> List[additional_files.AdditionalFilesEntry]:
 		"""
-		Parse the ``additional-files`` key,
-		giving `MANIFEST.in <https://packaging.python.org/guides/using-manifest-in/>`_-style
+		Parse the ``additional-files`` key, giving `MANIFEST.in`_-style
 		entries for additional files to include in distributions.
 
+		.. _MANIFEST.in: https://packaging.python.org/guides/using-manifest-in/
+
 		:param config: The unparsed TOML config for the ``[tool.whey]`` table.
 		"""  # noqa: D400
 
-		additional_files = config["additional-files"]
+		entries = config["additional-files"]
 
-		for idx, file in enumerate(additional_files):
+		for idx, file in enumerate(entries):
 			self.assert_indexed_type(file, str, ["tool", "whey", "additional-files"], idx=idx)
 
-		return additional_files
+		parsed_additional_files = []
+
+		for entry in entries:
+			parsed_entry = additional_files.from_entry(entry)
+			if parsed_entry is not None:
+				parsed_additional_files.append(parsed_entry)
+
+		return parsed_additional_files
 
 	def parse_platforms(self, config: Dict[str, TOML_TYPES]) -> List[str]:
 		"""
 		Parse the ``platforms`` key, giving a list of supported platforms. Optional.
 
 		:param config: The unparsed TOML config for the ``[tool.whey]`` table.
 		"""
@@ -192,17 +208,18 @@
 		"""
 
 		python_versions = config["python-versions"]
 
 		for idx, version in enumerate(python_versions):
 			if not isinstance(version, (str, int, float)):
 				raise TypeError(
-						f"Invalid type for 'tool.whey.python-versions[{idx}]': expected {str!r}, {int!r} or {float!r}, got {type(version)!r}"
+						f"Invalid type for 'tool.whey.python-versions[{idx}]': "
+						f"expected {str!r}, {int!r} or {float!r}, got {type(version)!r}"
 						)
-			if str(version) in "12":
+			if str(version)[0] in "12":
 				raise BadConfigError(
 						f"Invalid value for 'tool.whey.python-versions[{idx}]': whey only supports Python 3-only projects."
 						)
 
 		return list(map(str, python_versions))
 
 	def parse_python_implementations(self, config: Dict[str, TOML_TYPES]) -> List[str]:
@@ -217,22 +234,25 @@
 		for idx, impl in enumerate(python_implementations):
 			self.assert_indexed_type(impl, str, ["tool", "whey", "python-implementations"], idx=idx)
 
 		return python_implementations
 
 	def parse_base_classifiers(self, config: Dict[str, TOML_TYPES]) -> Set[str]:
 		"""
-		Parse the ``base-classifiers`` key, giving a list `trove classifiers <https://pypi.org/classifiers/>`_.
+		Parse the ``base-classifiers`` key, giving a list `trove classifiers <https://pypi.org/classifiers/>`__.
 
 		This list will be extended with the appropriate classifiers for supported platforms,
 		Python versions and implementations, and the project's license.
-		Ignored if `classifiers <https://www.python.org/dev/peps/pep-0621/#classifiers>`_
-		is not listed in `dynamic <https://www.python.org/dev/peps/pep-0621/#dynamic>`_
+		Ignored if :pep621:`classifiers` is not listed in :pep621:`dynamic`
 
 		:param config: The unparsed TOML config for the ``[tool.whey]`` table.
+
+		:rtype:
+
+		.. latex:clearpage::
 		"""
 
 		parsed_classifiers = set()
 
 		for idx, classifier in enumerate(config["base-classifiers"]):
 			self.assert_indexed_type(classifier, str, ["tool", "whey", "python-implementations"], idx=idx)
 			parsed_classifiers.add(classifier)
@@ -247,28 +267,28 @@
 
 		:param config: The unparsed TOML config for the ``[tool.whey]`` table.
 		"""
 
 		parsed_builders = get_default_builders()
 		builders = config["builders"]
 
-		entry_points: Dict[str, importlib_metadata.EntryPoint] = {ep.name: ep for ep in get_entry_points()}
+		entry_points: Dict[str, dist_meta.entry_points.EntryPoint] = get_entry_points()
 
 		self.assert_type(builders, dict, ["tool", "whey", "builders"])
 
 		for builder_type in ["binary", "sdist", "wheel"]:
 			if builder_type in builders:
 				entry_point_name = builders[builder_type]
 				if entry_point_name not in entry_points:
 					raise BadConfigError(
-							f"Unknown {builder_type} builder {entry_point_name}. \n"
+							f"Unknown {builder_type} builder {entry_point_name!r}. \n"
 							f"Is it registered as an entry point under 'whey.builder'?"
 							)
 
-				parsed_builders[builder_type] = entry_points[entry_point_name].load()
+				parsed_builders[builder_type] = cast(Type[AbstractBuilder], entry_points[entry_point_name].load())
 
 		return parsed_builders
 
 	@property
 	def keys(self) -> List[str]:
 		"""
 		The keys to parse from the TOML file.
@@ -332,20 +352,27 @@
 	parsed_classifiers.add("Programming Language :: Python")
 
 	validate_classifiers(parsed_classifiers)
 
 	return natsorted(parsed_classifiers)
 
 
-def get_entry_points() -> Iterable[importlib_metadata.EntryPoint]:
+def get_entry_points(group: str = "whey.builder") -> Dict[str, dist_meta.entry_points.EntryPoint]:
 	r"""
-	Returns an iterable over `EntryPoint <https://docs.python.org/3/library/importlib.metadata.html#entry-points>`_
-	objects in the ``whey.builder`` group.
+	Returns an iterable over `EntryPoint`_ objects in the ``group`` group.
 
-	:rtype: :class:`Iterable <typing.Iterable>`\[`EntryPoint <https://docs.python.org/3/library/importlib.metadata.html#entry-points>`_\]
-	"""  # noqa: D400
+	:param group:
+
+	:rtype: :class:`Iterable <typing.Iterable>`\[`EntryPoint`_\]
+
+	.. _EntryPoint: https://docs.python.org/3/library/importlib.metadata.html#entry-points
+	"""
+
+	eps = dist_meta.entry_points.get_entry_points(group)
+
+	entry_points: Dict[str, dist_meta.entry_points.EntryPoint] = {}
 
-	eps = itertools.chain.from_iterable(dist.entry_points for dist in importlib_metadata.distributions())
+	for entry_point in eps:  # pylint: disable=use-dict-comprehension
+		if entry_point.group == group:
+			entry_points[entry_point.name] = entry_point
 
-	for entry_point in eps:
-		if entry_point.group == "whey.builder":
-			yield entry_point
+	return entry_points
```

### Comparing `whey-0.0.9/whey/foreman.py` & `whey-0.1.0/whey/foreman.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,123 +23,124 @@
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
-from typing import Any, Mapping, Optional, Type
+from typing import Optional, Type
 
 # 3rd party
+from consolekit.terminal_colours import ColourTrilean
 from domdf_python_tools.paths import PathPlus, traverse_to_file
 from domdf_python_tools.typing import PathLike
 
 # this package
 from whey.builder import AbstractBuilder
 from whey.config import load_toml
 
-__all__ = ["Foreman"]
+__all__ = ("Foreman", )
 
 
 class Foreman:
 	"""
 	Responsible for loading the configuration calling the builders.
 	"""
 
 	def __init__(self, project_dir: PathLike):
 
-		# Walk up the tree until a "pyproject.toml" file is found.
+		# Walk up the tree until a ``pyproject.toml`` file is found.
 		#: The pyproject.toml directory
 		self.project_dir: PathPlus = traverse_to_file(PathPlus(project_dir), "pyproject.toml")
 
-		#: Configuration parsed from "pyproject.toml".
+		#: Configuration parsed from ``pyproject.toml``.
 		self.config = load_toml(self.project_dir / "pyproject.toml")
 
 	def get_builder(self, distribution_type: str) -> Type[AbstractBuilder]:
 		"""
-		Returns the builder for the given distribution type (e.g. "source").
+		Returns the builder for the given distribution type.
 
-		:param distribution_type:
+		:param distribution_type: The distribution type, such as ``'source'`` or ``'wheel'``.
 		"""
 
 		return self.config["builders"][distribution_type]
 
 	def build_sdist(
 			self,
 			build_dir: Optional[PathLike] = None,
 			out_dir: Optional[PathLike] = None,
 			*args,
 			verbose: bool = False,
-			colour: bool = None,
+			colour: ColourTrilean = None,
 			**kwargs,
-			):
+			) -> str:
 		"""
 		Build a sdist distribution using the ``sdist`` builder configured in ``pyproject.toml``.
 
 		:returns: The filename of the created archive.
 		"""
 
-		builder = self.get_builder("sdist")(  # type: ignore
-			self.project_dir,
-			self.config,
-			build_dir,
-			out_dir,
-			*args,
-			verbose=verbose,
-			colour=colour,
-			**kwargs,
-			)
+		builder = self.get_builder("sdist")(
+				self.project_dir,
+				self.config,
+				build_dir,
+				out_dir,
+				*args,
+				verbose=verbose,
+				colour=colour,
+				**kwargs,
+				)
 		return builder.build()
 
 	def build_binary(
 			self,
 			build_dir: Optional[PathLike] = None,
 			out_dir: Optional[PathLike] = None,
 			*args,
 			verbose: bool = False,
-			colour: bool = None,
+			colour: ColourTrilean = None,
 			**kwargs,
-			):
+			) -> str:
 		"""
 		Build a binary distribution using the ``binary`` builder configured in ``pyproject.toml``.
 
 		:returns: The filename of the created archive.
 		"""
 
-		builder = self.get_builder("binary")(  # type: ignore
-			self.project_dir,
-			self.config,
-			build_dir,
-			out_dir,
-			*args,
-			verbose=verbose,
-			colour=colour,
-			**kwargs,
-			)
+		builder = self.get_builder("binary")(
+				self.project_dir,
+				self.config,
+				build_dir,
+				out_dir,
+				*args,
+				verbose=verbose,
+				colour=colour,
+				**kwargs,
+				)
 		return builder.build()
 
 	def build_wheel(
 			self,
 			build_dir: Optional[PathLike] = None,
 			out_dir: Optional[PathLike] = None,
 			*args,
 			verbose: bool = False,
-			colour: bool = None,
+			colour: ColourTrilean = None,
 			**kwargs,
-			):
+			) -> str:
 		"""
 		Build a wheel distribution using the ``wheel`` builder configured in ``pyproject.toml``.
 
 		:returns: The filename of the created archive.
 		"""
 
-		builder = self.get_builder("wheel")(  # type: ignore
-			self.project_dir,
-			self.config,
-			build_dir,
-			out_dir,
-			*args,
-			verbose=verbose,
-			colour=colour,
-			**kwargs,
-			)
+		builder = self.get_builder("wheel")(
+				self.project_dir,
+				self.config,
+				build_dir,
+				out_dir,
+				*args,
+				verbose=verbose,
+				colour=colour,
+				**kwargs,
+				)
 		return builder.build()
```

