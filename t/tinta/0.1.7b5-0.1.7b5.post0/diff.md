# Comparing `tmp/tinta-0.1.7b5.tar.gz` & `tmp/tinta-0.1.7b5.post0.tar.gz`

## Comparing `tinta-0.1.7b5.tar` & `tinta-0.1.7b5.post0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.gitattributes
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.pylintrc
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.7b5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.7b5/DESCRIPTION.rst
--rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tinta-0.1.7b5/HIPPOCRATIC_LICENSE.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.7b5/MANIFEST.in
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tinta-0.1.7b5/Pipfile
--rw-r--r--   0        0        0    39666 2020-02-02 00:00:00.000000 tinta-0.1.7b5/Pipfile.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b5/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 tinta-0.1.7b5/requirements-dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b5/requirements.txt
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 tinta-0.1.7b5/setup.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.github/workflows/publish-test.yml
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.vscode/launch.json
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.vscode/settings.json
--rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.vscode/tasks.json
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 tinta-0.1.7b5/examples/basic_example.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.7b5/examples/colors.ini
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 tinta-0.1.7b5/examples/complete_example.py
--rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.7b5/examples/tinta-discover.png
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 tinta-0.1.7b5/junit/test-results.xml
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tests/conftest.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tests/test_colors_invalid.ini
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tests/test_discover.py
--rw-r--r--   0        0        0    36199 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tests/test_tinta.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/__main__.py
--rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/ansi.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/colors.ini
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/constants.py
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/discover.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/multi_version_imports.py
--rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/stylize.py
--rw-r--r--   0        0        0    28887 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/tinta.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/typ.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 tinta-0.1.7b5/tinta/utils.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tinta-0.1.7b5/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.7b5/LICENSE
--rw-r--r--   0        0        0    13519 2020-02-02 00:00:00.000000 tinta-0.1.7b5/README.md
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 tinta-0.1.7b5/pyproject.toml
--rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 tinta-0.1.7b5/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/.gitattributes
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/.pylintrc
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/DESCRIPTION.rst
+-rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/HIPPOCRATIC_LICENSE.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/MANIFEST.in
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/Pipfile
+-rw-r--r--   0        0        0    39666 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/Pipfile.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/requirements.txt
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/setup.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/.github/workflows/publish-test.yml
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/.vscode/launch.json
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/.vscode/settings.json
+-rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/.vscode/tasks.json
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/examples/basic_example.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/examples/colors.ini
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/examples/complete_example.py
+-rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/examples/tinta-discover.png
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/junit/test-results.xml
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tests/conftest.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tests/test_colors_invalid.ini
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tests/test_discover.py
+-rw-r--r--   0        0        0    36762 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tests/test_tinta.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tinta/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tinta/__main__.py
+-rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tinta/ansi.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tinta/colors.ini
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tinta/constants.py
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tinta/discover.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tinta/multi_version_imports.py
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tinta/stylize.py
+-rw-r--r--   0        0        0    28921 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tinta/tinta.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tinta/typ.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/tinta/utils.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/LICENSE
+-rw-r--r--   0        0        0    13537 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/README.md
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/pyproject.toml
+-rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 tinta-0.1.7b5.post0/PKG-INFO
```

### Comparing `tinta-0.1.7b5/CODE_OF_CONDUCT.md` & `tinta-0.1.7b5.post0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/HIPPOCRATIC_LICENSE.md` & `tinta-0.1.7b5.post0/HIPPOCRATIC_LICENSE.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/Pipfile.lock` & `tinta-0.1.7b5.post0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/setup.py` & `tinta-0.1.7b5.post0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from setuptools import setup
 
 with Path("README.md").open(encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="tinta",
-    version="0.1.7b5",
+    version="0.1.7b5-post0",
     description="Tinta, a magical console output tool.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/brandonscript/tinta",
     author="Brandon Shelley",
     author_email="brandon@pacificaviator.co",
     install_requires=[],
```

### Comparing `tinta-0.1.7b5/.github/workflows/publish-test.yml` & `tinta-0.1.7b5.post0/.github/workflows/publish-test.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/.github/workflows/publish.yml` & `tinta-0.1.7b5.post0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/.github/workflows/run-tests.yml` & `tinta-0.1.7b5.post0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/.vscode/launch.json` & `tinta-0.1.7b5.post0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/.vscode/settings.json` & `tinta-0.1.7b5.post0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/.vscode/tasks.json` & `tinta-0.1.7b5.post0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/examples/basic_example.py` & `tinta-0.1.7b5.post0/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/examples/complete_example.py` & `tinta-0.1.7b5.post0/examples/complete_example.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/examples/tinta-discover.png` & `tinta-0.1.7b5.post0/examples/tinta-discover.png`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/junit/test-results.xml` & `tinta-0.1.7b5.post0/junit/test-results.xml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/tests/conftest.py` & `tinta-0.1.7b5.post0/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,7 +40,22 @@
 
 @pytest.fixture(scope="session")
 def perf(request):
     import tinta.constants as C
 
     if request.config.option.perf is True:
         C.PERF_MEASURE = True
+
+
+@pytest.fixture(scope="function", autouse=False)
+def alt_colors_ini(tmp_path):
+
+    from tinta import Tinta
+
+    colors_ini = tmp_path / "colors.ini"
+    colors_ini.write_text("""[colors]\nsparkle = 195\ndragons_breath = 202\n""")
+
+    orig_colors_ini = Tinta._colors._colors_ini_path
+
+    Tinta.load_colors(colors_ini)
+    yield colors_ini
+    Tinta.load_colors(orig_colors_ini)
```

### Comparing `tinta-0.1.7b5/tests/test_discover.py` & `tinta-0.1.7b5.post0/tests/test_discover.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/tests/test_tinta.py` & `tinta-0.1.7b5.post0/tests/test_tinta.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,30 @@
 
     def test_init(self):
         assert len(Tinta("initialized").parts) == 1
 
     def test_accepts_string_on_init(self):
         assert Tinta("initialized").to_str() == "initialized"
 
+    def test_load_colors(self, alt_colors_ini):
+        # create a test colors.ini
+
+        # load the colors
+        Tinta.load_colors(alt_colors_ini)
+
+        assert Tinta._colors.color_dict == {"sparkle": 195, "dragons_breath": 202}
+        assert Tinta()._colors.color_list == ["sparkle", "dragons_breath"]
+
+        # check the colors
+        assert Tinta().sparkle("sparkle").to_str() == f"\x1b[38;5;195msparkle{O}"
+        assert (
+            Tinta().dragons_breath("dragon's breath").to_str()
+            == f"\x1b[38;5;202mdragon's breath{O}"
+        )
+
 
 class TestBasicColorizing:
 
     basic_colors = [
         # fmt: off
         ("green", lambda: Tinta().green("green"), f"{GREEN}green{O}"),
         ("green", lambda: Tinta().tint(35, "green"), f"{GREEN}green{O}"),
```

### Comparing `tinta-0.1.7b5/tinta/__init__.py` & `tinta-0.1.7b5.post0/tinta/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 from logging import getLogger
 
-__version__ = "0.1.7b5"
+__version__ = "0.1.7b5-post0"
 
 logger = getLogger(__name__)
 
 try:
     from .tinta import Tinta
 
     assert bool(Tinta)
```

### Comparing `tinta-0.1.7b5/tinta/__main__.py` & `tinta-0.1.7b5.post0/tinta/__main__.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/tinta/ansi.py` & `tinta-0.1.7b5.post0/tinta/ansi.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 def _alias_keys(colors: "Union[AnsiColors, Type[AnsiColors]]", search: str, repl: str):
     """Sets up an alias key for a color."""
 
     for k in (k for k in colors_ini["colors"].keys() if search.lower() in k.lower()):
         alias_key = k.replace(search.lower(), repl.lower())
         if (
             alias_key not in colors_ini["colors"]
-            and alias_key not in colors._dict_colors
+            and alias_key not in colors._color_dict
         ):
-            colors._dict_colors[alias_key] = int(colors_ini["colors"][k])
+            colors._color_dict[alias_key] = int(colors_ini["colors"][k])
             colors_ini["colors"][alias_key] = colors_ini["colors"][k]
 
 
 def _check_path(path: Optional[Union[str, Path]] = None):
     """Loads colors from a file."""
     path = Path(path) if path else Path(__file__).parent / "colors.ini"
     if not path.is_absolute():
@@ -75,31 +75,31 @@
 
     You can change the colors the terminal outputs by changing the
     ANSI values in colors.ini.
     """
 
     _initialized = False
     _colors_ini_path = None
-    _dict_colors: Dict[str, int] = {}
-    _list_colors: List[str] = []
+    _color_dict: Dict[str, int] = {}
 
     def __init__(self, path: Optional[Union[str, Path]] = None):
 
         if not AnsiColors._initialized:
             path = _check_path(path)
             AnsiColors.load_colors(path)
             AnsiColors._colors_ini_path = path
             AnsiColors._initialized = True
 
     @classmethod
     def load_colors(cls, path: Union[str, Path]):
         """Loads colors from a file."""
 
+        colors_ini["colors"] = {}
         colors_ini.read(path)
-        cls._dict_colors = {k: int(v) for (k, v) in colors_ini["colors"].items()}
+        cls._color_dict = {k: int(v) for (k, v) in colors_ini["colors"].items()}
         # Check if any of the color names loaded match the built-in methods. If so, raise an error.
         # for col in loaded_colors.keys():
         #     if hasattr(cls, col):
         #         # and not str(getattr(cls, col)).startswith(
         #         #     "functools.partial(<bound method Tinta.tint"
         #         # ):
         #         # if the color is a 'tint' method, update it
@@ -126,18 +126,18 @@
 
         if color == "default":
             return 0
 
         if is_ansi_str(color):
             return ansi_color_to_int(color)
 
-        if color not in self._dict_colors:
+        if color not in self._color_dict:
             raise MissingColorError(f"Color '{color}' not found in colors.ini.")
 
-        return self._dict_colors[color]
+        return self._color_dict[color]
 
     def reverse_get(self, code: int, ignore_errors: bool = False) -> str:
         """Returns the color name for an ANSI code.
 
         Args:
             code (int): An ANSI code.
             ignore_errors (bool, optional): If True, will return None if the code is not found. Defaults to False.
@@ -145,27 +145,29 @@
         Returns:
             str: The color name for the code.
         """
 
         if code == 0:
             return "default"
 
-        for k, v in self._dict_colors.items():
+        for k, v in self._color_dict.items():
             if v == code:
                 return k
 
         if not ignore_errors:
             raise MissingColorError(
                 f"Color with ANSI code '{code}' not found in colors.ini."
             )
 
         return "[undefined color]"
 
-    def list_colors(self) -> List[str]:
+    @property
+    def color_list(self) -> List[str]:
         """Returns a list of all colors in the colors.ini file."""
-        return list(self._dict_colors.keys())
+        return list(self.color_dict.keys())
 
-    def dict_colors(self) -> Dict[str, int]:
+    @property
+    def color_dict(self) -> Dict[str, int]:
         """Returns a dictionary of all colors in the colors.ini file."""
-        if not self._dict_colors:
-            self._dict_colors = {k: int(v) for (k, v) in colors_ini["colors"].items()}
-        return self._dict_colors
+        if not self._color_dict:
+            self._color_dict = {k: int(v) for (k, v) in colors_ini["colors"].items()}
+        return self._color_dict
```

### Comparing `tinta-0.1.7b5/tinta/constants.py` & `tinta-0.1.7b5.post0/tinta/constants.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/tinta/discover.py` & `tinta-0.1.7b5.post0/tinta/discover.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/tinta/multi_version_imports.py` & `tinta-0.1.7b5.post0/tinta/multi_version_imports.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/tinta/stylize.py` & `tinta-0.1.7b5.post0/tinta/stylize.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/tinta/tinta.py` & `tinta-0.1.7b5.post0/tinta/tinta.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
         if not cls._initialized:
             cls._colors = AnsiColors()
             cls._initialized = True
 
     def load_colors(cls, path: Union[str, Path]):
         cls._initialized = False
+        AnsiColors._initialized = False
         cls._colors = AnsiColors(path)
 
 
 class Tinta(metaclass=_MetaTinta):
     """Tinta is a magical console output tool with support for printing in
     beautiful colors and with rich formatting, like bold and underline. It's
     so pretty, it's almost like a unicorn.
@@ -113,15 +114,15 @@
             *s: Segments of text to add.
             color (Union[str, int], optional): A color name or ANSI color index. Defaults to None.
             styles (List[str], optional): A list of style strings. Defaults to None.
             sep (str, optional): Used to join strings. Defaults to ' '.
         """
 
         # Inject ANSI helper functions
-        for c in Tinta._colors.dict_colors():
+        for c in Tinta._colors.color_dict:
             if hasattr(self, c) and not str(getattr(self, c)).startswith(
                 "functools.partial(<bound method Tinta.tint"
             ):
                 raise AttributeError(
                     f"Cannot overwrite built-in method '{c}' with color name. Please rename the color in '{Tinta._colors._colors_ini_path}'."
                 )
             setattr(self, c, functools.partial(self.tint, color=c))
@@ -638,15 +639,15 @@
             # if hasattr(self.colors, name):
             #     return cast("Tinta", self.tint(color=name))
 
             # else:
             try:
                 return self.__getattribute__(name)  # type: ignore
             except AttributeError as e:
-                known_colors = "\n - ".join(self._colors.list_colors())
+                known_colors = "\n - ".join(self._colors.color_list)
                 known_colors = f" - {known_colors}"
                 raise AttributeError(
                     f"'{name}' not found.\nDid you try and access a color that doesn't exist? Available colors:\n{known_colors}\n"
                 ) from e
 
         return self.__getattribute__(name)  # type: ignore
```

### Comparing `tinta-0.1.7b5/tinta/typ.py` & `tinta-0.1.7b5.post0/tinta/typ.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/tinta/utils.py` & `tinta-0.1.7b5.post0/tinta/utils.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/.gitignore` & `tinta-0.1.7b5.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/LICENSE` & `tinta-0.1.7b5.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b5/README.md` & `tinta-0.1.7b5.post0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Tinta
 
 <img width="200" alt="Tinta Logo" src="https://user-images.githubusercontent.com/1480253/118584629-38023b80-b74c-11eb-8511-05258af553fb.png" />
 
 Tinta is a magical console output tool with support for printing in beautiful colors and with rich formatting, like bold and underline, using static, chain-able methods. It's so pretty, it's almost like a unicorn!
 
-![version](https://img.shields.io/badge/version-0.1.7b5-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
+![version](https://img.shields.io/badge/version-0.1.7b5-post0-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
 
 ## Features and Tinta Basics
 
 `Tinta` takes a statically typed approach to handling rich-color console output.
 
 In the past you might have fiddled with ANSI colors codes, or passed strings to a generic class, only to discover you typo'd one of them! (Yes, we've all been there).
 
@@ -189,15 +189,15 @@
 
 ### Common Args
 
 All "add" methods (each color and style method, `Tinta()`, `push()`, and `tint`) take the following common args:
 
 - `s (str)` – A sequence of one or more text strings, to be joined together.
 - `sep (str)` – Used to join segment strings. Defaults to `' '`.
-  > _Note: `sep` behavior has been changed in v0.1.7b5 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
+  > _Note: `sep` behavior has been changed in v0.1.7b5-post0 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
 
 For example:
 
 ```python
 Tinta('A set', 'of strings', 'joined', 'with', 'semicolons', sep=';').print()
 ```
 
@@ -224,15 +224,15 @@
 - `parts (list)` — A list of `Tinta.Part` segments, which each have a `fmt`, `pln`, and `esc` attribute.
 - ~~`parts_plaintext (list)` — A list of unstyled text segments.~~
 
 ### Built-in Methods
 
 _See below for detailed usage and arguments._
 
-> (Note: breaking changes in v0.1.7b5 - several methods have been renamed for better semantics).
+> (Note: breaking changes in v0.1.7b5-post0 - several methods have been renamed for better semantics).
 
 - `print()` – Prints to the console.
 - `to_str() -> str` – Returns a joined text string.
 - `discover()` – Prints a list of available colors to the console.
 
 Remember, all of the following methods return the current `Tinta` instance `-> self` so you can chain styles together:
```

### Comparing `tinta-0.1.7b5/pyproject.toml` & `tinta-0.1.7b5.post0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 [project]
 name = "tinta"
-version = "0.1.7b5"
+version = "0.1.7b5-post0"
 description = "Tinta, a magical console output tool."
 authors = [{ name = "Brandon Shelley", email = "brandon@pacificaviator.co" }]
 license = "MIT"
 readme = "README.md"
 dependencies = []
 keywords = [
   "console",
```

### Comparing `tinta-0.1.7b5/PKG-INFO` & `tinta-0.1.7b5.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinta
-Version: 0.1.7b5
+Version: 0.1.7b5.post0
 Summary: Tinta, a magical console output tool.
 Project-URL: homepage, https://github.com/brandonscript/tinta
 Project-URL: repository, https://github.com/brandonscript/tinta
 Author-email: Brandon Shelley <brandon@pacificaviator.co>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ansi,cli,colors,console,development,print,term,terminal
@@ -25,15 +25,15 @@
 
 ## Tinta
 
 <img width="200" alt="Tinta Logo" src="https://user-images.githubusercontent.com/1480253/118584629-38023b80-b74c-11eb-8511-05258af553fb.png" />
 
 Tinta is a magical console output tool with support for printing in beautiful colors and with rich formatting, like bold and underline, using static, chain-able methods. It's so pretty, it's almost like a unicorn!
 
-![version](https://img.shields.io/badge/version-0.1.7b5-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
+![version](https://img.shields.io/badge/version-0.1.7b5-post0-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
 
 ## Features and Tinta Basics
 
 `Tinta` takes a statically typed approach to handling rich-color console output.
 
 In the past you might have fiddled with ANSI colors codes, or passed strings to a generic class, only to discover you typo'd one of them! (Yes, we've all been there).
 
@@ -214,15 +214,15 @@
 
 ### Common Args
 
 All "add" methods (each color and style method, `Tinta()`, `push()`, and `tint`) take the following common args:
 
 - `s (str)` – A sequence of one or more text strings, to be joined together.
 - `sep (str)` – Used to join segment strings. Defaults to `' '`.
-  > _Note: `sep` behavior has been changed in v0.1.7b5 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
+  > _Note: `sep` behavior has been changed in v0.1.7b5-post0 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
 
 For example:
 
 ```python
 Tinta('A set', 'of strings', 'joined', 'with', 'semicolons', sep=';').print()
 ```
 
@@ -249,15 +249,15 @@
 - `parts (list)` — A list of `Tinta.Part` segments, which each have a `fmt`, `pln`, and `esc` attribute.
 - ~~`parts_plaintext (list)` — A list of unstyled text segments.~~
 
 ### Built-in Methods
 
 _See below for detailed usage and arguments._
 
-> (Note: breaking changes in v0.1.7b5 - several methods have been renamed for better semantics).
+> (Note: breaking changes in v0.1.7b5-post0 - several methods have been renamed for better semantics).
 
 - `print()` – Prints to the console.
 - `to_str() -> str` – Returns a joined text string.
 - `discover()` – Prints a list of available colors to the console.
 
 Remember, all of the following methods return the current `Tinta` instance `-> self` so you can chain styles together:
```

