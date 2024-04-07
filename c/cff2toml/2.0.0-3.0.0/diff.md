# Comparing `tmp/cff2toml-2.0.0.tar.gz` & `tmp/cff2toml-3.0.0.tar.gz`

## Comparing `cff2toml-2.0.0.tar` & `cff2toml-3.0.0.tar`

### file list

```diff
@@ -1,23 +1,50 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-2.0.0/CITATION.cff
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-2.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-2.0.0/.vscode/settings.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/__init__.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/cff2toml.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/getters.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/loaders.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/savers.py
--rw-r--r--   0        0        0     8674 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/setters.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/common_fixtures.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/temp_copied_file.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/test_getters.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/test_loaders.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/test_savers.py
--rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/test_setters.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-2.0.0/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-2.0.0/LICENSE
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 cff2toml-2.0.0/README.md
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 cff2toml-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    10021 2020-02-02 00:00:00.000000 cff2toml-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-3.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-3.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/cli/__init__.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/cli/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/__init__.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/basic_model.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/authors/cff_entity_author.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/authors/cff_person_author.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/authors/pyproject_toml_author.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/authors/synchronizers/cff_and_pyproject_toml_author_synchronizer.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/organizations/cff_entity.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/people/cff_person.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/people/human_name.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/__init__.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/cff_file.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/metadata_file.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/pyproject_toml_file.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/toml_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/synchronizers/__init__.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/synchronizers/cff_and_pyproject_toml_file_synchronizer.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/temp_copied_file.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/authors/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/authors/synchronizers/__init__.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/authors/synchronizers/test_cff_and_pyproject_toml_author_synchronizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/organizations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/people/__init__.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/people/test_human_name_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/__init__.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/test_cff_file.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/test_metadata_file.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/test_pyproject_toml_file.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/test_toml_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/synchronizers/__init__.py
+-rw-r--r--   0        0        0    12218 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/synchronizers/test_cff_and_pyproject_toml_synchronizer.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/CITATION.cff
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-3.0.0/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 cff2toml-3.0.0/README.md
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 cff2toml-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cff2toml-3.0.0/PKG-INFO
```

### Comparing `cff2toml-2.0.0/CITATION.cff` & `cff2toml-3.0.0/src/cff2toml/CITATION.cff`

 * *Files 19% similar despite different names*

```diff
@@ -8,17 +8,15 @@
   - given-names: Will
     family-names: Riley
     email: wanderingwill@gmail.com
     orcid: "https://orcid.org/0000-0003-1822-6756"
 repository-code: >-
   https://github.com/willynilly/cff2toml
 abstract: >-
-  A module to synchronize metadata between TOML 
-  and CFF files, including between pyproject.toml 
-  and CITATION.cff files.
+  A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 keywords:
   - Citation File Format
   - TOML
   - pyproject.toml
   - CITATION.cff
 license: Apache-2.0
-version: "2.0.0"
+version: "3.0.0"
```

### Comparing `cff2toml-2.0.0/.github/workflows/python-publish.yml` & `cff2toml-3.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-2.0.0/tests/temp_copied_file.py` & `cff2toml-3.0.0/tests/temp_copied_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-2.0.0/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-3.0.0/tests/dummy_files/dummy_pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 version = "0.0.1"
 description = "A module that does something uncool."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-1.0"
 keywords = []
 authors = [
-  { name = "Will Riley", email = "wanderingwill@gmail.com" },
+  { name = "Will Riley", email = "test1@willriley.net" },
+  { name = "Willy Riley", email = "test2@willriley.net" }
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
@@ -24,13 +25,13 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["toml==0.10.2", "PyYAML==6.0.1"]
 
 [project.urls]
 Documentation = "https://github.com/willynilly/somewhereuncool#readme"
 Issues = "https://github.com/willynilly/somewhereuncool/issues"
-Source = "https://github.com/willnilly/somewhereuncool"
+Source = "https://github.com/willynilly/somewhereuncool"
 
 [project.optional-dependencies]
 testing = [
     "pytest==8.1.1",
 ]
```

### Comparing `cff2toml-2.0.0/LICENSE` & `cff2toml-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-2.0.0/pyproject.toml` & `cff2toml-3.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "2.0.0"
+version = "3.0.0"
 description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
@@ -29,23 +29,30 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development",
     "Topic :: Utilities"
 ]
-dependencies = ["toml==0.10.2", "PyYAML==6.0.1", "pydash==8.0.0"]
+dependencies = ["toml>=0.10.2", "PyYAML>=6.0.1", "pydash>=8.0.0", "pydantic>=2.6.4", "typer>=0.12.1"]
+
+[project.scripts]
+cff2toml = "cff2toml.main:start"
 
 [project.urls]
 Documentation = "https://github.com/willynilly/cff2toml#readme"
 Issues = "https://github.com/willynilly/cff2toml/issues"
 Source = "https://github.com/willynilly/cff2toml"
 
 [project.optional-dependencies]
 testing = [
-    "pytest==8.1.1",
+    "pytest>=8.1.1",
 ]
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
-]
+]
+
+[tool.hatch.build.targets.sdist.force-include]
+"CITATION.cff" = "src/cff2toml/CITATION.cff"
+
```

