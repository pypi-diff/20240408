# Comparing `tmp/pixi-kernel-0.1.1.tar.gz` & `tmp/pixi-kernel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixi-kernel-0.1.1.tar", last modified: Fri Apr  5 00:29:13 2024, max compression
+gzip compressed data, was "pixi-kernel-0.1.2.tar", last modified: Mon Apr  8 02:39:27 2024, max compression
```

## Comparing `pixi-kernel-0.1.1.tar` & `pixi-kernel-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:29:13.588734 pixi-kernel-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 00:28:53.000000 pixi-kernel-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-05 00:29:13.584734 pixi-kernel-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-05 00:28:53.000000 pixi-kernel-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:29:13.584734 pixi-kernel-0.1.1/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 00:28:53.000000 pixi-kernel-0.1.1/assets/kernel.json
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-05 00:28:53.000000 pixi-kernel-0.1.1/assets/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-05 00:28:53.000000 pixi-kernel-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:29:13.588734 pixi-kernel-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:29:13.584734 pixi-kernel-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:29:13.584734 pixi-kernel-0.1.1/src/pixi_kernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:28:53.000000 pixi-kernel-0.1.1/src/pixi_kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-05 00:28:53.000000 pixi-kernel-0.1.1/src/pixi_kernel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 00:28:53.000000 pixi-kernel-0.1.1/src/pixi_kernel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-05 00:28:53.000000 pixi-kernel-0.1.1/src/pixi_kernel/kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 00:28:53.000000 pixi-kernel-0.1.1/src/pixi_kernel/pixi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:29:13.584734 pixi-kernel-0.1.1/src/pixi_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-05 00:29:13.000000 pixi-kernel-0.1.1/src/pixi_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-05 00:29:13.000000 pixi-kernel-0.1.1/src/pixi_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:29:13.000000 pixi-kernel-0.1.1/src/pixi_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 00:29:13.000000 pixi-kernel-0.1.1/src/pixi_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 00:29:13.000000 pixi-kernel-0.1.1/src/pixi_kernel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:27.624547 pixi-kernel-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-08 02:39:27.620547 pixi-kernel-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:27.620547 pixi-kernel-0.1.2/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/assets/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/assets/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 02:39:27.624547 pixi-kernel-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:27.620547 pixi-kernel-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:27.620547 pixi-kernel-0.1.2/src/pixi_kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/src/pixi_kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/src/pixi_kernel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/src/pixi_kernel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/src/pixi_kernel/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/src/pixi_kernel/pixi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:27.620547 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-08 02:39:27.000000 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-08 02:39:27.000000 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 02:39:27.000000 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 02:39:27.000000 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 02:39:27.000000 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/top_level.txt
```

### Comparing `pixi-kernel-0.1.1/LICENSE` & `pixi-kernel-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pixi-kernel-0.1.1/PKG-INFO` & `pixi-kernel-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pixi-kernel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Jupyter kernel using Pixi for reproducible notebooks
 Author-email: Renan Rodrigues dos Santos <renan.engmec@gmail.com>
 License: MIT
 Project-URL: Documentation, https://github.com/renan-r-santos/pixi-kernel
+Project-URL: Homepage, https://github.com/renan-r-santos/pixi-kernel
 Project-URL: Repository, https://github.com/renan-r-santos/pixi-kernel
 Keywords: kernel,jupyter,pixi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Jupyter
@@ -23,32 +24,33 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipykernel<7,>=6
-Requires-Dist: jupyter-client<9,>=8
 Requires-Dist: msgspec<1,>=0.18
 
 # Pixi Kernel
 
 Use per-directory Pixi environments to run Jupyter kernels. The idea behind this project is to
-allow you to capture the exact state of your environment while allowing you to make use of the rich
-PyPI and Conda ecosystems.
+capture the exact state of your environment while allowing you to make use of the rich PyPI and
+Conda ecosystems.
 
 Pixi Kernel supports Python 3.8+ and Pixi 0.18+ using `pyproject.toml` and `pixi.toml`
 configurations.
 
+**Disclaimer**: _This project is not affiliated with Pixi, and not an official Pixi plugin._
+
 ![JupyterLab launcher screen showing Pixi Kernel](assets/image1.png)
 
 ## Quick Start
 
-1. Install this package with `pip install pixi-kernel` in your JupyterLab environment and restart
-   it.
+1. Install this package in your JupyterLab environment and restart it. You can install it using
+   `pip`, `pixi` or any other conda or pip-based package manager.
 2. Create a new directory and notebook and select the **Pixi** kernel for the notebook.
 3. Initialize a Pixi project with `pixi init` and `pixi add ipykernel`.
 4. Restart the kernel and you are good to go.
 
 See the [Pixi docs](https://pixi.sh/latest/) for more information on how to use Pixi.
 
 ## User Experience
@@ -66,7 +68,8 @@
 idea how to support this, please open an issue or check the [contributing guide](CONTRIBUTING.md)
 to open a pull request.
 
 ## Related
 
 - [Pyproject Local Jupyter Kernel](https://github.com/bluss/pyproject-local-kernel)
 - [Poetry-kernel](https://github.com/pathbird/poetry-kernel)
+- [Python Local .venv Kernel](https://github.com/goerz/python-localvenv-kernel)
```

### Comparing `pixi-kernel-0.1.1/assets/logo-64x64.png` & `pixi-kernel-0.1.2/assets/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pixi-kernel-0.1.1/pyproject.toml` & `pixi-kernel-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixi-kernel"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python Jupyter kernel using Pixi for reproducible notebooks"
 license = { text = "MIT" }
 authors = [
     { name = "Renan Rodrigues dos Santos", email = "renan.engmec@gmail.com" },
 ]
 
 readme = "README.md"
@@ -26,46 +26,27 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 
 requires-python = ">=3.8,<4.0"
-dependencies = ["ipykernel>=6,<7", "jupyter-client>=8,<9", "msgspec>=0.18,<1"]
+dependencies = ["ipykernel>=6,<7", "msgspec>=0.18,<1"]
 
 [project.urls]
 Documentation = "https://github.com/renan-r-santos/pixi-kernel"
+Homepage = "https://github.com/renan-r-santos/pixi-kernel"
 Repository = "https://github.com/renan-r-santos/pixi-kernel"
 
 [tool.setuptools.data-files]
 "share/jupyter/kernels/pixi_kernel" = [
     "assets/kernel.json",
     "assets/logo-64x64.png",
 ]
 
-[tool.poetry]
-name = "pixi-kernel"
-version = "0.1.1"
-authors = ["Renan Rodrigues dos Santos <renan.engmec@gmail.com>"]
-description = "Python Jupyter kernel using Pixi for reproducible notebooks"
-packages = [{ include = "pixi_kernel", from = "src" }]
-
-[tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-ipykernel = ">=6,<7"
-jupyter-client = ">=8,<9"
-msgspec = ">=0.18,<1"
-
-[tool.poetry.group.dev.dependencies]
-build = ">=1.2,<2"
-nox_poetry = ">=1.0.3,<2"
-pytest = ">=8.1,<9"
-pytest-cov = "*"
-ruff = ">=0.3.5,<0.4"
-
 [tool.ruff]
 src = ["src"]
 line-length = 99
 
 [tool.ruff.lint]
 extend-select = [
     "I", # isort
@@ -88,16 +69,15 @@
     "ignore:Jupyter is migrating its paths to use standard platformdirs",
 ]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.paths]
-source = [
-    "src/",
-    ".nox/test*/lib/python*/site-packages/",
-    ".nox/test*/Lib/site-packages/",
-]
+source = ["src/", ".pixi/envs/**/lib/python*/site-packages/"]
+
+[tool.coverage.report]
+fail_under = 60
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

### Comparing `pixi-kernel-0.1.1/src/pixi_kernel/__main__.py` & `pixi-kernel-0.1.2/src/pixi_kernel/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,39 +48,44 @@
         )
     logger.info(f"Found pixi {pixi_version}")
 
     # Find project's manifest file
     cwd = Path.cwd().resolve()
     candidate_dirs = [cwd, *cwd.parents]
     for dir in candidate_dirs:
-        result = subprocess.run(["pixi", "info", "--json"], cwd=dir, capture_output=True)
-        if result.returncode != 0:
-            logger.error(f"Failed to get pixi info for directory {dir}: {result.stderr}")
-            continue
-
-        try:
-            pixi_info = msgspec.json.decode(result.stdout, type=PixiInfo)
-        except msgspec.ValidationError as exception:
-            logger.error(f"Failed to parse pixi info {result.stdout}: {exception}")
-            continue
-
-        if len(pixi_info.environments_info) == 0:
-            continue
-
-        for env in pixi_info.environments_info:
-            if env.name == "default" and pixi_info.project_info is not None:
-                if "ipykernel" not in env.dependencies + env.pypi_dependencies:
-                    return PixiKernelError(
-                        message=(
-                            f"The project at {dir} does not have ipykernel as a dependency in the "
-                            "default environment. Please add it by running `pixi add ipykernel` "
-                            "and restart your kernel."
+        for project_filename in ["pixi.toml", "pyproject.toml"]:
+            result = subprocess.run(
+                ["pixi", "info", f"--manifest-path={project_filename}", "--json"],
+                cwd=dir,
+                capture_output=True,
+            )
+            if result.returncode != 0:
+                logger.error(f"Failed to get pixi info for directory {dir}: {result.stderr}")
+                continue
+
+            try:
+                pixi_info = msgspec.json.decode(result.stdout, type=PixiInfo)
+            except msgspec.ValidationError as exception:
+                logger.error(f"Failed to parse pixi info {result.stdout}: {exception}")
+                continue
+
+            if len(pixi_info.environments_info) == 0:
+                continue
+
+            for env in pixi_info.environments_info:
+                if env.name == "default" and pixi_info.project_info is not None:
+                    if "ipykernel" not in env.dependencies + env.pypi_dependencies:
+                        return PixiKernelError(
+                            message=(
+                                f"The project at {dir} does not have ipykernel as a dependency in "
+                                "the default environment. Add it by running `pixi add ipykernel` "
+                                "and restart your kernel."
+                            )
                         )
-                    )
-                return pixi_info.project_info.manifest_path
+                    return str(dir / project_filename)
 
     return PixiKernelError(
         message=("Pixi project not found. Run `pixi init` in the project directory.")
     )
 
 
 def main():
```

### Comparing `pixi-kernel-0.1.1/src/pixi_kernel/kernels.py` & `pixi-kernel-0.1.2/src/pixi_kernel/kernels.py`

 * *Files identical despite different names*

### Comparing `pixi-kernel-0.1.1/src/pixi_kernel.egg-info/PKG-INFO` & `pixi-kernel-0.1.2/src/pixi_kernel.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pixi-kernel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Jupyter kernel using Pixi for reproducible notebooks
 Author-email: Renan Rodrigues dos Santos <renan.engmec@gmail.com>
 License: MIT
 Project-URL: Documentation, https://github.com/renan-r-santos/pixi-kernel
+Project-URL: Homepage, https://github.com/renan-r-santos/pixi-kernel
 Project-URL: Repository, https://github.com/renan-r-santos/pixi-kernel
 Keywords: kernel,jupyter,pixi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Jupyter
@@ -23,32 +24,33 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipykernel<7,>=6
-Requires-Dist: jupyter-client<9,>=8
 Requires-Dist: msgspec<1,>=0.18
 
 # Pixi Kernel
 
 Use per-directory Pixi environments to run Jupyter kernels. The idea behind this project is to
-allow you to capture the exact state of your environment while allowing you to make use of the rich
-PyPI and Conda ecosystems.
+capture the exact state of your environment while allowing you to make use of the rich PyPI and
+Conda ecosystems.
 
 Pixi Kernel supports Python 3.8+ and Pixi 0.18+ using `pyproject.toml` and `pixi.toml`
 configurations.
 
+**Disclaimer**: _This project is not affiliated with Pixi, and not an official Pixi plugin._
+
 ![JupyterLab launcher screen showing Pixi Kernel](assets/image1.png)
 
 ## Quick Start
 
-1. Install this package with `pip install pixi-kernel` in your JupyterLab environment and restart
-   it.
+1. Install this package in your JupyterLab environment and restart it. You can install it using
+   `pip`, `pixi` or any other conda or pip-based package manager.
 2. Create a new directory and notebook and select the **Pixi** kernel for the notebook.
 3. Initialize a Pixi project with `pixi init` and `pixi add ipykernel`.
 4. Restart the kernel and you are good to go.
 
 See the [Pixi docs](https://pixi.sh/latest/) for more information on how to use Pixi.
 
 ## User Experience
@@ -66,7 +68,8 @@
 idea how to support this, please open an issue or check the [contributing guide](CONTRIBUTING.md)
 to open a pull request.
 
 ## Related
 
 - [Pyproject Local Jupyter Kernel](https://github.com/bluss/pyproject-local-kernel)
 - [Poetry-kernel](https://github.com/pathbird/poetry-kernel)
+- [Python Local .venv Kernel](https://github.com/goerz/python-localvenv-kernel)
```

