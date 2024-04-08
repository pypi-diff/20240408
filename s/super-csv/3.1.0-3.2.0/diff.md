# Comparing `tmp/super-csv-3.1.0.tar.gz` & `tmp/super-csv-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super-csv-3.1.0.tar", last modified: Tue Aug  1 18:28:49 2023, max compression
+gzip compressed data, was "super-csv-3.2.0.tar", last modified: Mon Apr  8 19:07:54 2024, max compression
```

## Comparing `super-csv-3.1.0.tar` & `super-csv-3.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.759004 super-csv-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-08-01 18:28:43.000000 super-csv-3.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-08-01 18:28:43.000000 super-csv-3.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-08-01 18:28:43.000000 super-csv-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8672 2023-08-01 18:28:49.759004 super-csv-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4253 2023-08-01 18:28:43.000000 super-csv-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.751004 super-csv-3.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      313 2023-08-01 18:28:43.000000 super-csv-3.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-08-01 18:28:49.759004 super-csv-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-08-01 18:28:43.000000 super-csv-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.755004 super-csv-3.1.0/super_csv/
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      321 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/common_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)    11036 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/csv_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.759004 super-csv-3.1.0/super_csv/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      587 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/migrations/0002_csvoperation_user.py
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/migrations/0003_csvoperation_original_filename.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7410 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     2785 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      478 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.751004 super-csv-3.1.0/super_csv/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.759004 super-csv-3.1.0/super_csv/templates/super_csv/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/templates/super_csv/base.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.755004 super-csv-3.1.0/super_csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8672 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      846 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.759004 super-csv-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     9259 2023-08-01 18:28:43.000000 super-csv-3.1.0/tests/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-08-01 18:28:43.000000 super-csv-3.1.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-08-01 18:28:43.000000 super-csv-3.1.0/tests/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:07:54.845806 super-csv-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-08 19:07:38.000000 super-csv-3.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 19:07:38.000000 super-csv-3.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 19:07:38.000000 super-csv-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-04-08 19:07:54.845806 super-csv-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-08 19:07:38.000000 super-csv-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:07:54.837806 super-csv-3.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 19:07:38.000000 super-csv-3.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-08 19:07:54.845806 super-csv-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-08 19:07:38.000000 super-csv-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:07:54.841806 super-csv-3.2.0/super_csv/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/common_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/csv_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:07:54.841806 super-csv-3.2.0/super_csv/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/migrations/0002_csvoperation_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/migrations/0003_csvoperation_original_filename.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:07:54.837806 super-csv-3.2.0/super_csv/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:07:54.841806 super-csv-3.2.0/super_csv/templates/super_csv/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-08 19:07:38.000000 super-csv-3.2.0/super_csv/templates/super_csv/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:07:54.845806 super-csv-3.2.0/super_csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-04-08 19:07:54.000000 super-csv-3.2.0/super_csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-08 19:07:54.000000 super-csv-3.2.0/super_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:07:54.000000 super-csv-3.2.0/super_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 19:07:54.000000 super-csv-3.2.0/super_csv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:07:54.000000 super-csv-3.2.0/super_csv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 19:07:54.000000 super-csv-3.2.0/super_csv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 19:07:54.000000 super-csv-3.2.0/super_csv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:07:54.845806 super-csv-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9259 2024-04-08 19:07:38.000000 super-csv-3.2.0/tests/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-08 19:07:38.000000 super-csv-3.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-08 19:07:38.000000 super-csv-3.2.0/tests/test_serializers.py
```

### Comparing `super-csv-3.1.0/CHANGELOG.rst` & `super-csv-3.2.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+[3.2.0] - 2023-07-31
+~~~~~~~~~~~~~~~~~~~~
+
+* Added support of python 3.11 and 3.12
+* Dropped django32 support.
+
 
 [3.1.0] - 2023-07-31
 ~~~~~~~~~~~~~~~~~~~~
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
   more details.
```

### Comparing `super-csv-3.1.0/PKG-INFO` & `super-csv-3.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: super-csv
-Version: 3.1.0
+Version: 3.2.0
 Summary: CSV Processor
 Home-page: https://github.com/openedx/super-csv
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: Django
+Requires-Dist: django-crum
+Requires-Dist: django-model-utils
+Requires-Dist: edx-django-utils>=3.12.0
+Requires-Dist: simplejson
+Requires-Dist: djangorestframework
+Requires-Dist: edx-celeryutils
 
 super-csv
 =============================
 
 |pypi-badge| |CI| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
 
@@ -100,15 +108,15 @@
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/super-csv/blob/master/.github/ISSUE_TEMPLATE.md>`_.
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
 
@@ -151,14 +159,20 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+[3.2.0] - 2023-07-31
+~~~~~~~~~~~~~~~~~~~~
+
+* Added support of python 3.11 and 3.12
+* Dropped django32 support.
+
 
 [3.1.0] - 2023-07-31
 ~~~~~~~~~~~~~~~~~~~~
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
   more details.
```

### Comparing `super-csv-3.1.0/README.rst` & `super-csv-3.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/super-csv/blob/master/.github/ISSUE_TEMPLATE.md>`_.
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
```

### Comparing `super-csv-3.1.0/setup.cfg` & `super-csv-3.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `super-csv-3.1.0/setup.py` & `super-csv-3.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,21 +80,22 @@
     install_requires=load_requirements('requirements/base.in'),
     license="Apache 2.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     entry_points={
         'lms.djangoapp': [
             "super_csv = super_csv.apps:SuperCSVConfig",
         ],
     }
 )
```

### Comparing `super-csv-3.1.0/super_csv/csv_processor.py` & `super-csv-3.2.0/super_csv/csv_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -289,15 +289,15 @@
             rownum, row = self.stage.pop(0)
             try:
                 did_save, rollback_row = self.process_row(row)
                 if did_save:
                     saved += 1
                     if rollback_row:
                         self.rollback_rows.append((rownum, rollback_row))
-            except Exception as e:  # pylint: disable=broad-except
+            except Exception as e:
                 log.exception('Committing %r', self)
                 self.add_error(str(e), row=rownum)
                 if self.result_data:
                     self.result_data[rownum - 1]['error'] = str(e)
                     self.result_data[rownum - 1]['status'] = _('Failure')
         self.saved_rows = saved
         log.info('%r committed %d rows', self, saved)
@@ -309,15 +309,15 @@
         saved = 0
         while self.rollback_rows:
             rownum, row = self.rollback_rows.pop(0)
             try:
                 did_save, __ = self.process_row(row)
                 if did_save:
                     saved += 1
-            except Exception as e:  # pylint: disable=broad-except
+            except Exception as e:
                 log.exception('Rolling back %r', self)
                 self.add_error(str(e), row=rownum)
         self.saved_rows = saved
 
     def status(self):
         """
         Return a status dict.
```

### Comparing `super-csv-3.1.0/super_csv/migrations/0001_initial.py` & `super-csv-3.2.0/super_csv/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.1.0/super_csv/migrations/0002_csvoperation_user.py` & `super-csv-3.2.0/super_csv/migrations/0002_csvoperation_user.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.1.0/super_csv/mixins.py` & `super-csv-3.2.0/super_csv/mixins.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.1.0/super_csv/models.py` & `super-csv-3.2.0/super_csv/models.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.1.0/super_csv/serializers.py` & `super-csv-3.2.0/super_csv/serializers.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.1.0/super_csv/signals.py` & `super-csv-3.2.0/super_csv/signals.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.1.0/super_csv/templates/super_csv/base.html` & `super-csv-3.2.0/super_csv/templates/super_csv/base.html`

 * *Files identical despite different names*

### Comparing `super-csv-3.1.0/super_csv.egg-info/PKG-INFO` & `super-csv-3.2.0/super_csv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: super-csv
-Version: 3.1.0
+Version: 3.2.0
 Summary: CSV Processor
 Home-page: https://github.com/openedx/super-csv
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: Django
+Requires-Dist: django-crum
+Requires-Dist: django-model-utils
+Requires-Dist: edx-django-utils>=3.12.0
+Requires-Dist: simplejson
+Requires-Dist: djangorestframework
+Requires-Dist: edx-celeryutils
 
 super-csv
 =============================
 
 |pypi-badge| |CI| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
 
@@ -100,15 +108,15 @@
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/super-csv/blob/master/.github/ISSUE_TEMPLATE.md>`_.
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
 
@@ -151,14 +159,20 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+[3.2.0] - 2023-07-31
+~~~~~~~~~~~~~~~~~~~~
+
+* Added support of python 3.11 and 3.12
+* Dropped django32 support.
+
 
 [3.1.0] - 2023-07-31
 ~~~~~~~~~~~~~~~~~~~~
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
   more details.
```

### Comparing `super-csv-3.1.0/super_csv.egg-info/SOURCES.txt` & `super-csv-3.2.0/super_csv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `super-csv-3.1.0/tests/test_csv.py` & `super-csv-3.2.0/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.1.0/tests/test_models.py` & `super-csv-3.2.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.1.0/tests/test_serializers.py` & `super-csv-3.2.0/tests/test_serializers.py`

 * *Files identical despite different names*

