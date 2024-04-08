# Comparing `tmp/django-codenerix-email-4.0.3.tar.gz` & `tmp/django-codenerix-email-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-codenerix-email-4.0.3.tar", last modified: Wed Feb  7 09:57:34 2024, max compression
+gzip compressed data, was "django-codenerix-email-4.0.4.tar", last modified: Mon Apr  8 11:05:01 2024, max compression
```

## Comparing `django-codenerix-email-4.0.3.tar` & `django-codenerix-email-4.0.4.tar`

### file list

```diff
@@ -1,74 +1,84 @@
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-02-07 09:57:34.854020 django-codenerix-email-4.0.3/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11357 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/LICENSE
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      247 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/MANIFEST.in
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-02-07 09:57:34.854020 django-codenerix-email-4.0.3/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1344 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/README.rst
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-02-07 09:57:34.850020 django-codenerix-email-4.0.3/codenerix_email/
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-02-07 09:56:08.000000 django-codenerix-email-4.0.3/codenerix_email/__init__.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1208 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/admin.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      149 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/apps.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3157 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/forms.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-02-07 09:57:34.850020 django-codenerix-email-4.0.3/codenerix_email/management/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/management/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-02-07 09:57:34.850020 django-codenerix-email-4.0.3/codenerix_email/management/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2023-10-27 11:25:38.000000 django-codenerix-email-4.0.3/codenerix_email/management/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      160 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/management/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/management/__pycache__/__init__.cpython-39.pyc
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-02-07 09:57:34.850020 django-codenerix-email-4.0.3/codenerix_email/management/commands/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/management/commands/__init__.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5603 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/management/commands/send_emails.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1645 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/management/commands/test_email.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-02-07 09:57:34.850020 django-codenerix-email-4.0.3/codenerix_email/migrations/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3511 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/0001_initial.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2369 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/0002_auto_20170502_1043.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      656 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/0003_auto_20170921_1206.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      486 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/0004_auto_20171108_1628.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      495 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/0005_emailmessage_retries.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      489 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/0006_emailmessage_error.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      602 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/0007_emailmessage_next_retry.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      731 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/0008_auto_20171201_0928.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-02-07 09:57:34.854020 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2005 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2373 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2020 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1500 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1692 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1515 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      694 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      782 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      709 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      676 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      713 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      728 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      706 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      675 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      712 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      690 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      802 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      854 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      817 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      779 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      839 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      794 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      151 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      147 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    12659 2023-12-18 05:48:25.000000 django-codenerix-email-4.0.3/codenerix_email/models.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-02-07 09:57:34.850020 django-codenerix-email-4.0.3/codenerix_email/static/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-02-07 09:57:34.850020 django-codenerix-email-4.0.3/codenerix_email/static/codenerix_email/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-02-07 09:57:34.854020 django-codenerix-email-4.0.3/codenerix_email/static/codenerix_email/partials/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      994 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2595 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.3/codenerix_email/urls.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3804 2024-02-07 09:54:44.000000 django-codenerix-email-4.0.3/codenerix_email/views.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-02-07 09:57:34.854020 django-codenerix-email-4.0.3/django_codenerix_email.egg-info/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-02-07 09:57:34.000000 django-codenerix-email-4.0.3/django_codenerix_email.egg-info/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3465 2024-02-07 09:57:34.000000 django-codenerix-email-4.0.3/django_codenerix_email.egg-info/SOURCES.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-02-07 09:57:34.000000 django-codenerix-email-4.0.3/django_codenerix_email.egg-info/dependency_links.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/django_codenerix_email.egg-info/not-zip-safe
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       45 2024-02-07 09:57:34.000000 django-codenerix-email-4.0.3/django_codenerix_email.egg-info/requires.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       16 2024-02-07 09:57:34.000000 django-codenerix-email-4.0.3/django_codenerix_email.egg-info/top_level.txt
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-02-07 09:57:34.854020 django-codenerix-email-4.0.3/setup.cfg
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1698 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.3/setup.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11339 2024-03-27 07:06:52.000000 django-codenerix-email-4.0.4/LICENSE
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      247 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/MANIFEST.in
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1344 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/README.rst
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.040900 django-codenerix-email-4.0.4/codenerix_email/
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/codenerix_email/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1208 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/admin.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      149 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/apps.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3157 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/forms.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.040900 django-codenerix-email-4.0.4/codenerix_email/management/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/management/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.044900 django-codenerix-email-4.0.4/codenerix_email/management/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2023-10-27 11:25:38.000000 django-codenerix-email-4.0.4/codenerix_email/management/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-26 06:56:17.000000 django-codenerix-email-4.0.4/codenerix_email/management/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      160 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/management/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/management/__pycache__/__init__.cpython-39.pyc
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.044900 django-codenerix-email-4.0.4/codenerix_email/management/commands/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/management/commands/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5603 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/management/commands/send_emails.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1645 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/management/commands/test_email.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.044900 django-codenerix-email-4.0.4/codenerix_email/migrations/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3511 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0001_initial.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2369 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0002_auto_20170502_1043.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      656 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0003_auto_20170921_1206.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      486 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0004_auto_20171108_1628.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      495 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0005_emailmessage_retries.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      489 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0006_emailmessage_error.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      602 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0007_emailmessage_next_retry.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      731 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0008_auto_20171201_0928.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2005 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3682 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2373 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2020 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1500 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2664 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1692 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1515 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      694 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      967 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      782 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      709 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      676 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      939 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      713 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      954 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      728 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      706 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      675 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      938 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      712 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      690 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      802 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1111 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      854 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      817 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      779 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1178 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      839 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      794 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      151 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      147 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    12659 2024-04-08 11:00:35.000000 django-codenerix-email-4.0.4/codenerix_email/models.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.040900 django-codenerix-email-4.0.4/codenerix_email/static/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.040900 django-codenerix-email-4.0.4/codenerix_email/static/codenerix_email/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/codenerix_email/static/codenerix_email/partials/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      994 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2595 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/urls.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3804 2024-02-07 09:54:44.000000 django-codenerix-email-4.0.4/codenerix_email/views.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4221 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/SOURCES.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/dependency_links.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/not-zip-safe
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       53 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/requires.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       16 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/top_level.txt
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/setup.cfg
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1707 2024-04-08 11:04:22.000000 django-codenerix-email-4.0.4/setup.py
```

### Comparing `django-codenerix-email-4.0.3/LICENSE` & `django-codenerix-email-4.0.4/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright {yyyy} {name of copyright owner}
+   Copyright 2024 Codenerix
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `django-codenerix-email-4.0.3/PKG-INFO` & `django-codenerix-email-4.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-email
-Version: 4.0.3
+Version: 4.0.4
 Summary: Codenerix Email is a module that enables CODENERIX to set send emails in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-email
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,send email
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-email-4.0.3/README.rst` & `django-codenerix-email-4.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/admin.py` & `django-codenerix-email-4.0.4/codenerix_email/admin.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/forms.py` & `django-codenerix-email-4.0.4/codenerix_email/forms.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/management/commands/send_emails.py` & `django-codenerix-email-4.0.4/codenerix_email/management/commands/send_emails.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/management/commands/test_email.py` & `django-codenerix-email-4.0.4/codenerix_email/management/commands/test_email.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/0001_initial.py` & `django-codenerix-email-4.0.4/codenerix_email/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/0002_auto_20170502_1043.py` & `django-codenerix-email-4.0.4/codenerix_email/migrations/0002_auto_20170502_1043.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/0003_auto_20170921_1206.py` & `django-codenerix-email-4.0.4/codenerix_email/migrations/0003_auto_20170921_1206.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/0007_emailmessage_next_retry.py` & `django-codenerix-email-4.0.4/codenerix_email/migrations/0007_emailmessage_next_retry.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/0008_auto_20171201_0928.py` & `django-codenerix-email-4.0.4/codenerix_email/migrations/0008_auto_20171201_0928.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc` & `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/models.py` & `django-codenerix-email-4.0.4/codenerix_email/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from django.utils.translation import gettext_lazy as _
 from django.db import models
 from django.template import Context, Template
 from django.core.exceptions import ValidationError
 from django.conf import settings
 
 from codenerix.models import CodenerixModel
-from codenerix.lib.debugger import Debugger
+from codenerix_lib.debugger import Debugger
 from codenerix.lib.genmail import EmailMessage as EM, get_connection
 from codenerix.fields import WysiwygAngularField
 
 
 class EmailMessage(CodenerixModel, Debugger):
     efrom = models.EmailField(_("From"), blank=False, null=False)
     eto = models.EmailField(_("To"), blank=False, null=False)
```

### Comparing `django-codenerix-email-4.0.3/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html` & `django-codenerix-email-4.0.4/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/urls.py` & `django-codenerix-email-4.0.4/codenerix_email/urls.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/codenerix_email/views.py` & `django-codenerix-email-4.0.4/codenerix_email/views.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.3/django_codenerix_email.egg-info/PKG-INFO` & `django-codenerix-email-4.0.4/django_codenerix_email.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-email
-Version: 4.0.3
+Version: 4.0.4
 Summary: Codenerix Email is a module that enables CODENERIX to set send emails in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-email
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,send email
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-email-4.0.3/django_codenerix_email.egg-info/SOURCES.txt` & `django-codenerix-email-4.0.4/django_codenerix_email.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 codenerix_email/apps.py
 codenerix_email/forms.py
 codenerix_email/models.py
 codenerix_email/urls.py
 codenerix_email/views.py
 codenerix_email/management/__init__.py
 codenerix_email/management/__pycache__/__init__.cpython-310.pyc
+codenerix_email/management/__pycache__/__init__.cpython-311.pyc
 codenerix_email/management/__pycache__/__init__.cpython-35.pyc
 codenerix_email/management/__pycache__/__init__.cpython-39.pyc
 codenerix_email/management/commands/__init__.py
 codenerix_email/management/commands/send_emails.py
 codenerix_email/management/commands/test_email.py
 codenerix_email/migrations/0001_initial.py
 codenerix_email/migrations/0002_auto_20170502_1043.py
@@ -22,38 +23,47 @@
 codenerix_email/migrations/0004_auto_20171108_1628.py
 codenerix_email/migrations/0005_emailmessage_retries.py
 codenerix_email/migrations/0006_emailmessage_error.py
 codenerix_email/migrations/0007_emailmessage_next_retry.py
 codenerix_email/migrations/0008_auto_20171201_0928.py
 codenerix_email/migrations/__init__.py
 codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc
+codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc
 codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc
 codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc
 codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc
+codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc
 codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc
 codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc
 codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc
+codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc
 codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc
 codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc
 codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc
+codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc
 codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc
 codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc
 codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc
+codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc
 codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc
 codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc
 codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc
+codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc
 codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc
 codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc
 codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc
+codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc
 codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc
 codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc
 codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc
+codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc
 codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc
 codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc
 codenerix_email/migrations/__pycache__/__init__.cpython-310.pyc
+codenerix_email/migrations/__pycache__/__init__.cpython-311.pyc
 codenerix_email/migrations/__pycache__/__init__.cpython-35.pyc
 codenerix_email/migrations/__pycache__/__init__.cpython-39.pyc
 codenerix_email/static/codenerix_email/partials/emailmessages_rows.html
 django_codenerix_email.egg-info/PKG-INFO
 django_codenerix_email.egg-info/SOURCES.txt
 django_codenerix_email.egg-info/dependency_links.txt
 django_codenerix_email.egg-info/not-zip-safe
```

