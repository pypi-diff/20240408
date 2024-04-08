# Comparing `tmp/wagtail_fedit-1.4.1.tar.gz` & `tmp/wagtail_fedit-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.4.1.tar", last modified: Sun Apr  7 05:30:26 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.4.2.tar", last modified: Mon Apr  8 20:13:52 2024, max compression
```

## Comparing `wagtail_fedit-1.4.1.tar` & `wagtail_fedit-1.4.2.tar`

### file list

```diff
@@ -1,110 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.521357 wagtail_fedit-1.4.1/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.1/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0    12872 2024-04-07 05:30:26.520687 wagtail_fedit-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0    11822 2024-04-06 22:25:03.000000 wagtail_fedit-1.4.1/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.1/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-07 05:30:26.533746 wagtail_fedit-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.428827 wagtail_fedit-1.4.1/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.1/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.1/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.1/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.456266 wagtail_fedit-1.4.1/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.1/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.4.1/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.1/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     3356 2024-04-06 21:44:51.000000 wagtail_fedit-1.4.1/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.456776 wagtail_fedit-1.4.1/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.1/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.457795 wagtail_fedit-1.4.1/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.1/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.1/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.412966 wagtail_fedit-1.4.1/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.412966 wagtail_fedit-1.4.1/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.459787 wagtail_fedit-1.4.1/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.460791 wagtail_fedit-1.4.1/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15915 2024-04-06 00:14:04.000000 wagtail_fedit-1.4.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.415061 wagtail_fedit-1.4.1/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.416060 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.463214 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.464276 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.478720 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      789 2024-04-07 05:29:57.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.480904 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.481903 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.485908 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
--rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
--rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
--rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
--rw-rw-rw-   0        0        0     1285 2024-04-06 18:43:26.000000 wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.487943 wagtail_fedit-1.4.1/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.1/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.489943 wagtail_fedit-1.4.1/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.1/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    18951 2024-04-06 22:02:41.000000 wagtail_fedit-1.4.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    15092 2024-04-07 05:12:36.000000 wagtail_fedit-1.4.1/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.490938 wagtail_fedit-1.4.1/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.493150 wagtail_fedit-1.4.1/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.496663 wagtail_fedit-1.4.1/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     3529 2024-04-05 23:35:47.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.503678 wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7039 2024-04-05 23:57:48.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     4339 2024-04-06 00:03:48.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.507981 wagtail_fedit-1.4.1/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.1/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.4.1/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      916 2024-04-06 20:43:13.000000 wagtail_fedit-1.4.1/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    11238 2024-04-06 18:35:33.000000 wagtail_fedit-1.4.1/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.512241 wagtail_fedit-1.4.1/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.4.1/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.4.1/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    14621 2024-04-05 23:51:10.000000 wagtail_fedit-1.4.1/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12225 2024-04-06 19:48:05.000000 wagtail_fedit-1.4.1/wagtail_fedit/views/fields.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.1/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.518566 wagtail_fedit-1.4.1/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      160 2024-04-06 18:20:48.000000 wagtail_fedit-1.4.1/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.1/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.1/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.4.1/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.1/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.1/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     6061 2024-04-06 18:49:36.000000 wagtail_fedit-1.4.1/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-07 05:30:26.519624 wagtail_fedit-1.4.1/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    12872 2024-04-07 05:30:26.000000 wagtail_fedit-1.4.1/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3542 2024-04-07 05:30:26.000000 wagtail_fedit-1.4.1/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 05:30:26.000000 wagtail_fedit-1.4.1/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-07 05:30:26.000000 wagtail_fedit-1.4.1/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-07 05:30:26.000000 wagtail_fedit-1.4.1/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.921758 wagtail_fedit-1.4.2/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    12947 2024-04-08 20:13:52.921758 wagtail_fedit-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11954 2024-04-08 20:13:14.000000 wagtail_fedit-1.4.2/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-08 20:13:52.934635 wagtail_fedit-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.779712 wagtail_fedit-1.4.2/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.2/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.2/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.2/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.826655 wagtail_fedit-1.4.2/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.2/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.4.2/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.2/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     3356 2024-04-06 21:44:51.000000 wagtail_fedit-1.4.2/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.828661 wagtail_fedit-1.4.2/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.2/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.829656 wagtail_fedit-1.4.2/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.2/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.739663 wagtail_fedit-1.4.2/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.739663 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.834176 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.835353 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15915 2024-04-06 00:14:04.000000 wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.742063 wagtail_fedit-1.4.2/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.743064 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.837357 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.838357 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.851882 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      789 2024-04-07 05:29:57.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.863572 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.865583 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.869072 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
+-rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+-rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+-rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
+-rw-rw-rw-   0        0        0     1285 2024-04-06 18:43:26.000000 wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.871069 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.873073 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    19080 2024-04-08 20:04:44.000000 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    15398 2024-04-08 20:08:45.000000 wagtail_fedit-1.4.2/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.875135 wagtail_fedit-1.4.2/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.879137 wagtail_fedit-1.4.2/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.885616 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3529 2024-04-05 23:35:47.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.894694 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7039 2024-04-05 23:57:48.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     4339 2024-04-06 00:03:48.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.903238 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.4.2/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      916 2024-04-06 20:43:13.000000 wagtail_fedit-1.4.2/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    11238 2024-04-06 18:35:33.000000 wagtail_fedit-1.4.2/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.909210 wagtail_fedit-1.4.2/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.4.2/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.4.2/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    14621 2024-04-05 23:51:10.000000 wagtail_fedit-1.4.2/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12225 2024-04-06 19:48:05.000000 wagtail_fedit-1.4.2/wagtail_fedit/views/fields.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.2/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.920766 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      160 2024-04-06 18:20:48.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     6061 2024-04-06 18:49:36.000000 wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:13:52.823300 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    12947 2024-04-08 20:13:52.000000 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3476 2024-04-08 20:13:52.000000 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 20:13:52.000000 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-08 20:13:52.000000 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-08 20:13:52.000000 wagtail_fedit-1.4.2/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.4.1/LICENSE` & `wagtail_fedit-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/PKG-INFO` & `wagtail_fedit-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.4.1
+Version: 1.4.2
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,20 +18,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=4.2
 
 wagtail_fedit
 =============
 
+![Wagtail FEdit Example](https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
+
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
 
 # Table of Contents
 
 - [Getting Started](#getting-started)
 - [Getting Editing!](#getting-editing)
 - [Permissions](#permissions)
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.1 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.2 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier:
 Topic :: Internet :: WWW/HTTP :: Dynamic Content Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-Django>=4.2 Requires-Dist: Wagtail>=4.2 wagtail_fedit ============= Wagtail
-FEdit is a library to allow your Wagtail pages and content-blocks to be edited
-on the frontend. # Table of Contents - [Getting Started](#getting-started) -
-[Getting Editing!](#getting-editing) - [Permissions](#permissions) -
+Description-Content-Type: text/markdown License-File: LICENSE wagtail_fedit
+============= ![Wagtail FEdit Example](https://github.com/Nigel2392/
+wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
+Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be
+edited on the frontend. # Table of Contents - [Getting Started](#getting-
+started) - [Getting Editing!](#getting-editing) - [Permissions](#permissions) -
 [Revisions](#revisions) - [Workflows](#workflows) - [Logs](#logs) - [Caveats]
 (#caveats) - [Hooks](#hooks) - [Construct Block Toolbar]
 (#wagtail_feditconstruct_block_toolbar) - [Construct Field Toolbar]
 (#wagtail_feditconstruct_field_toolbar) - [Register Type Renderer]
 (#wagtail_feditregister_type_renderer) - [Register Field Renderer]
 (#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
```

### Comparing `wagtail_fedit-1.4.1/README.md` & `wagtail_fedit-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 wagtail_fedit
 =============
 
+![Wagtail FEdit Example](https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
+
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
 
 # Table of Contents
 
 - [Getting Started](#getting-started)
 - [Getting Editing!](#getting-editing)
 - [Permissions](#permissions)
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
-wagtail_fedit ============= Wagtail FEdit is a library to allow your Wagtail
-pages and content-blocks to be edited on the frontend. # Table of Contents -
-[Getting Started](#getting-started) - [Getting Editing!](#getting-editing) -
-[Permissions](#permissions) - [Revisions](#revisions) - [Workflows](#workflows)
-- [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) - [Construct Block
-Toolbar](#wagtail_feditconstruct_block_toolbar) - [Construct Field Toolbar]
-(#wagtail_feditconstruct_field_toolbar) - [Register Type Renderer]
-(#wagtail_feditregister_type_renderer) - [Register Field Renderer]
+wagtail_fedit ============= ![Wagtail FEdit Example](https://github.com/
+Nigel2392/wagtail_fedit/blob/main/.github/images/
+wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
+Wagtail pages and content-blocks to be edited on the frontend. # Table of
+Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
+editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
+(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) -
+[Construct Block Toolbar](#wagtail_feditconstruct_block_toolbar) - [Construct
+Field Toolbar](#wagtail_feditconstruct_field_toolbar) - [Register Type
+Renderer](#wagtail_feditregister_type_renderer) - [Register Field Renderer]
 (#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [How your field/block is rendered]
 (#how-your-fieldblock-is-rendered) - [Rendered block output HTML](#rendered-
 block-output-html) - [Rendered field output HTML](#rendered-field-output-html)
 - [Implemented](#implemented) Getting Started --------------- 1. Add
 'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
```

### Comparing `wagtail_fedit-1.4.1/setup.cfg` & `wagtail_fedit-1.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 342e  ..version = 1.4.
-00000030: 310d 0a64 6573 6372 6970 7469 6f6e 203d  1..description =
+00000030: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.4.2/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.4.2/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/hooks.py` & `wagtail_fedit-1.4.2/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/models.py` & `wagtail_fedit-1.4.2/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.4.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.4.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.4.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x76c61166 (Sat Apr  6 22:02:30 2024 UTC)
-files sz: 15073
+moddate:  0xda4d1466 (Mon Apr  8 20:04:42 2024 UTC)
+files sz: 15230
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -168,102 +168,102 @@
                276 STORE_NAME              39 (WARNING_FIELD_NAME_NOT_AVAILABLE)
    
     33         278 LOAD_CONST              19 ('Model instance is not available in the context for %(object)s.')
                280 STORE_NAME              40 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
    
     36         282 PUSH_NULL
                284 LOAD_BUILD_CLASS
-               286 LOAD_CONST              20 (<code object BlockEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 36>)
+               286 LOAD_CONST              20 (<code object BlockEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 36>)
                288 MAKE_FUNCTION            0
                290 LOAD_CONST              21 ('BlockEditNode')
                292 LOAD_NAME                2 (Node)
                294 PRECALL                  3
                298 CALL                     3
                308 STORE_NAME              41 (BlockEditNode)
    
-   228         310 LOAD_NAME               36 (register)
+   231         310 LOAD_NAME               36 (register)
                312 LOAD_METHOD             42 (tag)
                334 LOAD_CONST              22 ('fedit_block')
                336 KW_NAMES                23
                338 PRECALL                  1
                342 CALL                     1
    
-   229         352 LOAD_CONST              24 ('parser')
+   232         352 LOAD_CONST              24 ('parser')
                354 LOAD_NAME                7 (Parser)
                356 LOAD_CONST              25 ('token')
                358 LOAD_NAME                8 (Token)
                360 BUILD_TUPLE              4
-               362 LOAD_CONST              26 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 228>)
+               362 LOAD_CONST              26 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 231>)
                364 MAKE_FUNCTION            4 (annotations)
    
-   228         366 PRECALL                  0
+   231         366 PRECALL                  0
                370 CALL                     0
    
-   229         380 STORE_NAME              43 (do_render_fedit_block)
+   232         380 STORE_NAME              43 (do_render_fedit_block)
    
-   288         382 PUSH_NULL
+   291         382 PUSH_NULL
                384 LOAD_BUILD_CLASS
-               386 LOAD_CONST              27 (<code object FieldEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 288>)
+               386 LOAD_CONST              27 (<code object FieldEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 291>)
                388 MAKE_FUNCTION            0
                390 LOAD_CONST              28 ('FieldEditNode')
                392 LOAD_NAME                2 (Node)
                394 PRECALL                  3
                398 CALL                     3
                408 STORE_NAME              44 (FieldEditNode)
    
-   338         410 LOAD_NAME               36 (register)
+   344         410 LOAD_NAME               36 (register)
                412 LOAD_METHOD             42 (tag)
                434 LOAD_CONST              29 ('fedit_field')
                436 KW_NAMES                23
                438 PRECALL                  1
                442 CALL                     1
    
-   339         452 LOAD_CONST              24 ('parser')
+   345         452 LOAD_CONST              24 ('parser')
                454 LOAD_NAME                7 (Parser)
                456 LOAD_CONST              25 ('token')
                458 LOAD_NAME                8 (Token)
                460 BUILD_TUPLE              4
-               462 LOAD_CONST              30 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 338>)
+               462 LOAD_CONST              30 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 344>)
                464 MAKE_FUNCTION            4 (annotations)
    
-   338         466 PRECALL                  0
+   344         466 PRECALL                  0
                470 CALL                     0
    
-   339         480 STORE_NAME              45 (do_render_fedit_field)
+   345         480 STORE_NAME              45 (do_render_fedit_field)
    
-   381         482 LOAD_CONST              31 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 381>)
+   387         482 LOAD_CONST              31 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 387>)
                484 MAKE_FUNCTION            0
                486 STORE_NAME              46 (render_editable_field)
    
-   420         488 LOAD_CONST              24 ('parser')
+   426         488 LOAD_CONST              24 ('parser')
                490 LOAD_NAME                7 (Parser)
                492 LOAD_CONST              32 ('kwarg_list')
                494 LOAD_NAME               47 (list)
                496 LOAD_NAME               48 (str)
                498 BINARY_SUBSCR
                508 LOAD_CONST              33 ('tokens')
                510 LOAD_NAME               47 (list)
                512 LOAD_NAME               48 (str)
                514 BINARY_SUBSCR
                524 LOAD_CONST              34 ('return')
                526 LOAD_NAME               49 (dict)
                528 BUILD_TUPLE              8
-               530 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 420>)
+               530 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 426>)
                532 MAKE_FUNCTION            4 (annotations)
                534 STORE_NAME              50 (get_kwargs)
    
-   445         536 LOAD_CONST              36 ('obj')
+   451         536 LOAD_CONST              36 ('obj')
                538 LOAD_NAME               17 (models)
                540 LOAD_ATTR               51 (Model)
                550 BUILD_TUPLE              2
-               552 LOAD_CONST              37 (<code object _can_edit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 445>)
+               552 LOAD_CONST              37 (<code object _can_edit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 451>)
                554 MAKE_FUNCTION            4 (annotations)
                556 STORE_NAME              52 (_can_edit)
    
-   457         558 LOAD_CONST              38 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 457>)
+   463         558 LOAD_CONST              38 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 463>)
                560 MAKE_FUNCTION            0
                562 STORE_NAME              53 (_get_from_context_or_set)
                564 LOAD_CONST              13 (None)
                566 RETURN_VALUE
    consts
       0
       ('library', 'Node', 'NodeList')
@@ -303,15 +303,15 @@
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BlockEditNode')
                        8 STORE_NAME               2 (__qualname__)
          
           37          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object UnpackError, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 37>)
+                      14 LOAD_CONST               1 (<code object UnpackError, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 37>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('UnpackError')
                       20 LOAD_NAME                3 (Exception)
                       22 PRECALL                  3
                       26 CALL                     3
                       36 STORE_NAME               4 (UnpackError)
          
@@ -344,72 +344,72 @@
          
           40          66 LOAD_CONST               8 ('model')
          
           45          68 LOAD_NAME                8 (models)
                       70 LOAD_ATTR                9 (Model)
          
           40          80 BUILD_TUPLE             10
-                      82 LOAD_CONST               9 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 40>)
+                      82 LOAD_CONST               9 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 40>)
                       84 MAKE_FUNCTION            5 (defaults, annotations)
                       86 STORE_NAME              10 (__init__)
          
-          56          88 LOAD_CONST              10 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 56>)
+          56          88 LOAD_CONST              10 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 56>)
                       90 MAKE_FUNCTION            0
                       92 STORE_NAME              11 (render)
          
-         179          94 LOAD_NAME               12 (staticmethod)
+         182          94 LOAD_NAME               12 (staticmethod)
          
-         180          96 LOAD_CONST              11 ('return')
+         183          96 LOAD_CONST              11 ('return')
                       98 LOAD_NAME               13 (dict)
                      100 BUILD_TUPLE              2
-                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 179>)
+                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 182>)
                      104 MAKE_FUNCTION            4 (annotations)
          
-         179         106 PRECALL                  0
+         182         106 PRECALL                  0
                      110 CALL                     0
          
-         180         120 STORE_NAME              14 (pack)
+         183         120 STORE_NAME              14 (pack)
          
-         188         122 LOAD_NAME               15 (classmethod)
+         191         122 LOAD_NAME               15 (classmethod)
          
-         189         124 LOAD_CONST               3 (None)
+         192         124 LOAD_CONST               3 (None)
                      126 LOAD_CONST              13 (('request',))
                      128 BUILD_CONST_KEY_MAP      1
                      130 LOAD_CONST              14 ('expected')
                      132 LOAD_NAME                7 (str)
                      134 LOAD_CONST              11 ('return')
                      136 LOAD_NAME               13 (dict)
                      138 BUILD_TUPLE              4
-                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 188>)
+                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 191>)
                      142 MAKE_FUNCTION            6 (kwdefaults, annotations)
          
-         188         144 PRECALL                  0
+         191         144 PRECALL                  0
                      148 CALL                     0
          
-         189         158 STORE_NAME              16 (unpack)
+         192         158 STORE_NAME              16 (unpack)
          
-         211         160 LOAD_NAME               12 (staticmethod)
+         214         160 LOAD_NAME               12 (staticmethod)
          
-         212         162 LOAD_CONST               6 ('block_id')
+         215         162 LOAD_CONST               6 ('block_id')
                      164 LOAD_NAME                7 (str)
                      166 LOAD_CONST               7 ('field_name')
                      168 LOAD_NAME                7 (str)
                      170 LOAD_CONST              16 ('instance')
                      172 LOAD_NAME                8 (models)
                      174 LOAD_ATTR                9 (Model)
                      184 LOAD_CONST              11 ('return')
                      186 LOAD_NAME                7 (str)
                      188 BUILD_TUPLE              8
-                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 211>)
+                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 214>)
                      192 MAKE_FUNCTION            4 (annotations)
          
-         211         194 PRECALL                  0
+         214         194 PRECALL                  0
                      198 CALL                     0
          
-         212         208 STORE_NAME              17 (get_edit_url)
+         215         208 STORE_NAME              17 (get_edit_url)
                      210 LOAD_CONST               3 (None)
                      212 RETURN_VALUE
          consts
             'BlockEditNode'
             code
                argcount  : 0
                nlocals   : 0
@@ -427,15 +427,15 @@
                consts
                   'BlockEditNode.UnpackError'
                   None
                names      ('__name__', '__module__', '__qualname__')
                varnames   ()
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'UnpackError'
                firstlineno 37
                lnotab 0x0a01
             'UnpackError'
             None
             'nodelist'
             'block'
@@ -481,15 +481,15 @@
                             88 RETURN_VALUE
                consts
                   None
                names      ('nl', 'block', 'block_id', 'field_name', 'model', 'extra')
                varnames   ('self', 'nodelist', 'block', 'block_id', 'field_name', 'model', 'extra')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
                firstlineno 40
                lnotab 0x02090e010e010e010e010e01
             code
                argcount  : 2
                nlocals   : 13
                stacksize : 14
@@ -514,51 +514,52 @@
                   007c01a6010000ab0100000000000000007d04740d000000000000000000
                   00890d740e00000000000000000000a6020000ab02000000000000000072
                   15890da00800000000000000000000000000000000000000007c01a60100
                   00ab0100000000000000008a0d7c03731564027c01760172117c02730f74
                   13000000000000000000006403a6010000ab010000000000000000820189
                   0d70147c01a00a00000000000000000000000000000000000000006404a6
                   010000ab0100000000000000008a0d7c047c0164013c000000890d7c0164
-                  043c0000007c02725809007c01a00b000000000000000000000000000000
-                  0000000000a6000000ab0000000000000000007d086e1023007418000000
-                  0000000000000024007203010059006e0477007803590077017c08a00d00
-                  000000000000000000000000000000000000007c05a6010000ab01000000
-                  000000000001007c02a00e00000000000000000000000000000000000000
-                  007c08a6010000ab0100000000000000007d0964057c005f0f0000000000
-                  0000006e387c006a10000000000000000072227c006a1000000000000000
-                  00a01100000000000000000000000000000000000000007c01a6010000ab
-                  0100000000000000007d0964067c005f0f00000000000000006e0f741300
-                  0000000000000000006407a6010000ab01000000000000000082017c0473
-                  257425000000000000000000006a13000000000000000074280000000000
-                  000000000064087c016a15000000000000000069017a060000a6010000ab
-                  01000000000000000001007c095300890d732f7425000000000000000000
-                  006a130000000000000000742c0000000000000000000064087c026a0000
-                  000000000000006a1700000000000000006a18000000000000000069017a
-                  060000a6010000ab01000000000000000001007c0953007c03730d64027c
-                  01760072097c016402190000000000000000007d036e2d7c03731a7c0272
-                  187433000000000000000000007c026409a6020000ab0200000000000000
-                  0072087c026a1a00000000000000007d036e117c03730f74130000000000
-                  00000000006403a6010000ab01000000000000000082017c01a00a000000
-                  0000000000000000000000000000000000640aa6010000ab010000000000
-                  0000008a0e743700000000000000000000890e890da6020000ab02000000
-                  000000000073027c095300740d00000000000000000000890d7438000000
-                  00000000000000a6020000ab020000000000000000721d743b0000000000
-                  00000000007c01640b880d6601640c8408a6030000ab0300000000000000
-                  007d0a7c0a9b00640d7c039b00640e9d047d0a6e0264007d0a7c006a0f00
-                  000000000000007c05640f3c000000743d00000000000000000000a60000
-                  00ab00000000000000000067017d0b743f000000000000000000006a2000
-                  00000000000000744200000000000000000000a6010000ab010000000000
-                  00000044005d127d0c02007c0c890e7c0b890d7c037c04ac10a6050000ab
-                  05000000000000000001008c13880e6601641184087c0b4400a6000000ab
-                  0000000000000000007d0b74450000000000000000000074470000000000
-                  000000000064007c0ba6020000ab020000000000000000a6010000ab0100
-                  000000000000007d0b744900000000000000000000641202007c006a2500
-                  000000000000007c037c0466026413890d69017c05a4018e017c0a7c0389
-                  0d7c097c047c017c04890d7c0b64149c0aa6020000ab0200000000000000
-                  005300
+                  043c0000007c02725a09007c01a00b000000000000000000000000000000
+                  0000000000a6000000ab0000000000000000007d086e1223007418000000
+                  000000000000002400720501007c017d0859006e0477007803590077017c
+                  08a00d00000000000000000000000000000000000000007c05a6010000ab
+                  01000000000000000001007c02a00e000000000000000000000000000000
+                  00000000007c08a6010000ab0100000000000000007d0964057c005f0f00
+                  000000000000006e387c006a10000000000000000072227c006a10000000
+                  0000000000a01100000000000000000000000000000000000000007c01a6
+                  010000ab0100000000000000007d0964067c005f0f00000000000000006e
+                  0f7413000000000000000000006407a6010000ab01000000000000000082
+                  017c0473257425000000000000000000006a130000000000000000742800
+                  00000000000000000064087c016a15000000000000000069017a060000a6
+                  010000ab01000000000000000001007c095300890d732f74250000000000
+                  00000000006a130000000000000000742c0000000000000000000064087c
+                  026a0000000000000000006a1700000000000000006a1800000000000000
+                  0069017a060000a6010000ab01000000000000000001007c0953007c0373
+                  0d64027c01760072097c016402190000000000000000007d036e2d7c0373
+                  1a7c0272187433000000000000000000007c026409a6020000ab02000000
+                  000000000072087c026a1a00000000000000007d036e117c03730f741300
+                  0000000000000000006403a6010000ab01000000000000000082017c0973
+                  0f743700000000000000000000640aa6010000ab0100000000000000007d
+                  097c01a00a0000000000000000000000000000000000000000640ba60100
+                  00ab0100000000000000008a0e743900000000000000000000890e890da6
+                  020000ab02000000000000000073027c095300740d000000000000000000
+                  00890d743a00000000000000000000a6020000ab02000000000000000072
+                  1d743d000000000000000000007c01640c880d6601640d8408a6030000ab
+                  0300000000000000007d0a7c0a9b00640e7c039b00640f9d047d0a6e0264
+                  007d0a7c006a0f00000000000000007c0564103c000000743f0000000000
+                  0000000000a6000000ab00000000000000000067017d0b74410000000000
+                  00000000006a210000000000000000744400000000000000000000a60100
+                  00ab01000000000000000044005d127d0c02007c0c890e7c0b890d7c037c
+                  04ac11a6050000ab05000000000000000001008c13880e6601641284087c
+                  0b4400a6000000ab0000000000000000007d0b7447000000000000000000
+                  0074490000000000000000000064007c0ba6020000ab0200000000000000
+                  00a6010000ab0100000000000000007d0b744b0000000000000000000064
+                  1302007c006a2600000000000000007c037c0466026414890d69017c05a4
+                  018e017c0a7c03890d7c097c047c017c04890d7c0b64159c0aa6020000ab
+                  0200000000000000005300
                              0 MAKE_CELL               13 (model)
                              2 MAKE_CELL               14 (request)
                
                 56           4 RESUME                   0
                
                 57           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (block)
@@ -706,369 +707,381 @@
                
                 88         684 LOAD_DEREF              13 (model)
                            686 LOAD_FAST                1 (context)
                            688 LOAD_CONST               4 ('wagtail_fedit_instance')
                            690 STORE_SUBSCR
                
                 92         694 LOAD_FAST                2 (block)
-                           696 POP_JUMP_FORWARD_IF_FALSE    88 (to 874)
+                           696 POP_JUMP_FORWARD_IF_FALSE    90 (to 878)
                
                 93         698 NOP
                
                 94         700 LOAD_FAST                1 (context)
                            702 LOAD_METHOD             11 (flatten)
                            724 PRECALL                  0
                            728 CALL                     0
                            738 STORE_FAST               8 (block_context)
-                           740 JUMP_FORWARD            16 (to 774)
+                           740 JUMP_FORWARD            18 (to 778)
                        >>  742 PUSH_EXC_INFO
                
                 95         744 LOAD_GLOBAL             24 (AttributeError)
                            756 CHECK_EXC_MATCH
-                           758 POP_JUMP_FORWARD_IF_FALSE     3 (to 766)
+                           758 POP_JUMP_FORWARD_IF_FALSE     5 (to 770)
                            760 POP_TOP
                
-                96         762 POP_EXCEPT
-                           764 JUMP_FORWARD             4 (to 774)
-               
-                95     >>  766 RERAISE                  0
-                       >>  768 COPY                     3
-                           770 POP_EXCEPT
-                           772 RERAISE                  1
-               
-                97     >>  774 LOAD_FAST                8 (block_context)
-                           776 LOAD_METHOD             13 (update)
-                           798 LOAD_FAST                5 (extra)
-                           800 PRECALL                  1
-                           804 CALL                     1
-                           814 POP_TOP
-               
-                98         816 LOAD_FAST                2 (block)
-                           818 LOAD_METHOD             14 (render_as_block)
-                           840 LOAD_FAST                8 (block_context)
-                           842 PRECALL                  1
-                           846 CALL                     1
-                           856 STORE_FAST               9 (rendered)
-               
-                99         858 LOAD_CONST               5 (True)
-                           860 LOAD_FAST                0 (self)
-                           862 STORE_ATTR              15 (has_block)
-                           872 JUMP_FORWARD            56 (to 986)
-               
-               100     >>  874 LOAD_FAST                0 (self)
-                           876 LOAD_ATTR               16 (nl)
-                           886 POP_JUMP_FORWARD_IF_FALSE    34 (to 956)
-               
-               101         888 LOAD_FAST                0 (self)
-                           890 LOAD_ATTR               16 (nl)
-                           900 LOAD_METHOD             17 (render)
-                           922 LOAD_FAST                1 (context)
-                           924 PRECALL                  1
-                           928 CALL                     1
-                           938 STORE_FAST               9 (rendered)
-               
-               102         940 LOAD_CONST               6 (False)
-                           942 LOAD_FAST                0 (self)
-                           944 STORE_ATTR              15 (has_block)
-                           954 JUMP_FORWARD            15 (to 986)
-               
-               104     >>  956 LOAD_GLOBAL             19 (NULL + ValueError)
-                           968 LOAD_CONST               7 ('Block or nodelist is required')
-                           970 PRECALL                  1
-                           974 CALL                     1
-                           984 RAISE_VARARGS            1
-               
-               106     >>  986 LOAD_FAST                4 (field_name)
-                           988 POP_JUMP_FORWARD_IF_TRUE    37 (to 1064)
-               
-               107         990 LOAD_GLOBAL             37 (NULL + warnings)
-                          1002 LOAD_ATTR               19 (warn)
-               
-               108        1012 LOAD_GLOBAL             40 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-               
-               109        1024 LOAD_CONST               8 ('object')
-                          1026 LOAD_FAST                1 (context)
-                          1028 LOAD_ATTR               21 (template_name)
-                          1038 BUILD_MAP                1
-               
-               108        1040 BINARY_OP                6 (%)
-               
-               107        1044 PRECALL                  1
-                          1048 CALL                     1
-                          1058 POP_TOP
-               
-               111        1060 LOAD_FAST                9 (rendered)
-                          1062 RETURN_VALUE
-               
-               113     >> 1064 LOAD_DEREF              13 (model)
-                          1066 POP_JUMP_FORWARD_IF_TRUE    47 (to 1162)
-               
-               114        1068 LOAD_GLOBAL             37 (NULL + warnings)
-                          1080 LOAD_ATTR               19 (warn)
-               
-               115        1090 LOAD_GLOBAL             44 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-               
-               116        1102 LOAD_CONST               8 ('object')
-                          1104 LOAD_FAST                2 (block)
-                          1106 LOAD_ATTR                0 (block)
-                          1116 LOAD_ATTR               23 (__class__)
-                          1126 LOAD_ATTR               24 (__name__)
-                          1136 BUILD_MAP                1
-               
-               115        1138 BINARY_OP                6 (%)
-               
-               114        1142 PRECALL                  1
-                          1146 CALL                     1
-                          1156 POP_TOP
-               
-               118        1158 LOAD_FAST                9 (rendered)
-                          1160 RETURN_VALUE
-               
-               121     >> 1162 LOAD_FAST                3 (block_id)
-                          1164 POP_JUMP_FORWARD_IF_TRUE    13 (to 1192)
-                          1166 LOAD_CONST               2 ('block_id')
-                          1168 LOAD_FAST                1 (context)
-                          1170 CONTAINS_OP              0
-                          1172 POP_JUMP_FORWARD_IF_FALSE     9 (to 1192)
-               
-               122        1174 LOAD_FAST                1 (context)
-                          1176 LOAD_CONST               2 ('block_id')
-                          1178 BINARY_SUBSCR
-                          1188 STORE_FAST               3 (block_id)
-                          1190 JUMP_FORWARD            45 (to 1282)
-               
-               123     >> 1192 LOAD_FAST                3 (block_id)
-                          1194 POP_JUMP_FORWARD_IF_TRUE    26 (to 1248)
-                          1196 LOAD_FAST                2 (block)
-                          1198 POP_JUMP_FORWARD_IF_FALSE    24 (to 1248)
-                          1200 LOAD_GLOBAL             51 (NULL + hasattr)
-                          1212 LOAD_FAST                2 (block)
-                          1214 LOAD_CONST               9 ('id')
-                          1216 PRECALL                  2
-                          1220 CALL                     2
-                          1230 POP_JUMP_FORWARD_IF_FALSE     8 (to 1248)
-               
-               124        1232 LOAD_FAST                2 (block)
-                          1234 LOAD_ATTR               26 (id)
-                          1244 STORE_FAST               3 (block_id)
-                          1246 JUMP_FORWARD            17 (to 1282)
-               
-               125     >> 1248 LOAD_FAST                3 (block_id)
-                          1250 POP_JUMP_FORWARD_IF_TRUE    15 (to 1282)
-               
-               126        1252 LOAD_GLOBAL             19 (NULL + ValueError)
-                          1264 LOAD_CONST               3 ('Block ID is required')
-                          1266 PRECALL                  1
-                          1270 CALL                     1
-                          1280 RAISE_VARARGS            1
-               
-               129     >> 1282 LOAD_FAST                1 (context)
-                          1284 LOAD_METHOD             10 (get)
-                          1306 LOAD_CONST              10 ('request')
-                          1308 PRECALL                  1
-                          1312 CALL                     1
-                          1322 STORE_DEREF             14 (request)
-               
-               130        1324 LOAD_GLOBAL             55 (NULL + _can_edit)
-                          1336 LOAD_DEREF              14 (request)
-                          1338 LOAD_DEREF              13 (model)
-                          1340 PRECALL                  2
-                          1344 CALL                     2
-                          1354 POP_JUMP_FORWARD_IF_TRUE     2 (to 1360)
-               
-               131        1356 LOAD_FAST                9 (rendered)
-                          1358 RETURN_VALUE
-               
-               135     >> 1360 LOAD_GLOBAL             13 (NULL + isinstance)
-                          1372 LOAD_DEREF              13 (model)
-                          1374 LOAD_GLOBAL             56 (Page)
-                          1386 PRECALL                  2
-                          1390 CALL                     2
-                          1400 POP_JUMP_FORWARD_IF_FALSE    29 (to 1460)
-               
-               136        1402 LOAD_GLOBAL             59 (NULL + _get_from_context_or_set)
-               
-               137        1414 LOAD_FAST                1 (context)
-                          1416 LOAD_CONST              11 ('page_base_edit_url')
-               
-               138        1418 LOAD_CLOSURE            13 (model)
-                          1420 BUILD_TUPLE              1
-                          1422 LOAD_CONST              12 (<code object <lambda>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 138>)
-                          1424 MAKE_FUNCTION            8 (closure)
-               
-               136        1426 PRECALL                  3
-                          1430 CALL                     3
-                          1440 STORE_FAST              10 (admin_edit_url)
-               
-               143        1442 LOAD_FAST               10 (admin_edit_url)
-                          1444 FORMAT_VALUE             0
-                          1446 LOAD_CONST              13 ('#block-')
-                          1448 LOAD_FAST                3 (block_id)
-                          1450 FORMAT_VALUE             0
-                          1452 LOAD_CONST              14 ('-section')
-                          1454 BUILD_STRING             4
-                          1456 STORE_FAST              10 (admin_edit_url)
-                          1458 JUMP_FORWARD             2 (to 1464)
-               
-               145     >> 1460 LOAD_CONST               0 (None)
-                          1462 STORE_FAST              10 (admin_edit_url)
-               
-               147     >> 1464 LOAD_FAST                0 (self)
-                          1466 LOAD_ATTR               15 (has_block)
-                          1476 LOAD_FAST                5 (extra)
-                          1478 LOAD_CONST              15 ('has_block')
-                          1480 STORE_SUBSCR
-               
-               150        1484 LOAD_GLOBAL             61 (NULL + FeditBlockEditButton)
-                          1496 PRECALL                  0
-                          1500 CALL                     0
-               
-               149        1510 BUILD_LIST               1
-                          1512 STORE_FAST              11 (items)
-               
-               153        1514 LOAD_GLOBAL             63 (NULL + hooks)
-                          1526 LOAD_ATTR               32 (get_hooks)
-                          1536 LOAD_GLOBAL             66 (CONSTRUCT_BLOCK_TOOLBAR)
-                          1548 PRECALL                  1
-                          1552 CALL                     1
-                          1562 GET_ITER
-                       >> 1564 FOR_ITER                18 (to 1602)
-                          1566 STORE_FAST              12 (hook)
-               
-               154        1568 PUSH_NULL
-                          1570 LOAD_FAST               12 (hook)
-                          1572 LOAD_DEREF              14 (request)
-                          1574 LOAD_FAST               11 (items)
-                          1576 LOAD_DEREF              13 (model)
-                          1578 LOAD_FAST                3 (block_id)
-                          1580 LOAD_FAST                4 (field_name)
-                          1582 KW_NAMES                16
-                          1584 PRECALL                  5
-                          1588 CALL                     5
-                          1598 POP_TOP
-                          1600 JUMP_BACKWARD           19 (to 1564)
-               
-               156     >> 1602 LOAD_CLOSURE            14 (request)
-                          1604 BUILD_TUPLE              1
-                          1606 LOAD_CONST              17 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 156>)
-                          1608 MAKE_FUNCTION            8 (closure)
-                          1610 LOAD_FAST               11 (items)
-                          1612 GET_ITER
-                          1614 PRECALL                  0
-                          1618 CALL                     0
-                          1628 STORE_FAST              11 (items)
-               
-               157        1630 LOAD_GLOBAL             69 (NULL + list)
-                          1642 LOAD_GLOBAL             71 (NULL + filter)
-                          1654 LOAD_CONST               0 (None)
-                          1656 LOAD_FAST               11 (items)
-                          1658 PRECALL                  2
-                          1662 CALL                     2
-                          1672 PRECALL                  1
-                          1676 CALL                     1
-                          1686 STORE_FAST              11 (items)
-               
-               159        1688 LOAD_GLOBAL             73 (NULL + render_to_string)
-               
-               160        1700 LOAD_CONST              18 ('wagtail_fedit/content/editable_block.html')
-               
-               162        1702 PUSH_NULL
-                          1704 LOAD_FAST                0 (self)
-                          1706 LOAD_ATTR               37 (get_edit_url)
-               
-               163        1716 LOAD_FAST                3 (block_id)
-                          1718 LOAD_FAST                4 (field_name)
-               
-               162        1720 BUILD_TUPLE              2
-                          1722 LOAD_CONST              19 ('instance')
-               
-               164        1724 LOAD_DEREF              13 (model)
-               
-               162        1726 BUILD_MAP                1
-               
-               165        1728 LOAD_FAST                5 (extra)
-               
-               162        1730 DICT_MERGE               1
-                          1732 CALL_FUNCTION_EX         1
-               
-               167        1734 LOAD_FAST               10 (admin_edit_url)
-               
-               168        1736 LOAD_FAST                3 (block_id)
-               
-               169        1738 LOAD_DEREF              13 (model)
-               
-               170        1740 LOAD_FAST                9 (rendered)
-               
-               171        1742 LOAD_FAST                4 (field_name)
-               
-               172        1744 LOAD_FAST                1 (context)
-               
-               173        1746 LOAD_FAST                4 (field_name)
-               
-               174        1748 LOAD_DEREF              13 (model)
-               
-               175        1750 LOAD_FAST               11 (items)
-               
-               161        1752 LOAD_CONST              20 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items'))
-                          1754 BUILD_CONST_KEY_MAP     10
-               
-               159        1756 PRECALL                  2
-                          1760 CALL                     2
-                          1770 RETURN_VALUE
+                96         762 LOAD_FAST                1 (context)
+                           764 STORE_FAST               8 (block_context)
+                           766 POP_EXCEPT
+                           768 JUMP_FORWARD             4 (to 778)
+               
+                95     >>  770 RERAISE                  0
+                       >>  772 COPY                     3
+                           774 POP_EXCEPT
+                           776 RERAISE                  1
+               
+                97     >>  778 LOAD_FAST                8 (block_context)
+                           780 LOAD_METHOD             13 (update)
+                           802 LOAD_FAST                5 (extra)
+                           804 PRECALL                  1
+                           808 CALL                     1
+                           818 POP_TOP
+               
+                98         820 LOAD_FAST                2 (block)
+                           822 LOAD_METHOD             14 (render_as_block)
+                           844 LOAD_FAST                8 (block_context)
+                           846 PRECALL                  1
+                           850 CALL                     1
+                           860 STORE_FAST               9 (rendered)
+               
+                99         862 LOAD_CONST               5 (True)
+                           864 LOAD_FAST                0 (self)
+                           866 STORE_ATTR              15 (has_block)
+                           876 JUMP_FORWARD            56 (to 990)
+               
+               100     >>  878 LOAD_FAST                0 (self)
+                           880 LOAD_ATTR               16 (nl)
+                           890 POP_JUMP_FORWARD_IF_FALSE    34 (to 960)
+               
+               101         892 LOAD_FAST                0 (self)
+                           894 LOAD_ATTR               16 (nl)
+                           904 LOAD_METHOD             17 (render)
+                           926 LOAD_FAST                1 (context)
+                           928 PRECALL                  1
+                           932 CALL                     1
+                           942 STORE_FAST               9 (rendered)
+               
+               102         944 LOAD_CONST               6 (False)
+                           946 LOAD_FAST                0 (self)
+                           948 STORE_ATTR              15 (has_block)
+                           958 JUMP_FORWARD            15 (to 990)
+               
+               104     >>  960 LOAD_GLOBAL             19 (NULL + ValueError)
+                           972 LOAD_CONST               7 ('Block or nodelist is required')
+                           974 PRECALL                  1
+                           978 CALL                     1
+                           988 RAISE_VARARGS            1
+               
+               106     >>  990 LOAD_FAST                4 (field_name)
+                           992 POP_JUMP_FORWARD_IF_TRUE    37 (to 1068)
+               
+               107         994 LOAD_GLOBAL             37 (NULL + warnings)
+                          1006 LOAD_ATTR               19 (warn)
+               
+               108        1016 LOAD_GLOBAL             40 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+               
+               109        1028 LOAD_CONST               8 ('object')
+                          1030 LOAD_FAST                1 (context)
+                          1032 LOAD_ATTR               21 (template_name)
+                          1042 BUILD_MAP                1
+               
+               108        1044 BINARY_OP                6 (%)
+               
+               107        1048 PRECALL                  1
+                          1052 CALL                     1
+                          1062 POP_TOP
+               
+               111        1064 LOAD_FAST                9 (rendered)
+                          1066 RETURN_VALUE
+               
+               113     >> 1068 LOAD_DEREF              13 (model)
+                          1070 POP_JUMP_FORWARD_IF_TRUE    47 (to 1166)
+               
+               114        1072 LOAD_GLOBAL             37 (NULL + warnings)
+                          1084 LOAD_ATTR               19 (warn)
+               
+               115        1094 LOAD_GLOBAL             44 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+               
+               116        1106 LOAD_CONST               8 ('object')
+                          1108 LOAD_FAST                2 (block)
+                          1110 LOAD_ATTR                0 (block)
+                          1120 LOAD_ATTR               23 (__class__)
+                          1130 LOAD_ATTR               24 (__name__)
+                          1140 BUILD_MAP                1
+               
+               115        1142 BINARY_OP                6 (%)
+               
+               114        1146 PRECALL                  1
+                          1150 CALL                     1
+                          1160 POP_TOP
+               
+               118        1162 LOAD_FAST                9 (rendered)
+                          1164 RETURN_VALUE
+               
+               121     >> 1166 LOAD_FAST                3 (block_id)
+                          1168 POP_JUMP_FORWARD_IF_TRUE    13 (to 1196)
+                          1170 LOAD_CONST               2 ('block_id')
+                          1172 LOAD_FAST                1 (context)
+                          1174 CONTAINS_OP              0
+                          1176 POP_JUMP_FORWARD_IF_FALSE     9 (to 1196)
+               
+               122        1178 LOAD_FAST                1 (context)
+                          1180 LOAD_CONST               2 ('block_id')
+                          1182 BINARY_SUBSCR
+                          1192 STORE_FAST               3 (block_id)
+                          1194 JUMP_FORWARD            45 (to 1286)
+               
+               123     >> 1196 LOAD_FAST                3 (block_id)
+                          1198 POP_JUMP_FORWARD_IF_TRUE    26 (to 1252)
+                          1200 LOAD_FAST                2 (block)
+                          1202 POP_JUMP_FORWARD_IF_FALSE    24 (to 1252)
+                          1204 LOAD_GLOBAL             51 (NULL + hasattr)
+                          1216 LOAD_FAST                2 (block)
+                          1218 LOAD_CONST               9 ('id')
+                          1220 PRECALL                  2
+                          1224 CALL                     2
+                          1234 POP_JUMP_FORWARD_IF_FALSE     8 (to 1252)
+               
+               124        1236 LOAD_FAST                2 (block)
+                          1238 LOAD_ATTR               26 (id)
+                          1248 STORE_FAST               3 (block_id)
+                          1250 JUMP_FORWARD            17 (to 1286)
+               
+               125     >> 1252 LOAD_FAST                3 (block_id)
+                          1254 POP_JUMP_FORWARD_IF_TRUE    15 (to 1286)
+               
+               126        1256 LOAD_GLOBAL             19 (NULL + ValueError)
+                          1268 LOAD_CONST               3 ('Block ID is required')
+                          1270 PRECALL                  1
+                          1274 CALL                     1
+                          1284 RAISE_VARARGS            1
+               
+               128     >> 1286 LOAD_FAST                9 (rendered)
+                          1288 POP_JUMP_FORWARD_IF_TRUE    15 (to 1320)
+               
+               129        1290 LOAD_GLOBAL             55 (NULL + mark_safe)
+                          1302 LOAD_CONST              10 ('')
+                          1304 PRECALL                  1
+                          1308 CALL                     1
+                          1318 STORE_FAST               9 (rendered)
+               
+               132     >> 1320 LOAD_FAST                1 (context)
+                          1322 LOAD_METHOD             10 (get)
+                          1344 LOAD_CONST              11 ('request')
+                          1346 PRECALL                  1
+                          1350 CALL                     1
+                          1360 STORE_DEREF             14 (request)
+               
+               133        1362 LOAD_GLOBAL             57 (NULL + _can_edit)
+                          1374 LOAD_DEREF              14 (request)
+                          1376 LOAD_DEREF              13 (model)
+                          1378 PRECALL                  2
+                          1382 CALL                     2
+                          1392 POP_JUMP_FORWARD_IF_TRUE     2 (to 1398)
+               
+               134        1394 LOAD_FAST                9 (rendered)
+                          1396 RETURN_VALUE
+               
+               138     >> 1398 LOAD_GLOBAL             13 (NULL + isinstance)
+                          1410 LOAD_DEREF              13 (model)
+                          1412 LOAD_GLOBAL             58 (Page)
+                          1424 PRECALL                  2
+                          1428 CALL                     2
+                          1438 POP_JUMP_FORWARD_IF_FALSE    29 (to 1498)
+               
+               139        1440 LOAD_GLOBAL             61 (NULL + _get_from_context_or_set)
+               
+               140        1452 LOAD_FAST                1 (context)
+                          1454 LOAD_CONST              12 ('page_base_edit_url')
+               
+               141        1456 LOAD_CLOSURE            13 (model)
+                          1458 BUILD_TUPLE              1
+                          1460 LOAD_CONST              13 (<code object <lambda>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 141>)
+                          1462 MAKE_FUNCTION            8 (closure)
+               
+               139        1464 PRECALL                  3
+                          1468 CALL                     3
+                          1478 STORE_FAST              10 (admin_edit_url)
+               
+               146        1480 LOAD_FAST               10 (admin_edit_url)
+                          1482 FORMAT_VALUE             0
+                          1484 LOAD_CONST              14 ('#block-')
+                          1486 LOAD_FAST                3 (block_id)
+                          1488 FORMAT_VALUE             0
+                          1490 LOAD_CONST              15 ('-section')
+                          1492 BUILD_STRING             4
+                          1494 STORE_FAST              10 (admin_edit_url)
+                          1496 JUMP_FORWARD             2 (to 1502)
+               
+               148     >> 1498 LOAD_CONST               0 (None)
+                          1500 STORE_FAST              10 (admin_edit_url)
+               
+               150     >> 1502 LOAD_FAST                0 (self)
+                          1504 LOAD_ATTR               15 (has_block)
+                          1514 LOAD_FAST                5 (extra)
+                          1516 LOAD_CONST              16 ('has_block')
+                          1518 STORE_SUBSCR
+               
+               153        1522 LOAD_GLOBAL             63 (NULL + FeditBlockEditButton)
+                          1534 PRECALL                  0
+                          1538 CALL                     0
+               
+               152        1548 BUILD_LIST               1
+                          1550 STORE_FAST              11 (items)
+               
+               156        1552 LOAD_GLOBAL             65 (NULL + hooks)
+                          1564 LOAD_ATTR               33 (get_hooks)
+                          1574 LOAD_GLOBAL             68 (CONSTRUCT_BLOCK_TOOLBAR)
+                          1586 PRECALL                  1
+                          1590 CALL                     1
+                          1600 GET_ITER
+                       >> 1602 FOR_ITER                18 (to 1640)
+                          1604 STORE_FAST              12 (hook)
+               
+               157        1606 PUSH_NULL
+                          1608 LOAD_FAST               12 (hook)
+                          1610 LOAD_DEREF              14 (request)
+                          1612 LOAD_FAST               11 (items)
+                          1614 LOAD_DEREF              13 (model)
+                          1616 LOAD_FAST                3 (block_id)
+                          1618 LOAD_FAST                4 (field_name)
+                          1620 KW_NAMES                17
+                          1622 PRECALL                  5
+                          1626 CALL                     5
+                          1636 POP_TOP
+                          1638 JUMP_BACKWARD           19 (to 1602)
+               
+               159     >> 1640 LOAD_CLOSURE            14 (request)
+                          1642 BUILD_TUPLE              1
+                          1644 LOAD_CONST              18 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 159>)
+                          1646 MAKE_FUNCTION            8 (closure)
+                          1648 LOAD_FAST               11 (items)
+                          1650 GET_ITER
+                          1652 PRECALL                  0
+                          1656 CALL                     0
+                          1666 STORE_FAST              11 (items)
+               
+               160        1668 LOAD_GLOBAL             71 (NULL + list)
+                          1680 LOAD_GLOBAL             73 (NULL + filter)
+                          1692 LOAD_CONST               0 (None)
+                          1694 LOAD_FAST               11 (items)
+                          1696 PRECALL                  2
+                          1700 CALL                     2
+                          1710 PRECALL                  1
+                          1714 CALL                     1
+                          1724 STORE_FAST              11 (items)
+               
+               162        1726 LOAD_GLOBAL             75 (NULL + render_to_string)
+               
+               163        1738 LOAD_CONST              19 ('wagtail_fedit/content/editable_block.html')
+               
+               165        1740 PUSH_NULL
+                          1742 LOAD_FAST                0 (self)
+                          1744 LOAD_ATTR               38 (get_edit_url)
+               
+               166        1754 LOAD_FAST                3 (block_id)
+                          1756 LOAD_FAST                4 (field_name)
+               
+               165        1758 BUILD_TUPLE              2
+                          1760 LOAD_CONST              20 ('instance')
+               
+               167        1762 LOAD_DEREF              13 (model)
+               
+               165        1764 BUILD_MAP                1
+               
+               168        1766 LOAD_FAST                5 (extra)
+               
+               165        1768 DICT_MERGE               1
+                          1770 CALL_FUNCTION_EX         1
+               
+               170        1772 LOAD_FAST               10 (admin_edit_url)
+               
+               171        1774 LOAD_FAST                3 (block_id)
+               
+               172        1776 LOAD_DEREF              13 (model)
+               
+               173        1778 LOAD_FAST                9 (rendered)
+               
+               174        1780 LOAD_FAST                4 (field_name)
+               
+               175        1782 LOAD_FAST                1 (context)
+               
+               176        1784 LOAD_FAST                4 (field_name)
+               
+               177        1786 LOAD_DEREF              13 (model)
+               
+               178        1788 LOAD_FAST               11 (items)
+               
+               164        1790 LOAD_CONST              21 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items'))
+                          1792 BUILD_CONST_KEY_MAP     10
+               
+               162        1794 PRECALL                  2
+                          1798 CALL                     2
+                          1808 RETURN_VALUE
                ExceptionTable:
                  700 to 738 -> 742 [0]
-                 742 to 760 -> 768 [1] lasti
-                 766 to 766 -> 768 [1] lasti
+                 742 to 764 -> 772 [1] lasti
+                 770 to 770 -> 772 [1] lasti
                consts
                   None
                   'wagtail_fedit_field_name'
                   'block_id'
                   'Block ID is required'
                   'wagtail_fedit_instance'
                   True
                   False
                   'Block or nodelist is required'
                   'object'
                   'id'
+                  ''
                   'request'
                   'page_base_edit_url'
                   code
                      argcount  : 0
                      nlocals   : 0
                      stacksize : 4
                      flags     : 19
                      code
                         0x95019700740100000000000000000000640189006a0100000000000000
                         006701ac02a6020000ab0200000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     138           2 RESUME                   0
+                     141           2 RESUME                   0
                                    4 LOAD_GLOBAL              1 (NULL + reverse)
                      
-                     139          16 LOAD_CONST               1 ('wagtailadmin_pages:edit')
+                     142          16 LOAD_CONST               1 ('wagtailadmin_pages:edit')
                      
-                     140          18 LOAD_DEREF               0 (model)
+                     143          18 LOAD_DEREF               0 (model)
                                   20 LOAD_ATTR                1 (id)
                                   30 BUILD_LIST               1
                      
-                     138          32 KW_NAMES                 2
+                     141          32 KW_NAMES                 2
                                   34 PRECALL                  2
                                   38 CALL                     2
                                   48 RETURN_VALUE
                      consts
                         None
                         'wagtailadmin_pages:edit'
                         ('args',)
                      names      ('reverse', 'id')
                      varnames   ()
                      freevars   ('model',)
                      cellvars   ()
-                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<lambda>'
-                     firstlineno 138
+                     firstlineno 141
                      lnotab 0x100102010efe
                   '#block-'
                   '-section'
                   'has_block'
                   ('request', 'items', 'model', 'block_id', 'field_name')
                   code
                      argcount  : 1
@@ -1076,15 +1089,15 @@
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d177d017c01a00000000000000000000000000000
                         000000000000008902a6010000ab01000000000000000091028c185300
                                    0 COPY_FREE_VARS           1
                      
-                     156           2 RESUME                   0
+                     159           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                23 (to 56)
                                   10 STORE_FAST               1 (item)
                                   12 LOAD_FAST                1 (item)
                                   14 LOAD_METHOD              0 (render)
                                   36 LOAD_DEREF               2 (request)
@@ -1094,87 +1107,87 @@
                                   54 JUMP_BACKWARD           24 (to 8)
                              >>   56 RETURN_VALUE
                      consts
                      names      ('render',)
                      varnames   ('.0', 'item')
                      freevars   ('request',)
                      cellvars   ()
-                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<listcomp>'
-                     firstlineno 156
+                     firstlineno 159
                      lnotab 0x
                   'wagtail_fedit/content/editable_block.html'
                   'instance'
                   ('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items')
-               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', 'ValueError', 'get', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'warnings', 'warn', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'template_name', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__class__', '__name__', 'hasattr', 'id', '_can_edit', 'Page', '_get_from_context_or_set', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'get_edit_url')
+               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', 'ValueError', 'get', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'warnings', 'warn', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'template_name', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__class__', '__name__', 'hasattr', 'id', 'mark_safe', '_can_edit', 'Page', '_get_from_context_or_set', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'get_edit_url')
                varnames   ('self', 'context', 'block', 'block_id', 'field_name', 'extra', 'k', 'e', 'block_context', 'rendered', 'admin_edit_url', 'items', 'hook')
                freevars   ()
                cellvars   ('model', 'request')
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
                firstlineno 56
                lnotab
                   0x06010e010e010e010e010e0332012a0132020c0110022a012a012a012a
-                  012a012a012a012a0210011e052e010a010a04040102012c01120104ff08
+                  012a012a012a012a0210011e052e010a010a04040102012c01120108ff08
                   022a012a0110010e01340110021e02040116010c0110ff04ff1004040204
-                  0116010c0124ff04ff100404030c0112012801100104011e032a01200104
-                  042a010c01040108fe10071202040214031aff0404360122021c013a020c
-                  0102020e0104ff040202fe020302fd040502010201020102010201020102
-                  01020102f204fe
+                  0116010c0124ff04ff100404030c0112012801100104011e0204011e032a
+                  01200104042a010c01040108fe10071202040214031aff0404360122021c
+                  013a020c0102020e0104ff040202fe020302fd0405020102010201020102
+                  0102010201020102f204fe
             'return'
             code
                argcount  : 0
                nlocals   : 4
                stacksize : 6
                flags     : 11
                code
                   0x970069007d017c00a00000000000000000000000000000000000000000
                   00a6000000ab00000000000000000044005d2f5c0200007d027d03740200
                   000000000000000000a00200000000000000000000000000000000000000
                   007407000000000000000000007c03a6010000ab010000000000000000a6
                   010000ab0100000000000000007c017c023c0000008c307c015300
-               179           0 RESUME                   0
+               182           0 RESUME                   0
                
-               182           2 BUILD_MAP                0
+               185           2 BUILD_MAP                0
                              4 STORE_FAST               1 (packed)
                
-               183           6 LOAD_FAST                0 (kwargs)
+               186           6 LOAD_FAST                0 (kwargs)
                              8 LOAD_METHOD              0 (items)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 GET_ITER
                        >>   46 FOR_ITER                47 (to 142)
                             48 UNPACK_SEQUENCE          2
                             52 STORE_FAST               2 (k)
                             54 STORE_FAST               3 (v)
                
-               184          56 LOAD_GLOBAL              2 (url_value_signer)
+               187          56 LOAD_GLOBAL              2 (url_value_signer)
                             68 LOAD_METHOD              2 (sign)
                             90 LOAD_GLOBAL              7 (NULL + str)
                            102 LOAD_FAST                3 (v)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 PRECALL                  1
                            122 CALL                     1
                            132 LOAD_FAST                1 (packed)
                            134 LOAD_FAST                2 (k)
                            136 STORE_SUBSCR
                            140 JUMP_BACKWARD           48 (to 46)
                
-               186     >>  142 LOAD_FAST                1 (packed)
+               189     >>  142 LOAD_FAST                1 (packed)
                            144 RETURN_VALUE
                consts
                   None
                names      ('items', 'url_value_signer', 'sign', 'str')
                varnames   ('kwargs', 'packed', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'pack'
-               firstlineno 179
+               firstlineno 182
                lnotab 0x0203040132015602
             ('request',)
             'expected'
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 7
@@ -1195,130 +1208,130 @@
                   057c039b009d02a6010000ab010000000000000000820177007803590077
                   0174150000000000000000000088046601640684087c024400a6000000ab
                   000000000000000000a6010000ab01000000000000000073187c00a00700
                   0000000000000000000000000000000000000064057c039b009d02a60100
                   00ab010000000000000000820189045300
                              0 MAKE_CELL                4 (unpacked)
                
-               188           2 RESUME                   0
+               191           2 RESUME                   0
                
-               190           4 LOAD_FAST                1 (request)
+               193           4 LOAD_FAST                1 (request)
                              6 POP_JUMP_FORWARD_IF_TRUE    15 (to 38)
                
-               191           8 LOAD_GLOBAL              1 (NULL + ValueError)
+               194           8 LOAD_GLOBAL              1 (NULL + ValueError)
                             20 LOAD_CONST               1 ('Request is required')
                             22 PRECALL                  1
                             26 CALL                     1
                             36 RAISE_VARARGS            1
                
-               193     >>   38 BUILD_MAP                0
+               196     >>   38 BUILD_MAP                0
                             40 STORE_DEREF              4 (unpacked)
                
-               194          42 LOAD_FAST                2 (expected)
+               197          42 LOAD_FAST                2 (expected)
                             44 GET_ITER
                        >>   46 FOR_ITER               171 (to 390)
                             48 STORE_FAST               3 (key)
                
-               195          50 NOP
+               198          50 NOP
                
-               196          52 LOAD_GLOBAL              2 (url_value_signer)
+               199          52 LOAD_GLOBAL              2 (url_value_signer)
                             64 LOAD_METHOD              2 (unsign)
                
-               197          86 LOAD_FAST                1 (request)
+               200          86 LOAD_FAST                1 (request)
                             88 LOAD_ATTR                3 (GET)
                             98 LOAD_METHOD              4 (get)
                            120 LOAD_FAST                3 (key)
                            122 PRECALL                  1
                            126 CALL                     1
                
-               196         136 PRECALL                  1
+               199         136 PRECALL                  1
                            140 CALL                     1
                            150 LOAD_DEREF               4 (unpacked)
                            152 LOAD_FAST                3 (key)
                            154 STORE_SUBSCR
                            158 JUMP_BACKWARD           57 (to 46)
                        >>  160 PUSH_EXC_INFO
                
-               199         162 LOAD_GLOBAL             10 (signing)
+               202         162 LOAD_GLOBAL             10 (signing)
                            174 LOAD_ATTR                6 (SignatureExpired)
                            184 CHECK_EXC_MATCH
                            186 POP_JUMP_FORWARD_IF_FALSE    26 (to 240)
                            188 POP_TOP
                
-               200         190 LOAD_FAST                0 (cls)
+               203         190 LOAD_FAST                0 (cls)
                            192 LOAD_METHOD              7 (UnpackError)
                            214 LOAD_CONST               2 ('Value for ')
                            216 LOAD_FAST                3 (key)
                            218 FORMAT_VALUE             0
                            220 LOAD_CONST               3 (' has expired')
                            222 BUILD_STRING             3
                            224 PRECALL                  1
                            228 CALL                     1
                            238 RAISE_VARARGS            1
                
-               201     >>  240 LOAD_GLOBAL             10 (signing)
+               204     >>  240 LOAD_GLOBAL             10 (signing)
                            252 LOAD_ATTR                8 (BadSignature)
                            262 CHECK_EXC_MATCH
                            264 POP_JUMP_FORWARD_IF_FALSE    25 (to 316)
                            266 POP_TOP
                
-               202         268 LOAD_FAST                0 (cls)
+               205         268 LOAD_FAST                0 (cls)
                            270 LOAD_METHOD              7 (UnpackError)
                            292 LOAD_CONST               4 ('Invalid value for ')
                            294 LOAD_FAST                3 (key)
                            296 FORMAT_VALUE             0
                            298 BUILD_STRING             2
                            300 PRECALL                  1
                            304 CALL                     1
                            314 RAISE_VARARGS            1
                
-               203     >>  316 LOAD_GLOBAL             18 (TypeError)
+               206     >>  316 LOAD_GLOBAL             18 (TypeError)
                            328 CHECK_EXC_MATCH
                            330 POP_JUMP_FORWARD_IF_FALSE    25 (to 382)
                            332 POP_TOP
                
-               204         334 LOAD_FAST                0 (cls)
+               207         334 LOAD_FAST                0 (cls)
                            336 LOAD_METHOD              7 (UnpackError)
                            358 LOAD_CONST               5 ('Missing value for ')
                            360 LOAD_FAST                3 (key)
                            362 FORMAT_VALUE             0
                            364 BUILD_STRING             2
                            366 PRECALL                  1
                            370 CALL                     1
                            380 RAISE_VARARGS            1
                
-               203     >>  382 RERAISE                  0
+               206     >>  382 RERAISE                  0
                        >>  384 COPY                     3
                            386 POP_EXCEPT
                            388 RERAISE                  1
                
-               206     >>  390 LOAD_GLOBAL             21 (NULL + all)
+               209     >>  390 LOAD_GLOBAL             21 (NULL + all)
                            402 LOAD_CLOSURE             4 (unpacked)
                            404 BUILD_TUPLE              1
-                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 206>)
+                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 209>)
                            408 MAKE_FUNCTION            8 (closure)
                            410 LOAD_FAST                2 (expected)
                            412 GET_ITER
                            414 PRECALL                  0
                            418 CALL                     0
                            428 PRECALL                  1
                            432 CALL                     1
                            442 POP_JUMP_FORWARD_IF_TRUE    24 (to 492)
                
-               207         444 LOAD_FAST                0 (cls)
+               210         444 LOAD_FAST                0 (cls)
                            446 LOAD_METHOD              7 (UnpackError)
                            468 LOAD_CONST               5 ('Missing value for ')
                            470 LOAD_FAST                3 (key)
                            472 FORMAT_VALUE             0
                            474 BUILD_STRING             2
                            476 PRECALL                  1
                            480 CALL                     1
                            490 RAISE_VARARGS            1
                
-               209     >>  492 LOAD_DEREF               4 (unpacked)
+               212     >>  492 LOAD_DEREF               4 (unpacked)
                            494 RETURN_VALUE
                ExceptionTable:
                  52 to 156 -> 160 [1]
                  160 to 382 -> 384 [2] lasti
                consts
                   None
                   'Request is required'
@@ -1332,15 +1345,15 @@
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d177d018902a00000000000000000000000000000
                         000000000000007c01a6010000ab01000000000000000091028c185300
                                    0 COPY_FREE_VARS           1
                      
-                     206           2 RESUME                   0
+                     209           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                23 (to 56)
                                   10 STORE_FAST               1 (key)
                                   12 LOAD_DEREF               2 (unpacked)
                                   14 LOAD_METHOD              0 (get)
                                   36 LOAD_FAST                1 (key)
@@ -1350,25 +1363,25 @@
                                   54 JUMP_BACKWARD           24 (to 8)
                              >>   56 RETURN_VALUE
                      consts
                      names      ('get',)
                      varnames   ('.0', 'key')
                      freevars   ('unpacked',)
                      cellvars   ()
-                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+                     filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<listcomp>'
-                     firstlineno 206
+                     firstlineno 209
                      lnotab 0x
                names      ('ValueError', 'url_value_signer', 'unsign', 'GET', 'get', 'signing', 'SignatureExpired', 'UnpackError', 'BadSignature', 'TypeError', 'all')
                varnames   ('cls', 'request', 'expected', 'key')
                freevars   ()
                cellvars   ('unpacked',)
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'unpack'
-               firstlineno 188
+               firstlineno 191
                lnotab
                   0x040204011e02040108010201220132ff1a031c0132011c013001120130
                   ff080336013002
             'instance'
             code
                argcount  : 3
                nlocals   : 6
@@ -1377,58 +1390,58 @@
                code
                   0x970074010000000000000000000064017c007c017c026a010000000000
                   0000006a0200000000000000007c026a0100000000000000006a03000000
                   00000000007c026a0400000000000000006705ac02a6020000ab02000000
                   00000000007d047c0373027c045300740b00000000000000000000740d00
                   0000000000000000006a070000000000000000640469007c03a4018e01a6
                   010000ab0100000000000000007d057c049b0064037c059b009d035300
-               211           0 RESUME                   0
+               214           0 RESUME                   0
                
-               213           2 LOAD_GLOBAL              1 (NULL + reverse)
+               216           2 LOAD_GLOBAL              1 (NULL + reverse)
                
-               214          14 LOAD_CONST               1 ('wagtail_fedit:edit_block')
+               217          14 LOAD_CONST               1 ('wagtail_fedit:edit_block')
                
-               215          16 LOAD_FAST                0 (block_id)
+               218          16 LOAD_FAST                0 (block_id)
                             18 LOAD_FAST                1 (field_name)
                             20 LOAD_FAST                2 (instance)
                             22 LOAD_ATTR                1 (_meta)
                             32 LOAD_ATTR                2 (app_label)
                             42 LOAD_FAST                2 (instance)
                             44 LOAD_ATTR                1 (_meta)
                             54 LOAD_ATTR                3 (model_name)
                             64 LOAD_FAST                2 (instance)
                             66 LOAD_ATTR                4 (pk)
                             76 BUILD_LIST               5
                
-               213          78 KW_NAMES                 2
+               216          78 KW_NAMES                 2
                             80 PRECALL                  2
                             84 CALL                     2
                             94 STORE_FAST               4 (base_url)
                
-               218          96 LOAD_FAST                3 (kwargs)
+               221          96 LOAD_FAST                3 (kwargs)
                             98 POP_JUMP_FORWARD_IF_TRUE     2 (to 104)
                
-               219         100 LOAD_FAST                4 (base_url)
+               222         100 LOAD_FAST                4 (base_url)
                            102 RETURN_VALUE
                
-               221     >>  104 LOAD_GLOBAL             11 (NULL + urlencode)
+               224     >>  104 LOAD_GLOBAL             11 (NULL + urlencode)
                
-               222         116 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+               225         116 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                            128 LOAD_ATTR                7 (pack)
                            138 LOAD_CONST               4 (())
                            140 BUILD_MAP                0
                            142 LOAD_FAST                3 (kwargs)
                            144 DICT_MERGE               1
                            146 CALL_FUNCTION_EX         1
                
-               221         148 PRECALL                  1
+               224         148 PRECALL                  1
                            152 CALL                     1
                            162 STORE_FAST               5 (packed)
                
-               224         164 LOAD_FAST                4 (base_url)
+               227         164 LOAD_FAST                4 (base_url)
                            166 FORMAT_VALUE             0
                            168 LOAD_CONST               3 ('?')
                            170 LOAD_FAST                5 (packed)
                            172 FORMAT_VALUE             0
                            174 BUILD_STRING             3
                            176 RETURN_VALUE
                consts
@@ -1437,29 +1450,29 @@
                   ('args',)
                   '?'
                   ()
                names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack')
                varnames   ('block_id', 'field_name', 'instance', 'kwargs', 'base_url', 'packed')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'get_edit_url'
-               firstlineno 211
+               firstlineno 214
                lnotab 0x02020c0102013efe1205040104020c0120ff1003
             (None, None, None, None, None)
          names      ('__name__', '__module__', '__qualname__', 'Exception', 'UnpackError', 'NodeList', 'BoundBlock', 'str', 'models', 'Model', '__init__', 'render', 'staticmethod', 'dict', 'pack', 'classmethod', 'unpack', 'get_edit_url')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'BlockEditNode'
          firstlineno 36
          lnotab
             0x0a011c04020102010201020102fb040102ff020202fe020302fd020402
-            fc02050cfb0810067b02010aff0e010208020114ff0e010216020120ff0e
+            fc02050cfb0810067e02010aff0e010208020114ff0e010216020120ff0e
             01
       'BlockEditNode'
       'fedit_block'
       ('name',)
       'parser'
       'token'
       code
@@ -1481,123 +1494,123 @@
             000000000000000000640a7c067c05a00700000000000000000000000000
             000000000000006403a6010000ab0100000000000000007c05a007000000
             00000000000000000000000000000000006406a6010000ab010000000000
             0000007c05a00700000000000000000000000000000000000000006407a6
             010000ab0100000000000000007c05a00700000000000000000000000000
             000000000000006408a6010000ab01000000000000000064099c057c07a4
             018e015300
-         228           0 RESUME                   0
+         231           0 RESUME                   0
          
-         258           2 LOAD_FAST                1 (token)
+         261           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         259          42 LOAD_FAST                2 (tokens)
+         262          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         260          84 BUILD_LIST               0
+         263          84 BUILD_LIST               0
                       86 LOAD_CONST               2 (('block', 'block_id', 'field_name', 'model'))
                       88 LIST_EXTEND              1
                       90 STORE_FAST               4 (kwargs_names)
          
-         265          92 LOAD_GLOBAL              5 (NULL + get_kwargs)
+         268          92 LOAD_GLOBAL              5 (NULL + get_kwargs)
                      104 LOAD_FAST                0 (parser)
                      106 LOAD_FAST                4 (kwargs_names)
                      108 LOAD_FAST                2 (tokens)
                      110 PRECALL                  3
                      114 CALL                     3
                      124 STORE_FAST               5 (kwargs)
          
-         267         126 LOAD_CONST               3 ('block')
+         270         126 LOAD_CONST               3 ('block')
                      128 LOAD_FAST                5 (kwargs)
                      130 CONTAINS_OP              1
                      132 POP_JUMP_FORWARD_IF_FALSE    42 (to 218)
          
-         268         134 LOAD_FAST                0 (parser)
+         271         134 LOAD_FAST                0 (parser)
                      136 LOAD_METHOD              3 (parse)
                      158 LOAD_CONST               4 (('unfedit_block',))
                      160 PRECALL                  1
                      164 CALL                     1
                      174 STORE_FAST               6 (nodelist)
          
-         269         176 LOAD_FAST                0 (parser)
+         272         176 LOAD_FAST                0 (parser)
                      178 LOAD_METHOD              4 (delete_first_token)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
                      216 JUMP_FORWARD             2 (to 222)
          
-         271     >>  218 LOAD_CONST               5 (None)
+         274     >>  218 LOAD_CONST               5 (None)
                      220 STORE_FAST               6 (nodelist)
          
-         273     >>  222 BUILD_MAP                0
+         276     >>  222 BUILD_MAP                0
                      224 STORE_FAST               7 (extra)
          
-         274         226 LOAD_FAST                5 (kwargs)
+         277         226 LOAD_FAST                5 (kwargs)
                      228 LOAD_METHOD              5 (items)
                      250 PRECALL                  0
                      254 CALL                     0
                      264 GET_ITER
                  >>  266 FOR_ITER                14 (to 296)
                      268 UNPACK_SEQUENCE          2
                      272 STORE_FAST               8 (key)
                      274 STORE_FAST               9 (value)
          
-         275         276 LOAD_FAST                8 (key)
+         278         276 LOAD_FAST                8 (key)
                      278 LOAD_FAST                4 (kwargs_names)
                      280 CONTAINS_OP              1
                      282 POP_JUMP_FORWARD_IF_FALSE     5 (to 294)
          
-         276         284 LOAD_FAST                9 (value)
+         279         284 LOAD_FAST                9 (value)
                      286 LOAD_FAST                7 (extra)
                      288 LOAD_FAST                8 (key)
                      290 STORE_SUBSCR
                  >>  294 JUMP_BACKWARD           15 (to 266)
          
-         278     >>  296 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+         281     >>  296 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                      308 LOAD_CONST              10 (())
          
-         279         310 LOAD_FAST                6 (nodelist)
+         282         310 LOAD_FAST                6 (nodelist)
          
-         280         312 LOAD_FAST                5 (kwargs)
+         283         312 LOAD_FAST                5 (kwargs)
                      314 LOAD_METHOD              7 (get)
                      336 LOAD_CONST               3 ('block')
                      338 PRECALL                  1
                      342 CALL                     1
          
-         281         352 LOAD_FAST                5 (kwargs)
+         284         352 LOAD_FAST                5 (kwargs)
                      354 LOAD_METHOD              7 (get)
                      376 LOAD_CONST               6 ('block_id')
                      378 PRECALL                  1
                      382 CALL                     1
          
-         282         392 LOAD_FAST                5 (kwargs)
+         285         392 LOAD_FAST                5 (kwargs)
                      394 LOAD_METHOD              7 (get)
                      416 LOAD_CONST               7 ('field_name')
                      418 PRECALL                  1
                      422 CALL                     1
          
-         283         432 LOAD_FAST                5 (kwargs)
+         286         432 LOAD_FAST                5 (kwargs)
                      434 LOAD_METHOD              7 (get)
                      456 LOAD_CONST               8 ('model')
                      458 PRECALL                  1
                      462 CALL                     1
          
-         278         472 LOAD_CONST               9 (('nodelist', 'block', 'block_id', 'field_name', 'model'))
+         281         472 LOAD_CONST               9 (('nodelist', 'block', 'block_id', 'field_name', 'model'))
                      474 BUILD_CONST_KEY_MAP      5
          
-         284         476 LOAD_FAST                7 (extra)
+         287         476 LOAD_FAST                7 (extra)
          
-         278         478 DICT_MERGE               1
+         281         478 DICT_MERGE               1
                      480 CALL_FUNCTION_EX         1
                      482 RETURN_VALUE
          consts
             '\n    This tag is used to render an editable block.\n\n    This block will be wrapped and is able to be edited by the user on the frontend.\n\n    We will require the block_id and field_name of the streamfield this block belongs to.\n\n    You could omit needing to pass a block ID by passing in the StreamChild instance as opposed to the StructValue instance.\n    \n    Usage example 1:\n        ```python\n        {% fedit_block my_structvalue_instance block_id my_streamfield_attribute_name page_instance %}\n        ```\n\n    Optionally you can omit the block and pass in the block_id and field_name as keyword arguments.\n\n    This will allow you to use the block as a block tag.\n\n    Usage example 2:\n        ```python\n        {% fedit_block block_id=my_structvalue_instance field_name=my_streamfield_attribute_name model=page_instance %}\n            <p>Some content before block</p>\n            {% include_block my_block %}\n            <p>Some content after block</p>\n        {% unfedit_block %}\n        ```\n    '
             0
             ('block', 'block_id', 'field_name', 'model')
             'block'
@@ -1608,51 +1621,51 @@
             'model'
             ('nodelist', 'block', 'block_id', 'field_name', 'model')
             ()
          names      ('split_contents', 'pop', 'get_kwargs', 'parse', 'delete_first_token', 'items', 'BlockEditNode', 'get')
          varnames   ('parser', 'token', 'tokens', '_', 'kwargs_names', 'kwargs', 'nodelist', 'extra', 'key', 'value')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_block'
-         firstlineno 228
+         firstlineno 231
          lnotab
             0x021e28012a010805220208012a012a0204020401320108010c020e0102
             0128012801280128fb040602fa
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a026408640265036a040000000000000000640365
             05650619000000000000000000640465076606640584055a08640684005a
             0964075300
-         288           0 RESUME                   0
+         291           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('FieldEditNode')
                        8 STORE_NAME               2 (__qualname__)
          
-         289          10 LOAD_CONST               8 ((False,))
+         292          10 LOAD_CONST               8 ((False,))
                       12 LOAD_CONST               2 ('model')
                       14 LOAD_NAME                3 (models)
                       16 LOAD_ATTR                4 (Model)
                       26 LOAD_CONST               3 ('getters')
                       28 LOAD_NAME                5 (list)
                       30 LOAD_NAME                6 (str)
                       32 BINARY_SUBSCR
                       42 LOAD_CONST               4 ('inline')
                       44 LOAD_NAME                7 (bool)
                       46 BUILD_TUPLE              6
-                      48 LOAD_CONST               5 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 289>)
+                      48 LOAD_CONST               5 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 292>)
                       50 MAKE_FUNCTION            5 (defaults, annotations)
                       52 STORE_NAME               8 (__init__)
          
-         296          54 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 296>)
+         299          54 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 299>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               9 (render)
                       60 LOAD_CONST               7 (None)
                       62 RETURN_VALUE
          consts
             'FieldEditNode'
             False
@@ -1666,54 +1679,54 @@
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027403000000000000000000
                   007c02a6010000ab01000000000000000064017a0a000019000000000000
                   0000007c005f0200000000000000007c027c005f0300000000000000007c
                   037c005f0400000000000000007c047c005f050000000000000000640053
                   00
-               289           0 RESUME                   0
+               292           0 RESUME                   0
                
-               290           2 LOAD_FAST                1 (model)
+               293           2 LOAD_FAST                1 (model)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (model)
                
-               291          16 LOAD_FAST                2 (getters)
+               294          16 LOAD_FAST                2 (getters)
                             18 LOAD_GLOBAL              3 (NULL + len)
                             30 LOAD_FAST                2 (getters)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 LOAD_CONST               1 (1)
                             48 BINARY_OP               10 (-)
                             52 BINARY_SUBSCR
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               2 (field)
                
-               292          74 LOAD_FAST                2 (getters)
+               295          74 LOAD_FAST                2 (getters)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               3 (getters)
                
-               293          88 LOAD_FAST                3 (inline)
+               296          88 LOAD_FAST                3 (inline)
                             90 LOAD_FAST                0 (self)
                             92 STORE_ATTR               4 (inline)
                
-               294         102 LOAD_FAST                4 (kwargs)
+               297         102 LOAD_FAST                4 (kwargs)
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (kwargs)
                            116 LOAD_CONST               0 (None)
                            118 RETURN_VALUE
                consts
                   None
                   1
                names      ('model', 'len', 'field', 'getters', 'inline', 'kwargs')
                varnames   ('self', 'model', 'getters', 'inline', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 289
+               firstlineno 292
                lnotab 0x02010e013a010e010e01
             code
                argcount  : 2
                nlocals   : 10
                stacksize : 10
                flags     : 3
                code
@@ -1731,209 +1744,220 @@
                   007d058c1c23007412000000000000000000002400722001007413000000
                   0000000000000064027c036a0a00000000000000006a0b00000000000000
                   009b0064037c079b009d04a6010000ab0100000000000000008201770078
                   03590077017c01a00c000000000000000000000000000000000000000064
                   04a6010000ab0100000000000000007d08741b000000000000000000007c
                   087c057c056a0e0000000000000000a00f00000000000000000000000000
                   000000000000007c006a100000000000000000a6010000ab010000000000
-                  0000007c01a6040000ab0400000000000000007d09742300000000000000
-                  0000007c087c05a6020000ab02000000000000000073027c095300742500
-                  00000000000000000064067c087c097c006a1000000000000000007c057c
-                  017c0464059c067c006a130000000000000000a4018e015300
-               296           0 RESUME                   0
+                  0000007c01a6040000ab0400000000000000007d097c09730f7423000000
+                  000000000000006405a6010000ab0100000000000000007d097425000000
+                  000000000000007c087c05a6020000ab02000000000000000073027c0953
+                  0074270000000000000000000064077c087c097c006a1000000000000000
+                  007c057c017c0464069c067c006a140000000000000000a4018e015300
+               299           0 RESUME                   0
                
-               297           2 LOAD_FAST                0 (self)
+               300           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (getters)
                             14 STORE_FAST               2 (getters)
                
-               298          16 LOAD_FAST                0 (self)
+               301          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (model)
                             28 STORE_FAST               3 (model)
                
-               299          30 LOAD_FAST                0 (self)
+               302          30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                2 (inline)
                             42 STORE_FAST               4 (inline)
                
-               301          44 LOAD_GLOBAL              7 (NULL + isinstance)
+               304          44 LOAD_GLOBAL              7 (NULL + isinstance)
                             56 LOAD_FAST                3 (model)
                             58 LOAD_GLOBAL              8 (FilterExpression)
                             70 PRECALL                  2
                             74 CALL                     2
                             84 POP_JUMP_FORWARD_IF_FALSE    21 (to 128)
                
-               302          86 LOAD_FAST                3 (model)
+               305          86 LOAD_FAST                3 (model)
                             88 LOAD_METHOD              5 (resolve)
                            110 LOAD_FAST                1 (context)
                            112 PRECALL                  1
                            116 CALL                     1
                            126 STORE_FAST               3 (model)
                
-               304     >>  128 LOAD_GLOBAL              7 (NULL + isinstance)
+               307     >>  128 LOAD_GLOBAL              7 (NULL + isinstance)
                            140 LOAD_FAST                4 (inline)
                            142 LOAD_GLOBAL              8 (FilterExpression)
                            154 PRECALL                  2
                            158 CALL                     2
                            168 POP_JUMP_FORWARD_IF_FALSE    21 (to 212)
                
-               305         170 LOAD_FAST                4 (inline)
+               308         170 LOAD_FAST                4 (inline)
                            172 LOAD_METHOD              5 (resolve)
                            194 LOAD_FAST                1 (context)
                            196 PRECALL                  1
                            200 CALL                     1
                            210 STORE_FAST               4 (inline)
                
-               307     >>  212 LOAD_FAST                3 (model)
+               310     >>  212 LOAD_FAST                3 (model)
                            214 STORE_FAST               5 (obj)
                
-               308         216 LOAD_GLOBAL             13 (NULL + range)
+               311         216 LOAD_GLOBAL             13 (NULL + range)
                            228 LOAD_GLOBAL             15 (NULL + len)
                            240 LOAD_FAST                2 (getters)
                            242 PRECALL                  1
                            246 CALL                     1
                            256 LOAD_CONST               1 (1)
                            258 BINARY_OP               10 (-)
                            262 PRECALL                  1
                            266 CALL                     1
                            276 GET_ITER
                        >>  278 FOR_ITER                72 (to 424)
                            280 STORE_FAST               6 (i)
                
-               309         282 LOAD_FAST                2 (getters)
+               312         282 LOAD_FAST                2 (getters)
                            284 LOAD_FAST                6 (i)
                            286 BINARY_SUBSCR
                            296 STORE_FAST               7 (getter)
                
-               310         298 NOP
+               313         298 NOP
                
-               311         300 LOAD_GLOBAL             17 (NULL + getattr)
+               314         300 LOAD_GLOBAL             17 (NULL + getattr)
                            312 LOAD_FAST                5 (obj)
                            314 LOAD_FAST                7 (getter)
                            316 PRECALL                  2
                            320 CALL                     2
                            330 STORE_FAST               5 (obj)
                            332 JUMP_BACKWARD           28 (to 278)
                        >>  334 PUSH_EXC_INFO
                
-               312         336 LOAD_GLOBAL             18 (AttributeError)
+               315         336 LOAD_GLOBAL             18 (AttributeError)
                            348 CHECK_EXC_MATCH
                            350 POP_JUMP_FORWARD_IF_FALSE    32 (to 416)
                            352 POP_TOP
                
-               313         354 LOAD_GLOBAL             19 (NULL + AttributeError)
+               316         354 LOAD_GLOBAL             19 (NULL + AttributeError)
                            366 LOAD_CONST               2 ('Object ')
                            368 LOAD_FAST                3 (model)
                            370 LOAD_ATTR               10 (__class__)
                            380 LOAD_ATTR               11 (__name__)
                            390 FORMAT_VALUE             0
                            392 LOAD_CONST               3 (' does not have attribute ')
                            394 LOAD_FAST                7 (getter)
                            396 FORMAT_VALUE             0
                            398 BUILD_STRING             4
                            400 PRECALL                  1
                            404 CALL                     1
                            414 RAISE_VARARGS            1
                
-               312     >>  416 RERAISE                  0
+               315     >>  416 RERAISE                  0
                        >>  418 COPY                     3
                            420 POP_EXCEPT
                            422 RERAISE                  1
                
-               315     >>  424 LOAD_FAST                1 (context)
+               318     >>  424 LOAD_FAST                1 (context)
                            426 LOAD_METHOD             12 (get)
                            448 LOAD_CONST               4 ('request')
                            450 PRECALL                  1
                            454 CALL                     1
                            464 STORE_FAST               8 (request)
                
-               316         466 LOAD_GLOBAL             27 (NULL + get_field_content)
+               319         466 LOAD_GLOBAL             27 (NULL + get_field_content)
                
-               317         478 LOAD_FAST                8 (request)
+               320         478 LOAD_FAST                8 (request)
                
-               318         480 LOAD_FAST                5 (obj)
+               321         480 LOAD_FAST                5 (obj)
                
-               319         482 LOAD_FAST                5 (obj)
+               322         482 LOAD_FAST                5 (obj)
                            484 LOAD_ATTR               14 (_meta)
                            494 LOAD_METHOD             15 (get_field)
                            516 LOAD_FAST                0 (self)
                            518 LOAD_ATTR               16 (field)
                            528 PRECALL                  1
                            532 CALL                     1
                
-               320         542 LOAD_FAST                1 (context)
+               323         542 LOAD_FAST                1 (context)
                
-               316         544 PRECALL                  4
+               319         544 PRECALL                  4
                            548 CALL                     4
                            558 STORE_FAST               9 (content)
                
-               323         560 LOAD_GLOBAL             35 (NULL + _can_edit)
-                           572 LOAD_FAST                8 (request)
-                           574 LOAD_FAST                5 (obj)
-                           576 PRECALL                  2
-                           580 CALL                     2
-                           590 POP_JUMP_FORWARD_IF_TRUE     2 (to 596)
+               326         560 LOAD_FAST                9 (content)
+                           562 POP_JUMP_FORWARD_IF_TRUE    15 (to 594)
+               
+               327         564 LOAD_GLOBAL             35 (NULL + mark_safe)
+                           576 LOAD_CONST               5 ('')
+                           578 PRECALL                  1
+                           582 CALL                     1
+                           592 STORE_FAST               9 (content)
+               
+               329     >>  594 LOAD_GLOBAL             37 (NULL + _can_edit)
+                           606 LOAD_FAST                8 (request)
+                           608 LOAD_FAST                5 (obj)
+                           610 PRECALL                  2
+                           614 CALL                     2
+                           624 POP_JUMP_FORWARD_IF_TRUE     2 (to 630)
                
-               324         592 LOAD_FAST                9 (content)
-                           594 RETURN_VALUE
+               330         626 LOAD_FAST                9 (content)
+                           628 RETURN_VALUE
                
-               326     >>  596 LOAD_GLOBAL             37 (NULL + render_editable_field)
-                           608 LOAD_CONST               6 (())
+               332     >>  630 LOAD_GLOBAL             39 (NULL + render_editable_field)
+                           642 LOAD_CONST               7 (())
                
-               327         610 LOAD_FAST                8 (request)
+               333         644 LOAD_FAST                8 (request)
                
-               328         612 LOAD_FAST                9 (content)
+               334         646 LOAD_FAST                9 (content)
                
-               329         614 LOAD_FAST                0 (self)
-                           616 LOAD_ATTR               16 (field)
+               335         648 LOAD_FAST                0 (self)
+                           650 LOAD_ATTR               16 (field)
                
-               330         626 LOAD_FAST                5 (obj)
+               336         660 LOAD_FAST                5 (obj)
                
-               331         628 LOAD_FAST                1 (context)
+               337         662 LOAD_FAST                1 (context)
                
-               332         630 LOAD_FAST                4 (inline)
+               338         664 LOAD_FAST                4 (inline)
                
-               326         632 LOAD_CONST               5 (('request', 'content', 'field_name', 'model', 'context', 'inline'))
-                           634 BUILD_CONST_KEY_MAP      6
+               332         666 LOAD_CONST               6 (('request', 'content', 'field_name', 'model', 'context', 'inline'))
+                           668 BUILD_CONST_KEY_MAP      6
                
-               333         636 LOAD_FAST                0 (self)
-                           638 LOAD_ATTR               19 (kwargs)
+               339         670 LOAD_FAST                0 (self)
+                           672 LOAD_ATTR               20 (kwargs)
                
-               326         648 DICT_MERGE               1
-                           650 CALL_FUNCTION_EX         1
-                           652 RETURN_VALUE
+               332         682 DICT_MERGE               1
+                           684 CALL_FUNCTION_EX         1
+                           686 RETURN_VALUE
                ExceptionTable:
                  300 to 330 -> 334 [1]
                  334 to 416 -> 418 [2] lasti
                consts
                   None
                   1
                   'Object '
                   ' does not have attribute '
                   'request'
+                  ''
                   ('request', 'content', 'field_name', 'model', 'context', 'inline')
                   ()
-               names      ('getters', 'model', 'inline', 'isinstance', 'FilterExpression', 'resolve', 'range', 'len', 'getattr', 'AttributeError', '__class__', '__name__', 'get', 'get_field_content', '_meta', 'get_field', 'field', '_can_edit', 'render_editable_field', 'kwargs')
+               names      ('getters', 'model', 'inline', 'isinstance', 'FilterExpression', 'resolve', 'range', 'len', 'getattr', 'AttributeError', '__class__', '__name__', 'get', 'get_field_content', '_meta', 'get_field', 'field', 'mark_safe', '_can_edit', 'render_editable_field', 'kwargs')
                varnames   ('self', 'context', 'getters', 'model', 'inline', 'obj', 'i', 'getter', 'request', 'content')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 296
+               firstlineno 299
                lnotab
                   0x02010e010e010e022a012a022a012a020401420110010201240112013e
-                  ff08032a010c01020102013c0102fc1007200104020e01020102010c0102
-                  01020102fa04070cf9
+                  ff08032a010c01020102013c0102fc100704011e02200104020e01020102
+                  010c010201020102fa04070cf9
             None
             (False,)
          names      ('__name__', '__module__', '__qualname__', 'models', 'Model', 'list', 'str', 'bool', '__init__', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'FieldEditNode'
-         firstlineno 288
+         firstlineno 291
          lnotab 0x0a012c07
       'FieldEditNode'
       'fedit_field'
       code
          argcount  : 2
          nlocals   : 9
          stacksize : 6
@@ -1949,101 +1973,101 @@
             0000000000000000006404a6010000ab01000000000000000082017c00a0
             0500000000000000000000000000000000000000007c05a0010000000000
             0000000000000000000000000000006401a6010000ab0100000000000000
             00a6010000ab0100000000000000007d067c027215640567017d07740d00
             0000000000000000007c007c077c02a6030000ab0300000000000000007d
             086e0269007d08740f0000000000000000000064077c067c0564069c027c
             08a4018e015300
-         338           0 RESUME                   0
+         344           0 RESUME                   0
          
-         353           2 LOAD_FAST                1 (token)
+         359           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         354          42 LOAD_FAST                2 (tokens)
+         360          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         355          84 LOAD_FAST                2 (tokens)
+         361          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (model__field)
          
-         356         126 LOAD_FAST                4 (model__field)
+         362         126 LOAD_FAST                4 (model__field)
                      128 LOAD_METHOD              2 (split)
                      150 LOAD_CONST               2 ('.')
                      152 PRECALL                  1
                      156 CALL                     1
                      166 STORE_FAST               5 (model_tokens)
          
-         358         168 LOAD_GLOBAL              7 (NULL + len)
+         364         168 LOAD_GLOBAL              7 (NULL + len)
                      180 LOAD_FAST                5 (model_tokens)
                      182 PRECALL                  1
                      186 CALL                     1
                      196 LOAD_CONST               3 (2)
                      198 COMPARE_OP               0 (<)
                      204 POP_JUMP_FORWARD_IF_FALSE    15 (to 236)
          
-         359         206 LOAD_GLOBAL              9 (NULL + ValueError)
+         365         206 LOAD_GLOBAL              9 (NULL + ValueError)
                      218 LOAD_CONST               4 ('Model and field name are required')
                      220 PRECALL                  1
                      224 CALL                     1
                      234 RAISE_VARARGS            1
          
-         363     >>  236 LOAD_FAST                0 (parser)
+         369     >>  236 LOAD_FAST                0 (parser)
                      238 LOAD_METHOD              5 (compile_filter)
                      260 LOAD_FAST                5 (model_tokens)
                      262 LOAD_METHOD              1 (pop)
                      284 LOAD_CONST               1 (0)
                      286 PRECALL                  1
                      290 CALL                     1
                      300 PRECALL                  1
                      304 CALL                     1
                      314 STORE_FAST               6 (model)
          
-         365         316 LOAD_FAST                2 (tokens)
+         371         316 LOAD_FAST                2 (tokens)
                      318 POP_JUMP_FORWARD_IF_FALSE    21 (to 362)
          
-         367         320 LOAD_CONST               5 ('inline')
+         373         320 LOAD_CONST               5 ('inline')
          
-         366         322 BUILD_LIST               1
+         372         322 BUILD_LIST               1
                      324 STORE_FAST               7 (kwargs_names)
          
-         370         326 LOAD_GLOBAL             13 (NULL + get_kwargs)
+         376         326 LOAD_GLOBAL             13 (NULL + get_kwargs)
                      338 LOAD_FAST                0 (parser)
                      340 LOAD_FAST                7 (kwargs_names)
                      342 LOAD_FAST                2 (tokens)
                      344 PRECALL                  3
                      348 CALL                     3
                      358 STORE_FAST               8 (kwargs)
                      360 JUMP_FORWARD             2 (to 366)
          
-         372     >>  362 BUILD_MAP                0
+         378     >>  362 BUILD_MAP                0
                      364 STORE_FAST               8 (kwargs)
          
-         374     >>  366 LOAD_GLOBAL             15 (NULL + FieldEditNode)
+         380     >>  366 LOAD_GLOBAL             15 (NULL + FieldEditNode)
                      378 LOAD_CONST               7 (())
          
-         375         380 LOAD_FAST                6 (model)
+         381         380 LOAD_FAST                6 (model)
          
-         376         382 LOAD_FAST                5 (model_tokens)
+         382         382 LOAD_FAST                5 (model_tokens)
          
-         374         384 LOAD_CONST               6 (('model', 'getters'))
+         380         384 LOAD_CONST               6 (('model', 'getters'))
                      386 BUILD_CONST_KEY_MAP      2
          
-         377         388 LOAD_FAST                8 (kwargs)
+         383         388 LOAD_FAST                8 (kwargs)
          
-         374         390 DICT_MERGE               1
+         380         390 DICT_MERGE               1
                      392 CALL_FUNCTION_EX         1
                      394 RETURN_VALUE
          consts
             '\n    This tag is used to render an editable field.\n\n    This field will be wrapped and is able to be edited by the user on the frontend.\n\n    Usage example:\n        ```python\n        {% fedit_field mymodel.myfield inline=(default: False) key1=value1 key2=value2 %}\n        ```\n\n    Optionally your model can define a `render_fedit_{field_name}` method that will be used to render the field.\n    This will allow you to use custom rendering logic if need be.\n    '
             0
             '.'
             2
@@ -2051,17 +2075,17 @@
             'inline'
             ('model', 'getters')
             ()
          names      ('split_contents', 'pop', 'split', 'len', 'ValueError', 'compile_filter', 'get_kwargs', 'FieldEditNode')
          varnames   ('parser', 'token', 'tokens', '_', 'model__field', 'model_tokens', 'model', 'kwargs_names', 'kwargs')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_field'
-         firstlineno 338
+         firstlineno 344
          lnotab
             0x020f28012a012a012a0226011e045002040202ff0404240204020e0102
             0102fe040302fd
       code
          argcount  : 5
          nlocals   : 10
          stacksize : 10
@@ -2085,120 +2109,120 @@
             00a6010000ab010000000000000000a01000000000000000000000000000
             00000000000000a6000000ab000000000000000000640a6b02000000007c
             0564083c000000742300000000000000000000640b7c067c027c037c017c
             047c08640c9c067c05a5018900ac0da6030000ab03000000000000000053
             00
                        0 MAKE_CELL                0 (request)
          
-         381           2 RESUME                   0
+         387           2 RESUME                   0
          
-         382           4 LOAD_GLOBAL              1 (NULL + reverse)
+         388           4 LOAD_GLOBAL              1 (NULL + reverse)
          
-         383          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
+         389          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
          
-         384          18 LOAD_FAST                2 (field_name)
+         390          18 LOAD_FAST                2 (field_name)
                       20 LOAD_FAST                3 (model)
                       22 LOAD_ATTR                1 (_meta)
                       32 LOAD_ATTR                2 (app_label)
                       42 LOAD_FAST                3 (model)
                       44 LOAD_ATTR                1 (_meta)
                       54 LOAD_ATTR                3 (model_name)
                       64 LOAD_FAST                3 (model)
                       66 LOAD_ATTR                4 (pk)
                       76 BUILD_LIST               4
          
-         382          78 KW_NAMES                 2
+         388          78 KW_NAMES                 2
                       80 PRECALL                  2
                       84 CALL                     2
                       94 STORE_FAST               6 (edit_url)
          
-         387          96 LOAD_FAST                5 (kwargs)
+         393          96 LOAD_FAST                5 (kwargs)
                       98 POP_JUMP_FORWARD_IF_FALSE    37 (to 174)
          
-         388         100 LOAD_GLOBAL             11 (NULL + urlencode)
+         394         100 LOAD_GLOBAL             11 (NULL + urlencode)
          
-         389         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+         395         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                      124 LOAD_ATTR                7 (pack)
                      134 LOAD_CONST              14 (())
                      136 BUILD_MAP                0
                      138 LOAD_FAST                5 (kwargs)
                      140 DICT_MERGE               1
                      142 CALL_FUNCTION_EX         1
          
-         388         144 PRECALL                  1
+         394         144 PRECALL                  1
                      148 CALL                     1
                      158 STORE_FAST               7 (packed)
          
-         391         160 LOAD_FAST                6 (edit_url)
+         397         160 LOAD_FAST                6 (edit_url)
                      162 FORMAT_VALUE             0
                      164 LOAD_CONST               3 ('?')
                      166 LOAD_FAST                7 (packed)
                      168 FORMAT_VALUE             0
                      170 BUILD_STRING             3
                      172 STORE_FAST               6 (edit_url)
          
-         394     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
+         400     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
                      186 PRECALL                  0
                      190 CALL                     0
          
-         393         200 BUILD_LIST               1
+         399         200 BUILD_LIST               1
                      202 STORE_FAST               8 (items)
          
-         397         204 LOAD_GLOBAL             19 (NULL + hooks)
+         403         204 LOAD_GLOBAL             19 (NULL + hooks)
                      216 LOAD_ATTR               10 (get_hooks)
                      226 LOAD_GLOBAL             22 (CONSTRUCT_FIELD_TOOLBAR)
                      238 PRECALL                  1
                      242 CALL                     1
                      252 GET_ITER
                  >>  254 FOR_ITER                17 (to 290)
                      256 STORE_FAST               9 (hook)
          
-         398         258 PUSH_NULL
+         404         258 PUSH_NULL
                      260 LOAD_FAST                9 (hook)
                      262 LOAD_DEREF               0 (request)
                      264 LOAD_FAST                8 (items)
                      266 LOAD_FAST                3 (model)
                      268 LOAD_FAST                2 (field_name)
                      270 KW_NAMES                 4
                      272 PRECALL                  4
                      276 CALL                     4
                      286 POP_TOP
                      288 JUMP_BACKWARD           18 (to 254)
          
-         400     >>  290 LOAD_CLOSURE             0 (request)
+         406     >>  290 LOAD_CLOSURE             0 (request)
                      292 BUILD_TUPLE              1
-                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 400>)
+                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 406>)
                      296 MAKE_FUNCTION            8 (closure)
                      298 LOAD_FAST                8 (items)
                      300 GET_ITER
                      302 PRECALL                  0
                      306 CALL                     0
                      316 STORE_FAST               8 (items)
          
-         401         318 LOAD_GLOBAL             25 (NULL + list)
+         407         318 LOAD_GLOBAL             25 (NULL + list)
                      330 LOAD_GLOBAL             27 (NULL + filter)
                      342 LOAD_CONST               0 (None)
                      344 LOAD_FAST                8 (items)
                      346 PRECALL                  2
                      350 CALL                     2
                      360 PRECALL                  1
                      364 CALL                     1
                      374 STORE_FAST               8 (items)
          
-         403         376 LOAD_FAST                2 (field_name)
+         409         376 LOAD_FAST                2 (field_name)
                      378 LOAD_FAST                5 (kwargs)
                      380 LOAD_CONST               6 ('wagtail_fedit_field_name')
                      382 STORE_SUBSCR
          
-         404         386 LOAD_FAST                3 (model)
+         410         386 LOAD_FAST                3 (model)
                      388 LOAD_FAST                5 (kwargs)
                      390 LOAD_CONST               7 ('wagtail_fedit_instance')
                      392 STORE_SUBSCR
          
-         405         396 LOAD_GLOBAL             29 (NULL + str)
+         411         396 LOAD_GLOBAL             29 (NULL + str)
                      408 LOAD_FAST                5 (kwargs)
                      410 LOAD_METHOD             15 (get)
                      432 LOAD_CONST               8 ('inline')
                      434 LOAD_CONST               9 (False)
                      436 PRECALL                  2
                      440 CALL                     2
                      450 PRECALL                  1
@@ -2208,40 +2232,40 @@
                      490 CALL                     0
                      500 LOAD_CONST              10 ('true')
                      502 COMPARE_OP               2 (==)
                      508 LOAD_FAST                5 (kwargs)
                      510 LOAD_CONST               8 ('inline')
                      512 STORE_SUBSCR
          
-         406         516 LOAD_GLOBAL             35 (NULL + render_to_string)
+         412         516 LOAD_GLOBAL             35 (NULL + render_to_string)
          
-         407         528 LOAD_CONST              11 ('wagtail_fedit/content/editable_field.html')
+         413         528 LOAD_CONST              11 ('wagtail_fedit/content/editable_field.html')
          
-         409         530 LOAD_FAST                6 (edit_url)
+         415         530 LOAD_FAST                6 (edit_url)
          
-         410         532 LOAD_FAST                2 (field_name)
+         416         532 LOAD_FAST                2 (field_name)
          
-         411         534 LOAD_FAST                3 (model)
+         417         534 LOAD_FAST                3 (model)
          
-         412         536 LOAD_FAST                1 (content)
+         418         536 LOAD_FAST                1 (content)
          
-         413         538 LOAD_FAST                4 (context)
+         419         538 LOAD_FAST                4 (context)
          
-         414         540 LOAD_FAST                8 (items)
+         420         540 LOAD_FAST                8 (items)
          
-         408         542 LOAD_CONST              12 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
+         414         542 LOAD_CONST              12 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
                      544 BUILD_CONST_KEY_MAP      6
          
-         415         546 LOAD_FAST                5 (kwargs)
+         421         546 LOAD_FAST                5 (kwargs)
          
-         408         548 DICT_UPDATE              1
+         414         548 DICT_UPDATE              1
          
-         417         550 LOAD_DEREF               0 (request)
+         423         550 LOAD_DEREF               0 (request)
          
-         406         552 KW_NAMES                13
+         412         552 KW_NAMES                13
                      554 PRECALL                  3
                      558 CALL                     3
                      568 RETURN_VALUE
          consts
             None
             'wagtail_fedit:edit_field'
             ('args',)
@@ -2253,15 +2277,15 @@
                stacksize : 5
                flags     : 19
                code
                   0x9501970067007c005d177d017c01a00000000000000000000000000000
                   000000000000008902a6010000ab01000000000000000091028c185300
                              0 COPY_FREE_VARS           1
                
-               400           2 RESUME                   0
+               406           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                23 (to 56)
                             10 STORE_FAST               1 (item)
                             12 LOAD_FAST                1 (item)
                             14 LOAD_METHOD              0 (render)
                             36 LOAD_DEREF               2 (request)
@@ -2271,34 +2295,34 @@
                             54 JUMP_BACKWARD           24 (to 8)
                        >>   56 RETURN_VALUE
                consts
                names      ('render',)
                varnames   ('.0', 'item')
                freevars   ('request',)
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '<listcomp>'
-               firstlineno 400
+               firstlineno 406
                lnotab 0x
             'wagtail_fedit_field_name'
             'wagtail_fedit_instance'
             'inline'
             False
             'true'
             'wagtail_fedit/content/editable_field.html'
             ('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items')
             ('request',)
             ()
          names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack', 'FeditFieldEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_FIELD_TOOLBAR', 'list', 'filter', 'str', 'get', 'lower', 'render_to_string')
          varnames   ('request', 'content', 'field_name', 'model', 'context', 'kwargs', 'edit_url', 'packed', 'items', 'hook')
          freevars   ()
          cellvars   ('request',)
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_editable_field'
-         firstlineno 381
+         firstlineno 387
          lnotab
             0x04010c0102013cfe120504010c0120ff10030e031aff0404360120021c
             013a020a010a0178010c0102020201020102010201020102fa040702f902
             0902f5
       'kwarg_list'
       'tokens'
       'return'
@@ -2315,105 +2339,105 @@
             0064036b020000000072307c03720f7407000000000000000000006404a6
             010000ab01000000000000000082017c00a0040000000000000000000000
             0000000000000000007c06a6010000ab0100000000000000007c047c017c
             05190000000000000000003c0000008c5d7c076405190000000000000000
             007d087c00a00400000000000000000000000000000000000000007c0764
             0319000000000000000000a6010000ab0100000000000000007c047c083c
             00000064067d038c867c045300
-         420           0 RESUME                   0
+         426           0 RESUME                   0
          
-         421           2 LOAD_CONST               1 (False)
+         427           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               3 (had_kwargs)
          
-         422           6 BUILD_MAP                0
+         428           6 BUILD_MAP                0
                        8 STORE_FAST               4 (kwargs)
          
-         427          10 LOAD_GLOBAL              1 (NULL + enumerate)
+         433          10 LOAD_GLOBAL              1 (NULL + enumerate)
                       22 LOAD_FAST                2 (tokens)
                       24 PRECALL                  1
                       28 CALL                     1
                       38 GET_ITER
                  >>   40 FOR_ITER               133 (to 308)
                       42 UNPACK_SEQUENCE          2
                       46 STORE_FAST               5 (i)
                       48 STORE_FAST               6 (token)
          
-         428          50 LOAD_FAST                6 (token)
+         434          50 LOAD_FAST                6 (token)
                       52 LOAD_METHOD              1 (split)
                       74 LOAD_CONST               2 ('=')
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               7 (split)
          
-         429          92 LOAD_GLOBAL              5 (NULL + len)
+         435          92 LOAD_GLOBAL              5 (NULL + len)
                      104 LOAD_FAST                7 (split)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               3 (1)
                      122 COMPARE_OP               2 (==)
                      128 POP_JUMP_FORWARD_IF_FALSE    48 (to 226)
          
-         430         130 LOAD_FAST                3 (had_kwargs)
+         436         130 LOAD_FAST                3 (had_kwargs)
                      132 POP_JUMP_FORWARD_IF_FALSE    15 (to 164)
          
-         431         134 LOAD_GLOBAL              7 (NULL + ValueError)
+         437         134 LOAD_GLOBAL              7 (NULL + ValueError)
                      146 LOAD_CONST               4 ('Unexpected positional argument after keyword argument')
                      148 PRECALL                  1
                      152 CALL                     1
                      162 RAISE_VARARGS            1
          
-         433     >>  164 LOAD_FAST                0 (parser)
+         439     >>  164 LOAD_FAST                0 (parser)
                      166 LOAD_METHOD              4 (compile_filter)
                      188 LOAD_FAST                6 (token)
                      190 PRECALL                  1
                      194 CALL                     1
                      204 LOAD_FAST                4 (kwargs)
                      206 LOAD_FAST                1 (kwarg_list)
                      208 LOAD_FAST                5 (i)
                      210 BINARY_SUBSCR
                      220 STORE_SUBSCR
                      224 JUMP_BACKWARD           93 (to 40)
          
-         435     >>  226 LOAD_FAST                7 (split)
+         441     >>  226 LOAD_FAST                7 (split)
                      228 LOAD_CONST               5 (0)
                      230 BINARY_SUBSCR
                      240 STORE_FAST               8 (key)
          
-         439         242 LOAD_FAST                0 (parser)
+         445         242 LOAD_FAST                0 (parser)
                      244 LOAD_METHOD              4 (compile_filter)
                      266 LOAD_FAST                7 (split)
                      268 LOAD_CONST               3 (1)
                      270 BINARY_SUBSCR
                      280 PRECALL                  1
                      284 CALL                     1
                      294 LOAD_FAST                4 (kwargs)
                      296 LOAD_FAST                8 (key)
                      298 STORE_SUBSCR
          
-         440         302 LOAD_CONST               6 (True)
+         446         302 LOAD_CONST               6 (True)
                      304 STORE_FAST               3 (had_kwargs)
                      306 JUMP_BACKWARD          134 (to 40)
          
-         442     >>  308 LOAD_FAST                4 (kwargs)
+         448     >>  308 LOAD_FAST                4 (kwargs)
                      310 RETURN_VALUE
          consts
             None
             False
             '='
             1
             'Unexpected positional argument after keyword argument'
             0
             True
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter')
          varnames   ('parser', 'kwarg_list', 'tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 420
+         firstlineno 426
          lnotab 0x02010401040528012a01260104011e023e0210043c010602
       'obj'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 5
          flags     : 3
@@ -2423,41 +2447,41 @@
             0000000000000000000000000000006402a6010000ab0100000000000000
             000c00704a7c006a000000000000000000a0020000000000000000000000
             0000000000000000007c016a0300000000000000006a0400000000000000
             009b0064037c016a0300000000000000006a0500000000000000009b009d
             03a6010000ab0100000000000000000c007016740d000000000000000000
             007c00740e000000000000000000006401a6030000ab0300000000000000
             000c000c005300
-         445           0 RESUME                   0
+         451           0 RESUME                   0
          
-         446           2 LOAD_FAST                0 (request)
+         452           2 LOAD_FAST                0 (request)
                        4 POP_JUMP_FORWARD_IF_FALSE     2 (to 10)
                        6 LOAD_FAST                1 (obj)
                        8 POP_JUMP_FORWARD_IF_TRUE     2 (to 14)
          
-         447     >>   10 LOAD_CONST               1 (False)
+         453     >>   10 LOAD_CONST               1 (False)
                       12 RETURN_VALUE
          
-         450     >>   14 LOAD_FAST                0 (request)
+         456     >>   14 LOAD_FAST                0 (request)
                       16 LOAD_ATTR                0 (user)
                       26 LOAD_ATTR                1 (is_authenticated)
                       36 UNARY_NOT
                       38 JUMP_IF_TRUE_OR_POP    101 (to 242)
          
-         451          40 LOAD_FAST                0 (request)
+         457          40 LOAD_FAST                0 (request)
                       42 LOAD_ATTR                0 (user)
                       52 LOAD_METHOD              2 (has_perm)
                       74 LOAD_CONST               2 ('wagtailadmin.access_admin')
                       76 PRECALL                  1
                       80 CALL                     1
                       90 UNARY_NOT
          
-         450          92 JUMP_IF_TRUE_OR_POP     74 (to 242)
+         456          92 JUMP_IF_TRUE_OR_POP     74 (to 242)
          
-         452          94 LOAD_FAST                0 (request)
+         458          94 LOAD_FAST                0 (request)
                       96 LOAD_ATTR                0 (user)
                      106 LOAD_METHOD              2 (has_perm)
                      128 LOAD_FAST                1 (obj)
                      130 LOAD_ATTR                3 (_meta)
                      140 LOAD_ATTR                4 (app_label)
                      150 FORMAT_VALUE             0
                      152 LOAD_CONST               3 ('.change_')
@@ -2466,96 +2490,96 @@
                      166 LOAD_ATTR                5 (model_name)
                      176 FORMAT_VALUE             0
                      178 BUILD_STRING             3
                      180 PRECALL                  1
                      184 CALL                     1
                      194 UNARY_NOT
          
-         450         196 JUMP_IF_TRUE_OR_POP     22 (to 242)
+         456         196 JUMP_IF_TRUE_OR_POP     22 (to 242)
          
-         453         198 LOAD_GLOBAL             13 (NULL + getattr)
+         459         198 LOAD_GLOBAL             13 (NULL + getattr)
                      210 LOAD_FAST                0 (request)
                      212 LOAD_GLOBAL             14 (FEDIT_PREVIEW_VAR)
                      224 LOAD_CONST               1 (False)
                      226 PRECALL                  3
                      230 CALL                     3
                      240 UNARY_NOT
          
-         449     >>  242 UNARY_NOT
+         455     >>  242 UNARY_NOT
                      244 RETURN_VALUE
          consts
             None
             False
             'wagtailadmin.access_admin'
             '.change_'
          names      ('user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'getattr', 'FEDIT_PREVIEW_VAR')
          varnames   ('request', 'obj')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       '_can_edit'
-         firstlineno 445
+         firstlineno 451
          lnotab 0x0201080104031a0134ff020266fe02032cfc
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 5
          flags     : 15
          code
             0x97007c017c00760072087c007c01190000000000000000005300740100
             0000000000000000007c02a6010000ab010000000000000000720802007c
             027c0369007c04a4018e017d027c027c007c013c0000007c025300
-         457           0 RESUME                   0
+         463           0 RESUME                   0
          
-         458           2 LOAD_FAST                1 (key)
+         464           2 LOAD_FAST                1 (key)
                        4 LOAD_FAST                0 (context)
                        6 CONTAINS_OP              0
                        8 POP_JUMP_FORWARD_IF_FALSE     8 (to 26)
          
-         459          10 LOAD_FAST                0 (context)
+         465          10 LOAD_FAST                0 (context)
                       12 LOAD_FAST                1 (key)
                       14 BINARY_SUBSCR
                       24 RETURN_VALUE
          
-         461     >>   26 LOAD_GLOBAL              1 (NULL + callable)
+         467     >>   26 LOAD_GLOBAL              1 (NULL + callable)
                       38 LOAD_FAST                2 (value)
                       40 PRECALL                  1
                       44 CALL                     1
                       54 POP_JUMP_FORWARD_IF_FALSE     8 (to 72)
          
-         462          56 PUSH_NULL
+         468          56 PUSH_NULL
                       58 LOAD_FAST                2 (value)
                       60 LOAD_FAST                3 (args)
                       62 BUILD_MAP                0
                       64 LOAD_FAST                4 (kwargs)
                       66 DICT_MERGE               1
                       68 CALL_FUNCTION_EX         1
                       70 STORE_FAST               2 (value)
          
-         464     >>   72 LOAD_FAST                2 (value)
+         470     >>   72 LOAD_FAST                2 (value)
                       74 LOAD_FAST                0 (context)
                       76 LOAD_FAST                1 (key)
                       78 STORE_SUBSCR
          
-         465          82 LOAD_FAST                2 (value)
+         471          82 LOAD_FAST                2 (value)
                       84 RETURN_VALUE
          consts
             None
          names      ('callable',)
          varnames   ('context', 'key', 'value', 'args', 'kwargs')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       '_get_from_context_or_set'
-         firstlineno 457
+         firstlineno 463
          lnotab 0x0201080110021e0110020a01
    names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail.models', 'Page', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'warnings', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'utils', 'FEDIT_PREVIEW_VAR', 'get_field_content', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'FieldEditNode', 'do_render_fedit_field', 'render_editable_field', 'list', 'str', 'dict', 'get_kwargs', 'Model', '_can_edit', '_get_from_context_or_set')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020114010c0110010c010c010c010c010c020c010c010c010c0208
-      021004100110061e011e03040104031c7f00412a010eff0e01023b1c322a
+      021004100110061e011e03040104031c7f00442a010eff0e01023b1c352a
       010eff0e01022a06273019160c
```

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.4.2/wagtail_fedit/templatetags/fedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,17 @@
         # Get block id from block if bound or context.
         if not block_id and "block_id" in context:
             block_id = context["block_id"]
         elif not block_id and block and hasattr(block, "id"):
             block_id = block.id
         elif not block_id:
             raise ValueError("Block ID is required")
+        
+        if not rendered:
+            rendered = mark_safe("")
 
         # Check if the user has permission to edit the block.
         request = context.get("request")
         if not _can_edit(request, model):
             return rendered
 
         # If the model is a page, we can redirect the user to the page editor.
@@ -316,14 +319,20 @@
         content = get_field_content(
             request,
             obj,
             obj._meta.get_field(self.field),
             context,
         )
 
+        if not content:
+            content = mark_safe("")
+            # Force inline editing if no content is available.
+            # This will make sure the height of the field to edit is not 0.
+            inline = True
+
         if not _can_edit(request, obj):
             return content
             
         return render_editable_field(
             request=request, 
             content=content,
             field_name=self.field,
```

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.4.2/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.4.2/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/urls.py` & `wagtail_fedit-1.4.2/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/utils.py` & `wagtail_fedit-1.4.2/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.4.2/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.4.2/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.4.2/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.4.2/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.4.2/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.4.2/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail_fedit
-Version: 1.4.1
+Name: wagtail-fedit
+Version: 1.4.2
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,20 +18,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=4.2
 
 wagtail_fedit
 =============
 
+![Wagtail FEdit Example](https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
+
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
 
 # Table of Contents
 
 - [Getting Started](#getting-started)
 - [Getting Editing!](#getting-editing)
 - [Permissions](#permissions)
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.1 Summary: An
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.2 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier:
 Topic :: Internet :: WWW/HTTP :: Dynamic Content Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-Django>=4.2 Requires-Dist: Wagtail>=4.2 wagtail_fedit ============= Wagtail
-FEdit is a library to allow your Wagtail pages and content-blocks to be edited
-on the frontend. # Table of Contents - [Getting Started](#getting-started) -
-[Getting Editing!](#getting-editing) - [Permissions](#permissions) -
+Description-Content-Type: text/markdown License-File: LICENSE wagtail_fedit
+============= ![Wagtail FEdit Example](https://github.com/Nigel2392/
+wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
+Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be
+edited on the frontend. # Table of Contents - [Getting Started](#getting-
+started) - [Getting Editing!](#getting-editing) - [Permissions](#permissions) -
 [Revisions](#revisions) - [Workflows](#workflows) - [Logs](#logs) - [Caveats]
 (#caveats) - [Hooks](#hooks) - [Construct Block Toolbar]
 (#wagtail_feditconstruct_block_toolbar) - [Construct Field Toolbar]
 (#wagtail_feditconstruct_field_toolbar) - [Register Type Renderer]
 (#wagtail_feditregister_type_renderer) - [Register Field Renderer]
 (#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
```

### Comparing `wagtail_fedit-1.4.1/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.4.2/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
 wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
-wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
 wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
 wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
 wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
 wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
 wagtail_fedit/templatetags/__init__.py
```

