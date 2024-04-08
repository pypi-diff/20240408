# Comparing `tmp/cff2toml-3.0.0.tar.gz` & `tmp/cff2toml-3.1.0.tar.gz`

## Comparing `cff2toml-3.0.0.tar` & `cff2toml-3.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-3.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-3.0.0/.vscode/settings.json
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/cli/__init__.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/cli/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/__init__.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/basic_model.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/authors/cff_entity_author.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/authors/cff_person_author.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/authors/pyproject_toml_author.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/authors/synchronizers/cff_and_pyproject_toml_author_synchronizer.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/organizations/cff_entity.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/people/cff_person.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/agents/people/human_name.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/__init__.py
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/cff_file.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/metadata_file.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/pyproject_toml_file.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/toml_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/synchronizers/__init__.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/models/files/synchronizers/cff_and_pyproject_toml_file_synchronizer.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/conftest.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/temp_copied_file.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/authors/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/authors/synchronizers/__init__.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/authors/synchronizers/test_cff_and_pyproject_toml_author_synchronizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/organizations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/people/__init__.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/agents/people/test_human_name_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/__init__.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/test_cff_file.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/test_metadata_file.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/test_pyproject_toml_file.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/test_toml_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/synchronizers/__init__.py
--rw-r--r--   0        0        0    12218 2020-02-02 00:00:00.000000 cff2toml-3.0.0/tests/models/files/synchronizers/test_cff_and_pyproject_toml_synchronizer.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 cff2toml-3.0.0/src/cff2toml/CITATION.cff
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-3.0.0/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-3.0.0/LICENSE
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 cff2toml-3.0.0/README.md
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 cff2toml-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cff2toml-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-3.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-3.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/cli/__init__.py
+-rw-r--r--   0        0        0    12537 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/cli/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/__init__.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/basic_model.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/agents/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/agents/authors/cff_entity_author.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/agents/authors/cff_person_author.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/agents/authors/pyproject_toml_author.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/agents/authors/synchronizers/cff_and_pyproject_toml_author_synchronizer.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/agents/organizations/cff_entity.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/agents/people/cff_person.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/agents/people/human_name.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/files/__init__.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/files/cff_file.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/files/metadata_file.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/files/pyproject_toml_file.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/files/toml_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/files/synchronizers/__init__.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/models/files/synchronizers/cff_and_pyproject_toml_file_synchronizer.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/temp_copied_file.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/agents/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/agents/authors/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/agents/authors/synchronizers/__init__.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/agents/authors/synchronizers/test_cff_and_pyproject_toml_author_synchronizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/agents/organizations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/agents/people/__init__.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/agents/people/test_human_name_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/files/__init__.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/files/test_cff_file.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/files/test_metadata_file.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/files/test_pyproject_toml_file.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/files/test_toml_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/files/synchronizers/__init__.py
+-rw-r--r--   0        0        0    12218 2020-02-02 00:00:00.000000 cff2toml-3.1.0/tests/models/files/synchronizers/test_cff_and_pyproject_toml_synchronizer.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 cff2toml-3.1.0/src/cff2toml/CITATION.cff
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-3.1.0/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-3.1.0/LICENSE
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 cff2toml-3.1.0/README.md
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 cff2toml-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cff2toml-3.1.0/PKG-INFO
```

### Comparing `cff2toml-3.0.0/.github/workflows/python-publish.yml` & `cff2toml-3.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/models/basic_model.py` & `cff2toml-3.1.0/src/cff2toml/models/basic_model.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/models/metadata.py` & `cff2toml-3.1.0/src/cff2toml/models/metadata.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/models/agents/authors/synchronizers/cff_and_pyproject_toml_author_synchronizer.py` & `cff2toml-3.1.0/src/cff2toml/models/agents/authors/synchronizers/cff_and_pyproject_toml_author_synchronizer.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/models/agents/organizations/cff_entity.py` & `cff2toml-3.1.0/src/cff2toml/models/agents/organizations/cff_entity.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/models/agents/people/cff_person.py` & `cff2toml-3.1.0/src/cff2toml/models/agents/people/cff_person.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/models/agents/people/human_name.py` & `cff2toml-3.1.0/src/cff2toml/models/agents/people/human_name.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/models/files/cff_file.py` & `cff2toml-3.1.0/src/cff2toml/models/files/cff_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/models/files/metadata_file.py` & `cff2toml-3.1.0/src/cff2toml/models/files/metadata_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/models/files/pyproject_toml_file.py` & `cff2toml-3.1.0/src/cff2toml/models/files/pyproject_toml_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/models/files/toml_file.py` & `cff2toml-3.1.0/src/cff2toml/models/files/toml_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/models/files/synchronizers/cff_and_pyproject_toml_file_synchronizer.py` & `cff2toml-3.1.0/src/cff2toml/models/files/synchronizers/cff_and_pyproject_toml_file_synchronizer.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/tests/conftest.py` & `cff2toml-3.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/tests/temp_copied_file.py` & `cff2toml-3.1.0/tests/temp_copied_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/tests/dummy_files/dummy_CITATION.cff` & `cff2toml-3.1.0/tests/dummy_files/dummy_CITATION.cff`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-3.1.0/tests/dummy_files/dummy_pyproject.toml`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/tests/models/agents/authors/synchronizers/test_cff_and_pyproject_toml_author_synchronizer.py` & `cff2toml-3.1.0/tests/models/agents/authors/synchronizers/test_cff_and_pyproject_toml_author_synchronizer.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/tests/models/agents/people/test_human_name_parser.py` & `cff2toml-3.1.0/tests/models/agents/people/test_human_name_parser.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/tests/models/files/test_cff_file.py` & `cff2toml-3.1.0/tests/models/files/test_cff_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/tests/models/files/test_metadata_file.py` & `cff2toml-3.1.0/tests/models/files/test_metadata_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/tests/models/files/test_pyproject_toml_file.py` & `cff2toml-3.1.0/tests/models/files/test_pyproject_toml_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/tests/models/files/test_toml_file.py` & `cff2toml-3.1.0/tests/models/files/test_toml_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/tests/models/files/synchronizers/test_cff_and_pyproject_toml_synchronizer.py` & `cff2toml-3.1.0/tests/models/files/synchronizers/test_cff_and_pyproject_toml_synchronizer.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/src/cff2toml/CITATION.cff` & `cff2toml-3.1.0/src/cff2toml/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
   A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 keywords:
   - Citation File Format
   - TOML
   - pyproject.toml
   - CITATION.cff
 license: Apache-2.0
-version: "3.0.0"
+version: "3.1.0"
```

### Comparing `cff2toml-3.0.0/LICENSE` & `cff2toml-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/README.md` & `cff2toml-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cff2toml-3.0.0/pyproject.toml` & `cff2toml-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "3.0.0"
+version = "3.1.0"
 description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
```

### Comparing `cff2toml-3.0.0/PKG-INFO` & `cff2toml-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cff2toml
-Version: 3.0.0
+Version: 3.1.0
 Summary: A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 Project-URL: Documentation, https://github.com/willynilly/cff2toml#readme
 Project-URL: Issues, https://github.com/willynilly/cff2toml/issues
 Project-URL: Source, https://github.com/willynilly/cff2toml
 Author-email: Will Riley <wanderingwill@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

