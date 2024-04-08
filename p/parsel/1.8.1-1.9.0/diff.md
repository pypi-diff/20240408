# Comparing `tmp/parsel-1.8.1.tar.gz` & `tmp/parsel-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsel-1.8.1.tar", last modified: Tue Apr 18 13:40:43 2023, max compression
+gzip compressed data, was "parsel-1.9.0.tar", last modified: Thu Mar 14 10:17:22 2024, max compression
```

## Comparing `parsel-1.8.1.tar` & `parsel-1.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:40:43.213823 parsel-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-18 13:40:28.000000 parsel-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-18 13:40:28.000000 parsel-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-04-18 13:40:28.000000 parsel-1.8.1/NEWS
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-04-18 13:40:43.213823 parsel-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-18 13:40:28.000000 parsel-1.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:40:43.209823 parsel-1.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-04-18 13:40:28.000000 parsel-1.8.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     4104 2023-04-18 13:40:28.000000 parsel-1.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 13:40:28.000000 parsel-1.8.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-18 13:40:28.000000 parsel-1.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-18 13:40:28.000000 parsel-1.8.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-18 13:40:28.000000 parsel-1.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-18 13:40:28.000000 parsel-1.8.1/docs/parsel.rst
--rw-r--r--   0 runner    (1001) docker     (123)    42563 2023-04-18 13:40:28.000000 parsel-1.8.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:40:43.209823 parsel-1.8.1/parsel/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-18 13:40:28.000000 parsel-1.8.1/parsel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-18 13:40:28.000000 parsel-1.8.1/parsel/csstranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:40:28.000000 parsel-1.8.1/parsel/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28634 2023-04-18 13:40:28.000000 parsel-1.8.1/parsel/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-18 13:40:28.000000 parsel-1.8.1/parsel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-18 13:40:28.000000 parsel-1.8.1/parsel/xpathfuncs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:40:43.209823 parsel-1.8.1/parsel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-04-18 13:40:43.000000 parsel-1.8.1/parsel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-18 13:40:43.000000 parsel-1.8.1/parsel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:40:43.000000 parsel-1.8.1/parsel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:40:43.000000 parsel-1.8.1/parsel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 13:40:43.000000 parsel-1.8.1/parsel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 13:40:43.000000 parsel-1.8.1/parsel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-18 13:40:43.213823 parsel-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-18 13:40:28.000000 parsel-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:40:43.213823 parsel-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-18 13:40:28.000000 parsel-1.8.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    53734 2023-04-18 13:40:28.000000 parsel-1.8.1/tests/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-18 13:40:28.000000 parsel-1.8.1/tests/test_selector_csstranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-18 13:40:28.000000 parsel-1.8.1/tests/test_selector_jmespath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-18 13:40:28.000000 parsel-1.8.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-18 13:40:28.000000 parsel-1.8.1/tests/test_xml_attacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-18 13:40:28.000000 parsel-1.8.1/tests/test_xpathfuncs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:40:43.213823 parsel-1.8.1/tests/typing/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-18 13:40:28.000000 parsel-1.8.1/tests/typing/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:40:43.213823 parsel-1.8.1/tests/xml_attacks/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-18 13:40:28.000000 parsel-1.8.1/tests/xml_attacks/billion_laughs.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:17:22.951786 parsel-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-14 10:17:11.000000 parsel-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-14 10:17:11.000000 parsel-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-03-14 10:17:11.000000 parsel-1.9.0/NEWS
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-03-14 10:17:22.951786 parsel-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-14 10:17:11.000000 parsel-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:17:22.947786 parsel-1.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-03-14 10:17:11.000000 parsel-1.9.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4116 2024-03-14 10:17:11.000000 parsel-1.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-14 10:17:11.000000 parsel-1.9.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-14 10:17:11.000000 parsel-1.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-14 10:17:11.000000 parsel-1.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-03-14 10:17:11.000000 parsel-1.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-14 10:17:11.000000 parsel-1.9.0/docs/parsel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    42563 2024-03-14 10:17:11.000000 parsel-1.9.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:17:22.947786 parsel-1.9.0/parsel/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-14 10:17:11.000000 parsel-1.9.0/parsel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-03-14 10:17:11.000000 parsel-1.9.0/parsel/csstranslator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 10:17:11.000000 parsel-1.9.0/parsel/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28288 2024-03-14 10:17:11.000000 parsel-1.9.0/parsel/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-03-14 10:17:11.000000 parsel-1.9.0/parsel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-14 10:17:11.000000 parsel-1.9.0/parsel/xpathfuncs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:17:22.951786 parsel-1.9.0/parsel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-03-14 10:17:22.000000 parsel-1.9.0/parsel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-14 10:17:22.000000 parsel-1.9.0/parsel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 10:17:22.000000 parsel-1.9.0/parsel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 10:17:22.000000 parsel-1.9.0/parsel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-14 10:17:22.000000 parsel-1.9.0/parsel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-14 10:17:22.000000 parsel-1.9.0/parsel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-14 10:17:22.951786 parsel-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-14 10:17:11.000000 parsel-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:17:22.951786 parsel-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-14 10:17:11.000000 parsel-1.9.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    53050 2024-03-14 10:17:11.000000 parsel-1.9.0/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-03-14 10:17:11.000000 parsel-1.9.0/tests/test_selector_csstranslator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-03-14 10:17:11.000000 parsel-1.9.0/tests/test_selector_jmespath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-14 10:17:11.000000 parsel-1.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-14 10:17:11.000000 parsel-1.9.0/tests/test_xml_attacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-03-14 10:17:11.000000 parsel-1.9.0/tests/test_xpathfuncs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:17:22.951786 parsel-1.9.0/tests/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-14 10:17:11.000000 parsel-1.9.0/tests/typing/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:17:22.951786 parsel-1.9.0/tests/xml_attacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-14 10:17:11.000000 parsel-1.9.0/tests/xml_attacks/billion_laughs.xml
```

### Comparing `parsel-1.8.1/LICENSE` & `parsel-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parsel-1.8.1/NEWS` & `parsel-1.9.0/NEWS`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 .. :changelog:
 
 History
 -------
 
+1.9.0 (2024-03-14)
+~~~~~~~~~~~~~~~~~~
+
+* Now requires ``cssselect >= 1.2.0`` (this minimum version was required since
+  1.8.0 but that wasn't properly recorded)
+* Removed support for Python 3.7
+* Added support for Python 3.12 and PyPy 3.10
+* Fixed an exception when calling ``__str__`` or `__repr__`` on some JSON
+  selectors
+* Code formatted with ``black``
+* CI fixes and improvements
+
 1.8.1 (2023-04-18)
 ~~~~~~~~~~~~~~~~~~
 
 * Remove a Sphinx reference from NEWS to fix the PyPI description
 * Add a ``twine check`` CI check to detect such problems
 
 1.8.0 (2023-04-18)
```

### Comparing `parsel-1.8.1/PKG-INFO` & `parsel-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: parsel
-Version: 1.8.1
+Version: 1.9.0
 Summary: Parsel is a library to extract data from HTML and XML using XPath and CSS selectors
 Home-page: https://github.com/scrapy/parsel
 Author: Scrapy project
 Author-email: info@scrapy.org
 License: BSD
 Keywords: parsel
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: cssselect>=1.2.0
+Requires-Dist: jmespath
+Requires-Dist: lxml
+Requires-Dist: packaging
+Requires-Dist: w3lib>=1.19.0
 
 ======
 Parsel
 ======
 
 .. image:: https://github.com/scrapy/parsel/actions/workflows/tests.yml/badge.svg
    :target: https://github.com/scrapy/parsel/actions/workflows/tests.yml
@@ -102,14 +108,26 @@
 
 
 
 
 History
 -------
 
+1.9.0 (2024-03-14)
+~~~~~~~~~~~~~~~~~~
+
+* Now requires ``cssselect >= 1.2.0`` (this minimum version was required since
+  1.8.0 but that wasn't properly recorded)
+* Removed support for Python 3.7
+* Added support for Python 3.12 and PyPy 3.10
+* Fixed an exception when calling ``__str__`` or `__repr__`` on some JSON
+  selectors
+* Code formatted with ``black``
+* CI fixes and improvements
+
 1.8.1 (2023-04-18)
 ~~~~~~~~~~~~~~~~~~
 
 * Remove a Sphinx reference from NEWS to fix the PyPI description
 * Add a ``twine check`` CI check to detect such problems
 
 1.8.0 (2023-04-18)
```

### Comparing `parsel-1.8.1/README.rst` & `parsel-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `parsel-1.8.1/docs/Makefile` & `parsel-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parsel-1.8.1/docs/conf.py` & `parsel-1.9.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python
 
 import os
 import sys
 
-
 # Get the project root dir, which is the parent dir of this
 cwd = os.getcwd()
 project_root = os.path.dirname(cwd)
 
 # Insert the project root dir as the first element in the PYTHONPATH.
 # This lets us ensure that the source package is imported, and that its
 # version is used.
 sys.path.insert(0, project_root)
 
-import parsel
-
+import parsel  # noqa: E402
 
 # -- General configuration ---------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     "notfound.extension",
@@ -94,18 +92,17 @@
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ("index", "parsel", "Parsel Documentation", ["Scrapy Project"], 1)
+    ("index", "parsel", "Parsel Documentation", ["Scrapy Project"], 1),
 ]
 
-
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
```

### Comparing `parsel-1.8.1/docs/make.bat` & `parsel-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `parsel-1.8.1/docs/usage.rst` & `parsel-1.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `parsel-1.8.1/parsel/csstranslator.py` & `parsel-1.9.0/parsel/csstranslator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from functools import lru_cache
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any, Optional, Protocol
 
 from cssselect import GenericTranslator as OriginalGenericTranslator
 from cssselect import HTMLTranslator as OriginalHTMLTranslator
-from cssselect.xpath import XPathExpr as OriginalXPathExpr
-from cssselect.xpath import ExpressionError
 from cssselect.parser import Element, FunctionalPseudoElement, PseudoElement
-
+from cssselect.xpath import ExpressionError
+from cssselect.xpath import XPathExpr as OriginalXPathExpr
 
 if TYPE_CHECKING:
     # typing.Self requires Python 3.11
     from typing_extensions import Self
 
 
 class XPathExpr(OriginalXPathExpr):
@@ -21,17 +20,15 @@
     @classmethod
     def from_xpath(
         cls,
         xpath: OriginalXPathExpr,
         textnode: bool = False,
         attribute: Optional[str] = None,
     ) -> "Self":
-        x = cls(
-            path=xpath.path, element=xpath.element, condition=xpath.condition
-        )
+        x = cls(path=xpath.path, element=xpath.element, condition=xpath.condition)
         x.textnode = textnode
         x.attribute = attribute
         return x
 
     def __str__(self) -> str:
         path = super().__str__()
         if self.textnode:
@@ -63,36 +60,30 @@
             )
         super().join(combiner, other, *args, **kwargs)
         self.textnode = other.textnode
         self.attribute = other.attribute
         return self
 
 
-if TYPE_CHECKING:
-    # requires Python 3.8
-    from typing import Protocol
-
-    # e.g. cssselect.GenericTranslator, cssselect.HTMLTranslator
-    class TranslatorProtocol(Protocol):
-        def xpath_element(self, selector: Element) -> OriginalXPathExpr:
-            pass
+# e.g. cssselect.GenericTranslator, cssselect.HTMLTranslator
+class TranslatorProtocol(Protocol):
+    def xpath_element(self, selector: Element) -> OriginalXPathExpr:
+        pass
 
-        def css_to_xpath(self, css: str, prefix: str = ...) -> str:
-            pass
+    def css_to_xpath(self, css: str, prefix: str = ...) -> str:
+        pass
 
 
 class TranslatorMixin:
     """This mixin adds support to CSS pseudo elements via dynamic dispatch.
 
     Currently supported pseudo-elements are ``::text`` and ``::attr(ATTR_NAME)``.
     """
 
-    def xpath_element(
-        self: "TranslatorProtocol", selector: Element
-    ) -> XPathExpr:
+    def xpath_element(self: TranslatorProtocol, selector: Element) -> XPathExpr:
         # https://github.com/python/mypy/issues/12344
         xpath = super().xpath_element(selector)  # type: ignore[safe-super]
         return XPathExpr.from_xpath(xpath)
 
     def xpath_pseudo_element(
         self, xpath: OriginalXPathExpr, pseudo_element: PseudoElement
     ) -> OriginalXPathExpr:
@@ -104,15 +95,17 @@
             method = getattr(self, method_name, None)
             if not method:
                 raise ExpressionError(
                     f"The functional pseudo-element ::{pseudo_element.name}() is unknown"
                 )
             xpath = method(xpath, pseudo_element)
         else:
-            method_name = f"xpath_{pseudo_element.replace('-', '_')}_simple_pseudo_element"
+            method_name = (
+                f"xpath_{pseudo_element.replace('-', '_')}_simple_pseudo_element"
+            )
             method = getattr(self, method_name, None)
             if not method:
                 raise ExpressionError(
                     f"The pseudo-element ::{pseudo_element} is unknown"
                 )
             xpath = method(xpath)
         return xpath
@@ -121,38 +114,30 @@
         self, xpath: OriginalXPathExpr, function: FunctionalPseudoElement
     ) -> XPathExpr:
         """Support selecting attribute values using ::attr() pseudo-element"""
         if function.argument_types() not in (["STRING"], ["IDENT"]):
             raise ExpressionError(
                 f"Expected a single string or ident for ::attr(), got {function.arguments!r}"
             )
-        return XPathExpr.from_xpath(
-            xpath, attribute=function.arguments[0].value
-        )
+        return XPathExpr.from_xpath(xpath, attribute=function.arguments[0].value)
 
-    def xpath_text_simple_pseudo_element(
-        self, xpath: OriginalXPathExpr
-    ) -> XPathExpr:
+    def xpath_text_simple_pseudo_element(self, xpath: OriginalXPathExpr) -> XPathExpr:
         """Support selecting text nodes using ::text pseudo-element"""
         return XPathExpr.from_xpath(xpath, textnode=True)
 
 
 class GenericTranslator(TranslatorMixin, OriginalGenericTranslator):
     @lru_cache(maxsize=256)
-    def css_to_xpath(
-        self, css: str, prefix: str = "descendant-or-self::"
-    ) -> str:
+    def css_to_xpath(self, css: str, prefix: str = "descendant-or-self::") -> str:
         return super().css_to_xpath(css, prefix)
 
 
 class HTMLTranslator(TranslatorMixin, OriginalHTMLTranslator):
     @lru_cache(maxsize=256)
-    def css_to_xpath(
-        self, css: str, prefix: str = "descendant-or-self::"
-    ) -> str:
+    def css_to_xpath(self, css: str, prefix: str = "descendant-or-self::") -> str:
         return super().css_to_xpath(css, prefix)
 
 
 _translator = HTMLTranslator()
 
 
 def css2xpath(query: str) -> str:
```

### Comparing `parsel-1.8.1/parsel/selector.py` & `parsel-1.9.0/parsel/selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,49 +5,41 @@
 import typing
 import warnings
 from io import BytesIO
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     Mapping,
     Optional,
     Pattern,
+    SupportsIndex,
     Tuple,
     Type,
+    TypedDict,
     TypeVar,
     Union,
 )
 from warnings import warn
 
-try:
-    from typing import TypedDict  # pylint: disable=ungrouped-imports
-except ImportError:  # Python 3.7
-    from typing_extensions import TypedDict
-
 import jmespath
 from lxml import etree, html
 from packaging.version import Version
 
 from .csstranslator import GenericTranslator, HTMLTranslator
 from .utils import extract_regex, flatten, iflatten, shorten
 
-if typing.TYPE_CHECKING:
-    # both require Python 3.8
-    from typing import Literal, SupportsIndex
-
-    # simplified _OutputMethodArg from types-lxml
-    _TostringMethodType = Literal[
-        "html",
-        "xml",
-    ]
-
-
 _SelectorType = TypeVar("_SelectorType", bound="Selector")
-_ParserType = Union[etree.XMLParser, etree.HTMLParser]
+_ParserType = Union[etree.XMLParser, etree.HTMLParser]  # type: ignore[type-arg]
+# simplified _OutputMethodArg from types-lxml
+_TostringMethodType = Literal[
+    "html",
+    "xml",
+]
 
 lxml_version = Version(etree.__version__)
 lxml_huge_tree_version = Version("4.2")
 LXML_SUPPORTS_HUGE_TREE = lxml_version >= lxml_huge_tree_version
 
 
 class CannotRemoveElementWithoutRoot(Exception):
@@ -138,40 +130,34 @@
         pass
 
     def __getitem__(
         self, pos: Union["SupportsIndex", slice]
     ) -> Union[_SelectorType, "SelectorList[_SelectorType]"]:
         o = super().__getitem__(pos)
         if isinstance(pos, slice):
-            return self.__class__(
-                typing.cast("SelectorList[_SelectorType]", o)
-            )
+            return self.__class__(typing.cast("SelectorList[_SelectorType]", o))
         else:
             return typing.cast(_SelectorType, o)
 
     def __getstate__(self) -> None:
         raise TypeError("can't pickle SelectorList objects")
 
-    def jmespath(
-        self, query: str, **kwargs: Any
-    ) -> "SelectorList[_SelectorType]":
+    def jmespath(self, query: str, **kwargs: Any) -> "SelectorList[_SelectorType]":
         """
         Call the ``.jmespath()`` method for each element in this list and return
         their results flattened as another :class:`SelectorList`.
 
         ``query`` is the same argument as the one in :meth:`Selector.jmespath`.
 
         Any additional named arguments are passed to the underlying
         ``jmespath.search`` call, e.g.::
 
             selector.jmespath('author.name', options=jmespath.Options(dict_cls=collections.OrderedDict))
         """
-        return self.__class__(
-            flatten([x.jmespath(query, **kwargs) for x in self])
-        )
+        return self.__class__(flatten([x.jmespath(query, **kwargs) for x in self]))
 
     def xpath(
         self,
         xpath: str,
         namespaces: Optional[Mapping[str, str]] = None,
         **kwargs: Any,
     ) -> "SelectorList[_SelectorType]":
@@ -188,17 +174,15 @@
 
         Any additional named arguments can be used to pass values for XPath
         variables in the XPath expression, e.g.::
 
             selector.xpath('//a[href=$url]', url="http://www.example.com")
         """
         return self.__class__(
-            flatten(
-                [x.xpath(xpath, namespaces=namespaces, **kwargs) for x in self]
-            )
+            flatten([x.xpath(xpath, namespaces=namespaces, **kwargs) for x in self])
         )
 
     def css(self, query: str) -> "SelectorList[_SelectorType]":
         """
         Call the ``.css()`` method for each element in this list and return
         their results flattened as another :class:`SelectorList`.
 
@@ -214,17 +198,15 @@
         their results flattened, as a list of strings.
 
         By default, character entity references are replaced by their
         corresponding character (except for ``&amp;`` and ``&lt;``.
         Passing ``replace_entities`` as ``False`` switches off these
         replacements.
         """
-        return flatten(
-            [x.re(regex, replace_entities=replace_entities) for x in self]
-        )
+        return flatten([x.re(regex, replace_entities=replace_entities) for x in self])
 
     @typing.overload
     def re_first(
         self,
         regex: Union[str, Pattern[str]],
         default: None = None,
         replace_entities: bool = True,
@@ -319,17 +301,15 @@
         for x in self:
             x.drop()
 
 
 _NOT_SET = object()
 
 
-def _get_root_from_text(
-    text: str, *, type: str, **lxml_kwargs: Any
-) -> etree._Element:
+def _get_root_from_text(text: str, *, type: str, **lxml_kwargs: Any) -> etree._Element:
     return create_root_node(text, _ctgroup[type]["_parser"], **lxml_kwargs)
 
 
 def _get_root_and_type_from_bytes(
     body: bytes,
     encoding: str,
     *,
@@ -586,17 +566,15 @@
         def make_selector(x: Any) -> _SelectorType:  # closure function
             if isinstance(x, str):
                 return self.__class__(text=x, _expr=query, type="text")
             else:
                 return self.__class__(root=x, _expr=query)
 
         result = [make_selector(x) for x in result]
-        return typing.cast(
-            SelectorList[_SelectorType], self.selectorlist_cls(result)
-        )
+        return typing.cast(SelectorList[_SelectorType], self.selectorlist_cls(result))
 
     def xpath(
         self: _SelectorType,
         query: str,
         namespaces: Optional[Mapping[str, str]] = None,
         **kwargs: Any,
     ) -> SelectorList[_SelectorType]:
@@ -614,17 +592,15 @@
 
         Any additional named arguments can be used to pass values for XPath
         variables in the XPath expression, e.g.::
 
             selector.xpath('//a[href=$url]', url="http://www.example.com")
         """
         if self.type not in ("html", "xml", "text"):
-            raise ValueError(
-                f"Cannot use xpath on a Selector of type {self.type!r}"
-            )
+            raise ValueError(f"Cannot use xpath on a Selector of type {self.type!r}")
         if self.type in ("html", "xml"):
             try:
                 xpathev = self.root.xpath
             except AttributeError:
                 return typing.cast(
                     SelectorList[_SelectorType], self.selectorlist_cls([])
                 )
@@ -657,33 +633,29 @@
                 root=x,
                 _expr=query,
                 namespaces=self.namespaces,
                 type=_xml_or_html(self.type),
             )
             for x in result
         ]
-        return typing.cast(
-            SelectorList[_SelectorType], self.selectorlist_cls(result)
-        )
+        return typing.cast(SelectorList[_SelectorType], self.selectorlist_cls(result))
 
     def css(self: _SelectorType, query: str) -> SelectorList[_SelectorType]:
         """
         Apply the given CSS selector and return a :class:`SelectorList` instance.
 
         ``query`` is a string containing the CSS selector to apply.
 
         In the background, CSS queries are translated into XPath queries using
         `cssselect`_ library and run ``.xpath()`` method.
 
         .. _cssselect: https://pypi.python.org/pypi/cssselect/
         """
         if self.type not in ("html", "xml", "text"):
-            raise ValueError(
-                f"Cannot use css on a Selector of type {self.type!r}"
-            )
+            raise ValueError(f"Cannot use css on a Selector of type {self.type!r}")
         return self.xpath(self._css2xpath(query))
 
     def _css2xpath(self, query: str) -> str:
         type = _xml_or_html(self.type)
         return _ctgroup[type]["_csstranslator"].css_to_xpath(query)
 
     def re(
@@ -741,16 +713,18 @@
         return next(
             iflatten(self.re(regex, replace_entities=replace_entities)),
             default,
         )
 
     def get(self) -> Any:
         """
-        Serialize and return the matched nodes in a single string.
-        Percent encoded content is unquoted.
+        Serialize and return the matched nodes.
+
+        For HTML and XML, the result is always a string, and percent-encoded
+        content is unquoted.
         """
         if self.type in ("text", "json"):
             return self.root
         try:
             return typing.cast(
                 str,
                 etree.tostring(
@@ -869,11 +843,12 @@
         given by the contents it selects.
         """
         return bool(self.get())
 
     __nonzero__ = __bool__
 
     def __str__(self) -> str:
-        data = repr(shorten(self.get(), width=40))
-        return f"<{type(self).__name__} query={self._expr!r} data={data}>"
+        return str(self.get())
 
-    __repr__ = __str__
+    def __repr__(self) -> str:
+        data = repr(shorten(str(self.get()), width=40))
+        return f"<{type(self).__name__} query={self._expr!r} data={data}>"
```

### Comparing `parsel-1.8.1/parsel/utils.py` & `parsel-1.9.0/parsel/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 from typing import Any, Iterable, Iterator, List, Match, Pattern, Union, cast
+
 from w3lib.html import replace_entities as w3lib_replace_entities
 
 
 def flatten(x: Iterable[Any]) -> List[Any]:
     """flatten(sequence) -> list
     Returns a single, flat list which contains all elements retrieved
     from the sequence and all recursively contained sub-sequences
```

### Comparing `parsel-1.8.1/parsel/xpathfuncs.py` & `parsel-1.9.0/parsel/xpathfuncs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import re
 from typing import Any, Callable, Optional
 
 from lxml import etree
-
 from w3lib.html import HTML5_WHITESPACE
 
-
 regex = f"[{HTML5_WHITESPACE}]+"
 replace_html5_whitespaces = re.compile(regex).sub
 
 
 def set_xpathfunc(fname: str, func: Optional[Callable]) -> None:  # type: ignore[type-arg]
     """Register a custom extension function to use in XPath expressions.
 
@@ -20,15 +18,15 @@
     If ``func`` is ``None``, the extension function will be removed.
 
     See more `in lxml documentation`_.
 
     .. _`in lxml documentation`: https://lxml.de/extensions.html#xpath-extension-functions
 
     """
-    ns_fns = etree.FunctionNamespace(None)  # type: ignore[attr-defined]
+    ns_fns = etree.FunctionNamespace(None)
     if func is not None:
         ns_fns[fname] = func
     else:
         del ns_fns[fname]
 
 
 def setup() -> None:
@@ -39,22 +37,18 @@
     """has-class function.
 
     Return True if all ``classes`` are present in element's class attr.
 
     """
     if not context.eval_context.get("args_checked"):
         if not classes:
-            raise ValueError(
-                "XPath error: has-class must have at least 1 argument"
-            )
+            raise ValueError("XPath error: has-class must have at least 1 argument")
         for c in classes:
             if not isinstance(c, str):
-                raise ValueError(
-                    "XPath error: has-class arguments must be strings"
-                )
+                raise ValueError("XPath error: has-class arguments must be strings")
         context.eval_context["args_checked"] = True
 
     node_cls = context.context_node.get("class")
     if node_cls is None:
         return False
     node_cls = " " + node_cls + " "
     node_cls = replace_html5_whitespaces(" ", node_cls)
```

### Comparing `parsel-1.8.1/parsel.egg-info/PKG-INFO` & `parsel-1.9.0/parsel.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: parsel
-Version: 1.8.1
+Version: 1.9.0
 Summary: Parsel is a library to extract data from HTML and XML using XPath and CSS selectors
 Home-page: https://github.com/scrapy/parsel
 Author: Scrapy project
 Author-email: info@scrapy.org
 License: BSD
 Keywords: parsel
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: cssselect>=1.2.0
+Requires-Dist: jmespath
+Requires-Dist: lxml
+Requires-Dist: packaging
+Requires-Dist: w3lib>=1.19.0
 
 ======
 Parsel
 ======
 
 .. image:: https://github.com/scrapy/parsel/actions/workflows/tests.yml/badge.svg
    :target: https://github.com/scrapy/parsel/actions/workflows/tests.yml
@@ -102,14 +108,26 @@
 
 
 
 
 History
 -------
 
+1.9.0 (2024-03-14)
+~~~~~~~~~~~~~~~~~~
+
+* Now requires ``cssselect >= 1.2.0`` (this minimum version was required since
+  1.8.0 but that wasn't properly recorded)
+* Removed support for Python 3.7
+* Added support for Python 3.12 and PyPy 3.10
+* Fixed an exception when calling ``__str__`` or `__repr__`` on some JSON
+  selectors
+* Code formatted with ``black``
+* CI fixes and improvements
+
 1.8.1 (2023-04-18)
 ~~~~~~~~~~~~~~~~~~
 
 * Remove a Sphinx reference from NEWS to fix the PyPI description
 * Add a ``twine check`` CI check to detect such problems
 
 1.8.0 (2023-04-18)
```

### Comparing `parsel-1.8.1/parsel.egg-info/SOURCES.txt` & `parsel-1.9.0/parsel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsel-1.8.1/setup.py` & `parsel-1.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
-
 with open("README.rst", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 with open("NEWS", encoding="utf-8") as history_file:
     history = history_file.read().replace(".. :changelog:", "")
 
 setup(
     name="parsel",
-    version="1.8.1",
+    version="1.9.0",
     description="Parsel is a library to extract data from HTML and XML using XPath and CSS selectors",
     long_description=readme + "\n\n" + history,
+    long_description_content_type="text/x-rst",
     author="Scrapy project",
     author_email="info@scrapy.org",
     url="https://github.com/scrapy/parsel",
     packages=[
         "parsel",
     ],
     package_dir={
         "parsel": "parsel",
     },
     include_package_data=True,
     install_requires=[
-        "cssselect>=0.9",
+        "cssselect>=1.2.0",
         "jmespath",
         "lxml",
         "packaging",
-        "typing_extensions; python_version < '3.8'",
         "w3lib>=1.19.0",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     license="BSD",
     zip_safe=False,
     keywords="parsel",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Topic :: Text Processing :: Markup",
         "Topic :: Text Processing :: Markup :: HTML",
         "Topic :: Text Processing :: Markup :: XML",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     setup_requires=[
         "pytest-runner",
     ],
     tests_require=[
```

### Comparing `parsel-1.8.1/tests/test_selector.py` & `parsel-1.9.0/tests/test_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
+import pickle
 import re
+import typing
+import unittest
 import warnings
 import weakref
-import unittest
-import pickle
-
-import typing
-from typing import cast, Any, Optional, Mapping
+from typing import Any, Mapping, Optional, cast
 
 from lxml import etree
 from lxml.html import HtmlElement
-from pkg_resources import parse_version
+from packaging.version import Version
 
 from parsel import Selector, SelectorList
 from parsel.selector import (
-    CannotRemoveElementWithoutRoot,
-    CannotRemoveElementWithoutParent,
-    LXML_SUPPORTS_HUGE_TREE,
     _NOT_SET,
+    LXML_SUPPORTS_HUGE_TREE,
+    CannotRemoveElementWithoutParent,
+    CannotRemoveElementWithoutRoot,
 )
 
 
 class SelectorTestCase(unittest.TestCase):
 
     sscls = Selector
 
@@ -28,29 +27,25 @@
         self.assertEqual(type(value), type(self.sscls(text="")))
 
     def assertIsSelectorList(self, value: Any) -> None:
         self.assertEqual(type(value), type(self.sscls.selectorlist_cls()))
 
     def test_pickle_selector(self) -> None:
         sel = self.sscls(text="<html><body><p>some text</p></body></html>")
-        self.assertRaises(
-            TypeError, lambda s: pickle.dumps(s, protocol=2), sel
-        )
+        self.assertRaises(TypeError, lambda s: pickle.dumps(s, protocol=2), sel)
 
     def test_pickle_selector_list(self) -> None:
         sel = self.sscls(
             text="<html><body><ul><li>1</li><li>2</li><li>3</li></ul></body></html>"
         )
         sel_list = sel.css("li")
         empty_sel_list = sel.css("p")
         self.assertIsSelectorList(sel_list)
         self.assertIsSelectorList(empty_sel_list)
-        self.assertRaises(
-            TypeError, lambda s: pickle.dumps(s, protocol=2), sel_list
-        )
+        self.assertRaises(TypeError, lambda s: pickle.dumps(s, protocol=2), sel_list)
         self.assertRaises(
             TypeError, lambda s: pickle.dumps(s, protocol=2), empty_sel_list
         )
 
     def test_simple_selection(self) -> None:
         """Simple selector tests"""
         body = "<p><input name='a'value='1'/><input name='b'value='2'/></p>"
@@ -95,18 +90,15 @@
 
     def test_simple_selection_with_variables(self) -> None:
         """Using XPath variables"""
         body = "<p><input name='a' value='1'/><input name='b' value='2'/></p>"
         sel = self.sscls(text=body)
 
         self.assertEqual(
-            [
-                x.extract()
-                for x in sel.xpath("//input[@value=$number]/@name", number=1)
-            ],
+            [x.extract() for x in sel.xpath("//input[@value=$number]/@name", number=1)],
             ["a"],
         )
         self.assertEqual(
             [
                 x.extract()
                 for x in sel.xpath("//input[@name=$letter]/@value", letter="b")
             ],
@@ -120,23 +112,19 @@
                 letter="a",
             ).extract(),
             ["2.0"],
         )
 
         # you can also pass booleans
         self.assertEqual(
-            sel.xpath(
-                "boolean(count(//input)=$cnt)=$test", cnt=2, test=True
-            ).extract(),
+            sel.xpath("boolean(count(//input)=$cnt)=$test", cnt=2, test=True).extract(),
             ["1"],
         )
         self.assertEqual(
-            sel.xpath(
-                "boolean(count(//input)=$cnt)=$test", cnt=4, test=True
-            ).extract(),
+            sel.xpath("boolean(count(//input)=$cnt)=$test", cnt=4, test=True).extract(),
             ["0"],
         )
         self.assertEqual(
             sel.xpath(
                 "boolean(count(//input)=$cnt)=$test", cnt=4, test=False
             ).extract(),
             ["1"],
@@ -158,39 +146,32 @@
         body = """<p>I'm mixing single and <input name='a' value='I say "Yeah!"'/>
         "double quotes" and I don't care :)</p>"""
         sel = self.sscls(text=body)
 
         t = 'I say "Yeah!"'
         # naive string formatting with give something like:
         # ValueError: XPath error: Invalid predicate in //input[@value="I say "Yeah!""]/@name
-        self.assertRaises(
-            ValueError, sel.xpath, f'//input[@value="{t}"]/@name'
-        )
+        self.assertRaises(ValueError, sel.xpath, f'//input[@value="{t}"]/@name')
 
         # with XPath variables, escaping is done for you
         self.assertEqual(
-            [
-                x.extract()
-                for x in sel.xpath("//input[@value=$text]/@name", text=t)
-            ],
+            [x.extract() for x in sel.xpath("//input[@value=$text]/@name", text=t)],
             ["a"],
         )
         lt = """I'm mixing single and "double quotes" and I don't care :)"""
         # the following gives you something like
         # ValueError: XPath error: Invalid predicate in //p[normalize-space()='I'm mixing single and "double quotes" and I don't care :)']//@name
         self.assertRaises(
             ValueError, sel.xpath, f"//p[normalize-space()='{lt}']//@name"
         )
 
         self.assertEqual(
             [
                 x.extract()
-                for x in sel.xpath(
-                    "//p[normalize-space()=$lng]//@name", lng=lt
-                )
+                for x in sel.xpath("//p[normalize-space()=$lng]//@name", lng=lt)
             ],
             ["a"],
         )
 
     def test_accessing_attributes(self) -> None:
         body = """
 <html lang="en" version="1.0">
@@ -206,17 +187,15 @@
         sel = self.sscls(text=body)
         self.assertEqual({"lang": "en", "version": "1.0"}, sel.attrib)
         self.assertEqual(
             {"id": "some-list", "class": "list-cls"}, sel.css("ul")[0].attrib
         )
 
         # for a SelectorList, bring the attributes of first-element only
-        self.assertEqual(
-            {"id": "some-list", "class": "list-cls"}, sel.css("ul").attrib
-        )
+        self.assertEqual({"id": "some-list", "class": "list-cls"}, sel.css("ul").attrib)
         self.assertEqual(
             {"class": "item-cls", "id": "list-item-1"}, sel.css("li").attrib
         )
         self.assertEqual({}, sel.css("body").attrib)
         self.assertEqual({}, sel.css("non-existing-element").attrib)
 
         self.assertEqual(
@@ -228,28 +207,24 @@
             [e.attrib for e in sel.css("li")],
         )
 
     def test_representation_slice(self) -> None:
         body = f"<p><input name='{50 * 'b'}' value='\xa9'/></p>"
         sel = self.sscls(text=body)
 
-        representation = (
-            f"<Selector query='//input/@name' data='{37 * 'b'}...'>"
-        )
+        representation = f"<Selector query='//input/@name' data='{37 * 'b'}...'>"
 
         self.assertEqual(
             [repr(it) for it in sel.xpath("//input/@name")], [representation]
         )
 
     def test_representation_unicode_query(self) -> None:
         body = f"<p><input name='{50 * 'b'}' value='\xa9'/></p>"
 
-        representation = (
-            "<Selector query='//input[@value=\"©\"]/@value' data='©'>"
-        )
+        representation = "<Selector query='//input[@value=\"©\"]/@value' data='©'>"
 
         sel = self.sscls(text=body)
         self.assertEqual(
             [repr(it) for it in sel.xpath('//input[@value="\xa9"]/@value')],
             [representation],
         )
 
@@ -300,17 +275,15 @@
         """Test if get() returns extracted value on a Selector"""
         body = '<ul><li id="1">1</li><li id="2">2</li><li id="3">3</li></ul>'
         sel = self.sscls(text=body)
 
         self.assertEqual(
             sel.xpath("//ul/li[position()>1]")[0].get(), '<li id="2">2</li>'
         )
-        self.assertEqual(
-            sel.xpath("//ul/li[position()>1]/text()")[0].get(), "2"
-        )
+        self.assertEqual(sel.xpath("//ul/li[position()>1]/text()")[0].get(), "2")
 
     def test_selector_getall_alias(self) -> None:
         """Test if get() returns extracted value on a Selector"""
         body = '<ul><li id="1">1</li><li id="2">2</li><li id="3">3</li></ul>'
         sel = self.sscls(text=body)
 
         self.assertListEqual(
@@ -372,17 +345,15 @@
             sel.xpath("/ul/li/text()").re_first(r"\w+", default="missing"),
             "missing",
         )
 
     def test_select_unicode_query(self) -> None:
         body = "<p><input name='\xa9' value='1'/></p>"
         sel = self.sscls(text=body)
-        self.assertEqual(
-            sel.xpath('//input[@name="\xa9"]/@value').extract(), ["1"]
-        )
+        self.assertEqual(sel.xpath('//input[@name="\xa9"]/@value').extract(), ["1"])
 
     def test_list_elements_type(self) -> None:
         """Test Selector returning the same type in selection methods"""
         text = "<p>test<p>"
         self.assertEqual(
             type(self.sscls(text=text).xpath("//p")[0]),
             type(self.sscls(text=text)),
@@ -391,20 +362,16 @@
             type(self.sscls(text=text).css("p")[0]),
             type(self.sscls(text=text)),
         )
 
     def test_boolean_result(self) -> None:
         body = "<p><input name='a'value='1'/><input name='b'value='2'/></p>"
         xs = self.sscls(text=body)
-        self.assertEqual(
-            xs.xpath("//input[@name='a']/@name='a'").extract(), ["1"]
-        )
-        self.assertEqual(
-            xs.xpath("//input[@name='a']/@name='n'").extract(), ["0"]
-        )
+        self.assertEqual(xs.xpath("//input[@name='a']/@name='a'").extract(), ["1"])
+        self.assertEqual(xs.xpath("//input[@name='a']/@name='n'").extract(), ["0"])
 
     def test_differences_parsing_xml_vs_html(self) -> None:
         """Test that XML and HTML Selector's behave differently"""
         # some text which is parsed differently by XML and HTML flavors
         text = '<div><img src="a.jpg"><p>Hello</div>'
         hs = self.sscls(text=text, type="html")
         self.assertEqual(
@@ -526,17 +493,15 @@
                     <div id=1>not<span>me</span></div>
                     <div class="dos"><p>text</p><a href='#'>foo</a></div>
                </body>"""
         sel = self.sscls(text=body)
         self.assertEqual(
             sel.xpath('//div[@id="1"]').css("span::text").extract(), ["me"]
         )
-        self.assertEqual(
-            sel.css("#1").xpath("./span/text()").extract(), ["me"]
-        )
+        self.assertEqual(sel.css("#1").xpath("./span/text()").extract(), ["me"])
 
     def test_dont_strip(self) -> None:
         sel = self.sscls(text='<div>fff: <a href="#">zzz</a></div>')
         self.assertEqual(sel.xpath("//text()").extract(), ["fff: ", "zzz"])
 
     def test_namespaces_simple(self) -> None:
         body = """
@@ -603,24 +568,20 @@
             "xmlns",
             "http://webservices.amazon.com/AWSECommerceService/2005-10-05",
         )
         x.register_namespace("p", "http://www.scrapy.org/product")
         x.register_namespace("b", "http://somens.com")
         self.assertEqual(len(x.xpath("//xmlns:TestTag")), 1)
         self.assertEqual(x.xpath("//b:Operation/text()").extract()[0], "hello")
-        self.assertEqual(
-            x.xpath("//xmlns:TestTag/@b:att").extract()[0], "value"
-        )
+        self.assertEqual(x.xpath("//xmlns:TestTag/@b:att").extract()[0], "value")
         self.assertEqual(
             x.xpath("//p:SecondTestTag/xmlns:price/text()").extract()[0], "90"
         )
         self.assertEqual(
-            x.xpath("//p:SecondTestTag")
-            .xpath("./xmlns:price/text()")[0]
-            .extract(),
+            x.xpath("//p:SecondTestTag").xpath("./xmlns:price/text()")[0].extract(),
             "90",
         )
         self.assertEqual(
             x.xpath("//p:SecondTestTag/xmlns:material/text()").extract()[0],
             "iron",
         )
 
@@ -709,17 +670,15 @@
                     "p": "http://www.scrapy.org/product",
                 },
             ).extract_first(),
             "Dried Rose",
         )
 
         # "p" prefix is not cached from previous calls
-        self.assertRaises(
-            ValueError, x.xpath, "//p:SecondTestTag/xmlns:price/text()"
-        )
+        self.assertRaises(ValueError, x.xpath, "//p:SecondTestTag/xmlns:price/text()")
 
         x.register_namespace("p", "http://www.scrapy.org/product")
         self.assertEqual(
             x.xpath("//p:SecondTestTag/xmlns:material/text()").extract()[0],
             "iron",
         )
 
@@ -783,36 +742,30 @@
         )
         self.assertEqual(
             x.xpath("//script")[0].re(name_re, replace_entities=False),
             [expected],
         )
 
         self.assertEqual(
-            x.xpath("//script/text()").re_first(
-                name_re, replace_entities=False
-            ),
+            x.xpath("//script/text()").re_first(name_re, replace_entities=False),
             expected,
         )
         self.assertEqual(
             x.xpath("//script")[0].re_first(name_re, replace_entities=False),
             expected,
         )
 
     def test_re_intl(self) -> None:
         body = "<div>Evento: cumplea\xf1os</div>"
         x = self.sscls(text=body)
-        self.assertEqual(
-            x.xpath("//div").re(r"Evento: (\w+)"), ["cumplea\xf1os"]
-        )
+        self.assertEqual(x.xpath("//div").re(r"Evento: (\w+)"), ["cumplea\xf1os"])
 
     def test_selector_over_text(self) -> None:
         hs = self.sscls(text="<root>lala</root>")
-        self.assertEqual(
-            hs.extract(), "<html><body><root>lala</root></body></html>"
-        )
+        self.assertEqual(hs.extract(), "<html><body><root>lala</root></body></html>")
         xs = self.sscls(text="<root>lala</root>", type="xml")
         self.assertEqual(xs.extract(), "<root>lala</root>")
         self.assertEqual(xs.xpath(".").extract(), ["<root>lala</root>"])
 
     def test_invalid_xpath(self) -> None:
         "Test invalid xpath raises ValueError with the invalid xpath"
         x = self.sscls(text="<html></html>")
@@ -830,25 +783,21 @@
         # '\xc2\xa3' = pound symbol in utf-8
         # '\xa3'     = pound symbol in latin-1 (iso-8859-1)
 
         text = """<html>
         <head><meta http-equiv="Content-Type" content="text/html; charset=iso-8859-1"></head>
         <body><span id="blank">\xa3</span></body></html>"""
         x = self.sscls(text=text)
-        self.assertEqual(
-            x.xpath("//span[@id='blank']/text()").extract(), ["\xa3"]
-        )
+        self.assertEqual(x.xpath("//span[@id='blank']/text()").extract(), ["\xa3"])
 
     def test_empty_bodies_shouldnt_raise_errors(self) -> None:
         self.sscls(text="").xpath("//text()").extract()
 
     def test_bodies_with_comments_only(self) -> None:
-        sel = self.sscls(
-            text="<!-- hello world -->", base_url="http://example.com"
-        )
+        sel = self.sscls(text="<!-- hello world -->", base_url="http://example.com")
         self.assertEqual("http://example.com", sel.root.base)
 
     def test_null_bytes_shouldnt_raise_errors(self) -> None:
         text = "<root>pre\x00post</root>"
         self.sscls(text).xpath("//text()").extract()
 
     def test_replacement_char_from_badly_encoded_body(self) -> None:
@@ -866,33 +815,29 @@
         self.assertEqual(x1.xpath(".//b").extract(), [])
         # Tag attribute
         x1 = r.xpath("//span/@class")
         self.assertEqual(x1.extract(), ["big"])
         self.assertEqual(x1.xpath(".//text()").extract(), [])
 
     def test_select_on_text_nodes(self) -> None:
-        r = self.sscls(
-            text="<div><b>Options:</b>opt1</div><div><b>Other</b>opt2</div>"
-        )
+        r = self.sscls(text="<div><b>Options:</b>opt1</div><div><b>Other</b>opt2</div>")
         x1 = r.xpath(
             "//div/descendant::text()[preceding-sibling::b[contains(text(), 'Options')]]"
         )
         self.assertEqual(x1.extract(), ["opt1"])
 
         x1 = r.xpath(
             "//div/descendant::text()/preceding-sibling::b[contains(text(), 'Options')]"
         )
         self.assertEqual(x1.extract(), ["<b>Options:</b>"])
 
     @unittest.skip("Text nodes lost parent node reference in lxml")
     def test_nested_select_on_text_nodes(self) -> None:
         # FIXME: does not work with lxml backend [upstream]
-        r = self.sscls(
-            text="<div><b>Options:</b>opt1</div><div><b>Other</b>opt2</div>"
-        )
+        r = self.sscls(text="<div><b>Options:</b>opt1</div><div><b>Other</b>opt2</div>")
         x1 = r.xpath("//div/descendant::text()")
         x2 = x1.xpath("./preceding-sibling::b[contains(text(), 'Options')]")
         self.assertEqual(x2.extract(), ["<b>Options:</b>"])
 
     def test_weakref_slots(self) -> None:
         """Check that classes are using slots and are weak-referenceable"""
         x = self.sscls(text="")
@@ -944,19 +889,15 @@
                     "//f:link",
                     namespaces={"f": "http://www.w3.org/2005/Atom"},
                 )
             ),
             2,
         )
         self.assertEqual(
-            len(
-                sel.xpath(
-                    "//s:stop", namespaces={"s": "http://www.w3.org/2000/svg"}
-                )
-            ),
+            len(sel.xpath("//s:stop", namespaces={"s": "http://www.w3.org/2000/svg"})),
             2,
         )
         sel.remove_namespaces()
         self.assertEqual(len(sel.xpath("//link")), 2)
         self.assertEqual(len(sel.xpath("//stop")), 2)
         self.assertEqual(len(sel.xpath("./namespace::*")), 1)
 
@@ -996,27 +937,21 @@
 
         # .getparent() is available for text nodes and attributes
         # only when smart_strings are on
         x = self.sscls(text=body)
         li_text = x.xpath("//li/text()")
         self.assertFalse(any([hasattr(e.root, "getparent") for e in li_text]))
         div_class = x.xpath("//div/@class")
-        self.assertFalse(
-            any([hasattr(e.root, "getparent") for e in div_class])
-        )
+        self.assertFalse(any([hasattr(e.root, "getparent") for e in div_class]))
 
         smart_x = SmartStringsSelector(text=body)
         smart_li_text = smart_x.xpath("//li/text()")
-        self.assertTrue(
-            all([hasattr(e.root, "getparent") for e in smart_li_text])
-        )
+        self.assertTrue(all([hasattr(e.root, "getparent") for e in smart_li_text]))
         smart_div_class = smart_x.xpath("//div/@class")
-        self.assertTrue(
-            all([hasattr(e.root, "getparent") for e in smart_div_class])
-        )
+        self.assertTrue(all([hasattr(e.root, "getparent") for e in smart_div_class]))
 
     def test_xml_entity_expansion(self) -> None:
         malicious_xml = (
             '<?xml version="1.0" encoding="ISO-8859-1"?>'
             "<!DOCTYPE foo [ <!ELEMENT foo ANY > <!ENTITY xxe SYSTEM "
             '"file:///etc/passwd" >]><foo>&xxe;</foo>'
         )
@@ -1111,16 +1046,16 @@
         self.assertIsSelectorList(sel.css("li"))
         self.assertEqual(sel.css("li::text").getall(), ["1", "2", "3"])
 
         sel.css("body").drop()
         self.assertEqual(sel.get(), "<html></html>")
 
     def test_deep_nesting(self) -> None:
-        lxml_version = parse_version(etree.__version__)
-        lxml_huge_tree_version = parse_version("4.2")
+        lxml_version = Version(etree.__version__)
+        lxml_huge_tree_version = Version("4.2")
 
         content = """
         <html>
         <body>
         <span><span><span><span><span><span><span><span><span><span><span><span><span><span><span><span><span><span>
         <span><span><span><span><span><span><span><span><span><span><span><span><span><span><span><span><span><span>
         <span><span><span><span><span><span><span><span><span><span><span><span><span><span><span><span><span><span>
@@ -1248,14 +1183,22 @@
             ValueError,
             "object as root",
             Selector,
             root=selector.root,
             type="json",
         )
 
+    def test_json_selector_representation(self) -> None:
+        selector = Selector(text="true")
+        assert repr(selector) == "<Selector query=None data='True'>"
+        assert str(selector) == "True"
+        selector = Selector(text="1")
+        assert repr(selector) == "<Selector query=None data='1'>"
+        assert str(selector) == "1"
+
 
 class ExsltTestCase(unittest.TestCase):
 
     sscls = Selector
 
     def test_regexp(self) -> None:
         """EXSLT regular expression tests"""
@@ -1268,38 +1211,26 @@
         </div>
         """
         sel = self.sscls(text=body)
 
         # re:test()
         self.assertEqual(
             sel.xpath('//input[re:test(@name, "[A-Z]+", "i")]').extract(),
-            [
-                x.extract()
-                for x in sel.xpath('//input[re:test(@name, "[A-Z]+", "i")]')
-            ],
+            [x.extract() for x in sel.xpath('//input[re:test(@name, "[A-Z]+", "i")]')],
         )
         self.assertEqual(
-            [
-                x.extract()
-                for x in sel.xpath(r'//a[re:test(@href, "\.html$")]/text()')
-            ],
+            [x.extract() for x in sel.xpath(r'//a[re:test(@href, "\.html$")]/text()')],
             ["first link", "second link"],
         )
         self.assertEqual(
-            [
-                x.extract()
-                for x in sel.xpath('//a[re:test(@href, "first")]/text()')
-            ],
+            [x.extract() for x in sel.xpath('//a[re:test(@href, "first")]/text()')],
             ["first link"],
         )
         self.assertEqual(
-            [
-                x.extract()
-                for x in sel.xpath('//a[re:test(@href, "second")]/text()')
-            ],
+            [x.extract() for x in sel.xpath('//a[re:test(@href, "second")]/text()')],
             ["second link"],
         )
 
         # re:match() is rather special: it returns a node-set of <match> nodes
         # ['<match>http://www.bayes.co.uk/xml/index.xml?/xml/utils/rechecker.xml</match>',
         # '<match>http</match>',
         # '<match>www.bayes.co.uk</match>',
@@ -1321,17 +1252,15 @@
 
         # re:replace()
         self.assertEqual(
             sel.xpath(
                 r're:replace(//a[re:test(@href, "\.xml$")]/@href,'
                 r'"(\w+)://(.+)(\.xml)", "","https://\2.html")'
             ).extract(),
-            [
-                "https://www.bayes.co.uk/xml/index.xml?/xml/utils/rechecker.html"
-            ],
+            ["https://www.bayes.co.uk/xml/index.xml?/xml/utils/rechecker.html"],
         )
 
     def test_set(self) -> None:
         """EXSLT set manipulation tests"""
         # microdata example from http://schema.org/Event
         body = """
         <div itemscope itemtype="http://schema.org/Event">
```

### Comparing `parsel-1.8.1/tests/test_selector_csstranslator.py` & `parsel-1.9.0/tests/test_selector_csstranslator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Selector tests for cssselect backend
 """
+
 import unittest
-from typing import TYPE_CHECKING, Any, Callable, List, Type
+from typing import Any, Callable, List, Protocol, Tuple, Type, Union
 
 import cssselect
 import pytest
-from packaging.version import Version
-
-from parsel.csstranslator import GenericTranslator, HTMLTranslator
-from parsel import Selector
 from cssselect.parser import SelectorSyntaxError
 from cssselect.xpath import ExpressionError
+from packaging.version import Version
 
+from parsel import Selector
+from parsel.csstranslator import GenericTranslator, HTMLTranslator, TranslatorProtocol
 
 HTMLBODY = """
 <html>
 <body>
 <div>
  <a id="name-anchor" name="foo"></a>
  <a id="tag-anchor" rel="tag" href="http://localhost/foo">link</a>
@@ -46,69 +46,62 @@
 <div class="cool-footer" id="foobar-div" foobar="ab bc cde">
     <span id="foobar-span">foo ter</span>
 </div>
 </body></html>
 """
 
 
-if TYPE_CHECKING:
-    # requires Python 3.8
-    from typing import Protocol
-
-    from parsel.csstranslator import TranslatorProtocol
-
-    class TranslatorTestProtocol(Protocol):
-        tr_cls: Type[TranslatorProtocol]
-        tr: TranslatorProtocol
-
-        def c2x(self, css: str, prefix: str = ...) -> str:
-            pass
-
-        def assertEqual(self, first: Any, second: Any, msg: Any = ...) -> None:
-            pass
-
-        def assertRaises(
-            self,
-            expected_exception: type[BaseException]
-            | tuple[type[BaseException], ...],
-            callable: Callable[..., object],
-            *args: Any,
-            **kwargs: Any,
-        ) -> None:
-            pass
+class TranslatorTestProtocol(Protocol):
+    tr_cls: Type[TranslatorProtocol]
+    tr: TranslatorProtocol
+
+    def c2x(self, css: str, prefix: str = ...) -> str:
+        pass
+
+    def assertEqual(self, first: Any, second: Any, msg: Any = ...) -> None:
+        pass
+
+    def assertRaises(
+        self,
+        expected_exception: Union[Type[BaseException], Tuple[Type[BaseException], ...]],
+        callable: Callable[..., object],
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        pass
 
 
 class TranslatorTestMixin:
-    def setUp(self: "TranslatorTestProtocol") -> None:
+    def setUp(self: TranslatorTestProtocol) -> None:
         self.tr = self.tr_cls()
         self.c2x = self.tr.css_to_xpath
 
-    def test_attr_function(self: "TranslatorTestProtocol") -> None:
+    def test_attr_function(self: TranslatorTestProtocol) -> None:
         cases = [
             ("::attr(name)", "descendant-or-self::*/@name"),
             ("a::attr(href)", "descendant-or-self::a/@href"),
             (
                 "a ::attr(img)",
                 "descendant-or-self::a/descendant-or-self::*/@img",
             ),
             ("a > ::attr(class)", "descendant-or-self::a/*/@class"),
         ]
         for css, xpath in cases:
             self.assertEqual(self.c2x(css), xpath, css)
 
-    def test_attr_function_exception(self: "TranslatorTestProtocol") -> None:
+    def test_attr_function_exception(self: TranslatorTestProtocol) -> None:
         cases = [
             ("::attr(12)", ExpressionError),
             ("::attr(34test)", ExpressionError),
             ("::attr(@href)", SelectorSyntaxError),
         ]
         for css, exc in cases:
             self.assertRaises(exc, self.c2x, css)
 
-    def test_text_pseudo_element(self: "TranslatorTestProtocol") -> None:
+    def test_text_pseudo_element(self: TranslatorTestProtocol) -> None:
         cases = [
             ("::text", "descendant-or-self::text()"),
             ("p::text", "descendant-or-self::p/text()"),
             ("p ::text", "descendant-or-self::p/descendant-or-self::text()"),
             ("#id::text", "descendant-or-self::*[@id = 'id']/text()"),
             ("p#id::text", "descendant-or-self::p[@id = 'id']/text()"),
             (
@@ -129,31 +122,31 @@
                 "p::text, a::text",
                 "descendant-or-self::p/text() | descendant-or-self::a/text()",
             ),
         ]
         for css, xpath in cases:
             self.assertEqual(self.c2x(css), xpath, css)
 
-    def test_pseudo_function_exception(self: "TranslatorTestProtocol") -> None:
+    def test_pseudo_function_exception(self: TranslatorTestProtocol) -> None:
         cases = [
             ("::attribute(12)", ExpressionError),
             ("::text()", ExpressionError),
             ("::attr(@href)", SelectorSyntaxError),
         ]
         for css, exc in cases:
             self.assertRaises(exc, self.c2x, css)
 
-    def test_unknown_pseudo_element(self: "TranslatorTestProtocol") -> None:
+    def test_unknown_pseudo_element(self: TranslatorTestProtocol) -> None:
         cases = [
             ("::text-node", ExpressionError),
         ]
         for css, exc in cases:
             self.assertRaises(exc, self.c2x, css)
 
-    def test_unknown_pseudo_class(self: "TranslatorTestProtocol") -> None:
+    def test_unknown_pseudo_class(self: TranslatorTestProtocol) -> None:
         cases = [
             (":text", ExpressionError),
             (":attribute(name)", ExpressionError),
         ]
         for css, exc in cases:
             self.assertRaises(exc, self.c2x, css)
 
@@ -181,17 +174,15 @@
 
     sscls = Selector
 
     def setUp(self) -> None:
         self.sel = self.sscls(text=HTMLBODY)
 
     def x(self, *a: Any, **kw: Any) -> List[str]:
-        return [
-            v.strip() for v in self.sel.css(*a, **kw).extract() if v.strip()
-        ]
+        return [v.strip() for v in self.sel.css(*a, **kw).extract() if v.strip()]
 
     def test_selector_simple(self) -> None:
         for x in self.sel.css("input"):
             self.assertTrue(isinstance(x, self.sel.__class__), x)
         self.assertEqual(
             self.sel.css("input").extract(),
             [x.extract() for x in self.sel.css("input")],
@@ -203,32 +194,28 @@
         self.assertEqual(self.x("#p-b2 ::text"), ["guy"])
         self.assertEqual(self.x("#paragraph::text"), ["lorem ipsum text"])
         self.assertEqual(
             self.x("#paragraph ::text"),
             ["lorem ipsum text", "hi", "there", "guy"],
         )
         self.assertEqual(self.x("p::text"), ["lorem ipsum text"])
-        self.assertEqual(
-            self.x("p ::text"), ["lorem ipsum text", "hi", "there", "guy"]
-        )
+        self.assertEqual(self.x("p ::text"), ["lorem ipsum text", "hi", "there", "guy"])
 
     def test_attribute_function(self) -> None:
         self.assertEqual(self.x("#p-b2::attr(id)"), ["p-b2"])
         self.assertEqual(self.x(".cool-footer::attr(class)"), ["cool-footer"])
         self.assertEqual(
             self.x(".cool-footer ::attr(id)"), ["foobar-div", "foobar-span"]
         )
         self.assertEqual(
             self.x('map[name="dummymap"] ::attr(shape)'), ["circle", "default"]
         )
 
     def test_nested_selector(self) -> None:
-        self.assertEqual(
-            self.sel.css("p").css("b::text").extract(), ["hi", "guy"]
-        )
+        self.assertEqual(self.sel.css("p").css("b::text").extract(), ["hi", "guy"])
         self.assertEqual(
             self.sel.css("div").css("area:last-child").extract(),
             ['<area shape="default" id="area-nohref">'],
         )
 
     @pytest.mark.xfail(
         Version(cssselect.__version__) < Version("1.2.0"),
```

### Comparing `parsel-1.8.1/tests/test_selector_jmespath.py` & `parsel-1.9.0/tests/test_selector_jmespath.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,20 +39,16 @@
             sel.jmespath("html").get(),
             "<div><a>a<br>b</a>c</div><div><a>d</a>e<b>f</b></div>",
         )
         self.assertEqual(
             sel.jmespath("html").xpath("//div/a/text()").getall(),
             ["a", "b", "d"],
         )
-        self.assertEqual(
-            sel.jmespath("html").css("div > b").getall(), ["<b>f</b>"]
-        )
-        self.assertEqual(
-            sel.jmespath("content").jmespath("name.age").get(), 18
-        )
+        self.assertEqual(sel.jmespath("html").css("div > b").getall(), ["<b>f</b>"])
+        self.assertEqual(sel.jmespath("content").jmespath("name.age").get(), 18)
 
     def test_html_has_json(self) -> None:
         html_text = """
         <div>
             <h1>Information</h1>
             <content>
             {
@@ -78,17 +74,15 @@
               "status": "ok"
             }
             </content>
         </div>
         """
         sel = Selector(text=html_text)
         self.assertEqual(
-            sel.xpath("//div/content/text()")
-            .jmespath("user[*].name")
-            .getall(),
+            sel.xpath("//div/content/text()").jmespath("user[*].name").getall(),
             ["A", "B", "C", "D"],
         )
         self.assertEqual(
             sel.xpath("//div/content").jmespath("user[*].name").getall(),
             ["A", "B", "C", "D"],
         )
         self.assertEqual(sel.xpath("//div/content").jmespath("total").get(), 4)
@@ -121,17 +115,15 @@
                   "status": "ok"
                 }
                 </content>
             </div>
             """
         sel = Selector(text=html_text)
         self.assertEqual(
-            sel.xpath("//div/content/text()")
-            .jmespath("user[*].name")
-            .re(r"(\w+)"),
+            sel.xpath("//div/content/text()").jmespath("user[*].name").re(r"(\w+)"),
             ["A", "B", "C", "D"],
         )
         self.assertEqual(
             sel.xpath("//div/content").jmespath("user[*].name").re(r"(\w+)"),
             ["A", "B", "C", "D"],
         )
 
@@ -139,17 +131,15 @@
             sel.xpath("//div/content").jmespath("user[*].age").re(r"(\d+)")
 
         self.assertEqual(
             sel.xpath("//div/content").jmespath("unavailable").re(r"(\d+)"), []
         )
 
         self.assertEqual(
-            sel.xpath("//div/content")
-            .jmespath("unavailable")
-            .re_first(r"(\d+)"),
+            sel.xpath("//div/content").jmespath("unavailable").re_first(r"(\d+)"),
             None,
         )
 
         self.assertEqual(
             sel.xpath("//div/content")
             .jmespath("user[*].age.to_string(@)")
             .re(r"(\d+)"),
@@ -167,18 +157,14 @@
             ("1", 1),
             ("true", True),
             ("false", False),
             ("null", None),
         ):
             selector = Selector(text=text, root=_NOT_SET)
             self.assertEqual(selector.type, "json")
-            self.assertEqual(
-                selector._text, text  # pylint: disable=protected-access
-            )
+            self.assertEqual(selector._text, text)  # pylint: disable=protected-access
             self.assertEqual(selector.root, root)
 
             selector = Selector(text=None, root=root)
             self.assertEqual(selector.type, "json")
-            self.assertEqual(
-                selector._text, None  # pylint: disable=protected-access
-            )
+            self.assertEqual(selector._text, None)  # pylint: disable=protected-access
             self.assertEqual(selector.root, root)
```

### Comparing `parsel-1.8.1/tests/test_utils.py` & `parsel-1.9.0/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Pattern, List, Type, Union
-
-from parsel.utils import shorten, extract_regex
+from typing import List, Pattern, Type, Union
 
 from pytest import mark, raises
 
+from parsel.utils import extract_regex, shorten
+
 
 @mark.parametrize(
     "width,expected",
     (
         (-1, ValueError),
         (0, ""),
         (1, "."),
```

### Comparing `parsel-1.8.1/tests/test_xml_attacks.py` & `parsel-1.9.0/tests/test_xml_attacks.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from os import path
 from unittest import TestCase
 
 from psutil import Process
 
 from parsel import Selector
 
-
 MiB_1 = 1024**2
 
 
 def _load(attack: str) -> str:
     folder_path = path.dirname(__file__)
     file_path = path.join(folder_path, "xml_attacks", f"{attack}.xml")
     with open(file_path, "rb") as attack_file:
```

### Comparing `parsel-1.8.1/tests/test_xpathfuncs.py` & `parsel-1.9.0/tests/test_xpathfuncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Any
 import unittest
+from typing import Any
 
 from parsel import Selector
 from parsel.xpathfuncs import set_xpathfunc
 
 
 class XPathFuncsTestCase(unittest.TestCase):
     def test_has_class_simple(self) -> None:
@@ -19,25 +19,19 @@
             ["First", "Second"],
         )
         self.assertEqual(
             [x.extract() for x in sel.xpath('//p[has-class("bar")]/text()')],
             ["Third"],
         )
         self.assertEqual(
-            [
-                x.extract()
-                for x in sel.xpath('//p[has-class("foo","bar")]/text()')
-            ],
+            [x.extract() for x in sel.xpath('//p[has-class("foo","bar")]/text()')],
             [],
         )
         self.assertEqual(
-            [
-                x.extract()
-                for x in sel.xpath('//p[has-class("foo","bar-baz")]/text()')
-            ],
+            [x.extract() for x in sel.xpath('//p[has-class("foo","bar-baz")]/text()')],
             ["First"],
         )
 
     def test_has_class_error_no_args(self) -> None:
         body = """
         <p CLASS="foo">First</p>
         """
```

### Comparing `parsel-1.8.1/tests/typing/selector.py` & `parsel-1.9.0/tests/typing/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Basic usage of the Selector, strongly typed to test the typing of parsel's API.
 import re
+from typing import List
+
 from parsel import Selector
 
 
 def correct() -> None:
     selector = Selector(
         text="<html><body><ul><li>1</li><li>2</li><li>3</li></ul></body></html>"
     )
 
-    li_values: list[str] = selector.css("li").getall()
+    li_values: List[str] = selector.css("li").getall()
     selector.re_first(re.compile(r"[32]"), "").strip()
-    xpath_values: list[str] = selector.xpath(
+    xpath_values: List[str] = selector.xpath(
         "//somens:a/text()", namespaces={"somens": "http://scrapy.org"}
     ).extract()
 
     class MySelector(Selector):
         def my_own_func(self) -> int:
             return 3
```

### Comparing `parsel-1.8.1/tests/xml_attacks/billion_laughs.xml` & `parsel-1.9.0/tests/xml_attacks/billion_laughs.xml`

 * *Files identical despite different names*

