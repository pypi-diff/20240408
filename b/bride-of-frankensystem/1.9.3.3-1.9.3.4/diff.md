# Comparing `tmp/bride-of-frankensystem-1.9.3.3.tar.gz` & `tmp/bride-of-frankensystem-1.9.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\colby\Desktop\git\bride-of-frankensystem\dist\.tmp-zhcoez0i\bride-of-frankensystem-1.9.3.3.tar", last modified: Fri Apr  5 20:46:07 2024, max compression
+gzip compressed data, was "C:\Users\colby\Desktop\git\bride-of-frankensystem\dist\.tmp-7bc4suk5\bride-of-frankensystem-1.9.3.4.tar", last modified: Mon Apr  8 06:26:10 2024, max compression
```

## Comparing `bride-of-frankensystem-1.9.3.3.tar` & `bride-of-frankensystem-1.9.3.4.tar`

### file list

```diff
@@ -1,107 +1,124 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/
--rw-rw-rw-   0        0        0    13929 2024-04-02 04:10:20.000000 bride-of-frankensystem-1.9.3.3/BOFS/BOFSFlask.py
--rw-rw-rw-   0        0        0     3937 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.3/BOFS/BOFSSession.py
--rw-rw-rw-   0        0        0    10540 2024-04-03 05:08:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/JSONQuestionnaire.py
--rw-rw-rw-   0        0        0     5740 2024-04-01 07:10:51.000000 bride-of-frankensystem-1.9.3.3/BOFS/JSONTable.py
--rw-rw-rw-   0        0        0     5635 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.3/BOFS/PageList.py
--rw-rw-rw-   0        0        0      117 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.3/BOFS/__init__.py
--rw-rw-rw-   0        0        0       65 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.3/BOFS/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/
--rw-rw-rw-   0        0        0     7006 2024-03-27 03:35:45.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/QuestionnaireResults.py
--rw-rw-rw-   0        0        0       22 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/
--rw-rw-rw-   0        0        0     2007 2022-05-19 18:13:22.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/QuestionnaireResults.cpython-310.pyc
--rw-rw-rw-   0        0        0     3476 2024-03-27 03:36:06.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/QuestionnaireResults.cpython-311.pyc
--rw-rw-rw-   0        0        0      181 2022-05-18 21:12:21.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      252 2024-01-19 17:54:16.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    10843 2024-03-27 03:36:06.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/export_helpers.cpython-311.pyc
--rw-rw-rw-   0        0        0     3420 2022-07-15 22:52:11.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/util.cpython-310.pyc
--rw-rw-rw-   0        0        0     5979 2024-01-19 17:54:16.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/util.cpython-311.pyc
--rw-rw-rw-   0        0        0    14352 2022-07-15 22:51:49.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0    22823 2024-03-27 04:06:39.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/views.cpython-311.pyc
--rw-rw-rw-   0        0        0    10020 2024-03-27 03:35:45.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/export_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/
--rw-rw-rw-   0        0        0     1142 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/export.html
--rw-rw-rw-   0        0        0      304 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/export_csv.html
--rw-rw-rw-   0        0        0      967 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/login_admin.html
--rw-rw-rw-   0        0        0     1340 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/preview_questionnaire.html
--rw-rw-rw-   0        0        0      283 2024-04-02 04:25:23.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/preview_questionnaire_simple.html
--rw-rw-rw-   0        0        0      809 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/progress.html
--rw-rw-rw-   0        0        0     1780 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/progress_ajax.html
--rw-rw-rw-   0        0        0     3017 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/progress_summary_ajax.html
--rw-rw-rw-   0        0        0     3517 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/questionnaire_results.html
--rw-rw-rw-   0        0        0     1388 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/results.html
--rw-rw-rw-   0        0        0     1359 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/table_ajax.html
--rw-rw-rw-   0        0        0     1020 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/table_view.html
--rw-rw-rw-   0        0        0     5505 2024-04-02 04:24:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/template_admin.html
--rw-rw-rw-   0        0        0     3141 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/util.py
--rw-rw-rw-   0        0        0    14926 2024-03-27 04:06:09.000000 bride-of-frankensystem-1.9.3.3/BOFS/admin/views.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/bride_of_frankensystem.egg-info/
--rw-rw-rw-   0        0        0    12537 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/bride_of_frankensystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/bride_of_frankensystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/bride_of_frankensystem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/bride_of_frankensystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.3/BOFS/bride_of_frankensystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1286 2024-01-07 00:02:19.000000 bride-of-frankensystem-1.9.3.3/BOFS/cli.py
--rw-rw-rw-   0        0        0     3682 2024-04-01 21:58:33.000000 bride-of-frankensystem-1.9.3.3/BOFS/create_app.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/default/
--rw-rw-rw-   0        0        0       22 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/default/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/default/__pycache__/
--rw-rw-rw-   0        0        0      183 2022-05-18 21:12:21.000000 bride-of-frankensystem-1.9.3.3/BOFS/default/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      236 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/default/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     6970 2022-07-15 22:13:35.000000 bride-of-frankensystem-1.9.3.3/BOFS/default/__pycache__/models.cpython-310.pyc
--rw-rw-rw-   0        0        0    14869 2024-04-03 05:08:19.000000 bride-of-frankensystem-1.9.3.3/BOFS/default/__pycache__/models.cpython-311.pyc
--rw-rw-rw-   0        0        0     9983 2022-07-15 22:13:35.000000 bride-of-frankensystem-1.9.3.3/BOFS/default/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0    23256 2024-04-03 06:09:58.000000 bride-of-frankensystem-1.9.3.3/BOFS/default/__pycache__/views.cpython-311.pyc
--rw-rw-rw-   0        0        0     9195 2024-04-03 19:53:28.000000 bride-of-frankensystem-1.9.3.3/BOFS/default/models.py
--rw-rw-rw-   0        0        0    17678 2024-04-03 06:04:46.000000 bride-of-frankensystem-1.9.3.3/BOFS/default/views.py
--rw-rw-rw-   0        0        0     2036 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.3/BOFS/globals.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/img/
--rw-rw-rw-   0        0        0     1235 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/img/check.png
--rw-rw-rw-   0        0        0    26229 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/img/spinner32.gif
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/js/
--rw-rw-rw-   0        0        0    58078 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0    88147 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/js/jquery-3.4.1.min.js
--rw-rw-rw-   0        0        0  1219235 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/js/plotly-latest.min.js
--rw-rw-rw-   0        0        0    21009 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/js/popper.min.js
--rw-rw-rw-   0        0        0     9389 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/loading.gif
--rw-rw-rw-   0        0        0      253 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/logo.png
--rw-rw-rw-   0        0        0     2929 2023-10-09 16:15:27.000000 bride-of-frankensystem-1.9.3.3/BOFS/static/style.css
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/
--rw-rw-rw-   0        0        0     3650 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/consent.html
--rw-rw-rw-   0        0        0      651 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/end.html
--rw-rw-rw-   0        0        0     1188 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/external_id.html
--rw-rw-rw-   0        0        0      345 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/instructions.html
--rw-rw-rw-   0        0        0      319 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questionnaire.html
--rw-rw-rw-   0        0        0     1521 2024-04-02 03:30:14.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questionnaire_macro.html
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/
--rw-rw-rw-   0        0        0      467 2024-04-02 03:24:53.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/checklist.html
--rw-rw-rw-   0        0        0      426 2024-04-02 04:10:41.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/drop_down.html
--rw-rw-rw-   0        0        0      321 2024-04-02 04:11:05.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/field.html
--rw-rw-rw-   0        0        0      376 2024-04-02 04:11:25.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/multi_field.html
--rw-rw-rw-   0        0        0      374 2024-04-02 04:11:53.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/num_field.html
--rw-rw-rw-   0        0        0     1453 2024-04-02 05:17:59.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/radiogrid.html
--rw-rw-rw-   0        0        0      672 2024-04-02 04:12:29.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/radiolist.html
--rw-rw-rw-   0        0        0      541 2024-04-02 04:12:43.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/slider.html
--rw-rw-rw-   0        0        0       26 2024-04-02 03:06:08.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/textview.html
--rw-rw-rw-   0        0        0      136 2024-04-01 21:52:17.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/simple.html
--rw-rw-rw-   0        0        0     5770 2024-04-02 03:28:54.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/template.html
--rw-rw-rw-   0        0        0     3722 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/unity_webgl.html
--rw-rw-rw-   0        0        0     4224 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.3/BOFS/templates/unity_webgl_fullscreen.html
--rw-rw-rw-   0        0        0    11904 2024-01-29 02:11:16.000000 bride-of-frankensystem-1.9.3.3/BOFS/util.py
--rw-rw-rw-   0        0        0     7817 2022-05-18 16:56:46.000000 bride-of-frankensystem-1.9.3.3/LICENSE
--rw-rw-rw-   0        0        0       46 2024-04-05 20:45:50.000000 bride-of-frankensystem-1.9.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0    12537 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2731 2024-03-27 04:18:48.000000 bride-of-frankensystem-1.9.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/bride_of_frankensystem.egg-info/
--rw-rw-rw-   0        0        0    12537 2024-04-05 20:46:06.000000 bride-of-frankensystem-1.9.3.3/bride_of_frankensystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3219 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/bride_of_frankensystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:46:06.000000 bride-of-frankensystem-1.9.3.3/bride_of_frankensystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-05 20:46:06.000000 bride-of-frankensystem-1.9.3.3/bride_of_frankensystem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2024-04-05 20:46:06.000000 bride-of-frankensystem-1.9.3.3/bride_of_frankensystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-05 20:46:06.000000 bride-of-frankensystem-1.9.3.3/bride_of_frankensystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1020 2024-04-05 20:43:57.000000 bride-of-frankensystem-1.9.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 20:46:07.000000 bride-of-frankensystem-1.9.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/
+-rw-rw-rw-   0        0        0    13929 2024-04-02 04:10:20.000000 bride-of-frankensystem-1.9.3.4/BOFS/BOFSFlask.py
+-rw-rw-rw-   0        0        0     3937 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.4/BOFS/BOFSSession.py
+-rw-rw-rw-   0        0        0    10547 2024-04-07 06:00:46.000000 bride-of-frankensystem-1.9.3.4/BOFS/JSONQuestionnaire.py
+-rw-rw-rw-   0        0        0     5740 2024-04-01 07:10:51.000000 bride-of-frankensystem-1.9.3.4/BOFS/JSONTable.py
+-rw-rw-rw-   0        0        0     5635 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.4/BOFS/PageList.py
+-rw-rw-rw-   0        0        0      117 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.4/BOFS/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.4/BOFS/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/
+-rw-rw-rw-   0        0        0    18902 2024-04-05 21:05:42.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/BOFSFlask.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5318 2024-04-05 21:05:43.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/BOFSSession.cpython-311.pyc
+-rw-rw-rw-   0        0        0    15725 2024-04-07 06:00:50.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/JSONQuestionnaire.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8044 2024-04-05 21:05:43.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/JSONTable.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6815 2024-04-05 21:05:43.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/PageList.cpython-311.pyc
+-rw-rw-rw-   0        0        0      384 2024-04-05 21:05:42.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      337 2024-04-06 05:50:26.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/__main__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1998 2024-04-06 05:50:26.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/cli.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4238 2024-04-06 05:50:26.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/create_app.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2811 2024-04-05 21:05:43.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/globals.cpython-311.pyc
+-rw-rw-rw-   0        0        0    17197 2024-04-08 05:03:03.000000 bride-of-frankensystem-1.9.3.4/BOFS/__pycache__/util.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/
+-rw-rw-rw-   0        0        0     7006 2024-03-27 03:35:45.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/QuestionnaireResults.py
+-rw-rw-rw-   0        0        0       22 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/
+-rw-rw-rw-   0        0        0     2007 2022-05-19 18:13:22.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/QuestionnaireResults.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3476 2024-03-27 03:36:06.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/QuestionnaireResults.cpython-311.pyc
+-rw-rw-rw-   0        0        0      181 2022-05-18 21:12:21.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      252 2024-01-19 17:54:16.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    11147 2024-04-08 06:14:58.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/export_helpers.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3420 2022-07-15 22:52:11.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/util.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6084 2024-04-07 18:55:20.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/util.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14352 2022-07-15 22:51:49.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0    29316 2024-04-08 06:22:29.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/views.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10252 2024-04-08 06:13:56.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/export_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/
+-rw-rw-rw-   0        0        0      844 2024-04-07 19:31:03.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/database_delete.html
+-rw-rw-rw-   0        0        0     1716 2024-04-08 05:56:48.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/export.html
+-rw-rw-rw-   0        0        0      304 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/export_csv.html
+-rw-rw-rw-   0        0        0      877 2024-04-08 06:24:14.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/login_admin.html
+-rw-rw-rw-   0        0        0     2490 2024-04-08 04:55:02.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/preview_questionnaire.html
+-rw-rw-rw-   0        0        0      283 2024-04-02 04:25:23.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/preview_questionnaire_simple.html
+-rw-rw-rw-   0        0        0      606 2024-04-08 05:52:37.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/progress.html
+-rw-rw-rw-   0        0        0     2369 2024-04-08 05:37:40.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/progress_ajax.html
+-rw-rw-rw-   0        0        0     3196 2024-04-07 19:09:11.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/progress_summary_ajax.html
+-rw-rw-rw-   0        0        0     3517 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/questionnaire_results.html
+-rw-rw-rw-   0        0        0     1388 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/results.html
+-rw-rw-rw-   0        0        0     1366 2024-04-07 05:58:54.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/table_ajax.html
+-rw-rw-rw-   0        0        0     1056 2024-04-07 18:32:29.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/table_view.html
+-rw-rw-rw-   0        0        0     5018 2024-04-07 19:06:30.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/template_admin.html
+-rw-rw-rw-   0        0        0     1056 2024-04-07 19:28:04.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/template_admin_head.html
+-rw-rw-rw-   0        0        0     3182 2024-04-07 18:55:17.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/util.py
+-rw-rw-rw-   0        0        0    19208 2024-04-08 06:22:04.000000 bride-of-frankensystem-1.9.3.4/BOFS/admin/views.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/bride_of_frankensystem.egg-info/
+-rw-rw-rw-   0        0        0    12537 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.4/BOFS/bride_of_frankensystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.4/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.4/BOFS/bride_of_frankensystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.4/BOFS/bride_of_frankensystem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.4/BOFS/bride_of_frankensystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.4/BOFS/bride_of_frankensystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1286 2024-01-07 00:02:19.000000 bride-of-frankensystem-1.9.3.4/BOFS/cli.py
+-rw-rw-rw-   0        0        0     3682 2024-04-01 21:58:33.000000 bride-of-frankensystem-1.9.3.4/BOFS/create_app.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/default/
+-rw-rw-rw-   0        0        0       22 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/default/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/default/__pycache__/
+-rw-rw-rw-   0        0        0      183 2022-05-18 21:12:21.000000 bride-of-frankensystem-1.9.3.4/BOFS/default/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      236 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/default/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6970 2022-07-15 22:13:35.000000 bride-of-frankensystem-1.9.3.4/BOFS/default/__pycache__/models.cpython-310.pyc
+-rw-rw-rw-   0        0        0    15043 2024-04-08 04:59:08.000000 bride-of-frankensystem-1.9.3.4/BOFS/default/__pycache__/models.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9983 2022-07-15 22:13:35.000000 bride-of-frankensystem-1.9.3.4/BOFS/default/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0    23422 2024-04-07 18:36:40.000000 bride-of-frankensystem-1.9.3.4/BOFS/default/__pycache__/views.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9419 2024-04-08 04:57:33.000000 bride-of-frankensystem-1.9.3.4/BOFS/default/models.py
+-rw-rw-rw-   0        0        0    17838 2024-04-07 18:36:38.000000 bride-of-frankensystem-1.9.3.4/BOFS/default/views.py
+-rw-rw-rw-   0        0        0     2036 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.4/BOFS/globals.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/
+-rw-rw-rw-   0        0        0   103009 2024-04-06 05:46:45.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/all.min.css
+-rw-rw-rw-   0        0        0   232803 2024-04-06 05:38:05.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/img/
+-rw-rw-rw-   0        0        0     1235 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/img/check.png
+-rw-rw-rw-   0        0        0    26229 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/img/spinner32.gif
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/js/
+-rw-rw-rw-   0        0        0    80721 2024-04-06 05:35:59.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    48036 2024-04-06 05:47:33.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/js/htmx.min.js
+-rw-rw-rw-   0        0        0    87533 2024-04-06 05:34:06.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/js/jquery-3.7.1.min.js
+-rw-rw-rw-   0        0        0      360 2024-04-06 05:47:54.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/js/json-enc.js
+-rw-rw-rw-   0        0        0     9389 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/loading.gif
+-rw-rw-rw-   0        0        0      253 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/logo.png
+-rw-rw-rw-   0        0        0     2958 2024-04-07 19:19:18.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/style.css
+-rw-rw-rw-   0        0        0     2057 2024-04-07 19:30:25.000000 bride-of-frankensystem-1.9.3.4/BOFS/static/style_admin.css
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/
+-rw-rw-rw-   0        0        0     3650 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/consent.html
+-rw-rw-rw-   0        0        0      651 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/end.html
+-rw-rw-rw-   0        0        0     1188 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/external_id.html
+-rw-rw-rw-   0        0        0      345 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/instructions.html
+-rw-rw-rw-   0        0        0      319 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questionnaire.html
+-rw-rw-rw-   0        0        0     1521 2024-04-02 03:30:14.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questionnaire_macro.html
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/
+-rw-rw-rw-   0        0        0      467 2024-04-02 03:24:53.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/checklist.html
+-rw-rw-rw-   0        0        0      426 2024-04-02 04:10:41.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/drop_down.html
+-rw-rw-rw-   0        0        0      321 2024-04-02 04:11:05.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/field.html
+-rw-rw-rw-   0        0        0      376 2024-04-02 04:11:25.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/multi_field.html
+-rw-rw-rw-   0        0        0      374 2024-04-02 04:11:53.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/num_field.html
+-rw-rw-rw-   0        0        0     1453 2024-04-02 05:17:59.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/radiogrid.html
+-rw-rw-rw-   0        0        0      672 2024-04-02 04:12:29.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/radiolist.html
+-rw-rw-rw-   0        0        0      541 2024-04-02 04:12:43.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/slider.html
+-rw-rw-rw-   0        0        0       26 2024-04-02 03:06:08.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/textview.html
+-rw-rw-rw-   0        0        0      136 2024-04-01 21:52:17.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/simple.html
+-rw-rw-rw-   0        0        0     5646 2024-04-07 06:04:14.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/template.html
+-rw-rw-rw-   0        0        0     3722 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/unity_webgl.html
+-rw-rw-rw-   0        0        0     4224 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.4/BOFS/templates/unity_webgl_fullscreen.html
+-rw-rw-rw-   0        0        0    12043 2024-04-08 05:02:59.000000 bride-of-frankensystem-1.9.3.4/BOFS/util.py
+-rw-rw-rw-   0        0        0     7817 2022-05-18 16:56:46.000000 bride-of-frankensystem-1.9.3.4/LICENSE
+-rw-rw-rw-   0        0        0       46 2024-04-05 20:45:50.000000 bride-of-frankensystem-1.9.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    12537 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2731 2024-03-27 04:18:48.000000 bride-of-frankensystem-1.9.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/bride_of_frankensystem.egg-info/
+-rw-rw-rw-   0        0        0    12537 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/bride_of_frankensystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3853 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/bride_of_frankensystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/bride_of_frankensystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/bride_of_frankensystem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/bride_of_frankensystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/bride_of_frankensystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1020 2024-04-08 06:25:34.000000 bride-of-frankensystem-1.9.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 06:26:10.000000 bride-of-frankensystem-1.9.3.4/setup.cfg
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/BOFSFlask.py` & `bride-of-frankensystem-1.9.3.4/BOFS/BOFSFlask.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/BOFSSession.py` & `bride-of-frankensystem-1.9.3.4/BOFS/BOFSSession.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/JSONQuestionnaire.py` & `bride-of-frankensystem-1.9.3.4/BOFS/JSONQuestionnaire.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
         self.db_class = type(self.file_name, (db.Model,), table_attr)
 
     # Replace field_name with self.field_name
     def preprocess_calculation_string(self, calculationString):
         for field in self.fields:
             calculationString = re.sub("{}(?=,|\]|\)|-|\+|/|\*| |$)".
-                                       format(field.id), "getattr(self, '{}')".format(field.id), calculationString)
+                                       format(field.id), "float(getattr(self, '{}'))".format(field.id), calculationString)
 
         return calculationString
 
     def create_blank(self):
         blank = self.db_class()
 
         for column in blank.__table__.c:
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/JSONTable.py` & `bride-of-frankensystem-1.9.3.4/BOFS/JSONTable.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/PageList.py` & `bride-of-frankensystem-1.9.3.4/BOFS/PageList.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/QuestionnaireResults.py` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/QuestionnaireResults.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/QuestionnaireResults.cpython-310.pyc` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/QuestionnaireResults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/QuestionnaireResults.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/QuestionnaireResults.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/export_helpers.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/export_helpers.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,26 +1,26 @@
 magic:    0xa70d0d0a
-moddate:  0x11940366 (Wed Mar 27 03:35:45 2024 UTC)
-files sz: 10020
+moddate:  0x248b1366 (Mon Apr  8 06:13:56 2024 UTC)
+files sz: 10252
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c045a
       04640364046c056d065a066d075a076d085a080100640064056c096d0a5a
-      0a01006406650b6602640784045a0c090064116409650d650e1900000000
-      0000000000640a650b640b65046a0f00000000000000006a100000000000
-      0000006606640c84055a11090064116409650d650e190000000000000000
-      00640a650b640d65046a0f00000000000000006a10000000000000000064
-      0b64026608640e84055a12090064116409650d650e190000000000000000
-      00640a650b640d65046a0f00000000000000006a10000000000000000064
-      0b64026608640f84055a136409650d650e19000000000000000000640a65
-      0b640b650e6606641084045a1464025300
+      0a01006406650b6602640784045a0c0900090064116409650d650e190000
+      00000000000000640a650b640b65046a0f00000000000000006a10000000
+      00000000006606640c84055a11090064126409650d650e19000000000000
+      000000640a650b640d65046a0f00000000000000006a1000000000000000
+      00640b64026608640e84055a12090064126409650d650e19000000000000
+      000000640a650b640d65046a0f00000000000000006a1000000000000000
+      00640b64026608640f84055a136409650d650e1900000000000000000064
+      0a650b640b650e6606641084045a1464025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('db', 'questionnaires', 'page_list'))
                  6 IMPORT_NAME              0 (BOFS.globals)
                  8 IMPORT_FROM              1 (db)
                 10 STORE_NAME               1 (db)
@@ -58,100 +58,102 @@
                 66 BUILD_TUPLE              2
                 68 LOAD_CONST               7 (<code object create_export_base_query, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 7>)
                 70 MAKE_FUNCTION            4 (annotations)
                 72 STORE_NAME              12 (create_export_base_query)
    
     88          74 NOP
    
-    86          76 LOAD_CONST              17 ((True,))
-                78 LOAD_CONST               9 ('column_list')
-                80 LOAD_NAME               13 (list)
-                82 LOAD_NAME               14 (str)
-                84 BINARY_SUBSCR
-                94 LOAD_CONST              10 ('export_data')
-   
-    87          96 LOAD_NAME               11 (dict)
-   
-    86          98 LOAD_CONST              11 ('return')
-   
-    88         100 LOAD_NAME                4 (sqlalchemy)
-               102 LOAD_ATTR               15 (orm)
-               112 LOAD_ATTR               16 (Query)
-   
-    86         122 BUILD_TUPLE              6
-               124 LOAD_CONST              12 (<code object add_participants_to_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 86>)
-               126 MAKE_FUNCTION            5 (defaults, annotations)
-               128 STORE_NAME              17 (add_participants_to_export)
-   
-   124         130 NOP
-   
-   121         132 LOAD_CONST              17 ((True,))
-               134 LOAD_CONST               9 ('column_list')
-               136 LOAD_NAME               13 (list)
-               138 LOAD_NAME               14 (str)
-               140 BINARY_SUBSCR
-               150 LOAD_CONST              10 ('export_data')
-   
-   122         152 LOAD_NAME               11 (dict)
-   
-   121         154 LOAD_CONST              13 ('query_participants')
-   
-   123         156 LOAD_NAME                4 (sqlalchemy)
-               158 LOAD_ATTR               15 (orm)
-               168 LOAD_ATTR               16 (Query)
-   
-   121         178 LOAD_CONST              11 ('return')
-   
-   124         180 LOAD_CONST               2 (None)
-   
-   121         182 BUILD_TUPLE              8
-               184 LOAD_CONST              14 (<code object add_questionnaires_to_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 121>)
-               186 MAKE_FUNCTION            5 (defaults, annotations)
-               188 STORE_NAME              18 (add_questionnaires_to_export)
-   
-   191         190 NOP
-   
-   188         192 LOAD_CONST              17 ((True,))
-               194 LOAD_CONST               9 ('column_list')
-               196 LOAD_NAME               13 (list)
-               198 LOAD_NAME               14 (str)
-               200 BINARY_SUBSCR
-               210 LOAD_CONST              10 ('export_data')
-   
-   189         212 LOAD_NAME               11 (dict)
-   
-   188         214 LOAD_CONST              13 ('query_participants')
-   
-   190         216 LOAD_NAME                4 (sqlalchemy)
-               218 LOAD_ATTR               15 (orm)
-               228 LOAD_ATTR               16 (Query)
-   
-   188         238 LOAD_CONST              11 ('return')
-   
-   191         240 LOAD_CONST               2 (None)
-   
-   188         242 BUILD_TUPLE              8
-               244 LOAD_CONST              15 (<code object add_custom_exports_to_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 188>)
-               246 MAKE_FUNCTION            5 (defaults, annotations)
-               248 STORE_NAME              19 (add_custom_exports_to_export)
-   
-   235         250 LOAD_CONST               9 ('column_list')
-               252 LOAD_NAME               13 (list)
-               254 LOAD_NAME               14 (str)
-               256 BINARY_SUBSCR
-               266 LOAD_CONST              10 ('export_data')
-               268 LOAD_NAME               11 (dict)
-               270 LOAD_CONST              11 ('return')
-               272 LOAD_NAME               14 (str)
-               274 BUILD_TUPLE              6
-               276 LOAD_CONST              16 (<code object build_export_csv, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 235>)
-               278 MAKE_FUNCTION            4 (annotations)
-               280 STORE_NAME              20 (build_export_csv)
-               282 LOAD_CONST               2 (None)
-               284 RETURN_VALUE
+    89          76 NOP
+   
+    86          78 LOAD_CONST              17 ((True, True))
+                80 LOAD_CONST               9 ('column_list')
+                82 LOAD_NAME               13 (list)
+                84 LOAD_NAME               14 (str)
+                86 BINARY_SUBSCR
+                96 LOAD_CONST              10 ('export_data')
+   
+    87          98 LOAD_NAME               11 (dict)
+   
+    86         100 LOAD_CONST              11 ('return')
+   
+    89         102 LOAD_NAME                4 (sqlalchemy)
+               104 LOAD_ATTR               15 (orm)
+               114 LOAD_ATTR               16 (Query)
+   
+    86         124 BUILD_TUPLE              6
+               126 LOAD_CONST              12 (<code object add_participants_to_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 86>)
+               128 MAKE_FUNCTION            5 (defaults, annotations)
+               130 STORE_NAME              17 (add_participants_to_export)
+   
+   128         132 NOP
+   
+   125         134 LOAD_CONST              18 ((True,))
+               136 LOAD_CONST               9 ('column_list')
+               138 LOAD_NAME               13 (list)
+               140 LOAD_NAME               14 (str)
+               142 BINARY_SUBSCR
+               152 LOAD_CONST              10 ('export_data')
+   
+   126         154 LOAD_NAME               11 (dict)
+   
+   125         156 LOAD_CONST              13 ('query_participants')
+   
+   127         158 LOAD_NAME                4 (sqlalchemy)
+               160 LOAD_ATTR               15 (orm)
+               170 LOAD_ATTR               16 (Query)
+   
+   125         180 LOAD_CONST              11 ('return')
+   
+   128         182 LOAD_CONST               2 (None)
+   
+   125         184 BUILD_TUPLE              8
+               186 LOAD_CONST              14 (<code object add_questionnaires_to_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 125>)
+               188 MAKE_FUNCTION            5 (defaults, annotations)
+               190 STORE_NAME              18 (add_questionnaires_to_export)
+   
+   195         192 NOP
+   
+   192         194 LOAD_CONST              18 ((True,))
+               196 LOAD_CONST               9 ('column_list')
+               198 LOAD_NAME               13 (list)
+               200 LOAD_NAME               14 (str)
+               202 BINARY_SUBSCR
+               212 LOAD_CONST              10 ('export_data')
+   
+   193         214 LOAD_NAME               11 (dict)
+   
+   192         216 LOAD_CONST              13 ('query_participants')
+   
+   194         218 LOAD_NAME                4 (sqlalchemy)
+               220 LOAD_ATTR               15 (orm)
+               230 LOAD_ATTR               16 (Query)
+   
+   192         240 LOAD_CONST              11 ('return')
+   
+   195         242 LOAD_CONST               2 (None)
+   
+   192         244 BUILD_TUPLE              8
+               246 LOAD_CONST              15 (<code object add_custom_exports_to_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 192>)
+               248 MAKE_FUNCTION            5 (defaults, annotations)
+               250 STORE_NAME              19 (add_custom_exports_to_export)
+   
+   239         252 LOAD_CONST               9 ('column_list')
+               254 LOAD_NAME               13 (list)
+               256 LOAD_NAME               14 (str)
+               258 BINARY_SUBSCR
+               268 LOAD_CONST              10 ('export_data')
+               270 LOAD_NAME               11 (dict)
+               272 LOAD_CONST              11 ('return')
+               274 LOAD_NAME               14 (str)
+               276 BUILD_TUPLE              6
+               278 LOAD_CONST              16 (<code object build_export_csv, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 239>)
+               280 MAKE_FUNCTION            4 (annotations)
+               282 STORE_NAME              20 (build_export_csv)
+               284 LOAD_CONST               2 (None)
+               286 RETURN_VALUE
    consts
       0
       ('db', 'questionnaires', 'page_list')
       None
       1
       ('escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label')
       ('current_app',)
@@ -612,117 +614,149 @@
             0228033e0204012a0108014aff0203480204012c02460204012a0204012a
             0314015a0102012a018e02
       True
       'column_list'
       'export_data'
       'return'
       code
-         argcount  : 3
-         nlocals   : 6
+         argcount  : 4
+         nlocals   : 7
          stacksize : 7
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007400000000000000000000006a
-            030000000000000000a6010000ab0100000000000000007d037c0273287c
-            03a004000000000000000000000000000000000000000074000000000000
+            030000000000000000a6010000ab0100000000000000007d047c0273287c
+            04a004000000000000000000000000000000000000000074000000000000
             00000000006a0300000000000000006a05000000000000000064016b0200
-            000000a6010000ab0100000000000000007d037c00a00600000000000000
-            0000000000000000000000000067006402a201a6010000ab010000000000
-            00000001007c03a0070000000000000000000000000000000000000000a6
-            000000ab0000000000000000007d047c0444005d387d057c056a08000000
-            00000000007c056a0900000000000000007415000000000000000000007c
-            056a0b0000000000000000a6010000ab0100000000000000007c056a0c00
-            000000000000007c056a05000000000000000064029c057c017c056a0800
-            000000000000003c0000008c397c035300
+            000000a6010000ab0100000000000000007d047c03734e7c04a004000000
+            00000000000000000000000000000000007401000000000000000000006a
+            0600000000000000007400000000000000000000006a0300000000000000
+            006a07000000000000000064026b02000000007400000000000000000000
+            006a0300000000000000006a07000000000000000064036b0200000000a6
+            020000ab020000000000000000a6010000ab0100000000000000007d047c
+            00a008000000000000000000000000000000000000000067006404a201a6
+            010000ab01000000000000000001007c04a0090000000000000000000000
+            000000000000000000a6000000ab0000000000000000007d057c0544005d
+            387d067c066a0a00000000000000007c066a0b0000000000000000741900
+            0000000000000000007c066a0d0000000000000000a6010000ab01000000
+            00000000007c066a0e00000000000000007c066a05000000000000000064
+            049c057c017c066a0a00000000000000003c0000008c397c045300
           86           0 RESUME                   0
          
-          95           2 LOAD_GLOBAL              0 (db)
+          96           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_ATTR                1 (session)
                       24 LOAD_METHOD              2 (query)
                       46 LOAD_GLOBAL              0 (db)
                       58 LOAD_ATTR                3 (Participant)
                       68 PRECALL                  1
                       72 CALL                     1
-                      82 STORE_FAST               3 (query_participants)
+                      82 STORE_FAST               4 (query_participants)
          
-          96          84 LOAD_FAST                2 (include_unfinished)
+          97          84 LOAD_FAST                2 (include_unfinished)
                       86 POP_JUMP_FORWARD_IF_TRUE    40 (to 168)
          
-          97          88 LOAD_FAST                3 (query_participants)
+          98          88 LOAD_FAST                4 (query_participants)
                       90 LOAD_METHOD              4 (filter)
                      112 LOAD_GLOBAL              0 (db)
                      124 LOAD_ATTR                3 (Participant)
                      134 LOAD_ATTR                5 (finished)
                      144 LOAD_CONST               1 (True)
                      146 COMPARE_OP               2 (==)
                      152 PRECALL                  1
                      156 CALL                     1
-                     166 STORE_FAST               3 (query_participants)
+                     166 STORE_FAST               4 (query_participants)
          
-          99     >>  168 LOAD_FAST                0 (column_list)
-                     170 LOAD_METHOD              6 (extend)
-                     192 BUILD_LIST               0
-                     194 LOAD_CONST               2 (('participantID', 'externalID', 'condition', 'duration', 'finished'))
-                     196 LIST_EXTEND              1
-                     198 PRECALL                  1
-                     202 CALL                     1
-                     212 POP_TOP
-         
-         107         214 LOAD_FAST                3 (query_participants)
-                     216 LOAD_METHOD              7 (all)
-                     238 PRECALL                  0
-                     242 CALL                     0
-                     252 STORE_FAST               4 (query_result)
-         
-         109         254 LOAD_FAST                4 (query_result)
-                     256 GET_ITER
-                 >>  258 FOR_ITER                56 (to 372)
-                     260 STORE_FAST               5 (row)
-         
-         111         262 LOAD_FAST                5 (row)
-                     264 LOAD_ATTR                8 (participantID)
-         
-         112         274 LOAD_FAST                5 (row)
-                     276 LOAD_ATTR                9 (mTurkID)
-         
-         113         286 LOAD_GLOBAL             21 (NULL + condition_num_to_label)
-                     298 LOAD_FAST                5 (row)
-                     300 LOAD_ATTR               11 (condition)
-                     310 PRECALL                  1
-                     314 CALL                     1
-         
-         114         324 LOAD_FAST                5 (row)
-                     326 LOAD_ATTR               12 (duration)
-         
-         115         336 LOAD_FAST                5 (row)
-                     338 LOAD_ATTR                5 (finished)
-         
-         110         348 LOAD_CONST               2 (('participantID', 'externalID', 'condition', 'duration', 'finished'))
-                     350 BUILD_CONST_KEY_MAP      5
-                     352 LOAD_FAST                1 (export_data)
-                     354 LOAD_FAST                5 (row)
-                     356 LOAD_ATTR                8 (participantID)
-                     366 STORE_SUBSCR
-                     370 JUMP_BACKWARD           57 (to 258)
+         100     >>  168 LOAD_FAST                3 (include_exluded)
+                     170 POP_JUMP_FORWARD_IF_TRUE    78 (to 328)
          
-         118     >>  372 LOAD_FAST                3 (query_participants)
-                     374 RETURN_VALUE
+         101         172 LOAD_FAST                4 (query_participants)
+                     174 LOAD_METHOD              4 (filter)
+                     196 LOAD_GLOBAL              1 (NULL + db)
+                     208 LOAD_ATTR                6 (or_)
+                     218 LOAD_GLOBAL              0 (db)
+                     230 LOAD_ATTR                3 (Participant)
+                     240 LOAD_ATTR                7 (excludeFromCount)
+                     250 LOAD_CONST               2 (False)
+                     252 COMPARE_OP               2 (==)
+                     258 LOAD_GLOBAL              0 (db)
+                     270 LOAD_ATTR                3 (Participant)
+                     280 LOAD_ATTR                7 (excludeFromCount)
+                     290 LOAD_CONST               3 (None)
+                     292 COMPARE_OP               2 (==)
+                     298 PRECALL                  2
+                     302 CALL                     2
+                     312 PRECALL                  1
+                     316 CALL                     1
+                     326 STORE_FAST               4 (query_participants)
+         
+         103     >>  328 LOAD_FAST                0 (column_list)
+                     330 LOAD_METHOD              8 (extend)
+                     352 BUILD_LIST               0
+                     354 LOAD_CONST               4 (('participantID', 'externalID', 'condition', 'duration', 'finished'))
+                     356 LIST_EXTEND              1
+                     358 PRECALL                  1
+                     362 CALL                     1
+                     372 POP_TOP
+         
+         111         374 LOAD_FAST                4 (query_participants)
+                     376 LOAD_METHOD              9 (all)
+                     398 PRECALL                  0
+                     402 CALL                     0
+                     412 STORE_FAST               5 (query_result)
+         
+         113         414 LOAD_FAST                5 (query_result)
+                     416 GET_ITER
+                 >>  418 FOR_ITER                56 (to 532)
+                     420 STORE_FAST               6 (row)
+         
+         115         422 LOAD_FAST                6 (row)
+                     424 LOAD_ATTR               10 (participantID)
+         
+         116         434 LOAD_FAST                6 (row)
+                     436 LOAD_ATTR               11 (mTurkID)
+         
+         117         446 LOAD_GLOBAL             25 (NULL + condition_num_to_label)
+                     458 LOAD_FAST                6 (row)
+                     460 LOAD_ATTR               13 (condition)
+                     470 PRECALL                  1
+                     474 CALL                     1
+         
+         118         484 LOAD_FAST                6 (row)
+                     486 LOAD_ATTR               14 (duration)
+         
+         119         496 LOAD_FAST                6 (row)
+                     498 LOAD_ATTR                5 (finished)
+         
+         114         508 LOAD_CONST               4 (('participantID', 'externalID', 'condition', 'duration', 'finished'))
+                     510 BUILD_CONST_KEY_MAP      5
+                     512 LOAD_FAST                1 (export_data)
+                     514 LOAD_FAST                6 (row)
+                     516 LOAD_ATTR               10 (participantID)
+                     526 STORE_SUBSCR
+                     530 JUMP_BACKWARD           57 (to 418)
+         
+         122     >>  532 LOAD_FAST                4 (query_participants)
+                     534 RETURN_VALUE
          consts
             '\n    Add participant columns to column_list and their data to export_data.\n    :param column_list: A list of strings that will be the columns in the CSV export.\n    :param export_data: Gets updated with data for the participants\n    :return: A SQLAlchemy query.\n    '
             True
+            False
+            None
             ('participantID', 'externalID', 'condition', 'duration', 'finished')
-         names      ('db', 'session', 'query', 'Participant', 'filter', 'finished', 'extend', 'all', 'participantID', 'mTurkID', 'condition_num_to_label', 'condition', 'duration')
-         varnames   ('column_list', 'export_data', 'include_unfinished', 'query_participants', 'query_result', 'row')
+         names      ('db', 'session', 'query', 'Participant', 'filter', 'finished', 'or_', 'excludeFromCount', 'extend', 'all', 'participantID', 'mTurkID', 'condition_num_to_label', 'condition', 'duration')
+         varnames   ('column_list', 'export_data', 'include_unfinished', 'include_exluded', 'query_participants', 'query_result', 'row')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\export_helpers.py'
          name       'add_participants_to_export'
          firstlineno 86
-         lnotab 0x02095201040150022e08280208020c010c0126010c010cfb1808
+         lnotab
+            0x020a52010401500204019c022e08280208020c010c0126010c010cfb18
+            08
       'query_participants'
       code
          argcount  : 4
          nlocals   : 19
          stacksize : 8
          flags     : 3
          code
@@ -763,223 +797,223 @@
             005d357d127c11723102007427000000000000000000007c117c12a60200
             00ab020000000000000000a6000000ab0000000000000000007c017c106a
             0900000000000000006a080000000000000000190000000000000000007c
             0864047a0000007c127a0000003c0000008c367c11a01400000000000000
             00000000000000000000000000a6000000ab0000000000000000007c017c
             106a0900000000000000006a080000000000000000190000000000000000
             007c0864057a0000003c0000008cb18cb664005300
-         121           0 RESUME                   0
+         125           0 RESUME                   0
          
-         125           2 LOAD_GLOBAL              1 (NULL + page_list)
+         129           2 LOAD_GLOBAL              1 (NULL + page_list)
                       14 LOAD_ATTR                1 (get_questionnaire_list)
                       24 LOAD_CONST               1 (True)
                       26 KW_NAMES                 2
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_FAST               4 (list_of_questionnaires)
          
-         127          44 LOAD_FAST                2 (query_participants)
+         131          44 LOAD_FAST                2 (query_participants)
                       46 STORE_FAST               5 (query_questionnaires)
          
-         128          48 BUILD_MAP                0
+         132          48 BUILD_MAP                0
                       50 STORE_FAST               6 (columns)
          
-         129          52 BUILD_MAP                0
+         133          52 BUILD_MAP                0
                       54 STORE_FAST               7 (calculated_columns)
          
-         132          56 LOAD_FAST                4 (list_of_questionnaires)
+         136          56 LOAD_FAST                4 (list_of_questionnaires)
                       58 GET_ITER
                  >>   60 EXTENDED_ARG             1
                       62 FOR_ITER               372 (to 808)
                       64 STORE_FAST               8 (entry)
          
-         133          66 BUILD_LIST               0
+         137          66 BUILD_LIST               0
                       68 LOAD_FAST                6 (columns)
                       70 LOAD_FAST                8 (entry)
                       72 STORE_SUBSCR
          
-         134          76 BUILD_LIST               0
+         138          76 BUILD_LIST               0
                       78 LOAD_FAST                7 (calculated_columns)
                       80 LOAD_FAST                8 (entry)
                       82 STORE_SUBSCR
          
-         135          86 LOAD_GLOBAL              5 (NULL + questionnaire_name_and_tag)
+         139          86 LOAD_GLOBAL              5 (NULL + questionnaire_name_and_tag)
                       98 LOAD_FAST                8 (entry)
                      100 PRECALL                  1
                      104 CALL                     1
                      114 UNPACK_SEQUENCE          2
                      118 STORE_FAST               9 (questionnaire_name)
                      120 STORE_FAST              10 (questionnaire_tag)
          
-         138         122 LOAD_GLOBAL              6 (questionnaires)
+         142         122 LOAD_GLOBAL              6 (questionnaires)
                      134 LOAD_FAST                9 (questionnaire_name)
                      136 BINARY_SUBSCR
                      146 STORE_FAST              11 (questionnaire)
          
-         141         148 LOAD_GLOBAL              9 (NULL + db)
+         145         148 LOAD_GLOBAL              9 (NULL + db)
                      160 LOAD_ATTR                5 (aliased)
                      170 LOAD_FAST               11 (questionnaire)
                      172 LOAD_ATTR                6 (db_class)
                      182 LOAD_FAST                8 (entry)
                      184 KW_NAMES                 3
                      186 PRECALL                  2
                      190 CALL                     2
                      200 STORE_FAST              12 (questionnaire_db_class)
          
-         142         202 LOAD_GLOBAL              9 (NULL + db)
+         146         202 LOAD_GLOBAL              9 (NULL + db)
                      214 LOAD_ATTR                7 (and_)
                      224 LOAD_FAST               12 (questionnaire_db_class)
                      226 LOAD_ATTR                8 (participantID)
                      236 LOAD_GLOBAL              8 (db)
                      248 LOAD_ATTR                9 (Participant)
                      258 LOAD_ATTR                8 (participantID)
                      268 COMPARE_OP               2 (==)
          
-         143         274 LOAD_FAST               12 (questionnaire_db_class)
+         147         274 LOAD_FAST               12 (questionnaire_db_class)
                      276 LOAD_ATTR               10 (tag)
                      286 LOAD_FAST               10 (questionnaire_tag)
                      288 COMPARE_OP               2 (==)
          
-         142         294 PRECALL                  2
+         146         294 PRECALL                  2
                      298 CALL                     2
                      308 STORE_FAST              13 (join_condition)
          
-         146         310 LOAD_FAST                3 (include_missing)
+         150         310 LOAD_FAST                3 (include_missing)
                      312 POP_JUMP_FORWARD_IF_FALSE    42 (to 398)
          
-         147         314 LOAD_FAST                5 (query_questionnaires)
+         151         314 LOAD_FAST                5 (query_questionnaires)
                      316 LOAD_METHOD             11 (outerjoin)
                      338 LOAD_FAST               12 (questionnaire_db_class)
                      340 LOAD_FAST               13 (join_condition)
                      342 PRECALL                  2
                      346 CALL                     2
          
-         148         356 LOAD_METHOD             12 (add_entity)
+         152         356 LOAD_METHOD             12 (add_entity)
                      378 LOAD_FAST               12 (questionnaire_db_class)
                      380 PRECALL                  1
                      384 CALL                     1
          
-         147         394 STORE_FAST               5 (query_questionnaires)
+         151         394 STORE_FAST               5 (query_questionnaires)
                      396 JUMP_FORWARD            41 (to 480)
          
-         150     >>  398 LOAD_FAST                5 (query_questionnaires)
+         154     >>  398 LOAD_FAST                5 (query_questionnaires)
                      400 LOAD_METHOD             13 (join)
                      422 LOAD_FAST               12 (questionnaire_db_class)
                      424 LOAD_FAST               13 (join_condition)
                      426 PRECALL                  2
                      430 CALL                     2
          
-         151         440 LOAD_METHOD             12 (add_entity)
+         155         440 LOAD_METHOD             12 (add_entity)
                      462 LOAD_FAST               12 (questionnaire_db_class)
                      464 PRECALL                  1
                      468 CALL                     1
          
-         150         478 STORE_FAST               5 (query_questionnaires)
+         154         478 STORE_FAST               5 (query_questionnaires)
          
-         155     >>  480 LOAD_FAST               11 (questionnaire)
+         159     >>  480 LOAD_FAST               11 (questionnaire)
                      482 LOAD_ATTR               14 (fields)
                      492 GET_ITER
                  >>  494 FOR_ITER                66 (to 628)
                      496 STORE_FAST              14 (column)
          
-         156         498 LOAD_FAST                0 (column_list)
+         160         498 LOAD_FAST                0 (column_list)
                      500 LOAD_METHOD             15 (append)
                      522 LOAD_FAST                8 (entry)
                      524 LOAD_CONST               4 ('_')
                      526 BINARY_OP                0 (+)
                      530 LOAD_FAST               14 (column)
                      532 LOAD_ATTR               16 (id)
                      542 BINARY_OP                0 (+)
                      546 PRECALL                  1
                      550 CALL                     1
                      560 POP_TOP
          
-         157         562 LOAD_FAST                6 (columns)
+         161         562 LOAD_FAST                6 (columns)
                      564 LOAD_FAST                8 (entry)
                      566 BINARY_SUBSCR
                      576 LOAD_METHOD             15 (append)
                      598 LOAD_FAST               14 (column)
                      600 LOAD_ATTR               16 (id)
                      610 PRECALL                  1
                      614 CALL                     1
                      624 POP_TOP
                      626 JUMP_BACKWARD           67 (to 494)
          
-         160     >>  628 LOAD_FAST               11 (questionnaire)
+         164     >>  628 LOAD_FAST               11 (questionnaire)
                      630 LOAD_ATTR               17 (calc_fields)
                      640 GET_ITER
                  >>  642 FOR_ITER                56 (to 756)
                      644 STORE_FAST              14 (column)
          
-         161         646 LOAD_FAST                0 (column_list)
+         165         646 LOAD_FAST                0 (column_list)
                      648 LOAD_METHOD             15 (append)
                      670 LOAD_FAST                8 (entry)
                      672 LOAD_CONST               4 ('_')
                      674 BINARY_OP                0 (+)
                      678 LOAD_FAST               14 (column)
                      680 BINARY_OP                0 (+)
                      684 PRECALL                  1
                      688 CALL                     1
                      698 POP_TOP
          
-         162         700 LOAD_FAST                7 (calculated_columns)
+         166         700 LOAD_FAST                7 (calculated_columns)
                      702 LOAD_FAST                8 (entry)
                      704 BINARY_SUBSCR
                      714 LOAD_METHOD             15 (append)
                      736 LOAD_FAST               14 (column)
                      738 PRECALL                  1
                      742 CALL                     1
                      752 POP_TOP
                      754 JUMP_BACKWARD           57 (to 642)
          
-         165     >>  756 LOAD_FAST                0 (column_list)
+         169     >>  756 LOAD_FAST                0 (column_list)
                      758 LOAD_METHOD             15 (append)
                      780 LOAD_FAST                8 (entry)
                      782 LOAD_CONST               5 ('_duration')
                      784 BINARY_OP                0 (+)
                      788 PRECALL                  1
                      792 CALL                     1
                      802 POP_TOP
                      804 EXTENDED_ARG             1
                      806 JUMP_BACKWARD          374 (to 60)
          
-         167     >>  808 LOAD_FAST                5 (query_questionnaires)
+         171     >>  808 LOAD_FAST                5 (query_questionnaires)
                      810 LOAD_METHOD             18 (all)
                      832 PRECALL                  0
                      836 CALL                     0
                      846 STORE_FAST              15 (query_result)
          
-         170         848 LOAD_FAST               15 (query_result)
+         174         848 LOAD_FAST               15 (query_result)
                      850 GET_ITER
                  >>  852 FOR_ITER               181 (to 1216)
                      854 STORE_FAST              16 (row)
          
-         171         856 LOAD_FAST                4 (list_of_questionnaires)
+         175         856 LOAD_FAST                4 (list_of_questionnaires)
                      858 GET_ITER
                  >>  860 FOR_ITER               176 (to 1214)
                      862 STORE_FAST               8 (entry)
          
-         172         864 LOAD_GLOBAL             39 (NULL + getattr)
+         176         864 LOAD_GLOBAL             39 (NULL + getattr)
                      876 LOAD_FAST               16 (row)
                      878 LOAD_FAST                8 (entry)
                      880 PRECALL                  2
                      884 CALL                     2
                      894 STORE_FAST              17 (questionnaire_data)
          
-         174         896 LOAD_FAST               17 (questionnaire_data)
+         178         896 LOAD_FAST               17 (questionnaire_data)
                      898 POP_JUMP_FORWARD_IF_FALSE   156 (to 1212)
          
-         176         900 LOAD_FAST                6 (columns)
+         180         900 LOAD_FAST                6 (columns)
                      902 LOAD_FAST                8 (entry)
                      904 BINARY_SUBSCR
                      914 GET_ITER
                  >>  916 FOR_ITER                43 (to 1004)
                      918 STORE_FAST              18 (col)
          
-         177         920 LOAD_GLOBAL             39 (NULL + getattr)
+         181         920 LOAD_GLOBAL             39 (NULL + getattr)
                      932 LOAD_FAST               17 (questionnaire_data)
                      934 LOAD_FAST               18 (col)
                      936 PRECALL                  2
                      940 CALL                     2
                      950 LOAD_FAST                1 (export_data)
                      952 LOAD_FAST               16 (row)
                      954 LOAD_ATTR                9 (Participant)
@@ -989,25 +1023,25 @@
                      986 LOAD_CONST               4 ('_')
                      988 BINARY_OP                0 (+)
                      992 LOAD_FAST               18 (col)
                      994 BINARY_OP                0 (+)
                      998 STORE_SUBSCR
                     1002 JUMP_BACKWARD           44 (to 916)
          
-         180     >> 1004 LOAD_FAST                7 (calculated_columns)
+         184     >> 1004 LOAD_FAST                7 (calculated_columns)
                     1006 LOAD_FAST                8 (entry)
                     1008 BINARY_SUBSCR
                     1018 GET_ITER
                  >> 1020 FOR_ITER                53 (to 1128)
                     1022 STORE_FAST              18 (col)
          
-         181        1024 LOAD_FAST               17 (questionnaire_data)
+         185        1024 LOAD_FAST               17 (questionnaire_data)
                     1026 POP_JUMP_FORWARD_IF_FALSE    49 (to 1126)
          
-         182        1028 PUSH_NULL
+         186        1028 PUSH_NULL
                     1030 LOAD_GLOBAL             39 (NULL + getattr)
                     1042 LOAD_FAST               17 (questionnaire_data)
                     1044 LOAD_FAST               18 (col)
                     1046 PRECALL                  2
                     1050 CALL                     2
                     1060 PRECALL                  0
                     1064 CALL                     0
@@ -1020,47 +1054,47 @@
                     1110 LOAD_CONST               4 ('_')
                     1112 BINARY_OP                0 (+)
                     1116 LOAD_FAST               18 (col)
                     1118 BINARY_OP                0 (+)
                     1122 STORE_SUBSCR
                  >> 1126 JUMP_BACKWARD           54 (to 1020)
          
-         185     >> 1128 LOAD_FAST               17 (questionnaire_data)
+         189     >> 1128 LOAD_FAST               17 (questionnaire_data)
                     1130 LOAD_METHOD             20 (duration)
                     1152 PRECALL                  0
                     1156 CALL                     0
                     1166 LOAD_FAST                1 (export_data)
                     1168 LOAD_FAST               16 (row)
                     1170 LOAD_ATTR                9 (Participant)
                     1180 LOAD_ATTR                8 (participantID)
                     1190 BINARY_SUBSCR
                     1200 LOAD_FAST                8 (entry)
                     1202 LOAD_CONST               5 ('_duration')
                     1204 BINARY_OP                0 (+)
                     1208 STORE_SUBSCR
                  >> 1212 JUMP_BACKWARD          177 (to 860)
          
-         171     >> 1214 JUMP_BACKWARD          182 (to 852)
+         175     >> 1214 JUMP_BACKWARD          182 (to 852)
          
-         170     >> 1216 LOAD_CONST               0 (None)
+         174     >> 1216 LOAD_CONST               0 (None)
                     1218 RETURN_VALUE
          consts
             None
             True
             ('include_tags',)
             ('name',)
             '_'
             '_duration'
          names      ('page_list', 'get_questionnaire_list', 'questionnaire_name_and_tag', 'questionnaires', 'db', 'aliased', 'db_class', 'and_', 'participantID', 'Participant', 'tag', 'outerjoin', 'add_entity', 'join', 'fields', 'append', 'id', 'calc_fields', 'all', 'getattr', 'duration')
          varnames   ('column_list', 'export_data', 'query_participants', 'include_missing', 'list_of_questionnaires', 'query_questionnaires', 'columns', 'calculated_columns', 'entry', 'questionnaire_name', 'questionnaire_tag', 'questionnaire', 'questionnaire_db_class', 'join_condition', 'column', 'query_result', 'row', 'questionnaire_data', 'col')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\export_helpers.py'
          name       'add_questionnaires_to_export'
-         firstlineno 121
+         firstlineno 125
          lnotab
             0x02042a020401040104030a010a010a0124031a033601480114ff100404
             012a0126ff04032a0126ff02051201400142031201360138033402280308
             010801200204021401540314010401640356f202ff
       code
          argcount  : 4
          nlocals   : 21
@@ -1097,89 +1131,89 @@
             005d5c7d137c0564051900000000000000000044005d4c7d0a7c0a7d147c
             0564031900000000000000000072277c0a64097a00000074090000000000
             00000000007c056403190000000000000000007c12190000000000000000
             00640c19000000000000000000a6010000ab0100000000000000007a0000
             007d147419000000000000000000007c137c0aa6020000ab020000000000
             0000007c017c0f190000000000000000007c143c0000008c4d7c12640d7a
             0d00007d128c5d8cb08cbc64005300
-         188           0 RESUME                   0
+         192           0 RESUME                   0
          
-         193           2 BUILD_LIST               0
+         197           2 BUILD_LIST               0
                        4 STORE_FAST               4 (custom_exports)
          
-         195           6 LOAD_GLOBAL              0 (current_app)
+         199           6 LOAD_GLOBAL              0 (current_app)
                       18 LOAD_ATTR                1 (config)
                       28 LOAD_CONST               1 ('EXPORT')
                       30 BINARY_SUBSCR
                       40 GET_ITER
                  >>   42 FOR_ITER                47 (to 138)
                       44 STORE_FAST               5 (export)
          
-         196          46 LOAD_GLOBAL              5 (NULL + create_export_base_query)
+         200          46 LOAD_GLOBAL              5 (NULL + create_export_base_query)
                       58 LOAD_FAST                5 (export)
                       60 PRECALL                  1
                       64 CALL                     1
                       74 UNPACK_SEQUENCE          3
                       78 STORE_FAST               6 (levels)
                       80 STORE_FAST               7 (fields)
                       82 STORE_FAST               8 (base_query)
          
-         197          84 LOAD_FAST                4 (custom_exports)
+         201          84 LOAD_FAST                4 (custom_exports)
                       86 LOAD_METHOD              3 (append)
                      108 LOAD_FAST                5 (export)
                      110 LOAD_FAST                7 (fields)
                      112 LOAD_FAST                8 (base_query)
                      114 LOAD_FAST                6 (levels)
                      116 LOAD_CONST               2 (('options', 'fields', 'base_query', 'levels'))
                      118 BUILD_CONST_KEY_MAP      4
                      120 PRECALL                  1
                      124 CALL                     1
                      134 POP_TOP
                      136 JUMP_BACKWARD           48 (to 42)
          
-         200     >>  138 LOAD_FAST                4 (custom_exports)
+         204     >>  138 LOAD_FAST                4 (custom_exports)
                      140 GET_ITER
                  >>  142 FOR_ITER               218 (to 580)
                      144 STORE_FAST               5 (export)
          
-         201         146 LOAD_FAST                5 (export)
+         205         146 LOAD_FAST                5 (export)
                      148 LOAD_CONST               3 ('levels')
                      150 BINARY_SUBSCR
                      160 POP_JUMP_FORWARD_IF_FALSE   145 (to 452)
          
-         202         162 LOAD_FAST                5 (export)
+         206         162 LOAD_FAST                5 (export)
                      164 LOAD_CONST               3 ('levels')
                      166 BINARY_SUBSCR
                      176 GET_ITER
                  >>  178 FOR_ITER               135 (to 450)
                      180 STORE_FAST               9 (level)
          
-         203         182 LOAD_FAST                5 (export)
+         207         182 LOAD_FAST                5 (export)
                      184 LOAD_CONST               4 ('options')
                      186 BINARY_SUBSCR
                      196 LOAD_CONST               5 ('fields')
                      198 BINARY_SUBSCR
                      208 GET_ITER
                  >>  210 FOR_ITER               118 (to 448)
                      212 STORE_FAST              10 (field)
          
-         204         214 LOAD_GLOBAL              8 (str)
+         208         214 LOAD_GLOBAL              8 (str)
                      226 LOAD_METHOD              5 (format)
                      248 LOAD_CONST               6 ('{}')
                      250 LOAD_FAST               10 (field)
                      252 PRECALL                  2
                      256 CALL                     2
                      266 STORE_FAST              11 (column_header)
          
-         205         268 LOAD_FAST                9 (level)
+         209         268 LOAD_FAST                9 (level)
                      270 GET_ITER
                  >>  272 FOR_ITER                65 (to 404)
                      274 STORE_FAST              12 (level_name)
          
-         206         276 LOAD_FAST               11 (column_header)
+         210         276 LOAD_FAST               11 (column_header)
                      278 LOAD_GLOBAL              8 (str)
                      290 LOAD_METHOD              5 (format)
                      312 LOAD_CONST               7 ('_{}')
                      314 LOAD_GLOBAL              9 (NULL + str)
                      326 LOAD_FAST               12 (level_name)
                      328 PRECALL                  1
                      332 CALL                     1
@@ -1190,119 +1224,119 @@
                      372 CALL                     2
                      382 PRECALL                  2
                      386 CALL                     2
                      396 BINARY_OP               13 (+=)
                      400 STORE_FAST              11 (column_header)
                      402 JUMP_BACKWARD           66 (to 272)
          
-         207     >>  404 LOAD_FAST                0 (column_list)
+         211     >>  404 LOAD_FAST                0 (column_list)
                      406 LOAD_METHOD              3 (append)
                      428 LOAD_FAST               11 (column_header)
                      430 PRECALL                  1
                      434 CALL                     1
                      444 POP_TOP
                      446 JUMP_BACKWARD          119 (to 210)
          
-         203     >>  448 JUMP_BACKWARD          136 (to 178)
+         207     >>  448 JUMP_BACKWARD          136 (to 178)
          
-         202     >>  450 JUMP_BACKWARD          155 (to 142)
+         206     >>  450 JUMP_BACKWARD          155 (to 142)
          
-         209     >>  452 LOAD_FAST                5 (export)
+         213     >>  452 LOAD_FAST                5 (export)
                      454 LOAD_CONST               4 ('options')
                      456 BINARY_SUBSCR
                      466 LOAD_CONST               5 ('fields')
                      468 BINARY_SUBSCR
                      478 GET_ITER
                  >>  480 FOR_ITER                48 (to 578)
                      482 STORE_FAST              10 (field)
          
-         210         484 LOAD_FAST                0 (column_list)
+         214         484 LOAD_FAST                0 (column_list)
                      486 LOAD_METHOD              3 (append)
                      508 LOAD_GLOBAL              8 (str)
                      520 LOAD_METHOD              5 (format)
                      542 LOAD_CONST               6 ('{}')
                      544 LOAD_FAST               10 (field)
                      546 PRECALL                  2
                      550 CALL                     2
                      560 PRECALL                  1
                      564 CALL                     1
                      574 POP_TOP
                      576 JUMP_BACKWARD           49 (to 480)
          
-         209     >>  578 JUMP_BACKWARD          219 (to 142)
+         213     >>  578 JUMP_BACKWARD          219 (to 142)
          
-         212     >>  580 LOAD_FAST                2 (query_participants)
+         216     >>  580 LOAD_FAST                2 (query_participants)
                      582 LOAD_METHOD              7 (all)
                      604 PRECALL                  0
                      608 CALL                     0
                      618 STORE_FAST              13 (query_result)
          
-         215         620 LOAD_FAST               13 (query_result)
+         219         620 LOAD_FAST               13 (query_result)
                      622 GET_ITER
                  >>  624 FOR_ITER               187 (to 1000)
                      626 STORE_FAST              14 (row)
          
-         216         628 LOAD_FAST               14 (row)
+         220         628 LOAD_FAST               14 (row)
                      630 LOAD_ATTR                8 (participantID)
                      640 STORE_FAST              15 (participant_id)
          
-         218         642 LOAD_FAST                4 (custom_exports)
+         222         642 LOAD_FAST                4 (custom_exports)
                      644 GET_ITER
                  >>  646 FOR_ITER               175 (to 998)
                      648 STORE_FAST               5 (export)
          
-         219         650 LOAD_FAST                5 (export)
+         223         650 LOAD_FAST                5 (export)
                      652 LOAD_CONST              10 ('base_query')
                      654 BINARY_SUBSCR
                      664 STORE_FAST              16 (query)
          
-         220         666 LOAD_FAST               16 (query)
+         224         666 LOAD_FAST               16 (query)
                      668 LOAD_METHOD              9 (filter)
                      690 LOAD_GLOBAL             21 (NULL + db)
                      702 LOAD_ATTR               11 (literal_column)
                      712 LOAD_CONST              11 ('participantID')
                      714 PRECALL                  1
                      718 CALL                     1
                      728 LOAD_FAST               14 (row)
                      730 LOAD_ATTR                8 (participantID)
                      740 COMPARE_OP               2 (==)
                      746 PRECALL                  1
                      750 CALL                     1
                      760 STORE_FAST              16 (query)
          
-         221         762 LOAD_FAST               16 (query)
+         225         762 LOAD_FAST               16 (query)
                      764 LOAD_METHOD              7 (all)
                      786 PRECALL                  0
                      790 CALL                     0
                      800 STORE_FAST              17 (custom_export_data)
          
-         223         802 LOAD_CONST              12 (0)
+         227         802 LOAD_CONST              12 (0)
                      804 STORE_FAST              18 (export_row_index)
          
-         224         806 LOAD_FAST               17 (custom_export_data)
+         228         806 LOAD_FAST               17 (custom_export_data)
                      808 GET_ITER
                  >>  810 FOR_ITER                92 (to 996)
                      812 STORE_FAST              19 (custom_export_row)
          
-         225         814 LOAD_FAST                5 (export)
+         229         814 LOAD_FAST                5 (export)
                      816 LOAD_CONST               5 ('fields')
                      818 BINARY_SUBSCR
                      828 GET_ITER
                  >>  830 FOR_ITER                76 (to 984)
                      832 STORE_FAST              10 (field)
          
-         226         834 LOAD_FAST               10 (field)
+         230         834 LOAD_FAST               10 (field)
                      836 STORE_FAST              20 (export_column_name)
          
-         227         838 LOAD_FAST                5 (export)
+         231         838 LOAD_FAST                5 (export)
                      840 LOAD_CONST               3 ('levels')
                      842 BINARY_SUBSCR
                      852 POP_JUMP_FORWARD_IF_FALSE    39 (to 932)
          
-         228         854 LOAD_FAST               10 (field)
+         232         854 LOAD_FAST               10 (field)
                      856 LOAD_CONST               9 ('_')
                      858 BINARY_OP                0 (+)
                      862 LOAD_GLOBAL              9 (NULL + str)
                      874 LOAD_FAST                5 (export)
                      876 LOAD_CONST               3 ('levels')
                      878 BINARY_SUBSCR
                      888 LOAD_FAST               18 (export_row_index)
@@ -1310,37 +1344,37 @@
                      900 LOAD_CONST              12 (0)
                      902 BINARY_SUBSCR
                      912 PRECALL                  1
                      916 CALL                     1
                      926 BINARY_OP                0 (+)
                      930 STORE_FAST              20 (export_column_name)
          
-         230     >>  932 LOAD_GLOBAL             25 (NULL + getattr)
+         234     >>  932 LOAD_GLOBAL             25 (NULL + getattr)
                      944 LOAD_FAST               19 (custom_export_row)
                      946 LOAD_FAST               10 (field)
                      948 PRECALL                  2
                      952 CALL                     2
                      962 LOAD_FAST                1 (export_data)
                      964 LOAD_FAST               15 (participant_id)
                      966 BINARY_SUBSCR
                      976 LOAD_FAST               20 (export_column_name)
                      978 STORE_SUBSCR
                      982 JUMP_BACKWARD           77 (to 830)
          
-         232     >>  984 LOAD_FAST               18 (export_row_index)
+         236     >>  984 LOAD_FAST               18 (export_row_index)
                      986 LOAD_CONST              13 (1)
                      988 BINARY_OP               13 (+=)
                      992 STORE_FAST              18 (export_row_index)
                      994 JUMP_BACKWARD           93 (to 810)
          
-         224     >>  996 JUMP_BACKWARD          176 (to 646)
+         228     >>  996 JUMP_BACKWARD          176 (to 646)
          
-         218     >>  998 JUMP_BACKWARD          188 (to 624)
+         222     >>  998 JUMP_BACKWARD          188 (to 624)
          
-         215     >> 1000 LOAD_CONST               0 (None)
+         219     >> 1000 LOAD_CONST               0 (None)
                     1002 RETURN_VALUE
          consts
             None
             'EXPORT'
             ('options', 'fields', 'base_query', 'levels')
             'levels'
             'options'
@@ -1355,15 +1389,15 @@
             1
          names      ('current_app', 'config', 'create_export_base_query', 'append', 'str', 'format', 'replace', 'all', 'participantID', 'filter', 'db', 'literal_column', 'getattr')
          varnames   ('column_list', 'export_data', 'query_participants', 'include_missing', 'custom_exports', 'export', 'levels', 'fields', 'base_query', 'level', 'field', 'column_header', 'level_name', 'query_result', 'row', 'participant_id', 'query', 'custom_export_data', 'export_row_index', 'custom_export_row', 'export_column_name')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\export_helpers.py'
          name       'add_custom_exports_to_export'
-         firstlineno 188
+         firstlineno 192
          lnotab
             0x0205040228012601360308011001140120013601080180012cfc02ff02
             0720015eff0203280308010e020801100160012802040108011401040110
             014e0234020cf802fa02fd
       code
          argcount  : 2
          nlocals   : 6
@@ -1374,78 +1408,78 @@
             010000ab01000000000000000064027a0000007d027c01a0010000000000
             000000000000000000000000000000a6000000ab00000000000000000044
             005d3e7d0364037d047c0044005d277d057c057c037600721c7c04740500
             0000000000000000007c037c0519000000000000000000a6010000ab0100
             0000000000000064017a0000007a0d00007d048c227c0464017a0d00007d
             048c287c027c046400640485021900000000000000000064027a0000007a
             0d00007d028c3f7c02640064048502190000000000000000005300
-         235           0 RESUME                   0
+         239           0 RESUME                   0
          
-         236           2 LOAD_CONST               1 (',')
+         240           2 LOAD_CONST               1 (',')
                        4 LOAD_METHOD              0 (join)
                       26 LOAD_FAST                0 (column_list)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 LOAD_CONST               2 ('\n')
                       44 BINARY_OP                0 (+)
                       48 STORE_FAST               2 (csv_string)
          
-         238          50 LOAD_FAST                1 (export_data)
+         242          50 LOAD_FAST                1 (export_data)
                       52 LOAD_METHOD              1 (values)
                       74 PRECALL                  0
                       78 CALL                     0
                       88 GET_ITER
                  >>   90 FOR_ITER                62 (to 216)
                       92 STORE_FAST               3 (row)
          
-         239          94 LOAD_CONST               3 ('')
+         243          94 LOAD_CONST               3 ('')
                       96 STORE_FAST               4 (csv_line)
          
-         240          98 LOAD_FAST                0 (column_list)
+         244          98 LOAD_FAST                0 (column_list)
                      100 GET_ITER
                  >>  102 FOR_ITER                39 (to 182)
                      104 STORE_FAST               5 (column)
          
-         241         106 LOAD_FAST                5 (column)
+         245         106 LOAD_FAST                5 (column)
                      108 LOAD_FAST                3 (row)
                      110 CONTAINS_OP              0
                      112 POP_JUMP_FORWARD_IF_FALSE    28 (to 170)
          
-         242         114 LOAD_FAST                4 (csv_line)
+         246         114 LOAD_FAST                4 (csv_line)
                      116 LOAD_GLOBAL              5 (NULL + escape_csv)
                      128 LOAD_FAST                3 (row)
                      130 LOAD_FAST                5 (column)
                      132 BINARY_SUBSCR
                      142 PRECALL                  1
                      146 CALL                     1
                      156 LOAD_CONST               1 (',')
                      158 BINARY_OP                0 (+)
                      162 BINARY_OP               13 (+=)
                      166 STORE_FAST               4 (csv_line)
                      168 JUMP_BACKWARD           34 (to 102)
          
-         244     >>  170 LOAD_FAST                4 (csv_line)
+         248     >>  170 LOAD_FAST                4 (csv_line)
                      172 LOAD_CONST               1 (',')
                      174 BINARY_OP               13 (+=)
                      178 STORE_FAST               4 (csv_line)
                      180 JUMP_BACKWARD           40 (to 102)
          
-         246     >>  182 LOAD_FAST                2 (csv_string)
+         250     >>  182 LOAD_FAST                2 (csv_string)
                      184 LOAD_FAST                4 (csv_line)
                      186 LOAD_CONST               0 (None)
                      188 LOAD_CONST               4 (-1)
                      190 BUILD_SLICE              2
                      192 BINARY_SUBSCR
                      202 LOAD_CONST               2 ('\n')
                      204 BINARY_OP                0 (+)
                      208 BINARY_OP               13 (+=)
                      212 STORE_FAST               2 (csv_string)
                      214 JUMP_BACKWARD           63 (to 90)
          
-         248     >>  216 LOAD_FAST                2 (csv_string)
+         252     >>  216 LOAD_FAST                2 (csv_string)
                      218 LOAD_CONST               0 (None)
                      220 LOAD_CONST               4 (-1)
                      222 BUILD_SLICE              2
                      224 BINARY_SUBSCR
                      234 RETURN_VALUE
          consts
             None
@@ -1455,20 +1489,22 @@
             -1
          names      ('join', 'values', 'escape_csv')
          varnames   ('column_list', 'export_data', 'csv_string', 'row', 'csv_line', 'column')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\export_helpers.py'
          name       'build_export_csv'
-         firstlineno 235
+         firstlineno 239
          lnotab 0x020130022c0104010801080138020c022202
+      (True, True)
       (True,)
    names      ('BOFS.globals', 'db', 'questionnaires', 'page_list', 'sqlalchemy', 'util', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label', 'flask', 'current_app', 'dict', 'create_export_base_query', 'list', 'str', 'orm', 'Query', 'add_participants_to_export', 'add_questionnaires_to_export', 'add_custom_exports_to_export', 'build_export_csv')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\export_helpers.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02011401080114010c030c5102fe140102ff020216fe082602fd14
-      0102ff020216fe020302fd084602fd140102ff020216fe020302fd082f
+      0x00ff02011401080114010c030c51020102fd140102ff020316fd082a02
+      fd140102ff020216fe020302fd084602fd140102ff020216fe020302fd08
+      2f
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/util.cpython-310.pyc` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/util.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/util.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x47b7aa65 (Fri Jan 19 17:54:15 2024 UTC)
-files sz: 3141
+moddate:  0x15ec1266 (Sun Apr  7 18:55:17 2024 UTC)
+files sz: 3182
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -57,43 +57,43 @@
                 74 IMPORT_NAME             13 (decimal)
                 76 STORE_NAME              13 (decimal)
                 78 LOAD_CONST               0 (0)
                 80 LOAD_CONST               1 (None)
                 82 IMPORT_NAME             14 (datetime)
                 84 STORE_NAME              14 (datetime)
    
-     8          86 LOAD_CONST               5 (<code object _datetime_convert, file "C:\Users\colby\Desktop\UVic\With Max Friehs\tDCS Hexagon\BOF_SuperHexagon_tDCS\venv\Lib\site-packages\BOFS/admin/util.py", line 8>)
+     8          86 LOAD_CONST               5 (<code object _datetime_convert, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\util.py", line 8>)
                 88 MAKE_FUNCTION            0
                 90 STORE_NAME              15 (_datetime_convert)
    
-    12          92 LOAD_CONST               6 (<code object remove_non_ascii, file "C:\Users\colby\Desktop\UVic\With Max Friehs\tDCS Hexagon\BOF_SuperHexagon_tDCS\venv\Lib\site-packages\BOFS/admin/util.py", line 12>)
+    12          92 LOAD_CONST               6 (<code object remove_non_ascii, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\util.py", line 12>)
                 94 MAKE_FUNCTION            0
                 96 STORE_NAME              16 (remove_non_ascii)
    
-    16          98 LOAD_CONST               7 (<code object alchemy_encoder, file "C:\Users\colby\Desktop\UVic\With Max Friehs\tDCS Hexagon\BOF_SuperHexagon_tDCS\venv\Lib\site-packages\BOFS/admin/util.py", line 16>)
+    16          98 LOAD_CONST               7 (<code object alchemy_encoder, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\util.py", line 16>)
                100 MAKE_FUNCTION            0
                102 STORE_NAME              17 (alchemy_encoder)
    
-    27         104 LOAD_CONST               8 (<code object sqlalchemy_to_json, file "C:\Users\colby\Desktop\UVic\With Max Friehs\tDCS Hexagon\BOF_SuperHexagon_tDCS\venv\Lib\site-packages\BOFS/admin/util.py", line 27>)
+    27         104 LOAD_CONST               8 (<code object sqlalchemy_to_json, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\util.py", line 27>)
                106 MAKE_FUNCTION            0
                108 STORE_NAME              18 (sqlalchemy_to_json)
    
-    53         110 LOAD_CONST               9 (<code object verify_admin, file "C:\Users\colby\Desktop\UVic\With Max Friehs\tDCS Hexagon\BOF_SuperHexagon_tDCS\venv\Lib\site-packages\BOFS/admin/util.py", line 53>)
+    53         110 LOAD_CONST               9 (<code object verify_admin, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\util.py", line 53>)
                112 MAKE_FUNCTION            0
                114 STORE_NAME              19 (verify_admin)
    
-    65         116 LOAD_CONST              10 (<code object escape_csv, file "C:\Users\colby\Desktop\UVic\With Max Friehs\tDCS Hexagon\BOF_SuperHexagon_tDCS\venv\Lib\site-packages\BOFS/admin/util.py", line 65>)
+    65         116 LOAD_CONST              10 (<code object escape_csv, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\util.py", line 65>)
                118 MAKE_FUNCTION            0
                120 STORE_NAME              20 (escape_csv)
    
-    76         122 LOAD_CONST              11 (<code object condition_num_to_label, file "C:\Users\colby\Desktop\UVic\With Max Friehs\tDCS Hexagon\BOF_SuperHexagon_tDCS\venv\Lib\site-packages\BOFS/admin/util.py", line 76>)
+    76         122 LOAD_CONST              11 (<code object condition_num_to_label, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\util.py", line 76>)
                124 MAKE_FUNCTION            0
                126 STORE_NAME              21 (condition_num_to_label)
    
-    85         128 LOAD_CONST              12 (<code object questionnaire_name_and_tag, file "C:\Users\colby\Desktop\UVic\With Max Friehs\tDCS Hexagon\BOF_SuperHexagon_tDCS\venv\Lib\site-packages\BOFS/admin/util.py", line 85>)
+    85         128 LOAD_CONST              12 (<code object questionnaire_name_and_tag, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\util.py", line 85>)
                130 MAKE_FUNCTION            0
                132 STORE_NAME              22 (questionnaire_name_and_tag)
                134 LOAD_CONST               1 (None)
                136 RETURN_VALUE
    consts
       0
       None
@@ -119,15 +119,15 @@
          consts
             None
             '%Y-%m-%d %H:%M:%S'
          names      ('strftime',)
          varnames   ('v',)
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\UVic\\With Max Friehs\\tDCS Hexagon\\BOF_SuperHexagon_tDCS\\venv\\Lib\\site-packages\\BOFS/admin/util.py'
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\util.py'
          name       '_datetime_convert'
          firstlineno 8
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -137,15 +137,15 @@
             007c004400a6000000ab000000000000000000a6010000ab010000000000
             000000a001000000000000000000000000000000000000000064036404a6
             020000ab0200000000000000005300
           12           0 RESUME                   0
          
           13           2 LOAD_CONST               1 ('')
                        4 LOAD_METHOD              0 (join)
-                      26 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\colby\Desktop\UVic\With Max Friehs\tDCS Hexagon\BOF_SuperHexagon_tDCS\venv\Lib\site-packages\BOFS/admin/util.py", line 13>)
+                      26 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\util.py", line 13>)
                       28 MAKE_FUNCTION            0
                       30 LOAD_FAST                0 (s)
                       32 GET_ITER
                       34 PRECALL                  0
                       38 CALL                     0
                       48 PRECALL                  1
                       52 CALL                     1
@@ -184,25 +184,25 @@
                        >>   54 RETURN_VALUE
                consts
                   128
                names      ('ord',)
                varnames   ('.0', 'x')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\colby\\Desktop\\UVic\\With Max Friehs\\tDCS Hexagon\\BOF_SuperHexagon_tDCS\\venv\\Lib\\site-packages\\BOFS/admin/util.py'
+               filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\util.py'
                name       '<listcomp>'
                firstlineno 13
                lnotab 0x
             'ascii'
             'xmlcharrefreplace'
          names      ('join', 'encode')
          varnames   ('s',)
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\UVic\\With Max Friehs\\tDCS Hexagon\\BOF_SuperHexagon_tDCS\\venv\\Lib\\site-packages\\BOFS/admin/util.py'
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\util.py'
          name       'remove_non_ascii'
          firstlineno 12
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -250,15 +250,15 @@
          consts
             '\n    JSON encoder function for SQLAlchemy special classes.\n    https://codeandlife.com/2014/12/07/sqlalchemy-results-to-json-the-easy-way/\n    '
             None
          names      ('isinstance', 'datetime', 'date', 'isoformat', 'decimal', 'Decimal', 'float')
          varnames   ('obj',)
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\UVic\\With Max Friehs\\tDCS Hexagon\\BOF_SuperHexagon_tDCS\\venv\\Lib\\site-packages\\BOFS/admin/util.py'
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\util.py'
          name       'alchemy_encoder'
          firstlineno 16
          lnotab 0x02053401280134011eff
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 7
@@ -455,15 +455,15 @@
             '&#123;'
             '}'
             '&#125;'
          names      ('dict', '_datetime_convert', 'columns', 'getattr', 'name', 'type', 'list', 'keys', 'Exception', 'str', 'isinstance', 'remove_non_ascii', 'replace', 'json', 'dumps')
          varnames   ('inst', 'cls', 'convert', 'd', 'c', 'v')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\UVic\\With Max Friehs\\tDCS Hexagon\\BOF_SuperHexagon_tDCS\\venv\\Lib\\site-packages\\BOFS/admin/util.py'
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\util.py'
          name       'sqlalchemy_to_json'
          firstlineno 27
          lnotab
             0x02051c0114021c0114012a0154010201400112014cff080204012e022a
             01aa023201
       code
          argcount  : 1
@@ -481,84 +481,100 @@
           57           4 LOAD_GLOBAL              1 (NULL + wraps)
                       16 LOAD_DEREF               0 (f)
                       18 PRECALL                  1
                       22 CALL                     1
          
           58          32 LOAD_CLOSURE             0 (f)
                       34 BUILD_TUPLE              1
-                      36 LOAD_CONST               1 (<code object decorated_function, file "C:\Users\colby\Desktop\UVic\With Max Friehs\tDCS Hexagon\BOF_SuperHexagon_tDCS\venv\Lib\site-packages\BOFS/admin/util.py", line 57>)
+                      36 LOAD_CONST               1 (<code object decorated_function, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\util.py", line 57>)
                       38 MAKE_FUNCTION            8 (closure)
          
           57          40 PRECALL                  0
                       44 CALL                     0
          
           58          54 STORE_FAST               1 (decorated_function)
          
           62          56 LOAD_FAST                1 (decorated_function)
                       58 RETURN_VALUE
          consts
             '\n    A decorator to be used for admin routes, which checks if the user is logged in. If not, the login page is shown.\n    '
             code
                argcount  : 0
                nlocals   : 2
-               stacksize : 5
+               stacksize : 10
                flags     : 31
                code
                   0x9501970064017400000000000000000000007601730d74000000000000
-                  0000000000640119000000000000000000731c7403000000000000000000
-                  007405000000000000000000006402a6010000ab010000000000000000a6
-                  010000ab0100000000000000005300020089027c0069007c01a4018e0153
-                  00
+                  0000000000640119000000000000000000733e7403000000000000000000
+                  007405000000000000000000006402a6010000ab01000000000000000064
+                  037a00000074070000000000000000000089026404740900000000000000
+                  0000008902a6010000ab010000000000000000a6030000ab030000000000
+                  0000007a000000a6010000ab0100000000000000005300020089027c0069
+                  007c01a4018e015300
                              0 COPY_FREE_VARS           1
                
                 57           2 RESUME                   0
                
                 59           4 LOAD_CONST               1 ('loggedIn')
                              6 LOAD_GLOBAL              0 (session)
                             18 CONTAINS_OP              1
                             20 POP_JUMP_FORWARD_IF_TRUE    13 (to 48)
                             22 LOAD_GLOBAL              0 (session)
                             34 LOAD_CONST               1 ('loggedIn')
                             36 BINARY_SUBSCR
-                            46 POP_JUMP_FORWARD_IF_TRUE    28 (to 104)
+                            46 POP_JUMP_FORWARD_IF_TRUE    62 (to 172)
                
                 60     >>   48 LOAD_GLOBAL              3 (NULL + redirect)
                             60 LOAD_GLOBAL              5 (NULL + url_for)
                             72 LOAD_CONST               2 ('admin.admin_login')
                             74 PRECALL                  1
                             78 CALL                     1
-                            88 PRECALL                  1
-                            92 CALL                     1
-                           102 RETURN_VALUE
-               
-                61     >>  104 PUSH_NULL
+                            88 LOAD_CONST               3 ('?r=')
+                            90 BINARY_OP                0 (+)
+                            94 LOAD_GLOBAL              7 (NULL + getattr)
                            106 LOAD_DEREF               2 (f)
-                           108 LOAD_FAST                0 (args)
-                           110 BUILD_MAP                0
-                           112 LOAD_FAST                1 (kwargs)
-                           114 DICT_MERGE               1
-                           116 CALL_FUNCTION_EX         1
-                           118 RETURN_VALUE
+                           108 LOAD_CONST               4 ('__name__')
+                           110 LOAD_GLOBAL              9 (NULL + str)
+                           122 LOAD_DEREF               2 (f)
+                           124 PRECALL                  1
+                           128 CALL                     1
+                           138 PRECALL                  3
+                           142 CALL                     3
+                           152 BINARY_OP                0 (+)
+                           156 PRECALL                  1
+                           160 CALL                     1
+                           170 RETURN_VALUE
+               
+                61     >>  172 PUSH_NULL
+                           174 LOAD_DEREF               2 (f)
+                           176 LOAD_FAST                0 (args)
+                           178 BUILD_MAP                0
+                           180 LOAD_FAST                1 (kwargs)
+                           182 DICT_MERGE               1
+                           184 CALL_FUNCTION_EX         1
+                           186 RETURN_VALUE
                consts
                   None
                   'loggedIn'
                   'admin.admin_login'
-               names      ('session', 'redirect', 'url_for')
+                  '?r='
+                  '__name__'
+               names      ('session', 'redirect', 'url_for', 'getattr', 'str')
                varnames   ('args', 'kwargs')
                freevars   ('f',)
                cellvars   ()
-               filename   'C:\\Users\\colby\\Desktop\\UVic\\With Max Friehs\\tDCS Hexagon\\BOF_SuperHexagon_tDCS\\venv\\Lib\\site-packages\\BOFS/admin/util.py'
+               filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\util.py'
                name       'decorated_function'
                firstlineno 57
-               lnotab 0x04022c013801
+               lnotab 0x04022c017c01
          names      ('wraps',)
          varnames   ('f', 'decorated_function')
          freevars   ()
          cellvars   ('f',)
-         filename   'C:\\Users\\colby\\Desktop\\UVic\\With Max Friehs\\tDCS Hexagon\\BOF_SuperHexagon_tDCS\\venv\\Lib\\site-packages\\BOFS/admin/util.py'
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\util.py'
          name       'verify_admin'
          firstlineno 53
          lnotab 0x04041c0108ff0e010204
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 7
@@ -661,15 +677,15 @@
             True
             1
             0
          names      ('isinstance', 'str', 'format', 'strip', 'replace', 'type', 'bool')
          varnames   ('input',)
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\UVic\\With Max Friehs\\tDCS Hexagon\\BOF_SuperHexagon_tDCS\\venv\\Lib\\site-packages\\BOFS/admin/util.py'
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\util.py'
          name       'escape_csv'
          firstlineno 65
          lnotab 0x02012a01d20104011c012c014802
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -725,15 +741,15 @@
             ''
             1
             'label'
          names      ('len', 'current_app', 'config')
          varnames   ('condition',)
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\UVic\\With Max Friehs\\tDCS Hexagon\\BOF_SuperHexagon_tDCS\\venv\\Lib\\site-packages\\BOFS/admin/util.py'
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\util.py'
          name       'condition_num_to_label'
          firstlineno 76
          lnotab 0x02014601040110010402
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 3
@@ -784,19 +800,19 @@
             0
             1
             ''
          names      ('split',)
          varnames   ('questionnnaireNameAndTagString', 'split', 'qName', 'qTag')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\UVic\\With Max Friehs\\tDCS Hexagon\\BOF_SuperHexagon_tDCS\\venv\\Lib\\site-packages\\BOFS/admin/util.py'
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\util.py'
          name       'questionnaire_name_and_tag'
          firstlineno 85
          lnotab 0x020708012a011001120204010402
    names      ('json', 'functools', 'wraps', 'flask', 'request', 'session', 'current_app', 'render_template', 'g', 'redirect', 'url_for', 'BOFS.globals', 'db', 'decimal', 'datetime', '_datetime_convert', 'remove_non_ascii', 'alchemy_encoder', 'sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'condition_num_to_label', 'questionnaire_name_and_tag')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\colby\\Desktop\\UVic\\With Max Friehs\\tDCS Hexagon\\BOF_SuperHexagon_tDCS\\venv\\Lib\\site-packages\\BOFS/admin/util.py'
+   filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\util.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108010c0124010c01100306040604060b061a060c060b0609
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/views.cpython-310.pyc` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/__pycache__/views.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/__pycache__/views.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,70 +1,79 @@
 magic:    0xa70d0d0a
-moddate:  0x319b0366 (Wed Mar 27 04:06:09 2024 UTC)
-files sz: 14926
+moddate:  0x0c8d1366 (Mon Apr  8 06:22:04 2024 UTC)
+files sz: 19208
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a046d
-      055a056d065a066d075a076d085a086d095a096d0a5a0a0100640064036c
-      0b6d0c5a0c6d0d5a0d6d0e5a0e0100640064046c0f6d105a106d115a1101
-      00640564066c126d135a136d145a146d155a156d165a166d175a17010064
-      0564076c185400640064016c195a19640564076c1a5400640064086c1b6d
-      1b5a1b0100640064096c1c6d1d5a1d6d1e5a1e010002006502640a651f64
-      0b640c640dac0ea6050000ab0500000000000000005a2065206a21000000
-      0000000000640f8400a6000000ab0000000000000000005a226520a02300
-      000000000000000000000000000000000000006410a6010000ab01000000
-      000000000064118400a6000000ab0000000000000000005a246520a02300
-      000000000000000000000000000000000000006412641364146702ac15a6
-      020000ab02000000000000000064168400a6000000ab0000000000000000
-      005a25641784005a26641884005a276520a0230000000000000000000000
-      0000000000000000006419a6010000ab0100000000000000006514641a84
+      055a056d065a066d075a076d085a086d095a096d0a5a0a6d0b5a0b010064
+      0064036c0c6d0d5a0d6d0e5a0e6d0f5a0f0100640064046c106d115a116d
+      125a126d135a136d145a140100640564066c156d165a166d175a176d185a
+      186d195a196d1a5a1a0100640564076c1b5400640064016c1c5a1c640564
+      076c1d5400640064086c1e6d1e5a1e0100640064096c1f6d205a206d215a
+      2101006400640a6c226d235a23010002006502640b6524640c640d640eac
+      0fa6050000ab0500000000000000005a2565256a26000000000000000064
+      108400a6000000ab0000000000000000005a276525a02800000000000000
+      000000000000000000000000006411a6010000ab01000000000000000064
+      128400a6000000ab0000000000000000005a296525a02800000000000000
+      000000000000000000000000006413641464156702ac16a6020000ab0200
+      0000000000000064178400a6000000ab0000000000000000005a2a641884
+      005a2b641984005a2c6525a0280000000000000000000000000000000000
+      000000641aa6010000ab0100000000000000006517641b8400a6000000ab
+      000000000000000000a6000000ab0000000000000000005a2d6525a02800
+      00000000000000000000000000000000000000641ca6010000ab01000000
+      00000000006517641d8400a6000000ab000000000000000000a6000000ab
+      0000000000000000005a2e6525a028000000000000000000000000000000
+      0000000000641ea6010000ab0100000000000000006517641f8400a60000
+      00ab000000000000000000a6000000ab0000000000000000005a2f6525a0
+      3000000000000000000000000000000000000000006420a6010000ab0100
+      0000000000000064218400a6000000ab0000000000000000005a316525a0
+      2800000000000000000000000000000000000000006422a6010000ab0100
+      00000000000000651764238400a6000000ab000000000000000000a60000
+      00ab0000000000000000005a326525a02800000000000000000000000000
+      000000000000006424a6010000ab0100000000000000006525a028000000
+      000000000000000000000000000000000064256426ac27a6020000ab0200
+      00000000000000651764288400a6000000ab000000000000000000a60000
+      00ab000000000000000000a6000000ab0000000000000000005a336525a0
+      2800000000000000000000000000000000000000006429a6010000ab0100
+      000000000000006517642a8400a6000000ab000000000000000000a60000
+      00ab0000000000000000005a346525a02800000000000000000000000000
+      00000000000000642b641464156702ac16a6020000ab0200000000000000
+      006517642c8400a6000000ab000000000000000000a6000000ab00000000
+      00000000005a356525a02800000000000000000000000000000000000000
+      00642da6010000ab0100000000000000006517642e8400a6000000ab0000
+      00000000000000a6000000ab0000000000000000005a36642f84005a3765
+      25a02800000000000000000000000000000000000000006430a6010000ab
+      010000000000000000651764318400a6000000ab000000000000000000a6
+      000000ab0000000000000000005a386525a0280000000000000000000000
+      0000000000000000006432a6010000ab0100000000000000006517643384
       00a6000000ab000000000000000000a6000000ab0000000000000000005a
-      286520a0230000000000000000000000000000000000000000641ba60100
-      00ab0100000000000000006514641c8400a6000000ab0000000000000000
-      00a6000000ab0000000000000000005a296520a023000000000000000000
-      0000000000000000000000641da6010000ab010000000000000000651464
-      1e8400a6000000ab000000000000000000a6000000ab0000000000000000
-      005a2a6520a0230000000000000000000000000000000000000000641fa6
-      010000ab010000000000000000651464208400a6000000ab000000000000
-      000000a6000000ab0000000000000000005a2b6520a02300000000000000
-      000000000000000000000000006421a6010000ab01000000000000000065
-      20a023000000000000000000000000000000000000000064226423ac24a6
-      020000ab020000000000000000651464258400a6000000ab000000000000
-      000000a6000000ab000000000000000000a6000000ab0000000000000000
-      005a2c6520a02300000000000000000000000000000000000000006426a6
-      010000ab010000000000000000651464278400a6000000ab000000000000
-      000000a6000000ab0000000000000000005a2d6520a02300000000000000
-      000000000000000000000000006428a6010000ab01000000000000000065
-      1464298400a6000000ab000000000000000000a6000000ab000000000000
-      0000005a2e6520a023000000000000000000000000000000000000000064
-      2aa6010000ab0100000000000000006514642b8400a6000000ab00000000
-      0000000000a6000000ab0000000000000000005a2f642c84005a306520a0
-      230000000000000000000000000000000000000000642da6010000ab0100
-      000000000000006514642e8400a6000000ab000000000000000000a60000
-      00ab0000000000000000005a316520a02300000000000000000000000000
-      00000000000000642fa6010000ab010000000000000000651464308400a6
-      000000ab000000000000000000a6000000ab0000000000000000005a3265
-      20a02300000000000000000000000000000000000000006431a6010000ab
-      010000000000000000651464328400a6000000ab000000000000000000a6
-      000000ab0000000000000000005a336520a0340000000000000000000000
-      0000000000000000006433a6010000ab01000000000000000064348400a6
-      000000ab0000000000000000005a3564015300
+      396525a02800000000000000000000000000000000000000006434a60100
+      00ab010000000000000000651764358400a6000000ab0000000000000000
+      00a6000000ab0000000000000000005a3a6525a028000000000000000000
+      00000000000000000000006436a6010000ab010000000000000000651764
+      378400a6000000ab000000000000000000a6000000ab0000000000000000
+      005a3b6525a0280000000000000000000000000000000000000000643864
+      1464156702ac16a6020000ab020000000000000000651764398400a60000
+      00ab000000000000000000a6000000ab0000000000000000005a3c6525a0
+      3d0000000000000000000000000000000000000000643aa6010000ab0100
+      00000000000000643b8400a6000000ab0000000000000000005a3e640153
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (sqlalchemy)
                  8 STORE_NAME               0 (sqlalchemy)
    
      2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response'))
+                12 LOAD_CONST               2 (('Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response', 'send_file'))
                 14 IMPORT_NAME              1 (flask)
                 16 IMPORT_FROM              2 (Blueprint)
                 18 STORE_NAME               2 (Blueprint)
                 20 IMPORT_FROM              3 (render_template)
                 22 STORE_NAME               3 (render_template)
                 24 IMPORT_FROM              4 (current_app)
                 26 STORE_NAME               4 (current_app)
@@ -76,404 +85,478 @@
                 38 STORE_NAME               7 (request)
                 40 IMPORT_FROM              8 (session)
                 42 STORE_NAME               8 (session)
                 44 IMPORT_FROM              9 (url_for)
                 46 STORE_NAME               9 (url_for)
                 48 IMPORT_FROM             10 (Response)
                 50 STORE_NAME              10 (Response)
-                52 POP_TOP
+                52 IMPORT_FROM             11 (send_file)
+                54 STORE_NAME              11 (send_file)
+                56 POP_TOP
    
-     3          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               3 (('db', 'questionnaires', 'page_list'))
-                58 IMPORT_NAME             11 (BOFS.globals)
-                60 IMPORT_FROM             12 (db)
-                62 STORE_NAME              12 (db)
-                64 IMPORT_FROM             13 (questionnaires)
-                66 STORE_NAME              13 (questionnaires)
-                68 IMPORT_FROM             14 (page_list)
-                70 STORE_NAME              14 (page_list)
-                72 POP_TOP
+     3          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               3 (('db', 'questionnaires', 'page_list'))
+                62 IMPORT_NAME             12 (BOFS.globals)
+                64 IMPORT_FROM             13 (db)
+                66 STORE_NAME              13 (db)
+                68 IMPORT_FROM             14 (questionnaires)
+                70 STORE_NAME              14 (questionnaires)
+                72 IMPORT_FROM             15 (page_list)
+                74 STORE_NAME              15 (page_list)
+                76 POP_TOP
    
-     4          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               4 (('fetch_condition_count', 'display_time'))
-                78 IMPORT_NAME             15 (BOFS.util)
-                80 IMPORT_FROM             16 (fetch_condition_count)
-                82 STORE_NAME              16 (fetch_condition_count)
-                84 IMPORT_FROM             17 (display_time)
-                86 STORE_NAME              17 (display_time)
-                88 POP_TOP
+     4          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               4 (('fetch_condition_count', 'display_time', 'provide_consent', 'int_or_0'))
+                82 IMPORT_NAME             16 (BOFS.util)
+                84 IMPORT_FROM             17 (fetch_condition_count)
+                86 STORE_NAME              17 (fetch_condition_count)
+                88 IMPORT_FROM             18 (display_time)
+                90 STORE_NAME              18 (display_time)
+                92 IMPORT_FROM             19 (provide_consent)
+                94 STORE_NAME              19 (provide_consent)
+                96 IMPORT_FROM             20 (int_or_0)
+                98 STORE_NAME              20 (int_or_0)
+               100 POP_TOP
    
-     5          90 LOAD_CONST               5 (1)
-                92 LOAD_CONST               6 (('sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label'))
-                94 IMPORT_NAME             18 (util)
-                96 IMPORT_FROM             19 (sqlalchemy_to_json)
-                98 STORE_NAME              19 (sqlalchemy_to_json)
-               100 IMPORT_FROM             20 (verify_admin)
-               102 STORE_NAME              20 (verify_admin)
-               104 IMPORT_FROM             21 (escape_csv)
-               106 STORE_NAME              21 (escape_csv)
-               108 IMPORT_FROM             22 (questionnaire_name_and_tag)
-               110 STORE_NAME              22 (questionnaire_name_and_tag)
-               112 IMPORT_FROM             23 (condition_num_to_label)
-               114 STORE_NAME              23 (condition_num_to_label)
-               116 POP_TOP
+     5         102 LOAD_CONST               5 (1)
+               104 LOAD_CONST               6 (('sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label'))
+               106 IMPORT_NAME             21 (util)
+               108 IMPORT_FROM             22 (sqlalchemy_to_json)
+               110 STORE_NAME              22 (sqlalchemy_to_json)
+               112 IMPORT_FROM             23 (verify_admin)
+               114 STORE_NAME              23 (verify_admin)
+               116 IMPORT_FROM             24 (escape_csv)
+               118 STORE_NAME              24 (escape_csv)
+               120 IMPORT_FROM             25 (questionnaire_name_and_tag)
+               122 STORE_NAME              25 (questionnaire_name_and_tag)
+               124 IMPORT_FROM             26 (condition_num_to_label)
+               126 STORE_NAME              26 (condition_num_to_label)
+               128 POP_TOP
    
-     6         118 LOAD_CONST               5 (1)
-               120 LOAD_CONST               7 (('*',))
-               122 IMPORT_NAME             24 (export_helpers)
-               124 IMPORT_STAR
+     6         130 LOAD_CONST               5 (1)
+               132 LOAD_CONST               7 (('*',))
+               134 IMPORT_NAME             27 (export_helpers)
+               136 IMPORT_STAR
    
-     7         126 LOAD_CONST               0 (0)
-               128 LOAD_CONST               1 (None)
-               130 IMPORT_NAME             25 (json)
-               132 STORE_NAME              25 (json)
+     7         138 LOAD_CONST               0 (0)
+               140 LOAD_CONST               1 (None)
+               142 IMPORT_NAME             28 (json)
+               144 STORE_NAME              28 (json)
    
-     8         134 LOAD_CONST               5 (1)
-               136 LOAD_CONST               7 (('*',))
-               138 IMPORT_NAME             26 (QuestionnaireResults)
-               140 IMPORT_STAR
+     8         146 LOAD_CONST               5 (1)
+               148 LOAD_CONST               7 (('*',))
+               150 IMPORT_NAME             29 (QuestionnaireResults)
+               152 IMPORT_STAR
    
-     9         142 LOAD_CONST               0 (0)
-               144 LOAD_CONST               8 (('datetime',))
-               146 IMPORT_NAME             27 (datetime)
-               148 IMPORT_FROM             27 (datetime)
-               150 STORE_NAME              27 (datetime)
-               152 POP_TOP
+     9         154 LOAD_CONST               0 (0)
+               156 LOAD_CONST               8 (('datetime',))
+               158 IMPORT_NAME             30 (datetime)
+               160 IMPORT_FROM             30 (datetime)
+               162 STORE_NAME              30 (datetime)
+               164 POP_TOP
    
-    10         154 LOAD_CONST               0 (0)
-               156 LOAD_CONST               9 (('path', 'listdir'))
-               158 IMPORT_NAME             28 (os)
-               160 IMPORT_FROM             29 (path)
-               162 STORE_NAME              29 (path)
-               164 IMPORT_FROM             30 (listdir)
-               166 STORE_NAME              30 (listdir)
-               168 POP_TOP
+    10         166 LOAD_CONST               0 (0)
+               168 LOAD_CONST               9 (('path', 'listdir'))
+               170 IMPORT_NAME             31 (os)
+               172 IMPORT_FROM             32 (path)
+               174 STORE_NAME              32 (path)
+               176 IMPORT_FROM             33 (listdir)
+               178 STORE_NAME              33 (listdir)
+               180 POP_TOP
    
-    12         170 PUSH_NULL
-               172 LOAD_NAME                2 (Blueprint)
-               174 LOAD_CONST              10 ('admin')
-               176 LOAD_NAME               31 (__name__)
-               178 LOAD_CONST              11 ('templates')
-               180 LOAD_CONST              12 ('static')
-               182 LOAD_CONST              13 ('/admin')
-               184 KW_NAMES                14
-               186 PRECALL                  5
-               190 CALL                     5
-               200 STORE_NAME              32 (admin)
+    11         182 LOAD_CONST               0 (0)
+               184 LOAD_CONST              10 (('copyfile',))
+               186 IMPORT_NAME             34 (shutil)
+               188 IMPORT_FROM             35 (copyfile)
+               190 STORE_NAME              35 (copyfile)
+               192 POP_TOP
    
-    15         202 LOAD_NAME               32 (admin)
-               204 LOAD_ATTR               33 (context_processor)
+    13         194 PUSH_NULL
+               196 LOAD_NAME                2 (Blueprint)
+               198 LOAD_CONST              11 ('admin')
+               200 LOAD_NAME               36 (__name__)
+               202 LOAD_CONST              12 ('templates')
+               204 LOAD_CONST              13 ('static')
+               206 LOAD_CONST              14 ('/admin')
+               208 KW_NAMES                15
+               210 PRECALL                  5
+               214 CALL                     5
+               224 STORE_NAME              37 (admin)
    
-    16         214 LOAD_CONST              15 (<code object inject_template_vars, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 15>)
-               216 MAKE_FUNCTION            0
+    16         226 LOAD_NAME               37 (admin)
+               228 LOAD_ATTR               38 (context_processor)
    
-    15         218 PRECALL                  0
-               222 CALL                     0
+    17         238 LOAD_CONST              16 (<code object inject_template_vars, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 16>)
+               240 MAKE_FUNCTION            0
    
-    16         232 STORE_NAME              34 (inject_template_vars)
+    16         242 PRECALL                  0
+               246 CALL                     0
    
-    55         234 LOAD_NAME               32 (admin)
-               236 LOAD_METHOD             35 (route)
-               258 LOAD_CONST              16 ('/')
-               260 PRECALL                  1
-               264 CALL                     1
+    17         256 STORE_NAME              39 (inject_template_vars)
    
-    56         274 LOAD_CONST              17 (<code object admin_index, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 55>)
-               276 MAKE_FUNCTION            0
+    59         258 LOAD_NAME               37 (admin)
+               260 LOAD_METHOD             40 (route)
+               282 LOAD_CONST              17 ('/')
+               284 PRECALL                  1
+               288 CALL                     1
    
-    55         278 PRECALL                  0
-               282 CALL                     0
+    60         298 LOAD_CONST              18 (<code object admin_index, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 59>)
+               300 MAKE_FUNCTION            0
    
-    56         292 STORE_NAME              36 (admin_index)
+    59         302 PRECALL                  0
+               306 CALL                     0
    
-    60         294 LOAD_NAME               32 (admin)
-               296 LOAD_METHOD             35 (route)
-               318 LOAD_CONST              18 ('/login')
-               320 LOAD_CONST              19 ('GET')
-               322 LOAD_CONST              20 ('POST')
-               324 BUILD_LIST               2
-               326 KW_NAMES                21
-               328 PRECALL                  2
-               332 CALL                     2
+    60         316 STORE_NAME              41 (admin_index)
    
-    61         342 LOAD_CONST              22 (<code object admin_login, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 60>)
-               344 MAKE_FUNCTION            0
+    64         318 LOAD_NAME               37 (admin)
+               320 LOAD_METHOD             40 (route)
+               342 LOAD_CONST              19 ('/login')
+               344 LOAD_CONST              20 ('GET')
+               346 LOAD_CONST              21 ('POST')
+               348 BUILD_LIST               2
+               350 KW_NAMES                22
+               352 PRECALL                  2
+               356 CALL                     2
    
-    60         346 PRECALL                  0
-               350 CALL                     0
+    65         366 LOAD_CONST              23 (<code object admin_login, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 64>)
+               368 MAKE_FUNCTION            0
    
-    61         360 STORE_NAME              37 (admin_login)
+    64         370 PRECALL                  0
+               374 CALL                     0
    
-    77         362 LOAD_CONST              23 (<code object fetch_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 77>)
-               364 MAKE_FUNCTION            0
-               366 STORE_NAME              38 (fetch_progress)
+    65         384 STORE_NAME              42 (admin_login)
    
-   100         368 LOAD_CONST              24 (<code object fetch_progress_summary, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 100>)
-               370 MAKE_FUNCTION            0
-               372 STORE_NAME              39 (fetch_progress_summary)
+   106         386 LOAD_CONST              24 (<code object fetch_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 106>)
+               388 MAKE_FUNCTION            0
+               390 STORE_NAME              43 (fetch_progress)
    
-   123         374 LOAD_NAME               32 (admin)
-               376 LOAD_METHOD             35 (route)
-               398 LOAD_CONST              25 ('/progress')
-               400 PRECALL                  1
-               404 CALL                     1
+   129         392 LOAD_CONST              25 (<code object fetch_progress_summary, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 129>)
+               394 MAKE_FUNCTION            0
+               396 STORE_NAME              44 (fetch_progress_summary)
    
-   124         414 LOAD_NAME               20 (verify_admin)
+   154         398 LOAD_NAME               37 (admin)
+               400 LOAD_METHOD             40 (route)
+               422 LOAD_CONST              26 ('/progress')
+               424 PRECALL                  1
+               428 CALL                     1
    
-   125         416 LOAD_CONST              26 (<code object route_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 123>)
-               418 MAKE_FUNCTION            0
+   155         438 LOAD_NAME               23 (verify_admin)
    
-   124         420 PRECALL                  0
-               424 CALL                     0
+   156         440 LOAD_CONST              27 (<code object route_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 154>)
+               442 MAKE_FUNCTION            0
    
-   123         434 PRECALL                  0
-               438 CALL                     0
+   155         444 PRECALL                  0
+               448 CALL                     0
    
-   125         448 STORE_NAME              40 (route_progress)
+   154         458 PRECALL                  0
+               462 CALL                     0
    
-   134         450 LOAD_NAME               32 (admin)
-               452 LOAD_METHOD             35 (route)
-               474 LOAD_CONST              27 ('/progress_ajax')
-               476 PRECALL                  1
-               480 CALL                     1
+   156         472 STORE_NAME              45 (route_progress)
    
-   135         490 LOAD_NAME               20 (verify_admin)
+   165         474 LOAD_NAME               37 (admin)
+               476 LOAD_METHOD             40 (route)
+               498 LOAD_CONST              28 ('/progress_ajax')
+               500 PRECALL                  1
+               504 CALL                     1
    
-   136         492 LOAD_CONST              28 (<code object route_progress_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 134>)
-               494 MAKE_FUNCTION            0
+   166         514 LOAD_NAME               23 (verify_admin)
    
-   135         496 PRECALL                  0
-               500 CALL                     0
+   167         516 LOAD_CONST              29 (<code object route_progress_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 165>)
+               518 MAKE_FUNCTION            0
    
-   134         510 PRECALL                  0
-               514 CALL                     0
+   166         520 PRECALL                  0
+               524 CALL                     0
    
-   136         524 STORE_NAME              41 (route_progress_ajax)
+   165         534 PRECALL                  0
+               538 CALL                     0
    
-   141         526 LOAD_NAME               32 (admin)
-               528 LOAD_METHOD             35 (route)
-               550 LOAD_CONST              29 ('/progress_summary_ajax')
-               552 PRECALL                  1
-               556 CALL                     1
+   167         548 STORE_NAME              46 (route_progress_ajax)
    
-   142         566 LOAD_NAME               20 (verify_admin)
+   172         550 LOAD_NAME               37 (admin)
+               552 LOAD_METHOD             40 (route)
+               574 LOAD_CONST              30 ('/progress_summary_ajax')
+               576 PRECALL                  1
+               580 CALL                     1
    
-   143         568 LOAD_CONST              30 (<code object route_progress_summary_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 141>)
-               570 MAKE_FUNCTION            0
+   173         590 LOAD_NAME               23 (verify_admin)
    
-   142         572 PRECALL                  0
-               576 CALL                     0
+   174         592 LOAD_CONST              31 (<code object route_progress_summary_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 172>)
+               594 MAKE_FUNCTION            0
    
-   141         586 PRECALL                  0
-               590 CALL                     0
+   173         596 PRECALL                  0
+               600 CALL                     0
    
-   143         600 STORE_NAME              42 (route_progress_summary_ajax)
+   172         610 PRECALL                  0
+               614 CALL                     0
    
-   149         602 LOAD_NAME               32 (admin)
-               604 LOAD_METHOD             35 (route)
-               626 LOAD_CONST              31 ('/export_item_timing')
-               628 PRECALL                  1
-               632 CALL                     1
+   174         624 STORE_NAME              47 (route_progress_summary_ajax)
    
-   150         642 LOAD_NAME               20 (verify_admin)
+   179         626 LOAD_NAME               37 (admin)
+               628 LOAD_METHOD             48 (post)
+               650 LOAD_CONST              32 ('/update_exclude_from_count')
+               652 PRECALL                  1
+               656 CALL                     1
    
-   151         644 LOAD_CONST              32 (<code object route_export_item_timing, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 149>)
-               646 MAKE_FUNCTION            0
+   180         666 LOAD_CONST              33 (<code object route_update_exclude_from_count, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 179>)
+               668 MAKE_FUNCTION            0
    
-   150         648 PRECALL                  0
-               652 CALL                     0
+   179         670 PRECALL                  0
+               674 CALL                     0
    
-   149         662 PRECALL                  0
-               666 CALL                     0
+   180         684 STORE_NAME              49 (route_update_exclude_from_count)
    
-   151         676 STORE_NAME              43 (route_export_item_timing)
+   190         686 LOAD_NAME               37 (admin)
+               688 LOAD_METHOD             40 (route)
+               710 LOAD_CONST              34 ('/export_item_timing')
+               712 PRECALL                  1
+               716 CALL                     1
    
-   190         678 LOAD_NAME               32 (admin)
-               680 LOAD_METHOD             35 (route)
-               702 LOAD_CONST              33 ('/export')
-               704 PRECALL                  1
-               708 CALL                     1
+   191         726 LOAD_NAME               23 (verify_admin)
    
-   191         718 LOAD_NAME               32 (admin)
-               720 LOAD_METHOD             35 (route)
-               742 LOAD_CONST              34 ('/export/download')
-               744 LOAD_CONST              35 ('route_export_download')
-               746 KW_NAMES                36
-               748 PRECALL                  2
-               752 CALL                     2
+   192         728 LOAD_CONST              35 (<code object route_export_item_timing, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 190>)
+               730 MAKE_FUNCTION            0
    
-   192         762 LOAD_NAME               20 (verify_admin)
+   191         732 PRECALL                  0
+               736 CALL                     0
    
-   193         764 LOAD_CONST              37 (<code object route_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 190>)
-               766 MAKE_FUNCTION            0
+   190         746 PRECALL                  0
+               750 CALL                     0
    
-   192         768 PRECALL                  0
-               772 CALL                     0
+   192         760 STORE_NAME              50 (route_export_item_timing)
    
-   191         782 PRECALL                  0
-               786 CALL                     0
+   231         762 LOAD_NAME               37 (admin)
+               764 LOAD_METHOD             40 (route)
+               786 LOAD_CONST              36 ('/export')
+               788 PRECALL                  1
+               792 CALL                     1
    
-   190         796 PRECALL                  0
-               800 CALL                     0
+   232         802 LOAD_NAME               37 (admin)
+               804 LOAD_METHOD             40 (route)
+               826 LOAD_CONST              37 ('/export/download')
+               828 LOAD_CONST              38 ('route_export_download')
+               830 KW_NAMES                39
+               832 PRECALL                  2
+               836 CALL                     2
    
-   193         810 STORE_NAME              44 (route_export)
+   233         846 LOAD_NAME               23 (verify_admin)
    
-   223         812 LOAD_NAME               32 (admin)
-               814 LOAD_METHOD             35 (route)
-               836 LOAD_CONST              38 ('/results')
-               838 PRECALL                  1
-               842 CALL                     1
+   234         848 LOAD_CONST              40 (<code object route_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 231>)
+               850 MAKE_FUNCTION            0
    
-   224         852 LOAD_NAME               20 (verify_admin)
+   233         852 PRECALL                  0
+               856 CALL                     0
    
-   225         854 LOAD_CONST              39 (<code object route_results, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 223>)
-               856 MAKE_FUNCTION            0
+   232         866 PRECALL                  0
+               870 CALL                     0
    
-   224         858 PRECALL                  0
-               862 CALL                     0
+   231         880 PRECALL                  0
+               884 CALL                     0
    
-   223         872 PRECALL                  0
-               876 CALL                     0
+   234         894 STORE_NAME              51 (route_export)
    
-   225         886 STORE_NAME              45 (route_results)
+   268         896 LOAD_NAME               37 (admin)
+               898 LOAD_METHOD             40 (route)
+               920 LOAD_CONST              41 ('/results')
+               922 PRECALL                  1
+               926 CALL                     1
    
-   241         888 LOAD_NAME               32 (admin)
-               890 LOAD_METHOD             35 (route)
-               912 LOAD_CONST              40 ('/preview_questionnaire/<questionnaireName>')
-               914 PRECALL                  1
-               918 CALL                     1
+   269         936 LOAD_NAME               23 (verify_admin)
    
-   242         928 LOAD_NAME               20 (verify_admin)
+   270         938 LOAD_CONST              42 (<code object route_results, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 268>)
+               940 MAKE_FUNCTION            0
    
-   243         930 LOAD_CONST              41 (<code object route_preview_questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 241>)
-               932 MAKE_FUNCTION            0
+   269         942 PRECALL                  0
+               946 CALL                     0
    
-   242         934 PRECALL                  0
-               938 CALL                     0
+   268         956 PRECALL                  0
+               960 CALL                     0
    
-   241         948 PRECALL                  0
-               952 CALL                     0
+   270         970 STORE_NAME              52 (route_results)
    
-   243         962 STORE_NAME              46 (route_preview_questionnaire)
+   286         972 LOAD_NAME               37 (admin)
+               974 LOAD_METHOD             40 (route)
+               996 LOAD_CONST              43 ('/preview_questionnaire/<questionnaireName>')
+               998 LOAD_CONST              20 ('GET')
+              1000 LOAD_CONST              21 ('POST')
+              1002 BUILD_LIST               2
+              1004 KW_NAMES                22
+              1006 PRECALL                  2
+              1010 CALL                     2
    
-   292         964 LOAD_NAME               32 (admin)
-               966 LOAD_METHOD             35 (route)
-               988 LOAD_CONST              42 ('/questionnaire_html/<questionnaireName>')
-               990 PRECALL                  1
-               994 CALL                     1
+   287        1020 LOAD_NAME               23 (verify_admin)
    
-   293        1004 LOAD_NAME               20 (verify_admin)
+   288        1022 LOAD_CONST              44 (<code object route_preview_questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 286>)
+              1024 MAKE_FUNCTION            0
    
-   294        1006 LOAD_CONST              43 (<code object route_questionnaire_html, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 292>)
-              1008 MAKE_FUNCTION            0
+   287        1026 PRECALL                  0
+              1030 CALL                     0
    
-   293        1010 PRECALL                  0
-              1014 CALL                     0
+   286        1040 PRECALL                  0
+              1044 CALL                     0
    
-   292        1024 PRECALL                  0
-              1028 CALL                     0
+   288        1054 STORE_NAME              53 (route_preview_questionnaire)
    
-   294        1038 STORE_NAME              47 (route_questionnaire_html)
+   349        1056 LOAD_NAME               37 (admin)
+              1058 LOAD_METHOD             40 (route)
+              1080 LOAD_CONST              45 ('/questionnaire_html/<questionnaireName>')
+              1082 PRECALL                  1
+              1086 CALL                     1
    
-   343        1040 LOAD_CONST              44 (<code object table_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 343>)
-              1042 MAKE_FUNCTION            0
-              1044 STORE_NAME              48 (table_data)
+   350        1096 LOAD_NAME               23 (verify_admin)
    
-   364        1046 LOAD_NAME               32 (admin)
-              1048 LOAD_METHOD             35 (route)
-              1070 LOAD_CONST              45 ('/table_view/<tableName>')
-              1072 PRECALL                  1
-              1076 CALL                     1
+   351        1098 LOAD_CONST              46 (<code object route_questionnaire_html, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 349>)
+              1100 MAKE_FUNCTION            0
    
-   365        1086 LOAD_NAME               20 (verify_admin)
+   350        1102 PRECALL                  0
+              1106 CALL                     0
    
-   366        1088 LOAD_CONST              46 (<code object route_table_view, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 364>)
-              1090 MAKE_FUNCTION            0
+   349        1116 PRECALL                  0
+              1120 CALL                     0
    
-   365        1092 PRECALL                  0
-              1096 CALL                     0
+   351        1130 STORE_NAME              54 (route_questionnaire_html)
    
-   364        1106 PRECALL                  0
-              1110 CALL                     0
+   400        1132 LOAD_CONST              47 (<code object table_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 400>)
+              1134 MAKE_FUNCTION            0
+              1136 STORE_NAME              55 (table_data)
    
-   366        1120 STORE_NAME              49 (route_table_view)
+   421        1138 LOAD_NAME               37 (admin)
+              1140 LOAD_METHOD             40 (route)
+              1162 LOAD_CONST              48 ('/table_view/<tableName>')
+              1164 PRECALL                  1
+              1168 CALL                     1
    
-   371        1122 LOAD_NAME               32 (admin)
-              1124 LOAD_METHOD             35 (route)
-              1146 LOAD_CONST              47 ('/table_ajax/<tableName>')
-              1148 PRECALL                  1
-              1152 CALL                     1
+   422        1178 LOAD_NAME               23 (verify_admin)
    
-   372        1162 LOAD_NAME               20 (verify_admin)
+   423        1180 LOAD_CONST              49 (<code object route_table_view, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 421>)
+              1182 MAKE_FUNCTION            0
    
-   373        1164 LOAD_CONST              48 (<code object route_table_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 371>)
-              1166 MAKE_FUNCTION            0
+   422        1184 PRECALL                  0
+              1188 CALL                     0
    
-   372        1168 PRECALL                  0
-              1172 CALL                     0
+   421        1198 PRECALL                  0
+              1202 CALL                     0
    
-   371        1182 PRECALL                  0
-              1186 CALL                     0
+   423        1212 STORE_NAME              56 (route_table_view)
    
-   373        1196 STORE_NAME              50 (route_table_ajax)
+   428        1214 LOAD_NAME               37 (admin)
+              1216 LOAD_METHOD             40 (route)
+              1238 LOAD_CONST              50 ('/table_ajax/<tableName>')
+              1240 PRECALL                  1
+              1244 CALL                     1
    
-   378        1198 LOAD_NAME               32 (admin)
-              1200 LOAD_METHOD             35 (route)
-              1222 LOAD_CONST              49 ('/table_csv/<tableName>')
-              1224 PRECALL                  1
-              1228 CALL                     1
+   429        1254 LOAD_NAME               23 (verify_admin)
    
-   379        1238 LOAD_NAME               20 (verify_admin)
+   430        1256 LOAD_CONST              51 (<code object route_table_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 428>)
+              1258 MAKE_FUNCTION            0
    
-   380        1240 LOAD_CONST              50 (<code object route_table_csv, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 378>)
-              1242 MAKE_FUNCTION            0
+   429        1260 PRECALL                  0
+              1264 CALL                     0
    
-   379        1244 PRECALL                  0
-              1248 CALL                     0
+   428        1274 PRECALL                  0
+              1278 CALL                     0
    
-   378        1258 PRECALL                  0
-              1262 CALL                     0
+   430        1288 STORE_NAME              57 (route_table_ajax)
    
-   380        1272 STORE_NAME              51 (route_table_csv)
+   435        1290 LOAD_NAME               37 (admin)
+              1292 LOAD_METHOD             40 (route)
+              1314 LOAD_CONST              52 ('/table_csv/<tableName>')
+              1316 PRECALL                  1
+              1320 CALL                     1
    
-   397        1274 LOAD_NAME               32 (admin)
-              1276 LOAD_METHOD             52 (errorhandler)
-              1298 LOAD_CONST              51 (500)
-              1300 PRECALL                  1
-              1304 CALL                     1
+   436        1330 LOAD_NAME               23 (verify_admin)
    
-   398        1314 LOAD_CONST              52 (<code object internal_error, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 397>)
-              1316 MAKE_FUNCTION            0
+   437        1332 LOAD_CONST              53 (<code object route_table_csv, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 435>)
+              1334 MAKE_FUNCTION            0
    
-   397        1318 PRECALL                  0
-              1322 CALL                     0
+   436        1336 PRECALL                  0
+              1340 CALL                     0
    
-   398        1332 STORE_NAME              53 (internal_error)
-              1334 LOAD_CONST               1 (None)
-              1336 RETURN_VALUE
+   435        1350 PRECALL                  0
+              1354 CALL                     0
+   
+   437        1364 STORE_NAME              58 (route_table_csv)
+   
+   455        1366 LOAD_NAME               37 (admin)
+              1368 LOAD_METHOD             40 (route)
+              1390 LOAD_CONST              54 ('/database_download')
+              1392 PRECALL                  1
+              1396 CALL                     1
+   
+   456        1406 LOAD_NAME               23 (verify_admin)
+   
+   457        1408 LOAD_CONST              55 (<code object route_database_download, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 455>)
+              1410 MAKE_FUNCTION            0
+   
+   456        1412 PRECALL                  0
+              1416 CALL                     0
+   
+   455        1426 PRECALL                  0
+              1430 CALL                     0
+   
+   457        1440 STORE_NAME              59 (route_database_download)
+   
+   466        1442 LOAD_NAME               37 (admin)
+              1444 LOAD_METHOD             40 (route)
+              1466 LOAD_CONST              56 ('/database_delete')
+              1468 LOAD_CONST              20 ('GET')
+              1470 LOAD_CONST              21 ('POST')
+              1472 BUILD_LIST               2
+              1474 KW_NAMES                22
+              1476 PRECALL                  2
+              1480 CALL                     2
+   
+   467        1490 LOAD_NAME               23 (verify_admin)
+   
+   468        1492 LOAD_CONST              57 (<code object route_database_delete, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 466>)
+              1494 MAKE_FUNCTION            0
+   
+   467        1496 PRECALL                  0
+              1500 CALL                     0
+   
+   466        1510 PRECALL                  0
+              1514 CALL                     0
+   
+   468        1524 STORE_NAME              60 (route_database_delete)
+   
+   492        1526 LOAD_NAME               37 (admin)
+              1528 LOAD_METHOD             61 (errorhandler)
+              1550 LOAD_CONST              58 (500)
+              1552 PRECALL                  1
+              1556 CALL                     1
+   
+   493        1566 LOAD_CONST              59 (<code object internal_error, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 492>)
+              1568 MAKE_FUNCTION            0
+   
+   492        1570 PRECALL                  0
+              1574 CALL                     0
+   
+   493        1584 STORE_NAME              62 (internal_error)
+              1586 LOAD_CONST               1 (None)
+              1588 RETURN_VALUE
    consts
       0
       None
-      ('Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response')
+      ('Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response', 'send_file')
       ('db', 'questionnaires', 'page_list')
-      ('fetch_condition_count', 'display_time')
+      ('fetch_condition_count', 'display_time', 'provide_consent', 'int_or_0')
       1
       ('sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label')
       ('*',)
       ('datetime',)
       ('path', 'listdir')
+      ('copyfile',)
       'admin'
       'templates'
       'static'
       '/admin'
       ('template_folder', 'static_folder', 'url_prefix')
       code
          argcount  : 0
-         nlocals   : 7
-         stacksize : 9
+         nlocals   : 8
+         stacksize : 10
          flags     : 3
          code
             0x970064017400000000000000000000006a010000000000000000760072
             137400000000000000000000006a01000000000000000064011900000000
             00000000007d006e0264027d0067007d017404000000000000000000006a
             0300000000000000006a04000000000000000044005d177d027c01a00500
             000000000000000000000000000000000000007c02a6010000ab01000000
@@ -488,183 +571,200 @@
             00000000000000a6010000ab01000000000000000001008c417419000000
             000000000000007c01a6010000ab0100000000000000007d017400000000
             000000000000006a0d0000000000000000a00e0000000000000000000000
             0000000000000000006406a6010000ab0100000000000000007d05741900
             0000000000000000007400000000000000000000006a0d00000000000000
             00a00e0000000000000000000000000000000000000000a6000000ab0000
             00000000000000a6010000ab0100000000000000007d0674190000000000
-            00000000007c03a6010000ab0100000000000000007d03741f0000000000
-            00000000007c007c017c057c067c037400000000000000000000006a0100
-            000000000000006407190000000000000000007420000000000000000000
-            00ac08a6070000ab0700000000000000005300
-          15           0 RESUME                   0
+            00000000007c03a6010000ab0100000000000000007d0374000000000000
+            00000000006a010000000000000000640719000000000000000000a00f00
+            000000000000000000000000000000000000006408a6010000ab01000000
+            00000000007d077421000000000000000000007c007c017c057c067c0374
+            00000000000000000000006a010000000000000000640919000000000000
+            0000007c07742200000000000000000000ac0aa6080000ab080000000000
+            0000005300
+          16           0 RESUME                   0
          
-          23           2 LOAD_CONST               1 ('ADDITIONAL_ADMIN_PAGES')
+          24           2 LOAD_CONST               1 ('ADDITIONAL_ADMIN_PAGES')
                        4 LOAD_GLOBAL              0 (current_app)
                       16 LOAD_ATTR                1 (config)
                       26 CONTAINS_OP              0
                       28 POP_JUMP_FORWARD_IF_FALSE    19 (to 68)
          
-          24          30 LOAD_GLOBAL              0 (current_app)
+          25          30 LOAD_GLOBAL              0 (current_app)
                       42 LOAD_ATTR                1 (config)
                       52 LOAD_CONST               1 ('ADDITIONAL_ADMIN_PAGES')
                       54 BINARY_SUBSCR
                       64 STORE_FAST               0 (additionalAdminPages)
                       66 JUMP_FORWARD             2 (to 72)
          
-          26     >>   68 LOAD_CONST               2 (None)
+          27     >>   68 LOAD_CONST               2 (None)
                       70 STORE_FAST               0 (additionalAdminPages)
          
-          28     >>   72 BUILD_LIST               0
+          29     >>   72 BUILD_LIST               0
                       74 STORE_FAST               1 (tableNames)
          
-          29          76 LOAD_GLOBAL              4 (db)
+          30          76 LOAD_GLOBAL              4 (db)
                       88 LOAD_ATTR                3 (metadata)
                       98 LOAD_ATTR                4 (tables)
                      108 GET_ITER
                  >>  110 FOR_ITER                23 (to 158)
                      112 STORE_FAST               2 (t)
          
-          30         114 LOAD_FAST                1 (tableNames)
+          31         114 LOAD_FAST                1 (tableNames)
                      116 LOAD_METHOD              5 (append)
                      138 LOAD_FAST                2 (t)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 POP_TOP
                      156 JUMP_BACKWARD           24 (to 110)
          
-          32     >>  158 BUILD_LIST               0
+          33     >>  158 BUILD_LIST               0
                      160 STORE_FAST               3 (questionnairesSystem)
          
-          34         162 LOAD_GLOBAL             13 (NULL + path)
+          35         162 LOAD_GLOBAL             13 (NULL + path)
                      174 LOAD_ATTR                7 (exists)
                      184 LOAD_GLOBAL              0 (current_app)
                      196 LOAD_ATTR                8 (root_path)
                      206 LOAD_CONST               3 ('/questionnaires')
                      208 BINARY_OP                0 (+)
                      212 PRECALL                  1
                      216 CALL                     1
                      226 POP_JUMP_FORWARD_IF_FALSE    93 (to 414)
          
-          35         228 LOAD_GLOBAL             19 (NULL + listdir)
+          36         228 LOAD_GLOBAL             19 (NULL + listdir)
                      240 LOAD_GLOBAL              0 (current_app)
                      252 LOAD_ATTR                8 (root_path)
                      262 LOAD_CONST               3 ('/questionnaires')
                      264 BINARY_OP                0 (+)
                      268 PRECALL                  1
                      272 CALL                     1
                      282 GET_ITER
                  >>  284 FOR_ITER                64 (to 414)
                      286 STORE_FAST               4 (q)
          
-          36         288 LOAD_FAST                4 (q)
+          37         288 LOAD_FAST                4 (q)
                      290 LOAD_METHOD             10 (endswith)
                      312 LOAD_CONST               4 ('.json')
                      314 PRECALL                  1
                      318 CALL                     1
                      328 POP_JUMP_FORWARD_IF_FALSE    41 (to 412)
          
-          37         330 LOAD_FAST                3 (questionnairesSystem)
+          38         330 LOAD_FAST                3 (questionnairesSystem)
                      332 LOAD_METHOD              5 (append)
                      354 LOAD_FAST                4 (q)
                      356 LOAD_METHOD             11 (replace)
                      378 LOAD_CONST               4 ('.json')
                      380 LOAD_CONST               5 ('')
                      382 PRECALL                  2
                      386 CALL                     2
                      396 PRECALL                  1
                      400 CALL                     1
                      410 POP_TOP
                  >>  412 JUMP_BACKWARD           65 (to 284)
          
-          39     >>  414 LOAD_GLOBAL             25 (NULL + sorted)
+          40     >>  414 LOAD_GLOBAL             25 (NULL + sorted)
                      426 LOAD_FAST                1 (tableNames)
                      428 PRECALL                  1
                      432 CALL                     1
                      442 STORE_FAST               1 (tableNames)
          
-          40         444 LOAD_GLOBAL              0 (current_app)
+          41         444 LOAD_GLOBAL              0 (current_app)
                      456 LOAD_ATTR               13 (page_list)
                      466 LOAD_METHOD             14 (get_questionnaire_list)
                      488 LOAD_CONST               6 (True)
                      490 PRECALL                  1
                      494 CALL                     1
                      504 STORE_FAST               5 (questionnairesLive)
          
-          41         506 LOAD_GLOBAL             25 (NULL + sorted)
+          42         506 LOAD_GLOBAL             25 (NULL + sorted)
                      518 LOAD_GLOBAL              0 (current_app)
                      530 LOAD_ATTR               13 (page_list)
                      540 LOAD_METHOD             14 (get_questionnaire_list)
                      562 PRECALL                  0
                      566 CALL                     0
                      576 PRECALL                  1
                      580 CALL                     1
                      590 STORE_FAST               6 (questionnairesLiveUntagged)
          
-          42         592 LOAD_GLOBAL             25 (NULL + sorted)
+          43         592 LOAD_GLOBAL             25 (NULL + sorted)
                      604 LOAD_FAST                3 (questionnairesSystem)
                      606 PRECALL                  1
                      610 CALL                     1
                      620 STORE_FAST               3 (questionnairesSystem)
          
-          44         622 LOAD_GLOBAL             31 (NULL + dict)
+          44         622 LOAD_GLOBAL              0 (current_app)
+                     634 LOAD_ATTR                1 (config)
+                     644 LOAD_CONST               7 ('SQLALCHEMY_DATABASE_URI')
+                     646 BINARY_SUBSCR
+                     656 LOAD_METHOD             15 (startswith)
+                     678 LOAD_CONST               8 ('sqlite:///')
+                     680 PRECALL                  1
+                     684 CALL                     1
+                     694 STORE_FAST               7 (isSqliteDb)
+         
+          47         696 LOAD_GLOBAL             33 (NULL + dict)
          
-          45         634 LOAD_FAST                0 (additionalAdminPages)
+          48         708 LOAD_FAST                0 (additionalAdminPages)
          
-          46         636 LOAD_FAST                1 (tableNames)
+          49         710 LOAD_FAST                1 (tableNames)
          
-          47         638 LOAD_FAST                5 (questionnairesLive)
+          50         712 LOAD_FAST                5 (questionnairesLive)
          
-          48         640 LOAD_FAST                6 (questionnairesLiveUntagged)
+          51         714 LOAD_FAST                6 (questionnairesLiveUntagged)
          
-          49         642 LOAD_FAST                3 (questionnairesSystem)
+          52         716 LOAD_FAST                3 (questionnairesSystem)
          
-          50         644 LOAD_GLOBAL              0 (current_app)
-                     656 LOAD_ATTR                1 (config)
-                     666 LOAD_CONST               7 ('LOG_GRID_CLICKS')
-                     668 BINARY_SUBSCR
+          53         718 LOAD_GLOBAL              0 (current_app)
+                     730 LOAD_ATTR                1 (config)
+                     740 LOAD_CONST               9 ('LOG_GRID_CLICKS')
+                     742 BINARY_SUBSCR
          
-          51         678 LOAD_GLOBAL             32 (condition_num_to_label)
+          54         752 LOAD_FAST                7 (isSqliteDb)
          
-          44         690 KW_NAMES                 8
-                     692 PRECALL                  7
-                     696 CALL                     7
-                     706 RETURN_VALUE
+          55         754 LOAD_GLOBAL             34 (condition_num_to_label)
+         
+          47         766 KW_NAMES                10
+                     768 PRECALL                  8
+                     772 CALL                     8
+                     782 RETURN_VALUE
          consts
             '\n    Inject additional variables into the context of templates within this blueprint\n    See http://flask.pocoo.org/docs/1.0/templating/#context-processors\n    :return:\n    '
             'ADDITIONAL_ADMIN_PAGES'
             None
             '/questionnaires'
             '.json'
             ''
             True
+            'SQLALCHEMY_DATABASE_URI'
+            'sqlite:///'
             'LOG_GRID_CLICKS'
-            ('additionalAdminPages', 'tableNames', 'questionnairesLive', 'questionnairesLiveUntagged', 'questionnairesSystem', 'logGridClicks', 'condition_num_to_label')
-         names      ('current_app', 'config', 'db', 'metadata', 'tables', 'append', 'path', 'exists', 'root_path', 'listdir', 'endswith', 'replace', 'sorted', 'page_list', 'get_questionnaire_list', 'dict', 'condition_num_to_label')
-         varnames   ('additionalAdminPages', 'tableNames', 't', 'questionnairesSystem', 'q', 'questionnairesLive', 'questionnairesLiveUntagged')
+            ('additionalAdminPages', 'tableNames', 'questionnairesLive', 'questionnairesLiveUntagged', 'questionnairesSystem', 'logGridClicks', 'isSqliteDb', 'condition_num_to_label')
+         names      ('current_app', 'config', 'db', 'metadata', 'tables', 'append', 'path', 'exists', 'root_path', 'listdir', 'endswith', 'replace', 'sorted', 'page_list', 'get_questionnaire_list', 'startswith', 'dict', 'condition_num_to_label')
+         varnames   ('additionalAdminPages', 'tableNames', 't', 'questionnairesSystem', 'q', 'questionnairesLive', 'questionnairesLiveUntagged', 'isSqliteDb')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'inject_template_vars'
-         firstlineno 15
+         firstlineno 16
          lnotab
             0x02081c0126020402040126012c02040242013c012a0154021e013e0156
-            011e020c010201020102010201020122010cf9
+            011e014a030c0102010201020102010201220102010cf8
       '/'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007403000000000000000000006401a6
             010000ab010000000000000000a6010000ab0100000000000000005300
-          55           0 RESUME                   0
+          59           0 RESUME                   0
          
-          57           2 LOAD_GLOBAL              1 (NULL + redirect)
+          61           2 LOAD_GLOBAL              1 (NULL + redirect)
                       14 LOAD_GLOBAL              3 (NULL + url_for)
                       26 LOAD_CONST               1 ('admin.admin_login')
                       28 PRECALL                  1
                       32 CALL                     1
                       42 PRECALL                  1
                       46 CALL                     1
                       56 RETURN_VALUE
@@ -673,126 +773,322 @@
             'admin.admin_login'
          names      ('redirect', 'url_for')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'admin_index'
-         firstlineno 55
+         firstlineno 59
          lnotab 0x0202
       '/login'
       'GET'
       'POST'
       ('methods',)
       code
          argcount  : 0
-         nlocals   : 0
-         stacksize : 5
+         nlocals   : 5
+         stacksize : 7
          flags     : 3
          code
-            0x97007401000000000000000000006a01000000000000000064016402a6
-            020000ab020000000000000000721c740500000000000000000000740700
-            0000000000000000006403a6010000ab010000000000000000a6010000ab
-            01000000000000000053007408000000000000000000006a050000000000
-            00000064046b020000000072697408000000000000000000006a06000000
-            0000000000640519000000000000000000740e000000000000000000006a
-            0800000000000000006406190000000000000000006b0300000000721174
-            130000000000000000000064076408ac09a6020000ab0200000000000000
-            005300640a74000000000000000000000064013c000000640a7400000000
-            000000000000005f0a000000000000000074050000000000000000000074
-            07000000000000000000006403a6010000ab010000000000000000a60100
-            00ab01000000000000000053007413000000000000000000006407a60100
-            00ab0100000000000000005300
-          60           0 RESUME                   0
-         
-          62           2 LOAD_GLOBAL              1 (NULL + session)
-                      14 LOAD_ATTR                1 (get)
-                      24 LOAD_CONST               1 ('loggedIn')
-                      26 LOAD_CONST               2 (False)
-                      28 PRECALL                  2
-                      32 CALL                     2
-                      42 POP_JUMP_FORWARD_IF_FALSE    28 (to 100)
-         
-          63          44 LOAD_GLOBAL              5 (NULL + redirect)
-                      56 LOAD_GLOBAL              7 (NULL + url_for)
-                      68 LOAD_CONST               3 ('admin.route_progress')
-                      70 PRECALL                  1
-                      74 CALL                     1
-                      84 PRECALL                  1
-                      88 CALL                     1
-                      98 RETURN_VALUE
-         
-          65     >>  100 LOAD_GLOBAL              8 (request)
-                     112 LOAD_ATTR                5 (method)
-                     122 LOAD_CONST               4 ('POST')
-                     124 COMPARE_OP               2 (==)
-                     130 POP_JUMP_FORWARD_IF_FALSE   105 (to 342)
-         
-          66         132 LOAD_GLOBAL              8 (request)
-                     144 LOAD_ATTR                6 (form)
-                     154 LOAD_CONST               5 ('password')
-                     156 BINARY_SUBSCR
-                     166 LOAD_GLOBAL             14 (current_app)
-                     178 LOAD_ATTR                8 (config)
-                     188 LOAD_CONST               6 ('ADMIN_PASSWORD')
-                     190 BINARY_SUBSCR
-                     200 COMPARE_OP               3 (!=)
-                     206 POP_JUMP_FORWARD_IF_FALSE    17 (to 242)
-         
-          67         208 LOAD_GLOBAL             19 (NULL + render_template)
-                     220 LOAD_CONST               7 ('login_admin.html')
-                     222 LOAD_CONST               8 ('The password you entered is incorrect.')
-                     224 KW_NAMES                 9
-                     226 PRECALL                  2
-                     230 CALL                     2
-                     240 RETURN_VALUE
-         
-          69     >>  242 LOAD_CONST              10 (True)
-                     244 LOAD_GLOBAL              0 (session)
-                     256 LOAD_CONST               1 ('loggedIn')
-                     258 STORE_SUBSCR
-         
-          70         262 LOAD_CONST              10 (True)
-                     264 LOAD_GLOBAL              0 (session)
-                     276 STORE_ATTR              10 (modified)
-         
-          72         286 LOAD_GLOBAL              5 (NULL + redirect)
-                     298 LOAD_GLOBAL              7 (NULL + url_for)
-                     310 LOAD_CONST               3 ('admin.route_progress')
-                     312 PRECALL                  1
-                     316 CALL                     1
-                     326 PRECALL                  1
-                     330 CALL                     1
-                     340 RETURN_VALUE
-         
-          74     >>  342 LOAD_GLOBAL             19 (NULL + render_template)
-                     354 LOAD_CONST               7 ('login_admin.html')
-                     356 PRECALL                  1
-                     360 CALL                     1
-                     370 RETURN_VALUE
+            0x97006401740000000000000000000000760172f9090074030000000000
+            00000000006402a6010000ab0100000000000000007d006ec32300740400
+            000000000000000000240072b67d0164037407000000000000000000007c
+            01a6010000ab0100000000000000007600729e7409000000000000000000
+            006a0500000000000000006404a6010000ab0100000000000000007d0274
+            08000000000000000000006a060000000000000000a00700000000000000
+            00000000000000000000000000a6000000ab00000000000000000035007d
+            037c03a00800000000000000000000000000000000000000007c02a60100
+            00ab01000000000000000001007408000000000000000000006a00000000
+            0000000000a0090000000000000000000000000000000000000000a60000
+            00ab0000000000000000000100640064006400a6020000ab020000000000
+            00000001006e0b2300310073047702780359007701010059000100010074
+            15000000000000000000007417000000000000000000006405a6010000ab
+            010000000000000000a6010000ab0100000000000000006302590064007d
+            017e0153007c01820164007d017e017701770078035900770164027c005f
+            0c00000000000000007408000000000000000000006a0000000000000000
+            00a0090000000000000000000000000000000000000000a6000000ab0000
+            0000000000000001007401000000000000000000006a0d00000000000000
+            0064066407a6020000ab020000000000000000721c741500000000000000
+            0000007417000000000000000000006408a6010000ab0100000000000000
+            00a6010000ab0100000000000000005300741c000000000000000000006a
+            0f000000000000000064096b020000000072c2741c000000000000000000
+            006a100000000000000000640a1900000000000000000074220000000000
+            00000000006a120000000000000000640b190000000000000000006b0300
+            0000007211742700000000000000000000640c640dac0ea6020000ab0200
+            000000000000005300640274000000000000000000000064063c00000064
+            027400000000000000000000005f14000000000000000074170000000000
+            00000000006408a6010000ab0100000000000000007d040900741c000000
+            000000000000006a150000000000000000a00d0000000000000000000000
+            000000000000000000640fa6010000ab010000000000000000812f741700
+            0000000000000000006410741c000000000000000000006a150000000000
+            000000a00d0000000000000000000000000000000000000000640fa60100
+            00ab0100000000000000007a000000a6010000ab0100000000000000007d
+            046e072300010059006e037803590077017415000000000000000000007c
+            04a6010000ab010000000000000000530074270000000000000000000064
+            0ca6010000ab0100000000000000005300
+          64           0 RESUME                   0
+         
+          66           2 LOAD_CONST               1 ('participantID')
+                       4 LOAD_GLOBAL              0 (session)
+                      16 CONTAINS_OP              1
+                      18 POP_JUMP_FORWARD_IF_FALSE   249 (to 518)
+         
+          67          20 NOP
+         
+          68          22 LOAD_GLOBAL              3 (NULL + provide_consent)
+                      34 LOAD_CONST               2 (True)
+                      36 PRECALL                  1
+                      40 CALL                     1
+                      50 STORE_FAST               0 (p)
+                      52 JUMP_FORWARD           195 (to 444)
+                 >>   54 PUSH_EXC_INFO
+         
+          69          56 LOAD_GLOBAL              4 (Exception)
+                      68 CHECK_EXC_MATCH
+                      70 POP_JUMP_FORWARD_IF_FALSE   182 (to 436)
+                      72 STORE_FAST               1 (e)
+         
+          70          74 LOAD_CONST               3 ('table participant has no column named excludeFromCount')
+                      76 LOAD_GLOBAL              7 (NULL + str)
+                      88 LOAD_FAST                1 (e)
+                      90 PRECALL                  1
+                      94 CALL                     1
+                     104 CONTAINS_OP              0
+                     106 POP_JUMP_FORWARD_IF_FALSE   158 (to 424)
+         
+          71         108 LOAD_GLOBAL              9 (NULL + db)
+                     120 LOAD_ATTR                5 (DDL)
+                     130 LOAD_CONST               4 ('ALTER TABLE participant ADD COLUMN excludeFromCount BOOLEAN')
+                     132 PRECALL                  1
+                     136 CALL                     1
+                     146 STORE_FAST               2 (add_column)
+         
+          72         148 LOAD_GLOBAL              8 (db)
+                     160 LOAD_ATTR                6 (engine)
+                     170 LOAD_METHOD              7 (connect)
+                     192 PRECALL                  0
+                     196 CALL                     0
+                     206 BEFORE_WITH
+                     208 STORE_FAST               3 (conn)
+         
+          73         210 LOAD_FAST                3 (conn)
+                     212 LOAD_METHOD              8 (execute)
+                     234 LOAD_FAST                2 (add_column)
+                     236 PRECALL                  1
+                     240 CALL                     1
+                     250 POP_TOP
+         
+          74         252 LOAD_GLOBAL              8 (db)
+                     264 LOAD_ATTR                0 (session)
+                     274 LOAD_METHOD              9 (commit)
+                     296 PRECALL                  0
+                     300 CALL                     0
+                     310 POP_TOP
+         
+          72         312 LOAD_CONST               0 (None)
+                     314 LOAD_CONST               0 (None)
+                     316 LOAD_CONST               0 (None)
+                     318 PRECALL                  2
+                     322 CALL                     2
+                     332 POP_TOP
+                     334 JUMP_FORWARD            11 (to 358)
+                 >>  336 PUSH_EXC_INFO
+                     338 WITH_EXCEPT_START
+                     340 POP_JUMP_FORWARD_IF_TRUE     4 (to 350)
+                     342 RERAISE                  2
+                 >>  344 COPY                     3
+                     346 POP_EXCEPT
+                     348 RERAISE                  1
+                 >>  350 POP_TOP
+                     352 POP_EXCEPT
+                     354 POP_TOP
+                     356 POP_TOP
+         
+          76     >>  358 LOAD_GLOBAL             21 (NULL + redirect)
+                     370 LOAD_GLOBAL             23 (NULL + url_for)
+                     382 LOAD_CONST               5 ('admin.admin_login')
+                     384 PRECALL                  1
+                     388 CALL                     1
+                     398 PRECALL                  1
+                     402 CALL                     1
+                     412 SWAP                     2
+                     414 POP_EXCEPT
+                     416 LOAD_CONST               0 (None)
+                     418 STORE_FAST               1 (e)
+                     420 DELETE_FAST              1 (e)
+                     422 RETURN_VALUE
+         
+          78     >>  424 LOAD_FAST                1 (e)
+                     426 RAISE_VARARGS            1
+                 >>  428 LOAD_CONST               0 (None)
+                     430 STORE_FAST               1 (e)
+                     432 DELETE_FAST              1 (e)
+                     434 RERAISE                  1
+         
+          69     >>  436 RERAISE                  0
+                 >>  438 COPY                     3
+                     440 POP_EXCEPT
+                     442 RERAISE                  1
+         
+          80     >>  444 LOAD_CONST               2 (True)
+                     446 LOAD_FAST                0 (p)
+                     448 STORE_ATTR              12 (excludeFromCount)
+         
+          81         458 LOAD_GLOBAL              8 (db)
+                     470 LOAD_ATTR                0 (session)
+                     480 LOAD_METHOD              9 (commit)
+                     502 PRECALL                  0
+                     506 CALL                     0
+                     516 POP_TOP
+         
+          83     >>  518 LOAD_GLOBAL              1 (NULL + session)
+                     530 LOAD_ATTR               13 (get)
+                     540 LOAD_CONST               6 ('loggedIn')
+                     542 LOAD_CONST               7 (False)
+                     544 PRECALL                  2
+                     548 CALL                     2
+                     558 POP_JUMP_FORWARD_IF_FALSE    28 (to 616)
+         
+          84         560 LOAD_GLOBAL             21 (NULL + redirect)
+                     572 LOAD_GLOBAL             23 (NULL + url_for)
+                     584 LOAD_CONST               8 ('admin.route_progress')
+                     586 PRECALL                  1
+                     590 CALL                     1
+                     600 PRECALL                  1
+                     604 CALL                     1
+                     614 RETURN_VALUE
+         
+          86     >>  616 LOAD_GLOBAL             28 (request)
+                     628 LOAD_ATTR               15 (method)
+                     638 LOAD_CONST               9 ('POST')
+                     640 COMPARE_OP               2 (==)
+                     646 POP_JUMP_FORWARD_IF_FALSE   194 (to 1036)
+         
+          87         648 LOAD_GLOBAL             28 (request)
+                     660 LOAD_ATTR               16 (form)
+                     670 LOAD_CONST              10 ('password')
+                     672 BINARY_SUBSCR
+                     682 LOAD_GLOBAL             34 (current_app)
+                     694 LOAD_ATTR               18 (config)
+                     704 LOAD_CONST              11 ('ADMIN_PASSWORD')
+                     706 BINARY_SUBSCR
+                     716 COMPARE_OP               3 (!=)
+                     722 POP_JUMP_FORWARD_IF_FALSE    17 (to 758)
+         
+          88         724 LOAD_GLOBAL             39 (NULL + render_template)
+                     736 LOAD_CONST              12 ('login_admin.html')
+                     738 LOAD_CONST              13 ('The password you entered is incorrect.')
+                     740 KW_NAMES                14
+                     742 PRECALL                  2
+                     746 CALL                     2
+                     756 RETURN_VALUE
+         
+          90     >>  758 LOAD_CONST               2 (True)
+                     760 LOAD_GLOBAL              0 (session)
+                     772 LOAD_CONST               6 ('loggedIn')
+                     774 STORE_SUBSCR
+         
+          91         778 LOAD_CONST               2 (True)
+                     780 LOAD_GLOBAL              0 (session)
+                     792 STORE_ATTR              20 (modified)
+         
+          93         802 LOAD_GLOBAL             23 (NULL + url_for)
+                     814 LOAD_CONST               8 ('admin.route_progress')
+                     816 PRECALL                  1
+                     820 CALL                     1
+                     830 STORE_FAST               4 (redirect_to)
+         
+          95         832 NOP
+         
+          96         834 LOAD_GLOBAL             28 (request)
+                     846 LOAD_ATTR               21 (args)
+                     856 LOAD_METHOD             13 (get)
+                     878 LOAD_CONST              15 ('r')
+                     880 PRECALL                  1
+                     884 CALL                     1
+                     894 POP_JUMP_FORWARD_IF_NONE    47 (to 990)
+         
+          97         896 LOAD_GLOBAL             23 (NULL + url_for)
+                     908 LOAD_CONST              16 ('admin.')
+                     910 LOAD_GLOBAL             28 (request)
+                     922 LOAD_ATTR               21 (args)
+                     932 LOAD_METHOD             13 (get)
+                     954 LOAD_CONST              15 ('r')
+                     956 PRECALL                  1
+                     960 CALL                     1
+                     970 BINARY_OP                0 (+)
+                     974 PRECALL                  1
+                     978 CALL                     1
+                     988 STORE_FAST               4 (redirect_to)
+                 >>  990 JUMP_FORWARD             7 (to 1006)
+                 >>  992 PUSH_EXC_INFO
+         
+          98         994 POP_TOP
+         
+          99         996 POP_EXCEPT
+                     998 JUMP_FORWARD             3 (to 1006)
+                 >> 1000 COPY                     3
+                    1002 POP_EXCEPT
+                    1004 RERAISE                  1
+         
+         101     >> 1006 LOAD_GLOBAL             21 (NULL + redirect)
+                    1018 LOAD_FAST                4 (redirect_to)
+                    1020 PRECALL                  1
+                    1024 CALL                     1
+                    1034 RETURN_VALUE
+         
+         103     >> 1036 LOAD_GLOBAL             39 (NULL + render_template)
+                    1048 LOAD_CONST              12 ('login_admin.html')
+                    1050 PRECALL                  1
+                    1054 CALL                     1
+                    1064 RETURN_VALUE
+         ExceptionTable:
+           22 to 50 -> 54 [0]
+           54 to 72 -> 438 [1] lasti
+           74 to 206 -> 428 [1] lasti
+           208 to 310 -> 336 [2] lasti
+           312 to 334 -> 428 [1] lasti
+           336 to 342 -> 344 [4] lasti
+           344 to 348 -> 428 [1] lasti
+           350 to 350 -> 344 [4] lasti
+           352 to 410 -> 428 [1] lasti
+           412 to 412 -> 438 [1] lasti
+           424 to 426 -> 428 [1] lasti
+           428 to 436 -> 438 [1] lasti
+           834 to 988 -> 992 [0]
+           992 to 994 -> 1000 [1] lasti
          consts
             None
+            'participantID'
+            True
+            'table participant has no column named excludeFromCount'
+            'ALTER TABLE participant ADD COLUMN excludeFromCount BOOLEAN'
+            'admin.admin_login'
             'loggedIn'
             False
             'admin.route_progress'
             'POST'
             'password'
             'ADMIN_PASSWORD'
             'login_admin.html'
             'The password you entered is incorrect.'
             ('message',)
-            True
-         names      ('session', 'get', 'redirect', 'url_for', 'request', 'method', 'form', 'current_app', 'config', 'render_template', 'modified')
-         varnames   ()
+            'r'
+            'admin.'
+         names      ('session', 'provide_consent', 'Exception', 'str', 'db', 'DDL', 'engine', 'connect', 'execute', 'commit', 'redirect', 'url_for', 'excludeFromCount', 'get', 'request', 'method', 'form', 'current_app', 'config', 'render_template', 'modified', 'args')
+         varnames   ('p', 'e', 'add_column', 'conn', 'redirect_to')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'admin_login'
-         firstlineno 60
-         lnotab 0x02022a01380220014c012202140118023802
+         firstlineno 64
+         lnotab
+            0x02021201020122011201220128013e012a013cfe2e0442020cf7080b0e
+            013c022a01380220014c012202140118021e0202013e01620102010a021e
+            02
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 10
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
@@ -810,129 +1106,129 @@
             0000007406000000000000000000006a0600000000000000006a0c000000
             00000000006b02000000007c036a0d00000000000000007c026401190000
             000000000000006b0200000000a6020000ab020000000000000000a60200
             00ab020000000000000000a00e0000000000000000000000000000000000
             0000007c03a6010000ab0100000000000000007d018c8c7c01a00f000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             007d017c007c0166025300
-          77           0 RESUME                   0
+         106           0 RESUME                   0
          
-          78           2 LOAD_GLOBAL              0 (current_app)
+         107           2 LOAD_GLOBAL              0 (current_app)
                       14 LOAD_ATTR                1 (page_list)
                       24 LOAD_METHOD              2 (flat_page_list)
                       46 PRECALL                  0
                       50 CALL                     0
                       60 STORE_FAST               0 (pages)
          
-          80          62 LOAD_GLOBAL              6 (db)
+         109          62 LOAD_GLOBAL              6 (db)
                       74 LOAD_ATTR                4 (session)
                       84 LOAD_METHOD              5 (query)
                      106 LOAD_GLOBAL              6 (db)
                      118 LOAD_ATTR                6 (Participant)
                      128 PRECALL                  1
                      132 CALL                     1
                      142 STORE_FAST               1 (progress)
          
-          82         144 LOAD_FAST                0 (pages)
+         111         144 LOAD_FAST                0 (pages)
                      146 GET_ITER
                  >>  148 FOR_ITER                34 (to 218)
                      150 STORE_FAST               2 (page)
          
-          83         152 LOAD_FAST                2 (page)
+         112         152 LOAD_FAST                2 (page)
                      154 LOAD_CONST               1 ('path')
                      156 BINARY_SUBSCR
                      166 LOAD_CONST               2 (('end', 'consent'))
                      168 CONTAINS_OP              0
                      170 POP_JUMP_FORWARD_IF_FALSE    22 (to 216)
          
-          84         172 LOAD_FAST                0 (pages)
+         113         172 LOAD_FAST                0 (pages)
                      174 LOAD_METHOD              7 (remove)
                      196 LOAD_FAST                2 (page)
                      198 PRECALL                  1
                      202 CALL                     1
                      212 POP_TOP
          
-          85         214 JUMP_BACKWARD           34 (to 148)
+         114         214 JUMP_BACKWARD           34 (to 148)
          
-          83     >>  216 JUMP_BACKWARD           35 (to 148)
+         112     >>  216 JUMP_BACKWARD           35 (to 148)
          
-          87     >>  218 LOAD_FAST                0 (pages)
+         116     >>  218 LOAD_FAST                0 (pages)
                      220 GET_ITER
                  >>  222 FOR_ITER               139 (to 502)
                      224 STORE_FAST               2 (page)
          
-          88         226 LOAD_GLOBAL              7 (NULL + db)
+         117         226 LOAD_GLOBAL              7 (NULL + db)
                      238 LOAD_ATTR                8 (aliased)
                      248 LOAD_GLOBAL              6 (db)
                      260 LOAD_ATTR                9 (Progress)
                      270 LOAD_FAST                2 (page)
                      272 LOAD_CONST               1 ('path')
                      274 BINARY_SUBSCR
                      284 KW_NAMES                 3
                      286 PRECALL                  2
                      290 CALL                     2
                      300 STORE_FAST               3 (pp)
          
-          89         302 LOAD_FAST                1 (progress)
+         118         302 LOAD_FAST                1 (progress)
                      304 LOAD_METHOD             10 (outerjoin)
                      326 LOAD_FAST                3 (pp)
                      328 LOAD_GLOBAL              7 (NULL + db)
                      340 LOAD_ATTR               11 (and_)
          
-          90         350 LOAD_FAST                3 (pp)
+         119         350 LOAD_FAST                3 (pp)
                      352 LOAD_ATTR               12 (participantID)
                      362 LOAD_GLOBAL              6 (db)
                      374 LOAD_ATTR                6 (Participant)
                      384 LOAD_ATTR               12 (participantID)
                      394 COMPARE_OP               2 (==)
          
-          91         400 LOAD_FAST                3 (pp)
+         120         400 LOAD_FAST                3 (pp)
                      402 LOAD_ATTR               13 (path)
                      412 LOAD_FAST                2 (page)
                      414 LOAD_CONST               1 ('path')
                      416 BINARY_SUBSCR
                      426 COMPARE_OP               2 (==)
          
-          89         432 PRECALL                  2
+         118         432 PRECALL                  2
                      436 CALL                     2
                      446 PRECALL                  2
                      450 CALL                     2
          
-          92         460 LOAD_METHOD             14 (add_entity)
+         121         460 LOAD_METHOD             14 (add_entity)
          
-          93         482 LOAD_FAST                3 (pp)
+         122         482 LOAD_FAST                3 (pp)
          
-          92         484 PRECALL                  1
+         121         484 PRECALL                  1
                      488 CALL                     1
          
-          89         498 STORE_FAST               1 (progress)
+         118         498 STORE_FAST               1 (progress)
                      500 JUMP_BACKWARD          140 (to 222)
          
-          96     >>  502 LOAD_FAST                1 (progress)
+         125     >>  502 LOAD_FAST                1 (progress)
                      504 LOAD_METHOD             15 (all)
                      526 PRECALL                  0
                      530 CALL                     0
                      540 STORE_FAST               1 (progress)
          
-          97         542 LOAD_FAST                0 (pages)
+         126         542 LOAD_FAST                0 (pages)
                      544 LOAD_FAST                1 (progress)
                      546 BUILD_TUPLE              2
                      548 RETURN_VALUE
          consts
             None
             'path'
             ('end', 'consent')
             ('name',)
          names      ('current_app', 'page_list', 'flat_page_list', 'db', 'session', 'query', 'Participant', 'remove', 'aliased', 'Progress', 'outerjoin', 'and_', 'participantID', 'path', 'add_entity', 'all')
          varnames   ('pages', 'progress', 'page', 'pp')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'fetch_progress'
-         firstlineno 77
+         firstlineno 106
          lnotab
             0x02013c025202080114012a0102fe020408014c013001320120fe1c0316
             0102ff0efd04072801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 12
@@ -965,80 +1261,90 @@
             00000000000000a008000000000000000000000000000000000000000064
             04a6010000ab0100000000000000007400000000000000000000006a0500
             00000000000000a00f000000000000000000000000000000000000000074
             00000000000000000000006a0300000000000000006a1000000000000000
             00a6010000ab010000000000000000a00800000000000000000000000000
             000000000000006405a6010000ab010000000000000000a6060000ab0600
             00000000000000a011000000000000000000000000000000000000000074
-            00000000000000000000006a0300000000000000006a0400000000000000
-            00a6010000ab010000000000000000a01200000000000000000000000000
-            00000000000000a6000000ab0000000000000000007d0074000000000000
-            00000000006a010000000000000000a00200000000000000000000000000
-            000000000000007400000000000000000000006a050000000000000000a0
-            060000000000000000000000000000000000000000740000000000000000
-            0000006a0300000000000000006a070000000000000000a6010000ab0100
-            00000000000000a008000000000000000000000000000000000000000064
-            01a6010000ab0100000000000000007400000000000000000000006a0500
-            00000000000000a009000000000000000000000000000000000000000074
-            01000000000000000000006a0a0000000000000000740000000000000000
-            0000006a0300000000000000006a0b000000000000000074000000000000
-            00000000006a0c0000000000000000a6020000ab020000000000000000a6
-            010000ab010000000000000000a008000000000000000000000000000000
-            00000000006402a6010000ab010000000000000000740000000000000000
-            0000006a050000000000000000a009000000000000000000000000000000
-            00000000007401000000000000000000006a0a0000000000000000740000
-            0000000000000000006a0300000000000000006a0d000000000000000074
-            00000000000000000000006a0c0000000000000000a6020000ab02000000
-            0000000000a6010000ab010000000000000000a008000000000000000000
-            00000000000000000000006403a6010000ab010000000000000000740000
-            0000000000000000006a050000000000000000a009000000000000000000
-            00000000000000000000007401000000000000000000006a0a0000000000
-            0000007400000000000000000000006a0300000000000000006a0e000000
-            00000000007400000000000000000000006a0c0000000000000000a60200
-            00ab020000000000000000a6010000ab010000000000000000a008000000
-            00000000000000000000000000000000006404a6010000ab010000000000
-            0000007400000000000000000000006a050000000000000000a013000000
+            01000000000000000000006a120000000000000000740000000000000000
+            0000006a0300000000000000006a1300000000000000000f007400000000
+            000000000000006a0300000000000000006a13000000000000000064006b
+            0200000000a6020000ab020000000000000000a6010000ab010000000000
+            000000a01400000000000000000000000000000000000000007400000000
+            000000000000006a0300000000000000006a040000000000000000a60100
+            00ab010000000000000000a0150000000000000000000000000000000000
+            000000a6000000ab0000000000000000007d007400000000000000000000
+            006a010000000000000000a0020000000000000000000000000000000000
+            0000007400000000000000000000006a050000000000000000a006000000
             00000000000000000000000000000000007400000000000000000000006a
-            0300000000000000006a100000000000000000a6010000ab010000000000
-            000000a00800000000000000000000000000000000000000006406a60100
+            0300000000000000006a070000000000000000a6010000ab010000000000
+            000000a00800000000000000000000000000000000000000006401a60100
             00ab0100000000000000007400000000000000000000006a050000000000
-            000000a01400000000000000000000000000000000000000007400000000
-            000000000000006a0300000000000000006a100000000000000000a60100
-            00ab010000000000000000a0080000000000000000000000000000000000
-            0000006407a6010000ab0100000000000000007400000000000000000000
-            006a050000000000000000a00f0000000000000000000000000000000000
-            0000007400000000000000000000006a0300000000000000006a10000000
-            0000000000a6010000ab010000000000000000a008000000000000000000
-            00000000000000000000006408a6010000ab010000000000000000a60700
-            00ab070000000000000000a0150000000000000000000000000000000000
-            000000a6000000ab0000000000000000007d017c007c0166025300
-         100           0 RESUME                   0
+            000000a00900000000000000000000000000000000000000007401000000
+            000000000000006a0a00000000000000007400000000000000000000006a
+            0300000000000000006a0b00000000000000007400000000000000000000
+            006a0c0000000000000000a6020000ab020000000000000000a6010000ab
+            010000000000000000a00800000000000000000000000000000000000000
+            006402a6010000ab0100000000000000007400000000000000000000006a
+            050000000000000000a00900000000000000000000000000000000000000
+            007401000000000000000000006a0a000000000000000074000000000000
+            00000000006a0300000000000000006a0d00000000000000007400000000
+            000000000000006a0c0000000000000000a6020000ab0200000000000000
+            00a6010000ab010000000000000000a00800000000000000000000000000
+            000000000000006403a6010000ab01000000000000000074000000000000
+            00000000006a050000000000000000a00900000000000000000000000000
+            000000000000007401000000000000000000006a0a000000000000000074
+            00000000000000000000006a0300000000000000006a0e00000000000000
+            007400000000000000000000006a0c0000000000000000a6020000ab0200
+            00000000000000a6010000ab010000000000000000a00800000000000000
+            000000000000000000000000006404a6010000ab01000000000000000074
+            00000000000000000000006a050000000000000000a01600000000000000
+            000000000000000000000000007400000000000000000000006a03000000
+            00000000006a100000000000000000a6010000ab010000000000000000a0
+            0800000000000000000000000000000000000000006406a6010000ab0100
+            000000000000007400000000000000000000006a050000000000000000a0
+            170000000000000000000000000000000000000000740000000000000000
+            0000006a0300000000000000006a100000000000000000a6010000ab0100
+            00000000000000a008000000000000000000000000000000000000000064
+            07a6010000ab0100000000000000007400000000000000000000006a0500
+            00000000000000a00f000000000000000000000000000000000000000074
+            00000000000000000000006a0300000000000000006a1000000000000000
+            00a6010000ab010000000000000000a00800000000000000000000000000
+            000000000000006408a6010000ab010000000000000000a6070000ab0700
+            00000000000000a011000000000000000000000000000000000000000074
+            01000000000000000000006a120000000000000000740000000000000000
+            0000006a0300000000000000006a1300000000000000000f007400000000
+            000000000000006a0300000000000000006a13000000000000000064006b
+            0200000000a6020000ab020000000000000000a6010000ab010000000000
+            000000a0180000000000000000000000000000000000000000a6000000ab
+            0000000000000000007d017c007c0166025300
+         129           0 RESUME                   0
          
-         101           2 LOAD_GLOBAL              0 (db)
+         130           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_ATTR                1 (session)
                       24 LOAD_METHOD              2 (query)
          
-         102          46 LOAD_GLOBAL              0 (db)
+         131          46 LOAD_GLOBAL              0 (db)
                       58 LOAD_ATTR                3 (Participant)
                       68 LOAD_ATTR                4 (condition)
          
-         103          78 LOAD_GLOBAL              0 (db)
+         132          78 LOAD_GLOBAL              0 (db)
                       90 LOAD_ATTR                5 (func)
                      100 LOAD_METHOD              6 (count)
                      122 LOAD_GLOBAL              0 (db)
                      134 LOAD_ATTR                3 (Participant)
                      144 LOAD_ATTR                7 (participantID)
                      154 PRECALL                  1
                      158 CALL                     1
                      168 LOAD_METHOD              8 (label)
                      190 LOAD_CONST               1 ('count')
                      192 PRECALL                  1
                      196 CALL                     1
          
-         104         206 LOAD_GLOBAL              0 (db)
+         133         206 LOAD_GLOBAL              0 (db)
                      218 LOAD_ATTR                5 (func)
                      228 LOAD_METHOD              9 (sum)
                      250 LOAD_GLOBAL              1 (NULL + db)
                      262 LOAD_ATTR               10 (cast)
                      272 LOAD_GLOBAL              0 (db)
                      284 LOAD_ATTR                3 (Participant)
                      294 LOAD_ATTR               11 (is_abandoned)
@@ -1049,15 +1355,15 @@
                      340 PRECALL                  1
                      344 CALL                     1
                      354 LOAD_METHOD              8 (label)
                      376 LOAD_CONST               2 ('countAbandoned')
                      378 PRECALL                  1
                      382 CALL                     1
          
-         105         392 LOAD_GLOBAL              0 (db)
+         134         392 LOAD_GLOBAL              0 (db)
                      404 LOAD_ATTR                5 (func)
                      414 LOAD_METHOD              9 (sum)
                      436 LOAD_GLOBAL              1 (NULL + db)
                      448 LOAD_ATTR               10 (cast)
                      458 LOAD_GLOBAL              0 (db)
                      470 LOAD_ATTR                3 (Participant)
                      480 LOAD_ATTR               13 (is_in_progress)
@@ -1068,15 +1374,15 @@
                      526 PRECALL                  1
                      530 CALL                     1
                      540 LOAD_METHOD              8 (label)
                      562 LOAD_CONST               3 ('countInProgress')
                      564 PRECALL                  1
                      568 CALL                     1
          
-         106         578 LOAD_GLOBAL              0 (db)
+         135         578 LOAD_GLOBAL              0 (db)
                      590 LOAD_ATTR                5 (func)
                      600 LOAD_METHOD              9 (sum)
                      622 LOAD_GLOBAL              1 (NULL + db)
                      634 LOAD_ATTR               10 (cast)
                      644 LOAD_GLOBAL              0 (db)
                      656 LOAD_ATTR                3 (Participant)
                      666 LOAD_ATTR               14 (finished)
@@ -1087,262 +1393,296 @@
                      712 PRECALL                  1
                      716 CALL                     1
                      726 LOAD_METHOD              8 (label)
                      748 LOAD_CONST               4 ('countFinished')
                      750 PRECALL                  1
                      754 CALL                     1
          
-         107         764 LOAD_GLOBAL              0 (db)
+         136         764 LOAD_GLOBAL              0 (db)
                      776 LOAD_ATTR                5 (func)
                      786 LOAD_METHOD             15 (avg)
                      808 LOAD_GLOBAL              0 (db)
                      820 LOAD_ATTR                3 (Participant)
                      830 LOAD_ATTR               16 (duration)
                      840 PRECALL                  1
                      844 CALL                     1
                      854 LOAD_METHOD              8 (label)
                      876 LOAD_CONST               5 ('minutes')
                      878 PRECALL                  1
                      882 CALL                     1
          
-         101         892 PRECALL                  6
+         130         892 PRECALL                  6
                      896 CALL                     6
          
-         108         906 LOAD_METHOD             17 (group_by)
-                     928 LOAD_GLOBAL              0 (db)
-                     940 LOAD_ATTR                3 (Participant)
-                     950 LOAD_ATTR                4 (condition)
-                     960 PRECALL                  1
-                     964 CALL                     1
-                     974 LOAD_METHOD             18 (all)
-                     996 PRECALL                  0
-                    1000 CALL                     0
-         
-         101        1010 STORE_FAST               0 (summary_groups)
-         
-         110        1012 LOAD_GLOBAL              0 (db)
-                    1024 LOAD_ATTR                1 (session)
-                    1034 LOAD_METHOD              2 (query)
-         
-         111        1056 LOAD_GLOBAL              0 (db)
-                    1068 LOAD_ATTR                5 (func)
-                    1078 LOAD_METHOD              6 (count)
-                    1100 LOAD_GLOBAL              0 (db)
-                    1112 LOAD_ATTR                3 (Participant)
-                    1122 LOAD_ATTR                7 (participantID)
-                    1132 PRECALL                  1
-                    1136 CALL                     1
-                    1146 LOAD_METHOD              8 (label)
-                    1168 LOAD_CONST               1 ('count')
-                    1170 PRECALL                  1
-                    1174 CALL                     1
-         
-         112        1184 LOAD_GLOBAL              0 (db)
-                    1196 LOAD_ATTR                5 (func)
-                    1206 LOAD_METHOD              9 (sum)
-                    1228 LOAD_GLOBAL              1 (NULL + db)
-                    1240 LOAD_ATTR               10 (cast)
-                    1250 LOAD_GLOBAL              0 (db)
-                    1262 LOAD_ATTR                3 (Participant)
-                    1272 LOAD_ATTR               11 (is_abandoned)
-                    1282 LOAD_GLOBAL              0 (db)
-                    1294 LOAD_ATTR               12 (Integer)
-                    1304 PRECALL                  2
-                    1308 CALL                     2
-                    1318 PRECALL                  1
-                    1322 CALL                     1
-                    1332 LOAD_METHOD              8 (label)
-                    1354 LOAD_CONST               2 ('countAbandoned')
-                    1356 PRECALL                  1
-                    1360 CALL                     1
-         
-         113        1370 LOAD_GLOBAL              0 (db)
-                    1382 LOAD_ATTR                5 (func)
-                    1392 LOAD_METHOD              9 (sum)
-                    1414 LOAD_GLOBAL              1 (NULL + db)
-                    1426 LOAD_ATTR               10 (cast)
-                    1436 LOAD_GLOBAL              0 (db)
-                    1448 LOAD_ATTR                3 (Participant)
-                    1458 LOAD_ATTR               13 (is_in_progress)
-                    1468 LOAD_GLOBAL              0 (db)
-                    1480 LOAD_ATTR               12 (Integer)
-                    1490 PRECALL                  2
-                    1494 CALL                     2
-                    1504 PRECALL                  1
-                    1508 CALL                     1
-                    1518 LOAD_METHOD              8 (label)
-                    1540 LOAD_CONST               3 ('countInProgress')
-                    1542 PRECALL                  1
-                    1546 CALL                     1
-         
-         114        1556 LOAD_GLOBAL              0 (db)
-                    1568 LOAD_ATTR                5 (func)
-                    1578 LOAD_METHOD              9 (sum)
-                    1600 LOAD_GLOBAL              1 (NULL + db)
-                    1612 LOAD_ATTR               10 (cast)
-                    1622 LOAD_GLOBAL              0 (db)
-                    1634 LOAD_ATTR                3 (Participant)
-                    1644 LOAD_ATTR               14 (finished)
-                    1654 LOAD_GLOBAL              0 (db)
-                    1666 LOAD_ATTR               12 (Integer)
-                    1676 PRECALL                  2
-                    1680 CALL                     2
-                    1690 PRECALL                  1
-                    1694 CALL                     1
-                    1704 LOAD_METHOD              8 (label)
-                    1726 LOAD_CONST               4 ('countFinished')
-                    1728 PRECALL                  1
-                    1732 CALL                     1
-         
-         115        1742 LOAD_GLOBAL              0 (db)
-                    1754 LOAD_ATTR                5 (func)
-                    1764 LOAD_METHOD             19 (min)
-                    1786 LOAD_GLOBAL              0 (db)
-                    1798 LOAD_ATTR                3 (Participant)
-                    1808 LOAD_ATTR               16 (duration)
-                    1818 PRECALL                  1
-                    1822 CALL                     1
-                    1832 LOAD_METHOD              8 (label)
-                    1854 LOAD_CONST               6 ('minSeconds')
-                    1856 PRECALL                  1
-                    1860 CALL                     1
-         
-         116        1870 LOAD_GLOBAL              0 (db)
-                    1882 LOAD_ATTR                5 (func)
-                    1892 LOAD_METHOD             20 (max)
-                    1914 LOAD_GLOBAL              0 (db)
-                    1926 LOAD_ATTR                3 (Participant)
-                    1936 LOAD_ATTR               16 (duration)
-                    1946 PRECALL                  1
-                    1950 CALL                     1
-                    1960 LOAD_METHOD              8 (label)
-                    1982 LOAD_CONST               7 ('maxSeconds')
-                    1984 PRECALL                  1
-                    1988 CALL                     1
-         
-         117        1998 LOAD_GLOBAL              0 (db)
-                    2010 LOAD_ATTR                5 (func)
-                    2020 LOAD_METHOD             15 (avg)
-                    2042 LOAD_GLOBAL              0 (db)
-                    2054 LOAD_ATTR                3 (Participant)
-                    2064 LOAD_ATTR               16 (duration)
-                    2074 PRECALL                  1
-                    2078 CALL                     1
-                    2088 LOAD_METHOD              8 (label)
-                    2110 LOAD_CONST               8 ('seconds')
-                    2112 PRECALL                  1
-                    2116 CALL                     1
-         
-         110        2126 PRECALL                  7
-                    2130 CALL                     7
-         
-         118        2140 LOAD_METHOD             21 (one)
-                    2162 PRECALL                  0
-                    2166 CALL                     0
-         
-         110        2176 STORE_FAST               1 (summary)
-         
-         120        2178 LOAD_FAST                0 (summary_groups)
-                    2180 LOAD_FAST                1 (summary)
-                    2182 BUILD_TUPLE              2
-                    2184 RETURN_VALUE
+         137         906 LOAD_METHOD             17 (filter)
+                     928 LOAD_GLOBAL              1 (NULL + db)
+                     940 LOAD_ATTR               18 (or_)
+                     950 LOAD_GLOBAL              0 (db)
+                     962 LOAD_ATTR                3 (Participant)
+                     972 LOAD_ATTR               19 (excludeFromCount)
+                     982 UNARY_INVERT
+                     984 LOAD_GLOBAL              0 (db)
+                     996 LOAD_ATTR                3 (Participant)
+                    1006 LOAD_ATTR               19 (excludeFromCount)
+                    1016 LOAD_CONST               0 (None)
+                    1018 COMPARE_OP               2 (==)
+                    1024 PRECALL                  2
+                    1028 CALL                     2
+                    1038 PRECALL                  1
+                    1042 CALL                     1
+         
+         138        1052 LOAD_METHOD             20 (group_by)
+                    1074 LOAD_GLOBAL              0 (db)
+                    1086 LOAD_ATTR                3 (Participant)
+                    1096 LOAD_ATTR                4 (condition)
+                    1106 PRECALL                  1
+                    1110 CALL                     1
+                    1120 LOAD_METHOD             21 (all)
+                    1142 PRECALL                  0
+                    1146 CALL                     0
+         
+         130        1156 STORE_FAST               0 (summary_groups)
+         
+         140        1158 LOAD_GLOBAL              0 (db)
+                    1170 LOAD_ATTR                1 (session)
+                    1180 LOAD_METHOD              2 (query)
+         
+         141        1202 LOAD_GLOBAL              0 (db)
+                    1214 LOAD_ATTR                5 (func)
+                    1224 LOAD_METHOD              6 (count)
+                    1246 LOAD_GLOBAL              0 (db)
+                    1258 LOAD_ATTR                3 (Participant)
+                    1268 LOAD_ATTR                7 (participantID)
+                    1278 PRECALL                  1
+                    1282 CALL                     1
+                    1292 LOAD_METHOD              8 (label)
+                    1314 LOAD_CONST               1 ('count')
+                    1316 PRECALL                  1
+                    1320 CALL                     1
+         
+         142        1330 LOAD_GLOBAL              0 (db)
+                    1342 LOAD_ATTR                5 (func)
+                    1352 LOAD_METHOD              9 (sum)
+                    1374 LOAD_GLOBAL              1 (NULL + db)
+                    1386 LOAD_ATTR               10 (cast)
+                    1396 LOAD_GLOBAL              0 (db)
+                    1408 LOAD_ATTR                3 (Participant)
+                    1418 LOAD_ATTR               11 (is_abandoned)
+                    1428 LOAD_GLOBAL              0 (db)
+                    1440 LOAD_ATTR               12 (Integer)
+                    1450 PRECALL                  2
+                    1454 CALL                     2
+                    1464 PRECALL                  1
+                    1468 CALL                     1
+                    1478 LOAD_METHOD              8 (label)
+                    1500 LOAD_CONST               2 ('countAbandoned')
+                    1502 PRECALL                  1
+                    1506 CALL                     1
+         
+         143        1516 LOAD_GLOBAL              0 (db)
+                    1528 LOAD_ATTR                5 (func)
+                    1538 LOAD_METHOD              9 (sum)
+                    1560 LOAD_GLOBAL              1 (NULL + db)
+                    1572 LOAD_ATTR               10 (cast)
+                    1582 LOAD_GLOBAL              0 (db)
+                    1594 LOAD_ATTR                3 (Participant)
+                    1604 LOAD_ATTR               13 (is_in_progress)
+                    1614 LOAD_GLOBAL              0 (db)
+                    1626 LOAD_ATTR               12 (Integer)
+                    1636 PRECALL                  2
+                    1640 CALL                     2
+                    1650 PRECALL                  1
+                    1654 CALL                     1
+                    1664 LOAD_METHOD              8 (label)
+                    1686 LOAD_CONST               3 ('countInProgress')
+                    1688 PRECALL                  1
+                    1692 CALL                     1
+         
+         144        1702 LOAD_GLOBAL              0 (db)
+                    1714 LOAD_ATTR                5 (func)
+                    1724 LOAD_METHOD              9 (sum)
+                    1746 LOAD_GLOBAL              1 (NULL + db)
+                    1758 LOAD_ATTR               10 (cast)
+                    1768 LOAD_GLOBAL              0 (db)
+                    1780 LOAD_ATTR                3 (Participant)
+                    1790 LOAD_ATTR               14 (finished)
+                    1800 LOAD_GLOBAL              0 (db)
+                    1812 LOAD_ATTR               12 (Integer)
+                    1822 PRECALL                  2
+                    1826 CALL                     2
+                    1836 PRECALL                  1
+                    1840 CALL                     1
+                    1850 LOAD_METHOD              8 (label)
+                    1872 LOAD_CONST               4 ('countFinished')
+                    1874 PRECALL                  1
+                    1878 CALL                     1
+         
+         145        1888 LOAD_GLOBAL              0 (db)
+                    1900 LOAD_ATTR                5 (func)
+                    1910 LOAD_METHOD             22 (min)
+                    1932 LOAD_GLOBAL              0 (db)
+                    1944 LOAD_ATTR                3 (Participant)
+                    1954 LOAD_ATTR               16 (duration)
+                    1964 PRECALL                  1
+                    1968 CALL                     1
+                    1978 LOAD_METHOD              8 (label)
+                    2000 LOAD_CONST               6 ('minSeconds')
+                    2002 PRECALL                  1
+                    2006 CALL                     1
+         
+         146        2016 LOAD_GLOBAL              0 (db)
+                    2028 LOAD_ATTR                5 (func)
+                    2038 LOAD_METHOD             23 (max)
+                    2060 LOAD_GLOBAL              0 (db)
+                    2072 LOAD_ATTR                3 (Participant)
+                    2082 LOAD_ATTR               16 (duration)
+                    2092 PRECALL                  1
+                    2096 CALL                     1
+                    2106 LOAD_METHOD              8 (label)
+                    2128 LOAD_CONST               7 ('maxSeconds')
+                    2130 PRECALL                  1
+                    2134 CALL                     1
+         
+         147        2144 LOAD_GLOBAL              0 (db)
+                    2156 LOAD_ATTR                5 (func)
+                    2166 LOAD_METHOD             15 (avg)
+                    2188 LOAD_GLOBAL              0 (db)
+                    2200 LOAD_ATTR                3 (Participant)
+                    2210 LOAD_ATTR               16 (duration)
+                    2220 PRECALL                  1
+                    2224 CALL                     1
+                    2234 LOAD_METHOD              8 (label)
+                    2256 LOAD_CONST               8 ('seconds')
+                    2258 PRECALL                  1
+                    2262 CALL                     1
+         
+         140        2272 PRECALL                  7
+                    2276 CALL                     7
+         
+         148        2286 LOAD_METHOD             17 (filter)
+                    2308 LOAD_GLOBAL              1 (NULL + db)
+                    2320 LOAD_ATTR               18 (or_)
+                    2330 LOAD_GLOBAL              0 (db)
+                    2342 LOAD_ATTR                3 (Participant)
+                    2352 LOAD_ATTR               19 (excludeFromCount)
+                    2362 UNARY_INVERT
+                    2364 LOAD_GLOBAL              0 (db)
+                    2376 LOAD_ATTR                3 (Participant)
+                    2386 LOAD_ATTR               19 (excludeFromCount)
+                    2396 LOAD_CONST               0 (None)
+                    2398 COMPARE_OP               2 (==)
+                    2404 PRECALL                  2
+                    2408 CALL                     2
+                    2418 PRECALL                  1
+                    2422 CALL                     1
+         
+         149        2432 LOAD_METHOD             24 (one)
+                    2454 PRECALL                  0
+                    2458 CALL                     0
+         
+         140        2468 STORE_FAST               1 (summary)
+         
+         151        2470 LOAD_FAST                0 (summary_groups)
+                    2472 LOAD_FAST                1 (summary)
+                    2474 BUILD_TUPLE              2
+                    2476 RETURN_VALUE
          consts
             None
             'count'
             'countAbandoned'
             'countInProgress'
             'countFinished'
             'minutes'
             'minSeconds'
             'maxSeconds'
             'seconds'
-         names      ('db', 'session', 'query', 'Participant', 'condition', 'func', 'count', 'participantID', 'label', 'sum', 'cast', 'is_abandoned', 'Integer', 'is_in_progress', 'finished', 'avg', 'duration', 'group_by', 'all', 'min', 'max', 'one')
+         names      ('db', 'session', 'query', 'Participant', 'condition', 'func', 'count', 'participantID', 'label', 'sum', 'cast', 'is_abandoned', 'Integer', 'is_in_progress', 'finished', 'avg', 'duration', 'filter', 'or_', 'excludeFromCount', 'group_by', 'all', 'min', 'max', 'one')
          varnames   ('summary_groups', 'summary')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'fetch_progress_summary'
-         firstlineno 100
+         firstlineno 129
          lnotab
-            0x02012c0120018001ba01ba01ba0180fa0e0768f902092c018001ba01ba
-            01ba018001800180f90e0824f8020a
+            0x02012c0120018001ba01ba01ba0180fa0e07920168f8020a2c018001ba
+            01ba01ba018001800180f90e08920124f7020b
       '/progress'
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 8
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000005c
             0200007d007d01740300000000000000000000a6000000ab000000000000
             0000005c0200007d027d0374050000000000000000000064017c007c017c
             027c03740600000000000000000000ac02a6060000ab0600000000000000
             005300
-         123           0 RESUME                   0
+         154           0 RESUME                   0
          
-         126           2 LOAD_GLOBAL              1 (NULL + fetch_progress)
+         157           2 LOAD_GLOBAL              1 (NULL + fetch_progress)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 UNPACK_SEQUENCE          2
                       32 STORE_FAST               0 (pages)
                       34 STORE_FAST               1 (progress)
          
-         127          36 LOAD_GLOBAL              3 (NULL + fetch_progress_summary)
+         158          36 LOAD_GLOBAL              3 (NULL + fetch_progress_summary)
                       48 PRECALL                  0
                       52 CALL                     0
                       62 UNPACK_SEQUENCE          2
                       66 STORE_FAST               2 (summary_groups)
                       68 STORE_FAST               3 (summary)
          
-         129          70 LOAD_GLOBAL              5 (NULL + render_template)
+         160          70 LOAD_GLOBAL              5 (NULL + render_template)
                       82 LOAD_CONST               1 ('progress.html')
          
-         130          84 LOAD_FAST                0 (pages)
+         161          84 LOAD_FAST                0 (pages)
                       86 LOAD_FAST                1 (progress)
          
-         131          88 LOAD_FAST                2 (summary_groups)
+         162          88 LOAD_FAST                2 (summary_groups)
                       90 LOAD_FAST                3 (summary)
                       92 LOAD_GLOBAL              6 (display_time)
          
-         129         104 KW_NAMES                 2
+         160         104 KW_NAMES                 2
                      106 PRECALL                  6
                      110 CALL                     6
                      120 RETURN_VALUE
          consts
             None
             'progress.html'
             ('pages', 'progress', 'summary_groups', 'summary', 'display_time')
          names      ('fetch_progress', 'fetch_progress_summary', 'render_template', 'display_time')
          varnames   ('pages', 'progress', 'summary_groups', 'summary')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_progress'
-         firstlineno 123
+         firstlineno 154
          lnotab 0x0203220122020e01040110fe
       '/progress_ajax'
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 5
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000005c
             0200007d007d0174030000000000000000000064017c007c01ac02a60300
             00ab0300000000000000005300
-         134           0 RESUME                   0
+         165           0 RESUME                   0
          
-         137           2 LOAD_GLOBAL              1 (NULL + fetch_progress)
+         168           2 LOAD_GLOBAL              1 (NULL + fetch_progress)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 UNPACK_SEQUENCE          2
                       32 STORE_FAST               0 (pages)
                       34 STORE_FAST               1 (progress)
          
-         138          36 LOAD_GLOBAL              3 (NULL + render_template)
+         169          36 LOAD_GLOBAL              3 (NULL + render_template)
                       48 LOAD_CONST               1 ('progress_ajax.html')
                       50 LOAD_FAST                0 (pages)
                       52 LOAD_FAST                1 (progress)
                       54 KW_NAMES                 2
                       56 PRECALL                  3
                       60 CALL                     3
                       70 RETURN_VALUE
@@ -1352,58 +1692,154 @@
             ('pages', 'progress')
          names      ('fetch_progress', 'render_template')
          varnames   ('pages', 'progress')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_progress_ajax'
-         firstlineno 134
+         firstlineno 165
          lnotab 0x02032201
       '/progress_summary_ajax'
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000005c
             0200007d007d0174030000000000000000000064017c007c017404000000
             00000000000000ac02a6040000ab0400000000000000005300
-         141           0 RESUME                   0
+         172           0 RESUME                   0
          
-         144           2 LOAD_GLOBAL              1 (NULL + fetch_progress_summary)
+         175           2 LOAD_GLOBAL              1 (NULL + fetch_progress_summary)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 UNPACK_SEQUENCE          2
                       32 STORE_FAST               0 (summary_groups)
                       34 STORE_FAST               1 (summary)
          
-         145          36 LOAD_GLOBAL              3 (NULL + render_template)
+         176          36 LOAD_GLOBAL              3 (NULL + render_template)
                       48 LOAD_CONST               1 ('progress_summary_ajax.html')
          
-         146          50 LOAD_FAST                0 (summary_groups)
+         177          50 LOAD_FAST                0 (summary_groups)
                       52 LOAD_FAST                1 (summary)
                       54 LOAD_GLOBAL              4 (display_time)
          
-         145          66 KW_NAMES                 2
+         176          66 KW_NAMES                 2
                       68 PRECALL                  4
                       72 CALL                     4
                       82 RETURN_VALUE
          consts
             None
             'progress_summary_ajax.html'
             ('summary_groups', 'summary', 'display_time')
          names      ('fetch_progress_summary', 'render_template', 'display_time')
          varnames   ('summary_groups', 'summary')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_progress_summary_ajax'
-         firstlineno 141
+         firstlineno 172
          lnotab 0x020322010e0110ff
+      '/update_exclude_from_count'
+      code
+         argcount  : 0
+         nlocals   : 1
+         stacksize : 5
+         flags     : 3
+         code
+            0x970064017400000000000000000000006a010000000000000000760173
+            0e64027400000000000000000000006a0100000000000000007601720264
+            0353007404000000000000000000006a030000000000000000a004000000
+            00000000000000000000000000000000007404000000000000000000006a
+            050000000000000000a6010000ab010000000000000000a0060000000000
+            0000000000000000000000000000007400000000000000000000006a0100
+            00000000000000640119000000000000000000a6010000ab010000000000
+            0000007d007400000000000000000000006a010000000000000000640219
+            00000000000000000064046b02000000000c007c005f0700000000000000
+            007404000000000000000000006a030000000000000000a0080000000000
+            000000000000000000000000000000a6000000ab00000000000000000001
+            007413000000000000000000006405640664076901ac08a6020000ab0200
+            000000000000005300
+         179           0 RESUME                   0
+         
+         181           2 LOAD_CONST               1 ('participantID')
+                       4 LOAD_GLOBAL              0 (request)
+                      16 LOAD_ATTR                1 (form)
+                      26 CONTAINS_OP              1
+                      28 POP_JUMP_FORWARD_IF_TRUE    14 (to 58)
+                      30 LOAD_CONST               2 ('excludeFromCount')
+                      32 LOAD_GLOBAL              0 (request)
+                      44 LOAD_ATTR                1 (form)
+                      54 CONTAINS_OP              1
+                      56 POP_JUMP_FORWARD_IF_FALSE     2 (to 62)
+         
+         182     >>   58 LOAD_CONST               3 ('')
+                      60 RETURN_VALUE
+         
+         184     >>   62 LOAD_GLOBAL              4 (db)
+                      74 LOAD_ATTR                3 (session)
+                      84 LOAD_METHOD              4 (query)
+                     106 LOAD_GLOBAL              4 (db)
+                     118 LOAD_ATTR                5 (Participant)
+                     128 PRECALL                  1
+                     132 CALL                     1
+                     142 LOAD_METHOD              6 (get)
+                     164 LOAD_GLOBAL              0 (request)
+                     176 LOAD_ATTR                1 (form)
+                     186 LOAD_CONST               1 ('participantID')
+                     188 BINARY_SUBSCR
+                     198 PRECALL                  1
+                     202 CALL                     1
+                     212 STORE_FAST               0 (p)
+         
+         185         214 LOAD_GLOBAL              0 (request)
+                     226 LOAD_ATTR                1 (form)
+                     236 LOAD_CONST               2 ('excludeFromCount')
+                     238 BINARY_SUBSCR
+                     248 LOAD_CONST               4 ('True')
+                     250 COMPARE_OP               2 (==)
+                     256 UNARY_NOT
+                     258 LOAD_FAST                0 (p)
+                     260 STORE_ATTR               7 (excludeFromCount)
+         
+         186         270 LOAD_GLOBAL              4 (db)
+                     282 LOAD_ATTR                3 (session)
+                     292 LOAD_METHOD              8 (commit)
+                     314 PRECALL                  0
+                     318 CALL                     0
+                     328 POP_TOP
+         
+         188         330 LOAD_GLOBAL             19 (NULL + Response)
+                     342 LOAD_CONST               5 (200)
+                     344 LOAD_CONST               6 ('HX-Trigger')
+                     346 LOAD_CONST               7 ('excludeChanged')
+                     348 BUILD_MAP                1
+                     350 KW_NAMES                 8
+                     352 PRECALL                  2
+                     356 CALL                     2
+                     366 RETURN_VALUE
+         consts
+            None
+            'participantID'
+            'excludeFromCount'
+            ''
+            'True'
+            200
+            'HX-Trigger'
+            'excludeChanged'
+            ('status', 'headers')
+         names      ('request', 'form', 'db', 'session', 'query', 'Participant', 'get', 'excludeFromCount', 'commit', 'Response')
+         varnames   ('p',)
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
+         name       'route_update_exclude_from_count'
+         firstlineno 179
+         lnotab 0x020238010402980138013c02
       '/export_item_timing'
       code
          argcount  : 0
          nlocals   : 13
          stacksize : 8
          flags     : 3
          code
@@ -1435,34 +1871,34 @@
             00000000000000000000000000000000007c0b7c0ca6020000ab02000000
             00000000007a0d00007d017c02640ba00b00000000000000000000000000
             000000000000007c0a7c0c19000000000000000000a6010000ab01000000
             00000000007a0d00007d028c3c8ce27c02640c7a0d00007d0264017d0390
             018c2b742b00000000000000000000640d741400000000000000000000a0
             0b0000000000000000000000000000000000000000640e7c017c02a60300
             00ab030000000000000000ac0fa6020000ab0200000000000000005300
-         149           0 RESUME                   0
+         190           0 RESUME                   0
          
-         152           2 LOAD_GLOBAL              0 (current_app)
+         193           2 LOAD_GLOBAL              0 (current_app)
                       14 LOAD_ATTR                1 (page_list)
                       24 LOAD_METHOD              2 (get_questionnaire_list)
                       46 LOAD_CONST               1 (True)
                       48 PRECALL                  1
                       52 CALL                     1
                       62 STORE_FAST               0 (questionnaires)
          
-         153          64 LOAD_CONST               2 ('participantID,mTurkID')
+         194          64 LOAD_CONST               2 ('participantID,mTurkID')
                       66 STORE_FAST               1 (header)
          
-         154          68 LOAD_CONST               3 ('')
+         195          68 LOAD_CONST               3 ('')
                       70 STORE_FAST               2 (output)
          
-         156          72 LOAD_CONST               4 (False)
+         197          72 LOAD_CONST               4 (False)
                       74 STORE_FAST               3 (headerComplete)
          
-         158          76 LOAD_GLOBAL              6 (db)
+         199          76 LOAD_GLOBAL              6 (db)
                       88 LOAD_ATTR                4 (session)
                       98 LOAD_METHOD              5 (query)
                      120 LOAD_GLOBAL              6 (db)
                      132 LOAD_ATTR                6 (Participant)
                      142 PRECALL                  1
                      146 CALL                     1
                      156 LOAD_METHOD              7 (filter)
@@ -1474,21 +1910,21 @@
                      218 PRECALL                  1
                      222 CALL                     1
                      232 LOAD_METHOD              9 (all)
                      254 PRECALL                  0
                      258 CALL                     0
                      268 STORE_FAST               4 (results)
          
-         160         270 LOAD_FAST                4 (results)
+         201         270 LOAD_FAST                4 (results)
                      272 GET_ITER
                  >>  274 EXTENDED_ARG             1
                      276 FOR_ITER               297 (to 872)
                      278 STORE_FAST               5 (p)
          
-         161         280 LOAD_FAST                2 (output)
+         202         280 LOAD_FAST                2 (output)
                      282 LOAD_GLOBAL             20 (str)
                      294 LOAD_METHOD             11 (format)
                      316 LOAD_CONST               5 ('{},"{}"')
                      318 LOAD_FAST                5 (p)
                      320 LOAD_ATTR               12 (participantID)
                      330 LOAD_FAST                5 (p)
                      332 LOAD_ATTR               13 (mTurkID)
@@ -1496,128 +1932,128 @@
                      364 PRECALL                  0
                      368 CALL                     0
                      378 PRECALL                  3
                      382 CALL                     3
                      392 BINARY_OP               13 (+=)
                      396 STORE_FAST               2 (output)
          
-         163         398 LOAD_FAST                0 (questionnaires)
+         204         398 LOAD_FAST                0 (questionnaires)
                      400 GET_ITER
                  >>  402 FOR_ITER               225 (to 854)
                      404 STORE_FAST               6 (qName)
          
-         164         406 LOAD_CONST               3 ('')
+         205         406 LOAD_CONST               3 ('')
                      408 STORE_FAST               7 (tag)
          
-         166         410 LOAD_CONST               6 ('/')
+         207         410 LOAD_CONST               6 ('/')
                      412 LOAD_FAST                6 (qName)
                      414 CONTAINS_OP              0
                      416 POP_JUMP_FORWARD_IF_FALSE    37 (to 492)
          
-         167         418 LOAD_FAST                6 (qName)
+         208         418 LOAD_FAST                6 (qName)
                      420 LOAD_METHOD             15 (split)
                      442 LOAD_CONST               6 ('/')
                      444 PRECALL                  1
                      448 CALL                     1
                      458 STORE_FAST               8 (qNameParts)
          
-         168         460 LOAD_FAST                8 (qNameParts)
+         209         460 LOAD_FAST                8 (qNameParts)
                      462 LOAD_CONST               7 (0)
                      464 BINARY_SUBSCR
                      474 STORE_FAST               6 (qName)
          
-         169         476 LOAD_FAST                8 (qNameParts)
+         210         476 LOAD_FAST                8 (qNameParts)
                      478 LOAD_CONST               8 (1)
                      480 BINARY_SUBSCR
                      490 STORE_FAST               7 (tag)
          
-         171     >>  492 LOAD_FAST                5 (p)
+         212     >>  492 LOAD_FAST                5 (p)
                      494 LOAD_METHOD             16 (questionnaire)
                      516 LOAD_FAST                6 (qName)
                      518 LOAD_FAST                7 (tag)
                      520 PRECALL                  2
                      524 CALL                     2
                      534 STORE_FAST               9 (q)
          
-         172         536 LOAD_FAST                5 (p)
+         213         536 LOAD_FAST                5 (p)
                      538 LOAD_METHOD             17 (questionnaire_log)
                      560 LOAD_FAST                6 (qName)
                      562 LOAD_FAST                7 (tag)
                      564 PRECALL                  2
                      568 CALL                     2
                      578 STORE_FAST              10 (logs)
          
-         174         580 LOAD_FAST                6 (qName)
+         215         580 LOAD_FAST                6 (qName)
                      582 STORE_FAST              11 (qNameFull)
          
-         175         584 LOAD_GLOBAL             37 (NULL + len)
+         216         584 LOAD_GLOBAL             37 (NULL + len)
                      596 LOAD_FAST                7 (tag)
                      598 PRECALL                  1
                      602 CALL                     1
                      612 LOAD_CONST               7 (0)
                      614 COMPARE_OP               4 (>)
                      620 POP_JUMP_FORWARD_IF_FALSE    22 (to 666)
          
-         176         622 LOAD_CONST               9 ('{}_{}')
+         217         622 LOAD_CONST               9 ('{}_{}')
                      624 LOAD_METHOD             11 (format)
                      646 LOAD_FAST                6 (qName)
                      648 LOAD_FAST                7 (tag)
                      650 PRECALL                  2
                      654 CALL                     2
                      664 STORE_FAST              11 (qNameFull)
          
-         178     >>  666 LOAD_GLOBAL             39 (NULL + sorted)
+         219     >>  666 LOAD_GLOBAL             39 (NULL + sorted)
                      678 LOAD_FAST               10 (logs)
                      680 LOAD_METHOD             20 (keys)
                      702 PRECALL                  0
                      706 CALL                     0
                      716 PRECALL                  1
                      720 CALL                     1
                      730 GET_ITER
                  >>  732 FOR_ITER                59 (to 852)
                      734 STORE_FAST              12 (key)
          
-         179         736 LOAD_FAST                3 (headerComplete)
+         220         736 LOAD_FAST                3 (headerComplete)
                      738 POP_JUMP_FORWARD_IF_TRUE    25 (to 790)
          
-         180         740 LOAD_FAST                1 (header)
+         221         740 LOAD_FAST                1 (header)
                      742 LOAD_CONST              10 (',{}_{}')
                      744 LOAD_METHOD             11 (format)
                      766 LOAD_FAST               11 (qNameFull)
                      768 LOAD_FAST               12 (key)
                      770 PRECALL                  2
                      774 CALL                     2
                      784 BINARY_OP               13 (+=)
                      788 STORE_FAST               1 (header)
          
-         182     >>  790 LOAD_FAST                2 (output)
+         223     >>  790 LOAD_FAST                2 (output)
                      792 LOAD_CONST              11 (',{}')
                      794 LOAD_METHOD             11 (format)
                      816 LOAD_FAST               10 (logs)
                      818 LOAD_FAST               12 (key)
                      820 BINARY_SUBSCR
                      830 PRECALL                  1
                      834 CALL                     1
                      844 BINARY_OP               13 (+=)
                      848 STORE_FAST               2 (output)
                      850 JUMP_BACKWARD           60 (to 732)
          
-         178     >>  852 JUMP_BACKWARD          226 (to 402)
+         219     >>  852 JUMP_BACKWARD          226 (to 402)
          
-         184     >>  854 LOAD_FAST                2 (output)
+         225     >>  854 LOAD_FAST                2 (output)
                      856 LOAD_CONST              12 ('\n')
                      858 BINARY_OP               13 (+=)
                      862 STORE_FAST               2 (output)
          
-         185         864 LOAD_CONST               1 (True)
+         226         864 LOAD_CONST               1 (True)
                      866 STORE_FAST               3 (headerComplete)
                      868 EXTENDED_ARG             1
                      870 JUMP_BACKWARD          299 (to 274)
          
-         187     >>  872 LOAD_GLOBAL             43 (NULL + render_template)
+         228     >>  872 LOAD_GLOBAL             43 (NULL + render_template)
                      884 LOAD_CONST              13 ('export_csv.html')
                      886 LOAD_GLOBAL             20 (str)
                      898 LOAD_METHOD             11 (format)
                      920 LOAD_CONST              14 ('{}\n{}')
                      922 LOAD_FAST                1 (header)
                      924 LOAD_FAST                2 (output)
                      926 PRECALL                  3
@@ -1645,211 +2081,254 @@
             ('data',)
          names      ('current_app', 'page_list', 'get_questionnaire_list', 'db', 'session', 'query', 'Participant', 'filter', 'finished', 'all', 'str', 'format', 'participantID', 'mTurkID', 'strip', 'split', 'questionnaire', 'questionnaire_log', 'len', 'sorted', 'keys', 'render_template')
          varnames   ('questionnaires', 'header', 'output', 'headerComplete', 'results', 'p', 'qName', 'tag', 'qNameParts', 'q', 'logs', 'qNameFull', 'key')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_export_item_timing'
-         firstlineno 149
+         firstlineno 190
          lnotab
             0x02033e01040104020402c2020a0176020801040208012a01100110022c
             012c02040126012c024601040132023efc02060a010802
       '/export'
       '/export/download'
       'route_export_download'
       ('endpoint',)
       code
          argcount  : 0
-         nlocals   : 7
+         nlocals   : 9
          stacksize : 10
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007400000000000000000000006a
             030000000000000000a6010000ab010000000000000000a0040000000000
             0000000000000000000000000000007400000000000000000000006a0300
             000000000000006a05000000000000000064016b0200000000a6010000ab
             010000000000000000a00600000000000000000000000000000000000000
-            00a6000000ab0000000000000000007d00740e000000000000000000006a
-            080000000000000000a00900000000000000000000000000000000000000
-            0064026401a6020000ab0200000000000000007d01740e00000000000000
-            0000006a080000000000000000a009000000000000000000000000000000
-            000000000064036404a6020000ab0200000000000000007d0267007d0369
-            007d047415000000000000000000007c037c047c01a6030000ab03000000
-            00000000007d057417000000000000000000007c037c047c057c02a60400
-            00ab04000000000000000001007419000000000000000000007c037c047c
-            057c02a6040000ab0400000000000000000100741b000000000000000000
-            007c037c04a6020000ab0200000000000000007d06740e00000000000000
-            0000006a0e0000000000000000a00f000000000000000000000000000000
-            00000000006405a6010000ab010000000000000000723e74210000000000
-            00000000007c0664066407640864097423000000000000000000006a1200
-            00000000000000a6000000ab000000000000000000a01300000000000000
-            00000000000000000000000000640aa6010000ab0100000000000000007a
-            0000007a0600006901ac0ba6030000ab0300000000000000005300742900
-            000000000000000000640c7c06742b000000000000000000007c04a60100
-            00ab0100000000000000007c00ac0da6040000ab04000000000000000053
-            00
-         190           0 RESUME                   0
+            00a6000000ab0000000000000000007d007400000000000000000000006a
+            010000000000000000a00200000000000000000000000000000000000000
+            007400000000000000000000006a030000000000000000a6010000ab0100
+            00000000000000a004000000000000000000000000000000000000000074
+            00000000000000000000006a0300000000000000006a0700000000000000
+            0064026b0200000000a6010000ab010000000000000000a0060000000000
+            000000000000000000000000000000a6000000ab0000000000000000007d
+            017410000000000000000000006a090000000000000000a00a0000000000
+            00000000000000000000000000000064036401a6020000ab020000000000
+            0000007d027410000000000000000000006a090000000000000000a00a00
+            0000000000000000000000000000000000000064046402a6020000ab0200
+            000000000000007d037410000000000000000000006a0900000000000000
+            00a00a000000000000000000000000000000000000000064056401a60200
+            00ab0200000000000000007d0467007d0569007d06741700000000000000
+            0000007c057c067c027c04a6040000ab0400000000000000007d07741900
+            0000000000000000007c057c067c077c03a6040000ab0400000000000000
+            000100741b000000000000000000007c057c067c077c03a6040000ab0400
+            000000000000000100741d000000000000000000007c057c06a6020000ab
+            0200000000000000007d087410000000000000000000006a0f0000000000
+            000000a01000000000000000000000000000000000000000006406a60100
+            00ab010000000000000000723e7423000000000000000000007c08640764
+            086409640a7425000000000000000000006a130000000000000000a60000
+            00ab000000000000000000a0140000000000000000000000000000000000
+            000000640ba6010000ab0100000000000000007a0000007a0600006901ac
+            0ca6030000ab0300000000000000005300742b0000000000000000000064
+            0d7c08742d000000000000000000007c06a6010000ab0100000000000000
+            007c007c01ac0ea6050000ab0500000000000000005300
+         231           0 RESUME                   0
          
-         194           2 LOAD_GLOBAL              0 (db)
+         235           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_ATTR                1 (session)
                       24 LOAD_METHOD              2 (query)
                       46 LOAD_GLOBAL              0 (db)
                       58 LOAD_ATTR                3 (Participant)
                       68 PRECALL                  1
                       72 CALL                     1
          
-         195          82 LOAD_METHOD              4 (filter)
+         236          82 LOAD_METHOD              4 (filter)
                      104 LOAD_GLOBAL              0 (db)
                      116 LOAD_ATTR                3 (Participant)
                      126 LOAD_ATTR                5 (finished)
                      136 LOAD_CONST               1 (False)
                      138 COMPARE_OP               2 (==)
                      144 PRECALL                  1
                      148 CALL                     1
                      158 LOAD_METHOD              6 (count)
                      180 PRECALL                  0
                      184 CALL                     0
          
-         194         194 STORE_FAST               0 (unfinished_count)
-         
-         197         196 LOAD_GLOBAL             14 (request)
-                     208 LOAD_ATTR                8 (args)
-                     218 LOAD_METHOD              9 (get)
-                     240 LOAD_CONST               2 ('includeUnfinished')
-                     242 LOAD_CONST               1 (False)
-                     244 PRECALL                  2
-                     248 CALL                     2
-                     258 STORE_FAST               1 (include_unfinished)
-         
-         198         260 LOAD_GLOBAL             14 (request)
-                     272 LOAD_ATTR                8 (args)
-                     282 LOAD_METHOD              9 (get)
-                     304 LOAD_CONST               3 ('includeMissing')
-                     306 LOAD_CONST               4 (True)
-                     308 PRECALL                  2
-                     312 CALL                     2
-                     322 STORE_FAST               2 (include_missing)
-         
-         200         324 BUILD_LIST               0
-                     326 STORE_FAST               3 (column_list)
-         
-         201         328 BUILD_MAP                0
-                     330 STORE_FAST               4 (export_data)
-         
-         203         332 LOAD_GLOBAL             21 (NULL + add_participants_to_export)
-                     344 LOAD_FAST                3 (column_list)
-                     346 LOAD_FAST                4 (export_data)
-                     348 LOAD_FAST                1 (include_unfinished)
-                     350 PRECALL                  3
-                     354 CALL                     3
-                     364 STORE_FAST               5 (query)
+         235         194 STORE_FAST               0 (unfinished_count)
          
-         204         366 LOAD_GLOBAL             23 (NULL + add_questionnaires_to_export)
-                     378 LOAD_FAST                3 (column_list)
-                     380 LOAD_FAST                4 (export_data)
-                     382 LOAD_FAST                5 (query)
-                     384 LOAD_FAST                2 (include_missing)
-                     386 PRECALL                  4
-                     390 CALL                     4
-                     400 POP_TOP
-         
-         205         402 LOAD_GLOBAL             25 (NULL + add_custom_exports_to_export)
-                     414 LOAD_FAST                3 (column_list)
-                     416 LOAD_FAST                4 (export_data)
-                     418 LOAD_FAST                5 (query)
-                     420 LOAD_FAST                2 (include_missing)
-                     422 PRECALL                  4
-                     426 CALL                     4
-                     436 POP_TOP
-         
-         207         438 LOAD_GLOBAL             27 (NULL + build_export_csv)
-                     450 LOAD_FAST                3 (column_list)
-                     452 LOAD_FAST                4 (export_data)
-                     454 PRECALL                  2
-                     458 CALL                     2
-                     468 STORE_FAST               6 (csv_string)
-         
-         209         470 LOAD_GLOBAL             14 (request)
-                     482 LOAD_ATTR               14 (base_url)
-                     492 LOAD_METHOD             15 (endswith)
-                     514 LOAD_CONST               5 ('/download')
-                     516 PRECALL                  1
-                     520 CALL                     1
-                     530 POP_JUMP_FORWARD_IF_FALSE    62 (to 656)
-         
-         210         532 LOAD_GLOBAL             33 (NULL + Response)
-                     544 LOAD_FAST                6 (csv_string)
-         
-         211         546 LOAD_CONST               6 ('text/csv')
-         
-         213         548 LOAD_CONST               7 ('Content-disposition')
-                     550 LOAD_CONST               8 ('attachment; filename=%s.csv')
-         
-         214         552 LOAD_CONST               9 ('export_')
-                     554 LOAD_GLOBAL             35 (NULL + datetime)
-                     566 LOAD_ATTR               18 (utcnow)
-                     576 PRECALL                  0
-                     580 CALL                     0
-                     590 LOAD_METHOD             19 (strftime)
-                     612 LOAD_CONST              10 ('%Y-%m-%d_%H-%M')
-                     614 PRECALL                  1
-                     618 CALL                     1
-                     628 BINARY_OP                0 (+)
-         
-         213         632 BINARY_OP                6 (%)
-         
-         212         636 BUILD_MAP                1
-         
-         210         638 KW_NAMES                11
-                     640 PRECALL                  3
-                     644 CALL                     3
-                     654 RETURN_VALUE
-         
-         217     >>  656 LOAD_GLOBAL             41 (NULL + render_template)
-                     668 LOAD_CONST              12 ('export.html')
-         
-         218         670 LOAD_FAST                6 (csv_string)
-         
-         219         672 LOAD_GLOBAL             43 (NULL + len)
-                     684 LOAD_FAST                4 (export_data)
-                     686 PRECALL                  1
-                     690 CALL                     1
-         
-         220         700 LOAD_FAST                0 (unfinished_count)
-         
-         217         702 KW_NAMES                13
-                     704 PRECALL                  4
-                     708 CALL                     4
-                     718 RETURN_VALUE
+         237         196 LOAD_GLOBAL              0 (db)
+                     208 LOAD_ATTR                1 (session)
+                     218 LOAD_METHOD              2 (query)
+                     240 LOAD_GLOBAL              0 (db)
+                     252 LOAD_ATTR                3 (Participant)
+                     262 PRECALL                  1
+                     266 CALL                     1
+         
+         238         276 LOAD_METHOD              4 (filter)
+                     298 LOAD_GLOBAL              0 (db)
+                     310 LOAD_ATTR                3 (Participant)
+                     320 LOAD_ATTR                7 (excludeFromCount)
+                     330 LOAD_CONST               2 (True)
+                     332 COMPARE_OP               2 (==)
+                     338 PRECALL                  1
+                     342 CALL                     1
+                     352 LOAD_METHOD              6 (count)
+                     374 PRECALL                  0
+                     378 CALL                     0
+         
+         237         388 STORE_FAST               1 (excluded_count)
+         
+         240         390 LOAD_GLOBAL             16 (request)
+                     402 LOAD_ATTR                9 (args)
+                     412 LOAD_METHOD             10 (get)
+                     434 LOAD_CONST               3 ('includeUnfinished')
+                     436 LOAD_CONST               1 (False)
+                     438 PRECALL                  2
+                     442 CALL                     2
+                     452 STORE_FAST               2 (include_unfinished)
+         
+         241         454 LOAD_GLOBAL             16 (request)
+                     466 LOAD_ATTR                9 (args)
+                     476 LOAD_METHOD             10 (get)
+                     498 LOAD_CONST               4 ('includeMissing')
+                     500 LOAD_CONST               2 (True)
+                     502 PRECALL                  2
+                     506 CALL                     2
+                     516 STORE_FAST               3 (include_missing)
+         
+         242         518 LOAD_GLOBAL             16 (request)
+                     530 LOAD_ATTR                9 (args)
+                     540 LOAD_METHOD             10 (get)
+                     562 LOAD_CONST               5 ('includeExcluded')
+                     564 LOAD_CONST               1 (False)
+                     566 PRECALL                  2
+                     570 CALL                     2
+                     580 STORE_FAST               4 (include_excluded)
+         
+         244         582 BUILD_LIST               0
+                     584 STORE_FAST               5 (column_list)
+         
+         245         586 BUILD_MAP                0
+                     588 STORE_FAST               6 (export_data)
+         
+         247         590 LOAD_GLOBAL             23 (NULL + add_participants_to_export)
+                     602 LOAD_FAST                5 (column_list)
+                     604 LOAD_FAST                6 (export_data)
+                     606 LOAD_FAST                2 (include_unfinished)
+                     608 LOAD_FAST                4 (include_excluded)
+                     610 PRECALL                  4
+                     614 CALL                     4
+                     624 STORE_FAST               7 (query)
+         
+         248         626 LOAD_GLOBAL             25 (NULL + add_questionnaires_to_export)
+                     638 LOAD_FAST                5 (column_list)
+                     640 LOAD_FAST                6 (export_data)
+                     642 LOAD_FAST                7 (query)
+                     644 LOAD_FAST                3 (include_missing)
+                     646 PRECALL                  4
+                     650 CALL                     4
+                     660 POP_TOP
+         
+         249         662 LOAD_GLOBAL             27 (NULL + add_custom_exports_to_export)
+                     674 LOAD_FAST                5 (column_list)
+                     676 LOAD_FAST                6 (export_data)
+                     678 LOAD_FAST                7 (query)
+                     680 LOAD_FAST                3 (include_missing)
+                     682 PRECALL                  4
+                     686 CALL                     4
+                     696 POP_TOP
+         
+         251         698 LOAD_GLOBAL             29 (NULL + build_export_csv)
+                     710 LOAD_FAST                5 (column_list)
+                     712 LOAD_FAST                6 (export_data)
+                     714 PRECALL                  2
+                     718 CALL                     2
+                     728 STORE_FAST               8 (csv_string)
+         
+         253         730 LOAD_GLOBAL             16 (request)
+                     742 LOAD_ATTR               15 (base_url)
+                     752 LOAD_METHOD             16 (endswith)
+                     774 LOAD_CONST               6 ('/download')
+                     776 PRECALL                  1
+                     780 CALL                     1
+                     790 POP_JUMP_FORWARD_IF_FALSE    62 (to 916)
+         
+         254         792 LOAD_GLOBAL             35 (NULL + Response)
+                     804 LOAD_FAST                8 (csv_string)
+         
+         255         806 LOAD_CONST               7 ('text/csv')
+         
+         257         808 LOAD_CONST               8 ('Content-disposition')
+                     810 LOAD_CONST               9 ('attachment; filename=%s.csv')
+         
+         258         812 LOAD_CONST              10 ('export_')
+                     814 LOAD_GLOBAL             37 (NULL + datetime)
+                     826 LOAD_ATTR               19 (utcnow)
+                     836 PRECALL                  0
+                     840 CALL                     0
+                     850 LOAD_METHOD             20 (strftime)
+                     872 LOAD_CONST              11 ('%Y-%m-%d_%H-%M')
+                     874 PRECALL                  1
+                     878 CALL                     1
+                     888 BINARY_OP                0 (+)
+         
+         257         892 BINARY_OP                6 (%)
+         
+         256         896 BUILD_MAP                1
+         
+         254         898 KW_NAMES                12
+                     900 PRECALL                  3
+                     904 CALL                     3
+                     914 RETURN_VALUE
+         
+         261     >>  916 LOAD_GLOBAL             43 (NULL + render_template)
+                     928 LOAD_CONST              13 ('export.html')
+         
+         262         930 LOAD_FAST                8 (csv_string)
+         
+         263         932 LOAD_GLOBAL             45 (NULL + len)
+                     944 LOAD_FAST                6 (export_data)
+                     946 PRECALL                  1
+                     950 CALL                     1
+         
+         264         960 LOAD_FAST                0 (unfinished_count)
+         
+         265         962 LOAD_FAST                1 (excluded_count)
+         
+         261         964 KW_NAMES                14
+                     966 PRECALL                  5
+                     970 CALL                     5
+                     980 RETURN_VALUE
          consts
             None
             False
+            True
             'includeUnfinished'
             'includeMissing'
-            True
+            'includeExcluded'
             '/download'
             'text/csv'
             'Content-disposition'
             'attachment; filename=%s.csv'
             'export_'
             '%Y-%m-%d_%H-%M'
             ('mimetype', 'headers')
             'export.html'
-            ('data', 'rowCount', 'unfinishedCount')
-         names      ('db', 'session', 'query', 'Participant', 'filter', 'finished', 'count', 'request', 'args', 'get', 'add_participants_to_export', 'add_questionnaires_to_export', 'add_custom_exports_to_export', 'build_export_csv', 'base_url', 'endswith', 'Response', 'datetime', 'utcnow', 'strftime', 'render_template', 'len')
-         varnames   ('unfinished_count', 'include_unfinished', 'include_missing', 'column_list', 'export_data', 'query', 'csv_string')
+            ('data', 'rowCount', 'unfinishedCount', 'excludedCount')
+         names      ('db', 'session', 'query', 'Participant', 'filter', 'finished', 'count', 'excludeFromCount', 'request', 'args', 'get', 'add_participants_to_export', 'add_questionnaires_to_export', 'add_custom_exports_to_export', 'build_export_csv', 'base_url', 'endswith', 'Response', 'datetime', 'utcnow', 'strftime', 'render_template', 'len')
+         varnames   ('unfinished_count', 'excluded_count', 'include_unfinished', 'include_missing', 'include_excluded', 'column_list', 'export_data', 'query', 'csv_string')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_export'
-         firstlineno 190
+         firstlineno 231
          lnotab
-            0x0204500170ff0203400140020401040222012401240220023e010e0102
-            02040150ff04ff02fe12070e0102011c0102fd
+            0x0204500170ff0202500170ff0203400140014002040104022401240124
+            0220023e010e010202040150ff04ff02fe12070e0102011c01020102fc
       '/results'
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -1859,68 +2338,68 @@
             037d047407000000000000000000007408000000000000000000007c0319
             0000000000000000007c04a6020000ab0200000000000000007d057c05a0
             050000000000000000000000000000000000000000a6000000ab00000000
             000000000001007c05a00600000000000000000000000000000000000000
             00a6000000ab00000000000000000001007c057c017c023c0000008c5d74
             0f0000000000000000000064037c01ac04a6020000ab0200000000000000
             005300
-         223           0 RESUME                   0
+         268           0 RESUME                   0
          
-         226           2 LOAD_GLOBAL              1 (NULL + page_list)
+         271           2 LOAD_GLOBAL              1 (NULL + page_list)
                       14 LOAD_ATTR                1 (get_questionnaire_list)
                       24 LOAD_CONST               1 (True)
                       26 KW_NAMES                 2
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_FAST               0 (qList)
          
-         227          44 BUILD_MAP                0
+         272          44 BUILD_MAP                0
                       46 STORE_FAST               1 (results)
          
-         229          48 LOAD_FAST                0 (qList)
+         274          48 LOAD_FAST                0 (qList)
                       50 GET_ITER
                  >>   52 FOR_ITER                92 (to 238)
                       54 STORE_FAST               2 (qNameAndTag)
          
-         230          56 LOAD_GLOBAL              5 (NULL + questionnaire_name_and_tag)
+         275          56 LOAD_GLOBAL              5 (NULL + questionnaire_name_and_tag)
                       68 LOAD_FAST                2 (qNameAndTag)
                       70 PRECALL                  1
                       74 CALL                     1
                       84 UNPACK_SEQUENCE          2
                       88 STORE_FAST               3 (qName)
                       90 STORE_FAST               4 (qTag)
          
-         232          92 LOAD_GLOBAL              7 (NULL + QuestionnaireResults)
+         277          92 LOAD_GLOBAL              7 (NULL + QuestionnaireResults)
                      104 LOAD_GLOBAL              8 (questionnaires)
                      116 LOAD_FAST                3 (qName)
                      118 BINARY_SUBSCR
                      128 LOAD_FAST                4 (qTag)
                      130 PRECALL                  2
                      134 CALL                     2
                      144 STORE_FAST               5 (qResults)
          
-         233         146 LOAD_FAST                5 (qResults)
+         278         146 LOAD_FAST                5 (qResults)
                      148 LOAD_METHOD              5 (run_query)
                      170 PRECALL                  0
                      174 CALL                     0
                      184 POP_TOP
          
-         234         186 LOAD_FAST                5 (qResults)
+         279         186 LOAD_FAST                5 (qResults)
                      188 LOAD_METHOD              6 (calc_descriptives)
                      210 PRECALL                  0
                      214 CALL                     0
                      224 POP_TOP
          
-         236         226 LOAD_FAST                5 (qResults)
+         281         226 LOAD_FAST                5 (qResults)
                      228 LOAD_FAST                1 (results)
                      230 LOAD_FAST                2 (qNameAndTag)
                      232 STORE_SUBSCR
                      236 JUMP_BACKWARD           93 (to 52)
          
-         238     >>  238 LOAD_GLOBAL             15 (NULL + render_template)
+         283     >>  238 LOAD_GLOBAL             15 (NULL + render_template)
                      250 LOAD_CONST               3 ('results.html')
                      252 LOAD_FAST                1 (results)
                      254 KW_NAMES                 4
                      256 PRECALL                  2
                      260 CALL                     2
                      270 RETURN_VALUE
          consts
@@ -1931,362 +2410,470 @@
             ('results',)
          names      ('page_list', 'get_questionnaire_list', 'questionnaire_name_and_tag', 'QuestionnaireResults', 'questionnaires', 'run_query', 'calc_descriptives', 'render_template')
          varnames   ('qList', 'results', 'qNameAndTag', 'qName', 'qTag', 'qResults')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_results'
-         firstlineno 223
+         firstlineno 268
          lnotab 0x02032a010402080124023601280128020c02
       '/preview_questionnaire/<questionnaireName>'
       code
          argcount  : 1
-         nlocals   : 9
+         nlocals   : 11
          stacksize : 9
          flags     : 3
          code
-            0x970067007d010900740100000000000000000000740300000000000000
-            0000006a0200000000000000007c00a6010000ab01000000000000000064
-            01a6020000ab0200000000000000007d027c02a003000000000000000000
-            0000000000000000000000a6000000ab0000000000000000007d03740900
-            0000000000000000006a0500000000000000007c03a6010000ab01000000
-            00000000007d037c02a00600000000000000000000000000000000000000
-            00a6000000ab00000000000000000001006e2b2300740e00000000000000
-            0000002400721e7d047411000000000000000000007c046a090000000000
-            000000a6010000ab0100000000000000007d01590064007d047e046e0864
-            007d047e047701770078035900770164027c007a0000007d057c00741500
-            0000000000000000006a0b0000000000000000a6000000ab000000000000
-            00000076009002720209007418000000000000000000006a0d0000000000
-            000000a00e00000000000000000000000000000000000000007418000000
-            000000000000006a0f00000000000000006a1000000000000000007c0519
-            000000000000000000a6010000ab010000000000000000a0110000000000
-            000000000000000000000000000000a6000000ab00000000000000000001
-            006e872300740e000000000000000000002400727a7d047c01a012000000
-            00000000000000000000000000000000007411000000000000000000007c
-            046a090000000000000000a6010000ab010000000000000000a6010000ab
-            010000000000000000010064037c046a0900000000000000006404190000
-            00000000000000760072167c01a013000000000000000000000000000000
-            00000000006405a6010000ab01000000000000000001006e2464067c046a
-            090000000000000000640419000000000000000000760072157c01a01300
-            000000000000000000000000000000000000006407a6010000ab01000000
-            00000000000100590064007d047e046e0864007d047e0477017700780359
-            00770164087428000000000000000000006a090000000000000000760090
-            0172247c01440090015d207d0464037c04760072d57c04a0150000000000
-            0000000000000000000000000000007c0564097a000000a6010000ab0100
-            000000000000007d047c04742d000000000000000000007c04a6010000ab
-            010000000000000000640a7a0a0000190000000000000000007d06741800
-            0000000000000000006a0f00000000000000006a1000000000000000007c
-            05190000000000000000006a1700000000000000007c0619000000000000
-            0000006a1800000000000000007d077419000000000000000000006a1900
-            00000000000000743400000000000000000000a01b000000000000000000
-            0000000000000000000000640b7c057c067c07a6040000ab040000000000
-            000000a6010000ab0100000000000000007d087418000000000000000000
-            006a1c0000000000000000a01d0000000000000000000000000000000000
-            0000007c08a6010000ab01000000000000000001007c01a0130000000000
-            000000000000000000000000000000743400000000000000000000a01b00
-            00000000000000000000000000000000000000640c7c067c077c05a60400
-            00ab040000000000000000a6010000ab010000000000000000010064067c
-            04760072407419000000000000000000006a1e0000000000000000a60000
-            00ab00000000000000000001007c01a01300000000000000000000000000
-            00000000000000743400000000000000000000a01b000000000000000000
-            0000000000000000000000640da6010000ab010000000000000000a60100
-            00ab010000000000000000010090018c22743f0000000000000000000064
-            0e7c037c01ac0fa6030000ab0300000000000000005300
-         241           0 RESUME                   0
-         
-         244           2 BUILD_LIST               0
-                       4 STORE_FAST               1 (errors)
-         
-         246           6 NOP
-         
-         247           8 LOAD_GLOBAL              1 (NULL + open)
-                      20 LOAD_GLOBAL              3 (NULL + current_app)
-                      32 LOAD_ATTR                2 (get_questionnaire_path)
-                      42 LOAD_FAST                0 (questionnaireName)
-                      44 PRECALL                  1
-                      48 CALL                     1
-                      58 LOAD_CONST               1 ('r')
-                      60 PRECALL                  2
-                      64 CALL                     2
-                      74 STORE_FAST               2 (f)
-         
-         248          76 LOAD_FAST                2 (f)
-                      78 LOAD_METHOD              3 (read)
-                     100 PRECALL                  0
-                     104 CALL                     0
-                     114 STORE_FAST               3 (json_data)
-         
-         249         116 LOAD_GLOBAL              9 (NULL + json)
-                     128 LOAD_ATTR                5 (loads)
-                     138 LOAD_FAST                3 (json_data)
-                     140 PRECALL                  1
-                     144 CALL                     1
-                     154 STORE_FAST               3 (json_data)
-         
-         250         156 LOAD_FAST                2 (f)
-                     158 LOAD_METHOD              6 (close)
-                     180 PRECALL                  0
-                     184 CALL                     0
-                     194 POP_TOP
-                     196 JUMP_FORWARD            43 (to 284)
-                 >>  198 PUSH_EXC_INFO
-         
-         251         200 LOAD_GLOBAL             14 (Exception)
-                     212 CHECK_EXC_MATCH
-                     214 POP_JUMP_FORWARD_IF_FALSE    30 (to 276)
-                     216 STORE_FAST               4 (e)
-         
-         252         218 LOAD_GLOBAL             17 (NULL + list)
-                     230 LOAD_FAST                4 (e)
-                     232 LOAD_ATTR                9 (args)
-                     242 PRECALL                  1
-                     246 CALL                     1
-                     256 STORE_FAST               1 (errors)
-                     258 POP_EXCEPT
-                     260 LOAD_CONST               0 (None)
-                     262 STORE_FAST               4 (e)
-                     264 DELETE_FAST              4 (e)
-                     266 JUMP_FORWARD             8 (to 284)
-                 >>  268 LOAD_CONST               0 (None)
-                     270 STORE_FAST               4 (e)
-                     272 DELETE_FAST              4 (e)
-                     274 RERAISE                  1
-         
-         251     >>  276 RERAISE                  0
-                 >>  278 COPY                     3
-                     280 POP_EXCEPT
-                     282 RERAISE                  1
-         
-         254     >>  284 LOAD_CONST               2 ('questionnaire_')
-                     286 LOAD_FAST                0 (questionnaireName)
-                     288 BINARY_OP                0 (+)
-                     292 STORE_FAST               5 (table_name)
-         
-         256         294 LOAD_FAST                0 (questionnaireName)
-                     296 LOAD_GLOBAL             21 (NULL + page_list)
-                     308 LOAD_ATTR               11 (get_questionnaire_list)
-                     318 PRECALL                  0
-                     322 CALL                     0
-                     332 CONTAINS_OP              0
-                     334 EXTENDED_ARG             2
-                     336 POP_JUMP_FORWARD_IF_FALSE   514 (to 1366)
-         
-         257         338 NOP
-         
-         258         340 LOAD_GLOBAL             24 (db)
-                     352 LOAD_ATTR               13 (session)
-                     362 LOAD_METHOD             14 (query)
-                     384 LOAD_GLOBAL             24 (db)
-                     396 LOAD_ATTR               15 (metadata)
-                     406 LOAD_ATTR               16 (tables)
-                     416 LOAD_FAST                5 (table_name)
-                     418 BINARY_SUBSCR
-                     428 PRECALL                  1
-                     432 CALL                     1
-                     442 LOAD_METHOD             17 (first)
-                     464 PRECALL                  0
-                     468 CALL                     0
-                     478 POP_TOP
-                     480 JUMP_FORWARD           135 (to 752)
-                 >>  482 PUSH_EXC_INFO
-         
-         259         484 LOAD_GLOBAL             14 (Exception)
-                     496 CHECK_EXC_MATCH
-                     498 POP_JUMP_FORWARD_IF_FALSE   122 (to 744)
-                     500 STORE_FAST               4 (e)
-         
-         260         502 LOAD_FAST                1 (errors)
-                     504 LOAD_METHOD             18 (extend)
-                     526 LOAD_GLOBAL             17 (NULL + list)
-                     538 LOAD_FAST                4 (e)
-                     540 LOAD_ATTR                9 (args)
-                     550 PRECALL                  1
-                     554 CALL                     1
-                     564 PRECALL                  1
-                     568 CALL                     1
-                     578 POP_TOP
-         
-         261         580 LOAD_CONST               3 ('(OperationalError) no such column:')
-                     582 LOAD_FAST                4 (e)
-                     584 LOAD_ATTR                9 (args)
-                     594 LOAD_CONST               4 (0)
-                     596 BINARY_SUBSCR
-                     606 CONTAINS_OP              0
-                     608 POP_JUMP_FORWARD_IF_FALSE    22 (to 654)
-         
-         262         610 LOAD_FAST                1 (errors)
-                     612 LOAD_METHOD             19 (append)
-                     634 LOAD_CONST               5 ('Click <a href="?fix_errors">here</a> if you would like to try to automatically add this column. Alternatively, you can drop the table and it will be recreated.')
-                     636 PRECALL                  1
-                     640 CALL                     1
-                     650 POP_TOP
-                     652 JUMP_FORWARD            36 (to 726)
-         
-         264     >>  654 LOAD_CONST               6 ('(OperationalError) no such table:')
-                     656 LOAD_FAST                4 (e)
-                     658 LOAD_ATTR                9 (args)
-                     668 LOAD_CONST               4 (0)
-                     670 BINARY_SUBSCR
-                     680 CONTAINS_OP              0
-                     682 POP_JUMP_FORWARD_IF_FALSE    21 (to 726)
-         
-         265         684 LOAD_FAST                1 (errors)
-                     686 LOAD_METHOD             19 (append)
-                     708 LOAD_CONST               7 ('Click <a href="?fix_errors">here</a> if you would like to try to automatically create this table. Alternatively, you can restart the server and it will be created.')
-                     710 PRECALL                  1
-                     714 CALL                     1
-                     724 POP_TOP
-                 >>  726 POP_EXCEPT
-                     728 LOAD_CONST               0 (None)
-                     730 STORE_FAST               4 (e)
-                     732 DELETE_FAST              4 (e)
-                     734 JUMP_FORWARD             8 (to 752)
-                 >>  736 LOAD_CONST               0 (None)
-                     738 STORE_FAST               4 (e)
-                     740 DELETE_FAST              4 (e)
-                     742 RERAISE                  1
-         
-         259     >>  744 RERAISE                  0
-                 >>  746 COPY                     3
-                     748 POP_EXCEPT
-                     750 RERAISE                  1
-         
-         268     >>  752 LOAD_CONST               8 ('fix_errors')
-                     754 LOAD_GLOBAL             40 (request)
-                     766 LOAD_ATTR                9 (args)
-                     776 CONTAINS_OP              0
-                     778 EXTENDED_ARG             1
-                     780 POP_JUMP_FORWARD_IF_FALSE   292 (to 1366)
-         
-         270         782 LOAD_FAST                1 (errors)
-                     784 GET_ITER
-                 >>  786 EXTENDED_ARG             1
-                     788 FOR_ITER               288 (to 1366)
-                     790 STORE_FAST               4 (e)
-         
-         271         792 LOAD_CONST               3 ('(OperationalError) no such column:')
-                     794 LOAD_FAST                4 (e)
-                     796 CONTAINS_OP              0
-                     798 POP_JUMP_FORWARD_IF_FALSE   213 (to 1226)
-         
-         272         800 LOAD_FAST                4 (e)
-                     802 LOAD_METHOD             21 (split)
-                     824 LOAD_FAST                5 (table_name)
-                     826 LOAD_CONST               9 ('.')
-                     828 BINARY_OP                0 (+)
-                     832 PRECALL                  1
-                     836 CALL                     1
-                     846 STORE_FAST               4 (e)
-         
-         273         848 LOAD_FAST                4 (e)
-                     850 LOAD_GLOBAL             45 (NULL + len)
-                     862 LOAD_FAST                4 (e)
-                     864 PRECALL                  1
-                     868 CALL                     1
-                     878 LOAD_CONST              10 (1)
-                     880 BINARY_OP               10 (-)
-                     884 BINARY_SUBSCR
-                     894 STORE_FAST               6 (column_name)
-         
-         274         896 LOAD_GLOBAL             24 (db)
-                     908 LOAD_ATTR               15 (metadata)
-                     918 LOAD_ATTR               16 (tables)
-                     928 LOAD_FAST                5 (table_name)
-                     930 BINARY_SUBSCR
-                     940 LOAD_ATTR               23 (columns)
-                     950 LOAD_FAST                6 (column_name)
-                     952 BINARY_SUBSCR
-                     962 LOAD_ATTR               24 (type)
-                     972 STORE_FAST               7 (dataType)
-         
-         276         974 LOAD_GLOBAL             25 (NULL + db)
-                     986 LOAD_ATTR               25 (DDL)
-                     996 LOAD_GLOBAL             52 (str)
-                    1008 LOAD_METHOD             27 (format)
-                    1030 LOAD_CONST              11 ('ALTER TABLE {} ADD COLUMN {} {}')
-                    1032 LOAD_FAST                5 (table_name)
-                    1034 LOAD_FAST                6 (column_name)
-                    1036 LOAD_FAST                7 (dataType)
-                    1038 PRECALL                  4
-                    1042 CALL                     4
-                    1052 PRECALL                  1
-                    1056 CALL                     1
-                    1066 STORE_FAST               8 (add_column)
-         
-         277        1068 LOAD_GLOBAL             24 (db)
-                    1080 LOAD_ATTR               28 (engine)
-                    1090 LOAD_METHOD             29 (execute)
-                    1112 LOAD_FAST                8 (add_column)
-                    1114 PRECALL                  1
-                    1118 CALL                     1
-                    1128 POP_TOP
-         
-         279        1130 LOAD_FAST                1 (errors)
-                    1132 LOAD_METHOD             19 (append)
-                    1154 LOAD_GLOBAL             52 (str)
-                    1166 LOAD_METHOD             27 (format)
-                    1188 LOAD_CONST              12 ('{} {} was added to {}. This error should be gone when you refresh.')
-         
-         280        1190 LOAD_FAST                6 (column_name)
-                    1192 LOAD_FAST                7 (dataType)
-         
-         281        1194 LOAD_FAST                5 (table_name)
+            0x97007400000000000000000000006a01000000000000000064016b0200
+            00000072ac64027400000000000000000000006a02000000000000000076
+            00729e7407000000000000000000007400000000000000000000006a0200
+            00000000000000640219000000000000000000a6010000ab010000000000
+            00000074080000000000000000000064023c000000740a00000000000000
+            0000006a040000000000000000a006000000000000000000000000000000
+            0000000000740a000000000000000000006a070000000000000000a60100
+            00ab010000000000000000a0080000000000000000000000000000000000
+            000000740800000000000000000000640319000000000000000000a60100
+            00ab0100000000000000007d017408000000000000000000006402190000
+            000000000000007c015f090000000000000000740a000000000000000000
+            006a040000000000000000a00a0000000000000000000000000000000000
+            000000a6000000ab000000000000000000010067007d0209007417000000
+            000000000000007419000000000000000000006a0d00000000000000007c
+            00a6010000ab0100000000000000006404a6020000ab0200000000000000
+            007d037c03a00e0000000000000000000000000000000000000000a60000
+            00ab0000000000000000007d04741f000000000000000000006a10000000
+            00000000007c04a6010000ab0100000000000000007d047c03a011000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            0001006e2b23007424000000000000000000002400721e7d057427000000
+            000000000000007c056a140000000000000000a6010000ab010000000000
+            0000007d02590064007d057e056e0864007d057e05770177007803590077
+            0164057c007a0000007d067c00742b000000000000000000006a16000000
+            0000000000a6000000ab00000000000000000076009002724d0900740a00
+            0000000000000000006a040000000000000000a006000000000000000000
+            0000000000000000000000740a000000000000000000006a170000000000
+            0000006a1800000000000000007c0619000000000000000000a6010000ab
+            010000000000000000a01900000000000000000000000000000000000000
+            00a6000000ab00000000000000000001006e872300742400000000000000
+            0000002400727a7d057c02a01a0000000000000000000000000000000000
+            0000007427000000000000000000007c056a140000000000000000a60100
+            00ab010000000000000000a6010000ab010000000000000000010064067c
+            056a140000000000000000640719000000000000000000760072167c02a0
+            1b00000000000000000000000000000000000000006408a6010000ab0100
+            0000000000000001006e2464097c056a1400000000000000006407190000
+            00000000000000760072157c02a01b000000000000000000000000000000
+            0000000000640aa6010000ab0100000000000000000100590064007d057e
+            056e0864007d057e0577017700780359007701640b740000000000000000
+            0000006a14000000000000000076009001726f7c02440090015d6b7d0564
+            067c0576009001721f7c05a01c0000000000000000000000000000000000
+            0000007c06640c7a000000a6010000ab0100000000000000007d057c0574
+            3b000000000000000000007c05a6010000ab010000000000000000640d7a
+            0a0000190000000000000000007d07740a000000000000000000006a1700
+            000000000000006a1800000000000000007c06190000000000000000006a
+            1e00000000000000007c07190000000000000000006a1f00000000000000
+            007d08740b000000000000000000006a2000000000000000007442000000
+            00000000000000a022000000000000000000000000000000000000000064
+            0e7c067c077c08a6040000ab040000000000000000a6010000ab01000000
+            00000000007d09740a000000000000000000006a230000000000000000a0
+            240000000000000000000000000000000000000000a6000000ab00000000
+            000000000035007d0a7c0aa0250000000000000000000000000000000000
+            0000007c09a6010000ab0100000000000000000100740a00000000000000
+            0000006a040000000000000000a00a000000000000000000000000000000
+            0000000000a6000000ab0000000000000000000100640064006400a60200
+            00ab02000000000000000001006e0b230031007304770278035900770101
+            005900010001007c02a01b00000000000000000000000000000000000000
+            00744200000000000000000000a022000000000000000000000000000000
+            0000000000640f7c077c087c06a6040000ab040000000000000000a60100
+            00ab010000000000000000010064097c0576007240740b00000000000000
+            0000006a260000000000000000a6000000ab00000000000000000001007c
+            02a01b000000000000000000000000000000000000000074420000000000
+            0000000000a02200000000000000000000000000000000000000006410a6
+            010000ab010000000000000000a6010000ab010000000000000000010090
+            018c6d744f0000000000000000000064117c047c02ac12a6030000ab0300
+            000000000000005300
+         286           0 RESUME                   0
+         
+         289           2 LOAD_GLOBAL              0 (request)
+                      14 LOAD_ATTR                1 (method)
+                      24 LOAD_CONST               1 ('POST')
+                      26 COMPARE_OP               2 (==)
+                      32 POP_JUMP_FORWARD_IF_FALSE   172 (to 378)
+                      34 LOAD_CONST               2 ('condition')
+                      36 LOAD_GLOBAL              0 (request)
+                      48 LOAD_ATTR                2 (form)
+                      58 CONTAINS_OP              0
+                      60 POP_JUMP_FORWARD_IF_FALSE   158 (to 378)
+         
+         290          62 LOAD_GLOBAL              7 (NULL + int_or_0)
+                      74 LOAD_GLOBAL              0 (request)
+                      86 LOAD_ATTR                2 (form)
+                      96 LOAD_CONST               2 ('condition')
+                      98 BINARY_SUBSCR
+                     108 PRECALL                  1
+                     112 CALL                     1
+                     122 LOAD_GLOBAL              8 (session)
+                     134 LOAD_CONST               2 ('condition')
+                     136 STORE_SUBSCR
+         
+         292         140 LOAD_GLOBAL             10 (db)
+                     152 LOAD_ATTR                4 (session)
+                     162 LOAD_METHOD              6 (query)
+                     184 LOAD_GLOBAL             10 (db)
+                     196 LOAD_ATTR                7 (Participant)
+                     206 PRECALL                  1
+                     210 CALL                     1
+                     220 LOAD_METHOD              8 (get)
+                     242 LOAD_GLOBAL              8 (session)
+                     254 LOAD_CONST               3 ('participantID')
+                     256 BINARY_SUBSCR
+                     266 PRECALL                  1
+                     270 CALL                     1
+                     280 STORE_FAST               1 (p)
+         
+         293         282 LOAD_GLOBAL              8 (session)
+                     294 LOAD_CONST               2 ('condition')
+                     296 BINARY_SUBSCR
+                     306 LOAD_FAST                1 (p)
+                     308 STORE_ATTR               9 (condition)
+         
+         295         318 LOAD_GLOBAL             10 (db)
+                     330 LOAD_ATTR                4 (session)
+                     340 LOAD_METHOD             10 (commit)
+                     362 PRECALL                  0
+                     366 CALL                     0
+                     376 POP_TOP
+         
+         298     >>  378 BUILD_LIST               0
+                     380 STORE_FAST               2 (errors)
+         
+         300         382 NOP
+         
+         301         384 LOAD_GLOBAL             23 (NULL + open)
+                     396 LOAD_GLOBAL             25 (NULL + current_app)
+                     408 LOAD_ATTR               13 (get_questionnaire_path)
+                     418 LOAD_FAST                0 (questionnaireName)
+                     420 PRECALL                  1
+                     424 CALL                     1
+                     434 LOAD_CONST               4 ('r')
+                     436 PRECALL                  2
+                     440 CALL                     2
+                     450 STORE_FAST               3 (f)
+         
+         302         452 LOAD_FAST                3 (f)
+                     454 LOAD_METHOD             14 (read)
+                     476 PRECALL                  0
+                     480 CALL                     0
+                     490 STORE_FAST               4 (json_data)
+         
+         303         492 LOAD_GLOBAL             31 (NULL + json)
+                     504 LOAD_ATTR               16 (loads)
+                     514 LOAD_FAST                4 (json_data)
+                     516 PRECALL                  1
+                     520 CALL                     1
+                     530 STORE_FAST               4 (json_data)
          
-         279        1196 PRECALL                  4
-                    1200 CALL                     4
+         304         532 LOAD_FAST                3 (f)
+                     534 LOAD_METHOD             17 (close)
+                     556 PRECALL                  0
+                     560 CALL                     0
+                     570 POP_TOP
+                     572 JUMP_FORWARD            43 (to 660)
+                 >>  574 PUSH_EXC_INFO
+         
+         305         576 LOAD_GLOBAL             36 (Exception)
+                     588 CHECK_EXC_MATCH
+                     590 POP_JUMP_FORWARD_IF_FALSE    30 (to 652)
+                     592 STORE_FAST               5 (e)
+         
+         306         594 LOAD_GLOBAL             39 (NULL + list)
+                     606 LOAD_FAST                5 (e)
+                     608 LOAD_ATTR               20 (args)
+                     618 PRECALL                  1
+                     622 CALL                     1
+                     632 STORE_FAST               2 (errors)
+                     634 POP_EXCEPT
+                     636 LOAD_CONST               0 (None)
+                     638 STORE_FAST               5 (e)
+                     640 DELETE_FAST              5 (e)
+                     642 JUMP_FORWARD             8 (to 660)
+                 >>  644 LOAD_CONST               0 (None)
+                     646 STORE_FAST               5 (e)
+                     648 DELETE_FAST              5 (e)
+                     650 RERAISE                  1
+         
+         305     >>  652 RERAISE                  0
+                 >>  654 COPY                     3
+                     656 POP_EXCEPT
+                     658 RERAISE                  1
+         
+         308     >>  660 LOAD_CONST               5 ('questionnaire_')
+                     662 LOAD_FAST                0 (questionnaireName)
+                     664 BINARY_OP                0 (+)
+                     668 STORE_FAST               6 (table_name)
+         
+         310         670 LOAD_FAST                0 (questionnaireName)
+                     672 LOAD_GLOBAL             43 (NULL + page_list)
+                     684 LOAD_ATTR               22 (get_questionnaire_list)
+                     694 PRECALL                  0
+                     698 CALL                     0
+                     708 CONTAINS_OP              0
+                     710 EXTENDED_ARG             2
+                     712 POP_JUMP_FORWARD_IF_FALSE   589 (to 1892)
+         
+         311         714 NOP
+         
+         312         716 LOAD_GLOBAL             10 (db)
+                     728 LOAD_ATTR                4 (session)
+                     738 LOAD_METHOD              6 (query)
+                     760 LOAD_GLOBAL             10 (db)
+                     772 LOAD_ATTR               23 (metadata)
+                     782 LOAD_ATTR               24 (tables)
+                     792 LOAD_FAST                6 (table_name)
+                     794 BINARY_SUBSCR
+                     804 PRECALL                  1
+                     808 CALL                     1
+                     818 LOAD_METHOD             25 (first)
+                     840 PRECALL                  0
+                     844 CALL                     0
+                     854 POP_TOP
+                     856 JUMP_FORWARD           135 (to 1128)
+                 >>  858 PUSH_EXC_INFO
+         
+         313         860 LOAD_GLOBAL             36 (Exception)
+                     872 CHECK_EXC_MATCH
+                     874 POP_JUMP_FORWARD_IF_FALSE   122 (to 1120)
+                     876 STORE_FAST               5 (e)
+         
+         314         878 LOAD_FAST                2 (errors)
+                     880 LOAD_METHOD             26 (extend)
+                     902 LOAD_GLOBAL             39 (NULL + list)
+                     914 LOAD_FAST                5 (e)
+                     916 LOAD_ATTR               20 (args)
+                     926 PRECALL                  1
+                     930 CALL                     1
+                     940 PRECALL                  1
+                     944 CALL                     1
+                     954 POP_TOP
+         
+         315         956 LOAD_CONST               6 ('(OperationalError) no such column:')
+                     958 LOAD_FAST                5 (e)
+                     960 LOAD_ATTR               20 (args)
+                     970 LOAD_CONST               7 (0)
+                     972 BINARY_SUBSCR
+                     982 CONTAINS_OP              0
+                     984 POP_JUMP_FORWARD_IF_FALSE    22 (to 1030)
+         
+         316         986 LOAD_FAST                2 (errors)
+                     988 LOAD_METHOD             27 (append)
+                    1010 LOAD_CONST               8 ('Click <a href="?fix_errors">here</a> if you would like to try to automatically add this column. Alternatively, you can drop the table and it will be recreated.')
+                    1012 PRECALL                  1
+                    1016 CALL                     1
+                    1026 POP_TOP
+                    1028 JUMP_FORWARD            36 (to 1102)
+         
+         318     >> 1030 LOAD_CONST               9 ('(OperationalError) no such table:')
+                    1032 LOAD_FAST                5 (e)
+                    1034 LOAD_ATTR               20 (args)
+                    1044 LOAD_CONST               7 (0)
+                    1046 BINARY_SUBSCR
+                    1056 CONTAINS_OP              0
+                    1058 POP_JUMP_FORWARD_IF_FALSE    21 (to 1102)
+         
+         319        1060 LOAD_FAST                2 (errors)
+                    1062 LOAD_METHOD             27 (append)
+                    1084 LOAD_CONST              10 ('Click <a href="?fix_errors">here</a> if you would like to try to automatically create this table. Alternatively, you can restart the server and it will be created.')
+                    1086 PRECALL                  1
+                    1090 CALL                     1
+                    1100 POP_TOP
+                 >> 1102 POP_EXCEPT
+                    1104 LOAD_CONST               0 (None)
+                    1106 STORE_FAST               5 (e)
+                    1108 DELETE_FAST              5 (e)
+                    1110 JUMP_FORWARD             8 (to 1128)
+                 >> 1112 LOAD_CONST               0 (None)
+                    1114 STORE_FAST               5 (e)
+                    1116 DELETE_FAST              5 (e)
+                    1118 RERAISE                  1
+         
+         313     >> 1120 RERAISE                  0
+                 >> 1122 COPY                     3
+                    1124 POP_EXCEPT
+                    1126 RERAISE                  1
+         
+         322     >> 1128 LOAD_CONST              11 ('fix_errors')
+                    1130 LOAD_GLOBAL              0 (request)
+                    1142 LOAD_ATTR               20 (args)
+                    1152 CONTAINS_OP              0
+                    1154 EXTENDED_ARG             1
+                    1156 POP_JUMP_FORWARD_IF_FALSE   367 (to 1892)
+         
+         324        1158 LOAD_FAST                2 (errors)
+                    1160 GET_ITER
+                 >> 1162 EXTENDED_ARG             1
+                    1164 FOR_ITER               363 (to 1892)
+                    1166 STORE_FAST               5 (e)
+         
+         325        1168 LOAD_CONST               6 ('(OperationalError) no such column:')
+                    1170 LOAD_FAST                5 (e)
+                    1172 CONTAINS_OP              0
+                    1174 EXTENDED_ARG             1
+                    1176 POP_JUMP_FORWARD_IF_FALSE   287 (to 1752)
+         
+         326        1178 LOAD_FAST                5 (e)
+                    1180 LOAD_METHOD             28 (split)
+                    1202 LOAD_FAST                6 (table_name)
+                    1204 LOAD_CONST              12 ('.')
+                    1206 BINARY_OP                0 (+)
                     1210 PRECALL                  1
                     1214 CALL                     1
-                    1224 POP_TOP
+                    1224 STORE_FAST               5 (e)
          
-         283     >> 1226 LOAD_CONST               6 ('(OperationalError) no such table:')
-                    1228 LOAD_FAST                4 (e)
-                    1230 CONTAINS_OP              0
-                    1232 POP_JUMP_FORWARD_IF_FALSE    64 (to 1362)
-         
-         284        1234 LOAD_GLOBAL             25 (NULL + db)
-                    1246 LOAD_ATTR               30 (create_all)
-                    1256 PRECALL                  0
-                    1260 CALL                     0
-                    1270 POP_TOP
-         
-         285        1272 LOAD_FAST                1 (errors)
-                    1274 LOAD_METHOD             19 (append)
-                    1296 LOAD_GLOBAL             52 (str)
-                    1308 LOAD_METHOD             27 (format)
-                    1330 LOAD_CONST              13 ('The error should be gone if you refresh.')
-                    1332 PRECALL                  1
-                    1336 CALL                     1
-                    1346 PRECALL                  1
-                    1350 CALL                     1
-                    1360 POP_TOP
-                 >> 1362 EXTENDED_ARG             1
-                    1364 JUMP_BACKWARD          290 (to 786)
-         
-         287     >> 1366 LOAD_GLOBAL             63 (NULL + render_template)
-                    1378 LOAD_CONST              14 ('preview_questionnaire.html')
-         
-         288        1380 LOAD_FAST                3 (json_data)
-         
-         289        1382 LOAD_FAST                1 (errors)
-         
-         287        1384 KW_NAMES                15
-                    1386 PRECALL                  3
-                    1390 CALL                     3
-                    1400 RETURN_VALUE
+         327        1226 LOAD_FAST                5 (e)
+                    1228 LOAD_GLOBAL             59 (NULL + len)
+                    1240 LOAD_FAST                5 (e)
+                    1242 PRECALL                  1
+                    1246 CALL                     1
+                    1256 LOAD_CONST              13 (1)
+                    1258 BINARY_OP               10 (-)
+                    1262 BINARY_SUBSCR
+                    1272 STORE_FAST               7 (column_name)
+         
+         328        1274 LOAD_GLOBAL             10 (db)
+                    1286 LOAD_ATTR               23 (metadata)
+                    1296 LOAD_ATTR               24 (tables)
+                    1306 LOAD_FAST                6 (table_name)
+                    1308 BINARY_SUBSCR
+                    1318 LOAD_ATTR               30 (columns)
+                    1328 LOAD_FAST                7 (column_name)
+                    1330 BINARY_SUBSCR
+                    1340 LOAD_ATTR               31 (type)
+                    1350 STORE_FAST               8 (dataType)
+         
+         330        1352 LOAD_GLOBAL             11 (NULL + db)
+                    1364 LOAD_ATTR               32 (DDL)
+                    1374 LOAD_GLOBAL             66 (str)
+                    1386 LOAD_METHOD             34 (format)
+                    1408 LOAD_CONST              14 ('ALTER TABLE {} ADD COLUMN {} {}')
+                    1410 LOAD_FAST                6 (table_name)
+                    1412 LOAD_FAST                7 (column_name)
+                    1414 LOAD_FAST                8 (dataType)
+                    1416 PRECALL                  4
+                    1420 CALL                     4
+                    1430 PRECALL                  1
+                    1434 CALL                     1
+                    1444 STORE_FAST               9 (add_column)
+         
+         332        1446 LOAD_GLOBAL             10 (db)
+                    1458 LOAD_ATTR               35 (engine)
+                    1468 LOAD_METHOD             36 (connect)
+                    1490 PRECALL                  0
+                    1494 CALL                     0
+                    1504 BEFORE_WITH
+                    1506 STORE_FAST              10 (conn)
+         
+         333        1508 LOAD_FAST               10 (conn)
+                    1510 LOAD_METHOD             37 (execute)
+                    1532 LOAD_FAST                9 (add_column)
+                    1534 PRECALL                  1
+                    1538 CALL                     1
+                    1548 POP_TOP
+         
+         334        1550 LOAD_GLOBAL             10 (db)
+                    1562 LOAD_ATTR                4 (session)
+                    1572 LOAD_METHOD             10 (commit)
+                    1594 PRECALL                  0
+                    1598 CALL                     0
+                    1608 POP_TOP
+         
+         332        1610 LOAD_CONST               0 (None)
+                    1612 LOAD_CONST               0 (None)
+                    1614 LOAD_CONST               0 (None)
+                    1616 PRECALL                  2
+                    1620 CALL                     2
+                    1630 POP_TOP
+                    1632 JUMP_FORWARD            11 (to 1656)
+                 >> 1634 PUSH_EXC_INFO
+                    1636 WITH_EXCEPT_START
+                    1638 POP_JUMP_FORWARD_IF_TRUE     4 (to 1648)
+                    1640 RERAISE                  2
+                 >> 1642 COPY                     3
+                    1644 POP_EXCEPT
+                    1646 RERAISE                  1
+                 >> 1648 POP_TOP
+                    1650 POP_EXCEPT
+                    1652 POP_TOP
+                    1654 POP_TOP
+         
+         336     >> 1656 LOAD_FAST                2 (errors)
+                    1658 LOAD_METHOD             27 (append)
+                    1680 LOAD_GLOBAL             66 (str)
+                    1692 LOAD_METHOD             34 (format)
+                    1714 LOAD_CONST              15 ('{} {} was added to {}. This error should be gone when you refresh.')
+         
+         337        1716 LOAD_FAST                7 (column_name)
+                    1718 LOAD_FAST                8 (dataType)
+         
+         338        1720 LOAD_FAST                6 (table_name)
+         
+         336        1722 PRECALL                  4
+                    1726 CALL                     4
+                    1736 PRECALL                  1
+                    1740 CALL                     1
+                    1750 POP_TOP
+         
+         340     >> 1752 LOAD_CONST               9 ('(OperationalError) no such table:')
+                    1754 LOAD_FAST                5 (e)
+                    1756 CONTAINS_OP              0
+                    1758 POP_JUMP_FORWARD_IF_FALSE    64 (to 1888)
+         
+         341        1760 LOAD_GLOBAL             11 (NULL + db)
+                    1772 LOAD_ATTR               38 (create_all)
+                    1782 PRECALL                  0
+                    1786 CALL                     0
+                    1796 POP_TOP
+         
+         342        1798 LOAD_FAST                2 (errors)
+                    1800 LOAD_METHOD             27 (append)
+                    1822 LOAD_GLOBAL             66 (str)
+                    1834 LOAD_METHOD             34 (format)
+                    1856 LOAD_CONST              16 ('The error should be gone if you refresh.')
+                    1858 PRECALL                  1
+                    1862 CALL                     1
+                    1872 PRECALL                  1
+                    1876 CALL                     1
+                    1886 POP_TOP
+                 >> 1888 EXTENDED_ARG             1
+                    1890 JUMP_BACKWARD          365 (to 1162)
+         
+         344     >> 1892 LOAD_GLOBAL             79 (NULL + render_template)
+                    1904 LOAD_CONST              17 ('preview_questionnaire.html')
+         
+         345        1906 LOAD_FAST                4 (json_data)
+         
+         346        1908 LOAD_FAST                2 (errors)
+         
+         344        1910 KW_NAMES                18
+                    1912 PRECALL                  3
+                    1916 CALL                     3
+                    1926 RETURN_VALUE
          ExceptionTable:
-           8 to 194 -> 198 [0]
-           198 to 216 -> 278 [1] lasti
-           218 to 256 -> 268 [1] lasti
-           268 to 276 -> 278 [1] lasti
-           340 to 478 -> 482 [0]
-           482 to 500 -> 746 [1] lasti
-           502 to 724 -> 736 [1] lasti
-           736 to 744 -> 746 [1] lasti
+           384 to 570 -> 574 [0]
+           574 to 592 -> 654 [1] lasti
+           594 to 632 -> 644 [1] lasti
+           644 to 652 -> 654 [1] lasti
+           716 to 854 -> 858 [0]
+           858 to 876 -> 1122 [1] lasti
+           878 to 1100 -> 1112 [1] lasti
+           1112 to 1120 -> 1122 [1] lasti
+           1506 to 1608 -> 1634 [2] lasti
+           1634 to 1640 -> 1642 [4] lasti
+           1648 to 1648 -> 1642 [4] lasti
          consts
             None
+            'POST'
+            'condition'
+            'participantID'
             'r'
             'questionnaire_'
             '(OperationalError) no such column:'
             0
             'Click <a href="?fix_errors">here</a> if you would like to try to automatically add this column. Alternatively, you can drop the table and it will be recreated.'
             '(OperationalError) no such table:'
             'Click <a href="?fix_errors">here</a> if you would like to try to automatically create this table. Alternatively, you can restart the server and it will be created.'
@@ -2294,25 +2881,26 @@
             '.'
             1
             'ALTER TABLE {} ADD COLUMN {} {}'
             '{} {} was added to {}. This error should be gone when you refresh.'
             'The error should be gone if you refresh.'
             'preview_questionnaire.html'
             ('q', 'errors')
-         names      ('open', 'current_app', 'get_questionnaire_path', 'read', 'json', 'loads', 'close', 'Exception', 'list', 'args', 'page_list', 'get_questionnaire_list', 'db', 'session', 'query', 'metadata', 'tables', 'first', 'extend', 'append', 'request', 'split', 'len', 'columns', 'type', 'DDL', 'str', 'format', 'engine', 'execute', 'create_all', 'render_template')
-         varnames   ('questionnaireName', 'errors', 'f', 'json_data', 'e', 'table_name', 'column_name', 'dataType', 'add_column')
+         names      ('request', 'method', 'form', 'int_or_0', 'session', 'db', 'query', 'Participant', 'get', 'condition', 'commit', 'open', 'current_app', 'get_questionnaire_path', 'read', 'json', 'loads', 'close', 'Exception', 'list', 'args', 'page_list', 'get_questionnaire_list', 'metadata', 'tables', 'first', 'extend', 'append', 'split', 'len', 'columns', 'type', 'DDL', 'str', 'format', 'engine', 'connect', 'execute', 'create_all', 'render_template')
+         varnames   ('questionnaireName', 'p', 'errors', 'f', 'json_data', 'e', 'table_name', 'column_name', 'dataType', 'add_column', 'conn')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_preview_questionnaire'
-         firstlineno 241
+         firstlineno 286
          lnotab
-            0x0203040202014401280128012c0112013aff08030a022c010201900112
-            014e011e012c021e013cfa08091e020a010801300130014e025e013e023c
-            01040102fe1e04080126015e020e01020102fe
+            0x02033c014e028e0124023c03040202014401280128012c0112013aff08
+            030a022c010201900112014e011e012c021e013cfa08091e020a010a0130
+            0130014e025e023e012a013cfe2e043c01040102fe1e04080126015e020e
+            01020102fe
       '/questionnaire_html/<questionnaireName>'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -2323,59 +2911,59 @@
             0000000000000000006a0500000000000000007c03a6010000ab01000000
             00000000007d037c02a00600000000000000000000000000000000000000
             00a6000000ab00000000000000000001006e2b2300740e00000000000000
             0000002400721e7d047411000000000000000000007c046a090000000000
             000000a6010000ab0100000000000000007d01590064007d047e046e0864
             007d047e047701770078035900770174150000000000000000000064027c
             03ac03a6020000ab0200000000000000005300
-         292           0 RESUME                   0
+         349           0 RESUME                   0
          
-         295           2 BUILD_LIST               0
+         352           2 BUILD_LIST               0
                        4 STORE_FAST               1 (errors)
          
-         297           6 NOP
+         354           6 NOP
          
-         298           8 LOAD_GLOBAL              1 (NULL + open)
+         355           8 LOAD_GLOBAL              1 (NULL + open)
                       20 LOAD_GLOBAL              3 (NULL + current_app)
                       32 LOAD_ATTR                2 (get_questionnaire_path)
                       42 LOAD_FAST                0 (questionnaireName)
                       44 PRECALL                  1
                       48 CALL                     1
                       58 LOAD_CONST               1 ('r')
                       60 PRECALL                  2
                       64 CALL                     2
                       74 STORE_FAST               2 (f)
          
-         299          76 LOAD_FAST                2 (f)
+         356          76 LOAD_FAST                2 (f)
                       78 LOAD_METHOD              3 (read)
                      100 PRECALL                  0
                      104 CALL                     0
                      114 STORE_FAST               3 (json_data)
          
-         300         116 LOAD_GLOBAL              9 (NULL + json)
+         357         116 LOAD_GLOBAL              9 (NULL + json)
                      128 LOAD_ATTR                5 (loads)
                      138 LOAD_FAST                3 (json_data)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 STORE_FAST               3 (json_data)
          
-         301         156 LOAD_FAST                2 (f)
+         358         156 LOAD_FAST                2 (f)
                      158 LOAD_METHOD              6 (close)
                      180 PRECALL                  0
                      184 CALL                     0
                      194 POP_TOP
                      196 JUMP_FORWARD            43 (to 284)
                  >>  198 PUSH_EXC_INFO
          
-         302         200 LOAD_GLOBAL             14 (Exception)
+         359         200 LOAD_GLOBAL             14 (Exception)
                      212 CHECK_EXC_MATCH
                      214 POP_JUMP_FORWARD_IF_FALSE    30 (to 276)
                      216 STORE_FAST               4 (e)
          
-         303         218 LOAD_GLOBAL             17 (NULL + list)
+         360         218 LOAD_GLOBAL             17 (NULL + list)
                      230 LOAD_FAST                4 (e)
                      232 LOAD_ATTR                9 (args)
                      242 PRECALL                  1
                      246 CALL                     1
                      256 STORE_FAST               1 (errors)
                      258 POP_EXCEPT
                      260 LOAD_CONST               0 (None)
@@ -2383,20 +2971,20 @@
                      264 DELETE_FAST              4 (e)
                      266 JUMP_FORWARD             8 (to 284)
                  >>  268 LOAD_CONST               0 (None)
                      270 STORE_FAST               4 (e)
                      272 DELETE_FAST              4 (e)
                      274 RERAISE                  1
          
-         302     >>  276 RERAISE                  0
+         359     >>  276 RERAISE                  0
                  >>  278 COPY                     3
                      280 POP_EXCEPT
                      282 RERAISE                  1
          
-         305     >>  284 LOAD_GLOBAL             21 (NULL + render_template)
+         362     >>  284 LOAD_GLOBAL             21 (NULL + render_template)
                      296 LOAD_CONST               2 ('preview_questionnaire_simple.html')
                      298 LOAD_FAST                3 (json_data)
                      300 KW_NAMES                 3
                      302 PRECALL                  2
                      306 CALL                     2
                      316 RETURN_VALUE
          ExceptionTable:
@@ -2411,15 +2999,15 @@
             ('q',)
          names      ('open', 'current_app', 'get_questionnaire_path', 'read', 'json', 'loads', 'close', 'Exception', 'list', 'args', 'render_template')
          varnames   ('questionnaireName', 'errors', 'f', 'json_data', 'e')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_questionnaire_html'
-         firstlineno 292
+         firstlineno 349
          lnotab 0x0203040202014401280128012c0112013aff0803
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 10
          flags     : 3
          code
@@ -2439,22 +3027,22 @@
             00000000000000000000006404a6010000ab01000000000000000073157c
             05a00d00000000000000000000000000000000000000006405a6010000ab
             010000000000000000720264067d057c046a0e00000000000000007c05a0
             0f0000000000000000000000000000000000000000a6000000ab00000000
             000000000064079c027d067c03a010000000000000000000000000000000
             00000000007c06a6010000ab01000000000000000001008c747c037c0166
             025300
-         343           0 RESUME                   0
+         400           0 RESUME                   0
          
-         344           2 LOAD_CONST               0 (None)
+         401           2 LOAD_CONST               0 (None)
                        4 STORE_FAST               1 (rows)
          
-         345           6 NOP
+         402           6 NOP
          
-         346           8 LOAD_GLOBAL              0 (db)
+         403           8 LOAD_GLOBAL              0 (db)
                       20 LOAD_ATTR                1 (session)
                       30 LOAD_METHOD              2 (query)
                       52 LOAD_GLOBAL              0 (db)
                       64 LOAD_ATTR                3 (metadata)
                       74 LOAD_ATTR                4 (tables)
                       84 LOAD_FAST                0 (tableName)
                       86 BINARY_SUBSCR
@@ -2463,20 +3051,20 @@
                      110 LOAD_METHOD              5 (all)
                      132 PRECALL                  0
                      136 CALL                     0
                      146 STORE_FAST               1 (rows)
                      148 JUMP_FORWARD            61 (to 272)
                  >>  150 PUSH_EXC_INFO
          
-         347         152 LOAD_GLOBAL             12 (Exception)
+         404         152 LOAD_GLOBAL             12 (Exception)
                      164 CHECK_EXC_MATCH
                      166 POP_JUMP_FORWARD_IF_FALSE    48 (to 264)
                      168 STORE_FAST               2 (e)
          
-         348         170 LOAD_GLOBAL             15 (NULL + render_template)
+         405         170 LOAD_GLOBAL             15 (NULL + render_template)
                      182 LOAD_CONST               1 ('table_view.html')
                      184 LOAD_CONST               2 ('')
                      186 LOAD_CONST               2 ('')
                      188 LOAD_CONST               2 ('')
                      190 LOAD_GLOBAL             17 (NULL + list)
                      202 LOAD_FAST                2 (e)
                      204 LOAD_ATTR                9 (args)
@@ -2492,74 +3080,74 @@
                      252 DELETE_FAST              2 (e)
                      254 RETURN_VALUE
                  >>  256 LOAD_CONST               0 (None)
                      258 STORE_FAST               2 (e)
                      260 DELETE_FAST              2 (e)
                      262 RERAISE                  1
          
-         347     >>  264 RERAISE                  0
+         404     >>  264 RERAISE                  0
                  >>  266 COPY                     3
                      268 POP_EXCEPT
                      270 RERAISE                  1
          
-         350     >>  272 BUILD_LIST               0
+         407     >>  272 BUILD_LIST               0
                      274 STORE_FAST               3 (columns)
          
-         352         276 LOAD_GLOBAL              0 (db)
+         409         276 LOAD_GLOBAL              0 (db)
                      288 LOAD_ATTR                3 (metadata)
                      298 LOAD_ATTR                4 (tables)
                      308 LOAD_FAST                0 (tableName)
                      310 BINARY_SUBSCR
                      320 LOAD_ATTR               10 (columns)
                      330 GET_ITER
                  >>  332 FOR_ITER               115 (to 564)
                      334 STORE_FAST               4 (c)
          
-         353         336 LOAD_GLOBAL             23 (NULL + str)
+         410         336 LOAD_GLOBAL             23 (NULL + str)
                      348 LOAD_FAST                4 (c)
                      350 LOAD_ATTR               12 (type)
                      360 PRECALL                  1
                      364 CALL                     1
                      374 STORE_FAST               5 (type)
          
-         354         376 LOAD_FAST                5 (type)
+         411         376 LOAD_FAST                5 (type)
                      378 LOAD_METHOD             13 (startswith)
                      400 LOAD_CONST               4 ('VARCHAR')
                      402 PRECALL                  1
                      406 CALL                     1
                      416 POP_JUMP_FORWARD_IF_TRUE    21 (to 460)
                      418 LOAD_FAST                5 (type)
                      420 LOAD_METHOD             13 (startswith)
                      442 LOAD_CONST               5 ('TEXT')
                      444 PRECALL                  1
                      448 CALL                     1
                      458 POP_JUMP_FORWARD_IF_FALSE     2 (to 464)
          
-         355     >>  460 LOAD_CONST               6 ('string')
+         412     >>  460 LOAD_CONST               6 ('string')
                      462 STORE_FAST               5 (type)
          
-         357     >>  464 LOAD_FAST                4 (c)
+         414     >>  464 LOAD_FAST                4 (c)
                      466 LOAD_ATTR               14 (description)
                      476 LOAD_FAST                5 (type)
                      478 LOAD_METHOD             15 (lower)
                      500 PRECALL                  0
                      504 CALL                     0
                      514 LOAD_CONST               7 (('name', 'type'))
                      516 BUILD_CONST_KEY_MAP      2
                      518 STORE_FAST               6 (column)
          
-         359         520 LOAD_FAST                3 (columns)
+         416         520 LOAD_FAST                3 (columns)
                      522 LOAD_METHOD             16 (append)
                      544 LOAD_FAST                6 (column)
                      546 PRECALL                  1
                      550 CALL                     1
                      560 POP_TOP
                      562 JUMP_BACKWARD          116 (to 332)
          
-         361     >>  564 LOAD_FAST                3 (columns)
+         418     >>  564 LOAD_FAST                3 (columns)
                      566 LOAD_FAST                1 (rows)
                      568 BUILD_TUPLE              2
                      570 RETURN_VALUE
          ExceptionTable:
            8 to 146 -> 150 [0]
            150 to 168 -> 266 [1] lasti
            170 to 242 -> 256 [1] lasti
@@ -2576,37 +3164,37 @@
             ('name', 'type')
          names      ('db', 'session', 'query', 'metadata', 'tables', 'all', 'Exception', 'render_template', 'list', 'args', 'columns', 'str', 'type', 'startswith', 'description', 'lower', 'append')
          varnames   ('tableName', 'rows', 'e', 'columns', 'c', 'type', 'column')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'table_data'
-         firstlineno 343
+         firstlineno 400
          lnotab 0x020104010201900112015eff080304023c0128015401040238022c02
       '/table_view/<tableName>'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             005c0200007d017d0274030000000000000000000064017c007c027c01ac
             02a6040000ab0400000000000000005300
-         364           0 RESUME                   0
+         421           0 RESUME                   0
          
-         367           2 LOAD_GLOBAL              1 (NULL + table_data)
+         424           2 LOAD_GLOBAL              1 (NULL + table_data)
                       14 LOAD_FAST                0 (tableName)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 UNPACK_SEQUENCE          2
                       34 STORE_FAST               1 (columns)
                       36 STORE_FAST               2 (rows)
          
-         368          38 LOAD_GLOBAL              3 (NULL + render_template)
+         425          38 LOAD_GLOBAL              3 (NULL + render_template)
                       50 LOAD_CONST               1 ('table_view.html')
                       52 LOAD_FAST                0 (tableName)
                       54 LOAD_FAST                2 (rows)
                       56 LOAD_FAST                1 (columns)
                       58 KW_NAMES                 2
                       60 PRECALL                  4
                       64 CALL                     4
@@ -2617,37 +3205,37 @@
             ('tableName', 'rows', 'columns')
          names      ('table_data', 'render_template')
          varnames   ('tableName', 'columns', 'rows')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_table_view'
-         firstlineno 364
+         firstlineno 421
          lnotab 0x02032401
       '/table_ajax/<tableName>'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             005c0200007d017d0274030000000000000000000064017c027c01ac02a6
             030000ab0300000000000000005300
-         371           0 RESUME                   0
+         428           0 RESUME                   0
          
-         374           2 LOAD_GLOBAL              1 (NULL + table_data)
+         431           2 LOAD_GLOBAL              1 (NULL + table_data)
                       14 LOAD_FAST                0 (tableName)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 UNPACK_SEQUENCE          2
                       34 STORE_FAST               1 (columns)
                       36 STORE_FAST               2 (rows)
          
-         375          38 LOAD_GLOBAL              3 (NULL + render_template)
+         432          38 LOAD_GLOBAL              3 (NULL + render_template)
                       50 LOAD_CONST               1 ('table_ajax.html')
                       52 LOAD_FAST                2 (rows)
                       54 LOAD_FAST                1 (columns)
                       56 KW_NAMES                 2
                       58 PRECALL                  3
                       62 CALL                     3
                       72 RETURN_VALUE
@@ -2657,15 +3245,15 @@
             ('rows', 'columns')
          names      ('table_data', 'render_template')
          varnames   ('tableName', 'columns', 'rows')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_table_ajax'
-         firstlineno 371
+         firstlineno 428
          lnotab 0x02032401
       '/table_csv/<tableName>'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 10
          flags     : 3
@@ -2681,57 +3269,57 @@
             0000000000000000007c036406640764087c0064097a0000007409000000
             000000000000006a050000000000000000a6000000ab0000000000000000
             00a0060000000000000000000000000000000000000000640aa6010000ab
             0100000000000000007a0000007a0600006901ac0ba6030000ab03000000
             00000000005300
                        0 MAKE_CELL                5 (row)
          
-         378           2 RESUME                   0
+         435           2 RESUME                   0
          
-         381           4 LOAD_GLOBAL              1 (NULL + table_data)
+         438           4 LOAD_GLOBAL              1 (NULL + table_data)
                       16 LOAD_FAST                0 (tableName)
                       18 PRECALL                  1
                       22 CALL                     1
                       32 UNPACK_SEQUENCE          2
                       36 STORE_FAST               1 (columns)
                       38 STORE_FAST               2 (rows)
          
-         383          40 LOAD_CONST               1 ('')
+         440          40 LOAD_CONST               1 ('')
                       42 STORE_FAST               3 (csv)
          
-         384          44 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 384>)
+         441          44 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 441>)
                       46 MAKE_FUNCTION            0
                       48 LOAD_FAST                1 (columns)
                       50 GET_ITER
                       52 PRECALL                  0
                       56 CALL                     0
                       66 STORE_FAST               4 (headers)
          
-         385          68 LOAD_FAST                3 (csv)
+         442          68 LOAD_FAST                3 (csv)
                       70 LOAD_CONST               3 (',')
                       72 LOAD_METHOD              1 (join)
                       94 LOAD_FAST                4 (headers)
                       96 PRECALL                  1
                      100 CALL                     1
                      110 LOAD_CONST               4 ('\n')
                      112 BINARY_OP                0 (+)
                      116 BINARY_OP               13 (+=)
                      120 STORE_FAST               3 (csv)
          
-         387         122 LOAD_FAST                2 (rows)
+         444         122 LOAD_FAST                2 (rows)
                      124 GET_ITER
                  >>  126 FOR_ITER                54 (to 236)
                      128 STORE_DEREF              5 (row)
          
-         388         130 LOAD_FAST                3 (csv)
+         445         130 LOAD_FAST                3 (csv)
                      132 LOAD_CONST               3 (',')
                      134 LOAD_METHOD              1 (join)
                      156 LOAD_CLOSURE             5 (row)
                      158 BUILD_TUPLE              1
-                     160 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 388>)
+                     160 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 445>)
                      162 MAKE_FUNCTION            8 (closure)
                      164 LOAD_GLOBAL              5 (NULL + enumerate)
                      176 LOAD_FAST                1 (columns)
                      178 PRECALL                  1
                      182 CALL                     1
                      192 GET_ITER
                      194 PRECALL                  0
@@ -2740,55 +3328,55 @@
                      212 CALL                     1
                      222 LOAD_CONST               4 ('\n')
                      224 BINARY_OP                0 (+)
                      228 BINARY_OP               13 (+=)
                      232 STORE_FAST               3 (csv)
                      234 JUMP_BACKWARD           55 (to 126)
          
-         390     >>  236 LOAD_GLOBAL              7 (NULL + Response)
+         447     >>  236 LOAD_GLOBAL              7 (NULL + Response)
                      248 LOAD_FAST                3 (csv)
          
-         391         250 LOAD_CONST               6 ('text/csv')
+         448         250 LOAD_CONST               6 ('text/csv')
          
-         393         252 LOAD_CONST               7 ('Content-disposition')
+         450         252 LOAD_CONST               7 ('Content-disposition')
                      254 LOAD_CONST               8 ('attachment; filename=%s.csv')
          
-         394         256 LOAD_FAST                0 (tableName)
+         451         256 LOAD_FAST                0 (tableName)
                      258 LOAD_CONST               9 ('_')
                      260 BINARY_OP                0 (+)
                      264 LOAD_GLOBAL              9 (NULL + datetime)
                      276 LOAD_ATTR                5 (utcnow)
                      286 PRECALL                  0
                      290 CALL                     0
                      300 LOAD_METHOD              6 (strftime)
                      322 LOAD_CONST              10 ('%Y-%m-%d')
                      324 PRECALL                  1
                      328 CALL                     1
                      338 BINARY_OP                0 (+)
          
-         393         342 BINARY_OP                6 (%)
+         450         342 BINARY_OP                6 (%)
          
-         392         346 BUILD_MAP                1
+         449         346 BUILD_MAP                1
          
-         390         348 KW_NAMES                11
+         447         348 KW_NAMES                11
                      350 PRECALL                  3
                      354 CALL                     3
                      364 RETURN_VALUE
          consts
             None
             ''
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code
                   0x970067007c005d0a7d017c0164001900000000000000000091028c0b53
                   00
-               384           0 RESUME                   0
+               441           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                10 (to 28)
                              8 STORE_FAST               1 (c)
                             10 LOAD_FAST                1 (c)
                             12 LOAD_CONST               0 ('name')
                             14 BINARY_SUBSCR
@@ -2799,30 +3387,30 @@
                   'name'
                names      ()
                varnames   ('.0', 'c')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
                name       '<listcomp>'
-               firstlineno 384
+               firstlineno 441
                lnotab 0x
             ','
             '\n'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 19
                code
                   0x9501970067007c005d1a5c0200007d017d027401000000000000000000
                   0089037c0119000000000000000000a6010000ab01000000000000000091
                   028c1b5300
                              0 COPY_FREE_VARS           1
                
-               388           2 RESUME                   0
+               445           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                26 (to 62)
                             10 UNPACK_SEQUENCE          2
                             14 STORE_FAST               1 (i)
                             16 STORE_FAST               2 (c)
                             18 LOAD_GLOBAL              1 (NULL + escape_csv)
@@ -2837,42 +3425,282 @@
                consts
                names      ('escape_csv',)
                varnames   ('.0', 'i', 'c')
                freevars   ('row',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
                name       '<listcomp>'
-               firstlineno 388
+               firstlineno 445
                lnotab 0x
             'text/csv'
             'Content-disposition'
             'attachment; filename=%s.csv'
             '_'
             '%Y-%m-%d'
             ('mimetype', 'headers')
          names      ('table_data', 'join', 'enumerate', 'Response', 'datetime', 'utcnow', 'strftime')
          varnames   ('tableName', 'columns', 'rows', 'csv', 'headers')
          freevars   ()
          cellvars   ('row',)
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_table_csv'
-         firstlineno 378
+         firstlineno 435
          lnotab 0x0403240204011801360208016a020e010202040156ff04ff02fe
+      '/database_download'
+      code
+         argcount  : 0
+         nlocals   : 1
+         stacksize : 4
+         flags     : 3
+         code
+            0x97007400000000000000000000006a0100000000000000006401190000
+            00000000000000a002000000000000000000000000000000000000000064
+            02a6010000ab010000000000000000730264035300740000000000000000
+            0000006a010000000000000000640119000000000000000000a003000000
+            000000000000000000000000000000000064026404a6020000ab02000000
+            00000000007d007409000000000000000000007c006405ac06a6020000ab
+            0200000000000000005300
+         455           0 RESUME                   0
+         
+         458           2 LOAD_GLOBAL              0 (current_app)
+                      14 LOAD_ATTR                1 (config)
+                      24 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
+                      26 BINARY_SUBSCR
+                      36 LOAD_METHOD              2 (startswith)
+                      58 LOAD_CONST               2 ('sqlite:///')
+                      60 PRECALL                  1
+                      64 CALL                     1
+                      74 POP_JUMP_FORWARD_IF_TRUE     2 (to 80)
+         
+         459          76 LOAD_CONST               3 ('Not using a SQLite database.')
+                      78 RETURN_VALUE
+         
+         461     >>   80 LOAD_GLOBAL              0 (current_app)
+                      92 LOAD_ATTR                1 (config)
+                     102 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
+                     104 BINARY_SUBSCR
+                     114 LOAD_METHOD              3 (replace)
+                     136 LOAD_CONST               2 ('sqlite:///')
+                     138 LOAD_CONST               4 ('')
+                     140 PRECALL                  2
+                     144 CALL                     2
+                     154 STORE_FAST               0 (db_uri)
+         
+         463         156 LOAD_GLOBAL              9 (NULL + send_file)
+                     168 LOAD_FAST                0 (db_uri)
+                     170 LOAD_CONST               5 (True)
+                     172 KW_NAMES                 6
+                     174 PRECALL                  2
+                     178 CALL                     2
+                     188 RETURN_VALUE
+         consts
+            None
+            'SQLALCHEMY_DATABASE_URI'
+            'sqlite:///'
+            'Not using a SQLite database.'
+            ''
+            True
+            ('as_attachment',)
+         names      ('current_app', 'config', 'startswith', 'replace', 'send_file')
+         varnames   ('db_uri',)
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
+         name       'route_database_download'
+         firstlineno 455
+         lnotab 0x02034a0104024c02
+      '/database_delete'
+      code
+         argcount  : 0
+         nlocals   : 2
+         stacksize : 7
+         flags     : 3
+         code
+            0x97007400000000000000000000006a0100000000000000006401190000
+            00000000000000a002000000000000000000000000000000000000000064
+            02a6010000ab010000000000000000730264035300740600000000000000
+            0000006a04000000000000000064046b02000000009001723a7406000000
+            000000000000006a05000000000000000064051900000000000000000074
+            00000000000000000000006a010000000000000000640619000000000000
+            0000006b03000000007211740d0000000000000000000064076408ac09a6
+            020000ab02000000000000000053007400000000000000000000006a0100
+            00000000000000640119000000000000000000a007000000000000000000
+            00000000000000000000006402640aa6020000ab0200000000000000007d
+            007411000000000000000000007c007c00a0070000000000000000000000
+            000000000000000000640b640aa6020000ab020000000000000000640c7a
+            0000007413000000000000000000006a0a0000000000000000a6000000ab
+            000000000000000000a00b00000000000000000000000000000000000000
+            00640da6010000ab0100000000000000007a000000640b7a000000a60200
+            00ab0200000000000000000100741900000000000000000000741a000000
+            000000000000006a0e00000000000000006a0f0000000000000000a60100
+            00ab01000000000000000044005d337d01741a000000000000000000006a
+            100000000000000000a01100000000000000000000000000000000000000
+            007c01a6010000ab010000000000000000a0120000000000000000000000
+            000000000000000000a6000000ab00000000000000000001008c34741a00
+            0000000000000000006a100000000000000000a013000000000000000000
+            0000000000000000000000a6000000ab0000000000000000000100742900
+            000000000000000000742b00000000000000000000640ea6010000ab0100
+            00000000000000a6010000ab0100000000000000005300740d0000000000
+            00000000006407a6010000ab0100000000000000005300
+         466           0 RESUME                   0
+         
+         469           2 LOAD_GLOBAL              0 (current_app)
+                      14 LOAD_ATTR                1 (config)
+                      24 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
+                      26 BINARY_SUBSCR
+                      36 LOAD_METHOD              2 (startswith)
+                      58 LOAD_CONST               2 ('sqlite:///')
+                      60 PRECALL                  1
+                      64 CALL                     1
+                      74 POP_JUMP_FORWARD_IF_TRUE     2 (to 80)
+         
+         470          76 LOAD_CONST               3 ('Not using a SQLite database.')
+                      78 RETURN_VALUE
+         
+         472     >>   80 LOAD_GLOBAL              6 (request)
+                      92 LOAD_ATTR                4 (method)
+                     102 LOAD_CONST               4 ('POST')
+                     104 COMPARE_OP               2 (==)
+                     110 EXTENDED_ARG             1
+                     112 POP_JUMP_FORWARD_IF_FALSE   314 (to 742)
+         
+         473         114 LOAD_GLOBAL              6 (request)
+                     126 LOAD_ATTR                5 (form)
+                     136 LOAD_CONST               5 ('password')
+                     138 BINARY_SUBSCR
+                     148 LOAD_GLOBAL              0 (current_app)
+                     160 LOAD_ATTR                1 (config)
+                     170 LOAD_CONST               6 ('ADMIN_PASSWORD')
+                     172 BINARY_SUBSCR
+                     182 COMPARE_OP               3 (!=)
+                     188 POP_JUMP_FORWARD_IF_FALSE    17 (to 224)
+         
+         474         190 LOAD_GLOBAL             13 (NULL + render_template)
+                     202 LOAD_CONST               7 ('database_delete.html')
+                     204 LOAD_CONST               8 ('The password you entered is incorrect.')
+                     206 KW_NAMES                 9
+                     208 PRECALL                  2
+                     212 CALL                     2
+                     222 RETURN_VALUE
+         
+         476     >>  224 LOAD_GLOBAL              0 (current_app)
+                     236 LOAD_ATTR                1 (config)
+                     246 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
+                     248 BINARY_SUBSCR
+                     258 LOAD_METHOD              7 (replace)
+                     280 LOAD_CONST               2 ('sqlite:///')
+                     282 LOAD_CONST              10 ('')
+                     284 PRECALL                  2
+                     288 CALL                     2
+                     298 STORE_FAST               0 (db_uri)
+         
+         477         300 LOAD_GLOBAL             17 (NULL + copyfile)
+                     312 LOAD_FAST                0 (db_uri)
+                     314 LOAD_FAST                0 (db_uri)
+                     316 LOAD_METHOD              7 (replace)
+                     338 LOAD_CONST              11 ('.db')
+                     340 LOAD_CONST              10 ('')
+                     342 PRECALL                  2
+                     346 CALL                     2
+                     356 LOAD_CONST              12 ('_')
+                     358 BINARY_OP                0 (+)
+                     362 LOAD_GLOBAL             19 (NULL + datetime)
+                     374 LOAD_ATTR               10 (utcnow)
+                     384 PRECALL                  0
+                     388 CALL                     0
+                     398 LOAD_METHOD             11 (strftime)
+                     420 LOAD_CONST              13 ('%Y%m%d_%H%M%S')
+                     422 PRECALL                  1
+                     426 CALL                     1
+                     436 BINARY_OP                0 (+)
+                     440 LOAD_CONST              11 ('.db')
+                     442 BINARY_OP                0 (+)
+                     446 PRECALL                  2
+                     450 CALL                     2
+                     460 POP_TOP
+         
+         480         462 LOAD_GLOBAL             25 (NULL + reversed)
+                     474 LOAD_GLOBAL             26 (db)
+                     486 LOAD_ATTR               14 (metadata)
+                     496 LOAD_ATTR               15 (sorted_tables)
+                     506 PRECALL                  1
+                     510 CALL                     1
+                     520 GET_ITER
+                 >>  522 FOR_ITER                51 (to 626)
+                     524 STORE_FAST               1 (tbl)
+         
+         481         526 LOAD_GLOBAL             26 (db)
+                     538 LOAD_ATTR               16 (session)
+                     548 LOAD_METHOD             17 (query)
+                     570 LOAD_FAST                1 (tbl)
+                     572 PRECALL                  1
+                     576 CALL                     1
+                     586 LOAD_METHOD             18 (delete)
+                     608 PRECALL                  0
+                     612 CALL                     0
+                     622 POP_TOP
+                     624 JUMP_BACKWARD           52 (to 522)
+         
+         482     >>  626 LOAD_GLOBAL             26 (db)
+                     638 LOAD_ATTR               16 (session)
+                     648 LOAD_METHOD             19 (commit)
+                     670 PRECALL                  0
+                     674 CALL                     0
+                     684 POP_TOP
+         
+         484         686 LOAD_GLOBAL             41 (NULL + redirect)
+                     698 LOAD_GLOBAL             43 (NULL + url_for)
+                     710 LOAD_CONST              14 ('admin.route_progress')
+                     712 PRECALL                  1
+                     716 CALL                     1
+                     726 PRECALL                  1
+                     730 CALL                     1
+                     740 RETURN_VALUE
+         
+         486     >>  742 LOAD_GLOBAL             13 (NULL + render_template)
+                     754 LOAD_CONST               7 ('database_delete.html')
+                     756 PRECALL                  1
+                     760 CALL                     1
+                     770 RETURN_VALUE
+         consts
+            None
+            'SQLALCHEMY_DATABASE_URI'
+            'sqlite:///'
+            'Not using a SQLite database.'
+            'POST'
+            'password'
+            'ADMIN_PASSWORD'
+            'database_delete.html'
+            'The password you entered is incorrect.'
+            ('message',)
+            ''
+            '.db'
+            '_'
+            '%Y%m%d_%H%M%S'
+            'admin.route_progress'
+         names      ('current_app', 'config', 'startswith', 'request', 'method', 'form', 'render_template', 'replace', 'copyfile', 'datetime', 'utcnow', 'strftime', 'reversed', 'db', 'metadata', 'sorted_tables', 'session', 'query', 'delete', 'commit', 'redirect', 'url_for')
+         varnames   ('db_uri', 'tbl')
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
+         name       'route_database_delete'
+         firstlineno 466
+         lnotab 0x02034a01040222014c0122024c01a203400164013c023802
       500
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 5
          flags     : 3
          code
             0x970064017c006a0000000000000000009b0064027c006a010000000000
             0000009b0064039d055300
-         397           0 RESUME                   0
+         492           0 RESUME                   0
          
-         399           2 LOAD_CONST               1 ('<h1>Internal Server Error (500)</h1> <p>')
+         494           2 LOAD_CONST               1 ('<h1>Internal Server Error (500)</h1> <p>')
                        4 LOAD_FAST                0 (error)
                        6 LOAD_ATTR                0 (description)
                       16 FORMAT_VALUE             0
                       18 LOAD_CONST               2 ('</p><pre>')
                       20 LOAD_FAST                0 (error)
                       22 LOAD_ATTR                1 (original_exception)
                       32 FORMAT_VALUE             0
@@ -2886,24 +3714,25 @@
             '</pre>'
          names      ('description', 'original_exception')
          varnames   ('error',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'internal_error'
-         firstlineno 397
+         firstlineno 492
          lnotab 0x0202
-   names      ('sqlalchemy', 'flask', 'Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response', 'BOFS.globals', 'db', 'questionnaires', 'page_list', 'BOFS.util', 'fetch_condition_count', 'display_time', 'util', 'sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label', 'export_helpers', 'json', 'QuestionnaireResults', 'datetime', 'os', 'path', 'listdir', '__name__', 'admin', 'context_processor', 'inject_template_vars', 'route', 'admin_index', 'admin_login', 'fetch_progress', 'fetch_progress_summary', 'route_progress', 'route_progress_ajax', 'route_progress_summary_ajax', 'route_export_item_timing', 'route_export', 'route_results', 'route_preview_questionnaire', 'route_questionnaire_html', 'table_data', 'route_table_view', 'route_table_ajax', 'route_table_csv', 'errorhandler', 'internal_error')
+   names      ('sqlalchemy', 'flask', 'Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response', 'send_file', 'BOFS.globals', 'db', 'questionnaires', 'page_list', 'BOFS.util', 'fetch_condition_count', 'display_time', 'provide_consent', 'int_or_0', 'util', 'sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label', 'export_helpers', 'json', 'QuestionnaireResults', 'datetime', 'os', 'path', 'listdir', 'shutil', 'copyfile', '__name__', 'admin', 'context_processor', 'inject_template_vars', 'route', 'admin_index', 'admin_login', 'fetch_progress', 'fetch_progress_summary', 'route_progress', 'route_progress_ajax', 'route_progress_summary_ajax', 'post', 'route_update_exclude_from_count', 'route_export_item_timing', 'route_export', 'route_results', 'route_preview_questionnaire', 'route_questionnaire_html', 'table_data', 'route_table_view', 'route_table_ajax', 'route_table_csv', 'route_database_download', 'route_database_delete', 'errorhandler', 'internal_error')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108012c01140110011c010801080108010c01100220030c0104
-      ff0e010227280104ff0e010204300104ff0e010210061706172801020104
-      ff0eff0e0202092801020104ff0eff0e0202052801020104ff0eff0e0202
-      062801020104ff0eff0e02022728012c01020104ff0eff0eff0e03021e28
-      01020104ff0eff0e0202102801020104ff0eff0e0202312801020104ff0e
-      ff0e02023106152801020104ff0eff0e0202052801020104ff0eff0e0202
-      052801020104ff0eff0e020211280104ff0e01
+      0x00ff020108013001140118011c010801080108010c0110010c0220030c
+      0104ff0e01022a280104ff0e010204300104ff0e01022906170619280102
+      0104ff0eff0e0202092801020104ff0eff0e0202052801020104ff0eff0e
+      020205280104ff0e01020a2801020104ff0eff0e02022728012c01020104
+      ff0eff0eff0e0302222801020104ff0eff0e0202103001020104ff0eff0e
+      02023d2801020104ff0eff0e02023106152801020104ff0eff0e02020528
+      01020104ff0eff0e0202052801020104ff0eff0e0202122801020104ff0e
+      ff0e0202093001020104ff0eff0e020218280104ff0e01
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/export_helpers.py` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/export_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,25 +81,29 @@
         baseQuery = baseQuery.add_columns(db.literal_column(export_dict['fields'][field]).label(field))
 
     return levels, fields, baseQuery
 
 
 def add_participants_to_export(column_list: list[str],
                                export_data: dict,
-                               include_unfinished=True) -> sqlalchemy.orm.Query:
+                               include_unfinished=True,
+                               include_exluded=True) -> sqlalchemy.orm.Query:
     """
     Add participant columns to column_list and their data to export_data.
     :param column_list: A list of strings that will be the columns in the CSV export.
     :param export_data: Gets updated with data for the participants
     :return: A SQLAlchemy query.
     """
     query_participants = db.session.query(db.Participant)
     if not include_unfinished:
         query_participants = query_participants.filter(db.Participant.finished == True)
 
+    if not include_exluded:
+        query_participants = query_participants.filter(db.or_(db.Participant.excludeFromCount == False, db.Participant.excludeFromCount == None))
+
     column_list.extend([
         "participantID",
         "externalID",
         "condition",
         "duration",
         "finished"
     ])
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/login_admin.html` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/database_delete.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-{% extends "template.html" %}
-
+{% extends "template_admin.html" %}
 {% block head %}
-    <script>
-        $(document).ready(function () {
-            $("#password").jqxPasswordInput({ height: 25, width: 200, placeHolder: ""});
-            $("#submit").jqxButton({ width: 60, height: 25 });
-        });
-    </script>
 {% endblock %}
-{% block content %}
 
-    <form method="post">
+{% block content %}
+<div class="d-flex align-items-center">
+    <form method="post" class="m-auto">
 
+        <h1>Delete Database</h1>
         {% if message %}
-            <i>{{ message }}</i>
+            <div class="error-box">
+                <i>{{ message }}</i>
+            </div>
         {% endif %}
 
-        <div class="question">
-            <div class="padding">
-                <table style="margin: 0 auto;">
-                    <tr>
-                        <td style="padding-right: 10px;">Password:</td>
-                        <td><input style="width: 200px;" type="password" name="password" id="password" /></td>
-                        <td><input type="submit" id="submit" value="Login" /></td>
-                    </tr>
-                </table>
+        <h4>Please enter the password to continue</h4>
+
+        <div class="bg-body-tertiary p-3 rounded mt-3">
+            <div class="mb-3">
+                <label for="password" class="form-label">Password</label>
+                <input type="password" class="form-control" name="password" id="password">
             </div>
+            <input type="submit" id="submit" value="Delete Database" class="btn btn-primary w-100">
         </div>
-    </form>
 
+    </form>
+</div>
 {% endblock %}
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/preview_questionnaire.html` & `bride-of-frankensystem-1.9.3.4/BOFS/templates/external_id.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,75 @@
 00000000: 7b25 2065 7874 656e 6473 2022 7465 6d70  {% extends "temp
-00000010: 6c61 7465 5f61 646d 696e 2e68 746d 6c22  late_admin.html"
-00000020: 2025 7d0d 0a7b 2520 6672 6f6d 2022 7175   %}..{% from "qu
-00000030: 6573 7469 6f6e 6e61 6972 655f 6d61 6372  estionnaire_macr
-00000040: 6f2e 6874 6d6c 2220 696d 706f 7274 2063  o.html" import c
-00000050: 7265 6174 6551 7565 7374 696f 6e6e 6169  reateQuestionnai
-00000060: 7265 2077 6974 6820 636f 6e74 6578 7420  re with context 
-00000070: 257d 0d0a 7b25 2062 6c6f 636b 2068 6561  %}..{% block hea
-00000080: 6420 257d 0d0a 7b25 2065 6e64 626c 6f63  d %}..{% endbloc
-00000090: 6b20 257d 0d0a 0d0a 7b25 2062 6c6f 636b  k %}....{% block
-000000a0: 2063 6f6e 7465 6e74 2025 7d0d 0a0d 0a20   content %}.... 
-000000b0: 2020 207b 2520 6966 2028 6572 726f 7273     {% if (errors
-000000c0: 207c 206c 656e 6774 6829 203e 2030 2025   | length) > 0 %
-000000d0: 7d0d 0a20 2020 2020 2020 203c 6469 7620  }..        <div 
-000000e0: 636c 6173 733d 2265 7272 6f72 2d62 6f78  class="error-box
-000000f0: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
-00000100: 3c62 3e45 7272 6f72 7320 7765 7265 2066  <b>Errors were f
-00000110: 6f75 6e64 3c2f 623e 0d0a 2020 2020 2020  ound</b>..      
-00000120: 2020 2020 2020 3c75 6c3e 0d0a 2020 2020        <ul>..    
-00000130: 2020 2020 2020 2020 2020 2020 7b25 2066              {% f
-00000140: 6f72 2065 2069 6e20 6572 726f 7273 2025  or e in errors %
-00000150: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-00000160: 2020 203c 6c69 3e7b 7b20 6520 7c20 7361     <li>{{ e | sa
-00000170: 6665 207d 7d3c 2f6c 693e 0d0a 2020 2020  fe }}</li>..    
-00000180: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-00000190: 6e64 666f 7220 257d 0d0a 2020 2020 2020  ndfor %}..      
-000001a0: 2020 2020 2020 3c2f 756c 3e0d 0a20 2020        </ul>..   
-000001b0: 2020 2020 203c 2f64 6976 3e0d 0a20 2020       </div>..   
-000001c0: 207b 2520 656e 6469 6620 257d 0d0a 0d0a   {% endif %}....
-000001d0: 2020 2020 3c66 6f72 6d20 6964 3d22 666f      <form id="fo
-000001e0: 726d 223e 0d0a 0d0a 2020 2020 7b7b 2063  rm">....    {{ c
-000001f0: 7265 6174 6551 7565 7374 696f 6e6e 6169  reateQuestionnai
-00000200: 7265 2871 2920 7d7d 0d0a 0d0a 2020 2020  re(q) }}....    
-00000210: 3c2f 666f 726d 3e0d 0a0d 0a20 2020 203c  </form>....    <
-00000220: 6272 3e0d 0a0d 0a20 2020 203c 6469 7620  br>....    <div 
-00000230: 636c 6173 733d 2271 7565 7374 696f 6e20  class="question 
-00000240: 7061 6464 696e 6722 3e0d 0a20 2020 2020  padding">..     
-00000250: 2020 203c 6833 3e7b 7b20 712e 7469 746c     <h3>{{ q.titl
-00000260: 6520 6966 2071 2e74 6974 6c65 2065 6c73  e if q.title els
-00000270: 6520 2251 7565 7374 696f 6e6e 6169 7265  e "Questionnaire
-00000280: 204d 6574 6164 6174 6122 7d7d 3c2f 6833   Metadata"}}</h3
-00000290: 3e0d 0a0d 0a20 2020 2020 2020 203c 756c  >....        <ul
-000002a0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-000002b0: 6c69 3e3c 623e 5265 6665 7265 6e63 653a  li><b>Reference:
-000002c0: 3c2f 623e 207b 7b20 712e 7265 6665 7265  </b> {{ q.refere
-000002d0: 6e63 6520 6966 2071 2e72 6566 6572 656e  nce if q.referen
-000002e0: 6365 207d 7d3c 2f6c 693e 0d0a 2020 2020  ce }}</li>..    
-000002f0: 2020 2020 2020 2020 3c6c 693e 3c62 3e44          <li><b>D
-00000300: 4f49 3a20 3c2f 623e 207b 7b20 2827 3c61  OI: </b> {{ ('<a
-00000310: 2068 7265 663d 227b 307d 223e 7b30 7d3c   href="{0}">{0}<
-00000320: 2f61 3e27 2e66 6f72 6d61 7428 712e 646f  /a>'.format(q.do
-00000330: 6929 207c 2073 6166 6520 6966 2071 2e64  i) | safe if q.d
-00000340: 6f69 2e73 7461 7274 7377 6974 6828 2268  oi.startswith("h
-00000350: 7474 7022 2920 656c 7365 2027 3c61 2068  ttp") else '<a h
-00000360: 7265 663d 2268 7474 7073 3a2f 2f64 6f69  ref="https://doi
-00000370: 2e6f 7267 2f7b 307d 223e 6874 7470 733a  .org/{0}">https:
-00000380: 2f2f 646f 692e 6f72 672f 7b30 7d3c 2f61  //doi.org/{0}</a
-00000390: 3e27 2e66 6f72 6d61 7428 712e 646f 6929  >'.format(q.doi)
-000003a0: 207c 2073 6166 6529 2069 6620 712e 646f   | safe) if q.do
-000003b0: 6920 7d7d 3c2f 6c69 3e0d 0a20 2020 2020  i }}</li>..     
-000003c0: 2020 203c 2f75 6c3e 0d0a 2020 2020 3c2f     </ul>..    </
-000003d0: 6469 763e 0d0a 2020 2020 7b25 2069 6620  div>..    {% if 
-000003e0: 712e 7061 7274 6963 6970 616e 745f 6361  q.participant_ca
-000003f0: 6c63 756c 6174 696f 6e73 2025 7d0d 0a20  lculations %}.. 
-00000400: 2020 203c 6469 7620 636c 6173 733d 2271     <div class="q
-00000410: 7565 7374 696f 6e20 7061 6464 696e 6722  uestion padding"
-00000420: 3e0d 0a20 2020 2020 2020 203c 6833 3e50  >..        <h3>P
-00000430: 6572 2d52 6573 706f 6e73 6520 4361 6c63  er-Response Calc
-00000440: 756c 6174 696f 6e73 3c2f 6833 3e0d 0a0d  ulations</h3>...
-00000450: 0a20 2020 2020 2020 203c 756c 3e0d 0a20  .        <ul>.. 
-00000460: 2020 2020 2020 2020 2020 207b 2520 666f             {% fo
-00000470: 7220 6e61 6d65 2c20 6361 6c63 2069 6e20  r name, calc in 
-00000480: 712e 7061 7274 6963 6970 616e 745f 6361  q.participant_ca
-00000490: 6c63 756c 6174 696f 6e73 2e69 7465 6d73  lculations.items
-000004a0: 2829 2025 7d0d 0a20 2020 2020 2020 2020  () %}..         
-000004b0: 2020 203c 6c69 3e3c 623e 7b7b 206e 616d     <li><b>{{ nam
-000004c0: 6520 7d7d 3c2f 623e 3a20 3c70 7265 3e7b  e }}</b>: <pre>{
-000004d0: 7b20 6361 6c63 207d 7d3c 2f70 7265 3e3c  { calc }}</pre><
-000004e0: 2f6c 693e 0d0a 2020 2020 2020 2020 2020  /li>..          
-000004f0: 2020 7b25 2065 6e64 666f 7220 257d 0d0a    {% endfor %}..
-00000500: 2020 2020 2020 2020 3c2f 756c 3e0d 0a20          </ul>.. 
-00000510: 2020 203c 2f64 6976 3e0d 0a20 2020 207b     </div>..    {
-00000520: 2520 656e 6469 6620 257d 0d0a 0d0a 7b25  % endif %}....{%
-00000530: 2065 6e64 626c 6f63 6b20 257d             endblock %}
+00000010: 6c61 7465 2e68 746d 6c22 2025 7d0d 0a7b  late.html" %}..{
+00000020: 2520 626c 6f63 6b20 6865 6164 2025 7d0d  % block head %}.
+00000030: 0a7b 2520 656e 6462 6c6f 636b 2025 7d0d  .{% endblock %}.
+00000040: 0a0d 0a7b 2520 626c 6f63 6b20 636f 6e74  ...{% block cont
+00000050: 656e 7420 257d 0d0a 0d0a 2020 2020 2020  ent %}....      
+00000060: 2020 3c66 6f72 6d20 6964 3d22 666f 726d    <form id="form
+00000070: 2220 6d65 7468 6f64 3d22 706f 7374 223e  " method="post">
+00000080: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00000090: 3c69 3e57 656c 636f 6d65 2120 506c 6561  <i>Welcome! Plea
+000000a0: 7365 2066 696c 6c20 6f75 7420 7468 6520  se fill out the 
+000000b0: 666f 6c6c 6f77 696e 6720 696e 666f 726d  following inform
+000000c0: 6174 696f 6e20 746f 2062 6567 696e 2e3c  ation to begin.<
+000000d0: 2f69 3e3c 6272 3e0d 0a0d 0a20 2020 2020  /i><br>....     
+000000e0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+000000f0: 733d 2271 7565 7374 696f 6e22 2073 7479  s="question" sty
+00000100: 6c65 3d22 223e 0d0a 2020 2020 2020 2020  le="">..        
+00000110: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00000120: 7373 3d22 7061 6464 696e 6722 3e0d 0a20  ss="padding">.. 
+00000130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000140: 2020 203c 6833 3e50 6c65 6173 6520 656e     <h3>Please en
+00000150: 7465 7220 796f 7572 207b 7b20 636f 6e66  ter your {{ conf
+00000160: 6967 5b27 4558 5445 524e 414c 5f49 445f  ig['EXTERNAL_ID_
+00000170: 4c41 4245 4c27 5d20 7d7d 2e3c 2f68 333e  LABEL'] }}.</h3>
+00000180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000190: 2020 2020 2020 3c64 6976 3e0d 0a20 2020        <div>..   
+000001a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001b0: 2020 2020 203c 696e 7075 7420 636c 6173       <input clas
+000001c0: 733d 2266 6f72 6d2d 636f 6e74 726f 6c22  s="form-control"
+000001d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000001e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001f0: 2074 7970 653d 2274 6578 7422 0d0a 2020   type="text"..  
+00000200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000210: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00000220: 653d 226d 5475 726b 4944 220d 0a20 2020  e="mTurkID"..   
+00000230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000240: 2020 2020 2020 2020 2020 2020 6964 3d22              id="
+00000250: 6d54 7572 6b49 4422 0d0a 2020 2020 2020  mTurkID"..      
+00000260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000270: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00000280: 7769 6474 683a 2033 3030 7078 3b22 0d0a  width: 300px;"..
+00000290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000002b0: 6c61 6365 686f 6c64 6572 3d22 220d 0a20  laceholder="".. 
+000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002d0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000002e0: 2069 6620 6d54 7572 6b49 4420 213d 204e   if mTurkID != N
+000002f0: 6f6e 6520 257d 0d0a 2020 2020 2020 2020  one %}..        
+00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000310: 2020 2020 2020 2076 616c 7565 3d22 7b7b         value="{{
+00000320: 6d54 7572 6b49 447d 7d22 0d0a 2020 2020  mTurkID}}"..    
+00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000340: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+00000350: 6469 6620 257d 0d0a 2020 2020 2020 2020  dif %}..        
+00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000370: 2020 2020 2020 2072 6571 7569 7265 6420         required 
+00000380: 2f3e 0d0a 2020 2020 2020 2020 2020 2020  />..            
+00000390: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000003a0: 2063 6c61 7373 3d22 696e 7661 6c69 642d   class="invalid-
+000003b0: 6665 6564 6261 636b 223e 0d0a 2020 2020  feedback">..    
+000003c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003d0: 2020 2020 2020 2020 7b7b 2063 6f6e 6669          {{ confi
+000003e0: 675b 2745 5854 4552 4e41 4c5f 4944 5f50  g['EXTERNAL_ID_P
+000003f0: 524f 4d50 5427 5d20 7d7d 0d0a 2020 2020  ROMPT'] }}..    
+00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000410: 2020 2020 3c2f 6469 763e 0d0a 2020 2020      </div>..    
+00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000430: 3c2f 6469 763e 0d0a 2020 2020 2020 2020  </div>..        
+00000440: 2020 2020 2020 2020 3c2f 6469 763e 0d0a          </div>..
+00000450: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000460: 763e 0d0a 0d0a 2020 2020 2020 2020 7b7b  v>....        {{
+00000470: 2062 746e 436f 6e74 696e 7565 2829 207d   btnContinue() }
+00000480: 7d0d 0a0d 0a20 2020 2020 2020 203c 2f66  }....        </f
+00000490: 6f72 6d3e 0d0a 7b25 2065 6e64 626c 6f63  orm>..{% endbloc
+000004a0: 6b20 257d                                k %}
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/progress_ajax.html` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/progress_ajax.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-<table class="table table-striped" id="progress">
+<table class="table table-striped border" id="progress">
     <thead>
     <tr>
         <th scope="col" style="text-align: right; width: 50px;">PID</th>
         <th scope="col" style="text-align: left; width: 100px;">External ID</th>
         <th scope="col" style="text-align: right; width: 70px;">Condition</th>
         <th scope="col" style="text-align: center; width: 110px;">Started On</th>
         {% for page in pages %}
             <th scope="col" style="text-align: center; width: 110px;">{{ page['path'].replace("/", " ").replace("_", " ") }}</th>
         {% endfor %}
         <th scope="col" style="text-align: center; width:50px;">Finished</th>
+        <th scope="col" style="text-align: center; width:50px;">Excluded From Count</th>
         <th scope="col" style="text-align: center; width:70px;">Time Taken</th>
     </tr>
     </thead>
     <tbody>
     {% for r in progress %}
         <tr>
             <td style="text-align: right">{{ r.Participant.participantID }}</td>
@@ -25,12 +26,19 @@
                         {{ r[page['path']].display_duration() }}
                     {% endif %}
                 </td>
             {% endfor %}
             <td style="text-align: center;">
                 <input type="checkbox" disabled readonly {{ 'checked' if r.Participant.finished }}>
             </td>
+            <td style="text-align: center;">
+                <form>
+                    <input type="hidden" name="participantID" value="{{ r.Participant.participantID }}">
+                    <input type="hidden" name="excludeFromCount" value="{{ r.Participant.excludeFromCount }}">
+                    <input type="checkbox" {{ 'checked' if r.Participant.excludeFromCount }} hx-post="{{ url_for('admin.route_update_exclude_from_count') }}">
+                </form>
+            </td>
             <td style="text-align: center;">{{ r.Participant.display_duration() }}</td>
         </tr>
     {% endfor %}
     </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
                                                                                                                {{{{ ppaaggee[[''ppaatthh'']]..rreeppllaaccee((""//
-                        PPIIDD EExxtteerrnnaall IIDD                           CCoonnddiittiioonn                   SSttaarrtteedd OOnn       "",, "" ""))..rreeppllaaccee((""__"",, "" ""))            FFiinniisshheedd                    TTiimmee TTaakkeenn
+                        PPIIDD EExxtteerrnnaall IIDD                           CCoonnddiittiioonn                   SSttaarrtteedd OOnn       "",, "" ""))..rreeppllaaccee((""__"",, "" ""))            FFiinniisshheedd                     EExxcclluuddeedd FFrroomm CCoouunntt                      TTiimmee TTaakkeenn
                                                                                                                            }}}}
-{                           {                     {{ condition_num_to_label {                                  {% if r[page['path']] %} {     { 'checked' if                   {
-{                           {                     (r.Participant.condition) {                                  { r[page                   r.Participant.finished               {
-r.Participant.participantID r.Participant.mTurkID }}                        r.Participant.timeStarted.strftime ['path']].display_duration          }}>           r.Participant.display_duration
-}}                          }}                                              ('%Y-%m-%d %H:%M:%S') }}           () }} {% endif %}                                             () }}
+{                           {                                               {                                  {% if r[page['path']] %} {                                     { 'checked' if                             {
+{                           {                     {{ condition_num_to_label {                                  { r[page                       { 'checked' if       r.Participant.excludeFromCount }} hx-                 {
+r.Participant.participantID r.Participant.mTurkID (r.Participant.condition) r.Participant.timeStarted.strftime ['path']].display_duration r.Participant.finished             post="{{ url_for              r.Participant.display_duration
+}}                          }}                    }}                        ('%Y-%m-%d %H:%M:%S') }}           () }} {% endif %}                   }}>           ('admin.route_update_exclude_from_count')             () }}
+                                                                                                                                                                                   }}">
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/progress_summary_ajax.html` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/progress_summary_ajax.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 <div id="summary">
-    <div style="display: flex; flex-wrap: wrap; margin-left: -15px;" >
+    <div style="display: flex; flex-wrap: wrap; margin-left: -15px;">
         {% if (config['CONDITIONS'] | length) > 1 %}
-        <div class="question padding" style="flex-grow: 3; margin-left: 15px;">
-            <table class="table table-striped">
-                <thead>
-                <tr>
-                    <th scope="col" style="text-align: right; width: 50px;">Condition</th>
-                    <th scope="col" style="text-align: center; width: 100px;">Count</th>
-                    <th scope="col" style="text-align: center; width: 100px;">In Progress</th>
-                    <th scope="col" style="text-align: center; width: 100px;">Abandoned</th>
-                    <th scope="col" style="text-align: center; width: 100px;">Finished</th>
-                    <th scope="col" style="text-align: center; min-width: 70px;">Time Taken</th>
-                </tr>
-                </thead>
-                <tbody>
-                {% for r in summary_groups %}
+            <div class="" style="flex-grow: 3; margin-left: 15px;">
+                <table class="table table-striped border">
+                    <thead>
                     <tr>
-                        <td style="text-align: left">{{ condition_num_to_label(r.condition) }}</td>
-                        <td style="text-align: right">{{ r.count }}</td>
-                        <td style="text-align: right">{{ r.countInProgress }}</td>
-                        <td style="text-align: right">{{ r.countAbandoned }}</td>
-                        <td style="text-align: right">{{ r.countFinished }}</td>
-                        <td style="text-align: right">{{ display_time(r.minutes)  }}</td>
+                        <th scope="col" style="text-align: right; width: 50px;">Condition</th>
+                        <th scope="col" style="text-align: center; width: 100px;">Count</th>
+                        <th scope="col" style="text-align: center; width: 100px;">In Progress</th>
+                        <th scope="col" style="text-align: center; width: 100px;">Abandoned</th>
+                        <th scope="col" style="text-align: center; width: 100px;">Finished</th>
+                        <th scope="col" style="text-align: center; min-width: 70px;">Time Taken</th>
                     </tr>
-                {% endfor %}
-                </tbody>
-            </table>
-        </div>
+                    </thead>
+                    <tbody>
+                    {% for r in summary_groups %}
+                        <tr>
+                            <td style="text-align: left">{{ condition_num_to_label(r.condition) }}</td>
+                            <td style="text-align: right">{{ r.count }}</td>
+                            <td style="text-align: right">{{ r.countInProgress }}</td>
+                            <td style="text-align: right">{{ r.countAbandoned }}</td>
+                            <td style="text-align: right">{{ r.countFinished }}</td>
+                            <td style="text-align: right">{{ display_time(r.minutes) }}</td>
+                        </tr>
+                    {% endfor %}
+                    </tbody>
+                </table>
+            </div>
         {% endif %}
-        <div class="question padding" style="margin-left: 15px; flex-grow: 2">
+        <div class="" style="margin-left: 15px; flex-grow: 2">
 
             <div style="display: flex">
-                <div style="flex-grow: 1;">
-                    <h3>Summary</h3>
+                <div style="flex-grow: 1;" class="bg-body-tertiary p-3 rounded">
+                    <h4>Summary</h4>
                     <div style="display: grid; grid-template-columns: 160px auto;">
                         <b>Total Participants</b> <span>{{ summary.count }}</span>
                         <b>In Progress</b> <span>{{ summary.countInProgress }}</span>
                         <b>Abandoned</b> <span>{{ summary.countAbandoned }}</span>
                         <b>Finished</b> <span>{{ summary.countFinished }}</span>
                     </div>
                 </div>
-                <div style="flex-grow: 1; margin-left: 15px;">
+                <div style="flex-grow: 1; margin-left: 15px;" class="bg-body-tertiary p-3 rounded">
                     <div style="flex-grow: 1;">
-                    <h3>Completion Time</h3>
-                    <div style="display: grid; grid-template-columns: 120px auto;">
-                        <b>Average</b> <span>{{ display_time(summary.seconds) }}</span>
-                        <b>Minimum</b> <span>{{ display_time(summary.minSeconds) }}</span>
-                        <b>Maximum</b> <span>{{ display_time(summary.maxSeconds) }}</span>
+                        <h4>Completion Time</h4>
+                        <div style="display: grid; grid-template-columns: 120px auto;">
+                            <b>Average</b> <span>{{ display_time(summary.seconds) }}</span>
+                            <b>Minimum</b> <span>{{ display_time(summary.minSeconds) }}</span>
+                            <b>Maximum</b> <span>{{ display_time(summary.maxSeconds) }}</span>
+                        </div>
                     </div>
                 </div>
-                </div>
             </div>
         </div>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -2,13 +2,13 @@
              CCoonnddiittiioonn  CCoouunntt      IInn PPrrooggrreessss        AAbbaannddoonneedd        FFiinniisshheedd    TTiimmee TTaakkeenn
 {                      {       {                 {                {               {
 {                      {       {                 {                {               {
 condition_num_to_label r.count r.countInProgress r.countAbandoned r.countFinished display_time
 (r.condition) }}       }}      }}                }}               }}              (r.minutes)
                                                                                   }}
 {% endif %}
-******** SSuummmmaarryy ********
+****** SSuummmmaarryy ******
 TToottaall PPaarrttiicciippaannttss {{ summary.count }} IInn PPrrooggrreessss {{ summary.countInProgress
 }} AAbbaannddoonneedd {{ summary.countAbandoned }} FFiinniisshheedd {{ summary.countFinished }}
-******** CCoommpplleettiioonn TTiimmee ********
+****** CCoommpplleettiioonn TTiimmee ******
 AAvveerraaggee {{ display_time(summary.seconds) }} MMiinniimmuumm {{ display_time
 (summary.minSeconds) }} MMaaxxiimmuumm {{ display_time(summary.maxSeconds) }}
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/questionnaire_results.html` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/questionnaire_results.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/results.html` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/results.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/table_ajax.html` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/table_ajax.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<table class="table table-striped">
+<table class="table table-striped border">
     <thead>
     <tr>
         {% for c in columns %}
             {% if c.type in ['integer', 'float'] %}
                 <th scope="col" style="text-align: right;">{{ c.name }}</th>
             {% elif c.type == 'boolean' %}
                 <th scope="col" style="text-align: center;">{{ c.name }}</th>
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/templates/table_view.html` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/table_view.html`

 * *Files 21% similar despite different names*

```diff
@@ -14,15 +14,18 @@
             <li>{{ e }}</li>
             {% endfor %}
         </ul>
     </div>
 
     {% else %}
 
-    <div class="question padding table-responsive">
+    <div class="p-3">
+        <h2>{{ tableName }}</h2>
+    </div>
+    <div class="">
         {% include "table_ajax.html" %}
     </div>
 
     <div class="padding">
         <a href="{{ url_for('admin.route_table_csv', tableName=tableName) }}" class="btn btn-dark" role="button">Export as CSV <i class="fas fa-file-csv"></i></a>
     </div>
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/util.py` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 def verify_admin(f):
     """
     A decorator to be used for admin routes, which checks if the user is logged in. If not, the login page is shown.
     """
     @wraps(f)
     def decorated_function(*args, **kwargs):
         if 'loggedIn' not in session or not session['loggedIn']:
-            return redirect(url_for("admin.admin_login"))
+            return redirect(url_for("admin.admin_login") + "?r=" + getattr(f, "__name__", str(f)))
         return f(*args, **kwargs)
     return decorated_function
 
 
 def escape_csv(input):
     if isinstance(input, str):
         return str.format(u"\"{}\"", input.strip().replace("\n", " ").replace("\r", " ").replace("\"", "'"))
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/admin/views.py` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import sqlalchemy
-from flask import Blueprint, render_template, current_app, redirect, g, request, session, url_for, Response
+from flask import Blueprint, render_template, current_app, redirect, g, request, session, url_for, Response, send_file
 from BOFS.globals import db, questionnaires, page_list
-from BOFS.util import fetch_condition_count, display_time
+from BOFS.util import fetch_condition_count, display_time, provide_consent, int_or_0
 from .util import sqlalchemy_to_json, verify_admin, escape_csv, questionnaire_name_and_tag, condition_num_to_label
 from .export_helpers import *
 import json
 from .QuestionnaireResults import *
 from datetime import datetime
 from os import path, listdir
+from shutil import copyfile
 
 admin = Blueprint('admin', __name__, template_folder='templates', static_folder='static', url_prefix="/admin")
 
 
 @admin.context_processor
 def inject_template_vars():
     """
@@ -36,44 +37,72 @@
             if q.endswith(".json"):
                 questionnairesSystem.append(q.replace(".json", ""))
 
     tableNames = sorted(tableNames)
     questionnairesLive = current_app.page_list.get_questionnaire_list(True)
     questionnairesLiveUntagged = sorted(current_app.page_list.get_questionnaire_list())
     questionnairesSystem = sorted(questionnairesSystem)
+    isSqliteDb = current_app.config['SQLALCHEMY_DATABASE_URI'].startswith('sqlite:///')
+
 
     return dict(
         additionalAdminPages=additionalAdminPages,
         tableNames=tableNames,
         questionnairesLive=questionnairesLive,
         questionnairesLiveUntagged=questionnairesLiveUntagged,
         questionnairesSystem=questionnairesSystem,
         logGridClicks=current_app.config['LOG_GRID_CLICKS'],
+        isSqliteDb=isSqliteDb,
         condition_num_to_label=condition_num_to_label
     )
 
 
 @admin.route("/")
 def admin_index():
     return redirect(url_for("admin.admin_login"))
 
 
 @admin.route("/login", methods=['GET', 'POST'])
 def admin_login():
+    if 'participantID' not in session:
+        try:
+            p = provide_consent(True)  # Ensure that the previewing user is a valid user
+        except Exception as e:
+            if 'table participant has no column named excludeFromCount' in str(e):  # I added a new column and old databases won't open now. This is a workaround.
+                add_column = db.DDL("ALTER TABLE participant ADD COLUMN excludeFromCount BOOLEAN")
+                with db.engine.connect() as conn:
+                    conn.execute(add_column)
+                    db.session.commit()
+
+                return redirect(url_for("admin.admin_login"))  # This doesn't actually work... but the column gets added.
+            else:
+                raise e
+
+        p.excludeFromCount = True
+        db.session.commit()
+
     if session.get('loggedIn', False):
         return redirect(url_for("admin.route_progress"))
 
     if request.method == 'POST':
         if request.form['password'] != current_app.config['ADMIN_PASSWORD']:
             return render_template("login_admin.html", message="The password you entered is incorrect.")
         else:
             session['loggedIn'] = True
             session.modified = True
 
-        return redirect(url_for("admin.route_progress"))
+        redirect_to = url_for("admin.route_progress")
+
+        try:
+            if request.args.get('r') is not None:
+                redirect_to = url_for("admin." + request.args.get('r'))
+        except:  # Is there a better method here?
+            pass
+
+        return redirect(redirect_to)
     else:
         return render_template("login_admin.html")
 
 
 def fetch_progress():
     pages = current_app.page_list.flat_page_list()
 
@@ -101,24 +130,26 @@
     summary_groups = db.session.query(
         db.Participant.condition,
         db.func.count(db.Participant.participantID).label('count'),
         db.func.sum(db.cast(db.Participant.is_abandoned, db.Integer)).label('countAbandoned'),
         db.func.sum(db.cast(db.Participant.is_in_progress, db.Integer)).label('countInProgress'),
         db.func.sum(db.cast(db.Participant.finished, db.Integer)).label('countFinished'),
         db.func.avg(db.Participant.duration).label('minutes')). \
+        filter(db.or_(~db.Participant.excludeFromCount, db.Participant.excludeFromCount == None)). \
         group_by(db.Participant.condition).all()
 
     summary = db.session.query(
         db.func.count(db.Participant.participantID).label('count'),
         db.func.sum(db.cast(db.Participant.is_abandoned, db.Integer)).label('countAbandoned'),
         db.func.sum(db.cast(db.Participant.is_in_progress, db.Integer)).label('countInProgress'),
         db.func.sum(db.cast(db.Participant.finished, db.Integer)).label('countFinished'),
         db.func.min(db.Participant.duration).label('minSeconds'),
         db.func.max(db.Participant.duration).label('maxSeconds'),
         db.func.avg(db.Participant.duration).label('seconds')). \
+        filter(db.or_(~db.Participant.excludeFromCount, db.Participant.excludeFromCount == None)). \
         one()
 
     return summary_groups, summary
 
 
 @admin.route("/progress")
 @verify_admin
@@ -141,14 +172,24 @@
 @admin.route("/progress_summary_ajax")
 @verify_admin
 def route_progress_summary_ajax():
     summary_groups, summary = fetch_progress_summary()
     return render_template("progress_summary_ajax.html",
                            summary_groups=summary_groups, summary=summary, display_time=display_time)
 
+@admin.post("/update_exclude_from_count")
+def route_update_exclude_from_count():
+    if 'participantID' not in request.form or 'excludeFromCount' not in request.form:
+        return ""
+
+    p = db.session.query(db.Participant).get(request.form['participantID'])
+    p.excludeFromCount = not (request.form['excludeFromCount'] == 'True')
+    db.session.commit()
+
+    return Response(status=200, headers={'HX-Trigger': 'excludeChanged'})
 
 @admin.route("/export_item_timing")
 @verify_admin
 def route_export_item_timing():
     questionnaires = current_app.page_list.get_questionnaire_list(True)
     header = "participantID,mTurkID"
     output = ""
@@ -189,22 +230,25 @@
 
 @admin.route("/export")
 @admin.route("/export/download", endpoint="route_export_download")
 @verify_admin
 def route_export():
     unfinished_count = db.session.query(db.Participant). \
         filter(db.Participant.finished == False).count()  # For display only
+    excluded_count = db.session.query(db.Participant). \
+        filter(db.Participant.excludeFromCount == True).count()  # For display only
 
     include_unfinished = request.args.get('includeUnfinished', False)
     include_missing = request.args.get('includeMissing', True)
+    include_excluded = request.args.get('includeExcluded', False)
 
     column_list = []
     export_data = {}
 
-    query = add_participants_to_export(column_list, export_data, include_unfinished)
+    query = add_participants_to_export(column_list, export_data, include_unfinished, include_excluded)
     add_questionnaires_to_export(column_list, export_data, query, include_missing)
     add_custom_exports_to_export(column_list, export_data, query, include_missing)
 
     csv_string = build_export_csv(column_list, export_data)
 
     if request.base_url.endswith("/download"):
         return Response(csv_string,
@@ -213,15 +257,16 @@
                             "Content-disposition": "attachment; filename=%s.csv" %
                                                    ("export_" + datetime.utcnow().strftime("%Y-%m-%d_%H-%M"))
                         })
     else:
         return render_template("export.html",
                                data=csv_string,
                                rowCount=len(export_data),
-                               unfinishedCount=unfinished_count)
+                               unfinishedCount=unfinished_count,
+                               excludedCount=excluded_count)
 
 
 @admin.route("/results")
 @verify_admin
 def route_results():
     qList = page_list.get_questionnaire_list(include_tags=True)
     results = {}
@@ -234,17 +279,26 @@
         qResults.calc_descriptives()
 
         results[qNameAndTag] = qResults
 
     return render_template("results.html", results=results)
 
 
-@admin.route("/preview_questionnaire/<questionnaireName>")
+@admin.route("/preview_questionnaire/<questionnaireName>", methods=["GET", "POST"])
 @verify_admin
 def route_preview_questionnaire(questionnaireName):
+    if request.method == 'POST' and 'condition' in request.form:
+        session['condition'] = int_or_0(request.form['condition'])
+
+        p = db.session.query(db.Participant).get(session['participantID'])
+        p.condition = session['condition']
+
+        db.session.commit()
+
+
     errors = []
 
     try:
         f = open(current_app.get_questionnaire_path(questionnaireName), 'r')
         json_data = f.read()
         json_data = json.loads(json_data)
         f.close()
@@ -270,15 +324,18 @@
             for e in errors:
                 if "(OperationalError) no such column:" in e:
                     e = e.split(table_name + ".")
                     column_name = e[len(e) - 1]
                     dataType = db.metadata.tables[table_name].columns[column_name].type
 
                     add_column = db.DDL(str.format("ALTER TABLE {} ADD COLUMN {} {}", table_name, column_name, dataType))
-                    db.engine.execute(add_column)
+
+                    with db.engine.connect() as conn:
+                        conn.execute(add_column)
+                        db.session.commit()
 
                     errors.append(str.format(u"{} {} was added to {}. "
                                              u"This error should be gone when you refresh.", column_name, dataType,
                                              table_name))
 
                 if "(OperationalError) no such table:" in e:
                     db.create_all()
@@ -390,11 +447,49 @@
     return Response(csv,
                     mimetype="text/csv",
                     headers={
                         "Content-disposition": "attachment; filename=%s.csv" % (
                                     tableName + "_" + datetime.utcnow().strftime("%Y-%m-%d"))
                     })
 
+
+@admin.route("/database_download")
+@verify_admin
+def route_database_download():
+    if not current_app.config['SQLALCHEMY_DATABASE_URI'].startswith('sqlite:///'):
+        return "Not using a SQLite database."
+
+    db_uri = current_app.config['SQLALCHEMY_DATABASE_URI'].replace('sqlite:///', '')
+    # TODO: Do I need to do something special if the database is being written to by users?
+    return send_file(db_uri, as_attachment=True)
+
+
+@admin.route("/database_delete", methods=['GET', 'POST'])
+@verify_admin
+def route_database_delete():
+    if not current_app.config['SQLALCHEMY_DATABASE_URI'].startswith('sqlite:///'):
+        return "Not using a SQLite database."
+
+    if request.method == 'POST':
+        if request.form['password'] != current_app.config['ADMIN_PASSWORD']:
+            return render_template("database_delete.html", message="The password you entered is incorrect.")
+        else:
+            db_uri = current_app.config['SQLALCHEMY_DATABASE_URI'].replace('sqlite:///', '')
+            copyfile(db_uri, db_uri.replace('.db', '') + "_" + datetime.utcnow().strftime("%Y%m%d_%H%M%S") + ".db")  # Make a copy of the db, just in case we didn't truly want to delete everything.
+
+            # now delete everything from the database
+            for tbl in reversed(db.metadata.sorted_tables):
+                db.session.query(tbl).delete()
+            db.session.commit()
+
+        return redirect(url_for("admin.route_progress"))
+
+    return render_template("database_delete.html")
+
+    #db_uri = current_app.config['SQLALCHEMY_DATABASE_URI'].replace('sqlite:///', '')
+    #return send_file(db_uri, as_attachment=True)
+
+
 @admin.errorhandler(500)
 def internal_error(error):
     return f"<h1>Internal Server Error (500)</h1> <p>{error.description}</p><pre>{error.original_exception}</pre>"
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/bride_of_frankensystem.egg-info/PKG-INFO` & `bride-of-frankensystem-1.9.3.4/BOFS/bride_of_frankensystem.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt` & `bride-of-frankensystem-1.9.3.4/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/cli.py` & `bride-of-frankensystem-1.9.3.4/BOFS/cli.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/create_app.py` & `bride-of-frankensystem-1.9.3.4/BOFS/create_app.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/default/__pycache__/models.cpython-310.pyc` & `bride-of-frankensystem-1.9.3.4/BOFS/default/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/default/__pycache__/models.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.4/BOFS/default/__pycache__/models.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xfb450c66 (Tue Apr  2 17:52:59 2024 UTC)
-files sz: 9108
+moddate:  0x3d791366 (Mon Apr  8 04:57:33 2024 UTC)
+files sz: 9419
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d005a006d015a010100640064026c026d035a0301
@@ -96,67 +96,67 @@
                       16 LOAD_CONST               2 ('Participant')
                       18 LOAD_DEREF               0 (db)
                       20 LOAD_ATTR                0 (Model)
                       30 PRECALL                  3
                       34 CALL                     3
                       44 STORE_FAST               1 (Participant)
          
-         164          46 PUSH_NULL
+         169          46 PUSH_NULL
                       48 LOAD_BUILD_CLASS
                       50 LOAD_CLOSURE             0 (db)
                       52 BUILD_TUPLE              1
-                      54 LOAD_CONST               3 (<code object Progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 164>)
+                      54 LOAD_CONST               3 (<code object Progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 169>)
                       56 MAKE_FUNCTION            8 (closure)
                       58 LOAD_CONST               4 ('Progress')
                       60 LOAD_DEREF               0 (db)
                       62 LOAD_ATTR                0 (Model)
                       72 PRECALL                  3
                       76 CALL                     3
                       86 STORE_FAST               2 (Progress)
          
-         182          88 PUSH_NULL
+         187          88 PUSH_NULL
                       90 LOAD_BUILD_CLASS
                       92 LOAD_CLOSURE             0 (db)
                       94 BUILD_TUPLE              1
-                      96 LOAD_CONST               5 (<code object RadioGridLog, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 182>)
+                      96 LOAD_CONST               5 (<code object RadioGridLog, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 187>)
                       98 MAKE_FUNCTION            8 (closure)
                      100 LOAD_CONST               6 ('RadioGridLog')
                      102 LOAD_DEREF               0 (db)
                      104 LOAD_ATTR                0 (Model)
                      114 PRECALL                  3
                      118 CALL                     3
                      128 STORE_FAST               3 (RadioGridLog)
          
-         194         130 PUSH_NULL
+         199         130 PUSH_NULL
                      132 LOAD_BUILD_CLASS
                      134 LOAD_CLOSURE             0 (db)
                      136 BUILD_TUPLE              1
-                     138 LOAD_CONST               7 (<code object Display, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 194>)
+                     138 LOAD_CONST               7 (<code object Display, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 199>)
                      140 MAKE_FUNCTION            8 (closure)
                      142 LOAD_CONST               8 ('Display')
                      144 LOAD_DEREF               0 (db)
                      146 LOAD_ATTR                0 (Model)
                      156 PRECALL                  3
                      160 CALL                     3
                      170 STORE_FAST               4 (Display)
          
-         206         172 PUSH_NULL
+         211         172 PUSH_NULL
                      174 LOAD_BUILD_CLASS
                      176 LOAD_CLOSURE             0 (db)
                      178 BUILD_TUPLE              1
-                     180 LOAD_CONST               9 (<code object SessionStore, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 206>)
+                     180 LOAD_CONST               9 (<code object SessionStore, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 211>)
                      182 MAKE_FUNCTION            8 (closure)
                      184 LOAD_CONST              10 ('SessionStore')
                      186 LOAD_DEREF               0 (db)
                      188 LOAD_ATTR                0 (Model)
                      198 PRECALL                  3
                      202 CALL                     3
                      212 STORE_FAST               5 (SessionStore)
          
-         223         214 LOAD_FAST                1 (Participant)
+         228         214 LOAD_FAST                1 (Participant)
                      216 LOAD_FAST                2 (Progress)
                      218 LOAD_FAST                3 (RadioGridLog)
                      220 LOAD_FAST                4 (Display)
                      222 LOAD_FAST                5 (SessionStore)
                      224 BUILD_TUPLE              5
                      226 RETURN_VALUE
          consts
@@ -182,26 +182,28 @@
                   0500000000000000006402640aac07a6030000ab0300000000000000005a
                   0b9400a004000000000000000000000000000000000000000094006a0c00
                   000000000000006405650d6a0e0000000000000000ac07a6030000ab0300
                   000000000000005a0f9400a0040000000000000000000000000000000000
                   00000094006a0c00000000000000006402ac0ba6020000ab020000000000
                   0000005a109400a004000000000000000000000000000000000000000094
                   006a11000000000000000064056405ac07a6030000ab0300000000000000
-                  005a129400a00400000000000000000000000000000000000000009400a0
-                  070000000000000000000000000000000000000000640ca6010000ab0100
-                  000000000000006405640aac07a6030000ab0300000000000000005a1394
-                  00a004000000000000000000000000000000000000000094006a0c000000
-                  00000000006405650d6a0e0000000000000000ac07a6030000ab03000000
-                  00000000005a14640d84005a156419640e84015a166419640f6517660288
-                  0066016410840d5a18641a880066016412840c5a19641a641384045a1a65
-                  1b640f651c660264148404a6000000ab0000000000000000005a1d651d6a
-                  1e00000000000000008800660164158408a6000000ab0000000000000000
-                  005a1d651f8800660164168408a6000000ab0000000000000000005a2065
-                  1f8800660164178408a6000000ab0000000000000000005a21640f652266
-                  02641884045a2364115300
+                  005a129400a004000000000000000000000000000000000000000094006a
+                  11000000000000000064056405ac07a6030000ab0300000000000000005a
+                  139400a00400000000000000000000000000000000000000009400a00700
+                  00000000000000000000000000000000000000640ca6010000ab01000000
+                  00000000006405640aac07a6030000ab0300000000000000005a149400a0
+                  04000000000000000000000000000000000000000094006a0c0000000000
+                  0000006405650d6a0e0000000000000000ac07a6030000ab030000000000
+                  0000005a15640d84005a166419640e84015a176419640f65186602880066
+                  016410840d5a19641a880066016412840c5a1a641a641384045a1b651c64
+                  0f651d660264148404a6000000ab0000000000000000005a1e651e6a1f00
+                  000000000000008800660164158408a6000000ab0000000000000000005a
+                  1e65208800660164168408a6000000ab0000000000000000005a21652088
+                  00660164178408a6000000ab0000000000000000005a22640f6523660264
+                  1884045a2464115300
                              0 COPY_FREE_VARS           1
                
                 10           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create.<locals>.Participant')
                             10 STORE_NAME               2 (__qualname__)
@@ -305,126 +307,137 @@
                            556 PRECALL                  3
                            560 CALL                     3
                            570 STORE_NAME              18 (finished)
                
                 21         572 LOAD_CLASSDEREF          0 (db)
                            574 LOAD_METHOD              4 (Column)
                            596 LOAD_CLASSDEREF          0 (db)
-                           598 LOAD_METHOD              7 (String)
-                           620 LOAD_CONST              12 (36)
-                           622 PRECALL                  1
-                           626 CALL                     1
-                           636 LOAD_CONST               5 (False)
-                           638 LOAD_CONST              10 (0)
-                           640 KW_NAMES                 7
-                           642 PRECALL                  3
-                           646 CALL                     3
-                           656 STORE_NAME              19 (code)
-               
-                22         658 LOAD_CLASSDEREF          0 (db)
-                           660 LOAD_METHOD              4 (Column)
-                           682 LOAD_CLASSDEREF          0 (db)
-                           684 LOAD_ATTR               12 (DateTime)
+                           598 LOAD_ATTR               17 (Boolean)
+                           608 LOAD_CONST               5 (False)
+                           610 LOAD_CONST               5 (False)
+                           612 KW_NAMES                 7
+                           614 PRECALL                  3
+                           618 CALL                     3
+                           628 STORE_NAME              19 (excludeFromCount)
+               
+                22         630 LOAD_CLASSDEREF          0 (db)
+                           632 LOAD_METHOD              4 (Column)
+                           654 LOAD_CLASSDEREF          0 (db)
+                           656 LOAD_METHOD              7 (String)
+                           678 LOAD_CONST              12 (36)
+                           680 PRECALL                  1
+                           684 CALL                     1
                            694 LOAD_CONST               5 (False)
-                           696 LOAD_NAME               13 (datetime)
-                           698 LOAD_ATTR               14 (utcnow)
-                           708 KW_NAMES                 7
-                           710 PRECALL                  3
-                           714 CALL                     3
-                           724 STORE_NAME              20 (lastActiveOn)
-               
-                24         726 LOAD_CONST              13 (<code object table, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 24>)
-                           728 MAKE_FUNCTION            0
-                           730 STORE_NAME              21 (table)
-               
-                28         732 LOAD_CONST              25 (('',))
-                           734 LOAD_CONST              14 (<code object questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 28>)
-                           736 MAKE_FUNCTION            1 (defaults)
-                           738 STORE_NAME              22 (questionnaire)
-               
-                52         740 LOAD_CONST              25 (('',))
-                           742 LOAD_CONST              15 ('return')
-                           744 LOAD_NAME               23 (dict)
-                           746 BUILD_TUPLE              2
-                           748 LOAD_CLOSURE             0 (db)
-                           750 BUILD_TUPLE              1
-                           752 LOAD_CONST              16 (<code object questionnaire_log, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 52>)
-                           754 MAKE_FUNCTION           13 (defaults, annotations, closure)
-                           756 STORE_NAME              24 (questionnaire_log)
-               
-                76         758 LOAD_CONST              26 (('return', None))
-                           760 LOAD_CLOSURE             0 (db)
-                           762 BUILD_TUPLE              1
-                           764 LOAD_CONST              18 (<code object assign_condition, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 76>)
-                           766 MAKE_FUNCTION           12 (annotations, closure)
-                           768 STORE_NAME              25 (assign_condition)
-               
-               112         770 LOAD_CONST              26 (('return', None))
-                           772 LOAD_CONST              19 (<code object release_condition, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 112>)
-                           774 MAKE_FUNCTION            4 (annotations)
-                           776 STORE_NAME              26 (release_condition)
-               
-               116         778 LOAD_NAME               27 (hybrid_property)
-               
-               117         780 LOAD_CONST              15 ('return')
-                           782 LOAD_NAME               28 (int)
-                           784 BUILD_TUPLE              2
-                           786 LOAD_CONST              20 (<code object duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 116>)
-                           788 MAKE_FUNCTION            4 (annotations)
-               
-               116         790 PRECALL                  0
-                           794 CALL                     0
+                           696 LOAD_CONST              10 (0)
+                           698 KW_NAMES                 7
+                           700 PRECALL                  3
+                           704 CALL                     3
+                           714 STORE_NAME              20 (code)
+               
+                23         716 LOAD_CLASSDEREF          0 (db)
+                           718 LOAD_METHOD              4 (Column)
+                           740 LOAD_CLASSDEREF          0 (db)
+                           742 LOAD_ATTR               12 (DateTime)
+                           752 LOAD_CONST               5 (False)
+                           754 LOAD_NAME               13 (datetime)
+                           756 LOAD_ATTR               14 (utcnow)
+                           766 KW_NAMES                 7
+                           768 PRECALL                  3
+                           772 CALL                     3
+                           782 STORE_NAME              21 (lastActiveOn)
+               
+                25         784 LOAD_CONST              13 (<code object table, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 25>)
+                           786 MAKE_FUNCTION            0
+                           788 STORE_NAME              22 (table)
+               
+                29         790 LOAD_CONST              25 (('',))
+                           792 LOAD_CONST              14 (<code object questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 29>)
+                           794 MAKE_FUNCTION            1 (defaults)
+                           796 STORE_NAME              23 (questionnaire)
+               
+                53         798 LOAD_CONST              25 (('',))
+                           800 LOAD_CONST              15 ('return')
+                           802 LOAD_NAME               24 (dict)
+                           804 BUILD_TUPLE              2
+                           806 LOAD_CLOSURE             0 (db)
+                           808 BUILD_TUPLE              1
+                           810 LOAD_CONST              16 (<code object questionnaire_log, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 53>)
+                           812 MAKE_FUNCTION           13 (defaults, annotations, closure)
+                           814 STORE_NAME              25 (questionnaire_log)
                
-               117         804 STORE_NAME              29 (duration)
+                77         816 LOAD_CONST              26 (('return', None))
+                           818 LOAD_CLOSURE             0 (db)
+                           820 BUILD_TUPLE              1
+                           822 LOAD_CONST              18 (<code object assign_condition, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 77>)
+                           824 MAKE_FUNCTION           12 (annotations, closure)
+                           826 STORE_NAME              26 (assign_condition)
                
-               122         806 LOAD_NAME               29 (duration)
-                           808 LOAD_ATTR               30 (expression)
+               115         828 LOAD_CONST              26 (('return', None))
+                           830 LOAD_CONST              19 (<code object release_condition, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 115>)
+                           832 MAKE_FUNCTION            4 (annotations)
+                           834 STORE_NAME              27 (release_condition)
                
-               123         818 LOAD_CLOSURE             0 (db)
-                           820 BUILD_TUPLE              1
-                           822 LOAD_CONST              21 (<code object duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 122>)
-                           824 MAKE_FUNCTION            8 (closure)
+               119         836 LOAD_NAME               28 (hybrid_property)
+               
+               120         838 LOAD_CONST              15 ('return')
+                           840 LOAD_NAME               29 (int)
+                           842 BUILD_TUPLE              2
+                           844 LOAD_CONST              20 (<code object duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 119>)
+                           846 MAKE_FUNCTION            4 (annotations)
+               
+               119         848 PRECALL                  0
+                           852 CALL                     0
                
-               122         826 PRECALL                  0
-                           830 CALL                     0
+               120         862 STORE_NAME              30 (duration)
                
-               123         840 STORE_NAME              29 (duration)
+               125         864 LOAD_NAME               30 (duration)
+                           866 LOAD_ATTR               31 (expression)
                
-               129         842 LOAD_NAME               31 (declared_attr)
+               126         876 LOAD_CLOSURE             0 (db)
+                           878 BUILD_TUPLE              1
+                           880 LOAD_CONST              21 (<code object duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 125>)
+                           882 MAKE_FUNCTION            8 (closure)
                
-               130         844 LOAD_CLOSURE             0 (db)
-                           846 BUILD_TUPLE              1
-                           848 LOAD_CONST              22 (<code object is_in_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 129>)
-                           850 MAKE_FUNCTION            8 (closure)
+               125         884 PRECALL                  0
+                           888 CALL                     0
                
-               129         852 PRECALL                  0
-                           856 CALL                     0
+               126         898 STORE_NAME              30 (duration)
                
-               130         866 STORE_NAME              32 (is_in_progress)
+               132         900 LOAD_NAME               32 (declared_attr)
                
-               138         868 LOAD_NAME               31 (declared_attr)
+               133         902 LOAD_CLOSURE             0 (db)
+                           904 BUILD_TUPLE              1
+                           906 LOAD_CONST              22 (<code object is_in_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 132>)
+                           908 MAKE_FUNCTION            8 (closure)
                
-               139         870 LOAD_CLOSURE             0 (db)
-                           872 BUILD_TUPLE              1
-                           874 LOAD_CONST              23 (<code object is_abandoned, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 138>)
-                           876 MAKE_FUNCTION            8 (closure)
+               132         910 PRECALL                  0
+                           914 CALL                     0
                
-               138         878 PRECALL                  0
-                           882 CALL                     0
+               133         924 STORE_NAME              33 (is_in_progress)
                
-               139         892 STORE_NAME              33 (is_abandoned)
+               142         926 LOAD_NAME               32 (declared_attr)
                
-               147         894 LOAD_CONST              15 ('return')
-                           896 LOAD_NAME               34 (str)
-                           898 BUILD_TUPLE              2
-                           900 LOAD_CONST              24 (<code object display_duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 147>)
-                           902 MAKE_FUNCTION            4 (annotations)
-                           904 STORE_NAME              35 (display_duration)
-                           906 LOAD_CONST              17 (None)
-                           908 RETURN_VALUE
+               143         928 LOAD_CLOSURE             0 (db)
+                           930 BUILD_TUPLE              1
+                           932 LOAD_CONST              23 (<code object is_abandoned, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 142>)
+                           934 MAKE_FUNCTION            8 (closure)
+               
+               142         936 PRECALL                  0
+                           940 CALL                     0
+               
+               143         950 STORE_NAME              34 (is_abandoned)
+               
+               152         952 LOAD_CONST              15 ('return')
+                           954 LOAD_NAME               35 (str)
+                           956 BUILD_TUPLE              2
+                           958 LOAD_CONST              24 (<code object display_duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 152>)
+                           960 MAKE_FUNCTION            4 (annotations)
+                           962 STORE_NAME              36 (display_duration)
+                           964 LOAD_CONST              17 (None)
+                           966 RETURN_VALUE
                consts
                   'create.<locals>.Participant'
                   'participant'
                   True
                   ('primary_key', 'autoincrement')
                   50
                   False
@@ -437,17 +450,17 @@
                   36
                   code
                      argcount  : 2
                      nlocals   : 3
                      stacksize : 2
                      flags     : 19
                      code 0x9700640164026c006d017d02010064005300
-                      24           0 RESUME                   0
+                      25           0 RESUME                   0
                      
-                      25           2 LOAD_CONST               1 (0)
+                      26           2 LOAD_CONST               1 (0)
                                    4 LOAD_CONST               2 (('tables',))
                                    6 IMPORT_NAME              0 (BOFS.globals)
                                    8 IMPORT_FROM              1 (tables)
                                   10 STORE_FAST               2 (tables)
                                   12 POP_TOP
                                   14 LOAD_CONST               0 (None)
                                   16 RETURN_VALUE
@@ -457,15 +470,15 @@
                         ('tables',)
                      names      ('BOFS.globals', 'tables')
                      varnames   ('self', 'name', 'tables')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'table'
-                     firstlineno 24
+                     firstlineno 25
                      lnotab 0x0201
                   code
                      argcount  : 3
                      nlocals   : 8
                      stacksize : 5
                      flags     : 19
                      code
@@ -478,109 +491,109 @@
                         010000ab01000000000000000064066b020000000072087c056401190000
                         000000000000005300740b000000000000000000007c05a6010000ab0100
                         0000000000000064066b0400000000721d64007d077c0544005d167d067c
                         0781107c076a0600000000000000007c066a0600000000000000006b0400
                         00000072027c067d078c177c0753007c037c0119000000000000000000a0
                         070000000000000000000000000000000000000000a6000000ab00000000
                         00000000005300
-                      28           0 RESUME                   0
+                      29           0 RESUME                   0
                      
-                      29           2 LOAD_CONST               1 (0)
+                      30           2 LOAD_CONST               1 (0)
                                    4 LOAD_CONST               2 (('questionnaires',))
                                    6 IMPORT_NAME              0 (BOFS.globals)
                                    8 IMPORT_FROM              1 (questionnaires)
                                   10 STORE_FAST               3 (questionnaires)
                                   12 POP_TOP
                      
-                      30          14 LOAD_GLOBAL              5 (NULL + getattr)
+                      31          14 LOAD_GLOBAL              5 (NULL + getattr)
                                   26 LOAD_FAST                0 (self)
                                   28 LOAD_CONST               3 ('questionnaire_')
                                   30 LOAD_FAST                1 (name)
                                   32 BINARY_OP                0 (+)
                                   36 PRECALL                  2
                                   40 CALL                     2
                                   50 STORE_FAST               4 (qResults)
                      
-                      32          52 BUILD_LIST               0
+                      33          52 BUILD_LIST               0
                                   54 STORE_FAST               5 (toConsider)
                      
-                      34          56 LOAD_FAST                4 (qResults)
+                      35          56 LOAD_FAST                4 (qResults)
                                   58 GET_ITER
                              >>   60 FOR_ITER                51 (to 164)
                                   62 STORE_FAST               6 (result)
                      
-                      35          64 LOAD_FAST                6 (result)
+                      36          64 LOAD_FAST                6 (result)
                                   66 LOAD_ATTR                3 (tag)
                                   76 LOAD_FAST                2 (tag)
                                   78 COMPARE_OP               2 (==)
                                   84 POP_JUMP_FORWARD_IF_TRUE    17 (to 120)
                                   86 LOAD_FAST                6 (result)
                                   88 LOAD_ATTR                3 (tag)
                                   98 LOAD_CONST               4 ('0')
                                  100 COMPARE_OP               2 (==)
                                  106 POP_JUMP_FORWARD_IF_FALSE    27 (to 162)
                                  108 LOAD_FAST                2 (tag)
                                  110 LOAD_CONST               5 ('')
                                  112 COMPARE_OP               2 (==)
                                  118 POP_JUMP_FORWARD_IF_FALSE    21 (to 162)
                      
-                      36     >>  120 LOAD_FAST                5 (toConsider)
+                      37     >>  120 LOAD_FAST                5 (toConsider)
                                  122 LOAD_METHOD              4 (append)
                                  144 LOAD_FAST                6 (result)
                                  146 PRECALL                  1
                                  150 CALL                     1
                                  160 POP_TOP
                              >>  162 JUMP_BACKWARD           52 (to 60)
                      
-                      38     >>  164 LOAD_GLOBAL             11 (NULL + len)
+                      39     >>  164 LOAD_GLOBAL             11 (NULL + len)
                                  176 LOAD_FAST                5 (toConsider)
                                  178 PRECALL                  1
                                  182 CALL                     1
                                  192 LOAD_CONST               6 (1)
                                  194 COMPARE_OP               2 (==)
                                  200 POP_JUMP_FORWARD_IF_FALSE     8 (to 218)
                      
-                      39         202 LOAD_FAST                5 (toConsider)
+                      40         202 LOAD_FAST                5 (toConsider)
                                  204 LOAD_CONST               1 (0)
                                  206 BINARY_SUBSCR
                                  216 RETURN_VALUE
                      
-                      41     >>  218 LOAD_GLOBAL             11 (NULL + len)
+                      42     >>  218 LOAD_GLOBAL             11 (NULL + len)
                                  230 LOAD_FAST                5 (toConsider)
                                  232 PRECALL                  1
                                  236 CALL                     1
                                  246 LOAD_CONST               6 (1)
                                  248 COMPARE_OP               4 (>)
                                  254 POP_JUMP_FORWARD_IF_FALSE    29 (to 314)
                      
-                      42         256 LOAD_CONST               0 (None)
+                      43         256 LOAD_CONST               0 (None)
                                  258 STORE_FAST               7 (mostRecent)
                      
-                      43         260 LOAD_FAST                5 (toConsider)
+                      44         260 LOAD_FAST                5 (toConsider)
                                  262 GET_ITER
                              >>  264 FOR_ITER                22 (to 310)
                                  266 STORE_FAST               6 (result)
                      
-                      44         268 LOAD_FAST                7 (mostRecent)
+                      45         268 LOAD_FAST                7 (mostRecent)
                                  270 POP_JUMP_FORWARD_IF_NONE    16 (to 304)
                                  272 LOAD_FAST                7 (mostRecent)
                                  274 LOAD_ATTR                6 (timeEnded)
                                  284 LOAD_FAST                6 (result)
                                  286 LOAD_ATTR                6 (timeEnded)
                                  296 COMPARE_OP               4 (>)
                                  302 POP_JUMP_FORWARD_IF_FALSE     2 (to 308)
                      
-                      45     >>  304 LOAD_FAST                6 (result)
+                      46     >>  304 LOAD_FAST                6 (result)
                                  306 STORE_FAST               7 (mostRecent)
                              >>  308 JUMP_BACKWARD           23 (to 264)
                      
-                      47     >>  310 LOAD_FAST                7 (mostRecent)
+                      48     >>  310 LOAD_FAST                7 (mostRecent)
                                  312 RETURN_VALUE
                      
-                      49     >>  314 LOAD_FAST                3 (questionnaires)
+                      50     >>  314 LOAD_FAST                3 (questionnaires)
                                  316 LOAD_FAST                1 (name)
                                  318 BINARY_SUBSCR
                                  328 LOAD_METHOD              7 (create_blank)
                                  350 PRECALL                  0
                                  354 CALL                     0
                                  364 RETURN_VALUE
                      consts
@@ -593,15 +606,15 @@
                         1
                      names      ('BOFS.globals', 'questionnaires', 'getattr', 'tag', 'append', 'len', 'timeEnded', 'create_blank')
                      varnames   ('self', 'name', 'tag', 'questionnaires', 'qResults', 'toConsider', 'result', 'mostRecent')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'questionnaire'
-                     firstlineno 28
+                     firstlineno 29
                      lnotab
                         0x02010c0126020402080138012c02260110022601040108012401060204
                         02
                   'return'
                   code
                      argcount  : 3
                      nlocals   : 9
@@ -622,452 +635,463 @@
                         0000000000000000000000a6000000ab0000000000000000007d0469007d
                         057c036a0a00000000000000007d067c0444005d2f7d077c076a08000000
                         00000000007c067a0a0000a00b0000000000000000000000000000000000
                         000000a6000000ab0000000000000000007d087c076a0800000000000000
                         007d067c087c057c076a0c00000000000000003c0000008c307c055300
                                    0 COPY_FREE_VARS           1
                      
-                      52           2 RESUME                   0
+                      53           2 RESUME                   0
                      
-                      53           4 LOAD_FAST                0 (self)
+                      54           4 LOAD_FAST                0 (self)
                                    6 LOAD_METHOD              0 (questionnaire)
                                   28 LOAD_FAST                1 (name)
                                   30 LOAD_FAST                2 (tag)
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 STORE_FAST               3 (q)
                      
-                      55          48 LOAD_FAST                2 (tag)
+                      56          48 LOAD_FAST                2 (tag)
                                   50 LOAD_CONST               1 ('')
                                   52 COMPARE_OP               2 (==)
                                   58 POP_JUMP_FORWARD_IF_FALSE     2 (to 64)
                      
-                      56          60 LOAD_CONST               2 (0)
+                      57          60 LOAD_CONST               2 (0)
                                   62 STORE_FAST               2 (tag)
                      
-                      58     >>   64 LOAD_DEREF               9 (db)
+                      59     >>   64 LOAD_DEREF               9 (db)
                                   66 LOAD_ATTR                1 (session)
                                   76 LOAD_METHOD              2 (query)
                                   98 LOAD_DEREF               9 (db)
                                  100 LOAD_ATTR                3 (RadioGridLog)
                                  110 PRECALL                  1
                                  114 CALL                     1
                                  124 LOAD_METHOD              4 (filter)
                      
-                      59         146 LOAD_DEREF               9 (db)
+                      60         146 LOAD_DEREF               9 (db)
                                  148 LOAD_ATTR                3 (RadioGridLog)
                                  158 LOAD_ATTR                5 (participantID)
                                  168 LOAD_FAST                0 (self)
                                  170 LOAD_ATTR                5 (participantID)
                                  180 COMPARE_OP               2 (==)
                      
-                      60         186 LOAD_DEREF               9 (db)
+                      61         186 LOAD_DEREF               9 (db)
                                  188 LOAD_ATTR                3 (RadioGridLog)
                                  198 LOAD_ATTR                0 (questionnaire)
                                  208 LOAD_FAST                1 (name)
                                  210 COMPARE_OP               2 (==)
                      
-                      61         216 LOAD_DEREF               9 (db)
+                      62         216 LOAD_DEREF               9 (db)
                                  218 LOAD_ATTR                3 (RadioGridLog)
                                  228 LOAD_ATTR                6 (tag)
                                  238 LOAD_FAST                2 (tag)
                                  240 COMPARE_OP               2 (==)
                      
-                      58         246 PRECALL                  3
+                      59         246 PRECALL                  3
                                  250 CALL                     3
                      
-                      62         260 LOAD_METHOD              7 (order_by)
+                      63         260 LOAD_METHOD              7 (order_by)
                                  282 LOAD_DEREF               9 (db)
                                  284 LOAD_ATTR                3 (RadioGridLog)
                                  294 LOAD_ATTR                8 (timeClicked)
                                  304 PRECALL                  1
                                  308 CALL                     1
                                  318 LOAD_METHOD              9 (all)
                                  340 PRECALL                  0
                                  344 CALL                     0
                      
-                      58         354 STORE_FAST               4 (logs)
+                      59         354 STORE_FAST               4 (logs)
                      
-                      64         356 BUILD_MAP                0
+                      65         356 BUILD_MAP                0
                                  358 STORE_FAST               5 (result)
                      
-                      66         360 LOAD_FAST                3 (q)
+                      67         360 LOAD_FAST                3 (q)
                                  362 LOAD_ATTR               10 (timeStarted)
                                  372 STORE_FAST               6 (prevTime)
                      
-                      68         374 LOAD_FAST                4 (logs)
+                      69         374 LOAD_FAST                4 (logs)
                                  376 GET_ITER
                              >>  378 FOR_ITER                47 (to 474)
                                  380 STORE_FAST               7 (log)
                      
-                      69         382 LOAD_FAST                7 (log)
+                      70         382 LOAD_FAST                7 (log)
                                  384 LOAD_ATTR                8 (timeClicked)
                                  394 LOAD_FAST                6 (prevTime)
                                  396 BINARY_OP               10 (-)
                                  400 LOAD_METHOD             11 (total_seconds)
                                  422 PRECALL                  0
                                  426 CALL                     0
                                  436 STORE_FAST               8 (deltaTime)
                      
-                      70         438 LOAD_FAST                7 (log)
+                      71         438 LOAD_FAST                7 (log)
                                  440 LOAD_ATTR                8 (timeClicked)
                                  450 STORE_FAST               6 (prevTime)
                      
-                      72         452 LOAD_FAST                8 (deltaTime)
+                      73         452 LOAD_FAST                8 (deltaTime)
                                  454 LOAD_FAST                5 (result)
                                  456 LOAD_FAST                7 (log)
                                  458 LOAD_ATTR               12 (questionID)
                                  468 STORE_SUBSCR
                                  472 JUMP_BACKWARD           48 (to 378)
                      
-                      74     >>  474 LOAD_FAST                5 (result)
+                      75     >>  474 LOAD_FAST                5 (result)
                                  476 RETURN_VALUE
                      consts
                         None
                         ''
                         0
                      names      ('questionnaire', 'session', 'query', 'RadioGridLog', 'filter', 'participantID', 'tag', 'order_by', 'timeClicked', 'all', 'timeStarted', 'total_seconds', 'questionID')
                      varnames   ('self', 'name', 'tag', 'q', 'logs', 'result', 'prevTime', 'log', 'deltaTime')
                      freevars   ('db',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'questionnaire_log'
-                     firstlineno 52
+                     firstlineno 53
                      lnotab
                         0x04012c020c010402520128011e011efd0e045efc020604020e02080138
                         010e021602
                   None
                   code
                      argcount  : 1
-                     nlocals   : 10
-                     stacksize : 7
+                     nlocals   : 9
+                     stacksize : 8
                      flags     : 19
                      code
                         0x950197007401000000000000000000007402000000000000000000006a
                         020000000000000000640119000000000000000000a6010000ab01000000
-                        00000000007d017c0164026b0400000000900172c3640267017c017a0500
+                        00000000007d017c0164026b0400000000900172d9640267017c017a0500
                         007d026403a00300000000000000000000000000000000000000007c01a6
                         010000ab0100000000000000007d0374090000000000000000000064047c
-                        0164047a000000a6020000ab020000000000000000440090015d067d0474
+                        0164047a000000a6020000ab020000000000000000440090015d1e7d0474
                         02000000000000000000006a020000000000000000640519000000000000
-                        0000007259890a6a050000000000000000a0060000000000000000000000
-                        000000000000000000890a6a070000000000000000a6010000ab01000000
-                        0000000000a0080000000000000000000000000000000000000000890a6a
-                        0700000000000000006a0900000000000000007c046b0200000000a60100
-                        00ab010000000000000000a00a0000000000000000000000000000000000
-                        000000a6000000ab0000000000000000007c027c0464047a0a00003c0000
-                        006e77890a6a050000000000000000a00600000000000000000000000000
-                        00000000000000890a6a070000000000000000a6010000ab010000000000
-                        000000a0080000000000000000000000000000000000000000890aa00b00
-                        00000000000000000000000000000000000000890a6a0700000000000000
-                        006a0900000000000000007c046b0200000000890a6a0700000000000000
-                        006a0c00000000000000000f00a6020000ab020000000000000000a60100
-                        00ab010000000000000000a00a0000000000000000000000000000000000
-                        000000a6000000ab0000000000000000007c027c0464047a0a00003c0000
-                        007c036406a00300000000000000000000000000000000000000007c027c
-                        0464047a0a000019000000000000000000a6010000ab0100000000000000
-                        007a0d00007d0390018c08741b000000000000000000007c02a6010000ab
-                        0100000000000000007d0564077d067c0544005d4b7d077c02a00e000000
-                        00000000000000000000000000000000007c07a6010000ab010000000000
-                        0000007d087402000000000000000000006a020000000000000000640119
-                        0000000000000000007c08190000000000000000007d0964087c09760173
-                        0c7c0964081900000000000000000064096b0200000000720c7c0864047a
-                        0000007c005f09000000000000000001006e018c4c7c03640aa003000000
-                        00000000000000000000000000000000007c006a090000000000000000a6
-                        010000ab0100000000000000007a0d00007d03741f000000000000000000
-                        007c03a6010000ab01000000000000000001006400530064007c005f0900
-                        0000000000000064005300
+                        000000726589096a050000000000000000a0060000000000000000000000
+                        00000000000000000089096a070000000000000000a6010000ab01000000
+                        0000000000a008000000000000000000000000000000000000000089096a
+                        0700000000000000006a0900000000000000007c046b020000000089096a
+                        0700000000000000006a0a00000000000000000f00a6020000ab02000000
+                        0000000000a00b0000000000000000000000000000000000000000a60000
+                        00ab0000000000000000007c027c0464047a0a00003c0000006e8389096a
+                        050000000000000000a00600000000000000000000000000000000000000
+                        0089096a070000000000000000a6010000ab010000000000000000a00800
+                        000000000000000000000000000000000000008909a00c00000000000000
+                        0000000000000000000000000089096a0700000000000000006a09000000
+                        00000000007c046b020000000089096a0700000000000000006a0d000000
+                        00000000000f0089096a0700000000000000006a0a00000000000000000f
+                        00a6030000ab030000000000000000a6010000ab010000000000000000a0
+                        0b0000000000000000000000000000000000000000a6000000ab00000000
+                        00000000007c027c0464047a0a00003c0000007c036406a0030000000000
+                        0000000000000000000000000000007c027c0464047a0a00001900000000
+                        0000000000a6010000ab0100000000000000007a0d00007d0390018c2074
+                        1d000000000000000000007c02a6010000ab0100000000000000007d057c
+                        0544005d4b7d067c02a00f00000000000000000000000000000000000000
+                        007c06a6010000ab0100000000000000007d077402000000000000000000
+                        006a0200000000000000006401190000000000000000007c071900000000
+                        00000000007d0864077c087601730c7c0864071900000000000000000064
+                        086b0200000000720c7c0764047a0000007c005f09000000000000000001
+                        006e018c4c7c036409a00300000000000000000000000000000000000000
+                        007c006a090000000000000000a6010000ab0100000000000000007a0d00
+                        007d037421000000000000000000007c03a6010000ab0100000000000000
+                        0001006400530064007c005f09000000000000000064005300
                                    0 COPY_FREE_VARS           1
                      
-                      76           2 RESUME                   0
+                      77           2 RESUME                   0
                      
-                      77           4 LOAD_GLOBAL              1 (NULL + len)
+                      78           4 LOAD_GLOBAL              1 (NULL + len)
                                   16 LOAD_GLOBAL              2 (current_app)
                                   28 LOAD_ATTR                2 (config)
                                   38 LOAD_CONST               1 ('CONDITIONS')
                                   40 BINARY_SUBSCR
                                   50 PRECALL                  1
                                   54 CALL                     1
                                   64 STORE_FAST               1 (numConditions)
                      
-                      78          66 LOAD_FAST                1 (numConditions)
+                      79          66 LOAD_FAST                1 (numConditions)
                                   68 LOAD_CONST               2 (0)
                                   70 COMPARE_OP               4 (>)
                                   76 EXTENDED_ARG             1
-                                  78 POP_JUMP_FORWARD_IF_FALSE   451 (to 982)
+                                  78 POP_JUMP_FORWARD_IF_FALSE   473 (to 1026)
                      
-                      79          80 LOAD_CONST               2 (0)
+                      80          80 LOAD_CONST               2 (0)
                                   82 BUILD_LIST               1
                                   84 LOAD_FAST                1 (numConditions)
                                   86 BINARY_OP                5 (*)
                                   90 STORE_FAST               2 (pCount)
                      
-                      81          92 LOAD_CONST               3 ('Total conditions: {}, Counts: ')
+                      82          92 LOAD_CONST               3 ('Total conditions: {}, Counts: ')
                                   94 LOAD_METHOD              3 (format)
                                  116 LOAD_FAST                1 (numConditions)
                                  118 PRECALL                  1
                                  122 CALL                     1
                                  132 STORE_FAST               3 (printText)
                      
-                      83         134 LOAD_GLOBAL              9 (NULL + range)
+                      84         134 LOAD_GLOBAL              9 (NULL + range)
                                  146 LOAD_CONST               4 (1)
                                  148 LOAD_FAST                1 (numConditions)
                                  150 LOAD_CONST               4 (1)
                                  152 BINARY_OP                0 (+)
                                  156 PRECALL                  2
                                  160 CALL                     2
                                  170 GET_ITER
                              >>  172 EXTENDED_ARG             1
-                                 174 FOR_ITER               262 (to 700)
+                                 174 FOR_ITER               286 (to 748)
                                  176 STORE_FAST               4 (condition)
                      
-                      85         178 LOAD_GLOBAL              2 (current_app)
+                      86         178 LOAD_GLOBAL              2 (current_app)
                                  190 LOAD_ATTR                2 (config)
                                  200 LOAD_CONST               5 ('COUNTS_INCLUDE_ABANDONED')
                                  202 BINARY_SUBSCR
-                                 212 POP_JUMP_FORWARD_IF_FALSE    89 (to 392)
+                                 212 POP_JUMP_FORWARD_IF_FALSE   101 (to 416)
                      
-                      86         214 LOAD_DEREF              10 (db)
+                      87         214 LOAD_DEREF               9 (db)
                                  216 LOAD_ATTR                5 (session)
                                  226 LOAD_METHOD              6 (query)
-                                 248 LOAD_DEREF              10 (db)
+                                 248 LOAD_DEREF               9 (db)
                                  250 LOAD_ATTR                7 (Participant)
                                  260 PRECALL                  1
                                  264 CALL                     1
                      
-                      87         274 LOAD_METHOD              8 (filter)
-                                 296 LOAD_DEREF              10 (db)
+                      88         274 LOAD_METHOD              8 (filter)
+                                 296 LOAD_DEREF               9 (db)
                                  298 LOAD_ATTR                7 (Participant)
                                  308 LOAD_ATTR                9 (condition)
                                  318 LOAD_FAST                4 (condition)
                                  320 COMPARE_OP               2 (==)
-                                 326 PRECALL                  1
-                                 330 CALL                     1
                      
-                      88         340 LOAD_METHOD             10 (count)
-                                 362 PRECALL                  0
-                                 366 CALL                     0
-                     
-                      86         376 LOAD_FAST                2 (pCount)
-                                 378 LOAD_FAST                4 (condition)
-                                 380 LOAD_CONST               4 (1)
-                                 382 BINARY_OP               10 (-)
-                                 386 STORE_SUBSCR
-                                 390 JUMP_FORWARD           119 (to 630)
-                     
-                      90     >>  392 LOAD_DEREF              10 (db)
-                                 394 LOAD_ATTR                5 (session)
-                                 404 LOAD_METHOD              6 (query)
-                                 426 LOAD_DEREF              10 (db)
-                                 428 LOAD_ATTR                7 (Participant)
-                                 438 PRECALL                  1
-                                 442 CALL                     1
-                     
-                      91         452 LOAD_METHOD              8 (filter)
-                     
-                      92         474 LOAD_DEREF              10 (db)
-                                 476 LOAD_METHOD             11 (and_)
-                                 498 LOAD_DEREF              10 (db)
-                                 500 LOAD_ATTR                7 (Participant)
-                                 510 LOAD_ATTR                9 (condition)
-                                 520 LOAD_FAST                4 (condition)
-                                 522 COMPARE_OP               2 (==)
-                                 528 LOAD_DEREF              10 (db)
-                                 530 LOAD_ATTR                7 (Participant)
-                                 540 LOAD_ATTR               12 (is_abandoned)
-                                 550 UNARY_INVERT
-                                 552 PRECALL                  2
-                                 556 CALL                     2
-                     
-                      91         566 PRECALL                  1
-                                 570 CALL                     1
-                     
-                      93         580 LOAD_METHOD             10 (count)
-                                 602 PRECALL                  0
-                                 606 CALL                     0
-                     
-                      90         616 LOAD_FAST                2 (pCount)
-                                 618 LOAD_FAST                4 (condition)
-                                 620 LOAD_CONST               4 (1)
-                                 622 BINARY_OP               10 (-)
-                                 626 STORE_SUBSCR
-                     
-                      95     >>  630 LOAD_FAST                3 (printText)
-                                 632 LOAD_CONST               6 ('{}, ')
-                                 634 LOAD_METHOD              3 (format)
-                                 656 LOAD_FAST                2 (pCount)
-                                 658 LOAD_FAST                4 (condition)
-                                 660 LOAD_CONST               4 (1)
-                                 662 BINARY_OP               10 (-)
-                                 666 BINARY_SUBSCR
-                                 676 PRECALL                  1
-                                 680 CALL                     1
-                                 690 BINARY_OP               13 (+=)
-                                 694 STORE_FAST               3 (printText)
-                                 696 EXTENDED_ARG             1
-                                 698 JUMP_BACKWARD          264 (to 172)
-                     
-                      97     >>  700 LOAD_GLOBAL             27 (NULL + sorted)
-                                 712 LOAD_FAST                2 (pCount)
-                                 714 PRECALL                  1
-                                 718 CALL                     1
-                                 728 STORE_FAST               5 (pCountSorted)
-                     
-                      98         730 LOAD_CONST               7 (False)
-                                 732 STORE_FAST               6 (conditionAssigned)
-                     
-                     100         734 LOAD_FAST                5 (pCountSorted)
-                                 736 GET_ITER
-                             >>  738 FOR_ITER                75 (to 890)
-                                 740 STORE_FAST               7 (count)
-                     
-                     101         742 LOAD_FAST                2 (pCount)
-                                 744 LOAD_METHOD             14 (index)
-                                 766 LOAD_FAST                7 (count)
-                                 768 PRECALL                  1
-                                 772 CALL                     1
-                                 782 STORE_FAST               8 (idx)
-                     
-                     102         784 LOAD_GLOBAL              2 (current_app)
-                                 796 LOAD_ATTR                2 (config)
-                                 806 LOAD_CONST               1 ('CONDITIONS')
-                                 808 BINARY_SUBSCR
-                                 818 LOAD_FAST                8 (idx)
-                                 820 BINARY_SUBSCR
-                                 830 STORE_FAST               9 (conditionMeta)
-                     
-                     103         832 LOAD_CONST               8 ('enabled')
-                                 834 LOAD_FAST                9 (conditionMeta)
-                                 836 CONTAINS_OP              1
-                                 838 POP_JUMP_FORWARD_IF_TRUE    12 (to 864)
-                                 840 LOAD_FAST                9 (conditionMeta)
-                                 842 LOAD_CONST               8 ('enabled')
-                                 844 BINARY_SUBSCR
-                                 854 LOAD_CONST               9 (True)
-                                 856 COMPARE_OP               2 (==)
-                                 862 POP_JUMP_FORWARD_IF_FALSE    12 (to 888)
-                     
-                     104     >>  864 LOAD_FAST                8 (idx)
-                                 866 LOAD_CONST               4 (1)
-                                 868 BINARY_OP                0 (+)
-                                 872 LOAD_FAST                0 (self)
-                                 874 STORE_ATTR               9 (condition)
-                     
-                     105         884 POP_TOP
-                                 886 JUMP_FORWARD             1 (to 890)
-                     
-                     103     >>  888 JUMP_BACKWARD           76 (to 738)
-                     
-                     107     >>  890 LOAD_FAST                3 (printText)
-                                 892 LOAD_CONST              10 ('User put in condition {}.')
-                                 894 LOAD_METHOD              3 (format)
+                      89         326 LOAD_DEREF               9 (db)
+                                 328 LOAD_ATTR                7 (Participant)
+                                 338 LOAD_ATTR               10 (excludeFromCount)
+                                 348 UNARY_INVERT
+                     
+                      88         350 PRECALL                  2
+                                 354 CALL                     2
+                     
+                      90         364 LOAD_METHOD             11 (count)
+                                 386 PRECALL                  0
+                                 390 CALL                     0
+                     
+                      87         400 LOAD_FAST                2 (pCount)
+                                 402 LOAD_FAST                4 (condition)
+                                 404 LOAD_CONST               4 (1)
+                                 406 BINARY_OP               10 (-)
+                                 410 STORE_SUBSCR
+                                 414 JUMP_FORWARD           131 (to 678)
+                     
+                      92     >>  416 LOAD_DEREF               9 (db)
+                                 418 LOAD_ATTR                5 (session)
+                                 428 LOAD_METHOD              6 (query)
+                                 450 LOAD_DEREF               9 (db)
+                                 452 LOAD_ATTR                7 (Participant)
+                                 462 PRECALL                  1
+                                 466 CALL                     1
+                     
+                      93         476 LOAD_METHOD              8 (filter)
+                     
+                      94         498 LOAD_DEREF               9 (db)
+                                 500 LOAD_METHOD             12 (and_)
+                                 522 LOAD_DEREF               9 (db)
+                                 524 LOAD_ATTR                7 (Participant)
+                                 534 LOAD_ATTR                9 (condition)
+                                 544 LOAD_FAST                4 (condition)
+                                 546 COMPARE_OP               2 (==)
+                     
+                      95         552 LOAD_DEREF               9 (db)
+                                 554 LOAD_ATTR                7 (Participant)
+                                 564 LOAD_ATTR               13 (is_abandoned)
+                                 574 UNARY_INVERT
+                     
+                      96         576 LOAD_DEREF               9 (db)
+                                 578 LOAD_ATTR                7 (Participant)
+                                 588 LOAD_ATTR               10 (excludeFromCount)
+                                 598 UNARY_INVERT
+                     
+                      94         600 PRECALL                  3
+                                 604 CALL                     3
+                     
+                      93         614 PRECALL                  1
+                                 618 CALL                     1
+                     
+                      97         628 LOAD_METHOD             11 (count)
+                                 650 PRECALL                  0
+                                 654 CALL                     0
+                     
+                      92         664 LOAD_FAST                2 (pCount)
+                                 666 LOAD_FAST                4 (condition)
+                                 668 LOAD_CONST               4 (1)
+                                 670 BINARY_OP               10 (-)
+                                 674 STORE_SUBSCR
+                     
+                      99     >>  678 LOAD_FAST                3 (printText)
+                                 680 LOAD_CONST               6 ('{}, ')
+                                 682 LOAD_METHOD              3 (format)
+                                 704 LOAD_FAST                2 (pCount)
+                                 706 LOAD_FAST                4 (condition)
+                                 708 LOAD_CONST               4 (1)
+                                 710 BINARY_OP               10 (-)
+                                 714 BINARY_SUBSCR
+                                 724 PRECALL                  1
+                                 728 CALL                     1
+                                 738 BINARY_OP               13 (+=)
+                                 742 STORE_FAST               3 (printText)
+                                 744 EXTENDED_ARG             1
+                                 746 JUMP_BACKWARD          288 (to 172)
+                     
+                     101     >>  748 LOAD_GLOBAL             29 (NULL + sorted)
+                                 760 LOAD_FAST                2 (pCount)
+                                 762 PRECALL                  1
+                                 766 CALL                     1
+                                 776 STORE_FAST               5 (pCountSorted)
+                     
+                     103         778 LOAD_FAST                5 (pCountSorted)
+                                 780 GET_ITER
+                             >>  782 FOR_ITER                75 (to 934)
+                                 784 STORE_FAST               6 (count)
+                     
+                     104         786 LOAD_FAST                2 (pCount)
+                                 788 LOAD_METHOD             15 (index)
+                                 810 LOAD_FAST                6 (count)
+                                 812 PRECALL                  1
+                                 816 CALL                     1
+                                 826 STORE_FAST               7 (idx)
+                     
+                     105         828 LOAD_GLOBAL              2 (current_app)
+                                 840 LOAD_ATTR                2 (config)
+                                 850 LOAD_CONST               1 ('CONDITIONS')
+                                 852 BINARY_SUBSCR
+                                 862 LOAD_FAST                7 (idx)
+                                 864 BINARY_SUBSCR
+                                 874 STORE_FAST               8 (conditionMeta)
+                     
+                     106         876 LOAD_CONST               7 ('enabled')
+                                 878 LOAD_FAST                8 (conditionMeta)
+                                 880 CONTAINS_OP              1
+                                 882 POP_JUMP_FORWARD_IF_TRUE    12 (to 908)
+                                 884 LOAD_FAST                8 (conditionMeta)
+                                 886 LOAD_CONST               7 ('enabled')
+                                 888 BINARY_SUBSCR
+                                 898 LOAD_CONST               8 (True)
+                                 900 COMPARE_OP               2 (==)
+                                 906 POP_JUMP_FORWARD_IF_FALSE    12 (to 932)
+                     
+                     107     >>  908 LOAD_FAST                7 (idx)
+                                 910 LOAD_CONST               4 (1)
+                                 912 BINARY_OP                0 (+)
                                  916 LOAD_FAST                0 (self)
-                                 918 LOAD_ATTR                9 (condition)
-                                 928 PRECALL                  1
-                                 932 CALL                     1
-                                 942 BINARY_OP               13 (+=)
-                                 946 STORE_FAST               3 (printText)
-                     
-                     108         948 LOAD_GLOBAL             31 (NULL + print)
-                                 960 LOAD_FAST                3 (printText)
-                                 962 PRECALL                  1
-                                 966 CALL                     1
-                                 976 POP_TOP
-                                 978 LOAD_CONST               0 (None)
-                                 980 RETURN_VALUE
-                     
-                     110     >>  982 LOAD_CONST               0 (None)
-                                 984 LOAD_FAST                0 (self)
-                                 986 STORE_ATTR               9 (condition)
-                                 996 LOAD_CONST               0 (None)
-                                 998 RETURN_VALUE
+                                 918 STORE_ATTR               9 (condition)
+                     
+                     108         928 POP_TOP
+                                 930 JUMP_FORWARD             1 (to 934)
+                     
+                     106     >>  932 JUMP_BACKWARD           76 (to 782)
+                     
+                     110     >>  934 LOAD_FAST                3 (printText)
+                                 936 LOAD_CONST               9 ('User put in condition {}.')
+                                 938 LOAD_METHOD              3 (format)
+                                 960 LOAD_FAST                0 (self)
+                                 962 LOAD_ATTR                9 (condition)
+                                 972 PRECALL                  1
+                                 976 CALL                     1
+                                 986 BINARY_OP               13 (+=)
+                                 990 STORE_FAST               3 (printText)
+                     
+                     111         992 LOAD_GLOBAL             33 (NULL + print)
+                                1004 LOAD_FAST                3 (printText)
+                                1006 PRECALL                  1
+                                1010 CALL                     1
+                                1020 POP_TOP
+                                1022 LOAD_CONST               0 (None)
+                                1024 RETURN_VALUE
+                     
+                     113     >> 1026 LOAD_CONST               0 (None)
+                                1028 LOAD_FAST                0 (self)
+                                1030 STORE_ATTR               9 (condition)
+                                1040 LOAD_CONST               0 (None)
+                                1042 RETURN_VALUE
                      consts
                         None
                         'CONDITIONS'
                         0
                         'Total conditions: {}, Counts: '
                         1
                         'COUNTS_INCLUDE_ABANDONED'
                         '{}, '
-                        False
                         'enabled'
                         True
                         'User put in condition {}.'
-                     names      ('len', 'current_app', 'config', 'format', 'range', 'session', 'query', 'Participant', 'filter', 'condition', 'count', 'and_', 'is_abandoned', 'sorted', 'index', 'print')
-                     varnames   ('self', 'numConditions', 'pCount', 'printText', 'condition', 'pCountSorted', 'conditionAssigned', 'count', 'idx', 'conditionMeta')
+                     names      ('len', 'current_app', 'config', 'format', 'range', 'session', 'query', 'Participant', 'filter', 'condition', 'excludeFromCount', 'count', 'and_', 'is_abandoned', 'sorted', 'index', 'print')
+                     varnames   ('self', 'numConditions', 'pCount', 'printText', 'condition', 'pCountSorted', 'count', 'idx', 'conditionMeta')
                      freevars   ('db',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'assign_condition'
-                     firstlineno 76
+                     firstlineno 77
                      lnotab
-                        0x04013e010e010c022a022c0224013c01420124fe10043c0116015cff0e
-                        0224fd0e0546021e01040208012a0130012001140104fe02043a012202
+                        0x04013e010e010c022a022c0224013c01340118ff0e0224fd10053c0116
+                        013601180118fe0eff0e0424fb0e0746021e0208012a0130012001140104
+                        fe02043a012202
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x97007c006a000000000000000000811a7c006a00000000000000000064
                         016b040000000072117c006a0000000000000000000b007c005f00000000
                         0000000000640053006400530064005300
-                     112           0 RESUME                   0
+                     115           0 RESUME                   0
                      
-                     113           2 LOAD_FAST                0 (self)
+                     116           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (condition)
                                   14 POP_JUMP_FORWARD_IF_NONE    26 (to 68)
                                   16 LOAD_FAST                0 (self)
                                   18 LOAD_ATTR                0 (condition)
                                   28 LOAD_CONST               1 (0)
                                   30 COMPARE_OP               4 (>)
                                   36 POP_JUMP_FORWARD_IF_FALSE    17 (to 72)
                      
-                     114          38 LOAD_FAST                0 (self)
+                     117          38 LOAD_FAST                0 (self)
                                   40 LOAD_ATTR                0 (condition)
                                   50 UNARY_NEGATIVE
                                   52 LOAD_FAST                0 (self)
                                   54 STORE_ATTR               0 (condition)
                                   64 LOAD_CONST               0 (None)
                                   66 RETURN_VALUE
                      
-                     113     >>   68 LOAD_CONST               0 (None)
+                     116     >>   68 LOAD_CONST               0 (None)
                                   70 RETURN_VALUE
                              >>   72 LOAD_CONST               0 (None)
                                   74 RETURN_VALUE
                      consts
                         None
                         0
                      names      ('condition',)
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'release_condition'
-                     firstlineno 112
+                     firstlineno 115
                      lnotab 0x020124011eff
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x97007c006a0000000000000000008002640153007c006a000000000000
                         0000007c006a0100000000000000007a0a0000a002000000000000000000
                         0000000000000000000000a6000000ab0000000000000000005300
-                     116           0 RESUME                   0
+                     119           0 RESUME                   0
                      
-                     118           2 LOAD_FAST                0 (self)
+                     121           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (timeEnded)
                                   14 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 20)
                      
-                     119          16 LOAD_CONST               1 (0)
+                     122          16 LOAD_CONST               1 (0)
                                   18 RETURN_VALUE
                      
-                     120     >>   20 LOAD_FAST                0 (self)
+                     123     >>   20 LOAD_FAST                0 (self)
                                   22 LOAD_ATTR                0 (timeEnded)
                                   32 LOAD_FAST                0 (self)
                                   34 LOAD_ATTR                1 (timeStarted)
                                   44 BINARY_OP               10 (-)
                                   48 LOAD_METHOD              2 (total_seconds)
                                   70 PRECALL                  0
                                   74 CALL                     0
@@ -1077,15 +1101,15 @@
                         0
                      names      ('timeEnded', 'timeStarted', 'total_seconds')
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'duration'
-                     firstlineno 116
+                     firstlineno 119
                      lnotab 0x02020e010401
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 7
                      flags     : 19
                      code
@@ -1095,27 +1119,27 @@
                         010000000000000000a6010000ab01000000000000000089016a02000000
                         0000000000a00300000000000000000000000000000000000000007c006a
                         040000000000000000a6010000ab0100000000000000007a0a000064017a
                         050000ac02a6020000ab020000000000000000a005000000000000000000
                         00000000000000000000006403a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     122           2 RESUME                   0
+                     125           2 RESUME                   0
                      
-                     124           4 LOAD_DEREF               1 (db)
+                     127           4 LOAD_DEREF               1 (db)
                                    6 LOAD_METHOD              0 (case)
                      
-                     125          28 LOAD_FAST                0 (cls)
+                     128          28 LOAD_FAST                0 (cls)
                                   30 LOAD_ATTR                1 (timeEnded)
                                   40 LOAD_CONST               0 (None)
                                   42 COMPARE_OP               2 (==)
                                   48 LOAD_CONST               0 (None)
                                   50 BUILD_TUPLE              2
                      
-                     126          52 LOAD_DEREF               1 (db)
+                     129          52 LOAD_DEREF               1 (db)
                                   54 LOAD_ATTR                2 (func)
                                   64 LOAD_METHOD              3 (julianday)
                                   86 LOAD_FAST                0 (cls)
                                   88 LOAD_ATTR                1 (timeEnded)
                                   98 PRECALL                  1
                                  102 CALL                     1
                                  112 LOAD_DEREF               1 (db)
@@ -1125,233 +1149,239 @@
                                  148 LOAD_ATTR                4 (timeStarted)
                                  158 PRECALL                  1
                                  162 CALL                     1
                                  172 BINARY_OP               10 (-)
                                  176 LOAD_CONST               1 (86400)
                                  178 BINARY_OP                5 (*)
                      
-                     124         182 KW_NAMES                 2
+                     127         182 KW_NAMES                 2
                                  184 PRECALL                  2
                                  188 CALL                     2
                      
-                     127         198 LOAD_METHOD              5 (label)
+                     130         198 LOAD_METHOD              5 (label)
                                  220 LOAD_CONST               3 ('duration')
                                  222 PRECALL                  1
                                  226 CALL                     1
                      
-                     124         236 RETURN_VALUE
+                     127         236 RETURN_VALUE
                      consts
                         None
                         86400
                         ('else_',)
                         'duration'
                      names      ('case', 'timeEnded', 'func', 'julianday', 'timeStarted', 'label')
                      varnames   ('cls',)
                      freevars   ('db',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'duration'
-                     firstlineno 122
+                     firstlineno 125
                      lnotab 0x04021801180182fe100326fd
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 9
+                     stacksize : 10
                      flags     : 19
                      code
                         0x950197007401000000000000000000008901a001000000000000000000
-                        00000000000000000000007c006a0200000000000000000f0089016a0300
-                        00000000000000a004000000000000000000000000000000000000000074
-                        0b000000000000000000006a060000000000000000a6000000ab00000000
-                        0000000000a6010000ab01000000000000000089016a0300000000000000
-                        00a00400000000000000000000000000000000000000007c006a07000000
-                        0000000000a6010000ab0100000000000000007a0a000074100000000000
-                        00000000006a09000000000000000064011900000000000000000064027a
-                        0b00006b0100000000a6020000ab020000000000000000a00a0000000000
-                        0000000000000000000000000000006403a6010000ab0100000000000000
-                        00a6010000ab0100000000000000005300
+                        00000000000000000000007c006a0200000000000000000f00640189016a
+                        030000000000000000a00400000000000000000000000000000000000000
+                        0089016a030000000000000000a005000000000000000000000000000000
+                        0000000000a6000000ab000000000000000000a6010000ab010000000000
+                        00000089016a030000000000000000a00400000000000000000000000000
+                        000000000000007c006a060000000000000000a6010000ab010000000000
+                        0000007a0a00007a050000740e000000000000000000006a080000000000
+                        0000006402190000000000000000006b0100000000a6020000ab02000000
+                        0000000000a00900000000000000000000000000000000000000006403a6
+                        010000ab010000000000000000a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     129           2 RESUME                   0
+                     132           2 RESUME                   0
                      
-                     131           4 LOAD_GLOBAL              1 (NULL + column_property)
+                     134           4 LOAD_GLOBAL              1 (NULL + column_property)
                      
-                     132          16 LOAD_DEREF               1 (db)
+                     135          16 LOAD_DEREF               1 (db)
                                   18 LOAD_METHOD              1 (and_)
                      
-                     133          40 LOAD_FAST                0 (cls)
+                     136          40 LOAD_FAST                0 (cls)
                                   42 LOAD_ATTR                2 (finished)
                                   52 UNARY_INVERT
                      
-                     134          54 LOAD_DEREF               1 (db)
-                                  56 LOAD_ATTR                3 (func)
-                                  66 LOAD_METHOD              4 (julianday)
-                                  88 LOAD_GLOBAL             11 (NULL + datetime)
-                                 100 LOAD_ATTR                6 (utcnow)
-                                 110 PRECALL                  0
-                                 114 CALL                     0
-                                 124 PRECALL                  1
-                                 128 CALL                     1
-                                 138 LOAD_DEREF               1 (db)
-                                 140 LOAD_ATTR                3 (func)
-                                 150 LOAD_METHOD              4 (julianday)
-                                 172 LOAD_FAST                0 (cls)
-                                 174 LOAD_ATTR                7 (lastActiveOn)
-                                 184 PRECALL                  1
-                                 188 CALL                     1
-                                 198 BINARY_OP               10 (-)
-                                 202 LOAD_GLOBAL             16 (current_app)
-                                 214 LOAD_ATTR                9 (config)
-                                 224 LOAD_CONST               1 ('ABANDONED_MINUTES')
-                                 226 BINARY_SUBSCR
-                                 236 LOAD_CONST               2 (1440.0)
-                                 238 BINARY_OP               11 (/)
-                                 242 COMPARE_OP               1 (<=)
-                     
-                     132         248 PRECALL                  2
-                                 252 CALL                     2
-                     
-                     135         262 LOAD_METHOD             10 (label)
-                                 284 LOAD_CONST               3 ('is_in_progress')
-                                 286 PRECALL                  1
-                                 290 CALL                     1
-                     
-                     131         300 PRECALL                  1
-                                 304 CALL                     1
-                                 314 RETURN_VALUE
+                     137          54 LOAD_CONST               1 (1440.0)
+                                  56 LOAD_DEREF               1 (db)
+                                  58 LOAD_ATTR                3 (func)
+                                  68 LOAD_METHOD              4 (julianday)
+                                  90 LOAD_DEREF               1 (db)
+                                  92 LOAD_ATTR                3 (func)
+                                 102 LOAD_METHOD              5 (current_timestamp)
+                                 124 PRECALL                  0
+                                 128 CALL                     0
+                                 138 PRECALL                  1
+                                 142 CALL                     1
+                                 152 LOAD_DEREF               1 (db)
+                                 154 LOAD_ATTR                3 (func)
+                                 164 LOAD_METHOD              4 (julianday)
+                                 186 LOAD_FAST                0 (cls)
+                                 188 LOAD_ATTR                6 (lastActiveOn)
+                                 198 PRECALL                  1
+                                 202 CALL                     1
+                                 212 BINARY_OP               10 (-)
+                                 216 BINARY_OP                5 (*)
+                     
+                     138         220 LOAD_GLOBAL             14 (current_app)
+                                 232 LOAD_ATTR                8 (config)
+                                 242 LOAD_CONST               2 ('ABANDONED_MINUTES')
+                                 244 BINARY_SUBSCR
+                     
+                     137         254 COMPARE_OP               1 (<=)
+                     
+                     135         260 PRECALL                  2
+                                 264 CALL                     2
+                     
+                     139         274 LOAD_METHOD              9 (label)
+                                 296 LOAD_CONST               3 ('is_in_progress')
+                                 298 PRECALL                  1
+                                 302 CALL                     1
+                     
+                     134         312 PRECALL                  1
+                                 316 CALL                     1
+                                 326 RETURN_VALUE
                      consts
                         None
-                        'ABANDONED_MINUTES'
                         1440.0
+                        'ABANDONED_MINUTES'
                         'is_in_progress'
-                     names      ('column_property', 'and_', 'finished', 'func', 'julianday', 'datetime', 'utcnow', 'lastActiveOn', 'current_app', 'config', 'label')
+                     names      ('column_property', 'and_', 'finished', 'func', 'julianday', 'current_timestamp', 'lastActiveOn', 'current_app', 'config', 'label')
                      varnames   ('cls',)
                      freevars   ('db',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'is_in_progress'
-                     firstlineno 129
-                     lnotab 0x04020c0118010e01c2fe0e0326fc
+                     firstlineno 132
+                     lnotab 0x04020c0118010e01a60122ff06fe0e0426fb
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 9
+                     stacksize : 10
                      flags     : 19
                      code
                         0x950197007401000000000000000000008901a001000000000000000000
-                        00000000000000000000007c006a0200000000000000000f0089016a0300
-                        00000000000000a004000000000000000000000000000000000000000074
-                        0b000000000000000000006a060000000000000000a6000000ab00000000
-                        0000000000a6010000ab01000000000000000089016a0300000000000000
-                        00a00400000000000000000000000000000000000000007c006a07000000
-                        0000000000a6010000ab0100000000000000007a0a000074100000000000
-                        00000000006a09000000000000000064011900000000000000000064027a
-                        0b00006b0400000000a6020000ab020000000000000000a00a0000000000
-                        0000000000000000000000000000006403a6010000ab0100000000000000
-                        00a6010000ab0100000000000000005300
+                        00000000000000000000007c006a0200000000000000000f00640189016a
+                        030000000000000000a00400000000000000000000000000000000000000
+                        0089016a030000000000000000a005000000000000000000000000000000
+                        0000000000a6000000ab000000000000000000a6010000ab010000000000
+                        00000089016a030000000000000000a00400000000000000000000000000
+                        000000000000007c006a060000000000000000a6010000ab010000000000
+                        0000007a0a00007a050000740e000000000000000000006a080000000000
+                        0000006402190000000000000000006b0400000000a6020000ab02000000
+                        0000000000a00900000000000000000000000000000000000000006403a6
+                        010000ab010000000000000000a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     138           2 RESUME                   0
+                     142           2 RESUME                   0
                      
-                     140           4 LOAD_GLOBAL              1 (NULL + column_property)
+                     144           4 LOAD_GLOBAL              1 (NULL + column_property)
                      
-                     141          16 LOAD_DEREF               1 (db)
+                     145          16 LOAD_DEREF               1 (db)
                                   18 LOAD_METHOD              1 (and_)
                      
-                     142          40 LOAD_FAST                0 (cls)
+                     146          40 LOAD_FAST                0 (cls)
                                   42 LOAD_ATTR                2 (finished)
                                   52 UNARY_INVERT
                      
-                     143          54 LOAD_DEREF               1 (db)
-                                  56 LOAD_ATTR                3 (func)
-                                  66 LOAD_METHOD              4 (julianday)
-                                  88 LOAD_GLOBAL             11 (NULL + datetime)
-                                 100 LOAD_ATTR                6 (utcnow)
-                                 110 PRECALL                  0
-                                 114 CALL                     0
-                                 124 PRECALL                  1
-                                 128 CALL                     1
-                                 138 LOAD_DEREF               1 (db)
-                                 140 LOAD_ATTR                3 (func)
-                                 150 LOAD_METHOD              4 (julianday)
-                                 172 LOAD_FAST                0 (cls)
-                                 174 LOAD_ATTR                7 (lastActiveOn)
-                                 184 PRECALL                  1
-                                 188 CALL                     1
-                                 198 BINARY_OP               10 (-)
-                                 202 LOAD_GLOBAL             16 (current_app)
-                                 214 LOAD_ATTR                9 (config)
-                                 224 LOAD_CONST               1 ('ABANDONED_MINUTES')
-                                 226 BINARY_SUBSCR
-                                 236 LOAD_CONST               2 (1440.0)
-                                 238 BINARY_OP               11 (/)
-                                 242 COMPARE_OP               4 (>)
-                     
-                     141         248 PRECALL                  2
-                                 252 CALL                     2
-                     
-                     144         262 LOAD_METHOD             10 (label)
-                                 284 LOAD_CONST               3 ('is_abandoned')
-                                 286 PRECALL                  1
-                                 290 CALL                     1
-                     
-                     140         300 PRECALL                  1
-                                 304 CALL                     1
-                                 314 RETURN_VALUE
+                     147          54 LOAD_CONST               1 (1440.0)
+                                  56 LOAD_DEREF               1 (db)
+                                  58 LOAD_ATTR                3 (func)
+                                  68 LOAD_METHOD              4 (julianday)
+                                  90 LOAD_DEREF               1 (db)
+                                  92 LOAD_ATTR                3 (func)
+                                 102 LOAD_METHOD              5 (current_timestamp)
+                                 124 PRECALL                  0
+                                 128 CALL                     0
+                                 138 PRECALL                  1
+                                 142 CALL                     1
+                                 152 LOAD_DEREF               1 (db)
+                                 154 LOAD_ATTR                3 (func)
+                                 164 LOAD_METHOD              4 (julianday)
+                                 186 LOAD_FAST                0 (cls)
+                                 188 LOAD_ATTR                6 (lastActiveOn)
+                                 198 PRECALL                  1
+                                 202 CALL                     1
+                                 212 BINARY_OP               10 (-)
+                                 216 BINARY_OP                5 (*)
+                     
+                     148         220 LOAD_GLOBAL             14 (current_app)
+                                 232 LOAD_ATTR                8 (config)
+                                 242 LOAD_CONST               2 ('ABANDONED_MINUTES')
+                                 244 BINARY_SUBSCR
+                     
+                     147         254 COMPARE_OP               4 (>)
+                     
+                     145         260 PRECALL                  2
+                                 264 CALL                     2
+                     
+                     149         274 LOAD_METHOD              9 (label)
+                                 296 LOAD_CONST               3 ('is_abandoned')
+                                 298 PRECALL                  1
+                                 302 CALL                     1
+                     
+                     144         312 PRECALL                  1
+                                 316 CALL                     1
+                                 326 RETURN_VALUE
                      consts
                         None
-                        'ABANDONED_MINUTES'
                         1440.0
+                        'ABANDONED_MINUTES'
                         'is_abandoned'
-                     names      ('column_property', 'and_', 'finished', 'func', 'julianday', 'datetime', 'utcnow', 'lastActiveOn', 'current_app', 'config', 'label')
+                     names      ('column_property', 'and_', 'finished', 'func', 'julianday', 'current_timestamp', 'lastActiveOn', 'current_app', 'config', 'label')
                      varnames   ('cls',)
                      freevars   ('db',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'is_abandoned'
-                     firstlineno 138
-                     lnotab 0x04020c0118010e01c2fe0e0326fc
+                     firstlineno 142
+                     lnotab 0x04020c0118010e01a60122ff06fe0e0426fb
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code
                         0x97007c006a000000000000000000800b7c006a01000000000000000072
                         0264025300640353007c006a0000000000000000007c006a020000000000
                         0000007a0a0000a0030000000000000000000000000000000000000000a6
                         000000ab0000000000000000007d017409000000000000000000007c01a6
                         010000ab0100000000000000005300
-                     147           0 RESUME                   0
+                     152           0 RESUME                   0
                      
-                     153           2 LOAD_FAST                0 (self)
+                     158           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (timeEnded)
                                   14 POP_JUMP_FORWARD_IF_NOT_NONE    11 (to 38)
                      
-                     154          16 LOAD_FAST                0 (self)
+                     159          16 LOAD_FAST                0 (self)
                                   18 LOAD_ATTR                1 (is_in_progress)
                                   28 POP_JUMP_FORWARD_IF_FALSE     2 (to 34)
                      
-                     155          30 LOAD_CONST               2 ('In Progress')
+                     160          30 LOAD_CONST               2 ('In Progress')
                                   32 RETURN_VALUE
                      
-                     157     >>   34 LOAD_CONST               3 ('Abandoned')
+                     162     >>   34 LOAD_CONST               3 ('Abandoned')
                                   36 RETURN_VALUE
                      
-                     160     >>   38 LOAD_FAST                0 (self)
+                     165     >>   38 LOAD_FAST                0 (self)
                                   40 LOAD_ATTR                0 (timeEnded)
                                   50 LOAD_FAST                0 (self)
                                   52 LOAD_ATTR                2 (timeStarted)
                                   62 BINARY_OP               10 (-)
                                   66 LOAD_METHOD              3 (total_seconds)
                                   88 PRECALL                  0
                                   92 CALL                     0
                                  102 STORE_FAST               1 (seconds)
                      
-                     161         104 LOAD_GLOBAL              9 (NULL + display_time)
+                     166         104 LOAD_GLOBAL              9 (NULL + display_time)
                                  116 LOAD_FAST                1 (seconds)
                                  118 PRECALL                  1
                                  122 CALL                     1
                                  132 RETURN_VALUE
                      consts
                         '\n            display the time taken or status\n            :return:\n            '
                         None
@@ -1359,29 +1389,29 @@
                         'Abandoned'
                      names      ('timeEnded', 'is_in_progress', 'timeStarted', 'total_seconds', 'display_time')
                      varnames   ('self', 'seconds')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'display_duration'
-                     firstlineno 147
+                     firstlineno 152
                      lnotab 0x02060e010e01040204034201
                   ('',)
                   ('return', None)
-               names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'Integer', 'participantID', 'String', 'mTurkID', 'ipAddress', 'userAgent', 'condition', 'DateTime', 'datetime', 'utcnow', 'timeStarted', 'timeEnded', 'Boolean', 'finished', 'code', 'lastActiveOn', 'table', 'questionnaire', 'dict', 'questionnaire_log', 'assign_condition', 'release_condition', 'hybrid_property', 'int', 'duration', 'expression', 'declared_attr', 'is_in_progress', 'is_abandoned', 'str', 'display_duration')
+               names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'Integer', 'participantID', 'String', 'mTurkID', 'ipAddress', 'userAgent', 'condition', 'DateTime', 'datetime', 'utcnow', 'timeStarted', 'timeEnded', 'Boolean', 'finished', 'excludeFromCount', 'code', 'lastActiveOn', 'table', 'questionnaire', 'dict', 'questionnaire_log', 'assign_condition', 'release_condition', 'hybrid_property', 'int', 'duration', 'expression', 'declared_attr', 'is_in_progress', 'is_abandoned', 'str', 'display_duration')
                varnames   ()
                freevars   ('db',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                name       'Participant'
                firstlineno 10
                lnotab
-                  0x0c0104023a015601560156013a01440138013a01560144020604081812
-                  180c24080402010aff0e0102050c0108ff0e010206020108ff0e01020802
-                  0108ff0e010208
+                  0x0c0104023a015601560156013a01440138013a013a0156014402060408
+                  1812180c26080402010aff0e0102050c0108ff0e010206020108ff0e0102
+                  09020108ff0e010209
             'Participant'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 6
                flags     : 0
                code
@@ -1394,75 +1424,75 @@
                   00000000000000000000000000000094006a0a0000000000000000640565
                   0b6a0c0000000000000000ac07a6030000ab0300000000000000005a0d94
                   00a004000000000000000000000000000000000000000094006a0a000000
                   00000000006403ac08a6020000ab0200000000000000005a0e6409650f66
                   02640a84045a10640b5300
                              0 COPY_FREE_VARS           1
                
-               164           2 RESUME                   0
+               169           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create.<locals>.Progress')
                             10 STORE_NAME               2 (__qualname__)
                
-               165          12 LOAD_CONST               1 ('progress')
+               170          12 LOAD_CONST               1 ('progress')
                             14 STORE_NAME               3 (__tablename__)
                
-               167          16 LOAD_CLASSDEREF          0 (db)
+               172          16 LOAD_CLASSDEREF          0 (db)
                             18 LOAD_METHOD              4 (Column)
                             40 LOAD_CLASSDEREF          0 (db)
                             42 LOAD_ATTR                5 (Integer)
                             52 LOAD_CLASSDEREF          0 (db)
                             54 LOAD_METHOD              6 (ForeignKey)
                             76 LOAD_CONST               2 ('participant.participantID')
                             78 PRECALL                  1
                             82 CALL                     1
                             92 LOAD_CONST               3 (True)
                             94 KW_NAMES                 4
                             96 PRECALL                  3
                            100 CALL                     3
                            110 STORE_NAME               7 (participantID)
                
-               168         112 LOAD_CLASSDEREF          0 (db)
+               173         112 LOAD_CLASSDEREF          0 (db)
                            114 LOAD_METHOD              4 (Column)
                            136 LOAD_CLASSDEREF          0 (db)
                            138 LOAD_ATTR                8 (Text)
                            148 LOAD_CONST               5 (False)
                            150 LOAD_CONST               3 (True)
                            152 KW_NAMES                 6
                            154 PRECALL                  3
                            158 CALL                     3
                            168 STORE_NAME               9 (path)
                
-               169         170 LOAD_CLASSDEREF          0 (db)
+               174         170 LOAD_CLASSDEREF          0 (db)
                            172 LOAD_METHOD              4 (Column)
                            194 LOAD_CLASSDEREF          0 (db)
                            196 LOAD_ATTR               10 (DateTime)
                            206 LOAD_CONST               5 (False)
                            208 LOAD_NAME               11 (datetime)
                            210 LOAD_ATTR               12 (utcnow)
                            220 KW_NAMES                 7
                            222 PRECALL                  3
                            226 CALL                     3
                            236 STORE_NAME              13 (startedOn)
                
-               170         238 LOAD_CLASSDEREF          0 (db)
+               175         238 LOAD_CLASSDEREF          0 (db)
                            240 LOAD_METHOD              4 (Column)
                            262 LOAD_CLASSDEREF          0 (db)
                            264 LOAD_ATTR               10 (DateTime)
                            274 LOAD_CONST               3 (True)
                            276 KW_NAMES                 8
                            278 PRECALL                  2
                            282 CALL                     2
                            292 STORE_NAME              14 (submittedOn)
                
-               172         294 LOAD_CONST               9 ('return')
+               177         294 LOAD_CONST               9 ('return')
                            296 LOAD_NAME               15 (str)
                            298 BUILD_TUPLE              2
-                           300 LOAD_CONST              10 (<code object display_duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 172>)
+                           300 LOAD_CONST              10 (<code object display_duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 177>)
                            302 MAKE_FUNCTION            4 (annotations)
                            304 STORE_NAME              16 (display_duration)
                            306 LOAD_CONST              11 (None)
                            308 RETURN_VALUE
                consts
                   'create.<locals>.Progress'
                   'progress'
@@ -1484,54 +1514,54 @@
                         0000007c006a0100000000000000007a0a0000a002000000000000000000
                         0000000000000000000000a6000000ab0000000000000000007d017c0164
                         026b040000000072297407000000000000000000006403a6010000ab0100
                         00000000000000a00400000000000000000000000000000000000000007c
                         0164027a0b00007c0164027a060000a6020000ab02000000000000000053
                         00740700000000000000000000740b000000000000000000007c01a60100
                         00ab010000000000000000a6010000ab0100000000000000005300
-                     172           0 RESUME                   0
+                     177           0 RESUME                   0
                      
-                     173           2 LOAD_FAST                0 (self)
+                     178           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (submittedOn)
                                   14 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 20)
                      
-                     174          16 LOAD_CONST               1 ('...')
+                     179          16 LOAD_CONST               1 ('...')
                                   18 RETURN_VALUE
                      
-                     176     >>   20 LOAD_FAST                0 (self)
+                     181     >>   20 LOAD_FAST                0 (self)
                                   22 LOAD_ATTR                0 (submittedOn)
                                   32 LOAD_FAST                0 (self)
                                   34 LOAD_ATTR                1 (startedOn)
                                   44 BINARY_OP               10 (-)
                                   48 LOAD_METHOD              2 (total_seconds)
                                   70 PRECALL                  0
                                   74 CALL                     0
                                   84 STORE_FAST               1 (seconds)
                      
-                     177          86 LOAD_FAST                1 (seconds)
+                     182          86 LOAD_FAST                1 (seconds)
                                   88 LOAD_CONST               2 (60)
                                   90 COMPARE_OP               4 (>)
                                   96 POP_JUMP_FORWARD_IF_FALSE    41 (to 180)
                      
-                     178          98 LOAD_GLOBAL              7 (NULL + str)
+                     183          98 LOAD_GLOBAL              7 (NULL + str)
                                  110 LOAD_CONST               3 ('{:.0f}:{:02.0f}')
                                  112 PRECALL                  1
                                  116 CALL                     1
                                  126 LOAD_METHOD              4 (format)
                                  148 LOAD_FAST                1 (seconds)
                                  150 LOAD_CONST               2 (60)
                                  152 BINARY_OP               11 (/)
                                  156 LOAD_FAST                1 (seconds)
                                  158 LOAD_CONST               2 (60)
                                  160 BINARY_OP                6 (%)
                                  164 PRECALL                  2
                                  168 CALL                     2
                                  178 RETURN_VALUE
                      
-                     179     >>  180 LOAD_GLOBAL              7 (NULL + str)
+                     184     >>  180 LOAD_GLOBAL              7 (NULL + str)
                                  192 LOAD_GLOBAL             11 (NULL + int)
                                  204 LOAD_FAST                1 (seconds)
                                  206 PRECALL                  1
                                  210 CALL                     1
                                  220 PRECALL                  1
                                  224 CALL                     1
                                  234 RETURN_VALUE
@@ -1542,24 +1572,24 @@
                         '{:.0f}:{:02.0f}'
                      names      ('submittedOn', 'startedOn', 'total_seconds', 'str', 'format', 'int')
                      varnames   ('self', 'seconds')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'display_duration'
-                     firstlineno 172
+                     firstlineno 177
                      lnotab 0x02010e01040242010c015201
                   None
                names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'Integer', 'ForeignKey', 'participantID', 'Text', 'path', 'DateTime', 'datetime', 'utcnow', 'startedOn', 'submittedOn', 'str', 'display_duration')
                varnames   ()
                freevars   ('db',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                name       'Progress'
-               firstlineno 164
+               firstlineno 169
                lnotab 0x0c01040260013a0144013802
             'Progress'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 6
                flags     : 0
@@ -1578,93 +1608,93 @@
                   056407ac06a6030000ab0300000000000000005a0f9400a0040000000000
                   00000000000000000000000000000094006a0d0000000000000000640564
                   07ac06a6030000ab0300000000000000005a109400a00400000000000000
                   0000000000000000000000000094006a0d000000000000000064056407ac
                   06a6030000ab0300000000000000005a1164085300
                              0 COPY_FREE_VARS           1
                
-               182           2 RESUME                   0
+               187           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create.<locals>.RadioGridLog')
                             10 STORE_NAME               2 (__qualname__)
                
-               183          12 LOAD_CONST               1 ('radio_grid_log')
+               188          12 LOAD_CONST               1 ('radio_grid_log')
                             14 STORE_NAME               3 (__tablename__)
                
-               185          16 LOAD_CLASSDEREF          0 (db)
+               190          16 LOAD_CLASSDEREF          0 (db)
                             18 LOAD_METHOD              4 (Column)
                             40 LOAD_CLASSDEREF          0 (db)
                             42 LOAD_ATTR                5 (Integer)
                             52 LOAD_CONST               2 (True)
                             54 LOAD_CONST               2 (True)
                             56 KW_NAMES                 3
                             58 PRECALL                  3
                             62 CALL                     3
                             72 STORE_NAME               6 (radioGridLog)
                
-               186          74 LOAD_CLASSDEREF          0 (db)
+               191          74 LOAD_CLASSDEREF          0 (db)
                             76 LOAD_METHOD              4 (Column)
                             98 LOAD_CLASSDEREF          0 (db)
                            100 LOAD_ATTR                5 (Integer)
                            110 LOAD_CLASSDEREF          0 (db)
                            112 LOAD_METHOD              7 (ForeignKey)
                            134 LOAD_CONST               4 ('participant.participantID')
                            136 PRECALL                  1
                            140 CALL                     1
                            150 PRECALL                  2
                            154 CALL                     2
                            164 STORE_NAME               8 (participantID)
                
-               187         166 LOAD_CLASSDEREF          0 (db)
+               192         166 LOAD_CLASSDEREF          0 (db)
                            168 LOAD_METHOD              4 (Column)
                            190 LOAD_CLASSDEREF          0 (db)
                            192 LOAD_ATTR                9 (DateTime)
                            202 LOAD_CONST               5 (False)
                            204 LOAD_NAME               10 (datetime)
                            206 LOAD_ATTR               11 (utcnow)
                            216 KW_NAMES                 6
                            218 PRECALL                  3
                            222 CALL                     3
                            232 STORE_NAME              12 (timeClicked)
                
-               188         234 LOAD_CLASSDEREF          0 (db)
+               193         234 LOAD_CLASSDEREF          0 (db)
                            236 LOAD_METHOD              4 (Column)
                            258 LOAD_CLASSDEREF          0 (db)
                            260 LOAD_ATTR               13 (String)
                            270 LOAD_CONST               5 (False)
                            272 LOAD_CONST               7 ('')
                            274 KW_NAMES                 6
                            276 PRECALL                  3
                            280 CALL                     3
                            290 STORE_NAME              14 (questionnaire)
                
-               189         292 LOAD_CLASSDEREF          0 (db)
+               194         292 LOAD_CLASSDEREF          0 (db)
                            294 LOAD_METHOD              4 (Column)
                            316 LOAD_CLASSDEREF          0 (db)
                            318 LOAD_ATTR               13 (String)
                            328 LOAD_CONST               5 (False)
                            330 LOAD_CONST               7 ('')
                            332 KW_NAMES                 6
                            334 PRECALL                  3
                            338 CALL                     3
                            348 STORE_NAME              15 (tag)
                
-               190         350 LOAD_CLASSDEREF          0 (db)
+               195         350 LOAD_CLASSDEREF          0 (db)
                            352 LOAD_METHOD              4 (Column)
                            374 LOAD_CLASSDEREF          0 (db)
                            376 LOAD_ATTR               13 (String)
                            386 LOAD_CONST               5 (False)
                            388 LOAD_CONST               7 ('')
                            390 KW_NAMES                 6
                            392 PRECALL                  3
                            396 CALL                     3
                            406 STORE_NAME              16 (questionID)
                
-               191         408 LOAD_CLASSDEREF          0 (db)
+               196         408 LOAD_CLASSDEREF          0 (db)
                            410 LOAD_METHOD              4 (Column)
                            432 LOAD_CLASSDEREF          0 (db)
                            434 LOAD_ATTR               13 (String)
                            444 LOAD_CONST               5 (False)
                            446 LOAD_CONST               7 ('')
                            448 KW_NAMES                 6
                            450 PRECALL                  3
@@ -1684,15 +1714,15 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'Integer', 'radioGridLog', 'ForeignKey', 'participantID', 'DateTime', 'datetime', 'utcnow', 'timeClicked', 'String', 'questionnaire', 'tag', 'questionID', 'value')
                varnames   ()
                freevars   ('db',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                name       'RadioGridLog'
-               firstlineno 182
+               firstlineno 187
                lnotab 0x0c0104023a015c0144013a013a013a01
             'RadioGridLog'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 6
                flags     : 0
@@ -1711,92 +1741,92 @@
                   0300000000000000005a0c9400a004000000000000000000000000000000
                   000000000094006a05000000000000000064056408ac07a6030000ab0300
                   000000000000005a0d9400a0040000000000000000000000000000000000
                   00000094006a05000000000000000064056408ac07a6030000ab03000000
                   00000000005a0e64095300
                              0 COPY_FREE_VARS           1
                
-               194           2 RESUME                   0
+               199           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create.<locals>.Display')
                             10 STORE_NAME               2 (__qualname__)
                
-               195          12 LOAD_CONST               1 ('display')
+               200          12 LOAD_CONST               1 ('display')
                             14 STORE_NAME               3 (__tablename__)
                
-               197          16 LOAD_CLASSDEREF          0 (db)
+               202          16 LOAD_CLASSDEREF          0 (db)
                             18 LOAD_METHOD              4 (Column)
                             40 LOAD_CLASSDEREF          0 (db)
                             42 LOAD_ATTR                5 (Integer)
                             52 LOAD_CONST               2 (True)
                             54 LOAD_CONST               2 (True)
                             56 KW_NAMES                 3
                             58 PRECALL                  3
                             62 CALL                     3
                             72 STORE_NAME               6 (logDisplayID)
                
-               198          74 LOAD_CLASSDEREF          0 (db)
+               203          74 LOAD_CLASSDEREF          0 (db)
                             76 LOAD_METHOD              4 (Column)
                             98 LOAD_CLASSDEREF          0 (db)
                            100 LOAD_ATTR                5 (Integer)
                            110 LOAD_CLASSDEREF          0 (db)
                            112 LOAD_METHOD              7 (ForeignKey)
                            134 LOAD_CONST               4 ('participant.participantID')
                            136 PRECALL                  1
                            140 CALL                     1
                            150 PRECALL                  2
                            154 CALL                     2
                            164 STORE_NAME               8 (participantID)
                
-               199         166 LOAD_CLASSDEREF          0 (db)
+               204         166 LOAD_CLASSDEREF          0 (db)
                            168 LOAD_METHOD              4 (Column)
                            190 LOAD_CLASSDEREF          0 (db)
                            192 LOAD_ATTR                9 (Float)
                            202 LOAD_CONST               5 (False)
                            204 LOAD_CONST               6 (0.0)
                            206 KW_NAMES                 7
                            208 PRECALL                  3
                            212 CALL                     3
                            222 STORE_NAME              10 (dppx)
                
-               200         224 LOAD_CLASSDEREF          0 (db)
+               205         224 LOAD_CLASSDEREF          0 (db)
                            226 LOAD_METHOD              4 (Column)
                            248 LOAD_CLASSDEREF          0 (db)
                            250 LOAD_ATTR                5 (Integer)
                            260 LOAD_CONST               5 (False)
                            262 LOAD_CONST               8 (0)
                            264 KW_NAMES                 7
                            266 PRECALL                  3
                            270 CALL                     3
                            280 STORE_NAME              11 (screenWidth)
                
-               201         282 LOAD_CLASSDEREF          0 (db)
+               206         282 LOAD_CLASSDEREF          0 (db)
                            284 LOAD_METHOD              4 (Column)
                            306 LOAD_CLASSDEREF          0 (db)
                            308 LOAD_ATTR                5 (Integer)
                            318 LOAD_CONST               5 (False)
                            320 LOAD_CONST               8 (0)
                            322 KW_NAMES                 7
                            324 PRECALL                  3
                            328 CALL                     3
                            338 STORE_NAME              12 (screenHeight)
                
-               202         340 LOAD_CLASSDEREF          0 (db)
+               207         340 LOAD_CLASSDEREF          0 (db)
                            342 LOAD_METHOD              4 (Column)
                            364 LOAD_CLASSDEREF          0 (db)
                            366 LOAD_ATTR                5 (Integer)
                            376 LOAD_CONST               5 (False)
                            378 LOAD_CONST               8 (0)
                            380 KW_NAMES                 7
                            382 PRECALL                  3
                            386 CALL                     3
                            396 STORE_NAME              13 (innerWidth)
                
-               203         398 LOAD_CLASSDEREF          0 (db)
+               208         398 LOAD_CLASSDEREF          0 (db)
                            400 LOAD_METHOD              4 (Column)
                            422 LOAD_CLASSDEREF          0 (db)
                            424 LOAD_ATTR                5 (Integer)
                            434 LOAD_CONST               5 (False)
                            436 LOAD_CONST               8 (0)
                            438 KW_NAMES                 7
                            440 PRECALL                  3
@@ -1817,15 +1847,15 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'Integer', 'logDisplayID', 'ForeignKey', 'participantID', 'Float', 'dppx', 'screenWidth', 'screenHeight', 'innerWidth', 'innerHeight')
                varnames   ()
                freevars   ('db',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                name       'Display'
-               firstlineno 194
+               firstlineno 199
                lnotab 0x0c0104023a015c013a013a013a013a01
             'Display'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 6
                flags     : 0
@@ -1844,105 +1874,105 @@
                   006a0d0000000000000000a6010000ab0100000000000000005a0e9400a0
                   04000000000000000000000000000000000000000094006a0d0000000000
                   0000006407650f6a100000000000000000ac08a6030000ab030000000000
                   0000005a11640984005a126513640a65146602640b8404a6000000ab0000
                   000000000000005a15640c5300
                              0 COPY_FREE_VARS           1
                
-               206           2 RESUME                   0
+               211           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create.<locals>.SessionStore')
                             10 STORE_NAME               2 (__qualname__)
                
-               207          12 LOAD_CONST               1 ('session_store')
+               212          12 LOAD_CONST               1 ('session_store')
                             14 STORE_NAME               3 (__tablename__)
                
-               209          16 LOAD_CLASSDEREF          0 (db)
+               214          16 LOAD_CLASSDEREF          0 (db)
                             18 LOAD_METHOD              4 (Column)
                             40 LOAD_CLASSDEREF          0 (db)
                             42 LOAD_METHOD              5 (String)
                             64 LOAD_CONST               2 (255)
                             66 PRECALL                  1
                             70 CALL                     1
                             80 LOAD_CONST               3 (True)
                             82 KW_NAMES                 4
                             84 PRECALL                  2
                             88 CALL                     2
                             98 STORE_NAME               6 (sessionID)
                
-               210         100 LOAD_CLASSDEREF          0 (db)
+               215         100 LOAD_CLASSDEREF          0 (db)
                            102 LOAD_METHOD              4 (Column)
                            124 LOAD_CLASSDEREF          0 (db)
                            126 LOAD_ATTR                7 (Integer)
                            136 LOAD_CLASSDEREF          0 (db)
                            138 LOAD_METHOD              8 (ForeignKey)
                            160 LOAD_CONST               5 ('participant.participantID')
                            162 PRECALL                  1
                            166 CALL                     1
                            176 LOAD_CONST               3 (True)
                            178 KW_NAMES                 6
                            180 PRECALL                  3
                            184 CALL                     3
                            194 STORE_NAME               9 (participantID)
                
-               211         196 LOAD_CLASSDEREF          0 (db)
+               216         196 LOAD_CLASSDEREF          0 (db)
                            198 LOAD_METHOD              4 (Column)
                            220 LOAD_CLASSDEREF          0 (db)
                            222 LOAD_ATTR               10 (Text)
                            232 LOAD_CONST               3 (True)
                            234 KW_NAMES                 6
                            236 PRECALL                  2
                            240 CALL                     2
                            250 STORE_NAME              11 (mTurkID)
                
-               212         252 LOAD_CLASSDEREF          0 (db)
+               217         252 LOAD_CLASSDEREF          0 (db)
                            254 LOAD_METHOD              4 (Column)
                            276 LOAD_CLASSDEREF          0 (db)
                            278 LOAD_ATTR               10 (Text)
                            288 PRECALL                  1
                            292 CALL                     1
                            302 STORE_NAME              12 (data)
                
-               213         304 LOAD_CLASSDEREF          0 (db)
+               218         304 LOAD_CLASSDEREF          0 (db)
                            306 LOAD_METHOD              4 (Column)
                            328 LOAD_CLASSDEREF          0 (db)
                            330 LOAD_ATTR               13 (DateTime)
                            340 PRECALL                  1
                            344 CALL                     1
                            354 STORE_NAME              14 (expiry)
                
-               214         356 LOAD_CLASSDEREF          0 (db)
+               219         356 LOAD_CLASSDEREF          0 (db)
                            358 LOAD_METHOD              4 (Column)
                            380 LOAD_CLASSDEREF          0 (db)
                            382 LOAD_ATTR               13 (DateTime)
                            392 LOAD_CONST               7 (False)
                            394 LOAD_NAME               15 (datetime)
                            396 LOAD_ATTR               16 (utcnow)
                            406 KW_NAMES                 8
                            408 PRECALL                  3
                            412 CALL                     3
                            422 STORE_NAME              17 (createdOn)
                
-               216         424 LOAD_CONST               9 (<code object __repr__, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 216>)
+               221         424 LOAD_CONST               9 (<code object __repr__, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 221>)
                            426 MAKE_FUNCTION            0
                            428 STORE_NAME              18 (__repr__)
                
-               219         430 LOAD_NAME               19 (property)
+               224         430 LOAD_NAME               19 (property)
                
-               220         432 LOAD_CONST              10 ('return')
+               225         432 LOAD_CONST              10 ('return')
                            434 LOAD_NAME               20 (bool)
                            436 BUILD_TUPLE              2
-                           438 LOAD_CONST              11 (<code object expired, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 219>)
+                           438 LOAD_CONST              11 (<code object expired, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 224>)
                            440 MAKE_FUNCTION            4 (annotations)
                
-               219         442 PRECALL                  0
+               224         442 PRECALL                  0
                            446 CALL                     0
                
-               220         456 STORE_NAME              21 (expired)
+               225         456 STORE_NAME              21 (expired)
                            458 LOAD_CONST              12 (None)
                            460 RETURN_VALUE
                consts
                   'create.<locals>.SessionStore'
                   'session_store'
                   255
                   True
@@ -1955,17 +1985,17 @@
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 3
                      flags     : 19
                      code
                         0x97006401a00000000000000000000000000000000000000000007c006a
                         010000000000000000a6010000ab0100000000000000005300
-                     216           0 RESUME                   0
+                     221           0 RESUME                   0
                      
-                     217           2 LOAD_CONST               1 ('<Session data {0!s}>')
+                     222           2 LOAD_CONST               1 ('<Session data {0!s}>')
                                    4 LOAD_METHOD              0 (format)
                                   26 LOAD_FAST                0 (self)
                                   28 LOAD_ATTR                1 (data)
                                   38 PRECALL                  1
                                   42 CALL                     1
                                   52 RETURN_VALUE
                      consts
@@ -1973,29 +2003,29 @@
                         '<Session data {0!s}>'
                      names      ('format', 'data')
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       '__repr__'
-                     firstlineno 216
+                     firstlineno 221
                      lnotab 0x0201
                   'return'
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 3
                      flags     : 19
                      code
                         0x97007c006a00000000000000000064007500701b7c006a000000000000
                         0000007403000000000000000000006a020000000000000000a6000000ab
                         0000000000000000006b01000000005300
-                     219           0 RESUME                   0
+                     224           0 RESUME                   0
                      
-                     221           2 LOAD_FAST                0 (self)
+                     226           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (expiry)
                                   14 LOAD_CONST               0 (None)
                                   16 IS_OP                    0
                                   18 JUMP_IF_TRUE_OR_POP     27 (to 74)
                                   20 LOAD_FAST                0 (self)
                                   22 LOAD_ATTR                0 (expiry)
                                   32 LOAD_GLOBAL              3 (NULL + datetime)
@@ -2008,34 +2038,34 @@
                         None
                      names      ('expiry', 'datetime', 'utcnow')
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'expired'
-                     firstlineno 219
+                     firstlineno 224
                      lnotab 0x0202
                   None
                names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'String', 'sessionID', 'Integer', 'ForeignKey', 'participantID', 'Text', 'mTurkID', 'data', 'DateTime', 'expiry', 'datetime', 'utcnow', 'createdOn', '__repr__', 'property', 'bool', 'expired')
                varnames   ()
                freevars   ('db',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                name       'SessionStore'
-               firstlineno 206
+               firstlineno 211
                lnotab 0x0c010402540160013801340134014402060302010aff0e01
             'SessionStore'
          names      ('Model',)
          varnames   ('db', 'Participant', 'Progress', 'RadioGridLog', 'Display', 'SessionStore')
          freevars   ()
          cellvars   ('db',)
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
          name       'create'
          firstlineno 9
-         lnotab 0x04012a7f001b2a122a0c2a0c2a11
+         lnotab 0x04012a7f00202a122a0c2a0c2a11
       None
    names      ('datetime', 'timedelta', 'sqlalchemy.ext.hybrid', 'hybrid_property', 'sqlalchemy.orm', 'column_property', 'sqlalchemy.ext.declarative', 'declared_attr', 'BOFS.util', 'display_time', 'flask', 'current_app', 'create')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
    name       '<module>'
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/default/__pycache__/views.cpython-310.pyc` & `bride-of-frankensystem-1.9.3.4/BOFS/default/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/default/__pycache__/views.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.4/BOFS/default/__pycache__/views.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x7ef10c66 (Wed Apr  3 06:04:46 2024 UTC)
-files sz: 17678
+moddate:  0xb6e71266 (Sun Apr  7 18:36:38 2024 UTC)
+files sz: 17838
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a036d045a046d055a0501
@@ -375,208 +375,208 @@
               1064 MAKE_FUNCTION            4 (annotations)
    
    234        1066 PRECALL                  0
               1070 CALL                     0
    
    235        1080 STORE_NAME              35 (route_questionnaire_question)
    
-   252        1082 LOAD_NAME               21 (default)
+   255        1082 LOAD_NAME               21 (default)
               1084 LOAD_METHOD             22 (route)
               1106 LOAD_CONST              36 ('/redirect_previous_page')
               1108 PRECALL                  1
               1112 CALL                     1
    
-   253        1122 LOAD_CONST              37 (<code object route_redirect_previous_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 252>)
+   256        1122 LOAD_CONST              37 (<code object route_redirect_previous_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 255>)
               1124 MAKE_FUNCTION            0
    
-   252        1126 PRECALL                  0
+   255        1126 PRECALL                  0
               1130 CALL                     0
    
-   253        1140 STORE_NAME              36 (route_redirect_previous_page)
+   256        1140 STORE_NAME              36 (route_redirect_previous_page)
    
-   265        1142 LOAD_NAME               21 (default)
+   268        1142 LOAD_NAME               21 (default)
               1144 LOAD_METHOD             22 (route)
               1166 LOAD_CONST              38 ('/redirect_next_page')
               1168 PRECALL                  1
               1172 CALL                     1
    
-   266        1182 LOAD_CONST              39 (<code object route_redirect_next_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 265>)
+   269        1182 LOAD_CONST              39 (<code object route_redirect_next_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 268>)
               1184 MAKE_FUNCTION            0
    
-   265        1186 PRECALL                  0
+   268        1186 PRECALL                  0
               1190 CALL                     0
    
-   266        1200 STORE_NAME              37 (route_redirect_next_page)
+   269        1200 STORE_NAME              37 (route_redirect_next_page)
    
-   289        1202 LOAD_NAME               21 (default)
+   292        1202 LOAD_NAME               21 (default)
               1204 LOAD_METHOD             22 (route)
               1226 LOAD_CONST              40 ('/redirect_from_page/<path:page>')
               1228 PRECALL                  1
               1232 CALL                     1
    
-   290        1242 LOAD_CONST              41 (<code object route_redirect_from_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 289>)
+   293        1242 LOAD_CONST              41 (<code object route_redirect_from_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 292>)
               1244 MAKE_FUNCTION            0
    
-   289        1246 PRECALL                  0
+   292        1246 PRECALL                  0
               1250 CALL                     0
    
-   290        1260 STORE_NAME              38 (route_redirect_from_page)
+   293        1260 STORE_NAME              38 (route_redirect_from_page)
    
-   304        1262 LOAD_NAME               21 (default)
+   307        1262 LOAD_NAME               21 (default)
               1264 LOAD_METHOD             22 (route)
               1286 LOAD_CONST              42 ('/redirect_to_page/<path:page>')
               1288 PRECALL                  1
               1292 CALL                     1
    
-   305        1302 LOAD_CONST              43 (<code object route_redirect_to_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 304>)
+   308        1302 LOAD_CONST              43 (<code object route_redirect_to_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 307>)
               1304 MAKE_FUNCTION            0
    
-   304        1306 PRECALL                  0
+   307        1306 PRECALL                  0
               1310 CALL                     0
    
-   305        1320 STORE_NAME              39 (route_redirect_to_page)
+   308        1320 STORE_NAME              39 (route_redirect_to_page)
    
-   319        1322 LOAD_NAME               21 (default)
+   322        1322 LOAD_NAME               21 (default)
               1324 LOAD_METHOD             22 (route)
               1346 LOAD_CONST              44 ('/end')
               1348 PRECALL                  1
               1352 CALL                     1
    
-   320        1362 LOAD_NAME               23 (verify_correct_page)
+   323        1362 LOAD_NAME               23 (verify_correct_page)
    
-   321        1364 LOAD_NAME               29 (verify_session_valid)
+   324        1364 LOAD_NAME               29 (verify_session_valid)
    
-   322        1366 LOAD_CONST              45 (<code object route_end, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 319>)
+   325        1366 LOAD_CONST              45 (<code object route_end, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 322>)
               1368 MAKE_FUNCTION            0
    
-   321        1370 PRECALL                  0
+   324        1370 PRECALL                  0
               1374 CALL                     0
    
-   320        1384 PRECALL                  0
+   323        1384 PRECALL                  0
               1388 CALL                     0
    
-   319        1398 PRECALL                  0
+   322        1398 PRECALL                  0
               1402 CALL                     0
    
-   322        1412 STORE_NAME              40 (route_end)
+   325        1412 STORE_NAME              40 (route_end)
    
-   342        1414 LOAD_NAME               21 (default)
+   345        1414 LOAD_NAME               21 (default)
               1416 LOAD_METHOD             22 (route)
               1438 LOAD_CONST              46 ('/user_active')
               1440 PRECALL                  1
               1444 CALL                     1
    
-   343        1454 LOAD_CONST              47 (<code object route_user_active, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 342>)
+   346        1454 LOAD_CONST              47 (<code object route_user_active, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 345>)
               1456 MAKE_FUNCTION            0
    
-   342        1458 PRECALL                  0
+   345        1458 PRECALL                  0
               1462 CALL                     0
    
-   343        1472 STORE_NAME              41 (route_user_active)
+   346        1472 STORE_NAME              41 (route_user_active)
    
-   351        1474 LOAD_NAME               21 (default)
+   354        1474 LOAD_NAME               21 (default)
               1476 LOAD_METHOD             22 (route)
               1498 LOAD_CONST              48 ('/current_url')
               1500 PRECALL                  1
               1504 CALL                     1
    
-   352        1514 LOAD_CONST              49 (<code object route_current_url, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 351>)
+   355        1514 LOAD_CONST              49 (<code object route_current_url, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 354>)
               1516 MAKE_FUNCTION            0
    
-   351        1518 PRECALL                  0
+   354        1518 PRECALL                  0
               1522 CALL                     0
    
-   352        1532 STORE_NAME              42 (route_current_url)
+   355        1532 STORE_NAME              42 (route_current_url)
    
-   364        1534 LOAD_NAME               21 (default)
+   367        1534 LOAD_NAME               21 (default)
               1536 LOAD_METHOD             22 (route)
               1558 LOAD_CONST              50 ('/restart')
               1560 PRECALL                  1
               1564 CALL                     1
    
-   365        1574 LOAD_CONST              51 (<code object route_restart, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 364>)
+   368        1574 LOAD_CONST              51 (<code object route_restart, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 367>)
               1576 MAKE_FUNCTION            0
    
-   364        1578 PRECALL                  0
+   367        1578 PRECALL                  0
               1582 CALL                     0
    
-   365        1592 STORE_NAME              43 (route_restart)
+   368        1592 STORE_NAME              43 (route_restart)
    
-   399        1594 LOAD_NAME               21 (default)
+   402        1594 LOAD_NAME               21 (default)
               1596 LOAD_METHOD             22 (route)
               1618 LOAD_CONST              52 ('/submit')
               1620 LOAD_CONST              11 ('POST')
               1622 BUILD_LIST               1
               1624 KW_NAMES                13
               1626 PRECALL                  2
               1630 CALL                     2
    
-   400        1640 LOAD_CONST              53 (<code object submit, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 399>)
+   403        1640 LOAD_CONST              53 (<code object submit, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 402>)
               1642 MAKE_FUNCTION            0
    
-   399        1644 PRECALL                  0
+   402        1644 PRECALL                  0
               1648 CALL                     0
    
-   400        1658 STORE_NAME              44 (submit)
+   403        1658 STORE_NAME              44 (submit)
    
-   413        1660 LOAD_NAME               21 (default)
+   416        1660 LOAD_NAME               21 (default)
               1662 LOAD_METHOD             22 (route)
               1684 LOAD_CONST              54 ('/instructions/<pageName>')
               1686 LOAD_CONST              11 ('POST')
               1688 LOAD_CONST              12 ('GET')
               1690 BUILD_LIST               2
               1692 KW_NAMES                13
               1694 PRECALL                  2
               1698 CALL                     2
    
-   414        1708 LOAD_NAME               23 (verify_correct_page)
+   417        1708 LOAD_NAME               23 (verify_correct_page)
    
-   415        1710 LOAD_NAME               29 (verify_session_valid)
+   418        1710 LOAD_NAME               29 (verify_session_valid)
    
-   416        1712 LOAD_CONST              55 (<code object route_instructions, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 413>)
+   419        1712 LOAD_CONST              55 (<code object route_instructions, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 416>)
               1714 MAKE_FUNCTION            0
    
-   415        1716 PRECALL                  0
+   418        1716 PRECALL                  0
               1720 CALL                     0
    
-   414        1730 PRECALL                  0
+   417        1730 PRECALL                  0
               1734 CALL                     0
    
-   413        1744 PRECALL                  0
+   416        1744 PRECALL                  0
               1748 CALL                     0
    
-   416        1758 STORE_NAME              45 (route_instructions)
+   419        1758 STORE_NAME              45 (route_instructions)
    
-   442        1760 LOAD_NAME               21 (default)
+   445        1760 LOAD_NAME               21 (default)
               1762 LOAD_METHOD             22 (route)
               1784 LOAD_CONST              56 ('/simple/<pageName>')
               1786 LOAD_CONST              11 ('POST')
               1788 LOAD_CONST              12 ('GET')
               1790 BUILD_LIST               2
               1792 KW_NAMES                13
               1794 PRECALL                  2
               1798 CALL                     2
    
-   443        1808 LOAD_NAME               23 (verify_correct_page)
+   446        1808 LOAD_NAME               23 (verify_correct_page)
    
-   444        1810 LOAD_NAME               29 (verify_session_valid)
+   447        1810 LOAD_NAME               29 (verify_session_valid)
    
-   445        1812 LOAD_CONST              57 (<code object route_simple_html, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 442>)
+   448        1812 LOAD_CONST              57 (<code object route_simple_html, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 445>)
               1814 MAKE_FUNCTION            0
    
-   444        1816 PRECALL                  0
+   447        1816 PRECALL                  0
               1820 CALL                     0
    
-   443        1830 PRECALL                  0
+   446        1830 PRECALL                  0
               1834 CALL                     0
    
-   442        1844 PRECALL                  0
+   445        1844 PRECALL                  0
               1848 CALL                     0
    
-   445        1858 STORE_NAME              46 (route_simple_html)
+   448        1858 STORE_NAME              46 (route_simple_html)
               1860 LOAD_CONST              58 (None)
               1862 RETURN_VALUE
    consts
       0
       ('Blueprint', 'render_template', 'current_app', 'request', 'make_response')
       ('urlsplit',)
       ('JSONTable',)
@@ -1396,145 +1396,159 @@
       'questionType'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
-            0x97007400000000000000000000006a0100000000000000006a02000000
-            0000000000a0030000000000000000000000000000000000000000740800
-            000000000000000000640119000000000000000000a6010000ab01000000
-            00000000007d010900740b0000000000000000000064027c009b0064039d
-            03740c000000000000000000006a0700000000000000007c01ac04a60300
-            00ab03000000000000000053002300741000000000000000000000240072
-            127d0264057c009b0064067c029b009d046302590064077d027e02530064
-            077d027e0277017700780359007701
+            0x970064017400000000000000000000007601720f740300000000000000
+            0000006402a6010000ab0100000000000000008201740400000000000000
+            0000006a0300000000000000006a040000000000000000a0050000000000
+            000000000000000000000000000000740000000000000000000000640119
+            000000000000000000a6010000ab0100000000000000007d010900740d00
+            00000000000000000064037c009b0064049d03740e000000000000000000
+            006a0800000000000000007c01ac05a6030000ab03000000000000000053
+            002300740200000000000000000000240072127d0264067c009b0064077c
+            029b009d046302590064087d027e02530064087d027e0277017700780359
+            007701
          234           0 RESUME                   0
          
-         242           2 LOAD_GLOBAL              0 (db)
-                      14 LOAD_ATTR                1 (Participant)
-                      24 LOAD_ATTR                2 (query)
-                      34 LOAD_METHOD              3 (get)
-                      56 LOAD_GLOBAL              8 (session)
-                      68 LOAD_CONST               1 ('participantID')
-                      70 BINARY_SUBSCR
-                      80 PRECALL                  1
-                      84 CALL                     1
-                      94 STORE_FAST               1 (participant)
+         242           2 LOAD_CONST               1 ('participantID')
+                       4 LOAD_GLOBAL              0 (session)
+                      16 CONTAINS_OP              1
+                      18 POP_JUMP_FORWARD_IF_FALSE    15 (to 50)
+         
+         243          20 LOAD_GLOBAL              3 (NULL + Exception)
+                      32 LOAD_CONST               2 ('Error: No participantID in session. Did you forget /consent or /create_participant, etc.?')
+                      34 PRECALL                  1
+                      38 CALL                     1
+                      48 RAISE_VARARGS            1
+         
+         245     >>   50 LOAD_GLOBAL              4 (db)
+                      62 LOAD_ATTR                3 (Participant)
+                      72 LOAD_ATTR                4 (query)
+                      82 LOAD_METHOD              5 (get)
+                     104 LOAD_GLOBAL              0 (session)
+                     116 LOAD_CONST               1 ('participantID')
+                     118 BINARY_SUBSCR
+                     128 PRECALL                  1
+                     132 CALL                     1
+                     142 STORE_FAST               1 (participant)
          
-         244          96 NOP
+         247         144 NOP
          
-         245          98 LOAD_GLOBAL             11 (NULL + render_template)
-                     110 LOAD_CONST               2 ('questions/')
-                     112 LOAD_FAST                0 (questionType)
-                     114 FORMAT_VALUE             0
-                     116 LOAD_CONST               3 ('.html')
-                     118 BUILD_STRING             3
-         
-         246         120 LOAD_GLOBAL             12 (request)
-                     132 LOAD_ATTR                7 (json)
-         
-         247         142 LOAD_FAST                1 (participant)
-         
-         245         144 KW_NAMES                 4
-                     146 PRECALL                  3
-                     150 CALL                     3
-                     160 RETURN_VALUE
-                 >>  162 PUSH_EXC_INFO
-         
-         248         164 LOAD_GLOBAL             16 (Exception)
-                     176 CHECK_EXC_MATCH
-                     178 POP_JUMP_FORWARD_IF_FALSE    18 (to 216)
-                     180 STORE_FAST               2 (ex)
-         
-         249         182 LOAD_CONST               5 ('Exception in <b>')
-                     184 LOAD_FAST                0 (questionType)
-                     186 FORMAT_VALUE             0
-                     188 LOAD_CONST               6 ('.html</b>: ')
-                     190 LOAD_FAST                2 (ex)
-                     192 FORMAT_VALUE             0
-                     194 BUILD_STRING             4
-                     196 SWAP                     2
-                     198 POP_EXCEPT
-                     200 LOAD_CONST               7 (None)
-                     202 STORE_FAST               2 (ex)
-                     204 DELETE_FAST              2 (ex)
-                     206 RETURN_VALUE
-                 >>  208 LOAD_CONST               7 (None)
-                     210 STORE_FAST               2 (ex)
-                     212 DELETE_FAST              2 (ex)
-                     214 RERAISE                  1
-         
-         248     >>  216 RERAISE                  0
-                 >>  218 COPY                     3
-                     220 POP_EXCEPT
-                     222 RERAISE                  1
+         248         146 LOAD_GLOBAL             13 (NULL + render_template)
+                     158 LOAD_CONST               3 ('questions/')
+                     160 LOAD_FAST                0 (questionType)
+                     162 FORMAT_VALUE             0
+                     164 LOAD_CONST               4 ('.html')
+                     166 BUILD_STRING             3
+         
+         249         168 LOAD_GLOBAL             14 (request)
+                     180 LOAD_ATTR                8 (json)
+         
+         250         190 LOAD_FAST                1 (participant)
+         
+         248         192 KW_NAMES                 5
+                     194 PRECALL                  3
+                     198 CALL                     3
+                     208 RETURN_VALUE
+                 >>  210 PUSH_EXC_INFO
+         
+         251         212 LOAD_GLOBAL              2 (Exception)
+                     224 CHECK_EXC_MATCH
+                     226 POP_JUMP_FORWARD_IF_FALSE    18 (to 264)
+                     228 STORE_FAST               2 (ex)
+         
+         252         230 LOAD_CONST               6 ('Exception in <b>')
+                     232 LOAD_FAST                0 (questionType)
+                     234 FORMAT_VALUE             0
+                     236 LOAD_CONST               7 ('.html</b>: ')
+                     238 LOAD_FAST                2 (ex)
+                     240 FORMAT_VALUE             0
+                     242 BUILD_STRING             4
+                     244 SWAP                     2
+                     246 POP_EXCEPT
+                     248 LOAD_CONST               8 (None)
+                     250 STORE_FAST               2 (ex)
+                     252 DELETE_FAST              2 (ex)
+                     254 RETURN_VALUE
+                 >>  256 LOAD_CONST               8 (None)
+                     258 STORE_FAST               2 (ex)
+                     260 DELETE_FAST              2 (ex)
+                     262 RERAISE                  1
+         
+         251     >>  264 RERAISE                  0
+                 >>  266 COPY                     3
+                     268 POP_EXCEPT
+                     270 RERAISE                  1
          ExceptionTable:
-           98 to 158 -> 162 [0]
-           162 to 180 -> 218 [1] lasti
-           182 to 194 -> 208 [1] lasti
-           196 to 196 -> 218 [1] lasti
-           208 to 216 -> 218 [1] lasti
+           146 to 206 -> 210 [0]
+           210 to 228 -> 266 [1] lasti
+           230 to 242 -> 256 [1] lasti
+           244 to 244 -> 266 [1] lasti
+           256 to 264 -> 266 [1] lasti
          consts
             '\n    ``/questionnaire_question/<questionType>``\n\n    Render a specific question type for the questionnaire. Only accepts POST requests.\n    Data posted to this route must be a JSON object of the question data.\n    '
             'participantID'
+            'Error: No participantID in session. Did you forget /consent or /create_participant, etc.?'
             'questions/'
             '.html'
             ('question', 'participant')
             'Exception in <b>'
             '.html</b>: '
             None
-         names      ('db', 'Participant', 'query', 'get', 'session', 'render_template', 'request', 'json', 'Exception')
+         names      ('session', 'Exception', 'db', 'Participant', 'query', 'get', 'render_template', 'request', 'json')
          varnames   ('questionType', 'participant', 'ex')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_questionnaire_question'
          firstlineno 234
-         lnotab 0x02085e0202011601160102fe1403120122ff
+         lnotab 0x020812011e025e0202011601160102fe1403120122ff
       '/redirect_previous_page'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007404000000
             00000000000000640119000000000000000000a6010000ab010000000000
             00000074040000000000000000000064013c000000740600000000000000
             0000006a04000000000000000064021900000000000000000064037a0000
             007404000000000000000000006401190000000000000000007a0000007d
             00740b000000000000000000007c00a6010000ab01000000000000000053
             00
-         252           0 RESUME                   0
+         255           0 RESUME                   0
          
-         259           2 LOAD_GLOBAL              1 (NULL + page_list)
+         262           2 LOAD_GLOBAL              1 (NULL + page_list)
                       14 LOAD_ATTR                1 (previous_path)
                       24 LOAD_GLOBAL              4 (session)
                       36 LOAD_CONST               1 ('currentUrl')
                       38 BINARY_SUBSCR
                       48 PRECALL                  1
                       52 CALL                     1
                       62 LOAD_GLOBAL              4 (session)
                       74 LOAD_CONST               1 ('currentUrl')
                       76 STORE_SUBSCR
          
-         260          80 LOAD_GLOBAL              6 (current_app)
+         263          80 LOAD_GLOBAL              6 (current_app)
                       92 LOAD_ATTR                4 (config)
                      102 LOAD_CONST               2 ('APPLICATION_ROOT')
                      104 BINARY_SUBSCR
                      114 LOAD_CONST               3 ('/')
                      116 BINARY_OP                0 (+)
                      120 LOAD_GLOBAL              4 (session)
                      132 LOAD_CONST               1 ('currentUrl')
                      134 BINARY_SUBSCR
                      144 BINARY_OP                0 (+)
                      148 STORE_FAST               0 (nextUrl)
          
-         262         150 LOAD_GLOBAL             11 (NULL + redirect)
+         265         150 LOAD_GLOBAL             11 (NULL + redirect)
                      162 LOAD_FAST                0 (nextUrl)
                      164 PRECALL                  1
                      168 CALL                     1
                      178 RETURN_VALUE
          consts
             '\n    ``/redirect_previous_page``\n\n    Sends a user to the previous page. This is intended primarily for debugging purposes.\n    '
             'currentUrl'
@@ -1542,15 +1556,15 @@
             '/'
          names      ('page_list', 'previous_path', 'session', 'current_app', 'config', 'redirect')
          varnames   ('nextUrl',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_redirect_previous_page'
-         firstlineno 252
+         firstlineno 255
          lnotab 0x02074e014602
       '/redirect_next_page'
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 4
          flags     : 3
@@ -1564,77 +1578,77 @@
             041900000000000000000064057a000000a6010000ab0100000000000000
             0053007411000000000000000000006a0900000000000000007c01a60100
             00ab01000000000000000074080000000000000000000064023c00000074
             0c000000000000000000006a070000000000000000640419000000000000
             00000064067a000000740800000000000000000000640219000000000000
             0000007a0000007d02740b000000000000000000007c02a6010000ab0100
             000000000000005300
-         265           0 RESUME                   0
+         268           0 RESUME                   0
          
-         272           2 LOAD_GLOBAL              0 (request)
+         275           2 LOAD_GLOBAL              0 (request)
                       14 POP_JUMP_FORWARD_IF_NONE    45 (to 106)
                       16 LOAD_GLOBAL              0 (request)
                       28 LOAD_ATTR                1 (referrer)
                       38 POP_JUMP_FORWARD_IF_NONE    33 (to 106)
          
-         273          40 LOAD_GLOBAL              5 (NULL + urlsplit)
+         276          40 LOAD_GLOBAL              5 (NULL + urlsplit)
                       52 LOAD_GLOBAL              0 (request)
                       64 LOAD_ATTR                1 (referrer)
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_FAST               0 (parsed)
          
-         274          90 LOAD_FAST                0 (parsed)
+         277          90 LOAD_FAST                0 (parsed)
                       92 LOAD_ATTR                3 (path)
                      102 STORE_FAST               1 (current_page)
                      104 JUMP_FORWARD            13 (to 132)
          
-         278     >>  106 LOAD_GLOBAL              8 (session)
+         281     >>  106 LOAD_GLOBAL              8 (session)
                      118 LOAD_CONST               2 ('currentUrl')
                      120 BINARY_SUBSCR
                      130 STORE_FAST               1 (current_page)
          
-         280     >>  132 LOAD_FAST                1 (current_page)
+         283     >>  132 LOAD_FAST                1 (current_page)
                      134 LOAD_CONST               3 ('end')
                      136 COMPARE_OP               2 (==)
                      142 POP_JUMP_FORWARD_IF_FALSE    34 (to 212)
          
-         281         144 LOAD_GLOBAL             11 (NULL + redirect)
+         284         144 LOAD_GLOBAL             11 (NULL + redirect)
                      156 LOAD_GLOBAL             12 (current_app)
                      168 LOAD_ATTR                7 (config)
                      178 LOAD_CONST               4 ('APPLICATION_ROOT')
                      180 BINARY_SUBSCR
                      190 LOAD_CONST               5 ('/end')
                      192 BINARY_OP                0 (+)
                      196 PRECALL                  1
                      200 CALL                     1
                      210 RETURN_VALUE
          
-         283     >>  212 LOAD_GLOBAL             17 (NULL + page_list)
+         286     >>  212 LOAD_GLOBAL             17 (NULL + page_list)
                      224 LOAD_ATTR                9 (next_path)
                      234 LOAD_FAST                1 (current_page)
                      236 PRECALL                  1
                      240 CALL                     1
                      250 LOAD_GLOBAL              8 (session)
                      262 LOAD_CONST               2 ('currentUrl')
                      264 STORE_SUBSCR
          
-         284         268 LOAD_GLOBAL             12 (current_app)
+         287         268 LOAD_GLOBAL             12 (current_app)
                      280 LOAD_ATTR                7 (config)
                      290 LOAD_CONST               4 ('APPLICATION_ROOT')
                      292 BINARY_SUBSCR
                      302 LOAD_CONST               6 ('/')
                      304 BINARY_OP                0 (+)
                      308 LOAD_GLOBAL              8 (session)
                      320 LOAD_CONST               2 ('currentUrl')
                      322 BINARY_SUBSCR
                      332 BINARY_OP                0 (+)
                      336 STORE_FAST               2 (nextUrl)
          
-         286         338 LOAD_GLOBAL             11 (NULL + redirect)
+         289         338 LOAD_GLOBAL             11 (NULL + redirect)
                      350 LOAD_FAST                2 (nextUrl)
                      352 PRECALL                  1
                      356 CALL                     1
                      366 RETURN_VALUE
          consts
             '\n    ``/redirect_next_page``\n\n    This is the preferred way of sending a user to the next page.\n    '
             None
@@ -1645,53 +1659,53 @@
             '/'
          names      ('request', 'referrer', 'urlsplit', 'path', 'session', 'redirect', 'current_app', 'config', 'page_list', 'next_path')
          varnames   ('parsed', 'current_page', 'nextUrl')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_redirect_next_page'
-         firstlineno 265
+         firstlineno 268
          lnotab 0x02072601320110041a020c01440238014602
       '/redirect_from_page/<path:page>'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c00a60100
             00ab01000000000000000074040000000000000000000064013c00000074
             06000000000000000000006a040000000000000000640219000000000000
             00000064037a000000740400000000000000000000640119000000000000
             0000007a0000007d01740b000000000000000000007c01a6010000ab0100
             000000000000005300
-         289           0 RESUME                   0
+         292           0 RESUME                   0
          
-         298           2 LOAD_GLOBAL              1 (NULL + page_list)
+         301           2 LOAD_GLOBAL              1 (NULL + page_list)
                       14 LOAD_ATTR                1 (next_path)
                       24 LOAD_FAST                0 (page)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 LOAD_GLOBAL              4 (session)
                       52 LOAD_CONST               1 ('currentUrl')
                       54 STORE_SUBSCR
          
-         299          58 LOAD_GLOBAL              6 (current_app)
+         302          58 LOAD_GLOBAL              6 (current_app)
                       70 LOAD_ATTR                4 (config)
                       80 LOAD_CONST               2 ('APPLICATION_ROOT')
                       82 BINARY_SUBSCR
                       92 LOAD_CONST               3 ('/')
                       94 BINARY_OP                0 (+)
                       98 LOAD_GLOBAL              4 (session)
                      110 LOAD_CONST               1 ('currentUrl')
                      112 BINARY_SUBSCR
                      122 BINARY_OP                0 (+)
                      126 STORE_FAST               1 (nextUrl)
          
-         301         128 LOAD_GLOBAL             11 (NULL + redirect)
+         304         128 LOAD_GLOBAL             11 (NULL + redirect)
                      140 LOAD_FAST                1 (nextUrl)
                      142 PRECALL                  1
                      146 CALL                     1
                      156 RETURN_VALUE
          consts
             '\n    ``/redirect_from_page/<path:page>``\n\n    Redirect the user from a specific page.\n\n    :param page: The page to start from, the user will be sent to next page in the list\n    '
             'currentUrl'
@@ -1699,48 +1713,48 @@
             '/'
          names      ('page_list', 'next_path', 'session', 'current_app', 'config', 'redirect')
          varnames   ('page', 'nextUrl')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_redirect_from_page'
-         firstlineno 289
+         firstlineno 292
          lnotab 0x020938014602
       '/redirect_to_page/<path:page>'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007c0074000000000000000000000064013c00000074020000000000
             00000000006a02000000000000000064021900000000000000000064037a
             0000007400000000000000000000006401190000000000000000007a0000
             007d017407000000000000000000007c01a6010000ab0100000000000000
             005300
-         304           0 RESUME                   0
+         307           0 RESUME                   0
          
-         313           2 LOAD_FAST                0 (page)
+         316           2 LOAD_FAST                0 (page)
                        4 LOAD_GLOBAL              0 (session)
                       16 LOAD_CONST               1 ('currentUrl')
                       18 STORE_SUBSCR
          
-         314          22 LOAD_GLOBAL              2 (current_app)
+         317          22 LOAD_GLOBAL              2 (current_app)
                       34 LOAD_ATTR                2 (config)
                       44 LOAD_CONST               2 ('APPLICATION_ROOT')
                       46 BINARY_SUBSCR
                       56 LOAD_CONST               3 ('/')
                       58 BINARY_OP                0 (+)
                       62 LOAD_GLOBAL              0 (session)
                       74 LOAD_CONST               1 ('currentUrl')
                       76 BINARY_SUBSCR
                       86 BINARY_OP                0 (+)
                       90 STORE_FAST               1 (nextUrl)
          
-         316          92 LOAD_GLOBAL              7 (NULL + redirect)
+         319          92 LOAD_GLOBAL              7 (NULL + redirect)
                      104 LOAD_FAST                1 (nextUrl)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 RETURN_VALUE
          consts
             '\n    ``/redirect_to_page/<path:page>``\n\n    Redirect the user to a specific page path in ``PAGE_LIST``\n\n    :param page:\n    '
             'currentUrl'
@@ -1748,15 +1762,15 @@
             '/'
          names      ('session', 'current_app', 'config', 'redirect')
          varnames   ('page', 'nextUrl')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_redirect_to_page'
-         firstlineno 304
+         firstlineno 307
          lnotab 0x020914014602
       '/end'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 5
          flags     : 3
@@ -1773,71 +1787,71 @@
             0b0000000000000000760072317414000000000000000000006a0b000000
             0000000000640419000000000000000000811f7419000000000000000000
             007414000000000000000000006a0b000000000000000064041900000000
             0000000000a6010000ab0100000000000000005300741b00000000000000
             000000640564067408000000000000000000007600720d74080000000000
             00000000006406190000000000000000006e016402ac07a6020000ab0200
             000000000000005300
-         319           0 RESUME                   0
+         322           0 RESUME                   0
          
-         329           2 LOAD_GLOBAL              0 (db)
+         332           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_ATTR                1 (Participant)
                       24 LOAD_ATTR                2 (query)
                       34 LOAD_METHOD              3 (get)
                       56 LOAD_GLOBAL              8 (session)
                       68 LOAD_CONST               1 ('participantID')
                       70 BINARY_SUBSCR
                       80 PRECALL                  1
                       84 CALL                     1
                       94 STORE_FAST               0 (p)
          
-         330          96 LOAD_FAST                0 (p)
+         333          96 LOAD_FAST                0 (p)
                       98 LOAD_ATTR                5 (timeEnded)
                      108 POP_JUMP_FORWARD_IF_NOT_NONE    35 (to 180)
          
-         331         110 LOAD_GLOBAL             12 (datetime)
+         334         110 LOAD_GLOBAL             12 (datetime)
                      122 LOAD_ATTR                6 (datetime)
                      132 LOAD_METHOD              7 (utcnow)
                      154 PRECALL                  0
                      158 CALL                     0
                      168 LOAD_FAST                0 (p)
                      170 STORE_ATTR               5 (timeEnded)
          
-         332     >>  180 LOAD_CONST               3 (True)
+         335     >>  180 LOAD_CONST               3 (True)
                      182 LOAD_FAST                0 (p)
                      184 STORE_ATTR               8 (finished)
          
-         334         194 LOAD_GLOBAL              0 (db)
+         337         194 LOAD_GLOBAL              0 (db)
                      206 LOAD_ATTR                4 (session)
                      216 LOAD_METHOD              9 (commit)
                      238 PRECALL                  0
                      242 CALL                     0
                      252 POP_TOP
          
-         336         254 LOAD_CONST               4 ('OUTGOING_URL')
+         339         254 LOAD_CONST               4 ('OUTGOING_URL')
                      256 LOAD_GLOBAL             20 (current_app)
                      268 LOAD_ATTR               11 (config)
                      278 CONTAINS_OP              0
                      280 POP_JUMP_FORWARD_IF_FALSE    49 (to 380)
                      282 LOAD_GLOBAL             20 (current_app)
                      294 LOAD_ATTR               11 (config)
                      304 LOAD_CONST               4 ('OUTGOING_URL')
                      306 BINARY_SUBSCR
                      316 POP_JUMP_FORWARD_IF_NONE    31 (to 380)
          
-         337         318 LOAD_GLOBAL             25 (NULL + redirect)
+         340         318 LOAD_GLOBAL             25 (NULL + redirect)
                      330 LOAD_GLOBAL             20 (current_app)
                      342 LOAD_ATTR               11 (config)
                      352 LOAD_CONST               4 ('OUTGOING_URL')
                      354 BINARY_SUBSCR
                      364 PRECALL                  1
                      368 CALL                     1
                      378 RETURN_VALUE
          
-         339     >>  380 LOAD_GLOBAL             27 (NULL + render_template)
+         342     >>  380 LOAD_GLOBAL             27 (NULL + render_template)
                      392 LOAD_CONST               5 ('end.html')
                      394 LOAD_CONST               6 ('code')
                      396 LOAD_GLOBAL              8 (session)
                      408 CONTAINS_OP              0
                      410 POP_JUMP_FORWARD_IF_FALSE    13 (to 438)
                      412 LOAD_GLOBAL              8 (session)
                      424 LOAD_CONST               6 ('code')
@@ -1859,15 +1873,15 @@
             ('code',)
          names      ('db', 'Participant', 'query', 'get', 'session', 'timeEnded', 'datetime', 'utcnow', 'finished', 'commit', 'current_app', 'config', 'redirect', 'render_template')
          varnames   ('p',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_end'
-         firstlineno 319
+         firstlineno 322
          lnotab 0x020a5e010e0146010e023c0240013e02
       '/user_active'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
          flags     : 3
@@ -1878,99 +1892,99 @@
             00ab010000000000000000a0040000000000000000000000000000000000
             000000740000000000000000000000640119000000000000000000a60100
             00ab0100000000000000007d00740a000000000000000000006a05000000
             0000000000a0060000000000000000000000000000000000000000a60000
             00ab0000000000000000007c005f07000000000000000074020000000000
             00000000006a000000000000000000a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000010064025300
-         342           0 RESUME                   0
+         345           0 RESUME                   0
          
-         344           2 LOAD_CONST               1 ('participantID')
+         347           2 LOAD_CONST               1 ('participantID')
                        4 LOAD_GLOBAL              0 (session)
                       16 CONTAINS_OP              0
                       18 POP_JUMP_FORWARD_IF_FALSE   136 (to 292)
          
-         345          20 LOAD_GLOBAL              2 (db)
+         348          20 LOAD_GLOBAL              2 (db)
                       32 LOAD_ATTR                0 (session)
                       42 LOAD_METHOD              2 (query)
                       64 LOAD_GLOBAL              2 (db)
                       76 LOAD_ATTR                3 (Participant)
                       86 PRECALL                  1
                       90 CALL                     1
                      100 LOAD_METHOD              4 (get)
                      122 LOAD_GLOBAL              0 (session)
                      134 LOAD_CONST               1 ('participantID')
                      136 BINARY_SUBSCR
                      146 PRECALL                  1
                      150 CALL                     1
                      160 STORE_FAST               0 (participant)
          
-         346         162 LOAD_GLOBAL             10 (datetime)
+         349         162 LOAD_GLOBAL             10 (datetime)
                      174 LOAD_ATTR                5 (datetime)
                      184 LOAD_METHOD              6 (utcnow)
                      206 PRECALL                  0
                      210 CALL                     0
                      220 LOAD_FAST                0 (participant)
                      222 STORE_ATTR               7 (lastActiveOn)
          
-         347         232 LOAD_GLOBAL              2 (db)
+         350         232 LOAD_GLOBAL              2 (db)
                      244 LOAD_ATTR                0 (session)
                      254 LOAD_METHOD              8 (commit)
                      276 PRECALL                  0
                      280 CALL                     0
                      290 POP_TOP
          
-         348     >>  292 LOAD_CONST               2 ('')
+         351     >>  292 LOAD_CONST               2 ('')
                      294 RETURN_VALUE
          consts
             None
             'participantID'
             ''
          names      ('session', 'db', 'query', 'Participant', 'get', 'datetime', 'utcnow', 'lastActiveOn', 'commit')
          varnames   ('participant',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_user_active'
-         firstlineno 342
+         firstlineno 345
          lnotab 0x020212018e0146013c01
       '/current_url'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 3
          code
             0x970064017400000000000000000000007600720d740000000000000000
             000000640119000000000000000000530064025300
-         351           0 RESUME                   0
+         354           0 RESUME                   0
          
-         358           2 LOAD_CONST               1 ('currentUrl')
+         361           2 LOAD_CONST               1 ('currentUrl')
                        4 LOAD_GLOBAL              0 (session)
                       16 CONTAINS_OP              0
                       18 POP_JUMP_FORWARD_IF_FALSE    13 (to 46)
          
-         359          20 LOAD_GLOBAL              0 (session)
+         362          20 LOAD_GLOBAL              0 (session)
                       32 LOAD_CONST               1 ('currentUrl')
                       34 BINARY_SUBSCR
                       44 RETURN_VALUE
          
-         361     >>   46 LOAD_CONST               2 ('/')
+         364     >>   46 LOAD_CONST               2 ('/')
                       48 RETURN_VALUE
          consts
             '\n    ``/current_url``\n\n    :return: The current URL of the user. For a new user, it returns "/".\n    '
             'currentUrl'
             '/'
          names      ('session',)
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_current_url'
-         firstlineno 351
+         firstlineno 354
          lnotab 0x020712011a02
       '/restart'
       code
          argcount  : 0
          nlocals   : 5
          stacksize : 6
          flags     : 3
@@ -1989,110 +2003,110 @@
             0000000000a00a0000000000000000000000000000000000000000a60000
             00ab00000000000000000001007416000000000000000000006a0b000000
             000000000044005d417d0364047c03760172018c077c0364041900000000
             00000000007d047c04a00c00000000000000000000000000000000000000
             006401a6010000ab010000000000000000730564017c047a0000007d047c
             00a00d0000000000000000000000000000000000000000640264057c04ac
             06a6030000ab03000000000000000001008c427c005300
-         364           0 RESUME                   0
+         367           0 RESUME                   0
          
-         373           2 LOAD_GLOBAL              1 (NULL + make_response)
+         376           2 LOAD_GLOBAL              1 (NULL + make_response)
                       14 LOAD_GLOBAL              3 (NULL + redirect)
                       26 LOAD_CONST               1 ('/')
                       28 PRECALL                  1
                       32 CALL                     1
                       42 PRECALL                  1
                       46 CALL                     1
                       56 STORE_FAST               0 (response)
          
-         374          58 LOAD_GLOBAL              4 (request)
+         377          58 LOAD_GLOBAL              4 (request)
                       70 LOAD_ATTR                3 (cookies)
                       80 LOAD_METHOD              4 (get)
                      102 LOAD_CONST               2 ('session')
                      104 LOAD_CONST               3 (None)
                      106 PRECALL                  2
                      110 CALL                     2
                      120 STORE_FAST               1 (sessionID)
          
-         376         122 LOAD_FAST                1 (sessionID)
+         379         122 LOAD_FAST                1 (sessionID)
                      124 POP_JUMP_FORWARD_IF_FALSE   123 (to 372)
          
-         378         126 LOAD_GLOBAL             10 (db)
+         381         126 LOAD_GLOBAL             10 (db)
                      138 LOAD_ATTR                6 (session)
                      148 LOAD_METHOD              7 (query)
                      170 LOAD_GLOBAL             10 (db)
                      182 LOAD_ATTR                8 (SessionStore)
                      192 PRECALL                  1
                      196 CALL                     1
                      206 LOAD_METHOD              4 (get)
                      228 LOAD_FAST                1 (sessionID)
                      230 PRECALL                  1
                      234 CALL                     1
                      244 STORE_FAST               2 (ss)
          
-         380         246 LOAD_FAST                2 (ss)
+         383         246 LOAD_FAST                2 (ss)
                      248 POP_JUMP_FORWARD_IF_FALSE    61 (to 372)
          
-         381         250 LOAD_GLOBAL             10 (db)
+         384         250 LOAD_GLOBAL             10 (db)
                      262 LOAD_ATTR                6 (session)
                      272 LOAD_METHOD              9 (delete)
                      294 LOAD_FAST                2 (ss)
                      296 PRECALL                  1
                      300 CALL                     1
                      310 POP_TOP
          
-         382         312 LOAD_GLOBAL             10 (db)
+         385         312 LOAD_GLOBAL             10 (db)
                      324 LOAD_ATTR                6 (session)
                      334 LOAD_METHOD             10 (commit)
                      356 PRECALL                  0
                      360 CALL                     0
                      370 POP_TOP
          
-         385     >>  372 LOAD_GLOBAL             22 (page_list)
+         388     >>  372 LOAD_GLOBAL             22 (page_list)
                      384 LOAD_ATTR               11 (page_list)
                      394 GET_ITER
                  >>  396 FOR_ITER                65 (to 528)
                      398 STORE_FAST               3 (page)
          
-         387         400 LOAD_CONST               4 ('path')
+         390         400 LOAD_CONST               4 ('path')
                      402 LOAD_FAST                3 (page)
                      404 CONTAINS_OP              1
                      406 POP_JUMP_FORWARD_IF_FALSE     1 (to 410)
          
-         388         408 JUMP_BACKWARD            7 (to 396)
+         391         408 JUMP_BACKWARD            7 (to 396)
          
-         390     >>  410 LOAD_FAST                3 (page)
+         393     >>  410 LOAD_FAST                3 (page)
                      412 LOAD_CONST               4 ('path')
                      414 BINARY_SUBSCR
                      424 STORE_FAST               4 (path)
          
-         391         426 LOAD_FAST                4 (path)
+         394         426 LOAD_FAST                4 (path)
                      428 LOAD_METHOD             12 (startswith)
                      450 LOAD_CONST               1 ('/')
                      452 PRECALL                  1
                      456 CALL                     1
                      466 POP_JUMP_FORWARD_IF_TRUE     5 (to 478)
          
-         392         468 LOAD_CONST               1 ('/')
+         395         468 LOAD_CONST               1 ('/')
                      470 LOAD_FAST                4 (path)
                      472 BINARY_OP                0 (+)
                      476 STORE_FAST               4 (path)
          
-         394     >>  478 LOAD_FAST                0 (response)
+         397     >>  478 LOAD_FAST                0 (response)
                      480 LOAD_METHOD             13 (set_cookie)
                      502 LOAD_CONST               2 ('session')
                      504 LOAD_CONST               5 (0)
                      506 LOAD_FAST                4 (path)
                      508 KW_NAMES                 6
                      510 PRECALL                  3
                      514 CALL                     3
                      524 POP_TOP
                      526 JUMP_BACKWARD           66 (to 396)
          
-         396     >>  528 LOAD_FAST                0 (response)
+         399     >>  528 LOAD_FAST                0 (response)
                      530 RETURN_VALUE
          consts
             '\n    ``/restart``\n\n    Use this if you ever need to the user to start the experiment over for any reason.\n    This tries to clear out all the cookies.\n    '
             '/'
             'session'
             None
             'path'
@@ -2100,44 +2114,44 @@
             ('expires', 'path')
          names      ('make_response', 'redirect', 'request', 'cookies', 'get', 'db', 'session', 'query', 'SessionStore', 'delete', 'commit', 'page_list', 'startswith', 'set_cookie')
          varnames   ('response', 'sessionID', 'ss', 'page', 'path')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_restart'
-         firstlineno 364
+         firstlineno 367
          lnotab
             0x0209380140020402780204013e013c031c020801020210012a010a0232
             02
       '/submit'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         399           0 RESUME                   0
+         402           0 RESUME                   0
          
-         407           2 LOAD_GLOBAL              1 (NULL + redirect)
+         410           2 LOAD_GLOBAL              1 (NULL + redirect)
                       14 LOAD_CONST               1 ('/redirect_next_page')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             '\n    ``/submit``\n\n    Use this if you simply need to submit a form that redirects to the next page without doing anything with\n    the form data.\n    '
             '/redirect_next_page'
          names      ('redirect',)
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'submit'
-         firstlineno 399
+         firstlineno 402
          lnotab 0x0208
       '/instructions/<pageName>'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
@@ -2147,53 +2161,53 @@
             027400000000000000000000006a040000000000000000a6020000ab0200
             00000000000000a6010000ab0100000000000000005300740a0000000000
             00000000006a0600000000000000007d017c01a007000000000000000000
             000000000000000000000064037c007a060000a6010000ab010000000000
             0000007d027c02a0080000000000000000000000000000000000000000a6
             000000ab0000000000000000007d0374130000000000000000000064047c
             03ac05a6020000ab0200000000000000005300
-         413           0 RESUME                   0
+         416           0 RESUME                   0
          
-         432           2 LOAD_GLOBAL              0 (request)
+         435           2 LOAD_GLOBAL              0 (request)
                       14 LOAD_ATTR                1 (method)
                       24 LOAD_CONST               1 ('POST')
                       26 COMPARE_OP               2 (==)
                       32 POP_JUMP_FORWARD_IF_FALSE    39 (to 112)
          
-         433          34 LOAD_GLOBAL              5 (NULL + redirect)
+         436          34 LOAD_GLOBAL              5 (NULL + redirect)
                       46 LOAD_GLOBAL              7 (NULL + join_urls)
                       58 LOAD_CONST               2 ('/redirect_from_page')
                       60 LOAD_GLOBAL              0 (request)
                       72 LOAD_ATTR                4 (path)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 PRECALL                  1
                      100 CALL                     1
                      110 RETURN_VALUE
          
-         435     >>  112 LOAD_GLOBAL             10 (current_app)
+         438     >>  112 LOAD_GLOBAL             10 (current_app)
                      124 LOAD_ATTR                6 (jinja_env)
                      134 STORE_FAST               1 (jinja)
          
-         436         136 LOAD_FAST                1 (jinja)
+         439         136 LOAD_FAST                1 (jinja)
                      138 LOAD_METHOD              7 (get_or_select_template)
                      160 LOAD_CONST               3 ('instructions/%s.html')
                      162 LOAD_FAST                0 (pageName)
                      164 BINARY_OP                6 (%)
                      168 PRECALL                  1
                      172 CALL                     1
                      182 STORE_FAST               2 (instructionsTemplate)
          
-         437         184 LOAD_FAST                2 (instructionsTemplate)
+         440         184 LOAD_FAST                2 (instructionsTemplate)
                      186 LOAD_METHOD              8 (render)
                      208 PRECALL                  0
                      212 CALL                     0
                      222 STORE_FAST               3 (instructionsHtml)
          
-         439         224 LOAD_GLOBAL             19 (NULL + render_template)
+         442         224 LOAD_GLOBAL             19 (NULL + render_template)
                      236 LOAD_CONST               4 ('instructions.html')
                      238 LOAD_FAST                3 (instructionsHtml)
                      240 KW_NAMES                 5
                      242 PRECALL                  2
                      246 CALL                     2
                      256 RETURN_VALUE
          consts
@@ -2205,15 +2219,15 @@
             ('instructions',)
          names      ('request', 'method', 'redirect', 'join_urls', 'path', 'current_app', 'jinja_env', 'get_or_select_template', 'render', 'render_template')
          varnames   ('pageName', 'jinja', 'instructionsTemplate', 'instructionsHtml')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_instructions'
-         firstlineno 413
+         firstlineno 416
          lnotab 0x021320014e02180130012802
       '/simple/<pageName>'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -2223,50 +2237,50 @@
             027400000000000000000000006a040000000000000000a6020000ab0200
             00000000000000a6010000ab0100000000000000005300740a0000000000
             00000000006a0600000000000000007d017c01a007000000000000000000
             000000000000000000000064037c007a060000a6010000ab010000000000
             000000a0080000000000000000000000000000000000000000a6000000ab
             0000000000000000007d0274130000000000000000000064047c02ac05a6
             020000ab0200000000000000005300
-         442           0 RESUME                   0
+         445           0 RESUME                   0
          
-         464           2 LOAD_GLOBAL              0 (request)
+         467           2 LOAD_GLOBAL              0 (request)
                       14 LOAD_ATTR                1 (method)
                       24 LOAD_CONST               1 ('POST')
                       26 COMPARE_OP               2 (==)
                       32 POP_JUMP_FORWARD_IF_FALSE    39 (to 112)
          
-         465          34 LOAD_GLOBAL              5 (NULL + redirect)
+         468          34 LOAD_GLOBAL              5 (NULL + redirect)
                       46 LOAD_GLOBAL              7 (NULL + join_urls)
                       58 LOAD_CONST               2 ('/redirect_from_page')
                       60 LOAD_GLOBAL              0 (request)
                       72 LOAD_ATTR                4 (path)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 PRECALL                  1
                      100 CALL                     1
                      110 RETURN_VALUE
          
-         467     >>  112 LOAD_GLOBAL             10 (current_app)
+         470     >>  112 LOAD_GLOBAL             10 (current_app)
                      124 LOAD_ATTR                6 (jinja_env)
                      134 STORE_FAST               1 (jinja)
          
-         468         136 LOAD_FAST                1 (jinja)
+         471         136 LOAD_FAST                1 (jinja)
                      138 LOAD_METHOD              7 (get_or_select_template)
                      160 LOAD_CONST               3 ('simple/%s.html')
                      162 LOAD_FAST                0 (pageName)
                      164 BINARY_OP                6 (%)
                      168 PRECALL                  1
                      172 CALL                     1
                      182 LOAD_METHOD              8 (render)
                      204 PRECALL                  0
                      208 CALL                     0
                      218 STORE_FAST               2 (simple_html)
          
-         470         220 LOAD_GLOBAL             19 (NULL + render_template)
+         473         220 LOAD_GLOBAL             19 (NULL + render_template)
                      232 LOAD_CONST               4 ('simple.html')
                      234 LOAD_FAST                2 (simple_html)
                      236 KW_NAMES                 5
                      238 PRECALL                  2
                      242 CALL                     2
                      252 RETURN_VALUE
          consts
@@ -2278,15 +2292,15 @@
             ('simple_contents',)
          names      ('request', 'method', 'redirect', 'join_urls', 'path', 'current_app', 'jinja_env', 'get_or_select_template', 'render', 'render_template')
          varnames   ('pageName', 'jinja', 'simple_html')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_simple_html'
-         firstlineno 442
+         firstlineno 445
          lnotab 0x021620014e0218015402
       None
       ('',)
    names      ('flask', 'Blueprint', 'render_template', 'current_app', 'request', 'make_response', 'urllib.parse', 'urlsplit', 'BOFS.JSONTable', 'JSONTable', 'BOFS.util', 'BOFS.globals', 'db', 'referrer', 'page_list', 'questionnaires', 'tables', 'BOFS.BOFSSession', 'BOFSSessionInterface', 'BOFSSession', '__name__', 'default', 'route', 'verify_correct_page', 'route_index', 'route_consent', 'route_consent_nc', 'route_create_participant', 'route_create_participant_nc', 'verify_session_valid', 'route_assign_condition', 'route_external_id', 'route_table', 'route_questionnaire', 'str', 'route_questionnaire_question', 'route_redirect_previous_page', 'route_redirect_next_page', 'route_redirect_from_page', 'route_redirect_to_page', 'route_end', 'route_user_active', 'route_current_url', 'route_restart', 'submit', 'route_instructions', 'route_simple_html')
    varnames   ()
    freevars   ()
    cellvars   ()
@@ -2294,12 +2308,12 @@
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02011c010c020c0108011c01100318032801020104ff0eff0e0202
       043001020104ff0eff0e0202183001020104ff0eff0e02020d280104ff0e
       01020c280104ff0e01020e28010201020104ff0eff0eff0e030214300130
       013001020104ff0eff0eff0eff0e040247300104ff0e0102113001300102
-      0106ff0eff0eff0e03021b2e010aff0e010211280104ff0e01020c280104
+      0106ff0eff0eff0e03021b2e010aff0e010214280104ff0e01020c280104
       ff0e010217280104ff0e01020e280104ff0e01020e28010201020104ff0e
       ff0eff0e030214280104ff0e010208280104ff0e01020c280104ff0e0102
       222e0104ff0e01020d30010201020104ff0eff0eff0e03021a3001020102
       0104ff0eff0eff0e03
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/default/models.py` & `bride-of-frankensystem-1.9.3.4/BOFS/default/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         mTurkID = db.Column(db.String(50), nullable=False, default="")
         ipAddress = db.Column(db.String(32), nullable=False, default="")
         userAgent = db.Column(db.String(255), nullable=False, default="")
         condition = db.Column(db.Integer, nullable=True, default=0)
         timeStarted = db.Column(db.DateTime, nullable=False, default=datetime.utcnow)  # Starts after consent
         timeEnded = db.Column(db.DateTime, nullable=True)
         finished = db.Column(db.Boolean, nullable=False, default=False)
+        excludeFromCount = db.Column(db.Boolean, nullable=False, default=False)
         code = db.Column(db.String(36), nullable=False, default=0)
         lastActiveOn = db.Column(db.DateTime, nullable=False, default=datetime.utcnow)
 
         def table(self, name):
             from BOFS.globals import tables
 
 
@@ -80,26 +81,28 @@
 
                 printText = "Total conditions: {}, Counts: ".format(numConditions)
 
                 for condition in range(1, numConditions+1):
                     # Count the participants that have not abandoned the study.
                     if current_app.config['COUNTS_INCLUDE_ABANDONED']:
                         pCount[condition - 1] = db.session.query(db.Participant).\
-                            filter(db.Participant.condition == condition).\
+                            filter(db.Participant.condition == condition,
+                                   ~db.Participant.excludeFromCount).\
                             count()
                     else:
                         pCount[condition-1] = db.session.query(db.Participant).\
                             filter(
-                                db.and_(db.Participant.condition == condition, ~db.Participant.is_abandoned)
+                                db.and_(db.Participant.condition == condition,
+                                        ~db.Participant.is_abandoned,
+                                        ~db.Participant.excludeFromCount)
                             ).count()
 
                     printText += "{}, ".format(pCount[condition-1])
 
                 pCountSorted = sorted(pCount)
-                conditionAssigned = False
 
                 for count in pCountSorted:
                     idx = pCount.index(count)
                     conditionMeta = current_app.config['CONDITIONS'][idx]
                     if 'enabled' not in conditionMeta or conditionMeta['enabled'] == True:
                         self.condition = idx + 1
                         break
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/default/views.py` & `bride-of-frankensystem-1.9.3.4/BOFS/default/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,17 @@
 def route_questionnaire_question(questionType: str):
     """
     ``/questionnaire_question/<questionType>``
 
     Render a specific question type for the questionnaire. Only accepts POST requests.
     Data posted to this route must be a JSON object of the question data.
     """
+    if 'participantID' not in session:
+        raise Exception('Error: No participantID in session. Did you forget /consent or /create_participant, etc.?')
+
     participant = db.Participant.query.get(session['participantID'])
 
     try:
         return render_template(f'questions/{questionType}.html',
                                question=request.json,
                                participant=participant)
     except Exception as ex:
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/globals.py` & `bride-of-frankensystem-1.9.3.4/BOFS/globals.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/static/img/check.png` & `bride-of-frankensystem-1.9.3.4/BOFS/static/img/check.png`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/static/img/spinner32.gif` & `bride-of-frankensystem-1.9.3.4/BOFS/static/img/spinner32.gif`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/static/js/jquery-3.4.1.min.js` & `bride-of-frankensystem-1.9.3.4/BOFS/static/js/jquery-3.7.1.min.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,3219 +1,3182 @@
-/*! jQuery v3.4.1 | (c) JS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
-    "use strict";
-    "object" == typeof module && "object" == typeof module.exports ? module.exports = e.document ? t(e, !0) : function(e) {
-        if (!e.document) throw new Error("jQuery requires a window with a document");
-        return t(e)
-    } : t(e)
-}("undefined" != typeof window ? window : this, function(C, e) {
-    "use strict";
-    var t = [],
-        E = C.document,
-        r = Object.getPrototypeOf,
-        s = t.slice,
-        g = t.concat,
-        u = t.push,
-        i = t.indexOf,
-        n = {},
-        o = n.toString,
-        v = n.hasOwnProperty,
-        a = v.toString,
-        l = a.call(Object),
-        y = {},
-        m = function(e) {
-            return "function" == typeof e && "number" != typeof e.nodeType
-        },
-        x = function(e) {
-            return null != e && e === e.window
-        },
-        c = {
-            type: !0,
-            src: !0,
-            nonce: !0,
-            noModule: !0
-        };
-
-    function b(e, t, n) {
-        var r, i, o = (n = n || E).createElement("script");
-        if (o.text = e, t)
-            for (r in c)(i = t[r] || t.getAttribute && t.getAttribute(r)) && o.setAttribute(r, i);
-        n.head.appendChild(o).parentNode.removeChild(o)
-    }
-
-    function w(e) {
-        return null == e ? e + "" : "object" == typeof e || "function" == typeof e ? n[o.call(e)] || "object" : typeof e
-    }
-    var f = "3.4.1",
-        k = function(e, t) {
-            return new k.fn.init(e, t)
-        },
-        p = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
-
-    function d(e) {
-        var t = !!e && "length" in e && e.length,
-            n = w(e);
-        return !m(e) && !x(e) && ("array" === n || 0 === t || "number" == typeof t && 0 < t && t - 1 in e)
-    }
-    k.fn = k.prototype = {
-        jquery: f,
-        constructor: k,
-        length: 0,
-        toArray: function() {
-            return s.call(this)
-        },
-        get: function(e) {
-            return null == e ? s.call(this) : e < 0 ? this[e + this.length] : this[e]
-        },
-        pushStack: function(e) {
-            var t = k.merge(this.constructor(), e);
-            return t.prevObject = this, t
-        },
-        each: function(e) {
-            return k.each(this, e)
-        },
-        map: function(n) {
-            return this.pushStack(k.map(this, function(e, t) {
-                return n.call(e, t, e)
-            }))
-        },
-        slice: function() {
-            return this.pushStack(s.apply(this, arguments))
-        },
-        first: function() {
-            return this.eq(0)
-        },
-        last: function() {
-            return this.eq(-1)
-        },
-        eq: function(e) {
-            var t = this.length,
-                n = +e + (e < 0 ? t : 0);
-            return this.pushStack(0 <= n && n < t ? [this[n]] : [])
-        },
-        end: function() {
-            return this.prevObject || this.constructor()
-        },
-        push: u,
-        sort: t.sort,
-        splice: t.splice
-    }, k.extend = k.fn.extend = function() {
-        var e, t, n, r, i, o, a = arguments[0] || {},
-            s = 1,
-            u = arguments.length,
-            l = !1;
-        for ("boolean" == typeof a && (l = a, a = arguments[s] || {}, s++), "object" == typeof a || m(a) || (a = {}), s === u && (a = this, s--); s < u; s++)
-            if (null != (e = arguments[s]))
-                for (t in e) r = e[t], "__proto__" !== t && a !== r && (l && r && (k.isPlainObject(r) || (i = Array.isArray(r))) ? (n = a[t], o = i && !Array.isArray(n) ? [] : i || k.isPlainObject(n) ? n : {}, i = !1, a[t] = k.extend(l, o, r)) : void 0 !== r && (a[t] = r));
-        return a
-    }, k.extend({
-        expando: "jQuery" + (f + Math.random()).replace(/\D/g, ""),
-        isReady: !0,
-        error: function(e) {
-            throw new Error(e)
-        },
-        noop: function() {},
-        isPlainObject: function(e) {
-            var t, n;
-            return !(!e || "[object Object]" !== o.call(e)) && (!(t = r(e)) || "function" == typeof(n = v.call(t, "constructor") && t.constructor) && a.call(n) === l)
-        },
-        isEmptyObject: function(e) {
-            var t;
-            for (t in e) return !1;
-            return !0
-        },
-        globalEval: function(e, t) {
-            b(e, {
-                nonce: t && t.nonce
-            })
-        },
-        each: function(e, t) {
-            var n, r = 0;
-            if (d(e)) {
-                for (n = e.length; r < n; r++)
-                    if (!1 === t.call(e[r], r, e[r])) break
-            } else
-                for (r in e)
-                    if (!1 === t.call(e[r], r, e[r])) break;
-            return e
-        },
-        trim: function(e) {
-            return null == e ? "" : (e + "").replace(p, "")
-        },
-        makeArray: function(e, t) {
-            var n = t || [];
-            return null != e && (d(Object(e)) ? k.merge(n, "string" == typeof e ? [e] : e) : u.call(n, e)), n
-        },
-        inArray: function(e, t, n) {
-            return null == t ? -1 : i.call(t, e, n)
-        },
-        merge: function(e, t) {
-            for (var n = +t.length, r = 0, i = e.length; r < n; r++) e[i++] = t[r];
-            return e.length = i, e
-        },
-        grep: function(e, t, n) {
-            for (var r = [], i = 0, o = e.length, a = !n; i < o; i++) !t(e[i], i) !== a && r.push(e[i]);
-            return r
-        },
-        map: function(e, t, n) {
-            var r, i, o = 0,
-                a = [];
-            if (d(e))
-                for (r = e.length; o < r; o++) null != (i = t(e[o], o, n)) && a.push(i);
-            else
-                for (o in e) null != (i = t(e[o], o, n)) && a.push(i);
-            return g.apply([], a)
-        },
-        guid: 1,
-        support: y
-    }), "function" == typeof Symbol && (k.fn[Symbol.iterator] = t[Symbol.iterator]), k.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(e, t) {
-        n["[object " + t + "]"] = t.toLowerCase()
-    });
-    var h = function(n) {
-        var e, d, b, o, i, h, f, g, w, u, l, T, C, a, E, v, s, c, y, k = "sizzle" + 1 * new Date,
-            m = n.document,
-            S = 0,
-            r = 0,
-            p = ue(),
-            x = ue(),
-            N = ue(),
-            A = ue(),
-            D = function(e, t) {
-                return e === t && (l = !0), 0
-            },
-            j = {}.hasOwnProperty,
-            t = [],
-            q = t.pop,
-            L = t.push,
-            H = t.push,
-            O = t.slice,
-            P = function(e, t) {
-                for (var n = 0, r = e.length; n < r; n++)
-                    if (e[n] === t) return n;
-                return -1
-            },
-            R = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
-            M = "[\\x20\\t\\r\\n\\f]",
-            I = "(?:\\\\.|[\\w-]|[^\0-\\xa0])+",
-            W = "\\[" + M + "*(" + I + ")(?:" + M + "*([*^$|!~]?=)" + M + "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + I + "))|)" + M + "*\\]",
-            $ = ":(" + I + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + W + ")*)|.*)\\)|)",
-            F = new RegExp(M + "+", "g"),
-            B = new RegExp("^" + M + "+|((?:^|[^\\\\])(?:\\\\.)*)" + M + "+$", "g"),
-            _ = new RegExp("^" + M + "*," + M + "*"),
-            z = new RegExp("^" + M + "*([>+~]|" + M + ")" + M + "*"),
-            U = new RegExp(M + "|>"),
-            X = new RegExp($),
-            V = new RegExp("^" + I + "$"),
-            G = {
-                ID: new RegExp("^#(" + I + ")"),
-                CLASS: new RegExp("^\\.(" + I + ")"),
-                TAG: new RegExp("^(" + I + "|[*])"),
-                ATTR: new RegExp("^" + W),
-                PSEUDO: new RegExp("^" + $),
-                CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + M + "*(even|odd|(([+-]|)(\\d*)n|)" + M + "*(?:([+-]|)" + M + "*(\\d+)|))" + M + "*\\)|)", "i"),
-                bool: new RegExp("^(?:" + R + ")$", "i"),
-                needsContext: new RegExp("^" + M + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + M + "*((?:-\\d)?\\d*)" + M + "*\\)|)(?=[^-]|$)", "i")
-            },
-            Y = /HTML$/i,
-            Q = /^(?:input|select|textarea|button)$/i,
-            J = /^h\d$/i,
-            K = /^[^{]+\{\s*\[native \w/,
-            Z = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
-            ee = /[+~]/,
-            te = new RegExp("\\\\([\\da-f]{1,6}" + M + "?|(" + M + ")|.)", "ig"),
-            ne = function(e, t, n) {
-                var r = "0x" + t - 65536;
-                return r != r || n ? t : r < 0 ? String.fromCharCode(r + 65536) : String.fromCharCode(r >> 10 | 55296, 1023 & r | 56320)
-            },
-            re = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,
-            ie = function(e, t) {
-                return t ? "\0" === e ? "\ufffd" : e.slice(0, -1) + "\\" + e.charCodeAt(e.length - 1).toString(16) + " " : "\\" + e
-            },
-            oe = function() {
-                T()
-            },
-            ae = be(function(e) {
-                return !0 === e.disabled && "fieldset" === e.nodeName.toLowerCase()
-            }, {
-                dir: "parentNode",
-                next: "legend"
-            });
-        try {
-            H.apply(t = O.call(m.childNodes), m.childNodes), t[m.childNodes.length].nodeType
-        } catch (e) {
-            H = {
-                apply: t.length ? function(e, t) {
-                    L.apply(e, O.call(t))
-                } : function(e, t) {
-                    var n = e.length,
-                        r = 0;
-                    while (e[n++] = t[r++]);
-                    e.length = n - 1
-                }
-            }
-        }
-
-        function se(t, e, n, r) {
-            var i, o, a, s, u, l, c, f = e && e.ownerDocument,
-                p = e ? e.nodeType : 9;
-            if (n = n || [], "string" != typeof t || !t || 1 !== p && 9 !== p && 11 !== p) return n;
-            if (!r && ((e ? e.ownerDocument || e : m) !== C && T(e), e = e || C, E)) {
-                if (11 !== p && (u = Z.exec(t)))
-                    if (i = u[1]) {
-                        if (9 === p) {
-                            if (!(a = e.getElementById(i))) return n;
-                            if (a.id === i) return n.push(a), n
-                        } else if (f && (a = f.getElementById(i)) && y(e, a) && a.id === i) return n.push(a), n
-                    } else {
-                        if (u[2]) return H.apply(n, e.getElementsByTagName(t)), n;
-                        if ((i = u[3]) && d.getElementsByClassName && e.getElementsByClassName) return H.apply(n, e.getElementsByClassName(i)), n
-                    } if (d.qsa && !A[t + " "] && (!v || !v.test(t)) && (1 !== p || "object" !== e.nodeName.toLowerCase())) {
-                    if (c = t, f = e, 1 === p && U.test(t)) {
-                        (s = e.getAttribute("id")) ? s = s.replace(re, ie): e.setAttribute("id", s = k), o = (l = h(t)).length;
-                        while (o--) l[o] = "#" + s + " " + xe(l[o]);
-                        c = l.join(","), f = ee.test(t) && ye(e.parentNode) || e
-                    }
-                    try {
-                        return H.apply(n, f.querySelectorAll(c)), n
-                    } catch (e) {
-                        A(t, !0)
-                    } finally {
-                        s === k && e.removeAttribute("id")
-                    }
-                }
-            }
-            return g(t.replace(B, "$1"), e, n, r)
-        }
-
-        function ue() {
-            var r = [];
-            return function e(t, n) {
-                return r.push(t + " ") > b.cacheLength && delete e[r.shift()], e[t + " "] = n
-            }
-        }
-
-        function le(e) {
-            return e[k] = !0, e
-        }
-
-        function ce(e) {
-            var t = C.createElement("fieldset");
-            try {
-                return !!e(t)
-            } catch (e) {
-                return !1
-            } finally {
-                t.parentNode && t.parentNode.removeChild(t), t = null
-            }
-        }
-
-        function fe(e, t) {
-            var n = e.split("|"),
-                r = n.length;
-            while (r--) b.attrHandle[n[r]] = t
-        }
-
-        function pe(e, t) {
-            var n = t && e,
-                r = n && 1 === e.nodeType && 1 === t.nodeType && e.sourceIndex - t.sourceIndex;
-            if (r) return r;
-            if (n)
-                while (n = n.nextSibling)
-                    if (n === t) return -1;
-            return e ? 1 : -1
-        }
-
-        function de(t) {
-            return function(e) {
-                return "input" === e.nodeName.toLowerCase() && e.type === t
-            }
-        }
-
-        function he(n) {
-            return function(e) {
-                var t = e.nodeName.toLowerCase();
-                return ("input" === t || "button" === t) && e.type === n
-            }
-        }
-
-        function ge(t) {
-            return function(e) {
-                return "form" in e ? e.parentNode && !1 === e.disabled ? "label" in e ? "label" in e.parentNode ? e.parentNode.disabled === t : e.disabled === t : e.isDisabled === t || e.isDisabled !== !t && ae(e) === t : e.disabled === t : "label" in e && e.disabled === t
-            }
-        }
-
-        function ve(a) {
-            return le(function(o) {
-                return o = +o, le(function(e, t) {
-                    var n, r = a([], e.length, o),
-                        i = r.length;
-                    while (i--) e[n = r[i]] && (e[n] = !(t[n] = e[n]))
-                })
-            })
-        }
-
-        function ye(e) {
-            return e && "undefined" != typeof e.getElementsByTagName && e
-        }
-        for (e in d = se.support = {}, i = se.isXML = function(e) {
-                var t = e.namespaceURI,
-                    n = (e.ownerDocument || e).documentElement;
-                return !Y.test(t || n && n.nodeName || "HTML")
-            }, T = se.setDocument = function(e) {
-                var t, n, r = e ? e.ownerDocument || e : m;
-                return r !== C && 9 === r.nodeType && r.documentElement && (a = (C = r).documentElement, E = !i(C), m !== C && (n = C.defaultView) && n.top !== n && (n.addEventListener ? n.addEventListener("unload", oe, !1) : n.attachEvent && n.attachEvent("onunload", oe)), d.attributes = ce(function(e) {
-                    return e.className = "i", !e.getAttribute("className")
-                }), d.getElementsByTagName = ce(function(e) {
-                    return e.appendChild(C.createComment("")), !e.getElementsByTagName("*").length
-                }), d.getElementsByClassName = K.test(C.getElementsByClassName), d.getById = ce(function(e) {
-                    return a.appendChild(e).id = k, !C.getElementsByName || !C.getElementsByName(k).length
-                }), d.getById ? (b.filter.ID = function(e) {
-                    var t = e.replace(te, ne);
-                    return function(e) {
-                        return e.getAttribute("id") === t
-                    }
-                }, b.find.ID = function(e, t) {
-                    if ("undefined" != typeof t.getElementById && E) {
-                        var n = t.getElementById(e);
-                        return n ? [n] : []
-                    }
-                }) : (b.filter.ID = function(e) {
-                    var n = e.replace(te, ne);
-                    return function(e) {
-                        var t = "undefined" != typeof e.getAttributeNode && e.getAttributeNode("id");
-                        return t && t.value === n
-                    }
-                }, b.find.ID = function(e, t) {
-                    if ("undefined" != typeof t.getElementById && E) {
-                        var n, r, i, o = t.getElementById(e);
-                        if (o) {
-                            if ((n = o.getAttributeNode("id")) && n.value === e) return [o];
-                            i = t.getElementsByName(e), r = 0;
-                            while (o = i[r++])
-                                if ((n = o.getAttributeNode("id")) && n.value === e) return [o]
-                        }
-                        return []
-                    }
-                }), b.find.TAG = d.getElementsByTagName ? function(e, t) {
-                    return "undefined" != typeof t.getElementsByTagName ? t.getElementsByTagName(e) : d.qsa ? t.querySelectorAll(e) : void 0
-                } : function(e, t) {
-                    var n, r = [],
-                        i = 0,
-                        o = t.getElementsByTagName(e);
-                    if ("*" === e) {
-                        while (n = o[i++]) 1 === n.nodeType && r.push(n);
-                        return r
-                    }
-                    return o
-                }, b.find.CLASS = d.getElementsByClassName && function(e, t) {
-                    if ("undefined" != typeof t.getElementsByClassName && E) return t.getElementsByClassName(e)
-                }, s = [], v = [], (d.qsa = K.test(C.querySelectorAll)) && (ce(function(e) {
-                    a.appendChild(e).innerHTML = "<a id='" + k + "'></a><select id='" + k + "-\r\\' msallowcapture=''><option selected=''></option></select>", e.querySelectorAll("[msallowcapture^='']").length && v.push("[*^$]=" + M + "*(?:''|\"\")"), e.querySelectorAll("[selected]").length || v.push("\\[" + M + "*(?:value|" + R + ")"), e.querySelectorAll("[id~=" + k + "-]").length || v.push("~="), e.querySelectorAll(":checked").length || v.push(":checked"), e.querySelectorAll("a#" + k + "+*").length || v.push(".#.+[+~]")
-                }), ce(function(e) {
-                    e.innerHTML = "<a href='' disabled='disabled'></a><select disabled='disabled'><option/></select>";
-                    var t = C.createElement("input");
-                    t.setAttribute("type", "hidden"), e.appendChild(t).setAttribute("name", "D"), e.querySelectorAll("[name=d]").length && v.push("name" + M + "*[*^$|!~]?="), 2 !== e.querySelectorAll(":enabled").length && v.push(":enabled", ":disabled"), a.appendChild(e).disabled = !0, 2 !== e.querySelectorAll(":disabled").length && v.push(":enabled", ":disabled"), e.querySelectorAll("*,:x"), v.push(",.*:")
-                })), (d.matchesSelector = K.test(c = a.matches || a.webkitMatchesSelector || a.mozMatchesSelector || a.oMatchesSelector || a.msMatchesSelector)) && ce(function(e) {
-                    d.disconnectedMatch = c.call(e, "*"), c.call(e, "[s!='']:x"), s.push("!=", $)
-                }), v = v.length && new RegExp(v.join("|")), s = s.length && new RegExp(s.join("|")), t = K.test(a.compareDocumentPosition), y = t || K.test(a.contains) ? function(e, t) {
-                    var n = 9 === e.nodeType ? e.documentElement : e,
-                        r = t && t.parentNode;
-                    return e === r || !(!r || 1 !== r.nodeType || !(n.contains ? n.contains(r) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(r)))
-                } : function(e, t) {
-                    if (t)
-                        while (t = t.parentNode)
-                            if (t === e) return !0;
-                    return !1
-                }, D = t ? function(e, t) {
-                    if (e === t) return l = !0, 0;
-                    var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
-                    return n || (1 & (n = (e.ownerDocument || e) === (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !d.sortDetached && t.compareDocumentPosition(e) === n ? e === C || e.ownerDocument === m && y(m, e) ? -1 : t === C || t.ownerDocument === m && y(m, t) ? 1 : u ? P(u, e) - P(u, t) : 0 : 4 & n ? -1 : 1)
-                } : function(e, t) {
-                    if (e === t) return l = !0, 0;
-                    var n, r = 0,
-                        i = e.parentNode,
-                        o = t.parentNode,
-                        a = [e],
-                        s = [t];
-                    if (!i || !o) return e === C ? -1 : t === C ? 1 : i ? -1 : o ? 1 : u ? P(u, e) - P(u, t) : 0;
-                    if (i === o) return pe(e, t);
-                    n = e;
-                    while (n = n.parentNode) a.unshift(n);
-                    n = t;
-                    while (n = n.parentNode) s.unshift(n);
-                    while (a[r] === s[r]) r++;
-                    return r ? pe(a[r], s[r]) : a[r] === m ? -1 : s[r] === m ? 1 : 0
-                }), C
-            }, se.matches = function(e, t) {
-                return se(e, null, null, t)
-            }, se.matchesSelector = function(e, t) {
-                if ((e.ownerDocument || e) !== C && T(e), d.matchesSelector && E && !A[t + " "] && (!s || !s.test(t)) && (!v || !v.test(t))) try {
-                    var n = c.call(e, t);
-                    if (n || d.disconnectedMatch || e.document && 11 !== e.document.nodeType) return n
-                } catch (e) {
-                    A(t, !0)
-                }
-                return 0 < se(t, C, null, [e]).length
-            }, se.contains = function(e, t) {
-                return (e.ownerDocument || e) !== C && T(e), y(e, t)
-            }, se.attr = function(e, t) {
-                (e.ownerDocument || e) !== C && T(e);
-                var n = b.attrHandle[t.toLowerCase()],
-                    r = n && j.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
-                return void 0 !== r ? r : d.attributes || !E ? e.getAttribute(t) : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
-            }, se.escape = function(e) {
-                return (e + "").replace(re, ie)
-            }, se.error = function(e) {
-                throw new Error("Syntax error, unrecognized expression: " + e)
-            }, se.uniqueSort = function(e) {
-                var t, n = [],
-                    r = 0,
-                    i = 0;
-                if (l = !d.detectDuplicates, u = !d.sortStable && e.slice(0), e.sort(D), l) {
-                    while (t = e[i++]) t === e[i] && (r = n.push(i));
-                    while (r--) e.splice(n[r], 1)
-                }
-                return u = null, e
-            }, o = se.getText = function(e) {
-                var t, n = "",
-                    r = 0,
-                    i = e.nodeType;
-                if (i) {
-                    if (1 === i || 9 === i || 11 === i) {
-                        if ("string" == typeof e.textContent) return e.textContent;
-                        for (e = e.firstChild; e; e = e.nextSibling) n += o(e)
-                    } else if (3 === i || 4 === i) return e.nodeValue
-                } else
-                    while (t = e[r++]) n += o(t);
-                return n
-            }, (b = se.selectors = {
-                cacheLength: 50,
-                createPseudo: le,
-                match: G,
-                attrHandle: {},
-                find: {},
-                relative: {
-                    ">": {
-                        dir: "parentNode",
-                        first: !0
-                    },
-                    " ": {
-                        dir: "parentNode"
-                    },
-                    "+": {
-                        dir: "previousSibling",
-                        first: !0
-                    },
-                    "~": {
-                        dir: "previousSibling"
-                    }
-                },
-                preFilter: {
-                    ATTR: function(e) {
-                        return e[1] = e[1].replace(te, ne), e[3] = (e[3] || e[4] || e[5] || "").replace(te, ne), "~=" === e[2] && (e[3] = " " + e[3] + " "), e.slice(0, 4)
-                    },
-                    CHILD: function(e) {
-                        return e[1] = e[1].toLowerCase(), "nth" === e[1].slice(0, 3) ? (e[3] || se.error(e[0]), e[4] = +(e[4] ? e[5] + (e[6] || 1) : 2 * ("even" === e[3] || "odd" === e[3])), e[5] = +(e[7] + e[8] || "odd" === e[3])) : e[3] && se.error(e[0]), e
-                    },
-                    PSEUDO: function(e) {
-                        var t, n = !e[6] && e[2];
-                        return G.CHILD.test(e[0]) ? null : (e[3] ? e[2] = e[4] || e[5] || "" : n && X.test(n) && (t = h(n, !0)) && (t = n.indexOf(")", n.length - t) - n.length) && (e[0] = e[0].slice(0, t), e[2] = n.slice(0, t)), e.slice(0, 3))
-                    }
-                },
-                filter: {
-                    TAG: function(e) {
-                        var t = e.replace(te, ne).toLowerCase();
-                        return "*" === e ? function() {
-                            return !0
-                        } : function(e) {
-                            return e.nodeName && e.nodeName.toLowerCase() === t
-                        }
-                    },
-                    CLASS: function(e) {
-                        var t = p[e + " "];
-                        return t || (t = new RegExp("(^|" + M + ")" + e + "(" + M + "|$)")) && p(e, function(e) {
-                            return t.test("string" == typeof e.className && e.className || "undefined" != typeof e.getAttribute && e.getAttribute("class") || "")
-                        })
-                    },
-                    ATTR: function(n, r, i) {
-                        return function(e) {
-                            var t = se.attr(e, n);
-                            return null == t ? "!=" === r : !r || (t += "", "=" === r ? t === i : "!=" === r ? t !== i : "^=" === r ? i && 0 === t.indexOf(i) : "*=" === r ? i && -1 < t.indexOf(i) : "$=" === r ? i && t.slice(-i.length) === i : "~=" === r ? -1 < (" " + t.replace(F, " ") + " ").indexOf(i) : "|=" === r && (t === i || t.slice(0, i.length + 1) === i + "-"))
-                        }
-                    },
-                    CHILD: function(h, e, t, g, v) {
-                        var y = "nth" !== h.slice(0, 3),
-                            m = "last" !== h.slice(-4),
-                            x = "of-type" === e;
-                        return 1 === g && 0 === v ? function(e) {
-                            return !!e.parentNode
-                        } : function(e, t, n) {
-                            var r, i, o, a, s, u, l = y !== m ? "nextSibling" : "previousSibling",
-                                c = e.parentNode,
-                                f = x && e.nodeName.toLowerCase(),
-                                p = !n && !x,
-                                d = !1;
-                            if (c) {
-                                if (y) {
-                                    while (l) {
-                                        a = e;
-                                        while (a = a[l])
-                                            if (x ? a.nodeName.toLowerCase() === f : 1 === a.nodeType) return !1;
-                                        u = l = "only" === h && !u && "nextSibling"
-                                    }
-                                    return !0
-                                }
-                                if (u = [m ? c.firstChild : c.lastChild], m && p) {
-                                    d = (s = (r = (i = (o = (a = c)[k] || (a[k] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] || [])[0] === S && r[1]) && r[2], a = s && c.childNodes[s];
-                                    while (a = ++s && a && a[l] || (d = s = 0) || u.pop())
-                                        if (1 === a.nodeType && ++d && a === e) {
-                                            i[h] = [S, s, d];
-                                            break
-                                        }
-                                } else if (p && (d = s = (r = (i = (o = (a = e)[k] || (a[k] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] || [])[0] === S && r[1]), !1 === d)
-                                    while (a = ++s && a && a[l] || (d = s = 0) || u.pop())
-                                        if ((x ? a.nodeName.toLowerCase() === f : 1 === a.nodeType) && ++d && (p && ((i = (o = a[k] || (a[k] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] = [S, d]), a === e)) break;
-                                return (d -= v) === g || d % g == 0 && 0 <= d / g
-                            }
-                        }
-                    },
-                    PSEUDO: function(e, o) {
-                        var t, a = b.pseudos[e] || b.setFilters[e.toLowerCase()] || se.error("unsupported pseudo: " + e);
-                        return a[k] ? a(o) : 1 < a.length ? (t = [e, e, "", o], b.setFilters.hasOwnProperty(e.toLowerCase()) ? le(function(e, t) {
-                            var n, r = a(e, o),
-                                i = r.length;
-                            while (i--) e[n = P(e, r[i])] = !(t[n] = r[i])
-                        }) : function(e) {
-                            return a(e, 0, t)
-                        }) : a
-                    }
-                },
-                pseudos: {
-                    not: le(function(e) {
-                        var r = [],
-                            i = [],
-                            s = f(e.replace(B, "$1"));
-                        return s[k] ? le(function(e, t, n, r) {
-                            var i, o = s(e, null, r, []),
-                                a = e.length;
-                            while (a--)(i = o[a]) && (e[a] = !(t[a] = i))
-                        }) : function(e, t, n) {
-                            return r[0] = e, s(r, null, n, i), r[0] = null, !i.pop()
-                        }
-                    }),
-                    has: le(function(t) {
-                        return function(e) {
-                            return 0 < se(t, e).length
-                        }
-                    }),
-                    contains: le(function(t) {
-                        return t = t.replace(te, ne),
-                            function(e) {
-                                return -1 < (e.textContent || o(e)).indexOf(t)
-                            }
-                    }),
-                    lang: le(function(n) {
-                        return V.test(n || "") || se.error("unsupported lang: " + n), n = n.replace(te, ne).toLowerCase(),
-                            function(e) {
-                                var t;
-                                do {
-                                    if (t = E ? e.lang : e.getAttribute("xml:lang") || e.getAttribute("lang")) return (t = t.toLowerCase()) === n || 0 === t.indexOf(n + "-")
-                                } while ((e = e.parentNode) && 1 === e.nodeType);
-                                return !1
-                            }
-                    }),
-                    target: function(e) {
-                        var t = n.location && n.location.hash;
-                        return t && t.slice(1) === e.id
-                    },
-                    root: function(e) {
-                        return e === a
-                    },
-                    focus: function(e) {
-                        return e === C.activeElement && (!C.hasFocus || C.hasFocus()) && !!(e.type || e.href || ~e.tabIndex)
-                    },
-                    enabled: ge(!1),
-                    disabled: ge(!0),
-                    checked: function(e) {
-                        var t = e.nodeName.toLowerCase();
-                        return "input" === t && !!e.checked || "option" === t && !!e.selected
-                    },
-                    selected: function(e) {
-                        return e.parentNode && e.parentNode.selectedIndex, !0 === e.selected
-                    },
-                    empty: function(e) {
-                        for (e = e.firstChild; e; e = e.nextSibling)
-                            if (e.nodeType < 6) return !1;
-                        return !0
-                    },
-                    parent: function(e) {
-                        return !b.pseudos.empty(e)
-                    },
-                    header: function(e) {
-                        return J.test(e.nodeName)
-                    },
-                    input: function(e) {
-                        return Q.test(e.nodeName)
-                    },
-                    button: function(e) {
-                        var t = e.nodeName.toLowerCase();
-                        return "input" === t && "button" === e.type || "button" === t
-                    },
-                    text: function(e) {
-                        var t;
-                        return "input" === e.nodeName.toLowerCase() && "text" === e.type && (null == (t = e.getAttribute("type")) || "text" === t.toLowerCase())
-                    },
-                    first: ve(function() {
-                        return [0]
-                    }),
-                    last: ve(function(e, t) {
-                        return [t - 1]
-                    }),
-                    eq: ve(function(e, t, n) {
-                        return [n < 0 ? n + t : n]
-                    }),
-                    even: ve(function(e, t) {
-                        for (var n = 0; n < t; n += 2) e.push(n);
-                        return e
-                    }),
-                    odd: ve(function(e, t) {
-                        for (var n = 1; n < t; n += 2) e.push(n);
-                        return e
-                    }),
-                    lt: ve(function(e, t, n) {
-                        for (var r = n < 0 ? n + t : t < n ? t : n; 0 <= --r;) e.push(r);
-                        return e
-                    }),
-                    gt: ve(function(e, t, n) {
-                        for (var r = n < 0 ? n + t : n; ++r < t;) e.push(r);
-                        return e
-                    })
-                }
-            }).pseudos.nth = b.pseudos.eq, {
-                radio: !0,
-                checkbox: !0,
-                file: !0,
-                password: !0,
-                image: !0
-            }) b.pseudos[e] = de(e);
-        for (e in {
-                submit: !0,
-                reset: !0
-            }) b.pseudos[e] = he(e);
-
-        function me() {}
-
-        function xe(e) {
-            for (var t = 0, n = e.length, r = ""; t < n; t++) r += e[t].value;
-            return r
-        }
-
-        function be(s, e, t) {
-            var u = e.dir,
-                l = e.next,
-                c = l || u,
-                f = t && "parentNode" === c,
-                p = r++;
-            return e.first ? function(e, t, n) {
-                while (e = e[u])
-                    if (1 === e.nodeType || f) return s(e, t, n);
-                return !1
-            } : function(e, t, n) {
-                var r, i, o, a = [S, p];
-                if (n) {
-                    while (e = e[u])
-                        if ((1 === e.nodeType || f) && s(e, t, n)) return !0
-                } else
-                    while (e = e[u])
-                        if (1 === e.nodeType || f)
-                            if (i = (o = e[k] || (e[k] = {}))[e.uniqueID] || (o[e.uniqueID] = {}), l && l === e.nodeName.toLowerCase()) e = e[u] || e;
-                            else {
-                                if ((r = i[c]) && r[0] === S && r[1] === p) return a[2] = r[2];
-                                if ((i[c] = a)[2] = s(e, t, n)) return !0
-                            } return !1
-            }
-        }
-
-        function we(i) {
-            return 1 < i.length ? function(e, t, n) {
-                var r = i.length;
-                while (r--)
-                    if (!i[r](e, t, n)) return !1;
-                return !0
-            } : i[0]
-        }
-
-        function Te(e, t, n, r, i) {
-            for (var o, a = [], s = 0, u = e.length, l = null != t; s < u; s++)(o = e[s]) && (n && !n(o, r, i) || (a.push(o), l && t.push(s)));
-            return a
-        }
-
-        function Ce(d, h, g, v, y, e) {
-            return v && !v[k] && (v = Ce(v)), y && !y[k] && (y = Ce(y, e)), le(function(e, t, n, r) {
-                var i, o, a, s = [],
-                    u = [],
-                    l = t.length,
-                    c = e || function(e, t, n) {
-                        for (var r = 0, i = t.length; r < i; r++) se(e, t[r], n);
-                        return n
-                    }(h || "*", n.nodeType ? [n] : n, []),
-                    f = !d || !e && h ? c : Te(c, s, d, n, r),
-                    p = g ? y || (e ? d : l || v) ? [] : t : f;
-                if (g && g(f, p, n, r), v) {
-                    i = Te(p, u), v(i, [], n, r), o = i.length;
-                    while (o--)(a = i[o]) && (p[u[o]] = !(f[u[o]] = a))
-                }
-                if (e) {
-                    if (y || d) {
-                        if (y) {
-                            i = [], o = p.length;
-                            while (o--)(a = p[o]) && i.push(f[o] = a);
-                            y(null, p = [], i, r)
-                        }
-                        o = p.length;
-                        while (o--)(a = p[o]) && -1 < (i = y ? P(e, a) : s[o]) && (e[i] = !(t[i] = a))
-                    }
-                } else p = Te(p === t ? p.splice(l, p.length) : p), y ? y(null, t, p, r) : H.apply(t, p)
-            })
-        }
-
-        function Ee(e) {
-            for (var i, t, n, r = e.length, o = b.relative[e[0].type], a = o || b.relative[" "], s = o ? 1 : 0, u = be(function(e) {
-                    return e === i
-                }, a, !0), l = be(function(e) {
-                    return -1 < P(i, e)
-                }, a, !0), c = [function(e, t, n) {
-                    var r = !o && (n || t !== w) || ((i = t).nodeType ? u(e, t, n) : l(e, t, n));
-                    return i = null, r
-                }]; s < r; s++)
-                if (t = b.relative[e[s].type]) c = [be(we(c), t)];
-                else {
-                    if ((t = b.filter[e[s].type].apply(null, e[s].matches))[k]) {
-                        for (n = ++s; n < r; n++)
-                            if (b.relative[e[n].type]) break;
-                        return Ce(1 < s && we(c), 1 < s && xe(e.slice(0, s - 1).concat({
-                            value: " " === e[s - 2].type ? "*" : ""
-                        })).replace(B, "$1"), t, s < n && Ee(e.slice(s, n)), n < r && Ee(e = e.slice(n)), n < r && xe(e))
-                    }
-                    c.push(t)
-                } return we(c)
-        }
-        return me.prototype = b.filters = b.pseudos, b.setFilters = new me, h = se.tokenize = function(e, t) {
-            var n, r, i, o, a, s, u, l = x[e + " "];
-            if (l) return t ? 0 : l.slice(0);
-            a = e, s = [], u = b.preFilter;
-            while (a) {
-                for (o in n && !(r = _.exec(a)) || (r && (a = a.slice(r[0].length) || a), s.push(i = [])), n = !1, (r = z.exec(a)) && (n = r.shift(), i.push({
-                        value: n,
-                        type: r[0].replace(B, " ")
-                    }), a = a.slice(n.length)), b.filter) !(r = G[o].exec(a)) || u[o] && !(r = u[o](r)) || (n = r.shift(), i.push({
-                    value: n,
-                    type: o,
-                    matches: r
-                }), a = a.slice(n.length));
-                if (!n) break
-            }
-            return t ? a.length : a ? se.error(e) : x(e, s).slice(0)
-        }, f = se.compile = function(e, t) {
-            var n, v, y, m, x, r, i = [],
-                o = [],
-                a = N[e + " "];
-            if (!a) {
-                t || (t = h(e)), n = t.length;
-                while (n--)(a = Ee(t[n]))[k] ? i.push(a) : o.push(a);
-                (a = N(e, (v = o, m = 0 < (y = i).length, x = 0 < v.length, r = function(e, t, n, r, i) {
-                    var o, a, s, u = 0,
-                        l = "0",
-                        c = e && [],
-                        f = [],
-                        p = w,
-                        d = e || x && b.find.TAG("*", i),
-                        h = S += null == p ? 1 : Math.random() || .1,
-                        g = d.length;
-                    for (i && (w = t === C || t || i); l !== g && null != (o = d[l]); l++) {
-                        if (x && o) {
-                            a = 0, t || o.ownerDocument === C || (T(o), n = !E);
-                            while (s = v[a++])
-                                if (s(o, t || C, n)) {
-                                    r.push(o);
-                                    break
-                                } i && (S = h)
-                        }
-                        m && ((o = !s && o) && u--, e && c.push(o))
-                    }
-                    if (u += l, m && l !== u) {
-                        a = 0;
-                        while (s = y[a++]) s(c, f, t, n);
-                        if (e) {
-                            if (0 < u)
-                                while (l--) c[l] || f[l] || (f[l] = q.call(r));
-                            f = Te(f)
-                        }
-                        H.apply(r, f), i && !e && 0 < f.length && 1 < u + y.length && se.uniqueSort(r)
-                    }
-                    return i && (S = h, w = p), c
-                }, m ? le(r) : r))).selector = e
-            }
-            return a
-        }, g = se.select = function(e, t, n, r) {
-            var i, o, a, s, u, l = "function" == typeof e && e,
-                c = !r && h(e = l.selector || e);
-            if (n = n || [], 1 === c.length) {
-                if (2 < (o = c[0] = c[0].slice(0)).length && "ID" === (a = o[0]).type && 9 === t.nodeType && E && b.relative[o[1].type]) {
-                    if (!(t = (b.find.ID(a.matches[0].replace(te, ne), t) || [])[0])) return n;
-                    l && (t = t.parentNode), e = e.slice(o.shift().value.length)
-                }
-                i = G.needsContext.test(e) ? 0 : o.length;
-                while (i--) {
-                    if (a = o[i], b.relative[s = a.type]) break;
-                    if ((u = b.find[s]) && (r = u(a.matches[0].replace(te, ne), ee.test(o[0].type) && ye(t.parentNode) || t))) {
-                        if (o.splice(i, 1), !(e = r.length && xe(o))) return H.apply(n, r), n;
-                        break
-                    }
-                }
-            }
-            return (l || f(e, c))(r, t, !E, n, !t || ee.test(e) && ye(t.parentNode) || t), n
-        }, d.sortStable = k.split("").sort(D).join("") === k, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
-            return 1 & e.compareDocumentPosition(C.createElement("fieldset"))
-        }), ce(function(e) {
-            return e.innerHTML = "<a href='#'></a>", "#" === e.firstChild.getAttribute("href")
-        }) || fe("type|href|height|width", function(e, t, n) {
-            if (!n) return e.getAttribute(t, "type" === t.toLowerCase() ? 1 : 2)
-        }), d.attributes && ce(function(e) {
-            return e.innerHTML = "<input/>", e.firstChild.setAttribute("value", ""), "" === e.firstChild.getAttribute("value")
-        }) || fe("value", function(e, t, n) {
-            if (!n && "input" === e.nodeName.toLowerCase()) return e.defaultValue
-        }), ce(function(e) {
-            return null == e.getAttribute("disabled")
-        }) || fe(R, function(e, t, n) {
-            var r;
-            if (!n) return !0 === e[t] ? t.toLowerCase() : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
-        }), se
-    }(C);
-    k.find = h, k.expr = h.selectors, k.expr[":"] = k.expr.pseudos, k.uniqueSort = k.unique = h.uniqueSort, k.text = h.getText, k.isXMLDoc = h.isXML, k.contains = h.contains, k.escapeSelector = h.escape;
-    var T = function(e, t, n) {
-            var r = [],
-                i = void 0 !== n;
-            while ((e = e[t]) && 9 !== e.nodeType)
-                if (1 === e.nodeType) {
-                    if (i && k(e).is(n)) break;
-                    r.push(e)
-                } return r
-        },
-        S = function(e, t) {
-            for (var n = []; e; e = e.nextSibling) 1 === e.nodeType && e !== t && n.push(e);
-            return n
-        },
-        N = k.expr.match.needsContext;
-
-    function A(e, t) {
-        return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
-    }
-    var D = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
-
-    function j(e, n, r) {
-        return m(n) ? k.grep(e, function(e, t) {
-            return !!n.call(e, t, e) !== r
-        }) : n.nodeType ? k.grep(e, function(e) {
-            return e === n !== r
-        }) : "string" != typeof n ? k.grep(e, function(e) {
-            return -1 < i.call(n, e) !== r
-        }) : k.filter(n, e, r)
-    }
-    k.filter = function(e, t, n) {
-        var r = t[0];
-        return n && (e = ":not(" + e + ")"), 1 === t.length && 1 === r.nodeType ? k.find.matchesSelector(r, e) ? [r] : [] : k.find.matches(e, k.grep(t, function(e) {
-            return 1 === e.nodeType
-        }))
-    }, k.fn.extend({
-        find: function(e) {
-            var t, n, r = this.length,
-                i = this;
-            if ("string" != typeof e) return this.pushStack(k(e).filter(function() {
-                for (t = 0; t < r; t++)
-                    if (k.contains(i[t], this)) return !0
-            }));
-            for (n = this.pushStack([]), t = 0; t < r; t++) k.find(e, i[t], n);
-            return 1 < r ? k.uniqueSort(n) : n
-        },
-        filter: function(e) {
-            return this.pushStack(j(this, e || [], !1))
-        },
-        not: function(e) {
-            return this.pushStack(j(this, e || [], !0))
-        },
-        is: function(e) {
-            return !!j(this, "string" == typeof e && N.test(e) ? k(e) : e || [], !1).length
-        }
-    });
-    var q, L = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
-    (k.fn.init = function(e, t, n) {
-        var r, i;
-        if (!e) return this;
-        if (n = n || q, "string" == typeof e) {
-            if (!(r = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : L.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
-            if (r[1]) {
-                if (t = t instanceof k ? t[0] : t, k.merge(this, k.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : E, !0)), D.test(r[1]) && k.isPlainObject(t))
-                    for (r in t) m(this[r]) ? this[r](t[r]) : this.attr(r, t[r]);
-                return this
-            }
-            return (i = E.getElementById(r[2])) && (this[0] = i, this.length = 1), this
-        }
-        return e.nodeType ? (this[0] = e, this.length = 1, this) : m(e) ? void 0 !== n.ready ? n.ready(e) : e(k) : k.makeArray(e, this)
-    }).prototype = k.fn, q = k(E);
-    var H = /^(?:parents|prev(?:Until|All))/,
-        O = {
-            children: !0,
-            contents: !0,
-            next: !0,
-            prev: !0
-        };
-
-    function P(e, t) {
-        while ((e = e[t]) && 1 !== e.nodeType);
-        return e
-    }
-    k.fn.extend({
-        has: function(e) {
-            var t = k(e, this),
-                n = t.length;
-            return this.filter(function() {
-                for (var e = 0; e < n; e++)
-                    if (k.contains(this, t[e])) return !0
-            })
-        },
-        closest: function(e, t) {
-            var n, r = 0,
-                i = this.length,
-                o = [],
-                a = "string" != typeof e && k(e);
-            if (!N.test(e))
-                for (; r < i; r++)
-                    for (n = this[r]; n && n !== t; n = n.parentNode)
-                        if (n.nodeType < 11 && (a ? -1 < a.index(n) : 1 === n.nodeType && k.find.matchesSelector(n, e))) {
-                            o.push(n);
-                            break
-                        } return this.pushStack(1 < o.length ? k.uniqueSort(o) : o)
-        },
-        index: function(e) {
-            return e ? "string" == typeof e ? i.call(k(e), this[0]) : i.call(this, e.jquery ? e[0] : e) : this[0] && this[0].parentNode ? this.first().prevAll().length : -1
-        },
-        add: function(e, t) {
-            return this.pushStack(k.uniqueSort(k.merge(this.get(), k(e, t))))
-        },
-        addBack: function(e) {
-            return this.add(null == e ? this.prevObject : this.prevObject.filter(e))
-        }
-    }), k.each({
-        parent: function(e) {
-            var t = e.parentNode;
-            return t && 11 !== t.nodeType ? t : null
-        },
-        parents: function(e) {
-            return T(e, "parentNode")
-        },
-        parentsUntil: function(e, t, n) {
-            return T(e, "parentNode", n)
-        },
-        next: function(e) {
-            return P(e, "nextSibling")
-        },
-        prev: function(e) {
-            return P(e, "previousSibling")
-        },
-        nextAll: function(e) {
-            return T(e, "nextSibling")
-        },
-        prevAll: function(e) {
-            return T(e, "previousSibling")
-        },
-        nextUntil: function(e, t, n) {
-            return T(e, "nextSibling", n)
-        },
-        prevUntil: function(e, t, n) {
-            return T(e, "previousSibling", n)
-        },
-        siblings: function(e) {
-            return S((e.parentNode || {}).firstChild, e)
-        },
-        children: function(e) {
-            return S(e.firstChild)
-        },
-        contents: function(e) {
-            return "undefined" != typeof e.contentDocument ? e.contentDocument : (A(e, "template") && (e = e.content || e), k.merge([], e.childNodes))
-        }
-    }, function(r, i) {
-        k.fn[r] = function(e, t) {
-            var n = k.map(this, i, e);
-            return "Until" !== r.slice(-5) && (t = e), t && "string" == typeof t && (n = k.filter(t, n)), 1 < this.length && (O[r] || k.uniqueSort(n), H.test(r) && n.reverse()), this.pushStack(n)
-        }
-    });
-    var R = /[^\x20\t\r\n\f]+/g;
-
-    function M(e) {
-        return e
-    }
-
-    function I(e) {
-        throw e
-    }
-
-    function W(e, t, n, r) {
-        var i;
-        try {
-            e && m(i = e.promise) ? i.call(e).done(t).fail(n) : e && m(i = e.then) ? i.call(e, t, n) : t.apply(void 0, [e].slice(r))
-        } catch (e) {
-            n.apply(void 0, [e])
-        }
-    }
-    k.Callbacks = function(r) {
-        var e, n;
-        r = "string" == typeof r ? (e = r, n = {}, k.each(e.match(R) || [], function(e, t) {
-            n[t] = !0
-        }), n) : k.extend({}, r);
-        var i, t, o, a, s = [],
-            u = [],
-            l = -1,
-            c = function() {
-                for (a = a || r.once, o = i = !0; u.length; l = -1) {
-                    t = u.shift();
-                    while (++l < s.length) !1 === s[l].apply(t[0], t[1]) && r.stopOnFalse && (l = s.length, t = !1)
-                }
-                r.memory || (t = !1), i = !1, a && (s = t ? [] : "")
-            },
-            f = {
-                add: function() {
-                    return s && (t && !i && (l = s.length - 1, u.push(t)), function n(e) {
-                        k.each(e, function(e, t) {
-                            m(t) ? r.unique && f.has(t) || s.push(t) : t && t.length && "string" !== w(t) && n(t)
-                        })
-                    }(arguments), t && !i && c()), this
-                },
-                remove: function() {
-                    return k.each(arguments, function(e, t) {
-                        var n;
-                        while (-1 < (n = k.inArray(t, s, n))) s.splice(n, 1), n <= l && l--
-                    }), this
-                },
-                has: function(e) {
-                    return e ? -1 < k.inArray(e, s) : 0 < s.length
-                },
-                empty: function() {
-                    return s && (s = []), this
-                },
-                disable: function() {
-                    return a = u = [], s = t = "", this
-                },
-                disabled: function() {
-                    return !s
-                },
-                lock: function() {
-                    return a = u = [], t || i || (s = t = ""), this
-                },
-                locked: function() {
-                    return !!a
-                },
-                fireWith: function(e, t) {
-                    return a || (t = [e, (t = t || []).slice ? t.slice() : t], u.push(t), i || c()), this
-                },
-                fire: function() {
-                    return f.fireWith(this, arguments), this
-                },
-                fired: function() {
-                    return !!o
-                }
-            };
-        return f
-    }, k.extend({
-        Deferred: function(e) {
-            var o = [
-                    ["notify", "progress", k.Callbacks("memory"), k.Callbacks("memory"), 2],
-                    ["resolve", "done", k.Callbacks("once memory"), k.Callbacks("once memory"), 0, "resolved"],
-                    ["reject", "fail", k.Callbacks("once memory"), k.Callbacks("once memory"), 1, "rejected"]
-                ],
-                i = "pending",
-                a = {
-                    state: function() {
-                        return i
-                    },
-                    always: function() {
-                        return s.done(arguments).fail(arguments), this
-                    },
-                    "catch": function(e) {
-                        return a.then(null, e)
-                    },
-                    pipe: function() {
-                        var i = arguments;
-                        return k.Deferred(function(r) {
-                            k.each(o, function(e, t) {
-                                var n = m(i[t[4]]) && i[t[4]];
-                                s[t[1]](function() {
-                                    var e = n && n.apply(this, arguments);
-                                    e && m(e.promise) ? e.promise().progress(r.notify).done(r.resolve).fail(r.reject) : r[t[0] + "With"](this, n ? [e] : arguments)
-                                })
-                            }), i = null
-                        }).promise()
-                    },
-                    then: function(t, n, r) {
-                        var u = 0;
-
-                        function l(i, o, a, s) {
-                            return function() {
-                                var n = this,
-                                    r = arguments,
-                                    e = function() {
-                                        var e, t;
-                                        if (!(i < u)) {
-                                            if ((e = a.apply(n, r)) === o.promise()) throw new TypeError("Thenable self-resolution");
-                                            t = e && ("object" == typeof e || "function" == typeof e) && e.then, m(t) ? s ? t.call(e, l(u, o, M, s), l(u, o, I, s)) : (u++, t.call(e, l(u, o, M, s), l(u, o, I, s), l(u, o, M, o.notifyWith))) : (a !== M && (n = void 0, r = [e]), (s || o.resolveWith)(n, r))
-                                        }
-                                    },
-                                    t = s ? e : function() {
-                                        try {
-                                            e()
-                                        } catch (e) {
-                                            k.Deferred.exceptionHook && k.Deferred.exceptionHook(e, t.stackTrace), u <= i + 1 && (a !== I && (n = void 0, r = [e]), o.rejectWith(n, r))
-                                        }
-                                    };
-                                i ? t() : (k.Deferred.getStackHook && (t.stackTrace = k.Deferred.getStackHook()), C.setTimeout(t))
-                            }
-                        }
-                        return k.Deferred(function(e) {
-                            o[0][3].add(l(0, e, m(r) ? r : M, e.notifyWith)), o[1][3].add(l(0, e, m(t) ? t : M)), o[2][3].add(l(0, e, m(n) ? n : I))
-                        }).promise()
-                    },
-                    promise: function(e) {
-                        return null != e ? k.extend(e, a) : a
-                    }
-                },
-                s = {};
-            return k.each(o, function(e, t) {
-                var n = t[2],
-                    r = t[5];
-                a[t[1]] = n.add, r && n.add(function() {
-                    i = r
-                }, o[3 - e][2].disable, o[3 - e][3].disable, o[0][2].lock, o[0][3].lock), n.add(t[3].fire), s[t[0]] = function() {
-                    return s[t[0] + "With"](this === s ? void 0 : this, arguments), this
-                }, s[t[0] + "With"] = n.fireWith
-            }), a.promise(s), e && e.call(s, s), s
-        },
-        when: function(e) {
-            var n = arguments.length,
-                t = n,
-                r = Array(t),
-                i = s.call(arguments),
-                o = k.Deferred(),
-                a = function(t) {
-                    return function(e) {
-                        r[t] = this, i[t] = 1 < arguments.length ? s.call(arguments) : e, --n || o.resolveWith(r, i)
-                    }
-                };
-            if (n <= 1 && (W(e, o.done(a(t)).resolve, o.reject, !n), "pending" === o.state() || m(i[t] && i[t].then))) return o.then();
-            while (t--) W(i[t], a(t), o.reject);
-            return o.promise()
-        }
-    });
-    var $ = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
-    k.Deferred.exceptionHook = function(e, t) {
-        C.console && C.console.warn && e && $.test(e.name) && C.console.warn("jQuery.Deferred exception: " + e.message, e.stack, t)
-    }, k.readyException = function(e) {
-        C.setTimeout(function() {
-            throw e
-        })
-    };
-    var F = k.Deferred();
-
-    function B() {
-        E.removeEventListener("DOMContentLoaded", B), C.removeEventListener("load", B), k.ready()
-    }
-    k.fn.ready = function(e) {
-        return F.then(e)["catch"](function(e) {
-            k.readyException(e)
-        }), this
-    }, k.extend({
-        isReady: !1,
-        readyWait: 1,
-        ready: function(e) {
-            (!0 === e ? --k.readyWait : k.isReady) || (k.isReady = !0) !== e && 0 < --k.readyWait || F.resolveWith(E, [k])
-        }
-    }), k.ready.then = F.then, "complete" === E.readyState || "loading" !== E.readyState && !E.documentElement.doScroll ? C.setTimeout(k.ready) : (E.addEventListener("DOMContentLoaded", B), C.addEventListener("load", B));
-    var _ = function(e, t, n, r, i, o, a) {
-            var s = 0,
-                u = e.length,
-                l = null == n;
-            if ("object" === w(n))
-                for (s in i = !0, n) _(e, t, s, n[s], !0, o, a);
-            else if (void 0 !== r && (i = !0, m(r) || (a = !0), l && (a ? (t.call(e, r), t = null) : (l = t, t = function(e, t, n) {
-                    return l.call(k(e), n)
-                })), t))
-                for (; s < u; s++) t(e[s], n, a ? r : r.call(e[s], s, t(e[s], n)));
-            return i ? e : l ? t.call(e) : u ? t(e[0], n) : o
-        },
-        z = /^-ms-/,
-        U = /-([a-z])/g;
-
-    function X(e, t) {
-        return t.toUpperCase()
-    }
-
-    function V(e) {
-        return e.replace(z, "ms-").replace(U, X)
-    }
-    var G = function(e) {
-        return 1 === e.nodeType || 9 === e.nodeType || !+e.nodeType
-    };
-
-    function Y() {
-        this.expando = k.expando + Y.uid++
-    }
-    Y.uid = 1, Y.prototype = {
-        cache: function(e) {
-            var t = e[this.expando];
-            return t || (t = {}, G(e) && (e.nodeType ? e[this.expando] = t : Object.defineProperty(e, this.expando, {
-                value: t,
-                configurable: !0
-            }))), t
-        },
-        set: function(e, t, n) {
-            var r, i = this.cache(e);
-            if ("string" == typeof t) i[V(t)] = n;
-            else
-                for (r in t) i[V(r)] = t[r];
-            return i
-        },
-        get: function(e, t) {
-            return void 0 === t ? this.cache(e) : e[this.expando] && e[this.expando][V(t)]
-        },
-        access: function(e, t, n) {
-            return void 0 === t || t && "string" == typeof t && void 0 === n ? this.get(e, t) : (this.set(e, t, n), void 0 !== n ? n : t)
-        },
-        remove: function(e, t) {
-            var n, r = e[this.expando];
-            if (void 0 !== r) {
-                if (void 0 !== t) {
-                    n = (t = Array.isArray(t) ? t.map(V) : (t = V(t)) in r ? [t] : t.match(R) || []).length;
-                    while (n--) delete r[t[n]]
-                }(void 0 === t || k.isEmptyObject(r)) && (e.nodeType ? e[this.expando] = void 0 : delete e[this.expando])
-            }
-        },
-        hasData: function(e) {
-            var t = e[this.expando];
-            return void 0 !== t && !k.isEmptyObject(t)
-        }
-    };
-    var Q = new Y,
-        J = new Y,
-        K = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
-        Z = /[A-Z]/g;
-
-    function ee(e, t, n) {
-        var r, i;
-        if (void 0 === n && 1 === e.nodeType)
-            if (r = "data-" + t.replace(Z, "-$&").toLowerCase(), "string" == typeof(n = e.getAttribute(r))) {
-                try {
-                    n = "true" === (i = n) || "false" !== i && ("null" === i ? null : i === +i + "" ? +i : K.test(i) ? JSON.parse(i) : i)
-                } catch (e) {}
-                J.set(e, t, n)
-            } else n = void 0;
-        return n
-    }
-    k.extend({
-        hasData: function(e) {
-            return J.hasData(e) || Q.hasData(e)
-        },
-        data: function(e, t, n) {
-            return J.access(e, t, n)
-        },
-        removeData: function(e, t) {
-            J.remove(e, t)
-        },
-        _data: function(e, t, n) {
-            return Q.access(e, t, n)
-        },
-        _removeData: function(e, t) {
-            Q.remove(e, t)
-        }
-    }), k.fn.extend({
-        data: function(n, e) {
-            var t, r, i, o = this[0],
-                a = o && o.attributes;
-            if (void 0 === n) {
-                if (this.length && (i = J.get(o), 1 === o.nodeType && !Q.get(o, "hasDataAttrs"))) {
-                    t = a.length;
-                    while (t--) a[t] && 0 === (r = a[t].name).indexOf("data-") && (r = V(r.slice(5)), ee(o, r, i[r]));
-                    Q.set(o, "hasDataAttrs", !0)
-                }
-                return i
-            }
-            return "object" == typeof n ? this.each(function() {
-                J.set(this, n)
-            }) : _(this, function(e) {
-                var t;
-                if (o && void 0 === e) return void 0 !== (t = J.get(o, n)) ? t : void 0 !== (t = ee(o, n)) ? t : void 0;
-                this.each(function() {
-                    J.set(this, n, e)
-                })
-            }, null, e, 1 < arguments.length, null, !0)
-        },
-        removeData: function(e) {
-            return this.each(function() {
-                J.remove(this, e)
-            })
-        }
-    }), k.extend({
-        queue: function(e, t, n) {
-            var r;
-            if (e) return t = (t || "fx") + "queue", r = Q.get(e, t), n && (!r || Array.isArray(n) ? r = Q.access(e, t, k.makeArray(n)) : r.push(n)), r || []
-        },
-        dequeue: function(e, t) {
-            t = t || "fx";
-            var n = k.queue(e, t),
-                r = n.length,
-                i = n.shift(),
-                o = k._queueHooks(e, t);
-            "inprogress" === i && (i = n.shift(), r--), i && ("fx" === t && n.unshift("inprogress"), delete o.stop, i.call(e, function() {
-                k.dequeue(e, t)
-            }, o)), !r && o && o.empty.fire()
-        },
-        _queueHooks: function(e, t) {
-            var n = t + "queueHooks";
-            return Q.get(e, n) || Q.access(e, n, {
-                empty: k.Callbacks("once memory").add(function() {
-                    Q.remove(e, [t + "queue", n])
-                })
-            })
-        }
-    }), k.fn.extend({
-        queue: function(t, n) {
-            var e = 2;
-            return "string" != typeof t && (n = t, t = "fx", e--), arguments.length < e ? k.queue(this[0], t) : void 0 === n ? this : this.each(function() {
-                var e = k.queue(this, t, n);
-                k._queueHooks(this, t), "fx" === t && "inprogress" !== e[0] && k.dequeue(this, t)
-            })
-        },
-        dequeue: function(e) {
-            return this.each(function() {
-                k.dequeue(this, e)
-            })
-        },
-        clearQueue: function(e) {
-            return this.queue(e || "fx", [])
-        },
-        promise: function(e, t) {
-            var n, r = 1,
-                i = k.Deferred(),
-                o = this,
-                a = this.length,
-                s = function() {
-                    --r || i.resolveWith(o, [o])
-                };
-            "string" != typeof e && (t = e, e = void 0), e = e || "fx";
-            while (a--)(n = Q.get(o[a], e + "queueHooks")) && n.empty && (r++, n.empty.add(s));
-            return s(), i.promise(t)
-        }
-    });
-    var te = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
-        ne = new RegExp("^(?:([+-])=|)(" + te + ")([a-z%]*)$", "i"),
-        re = ["Top", "Right", "Bottom", "Left"],
-        ie = E.documentElement,
-        oe = function(e) {
-            return k.contains(e.ownerDocument, e)
-        },
-        ae = {
-            composed: !0
-        };
-    ie.getRootNode && (oe = function(e) {
-        return k.contains(e.ownerDocument, e) || e.getRootNode(ae) === e.ownerDocument
-    });
-    var se = function(e, t) {
-            return "none" === (e = t || e).style.display || "" === e.style.display && oe(e) && "none" === k.css(e, "display")
-        },
-        ue = function(e, t, n, r) {
-            var i, o, a = {};
-            for (o in t) a[o] = e.style[o], e.style[o] = t[o];
-            for (o in i = n.apply(e, r || []), t) e.style[o] = a[o];
-            return i
-        };
-
-    function le(e, t, n, r) {
-        var i, o, a = 20,
-            s = r ? function() {
-                return r.cur()
-            } : function() {
-                return k.css(e, t, "")
-            },
-            u = s(),
-            l = n && n[3] || (k.cssNumber[t] ? "" : "px"),
-            c = e.nodeType && (k.cssNumber[t] || "px" !== l && +u) && ne.exec(k.css(e, t));
-        if (c && c[3] !== l) {
-            u /= 2, l = l || c[3], c = +u || 1;
-            while (a--) k.style(e, t, c + l), (1 - o) * (1 - (o = s() / u || .5)) <= 0 && (a = 0), c /= o;
-            c *= 2, k.style(e, t, c + l), n = n || []
-        }
-        return n && (c = +c || +u || 0, i = n[1] ? c + (n[1] + 1) * n[2] : +n[2], r && (r.unit = l, r.start = c, r.end = i)), i
-    }
-    var ce = {};
-
-    function fe(e, t) {
-        for (var n, r, i, o, a, s, u, l = [], c = 0, f = e.length; c < f; c++)(r = e[c]).style && (n = r.style.display, t ? ("none" === n && (l[c] = Q.get(r, "display") || null, l[c] || (r.style.display = "")), "" === r.style.display && se(r) && (l[c] = (u = a = o = void 0, a = (i = r).ownerDocument, s = i.nodeName, (u = ce[s]) || (o = a.body.appendChild(a.createElement(s)), u = k.css(o, "display"), o.parentNode.removeChild(o), "none" === u && (u = "block"), ce[s] = u)))) : "none" !== n && (l[c] = "none", Q.set(r, "display", n)));
-        for (c = 0; c < f; c++) null != l[c] && (e[c].style.display = l[c]);
-        return e
-    }
-    k.fn.extend({
-        show: function() {
-            return fe(this, !0)
-        },
-        hide: function() {
-            return fe(this)
-        },
-        toggle: function(e) {
-            return "boolean" == typeof e ? e ? this.show() : this.hide() : this.each(function() {
-                se(this) ? k(this).show() : k(this).hide()
-            })
-        }
-    });
-    var pe = /^(?:checkbox|radio)$/i,
-        de = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
-        he = /^$|^module$|\/(?:java|ecma)script/i,
-        ge = {
-            option: [1, "<select multiple='multiple'>", "</select>"],
-            thead: [1, "<table>", "</table>"],
-            col: [2, "<table><colgroup>", "</colgroup></table>"],
-            tr: [2, "<table><tbody>", "</tbody></table>"],
-            td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
-            _default: [0, "", ""]
-        };
-
-    function ve(e, t) {
-        var n;
-        return n = "undefined" != typeof e.getElementsByTagName ? e.getElementsByTagName(t || "*") : "undefined" != typeof e.querySelectorAll ? e.querySelectorAll(t || "*") : [], void 0 === t || t && A(e, t) ? k.merge([e], n) : n
-    }
-
-    function ye(e, t) {
-        for (var n = 0, r = e.length; n < r; n++) Q.set(e[n], "globalEval", !t || Q.get(t[n], "globalEval"))
-    }
-    ge.optgroup = ge.option, ge.tbody = ge.tfoot = ge.colgroup = ge.caption = ge.thead, ge.th = ge.td;
-    var me, xe, be = /<|&#?\w+;/;
-
-    function we(e, t, n, r, i) {
-        for (var o, a, s, u, l, c, f = t.createDocumentFragment(), p = [], d = 0, h = e.length; d < h; d++)
-            if ((o = e[d]) || 0 === o)
-                if ("object" === w(o)) k.merge(p, o.nodeType ? [o] : o);
-                else if (be.test(o)) {
-            a = a || f.appendChild(t.createElement("div")), s = (de.exec(o) || ["", ""])[1].toLowerCase(), u = ge[s] || ge._default, a.innerHTML = u[1] + k.htmlPrefilter(o) + u[2], c = u[0];
-            while (c--) a = a.lastChild;
-            k.merge(p, a.childNodes), (a = f.firstChild).textContent = ""
-        } else p.push(t.createTextNode(o));
-        f.textContent = "", d = 0;
-        while (o = p[d++])
-            if (r && -1 < k.inArray(o, r)) i && i.push(o);
-            else if (l = oe(o), a = ve(f.appendChild(o), "script"), l && ye(a), n) {
-            c = 0;
-            while (o = a[c++]) he.test(o.type || "") && n.push(o)
-        }
-        return f
-    }
-    me = E.createDocumentFragment().appendChild(E.createElement("div")), (xe = E.createElement("input")).setAttribute("type", "radio"), xe.setAttribute("checked", "checked"), xe.setAttribute("name", "t"), me.appendChild(xe), y.checkClone = me.cloneNode(!0).cloneNode(!0).lastChild.checked, me.innerHTML = "<textarea>x</textarea>", y.noCloneChecked = !!me.cloneNode(!0).lastChild.defaultValue;
-    var Te = /^key/,
-        Ce = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
-        Ee = /^([^.]*)(?:\.(.+)|)/;
-
-    function ke() {
-        return !0
-    }
-
-    function Se() {
-        return !1
-    }
-
-    function Ne(e, t) {
-        return e === function() {
-            try {
-                return E.activeElement
-            } catch (e) {}
-        }() == ("focus" === t)
-    }
-
-    function Ae(e, t, n, r, i, o) {
-        var a, s;
-        if ("object" == typeof t) {
-            for (s in "string" != typeof n && (r = r || n, n = void 0), t) Ae(e, s, n, r, t[s], o);
-            return e
-        }
-        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Se;
-        else if (!i) return e;
-        return 1 === o && (a = i, (i = function(e) {
-            return k().off(e), a.apply(this, arguments)
-        }).guid = a.guid || (a.guid = k.guid++)), e.each(function() {
-            k.event.add(this, t, i, r, n)
-        })
-    }
-
-    function De(e, i, o) {
-        o ? (Q.set(e, i, !1), k.event.add(e, i, {
-            namespace: !1,
-            handler: function(e) {
-                var t, n, r = Q.get(this, i);
-                if (1 & e.isTrigger && this[i]) {
-                    if (r.length)(k.event.special[i] || {}).delegateType && e.stopPropagation();
-                    else if (r = s.call(arguments), Q.set(this, i, r), t = o(this, i), this[i](), r !== (n = Q.get(this, i)) || t ? Q.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n.value
-                } else r.length && (Q.set(this, i, {
-                    value: k.event.trigger(k.extend(r[0], k.Event.prototype), r.slice(1), this)
-                }), e.stopImmediatePropagation())
-            }
-        })) : void 0 === Q.get(e, i) && k.event.add(e, i, ke)
-    }
-    k.event = {
-        global: {},
-        add: function(t, e, n, r, i) {
-            var o, a, s, u, l, c, f, p, d, h, g, v = Q.get(t);
-            if (v) {
-                n.handler && (n = (o = n).handler, i = o.selector), i && k.find.matchesSelector(ie, i), n.guid || (n.guid = k.guid++), (u = v.events) || (u = v.events = {}), (a = v.handle) || (a = v.handle = function(e) {
-                    return "undefined" != typeof k && k.event.triggered !== e.type ? k.event.dispatch.apply(t, arguments) : void 0
-                }), l = (e = (e || "").match(R) || [""]).length;
-                while (l--) d = g = (s = Ee.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = k.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = k.event.special[d] || {}, c = k.extend({
-                    type: d,
-                    origType: g,
-                    data: r,
-                    handler: n,
-                    guid: n.guid,
-                    selector: i,
-                    needsContext: i && k.expr.match.needsContext.test(i),
-                    namespace: h.join(".")
-                }, o), (p = u[d]) || ((p = u[d] = []).delegateCount = 0, f.setup && !1 !== f.setup.call(t, r, h, a) || t.addEventListener && t.addEventListener(d, a)), f.add && (f.add.call(t, c), c.handler.guid || (c.handler.guid = n.guid)), i ? p.splice(p.delegateCount++, 0, c) : p.push(c), k.event.global[d] = !0)
-            }
-        },
-        remove: function(e, t, n, r, i) {
-            var o, a, s, u, l, c, f, p, d, h, g, v = Q.hasData(e) && Q.get(e);
-            if (v && (u = v.events)) {
-                l = (t = (t || "").match(R) || [""]).length;
-                while (l--)
-                    if (d = g = (s = Ee.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
-                        f = k.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length;
-                        while (o--) c = p[o], !i && g !== c.origType || n && n.guid !== c.guid || s && !s.test(c.namespace) || r && r !== c.selector && ("**" !== r || !c.selector) || (p.splice(o, 1), c.selector && p.delegateCount--, f.remove && f.remove.call(e, c));
-                        a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, v.handle) || k.removeEvent(e, d, v.handle), delete u[d])
-                    } else
-                        for (d in u) k.event.remove(e, d + t[l], n, r, !0);
-                k.isEmptyObject(u) && Q.remove(e, "handle events")
-            }
-        },
-        dispatch: function(e) {
-            var t, n, r, i, o, a, s = k.event.fix(e),
-                u = new Array(arguments.length),
-                l = (Q.get(this, "events") || {})[s.type] || [],
-                c = k.event.special[s.type] || {};
-            for (u[0] = s, t = 1; t < arguments.length; t++) u[t] = arguments[t];
-            if (s.delegateTarget = this, !c.preDispatch || !1 !== c.preDispatch.call(this, s)) {
-                a = k.event.handlers.call(this, s, l), t = 0;
-                while ((i = a[t++]) && !s.isPropagationStopped()) {
-                    s.currentTarget = i.elem, n = 0;
-                    while ((o = i.handlers[n++]) && !s.isImmediatePropagationStopped()) s.rnamespace && !1 !== o.namespace && !s.rnamespace.test(o.namespace) || (s.handleObj = o, s.data = o.data, void 0 !== (r = ((k.event.special[o.origType] || {}).handle || o.handler).apply(i.elem, u)) && !1 === (s.result = r) && (s.preventDefault(), s.stopPropagation()))
-                }
-                return c.postDispatch && c.postDispatch.call(this, s), s.result
-            }
-        },
-        handlers: function(e, t) {
-            var n, r, i, o, a, s = [],
-                u = t.delegateCount,
-                l = e.target;
-            if (u && l.nodeType && !("click" === e.type && 1 <= e.button))
-                for (; l !== this; l = l.parentNode || this)
-                    if (1 === l.nodeType && ("click" !== e.type || !0 !== l.disabled)) {
-                        for (o = [], a = {}, n = 0; n < u; n++) void 0 === a[i = (r = t[n]).selector + " "] && (a[i] = r.needsContext ? -1 < k(i, this).index(l) : k.find(i, this, null, [l]).length), a[i] && o.push(r);
-                        o.length && s.push({
-                            elem: l,
-                            handlers: o
-                        })
-                    } return l = this, u < t.length && s.push({
-                elem: l,
-                handlers: t.slice(u)
-            }), s
-        },
-        addProp: function(t, e) {
-            Object.defineProperty(k.Event.prototype, t, {
-                enumerable: !0,
-                configurable: !0,
-                get: m(e) ? function() {
-                    if (this.originalEvent) return e(this.originalEvent)
-                } : function() {
-                    if (this.originalEvent) return this.originalEvent[t]
-                },
-                set: function(e) {
-                    Object.defineProperty(this, t, {
-                        enumerable: !0,
-                        configurable: !0,
-                        writable: !0,
-                        value: e
-                    })
-                }
-            })
-        },
-        fix: function(e) {
-            return e[k.expando] ? e : new k.Event(e)
-        },
-        special: {
-            load: {
-                noBubble: !0
-            },
-            click: {
-                setup: function(e) {
-                    var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && De(t, "click", ke), !1
-                },
-                trigger: function(e) {
-                    var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && De(t, "click"), !0
-                },
-                _default: function(e) {
-                    var t = e.target;
-                    return pe.test(t.type) && t.click && A(t, "input") && Q.get(t, "click") || A(t, "a")
-                }
-            },
-            beforeunload: {
-                postDispatch: function(e) {
-                    void 0 !== e.result && e.originalEvent && (e.originalEvent.returnValue = e.result)
-                }
-            }
-        }
-    }, k.removeEvent = function(e, t, n) {
-        e.removeEventListener && e.removeEventListener(t, n)
-    }, k.Event = function(e, t) {
-        if (!(this instanceof k.Event)) return new k.Event(e, t);
-        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? ke : Se, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && k.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[k.expando] = !0
-    }, k.Event.prototype = {
-        constructor: k.Event,
-        isDefaultPrevented: Se,
-        isPropagationStopped: Se,
-        isImmediatePropagationStopped: Se,
-        isSimulated: !1,
-        preventDefault: function() {
-            var e = this.originalEvent;
-            this.isDefaultPrevented = ke, e && !this.isSimulated && e.preventDefault()
-        },
-        stopPropagation: function() {
-            var e = this.originalEvent;
-            this.isPropagationStopped = ke, e && !this.isSimulated && e.stopPropagation()
-        },
-        stopImmediatePropagation: function() {
-            var e = this.originalEvent;
-            this.isImmediatePropagationStopped = ke, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
-        }
-    }, k.each({
-        altKey: !0,
-        bubbles: !0,
-        cancelable: !0,
-        changedTouches: !0,
-        ctrlKey: !0,
-        detail: !0,
-        eventPhase: !0,
-        metaKey: !0,
-        pageX: !0,
-        pageY: !0,
-        shiftKey: !0,
-        view: !0,
-        "char": !0,
-        code: !0,
-        charCode: !0,
-        key: !0,
-        keyCode: !0,
-        button: !0,
-        buttons: !0,
-        clientX: !0,
-        clientY: !0,
-        offsetX: !0,
-        offsetY: !0,
-        pointerId: !0,
-        pointerType: !0,
-        screenX: !0,
-        screenY: !0,
-        targetTouches: !0,
-        toElement: !0,
-        touches: !0,
-        which: function(e) {
-            var t = e.button;
-            return null == e.which && Te.test(e.type) ? null != e.charCode ? e.charCode : e.keyCode : !e.which && void 0 !== t && Ce.test(e.type) ? 1 & t ? 1 : 2 & t ? 3 : 4 & t ? 2 : 0 : e.which
-        }
-    }, k.event.addProp), k.each({
-        focus: "focusin",
-        blur: "focusout"
-    }, function(e, t) {
-        k.event.special[e] = {
-            setup: function() {
-                return De(this, e, Ne), !1
-            },
-            trigger: function() {
-                return De(this, e), !0
-            },
-            delegateType: t
-        }
-    }), k.each({
-        mouseenter: "mouseover",
-        mouseleave: "mouseout",
-        pointerenter: "pointerover",
-        pointerleave: "pointerout"
-    }, function(e, i) {
-        k.event.special[e] = {
-            delegateType: i,
-            bindType: i,
-            handle: function(e) {
-                var t, n = e.relatedTarget,
-                    r = e.handleObj;
-                return n && (n === this || k.contains(this, n)) || (e.type = r.origType, t = r.handler.apply(this, arguments), e.type = i), t
-            }
-        }
-    }), k.fn.extend({
-        on: function(e, t, n, r) {
-            return Ae(this, e, t, n, r)
-        },
-        one: function(e, t, n, r) {
-            return Ae(this, e, t, n, r, 1)
-        },
-        off: function(e, t, n) {
-            var r, i;
-            if (e && e.preventDefault && e.handleObj) return r = e.handleObj, k(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
-            if ("object" == typeof e) {
-                for (i in e) this.off(i, t, e[i]);
-                return this
-            }
-            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Se), this.each(function() {
-                k.event.remove(this, e, n, t)
-            })
-        }
-    });
-    var je = /<(?!area|br|col|embed|hr|img|input|link|meta|param)(([a-z][^\/\0>\x20\t\r\n\f]*)[^>]*)\/>/gi,
-        qe = /<script|<style|<link/i,
-        Le = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        He = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
-
-    function Oe(e, t) {
-        return A(e, "table") && A(11 !== t.nodeType ? t : t.firstChild, "tr") && k(e).children("tbody")[0] || e
-    }
-
-    function Pe(e) {
-        return e.type = (null !== e.getAttribute("type")) + "/" + e.type, e
-    }
-
-    function Re(e) {
-        return "true/" === (e.type || "").slice(0, 5) ? e.type = e.type.slice(5) : e.removeAttribute("type"), e
-    }
-
-    function Me(e, t) {
-        var n, r, i, o, a, s, u, l;
-        if (1 === t.nodeType) {
-            if (Q.hasData(e) && (o = Q.access(e), a = Q.set(t, o), l = o.events))
-                for (i in delete a.handle, a.events = {}, l)
-                    for (n = 0, r = l[i].length; n < r; n++) k.event.add(t, i, l[i][n]);
-            J.hasData(e) && (s = J.access(e), u = k.extend({}, s), J.set(t, u))
-        }
-    }
-
-    function Ie(n, r, i, o) {
-        r = g.apply([], r);
-        var e, t, a, s, u, l, c = 0,
-            f = n.length,
-            p = f - 1,
-            d = r[0],
-            h = m(d);
-        if (h || 1 < f && "string" == typeof d && !y.checkClone && Le.test(d)) return n.each(function(e) {
-            var t = n.eq(e);
-            h && (r[0] = d.call(this, e, t.html())), Ie(t, r, i, o)
-        });
-        if (f && (t = (e = we(r, n[0].ownerDocument, !1, n, o)).firstChild, 1 === e.childNodes.length && (e = t), t || o)) {
-            for (s = (a = k.map(ve(e, "script"), Pe)).length; c < f; c++) u = e, c !== p && (u = k.clone(u, !0, !0), s && k.merge(a, ve(u, "script"))), i.call(n[c], u, c);
-            if (s)
-                for (l = a[a.length - 1].ownerDocument, k.map(a, Re), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Q.access(u, "globalEval") && k.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? k._evalUrl && !u.noModule && k._evalUrl(u.src, {
-                    nonce: u.nonce || u.getAttribute("nonce")
-                }) : b(u.textContent.replace(He, ""), u, l))
-        }
-        return n
-    }
-
-    function We(e, t, n) {
-        for (var r, i = t ? k.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || k.cleanData(ve(r)), r.parentNode && (n && oe(r) && ye(ve(r, "script")), r.parentNode.removeChild(r));
-        return e
-    }
-    k.extend({
-        htmlPrefilter: function(e) {
-            return e.replace(je, "<$1></$2>")
-        },
-        clone: function(e, t, n) {
-            var r, i, o, a, s, u, l, c = e.cloneNode(!0),
-                f = oe(e);
-            if (!(y.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || k.isXMLDoc(e)))
-                for (a = ve(c), r = 0, i = (o = ve(e)).length; r < i; r++) s = o[r], u = a[r], void 0, "input" === (l = u.nodeName.toLowerCase()) && pe.test(s.type) ? u.checked = s.checked : "input" !== l && "textarea" !== l || (u.defaultValue = s.defaultValue);
-            if (t)
-                if (n)
-                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Me(o[r], a[r]);
-                else Me(e, c);
-            return 0 < (a = ve(c, "script")).length && ye(a, !f && ve(e, "script")), c
-        },
-        cleanData: function(e) {
-            for (var t, n, r, i = k.event.special, o = 0; void 0 !== (n = e[o]); o++)
-                if (G(n)) {
-                    if (t = n[Q.expando]) {
-                        if (t.events)
-                            for (r in t.events) i[r] ? k.event.remove(n, r) : k.removeEvent(n, r, t.handle);
-                        n[Q.expando] = void 0
-                    }
-                    n[J.expando] && (n[J.expando] = void 0)
-                }
-        }
-    }), k.fn.extend({
-        detach: function(e) {
-            return We(this, e, !0)
-        },
-        remove: function(e) {
-            return We(this, e)
-        },
-        text: function(e) {
-            return _(this, function(e) {
-                return void 0 === e ? k.text(this) : this.empty().each(function() {
-                    1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || (this.textContent = e)
-                })
-            }, null, e, arguments.length)
-        },
-        append: function() {
-            return Ie(this, arguments, function(e) {
-                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || Oe(this, e).appendChild(e)
-            })
-        },
-        prepend: function() {
-            return Ie(this, arguments, function(e) {
-                if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                    var t = Oe(this, e);
-                    t.insertBefore(e, t.firstChild)
-                }
-            })
-        },
-        before: function() {
-            return Ie(this, arguments, function(e) {
-                this.parentNode && this.parentNode.insertBefore(e, this)
-            })
-        },
-        after: function() {
-            return Ie(this, arguments, function(e) {
-                this.parentNode && this.parentNode.insertBefore(e, this.nextSibling)
-            })
-        },
-        empty: function() {
-            for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (k.cleanData(ve(e, !1)), e.textContent = "");
-            return this
-        },
-        clone: function(e, t) {
-            return e = null != e && e, t = null == t ? e : t, this.map(function() {
-                return k.clone(this, e, t)
-            })
-        },
-        html: function(e) {
-            return _(this, function(e) {
-                var t = this[0] || {},
-                    n = 0,
-                    r = this.length;
-                if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
-                if ("string" == typeof e && !qe.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
-                    e = k.htmlPrefilter(e);
-                    try {
-                        for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (k.cleanData(ve(t, !1)), t.innerHTML = e);
-                        t = 0
-                    } catch (e) {}
-                }
-                t && this.empty().append(e)
-            }, null, e, arguments.length)
-        },
-        replaceWith: function() {
-            var n = [];
-            return Ie(this, arguments, function(e) {
-                var t = this.parentNode;
-                k.inArray(this, n) < 0 && (k.cleanData(ve(this)), t && t.replaceChild(e, this))
-            }, n)
-        }
-    }), k.each({
-        appendTo: "append",
-        prependTo: "prepend",
-        insertBefore: "before",
-        insertAfter: "after",
-        replaceAll: "replaceWith"
-    }, function(e, a) {
-        k.fn[e] = function(e) {
-            for (var t, n = [], r = k(e), i = r.length - 1, o = 0; o <= i; o++) t = o === i ? this : this.clone(!0), k(r[o])[a](t), u.apply(n, t.get());
-            return this.pushStack(n)
-        }
-    });
-    var $e = new RegExp("^(" + te + ")(?!px)[a-z%]+$", "i"),
-        Fe = function(e) {
-            var t = e.ownerDocument.defaultView;
-            return t && t.opener || (t = C), t.getComputedStyle(e)
-        },
-        Be = new RegExp(re.join("|"), "i");
-
-    function _e(e, t, n) {
-        var r, i, o, a, s = e.style;
-        return (n = n || Fe(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || oe(e) || (a = k.style(e, t)), !y.pixelBoxStyles() && $e.test(a) && Be.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
-    }
-
-    function ze(e, t) {
-        return {
-            get: function() {
-                if (!e()) return (this.get = t).apply(this, arguments);
-                delete this.get
-            }
-        }
-    }! function() {
-        function e() {
-            if (u) {
-                s.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", u.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", ie.appendChild(s).appendChild(u);
-                var e = C.getComputedStyle(u);
-                n = "1%" !== e.top, a = 12 === t(e.marginLeft), u.style.right = "60%", o = 36 === t(e.right), r = 36 === t(e.width), u.style.position = "absolute", i = 12 === t(u.offsetWidth / 3), ie.removeChild(s), u = null
-            }
-        }
-
-        function t(e) {
-            return Math.round(parseFloat(e))
-        }
-        var n, r, i, o, a, s = E.createElement("div"),
-            u = E.createElement("div");
-        u.style && (u.style.backgroundClip = "content-box", u.cloneNode(!0).style.backgroundClip = "", y.clearCloneStyle = "content-box" === u.style.backgroundClip, k.extend(y, {
-            boxSizingReliable: function() {
-                return e(), r
-            },
-            pixelBoxStyles: function() {
-                return e(), o
-            },
-            pixelPosition: function() {
-                return e(), n
-            },
-            reliableMarginLeft: function() {
-                return e(), a
-            },
-            scrollboxSize: function() {
-                return e(), i
-            }
-        }))
-    }();
-    var Ue = ["Webkit", "Moz", "ms"],
-        Xe = E.createElement("div").style,
-        Ve = {};
-
-    function Ge(e) {
-        var t = k.cssProps[e] || Ve[e];
-        return t || (e in Xe ? e : Ve[e] = function(e) {
-            var t = e[0].toUpperCase() + e.slice(1),
-                n = Ue.length;
-            while (n--)
-                if ((e = Ue[n] + t) in Xe) return e
-        }(e) || e)
-    }
-    var Ye = /^(none|table(?!-c[ea]).+)/,
-        Qe = /^--/,
-        Je = {
-            position: "absolute",
-            visibility: "hidden",
-            display: "block"
-        },
-        Ke = {
-            letterSpacing: "0",
-            fontWeight: "400"
-        };
-
-    function Ze(e, t, n) {
-        var r = ne.exec(t);
-        return r ? Math.max(0, r[2] - (n || 0)) + (r[3] || "px") : t
-    }
-
-    function et(e, t, n, r, i, o) {
-        var a = "width" === t ? 1 : 0,
-            s = 0,
-            u = 0;
-        if (n === (r ? "border" : "content")) return 0;
-        for (; a < 4; a += 2) "margin" === n && (u += k.css(e, n + re[a], !0, i)), r ? ("content" === n && (u -= k.css(e, "padding" + re[a], !0, i)), "margin" !== n && (u -= k.css(e, "border" + re[a] + "Width", !0, i))) : (u += k.css(e, "padding" + re[a], !0, i), "padding" !== n ? u += k.css(e, "border" + re[a] + "Width", !0, i) : s += k.css(e, "border" + re[a] + "Width", !0, i));
-        return !r && 0 <= o && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u
-    }
-
-    function tt(e, t, n) {
-        var r = Fe(e),
-            i = (!y.boxSizingReliable() || n) && "border-box" === k.css(e, "boxSizing", !1, r),
-            o = i,
-            a = _e(e, t, r),
-            s = "offset" + t[0].toUpperCase() + t.slice(1);
-        if ($e.test(a)) {
-            if (!n) return a;
-            a = "auto"
-        }
-        return (!y.boxSizingReliable() && i || "auto" === a || !parseFloat(a) && "inline" === k.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === k.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + et(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
-    }
-
-    function nt(e, t, n, r, i) {
-        return new nt.prototype.init(e, t, n, r, i)
-    }
-    k.extend({
-        cssHooks: {
-            opacity: {
-                get: function(e, t) {
-                    if (t) {
-                        var n = _e(e, "opacity");
-                        return "" === n ? "1" : n
-                    }
-                }
-            }
-        },
-        cssNumber: {
-            animationIterationCount: !0,
-            columnCount: !0,
-            fillOpacity: !0,
-            flexGrow: !0,
-            flexShrink: !0,
-            fontWeight: !0,
-            gridArea: !0,
-            gridColumn: !0,
-            gridColumnEnd: !0,
-            gridColumnStart: !0,
-            gridRow: !0,
-            gridRowEnd: !0,
-            gridRowStart: !0,
-            lineHeight: !0,
-            opacity: !0,
-            order: !0,
-            orphans: !0,
-            widows: !0,
-            zIndex: !0,
-            zoom: !0
-        },
-        cssProps: {},
-        style: function(e, t, n, r) {
-            if (e && 3 !== e.nodeType && 8 !== e.nodeType && e.style) {
-                var i, o, a, s = V(t),
-                    u = Qe.test(t),
-                    l = e.style;
-                if (u || (t = Ge(s)), a = k.cssHooks[t] || k.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
-                "string" === (o = typeof n) && (i = ne.exec(n)) && i[1] && (n = le(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (k.cssNumber[s] ? "" : "px")), y.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
-            }
-        },
-        css: function(e, t, n, r) {
-            var i, o, a, s = V(t);
-            return Qe.test(t) || (t = Ge(s)), (a = k.cssHooks[t] || k.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = _e(e, t, r)), "normal" === i && t in Ke && (i = Ke[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
-        }
-    }), k.each(["height", "width"], function(e, u) {
-        k.cssHooks[u] = {
-            get: function(e, t, n) {
-                if (t) return !Ye.test(k.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? tt(e, u, n) : ue(e, Je, function() {
-                    return tt(e, u, n)
-                })
-            },
-            set: function(e, t, n) {
-                var r, i = Fe(e),
-                    o = !y.scrollboxSize() && "absolute" === i.position,
-                    a = (o || n) && "border-box" === k.css(e, "boxSizing", !1, i),
-                    s = n ? et(e, u, n, a, i) : 0;
-                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - et(e, u, "border", !1, i) - .5)), s && (r = ne.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = k.css(e, u)), Ze(0, t, s)
-            }
-        }
-    }), k.cssHooks.marginLeft = ze(y.reliableMarginLeft, function(e, t) {
-        if (t) return (parseFloat(_e(e, "marginLeft")) || e.getBoundingClientRect().left - ue(e, {
-            marginLeft: 0
-        }, function() {
-            return e.getBoundingClientRect().left
-        })) + "px"
-    }), k.each({
-        margin: "",
-        padding: "",
-        border: "Width"
-    }, function(i, o) {
-        k.cssHooks[i + o] = {
-            expand: function(e) {
-                for (var t = 0, n = {}, r = "string" == typeof e ? e.split(" ") : [e]; t < 4; t++) n[i + re[t] + o] = r[t] || r[t - 2] || r[0];
-                return n
-            }
-        }, "margin" !== i && (k.cssHooks[i + o].set = Ze)
-    }), k.fn.extend({
-        css: function(e, t) {
-            return _(this, function(e, t, n) {
-                var r, i, o = {},
-                    a = 0;
-                if (Array.isArray(t)) {
-                    for (r = Fe(e), i = t.length; a < i; a++) o[t[a]] = k.css(e, t[a], !1, r);
-                    return o
-                }
-                return void 0 !== n ? k.style(e, t, n) : k.css(e, t)
-            }, e, t, 1 < arguments.length)
-        }
-    }), ((k.Tween = nt).prototype = {
-        constructor: nt,
-        init: function(e, t, n, r, i, o) {
-            this.elem = e, this.prop = n, this.easing = i || k.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (k.cssNumber[n] ? "" : "px")
-        },
-        cur: function() {
-            var e = nt.propHooks[this.prop];
-            return e && e.get ? e.get(this) : nt.propHooks._default.get(this)
-        },
-        run: function(e) {
-            var t, n = nt.propHooks[this.prop];
-            return this.options.duration ? this.pos = t = k.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : nt.propHooks._default.set(this), this
-        }
-    }).init.prototype = nt.prototype, (nt.propHooks = {
-        _default: {
-            get: function(e) {
-                var t;
-                return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = k.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
-            },
-            set: function(e) {
-                k.fx.step[e.prop] ? k.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !k.cssHooks[e.prop] && null == e.elem.style[Ge(e.prop)] ? e.elem[e.prop] = e.now : k.style(e.elem, e.prop, e.now + e.unit)
-            }
-        }
-    }).scrollTop = nt.propHooks.scrollLeft = {
-        set: function(e) {
-            e.elem.nodeType && e.elem.parentNode && (e.elem[e.prop] = e.now)
-        }
-    }, k.easing = {
-        linear: function(e) {
-            return e
-        },
-        swing: function(e) {
-            return .5 - Math.cos(e * Math.PI) / 2
-        },
-        _default: "swing"
-    }, k.fx = nt.prototype.init, k.fx.step = {};
-    var rt, it, ot, at, st = /^(?:toggle|show|hide)$/,
-        ut = /queueHooks$/;
-
-    function lt() {
-        it && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(lt) : C.setTimeout(lt, k.fx.interval), k.fx.tick())
-    }
-
-    function ct() {
-        return C.setTimeout(function() {
-            rt = void 0
-        }), rt = Date.now()
-    }
-
-    function ft(e, t) {
-        var n, r = 0,
-            i = {
-                height: e
-            };
-        for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = re[r])] = i["padding" + n] = e;
-        return t && (i.opacity = i.width = e), i
-    }
-
-    function pt(e, t, n) {
-        for (var r, i = (dt.tweeners[t] || []).concat(dt.tweeners["*"]), o = 0, a = i.length; o < a; o++)
-            if (r = i[o].call(n, t, e)) return r
-    }
-
-    function dt(o, e, t) {
-        var n, a, r = 0,
-            i = dt.prefilters.length,
-            s = k.Deferred().always(function() {
-                delete u.elem
-            }),
-            u = function() {
-                if (a) return !1;
-                for (var e = rt || ct(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
-                return s.notifyWith(o, [l, n, t]), n < 1 && i ? t : (i || s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l]), !1)
-            },
-            l = s.promise({
-                elem: o,
-                props: k.extend({}, e),
-                opts: k.extend(!0, {
-                    specialEasing: {},
-                    easing: k.easing._default
-                }, t),
-                originalProperties: e,
-                originalOptions: t,
-                startTime: rt || ct(),
-                duration: t.duration,
-                tweens: [],
-                createTween: function(e, t) {
-                    var n = k.Tween(o, l.opts, e, t, l.opts.specialEasing[e] || l.opts.easing);
-                    return l.tweens.push(n), n
-                },
-                stop: function(e) {
-                    var t = 0,
-                        n = e ? l.tweens.length : 0;
-                    if (a) return this;
-                    for (a = !0; t < n; t++) l.tweens[t].run(1);
-                    return e ? (s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l, e])) : s.rejectWith(o, [l, e]), this
-                }
-            }),
-            c = l.props;
-        for (! function(e, t) {
-                var n, r, i, o, a;
-                for (n in e)
-                    if (i = t[r = V(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = k.cssHooks[r]) && "expand" in a)
-                        for (n in o = a.expand(o), delete e[r], o) n in e || (e[n] = o[n], t[n] = i);
-                    else t[r] = i
-            }(c, l.opts.specialEasing); r < i; r++)
-            if (n = dt.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (k._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
-        return k.map(c, pt, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), k.fx.timer(k.extend(u, {
-            elem: o,
-            anim: l,
-            queue: l.opts.queue
-        })), l
-    }
-    k.Animation = k.extend(dt, {
-        tweeners: {
-            "*": [function(e, t) {
-                var n = this.createTween(e, t);
-                return le(n.elem, e, ne.exec(t), n), n
-            }]
-        },
-        tweener: function(e, t) {
-            m(e) ? (t = e, e = ["*"]) : e = e.match(R);
-            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], dt.tweeners[n] = dt.tweeners[n] || [], dt.tweeners[n].unshift(t)
-        },
-        prefilters: [function(e, t, n) {
-            var r, i, o, a, s, u, l, c, f = "width" in t || "height" in t,
-                p = this,
-                d = {},
-                h = e.style,
-                g = e.nodeType && se(e),
-                v = Q.get(e, "fxshow");
-            for (r in n.queue || (null == (a = k._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
-                    a.unqueued || s()
-                }), a.unqueued++, p.always(function() {
-                    p.always(function() {
-                        a.unqueued--, k.queue(e, "fx").length || a.empty.fire()
-                    })
-                })), t)
-                if (i = t[r], st.test(i)) {
-                    if (delete t[r], o = o || "toggle" === i, i === (g ? "hide" : "show")) {
-                        if ("show" !== i || !v || void 0 === v[r]) continue;
-                        g = !0
-                    }
-                    d[r] = v && v[r] || k.style(e, r)
-                } if ((u = !k.isEmptyObject(t)) || !k.isEmptyObject(d))
-                for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = Q.get(e, "display")), "none" === (c = k.css(e, "display")) && (l ? c = l : (fe([e], !0), l = e.style.display || l, c = k.css(e, "display"), fe([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === k.css(e, "float") && (u || (p.done(function() {
-                        h.display = l
-                    }), null == l && (c = h.display, l = "none" === c ? "" : c)), h.display = "inline-block")), n.overflow && (h.overflow = "hidden", p.always(function() {
-                        h.overflow = n.overflow[0], h.overflowX = n.overflow[1], h.overflowY = n.overflow[2]
-                    })), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = Q.access(e, "fxshow", {
-                    display: l
-                }), o && (v.hidden = !g), g && fe([e], !0), p.done(function() {
-                    for (r in g || fe([e]), Q.remove(e, "fxshow"), d) k.style(e, r, d[r])
-                })), u = pt(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
-        }],
-        prefilter: function(e, t) {
-            t ? dt.prefilters.unshift(e) : dt.prefilters.push(e)
-        }
-    }), k.speed = function(e, t, n) {
-        var r = e && "object" == typeof e ? k.extend({}, e) : {
-            complete: n || !n && t || m(e) && e,
-            duration: e,
-            easing: n && t || t && !m(t) && t
-        };
-        return k.fx.off ? r.duration = 0 : "number" != typeof r.duration && (r.duration in k.fx.speeds ? r.duration = k.fx.speeds[r.duration] : r.duration = k.fx.speeds._default), null != r.queue && !0 !== r.queue || (r.queue = "fx"), r.old = r.complete, r.complete = function() {
-            m(r.old) && r.old.call(this), r.queue && k.dequeue(this, r.queue)
-        }, r
-    }, k.fn.extend({
-        fadeTo: function(e, t, n, r) {
-            return this.filter(se).css("opacity", 0).show().end().animate({
-                opacity: t
-            }, e, n, r)
-        },
-        animate: function(t, e, n, r) {
-            var i = k.isEmptyObject(t),
-                o = k.speed(e, n, r),
-                a = function() {
-                    var e = dt(this, k.extend({}, t), o);
-                    (i || Q.get(this, "finish")) && e.stop(!0)
-                };
-            return a.finish = a, i || !1 === o.queue ? this.each(a) : this.queue(o.queue, a)
-        },
-        stop: function(i, e, o) {
-            var a = function(e) {
-                var t = e.stop;
-                delete e.stop, t(o)
-            };
-            return "string" != typeof i && (o = e, e = i, i = void 0), e && !1 !== i && this.queue(i || "fx", []), this.each(function() {
-                var e = !0,
-                    t = null != i && i + "queueHooks",
-                    n = k.timers,
-                    r = Q.get(this);
-                if (t) r[t] && r[t].stop && a(r[t]);
-                else
-                    for (t in r) r[t] && r[t].stop && ut.test(t) && a(r[t]);
-                for (t = n.length; t--;) n[t].elem !== this || null != i && n[t].queue !== i || (n[t].anim.stop(o), e = !1, n.splice(t, 1));
-                !e && o || k.dequeue(this, i)
-            })
-        },
-        finish: function(a) {
-            return !1 !== a && (a = a || "fx"), this.each(function() {
-                var e, t = Q.get(this),
-                    n = t[a + "queue"],
-                    r = t[a + "queueHooks"],
-                    i = k.timers,
-                    o = n ? n.length : 0;
-                for (t.finish = !0, k.queue(this, a, []), r && r.stop && r.stop.call(this, !0), e = i.length; e--;) i[e].elem === this && i[e].queue === a && (i[e].anim.stop(!0), i.splice(e, 1));
-                for (e = 0; e < o; e++) n[e] && n[e].finish && n[e].finish.call(this);
-                delete t.finish
-            })
-        }
-    }), k.each(["toggle", "show", "hide"], function(e, r) {
-        var i = k.fn[r];
-        k.fn[r] = function(e, t, n) {
-            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(ft(r, !0), e, t, n)
-        }
-    }), k.each({
-        slideDown: ft("show"),
-        slideUp: ft("hide"),
-        slideToggle: ft("toggle"),
-        fadeIn: {
-            opacity: "show"
-        },
-        fadeOut: {
-            opacity: "hide"
-        },
-        fadeToggle: {
-            opacity: "toggle"
-        }
-    }, function(e, r) {
-        k.fn[e] = function(e, t, n) {
-            return this.animate(r, e, t, n)
-        }
-    }), k.timers = [], k.fx.tick = function() {
-        var e, t = 0,
-            n = k.timers;
-        for (rt = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
-        n.length || k.fx.stop(), rt = void 0
-    }, k.fx.timer = function(e) {
-        k.timers.push(e), k.fx.start()
-    }, k.fx.interval = 13, k.fx.start = function() {
-        it || (it = !0, lt())
-    }, k.fx.stop = function() {
-        it = null
-    }, k.fx.speeds = {
-        slow: 600,
-        fast: 200,
-        _default: 400
-    }, k.fn.delay = function(r, e) {
-        return r = k.fx && k.fx.speeds[r] || r, e = e || "fx", this.queue(e, function(e, t) {
-            var n = C.setTimeout(e, r);
-            t.stop = function() {
-                C.clearTimeout(n)
-            }
-        })
-    }, ot = E.createElement("input"), at = E.createElement("select").appendChild(E.createElement("option")), ot.type = "checkbox", y.checkOn = "" !== ot.value, y.optSelected = at.selected, (ot = E.createElement("input")).value = "t", ot.type = "radio", y.radioValue = "t" === ot.value;
-    var ht, gt = k.expr.attrHandle;
-    k.fn.extend({
-        attr: function(e, t) {
-            return _(this, k.attr, e, t, 1 < arguments.length)
-        },
-        removeAttr: function(e) {
-            return this.each(function() {
-                k.removeAttr(this, e)
-            })
-        }
-    }), k.extend({
-        attr: function(e, t, n) {
-            var r, i, o = e.nodeType;
-            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? k.prop(e, t, n) : (1 === o && k.isXMLDoc(e) || (i = k.attrHooks[t.toLowerCase()] || (k.expr.match.bool.test(t) ? ht : void 0)), void 0 !== n ? null === n ? void k.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = k.find.attr(e, t)) ? void 0 : r)
-        },
-        attrHooks: {
-            type: {
-                set: function(e, t) {
-                    if (!y.radioValue && "radio" === t && A(e, "input")) {
-                        var n = e.value;
-                        return e.setAttribute("type", t), n && (e.value = n), t
-                    }
-                }
-            }
-        },
-        removeAttr: function(e, t) {
-            var n, r = 0,
-                i = t && t.match(R);
-            if (i && 1 === e.nodeType)
-                while (n = i[r++]) e.removeAttribute(n)
-        }
-    }), ht = {
-        set: function(e, t, n) {
-            return !1 === t ? k.removeAttr(e, n) : e.setAttribute(n, n), n
-        }
-    }, k.each(k.expr.match.bool.source.match(/\w+/g), function(e, t) {
-        var a = gt[t] || k.find.attr;
-        gt[t] = function(e, t, n) {
-            var r, i, o = t.toLowerCase();
-            return n || (i = gt[o], gt[o] = r, r = null != a(e, t, n) ? o : null, gt[o] = i), r
-        }
-    });
-    var vt = /^(?:input|select|textarea|button)$/i,
-        yt = /^(?:a|area)$/i;
-
-    function mt(e) {
-        return (e.match(R) || []).join(" ")
-    }
-
-    function xt(e) {
-        return e.getAttribute && e.getAttribute("class") || ""
-    }
-
-    function bt(e) {
-        return Array.isArray(e) ? e : "string" == typeof e && e.match(R) || []
-    }
-    k.fn.extend({
-        prop: function(e, t) {
-            return _(this, k.prop, e, t, 1 < arguments.length)
-        },
-        removeProp: function(e) {
-            return this.each(function() {
-                delete this[k.propFix[e] || e]
-            })
-        }
-    }), k.extend({
-        prop: function(e, t, n) {
-            var r, i, o = e.nodeType;
-            if (3 !== o && 8 !== o && 2 !== o) return 1 === o && k.isXMLDoc(e) || (t = k.propFix[t] || t, i = k.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
-        },
-        propHooks: {
-            tabIndex: {
-                get: function(e) {
-                    var t = k.find.attr(e, "tabindex");
-                    return t ? parseInt(t, 10) : vt.test(e.nodeName) || yt.test(e.nodeName) && e.href ? 0 : -1
-                }
-            }
-        },
-        propFix: {
-            "for": "htmlFor",
-            "class": "className"
-        }
-    }), y.optSelected || (k.propHooks.selected = {
-        get: function(e) {
-            var t = e.parentNode;
-            return t && t.parentNode && t.parentNode.selectedIndex, null
-        },
-        set: function(e) {
-            var t = e.parentNode;
-            t && (t.selectedIndex, t.parentNode && t.parentNode.selectedIndex)
-        }
-    }), k.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
-        k.propFix[this.toLowerCase()] = this
-    }), k.fn.extend({
-        addClass: function(t) {
-            var e, n, r, i, o, a, s, u = 0;
-            if (m(t)) return this.each(function(e) {
-                k(this).addClass(t.call(this, e, xt(this)))
-            });
-            if ((e = bt(t)).length)
-                while (n = this[u++])
-                    if (i = xt(n), r = 1 === n.nodeType && " " + mt(i) + " ") {
-                        a = 0;
-                        while (o = e[a++]) r.indexOf(" " + o + " ") < 0 && (r += o + " ");
-                        i !== (s = mt(r)) && n.setAttribute("class", s)
-                    } return this
-        },
-        removeClass: function(t) {
-            var e, n, r, i, o, a, s, u = 0;
-            if (m(t)) return this.each(function(e) {
-                k(this).removeClass(t.call(this, e, xt(this)))
-            });
-            if (!arguments.length) return this.attr("class", "");
-            if ((e = bt(t)).length)
-                while (n = this[u++])
-                    if (i = xt(n), r = 1 === n.nodeType && " " + mt(i) + " ") {
-                        a = 0;
-                        while (o = e[a++])
-                            while (-1 < r.indexOf(" " + o + " ")) r = r.replace(" " + o + " ", " ");
-                        i !== (s = mt(r)) && n.setAttribute("class", s)
-                    } return this
-        },
-        toggleClass: function(i, t) {
-            var o = typeof i,
-                a = "string" === o || Array.isArray(i);
-            return "boolean" == typeof t && a ? t ? this.addClass(i) : this.removeClass(i) : m(i) ? this.each(function(e) {
-                k(this).toggleClass(i.call(this, e, xt(this), t), t)
-            }) : this.each(function() {
-                var e, t, n, r;
-                if (a) {
-                    t = 0, n = k(this), r = bt(i);
-                    while (e = r[t++]) n.hasClass(e) ? n.removeClass(e) : n.addClass(e)
-                } else void 0 !== i && "boolean" !== o || ((e = xt(this)) && Q.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Q.get(this, "__className__") || ""))
-            })
-        },
-        hasClass: function(e) {
-            var t, n, r = 0;
-            t = " " + e + " ";
-            while (n = this[r++])
-                if (1 === n.nodeType && -1 < (" " + mt(xt(n)) + " ").indexOf(t)) return !0;
-            return !1
-        }
-    });
-    var wt = /\r/g;
-    k.fn.extend({
-        val: function(n) {
-            var r, e, i, t = this[0];
-            return arguments.length ? (i = m(n), this.each(function(e) {
-                var t;
-                1 === this.nodeType && (null == (t = i ? n.call(this, e, k(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = k.map(t, function(e) {
-                    return null == e ? "" : e + ""
-                })), (r = k.valHooks[this.type] || k.valHooks[this.nodeName.toLowerCase()]) && "set" in r && void 0 !== r.set(this, t, "value") || (this.value = t))
-            })) : t ? (r = k.valHooks[t.type] || k.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(wt, "") : null == e ? "" : e : void 0
-        }
-    }), k.extend({
-        valHooks: {
-            option: {
-                get: function(e) {
-                    var t = k.find.attr(e, "value");
-                    return null != t ? t : mt(k.text(e))
-                }
-            },
-            select: {
-                get: function(e) {
-                    var t, n, r, i = e.options,
-                        o = e.selectedIndex,
-                        a = "select-one" === e.type,
-                        s = a ? null : [],
-                        u = a ? o + 1 : i.length;
-                    for (r = o < 0 ? u : a ? o : 0; r < u; r++)
-                        if (((n = i[r]).selected || r === o) && !n.disabled && (!n.parentNode.disabled || !A(n.parentNode, "optgroup"))) {
-                            if (t = k(n).val(), a) return t;
-                            s.push(t)
-                        } return s
-                },
-                set: function(e, t) {
-                    var n, r, i = e.options,
-                        o = k.makeArray(t),
-                        a = i.length;
-                    while (a--)((r = i[a]).selected = -1 < k.inArray(k.valHooks.option.get(r), o)) && (n = !0);
-                    return n || (e.selectedIndex = -1), o
-                }
-            }
-        }
-    }), k.each(["radio", "checkbox"], function() {
-        k.valHooks[this] = {
-            set: function(e, t) {
-                if (Array.isArray(t)) return e.checked = -1 < k.inArray(k(e).val(), t)
-            }
-        }, y.checkOn || (k.valHooks[this].get = function(e) {
-            return null === e.getAttribute("value") ? "on" : e.value
-        })
-    }), y.focusin = "onfocusin" in C;
-    var Tt = /^(?:focusinfocus|focusoutblur)$/,
-        Ct = function(e) {
-            e.stopPropagation()
-        };
-    k.extend(k.event, {
-        trigger: function(e, t, n, r) {
-            var i, o, a, s, u, l, c, f, p = [n || E],
-                d = v.call(e, "type") ? e.type : e,
-                h = v.call(e, "namespace") ? e.namespace.split(".") : [];
-            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !Tt.test(d + k.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[k.expando] ? e : new k.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : k.makeArray(t, [e]), c = k.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
-                if (!r && !c.noBubble && !x(n)) {
-                    for (s = c.delegateType || d, Tt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
-                    a === (n.ownerDocument || E) && p.push(a.defaultView || a.parentWindow || C)
-                }
-                i = 0;
-                while ((o = p[i++]) && !e.isPropagationStopped()) f = o, e.type = 1 < i ? s : c.bindType || d, (l = (Q.get(o, "events") || {})[e.type] && Q.get(o, "handle")) && l.apply(o, t), (l = u && o[u]) && l.apply && G(o) && (e.result = l.apply(o, t), !1 === e.result && e.preventDefault());
-                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !G(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), k.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, Ct), n[d](), e.isPropagationStopped() && f.removeEventListener(d, Ct), k.event.triggered = void 0, a && (n[u] = a)), e.result
-            }
-        },
-        simulate: function(e, t, n) {
-            var r = k.extend(new k.Event, n, {
-                type: e,
-                isSimulated: !0
-            });
-            k.event.trigger(r, null, t)
-        }
-    }), k.fn.extend({
-        trigger: function(e, t) {
-            return this.each(function() {
-                k.event.trigger(e, t, this)
-            })
-        },
-        triggerHandler: function(e, t) {
-            var n = this[0];
-            if (n) return k.event.trigger(e, t, n, !0)
-        }
-    }), y.focusin || k.each({
-        focus: "focusin",
-        blur: "focusout"
-    }, function(n, r) {
-        var i = function(e) {
-            k.event.simulate(r, e.target, k.event.fix(e))
-        };
-        k.event.special[r] = {
-            setup: function() {
-                var e = this.ownerDocument || this,
-                    t = Q.access(e, r);
-                t || e.addEventListener(n, i, !0), Q.access(e, r, (t || 0) + 1)
-            },
-            teardown: function() {
-                var e = this.ownerDocument || this,
-                    t = Q.access(e, r) - 1;
-                t ? Q.access(e, r, t) : (e.removeEventListener(n, i, !0), Q.remove(e, r))
-            }
-        }
-    });
-    var Et = C.location,
-        kt = Date.now(),
-        St = /\?/;
-    k.parseXML = function(e) {
-        var t;
-        if (!e || "string" != typeof e) return null;
-        try {
-            t = (new C.DOMParser).parseFromString(e, "text/xml")
-        } catch (e) {
-            t = void 0
-        }
-        return t && !t.getElementsByTagName("parsererror").length || k.error("Invalid XML: " + e), t
-    };
-    var Nt = /\[\]$/,
-        At = /\r?\n/g,
-        Dt = /^(?:submit|button|image|reset|file)$/i,
-        jt = /^(?:input|select|textarea|keygen)/i;
-
-    function qt(n, e, r, i) {
-        var t;
-        if (Array.isArray(e)) k.each(e, function(e, t) {
-            r || Nt.test(n) ? i(n, t) : qt(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
-        });
-        else if (r || "object" !== w(e)) i(n, e);
-        else
-            for (t in e) qt(n + "[" + t + "]", e[t], r, i)
-    }
-    k.param = function(e, t) {
-        var n, r = [],
-            i = function(e, t) {
-                var n = m(t) ? t() : t;
-                r[r.length] = encodeURIComponent(e) + "=" + encodeURIComponent(null == n ? "" : n)
-            };
-        if (null == e) return "";
-        if (Array.isArray(e) || e.jquery && !k.isPlainObject(e)) k.each(e, function() {
-            i(this.name, this.value)
-        });
-        else
-            for (n in e) qt(n, e[n], t, i);
-        return r.join("&")
-    }, k.fn.extend({
-        serialize: function() {
-            return k.param(this.serializeArray())
-        },
-        serializeArray: function() {
-            return this.map(function() {
-                var e = k.prop(this, "elements");
-                return e ? k.makeArray(e) : this
-            }).filter(function() {
-                var e = this.type;
-                return this.name && !k(this).is(":disabled") && jt.test(this.nodeName) && !Dt.test(e) && (this.checked || !pe.test(e))
-            }).map(function(e, t) {
-                var n = k(this).val();
-                return null == n ? null : Array.isArray(n) ? k.map(n, function(e) {
-                    return {
-                        name: t.name,
-                        value: e.replace(At, "\r\n")
-                    }
-                }) : {
-                    name: t.name,
-                    value: n.replace(At, "\r\n")
-                }
-            }).get()
-        }
-    });
-    var Lt = /%20/g,
-        Ht = /#.*$/,
-        Ot = /([?&])_=[^&]*/,
-        Pt = /^(.*?):[ \t]*([^\r\n]*)$/gm,
-        Rt = /^(?:GET|HEAD)$/,
-        Mt = /^\/\//,
-        It = {},
-        Wt = {},
-        $t = "*/".concat("*"),
-        Ft = E.createElement("a");
-
-    function Bt(o) {
-        return function(e, t) {
-            "string" != typeof e && (t = e, e = "*");
-            var n, r = 0,
-                i = e.toLowerCase().match(R) || [];
-            if (m(t))
-                while (n = i[r++]) "+" === n[0] ? (n = n.slice(1) || "*", (o[n] = o[n] || []).unshift(t)) : (o[n] = o[n] || []).push(t)
-        }
-    }
-
-    function _t(t, i, o, a) {
-        var s = {},
-            u = t === Wt;
-
-        function l(e) {
-            var r;
-            return s[e] = !0, k.each(t[e] || [], function(e, t) {
-                var n = t(i, o, a);
-                return "string" != typeof n || u || s[n] ? u ? !(r = n) : void 0 : (i.dataTypes.unshift(n), l(n), !1)
-            }), r
-        }
-        return l(i.dataTypes[0]) || !s["*"] && l("*")
-    }
-
-    function zt(e, t) {
-        var n, r, i = k.ajaxSettings.flatOptions || {};
-        for (n in t) void 0 !== t[n] && ((i[n] ? e : r || (r = {}))[n] = t[n]);
-        return r && k.extend(!0, e, r), e
-    }
-    Ft.href = Et.href, k.extend({
-        active: 0,
-        lastModified: {},
-        etag: {},
-        ajaxSettings: {
-            url: Et.href,
-            type: "GET",
-            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Et.protocol),
-            global: !0,
-            processData: !0,
-            async: !0,
-            contentType: "application/x-www-form-urlencoded; charset=UTF-8",
-            accepts: {
-                "*": $t,
-                text: "text/plain",
-                html: "text/html",
-                xml: "application/xml, text/xml",
-                json: "application/json, text/javascript"
-            },
-            contents: {
-                xml: /\bxml\b/,
-                html: /\bhtml/,
-                json: /\bjson\b/
-            },
-            responseFields: {
-                xml: "responseXML",
-                text: "responseText",
-                json: "responseJSON"
-            },
-            converters: {
-                "* text": String,
-                "text html": !0,
-                "text json": JSON.parse,
-                "text xml": k.parseXML
-            },
-            flatOptions: {
-                url: !0,
-                context: !0
-            }
-        },
-        ajaxSetup: function(e, t) {
-            return t ? zt(zt(e, k.ajaxSettings), t) : zt(k.ajaxSettings, e)
-        },
-        ajaxPrefilter: Bt(It),
-        ajaxTransport: Bt(Wt),
-        ajax: function(e, t) {
-            "object" == typeof e && (t = e, e = void 0), t = t || {};
-            var c, f, p, n, d, r, h, g, i, o, v = k.ajaxSetup({}, t),
-                y = v.context || v,
-                m = v.context && (y.nodeType || y.jquery) ? k(y) : k.event,
-                x = k.Deferred(),
-                b = k.Callbacks("once memory"),
-                w = v.statusCode || {},
-                a = {},
-                s = {},
-                u = "canceled",
-                T = {
-                    readyState: 0,
-                    getResponseHeader: function(e) {
-                        var t;
-                        if (h) {
-                            if (!n) {
-                                n = {};
-                                while (t = Pt.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
-                            }
-                            t = n[e.toLowerCase() + " "]
-                        }
-                        return null == t ? null : t.join(", ")
-                    },
-                    getAllResponseHeaders: function() {
-                        return h ? p : null
-                    },
-                    setRequestHeader: function(e, t) {
-                        return null == h && (e = s[e.toLowerCase()] = s[e.toLowerCase()] || e, a[e] = t), this
-                    },
-                    overrideMimeType: function(e) {
-                        return null == h && (v.mimeType = e), this
-                    },
-                    statusCode: function(e) {
-                        var t;
-                        if (e)
-                            if (h) T.always(e[T.status]);
-                            else
-                                for (t in e) w[t] = [w[t], e[t]];
-                        return this
-                    },
-                    abort: function(e) {
-                        var t = e || u;
-                        return c && c.abort(t), l(0, t), this
-                    }
-                };
-            if (x.promise(T), v.url = ((e || v.url || Et.href) + "").replace(Mt, Et.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(R) || [""], null == v.crossDomain) {
-                r = E.createElement("a");
-                try {
-                    r.href = v.url, r.href = r.href, v.crossDomain = Ft.protocol + "//" + Ft.host != r.protocol + "//" + r.host
-                } catch (e) {
-                    v.crossDomain = !0
-                }
-            }
-            if (v.data && v.processData && "string" != typeof v.data && (v.data = k.param(v.data, v.traditional)), _t(It, v, t, T), h) return T;
-            for (i in (g = k.event && v.global) && 0 == k.active++ && k.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Rt.test(v.type), f = v.url.replace(Ht, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(Lt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (St.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Ot, "$1"), o = (St.test(f) ? "&" : "?") + "_=" + kt++ + o), v.url = f + o), v.ifModified && (k.lastModified[f] && T.setRequestHeader("If-Modified-Since", k.lastModified[f]), k.etag[f] && T.setRequestHeader("If-None-Match", k.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + $t + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
-            if (v.beforeSend && (!1 === v.beforeSend.call(y, T, v) || h)) return T.abort();
-            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = _t(Wt, v, t, T)) {
-                if (T.readyState = 1, g && m.trigger("ajaxSend", [T, v]), h) return T;
-                v.async && 0 < v.timeout && (d = C.setTimeout(function() {
-                    T.abort("timeout")
-                }, v.timeout));
-                try {
-                    h = !1, c.send(a, l)
-                } catch (e) {
-                    if (h) throw e;
-                    l(-1, e)
-                }
-            } else l(-1, "No Transport");
-
-            function l(e, t, n, r) {
-                var i, o, a, s, u, l = t;
-                h || (h = !0, d && C.clearTimeout(d), c = void 0, p = r || "", T.readyState = 0 < e ? 4 : 0, i = 200 <= e && e < 300 || 304 === e, n && (s = function(e, t, n) {
-                    var r, i, o, a, s = e.contents,
-                        u = e.dataTypes;
-                    while ("*" === u[0]) u.shift(), void 0 === r && (r = e.mimeType || t.getResponseHeader("Content-Type"));
-                    if (r)
-                        for (i in s)
-                            if (s[i] && s[i].test(r)) {
-                                u.unshift(i);
-                                break
-                            } if (u[0] in n) o = u[0];
-                    else {
-                        for (i in n) {
-                            if (!u[0] || e.converters[i + " " + u[0]]) {
-                                o = i;
-                                break
-                            }
-                            a || (a = i)
-                        }
-                        o = o || a
-                    }
-                    if (o) return o !== u[0] && u.unshift(o), n[o]
-                }(v, T, n)), s = function(e, t, n, r) {
-                    var i, o, a, s, u, l = {},
-                        c = e.dataTypes.slice();
-                    if (c[1])
-                        for (a in e.converters) l[a.toLowerCase()] = e.converters[a];
-                    o = c.shift();
-                    while (o)
-                        if (e.responseFields[o] && (n[e.responseFields[o]] = t), !u && r && e.dataFilter && (t = e.dataFilter(t, e.dataType)), u = o, o = c.shift())
-                            if ("*" === o) o = u;
-                            else if ("*" !== u && u !== o) {
-                        if (!(a = l[u + " " + o] || l["* " + o]))
-                            for (i in l)
-                                if ((s = i.split(" "))[1] === o && (a = l[u + " " + s[0]] || l["* " + s[0]])) {
-                                    !0 === a ? a = l[i] : !0 !== l[i] && (o = s[0], c.unshift(s[1]));
-                                    break
-                                } if (!0 !== a)
-                            if (a && e["throws"]) t = a(t);
-                            else try {
-                                t = a(t)
-                            } catch (e) {
-                                return {
-                                    state: "parsererror",
-                                    error: a ? e : "No conversion from " + u + " to " + o
-                                }
-                            }
-                    }
-                    return {
-                        state: "success",
-                        data: t
-                    }
-                }(v, s, T, i), i ? (v.ifModified && ((u = T.getResponseHeader("Last-Modified")) && (k.lastModified[f] = u), (u = T.getResponseHeader("etag")) && (k.etag[f] = u)), 204 === e || "HEAD" === v.type ? l = "nocontent" : 304 === e ? l = "notmodified" : (l = s.state, o = s.data, i = !(a = s.error))) : (a = l, !e && l || (l = "error", e < 0 && (e = 0))), T.status = e, T.statusText = (t || l) + "", i ? x.resolveWith(y, [o, l, T]) : x.rejectWith(y, [T, l, a]), T.statusCode(w), w = void 0, g && m.trigger(i ? "ajaxSuccess" : "ajaxError", [T, v, i ? o : a]), b.fireWith(y, [T, l]), g && (m.trigger("ajaxComplete", [T, v]), --k.active || k.event.trigger("ajaxStop")))
-            }
-            return T
-        },
-        getJSON: function(e, t, n) {
-            return k.get(e, t, n, "json")
-        },
-        getScript: function(e, t) {
-            return k.get(e, void 0, t, "script")
-        }
-    }), k.each(["get", "post"], function(e, i) {
-        k[i] = function(e, t, n, r) {
-            return m(t) && (r = r || n, n = t, t = void 0), k.ajax(k.extend({
-                url: e,
-                type: i,
-                dataType: r,
-                data: t,
-                success: n
-            }, k.isPlainObject(e) && e))
-        }
-    }), k._evalUrl = function(e, t) {
-        return k.ajax({
-            url: e,
-            type: "GET",
-            dataType: "script",
-            cache: !0,
-            async: !1,
-            global: !1,
-            converters: {
-                "text script": function() {}
-            },
-            dataFilter: function(e) {
-                k.globalEval(e, t)
-            }
-        })
-    }, k.fn.extend({
-        wrapAll: function(e) {
-            var t;
-            return this[0] && (m(e) && (e = e.call(this[0])), t = k(e, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && t.insertBefore(this[0]), t.map(function() {
-                var e = this;
-                while (e.firstElementChild) e = e.firstElementChild;
-                return e
-            }).append(this)), this
-        },
-        wrapInner: function(n) {
-            return m(n) ? this.each(function(e) {
-                k(this).wrapInner(n.call(this, e))
-            }) : this.each(function() {
-                var e = k(this),
-                    t = e.contents();
-                t.length ? t.wrapAll(n) : e.append(n)
-            })
-        },
-        wrap: function(t) {
-            var n = m(t);
-            return this.each(function(e) {
-                k(this).wrapAll(n ? t.call(this, e) : t)
-            })
-        },
-        unwrap: function(e) {
-            return this.parent(e).not("body").each(function() {
-                k(this).replaceWith(this.childNodes)
-            }), this
-        }
-    }), k.expr.pseudos.hidden = function(e) {
-        return !k.expr.pseudos.visible(e)
-    }, k.expr.pseudos.visible = function(e) {
-        return !!(e.offsetWidth || e.offsetHeight || e.getClientRects().length)
-    }, k.ajaxSettings.xhr = function() {
-        try {
-            return new C.XMLHttpRequest
-        } catch (e) {}
-    };
-    var Ut = {
-            0: 200,
-            1223: 204
-        },
-        Xt = k.ajaxSettings.xhr();
-    y.cors = !!Xt && "withCredentials" in Xt, y.ajax = Xt = !!Xt, k.ajaxTransport(function(i) {
-        var o, a;
-        if (y.cors || Xt && !i.crossDomain) return {
-            send: function(e, t) {
-                var n, r = i.xhr();
-                if (r.open(i.type, i.url, i.async, i.username, i.password), i.xhrFields)
-                    for (n in i.xhrFields) r[n] = i.xhrFields[n];
-                for (n in i.mimeType && r.overrideMimeType && r.overrideMimeType(i.mimeType), i.crossDomain || e["X-Requested-With"] || (e["X-Requested-With"] = "XMLHttpRequest"), e) r.setRequestHeader(n, e[n]);
-                o = function(e) {
-                    return function() {
-                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(Ut[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
-                            binary: r.response
-                        } : {
-                            text: r.responseText
-                        }, r.getAllResponseHeaders()))
-                    }
-                }, r.onload = o(), a = r.onerror = r.ontimeout = o("error"), void 0 !== r.onabort ? r.onabort = a : r.onreadystatechange = function() {
-                    4 === r.readyState && C.setTimeout(function() {
-                        o && a()
-                    })
-                }, o = o("abort");
-                try {
-                    r.send(i.hasContent && i.data || null)
-                } catch (e) {
-                    if (o) throw e
-                }
-            },
-            abort: function() {
-                o && o()
-            }
-        }
-    }), k.ajaxPrefilter(function(e) {
-        e.crossDomain && (e.contents.script = !1)
-    }), k.ajaxSetup({
-        accepts: {
-            script: "text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"
-        },
-        contents: {
-            script: /\b(?:java|ecma)script\b/
-        },
-        converters: {
-            "text script": function(e) {
-                return k.globalEval(e), e
-            }
-        }
-    }), k.ajaxPrefilter("script", function(e) {
-        void 0 === e.cache && (e.cache = !1), e.crossDomain && (e.type = "GET")
-    }), k.ajaxTransport("script", function(n) {
-        var r, i;
-        if (n.crossDomain || n.scriptAttrs) return {
-            send: function(e, t) {
-                r = k("<script>").attr(n.scriptAttrs || {}).prop({
-                    charset: n.scriptCharset,
-                    src: n.url
-                }).on("load error", i = function(e) {
-                    r.remove(), i = null, e && t("error" === e.type ? 404 : 200, e.type)
-                }), E.head.appendChild(r[0])
-            },
-            abort: function() {
-                i && i()
-            }
-        }
-    });
-    var Vt, Gt = [],
-        Yt = /(=)\?(?=&|$)|\?\?/;
-    k.ajaxSetup({
-        jsonp: "callback",
-        jsonpCallback: function() {
-            var e = Gt.pop() || k.expando + "_" + kt++;
-            return this[e] = !0, e
-        }
-    }), k.ajaxPrefilter("json jsonp", function(e, t, n) {
-        var r, i, o, a = !1 !== e.jsonp && (Yt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Yt.test(e.data) && "data");
-        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Yt, "$1" + r) : !1 !== e.jsonp && (e.url += (St.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
-            return o || k.error(r + " was not called"), o[0]
-        }, e.dataTypes[0] = "json", i = C[r], C[r] = function() {
-            o = arguments
-        }, n.always(function() {
-            void 0 === i ? k(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, Gt.push(r)), o && m(i) && i(o[0]), o = i = void 0
-        }), "script"
-    }), y.createHTMLDocument = ((Vt = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Vt.childNodes.length), k.parseHTML = function(e, t, n) {
-        return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (y.createHTMLDocument ? ((r = (t = E.implementation.createHTMLDocument("")).createElement("base")).href = E.location.href, t.head.appendChild(r)) : t = E), o = !n && [], (i = D.exec(e)) ? [t.createElement(i[1])] : (i = we([e], t, o), o && o.length && k(o).remove(), k.merge([], i.childNodes)));
-        var r, i, o
-    }, k.fn.load = function(e, t, n) {
-        var r, i, o, a = this,
-            s = e.indexOf(" ");
-        return -1 < s && (r = mt(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && k.ajax({
-            url: e,
-            type: i || "GET",
-            dataType: "html",
-            data: t
-        }).done(function(e) {
-            o = arguments, a.html(r ? k("<div>").append(k.parseHTML(e)).find(r) : e)
-        }).always(n && function(e, t) {
-            a.each(function() {
-                n.apply(this, o || [e.responseText, t, e])
-            })
-        }), this
-    }, k.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(e, t) {
-        k.fn[t] = function(e) {
-            return this.on(t, e)
-        }
-    }), k.expr.pseudos.animated = function(t) {
-        return k.grep(k.timers, function(e) {
-            return t === e.elem
-        }).length
-    }, k.offset = {
-        setOffset: function(e, t, n) {
-            var r, i, o, a, s, u, l = k.css(e, "position"),
-                c = k(e),
-                f = {};
-            "static" === l && (e.style.position = "relative"), s = c.offset(), o = k.css(e, "top"), u = k.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, k.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : c.css(f)
-        }
-    }, k.fn.extend({
-        offset: function(t) {
-            if (arguments.length) return void 0 === t ? this : this.each(function(e) {
-                k.offset.setOffset(this, t, e)
-            });
-            var e, n, r = this[0];
-            return r ? r.getClientRects().length ? (e = r.getBoundingClientRect(), n = r.ownerDocument.defaultView, {
-                top: e.top + n.pageYOffset,
-                left: e.left + n.pageXOffset
-            }) : {
-                top: 0,
-                left: 0
-            } : void 0
-        },
-        position: function() {
-            if (this[0]) {
-                var e, t, n, r = this[0],
-                    i = {
-                        top: 0,
-                        left: 0
-                    };
-                if ("fixed" === k.css(r, "position")) t = r.getBoundingClientRect();
-                else {
-                    t = this.offset(), n = r.ownerDocument, e = r.offsetParent || n.documentElement;
-                    while (e && (e === n.body || e === n.documentElement) && "static" === k.css(e, "position")) e = e.parentNode;
-                    e && e !== r && 1 === e.nodeType && ((i = k(e).offset()).top += k.css(e, "borderTopWidth", !0), i.left += k.css(e, "borderLeftWidth", !0))
-                }
-                return {
-                    top: t.top - i.top - k.css(r, "marginTop", !0),
-                    left: t.left - i.left - k.css(r, "marginLeft", !0)
-                }
-            }
-        },
-        offsetParent: function() {
-            return this.map(function() {
-                var e = this.offsetParent;
-                while (e && "static" === k.css(e, "position")) e = e.offsetParent;
-                return e || ie
-            })
-        }
-    }), k.each({
-        scrollLeft: "pageXOffset",
-        scrollTop: "pageYOffset"
-    }, function(t, i) {
-        var o = "pageYOffset" === i;
-        k.fn[t] = function(e) {
-            return _(this, function(e, t, n) {
-                var r;
-                if (x(e) ? r = e : 9 === e.nodeType && (r = e.defaultView), void 0 === n) return r ? r[i] : e[t];
-                r ? r.scrollTo(o ? r.pageXOffset : n, o ? n : r.pageYOffset) : e[t] = n
-            }, t, e, arguments.length)
-        }
-    }), k.each(["top", "left"], function(e, n) {
-        k.cssHooks[n] = ze(y.pixelPosition, function(e, t) {
-            if (t) return t = _e(e, n), $e.test(t) ? k(e).position()[n] + "px" : t
-        })
-    }), k.each({
-        Height: "height",
-        Width: "width"
-    }, function(a, s) {
-        k.each({
-            padding: "inner" + a,
-            content: s,
-            "": "outer" + a
-        }, function(r, o) {
-            k.fn[o] = function(e, t) {
-                var n = arguments.length && (r || "boolean" != typeof e),
-                    i = r || (!0 === e || !0 === t ? "margin" : "border");
-                return _(this, function(e, t, n) {
-                    var r;
-                    return x(e) ? 0 === o.indexOf("outer") ? e["inner" + a] : e.document.documentElement["client" + a] : 9 === e.nodeType ? (r = e.documentElement, Math.max(e.body["scroll" + a], r["scroll" + a], e.body["offset" + a], r["offset" + a], r["client" + a])) : void 0 === n ? k.css(e, t, i) : k.style(e, t, n, i)
-                }, s, n ? e : void 0, n)
-            }
-        })
-    }), k.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(e, n) {
-        k.fn[n] = function(e, t) {
-            return 0 < arguments.length ? this.on(n, null, e, t) : this.trigger(n)
-        }
-    }), k.fn.extend({
-        hover: function(e, t) {
-            return this.mouseenter(e).mouseleave(t || e)
-        }
-    }), k.fn.extend({
-        bind: function(e, t, n) {
-            return this.on(e, null, t, n)
-        },
-        unbind: function(e, t) {
-            return this.off(e, null, t)
-        },
-        delegate: function(e, t, n, r) {
-            return this.on(t, e, n, r)
-        },
-        undelegate: function(e, t, n) {
-            return 1 === arguments.length ? this.off(e, "**") : this.off(t, e || "**", n)
-        }
-    }), k.proxy = function(e, t) {
-        var n, r, i;
-        if ("string" == typeof t && (n = e[t], t = e, e = n), m(e)) return r = s.call(arguments, 2), (i = function() {
-            return e.apply(t || this, r.concat(s.call(arguments)))
-        }).guid = e.guid = e.guid || k.guid++, i
-    }, k.holdReady = function(e) {
-        e ? k.readyWait++ : k.ready(!0)
-    }, k.isArray = Array.isArray, k.parseJSON = JSON.parse, k.nodeName = A, k.isFunction = m, k.isWindow = x, k.camelCase = V, k.type = w, k.now = Date.now, k.isNumeric = function(e) {
-        var t = k.type(e);
-        return ("number" === t || "string" === t) && !isNaN(e - parseFloat(e))
-    }, "function" == typeof define && define.amd && define("jquery", [], function() {
-        return k
-    });
-    var Qt = C.jQuery,
-        Jt = C.$;
-    return k.noConflict = function(e) {
-        return C.$ === k && (C.$ = Jt), e && C.jQuery === k && (C.jQuery = Qt), k
-    }, e || (C.jQuery = C.$ = k), k
+/*! jQuery v3.7.1 | (c) OpenJS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
+    "use strict";
+    "object" == typeof module && "object" == typeof module.exports ? module.exports = e.document ? t(e, !0) : function(e) {
+        if (!e.document) throw new Error("jQuery requires a window with a document");
+        return t(e)
+    } : t(e)
+}("undefined" != typeof window ? window : this, function(ie, e) {
+    "use strict";
+    var oe = [],
+        r = Object.getPrototypeOf,
+        ae = oe.slice,
+        g = oe.flat ? function(e) {
+            return oe.flat.call(e)
+        } : function(e) {
+            return oe.concat.apply([], e)
+        },
+        s = oe.push,
+        se = oe.indexOf,
+        n = {},
+        i = n.toString,
+        ue = n.hasOwnProperty,
+        o = ue.toString,
+        a = o.call(Object),
+        le = {},
+        v = function(e) {
+            return "function" == typeof e && "number" != typeof e.nodeType && "function" != typeof e.item
+        },
+        y = function(e) {
+            return null != e && e === e.window
+        },
+        C = ie.document,
+        u = {
+            type: !0,
+            src: !0,
+            nonce: !0,
+            noModule: !0
+        };
+
+    function m(e, t, n) {
+        var r, i, o = (n = n || C).createElement("script");
+        if (o.text = e, t)
+            for (r in u)(i = t[r] || t.getAttribute && t.getAttribute(r)) && o.setAttribute(r, i);
+        n.head.appendChild(o).parentNode.removeChild(o)
+    }
+
+    function x(e) {
+        return null == e ? e + "" : "object" == typeof e || "function" == typeof e ? n[i.call(e)] || "object" : typeof e
+    }
+    var t = "3.7.1",
+        l = /HTML$/i,
+        ce = function(e, t) {
+            return new ce.fn.init(e, t)
+        };
+
+    function c(e) {
+        var t = !!e && "length" in e && e.length,
+            n = x(e);
+        return !v(e) && !y(e) && ("array" === n || 0 === t || "number" == typeof t && 0 < t && t - 1 in e)
+    }
+
+    function fe(e, t) {
+        return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
+    }
+    ce.fn = ce.prototype = {
+        jquery: t,
+        constructor: ce,
+        length: 0,
+        toArray: function() {
+            return ae.call(this)
+        },
+        get: function(e) {
+            return null == e ? ae.call(this) : e < 0 ? this[e + this.length] : this[e]
+        },
+        pushStack: function(e) {
+            var t = ce.merge(this.constructor(), e);
+            return t.prevObject = this, t
+        },
+        each: function(e) {
+            return ce.each(this, e)
+        },
+        map: function(n) {
+            return this.pushStack(ce.map(this, function(e, t) {
+                return n.call(e, t, e)
+            }))
+        },
+        slice: function() {
+            return this.pushStack(ae.apply(this, arguments))
+        },
+        first: function() {
+            return this.eq(0)
+        },
+        last: function() {
+            return this.eq(-1)
+        },
+        even: function() {
+            return this.pushStack(ce.grep(this, function(e, t) {
+                return (t + 1) % 2
+            }))
+        },
+        odd: function() {
+            return this.pushStack(ce.grep(this, function(e, t) {
+                return t % 2
+            }))
+        },
+        eq: function(e) {
+            var t = this.length,
+                n = +e + (e < 0 ? t : 0);
+            return this.pushStack(0 <= n && n < t ? [this[n]] : [])
+        },
+        end: function() {
+            return this.prevObject || this.constructor()
+        },
+        push: s,
+        sort: oe.sort,
+        splice: oe.splice
+    }, ce.extend = ce.fn.extend = function() {
+        var e, t, n, r, i, o, a = arguments[0] || {},
+            s = 1,
+            u = arguments.length,
+            l = !1;
+        for ("boolean" == typeof a && (l = a, a = arguments[s] || {}, s++), "object" == typeof a || v(a) || (a = {}), s === u && (a = this, s--); s < u; s++)
+            if (null != (e = arguments[s]))
+                for (t in e) r = e[t], "__proto__" !== t && a !== r && (l && r && (ce.isPlainObject(r) || (i = Array.isArray(r))) ? (n = a[t], o = i && !Array.isArray(n) ? [] : i || ce.isPlainObject(n) ? n : {}, i = !1, a[t] = ce.extend(l, o, r)) : void 0 !== r && (a[t] = r));
+        return a
+    }, ce.extend({
+        expando: "jQuery" + (t + Math.random()).replace(/\D/g, ""),
+        isReady: !0,
+        error: function(e) {
+            throw new Error(e)
+        },
+        noop: function() {},
+        isPlainObject: function(e) {
+            var t, n;
+            return !(!e || "[object Object]" !== i.call(e)) && (!(t = r(e)) || "function" == typeof(n = ue.call(t, "constructor") && t.constructor) && o.call(n) === a)
+        },
+        isEmptyObject: function(e) {
+            var t;
+            for (t in e) return !1;
+            return !0
+        },
+        globalEval: function(e, t, n) {
+            m(e, {
+                nonce: t && t.nonce
+            }, n)
+        },
+        each: function(e, t) {
+            var n, r = 0;
+            if (c(e)) {
+                for (n = e.length; r < n; r++)
+                    if (!1 === t.call(e[r], r, e[r])) break
+            } else
+                for (r in e)
+                    if (!1 === t.call(e[r], r, e[r])) break;
+            return e
+        },
+        text: function(e) {
+            var t, n = "",
+                r = 0,
+                i = e.nodeType;
+            if (!i)
+                while (t = e[r++]) n += ce.text(t);
+            return 1 === i || 11 === i ? e.textContent : 9 === i ? e.documentElement.textContent : 3 === i || 4 === i ? e.nodeValue : n
+        },
+        makeArray: function(e, t) {
+            var n = t || [];
+            return null != e && (c(Object(e)) ? ce.merge(n, "string" == typeof e ? [e] : e) : s.call(n, e)), n
+        },
+        inArray: function(e, t, n) {
+            return null == t ? -1 : se.call(t, e, n)
+        },
+        isXMLDoc: function(e) {
+            var t = e && e.namespaceURI,
+                n = e && (e.ownerDocument || e).documentElement;
+            return !l.test(t || n && n.nodeName || "HTML")
+        },
+        merge: function(e, t) {
+            for (var n = +t.length, r = 0, i = e.length; r < n; r++) e[i++] = t[r];
+            return e.length = i, e
+        },
+        grep: function(e, t, n) {
+            for (var r = [], i = 0, o = e.length, a = !n; i < o; i++) !t(e[i], i) !== a && r.push(e[i]);
+            return r
+        },
+        map: function(e, t, n) {
+            var r, i, o = 0,
+                a = [];
+            if (c(e))
+                for (r = e.length; o < r; o++) null != (i = t(e[o], o, n)) && a.push(i);
+            else
+                for (o in e) null != (i = t(e[o], o, n)) && a.push(i);
+            return g(a)
+        },
+        guid: 1,
+        support: le
+    }), "function" == typeof Symbol && (ce.fn[Symbol.iterator] = oe[Symbol.iterator]), ce.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(e, t) {
+        n["[object " + t + "]"] = t.toLowerCase()
+    });
+    var pe = oe.pop,
+        de = oe.sort,
+        he = oe.splice,
+        ge = "[\\x20\\t\\r\\n\\f]",
+        ve = new RegExp("^" + ge + "+|((?:^|[^\\\\])(?:\\\\.)*)" + ge + "+$", "g");
+    ce.contains = function(e, t) {
+        var n = t && t.parentNode;
+        return e === n || !(!n || 1 !== n.nodeType || !(e.contains ? e.contains(n) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(n)))
+    };
+    var f = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\x80-\uFFFF\w-]/g;
+
+    function p(e, t) {
+        return t ? "\0" === e ? "\ufffd" : e.slice(0, -1) + "\\" + e.charCodeAt(e.length - 1).toString(16) + " " : "\\" + e
+    }
+    ce.escapeSelector = function(e) {
+        return (e + "").replace(f, p)
+    };
+    var ye = C,
+        me = s;
+    ! function() {
+        var e, b, w, o, a, T, r, C, d, i, k = me,
+            S = ce.expando,
+            E = 0,
+            n = 0,
+            s = W(),
+            c = W(),
+            u = W(),
+            h = W(),
+            l = function(e, t) {
+                return e === t && (a = !0), 0
+            },
+            f = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
+            t = "(?:\\\\[\\da-fA-F]{1,6}" + ge + "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
+            p = "\\[" + ge + "*(" + t + ")(?:" + ge + "*([*^$|!~]?=)" + ge + "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + t + "))|)" + ge + "*\\]",
+            g = ":(" + t + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + p + ")*)|.*)\\)|)",
+            v = new RegExp(ge + "+", "g"),
+            y = new RegExp("^" + ge + "*," + ge + "*"),
+            m = new RegExp("^" + ge + "*([>+~]|" + ge + ")" + ge + "*"),
+            x = new RegExp(ge + "|>"),
+            j = new RegExp(g),
+            A = new RegExp("^" + t + "$"),
+            D = {
+                ID: new RegExp("^#(" + t + ")"),
+                CLASS: new RegExp("^\\.(" + t + ")"),
+                TAG: new RegExp("^(" + t + "|[*])"),
+                ATTR: new RegExp("^" + p),
+                PSEUDO: new RegExp("^" + g),
+                CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + ge + "*(even|odd|(([+-]|)(\\d*)n|)" + ge + "*(?:([+-]|)" + ge + "*(\\d+)|))" + ge + "*\\)|)", "i"),
+                bool: new RegExp("^(?:" + f + ")$", "i"),
+                needsContext: new RegExp("^" + ge + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + ge + "*((?:-\\d)?\\d*)" + ge + "*\\)|)(?=[^-]|$)", "i")
+            },
+            N = /^(?:input|select|textarea|button)$/i,
+            q = /^h\d$/i,
+            L = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
+            H = /[+~]/,
+            O = new RegExp("\\\\[\\da-fA-F]{1,6}" + ge + "?|\\\\([^\\r\\n\\f])", "g"),
+            P = function(e, t) {
+                var n = "0x" + e.slice(1) - 65536;
+                return t || (n < 0 ? String.fromCharCode(n + 65536) : String.fromCharCode(n >> 10 | 55296, 1023 & n | 56320))
+            },
+            M = function() {
+                V()
+            },
+            R = J(function(e) {
+                return !0 === e.disabled && fe(e, "fieldset")
+            }, {
+                dir: "parentNode",
+                next: "legend"
+            });
+        try {
+            k.apply(oe = ae.call(ye.childNodes), ye.childNodes), oe[ye.childNodes.length].nodeType
+        } catch (e) {
+            k = {
+                apply: function(e, t) {
+                    me.apply(e, ae.call(t))
+                },
+                call: function(e) {
+                    me.apply(e, ae.call(arguments, 1))
+                }
+            }
+        }
+
+        function I(t, e, n, r) {
+            var i, o, a, s, u, l, c, f = e && e.ownerDocument,
+                p = e ? e.nodeType : 9;
+            if (n = n || [], "string" != typeof t || !t || 1 !== p && 9 !== p && 11 !== p) return n;
+            if (!r && (V(e), e = e || T, C)) {
+                if (11 !== p && (u = L.exec(t)))
+                    if (i = u[1]) {
+                        if (9 === p) {
+                            if (!(a = e.getElementById(i))) return n;
+                            if (a.id === i) return k.call(n, a), n
+                        } else if (f && (a = f.getElementById(i)) && I.contains(e, a) && a.id === i) return k.call(n, a), n
+                    } else {
+                        if (u[2]) return k.apply(n, e.getElementsByTagName(t)), n;
+                        if ((i = u[3]) && e.getElementsByClassName) return k.apply(n, e.getElementsByClassName(i)), n
+                    } if (!(h[t + " "] || d && d.test(t))) {
+                    if (c = t, f = e, 1 === p && (x.test(t) || m.test(t))) {
+                        (f = H.test(t) && U(e.parentNode) || e) == e && le.scope || ((s = e.getAttribute("id")) ? s = ce.escapeSelector(s) : e.setAttribute("id", s = S)), o = (l = Y(t)).length;
+                        while (o--) l[o] = (s ? "#" + s : ":scope") + " " + Q(l[o]);
+                        c = l.join(",")
+                    }
+                    try {
+                        return k.apply(n, f.querySelectorAll(c)), n
+                    } catch (e) {
+                        h(t, !0)
+                    } finally {
+                        s === S && e.removeAttribute("id")
+                    }
+                }
+            }
+            return re(t.replace(ve, "$1"), e, n, r)
+        }
+
+        function W() {
+            var r = [];
+            return function e(t, n) {
+                return r.push(t + " ") > b.cacheLength && delete e[r.shift()], e[t + " "] = n
+            }
+        }
+
+        function F(e) {
+            return e[S] = !0, e
+        }
+
+        function $(e) {
+            var t = T.createElement("fieldset");
+            try {
+                return !!e(t)
+            } catch (e) {
+                return !1
+            } finally {
+                t.parentNode && t.parentNode.removeChild(t), t = null
+            }
+        }
+
+        function B(t) {
+            return function(e) {
+                return fe(e, "input") && e.type === t
+            }
+        }
+
+        function _(t) {
+            return function(e) {
+                return (fe(e, "input") || fe(e, "button")) && e.type === t
+            }
+        }
+
+        function z(t) {
+            return function(e) {
+                return "form" in e ? e.parentNode && !1 === e.disabled ? "label" in e ? "label" in e.parentNode ? e.parentNode.disabled === t : e.disabled === t : e.isDisabled === t || e.isDisabled !== !t && R(e) === t : e.disabled === t : "label" in e && e.disabled === t
+            }
+        }
+
+        function X(a) {
+            return F(function(o) {
+                return o = +o, F(function(e, t) {
+                    var n, r = a([], e.length, o),
+                        i = r.length;
+                    while (i--) e[n = r[i]] && (e[n] = !(t[n] = e[n]))
+                })
+            })
+        }
+
+        function U(e) {
+            return e && "undefined" != typeof e.getElementsByTagName && e
+        }
+
+        function V(e) {
+            var t, n = e ? e.ownerDocument || e : ye;
+            return n != T && 9 === n.nodeType && n.documentElement && (r = (T = n).documentElement, C = !ce.isXMLDoc(T), i = r.matches || r.webkitMatchesSelector || r.msMatchesSelector, r.msMatchesSelector && ye != T && (t = T.defaultView) && t.top !== t && t.addEventListener("unload", M), le.getById = $(function(e) {
+                return r.appendChild(e).id = ce.expando, !T.getElementsByName || !T.getElementsByName(ce.expando).length
+            }), le.disconnectedMatch = $(function(e) {
+                return i.call(e, "*")
+            }), le.scope = $(function() {
+                return T.querySelectorAll(":scope")
+            }), le.cssHas = $(function() {
+                try {
+                    return T.querySelector(":has(*,:jqfake)"), !1
+                } catch (e) {
+                    return !0
+                }
+            }), le.getById ? (b.filter.ID = function(e) {
+                var t = e.replace(O, P);
+                return function(e) {
+                    return e.getAttribute("id") === t
+                }
+            }, b.find.ID = function(e, t) {
+                if ("undefined" != typeof t.getElementById && C) {
+                    var n = t.getElementById(e);
+                    return n ? [n] : []
+                }
+            }) : (b.filter.ID = function(e) {
+                var n = e.replace(O, P);
+                return function(e) {
+                    var t = "undefined" != typeof e.getAttributeNode && e.getAttributeNode("id");
+                    return t && t.value === n
+                }
+            }, b.find.ID = function(e, t) {
+                if ("undefined" != typeof t.getElementById && C) {
+                    var n, r, i, o = t.getElementById(e);
+                    if (o) {
+                        if ((n = o.getAttributeNode("id")) && n.value === e) return [o];
+                        i = t.getElementsByName(e), r = 0;
+                        while (o = i[r++])
+                            if ((n = o.getAttributeNode("id")) && n.value === e) return [o]
+                    }
+                    return []
+                }
+            }), b.find.TAG = function(e, t) {
+                return "undefined" != typeof t.getElementsByTagName ? t.getElementsByTagName(e) : t.querySelectorAll(e)
+            }, b.find.CLASS = function(e, t) {
+                if ("undefined" != typeof t.getElementsByClassName && C) return t.getElementsByClassName(e)
+            }, d = [], $(function(e) {
+                var t;
+                r.appendChild(e).innerHTML = "<a id='" + S + "' href='' disabled='disabled'></a><select id='" + S + "-\r\\' disabled='disabled'><option selected=''></option></select>", e.querySelectorAll("[selected]").length || d.push("\\[" + ge + "*(?:value|" + f + ")"), e.querySelectorAll("[id~=" + S + "-]").length || d.push("~="), e.querySelectorAll("a#" + S + "+*").length || d.push(".#.+[+~]"), e.querySelectorAll(":checked").length || d.push(":checked"), (t = T.createElement("input")).setAttribute("type", "hidden"), e.appendChild(t).setAttribute("name", "D"), r.appendChild(e).disabled = !0, 2 !== e.querySelectorAll(":disabled").length && d.push(":enabled", ":disabled"), (t = T.createElement("input")).setAttribute("name", ""), e.appendChild(t), e.querySelectorAll("[name='']").length || d.push("\\[" + ge + "*name" + ge + "*=" + ge + "*(?:''|\"\")")
+            }), le.cssHas || d.push(":has"), d = d.length && new RegExp(d.join("|")), l = function(e, t) {
+                if (e === t) return a = !0, 0;
+                var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
+                return n || (1 & (n = (e.ownerDocument || e) == (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !le.sortDetached && t.compareDocumentPosition(e) === n ? e === T || e.ownerDocument == ye && I.contains(ye, e) ? -1 : t === T || t.ownerDocument == ye && I.contains(ye, t) ? 1 : o ? se.call(o, e) - se.call(o, t) : 0 : 4 & n ? -1 : 1)
+            }), T
+        }
+        for (e in I.matches = function(e, t) {
+                return I(e, null, null, t)
+            }, I.matchesSelector = function(e, t) {
+                if (V(e), C && !h[t + " "] && (!d || !d.test(t))) try {
+                    var n = i.call(e, t);
+                    if (n || le.disconnectedMatch || e.document && 11 !== e.document.nodeType) return n
+                } catch (e) {
+                    h(t, !0)
+                }
+                return 0 < I(t, T, null, [e]).length
+            }, I.contains = function(e, t) {
+                return (e.ownerDocument || e) != T && V(e), ce.contains(e, t)
+            }, I.attr = function(e, t) {
+                (e.ownerDocument || e) != T && V(e);
+                var n = b.attrHandle[t.toLowerCase()],
+                    r = n && ue.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !C) : void 0;
+                return void 0 !== r ? r : e.getAttribute(t)
+            }, I.error = function(e) {
+                throw new Error("Syntax error, unrecognized expression: " + e)
+            }, ce.uniqueSort = function(e) {
+                var t, n = [],
+                    r = 0,
+                    i = 0;
+                if (a = !le.sortStable, o = !le.sortStable && ae.call(e, 0), de.call(e, l), a) {
+                    while (t = e[i++]) t === e[i] && (r = n.push(i));
+                    while (r--) he.call(e, n[r], 1)
+                }
+                return o = null, e
+            }, ce.fn.uniqueSort = function() {
+                return this.pushStack(ce.uniqueSort(ae.apply(this)))
+            }, (b = ce.expr = {
+                cacheLength: 50,
+                createPseudo: F,
+                match: D,
+                attrHandle: {},
+                find: {},
+                relative: {
+                    ">": {
+                        dir: "parentNode",
+                        first: !0
+                    },
+                    " ": {
+                        dir: "parentNode"
+                    },
+                    "+": {
+                        dir: "previousSibling",
+                        first: !0
+                    },
+                    "~": {
+                        dir: "previousSibling"
+                    }
+                },
+                preFilter: {
+                    ATTR: function(e) {
+                        return e[1] = e[1].replace(O, P), e[3] = (e[3] || e[4] || e[5] || "").replace(O, P), "~=" === e[2] && (e[3] = " " + e[3] + " "), e.slice(0, 4)
+                    },
+                    CHILD: function(e) {
+                        return e[1] = e[1].toLowerCase(), "nth" === e[1].slice(0, 3) ? (e[3] || I.error(e[0]), e[4] = +(e[4] ? e[5] + (e[6] || 1) : 2 * ("even" === e[3] || "odd" === e[3])), e[5] = +(e[7] + e[8] || "odd" === e[3])) : e[3] && I.error(e[0]), e
+                    },
+                    PSEUDO: function(e) {
+                        var t, n = !e[6] && e[2];
+                        return D.CHILD.test(e[0]) ? null : (e[3] ? e[2] = e[4] || e[5] || "" : n && j.test(n) && (t = Y(n, !0)) && (t = n.indexOf(")", n.length - t) - n.length) && (e[0] = e[0].slice(0, t), e[2] = n.slice(0, t)), e.slice(0, 3))
+                    }
+                },
+                filter: {
+                    TAG: function(e) {
+                        var t = e.replace(O, P).toLowerCase();
+                        return "*" === e ? function() {
+                            return !0
+                        } : function(e) {
+                            return fe(e, t)
+                        }
+                    },
+                    CLASS: function(e) {
+                        var t = s[e + " "];
+                        return t || (t = new RegExp("(^|" + ge + ")" + e + "(" + ge + "|$)")) && s(e, function(e) {
+                            return t.test("string" == typeof e.className && e.className || "undefined" != typeof e.getAttribute && e.getAttribute("class") || "")
+                        })
+                    },
+                    ATTR: function(n, r, i) {
+                        return function(e) {
+                            var t = I.attr(e, n);
+                            return null == t ? "!=" === r : !r || (t += "", "=" === r ? t === i : "!=" === r ? t !== i : "^=" === r ? i && 0 === t.indexOf(i) : "*=" === r ? i && -1 < t.indexOf(i) : "$=" === r ? i && t.slice(-i.length) === i : "~=" === r ? -1 < (" " + t.replace(v, " ") + " ").indexOf(i) : "|=" === r && (t === i || t.slice(0, i.length + 1) === i + "-"))
+                        }
+                    },
+                    CHILD: function(d, e, t, h, g) {
+                        var v = "nth" !== d.slice(0, 3),
+                            y = "last" !== d.slice(-4),
+                            m = "of-type" === e;
+                        return 1 === h && 0 === g ? function(e) {
+                            return !!e.parentNode
+                        } : function(e, t, n) {
+                            var r, i, o, a, s, u = v !== y ? "nextSibling" : "previousSibling",
+                                l = e.parentNode,
+                                c = m && e.nodeName.toLowerCase(),
+                                f = !n && !m,
+                                p = !1;
+                            if (l) {
+                                if (v) {
+                                    while (u) {
+                                        o = e;
+                                        while (o = o[u])
+                                            if (m ? fe(o, c) : 1 === o.nodeType) return !1;
+                                        s = u = "only" === d && !s && "nextSibling"
+                                    }
+                                    return !0
+                                }
+                                if (s = [y ? l.firstChild : l.lastChild], y && f) {
+                                    p = (a = (r = (i = l[S] || (l[S] = {}))[d] || [])[0] === E && r[1]) && r[2], o = a && l.childNodes[a];
+                                    while (o = ++a && o && o[u] || (p = a = 0) || s.pop())
+                                        if (1 === o.nodeType && ++p && o === e) {
+                                            i[d] = [E, a, p];
+                                            break
+                                        }
+                                } else if (f && (p = a = (r = (i = e[S] || (e[S] = {}))[d] || [])[0] === E && r[1]), !1 === p)
+                                    while (o = ++a && o && o[u] || (p = a = 0) || s.pop())
+                                        if ((m ? fe(o, c) : 1 === o.nodeType) && ++p && (f && ((i = o[S] || (o[S] = {}))[d] = [E, p]), o === e)) break;
+                                return (p -= g) === h || p % h == 0 && 0 <= p / h
+                            }
+                        }
+                    },
+                    PSEUDO: function(e, o) {
+                        var t, a = b.pseudos[e] || b.setFilters[e.toLowerCase()] || I.error("unsupported pseudo: " + e);
+                        return a[S] ? a(o) : 1 < a.length ? (t = [e, e, "", o], b.setFilters.hasOwnProperty(e.toLowerCase()) ? F(function(e, t) {
+                            var n, r = a(e, o),
+                                i = r.length;
+                            while (i--) e[n = se.call(e, r[i])] = !(t[n] = r[i])
+                        }) : function(e) {
+                            return a(e, 0, t)
+                        }) : a
+                    }
+                },
+                pseudos: {
+                    not: F(function(e) {
+                        var r = [],
+                            i = [],
+                            s = ne(e.replace(ve, "$1"));
+                        return s[S] ? F(function(e, t, n, r) {
+                            var i, o = s(e, null, r, []),
+                                a = e.length;
+                            while (a--)(i = o[a]) && (e[a] = !(t[a] = i))
+                        }) : function(e, t, n) {
+                            return r[0] = e, s(r, null, n, i), r[0] = null, !i.pop()
+                        }
+                    }),
+                    has: F(function(t) {
+                        return function(e) {
+                            return 0 < I(t, e).length
+                        }
+                    }),
+                    contains: F(function(t) {
+                        return t = t.replace(O, P),
+                            function(e) {
+                                return -1 < (e.textContent || ce.text(e)).indexOf(t)
+                            }
+                    }),
+                    lang: F(function(n) {
+                        return A.test(n || "") || I.error("unsupported lang: " + n), n = n.replace(O, P).toLowerCase(),
+                            function(e) {
+                                var t;
+                                do {
+                                    if (t = C ? e.lang : e.getAttribute("xml:lang") || e.getAttribute("lang")) return (t = t.toLowerCase()) === n || 0 === t.indexOf(n + "-")
+                                } while ((e = e.parentNode) && 1 === e.nodeType);
+                                return !1
+                            }
+                    }),
+                    target: function(e) {
+                        var t = ie.location && ie.location.hash;
+                        return t && t.slice(1) === e.id
+                    },
+                    root: function(e) {
+                        return e === r
+                    },
+                    focus: function(e) {
+                        return e === function() {
+                            try {
+                                return T.activeElement
+                            } catch (e) {}
+                        }() && T.hasFocus() && !!(e.type || e.href || ~e.tabIndex)
+                    },
+                    enabled: z(!1),
+                    disabled: z(!0),
+                    checked: function(e) {
+                        return fe(e, "input") && !!e.checked || fe(e, "option") && !!e.selected
+                    },
+                    selected: function(e) {
+                        return e.parentNode && e.parentNode.selectedIndex, !0 === e.selected
+                    },
+                    empty: function(e) {
+                        for (e = e.firstChild; e; e = e.nextSibling)
+                            if (e.nodeType < 6) return !1;
+                        return !0
+                    },
+                    parent: function(e) {
+                        return !b.pseudos.empty(e)
+                    },
+                    header: function(e) {
+                        return q.test(e.nodeName)
+                    },
+                    input: function(e) {
+                        return N.test(e.nodeName)
+                    },
+                    button: function(e) {
+                        return fe(e, "input") && "button" === e.type || fe(e, "button")
+                    },
+                    text: function(e) {
+                        var t;
+                        return fe(e, "input") && "text" === e.type && (null == (t = e.getAttribute("type")) || "text" === t.toLowerCase())
+                    },
+                    first: X(function() {
+                        return [0]
+                    }),
+                    last: X(function(e, t) {
+                        return [t - 1]
+                    }),
+                    eq: X(function(e, t, n) {
+                        return [n < 0 ? n + t : n]
+                    }),
+                    even: X(function(e, t) {
+                        for (var n = 0; n < t; n += 2) e.push(n);
+                        return e
+                    }),
+                    odd: X(function(e, t) {
+                        for (var n = 1; n < t; n += 2) e.push(n);
+                        return e
+                    }),
+                    lt: X(function(e, t, n) {
+                        var r;
+                        for (r = n < 0 ? n + t : t < n ? t : n; 0 <= --r;) e.push(r);
+                        return e
+                    }),
+                    gt: X(function(e, t, n) {
+                        for (var r = n < 0 ? n + t : n; ++r < t;) e.push(r);
+                        return e
+                    })
+                }
+            }).pseudos.nth = b.pseudos.eq, {
+                radio: !0,
+                checkbox: !0,
+                file: !0,
+                password: !0,
+                image: !0
+            }) b.pseudos[e] = B(e);
+        for (e in {
+                submit: !0,
+                reset: !0
+            }) b.pseudos[e] = _(e);
+
+        function G() {}
+
+        function Y(e, t) {
+            var n, r, i, o, a, s, u, l = c[e + " "];
+            if (l) return t ? 0 : l.slice(0);
+            a = e, s = [], u = b.preFilter;
+            while (a) {
+                for (o in n && !(r = y.exec(a)) || (r && (a = a.slice(r[0].length) || a), s.push(i = [])), n = !1, (r = m.exec(a)) && (n = r.shift(), i.push({
+                        value: n,
+                        type: r[0].replace(ve, " ")
+                    }), a = a.slice(n.length)), b.filter) !(r = D[o].exec(a)) || u[o] && !(r = u[o](r)) || (n = r.shift(), i.push({
+                    value: n,
+                    type: o,
+                    matches: r
+                }), a = a.slice(n.length));
+                if (!n) break
+            }
+            return t ? a.length : a ? I.error(e) : c(e, s).slice(0)
+        }
+
+        function Q(e) {
+            for (var t = 0, n = e.length, r = ""; t < n; t++) r += e[t].value;
+            return r
+        }
+
+        function J(a, e, t) {
+            var s = e.dir,
+                u = e.next,
+                l = u || s,
+                c = t && "parentNode" === l,
+                f = n++;
+            return e.first ? function(e, t, n) {
+                while (e = e[s])
+                    if (1 === e.nodeType || c) return a(e, t, n);
+                return !1
+            } : function(e, t, n) {
+                var r, i, o = [E, f];
+                if (n) {
+                    while (e = e[s])
+                        if ((1 === e.nodeType || c) && a(e, t, n)) return !0
+                } else
+                    while (e = e[s])
+                        if (1 === e.nodeType || c)
+                            if (i = e[S] || (e[S] = {}), u && fe(e, u)) e = e[s] || e;
+                            else {
+                                if ((r = i[l]) && r[0] === E && r[1] === f) return o[2] = r[2];
+                                if ((i[l] = o)[2] = a(e, t, n)) return !0
+                            } return !1
+            }
+        }
+
+        function K(i) {
+            return 1 < i.length ? function(e, t, n) {
+                var r = i.length;
+                while (r--)
+                    if (!i[r](e, t, n)) return !1;
+                return !0
+            } : i[0]
+        }
+
+        function Z(e, t, n, r, i) {
+            for (var o, a = [], s = 0, u = e.length, l = null != t; s < u; s++)(o = e[s]) && (n && !n(o, r, i) || (a.push(o), l && t.push(s)));
+            return a
+        }
+
+        function ee(d, h, g, v, y, e) {
+            return v && !v[S] && (v = ee(v)), y && !y[S] && (y = ee(y, e)), F(function(e, t, n, r) {
+                var i, o, a, s, u = [],
+                    l = [],
+                    c = t.length,
+                    f = e || function(e, t, n) {
+                        for (var r = 0, i = t.length; r < i; r++) I(e, t[r], n);
+                        return n
+                    }(h || "*", n.nodeType ? [n] : n, []),
+                    p = !d || !e && h ? f : Z(f, u, d, n, r);
+                if (g ? g(p, s = y || (e ? d : c || v) ? [] : t, n, r) : s = p, v) {
+                    i = Z(s, l), v(i, [], n, r), o = i.length;
+                    while (o--)(a = i[o]) && (s[l[o]] = !(p[l[o]] = a))
+                }
+                if (e) {
+                    if (y || d) {
+                        if (y) {
+                            i = [], o = s.length;
+                            while (o--)(a = s[o]) && i.push(p[o] = a);
+                            y(null, s = [], i, r)
+                        }
+                        o = s.length;
+                        while (o--)(a = s[o]) && -1 < (i = y ? se.call(e, a) : u[o]) && (e[i] = !(t[i] = a))
+                    }
+                } else s = Z(s === t ? s.splice(c, s.length) : s), y ? y(null, t, s, r) : k.apply(t, s)
+            })
+        }
+
+        function te(e) {
+            for (var i, t, n, r = e.length, o = b.relative[e[0].type], a = o || b.relative[" "], s = o ? 1 : 0, u = J(function(e) {
+                    return e === i
+                }, a, !0), l = J(function(e) {
+                    return -1 < se.call(i, e)
+                }, a, !0), c = [function(e, t, n) {
+                    var r = !o && (n || t != w) || ((i = t).nodeType ? u(e, t, n) : l(e, t, n));
+                    return i = null, r
+                }]; s < r; s++)
+                if (t = b.relative[e[s].type]) c = [J(K(c), t)];
+                else {
+                    if ((t = b.filter[e[s].type].apply(null, e[s].matches))[S]) {
+                        for (n = ++s; n < r; n++)
+                            if (b.relative[e[n].type]) break;
+                        return ee(1 < s && K(c), 1 < s && Q(e.slice(0, s - 1).concat({
+                            value: " " === e[s - 2].type ? "*" : ""
+                        })).replace(ve, "$1"), t, s < n && te(e.slice(s, n)), n < r && te(e = e.slice(n)), n < r && Q(e))
+                    }
+                    c.push(t)
+                } return K(c)
+        }
+
+        function ne(e, t) {
+            var n, v, y, m, x, r, i = [],
+                o = [],
+                a = u[e + " "];
+            if (!a) {
+                t || (t = Y(e)), n = t.length;
+                while (n--)(a = te(t[n]))[S] ? i.push(a) : o.push(a);
+                (a = u(e, (v = o, m = 0 < (y = i).length, x = 0 < v.length, r = function(e, t, n, r, i) {
+                    var o, a, s, u = 0,
+                        l = "0",
+                        c = e && [],
+                        f = [],
+                        p = w,
+                        d = e || x && b.find.TAG("*", i),
+                        h = E += null == p ? 1 : Math.random() || .1,
+                        g = d.length;
+                    for (i && (w = t == T || t || i); l !== g && null != (o = d[l]); l++) {
+                        if (x && o) {
+                            a = 0, t || o.ownerDocument == T || (V(o), n = !C);
+                            while (s = v[a++])
+                                if (s(o, t || T, n)) {
+                                    k.call(r, o);
+                                    break
+                                } i && (E = h)
+                        }
+                        m && ((o = !s && o) && u--, e && c.push(o))
+                    }
+                    if (u += l, m && l !== u) {
+                        a = 0;
+                        while (s = y[a++]) s(c, f, t, n);
+                        if (e) {
+                            if (0 < u)
+                                while (l--) c[l] || f[l] || (f[l] = pe.call(r));
+                            f = Z(f)
+                        }
+                        k.apply(r, f), i && !e && 0 < f.length && 1 < u + y.length && ce.uniqueSort(r)
+                    }
+                    return i && (E = h, w = p), c
+                }, m ? F(r) : r))).selector = e
+            }
+            return a
+        }
+
+        function re(e, t, n, r) {
+            var i, o, a, s, u, l = "function" == typeof e && e,
+                c = !r && Y(e = l.selector || e);
+            if (n = n || [], 1 === c.length) {
+                if (2 < (o = c[0] = c[0].slice(0)).length && "ID" === (a = o[0]).type && 9 === t.nodeType && C && b.relative[o[1].type]) {
+                    if (!(t = (b.find.ID(a.matches[0].replace(O, P), t) || [])[0])) return n;
+                    l && (t = t.parentNode), e = e.slice(o.shift().value.length)
+                }
+                i = D.needsContext.test(e) ? 0 : o.length;
+                while (i--) {
+                    if (a = o[i], b.relative[s = a.type]) break;
+                    if ((u = b.find[s]) && (r = u(a.matches[0].replace(O, P), H.test(o[0].type) && U(t.parentNode) || t))) {
+                        if (o.splice(i, 1), !(e = r.length && Q(o))) return k.apply(n, r), n;
+                        break
+                    }
+                }
+            }
+            return (l || ne(e, c))(r, t, !C, n, !t || H.test(e) && U(t.parentNode) || t), n
+        }
+        G.prototype = b.filters = b.pseudos, b.setFilters = new G, le.sortStable = S.split("").sort(l).join("") === S, V(), le.sortDetached = $(function(e) {
+            return 1 & e.compareDocumentPosition(T.createElement("fieldset"))
+        }), ce.find = I, ce.expr[":"] = ce.expr.pseudos, ce.unique = ce.uniqueSort, I.compile = ne, I.select = re, I.setDocument = V, I.tokenize = Y, I.escape = ce.escapeSelector, I.getText = ce.text, I.isXML = ce.isXMLDoc, I.selectors = ce.expr, I.support = ce.support, I.uniqueSort = ce.uniqueSort
+    }();
+    var d = function(e, t, n) {
+            var r = [],
+                i = void 0 !== n;
+            while ((e = e[t]) && 9 !== e.nodeType)
+                if (1 === e.nodeType) {
+                    if (i && ce(e).is(n)) break;
+                    r.push(e)
+                } return r
+        },
+        h = function(e, t) {
+            for (var n = []; e; e = e.nextSibling) 1 === e.nodeType && e !== t && n.push(e);
+            return n
+        },
+        b = ce.expr.match.needsContext,
+        w = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
+
+    function T(e, n, r) {
+        return v(n) ? ce.grep(e, function(e, t) {
+            return !!n.call(e, t, e) !== r
+        }) : n.nodeType ? ce.grep(e, function(e) {
+            return e === n !== r
+        }) : "string" != typeof n ? ce.grep(e, function(e) {
+            return -1 < se.call(n, e) !== r
+        }) : ce.filter(n, e, r)
+    }
+    ce.filter = function(e, t, n) {
+        var r = t[0];
+        return n && (e = ":not(" + e + ")"), 1 === t.length && 1 === r.nodeType ? ce.find.matchesSelector(r, e) ? [r] : [] : ce.find.matches(e, ce.grep(t, function(e) {
+            return 1 === e.nodeType
+        }))
+    }, ce.fn.extend({
+        find: function(e) {
+            var t, n, r = this.length,
+                i = this;
+            if ("string" != typeof e) return this.pushStack(ce(e).filter(function() {
+                for (t = 0; t < r; t++)
+                    if (ce.contains(i[t], this)) return !0
+            }));
+            for (n = this.pushStack([]), t = 0; t < r; t++) ce.find(e, i[t], n);
+            return 1 < r ? ce.uniqueSort(n) : n
+        },
+        filter: function(e) {
+            return this.pushStack(T(this, e || [], !1))
+        },
+        not: function(e) {
+            return this.pushStack(T(this, e || [], !0))
+        },
+        is: function(e) {
+            return !!T(this, "string" == typeof e && b.test(e) ? ce(e) : e || [], !1).length
+        }
+    });
+    var k, S = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
+    (ce.fn.init = function(e, t, n) {
+        var r, i;
+        if (!e) return this;
+        if (n = n || k, "string" == typeof e) {
+            if (!(r = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : S.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
+            if (r[1]) {
+                if (t = t instanceof ce ? t[0] : t, ce.merge(this, ce.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : C, !0)), w.test(r[1]) && ce.isPlainObject(t))
+                    for (r in t) v(this[r]) ? this[r](t[r]) : this.attr(r, t[r]);
+                return this
+            }
+            return (i = C.getElementById(r[2])) && (this[0] = i, this.length = 1), this
+        }
+        return e.nodeType ? (this[0] = e, this.length = 1, this) : v(e) ? void 0 !== n.ready ? n.ready(e) : e(ce) : ce.makeArray(e, this)
+    }).prototype = ce.fn, k = ce(C);
+    var E = /^(?:parents|prev(?:Until|All))/,
+        j = {
+            children: !0,
+            contents: !0,
+            next: !0,
+            prev: !0
+        };
+
+    function A(e, t) {
+        while ((e = e[t]) && 1 !== e.nodeType);
+        return e
+    }
+    ce.fn.extend({
+        has: function(e) {
+            var t = ce(e, this),
+                n = t.length;
+            return this.filter(function() {
+                for (var e = 0; e < n; e++)
+                    if (ce.contains(this, t[e])) return !0
+            })
+        },
+        closest: function(e, t) {
+            var n, r = 0,
+                i = this.length,
+                o = [],
+                a = "string" != typeof e && ce(e);
+            if (!b.test(e))
+                for (; r < i; r++)
+                    for (n = this[r]; n && n !== t; n = n.parentNode)
+                        if (n.nodeType < 11 && (a ? -1 < a.index(n) : 1 === n.nodeType && ce.find.matchesSelector(n, e))) {
+                            o.push(n);
+                            break
+                        } return this.pushStack(1 < o.length ? ce.uniqueSort(o) : o)
+        },
+        index: function(e) {
+            return e ? "string" == typeof e ? se.call(ce(e), this[0]) : se.call(this, e.jquery ? e[0] : e) : this[0] && this[0].parentNode ? this.first().prevAll().length : -1
+        },
+        add: function(e, t) {
+            return this.pushStack(ce.uniqueSort(ce.merge(this.get(), ce(e, t))))
+        },
+        addBack: function(e) {
+            return this.add(null == e ? this.prevObject : this.prevObject.filter(e))
+        }
+    }), ce.each({
+        parent: function(e) {
+            var t = e.parentNode;
+            return t && 11 !== t.nodeType ? t : null
+        },
+        parents: function(e) {
+            return d(e, "parentNode")
+        },
+        parentsUntil: function(e, t, n) {
+            return d(e, "parentNode", n)
+        },
+        next: function(e) {
+            return A(e, "nextSibling")
+        },
+        prev: function(e) {
+            return A(e, "previousSibling")
+        },
+        nextAll: function(e) {
+            return d(e, "nextSibling")
+        },
+        prevAll: function(e) {
+            return d(e, "previousSibling")
+        },
+        nextUntil: function(e, t, n) {
+            return d(e, "nextSibling", n)
+        },
+        prevUntil: function(e, t, n) {
+            return d(e, "previousSibling", n)
+        },
+        siblings: function(e) {
+            return h((e.parentNode || {}).firstChild, e)
+        },
+        children: function(e) {
+            return h(e.firstChild)
+        },
+        contents: function(e) {
+            return null != e.contentDocument && r(e.contentDocument) ? e.contentDocument : (fe(e, "template") && (e = e.content || e), ce.merge([], e.childNodes))
+        }
+    }, function(r, i) {
+        ce.fn[r] = function(e, t) {
+            var n = ce.map(this, i, e);
+            return "Until" !== r.slice(-5) && (t = e), t && "string" == typeof t && (n = ce.filter(t, n)), 1 < this.length && (j[r] || ce.uniqueSort(n), E.test(r) && n.reverse()), this.pushStack(n)
+        }
+    });
+    var D = /[^\x20\t\r\n\f]+/g;
+
+    function N(e) {
+        return e
+    }
+
+    function q(e) {
+        throw e
+    }
+
+    function L(e, t, n, r) {
+        var i;
+        try {
+            e && v(i = e.promise) ? i.call(e).done(t).fail(n) : e && v(i = e.then) ? i.call(e, t, n) : t.apply(void 0, [e].slice(r))
+        } catch (e) {
+            n.apply(void 0, [e])
+        }
+    }
+    ce.Callbacks = function(r) {
+        var e, n;
+        r = "string" == typeof r ? (e = r, n = {}, ce.each(e.match(D) || [], function(e, t) {
+            n[t] = !0
+        }), n) : ce.extend({}, r);
+        var i, t, o, a, s = [],
+            u = [],
+            l = -1,
+            c = function() {
+                for (a = a || r.once, o = i = !0; u.length; l = -1) {
+                    t = u.shift();
+                    while (++l < s.length) !1 === s[l].apply(t[0], t[1]) && r.stopOnFalse && (l = s.length, t = !1)
+                }
+                r.memory || (t = !1), i = !1, a && (s = t ? [] : "")
+            },
+            f = {
+                add: function() {
+                    return s && (t && !i && (l = s.length - 1, u.push(t)), function n(e) {
+                        ce.each(e, function(e, t) {
+                            v(t) ? r.unique && f.has(t) || s.push(t) : t && t.length && "string" !== x(t) && n(t)
+                        })
+                    }(arguments), t && !i && c()), this
+                },
+                remove: function() {
+                    return ce.each(arguments, function(e, t) {
+                        var n;
+                        while (-1 < (n = ce.inArray(t, s, n))) s.splice(n, 1), n <= l && l--
+                    }), this
+                },
+                has: function(e) {
+                    return e ? -1 < ce.inArray(e, s) : 0 < s.length
+                },
+                empty: function() {
+                    return s && (s = []), this
+                },
+                disable: function() {
+                    return a = u = [], s = t = "", this
+                },
+                disabled: function() {
+                    return !s
+                },
+                lock: function() {
+                    return a = u = [], t || i || (s = t = ""), this
+                },
+                locked: function() {
+                    return !!a
+                },
+                fireWith: function(e, t) {
+                    return a || (t = [e, (t = t || []).slice ? t.slice() : t], u.push(t), i || c()), this
+                },
+                fire: function() {
+                    return f.fireWith(this, arguments), this
+                },
+                fired: function() {
+                    return !!o
+                }
+            };
+        return f
+    }, ce.extend({
+        Deferred: function(e) {
+            var o = [
+                    ["notify", "progress", ce.Callbacks("memory"), ce.Callbacks("memory"), 2],
+                    ["resolve", "done", ce.Callbacks("once memory"), ce.Callbacks("once memory"), 0, "resolved"],
+                    ["reject", "fail", ce.Callbacks("once memory"), ce.Callbacks("once memory"), 1, "rejected"]
+                ],
+                i = "pending",
+                a = {
+                    state: function() {
+                        return i
+                    },
+                    always: function() {
+                        return s.done(arguments).fail(arguments), this
+                    },
+                    "catch": function(e) {
+                        return a.then(null, e)
+                    },
+                    pipe: function() {
+                        var i = arguments;
+                        return ce.Deferred(function(r) {
+                            ce.each(o, function(e, t) {
+                                var n = v(i[t[4]]) && i[t[4]];
+                                s[t[1]](function() {
+                                    var e = n && n.apply(this, arguments);
+                                    e && v(e.promise) ? e.promise().progress(r.notify).done(r.resolve).fail(r.reject) : r[t[0] + "With"](this, n ? [e] : arguments)
+                                })
+                            }), i = null
+                        }).promise()
+                    },
+                    then: function(t, n, r) {
+                        var u = 0;
+
+                        function l(i, o, a, s) {
+                            return function() {
+                                var n = this,
+                                    r = arguments,
+                                    e = function() {
+                                        var e, t;
+                                        if (!(i < u)) {
+                                            if ((e = a.apply(n, r)) === o.promise()) throw new TypeError("Thenable self-resolution");
+                                            t = e && ("object" == typeof e || "function" == typeof e) && e.then, v(t) ? s ? t.call(e, l(u, o, N, s), l(u, o, q, s)) : (u++, t.call(e, l(u, o, N, s), l(u, o, q, s), l(u, o, N, o.notifyWith))) : (a !== N && (n = void 0, r = [e]), (s || o.resolveWith)(n, r))
+                                        }
+                                    },
+                                    t = s ? e : function() {
+                                        try {
+                                            e()
+                                        } catch (e) {
+                                            ce.Deferred.exceptionHook && ce.Deferred.exceptionHook(e, t.error), u <= i + 1 && (a !== q && (n = void 0, r = [e]), o.rejectWith(n, r))
+                                        }
+                                    };
+                                i ? t() : (ce.Deferred.getErrorHook ? t.error = ce.Deferred.getErrorHook() : ce.Deferred.getStackHook && (t.error = ce.Deferred.getStackHook()), ie.setTimeout(t))
+                            }
+                        }
+                        return ce.Deferred(function(e) {
+                            o[0][3].add(l(0, e, v(r) ? r : N, e.notifyWith)), o[1][3].add(l(0, e, v(t) ? t : N)), o[2][3].add(l(0, e, v(n) ? n : q))
+                        }).promise()
+                    },
+                    promise: function(e) {
+                        return null != e ? ce.extend(e, a) : a
+                    }
+                },
+                s = {};
+            return ce.each(o, function(e, t) {
+                var n = t[2],
+                    r = t[5];
+                a[t[1]] = n.add, r && n.add(function() {
+                    i = r
+                }, o[3 - e][2].disable, o[3 - e][3].disable, o[0][2].lock, o[0][3].lock), n.add(t[3].fire), s[t[0]] = function() {
+                    return s[t[0] + "With"](this === s ? void 0 : this, arguments), this
+                }, s[t[0] + "With"] = n.fireWith
+            }), a.promise(s), e && e.call(s, s), s
+        },
+        when: function(e) {
+            var n = arguments.length,
+                t = n,
+                r = Array(t),
+                i = ae.call(arguments),
+                o = ce.Deferred(),
+                a = function(t) {
+                    return function(e) {
+                        r[t] = this, i[t] = 1 < arguments.length ? ae.call(arguments) : e, --n || o.resolveWith(r, i)
+                    }
+                };
+            if (n <= 1 && (L(e, o.done(a(t)).resolve, o.reject, !n), "pending" === o.state() || v(i[t] && i[t].then))) return o.then();
+            while (t--) L(i[t], a(t), o.reject);
+            return o.promise()
+        }
+    });
+    var H = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
+    ce.Deferred.exceptionHook = function(e, t) {
+        ie.console && ie.console.warn && e && H.test(e.name) && ie.console.warn("jQuery.Deferred exception: " + e.message, e.stack, t)
+    }, ce.readyException = function(e) {
+        ie.setTimeout(function() {
+            throw e
+        })
+    };
+    var O = ce.Deferred();
+
+    function P() {
+        C.removeEventListener("DOMContentLoaded", P), ie.removeEventListener("load", P), ce.ready()
+    }
+    ce.fn.ready = function(e) {
+        return O.then(e)["catch"](function(e) {
+            ce.readyException(e)
+        }), this
+    }, ce.extend({
+        isReady: !1,
+        readyWait: 1,
+        ready: function(e) {
+            (!0 === e ? --ce.readyWait : ce.isReady) || (ce.isReady = !0) !== e && 0 < --ce.readyWait || O.resolveWith(C, [ce])
+        }
+    }), ce.ready.then = O.then, "complete" === C.readyState || "loading" !== C.readyState && !C.documentElement.doScroll ? ie.setTimeout(ce.ready) : (C.addEventListener("DOMContentLoaded", P), ie.addEventListener("load", P));
+    var M = function(e, t, n, r, i, o, a) {
+            var s = 0,
+                u = e.length,
+                l = null == n;
+            if ("object" === x(n))
+                for (s in i = !0, n) M(e, t, s, n[s], !0, o, a);
+            else if (void 0 !== r && (i = !0, v(r) || (a = !0), l && (a ? (t.call(e, r), t = null) : (l = t, t = function(e, t, n) {
+                    return l.call(ce(e), n)
+                })), t))
+                for (; s < u; s++) t(e[s], n, a ? r : r.call(e[s], s, t(e[s], n)));
+            return i ? e : l ? t.call(e) : u ? t(e[0], n) : o
+        },
+        R = /^-ms-/,
+        I = /-([a-z])/g;
+
+    function W(e, t) {
+        return t.toUpperCase()
+    }
+
+    function F(e) {
+        return e.replace(R, "ms-").replace(I, W)
+    }
+    var $ = function(e) {
+        return 1 === e.nodeType || 9 === e.nodeType || !+e.nodeType
+    };
+
+    function B() {
+        this.expando = ce.expando + B.uid++
+    }
+    B.uid = 1, B.prototype = {
+        cache: function(e) {
+            var t = e[this.expando];
+            return t || (t = {}, $(e) && (e.nodeType ? e[this.expando] = t : Object.defineProperty(e, this.expando, {
+                value: t,
+                configurable: !0
+            }))), t
+        },
+        set: function(e, t, n) {
+            var r, i = this.cache(e);
+            if ("string" == typeof t) i[F(t)] = n;
+            else
+                for (r in t) i[F(r)] = t[r];
+            return i
+        },
+        get: function(e, t) {
+            return void 0 === t ? this.cache(e) : e[this.expando] && e[this.expando][F(t)]
+        },
+        access: function(e, t, n) {
+            return void 0 === t || t && "string" == typeof t && void 0 === n ? this.get(e, t) : (this.set(e, t, n), void 0 !== n ? n : t)
+        },
+        remove: function(e, t) {
+            var n, r = e[this.expando];
+            if (void 0 !== r) {
+                if (void 0 !== t) {
+                    n = (t = Array.isArray(t) ? t.map(F) : (t = F(t)) in r ? [t] : t.match(D) || []).length;
+                    while (n--) delete r[t[n]]
+                }(void 0 === t || ce.isEmptyObject(r)) && (e.nodeType ? e[this.expando] = void 0 : delete e[this.expando])
+            }
+        },
+        hasData: function(e) {
+            var t = e[this.expando];
+            return void 0 !== t && !ce.isEmptyObject(t)
+        }
+    };
+    var _ = new B,
+        z = new B,
+        X = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
+        U = /[A-Z]/g;
+
+    function V(e, t, n) {
+        var r, i;
+        if (void 0 === n && 1 === e.nodeType)
+            if (r = "data-" + t.replace(U, "-$&").toLowerCase(), "string" == typeof(n = e.getAttribute(r))) {
+                try {
+                    n = "true" === (i = n) || "false" !== i && ("null" === i ? null : i === +i + "" ? +i : X.test(i) ? JSON.parse(i) : i)
+                } catch (e) {}
+                z.set(e, t, n)
+            } else n = void 0;
+        return n
+    }
+    ce.extend({
+        hasData: function(e) {
+            return z.hasData(e) || _.hasData(e)
+        },
+        data: function(e, t, n) {
+            return z.access(e, t, n)
+        },
+        removeData: function(e, t) {
+            z.remove(e, t)
+        },
+        _data: function(e, t, n) {
+            return _.access(e, t, n)
+        },
+        _removeData: function(e, t) {
+            _.remove(e, t)
+        }
+    }), ce.fn.extend({
+        data: function(n, e) {
+            var t, r, i, o = this[0],
+                a = o && o.attributes;
+            if (void 0 === n) {
+                if (this.length && (i = z.get(o), 1 === o.nodeType && !_.get(o, "hasDataAttrs"))) {
+                    t = a.length;
+                    while (t--) a[t] && 0 === (r = a[t].name).indexOf("data-") && (r = F(r.slice(5)), V(o, r, i[r]));
+                    _.set(o, "hasDataAttrs", !0)
+                }
+                return i
+            }
+            return "object" == typeof n ? this.each(function() {
+                z.set(this, n)
+            }) : M(this, function(e) {
+                var t;
+                if (o && void 0 === e) return void 0 !== (t = z.get(o, n)) ? t : void 0 !== (t = V(o, n)) ? t : void 0;
+                this.each(function() {
+                    z.set(this, n, e)
+                })
+            }, null, e, 1 < arguments.length, null, !0)
+        },
+        removeData: function(e) {
+            return this.each(function() {
+                z.remove(this, e)
+            })
+        }
+    }), ce.extend({
+        queue: function(e, t, n) {
+            var r;
+            if (e) return t = (t || "fx") + "queue", r = _.get(e, t), n && (!r || Array.isArray(n) ? r = _.access(e, t, ce.makeArray(n)) : r.push(n)), r || []
+        },
+        dequeue: function(e, t) {
+            t = t || "fx";
+            var n = ce.queue(e, t),
+                r = n.length,
+                i = n.shift(),
+                o = ce._queueHooks(e, t);
+            "inprogress" === i && (i = n.shift(), r--), i && ("fx" === t && n.unshift("inprogress"), delete o.stop, i.call(e, function() {
+                ce.dequeue(e, t)
+            }, o)), !r && o && o.empty.fire()
+        },
+        _queueHooks: function(e, t) {
+            var n = t + "queueHooks";
+            return _.get(e, n) || _.access(e, n, {
+                empty: ce.Callbacks("once memory").add(function() {
+                    _.remove(e, [t + "queue", n])
+                })
+            })
+        }
+    }), ce.fn.extend({
+        queue: function(t, n) {
+            var e = 2;
+            return "string" != typeof t && (n = t, t = "fx", e--), arguments.length < e ? ce.queue(this[0], t) : void 0 === n ? this : this.each(function() {
+                var e = ce.queue(this, t, n);
+                ce._queueHooks(this, t), "fx" === t && "inprogress" !== e[0] && ce.dequeue(this, t)
+            })
+        },
+        dequeue: function(e) {
+            return this.each(function() {
+                ce.dequeue(this, e)
+            })
+        },
+        clearQueue: function(e) {
+            return this.queue(e || "fx", [])
+        },
+        promise: function(e, t) {
+            var n, r = 1,
+                i = ce.Deferred(),
+                o = this,
+                a = this.length,
+                s = function() {
+                    --r || i.resolveWith(o, [o])
+                };
+            "string" != typeof e && (t = e, e = void 0), e = e || "fx";
+            while (a--)(n = _.get(o[a], e + "queueHooks")) && n.empty && (r++, n.empty.add(s));
+            return s(), i.promise(t)
+        }
+    });
+    var G = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
+        Y = new RegExp("^(?:([+-])=|)(" + G + ")([a-z%]*)$", "i"),
+        Q = ["Top", "Right", "Bottom", "Left"],
+        J = C.documentElement,
+        K = function(e) {
+            return ce.contains(e.ownerDocument, e)
+        },
+        Z = {
+            composed: !0
+        };
+    J.getRootNode && (K = function(e) {
+        return ce.contains(e.ownerDocument, e) || e.getRootNode(Z) === e.ownerDocument
+    });
+    var ee = function(e, t) {
+        return "none" === (e = t || e).style.display || "" === e.style.display && K(e) && "none" === ce.css(e, "display")
+    };
+
+    function te(e, t, n, r) {
+        var i, o, a = 20,
+            s = r ? function() {
+                return r.cur()
+            } : function() {
+                return ce.css(e, t, "")
+            },
+            u = s(),
+            l = n && n[3] || (ce.cssNumber[t] ? "" : "px"),
+            c = e.nodeType && (ce.cssNumber[t] || "px" !== l && +u) && Y.exec(ce.css(e, t));
+        if (c && c[3] !== l) {
+            u /= 2, l = l || c[3], c = +u || 1;
+            while (a--) ce.style(e, t, c + l), (1 - o) * (1 - (o = s() / u || .5)) <= 0 && (a = 0), c /= o;
+            c *= 2, ce.style(e, t, c + l), n = n || []
+        }
+        return n && (c = +c || +u || 0, i = n[1] ? c + (n[1] + 1) * n[2] : +n[2], r && (r.unit = l, r.start = c, r.end = i)), i
+    }
+    var ne = {};
+
+    function re(e, t) {
+        for (var n, r, i, o, a, s, u, l = [], c = 0, f = e.length; c < f; c++)(r = e[c]).style && (n = r.style.display, t ? ("none" === n && (l[c] = _.get(r, "display") || null, l[c] || (r.style.display = "")), "" === r.style.display && ee(r) && (l[c] = (u = a = o = void 0, a = (i = r).ownerDocument, s = i.nodeName, (u = ne[s]) || (o = a.body.appendChild(a.createElement(s)), u = ce.css(o, "display"), o.parentNode.removeChild(o), "none" === u && (u = "block"), ne[s] = u)))) : "none" !== n && (l[c] = "none", _.set(r, "display", n)));
+        for (c = 0; c < f; c++) null != l[c] && (e[c].style.display = l[c]);
+        return e
+    }
+    ce.fn.extend({
+        show: function() {
+            return re(this, !0)
+        },
+        hide: function() {
+            return re(this)
+        },
+        toggle: function(e) {
+            return "boolean" == typeof e ? e ? this.show() : this.hide() : this.each(function() {
+                ee(this) ? ce(this).show() : ce(this).hide()
+            })
+        }
+    });
+    var xe, be, we = /^(?:checkbox|radio)$/i,
+        Te = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
+        Ce = /^$|^module$|\/(?:java|ecma)script/i;
+    xe = C.createDocumentFragment().appendChild(C.createElement("div")), (be = C.createElement("input")).setAttribute("type", "radio"), be.setAttribute("checked", "checked"), be.setAttribute("name", "t"), xe.appendChild(be), le.checkClone = xe.cloneNode(!0).cloneNode(!0).lastChild.checked, xe.innerHTML = "<textarea>x</textarea>", le.noCloneChecked = !!xe.cloneNode(!0).lastChild.defaultValue, xe.innerHTML = "<option></option>", le.option = !!xe.lastChild;
+    var ke = {
+        thead: [1, "<table>", "</table>"],
+        col: [2, "<table><colgroup>", "</colgroup></table>"],
+        tr: [2, "<table><tbody>", "</tbody></table>"],
+        td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
+        _default: [0, "", ""]
+    };
+
+    function Se(e, t) {
+        var n;
+        return n = "undefined" != typeof e.getElementsByTagName ? e.getElementsByTagName(t || "*") : "undefined" != typeof e.querySelectorAll ? e.querySelectorAll(t || "*") : [], void 0 === t || t && fe(e, t) ? ce.merge([e], n) : n
+    }
+
+    function Ee(e, t) {
+        for (var n = 0, r = e.length; n < r; n++) _.set(e[n], "globalEval", !t || _.get(t[n], "globalEval"))
+    }
+    ke.tbody = ke.tfoot = ke.colgroup = ke.caption = ke.thead, ke.th = ke.td, le.option || (ke.optgroup = ke.option = [1, "<select multiple='multiple'>", "</select>"]);
+    var je = /<|&#?\w+;/;
+
+    function Ae(e, t, n, r, i) {
+        for (var o, a, s, u, l, c, f = t.createDocumentFragment(), p = [], d = 0, h = e.length; d < h; d++)
+            if ((o = e[d]) || 0 === o)
+                if ("object" === x(o)) ce.merge(p, o.nodeType ? [o] : o);
+                else if (je.test(o)) {
+            a = a || f.appendChild(t.createElement("div")), s = (Te.exec(o) || ["", ""])[1].toLowerCase(), u = ke[s] || ke._default, a.innerHTML = u[1] + ce.htmlPrefilter(o) + u[2], c = u[0];
+            while (c--) a = a.lastChild;
+            ce.merge(p, a.childNodes), (a = f.firstChild).textContent = ""
+        } else p.push(t.createTextNode(o));
+        f.textContent = "", d = 0;
+        while (o = p[d++])
+            if (r && -1 < ce.inArray(o, r)) i && i.push(o);
+            else if (l = K(o), a = Se(f.appendChild(o), "script"), l && Ee(a), n) {
+            c = 0;
+            while (o = a[c++]) Ce.test(o.type || "") && n.push(o)
+        }
+        return f
+    }
+    var De = /^([^.]*)(?:\.(.+)|)/;
+
+    function Ne() {
+        return !0
+    }
+
+    function qe() {
+        return !1
+    }
+
+    function Le(e, t, n, r, i, o) {
+        var a, s;
+        if ("object" == typeof t) {
+            for (s in "string" != typeof n && (r = r || n, n = void 0), t) Le(e, s, n, r, t[s], o);
+            return e
+        }
+        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = qe;
+        else if (!i) return e;
+        return 1 === o && (a = i, (i = function(e) {
+            return ce().off(e), a.apply(this, arguments)
+        }).guid = a.guid || (a.guid = ce.guid++)), e.each(function() {
+            ce.event.add(this, t, i, r, n)
+        })
+    }
+
+    function He(e, r, t) {
+        t ? (_.set(e, r, !1), ce.event.add(e, r, {
+            namespace: !1,
+            handler: function(e) {
+                var t, n = _.get(this, r);
+                if (1 & e.isTrigger && this[r]) {
+                    if (n)(ce.event.special[r] || {}).delegateType && e.stopPropagation();
+                    else if (n = ae.call(arguments), _.set(this, r, n), this[r](), t = _.get(this, r), _.set(this, r, !1), n !== t) return e.stopImmediatePropagation(), e.preventDefault(), t
+                } else n && (_.set(this, r, ce.event.trigger(n[0], n.slice(1), this)), e.stopPropagation(), e.isImmediatePropagationStopped = Ne)
+            }
+        })) : void 0 === _.get(e, r) && ce.event.add(e, r, Ne)
+    }
+    ce.event = {
+        global: {},
+        add: function(t, e, n, r, i) {
+            var o, a, s, u, l, c, f, p, d, h, g, v = _.get(t);
+            if ($(t)) {
+                n.handler && (n = (o = n).handler, i = o.selector), i && ce.find.matchesSelector(J, i), n.guid || (n.guid = ce.guid++), (u = v.events) || (u = v.events = Object.create(null)), (a = v.handle) || (a = v.handle = function(e) {
+                    return "undefined" != typeof ce && ce.event.triggered !== e.type ? ce.event.dispatch.apply(t, arguments) : void 0
+                }), l = (e = (e || "").match(D) || [""]).length;
+                while (l--) d = g = (s = De.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = ce.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = ce.event.special[d] || {}, c = ce.extend({
+                    type: d,
+                    origType: g,
+                    data: r,
+                    handler: n,
+                    guid: n.guid,
+                    selector: i,
+                    needsContext: i && ce.expr.match.needsContext.test(i),
+                    namespace: h.join(".")
+                }, o), (p = u[d]) || ((p = u[d] = []).delegateCount = 0, f.setup && !1 !== f.setup.call(t, r, h, a) || t.addEventListener && t.addEventListener(d, a)), f.add && (f.add.call(t, c), c.handler.guid || (c.handler.guid = n.guid)), i ? p.splice(p.delegateCount++, 0, c) : p.push(c), ce.event.global[d] = !0)
+            }
+        },
+        remove: function(e, t, n, r, i) {
+            var o, a, s, u, l, c, f, p, d, h, g, v = _.hasData(e) && _.get(e);
+            if (v && (u = v.events)) {
+                l = (t = (t || "").match(D) || [""]).length;
+                while (l--)
+                    if (d = g = (s = De.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
+                        f = ce.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length;
+                        while (o--) c = p[o], !i && g !== c.origType || n && n.guid !== c.guid || s && !s.test(c.namespace) || r && r !== c.selector && ("**" !== r || !c.selector) || (p.splice(o, 1), c.selector && p.delegateCount--, f.remove && f.remove.call(e, c));
+                        a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, v.handle) || ce.removeEvent(e, d, v.handle), delete u[d])
+                    } else
+                        for (d in u) ce.event.remove(e, d + t[l], n, r, !0);
+                ce.isEmptyObject(u) && _.remove(e, "handle events")
+            }
+        },
+        dispatch: function(e) {
+            var t, n, r, i, o, a, s = new Array(arguments.length),
+                u = ce.event.fix(e),
+                l = (_.get(this, "events") || Object.create(null))[u.type] || [],
+                c = ce.event.special[u.type] || {};
+            for (s[0] = u, t = 1; t < arguments.length; t++) s[t] = arguments[t];
+            if (u.delegateTarget = this, !c.preDispatch || !1 !== c.preDispatch.call(this, u)) {
+                a = ce.event.handlers.call(this, u, l), t = 0;
+                while ((i = a[t++]) && !u.isPropagationStopped()) {
+                    u.currentTarget = i.elem, n = 0;
+                    while ((o = i.handlers[n++]) && !u.isImmediatePropagationStopped()) u.rnamespace && !1 !== o.namespace && !u.rnamespace.test(o.namespace) || (u.handleObj = o, u.data = o.data, void 0 !== (r = ((ce.event.special[o.origType] || {}).handle || o.handler).apply(i.elem, s)) && !1 === (u.result = r) && (u.preventDefault(), u.stopPropagation()))
+                }
+                return c.postDispatch && c.postDispatch.call(this, u), u.result
+            }
+        },
+        handlers: function(e, t) {
+            var n, r, i, o, a, s = [],
+                u = t.delegateCount,
+                l = e.target;
+            if (u && l.nodeType && !("click" === e.type && 1 <= e.button))
+                for (; l !== this; l = l.parentNode || this)
+                    if (1 === l.nodeType && ("click" !== e.type || !0 !== l.disabled)) {
+                        for (o = [], a = {}, n = 0; n < u; n++) void 0 === a[i = (r = t[n]).selector + " "] && (a[i] = r.needsContext ? -1 < ce(i, this).index(l) : ce.find(i, this, null, [l]).length), a[i] && o.push(r);
+                        o.length && s.push({
+                            elem: l,
+                            handlers: o
+                        })
+                    } return l = this, u < t.length && s.push({
+                elem: l,
+                handlers: t.slice(u)
+            }), s
+        },
+        addProp: function(t, e) {
+            Object.defineProperty(ce.Event.prototype, t, {
+                enumerable: !0,
+                configurable: !0,
+                get: v(e) ? function() {
+                    if (this.originalEvent) return e(this.originalEvent)
+                } : function() {
+                    if (this.originalEvent) return this.originalEvent[t]
+                },
+                set: function(e) {
+                    Object.defineProperty(this, t, {
+                        enumerable: !0,
+                        configurable: !0,
+                        writable: !0,
+                        value: e
+                    })
+                }
+            })
+        },
+        fix: function(e) {
+            return e[ce.expando] ? e : new ce.Event(e)
+        },
+        special: {
+            load: {
+                noBubble: !0
+            },
+            click: {
+                setup: function(e) {
+                    var t = this || e;
+                    return we.test(t.type) && t.click && fe(t, "input") && He(t, "click", !0), !1
+                },
+                trigger: function(e) {
+                    var t = this || e;
+                    return we.test(t.type) && t.click && fe(t, "input") && He(t, "click"), !0
+                },
+                _default: function(e) {
+                    var t = e.target;
+                    return we.test(t.type) && t.click && fe(t, "input") && _.get(t, "click") || fe(t, "a")
+                }
+            },
+            beforeunload: {
+                postDispatch: function(e) {
+                    void 0 !== e.result && e.originalEvent && (e.originalEvent.returnValue = e.result)
+                }
+            }
+        }
+    }, ce.removeEvent = function(e, t, n) {
+        e.removeEventListener && e.removeEventListener(t, n)
+    }, ce.Event = function(e, t) {
+        if (!(this instanceof ce.Event)) return new ce.Event(e, t);
+        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? Ne : qe, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && ce.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[ce.expando] = !0
+    }, ce.Event.prototype = {
+        constructor: ce.Event,
+        isDefaultPrevented: qe,
+        isPropagationStopped: qe,
+        isImmediatePropagationStopped: qe,
+        isSimulated: !1,
+        preventDefault: function() {
+            var e = this.originalEvent;
+            this.isDefaultPrevented = Ne, e && !this.isSimulated && e.preventDefault()
+        },
+        stopPropagation: function() {
+            var e = this.originalEvent;
+            this.isPropagationStopped = Ne, e && !this.isSimulated && e.stopPropagation()
+        },
+        stopImmediatePropagation: function() {
+            var e = this.originalEvent;
+            this.isImmediatePropagationStopped = Ne, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
+        }
+    }, ce.each({
+        altKey: !0,
+        bubbles: !0,
+        cancelable: !0,
+        changedTouches: !0,
+        ctrlKey: !0,
+        detail: !0,
+        eventPhase: !0,
+        metaKey: !0,
+        pageX: !0,
+        pageY: !0,
+        shiftKey: !0,
+        view: !0,
+        "char": !0,
+        code: !0,
+        charCode: !0,
+        key: !0,
+        keyCode: !0,
+        button: !0,
+        buttons: !0,
+        clientX: !0,
+        clientY: !0,
+        offsetX: !0,
+        offsetY: !0,
+        pointerId: !0,
+        pointerType: !0,
+        screenX: !0,
+        screenY: !0,
+        targetTouches: !0,
+        toElement: !0,
+        touches: !0,
+        which: !0
+    }, ce.event.addProp), ce.each({
+        focus: "focusin",
+        blur: "focusout"
+    }, function(r, i) {
+        function o(e) {
+            if (C.documentMode) {
+                var t = _.get(this, "handle"),
+                    n = ce.event.fix(e);
+                n.type = "focusin" === e.type ? "focus" : "blur", n.isSimulated = !0, t(e), n.target === n.currentTarget && t(n)
+            } else ce.event.simulate(i, e.target, ce.event.fix(e))
+        }
+        ce.event.special[r] = {
+            setup: function() {
+                var e;
+                if (He(this, r, !0), !C.documentMode) return !1;
+                (e = _.get(this, i)) || this.addEventListener(i, o), _.set(this, i, (e || 0) + 1)
+            },
+            trigger: function() {
+                return He(this, r), !0
+            },
+            teardown: function() {
+                var e;
+                if (!C.documentMode) return !1;
+                (e = _.get(this, i) - 1) ? _.set(this, i, e): (this.removeEventListener(i, o), _.remove(this, i))
+            },
+            _default: function(e) {
+                return _.get(e.target, r)
+            },
+            delegateType: i
+        }, ce.event.special[i] = {
+            setup: function() {
+                var e = this.ownerDocument || this.document || this,
+                    t = C.documentMode ? this : e,
+                    n = _.get(t, i);
+                n || (C.documentMode ? this.addEventListener(i, o) : e.addEventListener(r, o, !0)), _.set(t, i, (n || 0) + 1)
+            },
+            teardown: function() {
+                var e = this.ownerDocument || this.document || this,
+                    t = C.documentMode ? this : e,
+                    n = _.get(t, i) - 1;
+                n ? _.set(t, i, n) : (C.documentMode ? this.removeEventListener(i, o) : e.removeEventListener(r, o, !0), _.remove(t, i))
+            }
+        }
+    }), ce.each({
+        mouseenter: "mouseover",
+        mouseleave: "mouseout",
+        pointerenter: "pointerover",
+        pointerleave: "pointerout"
+    }, function(e, i) {
+        ce.event.special[e] = {
+            delegateType: i,
+            bindType: i,
+            handle: function(e) {
+                var t, n = e.relatedTarget,
+                    r = e.handleObj;
+                return n && (n === this || ce.contains(this, n)) || (e.type = r.origType, t = r.handler.apply(this, arguments), e.type = i), t
+            }
+        }
+    }), ce.fn.extend({
+        on: function(e, t, n, r) {
+            return Le(this, e, t, n, r)
+        },
+        one: function(e, t, n, r) {
+            return Le(this, e, t, n, r, 1)
+        },
+        off: function(e, t, n) {
+            var r, i;
+            if (e && e.preventDefault && e.handleObj) return r = e.handleObj, ce(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
+            if ("object" == typeof e) {
+                for (i in e) this.off(i, t, e[i]);
+                return this
+            }
+            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = qe), this.each(function() {
+                ce.event.remove(this, e, n, t)
+            })
+        }
+    });
+    var Oe = /<script|<style|<link/i,
+        Pe = /checked\s*(?:[^=]|=\s*.checked.)/i,
+        Me = /^\s*<!\[CDATA\[|\]\]>\s*$/g;
+
+    function Re(e, t) {
+        return fe(e, "table") && fe(11 !== t.nodeType ? t : t.firstChild, "tr") && ce(e).children("tbody")[0] || e
+    }
+
+    function Ie(e) {
+        return e.type = (null !== e.getAttribute("type")) + "/" + e.type, e
+    }
+
+    function We(e) {
+        return "true/" === (e.type || "").slice(0, 5) ? e.type = e.type.slice(5) : e.removeAttribute("type"), e
+    }
+
+    function Fe(e, t) {
+        var n, r, i, o, a, s;
+        if (1 === t.nodeType) {
+            if (_.hasData(e) && (s = _.get(e).events))
+                for (i in _.remove(t, "handle events"), s)
+                    for (n = 0, r = s[i].length; n < r; n++) ce.event.add(t, i, s[i][n]);
+            z.hasData(e) && (o = z.access(e), a = ce.extend({}, o), z.set(t, a))
+        }
+    }
+
+    function $e(n, r, i, o) {
+        r = g(r);
+        var e, t, a, s, u, l, c = 0,
+            f = n.length,
+            p = f - 1,
+            d = r[0],
+            h = v(d);
+        if (h || 1 < f && "string" == typeof d && !le.checkClone && Pe.test(d)) return n.each(function(e) {
+            var t = n.eq(e);
+            h && (r[0] = d.call(this, e, t.html())), $e(t, r, i, o)
+        });
+        if (f && (t = (e = Ae(r, n[0].ownerDocument, !1, n, o)).firstChild, 1 === e.childNodes.length && (e = t), t || o)) {
+            for (s = (a = ce.map(Se(e, "script"), Ie)).length; c < f; c++) u = e, c !== p && (u = ce.clone(u, !0, !0), s && ce.merge(a, Se(u, "script"))), i.call(n[c], u, c);
+            if (s)
+                for (l = a[a.length - 1].ownerDocument, ce.map(a, We), c = 0; c < s; c++) u = a[c], Ce.test(u.type || "") && !_.access(u, "globalEval") && ce.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? ce._evalUrl && !u.noModule && ce._evalUrl(u.src, {
+                    nonce: u.nonce || u.getAttribute("nonce")
+                }, l) : m(u.textContent.replace(Me, ""), u, l))
+        }
+        return n
+    }
+
+    function Be(e, t, n) {
+        for (var r, i = t ? ce.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || ce.cleanData(Se(r)), r.parentNode && (n && K(r) && Ee(Se(r, "script")), r.parentNode.removeChild(r));
+        return e
+    }
+    ce.extend({
+        htmlPrefilter: function(e) {
+            return e
+        },
+        clone: function(e, t, n) {
+            var r, i, o, a, s, u, l, c = e.cloneNode(!0),
+                f = K(e);
+            if (!(le.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || ce.isXMLDoc(e)))
+                for (a = Se(c), r = 0, i = (o = Se(e)).length; r < i; r++) s = o[r], u = a[r], void 0, "input" === (l = u.nodeName.toLowerCase()) && we.test(s.type) ? u.checked = s.checked : "input" !== l && "textarea" !== l || (u.defaultValue = s.defaultValue);
+            if (t)
+                if (n)
+                    for (o = o || Se(e), a = a || Se(c), r = 0, i = o.length; r < i; r++) Fe(o[r], a[r]);
+                else Fe(e, c);
+            return 0 < (a = Se(c, "script")).length && Ee(a, !f && Se(e, "script")), c
+        },
+        cleanData: function(e) {
+            for (var t, n, r, i = ce.event.special, o = 0; void 0 !== (n = e[o]); o++)
+                if ($(n)) {
+                    if (t = n[_.expando]) {
+                        if (t.events)
+                            for (r in t.events) i[r] ? ce.event.remove(n, r) : ce.removeEvent(n, r, t.handle);
+                        n[_.expando] = void 0
+                    }
+                    n[z.expando] && (n[z.expando] = void 0)
+                }
+        }
+    }), ce.fn.extend({
+        detach: function(e) {
+            return Be(this, e, !0)
+        },
+        remove: function(e) {
+            return Be(this, e)
+        },
+        text: function(e) {
+            return M(this, function(e) {
+                return void 0 === e ? ce.text(this) : this.empty().each(function() {
+                    1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || (this.textContent = e)
+                })
+            }, null, e, arguments.length)
+        },
+        append: function() {
+            return $e(this, arguments, function(e) {
+                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || Re(this, e).appendChild(e)
+            })
+        },
+        prepend: function() {
+            return $e(this, arguments, function(e) {
+                if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
+                    var t = Re(this, e);
+                    t.insertBefore(e, t.firstChild)
+                }
+            })
+        },
+        before: function() {
+            return $e(this, arguments, function(e) {
+                this.parentNode && this.parentNode.insertBefore(e, this)
+            })
+        },
+        after: function() {
+            return $e(this, arguments, function(e) {
+                this.parentNode && this.parentNode.insertBefore(e, this.nextSibling)
+            })
+        },
+        empty: function() {
+            for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (ce.cleanData(Se(e, !1)), e.textContent = "");
+            return this
+        },
+        clone: function(e, t) {
+            return e = null != e && e, t = null == t ? e : t, this.map(function() {
+                return ce.clone(this, e, t)
+            })
+        },
+        html: function(e) {
+            return M(this, function(e) {
+                var t = this[0] || {},
+                    n = 0,
+                    r = this.length;
+                if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
+                if ("string" == typeof e && !Oe.test(e) && !ke[(Te.exec(e) || ["", ""])[1].toLowerCase()]) {
+                    e = ce.htmlPrefilter(e);
+                    try {
+                        for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (ce.cleanData(Se(t, !1)), t.innerHTML = e);
+                        t = 0
+                    } catch (e) {}
+                }
+                t && this.empty().append(e)
+            }, null, e, arguments.length)
+        },
+        replaceWith: function() {
+            var n = [];
+            return $e(this, arguments, function(e) {
+                var t = this.parentNode;
+                ce.inArray(this, n) < 0 && (ce.cleanData(Se(this)), t && t.replaceChild(e, this))
+            }, n)
+        }
+    }), ce.each({
+        appendTo: "append",
+        prependTo: "prepend",
+        insertBefore: "before",
+        insertAfter: "after",
+        replaceAll: "replaceWith"
+    }, function(e, a) {
+        ce.fn[e] = function(e) {
+            for (var t, n = [], r = ce(e), i = r.length - 1, o = 0; o <= i; o++) t = o === i ? this : this.clone(!0), ce(r[o])[a](t), s.apply(n, t.get());
+            return this.pushStack(n)
+        }
+    });
+    var _e = new RegExp("^(" + G + ")(?!px)[a-z%]+$", "i"),
+        ze = /^--/,
+        Xe = function(e) {
+            var t = e.ownerDocument.defaultView;
+            return t && t.opener || (t = ie), t.getComputedStyle(e)
+        },
+        Ue = function(e, t, n) {
+            var r, i, o = {};
+            for (i in t) o[i] = e.style[i], e.style[i] = t[i];
+            for (i in r = n.call(e), t) e.style[i] = o[i];
+            return r
+        },
+        Ve = new RegExp(Q.join("|"), "i");
+
+    function Ge(e, t, n) {
+        var r, i, o, a, s = ze.test(t),
+            u = e.style;
+        return (n = n || Xe(e)) && (a = n.getPropertyValue(t) || n[t], s && a && (a = a.replace(ve, "$1") || void 0), "" !== a || K(e) || (a = ce.style(e, t)), !le.pixelBoxStyles() && _e.test(a) && Ve.test(t) && (r = u.width, i = u.minWidth, o = u.maxWidth, u.minWidth = u.maxWidth = u.width = a, a = n.width, u.width = r, u.minWidth = i, u.maxWidth = o)), void 0 !== a ? a + "" : a
+    }
+
+    function Ye(e, t) {
+        return {
+            get: function() {
+                if (!e()) return (this.get = t).apply(this, arguments);
+                delete this.get
+            }
+        }
+    }! function() {
+        function e() {
+            if (l) {
+                u.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", l.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", J.appendChild(u).appendChild(l);
+                var e = ie.getComputedStyle(l);
+                n = "1%" !== e.top, s = 12 === t(e.marginLeft), l.style.right = "60%", o = 36 === t(e.right), r = 36 === t(e.width), l.style.position = "absolute", i = 12 === t(l.offsetWidth / 3), J.removeChild(u), l = null
+            }
+        }
+
+        function t(e) {
+            return Math.round(parseFloat(e))
+        }
+        var n, r, i, o, a, s, u = C.createElement("div"),
+            l = C.createElement("div");
+        l.style && (l.style.backgroundClip = "content-box", l.cloneNode(!0).style.backgroundClip = "", le.clearCloneStyle = "content-box" === l.style.backgroundClip, ce.extend(le, {
+            boxSizingReliable: function() {
+                return e(), r
+            },
+            pixelBoxStyles: function() {
+                return e(), o
+            },
+            pixelPosition: function() {
+                return e(), n
+            },
+            reliableMarginLeft: function() {
+                return e(), s
+            },
+            scrollboxSize: function() {
+                return e(), i
+            },
+            reliableTrDimensions: function() {
+                var e, t, n, r;
+                return null == a && (e = C.createElement("table"), t = C.createElement("tr"), n = C.createElement("div"), e.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", t.style.cssText = "box-sizing:content-box;border:1px solid", t.style.height = "1px", n.style.height = "9px", n.style.display = "block", J.appendChild(e).appendChild(t).appendChild(n), r = ie.getComputedStyle(t), a = parseInt(r.height, 10) + parseInt(r.borderTopWidth, 10) + parseInt(r.borderBottomWidth, 10) === t.offsetHeight, J.removeChild(e)), a
+            }
+        }))
+    }();
+    var Qe = ["Webkit", "Moz", "ms"],
+        Je = C.createElement("div").style,
+        Ke = {};
+
+    function Ze(e) {
+        var t = ce.cssProps[e] || Ke[e];
+        return t || (e in Je ? e : Ke[e] = function(e) {
+            var t = e[0].toUpperCase() + e.slice(1),
+                n = Qe.length;
+            while (n--)
+                if ((e = Qe[n] + t) in Je) return e
+        }(e) || e)
+    }
+    var et = /^(none|table(?!-c[ea]).+)/,
+        tt = {
+            position: "absolute",
+            visibility: "hidden",
+            display: "block"
+        },
+        nt = {
+            letterSpacing: "0",
+            fontWeight: "400"
+        };
+
+    function rt(e, t, n) {
+        var r = Y.exec(t);
+        return r ? Math.max(0, r[2] - (n || 0)) + (r[3] || "px") : t
+    }
+
+    function it(e, t, n, r, i, o) {
+        var a = "width" === t ? 1 : 0,
+            s = 0,
+            u = 0,
+            l = 0;
+        if (n === (r ? "border" : "content")) return 0;
+        for (; a < 4; a += 2) "margin" === n && (l += ce.css(e, n + Q[a], !0, i)), r ? ("content" === n && (u -= ce.css(e, "padding" + Q[a], !0, i)), "margin" !== n && (u -= ce.css(e, "border" + Q[a] + "Width", !0, i))) : (u += ce.css(e, "padding" + Q[a], !0, i), "padding" !== n ? u += ce.css(e, "border" + Q[a] + "Width", !0, i) : s += ce.css(e, "border" + Q[a] + "Width", !0, i));
+        return !r && 0 <= o && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u + l
+    }
+
+    function ot(e, t, n) {
+        var r = Xe(e),
+            i = (!le.boxSizingReliable() || n) && "border-box" === ce.css(e, "boxSizing", !1, r),
+            o = i,
+            a = Ge(e, t, r),
+            s = "offset" + t[0].toUpperCase() + t.slice(1);
+        if (_e.test(a)) {
+            if (!n) return a;
+            a = "auto"
+        }
+        return (!le.boxSizingReliable() && i || !le.reliableTrDimensions() && fe(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === ce.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === ce.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + it(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
+    }
+
+    function at(e, t, n, r, i) {
+        return new at.prototype.init(e, t, n, r, i)
+    }
+    ce.extend({
+        cssHooks: {
+            opacity: {
+                get: function(e, t) {
+                    if (t) {
+                        var n = Ge(e, "opacity");
+                        return "" === n ? "1" : n
+                    }
+                }
+            }
+        },
+        cssNumber: {
+            animationIterationCount: !0,
+            aspectRatio: !0,
+            borderImageSlice: !0,
+            columnCount: !0,
+            flexGrow: !0,
+            flexShrink: !0,
+            fontWeight: !0,
+            gridArea: !0,
+            gridColumn: !0,
+            gridColumnEnd: !0,
+            gridColumnStart: !0,
+            gridRow: !0,
+            gridRowEnd: !0,
+            gridRowStart: !0,
+            lineHeight: !0,
+            opacity: !0,
+            order: !0,
+            orphans: !0,
+            scale: !0,
+            widows: !0,
+            zIndex: !0,
+            zoom: !0,
+            fillOpacity: !0,
+            floodOpacity: !0,
+            stopOpacity: !0,
+            strokeMiterlimit: !0,
+            strokeOpacity: !0
+        },
+        cssProps: {},
+        style: function(e, t, n, r) {
+            if (e && 3 !== e.nodeType && 8 !== e.nodeType && e.style) {
+                var i, o, a, s = F(t),
+                    u = ze.test(t),
+                    l = e.style;
+                if (u || (t = Ze(s)), a = ce.cssHooks[t] || ce.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
+                "string" === (o = typeof n) && (i = Y.exec(n)) && i[1] && (n = te(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (ce.cssNumber[s] ? "" : "px")), le.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
+            }
+        },
+        css: function(e, t, n, r) {
+            var i, o, a, s = F(t);
+            return ze.test(t) || (t = Ze(s)), (a = ce.cssHooks[t] || ce.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = Ge(e, t, r)), "normal" === i && t in nt && (i = nt[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
+        }
+    }), ce.each(["height", "width"], function(e, u) {
+        ce.cssHooks[u] = {
+            get: function(e, t, n) {
+                if (t) return !et.test(ce.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? ot(e, u, n) : Ue(e, tt, function() {
+                    return ot(e, u, n)
+                })
+            },
+            set: function(e, t, n) {
+                var r, i = Xe(e),
+                    o = !le.scrollboxSize() && "absolute" === i.position,
+                    a = (o || n) && "border-box" === ce.css(e, "boxSizing", !1, i),
+                    s = n ? it(e, u, n, a, i) : 0;
+                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - it(e, u, "border", !1, i) - .5)), s && (r = Y.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = ce.css(e, u)), rt(0, t, s)
+            }
+        }
+    }), ce.cssHooks.marginLeft = Ye(le.reliableMarginLeft, function(e, t) {
+        if (t) return (parseFloat(Ge(e, "marginLeft")) || e.getBoundingClientRect().left - Ue(e, {
+            marginLeft: 0
+        }, function() {
+            return e.getBoundingClientRect().left
+        })) + "px"
+    }), ce.each({
+        margin: "",
+        padding: "",
+        border: "Width"
+    }, function(i, o) {
+        ce.cssHooks[i + o] = {
+            expand: function(e) {
+                for (var t = 0, n = {}, r = "string" == typeof e ? e.split(" ") : [e]; t < 4; t++) n[i + Q[t] + o] = r[t] || r[t - 2] || r[0];
+                return n
+            }
+        }, "margin" !== i && (ce.cssHooks[i + o].set = rt)
+    }), ce.fn.extend({
+        css: function(e, t) {
+            return M(this, function(e, t, n) {
+                var r, i, o = {},
+                    a = 0;
+                if (Array.isArray(t)) {
+                    for (r = Xe(e), i = t.length; a < i; a++) o[t[a]] = ce.css(e, t[a], !1, r);
+                    return o
+                }
+                return void 0 !== n ? ce.style(e, t, n) : ce.css(e, t)
+            }, e, t, 1 < arguments.length)
+        }
+    }), ((ce.Tween = at).prototype = {
+        constructor: at,
+        init: function(e, t, n, r, i, o) {
+            this.elem = e, this.prop = n, this.easing = i || ce.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (ce.cssNumber[n] ? "" : "px")
+        },
+        cur: function() {
+            var e = at.propHooks[this.prop];
+            return e && e.get ? e.get(this) : at.propHooks._default.get(this)
+        },
+        run: function(e) {
+            var t, n = at.propHooks[this.prop];
+            return this.options.duration ? this.pos = t = ce.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : at.propHooks._default.set(this), this
+        }
+    }).init.prototype = at.prototype, (at.propHooks = {
+        _default: {
+            get: function(e) {
+                var t;
+                return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = ce.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
+            },
+            set: function(e) {
+                ce.fx.step[e.prop] ? ce.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !ce.cssHooks[e.prop] && null == e.elem.style[Ze(e.prop)] ? e.elem[e.prop] = e.now : ce.style(e.elem, e.prop, e.now + e.unit)
+            }
+        }
+    }).scrollTop = at.propHooks.scrollLeft = {
+        set: function(e) {
+            e.elem.nodeType && e.elem.parentNode && (e.elem[e.prop] = e.now)
+        }
+    }, ce.easing = {
+        linear: function(e) {
+            return e
+        },
+        swing: function(e) {
+            return .5 - Math.cos(e * Math.PI) / 2
+        },
+        _default: "swing"
+    }, ce.fx = at.prototype.init, ce.fx.step = {};
+    var st, ut, lt, ct, ft = /^(?:toggle|show|hide)$/,
+        pt = /queueHooks$/;
+
+    function dt() {
+        ut && (!1 === C.hidden && ie.requestAnimationFrame ? ie.requestAnimationFrame(dt) : ie.setTimeout(dt, ce.fx.interval), ce.fx.tick())
+    }
+
+    function ht() {
+        return ie.setTimeout(function() {
+            st = void 0
+        }), st = Date.now()
+    }
+
+    function gt(e, t) {
+        var n, r = 0,
+            i = {
+                height: e
+            };
+        for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = Q[r])] = i["padding" + n] = e;
+        return t && (i.opacity = i.width = e), i
+    }
+
+    function vt(e, t, n) {
+        for (var r, i = (yt.tweeners[t] || []).concat(yt.tweeners["*"]), o = 0, a = i.length; o < a; o++)
+            if (r = i[o].call(n, t, e)) return r
+    }
+
+    function yt(o, e, t) {
+        var n, a, r = 0,
+            i = yt.prefilters.length,
+            s = ce.Deferred().always(function() {
+                delete u.elem
+            }),
+            u = function() {
+                if (a) return !1;
+                for (var e = st || ht(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
+                return s.notifyWith(o, [l, n, t]), n < 1 && i ? t : (i || s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l]), !1)
+            },
+            l = s.promise({
+                elem: o,
+                props: ce.extend({}, e),
+                opts: ce.extend(!0, {
+                    specialEasing: {},
+                    easing: ce.easing._default
+                }, t),
+                originalProperties: e,
+                originalOptions: t,
+                startTime: st || ht(),
+                duration: t.duration,
+                tweens: [],
+                createTween: function(e, t) {
+                    var n = ce.Tween(o, l.opts, e, t, l.opts.specialEasing[e] || l.opts.easing);
+                    return l.tweens.push(n), n
+                },
+                stop: function(e) {
+                    var t = 0,
+                        n = e ? l.tweens.length : 0;
+                    if (a) return this;
+                    for (a = !0; t < n; t++) l.tweens[t].run(1);
+                    return e ? (s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l, e])) : s.rejectWith(o, [l, e]), this
+                }
+            }),
+            c = l.props;
+        for (! function(e, t) {
+                var n, r, i, o, a;
+                for (n in e)
+                    if (i = t[r = F(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = ce.cssHooks[r]) && "expand" in a)
+                        for (n in o = a.expand(o), delete e[r], o) n in e || (e[n] = o[n], t[n] = i);
+                    else t[r] = i
+            }(c, l.opts.specialEasing); r < i; r++)
+            if (n = yt.prefilters[r].call(l, o, c, l.opts)) return v(n.stop) && (ce._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
+        return ce.map(c, vt, l), v(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), ce.fx.timer(ce.extend(u, {
+            elem: o,
+            anim: l,
+            queue: l.opts.queue
+        })), l
+    }
+    ce.Animation = ce.extend(yt, {
+        tweeners: {
+            "*": [function(e, t) {
+                var n = this.createTween(e, t);
+                return te(n.elem, e, Y.exec(t), n), n
+            }]
+        },
+        tweener: function(e, t) {
+            v(e) ? (t = e, e = ["*"]) : e = e.match(D);
+            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], yt.tweeners[n] = yt.tweeners[n] || [], yt.tweeners[n].unshift(t)
+        },
+        prefilters: [function(e, t, n) {
+            var r, i, o, a, s, u, l, c, f = "width" in t || "height" in t,
+                p = this,
+                d = {},
+                h = e.style,
+                g = e.nodeType && ee(e),
+                v = _.get(e, "fxshow");
+            for (r in n.queue || (null == (a = ce._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
+                    a.unqueued || s()
+                }), a.unqueued++, p.always(function() {
+                    p.always(function() {
+                        a.unqueued--, ce.queue(e, "fx").length || a.empty.fire()
+                    })
+                })), t)
+                if (i = t[r], ft.test(i)) {
+                    if (delete t[r], o = o || "toggle" === i, i === (g ? "hide" : "show")) {
+                        if ("show" !== i || !v || void 0 === v[r]) continue;
+                        g = !0
+                    }
+                    d[r] = v && v[r] || ce.style(e, r)
+                } if ((u = !ce.isEmptyObject(t)) || !ce.isEmptyObject(d))
+                for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = _.get(e, "display")), "none" === (c = ce.css(e, "display")) && (l ? c = l : (re([e], !0), l = e.style.display || l, c = ce.css(e, "display"), re([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === ce.css(e, "float") && (u || (p.done(function() {
+                        h.display = l
+                    }), null == l && (c = h.display, l = "none" === c ? "" : c)), h.display = "inline-block")), n.overflow && (h.overflow = "hidden", p.always(function() {
+                        h.overflow = n.overflow[0], h.overflowX = n.overflow[1], h.overflowY = n.overflow[2]
+                    })), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = _.access(e, "fxshow", {
+                    display: l
+                }), o && (v.hidden = !g), g && re([e], !0), p.done(function() {
+                    for (r in g || re([e]), _.remove(e, "fxshow"), d) ce.style(e, r, d[r])
+                })), u = vt(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
+        }],
+        prefilter: function(e, t) {
+            t ? yt.prefilters.unshift(e) : yt.prefilters.push(e)
+        }
+    }), ce.speed = function(e, t, n) {
+        var r = e && "object" == typeof e ? ce.extend({}, e) : {
+            complete: n || !n && t || v(e) && e,
+            duration: e,
+            easing: n && t || t && !v(t) && t
+        };
+        return ce.fx.off ? r.duration = 0 : "number" != typeof r.duration && (r.duration in ce.fx.speeds ? r.duration = ce.fx.speeds[r.duration] : r.duration = ce.fx.speeds._default), null != r.queue && !0 !== r.queue || (r.queue = "fx"), r.old = r.complete, r.complete = function() {
+            v(r.old) && r.old.call(this), r.queue && ce.dequeue(this, r.queue)
+        }, r
+    }, ce.fn.extend({
+        fadeTo: function(e, t, n, r) {
+            return this.filter(ee).css("opacity", 0).show().end().animate({
+                opacity: t
+            }, e, n, r)
+        },
+        animate: function(t, e, n, r) {
+            var i = ce.isEmptyObject(t),
+                o = ce.speed(e, n, r),
+                a = function() {
+                    var e = yt(this, ce.extend({}, t), o);
+                    (i || _.get(this, "finish")) && e.stop(!0)
+                };
+            return a.finish = a, i || !1 === o.queue ? this.each(a) : this.queue(o.queue, a)
+        },
+        stop: function(i, e, o) {
+            var a = function(e) {
+                var t = e.stop;
+                delete e.stop, t(o)
+            };
+            return "string" != typeof i && (o = e, e = i, i = void 0), e && this.queue(i || "fx", []), this.each(function() {
+                var e = !0,
+                    t = null != i && i + "queueHooks",
+                    n = ce.timers,
+                    r = _.get(this);
+                if (t) r[t] && r[t].stop && a(r[t]);
+                else
+                    for (t in r) r[t] && r[t].stop && pt.test(t) && a(r[t]);
+                for (t = n.length; t--;) n[t].elem !== this || null != i && n[t].queue !== i || (n[t].anim.stop(o), e = !1, n.splice(t, 1));
+                !e && o || ce.dequeue(this, i)
+            })
+        },
+        finish: function(a) {
+            return !1 !== a && (a = a || "fx"), this.each(function() {
+                var e, t = _.get(this),
+                    n = t[a + "queue"],
+                    r = t[a + "queueHooks"],
+                    i = ce.timers,
+                    o = n ? n.length : 0;
+                for (t.finish = !0, ce.queue(this, a, []), r && r.stop && r.stop.call(this, !0), e = i.length; e--;) i[e].elem === this && i[e].queue === a && (i[e].anim.stop(!0), i.splice(e, 1));
+                for (e = 0; e < o; e++) n[e] && n[e].finish && n[e].finish.call(this);
+                delete t.finish
+            })
+        }
+    }), ce.each(["toggle", "show", "hide"], function(e, r) {
+        var i = ce.fn[r];
+        ce.fn[r] = function(e, t, n) {
+            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(gt(r, !0), e, t, n)
+        }
+    }), ce.each({
+        slideDown: gt("show"),
+        slideUp: gt("hide"),
+        slideToggle: gt("toggle"),
+        fadeIn: {
+            opacity: "show"
+        },
+        fadeOut: {
+            opacity: "hide"
+        },
+        fadeToggle: {
+            opacity: "toggle"
+        }
+    }, function(e, r) {
+        ce.fn[e] = function(e, t, n) {
+            return this.animate(r, e, t, n)
+        }
+    }), ce.timers = [], ce.fx.tick = function() {
+        var e, t = 0,
+            n = ce.timers;
+        for (st = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
+        n.length || ce.fx.stop(), st = void 0
+    }, ce.fx.timer = function(e) {
+        ce.timers.push(e), ce.fx.start()
+    }, ce.fx.interval = 13, ce.fx.start = function() {
+        ut || (ut = !0, dt())
+    }, ce.fx.stop = function() {
+        ut = null
+    }, ce.fx.speeds = {
+        slow: 600,
+        fast: 200,
+        _default: 400
+    }, ce.fn.delay = function(r, e) {
+        return r = ce.fx && ce.fx.speeds[r] || r, e = e || "fx", this.queue(e, function(e, t) {
+            var n = ie.setTimeout(e, r);
+            t.stop = function() {
+                ie.clearTimeout(n)
+            }
+        })
+    }, lt = C.createElement("input"), ct = C.createElement("select").appendChild(C.createElement("option")), lt.type = "checkbox", le.checkOn = "" !== lt.value, le.optSelected = ct.selected, (lt = C.createElement("input")).value = "t", lt.type = "radio", le.radioValue = "t" === lt.value;
+    var mt, xt = ce.expr.attrHandle;
+    ce.fn.extend({
+        attr: function(e, t) {
+            return M(this, ce.attr, e, t, 1 < arguments.length)
+        },
+        removeAttr: function(e) {
+            return this.each(function() {
+                ce.removeAttr(this, e)
+            })
+        }
+    }), ce.extend({
+        attr: function(e, t, n) {
+            var r, i, o = e.nodeType;
+            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? ce.prop(e, t, n) : (1 === o && ce.isXMLDoc(e) || (i = ce.attrHooks[t.toLowerCase()] || (ce.expr.match.bool.test(t) ? mt : void 0)), void 0 !== n ? null === n ? void ce.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = ce.find.attr(e, t)) ? void 0 : r)
+        },
+        attrHooks: {
+            type: {
+                set: function(e, t) {
+                    if (!le.radioValue && "radio" === t && fe(e, "input")) {
+                        var n = e.value;
+                        return e.setAttribute("type", t), n && (e.value = n), t
+                    }
+                }
+            }
+        },
+        removeAttr: function(e, t) {
+            var n, r = 0,
+                i = t && t.match(D);
+            if (i && 1 === e.nodeType)
+                while (n = i[r++]) e.removeAttribute(n)
+        }
+    }), mt = {
+        set: function(e, t, n) {
+            return !1 === t ? ce.removeAttr(e, n) : e.setAttribute(n, n), n
+        }
+    }, ce.each(ce.expr.match.bool.source.match(/\w+/g), function(e, t) {
+        var a = xt[t] || ce.find.attr;
+        xt[t] = function(e, t, n) {
+            var r, i, o = t.toLowerCase();
+            return n || (i = xt[o], xt[o] = r, r = null != a(e, t, n) ? o : null, xt[o] = i), r
+        }
+    });
+    var bt = /^(?:input|select|textarea|button)$/i,
+        wt = /^(?:a|area)$/i;
+
+    function Tt(e) {
+        return (e.match(D) || []).join(" ")
+    }
+
+    function Ct(e) {
+        return e.getAttribute && e.getAttribute("class") || ""
+    }
+
+    function kt(e) {
+        return Array.isArray(e) ? e : "string" == typeof e && e.match(D) || []
+    }
+    ce.fn.extend({
+        prop: function(e, t) {
+            return M(this, ce.prop, e, t, 1 < arguments.length)
+        },
+        removeProp: function(e) {
+            return this.each(function() {
+                delete this[ce.propFix[e] || e]
+            })
+        }
+    }), ce.extend({
+        prop: function(e, t, n) {
+            var r, i, o = e.nodeType;
+            if (3 !== o && 8 !== o && 2 !== o) return 1 === o && ce.isXMLDoc(e) || (t = ce.propFix[t] || t, i = ce.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
+        },
+        propHooks: {
+            tabIndex: {
+                get: function(e) {
+                    var t = ce.find.attr(e, "tabindex");
+                    return t ? parseInt(t, 10) : bt.test(e.nodeName) || wt.test(e.nodeName) && e.href ? 0 : -1
+                }
+            }
+        },
+        propFix: {
+            "for": "htmlFor",
+            "class": "className"
+        }
+    }), le.optSelected || (ce.propHooks.selected = {
+        get: function(e) {
+            var t = e.parentNode;
+            return t && t.parentNode && t.parentNode.selectedIndex, null
+        },
+        set: function(e) {
+            var t = e.parentNode;
+            t && (t.selectedIndex, t.parentNode && t.parentNode.selectedIndex)
+        }
+    }), ce.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
+        ce.propFix[this.toLowerCase()] = this
+    }), ce.fn.extend({
+        addClass: function(t) {
+            var e, n, r, i, o, a;
+            return v(t) ? this.each(function(e) {
+                ce(this).addClass(t.call(this, e, Ct(this)))
+            }) : (e = kt(t)).length ? this.each(function() {
+                if (r = Ct(this), n = 1 === this.nodeType && " " + Tt(r) + " ") {
+                    for (o = 0; o < e.length; o++) i = e[o], n.indexOf(" " + i + " ") < 0 && (n += i + " ");
+                    a = Tt(n), r !== a && this.setAttribute("class", a)
+                }
+            }) : this
+        },
+        removeClass: function(t) {
+            var e, n, r, i, o, a;
+            return v(t) ? this.each(function(e) {
+                ce(this).removeClass(t.call(this, e, Ct(this)))
+            }) : arguments.length ? (e = kt(t)).length ? this.each(function() {
+                if (r = Ct(this), n = 1 === this.nodeType && " " + Tt(r) + " ") {
+                    for (o = 0; o < e.length; o++) {
+                        i = e[o];
+                        while (-1 < n.indexOf(" " + i + " ")) n = n.replace(" " + i + " ", " ")
+                    }
+                    a = Tt(n), r !== a && this.setAttribute("class", a)
+                }
+            }) : this : this.attr("class", "")
+        },
+        toggleClass: function(t, n) {
+            var e, r, i, o, a = typeof t,
+                s = "string" === a || Array.isArray(t);
+            return v(t) ? this.each(function(e) {
+                ce(this).toggleClass(t.call(this, e, Ct(this), n), n)
+            }) : "boolean" == typeof n && s ? n ? this.addClass(t) : this.removeClass(t) : (e = kt(t), this.each(function() {
+                if (s)
+                    for (o = ce(this), i = 0; i < e.length; i++) r = e[i], o.hasClass(r) ? o.removeClass(r) : o.addClass(r);
+                else void 0 !== t && "boolean" !== a || ((r = Ct(this)) && _.set(this, "__className__", r), this.setAttribute && this.setAttribute("class", r || !1 === t ? "" : _.get(this, "__className__") || ""))
+            }))
+        },
+        hasClass: function(e) {
+            var t, n, r = 0;
+            t = " " + e + " ";
+            while (n = this[r++])
+                if (1 === n.nodeType && -1 < (" " + Tt(Ct(n)) + " ").indexOf(t)) return !0;
+            return !1
+        }
+    });
+    var St = /\r/g;
+    ce.fn.extend({
+        val: function(n) {
+            var r, e, i, t = this[0];
+            return arguments.length ? (i = v(n), this.each(function(e) {
+                var t;
+                1 === this.nodeType && (null == (t = i ? n.call(this, e, ce(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = ce.map(t, function(e) {
+                    return null == e ? "" : e + ""
+                })), (r = ce.valHooks[this.type] || ce.valHooks[this.nodeName.toLowerCase()]) && "set" in r && void 0 !== r.set(this, t, "value") || (this.value = t))
+            })) : t ? (r = ce.valHooks[t.type] || ce.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(St, "") : null == e ? "" : e : void 0
+        }
+    }), ce.extend({
+        valHooks: {
+            option: {
+                get: function(e) {
+                    var t = ce.find.attr(e, "value");
+                    return null != t ? t : Tt(ce.text(e))
+                }
+            },
+            select: {
+                get: function(e) {
+                    var t, n, r, i = e.options,
+                        o = e.selectedIndex,
+                        a = "select-one" === e.type,
+                        s = a ? null : [],
+                        u = a ? o + 1 : i.length;
+                    for (r = o < 0 ? u : a ? o : 0; r < u; r++)
+                        if (((n = i[r]).selected || r === o) && !n.disabled && (!n.parentNode.disabled || !fe(n.parentNode, "optgroup"))) {
+                            if (t = ce(n).val(), a) return t;
+                            s.push(t)
+                        } return s
+                },
+                set: function(e, t) {
+                    var n, r, i = e.options,
+                        o = ce.makeArray(t),
+                        a = i.length;
+                    while (a--)((r = i[a]).selected = -1 < ce.inArray(ce.valHooks.option.get(r), o)) && (n = !0);
+                    return n || (e.selectedIndex = -1), o
+                }
+            }
+        }
+    }), ce.each(["radio", "checkbox"], function() {
+        ce.valHooks[this] = {
+            set: function(e, t) {
+                if (Array.isArray(t)) return e.checked = -1 < ce.inArray(ce(e).val(), t)
+            }
+        }, le.checkOn || (ce.valHooks[this].get = function(e) {
+            return null === e.getAttribute("value") ? "on" : e.value
+        })
+    });
+    var Et = ie.location,
+        jt = {
+            guid: Date.now()
+        },
+        At = /\?/;
+    ce.parseXML = function(e) {
+        var t, n;
+        if (!e || "string" != typeof e) return null;
+        try {
+            t = (new ie.DOMParser).parseFromString(e, "text/xml")
+        } catch (e) {}
+        return n = t && t.getElementsByTagName("parsererror")[0], t && !n || ce.error("Invalid XML: " + (n ? ce.map(n.childNodes, function(e) {
+            return e.textContent
+        }).join("\n") : e)), t
+    };
+    var Dt = /^(?:focusinfocus|focusoutblur)$/,
+        Nt = function(e) {
+            e.stopPropagation()
+        };
+    ce.extend(ce.event, {
+        trigger: function(e, t, n, r) {
+            var i, o, a, s, u, l, c, f, p = [n || C],
+                d = ue.call(e, "type") ? e.type : e,
+                h = ue.call(e, "namespace") ? e.namespace.split(".") : [];
+            if (o = f = a = n = n || C, 3 !== n.nodeType && 8 !== n.nodeType && !Dt.test(d + ce.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[ce.expando] ? e : new ce.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : ce.makeArray(t, [e]), c = ce.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
+                if (!r && !c.noBubble && !y(n)) {
+                    for (s = c.delegateType || d, Dt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
+                    a === (n.ownerDocument || C) && p.push(a.defaultView || a.parentWindow || ie)
+                }
+                i = 0;
+                while ((o = p[i++]) && !e.isPropagationStopped()) f = o, e.type = 1 < i ? s : c.bindType || d, (l = (_.get(o, "events") || Object.create(null))[e.type] && _.get(o, "handle")) && l.apply(o, t), (l = u && o[u]) && l.apply && $(o) && (e.result = l.apply(o, t), !1 === e.result && e.preventDefault());
+                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !$(n) || u && v(n[d]) && !y(n) && ((a = n[u]) && (n[u] = null), ce.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, Nt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, Nt), ce.event.triggered = void 0, a && (n[u] = a)), e.result
+            }
+        },
+        simulate: function(e, t, n) {
+            var r = ce.extend(new ce.Event, n, {
+                type: e,
+                isSimulated: !0
+            });
+            ce.event.trigger(r, null, t)
+        }
+    }), ce.fn.extend({
+        trigger: function(e, t) {
+            return this.each(function() {
+                ce.event.trigger(e, t, this)
+            })
+        },
+        triggerHandler: function(e, t) {
+            var n = this[0];
+            if (n) return ce.event.trigger(e, t, n, !0)
+        }
+    });
+    var qt = /\[\]$/,
+        Lt = /\r?\n/g,
+        Ht = /^(?:submit|button|image|reset|file)$/i,
+        Ot = /^(?:input|select|textarea|keygen)/i;
+
+    function Pt(n, e, r, i) {
+        var t;
+        if (Array.isArray(e)) ce.each(e, function(e, t) {
+            r || qt.test(n) ? i(n, t) : Pt(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
+        });
+        else if (r || "object" !== x(e)) i(n, e);
+        else
+            for (t in e) Pt(n + "[" + t + "]", e[t], r, i)
+    }
+    ce.param = function(e, t) {
+        var n, r = [],
+            i = function(e, t) {
+                var n = v(t) ? t() : t;
+                r[r.length] = encodeURIComponent(e) + "=" + encodeURIComponent(null == n ? "" : n)
+            };
+        if (null == e) return "";
+        if (Array.isArray(e) || e.jquery && !ce.isPlainObject(e)) ce.each(e, function() {
+            i(this.name, this.value)
+        });
+        else
+            for (n in e) Pt(n, e[n], t, i);
+        return r.join("&")
+    }, ce.fn.extend({
+        serialize: function() {
+            return ce.param(this.serializeArray())
+        },
+        serializeArray: function() {
+            return this.map(function() {
+                var e = ce.prop(this, "elements");
+                return e ? ce.makeArray(e) : this
+            }).filter(function() {
+                var e = this.type;
+                return this.name && !ce(this).is(":disabled") && Ot.test(this.nodeName) && !Ht.test(e) && (this.checked || !we.test(e))
+            }).map(function(e, t) {
+                var n = ce(this).val();
+                return null == n ? null : Array.isArray(n) ? ce.map(n, function(e) {
+                    return {
+                        name: t.name,
+                        value: e.replace(Lt, "\r\n")
+                    }
+                }) : {
+                    name: t.name,
+                    value: n.replace(Lt, "\r\n")
+                }
+            }).get()
+        }
+    });
+    var Mt = /%20/g,
+        Rt = /#.*$/,
+        It = /([?&])_=[^&]*/,
+        Wt = /^(.*?):[ \t]*([^\r\n]*)$/gm,
+        Ft = /^(?:GET|HEAD)$/,
+        $t = /^\/\//,
+        Bt = {},
+        _t = {},
+        zt = "*/".concat("*"),
+        Xt = C.createElement("a");
+
+    function Ut(o) {
+        return function(e, t) {
+            "string" != typeof e && (t = e, e = "*");
+            var n, r = 0,
+                i = e.toLowerCase().match(D) || [];
+            if (v(t))
+                while (n = i[r++]) "+" === n[0] ? (n = n.slice(1) || "*", (o[n] = o[n] || []).unshift(t)) : (o[n] = o[n] || []).push(t)
+        }
+    }
+
+    function Vt(t, i, o, a) {
+        var s = {},
+            u = t === _t;
+
+        function l(e) {
+            var r;
+            return s[e] = !0, ce.each(t[e] || [], function(e, t) {
+                var n = t(i, o, a);
+                return "string" != typeof n || u || s[n] ? u ? !(r = n) : void 0 : (i.dataTypes.unshift(n), l(n), !1)
+            }), r
+        }
+        return l(i.dataTypes[0]) || !s["*"] && l("*")
+    }
+
+    function Gt(e, t) {
+        var n, r, i = ce.ajaxSettings.flatOptions || {};
+        for (n in t) void 0 !== t[n] && ((i[n] ? e : r || (r = {}))[n] = t[n]);
+        return r && ce.extend(!0, e, r), e
+    }
+    Xt.href = Et.href, ce.extend({
+        active: 0,
+        lastModified: {},
+        etag: {},
+        ajaxSettings: {
+            url: Et.href,
+            type: "GET",
+            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Et.protocol),
+            global: !0,
+            processData: !0,
+            async: !0,
+            contentType: "application/x-www-form-urlencoded; charset=UTF-8",
+            accepts: {
+                "*": zt,
+                text: "text/plain",
+                html: "text/html",
+                xml: "application/xml, text/xml",
+                json: "application/json, text/javascript"
+            },
+            contents: {
+                xml: /\bxml\b/,
+                html: /\bhtml/,
+                json: /\bjson\b/
+            },
+            responseFields: {
+                xml: "responseXML",
+                text: "responseText",
+                json: "responseJSON"
+            },
+            converters: {
+                "* text": String,
+                "text html": !0,
+                "text json": JSON.parse,
+                "text xml": ce.parseXML
+            },
+            flatOptions: {
+                url: !0,
+                context: !0
+            }
+        },
+        ajaxSetup: function(e, t) {
+            return t ? Gt(Gt(e, ce.ajaxSettings), t) : Gt(ce.ajaxSettings, e)
+        },
+        ajaxPrefilter: Ut(Bt),
+        ajaxTransport: Ut(_t),
+        ajax: function(e, t) {
+            "object" == typeof e && (t = e, e = void 0), t = t || {};
+            var c, f, p, n, d, r, h, g, i, o, v = ce.ajaxSetup({}, t),
+                y = v.context || v,
+                m = v.context && (y.nodeType || y.jquery) ? ce(y) : ce.event,
+                x = ce.Deferred(),
+                b = ce.Callbacks("once memory"),
+                w = v.statusCode || {},
+                a = {},
+                s = {},
+                u = "canceled",
+                T = {
+                    readyState: 0,
+                    getResponseHeader: function(e) {
+                        var t;
+                        if (h) {
+                            if (!n) {
+                                n = {};
+                                while (t = Wt.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
+                            }
+                            t = n[e.toLowerCase() + " "]
+                        }
+                        return null == t ? null : t.join(", ")
+                    },
+                    getAllResponseHeaders: function() {
+                        return h ? p : null
+                    },
+                    setRequestHeader: function(e, t) {
+                        return null == h && (e = s[e.toLowerCase()] = s[e.toLowerCase()] || e, a[e] = t), this
+                    },
+                    overrideMimeType: function(e) {
+                        return null == h && (v.mimeType = e), this
+                    },
+                    statusCode: function(e) {
+                        var t;
+                        if (e)
+                            if (h) T.always(e[T.status]);
+                            else
+                                for (t in e) w[t] = [w[t], e[t]];
+                        return this
+                    },
+                    abort: function(e) {
+                        var t = e || u;
+                        return c && c.abort(t), l(0, t), this
+                    }
+                };
+            if (x.promise(T), v.url = ((e || v.url || Et.href) + "").replace($t, Et.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(D) || [""], null == v.crossDomain) {
+                r = C.createElement("a");
+                try {
+                    r.href = v.url, r.href = r.href, v.crossDomain = Xt.protocol + "//" + Xt.host != r.protocol + "//" + r.host
+                } catch (e) {
+                    v.crossDomain = !0
+                }
+            }
+            if (v.data && v.processData && "string" != typeof v.data && (v.data = ce.param(v.data, v.traditional)), Vt(Bt, v, t, T), h) return T;
+            for (i in (g = ce.event && v.global) && 0 == ce.active++ && ce.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Ft.test(v.type), f = v.url.replace(Rt, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(Mt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (At.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(It, "$1"), o = (At.test(f) ? "&" : "?") + "_=" + jt.guid++ + o), v.url = f + o), v.ifModified && (ce.lastModified[f] && T.setRequestHeader("If-Modified-Since", ce.lastModified[f]), ce.etag[f] && T.setRequestHeader("If-None-Match", ce.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + zt + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
+            if (v.beforeSend && (!1 === v.beforeSend.call(y, T, v) || h)) return T.abort();
+            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = Vt(_t, v, t, T)) {
+                if (T.readyState = 1, g && m.trigger("ajaxSend", [T, v]), h) return T;
+                v.async && 0 < v.timeout && (d = ie.setTimeout(function() {
+                    T.abort("timeout")
+                }, v.timeout));
+                try {
+                    h = !1, c.send(a, l)
+                } catch (e) {
+                    if (h) throw e;
+                    l(-1, e)
+                }
+            } else l(-1, "No Transport");
+
+            function l(e, t, n, r) {
+                var i, o, a, s, u, l = t;
+                h || (h = !0, d && ie.clearTimeout(d), c = void 0, p = r || "", T.readyState = 0 < e ? 4 : 0, i = 200 <= e && e < 300 || 304 === e, n && (s = function(e, t, n) {
+                    var r, i, o, a, s = e.contents,
+                        u = e.dataTypes;
+                    while ("*" === u[0]) u.shift(), void 0 === r && (r = e.mimeType || t.getResponseHeader("Content-Type"));
+                    if (r)
+                        for (i in s)
+                            if (s[i] && s[i].test(r)) {
+                                u.unshift(i);
+                                break
+                            } if (u[0] in n) o = u[0];
+                    else {
+                        for (i in n) {
+                            if (!u[0] || e.converters[i + " " + u[0]]) {
+                                o = i;
+                                break
+                            }
+                            a || (a = i)
+                        }
+                        o = o || a
+                    }
+                    if (o) return o !== u[0] && u.unshift(o), n[o]
+                }(v, T, n)), !i && -1 < ce.inArray("script", v.dataTypes) && ce.inArray("json", v.dataTypes) < 0 && (v.converters["text script"] = function() {}), s = function(e, t, n, r) {
+                    var i, o, a, s, u, l = {},
+                        c = e.dataTypes.slice();
+                    if (c[1])
+                        for (a in e.converters) l[a.toLowerCase()] = e.converters[a];
+                    o = c.shift();
+                    while (o)
+                        if (e.responseFields[o] && (n[e.responseFields[o]] = t), !u && r && e.dataFilter && (t = e.dataFilter(t, e.dataType)), u = o, o = c.shift())
+                            if ("*" === o) o = u;
+                            else if ("*" !== u && u !== o) {
+                        if (!(a = l[u + " " + o] || l["* " + o]))
+                            for (i in l)
+                                if ((s = i.split(" "))[1] === o && (a = l[u + " " + s[0]] || l["* " + s[0]])) {
+                                    !0 === a ? a = l[i] : !0 !== l[i] && (o = s[0], c.unshift(s[1]));
+                                    break
+                                } if (!0 !== a)
+                            if (a && e["throws"]) t = a(t);
+                            else try {
+                                t = a(t)
+                            } catch (e) {
+                                return {
+                                    state: "parsererror",
+                                    error: a ? e : "No conversion from " + u + " to " + o
+                                }
+                            }
+                    }
+                    return {
+                        state: "success",
+                        data: t
+                    }
+                }(v, s, T, i), i ? (v.ifModified && ((u = T.getResponseHeader("Last-Modified")) && (ce.lastModified[f] = u), (u = T.getResponseHeader("etag")) && (ce.etag[f] = u)), 204 === e || "HEAD" === v.type ? l = "nocontent" : 304 === e ? l = "notmodified" : (l = s.state, o = s.data, i = !(a = s.error))) : (a = l, !e && l || (l = "error", e < 0 && (e = 0))), T.status = e, T.statusText = (t || l) + "", i ? x.resolveWith(y, [o, l, T]) : x.rejectWith(y, [T, l, a]), T.statusCode(w), w = void 0, g && m.trigger(i ? "ajaxSuccess" : "ajaxError", [T, v, i ? o : a]), b.fireWith(y, [T, l]), g && (m.trigger("ajaxComplete", [T, v]), --ce.active || ce.event.trigger("ajaxStop")))
+            }
+            return T
+        },
+        getJSON: function(e, t, n) {
+            return ce.get(e, t, n, "json")
+        },
+        getScript: function(e, t) {
+            return ce.get(e, void 0, t, "script")
+        }
+    }), ce.each(["get", "post"], function(e, i) {
+        ce[i] = function(e, t, n, r) {
+            return v(t) && (r = r || n, n = t, t = void 0), ce.ajax(ce.extend({
+                url: e,
+                type: i,
+                dataType: r,
+                data: t,
+                success: n
+            }, ce.isPlainObject(e) && e))
+        }
+    }), ce.ajaxPrefilter(function(e) {
+        var t;
+        for (t in e.headers) "content-type" === t.toLowerCase() && (e.contentType = e.headers[t] || "")
+    }), ce._evalUrl = function(e, t, n) {
+        return ce.ajax({
+            url: e,
+            type: "GET",
+            dataType: "script",
+            cache: !0,
+            async: !1,
+            global: !1,
+            converters: {
+                "text script": function() {}
+            },
+            dataFilter: function(e) {
+                ce.globalEval(e, t, n)
+            }
+        })
+    }, ce.fn.extend({
+        wrapAll: function(e) {
+            var t;
+            return this[0] && (v(e) && (e = e.call(this[0])), t = ce(e, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && t.insertBefore(this[0]), t.map(function() {
+                var e = this;
+                while (e.firstElementChild) e = e.firstElementChild;
+                return e
+            }).append(this)), this
+        },
+        wrapInner: function(n) {
+            return v(n) ? this.each(function(e) {
+                ce(this).wrapInner(n.call(this, e))
+            }) : this.each(function() {
+                var e = ce(this),
+                    t = e.contents();
+                t.length ? t.wrapAll(n) : e.append(n)
+            })
+        },
+        wrap: function(t) {
+            var n = v(t);
+            return this.each(function(e) {
+                ce(this).wrapAll(n ? t.call(this, e) : t)
+            })
+        },
+        unwrap: function(e) {
+            return this.parent(e).not("body").each(function() {
+                ce(this).replaceWith(this.childNodes)
+            }), this
+        }
+    }), ce.expr.pseudos.hidden = function(e) {
+        return !ce.expr.pseudos.visible(e)
+    }, ce.expr.pseudos.visible = function(e) {
+        return !!(e.offsetWidth || e.offsetHeight || e.getClientRects().length)
+    }, ce.ajaxSettings.xhr = function() {
+        try {
+            return new ie.XMLHttpRequest
+        } catch (e) {}
+    };
+    var Yt = {
+            0: 200,
+            1223: 204
+        },
+        Qt = ce.ajaxSettings.xhr();
+    le.cors = !!Qt && "withCredentials" in Qt, le.ajax = Qt = !!Qt, ce.ajaxTransport(function(i) {
+        var o, a;
+        if (le.cors || Qt && !i.crossDomain) return {
+            send: function(e, t) {
+                var n, r = i.xhr();
+                if (r.open(i.type, i.url, i.async, i.username, i.password), i.xhrFields)
+                    for (n in i.xhrFields) r[n] = i.xhrFields[n];
+                for (n in i.mimeType && r.overrideMimeType && r.overrideMimeType(i.mimeType), i.crossDomain || e["X-Requested-With"] || (e["X-Requested-With"] = "XMLHttpRequest"), e) r.setRequestHeader(n, e[n]);
+                o = function(e) {
+                    return function() {
+                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(Yt[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
+                            binary: r.response
+                        } : {
+                            text: r.responseText
+                        }, r.getAllResponseHeaders()))
+                    }
+                }, r.onload = o(), a = r.onerror = r.ontimeout = o("error"), void 0 !== r.onabort ? r.onabort = a : r.onreadystatechange = function() {
+                    4 === r.readyState && ie.setTimeout(function() {
+                        o && a()
+                    })
+                }, o = o("abort");
+                try {
+                    r.send(i.hasContent && i.data || null)
+                } catch (e) {
+                    if (o) throw e
+                }
+            },
+            abort: function() {
+                o && o()
+            }
+        }
+    }), ce.ajaxPrefilter(function(e) {
+        e.crossDomain && (e.contents.script = !1)
+    }), ce.ajaxSetup({
+        accepts: {
+            script: "text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"
+        },
+        contents: {
+            script: /\b(?:java|ecma)script\b/
+        },
+        converters: {
+            "text script": function(e) {
+                return ce.globalEval(e), e
+            }
+        }
+    }), ce.ajaxPrefilter("script", function(e) {
+        void 0 === e.cache && (e.cache = !1), e.crossDomain && (e.type = "GET")
+    }), ce.ajaxTransport("script", function(n) {
+        var r, i;
+        if (n.crossDomain || n.scriptAttrs) return {
+            send: function(e, t) {
+                r = ce("<script>").attr(n.scriptAttrs || {}).prop({
+                    charset: n.scriptCharset,
+                    src: n.url
+                }).on("load error", i = function(e) {
+                    r.remove(), i = null, e && t("error" === e.type ? 404 : 200, e.type)
+                }), C.head.appendChild(r[0])
+            },
+            abort: function() {
+                i && i()
+            }
+        }
+    });
+    var Jt, Kt = [],
+        Zt = /(=)\?(?=&|$)|\?\?/;
+    ce.ajaxSetup({
+        jsonp: "callback",
+        jsonpCallback: function() {
+            var e = Kt.pop() || ce.expando + "_" + jt.guid++;
+            return this[e] = !0, e
+        }
+    }), ce.ajaxPrefilter("json jsonp", function(e, t, n) {
+        var r, i, o, a = !1 !== e.jsonp && (Zt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Zt.test(e.data) && "data");
+        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = v(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Zt, "$1" + r) : !1 !== e.jsonp && (e.url += (At.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
+            return o || ce.error(r + " was not called"), o[0]
+        }, e.dataTypes[0] = "json", i = ie[r], ie[r] = function() {
+            o = arguments
+        }, n.always(function() {
+            void 0 === i ? ce(ie).removeProp(r) : ie[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, Kt.push(r)), o && v(i) && i(o[0]), o = i = void 0
+        }), "script"
+    }), le.createHTMLDocument = ((Jt = C.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Jt.childNodes.length), ce.parseHTML = function(e, t, n) {
+        return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (le.createHTMLDocument ? ((r = (t = C.implementation.createHTMLDocument("")).createElement("base")).href = C.location.href, t.head.appendChild(r)) : t = C), o = !n && [], (i = w.exec(e)) ? [t.createElement(i[1])] : (i = Ae([e], t, o), o && o.length && ce(o).remove(), ce.merge([], i.childNodes)));
+        var r, i, o
+    }, ce.fn.load = function(e, t, n) {
+        var r, i, o, a = this,
+            s = e.indexOf(" ");
+        return -1 < s && (r = Tt(e.slice(s)), e = e.slice(0, s)), v(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && ce.ajax({
+            url: e,
+            type: i || "GET",
+            dataType: "html",
+            data: t
+        }).done(function(e) {
+            o = arguments, a.html(r ? ce("<div>").append(ce.parseHTML(e)).find(r) : e)
+        }).always(n && function(e, t) {
+            a.each(function() {
+                n.apply(this, o || [e.responseText, t, e])
+            })
+        }), this
+    }, ce.expr.pseudos.animated = function(t) {
+        return ce.grep(ce.timers, function(e) {
+            return t === e.elem
+        }).length
+    }, ce.offset = {
+        setOffset: function(e, t, n) {
+            var r, i, o, a, s, u, l = ce.css(e, "position"),
+                c = ce(e),
+                f = {};
+            "static" === l && (e.style.position = "relative"), s = c.offset(), o = ce.css(e, "top"), u = ce.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), v(t) && (t = t.call(e, n, ce.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : c.css(f)
+        }
+    }, ce.fn.extend({
+        offset: function(t) {
+            if (arguments.length) return void 0 === t ? this : this.each(function(e) {
+                ce.offset.setOffset(this, t, e)
+            });
+            var e, n, r = this[0];
+            return r ? r.getClientRects().length ? (e = r.getBoundingClientRect(), n = r.ownerDocument.defaultView, {
+                top: e.top + n.pageYOffset,
+                left: e.left + n.pageXOffset
+            }) : {
+                top: 0,
+                left: 0
+            } : void 0
+        },
+        position: function() {
+            if (this[0]) {
+                var e, t, n, r = this[0],
+                    i = {
+                        top: 0,
+                        left: 0
+                    };
+                if ("fixed" === ce.css(r, "position")) t = r.getBoundingClientRect();
+                else {
+                    t = this.offset(), n = r.ownerDocument, e = r.offsetParent || n.documentElement;
+                    while (e && (e === n.body || e === n.documentElement) && "static" === ce.css(e, "position")) e = e.parentNode;
+                    e && e !== r && 1 === e.nodeType && ((i = ce(e).offset()).top += ce.css(e, "borderTopWidth", !0), i.left += ce.css(e, "borderLeftWidth", !0))
+                }
+                return {
+                    top: t.top - i.top - ce.css(r, "marginTop", !0),
+                    left: t.left - i.left - ce.css(r, "marginLeft", !0)
+                }
+            }
+        },
+        offsetParent: function() {
+            return this.map(function() {
+                var e = this.offsetParent;
+                while (e && "static" === ce.css(e, "position")) e = e.offsetParent;
+                return e || J
+            })
+        }
+    }), ce.each({
+        scrollLeft: "pageXOffset",
+        scrollTop: "pageYOffset"
+    }, function(t, i) {
+        var o = "pageYOffset" === i;
+        ce.fn[t] = function(e) {
+            return M(this, function(e, t, n) {
+                var r;
+                if (y(e) ? r = e : 9 === e.nodeType && (r = e.defaultView), void 0 === n) return r ? r[i] : e[t];
+                r ? r.scrollTo(o ? r.pageXOffset : n, o ? n : r.pageYOffset) : e[t] = n
+            }, t, e, arguments.length)
+        }
+    }), ce.each(["top", "left"], function(e, n) {
+        ce.cssHooks[n] = Ye(le.pixelPosition, function(e, t) {
+            if (t) return t = Ge(e, n), _e.test(t) ? ce(e).position()[n] + "px" : t
+        })
+    }), ce.each({
+        Height: "height",
+        Width: "width"
+    }, function(a, s) {
+        ce.each({
+            padding: "inner" + a,
+            content: s,
+            "": "outer" + a
+        }, function(r, o) {
+            ce.fn[o] = function(e, t) {
+                var n = arguments.length && (r || "boolean" != typeof e),
+                    i = r || (!0 === e || !0 === t ? "margin" : "border");
+                return M(this, function(e, t, n) {
+                    var r;
+                    return y(e) ? 0 === o.indexOf("outer") ? e["inner" + a] : e.document.documentElement["client" + a] : 9 === e.nodeType ? (r = e.documentElement, Math.max(e.body["scroll" + a], r["scroll" + a], e.body["offset" + a], r["offset" + a], r["client" + a])) : void 0 === n ? ce.css(e, t, i) : ce.style(e, t, n, i)
+                }, s, n ? e : void 0, n)
+            }
+        })
+    }), ce.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(e, t) {
+        ce.fn[t] = function(e) {
+            return this.on(t, e)
+        }
+    }), ce.fn.extend({
+        bind: function(e, t, n) {
+            return this.on(e, null, t, n)
+        },
+        unbind: function(e, t) {
+            return this.off(e, null, t)
+        },
+        delegate: function(e, t, n, r) {
+            return this.on(t, e, n, r)
+        },
+        undelegate: function(e, t, n) {
+            return 1 === arguments.length ? this.off(e, "**") : this.off(t, e || "**", n)
+        },
+        hover: function(e, t) {
+            return this.on("mouseenter", e).on("mouseleave", t || e)
+        }
+    }), ce.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(e, n) {
+        ce.fn[n] = function(e, t) {
+            return 0 < arguments.length ? this.on(n, null, e, t) : this.trigger(n)
+        }
+    });
+    var en = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
+    ce.proxy = function(e, t) {
+        var n, r, i;
+        if ("string" == typeof t && (n = e[t], t = e, e = n), v(e)) return r = ae.call(arguments, 2), (i = function() {
+            return e.apply(t || this, r.concat(ae.call(arguments)))
+        }).guid = e.guid = e.guid || ce.guid++, i
+    }, ce.holdReady = function(e) {
+        e ? ce.readyWait++ : ce.ready(!0)
+    }, ce.isArray = Array.isArray, ce.parseJSON = JSON.parse, ce.nodeName = fe, ce.isFunction = v, ce.isWindow = y, ce.camelCase = F, ce.type = x, ce.now = Date.now, ce.isNumeric = function(e) {
+        var t = ce.type(e);
+        return ("number" === t || "string" === t) && !isNaN(e - parseFloat(e))
+    }, ce.trim = function(e) {
+        return null == e ? "" : (e + "").replace(en, "$1")
+    }, "function" == typeof define && define.amd && define("jquery", [], function() {
+        return ce
+    });
+    var tn = ie.jQuery,
+        nn = ie.$;
+    return ce.noConflict = function(e) {
+        return ie.$ === ce && (ie.$ = nn), e && ie.jQuery === ce && (ie.jQuery = tn), ce
+    }, "undefined" == typeof e && (ie.jQuery = ie.$ = ce), ce
 });
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/static/loading.gif` & `bride-of-frankensystem-1.9.3.4/BOFS/static/loading.gif`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/static/style.css` & `bride-of-frankensystem-1.9.3.4/BOFS/static/style.css`

 * *Files 4% similar despite different names*

```diff
@@ -105,17 +105,18 @@
 .slider-labels {
     display: flex;
     align-items: flex-start;
     justify-content: space-between;
 }
 
 .error-box {
-    padding: 5px;
+    padding: 1em;
     margin: 5px;
     border: 1px solid rgba(0, 0, 0, 0.33);
+    border-left-width: 3px;
     background-color: rgba(255, 0, 0, 0.05);
 }
 
 
 .debug-session pre {
     display: block; margin: 0;
 }
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/templates/consent.html` & `bride-of-frankensystem-1.9.3.4/BOFS/templates/consent.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/templates/end.html` & `bride-of-frankensystem-1.9.3.4/BOFS/templates/end.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/templates/external_id.html` & `bride-of-frankensystem-1.9.3.4/BOFS/admin/templates/login_admin.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,55 @@
-00000000: 7b25 2065 7874 656e 6473 2022 7465 6d70  {% extends "temp
-00000010: 6c61 7465 2e68 746d 6c22 2025 7d0d 0a7b  late.html" %}..{
-00000020: 2520 626c 6f63 6b20 6865 6164 2025 7d0d  % block head %}.
-00000030: 0a7b 2520 656e 6462 6c6f 636b 2025 7d0d  .{% endblock %}.
-00000040: 0a0d 0a7b 2520 626c 6f63 6b20 636f 6e74  ...{% block cont
-00000050: 656e 7420 257d 0d0a 0d0a 2020 2020 2020  ent %}....      
-00000060: 2020 3c66 6f72 6d20 6964 3d22 666f 726d    <form id="form
-00000070: 2220 6d65 7468 6f64 3d22 706f 7374 223e  " method="post">
-00000080: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00000090: 3c69 3e57 656c 636f 6d65 2120 506c 6561  <i>Welcome! Plea
-000000a0: 7365 2066 696c 6c20 6f75 7420 7468 6520  se fill out the 
-000000b0: 666f 6c6c 6f77 696e 6720 696e 666f 726d  following inform
-000000c0: 6174 696f 6e20 746f 2062 6567 696e 2e3c  ation to begin.<
-000000d0: 2f69 3e3c 6272 3e0d 0a0d 0a20 2020 2020  /i><br>....     
-000000e0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000000f0: 733d 2271 7565 7374 696f 6e22 2073 7479  s="question" sty
-00000100: 6c65 3d22 223e 0d0a 2020 2020 2020 2020  le="">..        
-00000110: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00000120: 7373 3d22 7061 6464 696e 6722 3e0d 0a20  ss="padding">.. 
-00000130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000140: 2020 203c 6833 3e50 6c65 6173 6520 656e     <h3>Please en
-00000150: 7465 7220 796f 7572 207b 7b20 636f 6e66  ter your {{ conf
-00000160: 6967 5b27 4558 5445 524e 414c 5f49 445f  ig['EXTERNAL_ID_
-00000170: 4c41 4245 4c27 5d20 7d7d 2e3c 2f68 333e  LABEL'] }}.</h3>
-00000180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000190: 2020 2020 2020 3c64 6976 3e0d 0a20 2020        <div>..   
-000001a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001b0: 2020 2020 203c 696e 7075 7420 636c 6173       <input clas
-000001c0: 733d 2266 6f72 6d2d 636f 6e74 726f 6c22  s="form-control"
-000001d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000001e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001f0: 2074 7970 653d 2274 6578 7422 0d0a 2020   type="text"..  
-00000200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000210: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00000220: 653d 226d 5475 726b 4944 220d 0a20 2020  e="mTurkID"..   
-00000230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000240: 2020 2020 2020 2020 2020 2020 6964 3d22              id="
-00000250: 6d54 7572 6b49 4422 0d0a 2020 2020 2020  mTurkID"..      
-00000260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000270: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00000280: 7769 6474 683a 2033 3030 7078 3b22 0d0a  width: 300px;"..
-00000290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000002b0: 6c61 6365 686f 6c64 6572 3d22 220d 0a20  laceholder="".. 
-000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002d0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-000002e0: 2069 6620 6d54 7572 6b49 4420 213d 204e   if mTurkID != N
-000002f0: 6f6e 6520 257d 0d0a 2020 2020 2020 2020  one %}..        
-00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000310: 2020 2020 2020 2076 616c 7565 3d22 7b7b         value="{{
-00000320: 6d54 7572 6b49 447d 7d22 0d0a 2020 2020  mTurkID}}"..    
-00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000340: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00000350: 6469 6620 257d 0d0a 2020 2020 2020 2020  dif %}..        
-00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000370: 2020 2020 2020 2072 6571 7569 7265 6420         required 
-00000380: 2f3e 0d0a 2020 2020 2020 2020 2020 2020  />..            
-00000390: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-000003a0: 2063 6c61 7373 3d22 696e 7661 6c69 642d   class="invalid-
-000003b0: 6665 6564 6261 636b 223e 0d0a 2020 2020  feedback">..    
-000003c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003d0: 2020 2020 2020 2020 7b7b 2063 6f6e 6669          {{ confi
-000003e0: 675b 2745 5854 4552 4e41 4c5f 4944 5f50  g['EXTERNAL_ID_P
-000003f0: 524f 4d50 5427 5d20 7d7d 0d0a 2020 2020  ROMPT'] }}..    
-00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000410: 2020 2020 3c2f 6469 763e 0d0a 2020 2020      </div>..    
-00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000430: 3c2f 6469 763e 0d0a 2020 2020 2020 2020  </div>..        
-00000440: 2020 2020 2020 2020 3c2f 6469 763e 0d0a          </div>..
-00000450: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00000460: 763e 0d0a 0d0a 2020 2020 2020 2020 7b7b  v>....        {{
-00000470: 2062 746e 436f 6e74 696e 7565 2829 207d   btnContinue() }
-00000480: 7d0d 0a0d 0a20 2020 2020 2020 203c 2f66  }....        </f
-00000490: 6f72 6d3e 0d0a 7b25 2065 6e64 626c 6f63  orm>..{% endbloc
-000004a0: 6b20 257d                                k %}
+00000000: 3c21 444f 4354 5950 4520 6874 6d6c 3e0d  <!DOCTYPE html>.
+00000010: 0a3c 6874 6d6c 3e0d 0a3c 6865 6164 3e0d  .<html>..<head>.
+00000020: 0a20 2020 207b 2520 696e 636c 7564 6520  .    {% include 
+00000030: 2274 656d 706c 6174 655f 6164 6d69 6e5f  "template_admin_
+00000040: 6865 6164 2e68 746d 6c22 2025 7d0d 0a3c  head.html" %}..<
+00000050: 2f68 6561 643e 0d0a 3c62 6f64 7920 7374  /head>..<body st
+00000060: 796c 653d 2270 6164 6469 6e67 3a20 3635  yle="padding: 65
+00000070: 7078 2032 3070 7820 3230 7078 2032 3070  px 20px 20px 20p
+00000080: 7822 2063 6c61 7373 3d22 642d 666c 6578  x" class="d-flex
+00000090: 2061 6c69 676e 2d69 7465 6d73 2d63 656e   align-items-cen
+000000a0: 7465 7222 3e0d 0a3c 6d61 696e 2063 6c61  ter">..<main cla
+000000b0: 7373 3d22 6d2d 6175 746f 223e 0d0a 2020  ss="m-auto">..  
+000000c0: 2020 3c66 6f72 6d20 6d65 7468 6f64 3d22    <form method="
+000000d0: 706f 7374 2220 7374 796c 653d 226d 696e  post" style="min
+000000e0: 2d77 6964 7468 3a20 3430 3070 783b 223e  -width: 400px;">
+000000f0: 0d0a 2020 2020 2020 2020 3c68 313e 7b7b  ..        <h1>{{
+00000100: 2063 6f6e 6669 675b 2754 4954 4c45 275d   config['TITLE']
+00000110: 207d 7d3c 2f68 313e 0d0a 2020 2020 2020   }}</h1>..      
+00000120: 2020 7b25 2069 6620 6d65 7373 6167 6520    {% if message 
+00000130: 257d 0d0a 2020 2020 2020 2020 2020 2020  %}..            
+00000140: 3c64 6976 2063 6c61 7373 3d22 6572 726f  <div class="erro
+00000150: 722d 626f 7822 3e0d 0a20 2020 2020 2020  r-box">..       
+00000160: 2020 2020 2020 2020 203c 693e 7b7b 206d           <i>{{ m
+00000170: 6573 7361 6765 207d 7d3c 2f69 3e0d 0a20  essage }}</i>.. 
+00000180: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00000190: 3e0d 0a20 2020 2020 2020 207b 2520 656e  >..        {% en
+000001a0: 6469 6620 257d 0d0a 0d0a 2020 2020 2020  dif %}....      
+000001b0: 2020 3c68 343e 506c 6561 7365 2073 6967    <h4>Please sig
+000001c0: 6e20 696e 3c2f 6834 3e0d 0a0d 0a20 2020  n in</h4>....   
+000001d0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000001e0: 2262 672d 626f 6479 2d74 6572 7469 6172  "bg-body-tertiar
+000001f0: 7920 702d 3320 726f 756e 6465 6422 3e0d  y p-3 rounded">.
+00000200: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
+00000210: 7620 636c 6173 733d 226d 622d 3322 3e0d  v class="mb-3">.
+00000220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000230: 203c 6c61 6265 6c20 666f 723d 2270 6173   <label for="pas
+00000240: 7377 6f72 6422 2063 6c61 7373 3d22 666f  sword" class="fo
+00000250: 726d 2d6c 6162 656c 223e 5061 7373 776f  rm-label">Passwo
+00000260: 7264 3c2f 6c61 6265 6c3e 0d0a 2020 2020  rd</label>..    
+00000270: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
+00000280: 7574 2074 7970 653d 2270 6173 7377 6f72  ut type="passwor
+00000290: 6422 2063 6c61 7373 3d22 666f 726d 2d63  d" class="form-c
+000002a0: 6f6e 7472 6f6c 2220 6e61 6d65 3d22 7061  ontrol" name="pa
+000002b0: 7373 776f 7264 2220 6964 3d22 7061 7373  ssword" id="pass
+000002c0: 776f 7264 223e 0d0a 2020 2020 2020 2020  word">..        
+000002d0: 2020 2020 3c2f 6469 763e 0d0a 2020 2020      </div>..    
+000002e0: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
+000002f0: 7970 653d 2273 7562 6d69 7422 2069 643d  ype="submit" id=
+00000300: 2273 7562 6d69 7422 2076 616c 7565 3d22  "submit" value="
+00000310: 4c6f 6769 6e22 2063 6c61 7373 3d22 6274  Login" class="bt
+00000320: 6e20 6274 6e2d 7072 696d 6172 7920 772d  n btn-primary w-
+00000330: 3130 3022 3e0d 0a20 2020 2020 2020 203c  100">..        <
+00000340: 2f64 6976 3e0d 0a20 2020 203c 2f66 6f72  /div>..    </for
+00000350: 6d3e 0d0a 3c2f 6d61 696e 3e0d 0a3c 2f62  m>..</main>..</b
+00000360: 6f64 793e 0d0a 3c2f 6874 6d6c 3e         ody>..</html>
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/templates/questionnaire_macro.html` & `bride-of-frankensystem-1.9.3.4/BOFS/templates/questionnaire_macro.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/radiogrid.html` & `bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/radiogrid.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/radiolist.html` & `bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/radiolist.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/templates/questions/slider.html` & `bride-of-frankensystem-1.9.3.4/BOFS/templates/questions/slider.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/templates/template.html` & `bride-of-frankensystem-1.9.3.4/BOFS/templates/template.html`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,22 @@
         </div>
     {% endif %}
 {%- endmacro %}
 <!DOCTYPE html>
 <html>
 <head>
     <title>{% block title %}{{ config['TITLE'] }}{% endblock %}</title>
-    <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.9.0/css/all.min.css" integrity="sha256-UzFD2WYH2U1dQpKDjjZK72VtPeWP50NoJjd26rnAdUI=" crossorigin="anonymous" />
-    <link rel="stylesheet" href="{{ url_for('BOFS_static', filename='style.css') }}" type="text/css" />
+    <link rel="stylesheet" href="{{ url_for('BOFS_static', filename='bootstrap.min.css') }}">
+    <link rel="stylesheet" href="{{ url_for('BOFS_static', filename='style.css') }}">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9/2PkPKZ5QiAj6Ta86w+fsb2TkcmfRyVX3pBnMFcV7oQPJkl9QevSCWr3W6A==" crossorigin="anonymous" referrerpolicy="no-referrer" />
 
-    <script src="{{ url_for('BOFS_static', filename='js/jquery-3.4.1.min.js') }}"></script>
-    <script src="{{ url_for('BOFS_static', filename='js/popper.min.js') }}"></script>
-    <script src="{{ url_for('BOFS_static', filename='js/bootstrap.min.js') }}"></script>
-    <script src="https://unpkg.com/htmx.org@1.9.11"></script>
-    <script src="https://unpkg.com/htmx.org@1.9.11/dist/ext/json-enc.js"></script>
+    <script src="{{ url_for('BOFS_static', filename='js/jquery-3.7.1.min.js') }}"></script>
+    <script src="{{ url_for('BOFS_static', filename='js/bootstrap.bundle.min.js') }}"></script>
+    <script src="{{ url_for('BOFS_static', filename='js/htmx.min.js') }}"></script>
+    <script src="{{ url_for('BOFS_static', filename='js/json-enc.js') }}"></script>
 
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     {% block head %}{% endblock %}
 </head>
 <body>
 
 <div class="title-bar">
```

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/templates/unity_webgl.html` & `bride-of-frankensystem-1.9.3.4/BOFS/templates/unity_webgl.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/templates/unity_webgl_fullscreen.html` & `bride-of-frankensystem-1.9.3.4/BOFS/templates/unity_webgl_fullscreen.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/BOFS/util.py` & `bride-of-frankensystem-1.9.3.4/BOFS/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,21 +216,29 @@
         return None  # This is almost definitely a "Working outside of request context" error
 
 
 def fetch_condition_count():
     return len(current_app.config["CONDITIONS"])
 
 
-# This is useful only after data has been collected.
 def fetch_condition_count_db():
+    """
+    This is useful only after data has been collected.
+    :return:
+    """
     return db.session.query(db.func.max(db.Participant.condition)).one()[0]
 
 
-# This needs to be used inside of a route, otherwise session, request won't work.
-def provide_consent(assignCondition=True, logDisplaySize=True):
+def provide_consent(assignCondition=True, logDisplaySize=False):
+    """
+    This needs to be used inside a route, otherwise session, request won't work.
+    :param assignCondition:
+    :param logDisplaySize:
+    :return:
+    """
     from flask import request, session
     from BOFS.globals import db
     import datetime
 
     p = db.Participant()
     ip_address = request.headers.get('X-Real-IP')
 
@@ -267,14 +275,16 @@
         entry.screenHeight = request.form['screenHeight']
         entry.innerWidth = request.form['innerWidth']
         entry.innerHeight = request.form['innerHeight']
 
         db.session.add(entry)
         db.session.commit()
 
+    return p
+
 
 # Provides some error checking for when converting results of form submission
 def float_or_0(value):
     value = float(value)
 
     if math.isnan(value):
         return 0.0
```

### Comparing `bride-of-frankensystem-1.9.3.3/LICENSE` & `bride-of-frankensystem-1.9.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/PKG-INFO` & `bride-of-frankensystem-1.9.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bride-of-frankensystem
-Version: 1.9.3.3
+Version: 1.9.3.4
 Summary: A framework that allows for the development of custom online experiments and surveys.
 Author-email: Colby Johanson <colby.johanson@usask.ca>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bride-of-frankensystem-1.9.3.3/README.md` & `bride-of-frankensystem-1.9.3.4/README.md`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.3/bride_of_frankensystem.egg-info/PKG-INFO` & `bride-of-frankensystem-1.9.3.4/bride_of_frankensystem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bride-of-frankensystem
-Version: 1.9.3.3
+Version: 1.9.3.4
 Summary: A framework that allows for the development of custom online experiments and surveys.
 Author-email: Colby Johanson <colby.johanson@usask.ca>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bride-of-frankensystem-1.9.3.3/bride_of_frankensystem.egg-info/SOURCES.txt` & `bride-of-frankensystem-1.9.3.4/bride_of_frankensystem.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,41 +9,54 @@
 BOFS/PageList.py
 BOFS/__init__.py
 BOFS/__main__.py
 BOFS/cli.py
 BOFS/create_app.py
 BOFS/globals.py
 BOFS/util.py
+BOFS/__pycache__/BOFSFlask.cpython-311.pyc
+BOFS/__pycache__/BOFSSession.cpython-311.pyc
+BOFS/__pycache__/JSONQuestionnaire.cpython-311.pyc
+BOFS/__pycache__/JSONTable.cpython-311.pyc
+BOFS/__pycache__/PageList.cpython-311.pyc
+BOFS/__pycache__/__init__.cpython-311.pyc
+BOFS/__pycache__/__main__.cpython-311.pyc
+BOFS/__pycache__/cli.cpython-311.pyc
+BOFS/__pycache__/create_app.cpython-311.pyc
+BOFS/__pycache__/globals.cpython-311.pyc
+BOFS/__pycache__/util.cpython-311.pyc
 BOFS/admin/QuestionnaireResults.py
 BOFS/admin/__init__.py
 BOFS/admin/export_helpers.py
 BOFS/admin/util.py
 BOFS/admin/views.py
 BOFS/admin/__pycache__/QuestionnaireResults.cpython-310.pyc
 BOFS/admin/__pycache__/QuestionnaireResults.cpython-311.pyc
 BOFS/admin/__pycache__/__init__.cpython-310.pyc
 BOFS/admin/__pycache__/__init__.cpython-311.pyc
 BOFS/admin/__pycache__/export_helpers.cpython-311.pyc
 BOFS/admin/__pycache__/util.cpython-310.pyc
 BOFS/admin/__pycache__/util.cpython-311.pyc
 BOFS/admin/__pycache__/views.cpython-310.pyc
 BOFS/admin/__pycache__/views.cpython-311.pyc
+BOFS/admin/templates/database_delete.html
 BOFS/admin/templates/export.html
 BOFS/admin/templates/export_csv.html
 BOFS/admin/templates/login_admin.html
 BOFS/admin/templates/preview_questionnaire.html
 BOFS/admin/templates/preview_questionnaire_simple.html
 BOFS/admin/templates/progress.html
 BOFS/admin/templates/progress_ajax.html
 BOFS/admin/templates/progress_summary_ajax.html
 BOFS/admin/templates/questionnaire_results.html
 BOFS/admin/templates/results.html
 BOFS/admin/templates/table_ajax.html
 BOFS/admin/templates/table_view.html
 BOFS/admin/templates/template_admin.html
+BOFS/admin/templates/template_admin_head.html
 BOFS/bride_of_frankensystem.egg-info/PKG-INFO
 BOFS/bride_of_frankensystem.egg-info/SOURCES.txt
 BOFS/bride_of_frankensystem.egg-info/dependency_links.txt
 BOFS/bride_of_frankensystem.egg-info/entry_points.txt
 BOFS/bride_of_frankensystem.egg-info/requires.txt
 BOFS/bride_of_frankensystem.egg-info/top_level.txt
 BOFS/default/__init__.py
@@ -51,23 +64,26 @@
 BOFS/default/views.py
 BOFS/default/__pycache__/__init__.cpython-310.pyc
 BOFS/default/__pycache__/__init__.cpython-311.pyc
 BOFS/default/__pycache__/models.cpython-310.pyc
 BOFS/default/__pycache__/models.cpython-311.pyc
 BOFS/default/__pycache__/views.cpython-310.pyc
 BOFS/default/__pycache__/views.cpython-311.pyc
+BOFS/static/all.min.css
+BOFS/static/bootstrap.min.css
 BOFS/static/loading.gif
 BOFS/static/logo.png
 BOFS/static/style.css
+BOFS/static/style_admin.css
 BOFS/static/img/check.png
 BOFS/static/img/spinner32.gif
-BOFS/static/js/bootstrap.min.js
-BOFS/static/js/jquery-3.4.1.min.js
-BOFS/static/js/plotly-latest.min.js
-BOFS/static/js/popper.min.js
+BOFS/static/js/bootstrap.bundle.min.js
+BOFS/static/js/htmx.min.js
+BOFS/static/js/jquery-3.7.1.min.js
+BOFS/static/js/json-enc.js
 BOFS/templates/consent.html
 BOFS/templates/end.html
 BOFS/templates/external_id.html
 BOFS/templates/instructions.html
 BOFS/templates/questionnaire.html
 BOFS/templates/questionnaire_macro.html
 BOFS/templates/simple.html
```

### Comparing `bride-of-frankensystem-1.9.3.3/pyproject.toml` & `bride-of-frankensystem-1.9.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bride-of-frankensystem"
-version = "1.9.3.3"
+version = "1.9.3.4"
 description = "A framework that allows for the development of custom online experiments and surveys."
 readme = "README.md"
 authors = [{ name = "Colby Johanson", email = "colby.johanson@usask.ca" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Programming Language :: Python",
```

