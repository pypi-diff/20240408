# Comparing `tmp/django-import-export-4.0.0rc0.tar.gz` & `tmp/django-import-export-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-import-export-4.0.0rc0.tar", last modified: Wed Feb 14 15:15:40 2024, max compression
+gzip compressed data, was "django-import-export-4.0.0rc1.tar", last modified: Fri Mar 15 14:18:19 2024, max compression
```

## Comparing `django-import-export-4.0.0rc0.tar` & `django-import-export-4.0.0rc1.tar`

### file list

```diff
@@ -1,332 +1,332 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.164438 django-import-export-4.0.0rc0/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.124438 django-import-export-4.0.0rc0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.124438 django-import-export-4.0.0rc0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.124438 django-import-export-4.0.0rc0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-02-14 15:15:40.164438 django-import-export-4.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.164438 django-import-export-4.0.0rc0/django_import_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-02-14 15:15:40.000000 django-import-export-4.0.0rc0/django_import_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-02-14 15:15:40.000000 django-import-export-4.0.0rc0/django_import_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 15:15:40.000000 django-import-export-4.0.0rc0/django_import_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-14 15:15:40.000000 django-import-export-4.0.0rc0/django_import_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-14 15:15:40.000000 django-import-export-4.0.0rc0/django_import_export.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.132438 django-import-export-4.0.0rc0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.112438 django-import-export-4.0.0rc0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.132438 django-import-export-4.0.0rc0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/change-form-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/custom-export-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/custom-import-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/date-widget-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/django-import-export-change.png
--rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/django-import-export-export-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/django-import-export-import-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/django-import-export-import.png
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/export-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    33286 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/export_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/import-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/import_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/non-field-specific-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/_static/images/select-for-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/admin_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30548 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/api_admin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/api_fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/api_forms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/api_instance_loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/api_mixins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/api_resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/api_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/api_tmp_storages.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/api_widgets.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/bulk_import.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29325 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/export_workflow.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    10047 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.136438 django-import-export-4.0.0rc0/docs/image_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/image_src/export_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/image_src/import_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/import_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.136438 django-import-export-4.0.0rc0/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-14 15:15:39.000000 django-import-export-4.0.0rc0/import_export/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35020 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.136438 django-import-export-4.0.0rc0/import_export/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/formats/base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/instance_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.112438 django-import-export-4.0.0rc0/import_export/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.136438 django-import-export-4.0.0rc0/import_export/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.112438 django-import-export-4.0.0rc0/import_export/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.136438 django-import-export-4.0.0rc0/import_export/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.112438 django-import-export-4.0.0rc0/import_export/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.112438 django-import-export-4.0.0rc0/import_export/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.112438 django-import-export-4.0.0rc0/import_export/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.112438 django-import-export-4.0.0rc0/import_export/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/kz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.140438 django-import-export-4.0.0rc0/import_export/locale/kz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/kz/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/kz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.144438 django-import-export-4.0.0rc0/import_export/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.144438 django-import-export-4.0.0rc0/import_export/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.144438 django-import-export-4.0.0rc0/import_export/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.144438 django-import-export-4.0.0rc0/import_export/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.144438 django-import-export-4.0.0rc0/import_export/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.144438 django-import-export-4.0.0rc0/import_export/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.144438 django-import-export-4.0.0rc0/import_export/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    47866 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.144438 django-import-export-4.0.0rc0/import_export/static/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/static/import_export/export.css
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/static/import_export/export_selectable_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/static/import_export/guess_format.js
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/static/import_export/import.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.116438 django-import-export-4.0.0rc0/import_export/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.148438 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/change_list_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/change_list_export_item.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/change_list_import.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/change_list_import_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/change_list_import_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/export.html
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/import.html
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templates/admin/import_export/resource_fields_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.148438 django-import-export-4.0.0rc0/import_export/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/templatetags/import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21116 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/import_export/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.148438 django-import-export-4.0.0rc0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/runtests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/runtests.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 15:15:40.164438 django-import-export-4.0.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.148438 django-import-export-4.0.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/books-sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.148438 django-import-export-4.0.0rc0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.152438 django-import-export-4.0.0rc0/tests/core/exports/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/authors.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books-ISO-8859-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books-dos.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books-empty-author-email.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books-for-delete.csv
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books-invalid-date.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books-mac.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books-mac.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books-unicode.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books-unicode.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books.csv
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books.json
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books.xls
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/books.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/exports/child.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.152438 django-import-export-4.0.0rc0/tests/core/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/fixtures/author.json
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/fixtures/book.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/fixtures/category.json
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.156438 django-import-export-4.0.0rc0/tests/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0002_book_published_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0003_withfloatfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0004_bookwithchapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0005_addparentchild.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0006_auto_20171130_0147.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0007_auto_20180628_0411.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0008_auto_20190409_0846.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0009_auto_20211111_0807.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0010_uuidbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0012_delete_legacybook.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0013_alter_author_birthday.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/0014_bookwithchapternumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.120438 django-import-export-4.0.0rc0/tests/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.156438 django-import-export-4.0.0rc0/tests/core/templates/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.156438 django-import-export-4.0.0rc0/tests/core/templates/core/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/templates/core/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/templates/core/category_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.156438 django-import-export-4.0.0rc0/tests/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.160438 django-import-export-4.0.0rc0/tests/core/tests/admin_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/admin_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/admin_integration/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/admin_integration/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/admin_integration/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    39409 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/admin_integration/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/admin_integration/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_instance_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_invalidrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.160438 django-import-export-4.0.0rc0/tests/core/tests/test_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13918 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.164438 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)    27918 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/tests/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.120438 django-import-export-4.0.0rc0/tests/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.164438 django-import-export-4.0.0rc0/tests/docker/db/
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/docker/db/init-mysql-db.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/docker/db/init-postgres-db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:40.164438 django-import-export-4.0.0rc0/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/scripts/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-02-14 15:15:32.000000 django-import-export-4.0.0rc0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.288315 django-import-export-4.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.244315 django-import-export-4.0.0rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.244315 django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.244315 django-import-export-4.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-15 14:18:19.288315 django-import-export-4.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.284315 django-import-export-4.0.0rc1/django_import_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/django_import_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/django_import_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/django_import_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/django_import_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/django_import_export.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.252315 django-import-export-4.0.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.252315 django-import-export-4.0.0rc1/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/change-form-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/custom-export-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/custom-import-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/date-widget-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/django-import-export-change.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/django-import-export-export-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/django-import-export-import-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/django-import-export-import.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/export-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33286 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/export_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/import-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/import_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/non-field-specific-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/select-for-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/admin_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30548 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_forms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_instance_loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_tmp_storages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_widgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/bulk_import.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29802 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/export_workflow.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10047 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.252315 django-import-export-4.0.0rc1/docs/image_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/image_src/export_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/image_src/import_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/import_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/import_export/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35020 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/formats/base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/instance_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/kz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/kz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/kz/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/kz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48428 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/static/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/static/import_export/export.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/static/import_export/export_selectable_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/static/import_export/guess_format.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/static/import_export/import.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.268315 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/export.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/resource_fields_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.268315 django-import-export-4.0.0rc1/import_export/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templatetags/import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21360 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.268315 django-import-export-4.0.0rc1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/runtests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/runtests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 14:18:19.288315 django-import-export-4.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.268315 django-import-export-4.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/books-sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.268315 django-import-export-4.0.0rc1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.272315 django-import-export-4.0.0rc1/tests/core/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/authors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-ISO-8859-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-dos.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-empty-author-email.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-for-delete.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-invalid-date.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-mac.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-mac.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-unicode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-unicode.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/child.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.272315 django-import-export-4.0.0rc1/tests/core/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/fixtures/author.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/fixtures/book.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/fixtures/category.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.276315 django-import-export-4.0.0rc1/tests/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0002_book_published_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0003_withfloatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0004_bookwithchapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0005_addparentchild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0006_auto_20171130_0147.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0007_auto_20180628_0411.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0008_auto_20190409_0846.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0009_auto_20211111_0807.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0010_uuidbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0012_delete_legacybook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0013_alter_author_birthday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0014_bookwithchapternumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/tests/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.276315 django-import-export-4.0.0rc1/tests/core/templates/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.276315 django-import-export-4.0.0rc1/tests/core/templates/core/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/templates/core/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/templates/core/category_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.280315 django-import-export-4.0.0rc1/tests/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.280315 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39409 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_instance_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_invalidrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.280315 django-import-export-4.0.0rc1/tests/core/tests/test_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.284315 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28373 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.240315 django-import-export-4.0.0rc1/tests/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.284315 django-import-export-4.0.0rc1/tests/docker/db/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/docker/db/init-mysql-db.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/docker/db/init-postgres-db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.284315 django-import-export-4.0.0rc1/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/scripts/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tox.ini
```

### Comparing `django-import-export-4.0.0rc0/.github/ISSUE_TEMPLATE/bug_report.md` & `django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/.github/ISSUE_TEMPLATE/question.md` & `django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/.github/stale.yml` & `django-import-export-4.0.0rc1/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/.github/workflows/release.yml` & `django-import-export-4.0.0rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/.github/workflows/test.yml` & `django-import-export-4.0.0rc1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/AUTHORS` & `django-import-export-4.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/CODE_OF_CONDUCT.md` & `django-import-export-4.0.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/LICENSE` & `django-import-export-4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/Makefile` & `django-import-export-4.0.0rc1/Makefile`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/PKG-INFO` & `django-import-export-4.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.0rc0
+Version: 4.0.0rc1
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `django-import-export-4.0.0rc0/README.rst` & `django-import-export-4.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/RELEASE.md` & `django-import-export-4.0.0rc1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/django_import_export.egg-info/PKG-INFO` & `django-import-export-4.0.0rc1/django_import_export.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.0rc0
+Version: 4.0.0rc1
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `django-import-export-4.0.0rc0/django_import_export.egg-info/SOURCES.txt` & `django-import-export-4.0.0rc1/django_import_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/Makefile` & `django-import-export-4.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/change-form-export.png` & `django-import-export-4.0.0rc1/docs/_static/images/change-form-export.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/custom-export-form.png` & `django-import-export-4.0.0rc1/docs/_static/images/custom-export-form.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/custom-import-form.png` & `django-import-export-4.0.0rc1/docs/_static/images/custom-import-form.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/date-widget-validation-error.png` & `django-import-export-4.0.0rc1/docs/_static/images/date-widget-validation-error.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/django-import-export-change.png` & `django-import-export-4.0.0rc1/docs/_static/images/django-import-export-change.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/django-import-export-export-confirm.png` & `django-import-export-4.0.0rc1/docs/_static/images/django-import-export-export-confirm.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/django-import-export-import-confirm.png` & `django-import-export-4.0.0rc1/docs/_static/images/django-import-export-import-confirm.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/django-import-export-import.png` & `django-import-export-4.0.0rc1/docs/_static/images/django-import-export-import.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/export-button.png` & `django-import-export-4.0.0rc1/docs/_static/images/export-button.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/export_workflow.svg` & `django-import-export-4.0.0rc1/docs/_static/images/export_workflow.svg`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/import-button.png` & `django-import-export-4.0.0rc1/docs/_static/images/import-button.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/import_workflow.svg` & `django-import-export-4.0.0rc1/docs/_static/images/import_workflow.svg`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/non-field-specific-validation-error.png` & `django-import-export-4.0.0rc1/docs/_static/images/non-field-specific-validation-error.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/_static/images/select-for-export.png` & `django-import-export-4.0.0rc1/docs/_static/images/select-for-export.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/admin_integration.rst` & `django-import-export-4.0.0rc1/docs/admin_integration.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/advanced_usage.rst` & `django-import-export-4.0.0rc1/docs/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/api_mixins.rst` & `django-import-export-4.0.0rc1/docs/api_mixins.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/api_widgets.rst` & `django-import-export-4.0.0rc1/docs/api_widgets.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/bulk_import.rst` & `django-import-export-4.0.0rc1/docs/bulk_import.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/changelog.rst` & `django-import-export-4.0.0rc1/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 Changelog
 =========
 
 .. warning::
 
     Version 4 introduces breaking changes.  Please refer to :doc:`release notes<release_notes>`.
 
+4.0.0-rc.1 (unreleased)
+-----------------------
+
+- added try / catch to :meth:`~import_export.results.RowResult.add_instance_info` to handle unserializable instances (#1767)
+- fix: YAML export does not work with SafeString (#1762)
+- pass ``is_create``` param into :meth:`~import_export.resources.Resource.do_instance_save` (#1772)
+- fix: :meth:`~import_export.widgets.SimpleArrayWidget.render` crashes if value is ``None`` (#1771)
+- updated translations for release-4 (#1775)
+
 4.0.0-rc.0 (2024-02-14)
 -----------------------
 
 Deprecations
 ############
 
 - Removed v3 deprecations (#1629)
```

### Comparing `django-import-export-4.0.0rc0/docs/conf.py` & `django-import-export-4.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/contributing.rst` & `django-import-export-4.0.0rc1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/export_workflow.rst` & `django-import-export-4.0.0rc1/docs/export_workflow.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/faq.rst` & `django-import-export-4.0.0rc1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/getting_started.rst` & `django-import-export-4.0.0rc1/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/image_src/export_workflow.txt` & `django-import-export-4.0.0rc1/docs/image_src/export_workflow.txt`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/image_src/import_workflow.txt` & `django-import-export-4.0.0rc1/docs/image_src/import_workflow.txt`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/import_workflow.rst` & `django-import-export-4.0.0rc1/docs/import_workflow.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/index.rst` & `django-import-export-4.0.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/installation.rst` & `django-import-export-4.0.0rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/make.bat` & `django-import-export-4.0.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/release_notes.rst` & `django-import-export-4.0.0rc1/docs/release_notes.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/docs/testing.rst` & `django-import-export-4.0.0rc1/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/admin.py` & `django-import-export-4.0.0rc1/import_export/admin.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/declarative.py` & `django-import-export-4.0.0rc1/import_export/declarative.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/fields.py` & `django-import-export-4.0.0rc1/import_export/fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/formats/base_formats.py` & `django-import-export-4.0.0rc1/import_export/formats/base_formats.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/forms.py` & `django-import-export-4.0.0rc1/import_export/forms.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/instance_loaders.py` & `django-import-export-4.0.0rc1/import_export/instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/locale/ar/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/ar/LC_MESSAGES/django.mo`

 * *Files 25% similar despite different names*

#### msgunfmt {}

```diff
@@ -62,10 +62,7 @@
 msgstr "إرسال"
 
 msgid "This importer will import the following fields: "
 msgstr "هذا المستورد سوف يستورد الحقول التالية : "
 
 msgid "Update"
 msgstr "تحديث"
-
-msgid "You must select an export format."
-msgstr "يجب تحديد تنسيق التصدير."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/ar/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/ar/LC_MESSAGES/django.po`

 * *Files 21% similar despite different names*

```diff
@@ -4,78 +4,127 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
 msgstr ""
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
+#: admin.py:254
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
 msgstr ""
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "إستبراد"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "تصدير"
 
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "يجب تحديد تنسيق التصدير."
-
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "تصدير %(verbose_name_plural)s المحددة"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr ""
 
-#: forms.py:40
+#: forms.py:20
+msgid "Format"
+msgstr "تنسيق"
+
+#: forms.py:58
 msgid "File to import"
 msgstr "ملف للإستيراد"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "تنسيق"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "الرئيسية"
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
+msgstr[4] ""
+msgstr[5] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "هذا المستورد سوف يستورد الحقول التالية : "
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
 msgstr "إرسال"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
@@ -83,57 +132,76 @@
 "فيما يلي إستعراض للبيانات التي سيتم إستيرادها. إذا كنت راضيا عن النتائج, "
 "انقر على 'تأكيد الإستيراد'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
 msgstr "تأكيد الإستيراد"
 
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "هذا المستورد سوف يستورد الحقول التالية : "
-
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
 msgstr "أخطاء"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
 msgstr "رقم الصطر"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
 msgstr ""
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
 msgstr ""
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
 msgstr ""
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
 msgstr "معاينة"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
 msgstr "جديد"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
 msgstr "تجاهل"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
 msgstr "حذف"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
 msgstr "تحديث"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "هذا المستورد سوف يستورد الحقول التالية : "
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "يجب تحديد تنسيق التصدير."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/bg/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/bg/LC_MESSAGES/django.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -44,17 +44,14 @@
 
 msgid "Home"
 msgstr "Начало"
 
 msgid "Import"
 msgstr "Импортиране"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Импортирането е завършено, с {} нови и {} обновени {}."
-
 msgid "Line number"
 msgstr "Номер на реда"
 
 msgid "New"
 msgstr "Нов"
 
 msgid "Preview"
@@ -67,10 +64,7 @@
 msgstr "Изпълни"
 
 msgid "This importer will import the following fields: "
 msgstr "Ще бъдат импортирани следните полета: "
 
 msgid "Update"
 msgstr "Обновен"
-
-msgid "You must select an export format."
-msgstr "Трябва да изберете формат за експортиране."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/ca/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/ca/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -61,10 +61,7 @@
 msgstr "Enviar"
 
 msgid "This importer will import the following fields: "
 msgstr "Aquest importador importarà els següents camps: "
 
 msgid "Update"
 msgstr "Actualitzar"
-
-msgid "You must select an export format."
-msgstr "Heu de seleccionar un format d'exportació"
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/ca/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/it/LC_MESSAGES/django.po`

 * *Files 25% similar despite different names*

```diff
@@ -1,138 +1,201 @@
-# SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Manel Clos <manelclos@gmail.com>, 2016.
 #
-#, fuzzy
+# Christian Galeffi <chri@gallochri.com>, 2015.
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
+"PO-Revision-Date: 2015-08-30 20:32+0100\n"
+"Last-Translator: Christian Galeffi <chri@gallochri.com>\n"
+"Language-Team: Italian <kde-i18n-it@kde.org>\n"
+"Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 1.5.4\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
 msgstr ""
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
+#: admin.py:254
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
 msgstr ""
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importar"
+msgstr "Importare"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Exportar"
-
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "Heu de seleccionar un format d'exportació"
+msgstr "Esportare"
 
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exportar %(verbose_name_plural)s seleccionats"
+msgstr "Esporta selezionati %(verbose_name_plural)s"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr ""
 
-#: forms.py:40
+#: forms.py:20
+msgid "Format"
+msgstr "Formato"
+
+#: forms.py:58
 msgid "File to import"
-msgstr "Arxiu a importar"
+msgstr "File da importare"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "Format"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Inici"
+msgstr "Home"
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "Verranno importati i seguenti campi:"
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "Enviar"
+msgstr "Inviare"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"A continuació podeu veure una vista prèvia de les dades que s'importaran. Si "
-"esteu satisfets amb els resultats, premeu 'Confirmar importació'"
+"Questa è un'anteprima dei dati che saranno importati. Se il risultato è "
+"soddisfacente, premi 'Conferma importazione'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Confirmar importació"
+msgstr "Conferma importazione"
 
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "Aquest importador importarà els següents camps: "
-
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "Errors"
+msgstr "Errori"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Número de línia"
+msgstr "Numero linea"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
 msgstr ""
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
 msgstr ""
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
 msgstr ""
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "Vista prèvia"
+msgstr "Anteprima"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "Nou"
+msgstr "Nuovo"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "Omès"
+msgstr "Salta"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "Esborrar"
+msgstr "Cancella"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
-msgstr "Actualitzar"
+msgstr "Aggiorna"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "Verranno importati i seguenti campi:"
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "Devi selezionare un formato di esportazione."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/cs/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/cs/LC_MESSAGES/django.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -45,17 +45,14 @@
 
 msgid "Home"
 msgstr "Domů"
 
 msgid "Import"
 msgstr "Import"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Import dokončen, {} nové a {} aktualizované {}."
-
 msgid "Line number"
 msgstr "Číslo řádku"
 
 msgid "New"
 msgstr "Nové"
 
 msgid "Preview"
@@ -68,10 +65,7 @@
 msgstr "Odeslat"
 
 msgid "This importer will import the following fields: "
 msgstr "Budou importována následující pole: "
 
 msgid "Update"
 msgstr "Aktualizace"
-
-msgid "You must select an export format."
-msgstr "Musíte vybrat formát pro export."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/cs/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,138 +1,205 @@
-# SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+# Dan <pluthd@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
-"PO-Revision-Date: 2017-05-02 19:17+0200\n"
-"Last-Translator: \n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
+"PO-Revision-Date: 2020-06-06 10:30-0500\n"
+"Last-Translator: Daniel Pluth <pluthd@gmail.com>\n"
 "Language-Team: \n"
-"Language: cs\n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
-"X-Generator: Poedit 2.0.1\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"X-Generator: Lokalize 20.04.1\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
-msgstr "%s skrz import_export"
+msgstr "%s através import_export "
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Import dokončen, {} nové a {} aktualizované {}."
+#: admin.py:254
+#, fuzzy
+#| msgid "Import finished, with {} new and {} updated {}."
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
+msgstr "A importação foi completada com {} novas e {} atualizadas {}"
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Import"
+msgstr "Importar"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Export"
+msgstr "Exportar"
 
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "Musíte vybrat formát pro export."
-
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Vybrán export %(verbose_name_plural)s"
+msgstr "Exportar %(verbose_name_plural)s selecionados"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr ""
 
-#: forms.py:40
+#: forms.py:20
+msgid "Format"
+msgstr "Formato"
+
+#: forms.py:58
 msgid "File to import"
-msgstr "Soubor k importu"
+msgstr "Arquivo a ser importado"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "Formát"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Domů"
+msgstr "Início"
+
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "Este importador vai importar os seguintes campos:"
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "Odeslat"
+msgstr "Enviar"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"Níže je zobrazen náhled importovaných dat. Pokud je vše v pořádku, stiskněte "
-"tlačítko „Provést import”"
+"Ver abaixo uma prévia dos dados a serem importados. Se você esta satisfeito "
+"com os resultados, clique em 'Confirmar importação'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Provést import"
+msgstr "Confirmar importação"
 
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "Budou importována následující pole: "
-
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "Chyby"
+msgstr "Erros"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Číslo řádku"
+msgstr "Número da linha"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
-msgstr ""
+msgstr "Algumas linhas não foram validadas"
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
+"Por favor corrigir os erros nos dados onde possível e recarregar os dados "
+"com o formato acima."
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
-msgstr ""
+msgstr "Linha"
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
-msgstr ""
+msgstr "Campo não é específico"
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "Náhled"
+msgstr "Prévia"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "Nové"
+msgstr "Novo"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "Přeskočené"
+msgstr "Não usados"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "Smazání"
+msgstr "Remover"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
-msgstr "Aktualizace"
+msgstr "Atualizar"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "Este importador vai importar os seguintes campos:"
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "Você tem que selecionar um formato de exportação."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/de/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/de/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -52,17 +52,14 @@
 
 msgid "Home"
 msgstr "Start"
 
 msgid "Import"
 msgstr "Importieren"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Import fertiggestellt, mit {} neuen und {} aktualisierten {}."
-
 msgid "Line number"
 msgstr "Zeilennummer"
 
 msgid "New"
 msgstr "Neu"
 
 msgid "Non field specific"
@@ -94,10 +91,7 @@
 msgstr "Absenden"
 
 msgid "This importer will import the following fields: "
 msgstr "Es werden die folgenden Felder importiert: "
 
 msgid "Update"
 msgstr "Update"
-
-msgid "You must select an export format."
-msgstr "Es muss ein Exportformat ausgewählt werden."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/de/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/fr/LC_MESSAGES/django.po`

 * *Files 27% similar despite different names*

```diff
@@ -1,142 +1,202 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
-"PO-Revision-Date: 2022-10-17 17:42+0200\n"
-"Last-Translator: Jannes Blobel <jannes.blobel@inlang.com>\n"
-"Language-Team: \n"
-"Language: de\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 3.1.1\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
-msgstr "%s durch import_export"
+msgstr ""
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Import fertiggestellt, mit {} neuen und {} aktualisierten {}."
+#: admin.py:254
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
+msgstr ""
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
-"%(exc_name)s beim Versuch, die Datei zu lesen ist aufgetretten. Stellen Sie "
-"sicher, dass du  das richtige Format für deine Datei gewählt hast"
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importieren"
+msgstr "Importer"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Exportieren"
-
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "Es muss ein Exportformat ausgewählt werden."
+msgstr "Exporter"
 
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Ausgewählte %(verbose_name_plural)s exportieren"
+msgstr "Exporter %(verbose_name_plural)s selectionnés"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
-msgstr "Ressource"
+msgstr ""
+
+#: forms.py:20
+msgid "Format"
+msgstr "Format"
 
-#: forms.py:40
+#: forms.py:58
 msgid "File to import"
-msgstr "Zu importierende Datei"
+msgstr "Fichier à importer"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "Dateiformat"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Start"
+msgstr "Accueil"
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "Cet importateur va importer les champs suivants: "
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "Absenden"
+msgstr "Soumettre"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"Unten befindet sich eine Vorschau der zu importierenden Daten. Wenn die "
-"Ergebnisse zufriedenstellend sind, klicke auf \"Import bestätigen\"."
+"Voici un aperçu des données à importer. Si vous êtes satisfait des "
+"résultats, cliquez sur 'Confirmer l'importation'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Import bestätigen"
+msgstr "Confirmer l'importation"
 
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "Es werden die folgenden Felder importiert: "
-
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "Fehler"
+msgstr "Erreurs"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Zeilennummer"
+msgstr "Numéro de ligne"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
-msgstr "Die Validierung einiger Zeilen schlug fehl"
+msgstr ""
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
-"Bitte korrigiere falls möglich diese Fehler in deiner Datei und lade sie "
-"anschließend erneut mit dem obigen Formular hoch."
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
-msgstr "Zeile"
+msgstr ""
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
-msgstr "Nicht feldspezifisch"
+msgstr ""
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "Vorschau"
+msgstr "Aperçu"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "Neu"
+msgstr "Nouveau"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "Übersprungen"
+msgstr "Ignoré"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "Löschen"
+msgstr "Supprimer"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
-msgstr "Update"
+msgstr "Mettre à jour"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "Cet importateur va importer les champs suivants: "
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "Vous devez sélectionner un format d'exportation."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/es/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/es/LC_MESSAGES/django.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -48,17 +48,14 @@
 
 msgid "Home"
 msgstr "Inicio"
 
 msgid "Import"
 msgstr "Importar"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Proceso de importación finalizado, con {} nuevos y {} actualizados"
-
 msgid "Line number"
 msgstr "Número de línea"
 
 msgid "New"
 msgstr "Nuevo"
 
 msgid "Non field specific"
@@ -91,10 +88,7 @@
 msgstr "Enviar"
 
 msgid "This importer will import the following fields: "
 msgstr "Este importador importará los siguientes campos:"
 
 msgid "Update"
 msgstr "Actualizar"
-
-msgid "You must select an export format."
-msgstr "Debes seleccionar un formato de exportación."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/es/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/ko/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,144 +1,203 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# David Díaz <d.diazp@gmail.com>, 2015.
-# Santiago Muñoz <smunoz@mythologylabs.com.uy>, 2023.
+# Jinmyeong Cho <britzegs@gmail.com>, 2020.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
-"PO-Revision-Date: 2023-09-22 11:53-0300\n"
-"Last-Translator: Santiago Muñoz <smunoz@mythologylabs.com.uy>\n"
-"Language-Team: Spanish\n"
-"Language: es\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: Yeongkwang Yang <immutable000@gmail.com>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
-msgstr ""
+msgstr "%s은(는) django-import-export를 통해 가져왔습니다."
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Proceso de importación finalizado, con {} nuevos y {} actualizados"
+#: admin.py:254
+#, fuzzy
+#| msgid "Import finished, with {} new and {} updated {}."
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
+msgstr "가져오기 성공, {} 행 추가, {} 행 업데이트"
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
-"Se encontró %(exc_name)s mientras se intentaba leer el archivo. Asegúrese "
-"que seleccionó el formato correcto para el archivo."
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importar"
+msgstr "가져오기"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Exportar"
-
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "Debes seleccionar un formato de exportación."
+msgstr "내보내기"
 
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exportar %(verbose_name_plural)s seleccionados"
+msgstr "선택한 %(verbose_name_plural)s 내보내기"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
-msgstr "Recurso"
+msgstr ""
+
+#: forms.py:20
+msgid "Format"
+msgstr "형식"
 
-#: forms.py:40
+#: forms.py:58
 msgid "File to import"
-msgstr "Fichero a importar"
+msgstr "파일"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "Formato"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Inicio"
+msgstr ""
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "다음의 필드를 가져옵니다: "
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "Enviar"
+msgstr "제출"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"A continuación se muestra una vista previa de los datos a importar. Si estás "
-"satisfecho con los resultados, haz clic en 'Confirmar importación'"
+"다음은 불러올 데이터의 미리보기 입니다.데이터에 문제가 없다면 확인을 눌러 가"
+"져오기를 진행하세요."
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Confirmar importación"
+msgstr "확인"
 
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "Este importador importará los siguientes campos:"
-
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "Errores"
+msgstr "에러"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Número de línea"
+msgstr "행 번호"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
-msgstr "Falló la validación de algunas filas"
+msgstr "유효성 검증에 실패한 행이 있습니다."
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
-msgstr ""
-"Por favor corrija los siguientes errores en la información ingresada donde "
-"sea posible, luego vuelva a subir el archivo utilizando el formulario de la "
-"parte superior."
+msgstr "에러를 수정한 후 파일을 다시 업로드 해주세요."
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
-msgstr "Fila"
+msgstr ""
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
-msgstr "No específico del campo"
+msgstr "지정된 필드 없음"
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "Vista previa"
+msgstr "미리보기"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "Nuevo"
+msgstr "생성"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "Omitido"
+msgstr "넘어감"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "Borrar"
+msgstr "삭제"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
-msgstr "Actualizar"
+msgstr "갱신"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "다음의 필드를 가져옵니다: "
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "내보낼 형식을 선택해주세요."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/es_AR/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -49,17 +49,14 @@
 
 msgid "Home"
 msgstr "Inicio"
 
 msgid "Import"
 msgstr "Importar"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Proceso de importación finalizado, con {} nuevos y {} actualizados"
-
 msgid "Line number"
 msgstr "Número de línea"
 
 msgid "New"
 msgstr "Nuevo"
 
 msgid "Non field specific"
@@ -92,10 +89,7 @@
 msgstr "Enviar"
 
 msgid "This importer will import the following fields: "
 msgstr "Este importador importará los siguientes campos:"
 
 msgid "Update"
 msgstr "Actualizar"
-
-msgid "You must select an export format."
-msgstr "Debe seleccionar un formato de exportación."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/es_AR/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/nl/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,206 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Gonzalo Bustos, 2015.
-# Santiago Muñoz <smunoz@mythologylabs.com.uy>, 2023.
+# Bram Janssen <zakelijk@bram-janssen.nl>, 2019.
 #
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
-"PO-Revision-Date: 2023-09-22 11:53-0300\n"
-"Last-Translator: Santiago Muñoz <smunoz@mythologylabs.com.uy>\n"
-"Language-Team: Spanish (Argentina)\n"
-"Language: es_AR\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 1.6.10\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
-msgstr ""
+msgstr "%s door import_export"
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Proceso de importación finalizado, con {} nuevos y {} actualizados"
+#: admin.py:254
+#, fuzzy
+#| msgid "Import finished, with {} new and {} updated {}."
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
+msgstr "Import is klaar met {} nieuwe en {} geupdate {}."
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
-"Se encontró %(exc_name)s mientras se intentaba leer el archivo. Asegúrese "
-"que seleccionó el formato correcto para el archivo."
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importar"
+msgstr "Importeren"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Exportar"
-
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "Debe seleccionar un formato de exportación."
+msgstr "Exporteren"
 
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exportar %(verbose_name_plural)s seleccionados"
+msgstr "Exporteer geselecteerde %(verbose_name_plural)s"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
-msgstr "Recurso"
+msgstr ""
+
+#: forms.py:20
+msgid "Format"
+msgstr "Formaat"
 
-#: forms.py:40
+#: forms.py:58
 msgid "File to import"
-msgstr "Archivo a importar"
+msgstr "Bestand om te importeren"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "Formato"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Inicio"
+msgstr "Terug"
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "Deze import zal de volgende velden toevoegen"
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "Enviar"
+msgstr "Indienen"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"A continuación se muestra una vista previa de los datos a importar. Si está "
-"satisfecho con los resultados, haga clic en 'Confirmar importación'"
+"Hieronder is een voorvertoning van de data die geïmporteerd zal worden. Als "
+"u tevreden bent met het resultaat, klik dan op 'Accepteer de import'."
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Confirmar importación"
-
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "Este importador importará los siguientes campos:"
+msgstr "Accepteer de import"
 
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "Errores"
+msgstr "Fouten"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Número de línea"
+msgstr "Regel nummer"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
-msgstr "Falló la validación de algunas filas"
+msgstr "Sommige regels zijn niet goedgekeurd"
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
-"Por favor corrija los siguientes errores en la información ingresada donde "
-"sea posible, luego vuelva a subir el archivo utilizando el formulario de la "
-"parte superior."
+"Verander alstublieft de volgende fouten in uw data waar mogelijk. Upload het "
+"bestand daarna nogmaals met het veld hierboven."
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
-msgstr "Fila"
+msgstr "Regel"
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
-msgstr "No específico del campo"
+msgstr "Niet veld specifiek"
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "Vista previa"
+msgstr "Voorbeeldweergave"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "Nuevo"
+msgstr "Nieuw"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "Omitido"
+msgstr "Overgeslagen"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "Borrar"
+msgstr "Verwijderen"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
-msgstr "Actualizar"
+msgstr "Bijwerken"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "Deze import zal de volgende velden toevoegen"
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "U moet een export formaat kiezen."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/fa/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/fa/LC_MESSAGES/django.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -45,17 +45,14 @@
 
 msgid "Home"
 msgstr "خانه"
 
 msgid "Import"
 msgstr "بارگذاری"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "بارگذاری تمام شد، با {} مورد جدید و {} مورد به روز شده."
-
 msgid "Line number"
 msgstr "شماره خط"
 
 msgid "New"
 msgstr "جدید"
 
 msgid "Non field specific"
@@ -82,10 +79,7 @@
 msgstr "ارسال"
 
 msgid "This importer will import the following fields: "
 msgstr "این بارگذاری شامل این فیلد‌ها هست:"
 
 msgid "Update"
 msgstr "بروزرسانی"
-
-msgid "You must select an export format."
-msgstr "شما باید یک فرمت خروجی انتخاب کنید"
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/fa/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/sk/LC_MESSAGES/django.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,137 +1,203 @@
-# Copyright (C) 2021 THE django-import-export
-# This file is distributed under the same license as the django-import-export package.
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
+# This file is distributed under the same license as the PACKAGE package.
+# Juraj Bubniak <contact@jbub.eu>, 2015.
 #
-# Yazdan Ranjbar <Yazdan_ra@icloud.com>, 2021.
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: 0.0.1\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
-"PO-Revision-Date: 2021-03-09 00:29+0030\n"
-"Last-Translator: Yazdan Ranjbar <Yazdan_ra@icloud.com>\n"
-"Language-Team: Persain/Farsi <kde-i18n-it@kde.org>\n"
-"Language: Farsi/Persian\n"
-"MIME-Version: 0.1\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 1.5.4\n"
+"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
-msgstr "%s یه وسیله ورودی-خروجی"
+msgstr ""
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "بارگذاری تمام شد، با {} مورد جدید و {} مورد به روز شده."
+#: admin.py:254
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
+msgstr ""
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "بارگذاری"
+msgstr "Importovať"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "خروجی"
-
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "شما باید یک فرمت خروجی انتخاب کنید"
+msgstr "Exportovať"
 
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "خروجی %(verbose_name_plural)s انتخاب شده"
+msgstr "Exportovať vybrané %(verbose_name_plural)s"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr ""
 
-#: forms.py:40
+#: forms.py:20
+msgid "Format"
+msgstr "Formát"
+
+#: forms.py:58
 msgid "File to import"
-msgstr "قایل برای بارگذاری"
+msgstr "Importovať súbor"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "فرمت"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "خانه"
+msgstr "Domov"
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "Budú importované nasledujúce polia: "
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "ارسال"
+msgstr "Odoslať"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"پایین یک پیش‌نمایش از دیتا‌هایی است که بارگذاری خواهند شد اگر این موارد درست "
-"هستروی 'تایید بارگذاری' گلیگ گنید"
+"Nižšie je zobrazený náhľad importovaných dát. Ak je všetko v poriadku, "
+"kliknite na tlačidlo 'Potvrdiť import'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "تایید بارگذاری"
-
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "این بارگذاری شامل این فیلد‌ها هست:"
+msgstr "Potvrdiť import"
 
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "خطاها"
+msgstr "Chyby"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "شماره خط"
+msgstr "Číslo riadku"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
-msgstr "برخی از سطر‌ها معتبر نبودند"
+msgstr ""
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
-msgstr "لطفا این خطا را تصحیح کنید و سپس مجدد فایل را بارگذاری کنید"
+msgstr ""
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
-msgstr "سظر"
+msgstr ""
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
-msgstr "فیلد‌های غیر اختصاصی"
+msgstr ""
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "نمایش"
+msgstr "Náhľad"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "جدید"
+msgstr "Nový"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "در شد"
+msgstr "Preskočený"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "حذف"
+msgstr "Vymazaný"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
-msgstr "بروزرسانی"
+msgstr "Aktualizovaný"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "Budú importované nasledujúce polia: "
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "Je potrebné vybrať formát exportu."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/fi/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/fi/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -51,17 +51,14 @@
 
 msgid "Home"
 msgstr "Etusivu"
 
 msgid "Import"
 msgstr "Tuo"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Tuonti valmis. Lisätty {} ja päivitetty {} kohteita {}."
-
 msgid "Line number"
 msgstr "Rivinumero"
 
 msgid "New"
 msgstr "Uusi"
 
 msgid "Non field specific"
@@ -96,10 +93,7 @@
 msgstr "Tämä vienti vie seuraavat kentät: "
 
 msgid "This importer will import the following fields: "
 msgstr "Tämä tuonti tuo seuraavat kentät: "
 
 msgid "Update"
 msgstr "Päivitys"
-
-msgid "You must select an export format."
-msgstr "Sinun täytyy valita tiedostotyyppi."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/fi/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/fi/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,121 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-12-04 16:50+0200\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
 "PO-Revision-Date: 2023-05-10 15:23+0300\n"
 "Last-Translator: Lauri Virtanen <lauri.virtanen@iki.fi>\n"
 "Language-Team: \n"
 "Language: fi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin.py:244
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
 msgstr "%s käyttäen import_export"
 
-#: admin.py:252
-msgid "Import finished, with {} new and {} updated {}."
+#: admin.py:254
+#, fuzzy
+#| msgid "Import finished, with {} new and {} updated {}."
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
 msgstr "Tuonti valmis. Lisätty {} ja päivitetty {} kohteita {}."
 
-#: admin.py:497
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 "Kohdattiin %(exc_name)s tiedostoa lukiessa. Varmista, että olet valinnut "
 "oikean tiedostotyypin."
 
-#: admin.py:648 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "Tuo"
 
-#: admin.py:833 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Vie"
 
-#: admin.py:908
-msgid "You must select an export format."
-msgstr "Sinun täytyy valita tiedostotyyppi."
-
-#: admin.py:933
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Vie valitut %(verbose_name_plural)s"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr "Resurssi"
 
-#: forms.py:40
+#: forms.py:20
+msgid "Format"
+msgstr "Tiedostotyyppi"
+
+#: forms.py:58
 msgid "File to import"
 msgstr "Tuotava tiedosto"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "Tiedostotyyppi"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Etusivu"
 
-#: templates/admin/import_export/export.html:38
-#: templates/admin/import_export/import.html:64
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+msgid "This exporter will export the following fields: "
+msgstr "Tämä vienti vie seuraavat kentät: "
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
 msgstr "Lähetä"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
@@ -78,63 +123,78 @@
 "Alla on esikatselu tuotavista tiedoista. Jos olet tyytyväinen, paina "
 "'Vahvista tuonti'."
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
 msgstr "Vahvista tuonti"
 
-#: templates/admin/import_export/import.html:75
-#: templates/admin/import_export/import.html:106
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
 msgstr "Virheet"
 
-#: templates/admin/import_export/import.html:86
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
 msgstr "Rivinumero"
 
-#: templates/admin/import_export/import.html:98
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
 msgstr "Joitakin rivejä ei voitu vahvistaa"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
 "Korjaa nämä virheet tiedoissasi ja lähetä uudelleen käyttäen yllä olevaa "
 "lomaketta."
 
-#: templates/admin/import_export/import.html:105
+#: templates/admin/import_export/import.html:120
 msgid "Row"
 msgstr "Rivi"
 
-#: templates/admin/import_export/import.html:132
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
 msgstr "Ei liity mihinkään kenttään"
 
-#: templates/admin/import_export/import.html:155
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
 msgstr "Esikatselu"
 
-#: templates/admin/import_export/import.html:170
+#: templates/admin/import_export/import.html:185
 msgid "New"
 msgstr "Uusi"
 
-#: templates/admin/import_export/import.html:172
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
 msgstr "Ohitettu"
 
-#: templates/admin/import_export/import.html:174
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
 msgstr "Poisto"
 
-#: templates/admin/import_export/import.html:176
+#: templates/admin/import_export/import.html:191
 msgid "Update"
 msgstr "Päivitys"
 
-#: templates/admin/import_export/resource_fields_list.html:5
-msgid "This exporter will export the following fields: "
-msgstr "Tämä vienti vie seuraavat kentät: "
-
 #: templates/admin/import_export/resource_fields_list.html:7
 msgid "This importer will import the following fields: "
 msgstr "Tämä tuonti tuo seuraavat kentät: "
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "Sinun täytyy valita tiedostotyyppi."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/fr/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/it/LC_MESSAGES/django.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,70 +1,68 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2015-08-30 20:32+0100\n"
+"Last-Translator: Christian Galeffi <chri@gallochri.com>\n"
+"Language-Team: Italian <kde-i18n-it@kde.org>\n"
+"Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 1.5.4\n"
 
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"Voici un aperçu des données à importer. Si vous êtes satisfait des "
-"résultats, cliquez sur 'Confirmer l'importation'"
+"Questa è un'anteprima dei dati che saranno importati. Se il risultato è "
+"soddisfacente, premi 'Conferma importazione'"
 
 msgid "Confirm import"
-msgstr "Confirmer l'importation"
+msgstr "Conferma importazione"
 
 msgid "Delete"
-msgstr "Supprimer"
+msgstr "Cancella"
 
 msgid "Errors"
-msgstr "Erreurs"
+msgstr "Errori"
 
 msgid "Export"
-msgstr "Exporter"
+msgstr "Esportare"
 
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exporter %(verbose_name_plural)s selectionnés"
+msgstr "Esporta selezionati %(verbose_name_plural)s"
 
 msgid "File to import"
-msgstr "Fichier à importer"
+msgstr "File da importare"
 
 msgid "Format"
-msgstr "Format"
+msgstr "Formato"
 
 msgid "Home"
-msgstr "Accueil"
+msgstr "Home"
 
 msgid "Import"
-msgstr "Importer"
+msgstr "Importare"
 
 msgid "Line number"
-msgstr "Numéro de ligne"
+msgstr "Numero linea"
 
 msgid "New"
-msgstr "Nouveau"
+msgstr "Nuovo"
 
 msgid "Preview"
-msgstr "Aperçu"
+msgstr "Anteprima"
 
 msgid "Skipped"
-msgstr "Ignoré"
+msgstr "Salta"
 
 msgid "Submit"
-msgstr "Soumettre"
+msgstr "Inviare"
 
 msgid "This importer will import the following fields: "
-msgstr "Cet importateur va importer les champs suivants: "
+msgstr "Verranno importati i seguenti campi:"
 
 msgid "Update"
-msgstr "Mettre à jour"
-
-msgid "You must select an export format."
-msgstr "Vous devez sélectionner un format d'exportation."
+msgstr "Aggiorna"
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/fr/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/pl/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,206 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+# Ludwik Trammer <ludwik@gmail.com>, 2015.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2);\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
-msgstr ""
+msgstr "%s przez import_export"
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
-msgstr ""
+#: admin.py:254
+#, fuzzy
+#| msgid "Import finished, with {} new and {} updated {}."
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
+msgstr "Import zakończony, z {} nowymi i {} zaktualizowanymi {}."
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importer"
+msgstr "Import"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Exporter"
+msgstr "Eksport"
 
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "Vous devez sélectionner un format d'exportation."
-
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exporter %(verbose_name_plural)s selectionnés"
+msgstr "Eksportuj wybrane %(verbose_name_plural)s"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr ""
 
-#: forms.py:40
-msgid "File to import"
-msgstr "Fichier à importer"
-
-#: forms.py:42 forms.py:83 forms.py:116
+#: forms.py:20
 msgid "Format"
 msgstr "Format"
 
+#: forms.py:58
+msgid "File to import"
+msgstr "Plik do importu"
+
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
+
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Accueil"
+msgstr "Powrót"
+
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "Zostaną zaimportowane następujące pola: "
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "Soumettre"
+msgstr "Wyślij"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"Voici un aperçu des données à importer. Si vous êtes satisfait des "
-"résultats, cliquez sur 'Confirmer l'importation'"
+"Poniżej znajdują się przykładowe dane do zaimportowania. Jeśli "
+"satysfakcjonuje Cię wynik, kliknij 'Potwierdź import'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Confirmer l'importation"
-
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "Cet importateur va importer les champs suivants: "
+msgstr "Potwierdź import"
 
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "Erreurs"
+msgstr "Błędy"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Numéro de ligne"
+msgstr "Numer linii"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
 msgstr ""
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
 msgstr ""
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
 msgstr ""
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "Aperçu"
+msgstr "Podgląd"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "Nouveau"
+msgstr "Nowy"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "Ignoré"
+msgstr "Pominięty"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "Supprimer"
+msgstr "Usuń"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
-msgstr "Mettre à jour"
+msgstr "Zaktualizowany"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "Zostaną zaimportowane następujące pola: "
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "Musisz wybrać format eksportu."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/it/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,201 @@
+# SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-# Christian Galeffi <chri@gallochri.com>, 2015.
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
-"PO-Revision-Date: 2015-08-30 20:32+0100\n"
-"Last-Translator: Christian Galeffi <chri@gallochri.com>\n"
-"Language-Team: Italian <kde-i18n-it@kde.org>\n"
-"Language: it\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: hao wang <173300430@qq.com>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 1.5.4\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
-msgstr ""
+msgstr "%s 通过 django-import-export导入"
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
-msgstr ""
+#: admin.py:254
+#, fuzzy
+#| msgid "Import finished, with {} new and {} updated {}."
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
+msgstr "导入成功，新增{}条记录，更新{}条记录。"
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importare"
+msgstr "导入"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Esportare"
-
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "Devi selezionare un formato di esportazione."
+msgstr "导出"
 
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Esporta selezionati %(verbose_name_plural)s"
+msgstr "导出选中的 %(verbose_name_plural)s"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr ""
 
-#: forms.py:40
+#: forms.py:20
+msgid "Format"
+msgstr "格式"
+
+#: forms.py:58
 msgid "File to import"
-msgstr "File da importare"
+msgstr "导入文件"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "Formato"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Home"
+msgstr ""
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "此次将导入以下字段："
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "Inviare"
+msgstr "提交"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
-msgstr ""
-"Questa è un'anteprima dei dati che saranno importati. Se il risultato è "
-"soddisfacente, premi 'Conferma importazione'"
+msgstr "以下是导入数据的预览。如果确认结果没有问题，可以点击 “确认导入”"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Conferma importazione"
+msgstr "确认导入"
 
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "Verranno importati i seguenti campi:"
-
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "Errori"
+msgstr "错误"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Numero linea"
+msgstr "行号"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
-msgstr ""
+msgstr "某些行验数据证失败"
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
-msgstr ""
+msgstr "请使用上面的表单，纠正这些提示有错误的数据，并重新上传"
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
-msgstr ""
+msgstr "行"
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
-msgstr ""
+msgstr "没有指定的字段"
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "Anteprima"
+msgstr "预览"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "Nuovo"
+msgstr "新增"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "Salta"
+msgstr "忽略"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "Cancella"
+msgstr "删除"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
-msgstr "Aggiorna"
+msgstr "更新"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "此次将导入以下字段："
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "您必须选择一个导出格式。"
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/ja/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/ja/LC_MESSAGES/django.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -61,10 +61,7 @@
 msgstr "確定"
 
 msgid "This importer will import the following fields: "
 msgstr "以下の列をインポートします。"
 
 msgid "Update"
 msgstr "更新"
-
-msgid "You must select an export format."
-msgstr "エクスポートフォーマットを選択してください。"
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/ko/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/ko/LC_MESSAGES/django.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -41,17 +41,14 @@
 
 msgid "Format"
 msgstr "형식"
 
 msgid "Import"
 msgstr "가져오기"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "가져오기 성공, {} 행 추가, {} 행 업데이트"
-
 msgid "Line number"
 msgstr "행 번호"
 
 msgid "New"
 msgstr "생성"
 
 msgid "Non field specific"
@@ -75,10 +72,7 @@
 msgstr "제출"
 
 msgid "This importer will import the following fields: "
 msgstr "다음의 필드를 가져옵니다: "
 
 msgid "Update"
 msgstr "갱신"
-
-msgid "You must select an export format."
-msgstr "내보낼 형식을 선택해주세요."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/ko/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/de/LC_MESSAGES/django.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,208 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Jinmyeong Cho <britzegs@gmail.com>, 2020.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Yeongkwang Yang <immutable000@gmail.com>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
+"PO-Revision-Date: 2022-10-17 17:42+0200\n"
+"Last-Translator: Jannes Blobel <jannes.blobel@inlang.com>\n"
+"Language-Team: \n"
+"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 3.1.1\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
-msgstr "%s은(는) django-import-export를 통해 가져왔습니다."
+msgstr "%s durch import_export"
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "가져오기 성공, {} 행 추가, {} 행 업데이트"
+#: admin.py:254
+#, fuzzy
+#| msgid "Import finished, with {} new and {} updated {}."
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
+msgstr "Import fertiggestellt, mit {} neuen und {} aktualisierten {}."
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
+"%(exc_name)s beim Versuch, die Datei zu lesen ist aufgetretten. Stellen Sie "
+"sicher, dass du  das richtige Format für deine Datei gewählt hast"
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "가져오기"
+msgstr "Importieren"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "내보내기"
-
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "내보낼 형식을 선택해주세요."
+msgstr "Exportieren"
 
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "선택한 %(verbose_name_plural)s 내보내기"
+msgstr "Ausgewählte %(verbose_name_plural)s exportieren"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
-msgstr ""
+msgstr "Ressource"
+
+#: forms.py:20
+msgid "Format"
+msgstr "Dateiformat"
 
-#: forms.py:40
+#: forms.py:58
 msgid "File to import"
-msgstr "파일"
+msgstr "Zu importierende Datei"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "형식"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr ""
+msgstr "Start"
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "Es werden die folgenden Felder importiert: "
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "제출"
+msgstr "Absenden"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"다음은 불러올 데이터의 미리보기 입니다.데이터에 문제가 없다면 확인을 눌러 가"
-"져오기를 진행하세요."
+"Unten befindet sich eine Vorschau der zu importierenden Daten. Wenn die "
+"Ergebnisse zufriedenstellend sind, klicke auf \"Import bestätigen\"."
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "확인"
+msgstr "Import bestätigen"
 
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "다음의 필드를 가져옵니다: "
-
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "에러"
+msgstr "Fehler"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "행 번호"
+msgstr "Zeilennummer"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
-msgstr "유효성 검증에 실패한 행이 있습니다."
+msgstr "Die Validierung einiger Zeilen schlug fehl"
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
-msgstr "에러를 수정한 후 파일을 다시 업로드 해주세요."
+msgstr ""
+"Bitte korrigiere falls möglich diese Fehler in deiner Datei und lade sie "
+"anschließend erneut mit dem obigen Formular hoch."
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
-msgstr ""
+msgstr "Zeile"
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
-msgstr "지정된 필드 없음"
+msgstr "Nicht feldspezifisch"
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "미리보기"
+msgstr "Vorschau"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "생성"
+msgstr "Neu"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "넘어감"
+msgstr "Übersprungen"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "삭제"
+msgstr "Löschen"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
-msgstr "갱신"
+msgstr "Update"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "Es werden die folgenden Felder importiert: "
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "Es muss ein Exportformat ausgewählt werden."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/kz/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/kz/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -43,17 +43,14 @@
 
 msgid "Home"
 msgstr "Басты бет"
 
 msgid "Import"
 msgstr "Импорт"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Импорт аяқталды, {} жаңа және {} жаңартылды {}."
-
 msgid "Line number"
 msgstr "Жол нөмірі"
 
 msgid "New"
 msgstr "Жаңа"
 
 msgid "Non field specific"
@@ -82,10 +79,7 @@
 msgstr "Жіберу"
 
 msgid "This importer will import the following fields: "
 msgstr "Бұл импорттаушы келесі өрістерді импорттайды: "
 
 msgid "Update"
 msgstr "Жаңарту"
-
-msgid "You must select an export format."
-msgstr "Сіз экспорт форматын таңдауыңыз керек."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/kz/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/kz/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -4,76 +4,123 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Muslim Beibytuly <muslimbeibytuly@gmail.com>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: Kazakh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
 msgstr "%s арқылы import_export"
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
+#: admin.py:254
+#, fuzzy
+#| msgid "Import finished, with {} new and {} updated {}."
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
 msgstr "Импорт аяқталды, {} жаңа және {} жаңартылды {}."
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "Импорт"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Экспорт"
 
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "Сіз экспорт форматын таңдауыңыз керек."
-
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Таңдалған %(verbose_name_plural)s экспорттаңыз"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr ""
 
-#: forms.py:40
+#: forms.py:20
+msgid "Format"
+msgstr "Формат"
+
+#: forms.py:58
 msgid "File to import"
 msgstr "Импорттауға арналған файл"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "Формат"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Басты бет"
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "Бұл импорттаушы келесі өрістерді импорттайды: "
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
 msgstr "Жіберу"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
@@ -81,59 +128,78 @@
 "Төменде импортталатын деректерді алдын ала қарау берілген. Егер сіз "
 "нәтижелерге қанағаттансаңыз, 'Импортты растау' түймесін басыңыз."
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
 msgstr "Импортты растау"
 
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "Бұл импорттаушы келесі өрістерді импорттайды: "
-
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
 msgstr "Қателер"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
 msgstr "Жол нөмірі"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
 msgstr "Кейбір жолдар тексерілмеді"
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
 "Мүмкіндігінше деректеріңіздегі қателерді түзетіңіз, содан кейін жоғарыдағы "
 "пішінді қолданып қайта жүктеңіз."
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
 msgstr "Қатар"
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
 msgstr "Өріске қатысты емес"
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
 msgstr "Алдын-ала қарау"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
 msgstr "Жаңа"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
 msgstr "Өткізілді"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
 msgstr "Жою"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
 msgstr "Жаңарту"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "Бұл импорттаушы келесі өрістерді импорттайды: "
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "Сіз экспорт форматын таңдауыңыз керек."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/nl/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/nl/LC_MESSAGES/django.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -44,17 +44,14 @@
 
 msgid "Home"
 msgstr "Terug"
 
 msgid "Import"
 msgstr "Importeren"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Import is klaar met {} nieuwe en {} geupdate {}."
-
 msgid "Line number"
 msgstr "Regel nummer"
 
 msgid "New"
 msgstr "Nieuw"
 
 msgid "Non field specific"
@@ -83,10 +80,7 @@
 msgstr "Indienen"
 
 msgid "This importer will import the following fields: "
 msgstr "Deze import zal de volgende velden toevoegen"
 
 msgid "Update"
 msgstr "Bijwerken"
-
-msgid "You must select an export format."
-msgstr "U moet een export formaat kiezen."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/nl/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/ca/LC_MESSAGES/django.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,140 +1,202 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Bram Janssen <zakelijk@bram-janssen.nl>, 2019.
+# Manel Clos <manelclos@gmail.com>, 2016.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
-msgstr "%s door import_export"
+msgstr ""
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Import is klaar met {} nieuwe en {} geupdate {}."
+#: admin.py:254
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
+msgstr ""
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Importeren"
+msgstr "Importar"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Exporteren"
-
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "U moet een export formaat kiezen."
+msgstr "Exportar"
 
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exporteer geselecteerde %(verbose_name_plural)s"
+msgstr "Exportar %(verbose_name_plural)s seleccionats"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr ""
 
-#: forms.py:40
+#: forms.py:20
+msgid "Format"
+msgstr "Format"
+
+#: forms.py:58
 msgid "File to import"
-msgstr "Bestand om te importeren"
+msgstr "Arxiu a importar"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "Formaat"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Terug"
+msgstr "Inici"
+
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "Aquest importador importarà els següents camps: "
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "Indienen"
+msgstr "Enviar"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"Hieronder is een voorvertoning van de data die geïmporteerd zal worden. Als "
-"u tevreden bent met het resultaat, klik dan op 'Accepteer de import'."
+"A continuació podeu veure una vista prèvia de les dades que s'importaran. Si "
+"esteu satisfets amb els resultats, premeu 'Confirmar importació'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Accepteer de import"
-
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "Deze import zal de volgende velden toevoegen"
+msgstr "Confirmar importació"
 
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "Fouten"
+msgstr "Errors"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Regel nummer"
+msgstr "Número de línia"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
-msgstr "Sommige regels zijn niet goedgekeurd"
+msgstr ""
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
-"Verander alstublieft de volgende fouten in uw data waar mogelijk. Upload het "
-"bestand daarna nogmaals met het veld hierboven."
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
-msgstr "Regel"
+msgstr ""
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
-msgstr "Niet veld specifiek"
+msgstr ""
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "Voorbeeldweergave"
+msgstr "Vista prèvia"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "Nieuw"
+msgstr "Nou"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "Overgeslagen"
+msgstr "Omès"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "Verwijderen"
+msgstr "Esborrar"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
-msgstr "Bijwerken"
+msgstr "Actualitzar"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "Aquest importador importarà els següents camps: "
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "Heu de seleccionar un format d'exportació"
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/pl/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/pl/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -45,17 +45,14 @@
 
 msgid "Home"
 msgstr "Powrót"
 
 msgid "Import"
 msgstr "Import"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Import zakończony, z {} nowymi i {} zaktualizowanymi {}."
-
 msgid "Line number"
 msgstr "Numer linii"
 
 msgid "New"
 msgstr "Nowy"
 
 msgid "Preview"
@@ -68,10 +65,7 @@
 msgstr "Wyślij"
 
 msgid "This importer will import the following fields: "
 msgstr "Zostaną zaimportowane następujące pola: "
 
 msgid "Update"
 msgstr "Zaktualizowany"
-
-msgid "You must select an export format."
-msgstr "Musisz wybrać format eksportu."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/pt_BR/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -45,17 +45,14 @@
 
 msgid "Home"
 msgstr "Início"
 
 msgid "Import"
 msgstr "Importar"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "A importação foi completada com {} novas e {} atualizadas {}"
-
 msgid "Line number"
 msgstr "Número da linha"
 
 msgid "New"
 msgstr "Novo"
 
 msgid "Non field specific"
@@ -84,10 +81,7 @@
 msgstr "Enviar"
 
 msgid "This importer will import the following fields: "
 msgstr "Este importador vai importar os seguintes campos:"
 
 msgid "Update"
 msgstr "Atualizar"
-
-msgid "You must select an export format."
-msgstr "Você tem que selecionar um formato de exportação."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/ru/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/ru/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -45,17 +45,14 @@
 
 msgid "Home"
 msgstr "Главная"
 
 msgid "Import"
 msgstr "Импорт"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Импорт завершен, {} новых и {} обновлено."
-
 msgid "Line number"
 msgstr "Номер строки"
 
 msgid "New"
 msgstr "Добавлено"
 
 msgid "Non field specific"
@@ -84,10 +81,7 @@
 msgstr "Отправить"
 
 msgid "This importer will import the following fields: "
 msgstr "Будут импортированы следующие поля: "
 
 msgid "Update"
 msgstr "Обновлено"
-
-msgid "You must select an export format."
-msgstr "Необходимо выбрать формат экспорта"
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/ru/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/bg/LC_MESSAGES/django.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,141 +1,204 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+# Hristo Gatsinski <gatsinski@gmail.com>, 2017.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Last-Translator: Hristo Gatsinski <gatsinski@gmail.com>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"Language: Bulgarian\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
-msgstr "%s через import_export"
+msgstr "%s чрез import_export"
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "Импорт завершен, {} новых и {} обновлено."
+#: admin.py:254
+#, fuzzy
+#| msgid "Import finished, with {} new and {} updated {}."
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
+msgstr "Импортирането е завършено, с {} нови и {} обновени {}."
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "Импорт"
+msgstr "Импортиране"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "Экспорт"
-
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "Необходимо выбрать формат экспорта"
+msgstr "Експортиране"
 
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Экспортировать выбранные %(verbose_name_plural)s"
+msgstr "Експортиране на избраните %(verbose_name_plural)s"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr ""
 
-#: forms.py:40
-msgid "File to import"
-msgstr "Файл для импорта"
-
-#: forms.py:42 forms.py:83 forms.py:116
+#: forms.py:20
 msgid "Format"
 msgstr "Формат"
 
+#: forms.py:58
+msgid "File to import"
+msgstr "Файл за импортиране"
+
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
+
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr "Главная"
+msgstr "Начало"
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "Ще бъдат импортирани следните полета: "
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "Отправить"
+msgstr "Изпълни"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"Ниже показано то, что будет импортировано. Нажмите 'Подтвердить импорт', "
-"если Вас устраивает результат"
+"Отдолу виждате преглед на данните за импортиране. Ако сте доволни от "
+"резултата, изберете 'Потвърди импортирането'"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "Подтвердить импорт"
-
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "Будут импортированы следующие поля: "
+msgstr "Потвърди импортирането"
 
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "Ошибки"
+msgstr "Грешки"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "Номер строки"
+msgstr "Номер на реда"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
-msgstr "Некоторые строки не прошли валидацию"
+msgstr ""
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
-"По возможности исправьте эти ошибки в своих данных, а затем повторно "
-"загрузите их, используя форму выше."
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
-msgstr "Строка"
+msgstr ""
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
-msgstr "Не относящиеся к конкретному полю"
+msgstr ""
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "Предпросмотр"
+msgstr "Преглед"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "Добавлено"
+msgstr "Нов"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "Пропущено"
+msgstr "Пропуснат"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "Удалено"
+msgstr "Изтрит"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
-msgstr "Обновлено"
+msgstr "Обновен"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "Ще бъдат импортирани следните полета: "
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "Трябва да изберете формат за експортиране."
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/sk/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/fr/LC_MESSAGES/django.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -5,66 +5,63 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
 msgstr ""
-"Nižšie je zobrazený náhľad importovaných dát. Ak je všetko v poriadku, "
-"kliknite na tlačidlo 'Potvrdiť import'"
+"Voici un aperçu des données à importer. Si vous êtes satisfait des "
+"résultats, cliquez sur 'Confirmer l'importation'"
 
 msgid "Confirm import"
-msgstr "Potvrdiť import"
+msgstr "Confirmer l'importation"
 
 msgid "Delete"
-msgstr "Vymazaný"
+msgstr "Supprimer"
 
 msgid "Errors"
-msgstr "Chyby"
+msgstr "Erreurs"
 
 msgid "Export"
-msgstr "Exportovať"
+msgstr "Exporter"
 
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "Exportovať vybrané %(verbose_name_plural)s"
+msgstr "Exporter %(verbose_name_plural)s selectionnés"
 
 msgid "File to import"
-msgstr "Importovať súbor"
+msgstr "Fichier à importer"
 
 msgid "Format"
-msgstr "Formát"
+msgstr "Format"
 
 msgid "Home"
-msgstr "Domov"
+msgstr "Accueil"
 
 msgid "Import"
-msgstr "Importovať"
+msgstr "Importer"
 
 msgid "Line number"
-msgstr "Číslo riadku"
+msgstr "Numéro de ligne"
 
 msgid "New"
-msgstr "Nový"
+msgstr "Nouveau"
 
 msgid "Preview"
-msgstr "Náhľad"
+msgstr "Aperçu"
 
 msgid "Skipped"
-msgstr "Preskočený"
+msgstr "Ignoré"
 
 msgid "Submit"
-msgstr "Odoslať"
+msgstr "Soumettre"
 
 msgid "This importer will import the following fields: "
-msgstr "Budú importované nasledujúce polia: "
+msgstr "Cet importateur va importer les champs suivants: "
 
 msgid "Update"
-msgstr "Aktualizovaný"
-
-msgid "You must select an export format."
-msgstr "Je potrebné vybrať formát exportu."
+msgstr "Mettre à jour"
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/tr/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/tr/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -44,17 +44,14 @@
 
 msgid "Home"
 msgstr "Ana sayfa"
 
 msgid "Import"
 msgstr "İçe aktar"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "{} yeni ve {} güncellenen {} ile içe aktarma bitti"
-
 msgid "Line number"
 msgstr "Satır numarası"
 
 msgid "New"
 msgstr "Yeni"
 
 msgid "Non field specific"
@@ -83,10 +80,7 @@
 msgstr "Kaydet"
 
 msgid "This importer will import the following fields: "
 msgstr "Bu içe aktarıcı aşağıdaki alanları içe aktaracaktır: "
 
 msgid "Update"
 msgstr "Güncelle"
-
-msgid "You must select an export format."
-msgstr "Bir dosya biçimi seçmelisiniz"
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/tr/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/tr/LC_MESSAGES/django.po`

 * *Files 25% similar despite different names*

```diff
@@ -4,77 +4,124 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
 msgstr "%s vasıtasıyla import_export"
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
+#: admin.py:254
+#, fuzzy
+#| msgid "Import finished, with {} new and {} updated {}."
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
 msgstr "{} yeni ve {} güncellenen {} ile içe aktarma bitti"
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
 msgstr "İçe aktar"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "Dışa aktar"
 
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "Bir dosya biçimi seçmelisiniz"
-
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
 msgstr "Seçililenleri dışa aktar %(verbose_name_plural)s"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr ""
 
-#: forms.py:40
+#: forms.py:20
+msgid "Format"
+msgstr "Dosya biçimi"
+
+#: forms.py:58
 msgid "File to import"
 msgstr "İçe alınacak dosya"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "Dosya biçimi"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
 msgstr "Ana sayfa"
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+msgstr[1] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "Bu içe aktarıcı aşağıdaki alanları içe aktaracaktır: "
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
 msgstr "Kaydet"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
@@ -82,59 +129,78 @@
 "Aşağıda içe aktarılacak verilerin önizlemesi verilmiştir. Sonuçlardan "
 "memnunsanız 'İçe aktarmayı onayla'yı tıklayın."
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
 msgstr "İçe aktarmayı onayla"
 
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "Bu içe aktarıcı aşağıdaki alanları içe aktaracaktır: "
-
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
 msgstr "Hatalar"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
 msgstr "Satır numarası"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
 msgstr "Bazı satırlar doğrulanamadı"
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
 msgstr ""
 "Lütfen verilerinizdeki bu hataları olabildiğince düzeltin, sonra yukarıdaki "
 "formu kullanarak tekrar yükleyin."
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
 msgstr "Satır"
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
 msgstr "Alan olmayana özgü"
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
 msgstr "Ön izleme"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
 msgstr "Yeni"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
 msgstr "Atlandı"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
 msgstr "Sil"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
 msgstr "Güncelle"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "Bu içe aktarıcı aşağıdaki alanları içe aktaracaktır: "
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "Bir dosya biçimi seçmelisiniz"
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc1/import_export/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -39,17 +39,14 @@
 
 msgid "Format"
 msgstr "格式"
 
 msgid "Import"
 msgstr "导入"
 
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "导入成功，新增{}条记录，更新{}条记录。"
-
 msgid "Line number"
 msgstr "行号"
 
 msgid "New"
 msgstr "新增"
 
 msgid "Non field specific"
@@ -76,10 +73,7 @@
 msgstr "提交"
 
 msgid "This importer will import the following fields: "
 msgstr "此次将导入以下字段："
 
 msgid "Update"
 msgstr "更新"
-
-msgid "You must select an export format."
-msgstr "您必须选择一个导出格式。"
```

### Comparing `django-import-export-4.0.0rc0/import_export/locale/zh_Hans/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc1/import_export/locale/ja/LC_MESSAGES/django.po`

 * *Files 24% similar despite different names*

```diff
@@ -4,133 +4,198 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:22+0000\n"
+"POT-Creation-Date: 2024-03-15 13:54+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: hao wang <173300430@qq.com>\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: admin.py:239
+#: admin.py:246 admin.py:588
 #, python-format
 msgid "%s through import_export"
-msgstr "%s 通过 django-import-export导入"
+msgstr ""
 
-#: admin.py:246
-msgid "Import finished, with {} new and {} updated {}."
-msgstr "导入成功，新增{}条记录，更新{}条记录。"
+#: admin.py:254
+msgid "Import finished: {} new, {} updated, {} deleted and {} skipped {}."
+msgstr ""
 
-#: admin.py:491
+#: admin.py:423
 #, python-format
 msgid ""
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
-#: admin.py:642 templates/admin/import_export/change_list_import_item.html:5
+#: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "导入"
+msgstr "インポート"
 
-#: admin.py:827 templates/admin/import_export/change_list_export_item.html:5
+#: admin.py:785 templates/admin/import_export/change_form.html:8
+#: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
-msgstr "导出"
-
-#: admin.py:892
-msgid "You must select an export format."
-msgstr "您必须选择一个导出格式。"
+msgstr "エクスポート"
 
-#: admin.py:917
+#: admin.py:911
 #, python-format
 msgid "Export selected %(verbose_name_plural)s"
-msgstr "导出选中的 %(verbose_name_plural)s"
+msgstr "選択した %(verbose_name_plural)s をエクスポート"
 
-#: forms.py:12
+#: forms.py:15
 msgid "Resource"
 msgstr ""
 
-#: forms.py:40
+#: forms.py:20
+msgid "Format"
+msgstr "フォーマット"
+
+#: forms.py:58
 msgid "File to import"
-msgstr "导入文件"
+msgstr "インポートするファイル"
 
-#: forms.py:42 forms.py:83 forms.py:116
-msgid "Format"
-msgstr "格式"
+#: forms.py:209
+msgid "Form is not validated, call `is_valid` first"
+msgstr ""
+
+#: forms.py:261
+#, python-format
+msgid "Select at least 1 field for \"%(resource_name)s\" to export"
+msgstr ""
+
+#: resources.py:1137
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the resource fields: %s"
+msgstr ""
+
+#: resources.py:1152
+#, python-format
+msgid ""
+"The following fields are declared in 'import_id_fields' but are not present "
+"in the file headers: %s"
+msgstr ""
+
+#: results.py:120
+#, python-format
+msgid "call to force_str() on instance failed: %s"
+msgstr ""
 
 #: templates/admin/import_export/base.html:11
 msgid "Home"
-msgstr ""
+msgstr "ホーム"
 
-#: templates/admin/import_export/export.html:36
-#: templates/admin/import_export/import.html:78
+#: templates/admin/import_export/export.html:21
+#, python-format
+msgid ""
+"\n"
+"        Export %(len)s selected item.\n"
+"        "
+msgid_plural ""
+"\n"
+"        Export %(len)s selected items.\n"
+"      "
+msgstr[0] ""
+
+#: templates/admin/import_export/export.html:48
+#: templates/admin/import_export/resource_fields_list.html:5
+#, fuzzy
+#| msgid "This importer will import the following fields: "
+msgid "This exporter will export the following fields: "
+msgstr "以下の列をインポートします。"
+
+#: templates/admin/import_export/export.html:76
+#: templates/admin/import_export/import.html:69
 msgid "Submit"
-msgstr "提交"
+msgstr "確定"
 
 #: templates/admin/import_export/import.html:30
 msgid ""
 "Below is a preview of data to be imported. If you are satisfied with the "
 "results, click 'Confirm import'"
-msgstr "以下是导入数据的预览。如果确认结果没有问题，可以点击 “确认导入”"
+msgstr ""
+"インポートされるデータのプレビューを表示しています。この内容で問題なければ"
+"「インポート実行」をクリックしてください。"
 
 #: templates/admin/import_export/import.html:33
 msgid "Confirm import"
-msgstr "确认导入"
-
-#: templates/admin/import_export/import.html:44
-msgid "This importer will import the following fields: "
-msgstr "此次将导入以下字段："
+msgstr "インポート実行"
 
-#: templates/admin/import_export/import.html:89
-#: templates/admin/import_export/import.html:120
+#: templates/admin/import_export/import.html:80
+#: templates/admin/import_export/import.html:121
 msgid "Errors"
-msgstr "错误"
+msgstr "エラー"
 
-#: templates/admin/import_export/import.html:100
+#: templates/admin/import_export/import.html:94
 msgid "Line number"
-msgstr "行号"
+msgstr "行番号"
 
-#: templates/admin/import_export/import.html:112
+#: templates/admin/import_export/import.html:113
 msgid "Some rows failed to validate"
-msgstr "某些行验数据证失败"
+msgstr ""
 
-#: templates/admin/import_export/import.html:114
+#: templates/admin/import_export/import.html:115
 msgid ""
 "Please correct these errors in your data where possible, then reupload it "
 "using the form above."
-msgstr "请使用上面的表单，纠正这些提示有错误的数据，并重新上传"
+msgstr ""
 
-#: templates/admin/import_export/import.html:119
+#: templates/admin/import_export/import.html:120
 msgid "Row"
-msgstr "行"
+msgstr ""
 
-#: templates/admin/import_export/import.html:146
+#: templates/admin/import_export/import.html:147
 msgid "Non field specific"
-msgstr "没有指定的字段"
+msgstr ""
 
-#: templates/admin/import_export/import.html:169
+#: templates/admin/import_export/import.html:170
 msgid "Preview"
-msgstr "预览"
+msgstr "プレビュー"
 
-#: templates/admin/import_export/import.html:184
+#: templates/admin/import_export/import.html:185
 msgid "New"
-msgstr "新增"
+msgstr "新規"
 
-#: templates/admin/import_export/import.html:186
+#: templates/admin/import_export/import.html:187
 msgid "Skipped"
-msgstr "忽略"
+msgstr "スキップ"
 
-#: templates/admin/import_export/import.html:188
+#: templates/admin/import_export/import.html:189
 msgid "Delete"
-msgstr "删除"
+msgstr "削除"
 
-#: templates/admin/import_export/import.html:190
+#: templates/admin/import_export/import.html:191
 msgid "Update"
 msgstr "更新"
+
+#: templates/admin/import_export/resource_fields_list.html:7
+msgid "This importer will import the following fields: "
+msgstr "以下の列をインポートします。"
+
+#: widgets.py:250
+msgid "Value could not be parsed using defined date formats."
+msgstr ""
+
+#: widgets.py:300
+msgid "Value could not be parsed using defined datetime formats."
+msgstr ""
+
+#: widgets.py:346
+msgid "Value could not be parsed using defined time formats."
+msgstr ""
+
+#: widgets.py:374
+msgid "Value could not be parsed."
+msgstr ""
+
+#~ msgid "You must select an export format."
+#~ msgstr "エクスポートフォーマットを選択してください。"
```

### Comparing `django-import-export-4.0.0rc0/import_export/mixins.py` & `django-import-export-4.0.0rc1/import_export/mixins.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/options.py` & `django-import-export-4.0.0rc1/import_export/options.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/resources.py` & `django-import-export-4.0.0rc1/import_export/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,24 +301,26 @@
             else:
                 self.update_instances.append(instance)
         else:
             if not self._is_using_transactions(kwargs) and self._is_dry_run(kwargs):
                 # we don't have transactions and we want to do a dry_run
                 pass
             else:
-                self.do_instance_save(instance)
+                self.do_instance_save(instance, is_create)
         self.after_save_instance(instance, row, **kwargs)
 
-    def do_instance_save(self, instance):
+    def do_instance_save(self, instance, is_create):
         """
         A method specifically to provide a single overridable hook for the instance
         save operation.
         For example, this can be overridden to implement update_or_create().
 
         :param instance: The model instance to be saved.
+        :param is_create: A boolean flag to indicate whether this is a new object
+                          to be created, or an existing object to be updated.
         """
         instance.save()
 
     def before_save_instance(self, instance, row, **kwargs):
         r"""
         Override to add additional logic. Does nothing by default.
 
@@ -862,18 +864,18 @@
         result.diff_headers = self.get_diff_headers()
         result.total_rows = len(dataset)
         db_connection = self.get_db_connection_name()
 
         try:
             with atomic_if_using_transaction(using_transactions, using=db_connection):
                 self.before_import(dataset, **kwargs)
+            self._check_import_id_fields(dataset.headers)
         except Exception as e:
             self.handle_import_error(result, e, raise_errors)
 
-        self._check_import_id_fields(dataset.headers)
         instance_loader = self._meta.instance_loader_class(self, dataset)
 
         # Update the total in case the dataset was altered by before_import()
         result.total_rows = len(dataset)
 
         if collect_failed_rows:
             result.add_dataset_headers(dataset.headers)
@@ -1117,32 +1119,43 @@
 
     def _is_dry_run(self, kwargs):
         return kwargs.get("dry_run", False)
 
     def _check_import_id_fields(self, headers):
         import_id_fields = list()
         missing_fields = list()
+        missing_headers = list()
 
         for field_name in self.get_import_id_fields():
             if field_name not in self.fields:
                 missing_fields.append(field_name)
             else:
                 import_id_fields.append(self.fields[field_name])
 
+        if missing_fields:
+            raise exceptions.FieldError(
+                _(
+                    "The following fields are declared in 'import_id_fields' but "
+                    "are not present in the resource fields: %s"
+                    % ", ".join(missing_fields)
+                )
+            )
+
         for field in import_id_fields:
             if not headers or field.column_name not in headers:
                 # escape to be safe (exception could end up in logs)
                 col = escape(field.column_name)
-                missing_fields.append(col)
+                missing_headers.append(col)
 
-        if missing_fields:
+        if missing_headers:
             raise exceptions.FieldError(
                 _(
                     "The following fields are declared in 'import_id_fields' but "
-                    "are not present in the resource: %s" % ", ".join(missing_fields)
+                    "are not present in the file headers: %s"
+                    % ", ".join(missing_headers)
                 )
             )
 
 
 class ModelResource(Resource, metaclass=ModelDeclarativeMetaclass):
     """
     ModelResource is Resource subclass for handling Django models.
```

### Comparing `django-import-export-4.0.0rc0/import_export/results.py` & `django-import-export-4.0.0rc1/import_export/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+import logging
 from collections import OrderedDict
 
 from django.core.exceptions import NON_FIELD_ERRORS
 from django.utils.encoding import force_str
+from django.utils.translation import gettext_lazy as _
 from tablib import Dataset
 
+logger = logging.getLogger(__name__)
+
 
 class Error:
     def __init__(self, error, traceback=None, row=None, number=None):
         self.error = error
         self.traceback = traceback
         self.row = row
         self.number = number
@@ -106,15 +110,18 @@
         """
         return self.import_type in self.valid_import_types
 
     def add_instance_info(self, instance):
         if instance is not None:
             # Add object info to RowResult (e.g. for LogEntry)
             self.object_id = getattr(instance, "pk", None)
-            self.object_repr = force_str(instance)
+            try:
+                self.object_repr = force_str(instance)
+            except Exception as e:
+                logger.debug(_("call to force_str() on instance failed: %s" % str(e)))
 
 
 class InvalidRow:
     """A row that resulted in one or more ``ValidationError``
     being raised during import."""
 
     def __init__(self, number, validation_error, values):
```

### Comparing `django-import-export-4.0.0rc0/import_export/static/import_export/export_selectable_fields.js` & `django-import-export-4.0.0rc1/import_export/static/import_export/export_selectable_fields.js`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/static/import_export/guess_format.js` & `django-import-export-4.0.0rc1/import_export/static/import_export/guess_format.js`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/static/import_export/import.css` & `django-import-export-4.0.0rc1/import_export/static/import_export/import.css`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/templates/admin/import_export/base.html` & `django-import-export-4.0.0rc1/import_export/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/templates/admin/import_export/export.html` & `django-import-export-4.0.0rc1/import_export/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/templates/admin/import_export/import.html` & `django-import-export-4.0.0rc1/import_export/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/templates/admin/import_export/resource_fields_list.html` & `django-import-export-4.0.0rc1/import_export/templates/admin/import_export/resource_fields_list.html`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/tmp_storages.py` & `django-import-export-4.0.0rc1/import_export/tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/utils.py` & `django-import-export-4.0.0rc1/import_export/utils.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/import_export/widgets.py` & `django-import-export-4.0.0rc1/import_export/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     def render(self, value, obj=None):
         self._obj_deprecation_warning(obj)
         if self.coerce_to_string:
             return (
                 ""
                 if value is None or not isinstance(value, numbers.Number)
-                else number_format(value)
+                else "" + number_format(value)
             )
         return value
 
 
 class FloatWidget(NumberWidget):
     """
     Widget for converting float fields.
@@ -398,16 +398,20 @@
     def clean(self, value, row=None, **kwargs):
         return value.split(self.separator) if value else []
 
     def render(self, value, obj=None):
         """
         :return: A string with values separated by ``separator``.
           If ``coerce_to_string`` is ``False``, the native array will be returned.
+          If ``value`` is None, None will be returned if ``coerce_to_string``
+            is ``False``, otherwise an empty string will be returned.
         """
         self._obj_deprecation_warning(obj)
+        if value is None:
+            return "" if self.coerce_to_string is True else None
         if not self.coerce_to_string:
             return value
         return self.separator.join(str(v) for v in value)
 
 
 class JSONWidget(Widget):
     """
```

### Comparing `django-import-export-4.0.0rc0/pyproject.toml` & `django-import-export-4.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/runtests.py` & `django-import-export-4.0.0rc1/runtests.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/runtests.sh` & `django-import-export-4.0.0rc1/runtests.sh`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/admin.py` & `django-import-export-4.0.0rc1/tests/core/admin.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/exports/books-empty-author-email.xlsx` & `django-import-export-4.0.0rc1/tests/core/exports/books-empty-author-email.xlsx`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/exports/books.json` & `django-import-export-4.0.0rc1/tests/core/exports/books.json`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/exports/books.xls` & `django-import-export-4.0.0rc1/tests/core/exports/books.xls`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/exports/books.xlsx` & `django-import-export-4.0.0rc1/tests/core/exports/books.xlsx`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/fixtures/book.json` & `django-import-export-4.0.0rc1/tests/core/fixtures/book.json`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/forms.py` & `django-import-export-4.0.0rc1/tests/core/forms.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/migrations/0001_initial.py` & `django-import-export-4.0.0rc1/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/migrations/0003_withfloatfield.py` & `django-import-export-4.0.0rc1/tests/core/migrations/0003_withfloatfield.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/migrations/0004_bookwithchapters.py` & `django-import-export-4.0.0rc1/tests/core/migrations/0004_bookwithchapters.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/migrations/0005_addparentchild.py` & `django-import-export-4.0.0rc1/tests/core/migrations/0005_addparentchild.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/migrations/0007_auto_20180628_0411.py` & `django-import-export-4.0.0rc1/tests/core/migrations/0007_auto_20180628_0411.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/migrations/0008_auto_20190409_0846.py` & `django-import-export-4.0.0rc1/tests/core/migrations/0008_auto_20190409_0846.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/migrations/0009_auto_20211111_0807.py` & `django-import-export-4.0.0rc1/tests/core/migrations/0009_auto_20211111_0807.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/migrations/0010_uuidbook.py` & `django-import-export-4.0.0rc1/tests/core/migrations/0010_uuidbook.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py` & `django-import-export-4.0.0rc1/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/migrations/0014_bookwithchapternumbers.py` & `django-import-export-4.0.0rc1/tests/core/migrations/0014_bookwithchapternumbers.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/models.py` & `django-import-export-4.0.0rc1/tests/core/models.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/admin_integration/mixins.py` & `django-import-export-4.0.0rc1/tests/core/tests/admin_integration/mixins.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/admin_integration/test_action.py` & `django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_action.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/admin_integration/test_export.py` & `django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_export.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/admin_integration/test_import.py` & `django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         # issue 1722
         with mock.patch(
             "import_export.resources.Resource._check_import_id_fields"
         ) as mock_check_import_id_fields:
             mock_check_import_id_fields.side_effect = FieldError("some unknown error")
             response = self._do_import_post(self.book_import_url, "books.csv")
         self.assertEqual(response.status_code, 200)
-        target_msg = "Some unknown error"
+        target_msg = "some unknown error"
         self.assertIn(target_msg, str(response.content))
 
     @override_settings(LANGUAGE_CODE="es")
     def test_import_action_handles_ValueError_as_form_error_with_translation(self):
         with mock.patch(
             "import_export.admin.TempFolderStorage.read"
         ) as mock_tmp_folder_storage:
```

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/admin_integration/test_views.py` & `django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_views.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/resources.py` & `django-import-export-4.0.0rc1/tests/core/tests/resources.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_base_formats.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_base_formats.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import tablib
 from core.tests.utils import ignore_utcnow_deprecation_warning
 from django.test import TestCase
 from django.utils.encoding import force_str
 from tablib.core import UnsupportedFormat
 
 from import_export.formats import base_formats
+from import_export.widgets import NumberWidget
 
 
 class FormatTest(TestCase):
     def setUp(self):
         self.format = base_formats.Format()
 
     @mock.patch(
@@ -223,7 +224,15 @@
     #             "<tr><td>2</td>"
     #             "<td>evil_user</td>"
     #             '<td>&lt;script&gt;alert("I want to steal your credit card data")'
     #             "&lt;/script&gt;</td></tr>"
     #         ),
     #         res,
     #     )
+
+
+class YAMLFormatTest(TestCase):
+    def test_numeric_widget_export(self):
+        dataset = tablib.Dataset(headers=["id", "username"])
+        dataset.append((NumberWidget().render(1), "x"))
+        res = base_formats.YAML().export_data(dataset)
+        self.assertEqual("- {id: '1', username: x}\n", res)
```

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_declarative.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_declarative.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_fields.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_forms.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_instance_loaders.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_invalidrow.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_invalidrow.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_mixins.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_permissions.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_bulk_operations.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_bulk_operations.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_diffs.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_diffs.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_import_export.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_import_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,59 +277,70 @@
         self.book = Book.objects.create(name="The Hobbit")
         self.resource = ImportIdFieldsTestCase.BookResource()
 
     def test_custom_column_name_warns_if_not_present(self):
         dataset = tablib.Dataset(
             *[(self.book.pk, "Some book")], headers=["id", "wrong_name"]
         )
-        with self.assertRaises(exceptions.FieldError) as e:
-            self.resource.import_data(dataset)
+        with self.assertRaises(exceptions.ImportError) as e:
+            self.resource.import_data(dataset, raise_errors=True)
         self.assertEqual(
             "The following fields are declared in 'import_id_fields' "
-            "but are not present in the resource: book_name",
+            "but are not present in the file headers: book_name",
             str(e.exception),
         )
 
+    def test_custom_column_name_warns_if_not_present_as_error_in_result(self):
+        dataset = tablib.Dataset(
+            *[(self.book.pk, "Some book")], headers=["id", "wrong_name"]
+        )
+        res = self.resource.import_data(dataset, raise_errors=False)
+        target = (
+            "The following fields are declared in 'import_id_fields' "
+            "but are not present in the file headers: book_name"
+        )
+        self.assertEqual(target, str(res.base_errors[0].error))
+
     def test_missing_import_id_field_raises_exception(self):
         class TestBookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 import_id_fields = ("id", "a", "b")
 
         resource = TestBookResource()
 
         book = Book.objects.create(name="Some book")
         row = [book.pk, "Some book"]
         dataset = tablib.Dataset(*[row], headers=["id", "name"])
         dataset.append(row)
 
-        with self.assertRaises(exceptions.FieldError) as e:
-            resource.import_data(dataset)
+        with self.assertRaises(exceptions.ImportError) as e:
+            resource.import_data(dataset, raise_errors=True)
         self.assertEqual(
             "The following fields are declared in 'import_id_fields' "
-            "but are not present in the resource: a, b",
+            "but are not present in the resource fields: a, b",
             str(e.exception),
         )
 
     def test_multiple_import_id_fields(self):
         class BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 import_id_fields = ("id", "name", "author_email")
 
         self.resource = BookResource()
         dataset = tablib.Dataset(
             *[(self.book.pk, "Goldeneye", "ian.fleming@example.com")],
             headers=["A", "name", "B"],
         )
-        with self.assertRaises(exceptions.FieldError) as e:
-            self.resource.import_data(dataset)
+        with self.assertRaises(exceptions.ImportError) as e:
+            self.resource.import_data(dataset, raise_errors=True)
         self.assertEqual(
             "The following fields are declared in 'import_id_fields' "
-            "but are not present in the resource: id, author_email",
+            "but are not present in the file headers: id, author_email",
             str(e.exception),
         )
 
 
 class ImportWithMissingFields(TestCase):
     # issue 1517
```

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_misc.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_misc.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_data_handling.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_handling.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,9 +113,10 @@
         actual = result.rows[0].errors[0].error
         self.assertIsInstance(actual, (ValueError, InvalidOperation))
         self.assertIn(
             str(actual),
             {
                 "could not convert string to float",
                 "[<class 'decimal.ConversionSyntax'>]",
+                "Invalid literal for Decimal: 'foo'",
             },
         )
```

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_data_import.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_import.py`

 * *Files 21% similar despite different names*

```diff
@@ -121,7 +121,27 @@
         self.assertEqual(len(result.rows), 1)
         self.assertTrue(result.rows[0].diff)
         self.assertEqual(
             result.rows[0].import_type, results.RowResult.IMPORT_TYPE_UPDATE
         )
         self.assertEqual(result.rows[0].row_values.get("name"), None)
         self.assertEqual(result.rows[0].row_values.get("author_email"), None)
+
+    @ignore_widget_deprecation_warning
+    def test_import_data_new_override_do_instance_save(self):
+        class CustomDoInstanceSave(BookResource):
+            is_create = False
+
+            def do_instance_save(self, instance, is_create):
+                self.is_create = is_create
+                super().do_instance_save(instance, is_create)
+
+        Book.objects.all().delete()
+        self.assertEqual(0, Book.objects.count())
+        self.resource = CustomDoInstanceSave()
+        self.assertFalse(self.resource.is_create)
+
+        result = self.resource.import_data(self.dataset, raise_errors=True)
+
+        self.assertFalse(result.has_errors())
+        self.assertEqual(1, Book.objects.count())
+        self.assertTrue(self.resource.is_create)
```

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_error_handling.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_error_handling.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,19 +76,21 @@
 
         self.assertTrue(result.has_validation_errors())
         self.assertIs(result.rows[0].import_type, results.RowResult.IMPORT_TYPE_INVALID)
         self.assertIn("birthday", result.invalid_rows[0].field_specific_errors)
 
     def test_import_data_empty_dataset_with_collect_failed_rows(self):
         resource = AuthorResource()
-        with self.assertRaises(exceptions.FieldError) as e:
-            resource.import_data(tablib.Dataset(), collect_failed_rows=True)
+        with self.assertRaises(exceptions.ImportError) as e:
+            resource.import_data(
+                tablib.Dataset(), collect_failed_rows=True, raise_errors=True
+            )
         self.assertEqual(
             "The following fields are declared in 'import_id_fields' "
-            "but are not present in the resource: id",
+            "but are not present in the file headers: id",
             str(e.exception),
         )
 
     @ignore_widget_deprecation_warning
     def test_collect_failed_rows(self):
         resource = ProfileResource()
         headers = ["id", "user"]
```

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_export.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_export.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_fields.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_m2m.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_m2m.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_queryset.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_queryset.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_relationship.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_relationship.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_resource.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_resources/test_relationships.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_relationships.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_results.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_results.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from unittest.mock import patch
+
 from core.models import Book
 from django.core.exceptions import ValidationError
 from django.test.testcases import TestCase
 from tablib import Dataset
 
 from import_export.results import Error, Result, RowResult
 
@@ -57,14 +59,30 @@
 
     def test_add_instance_info(self):
         row_result = RowResult()
         row_result.add_instance_info(Book(pk=1, name="some book"))
         self.assertEqual(1, row_result.object_id)
         self.assertEqual("some book", row_result.object_repr)
 
+    @patch("import_export.results.logger")
+    def test_add_instance_info_instance_unserializable(self, mock_logger):
+        # issue 1763
+        class UnserializableBook(object):
+            # will raise TypeError
+            def __str__(self):
+                return None
+
+        row_result = RowResult()
+        row_result.add_instance_info(UnserializableBook())
+        mock_logger.debug.assert_called_with(
+            "call to force_str() on instance failed: "
+            "__str__ returned non-string (type NoneType)"
+        )
+        self.assertEqual(None, row_result.object_repr)
+
     def test_is_new(self):
         row_result = RowResult()
         self.assertFalse(row_result.is_new())
         row_result.import_type = RowResult.IMPORT_TYPE_NEW
         self.assertTrue(row_result.is_new())
         self.assertTrue(row_result.is_valid())
```

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_tmp_storages.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/test_widgets.py` & `django-import-export-4.0.0rc1/tests/core/tests/test_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -753,7 +753,17 @@
         s = "a,b,c"
         self.assertEqual(s, self.widget.render(v))
 
     def test_render_no_coerce_to_string(self):
         v = [1, 2, 3]
         self.widget = widgets.SimpleArrayWidget(coerce_to_string=False)
         self.assertEqual(v, self.widget.render(v))
+
+    def test_render_none_coerce_to_string_is_True(self):
+        self.widget = widgets.SimpleArrayWidget()
+        self.assertTrue(self.widget.coerce_to_string)
+        self.assertEqual("", self.widget.render(None))
+
+    def test_render_none_coerce_to_string_is_False(self):
+        self.widget = widgets.SimpleArrayWidget(coerce_to_string=False)
+        self.assertFalse(self.widget.coerce_to_string)
+        self.assertIsNone(self.widget.render(None))
```

### Comparing `django-import-export-4.0.0rc0/tests/core/tests/utils.py` & `django-import-export-4.0.0rc1/tests/core/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/docker-compose.yml` & `django-import-export-4.0.0rc1/tests/docker-compose.yml`

 * *Files 7% similar despite different names*

```diff
@@ -8,32 +8,33 @@
       DB_NAME: import_export
       IMPORT_EXPORT_POSTGRESQL_USER: ${IMPORT_EXPORT_POSTGRESQL_USER}
       IMPORT_EXPORT_POSTGRESQL_PASSWORD: ${IMPORT_EXPORT_POSTGRESQL_PASSWORD}
       POSTGRES_PASSWORD: ${IMPORT_EXPORT_POSTGRESQL_PASSWORD}
     image: postgres:13
     restart: "no"
     ports:
-      - "5432:5432"
+      - "${IMPORT_EXPORT_POSTGRESQL_PORT:-5432}:5432"
     volumes:
       - ./docker/db/init-postgres-db.sh/:/docker-entrypoint-initdb.d/init-postgres-db.sh
       - postgres-db-data:/var/lib/postgresql/data
   mysqldb:
     container_name: importexport_mysqldb
     image: mysql:8.0
     platform: linux/x86_64
     restart: "no"
     environment:
       MYSQL_DATABASE: import_export
       MYSQL_USER: ${IMPORT_EXPORT_MYSQL_USER}
       MYSQL_PASSWORD: ${IMPORT_EXPORT_MYSQL_PASSWORD}
       MYSQL_ROOT_PASSWORD: ${IMPORT_EXPORT_MYSQL_PASSWORD}
+      MYSQL_PORT:
     ports:
-      - "3306:3306"
+      - "${IMPORT_EXPORT_MYSQL_PORT:-3306}:3306"
     expose:
-      - '3306'
+      - '${IMPORT_EXPORT_MYSQL_PORT:-3306}'
     volumes:
       - ./docker/db/init-mysql-db.sh:/docker-entrypoint-initdb.d/init-mysql-db.sh
       - mysql-db-data:/var/lib/mysql
 
 volumes:
   postgres-db-data:
     driver: local
```

### Comparing `django-import-export-4.0.0rc0/tests/scripts/bulk_import.py` & `django-import-export-4.0.0rc1/tests/scripts/bulk_import.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc0/tests/settings.py` & `django-import-export-4.0.0rc1/tests/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     DATABASES = {
         "default": {
             "ENGINE": "django.db.backends.mysql",
             "NAME": "import_export",
             "USER": os.environ.get("IMPORT_EXPORT_MYSQL_USER"),
             "PASSWORD": os.environ.get("IMPORT_EXPORT_MYSQL_PASSWORD"),
             "HOST": "127.0.0.1",
-            "PORT": 3306,
+            "PORT": os.environ.get("IMPORT_EXPORT_MYSQL_PORT", "3306"),
             "TEST": {
                 "CHARSET": "utf8",
                 "COLLATION": "utf8_general_ci",
                 "NAME": "test_import_export",
             },
         }
     }
@@ -74,15 +74,15 @@
     DATABASES = {
         "default": {
             "ENGINE": "django.db.backends.postgresql",
             "NAME": "import_export",
             "USER": os.environ.get("IMPORT_EXPORT_POSTGRESQL_USER"),
             "PASSWORD": os.environ.get("IMPORT_EXPORT_POSTGRESQL_PASSWORD"),
             "HOST": "localhost",
-            "PORT": 5432,
+            "PORT": os.environ.get("IMPORT_EXPORT_POSTGRESQL_PORT", "5432"),
         }
     }
 else:
     if "test" in sys.argv:
         database_name = ""
     else:
         database_name = os.path.join(os.path.dirname(__file__), "database.db")
```

### Comparing `django-import-export-4.0.0rc0/tox.ini` & `django-import-export-4.0.0rc1/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -26,10 +26,12 @@
     -rrequirements/test.txt
 
 # if postgres / mysql environment variables exist, we can go ahead and run db specific tests
 passenv =
     COVERAGE
     IMPORT_EXPORT_POSTGRESQL_USER
     IMPORT_EXPORT_POSTGRESQL_PASSWORD
+    IMPORT_EXPORT_POSTGRESQL_PORT
     IMPORT_EXPORT_MYSQL_USER
     IMPORT_EXPORT_MYSQL_PASSWORD
+    IMPORT_EXPORT_MYSQL_PORT
     IMPORT_EXPORT_TEST_TYPE
```

