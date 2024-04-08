# Comparing `tmp/nens-meta-0.4.tar.gz` & `tmp/nens-meta-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nens-meta-0.4.tar", last modified: Tue Feb 20 20:06:06 2024, max compression
+gzip compressed data, was "nens-meta-0.5.tar", last modified: Mon Apr  8 09:53:03 2024, max compression
```

## Comparing `nens-meta-0.4.tar` & `nens-meta-0.5.tar`

### file list

```diff
@@ -1,24 +1,38 @@
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-02-20 20:06:06.604215 nens-meta-0.4/
--rw-r--r--   0 reinout    (501) staff       (20)     2292 2024-02-20 20:06:06.000000 nens-meta-0.4/CHANGES.md
--rw-r--r--   0 reinout    (501) staff       (20)     1766 2024-02-20 20:06:06.000000 nens-meta-0.4/DEVELOPMENT.md
--rw-r--r--   0 reinout    (501) staff       (20)     1075 2024-02-20 20:06:06.000000 nens-meta-0.4/LICENSE
--rw-r--r--   0 reinout    (501) staff       (20)      137 2024-02-20 20:06:06.000000 nens-meta-0.4/MANIFEST.in
--rw-r--r--   0 reinout    (501) staff       (20)     2258 2024-02-20 20:06:06.603997 nens-meta-0.4/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)     1568 2024-02-20 20:06:06.000000 nens-meta-0.4/README.md
--rw-r--r--   0 reinout    (501) staff       (20)     1002 2024-02-20 20:06:06.000000 nens-meta-0.4/USAGE.md
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-02-20 20:06:06.601897 nens-meta-0.4/nens_meta/
--rw-r--r--   0 reinout    (501) staff       (20)       20 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)     7318 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta/nens_toml.py
--rw-r--r--   0 reinout    (501) staff       (20)     8257 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta/pyproject_toml.py
--rw-r--r--   0 reinout    (501) staff       (20)     8968 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta/update_project.py
--rw-r--r--   0 reinout    (501) staff       (20)     2709 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta/utils.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-02-20 20:06:06.603500 nens-meta-0.4/nens_meta.egg-info/
--rw-r--r--   0 reinout    (501) staff       (20)     2258 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta.egg-info/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)      431 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta.egg-info/SOURCES.txt
--rw-r--r--   0 reinout    (501) staff       (20)        1 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta.egg-info/dependency_links.txt
--rw-r--r--   0 reinout    (501) staff       (20)       70 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta.egg-info/entry_points.txt
--rw-r--r--   0 reinout    (501) staff       (20)        1 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta.egg-info/not-zip-safe
--rw-r--r--   0 reinout    (501) staff       (20)       66 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta.egg-info/requires.txt
--rw-r--r--   0 reinout    (501) staff       (20)       10 2024-02-20 20:06:06.000000 nens-meta-0.4/nens_meta.egg-info/top_level.txt
--rw-r--r--   0 reinout    (501) staff       (20)     1609 2024-02-20 20:06:06.000000 nens-meta-0.4/pyproject.toml
--rw-r--r--   0 reinout    (501) staff       (20)       38 2024-02-20 20:06:06.604257 nens-meta-0.4/setup.cfg
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.860541 nens-meta-0.5/
+-rw-r--r--   0 reinout    (501) staff       (20)     2680 2024-04-08 09:53:03.000000 nens-meta-0.5/CHANGES.md
+-rw-r--r--   0 reinout    (501) staff       (20)     1766 2024-04-08 09:53:03.000000 nens-meta-0.5/DEVELOPMENT.md
+-rw-r--r--   0 reinout    (501) staff       (20)     1075 2024-04-08 09:53:03.000000 nens-meta-0.5/LICENSE
+-rw-r--r--   0 reinout    (501) staff       (20)      153 2024-04-08 09:53:03.000000 nens-meta-0.5/MANIFEST.in
+-rw-r--r--   0 reinout    (501) staff       (20)     2356 2024-04-08 09:53:03.860343 nens-meta-0.5/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)     1666 2024-04-08 09:53:03.000000 nens-meta-0.5/README.md
+-rw-r--r--   0 reinout    (501) staff       (20)     1002 2024-04-08 09:53:03.000000 nens-meta-0.5/USAGE.md
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.857248 nens-meta-0.5/nens_meta/
+-rw-r--r--   0 reinout    (501) staff       (20)       20 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)     6386 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/nens_toml.py
+-rw-r--r--   0 reinout    (501) staff       (20)     8601 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/pyproject_toml.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.858274 nens-meta-0.5/nens_meta/templates/
+-rw-r--r--   0 reinout    (501) staff       (20)       75 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/README.md
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.859071 nens-meta-0.5/nens_meta/templates/default/
+-rw-r--r--   0 reinout    (501) staff       (20)      120 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/dependabot.yml.j2
+-rw-r--r--   0 reinout    (501) staff       (20)      345 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/editorconfig.j2
+-rw-r--r--   0 reinout    (501) staff       (20)      452 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/gitignore.j2
+-rw-r--r--   0 reinout    (501) staff       (20)     1013 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/meta_workflow.yml.j2
+-rw-r--r--   0 reinout    (501) staff       (20)      732 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/pre-commit-config.yaml.j2
+-rw-r--r--   0 reinout    (501) staff       (20)      278 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/requirements.yml.j2
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.859738 nens-meta-0.5/nens_meta/tests/
+-rw-r--r--   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/tests/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)     4522 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/tests/test_nens_toml.py
+-rw-r--r--   0 reinout    (501) staff       (20)     6072 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/tests/test_pyproject_toml.py
+-rw-r--r--   0 reinout    (501) staff       (20)     3197 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/tests/test_update_project.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2429 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/tests/test_utils.py
+-rw-r--r--   0 reinout    (501) staff       (20)     8375 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/update_project.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2709 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/utils.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.859927 nens-meta-0.5/nens_meta.egg-info/
+-rw-r--r--   0 reinout    (501) staff       (20)     2356 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)      881 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/SOURCES.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/dependency_links.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       70 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/entry_points.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       66 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/requires.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       10 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/top_level.txt
+-rw-r--r--   0 reinout    (501) staff       (20)     1583 2024-04-08 09:53:03.000000 nens-meta-0.5/pyproject.toml
+-rw-r--r--   0 reinout    (501) staff       (20)       38 2024-04-08 09:53:03.860578 nens-meta-0.5/setup.cfg
```

### Comparing `nens-meta-0.4/CHANGES.md` & `nens-meta-0.5/CHANGES.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Changelog of nens-meta
 
 
+## 0.5 (2024-04-08)
+
+- Simplified everything by removing tox for now.
+- Suggesting initial `requirements.yml` for ansible projects as ansible-lint almost always needs it.
+- Allow additional directories (`extra_package_names`) with python code next to the "main" one (`package_name`). Some projects use more than one directory. This has effect on the test runner, coverage reports, etc.
+
+
 ## 0.4 (2024-02-20)
 
 
 - Removed "tox -e format", we only use "tox -e lint" in practice.
 - Detecting `ansible/` directory and adding ansible-lint to the pre-commit config if found.
 
 ## 0.3 (2024-02-20)
```

### Comparing `nens-meta-0.4/DEVELOPMENT.md` & `nens-meta-0.5/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `nens-meta-0.4/LICENSE` & `nens-meta-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nens-meta-0.4/PKG-INFO` & `nens-meta-0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nens-meta
-Version: 0.4
+Version: 0.5
 Summary: Basic project automation and update tool
 Author-email: Reinout van Rees <reinout.vanrees@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Documentation, https://nens-meta.readthedocs.io/
 Project-URL: Repository, https://github.com/nens/nens-meta
 Project-URL: Changelog, https://github.com/nens/nens-meta/blob/main/CHANGES.md
 Requires-Python: >=3.11
@@ -31,21 +31,24 @@
 Note that [our cookiecutter template](https://github.com/nens/cookiecutter-python-template) normally should have been the basis from which you started your project. But it might have been created by hand. Or it might have been a long time ago. "Meta" tries to fix up your project a bit.
 
 
 ## Installing/developing this project
 
 For the basic instructions, see [our own documentation](https://nens-meta.readthedocs.io/en/latest/usage.html). So:
 
-    $ pip install tox
-    $ tox -q
+    $ python3 -m venv .venv
+    $ source .venv/bin/activate
+    $ pip install -r requirements
+    $ pytest
+    $ pre-commit run --all
 
 
 ## TODO
 
-- manifest.ini
+- manifest.in
 
 - docker-compose
 
 - Projectnummer
 
 - testen met vscode
```

### Comparing `nens-meta-0.4/README.md` & `nens-meta-0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 Note that [our cookiecutter template](https://github.com/nens/cookiecutter-python-template) normally should have been the basis from which you started your project. But it might have been created by hand. Or it might have been a long time ago. "Meta" tries to fix up your project a bit.
 
 
 ## Installing/developing this project
 
 For the basic instructions, see [our own documentation](https://nens-meta.readthedocs.io/en/latest/usage.html). So:
 
-    $ pip install tox
-    $ tox -q
+    $ python3 -m venv .venv
+    $ source .venv/bin/activate
+    $ pip install -r requirements
+    $ pytest
+    $ pre-commit run --all
 
 
 ## TODO
 
-- manifest.ini
+- manifest.in
 
 - docker-compose
 
 - Projectnummer
 
 - testen met vscode
```

### Comparing `nens-meta-0.4/USAGE.md` & `nens-meta-0.5/USAGE.md`

 * *Files identical despite different names*

### Comparing `nens-meta-0.4/nens_meta/nens_toml.py` & `nens-meta-0.5/nens_meta/nens_toml.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,56 +41,29 @@
     Option(
         key="uses_ansible",
         description="Whether we have an ansible dir",
         default=False,
         value_type=bool,
     ),
     Option(key="package_name", description="Name of the main python package"),
-]
-KNOWN_SECTIONS["pyprojecttoml"] = []
-KNOWN_SECTIONS["tox"] = [
-    Option(key="minimum_coverage", description="Minimum code coverage percentage"),
     Option(
-        key="default_environments",
-        description="List of envs to run when you call 'tox'",
+        key="extra_package_names",
+        description="Extra dirs with packages, in addition to package_name",
+        default=[],
         value_type=list,
-        default=["lint"],
-        default_if_python=[
-            "lint",
-            "py310",
-            "py311",
-            "py312",
-            "coverage",
-        ],
     ),
+    Option(key="minimum_coverage", description="Minimum code coverage percentage"),
 ]
+KNOWN_SECTIONS["pyprojecttoml"] = []
 KNOWN_SECTIONS["meta_workflow"] = [
     Option(
-        key="environments",
-        description="Tox environments that should be called, 'TEST' means 'py*'",
-        value_type=list,
-        default=["lint"],
-        default_if_python=[
-            "lint",
-            "coverage",
-            "TEST",
-        ],
-    ),
-    Option(
         key="main_python_version",
         description="Python version to use for linting and so",
         default="3.11",
     ),
-    Option(
-        key="python_versions",
-        description="Python version(s) to run tests as",
-        value_type=list,
-        default=["3.11"],
-        default_if_python=["3.10", "3.11", "3.12"],
-    ),
 ]
 
 logger = logging.getLogger(__name__)
 
 
 def write_documentation():
     target = Path(__file__).parent.parent / "doc" / "nens_toml_example.toml"
@@ -119,25 +92,14 @@
         nens_toml_file(project).write_text("")
     our_config = OurConfig(project)
     our_config.read()
     our_config.update_meta_options()
     our_config.write()
 
 
-def _default_for_key(key: str) -> str | bool | list:
-    """Return default (''), but handle the _TRUE/_FALSE postfix tricks"""
-    if "_TRUE" in key:
-        return True
-    if "_FALSE" in key:
-        return False
-    if "_LIST" in key:
-        return []
-    return ""
-
-
 def detected_meta_values(project: Path) -> dict[str, str | bool | list]:
     """Return values we can detect about the project, normally set in [meta]"""
     detected: dict[str, str | bool | list] = {}
     detected["is_python_project"] = utils.is_python_project(project)
     detected["uses_ansible"] = utils.uses_ansible(project)
     detected["meta_version"] = __version__
     name = project.resolve().name
```

### Comparing `nens-meta-0.4/nens_meta/pyproject_toml.py` & `nens-meta-0.5/nens_meta/pyproject_toml.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,17 @@
     def _suggest(self, section_name: str, key: str, value: Any, strongly=False):
         section = self.get_or_create_section(section_name)
         if key not in section:
             section[key] = value
             logger.info(f"pyproject.toml: suggesting [{section_name}]->{key}")
         if strongly:
             if section[key] != value:
-                logger.info(f"    Note: our suggested value: {value}")
+                logger.info(
+                    f"    Note: our suggested pyproject.toml value for [{section_name}]->{key}: {value}"
+                )
 
     def _force(self, section_name: str, key: str, value: Any):
         section = self.get_or_create_section(section_name)
         if section.get(key) != value:
             section[key] = value
             logger.info(f"pyproject.toml: setting [{section_name}]->{key}")
 
@@ -140,31 +142,41 @@
         if not name:
             logger.error("package_name not set in `.nens.toml` [meta]")
             name = "not_set"
         if not (self._project / name).exists():
             logger.error(f"Python package {name} doesn't exist in the current project")
         return name
 
+    @property
+    def extra_package_names(self) -> list[str]:
+        extra_names = self._options.get("extra_package_names")
+        if not extra_names:
+            return []
+        return extra_names
+
+    @property
+    def package_names(self) -> list[str]:
+        return [self.package_name] + self.extra_package_names
+
     def adjust_setuptools(self):
         section_name = "tool.setuptools"
         # TODO: optional extra packages
-        self._suggest(section_name, "packages", [self.package_name], strongly=True)
-        self._suggest(section_name, "zip-safe", False)
+        self._suggest(section_name, "packages", self.package_names, strongly=True)
 
     def adjust_pytest(self):
         section_name = "tool.pytest.ini_options"
         self._force(
-            section_name, "testpaths", [self.package_name]
+            section_name, "testpaths", self.package_names
         )  # TODO: optional extra packages
         self._suggest(section_name, "log_level", "DEBUG")
 
     def adjust_coverage(self):
         section_name = "tool.coverage.run"
         self._force(
-            section_name, "source", [self.package_name]
+            section_name, "source", self.package_names
         )  # TODO: optional extra packages
 
         section_name = "tool.coverage.report"
         self._force(section_name, "show_missing", True)
         self._force(section_name, "skip_empty", True)
 
     def adjust_ruff(self):
@@ -173,15 +185,15 @@
 
         section_name = "tool.ruff.lint"
         self._suggest(section_name, "select", ["E4", "E7", "E9", "F", "I", "UP"])
 
     def adjust_pyright(self):
         section_name = "tool.pyright"
         self._force(
-            section_name, "include", [self.package_name]
+            section_name, "include", self.package_names
         )  # TODO: optional extra packages
         self._suggest(section_name, "venvPath", ".", strongly=True)
         self._suggest(section_name, "venv", ".venv", strongly=True)
 
     def adjust_zestreleaser(self):
         section_name = "tool.zest-releaser"
         self._suggest(section_name, "release", False)
```

### Comparing `nens-meta-0.4/nens_meta/update_project.py` & `nens-meta-0.5/nens_meta/update_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 class TemplatedFile:
     project_dir: Path
     our_config: nens_toml.OurConfig
     template_name: str
     target_name: str  # Note: can be "subdir/some-file.txt"
     section_name: str
+    only_create_dont_change: bool = False
 
     def __init__(self, project_dir: Path, our_config: nens_toml.OurConfig) -> None:
         self.project_dir = project_dir
         self.our_config = our_config
 
     @property
     def target(self) -> Path:
@@ -98,15 +99,25 @@
                 return
             target_dir.mkdir(parents=True)
             logger.info(f"Created directory {target_dir}")
 
     def write(self):
         """Copy the source template to the target, doing the jinja2 stuff"""
         self.create_dirs_if_needed()
-        utils.write_if_changed(self.target, self.content)
+        handle_extra_lines = True  # default
+        if self.only_create_dont_change:
+            handle_extra_lines = (
+                False  # No need for this if we're not updating the file.
+            )
+            if self.target.exists():
+                logger.debug(f"{self.target} already exists, skipping")
+                return
+        utils.write_if_changed(
+            self.target, self.content, handle_extra_lines=handle_extra_lines
+        )
 
 
 class Editorconfig(TemplatedFile):
     """Wrapper around a project's editorconfig"""
 
     template_name = "editorconfig.j2"
     target_name = ".editorconfig"
@@ -125,31 +136,14 @@
     """Wrapper around a project's .pre-commit-config.yaml"""
 
     template_name = "pre-commit-config.yaml.j2"
     target_name = ".pre-commit-config.yaml"
     section_name = "pre-commit-config"
 
 
-class ToxIni(TemplatedFile):
-    """Wrapper around a project's tox.ini"""
-
-    template_name = "tox.ini.j2"
-    target_name = "tox.ini"
-    section_name = "tox"
-
-    def envlist(self) -> str:
-        """Return formatted indented envlist, possibly with default content"""
-        environments = self.our_options["default_environments"]
-        lines = [f"    {environment}" for environment in environments]
-        return "\n".join(lines)
-
-    def extra_options(self) -> dict:
-        return {"envlist": self.envlist()}
-
-
 class DependabotYml(TemplatedFile):
     """Wrapper around a dependabot.yml file"""
 
     template_name = "dependabot.yml.j2"
     target_name = ".github/dependabot.yml"
     section_name = "dependabot"
 
@@ -157,41 +151,22 @@
 class MetaWorkflowYml(TemplatedFile):
     """Wrapper around a nens-meta.yml file"""
 
     template_name = "meta_workflow.yml.j2"
     target_name = ".github/workflows/nens-meta.yml"
     section_name = "meta_workflow"
 
-    def python_tox_pairs(self) -> list[dict]:
-        environments = self.our_options["environments"]
-        result = []
-
-        main_python_version = self.our_options["main_python_version"]
-        python_versions = self.our_options["python_versions"]
-
-        for environment in environments:
-            if environment == "TEST":
-                pairs = [
-                    {
-                        "python": python_version,
-                        "tox": f"py{python_version.replace('.', '')}",
-                    }
-                    for python_version in python_versions
-                ]
-            else:
-                pairs = [{"python": main_python_version, "tox": environment}]
-            result += pairs
-        logger.debug(f"Adding the following pairs to the test matrix: {result}")
-        return result
 
-    def extra_options(self) -> dict:
-        return {
-            "python_tox_pairs": self.python_tox_pairs(),
-            "workflow_name": "nens-meta",
-        }
+class RequirementsYml(TemplatedFile):
+    """Wrapper around an ansible requirements.yml file"""
+
+    template_name = "requirements.yml.j2"
+    target_name = "requirements.yml"
+    section_name = "ansible"
+    only_create_dont_change = True
 
 
 def check_prerequisites(project_dir: Path):
     """Check prerequisites, exit if not met"""
     if not (project_dir / ".git").exists():
         logger.error("Project has no .git dir")
         sys.exit(1)
@@ -213,14 +188,16 @@
             dev_indicator1 in requirementstxt.read_text()
             and dev_indicator2 in requirementstxt.read_text()
         ):
             logger.warning(
                 f"The text '{dev_indicator1}' and '{dev_indicator2}' are "
                 f"not both found in {requirementstxt}"
             )
+        if "coverage" not in requirementstxt.read_text():
+            logger.warning("You might want to add 'coverage' to requirements.txt")
     for file_to_check in project_dir.glob("*.outdated"):
         logger.warning(
             f"Check the old {file_to_check}: move settings to pyproject.toml, perhaps?"
         )
     website = "https://nens-meta.readthedocs.io"
     readme = Path("README.md")
     if readme.exists():
@@ -256,20 +233,22 @@
     # Grab editorconfig table and pass it along. Or rather the whole thing?
     editorconfig = Editorconfig(project_dir, our_config)
     editorconfig.write()
     gitignore = Gitignore(project_dir, our_config)
     gitignore.write()
     precommitconfig = Precommitconfig(project_dir, our_config)
     precommitconfig.write()
-    tox_ini = ToxIni(project_dir, our_config)
-    tox_ini.write()
     dependabot_yml = DependabotYml(project_dir, our_config)
     dependabot_yml.write()
     meta_workflow_yml = MetaWorkflowYml(project_dir, our_config)
     meta_workflow_yml.write()
 
+    if our_config.section_options("meta")["uses_ansible"]:
+        requirements_yml = RequirementsYml(project_dir, our_config)
+        requirements_yml.write()
+
     if our_config.section_options("meta")["is_python_project"]:
         do_some_python_checks(project_dir)
 
 
 def main():  # pragma: no cover
     typer.run(update_project)
```

### Comparing `nens-meta-0.4/nens_meta/utils.py` & `nens-meta-0.5/nens_meta/utils.py`

 * *Files identical despite different names*

### Comparing `nens-meta-0.4/nens_meta.egg-info/PKG-INFO` & `nens-meta-0.5/nens_meta.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nens-meta
-Version: 0.4
+Version: 0.5
 Summary: Basic project automation and update tool
 Author-email: Reinout van Rees <reinout.vanrees@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Documentation, https://nens-meta.readthedocs.io/
 Project-URL: Repository, https://github.com/nens/nens-meta
 Project-URL: Changelog, https://github.com/nens/nens-meta/blob/main/CHANGES.md
 Requires-Python: >=3.11
@@ -31,21 +31,24 @@
 Note that [our cookiecutter template](https://github.com/nens/cookiecutter-python-template) normally should have been the basis from which you started your project. But it might have been created by hand. Or it might have been a long time ago. "Meta" tries to fix up your project a bit.
 
 
 ## Installing/developing this project
 
 For the basic instructions, see [our own documentation](https://nens-meta.readthedocs.io/en/latest/usage.html). So:
 
-    $ pip install tox
-    $ tox -q
+    $ python3 -m venv .venv
+    $ source .venv/bin/activate
+    $ pip install -r requirements
+    $ pytest
+    $ pre-commit run --all
 
 
 ## TODO
 
-- manifest.ini
+- manifest.in
 
 - docker-compose
 
 - Projectnummer
 
 - testen met vscode
```

### Comparing `nens-meta-0.4/pyproject.toml` & `nens-meta-0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=69", "wheel"]
+requires = ["setuptools>=69"]
 
 [project]
 name = "nens-meta"
 description = "Basic project automation and update tool"
 authors = [
     {name = "Reinout van Rees", email = "reinout.vanrees@nelen-schuurmans.nl"},
 ]
@@ -27,15 +27,14 @@
 [project.urls]
 Documentation = "https://nens-meta.readthedocs.io/"
 Repository = "https://github.com/nens/nens-meta"
 Changelog = "https://github.com/nens/nens-meta/blob/main/CHANGES.md"
 
 [tool.setuptools]
 packages = ["nens_meta"]
-zip-safe = false
 
 [tool.setuptools.dynamic]
 version = {attr = "nens_meta.__version__"}
 
 [project.scripts]
 nens-update-project = "nens_meta.update_project:main"
```

