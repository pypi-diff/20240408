# Comparing `tmp/markdown_convert-0.9.6.tar.gz` & `tmp/markdown_convert-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-0.9.6.tar", max compression
+gzip compressed data, was "markdown_convert-0.9.8.tar", max compression
```

## Comparing `markdown_convert-0.9.6.tar` & `markdown_convert-0.9.8.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-0.9.6/LICENSE
--rw-r--r--   0        0        0     1631 2023-10-23 17:37:06.761873 markdown_convert-0.9.6/README.md
--rw-r--r--   0        0        0      315 2023-10-23 17:37:06.761873 markdown_convert-0.9.6/markdown_convert/__init__.py
--rw-r--r--   0        0        0     1071 2023-10-23 17:37:06.761873 markdown_convert-0.9.6/markdown_convert/default.css
--rw-r--r--   0        0        0     6871 2023-10-23 17:37:06.761873 markdown_convert-0.9.6/markdown_convert/markdown_convert.py
--rw-r--r--   0        0        0      670 2023-10-23 18:37:48.745222 markdown_convert-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     2419 1970-01-01 00:00:00.000000 markdown_convert-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-0.9.8/LICENSE
+-rw-r--r--   0        0        0     1531 2024-04-08 21:24:43.477483 markdown_convert-0.9.8/README.md
+-rw-r--r--   0        0        0      183 2024-04-08 21:28:46.972862 markdown_convert-0.9.8/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2823 2024-04-08 14:55:19.194948 markdown_convert-0.9.8/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-0.9.8/markdown_convert/code.css
+-rw-r--r--   0        0        0     5481 2024-04-08 19:33:11.286944 markdown_convert-0.9.8/markdown_convert/default.css
+-rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-0.9.8/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-0.9.8/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     3900 2024-04-08 19:10:52.451331 markdown_convert-0.9.8/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2266 2024-04-08 19:10:22.667055 markdown_convert-0.9.8/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      316 2024-04-08 14:38:44.344993 markdown_convert-0.9.8/markdown_convert/modules/utils_strings.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-0.9.8/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      658 2024-04-08 21:30:39.962970 markdown_convert-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 markdown_convert-0.9.8/PKG-INFO
```

### Comparing `markdown_convert-0.9.6/LICENSE` & `markdown_convert-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.6/pyproject.toml` & `markdown_convert-0.9.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "0.9.6"
-description = "Python package to convert Markdown files to other formats."
+version = "0.9.8"
+description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
-include = ["markdown_convert/default.css"]
+include = ["markdown_convert/default.css", "markdown_convert/code.css"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<=4.0"
-Markdown = { version = ">=3.3.0,<=4.0.0" }
-PyMuPDF = { version = ">=1.23.5,<=2.0.0" }
-watchdog = { version = ">=3.0.0,<=4.0.0" }
+python = ">=3.8,<4.0"
+argsdict = "1.0.0"
+setuptools = "^49.6.0"
+weasyprint = "^61.2"
+markdown2 = "^2.4.13"
 
 [tool.poetry.scripts]
-markdown-convert = "markdown_convert:main"
+markdown-convert = "markdown_convert.__main__:main"
```

### Comparing `markdown_convert-0.9.6/PKG-INFO` & `markdown_convert-0.9.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,69 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 0.9.6
-Summary: Python package to convert Markdown files to other formats.
+Version: 0.9.8
+Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
-Requires-Python: >=3.8,<=4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Markdown (>=3.3.0,<=4.0.0)
-Requires-Dist: PyMuPDF (>=1.23.5,<=2.0.0)
-Requires-Dist: watchdog (>=3.0.0,<=4.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: argsdict (==1.0.0)
+Requires-Dist: markdown2 (>=2.4.13,<3.0.0)
+Requires-Dist: setuptools (>=49.6.0,<50.0.0)
+Requires-Dist: weasyprint (>=61.2,<62.0)
 Description-Content-Type: text/markdown
 
 # markdown-convert
 
-_Python package to convert Markdown files to other formats._
+_Convert Markdown files to PDF from your command line._
 
-<br>
-<p align="center">
-  <img width="600" src="https://i.imgur.com/VZJc4cN.png">
-</p>
-<br>
+### `pip install markdown-convert`
+<img src='https://i.imgur.com/UuJL8Ls.png' width='80%'>
 
-With `markdown-convert`, you can easily convert a Markdown file to PDF
-with the following features:
+`markdown-convert` is an elegant command-line tool that converts Markdown files to PDF.
 
-- User-defined CSS styles.
-- Customizable document margins.
-- Live PDF compilation.
-- Manual insertion of page breaks.
+It is powered by the amazing `markdown2` and `weasyprint` libraries, and unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies.
 
-To start using it, simply `pip install markdown-convert`.
+### Features
 
-<br>
+- Supports live compilation, so you can preview your PDF in real-time as you type.
+- Comes with beautiful CSS out of the box, making your documents look great from the start.
+- Syntax highlighting for code blocks included.
+- Designed for the 21st century, with relative links, pipe tables, and modern CSS paged media features.
 
-## Usage example
+### Usage
 
-```python
-from markdown_convert import MarkdownFile
-
-MarkdownFile("markdown.md").to_pdf()    # One time conversion
-MarkdownFile("markdown.md").live_pdf()  # Real-time conversion
-```
-
-<br>
-
-## Documentation
-
-### MarkdownFile
-
-#### __init__
-
-- `md_path` - Path to the Markdown file.
-- `css_path='css/default.css'` - Path to the CSS file.
-- `margin_h=62` - Horizontal margin of the PDF file.
-- `margin_v=60` - Vertical margin of the PDF file.
-
-#### use
-
-- `plugin` - Name of the [extension](https://python-markdown.github.io/extensions/) to add to the set of used extensions.
+Run `markdown-convert -h` right from your terminal to check out the available options:
 
-  > The extensions `extra` and `sane_lists` are included by default.
+```bash
+Usage:
+  markdown-convert [markdown_file_path] [options]
 
-#### to_html
-
-- `output_path=None` - Path to the output HTML file.
-
-  > If not specified, the HTML file will have the same name, but with the `.html` extension.
-
-#### to_pdf
-
-- `output_path=None` - Path to the output PDF file.
-
-  > If not specified, the PDF file will have the same name, but with the `.pdf` extension.
-
-#### live_pdf
+Options:
+  --mode=once|live
+    Convert the markdown file once (default) or live.
+  --css=[css_file_path]
+    Use a custom CSS file.
+  --out=[output_file_path]
+    Specify the output file path.
+```
 
-- (Takes no arguments).
+...or import any of the functions from the package to use them in your own code:
 
-  > The PDF file will be updated whenever the Markdown file changes on disk.
+```python
+from markdown_convert import convert, live_convert
 
-<br>
+# Convert your Markdown file to PDF once
+convert('README.md', "style.css", 'README.pdf')
 
-## Contributing
+# Convert your Markdown file to PDF every time it changes
+live_convert('README.md', "style.css", 'README.pdf')
+```
 
-See [CONTRIBUTING.md](.github/CONTRIBUTING.md).
```

