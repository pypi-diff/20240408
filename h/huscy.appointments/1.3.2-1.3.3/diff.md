# Comparing `tmp/huscy.appointments-1.3.2.tar.gz` & `tmp/huscy.appointments-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.appointments-1.3.2.tar", last modified: Thu Sep  7 18:04:16 2023, max compression
+gzip compressed data, was "huscy.appointments-1.3.3.tar", last modified: Mon Apr  8 10:17:26 2024, max compression
```

## Comparing `huscy.appointments-1.3.2.tar` & `huscy.appointments-1.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-09-07 18:04:16.950737 huscy.appointments-1.3.2/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1036 2023-09-07 18:04:16.950737 huscy.appointments-1.3.2/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1496 2023-04-11 10:53:38.000000 huscy.appointments-1.3.2/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-09-07 18:04:16.946737 huscy.appointments-1.3.2/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-09-07 18:04:16.950737 huscy.appointments-1.3.2/huscy/appointments/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2023-09-07 17:17:31.000000 huscy.appointments-1.3.2/huscy/appointments/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      226 2020-04-27 18:13:51.000000 huscy.appointments-1.3.2/huscy/appointments/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      190 2022-06-23 09:02:55.000000 huscy.appointments-1.3.2/huscy/appointments/apps.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1472 2020-04-27 18:13:51.000000 huscy.appointments-1.3.2/huscy/appointments/feed.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      577 2020-04-27 18:13:51.000000 huscy.appointments-1.3.2/huscy/appointments/filters.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-09-07 18:04:16.950737 huscy.appointments-1.3.2/huscy/appointments/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2834 2020-04-27 18:13:51.000000 huscy.appointments-1.3.2/huscy/appointments/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4178 2020-04-27 18:13:51.000000 huscy.appointments-1.3.2/huscy/appointments/migrations/0002_auto_20200226_0735.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      453 2020-04-27 18:13:51.000000 huscy.appointments-1.3.2/huscy/appointments/migrations/0003_auto_20200226_0756.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1251 2021-10-26 09:34:30.000000 huscy.appointments-1.3.2/huscy/appointments/migrations/0004_auto_20211026_0424.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-04-27 18:13:51.000000 huscy.appointments-1.3.2/huscy/appointments/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2765 2023-04-11 10:53:38.000000 huscy.appointments-1.3.2/huscy/appointments/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2164 2020-04-27 18:13:51.000000 huscy.appointments-1.3.2/huscy/appointments/serializers.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     5198 2023-08-07 07:44:07.000000 huscy.appointments-1.3.2/huscy/appointments/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      591 2023-09-07 17:17:31.000000 huscy.appointments-1.3.2/huscy/appointments/urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      424 2020-04-27 18:13:51.000000 huscy.appointments-1.3.2/huscy/appointments/validators.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2206 2020-04-27 18:13:51.000000 huscy.appointments-1.3.2/huscy/appointments/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-09-07 18:04:16.950737 huscy.appointments-1.3.2/huscy.appointments.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1036 2023-09-07 18:04:16.000000 huscy.appointments-1.3.2/huscy.appointments.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      811 2023-09-07 18:04:16.000000 huscy.appointments-1.3.2/huscy.appointments.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-09-07 18:04:16.000000 huscy.appointments-1.3.2/huscy.appointments.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      129 2023-09-07 18:04:16.000000 huscy.appointments-1.3.2/huscy.appointments.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-09-07 18:04:16.000000 huscy.appointments-1.3.2/huscy.appointments.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-09-07 18:04:16.950737 huscy.appointments-1.3.2/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1364 2023-04-11 10:53:38.000000 huscy.appointments-1.3.2/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-04-08 10:17:26.547077 huscy.appointments-1.3.3/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1048 2024-04-08 10:17:26.547077 huscy.appointments-1.3.3/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1491 2024-03-22 13:05:40.000000 huscy.appointments-1.3.3/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-04-08 10:17:26.543077 huscy.appointments-1.3.3/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-04-08 10:17:26.547077 huscy.appointments-1.3.3/huscy/appointments/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2024-03-22 13:05:40.000000 huscy.appointments-1.3.3/huscy/appointments/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      226 2020-04-27 18:13:51.000000 huscy.appointments-1.3.3/huscy/appointments/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      190 2022-06-23 09:02:55.000000 huscy.appointments-1.3.3/huscy/appointments/apps.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1472 2020-04-27 18:13:51.000000 huscy.appointments-1.3.3/huscy/appointments/feed.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      577 2020-04-27 18:13:51.000000 huscy.appointments-1.3.3/huscy/appointments/filters.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-04-08 10:17:26.547077 huscy.appointments-1.3.3/huscy/appointments/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2834 2020-04-27 18:13:51.000000 huscy.appointments-1.3.3/huscy/appointments/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4178 2020-04-27 18:13:51.000000 huscy.appointments-1.3.3/huscy/appointments/migrations/0002_auto_20200226_0735.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      453 2020-04-27 18:13:51.000000 huscy.appointments-1.3.3/huscy/appointments/migrations/0003_auto_20200226_0756.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1251 2021-10-26 09:34:30.000000 huscy.appointments-1.3.3/huscy/appointments/migrations/0004_auto_20211026_0424.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-04-27 18:13:51.000000 huscy.appointments-1.3.3/huscy/appointments/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2765 2023-04-11 10:53:38.000000 huscy.appointments-1.3.3/huscy/appointments/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2164 2020-04-27 18:13:51.000000 huscy.appointments-1.3.3/huscy/appointments/serializers.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     5198 2023-08-07 07:44:07.000000 huscy.appointments-1.3.3/huscy/appointments/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      591 2023-09-07 17:17:31.000000 huscy.appointments-1.3.3/huscy/appointments/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      424 2020-04-27 18:13:51.000000 huscy.appointments-1.3.3/huscy/appointments/validators.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2206 2020-04-27 18:13:51.000000 huscy.appointments-1.3.3/huscy/appointments/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-04-08 10:17:26.543077 huscy.appointments-1.3.3/huscy.appointments.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1048 2024-04-08 10:17:26.000000 huscy.appointments-1.3.3/huscy.appointments.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      811 2024-04-08 10:17:26.000000 huscy.appointments-1.3.3/huscy.appointments.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2024-04-08 10:17:26.000000 huscy.appointments-1.3.3/huscy.appointments.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      129 2024-04-08 10:17:26.000000 huscy.appointments-1.3.3/huscy.appointments.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2024-04-08 10:17:26.000000 huscy.appointments-1.3.3/huscy.appointments.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2024-04-08 10:17:26.547077 huscy.appointments-1.3.3/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1376 2024-03-22 13:05:40.000000 huscy.appointments-1.3.3/setup.py
```

### Comparing `huscy.appointments-1.3.2/PKG-INFO` & `huscy.appointments-1.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.appointments
-Version: 1.3.2
+Version: 1.3.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: UNKNOWN
 Platform: UNKNOWN
@@ -14,13 +14,13 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.appointments-1.3.2/README.md` & `huscy.appointments-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Requirements
 ------
 
 - Python 3.8+
 - A supported version of Django
 
-Tox tests on Django versions 3.2, 4.1 and 4.2.
+Tox tests on Django versions 4.2 and 5.0.
 
 
 
 Installation
 ------
 
 To install `husy.appointments` simply run:
```

### Comparing `huscy.appointments-1.3.2/huscy/appointments/feed.py` & `huscy.appointments-1.3.3/huscy/appointments/feed.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.2/huscy/appointments/filters.py` & `huscy.appointments-1.3.3/huscy/appointments/filters.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.2/huscy/appointments/migrations/0001_initial.py` & `huscy.appointments-1.3.3/huscy/appointments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.2/huscy/appointments/migrations/0002_auto_20200226_0735.py` & `huscy.appointments-1.3.3/huscy/appointments/migrations/0002_auto_20200226_0735.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.2/huscy/appointments/migrations/0004_auto_20211026_0424.py` & `huscy.appointments-1.3.3/huscy/appointments/migrations/0004_auto_20211026_0424.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.2/huscy/appointments/models.py` & `huscy.appointments-1.3.3/huscy/appointments/models.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.2/huscy/appointments/serializers.py` & `huscy.appointments-1.3.3/huscy/appointments/serializers.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.2/huscy/appointments/services.py` & `huscy.appointments-1.3.3/huscy/appointments/services.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.2/huscy/appointments/urls.py` & `huscy.appointments-1.3.3/huscy/appointments/urls.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.2/huscy/appointments/views.py` & `huscy.appointments-1.3.3/huscy/appointments/views.py`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.2/huscy.appointments.egg-info/PKG-INFO` & `huscy.appointments-1.3.3/huscy.appointments.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.appointments
-Version: 1.3.2
+Version: 1.3.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: UNKNOWN
 Platform: UNKNOWN
@@ -14,13 +14,13 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.appointments-1.3.2/huscy.appointments.egg-info/SOURCES.txt` & `huscy.appointments-1.3.3/huscy.appointments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.appointments-1.3.2/setup.py` & `huscy.appointments-1.3.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
     author='Alexander Tyapkov, Mathias Goldau, Stefan Bunde',
     author_email='tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de',
 
     packages=find_namespace_packages(include=['huscy.*']),
 
     install_requires=[
-        "Django>=3.2",
-        "djangorestframework>=3.11",
+        "Django>=4.2",
+        "djangorestframework>=3.14",
         "django-filter>=2.3",
         "django-ical>=1.4",
     ],
     extras_require={
         'development': ['psycopg2-binary'],
         'testing': ['tox', 'watchdog'],
     },
@@ -31,13 +31,13 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.1',
         'Framework :: Django :: 4.2',
+        'Framework :: Django :: 5.0',
     ],
 )
```

