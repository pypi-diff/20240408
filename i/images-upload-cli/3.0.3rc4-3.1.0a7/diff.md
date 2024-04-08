# Comparing `tmp/images_upload_cli-3.0.3rc4.tar.gz` & `tmp/images_upload_cli-3.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "images_upload_cli-3.0.3rc4.tar", max compression
+gzip compressed data, was "images_upload_cli-3.1.0a7.tar", max compression
```

## Comparing `images_upload_cli-3.0.3rc4.tar` & `images_upload_cli-3.1.0a7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/LICENSE
--rw-r--r--   0        0        0     6440 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/README.md
--rw-r--r--   0        0        0     3809 2024-04-03 21:31:22.763785 images_upload_cli-3.0.3rc4/pyproject.toml
--rw-r--r--   0        0        0      207 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/__init__.py
--rw-r--r--   0        0        0      158 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/__main__.py
--rw-r--r--   0        0        0     3395 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/_cli.py
--rw-r--r--   0        0        0     3304 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/image.py
--rw-r--r--   0        0        0     1217 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/logger.py
--rw-r--r--   0        0        0     2982 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/main.py
--rw-r--r--   0        0        0    19146 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/upload.py
--rw-r--r--   0        0        0     2534 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/util.py
--rw-r--r--   0        0        0     7556 1970-01-01 00:00:00.000000 images_upload_cli-3.0.3rc4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 20:51:23.935191 images_upload_cli-3.1.0a7/LICENSE
+-rw-r--r--   0        0        0     6440 2024-04-08 20:51:23.935191 images_upload_cli-3.1.0a7/README.md
+-rw-r--r--   0        0        0     3839 2024-04-08 20:51:35.863212 images_upload_cli-3.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-08 20:51:23.935191 images_upload_cli-3.1.0a7/src/images_upload_cli/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-08 20:51:23.939191 images_upload_cli-3.1.0a7/src/images_upload_cli/__main__.py
+-rw-r--r--   0        0        0     3395 2024-04-08 20:51:23.939191 images_upload_cli-3.1.0a7/src/images_upload_cli/_cli.py
+-rw-r--r--   0        0        0     3304 2024-04-08 20:51:23.939191 images_upload_cli-3.1.0a7/src/images_upload_cli/image.py
+-rw-r--r--   0        0        0     1217 2024-04-08 20:51:23.939191 images_upload_cli-3.1.0a7/src/images_upload_cli/logger.py
+-rw-r--r--   0        0        0     2982 2024-04-08 20:51:23.939191 images_upload_cli-3.1.0a7/src/images_upload_cli/main.py
+-rw-r--r--   0        0        0    19146 2024-04-08 20:51:23.939191 images_upload_cli-3.1.0a7/src/images_upload_cli/upload.py
+-rw-r--r--   0        0        0     2534 2024-04-08 20:51:23.939191 images_upload_cli-3.1.0a7/src/images_upload_cli/util.py
+-rw-r--r--   0        0        0     7555 1970-01-01 00:00:00.000000 images_upload_cli-3.1.0a7/PKG-INFO
```

### Comparing `images_upload_cli-3.0.3rc4/LICENSE` & `images_upload_cli-3.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc4/README.md` & `images_upload_cli-3.1.0a7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 > Upload images via APIs
 
 [![PyPI: Version](https://img.shields.io/pypi/v/images-upload-cli?logo=pypi&logoColor=white)](https://pypi.org/project/images-upload-cli)
 [![AUR: version](https://img.shields.io/aur/version/python-images-upload-cli?logo=archlinux&logoColor=white)](https://aur.archlinux.org/packages/python-images-upload-cli)
 [![GitHub: Release](https://img.shields.io/github/v/release/deadnews/images-upload-cli?logo=github&logoColor=white)](https://github.com/deadnews/images-upload-cli/releases/latest)
 [![Documentation](https://img.shields.io/badge/documentation-gray.svg?logo=materialformkdocs&logoColor=white)](https://deadnews.github.io/images-upload-cli)
 [![CI: pre-commit](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/deadnews/images-upload-cli/main)
-[![CI: main](https://img.shields.io/github/actions/workflow/status/deadnews/images-upload-cli/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/images-upload-cli/actions/workflows/main.yml)
-[![CI: coverage](https://img.shields.io/codecov/c/github/deadnews/images-upload-cli?token=OCZDZIYPMC&logo=codecov&logoColor=white)](https://app.codecov.io/gh/deadnews/images-upload-cli)
+[![CI: Main](https://img.shields.io/github/actions/workflow/status/deadnews/images-upload-cli/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/images-upload-cli/actions/workflows/main.yml)
+[![CI: Coverage](https://img.shields.io/codecov/c/github/deadnews/images-upload-cli?token=OCZDZIYPMC&logo=codecov&logoColor=white)](https://app.codecov.io/gh/deadnews/images-upload-cli)
 
 **[Installation](#installation)** • **[Hostings](#hostings)** • **[Usage](#usage)** • **[Env Variables](#env-variables)**
 
 ## Installation
 
 PyPI
```

### Comparing `images_upload_cli-3.0.3rc4/pyproject.toml` & `images_upload_cli-3.1.0a7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "images-upload-cli"
-version = "3.0.3-rc.4"
+version = "3.1.0-alpha.7"
 description = "Upload images via APIs"
 authors = ["DeadNews <deadnewsgit@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/images-upload-cli"
 repository = "https://github.com/DeadNews/images-upload-cli"
 documentation = "https://deadnews.github.io/images-upload-cli"
@@ -45,19 +45,19 @@
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-click = "^0.8.1"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.1"
 mkdocs-material = "^9.5.17"
-mkdocstrings = "^0.24.2"
+mkdocstrings = "^0.24.3"
 mkdocstrings-python = "^1.9.2"
 
 [tool.poetry.group.build.dependencies]
-nuitka = "^2.1.4"
+nuitka = { version = "^2.1.5", platform = "win32" }
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poe.tasks]
@@ -69,22 +69,22 @@
 
 [tool.poe.tasks.nuitka]
 cmd = """
 python -m nuitka
   --assume-yes-for-downloads
   --onefile
   --output-dir=dist
-  --output-file=${output-file}
+  --output-file=${outfile}
   --script-name=src/images_upload_cli/__main__.py
 """
 
-[tool.poe.tasks.nuitka.args.output-file]
+[tool.poe.tasks.nuitka.args.outfile]
 options = ["--output-file"]
-default = "images-upload-cli.bin"
-help = "Output file name"
+default = "images-upload-cli.exe"
+help = "Output file name."
 
 [tool.poe.tasks.test]
 cmd = "pytest -m 'not (online or benchmark)'"
 
 [tool.poe.tasks.benchmark]
 cmd = "pytest -m 'benchmark and not online' --benchmark-autosave --benchmark-compare"
```

### Comparing `images_upload_cli-3.0.3rc4/src/images_upload_cli/_cli.py` & `images_upload_cli-3.1.0a7/src/images_upload_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc4/src/images_upload_cli/image.py` & `images_upload_cli-3.1.0a7/src/images_upload_cli/image.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc4/src/images_upload_cli/logger.py` & `images_upload_cli-3.1.0a7/src/images_upload_cli/logger.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc4/src/images_upload_cli/main.py` & `images_upload_cli-3.1.0a7/src/images_upload_cli/main.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc4/src/images_upload_cli/upload.py` & `images_upload_cli-3.1.0a7/src/images_upload_cli/upload.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc4/src/images_upload_cli/util.py` & `images_upload_cli-3.1.0a7/src/images_upload_cli/util.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc4/PKG-INFO` & `images_upload_cli-3.1.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: images-upload-cli
-Version: 3.0.3rc4
+Version: 3.1.0a7
 Summary: Upload images via APIs
 Home-page: https://github.com/DeadNews/images-upload-cli
 License: MIT
 Keywords: cli,imgur,image-upload,upload-images,upload-pictures
 Author: DeadNews
 Author-email: deadnewsgit@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -31,16 +31,16 @@
 > Upload images via APIs
 
 [![PyPI: Version](https://img.shields.io/pypi/v/images-upload-cli?logo=pypi&logoColor=white)](https://pypi.org/project/images-upload-cli)
 [![AUR: version](https://img.shields.io/aur/version/python-images-upload-cli?logo=archlinux&logoColor=white)](https://aur.archlinux.org/packages/python-images-upload-cli)
 [![GitHub: Release](https://img.shields.io/github/v/release/deadnews/images-upload-cli?logo=github&logoColor=white)](https://github.com/deadnews/images-upload-cli/releases/latest)
 [![Documentation](https://img.shields.io/badge/documentation-gray.svg?logo=materialformkdocs&logoColor=white)](https://deadnews.github.io/images-upload-cli)
 [![CI: pre-commit](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/deadnews/images-upload-cli/main)
-[![CI: main](https://img.shields.io/github/actions/workflow/status/deadnews/images-upload-cli/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/images-upload-cli/actions/workflows/main.yml)
-[![CI: coverage](https://img.shields.io/codecov/c/github/deadnews/images-upload-cli?token=OCZDZIYPMC&logo=codecov&logoColor=white)](https://app.codecov.io/gh/deadnews/images-upload-cli)
+[![CI: Main](https://img.shields.io/github/actions/workflow/status/deadnews/images-upload-cli/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/images-upload-cli/actions/workflows/main.yml)
+[![CI: Coverage](https://img.shields.io/codecov/c/github/deadnews/images-upload-cli?token=OCZDZIYPMC&logo=codecov&logoColor=white)](https://app.codecov.io/gh/deadnews/images-upload-cli)
 
 **[Installation](#installation)** • **[Hostings](#hostings)** • **[Usage](#usage)** • **[Env Variables](#env-variables)**
 
 ## Installation
 
 PyPI
```

