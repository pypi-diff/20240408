# Comparing `tmp/pyconverters_whisperx-0.5.6.tar.gz` & `tmp/pyconverters_whisperx-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconverters_whisperx-0.5.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyconverters_whisperx-0.5.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyconverters_whisperx-0.5.6.tar` & `pyconverters_whisperx-0.5.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      497 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/.bumpversion.cfg
--rw-r--r--   0        0        0     1767 2024-04-08 08:52:46.009994 pyconverters_whisperx-0.5.6/.gitignore
--rw-r--r--   0        0        0      176 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/.idea/.gitignore
--rw-r--r--   0        0        0      901 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      203 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/.idea/misc.xml
--rw-r--r--   0        0        0      294 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/.idea/modules.xml
--rw-r--r--   0        0        0      446 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/.idea/pyconverters_whisperx.iml
--rw-r--r--   0        0        0      419 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      202 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.6/.readthedocs.yml
--rw-r--r--   0        0        0      117 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/AUTHORS.md
--rw-r--r--   0        0        0      268 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.6/CHANGELOG.md
--rw-r--r--   0        0        0      461 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.6/Dockerfile
--rw-r--r--   0        0        0    13953 2024-04-08 08:52:46.009994 pyconverters_whisperx-0.5.6/Jenkinsfile
--rw-r--r--   0        0        0     1082 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/LICENSE
--rw-r--r--   0        0        0     1527 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/README.md
--rw-r--r--   0        0        0      941 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/RELEASE.md
--rw-r--r--   0        0        0     1559 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.6/bumpversion.py
--rw-r--r--   0        0        0       62 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.6/docs/.gitignore
--rw-r--r--   0        0        0      268 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.6/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/docs/LICENSE
--rw-r--r--   0        0        0        0 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.6/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.6/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     2879 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/docs/conf.py
--rw-r--r--   0        0        0      142 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/docs/index.rst
--rw-r--r--   0        0        0       98 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.6/mypy.ini
--rw-r--r--   0        0        0     2227 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      969 2024-04-08 08:54:36.109402 pyconverters_whisperx-0.5.6/results.xml
--rw-r--r--   0        0        0       48 2024-04-08 08:56:06.760210 pyconverters_whisperx-0.5.6/src/pyconverters_whisperx/__init__.py
--rw-r--r--   0        0        0     6312 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/src/pyconverters_whisperx/whisperx.py
--rw-r--r--   0        0        0      422 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/tests/data/test.yaml
--rw-r--r--   0        0        0     1011 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.6/tests/test_whisperx.py
--rw-r--r--   0        0        0     1041 2024-04-08 08:35:38.574570 pyconverters_whisperx-0.5.6/tox.ini
--rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 pyconverters_whisperx-0.5.6/setup.py
--rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 pyconverters_whisperx-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      497 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/.bumpversion.cfg
+-rw-r--r--   0        0        0     1767 2024-04-08 08:52:46.009994 pyconverters_whisperx-0.5.8/.gitignore
+-rw-r--r--   0        0        0      176 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/.idea/.gitignore
+-rw-r--r--   0        0        0      901 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      203 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/.idea/modules.xml
+-rw-r--r--   0        0        0      446 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/.idea/pyconverters_whisperx.iml
+-rw-r--r--   0        0        0      419 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      202 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.8/.readthedocs.yml
+-rw-r--r--   0        0        0      117 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/AUTHORS.md
+-rw-r--r--   0        0        0      268 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.8/CHANGELOG.md
+-rw-r--r--   0        0        0      461 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.8/Dockerfile
+-rw-r--r--   0        0        0    13953 2024-04-08 08:52:46.009994 pyconverters_whisperx-0.5.8/Jenkinsfile
+-rw-r--r--   0        0        0     1082 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/LICENSE
+-rw-r--r--   0        0        0     1527 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/README.md
+-rw-r--r--   0        0        0      941 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/RELEASE.md
+-rw-r--r--   0        0        0     1559 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.8/bumpversion.py
+-rw-r--r--   0        0        0       62 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.8/docs/.gitignore
+-rw-r--r--   0        0        0      268 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.8/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/docs/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.8/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.8/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2879 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/docs/conf.py
+-rw-r--r--   0        0        0      142 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/docs/index.rst
+-rw-r--r--   0        0        0       98 2024-04-08 08:35:38.562569 pyconverters_whisperx-0.5.8/mypy.ini
+-rw-r--r--   0        0        0     2227 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      969 2024-04-08 08:59:40.030824 pyconverters_whisperx-0.5.8/results.xml
+-rw-r--r--   0        0        0       48 2024-04-08 09:01:10.029616 pyconverters_whisperx-0.5.8/src/pyconverters_whisperx/__init__.py
+-rw-r--r--   0        0        0     6312 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/src/pyconverters_whisperx/whisperx.py
+-rw-r--r--   0        0        0      422 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/tests/data/test.yaml
+-rw-r--r--   0        0        0     1011 2024-04-08 08:40:40.975703 pyconverters_whisperx-0.5.8/tests/test_whisperx.py
+-rw-r--r--   0        0        0     1041 2024-04-08 08:35:38.574570 pyconverters_whisperx-0.5.8/tox.ini
+-rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 pyconverters_whisperx-0.5.8/setup.py
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 pyconverters_whisperx-0.5.8/PKG-INFO
```

### Comparing `pyconverters_whisperx-0.5.6/.gitignore` & `pyconverters_whisperx-0.5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/.idea/inspectionProfiles/Project_Default.xml` & `pyconverters_whisperx-0.5.8/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/Jenkinsfile` & `pyconverters_whisperx-0.5.8/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/LICENSE` & `pyconverters_whisperx-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/README.md` & `pyconverters_whisperx-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/RELEASE.md` & `pyconverters_whisperx-0.5.8/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/bumpversion.py` & `pyconverters_whisperx-0.5.8/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/docs/LICENSE` & `pyconverters_whisperx-0.5.8/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/docs/conf.py` & `pyconverters_whisperx-0.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/pyproject.toml` & `pyconverters_whisperx-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/results.xml` & `pyconverters_whisperx-0.5.8/results.xml`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/src/pyconverters_whisperx/whisperx.py` & `pyconverters_whisperx-0.5.8/src/pyconverters_whisperx/whisperx.py`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/tests/test_whisperx.py` & `pyconverters_whisperx-0.5.8/tests/test_whisperx.py`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/tox.ini` & `pyconverters_whisperx-0.5.8/tox.ini`

 * *Files identical despite different names*

### Comparing `pyconverters_whisperx-0.5.6/setup.py` & `pyconverters_whisperx-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
           'tox']}
 
 entry_points = \
 {'pyconverters.plugins': ['whisperx = '
                           'pyconverters_whisperx.whisperx:WhisperXConverter']}
 
 setup(name='pyconverters-whisperx',
-      version='0.5.6',
+      version='0.5.8',
       description='WhisperX converter.',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyconverters_whisperx/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyconverters_whisperx-0.5.6/PKG-INFO` & `pyconverters_whisperx-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconverters-whisperx
-Version: 0.5.6
+Version: 0.5.8
 Summary: WhisperX converter.
 Home-page: https://github.com/oterrier/pyconverters_whisperx/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

