# Comparing `tmp/django-import-export-4.0.0rc1.tar.gz` & `tmp/django-import-export-4.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-import-export-4.0.0rc1.tar", last modified: Fri Mar 15 14:18:19 2024, max compression
+gzip compressed data, was "django-import-export-4.0.0rc2.tar", last modified: Mon Apr  8 18:43:19 2024, max compression
```

## Comparing `django-import-export-4.0.0rc1.tar` & `django-import-export-4.0.0rc2.tar`

### file list

```diff
@@ -1,332 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.288315 django-import-export-4.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.244315 django-import-export-4.0.0rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.244315 django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.244315 django-import-export-4.0.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-15 14:18:19.288315 django-import-export-4.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.284315 django-import-export-4.0.0rc1/django_import_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/django_import_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/django_import_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/django_import_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/django_import_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/django_import_export.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.252315 django-import-export-4.0.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.252315 django-import-export-4.0.0rc1/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/change-form-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/custom-export-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/custom-import-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/date-widget-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/django-import-export-change.png
--rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/django-import-export-export-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/django-import-export-import-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/django-import-export-import.png
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/export-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    33286 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/export_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/import-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/import_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/non-field-specific-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/_static/images/select-for-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/admin_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30548 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_admin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_forms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_instance_loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_mixins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_tmp_storages.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/api_widgets.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/bulk_import.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29802 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/export_workflow.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    10047 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.252315 django-import-export-4.0.0rc1/docs/image_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/image_src/export_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/image_src/import_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/import_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-15 14:18:19.000000 django-import-export-4.0.0rc1/import_export/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35020 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/formats/base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/instance_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.256315 django-import-export-4.0.0rc1/import_export/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.232315 django-import-export-4.0.0rc1/import_export/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/kz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/kz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/kz/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/kz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.260315 django-import-export-4.0.0rc1/import_export/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    48428 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.264315 django-import-export-4.0.0rc1/import_export/static/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/static/import_export/export.css
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/static/import_export/export_selectable_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/static/import_export/guess_format.js
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/static/import_export/import.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/import_export/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.268315 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list_export_item.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list_import.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list_import_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/change_list_import_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/export.html
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/import.html
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templates/admin/import_export/resource_fields_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.268315 django-import-export-4.0.0rc1/import_export/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/templatetags/import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21360 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/import_export/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.268315 django-import-export-4.0.0rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/runtests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/runtests.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 14:18:19.288315 django-import-export-4.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.268315 django-import-export-4.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/books-sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.268315 django-import-export-4.0.0rc1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.272315 django-import-export-4.0.0rc1/tests/core/exports/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/authors.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-ISO-8859-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-dos.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-empty-author-email.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-for-delete.csv
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-invalid-date.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-mac.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-mac.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-unicode.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books-unicode.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books.csv
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books.json
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books.xls
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/books.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/exports/child.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.272315 django-import-export-4.0.0rc1/tests/core/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/fixtures/author.json
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/fixtures/book.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/fixtures/category.json
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.276315 django-import-export-4.0.0rc1/tests/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0002_book_published_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0003_withfloatfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0004_bookwithchapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0005_addparentchild.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0006_auto_20171130_0147.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0007_auto_20180628_0411.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0008_auto_20190409_0846.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0009_auto_20211111_0807.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0010_uuidbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0012_delete_legacybook.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0013_alter_author_birthday.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/0014_bookwithchapternumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.236315 django-import-export-4.0.0rc1/tests/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.276315 django-import-export-4.0.0rc1/tests/core/templates/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.276315 django-import-export-4.0.0rc1/tests/core/templates/core/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/templates/core/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/templates/core/category_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.280315 django-import-export-4.0.0rc1/tests/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.280315 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    39409 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_instance_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_invalidrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.280315 django-import-export-4.0.0rc1/tests/core/tests/test_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.284315 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)    28373 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/tests/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.240315 django-import-export-4.0.0rc1/tests/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.284315 django-import-export-4.0.0rc1/tests/docker/db/
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/docker/db/init-mysql-db.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/docker/db/init-postgres-db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:19.284315 django-import-export-4.0.0rc1/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/scripts/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-15 14:18:14.000000 django-import-export-4.0.0rc1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.729486 django-import-export-4.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.689487 django-import-export-4.0.0rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.689487 django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.689487 django-import-export-4.0.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-08 18:43:19.729486 django-import-export-4.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.725486 django-import-export-4.0.0rc2/django_import_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/django_import_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/django_import_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/django_import_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/django_import_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/django_import_export.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.697486 django-import-export-4.0.0rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.697486 django-import-export-4.0.0rc2/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/change-form-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/custom-export-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/custom-import-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/date-widget-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/django-import-export-change.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/django-import-export-export-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/django-import-export-import-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/django-import-export-import.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/export-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33286 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/export_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/import-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/import_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/non-field-specific-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/select-for-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/admin_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30548 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_forms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_instance_loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_tmp_storages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_widgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/bulk_import.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30218 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/export_workflow.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10047 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.697486 django-import-export-4.0.0rc2/docs/image_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/image_src/export_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/image_src/import_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/import_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/import_export/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35251 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/formats/base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/instance_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/kz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/kz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/kz/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/kz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48286 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/static/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/static/import_export/export.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/static/import_export/export_selectable_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/static/import_export/guess_format.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/static/import_export/import.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/export.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/resource_fields_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templatetags/import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21360 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/runtests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/runtests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:43:19.729486 django-import-export-4.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.713486 django-import-export-4.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/books-sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.713486 django-import-export-4.0.0rc2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.713486 django-import-export-4.0.0rc2/tests/core/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/authors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-ISO-8859-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-dos.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-empty-author-email.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-for-delete.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-invalid-date.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-mac.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-mac.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-unicode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-unicode.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/child.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.717486 django-import-export-4.0.0rc2/tests/core/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/fixtures/author.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/fixtures/book.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/fixtures/category.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.717486 django-import-export-4.0.0rc2/tests/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0002_book_published_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0003_withfloatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0004_bookwithchapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0005_addparentchild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0006_auto_20171130_0147.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0007_auto_20180628_0411.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0008_auto_20190409_0846.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0009_auto_20211111_0807.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0010_uuidbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0012_delete_legacybook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0013_alter_author_birthday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0014_bookwithchapternumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/tests/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.717486 django-import-export-4.0.0rc2/tests/core/templates/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.717486 django-import-export-4.0.0rc2/tests/core/templates/core/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/templates/core/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/templates/core/category_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.721486 django-import-export-4.0.0rc2/tests/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.721486 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41866 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_instance_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_invalidrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.721486 django-import-export-4.0.0rc2/tests/core/tests/test_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.725486 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28373 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/tests/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.725486 django-import-export-4.0.0rc2/tests/docker/db/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/docker/db/init-mysql-db.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/docker/db/init-postgres-db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.725486 django-import-export-4.0.0rc2/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/scripts/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tox.ini
```

### Comparing `django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/.github/ISSUE_TEMPLATE/question.md` & `django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/.github/stale.yml` & `django-import-export-4.0.0rc2/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/.github/workflows/release.yml` & `django-import-export-4.0.0rc2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/.github/workflows/test.yml` & `django-import-export-4.0.0rc2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/AUTHORS` & `django-import-export-4.0.0rc2/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/CODE_OF_CONDUCT.md` & `django-import-export-4.0.0rc2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/LICENSE` & `django-import-export-4.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/Makefile` & `django-import-export-4.0.0rc2/Makefile`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/PKG-INFO` & `django-import-export-4.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.0rc1
+Version: 4.0.0rc2
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `django-import-export-4.0.0rc1/README.rst` & `django-import-export-4.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/RELEASE.md` & `django-import-export-4.0.0rc2/RELEASE.md`

 * *Files 14% similar despite different names*

```diff
@@ -25,7 +25,9 @@
 The webhook endpoint on readthedocs is configured using
 [these instructions](https://docs.readthedocs.io/en/latest/guides/setup/git-repo-manual.html).
 
 This is implemented using a Webhook defined in the Github repo (Settings / Webhooks).
 
 readthedocs should be checked after each release to ensure that the docs have built correctly.
 Login to [readthedocs.org](https://readthedocs.org) to check that the build ran OK (click on 'Builds' tab).
+
+For pre-releases, the release version has to be activated via the readthedocs UI before it can be built.
```

### Comparing `django-import-export-4.0.0rc1/django_import_export.egg-info/PKG-INFO` & `django-import-export-4.0.0rc2/django_import_export.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.0rc1
+Version: 4.0.0rc2
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `django-import-export-4.0.0rc1/django_import_export.egg-info/SOURCES.txt` & `django-import-export-4.0.0rc2/django_import_export.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
 tests/core/exports/books-ISO-8859-1.csv
 tests/core/exports/books-dos.csv
 tests/core/exports/books-empty-author-email.xlsx
 tests/core/exports/books-for-delete.csv
 tests/core/exports/books-invalid-date.csv
 tests/core/exports/books-mac.csv
 tests/core/exports/books-mac.tsv
+tests/core/exports/books-no-headers.csv
 tests/core/exports/books-unicode.csv
 tests/core/exports/books-unicode.tsv
 tests/core/exports/books.csv
 tests/core/exports/books.json
 tests/core/exports/books.xls
 tests/core/exports/books.xlsx
 tests/core/exports/child.csv
```

### Comparing `django-import-export-4.0.0rc1/docs/Makefile` & `django-import-export-4.0.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/change-form-export.png` & `django-import-export-4.0.0rc2/docs/_static/images/change-form-export.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/custom-export-form.png` & `django-import-export-4.0.0rc2/docs/_static/images/custom-export-form.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/custom-import-form.png` & `django-import-export-4.0.0rc2/docs/_static/images/custom-import-form.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/date-widget-validation-error.png` & `django-import-export-4.0.0rc2/docs/_static/images/date-widget-validation-error.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/django-import-export-change.png` & `django-import-export-4.0.0rc2/docs/_static/images/django-import-export-change.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/django-import-export-export-confirm.png` & `django-import-export-4.0.0rc2/docs/_static/images/django-import-export-export-confirm.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/django-import-export-import-confirm.png` & `django-import-export-4.0.0rc2/docs/_static/images/django-import-export-import-confirm.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/django-import-export-import.png` & `django-import-export-4.0.0rc2/docs/_static/images/django-import-export-import.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/export-button.png` & `django-import-export-4.0.0rc2/docs/_static/images/export-button.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/export_workflow.svg` & `django-import-export-4.0.0rc2/docs/_static/images/export_workflow.svg`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/import-button.png` & `django-import-export-4.0.0rc2/docs/_static/images/import-button.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/import_workflow.svg` & `django-import-export-4.0.0rc2/docs/_static/images/import_workflow.svg`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/non-field-specific-validation-error.png` & `django-import-export-4.0.0rc2/docs/_static/images/non-field-specific-validation-error.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/_static/images/select-for-export.png` & `django-import-export-4.0.0rc2/docs/_static/images/select-for-export.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/admin_integration.rst` & `django-import-export-4.0.0rc2/docs/admin_integration.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/advanced_usage.rst` & `django-import-export-4.0.0rc2/docs/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/api_mixins.rst` & `django-import-export-4.0.0rc2/docs/api_mixins.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/api_widgets.rst` & `django-import-export-4.0.0rc2/docs/api_widgets.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/bulk_import.rst` & `django-import-export-4.0.0rc2/docs/bulk_import.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/changelog.rst` & `django-import-export-4.0.0rc2/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 Changelog
 =========
 
 .. warning::
 
     Version 4 introduces breaking changes.  Please refer to :doc:`release notes<release_notes>`.
 
-4.0.0-rc.1 (unreleased)
+4.0.0-rc.2 (2024-04-08)
+-----------------------
+
+- Add form error if source file contains invalid header (#1780)
+- Fix for incorrect header order on 'confirm' page (#1786)
+- Remove unneeded format method overrides (#1785)
+- Support dynamic selection of Resource class based on request property (#1787)
+
+4.0.0-rc.1 (2024-03-15)
 -----------------------
 
 - added try / catch to :meth:`~import_export.results.RowResult.add_instance_info` to handle unserializable instances (#1767)
 - fix: YAML export does not work with SafeString (#1762)
 - pass ``is_create``` param into :meth:`~import_export.resources.Resource.do_instance_save` (#1772)
 - fix: :meth:`~import_export.widgets.SimpleArrayWidget.render` crashes if value is ``None`` (#1771)
 - updated translations for release-4 (#1775)
@@ -90,14 +98,19 @@
 - Updated Admin integration documentation to clarify how to save custom form values (#1746)
 
 Performance
 ###########
 
 - Fix slow export with ForeignKey id (#1717)
 
+3.3.8 (2024-04-08)
+------------------
+
+- Add additional django template block for extending import page (#1776)
+
 3.3.7 (2024-02-03)
 ------------------
 
 - Pass :meth:`~import_export.mixins.BaseExportMixin.get_export_resource_kwargs` to Resource constructor
   :meth:`~import_export.admin.ExportMixin.export_action` (#1739)
 - Fix issue with model class passed to Resource constructor crashing on export (#1745)
 - Fix indentation for skip_row docstring (#1743)
```

### Comparing `django-import-export-4.0.0rc1/docs/conf.py` & `django-import-export-4.0.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/contributing.rst` & `django-import-export-4.0.0rc2/docs/contributing.rst`

 * *Files 4% similar despite different names*

```diff
@@ -128,14 +128,17 @@
 into django-import-export proper, which may take substantial time for the all-volunteer team to get to.
 
 .. _`AUTHORS`: https://github.com/django-import-export/django-import-export/blob/main/AUTHORS
 
 Development
 -----------
 
+Formatting
+^^^^^^^^^^
+
 * All files should be formatted using the black auto-formatter. This will be run by pre-commit if configured.
 
 * The project repository includes an ``.editorconfig`` file. We recommend using a text editor with EditorConfig support
   to avoid indentation and whitespace issues.
 
 * We allow up to 88 characters as this is the line length used by black. This check is included when you run flake8.
   Documentation, comments, and docstrings should be wrapped at 79 characters, even though PEP 8 suggests 72.
@@ -149,23 +152,34 @@
     pre-commit install
 
 * If using ``git blame``, you can ignore commits which made large changes to the code base, such as reformatting.
   Run this command from the base project directory::
 
     git config blame.ignoreRevsFile .git-blame-ignore-revs
 
+.. _create_venv:
+
+Create virtual environment
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
 Once you have cloned and checked out the repository, you can install a new development environment as follows::
 
   python -m venv django-import-export-venv
   source django-import-export-venv/bin/activate
   pip install -r requirements/base.txt -r requirements/test.txt
 
+Run tests
+^^^^^^^^^
+
 You can run the test suite with::
 
   make clean test
 
+Build documentation
+^^^^^^^^^^^^^^^^^^^
+
 To build a local version of the documentation::
 
   pip install -r requirements/docs.txt
   make build-html-doc
 
 The documentation will be present in ``docs/_build/html/index.html``.
```

### Comparing `django-import-export-4.0.0rc1/docs/export_workflow.rst` & `django-import-export-4.0.0rc2/docs/export_workflow.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/faq.rst` & `django-import-export-4.0.0rc2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/getting_started.rst` & `django-import-export-4.0.0rc2/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/image_src/export_workflow.txt` & `django-import-export-4.0.0rc2/docs/image_src/export_workflow.txt`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/image_src/import_workflow.txt` & `django-import-export-4.0.0rc2/docs/image_src/import_workflow.txt`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/import_workflow.rst` & `django-import-export-4.0.0rc2/docs/import_workflow.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/index.rst` & `django-import-export-4.0.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/installation.rst` & `django-import-export-4.0.0rc2/docs/installation.rst`

 * *Files 5% similar despite different names*

```diff
@@ -220,18 +220,18 @@
 
 .. _exampleapp:
 
 Example app
 ===========
 
 There's an example application that showcases what import_export can do.
-It's assumed that you have set up a Python ``venv`` with all required dependencies
-(from ``test.txt`` requirements file) and are able to run Django locally.
 
-You can run the example application as follows::
+Before starting, set up a virtual environment ("venv") using :ref:`these instructions<create_venv>`.
+
+You can initialize and run the example application as follows::
 
     cd tests
     ./manage.py makemigrations
     ./manage.py migrate
     ./manage.py createsuperuser
     ./manage.py loaddata author.json category.json book.json
     ./manage.py runserver
```

### Comparing `django-import-export-4.0.0rc1/docs/make.bat` & `django-import-export-4.0.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/docs/release_notes.rst` & `django-import-export-4.0.0rc2/docs/release_notes.rst`

 * *Files 10% similar despite different names*

```diff
@@ -131,31 +131,29 @@
 
 
 See `this issue <https://github.com/django-import-export/django-import-export/issues/1724>`_.
 
 API changes
 ===========
 
-v4 of import-export contains a number of minor changes to the API.
+v4 of import-export contains a number of changes to the API.  These changes are summarized in the table below.
+Refer to
+`this PR <https://github.com/django-import-export/django-import-export/pull/1641/>`_ for detailed information.
+
+If you have customized import-export by overriding methods, then you may have to modify your installation before
+working with v4.
 
-If you have customized import-export by overriding methods, then you will have to
-modify your installation before working with v4.  If you have not overridden any
-methods then you should not be affected by these changes and no changes to your code
+If you have not overridden any methods then you should not be affected by these changes and no changes to your code
 should be necessary.
 
-The API changes include changes to method arguments, although some method names have
-changed.
-
-Refer to
-`this PR <https://github.com/django-import-export/django-import-export/pull/1641/>`_
-for more information.
+The API changes include changes to method arguments, although some method names have changed.
 
 Methods which process row data have been updated so that method args are standardized.
-This has been done to resolve inconsistency issues where the parameters differed between
-method calls, and to allow easier extensibility.
+This has been done to resolve inconsistency issues where the parameters differed between method calls, and to allow
+easier extensibility.
 
 :class:`import_export.resources.Resource`
 -----------------------------------------
 
 .. _renamed_methods:
 
 Renamed methods
@@ -254,14 +252,19 @@
 
    * - ``after_delete_instance(self, instance, dry_run)``
      - ``after_delete_instance(self, instance, row, **kwargs)``
      - * ``row`` added as mandatory arg
        * ``dry_run`` param now in ``kwargs``
        * ``using_transactions`` param now in ``kwargs``
 
+   * - ``import_field(self, field, obj, data, is_m2m=False, **kwargs)``
+     - ``import_field(self, field, instance, row, is_m2m=False, **kwargs):``
+     - * ``obj`` renamed to ``instance``
+       * ``data`` renamed to ``row``
+
    * - ``before_export(self, queryset, *args, **kwargs)``
      - ``before_export(self, queryset, **kwargs)``
      - * unused ``*args`` list removed
 
    * - ``after_export(self, queryset, data, *args, **kwargs)``
      - ``after_export(self, queryset, dataset, **kwargs)``
      - * unused ``*args`` list removed
@@ -271,18 +274,49 @@
      - ``filter_export(self, queryset, **kwargs)``
      - * unused ``*args`` list removed
 
    * - ``export_field(self, field, obj)``
      - ``export_field(self, field, instance)``
      - * ``obj`` renamed to ``instance``
 
+   * - ``export_resource(self, obj)``
+     - ``export_resource(self, instance, fields=None)``
+     - * ``obj`` renamed to ``instance``
+       * ``fields`` passed as kwarg
+
    * - ``export(self, *args, queryset=None, **kwargs)``
      - ``export(self, queryset=None, **kwargs)``
      - * unused ``*args`` list removed
 
+   * - ``get_export_headers(self)``
+     - ``get_export_headers(self, fields=None)``
+     - * ``fields`` passed as kwarg
+
+
+:class:`import_export.mixins.BaseImportExportMixin`
+---------------------------------------------
+
+Parameter changes
+^^^^^^^^^^^^^^^^^
+
+.. list-table::
+   :header-rows: 1
+
+   * - Previous
+     - New
+     - Summary
+
+   * - ``get_resource_classes(self)``
+     - ``get_resource_classes(self, request)``
+     -  * Added ``request`` param
+
+   * - ``get_resource_kwargs(self, request, *args, **kwargs)``
+     - ``get_resource_kwargs(self, request, **kwargs)``
+     -  * unused ``*args`` list removed
+
 :class:`import_export.mixins.BaseImportMixin`
 ---------------------------------------------
 
 Parameter changes
 ^^^^^^^^^^^^^^^^^
 
 .. list-table::
@@ -290,44 +324,53 @@
 
    * - Previous
      - New
      - Summary
 
    * - ``get_import_resource_kwargs(self, request, *args, **kwargs)``
      - ``get_import_resource_kwargs(self, request, **kwargs)``
-     -  * ``using_transactions`` param now in ``kwargs``
-        * ``dry_run`` param now in ``kwargs``
-        * unused ``*args`` list removed
+     -  * unused ``*args`` list removed
 
+   * - ``get_import_resource_classes(self)``
+     - ``get_import_resource_classes(self, request)``
+     -  * Added ``request`` param
+
+   * - ``choose_import_resource_class(self, form)``
+     - ``choose_import_resource_class(self, form, request)``
+     -  * Added ``request`` param
 
 :class:`import_export.mixins.BaseExportMixin`
 ---------------------------------------------
 
 Parameter changes
 ^^^^^^^^^^^^^^^^^
 
 .. list-table::
    :header-rows: 1
 
    * - Previous
      - New
      - Summary
 
-   * - ``get_export_resource_kwargs(self, request, *args, **kwargs)``
-     - ``get_export_resource_kwargs(self, request, **kwargs)``
-     -  * unused ``*args`` list removed
+   * - ``get_export_resource_classes(self)``
+     - ``get_export_resource_classes(self, request)``
+     -  * Added ``request`` param
 
    * - ``get_export_resource_kwargs(self, request, *args, **kwargs)``
      - ``get_export_resource_kwargs(self, request, **kwargs)``
      -  * unused ``*args`` list removed
 
-   * - ``get_data_for_export(self, request, *args, **kwargs)``
+   * - ``get_data_for_export(self, request, queryset, *args, **kwargs)``
      - ``get_data_for_export(self, request, queryset, **kwargs)``
      -  * unused ``*args`` list removed
 
+   * - ``choose_export_resource_class(self, form)``
+     - ``choose_export_resource_class(self, form, request)``
+     -  * Added ``request`` param
+
 
 :class:`import_export.fields.Field`
 -----------------------------------
 
 Parameter changes
 ^^^^^^^^^^^^^^^^^
 
@@ -361,21 +404,25 @@
 
 If you have subclassed one of the :mod:`~import_export.forms` then you may need to
 modify the parameters passed to constructors.
 
 The ``input_format`` field of :class:`~import_export.forms.ImportForm` has been moved to the parent class
 (:class:`~import_export.forms.ImportExportFormBase`) and renamed to ``format``.
 
+The ``file_format`` field of :class:`~import_export.forms.ExportForm` has been removed and is now replaced by
+:attr:`~import_export.forms.ImportExportFormBase.format`.
+
 Parameter changes
 ^^^^^^^^^^^^^^^^^
 
 .. list-table::
    :header-rows: 1
 
    * - Previous
      - New
      - Summary
 
    * - ``__init__(self, *args, resources=None, **kwargs)``
-     - ``__init__(self, formats, resources, *args, **kwargs)``
+     - ``__init__(self, formats, resources, **kwargs)``
      - * ``formats`` added as a mandatory arg
        * ``resources`` added as a mandatory arg
+       * unused ``*args`` list removed
```

### Comparing `django-import-export-4.0.0rc1/docs/testing.rst` & `django-import-export-4.0.0rc2/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/admin.py` & `django-import-export-4.0.0rc2/import_export/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                 self.admin_site.admin_view(self.import_action),
                 name="%s_%s_import" % info,
             ),
         ]
         return my_urls + urls
 
     @method_decorator(require_POST)
-    def process_import(self, request, *args, **kwargs):
+    def process_import(self, request, **kwargs):
         """
         Perform the actual import action (after the user has confirmed the import)
         """
         if not self.has_import_permission(request):
             raise PermissionDenied
 
         confirm_form = self.create_confirm_form(request)
@@ -169,41 +169,36 @@
                 encoding=encoding,
                 read_mode=input_format.get_read_mode(),
                 **self.get_tmp_storage_class_kwargs(),
             )
 
             data = tmp_storage.read()
             dataset = input_format.create_dataset(data)
-            result = self.process_dataset(
-                dataset, confirm_form, request, *args, **kwargs
-            )
+            result = self.process_dataset(dataset, confirm_form, request, **kwargs)
 
             tmp_storage.remove()
 
             return self.process_result(result, request)
 
     def process_dataset(
         self,
         dataset,
-        confirm_form,
+        form,
         request,
-        *args,
         **kwargs,
     ):
-        res_kwargs = self.get_import_resource_kwargs(
-            request, form=confirm_form, **kwargs
-        )
-        resource = self.choose_import_resource_class(confirm_form)(**res_kwargs)
-        imp_kwargs = self.get_import_data_kwargs(request, form=confirm_form, **kwargs)
+        res_kwargs = self.get_import_resource_kwargs(request, **kwargs)
+        resource = self.choose_import_resource_class(form, request)(**res_kwargs)
+        imp_kwargs = self.get_import_data_kwargs(request=request, form=form, **kwargs)
         imp_kwargs["retain_instance_in_row_result"] = True
 
         return resource.import_data(
             dataset,
             dry_run=False,
-            file_name=confirm_form.cleaned_data.get("original_file_name"),
+            file_name=form.cleaned_data.get("original_file_name"),
             user=request.user,
             **imp_kwargs,
         )
 
     def process_result(self, result, request):
         self.generate_log_entries(result, request)
         self.add_success_message(result, request)
@@ -282,15 +277,15 @@
         * :meth:`~import_export.admin.ImportMixin.get_import_form_initial`
         * :meth:`~import_export.mixins.BaseImportMixin.get_import_resource_classes`
         """
         formats = self.get_import_formats()
         form_class = self.get_import_form_class(request)
         kwargs = self.get_import_form_kwargs(request)
 
-        return form_class(formats, self.get_import_resource_classes(), **kwargs)
+        return form_class(formats, self.get_import_resource_classes(request), **kwargs)
 
     def get_import_form_class(self, request):
         """
         .. versionadded:: 3.0
 
         Return the form class to use for the 'import' step. If you only have
         a single custom form class, you can set the ``import_form_class``
@@ -385,23 +380,23 @@
                 "import_file"
             ].tmp_storage_name,
             "original_file_name": import_form.cleaned_data["import_file"].name,
             "format": import_form.cleaned_data["format"],
             "resource": import_form.cleaned_data.get("resource", ""),
         }
 
-    def get_import_data_kwargs(self, request, *args, **kwargs):
+    def get_import_data_kwargs(self, **kwargs):
         """
         Prepare kwargs for import_data.
         """
         form = kwargs.get("form")
         if form:
             kwargs.pop("form")
             return kwargs
-        return {}
+        return kwargs
 
     def write_to_tmp_storage(self, import_file, input_format):
         encoding = None
         if not input_format.is_binary():
             encoding = self.from_encoding
 
         tmp_storage_cls = self.get_tmp_storage_class()
@@ -421,15 +416,15 @@
         exc_name = repr(type(e).__name__)
         msg = _(
             "%(exc_name)s encountered while trying to read file. "
             "Ensure you have chosen the correct format for the file."
         ) % {"exc_name": exc_name}
         form.add_error("import_file", msg)
 
-    def import_action(self, request, *args, **kwargs):
+    def import_action(self, request, **kwargs):
         """
         Perform a dry_run of the import to make sure the import will not
         result in errors.  If there are no errors, save the user
         uploaded file to a local temp file that will be used by
         'process_import' for the actual import.
         """
         if not self.has_import_permission(request):
@@ -461,15 +456,14 @@
                 except Exception as e:
                     self.add_data_read_fail_error_to_form(import_form, e)
                 if not import_form.errors:
                     result = self.process_dataset(
                         dataset,
                         import_form,
                         request,
-                        *args,
                         raise_errors=False,
                         rollback_on_validation_errors=True,
                         **kwargs,
                     )
                     if not result.has_errors() and not result.has_validation_errors():
                         return self.process_result(result, request)
                     else:
@@ -485,28 +479,37 @@
                 try:
                     # then read the file, using the proper format-specific mode
                     # warning, big files may exceed memory
                     data = tmp_storage.read()
                     dataset = input_format.create_dataset(data)
                 except Exception as e:
                     self.add_data_read_fail_error_to_form(import_form, e)
+                else:
+                    if len(dataset) == 0:
+                        import_form.add_error(
+                            "import_file",
+                            _(
+                                "No valid data to import. Ensure your file "
+                                "has the correct headers or data for import."
+                            ),
+                        )
 
                 if not import_form.errors:
                     # prepare kwargs for import data, if needed
                     res_kwargs = self.get_import_resource_kwargs(
                         request, form=import_form, **kwargs
                     )
-                    resource = self.choose_import_resource_class(import_form)(
+                    resource = self.choose_import_resource_class(import_form, request)(
                         **res_kwargs
                     )
                     resources = [resource]
 
                     # prepare additional kwargs for import_data, if needed
                     imp_kwargs = self.get_import_data_kwargs(
-                        request, *args, form=import_form, **kwargs
+                        request=request, form=import_form, **kwargs
                     )
                     try:
                         result = resource.import_data(
                             dataset,
                             dry_run=True,
                             raise_errors=False,
                             file_name=import_file.name,
@@ -523,17 +526,17 @@
                                 request, import_form=import_form
                             )
                     except exceptions.FieldError as e:
                         messages.error(request, str(e))
 
         else:
             res_kwargs = self.get_import_resource_kwargs(
-                request, form=import_form, **kwargs
+                request=request, form=import_form, **kwargs
             )
-            resource_classes = self.get_import_resource_classes()
+            resource_classes = self.get_import_resource_classes(request)
             resources = [
                 resource_class(**res_kwargs) for resource_class in resource_classes
             ]
 
         context.update(self.admin_site.each_context(request))
 
         context["title"] = _("Import")
@@ -683,19 +686,18 @@
         # it is enough to get its results
         if hasattr(cl, "queryset"):
             return cl.queryset
 
         # Fallback in case the ChangeList doesn't have queryset attribute set
         return cl.get_queryset(request)
 
-    def get_export_data(self, file_format, queryset, *args, **kwargs):
+    def get_export_data(self, file_format, request, queryset, **kwargs):
         """
         Returns file_format representation for given queryset.
         """
-        request = kwargs.pop("request")
         if not self.has_export_permission(request):
             raise PermissionDenied
 
         data = self.get_data_for_export(
             request,
             queryset,
             **kwargs,
@@ -722,15 +724,15 @@
         if not self.has_export_permission(request):
             raise PermissionDenied
 
         form_type = self.get_export_form_class()
         formats = self.get_export_formats()
         form = form_type(
             formats,
-            self.get_export_resource_classes(),
+            self.get_export_resource_classes(request),
             data=request.POST or None,
         )
         form.fields["export_items"] = MultipleChoiceField(
             widget=MultipleHiddenInput,
             required=False,
             choices=[(o.id, o.id) for o in self.model.objects.all()],
         )
@@ -746,16 +748,16 @@
                 )
             else:
                 queryset = self.get_export_queryset(request)
 
             try:
                 export_data = self.get_export_data(
                     file_format,
+                    request,
                     queryset,
-                    request=request,
                     encoding=self.to_encoding,
                     export_form=form,
                 )
                 content_type = file_format.get_content_type()
                 response = HttpResponse(export_data, content_type=content_type)
                 response["Content-Disposition"] = 'attachment; filename="%s"' % (
                     self.get_export_filename(request, queryset, file_format),
@@ -791,15 +793,15 @@
                 [
                     field.column_name
                     for field in res(
                         **self.get_export_resource_kwargs(request)
                     ).get_user_visible_fields()
                 ],
             )
-            for res in self.get_export_resource_classes()
+            for res in self.get_export_resource_classes(request)
         ]
         return context
 
 
 class ImportExportMixin(ImportMixin, ExportMixin):
     """
     Import and export mixin.
@@ -857,28 +859,28 @@
         if (
             getattr(settings, "IMPORT_EXPORT_SKIP_ADMIN_ACTION_EXPORT_UI", False)
             is True
         ):
             file_format = formats[0]()
 
             export_data = self.get_export_data(
-                file_format, queryset, request=request, encoding=self.to_encoding
+                file_format, request, queryset, encoding=self.to_encoding
             )
             content_type = file_format.get_content_type()
             response = HttpResponse(export_data, content_type=content_type)
             response["Content-Disposition"] = 'attachment; filename="%s"' % (
                 self.get_export_filename(request, queryset, file_format),
             )
             return response
 
         form_type = self.get_export_form_class()
         formats = self.get_export_formats()
         form = form_type(
             formats=formats,
-            resources=self.get_export_resource_classes(),
+            resources=self.get_export_resource_classes(request),
             initial={"export_items": list(queryset.values_list("id", flat=True))},
         )
         # selected items are to be stored as a hidden input on the form
         form.fields["export_items"] = MultipleChoiceField(
             widget=MultipleHiddenInput,
             required=False,
             choices=[(str(o), str(o)) for o in queryset.all()],
```

### Comparing `django-import-export-4.0.0rc1/import_export/declarative.py` & `django-import-export-4.0.0rc2/import_export/declarative.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/exceptions.py` & `django-import-export-4.0.0rc2/import_export/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/fields.py` & `django-import-export-4.0.0rc2/import_export/fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/formats/base_formats.py` & `django-import-export-4.0.0rc2/import_export/formats/base_formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,17 +141,14 @@
     CONTENT_TYPE = "text/yaml"
 
 
 class TSV(TextFormat):
     TABLIB_MODULE = "tablib.formats._tsv"
     CONTENT_TYPE = "text/tab-separated-values"
 
-    def create_dataset(self, in_stream, **kwargs):
-        return super().create_dataset(in_stream, **kwargs)
-
 
 class ODS(TextFormat):
     TABLIB_MODULE = "tablib.formats._ods"
     CONTENT_TYPE = "application/vnd.oasis.opendocument.spreadsheet"
 
 
 class HTML(TextFormat):
```

### Comparing `django-import-export-4.0.0rc1/import_export/forms.py` & `django-import-export-4.0.0rc2/import_export/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         required=False,
     )
     format = forms.ChoiceField(
         label=_("Format"),
         choices=(),
     )
 
-    def __init__(self, formats, resources, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, formats, resources, **kwargs):
+        super().__init__(**kwargs)
         self._init_resources(resources)
         self._init_formats(formats)
 
     def _init_resources(self, resources):
         if not resources:
             raise ValueError("no defined resources")
         if len(resources) == 1:
@@ -58,16 +58,16 @@
     import_file = forms.FileField(label=_("File to import"))
 
     # field ordered for usability:
     # ensure that the 'file' select appears before 'format'
     # so that the 'guess_format' js logic makes sense
     field_order = ["resource", "import_file", "format"]
 
-    def __init__(self, formats, resources, *args, **kwargs):
-        super().__init__(formats, resources, *args, **kwargs)
+    def __init__(self, formats, resources, **kwargs):
+        super().__init__(formats, resources, **kwargs)
         if len(formats) > 1:
             self.fields["import_file"].widget.attrs["class"] = "guess_format"
             self.fields["format"].widget.attrs["class"] = "guess_format"
 
     @property
     def media(self):
         extra = "" if settings.DEBUG else ".min"
@@ -95,16 +95,16 @@
 class ExportForm(ImportExportFormBase):
     export_items = forms.MultipleChoiceField(
         widget=forms.MultipleHiddenInput(), required=False
     )
 
 
 class SelectableFieldsExportForm(ExportForm):
-    def __init__(self, formats, resources, *args, **kwargs):
-        super().__init__(formats, resources, *args, **kwargs)
+    def __init__(self, formats, resources, **kwargs):
+        super().__init__(formats, resources, **kwargs)
         self._init_selectable_fields(resources)
 
     @property
     def media(self):
         media = super().media
         return media + forms.Media(
             js=("import_export/export_selectable_fields.js",),
```

### Comparing `django-import-export-4.0.0rc1/import_export/instance_loaders.py` & `django-import-export-4.0.0rc2/import_export/instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/ar/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/ar/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/bg/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/bg/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/ca/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/ca/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/cs/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/cs/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/de/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/de/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/es/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/es/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/es_AR/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/es_AR/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/fa/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/fa/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/fi/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/fi/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/fr/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/fr/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/it/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/it/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/ja/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/ja/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/ko/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/ko/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/kz/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/kz/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/kz/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/kz/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/nl/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/nl/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/pl/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/pl/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/pt_BR/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/pt_BR/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/ru/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/ru/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/sk/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/sk/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/tr/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/tr/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-import-export-4.0.0rc2/import_export/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/locale/zh_Hans/LC_MESSAGES/django.po` & `django-import-export-4.0.0rc2/import_export/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/mixins.py` & `django-import-export-4.0.0rc2/import_export/mixins.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 class BaseImportExportMixin:
     """
     Base mixin for functionality related to importing and exporting via the Admin
     interface.
     """
 
-    resource_class = None
     resource_classes = []
 
     @property
     def formats(self):
         return getattr(settings, "IMPORT_EXPORT_FORMATS", base_formats.DEFAULT_FORMATS)
 
     @property
@@ -38,27 +37,30 @@
     def check_resource_classes(self, resource_classes):
         if resource_classes and not hasattr(resource_classes, "__getitem__"):
             raise Exception(
                 "The resource_classes field type must be "
                 "subscriptable (list, tuple, ...)"
             )
 
-    def get_resource_classes(self):
-        """Return subscriptable type (list, tuple, ...) containing resource classes"""
+    def get_resource_classes(self, request):
+        """
+        Return subscriptable type (list, tuple, ...) containing resource classes
+        :param request: The request object.
+        :returns: The Resource classes.
+        """
         if not self.resource_classes:
             return [modelresource_factory(self.model)]
         return self.resource_classes
 
-    def get_resource_kwargs(self, request, *args, **kwargs):
+    def get_resource_kwargs(self, request, **kwargs):
         """
         Return the kwargs which are to be passed to the Resource constructor.
         Can be overridden to provide additional kwarg params.
 
         :param request: The request object.
-        :param args: Positional arguments.
         :param kwargs: Keyword arguments.
         :returns: The Resource kwargs (by default, is the kwargs passed).
         """
         return kwargs
 
     def get_resource_index(self, form):
         """
@@ -73,71 +75,98 @@
                 resource_index = int(form.cleaned_data["resource"])
             except ValueError:
                 pass
         return resource_index
 
 
 class BaseImportMixin(BaseImportExportMixin):
-    def get_import_resource_classes(self):
+    def get_import_resource_classes(self, request):
         """
+        :param request: The request object.
         Returns ResourceClass subscriptable (list, tuple, ...) to use for import.
         """
-        resource_classes = self.get_resource_classes()
+        resource_classes = self.get_resource_classes(request)
         self.check_resource_classes(resource_classes)
         return resource_classes
 
     def get_import_formats(self):
         """
         Returns available import formats.
         """
         return [f for f in self.import_formats if f().can_import()]
 
     def get_import_resource_kwargs(self, request, **kwargs):
+        """
+        Returns kwargs which will be passed to the Resource constructor.
+        :param request: The request object.
+        :param kwargs: Keyword arguments.
+        :returns: The kwargs (dict)
+        """
         return self.get_resource_kwargs(request, **kwargs)
 
-    def choose_import_resource_class(self, form):
+    def choose_import_resource_class(self, form, request):
+        """
+        Identify which class should be used for import
+        :param form: The form object.
+        :param request: The request object.
+        :returns: The export Resource class.
+        """
         resource_index = self.get_resource_index(form)
-        return self.get_import_resource_classes()[resource_index]
+        return self.get_import_resource_classes(request)[resource_index]
 
 
 class BaseExportMixin(BaseImportExportMixin):
     model = None
 
     def get_export_formats(self):
         """
         Returns available export formats.
         """
         return [f for f in self.export_formats if f().can_export()]
 
-    def get_export_resource_classes(self):
+    def get_export_resource_classes(self, request):
         """
         Returns ResourceClass subscriptable (list, tuple, ...) to use for export.
+        :param request: The request object.
+        :returns: The Resource classes.
         """
-        resource_classes = self.get_resource_classes()
+        resource_classes = self.get_resource_classes(request)
         self.check_resource_classes(resource_classes)
         return resource_classes
 
-    def choose_export_resource_class(self, form):
+    def choose_export_resource_class(self, form, request):
+        """
+        Identify which class should be used for export
+        :param request: The request object.
+        :param form: The form object.
+        :returns: The export Resource class.
+        """
         resource_index = self.get_resource_index(form)
-        return self.get_export_resource_classes()[resource_index]
+        return self.get_export_resource_classes(request)[resource_index]
 
     def get_export_resource_kwargs(self, request, **kwargs):
+        """
+        Returns kwargs which will be passed to the Resource constructor.
+        :param request: The request object.
+        :param kwargs: Keyword arguments.
+        :returns: The kwargs (dict)
+        """
         return self.get_resource_kwargs(request, **kwargs)
 
     def get_export_resource_fields_from_form(self, form):
         if isinstance(form, SelectableFieldsExportForm):
             export_fields = form.get_selected_resource_export_fields()
             if export_fields:
                 return export_fields
 
         return
 
     def get_data_for_export(self, request, queryset, **kwargs):
         export_form = kwargs.get("export_form")
-        export_class = self.choose_export_resource_class(export_form)
+        export_class = self.choose_export_resource_class(export_form, request)
         export_resource_kwargs = self.get_export_resource_kwargs(request, **kwargs)
         export_fields = self.get_export_resource_fields_from_form(export_form)
         cls = export_class(**export_resource_kwargs)
         export_data = cls.export(
             queryset=queryset, export_fields=export_fields, **kwargs
         )
         return export_data
@@ -151,30 +180,30 @@
         )
         return filename
 
 
 class ExportViewMixin(BaseExportMixin):
     form_class = SelectableFieldsExportForm
 
-    def get_export_data(self, file_format, queryset, *args, **kwargs):
+    def get_export_data(self, file_format, queryset, **kwargs):
         """
         Returns file_format representation for given queryset.
         """
-        data = self.get_data_for_export(self.request, queryset, *args, **kwargs)
+        data = self.get_data_for_export(self.request, queryset, **kwargs)
         export_data = file_format.export_data(data)
         return export_data
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         return context
 
     def get_form_kwargs(self):
         kwargs = super().get_form_kwargs()
         kwargs["formats"] = self.get_export_formats()
-        kwargs["resources"] = self.get_export_resource_classes()
+        kwargs["resources"] = self.get_export_resource_classes(self.request)
         return kwargs
 
 
 class ExportViewFormMixin(ExportViewMixin, FormView):
     def form_valid(self, form):
         warn(
             "ExportViewFormMixin is deprecated and will be removed "
```

### Comparing `django-import-export-4.0.0rc1/import_export/options.py` & `django-import-export-4.0.0rc2/import_export/options.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/resources.py` & `django-import-export-4.0.0rc2/import_export/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -575,15 +575,15 @@
                     return False
         return True
 
     def get_diff_headers(self):
         """
         Diff representation headers.
         """
-        return self.get_user_visible_headers()
+        return [force_str(field.column_name) for field in self.get_import_fields()]
 
     def before_import(self, dataset, **kwargs):
         r"""
         Override to add additional logic. Does nothing by default.
 
         :param dataset: A ``tablib.Dataset``.
 
@@ -1047,20 +1047,14 @@
         headers = [force_str(field.column_name) for field in self.get_export_fields()]
 
         if isinstance(fields, list) and fields:
             return [f for f in headers if f in fields]
 
         return headers
 
-    def get_user_visible_headers(self):
-        headers = [
-            force_str(field.column_name) for field in self.get_user_visible_fields()
-        ]
-        return headers
-
     def get_user_visible_fields(self):
         return self.get_fields()
 
     def iter_queryset(self, queryset):
         if not isinstance(queryset, QuerySet):
             yield from queryset
         elif queryset._prefetch_related_lookups:
```

### Comparing `django-import-export-4.0.0rc1/import_export/results.py` & `django-import-export-4.0.0rc2/import_export/results.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/static/import_export/export_selectable_fields.js` & `django-import-export-4.0.0rc2/import_export/static/import_export/export_selectable_fields.js`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/static/import_export/guess_format.js` & `django-import-export-4.0.0rc2/import_export/static/import_export/guess_format.js`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/static/import_export/import.css` & `django-import-export-4.0.0rc2/import_export/static/import_export/import.css`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/templates/admin/import_export/base.html` & `django-import-export-4.0.0rc2/import_export/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/templates/admin/import_export/export.html` & `django-import-export-4.0.0rc2/import_export/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/templates/admin/import_export/import.html` & `django-import-export-4.0.0rc2/import_export/templates/admin/import_export/import.html`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     {% endblock %}
   {% else %}
     {% block import_form %}
     <form action="" method="post" enctype="multipart/form-data">
       {% csrf_token %}
 
       {% include "admin/import_export/resource_fields_list.html" with import_or_export="import" %}
+      {% block import_form_additional_info %}{% endblock %}
 
       {% block form_detail %}
           <fieldset class="module aligned">
           {% for field in form %}
             <div class="form-row">
               {{ field.errors }}
```

#### html2text {}

```diff
@@ -8,16 +8,16 @@
 confirm_import_form %}
 }" method="POST"> {% csrf_token %} {{ confirm_form.as_p }}
 {% translate "Below is a preview of data to be imported. If you are satisfied
 with the results, click 'Confirm import'" %}
 }">
 {% endblock %} {% else %} {% block import_form %}
 {% csrf_token %} {% include "admin/import_export/resource_fields_list.html"
-with import_or_export="import" %} {% block form_detail %} {% for field in form
-%}
+with import_or_export="import" %} {% block import_form_additional_info %}{%
+endblock %} {% block form_detail %} {% for field in form %}
 {{ field.errors }} {{ field.label_tag }} {% if
 field.field.widget.attrs.readonly %} {{ field.field.value }} {{ field.as_hidden
 }} {% else %} {{ field }} {% endif %} {% if field.field.help_text %}
 {{ field.field.help_text|safe }}
 {% endif %}
 {% endfor %} {% endblock %} {% block form_submit_button %}
 }">
```

### Comparing `django-import-export-4.0.0rc1/import_export/templates/admin/import_export/resource_fields_list.html` & `django-import-export-4.0.0rc2/import_export/templates/admin/import_export/resource_fields_list.html`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/tmp_storages.py` & `django-import-export-4.0.0rc2/import_export/tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/utils.py` & `django-import-export-4.0.0rc2/import_export/utils.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/import_export/widgets.py` & `django-import-export-4.0.0rc2/import_export/widgets.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/pyproject.toml` & `django-import-export-4.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/runtests.py` & `django-import-export-4.0.0rc2/runtests.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/runtests.sh` & `django-import-export-4.0.0rc2/runtests.sh`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/admin.py` & `django-import-export-4.0.0rc2/tests/core/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,24 @@
 
 
 class EBookResource(ModelResource):
     def __init__(self, **kwargs):
         super().__init__()
         self.author_id = kwargs.get("author_id")
 
-    def filter_export(self, queryset, *args, **kwargs):
+    def filter_export(self, queryset, **kwargs):
         return queryset.filter(author_id=self.author_id)
 
     class Meta:
         model = EBook
+        fields = (
+            "id",
+            "author_email",
+            "name",
+        )
 
 
 class CustomBookAdmin(ImportExportModelAdmin):
     """Example usage of custom import / export forms"""
 
     resource_classes = [EBookResource]
     import_form_class = CustomImportForm
```

### Comparing `django-import-export-4.0.0rc1/tests/core/exports/books-empty-author-email.xlsx` & `django-import-export-4.0.0rc2/tests/core/exports/books-empty-author-email.xlsx`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/exports/books.json` & `django-import-export-4.0.0rc2/tests/core/exports/books.json`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/exports/books.xls` & `django-import-export-4.0.0rc2/tests/core/exports/books.xls`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/exports/books.xlsx` & `django-import-export-4.0.0rc2/tests/core/exports/books.xlsx`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/fixtures/book.json` & `django-import-export-4.0.0rc2/tests/core/fixtures/book.json`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/forms.py` & `django-import-export-4.0.0rc2/tests/core/forms.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/migrations/0001_initial.py` & `django-import-export-4.0.0rc2/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/migrations/0003_withfloatfield.py` & `django-import-export-4.0.0rc2/tests/core/migrations/0003_withfloatfield.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/migrations/0004_bookwithchapters.py` & `django-import-export-4.0.0rc2/tests/core/migrations/0004_bookwithchapters.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/migrations/0005_addparentchild.py` & `django-import-export-4.0.0rc2/tests/core/migrations/0005_addparentchild.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/migrations/0007_auto_20180628_0411.py` & `django-import-export-4.0.0rc2/tests/core/migrations/0007_auto_20180628_0411.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/migrations/0008_auto_20190409_0846.py` & `django-import-export-4.0.0rc2/tests/core/migrations/0008_auto_20190409_0846.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/migrations/0009_auto_20211111_0807.py` & `django-import-export-4.0.0rc2/tests/core/migrations/0009_auto_20211111_0807.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/migrations/0010_uuidbook.py` & `django-import-export-4.0.0rc2/tests/core/migrations/0010_uuidbook.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py` & `django-import-export-4.0.0rc2/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/migrations/0014_bookwithchapternumbers.py` & `django-import-export-4.0.0rc2/tests/core/migrations/0014_bookwithchapternumbers.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/models.py` & `django-import-export-4.0.0rc2/tests/core/models.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/admin_integration/mixins.py` & `django-import-export-4.0.0rc2/tests/core/tests/admin_integration/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from import_export.formats.base_formats import DEFAULT_FORMATS
 
 
 class AdminTestMixin(object):
     category_change_url = "/admin/core/category/"
     book_import_url = "/admin/core/book/import/"
+    ebook_import_url = "/admin/core/ebook/import/"
     book_process_import_url = "/admin/core/book/process_import/"
     legacybook_import_url = "/admin/core/legacybook/import/"
     legacybook_process_import_url = "/admin/core/legacybook/process_import/"
     child_import_url = "/admin/core/child/import/"
     child_process_import_url = "/admin/core/child/process_import/"
 
     def setUp(self):
@@ -20,29 +21,40 @@
         self.user = User.objects.create_user("admin", "admin@example.com", "password")
         self.user.is_staff = True
         self.user.is_superuser = True
         self.user.save()
         self.client.login(username="admin", password="password")
 
     def _do_import_post(
-        self, url, filename, input_format=0, encoding=None, resource=None, follow=False
+        self,
+        url,
+        filename,
+        input_format=0,
+        encoding=None,
+        resource=None,
+        follow=False,
+        data=None,
     ):
         input_format = input_format
         filename = os.path.join(
             os.path.dirname(__file__),
             os.path.pardir,
             os.path.pardir,
             "exports",
             filename,
         )
         with open(filename, "rb") as f:
-            data = {
-                "format": str(input_format),
-                "import_file": f,
-            }
+            if data is None:
+                data = dict()
+            data.update(
+                {
+                    "format": str(input_format),
+                    "import_file": f,
+                }
+            )
             if encoding:
                 BookAdmin.from_encoding = encoding
             if resource:
                 data.update({"resource": resource})
             response = self.client.post(url, data, follow=follow)
         return response
```

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_action.py` & `django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             model = Book
 
             def has_export_permission(self, request):
                 return False
 
         m = TestMixin()
         with self.assertRaises(PermissionDenied):
-            m.get_export_data("0", Book.objects.none(), request=request)
+            m.get_export_data("0", request, Book.objects.none())
 
 
 class TestExportButtonOnChangeForm(AdminTestMixin, TestCase):
     def setUp(self):
         super().setUp()
         self.cat1 = Category.objects.create(name="Cat 1")
         self.change_url = reverse(
```

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_export.py` & `django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     ):
         # issue 1738
         mock_get_export_resource_kwargs.return_value = {"a": 1}
         response = self.client.get("/admin/core/book/export/")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(2, mock_get_export_resource_kwargs.call_count)
 
-    def book_resource_init(self):
+    def book_resource_init(self, **kwargs):
         # stub call to the resource constructor
         pass
 
     @mock.patch.object(BookResource, "__init__", book_resource_init)
     def test_export_passes_no_resource_constructor_params(self):
         # issue 1716
         # assert that the export call with a no-arg constructor
@@ -323,33 +323,31 @@
         self.assertTrue(response.has_header("Content-Disposition"))
         self.assertEqual(response["Content-Type"], "text/csv")
         self.assertEqual(
             response["Content-Disposition"],
             'attachment; filename="EBook-{}.csv"'.format(date_str),
         )
         self.assertEqual(
-            b"id,name,author,author_email,imported,published,"
-            b"published_time,price,added,categories\r\n"
-            b"5,The Man with the Golden Gun,5,ian@example.com,"
-            b"0,1965-04-01,21:00:00,5.00,,2\r\n",
+            b"id,author_email,name\r\n"
+            b"5,ian@example.com,The Man with the Golden Gun\r\n",
             response.content,
         )
 
 
 class TestExportEncoding(TestCase):
     mock_request = MagicMock(spec=HttpRequest)
     mock_request.POST = {"format": 0, "bookresource_id": True}
 
     class TestMixin(ExportMixin):
         model = Book
 
         def __init__(self, test_str=None):
             self.test_str = test_str
 
-        def get_data_for_export(self, request, queryset, *args, **kwargs):
+        def get_data_for_export(self, request, queryset, **kwargs):
             dataset = Dataset(headers=["id", "name"])
             dataset.append([1, self.test_str])
             return dataset
 
         def get_export_queryset(self, request):
             return list()
 
@@ -359,43 +357,45 @@
     def setUp(self):
         self.file_format = formats.base_formats.CSV()
         self.export_mixin = self.TestMixin(test_str="teststr")
 
     def test_to_encoding_not_set_default_encoding_is_utf8(self):
         self.export_mixin = self.TestMixin(test_str="teststr")
         data = self.export_mixin.get_export_data(
-            self.file_format, list(), request=self.mock_request
+            self.file_format, self.mock_request, list()
         )
         csv_dataset = tablib.import_set(data)
         self.assertEqual("teststr", csv_dataset.dict[0]["name"])
 
     def test_to_encoding_set(self):
         self.export_mixin = self.TestMixin(test_str="ハローワールド")
         data = self.export_mixin.get_export_data(
-            self.file_format, list(), request=self.mock_request, encoding="shift-jis"
+            self.file_format, self.mock_request, list(), encoding="shift-jis"
         )
         encoding = chardet.detect(bytes(data))["encoding"]
         self.assertEqual("SHIFT_JIS", encoding)
 
     def test_to_encoding_set_incorrect(self):
         self.export_mixin = self.TestMixin()
         with self.assertRaises(LookupError):
             self.export_mixin.get_export_data(
                 self.file_format,
+                self.mock_request,
                 list(),
-                request=self.mock_request,
                 encoding="bad-encoding",
             )
 
     @ignore_utcnow_deprecation_warning
     def test_to_encoding_not_set_for_binary_file(self):
         self.export_mixin = self.TestMixin(test_str="teststr")
         self.file_format = formats.base_formats.XLSX()
         data = self.export_mixin.get_export_data(
-            self.file_format, list(), request=self.mock_request
+            self.file_format,
+            self.mock_request,
+            list(),
         )
         binary_dataset = tablib.import_set(data)
         self.assertEqual("teststr", binary_dataset.dict[0]["name"])
 
     def test_export_action_to_encoding(self):
         self.export_mixin.to_encoding = "utf-8"
         with mock.patch(
```

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_import.py` & `django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 import warnings
 from io import StringIO
 from unittest import mock
-from unittest.mock import MagicMock, patch
+from unittest.mock import patch
 
 import django
 from core.admin import AuthorAdmin, BookAdmin, CustomBookAdmin, ImportMixin
 from core.models import Author, Book, EBook, Parent
 from core.tests.admin_integration.mixins import AdminTestMixin
 from core.tests.utils import ignore_widget_deprecation_warning
 from django.contrib.admin.models import DELETION, LogEntry
 from django.contrib.admin.sites import AdminSite
 from django.contrib.auth.models import User
-from django.http import HttpRequest
 from django.test import RequestFactory
 from django.test.testcases import TestCase, TransactionTestCase
 from django.test.utils import override_settings
 from django.utils.translation import gettext_lazy as _
 
 from import_export.admin import ExportMixin
 from import_export.exceptions import FieldError
@@ -237,14 +236,44 @@
                         response.context["form"], "import_file", target_msg
                     )
                 except TypeError:
                     self.assertFormError(response, "form", "import_file", target_msg)
         else:
             self.assertFormError(response, "form", "import_file", target_msg)
 
+    def test_import_action_invalidates_data_sheet_with_no_headers_or_data(self):
+        # GET the import form
+        response = self.client.get(self.book_import_url)
+        self.assertEqual(response.status_code, 200)
+        self.assertTemplateUsed(response, "admin/import_export/import.html")
+        self.assertContains(response, 'form action=""')
+
+        response = self._do_import_post(
+            self.book_import_url, "books-no-headers.csv", input_format=0
+        )
+        self.assertEqual(response.status_code, 200)
+        target_msg = (
+            "No valid data to import. Ensure your file "
+            "has the correct headers or data for import."
+        )
+
+        # required for testing via tox
+        # remove after django 5.0 released
+        if django.VERSION >= (4, 0):
+            with warnings.catch_warnings():
+                warnings.filterwarnings("ignore", category=DeprecationWarning)
+                try:
+                    self.assertFormError(
+                        response.context["form"], "import_file", target_msg
+                    )
+                except TypeError:
+                    self.assertFormError(response, "form", "import_file", target_msg)
+        else:
+            self.assertFormError(response, "form", "import_file", target_msg)
+
     @ignore_widget_deprecation_warning
     def test_delete_from_admin(self):
         # test delete from admin site (see #432)
 
         # create a book which can be deleted
         b = Book.objects.create(id=1)
 
@@ -446,35 +475,33 @@
         m.tmp_storage_class = "tmpClass"
         with mock.patch("import_export.admin.import_string") as mock_import_string:
             mock_import_string.return_value = target
             self.assertEqual(target, m.get_tmp_storage_class())
 
     def test_get_import_data_kwargs_with_form_kwarg(self):
         """
-        Test that if a the method is called with a 'form' kwarg,
+        Test that if the method is called with a 'form' kwarg,
         then it is removed and the updated dict is returned
         """
-        request = MagicMock(spec=HttpRequest)
         m = ImportMixin()
         kw = {"a": 1, "form": "some_form"}
         target = {"a": 1}
-        self.assertEqual(target, m.get_import_data_kwargs(request, **kw))
+        self.assertEqual(target, m.get_import_data_kwargs(**kw))
 
-    def test_get_import_data_kwargs_with_no_form_kwarg_returns_empty_dict(self):
+    def test_get_import_data_kwargs_with_no_form_kwarg_returns_kwarg_dict(self):
         """
         Test that if the method is called with no 'form' kwarg,
         then an empty dict is returned
         """
-        request = MagicMock(spec=HttpRequest)
         m = ImportMixin()
         kw = {
             "a": 1,
         }
-        target = {}
-        self.assertEqual(target, m.get_import_data_kwargs(request, **kw))
+        target = {"a": 1}
+        self.assertEqual(target, m.get_import_data_kwargs(**kw))
 
     def test_get_context_data_returns_empty_dict(self):
         m = ExportMixin()
         self.assertEqual(dict(), m.get_context_data())
 
     @patch("import_export.admin.logger")
     def test_issue_1521_change_list_template_as_property(self, mock_logger):
@@ -950,7 +977,40 @@
         self._is_str_in_response(
             "books.xls",
             "1",
             follow=True,
             str_in_response="Import finished: 1 new, 0 updated, "
             + "0 deleted and 0 skipped books.",
         )
+
+
+class ConfirmImportPreviewOrderTest(AdminTestMixin, TestCase):
+    """Test preview order displayed correctly (issue 1784)."""
+
+    fixtures = ["author"]
+
+    @ignore_widget_deprecation_warning
+    def test_import_preview_order(self):
+        author_id = Author.objects.first().id
+        response = self._do_import_post(
+            self.ebook_import_url,
+            "books.csv",
+            input_format="0",
+            data={"author": author_id},
+        )
+        # test header rendered in correct order
+        target_header_re = (
+            r"<thead>[\\n\s]+<tr>[\\n\s]+<th></th>[\\n\s]+<th>id</th>"
+            r"[\\n\s]+<th>author_email</th>[\\n\s]+<th>name</th>[\\n\s]+</tr>[\\n\s]+"
+            "</thead>"
+        )
+        self.assertRegex(str(response.content), target_header_re)
+        # test row rendered in correct order
+        target_row_re = (
+            r'<tr class="new">[\\n\s]+'
+            r'<td class="import-type">[\\n\s]+New[\\n\s]+</td>[\\n\s]+'
+            r'<td><ins style="background:#e6ffe6;">1</ins></td>[\\n\s]+'
+            r'<td><ins style="background:#e6ffe6;">test@example.com</ins></td>[\\n\s]+'
+            r'<td><ins style="background:#e6ffe6;">Some book</ins></td>[\\n\s]+'
+            "</tr>"
+        )
+        self.assertRegex(str(response.content), target_row_re)
```

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/admin_integration/test_views.py` & `django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_views.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/resources.py` & `django-import-export-4.0.0rc2/tests/core/tests/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 class BookResourceWithStoreInstance(resources.ModelResource):
     class Meta:
         model = Book
         store_instance = True
 
 
 class BookResourceWithLineNumberLogger(BookResource):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, **kwargs):
         self.before_lines = []
         self.after_lines = []
-        return super().__init__(*args, **kwargs)
+        return super().__init__(**kwargs)
 
     def before_import_row(self, row, **kwargs):
         row_number = kwargs.pop("row_number")
         self.before_lines.append(row_number)
 
     def after_import_row(self, row, row_result, **kwargs):
         row_number = kwargs.pop("row_number")
```

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_base_formats.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_base_formats.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_declarative.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_declarative.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_fields.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_forms.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_instance_loaders.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_invalidrow.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_invalidrow.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_mixins.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,42 +146,42 @@
     """
 
     request = MagicMock(spec=HttpRequest)
 
     class BaseImportModelAdminTest(mixins.BaseImportMixin):
         call_count = 0
 
-        def get_resource_classes(self):
+        def get_resource_classes(self, request, **kwargs):
             self.call_count += 1
 
-        def get_resource_kwargs(self, request, *args, **kwargs):
+        def get_resource_kwargs(self, request, **kwargs):
             self.call_count += 1
 
     class BaseExportModelAdminTest(mixins.BaseExportMixin):
         call_count = 0
 
-        def get_resource_classes(self):
+        def get_resource_classes(self, request, **kwargs):
             self.call_count += 1
 
-        def get_resource_kwargs(self, request, *args, **kwargs):
+        def get_export_resource_kwargs(self, request, **kwargs):
             self.call_count += 1
 
     def test_get_import_resource_class_calls_self_get_resource_class(self):
         admin = self.BaseImportModelAdminTest()
-        admin.get_import_resource_classes()
+        admin.get_import_resource_classes(self.request)
         self.assertEqual(1, admin.call_count)
 
     def test_get_import_resource_kwargs_calls_self_get_resource_kwargs(self):
         admin = self.BaseImportModelAdminTest()
         admin.get_import_resource_kwargs(self.request)
         self.assertEqual(1, admin.call_count)
 
     def test_get_export_resource_class_calls_self_get_resource_class(self):
         admin = self.BaseExportModelAdminTest()
-        admin.get_export_resource_classes()
+        admin.get_export_resource_classes(self.request)
         self.assertEqual(1, admin.call_count)
 
     def test_get_export_resource_kwargs_calls_self_get_resource_kwargs(self):
         admin = self.BaseExportModelAdminTest()
         admin.get_export_resource_kwargs(self.request)
         self.assertEqual(1, admin.call_count)
 
@@ -190,45 +190,53 @@
 
     def test_faulty_resource_class_raises_exception(self):
         """Test fallback mechanism to old get_export_resource_class() method"""
         admin = self.BaseModelAdminFaultyResourceClassesTest()
         with self.assertRaisesRegex(
             Exception, r"^The resource_classes field type must be subscriptable"
         ):
-            admin.get_export_resource_classes()
+            admin.get_export_resource_classes(self.request)
 
     class BaseModelAdminBothResourceTest(mixins.BaseExportMixin):
         call_count = 0
 
         resource_class = resources.Resource
         resource_classes = [resources.Resource]
 
     class BaseModelExportChooseTest(mixins.BaseExportMixin):
         resource_classes = [resources.Resource, FooResource]
 
     @mock.patch("import_export.admin.SelectableFieldsExportForm")
     def test_choose_export_resource_class(self, form):
         """Test choose_export_resource_class() method"""
         admin = self.BaseModelExportChooseTest()
-        self.assertEqual(admin.choose_export_resource_class(form), resources.Resource)
+        self.assertEqual(
+            admin.choose_export_resource_class(form, self.request), resources.Resource
+        )
 
         form.cleaned_data = {"resource": 1}
-        self.assertEqual(admin.choose_export_resource_class(form), FooResource)
+        self.assertEqual(
+            admin.choose_export_resource_class(form, self.request), FooResource
+        )
 
     class BaseModelImportChooseTest(mixins.BaseImportMixin):
         resource_classes = [resources.Resource, FooResource]
 
     @mock.patch("import_export.admin.ImportForm")
     def test_choose_import_resource_class(self, form):
         """Test choose_import_resource_class() method"""
         admin = self.BaseModelImportChooseTest()
-        self.assertEqual(admin.choose_import_resource_class(form), resources.Resource)
+        request = MagicMock(spec=HttpRequest)
+        self.assertEqual(
+            admin.choose_import_resource_class(form, request),
+            resources.Resource,
+        )
 
         form.cleaned_data = {"resource": 1}
-        self.assertEqual(admin.choose_import_resource_class(form), FooResource)
+        self.assertEqual(admin.choose_import_resource_class(form, request), FooResource)
 
 
 class BaseExportMixinTest(TestCase):
     class TestBaseExportMixin(mixins.BaseExportMixin):
         def get_export_resource_kwargs(self, request, **kwargs):
             self.kwargs = kwargs
             return super().get_resource_kwargs(request, **kwargs)
@@ -297,11 +305,11 @@
 class BaseExportImportMixinTest(TestCase):
     class TestMixin(mixins.BaseImportExportMixin):
         pass
 
     def test_get_resource_kwargs(self):
         mixin_instance = self.TestMixin()
         test_kwargs = {"key1": "value1", "key2": "value2"}
-
-        result = mixin_instance.get_resource_kwargs(HttpRequest, **test_kwargs)
+        mock_request = MagicMock(spec=HttpRequest)
+        result = mixin_instance.get_resource_kwargs(mock_request, **test_kwargs)
 
         self.assertEqual(result, test_kwargs)
```

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_permissions.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_bulk_operations.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_bulk_operations.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_diffs.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_diffs.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
         resource = BookResource()
 
         with mock.patch(
             "import_export.resources.Resource.get_import_fields"
         ) as mock_get_import_fields:
             resource.import_data(self.dataset, dry_run=True)
-            self.assertEqual(2, mock_get_import_fields.call_count)
+            self.assertEqual(3, mock_get_import_fields.call_count)
 
 
 class SkipHtmlDiffTest(TestCase):
     def test_skip_html_diff(self):
         class BookResource(resources.ModelResource):
             class Meta:
                 model = Book
```

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_import_export.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_import_export.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_misc.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_misc.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_handling.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_handling.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_data_import.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_import.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_error_handling.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_export.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_export.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_fields.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_m2m.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_m2m.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_queryset.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_queryset.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_relationship.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_relationship.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_resources/test_relationships.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_relationships.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_results.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_tmp_storages.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/test_widgets.py` & `django-import-export-4.0.0rc2/tests/core/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/core/tests/utils.py` & `django-import-export-4.0.0rc2/tests/core/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/docker-compose.yml` & `django-import-export-4.0.0rc2/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/scripts/bulk_import.py` & `django-import-export-4.0.0rc2/tests/scripts/bulk_import.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tests/settings.py` & `django-import-export-4.0.0rc2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc1/tox.ini` & `django-import-export-4.0.0rc2/tox.ini`

 * *Files identical despite different names*

