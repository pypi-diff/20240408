# Comparing `tmp/dom_toml-1.0.0.tar.gz` & `tmp/dom_toml-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dom_toml-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dom_toml-2.0.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dom_toml-1.0.0.tar` & `dom_toml-2.0.0b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2024-04-08 10:27:20.869920 dom_toml-1.0.0/LICENSE
--rw-r--r--   0        0        0     5071 2024-04-08 10:27:20.869920 dom_toml-1.0.0/README.rst
--rw-r--r--   0        0        0     4441 2024-04-08 10:27:20.869920 dom_toml-1.0.0/dom_toml/__init__.py
--rw-r--r--   0        0        0     1816 2024-04-08 10:27:20.873920 dom_toml-1.0.0/dom_toml/decoder.py
--rw-r--r--   0        0        0     5470 2024-04-08 10:27:20.873920 dom_toml-1.0.0/dom_toml/encoder.py
--rw-r--r--   0        0        0     7446 2024-04-08 10:27:20.873920 dom_toml-1.0.0/dom_toml/parser.py
--rw-r--r--   0        0        0        0 2024-04-08 10:27:20.873920 dom_toml-1.0.0/dom_toml/py.typed
--rw-r--r--   0        0        0     4588 2024-04-08 10:27:20.873920 dom_toml-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6570 1970-01-01 00:00:00.000000 dom_toml-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-08 11:00:11.113636 dom_toml-2.0.0b1/LICENSE
+-rw-r--r--   0        0        0     5073 2024-04-08 11:00:11.113636 dom_toml-2.0.0b1/README.rst
+-rw-r--r--   0        0        0     4321 2024-04-08 11:00:11.117636 dom_toml-2.0.0b1/dom_toml/__init__.py
+-rw-r--r--   0        0        0     2775 2024-04-08 11:00:11.117636 dom_toml-2.0.0b1/dom_toml/decoder.py
+-rw-r--r--   0        0        0    10658 2024-04-08 11:00:11.117636 dom_toml-2.0.0b1/dom_toml/encoder.py
+-rw-r--r--   0        0        0     7457 2024-04-08 11:00:11.117636 dom_toml-2.0.0b1/dom_toml/parser.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:00:11.117636 dom_toml-2.0.0b1/dom_toml/py.typed
+-rw-r--r--   0        0        0     4590 2024-04-08 11:00:11.117636 dom_toml-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     6574 1970-01-01 00:00:00.000000 dom_toml-2.0.0b1/PKG-INFO
```

### Comparing `dom_toml-1.0.0/LICENSE` & `dom_toml-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `dom_toml-1.0.0/README.rst` & `dom_toml-2.0.0b1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/dom_toml
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v1.0.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v2.0.0b1
 	:target: https://github.com/domdfcoding/dom_toml/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/commit/master
 	:alt: GitHub last commit
```

### Comparing `dom_toml-1.0.0/dom_toml/__init__.py` & `dom_toml-2.0.0b1/dom_toml/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,113 +33,114 @@
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
-from typing import Any, Mapping, MutableMapping, Type, Union
+from typing import Any, Dict, Mapping, Type, Union
 
 # 3rd party
-import toml
 from domdf_python_tools.paths import PathPlus
 from domdf_python_tools.typing import PathLike
 
 # this package
+from dom_toml.decoder import TomlDecoder
 from dom_toml.encoder import TomlEncoder
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "1.0.0"
+__version__: str = "2.0.0b1"
 __email__: str = "dominic@davis-foster.co.uk"
 
-__all__ = ["TomlEncoder", "dumps", "loads", "dump", "load"]
+__all__ = ["dumps", "loads", "dump", "load"]
 
 
 def dumps(
 		data: Mapping[str, Any],
-		encoder: Union[Type[toml.TomlEncoder], toml.TomlEncoder] = toml.TomlEncoder,
+		encoder: Union[Type[TomlEncoder], TomlEncoder] = TomlEncoder,
 		) -> str:
 	r"""
 	Convert ``data`` to a TOML string.
 
 	:param data:
-	:param encoder: The :class:`toml.TomlEncoder` to use for constructing the output string.
+	:param encoder: The :class:`~.TomlEncoder` to use for constructing the output string.
 
 	:returns: A string containing the ``TOML`` corresponding to ``data``.
 
-	.. versionchanged:: 1.0.0  ``encoder`` must now be a :class:`toml.TomlEncoder` type or instance.
+	.. versionchanged:: 2.0.0  ``encoder`` must now be a :class:`~.TomlEncoder` type or instance.
 	.. latex:clearpage::
 	"""
 
 	if isinstance(encoder, type):
 		encoder = encoder()
 
-	return toml.dumps(data, encoder=encoder)
+	return ''.join(encoder.dumps(data, name=''))
 
 
 def dump(
 		data: Mapping[str, Any],
 		filename: PathLike,
-		encoder: Union[Type[toml.TomlEncoder], toml.TomlEncoder] = toml.TomlEncoder,
+		encoder: Union[Type[TomlEncoder], TomlEncoder] = TomlEncoder,
 		) -> str:
 	r"""
 	Writes out ``data`` as TOML to the given file.
 
 	:param data:
 	:param filename: The filename to write to.
-	:param encoder: The :class:`toml.TomlEncoder` to use for constructing the output string.
+	:param encoder: The :class:`~.TomlEncoder` to use for constructing the output string.
 
 	:returns: A string containing the ``TOML`` corresponding to ``data``.
 
-	.. versionchanged:: 1.0.0  ``encoder`` must now be a :class:`toml.TomlEncoder` type or instance.
+	.. versionchanged:: 2.0.0  ``encoder`` must now be a :class:`~.TomlEncoder` type or instance.
 	"""
 
 	filename = PathPlus(filename)
 	as_toml = dumps(data, encoder=encoder)
 	filename.write_clean(as_toml)
 	return as_toml
 
 
 def loads(
 		s: str,
-		decoder: Union[Type[toml.TomlDecoder], toml.TomlDecoder] = toml.TomlDecoder,
-		) -> MutableMapping[str, Any]:
+		decoder: Union[Type[TomlDecoder], TomlDecoder] = TomlDecoder,
+		) -> Dict[str, Any]:
 	r"""
 	Parse the given string as TOML.
 
 	:param s:
-	:param dict\_: The class of the returned data.
-	:param decoder: The :class:`toml.TomlEncoder` to use for constructing the output string.
+	:param decoder: The :class:`~.TomlEncoder` to use for constructing the output string.
 
 	:returns: A mapping containing the ``TOML`` data.
 
-	.. versionchanged:: 1.0.0  ``decoder`` must now be a :class:`toml.TomlDecoder` type or instance.
+	.. versionchanged:: 2.0.0  ``decoder`` must now be a :class:`~.TomlDecoder` type or instance.
 	"""
 
+	if not isinstance(s, str):
+		raise TypeError("Expecting something like a string")
+
 	if isinstance(decoder, type):
 		decoder = decoder()
 
-	return toml.loads(s, decoder=decoder)
+	return decoder.loads(s)
 
 
 def load(
 		filename: PathLike,
-		decoder: Union[Type[toml.TomlDecoder], toml.TomlDecoder] = toml.TomlDecoder,
-		) -> MutableMapping[str, Any]:
+		decoder: Union[Type[TomlDecoder], TomlDecoder] = TomlDecoder,
+		) -> Dict[str, Any]:
 	r"""
 	Parse TOML from the given file.
 
 	:param filename: The filename to read from to.
-	:param dict\_: The class of the returned data.
-	:param decoder: The :class:`toml.TomlEncoder` to use for constructing the output string.
+	:param decoder: The :class:`~.TomlEncoder` to use for constructing the output string.
 
 	:returns: A mapping containing the ``TOML`` data.
 
-	.. versionchanged:: 1.0.0  ``decoder`` must now be a :class:`toml.TomlDecoder` type or instance.
+	.. versionchanged:: 2.0.0  ``decoder`` must now be a :class:`~.TomlDecoder` type or instance.
 	"""
 
 	return loads(
 			PathPlus(filename).read_text(),
 			decoder=decoder,
 			)
```

### Comparing `dom_toml-1.0.0/dom_toml/parser.py` & `dom_toml-2.0.0b1/dom_toml/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 from abc import ABC, abstractmethod
 from typing import Any, Callable, ClassVar, Dict, Iterable, List, Optional, Tuple, Type, TypeVar, Union
 
-# 3rd party
-import toml
+# this package
+import dom_toml
 
 __all__ = ["AbstractConfigParser", "BadConfigError", "construct_path", "TOML_TYPES"]
 
 TOML_TYPES = Any
 
 
 class BadConfigError(ValueError):
@@ -62,15 +62,15 @@
 def construct_path(path: Iterable[str]) -> str:
 	"""
 	Construct a dotted path to a key.
 
 	:param path: The path elements.
 	"""
 
-	return '.'.join([toml.dumps({elem: 0})[:-5] for elem in path])
+	return '.'.join([dom_toml.dumps({elem: 0})[:-5] for elem in path])
 
 
 _C = TypeVar("_C", bound=Callable)
 
 
 class AbstractConfigParser(ABC):
 	"""
```

### Comparing `dom_toml-1.0.0/pyproject.toml` & `dom_toml-2.0.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "flit-core<4,>=3.2",]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "dom_toml"
-version = "1.0.0"
+version = "2.0.0b1"
 description = "Dom's tools for Tom's Obvious, Minimal Language."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "configuration", "serialize", "toml",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -24,15 +24,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-dependencies = [ "domdf-python-tools>=2.8.0", "toml>=0.10.2",]
+dependencies = [ "domdf-python-tools>=2.8.0", "tomli>=1.2.3",]
 dynamic = []
 
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
```

### Comparing `dom_toml-1.0.0/PKG-INFO` & `dom_toml-2.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dom_toml
-Version: 1.0.0
+Version: 2.0.0b1
 Summary: Dom's tools for Tom's Obvious, Minimal Language.
 Keywords: configuration,serialize,toml
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: domdf-python-tools>=2.8.0
-Requires-Dist: toml>=0.10.2
+Requires-Dist: tomli>=1.2.3
 Project-URL: Documentation, https://dom-toml.readthedocs.io/en/latest
 Project-URL: Homepage, https://github.com/domdfcoding/dom_toml
 Project-URL: Issue Tracker, https://github.com/domdfcoding/dom_toml/issues
 Project-URL: Source Code, https://github.com/domdfcoding/dom_toml
 
 #########
 dom_toml
@@ -129,15 +129,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/dom_toml
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v1.0.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/dom_toml/v2.0.0b1
 	:target: https://github.com/domdfcoding/dom_toml/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/dom_toml
 	:target: https://github.com/domdfcoding/dom_toml/commit/master
 	:alt: GitHub last commit
```

