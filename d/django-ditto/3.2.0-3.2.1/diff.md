# Comparing `tmp/django-ditto-3.2.0.tar.gz` & `tmp/django-ditto-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ditto-3.2.0.tar", last modified: Wed Dec 13 12:05:50 2023, max compression
+gzip compressed data, was "django-ditto-3.2.1.tar", last modified: Mon Apr  8 15:05:16 2024, max compression
```

## Comparing `django-ditto-3.2.0.tar` & `django-ditto-3.2.1.tar`

### file list

```diff
@@ -1,385 +1,385 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.649081 django-ditto-3.2.0/
--rw-r--r--   0 phil       (501) staff       (20)     1083 2021-10-22 16:10:52.000000 django-ditto-3.2.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      326 2022-03-25 12:40:03.000000 django-ditto-3.2.0/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)     3733 2023-12-13 12:05:50.648934 django-ditto-3.2.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     2282 2023-12-12 14:20:03.000000 django-ditto-3.2.0/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.583170 django-ditto-3.2.0/ditto/
--rw-r--r--   0 phil       (501) staff       (20)      196 2023-12-13 11:39:23.000000 django-ditto-3.2.0/ditto/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.585289 django-ditto-3.2.0/ditto/core/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:28.000000 django-ditto-3.2.0/ditto/core/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)      263 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/core/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      708 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/core/app_settings.py
--rw-r--r--   0 phil       (501) staff       (20)     1785 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/core/apps.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.578825 django-ditto-3.2.0/ditto/core/management/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.585738 django-ditto-3.2.0/ditto/core/management/commands/
--rw-r--r--   0 phil       (501) staff       (20)     1976 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/core/management/commands/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)      272 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/core/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.585969 django-ditto-3.2.0/ditto/core/migrations/
--rw-r--r--   0 phil       (501) staff       (20)        0 2020-05-23 15:29:03.000000 django-ditto-3.2.0/ditto/core/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     5446 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/core/models.py
--rw-r--r--   0 phil       (501) staff       (20)    11629 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/core/paginator.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.579003 django-ditto-3.2.0/ditto/core/static/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.579186 django-ditto-3.2.0/ditto/core/static/ditto-core/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.586936 django-ditto-3.2.0/ditto/core/static/ditto-core/css/
--rw-rw-r--   0 phil       (501) staff       (20)   162264 2022-07-19 15:13:44.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/css/bootstrap.min.css
--rw-rw-r--   0 phil       (501) staff       (20)   654593 2022-07-19 15:13:44.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/css/bootstrap.min.css.map
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.588466 django-ditto-3.2.0/ditto/core/static/ditto-core/img/
--rw-r--r--   0 phil       (501) staff       (20)      142 2016-09-06 12:05:37.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/img/default_avatar.png
--rw-r--r--   0 phil       (501) staff       (20)     3520 2016-09-06 12:05:37.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/img/original_error.jpg
--rw-r--r--   0 phil       (501) staff       (20)     3309 2016-09-06 12:05:37.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/img/original_missing.jpg
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.589636 django-ditto-3.2.0/ditto/core/static/ditto-core/js/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.591364 django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/
--rw-rw-r--   0 phil       (501) staff       (20)    20871 2022-07-19 15:13:44.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/carousel.js
--rw-rw-r--   0 phil       (501) staff       (20)    38793 2022-07-19 15:13:44.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/carousel.js.map
--rw-rw-r--   0 phil       (501) staff       (20)    13394 2022-07-19 15:13:44.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/collapse.js
--rw-rw-r--   0 phil       (501) staff       (20)    24048 2022-07-19 15:13:44.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/collapse.js.map
--rw-rw-r--   0 phil       (501) staff       (20)     6631 2022-07-19 15:13:44.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/util.js
--rw-rw-r--   0 phil       (501) staff       (20)    12040 2022-07-19 15:13:44.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/util.js.map
--rw-r--r--   0 phil       (501) staff       (20)    72380 2020-05-24 12:52:06.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.js
--rw-r--r--   0 phil       (501) staff       (20)   110382 2020-05-24 12:52:06.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.map
--rw-r--r--   0 phil       (501) staff       (20)    21233 2020-11-19 17:03:58.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/js/popper.min.js
--rw-r--r--   0 phil       (501) staff       (20)   117179 2018-04-16 15:41:13.000000 django-ditto-3.2.0/ditto/core/static/ditto-core/js/popper.min.js.map
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.579363 django-ditto-3.2.0/ditto/core/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.592544 django-ditto-3.2.0/ditto/core/templates/ditto/
--rw-r--r--   0 phil       (501) staff       (20)     2230 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/core/templates/ditto/archive_day.html
--rw-r--r--   0 phil       (501) staff       (20)     4738 2020-08-10 13:47:31.000000 django-ditto-3.2.0/ditto/core/templates/ditto/base.html
--rw-r--r--   0 phil       (501) staff       (20)     1029 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/core/templates/ditto/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.594378 django-ditto-3.2.0/ditto/core/templates/ditto/includes/
--rw-r--r--   0 phil       (501) staff       (20)      643 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/core/templates/ditto/includes/account_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1180 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/core/templates/ditto/includes/item_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1760 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/core/templates/ditto/includes/item_lists.html
--rw-r--r--   0 phil       (501) staff       (20)     1108 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/core/templates/ditto/includes/pager.html
--rw-r--r--   0 phil       (501) staff       (20)     2478 2017-08-22 13:41:35.000000 django-ditto-3.2.0/ditto/core/templates/ditto/includes/pagination.html
--rw-r--r--   0 phil       (501) staff       (20)     2272 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/core/templates/ditto/includes/variety_nav.html
--rw-r--r--   0 phil       (501) staff       (20)      681 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/core/templates/ditto/tag_detail.html
--rw-r--r--   0 phil       (501) staff       (20)      399 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/core/templates/ditto/tag_list.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.594594 django-ditto-3.2.0/ditto/core/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.2.0/ditto/core/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     5114 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/core/templatetags/ditto_core.py
--rw-r--r--   0 phil       (501) staff       (20)      620 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/core/urls.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.595084 django-ditto-3.2.0/ditto/core/utils/
--rw-r--r--   0 phil       (501) staff       (20)     3477 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/core/utils/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     3543 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/core/utils/downloader.py
--rw-r--r--   0 phil       (501) staff       (20)    23863 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/core/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.597655 django-ditto-3.2.0/ditto/flickr/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:33.000000 django-ditto-3.2.0/ditto/flickr/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    12121 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      444 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/app_settings.py
--rw-r--r--   0 phil       (501) staff       (20)      345 2021-04-07 17:01:46.000000 django-ditto-3.2.0/ditto/flickr/apps.py
--rw-r--r--   0 phil       (501) staff       (20)      845 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/checks.py
--rw-r--r--   0 phil       (501) staff       (20)     4051 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/factories.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.599026 django-ditto-3.2.0/ditto/flickr/fetch/
--rw-r--r--   0 phil       (501) staff       (20)       38 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/fetch/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    20401 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/fetch/fetchers.py
--rw-r--r--   0 phil       (501) staff       (20)     4752 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/fetch/filesfetchers.py
--rw-r--r--   0 phil       (501) staff       (20)     4604 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/fetch/multifetchers.py
--rw-r--r--   0 phil       (501) staff       (20)    16297 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/fetch/savers.py
--rw-r--r--   0 phil       (501) staff       (20)     3065 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/imagegenerators.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.579802 django-ditto-3.2.0/ditto/flickr/management/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.599811 django-ditto-3.2.0/ditto/flickr/management/commands/
--rw-r--r--   0 phil       (501) staff       (20)     2953 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/management/commands/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     2721 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/management/commands/fetch_flickr_account_user.py
--rw-r--r--   0 phil       (501) staff       (20)     1448 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/management/commands/fetch_flickr_originals.py
--rw-r--r--   0 phil       (501) staff       (20)     1451 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/management/commands/fetch_flickr_photos.py
--rw-r--r--   0 phil       (501) staff       (20)      866 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/management/commands/fetch_flickr_photosets.py
--rw-r--r--   0 phil       (501) staff       (20)     1927 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.605658 django-ditto-3.2.0/ditto/flickr/migrations/
--rw-r--r--   0 phil       (501) staff       (20)    23757 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0001_initial.py
--rw-r--r--   0 phil       (501) staff       (20)      426 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0002_auto_20160406_1548.py
--rw-r--r--   0 phil       (501) staff       (20)     1069 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0003_auto_20160413_0906.py
--rw-r--r--   0 phil       (501) staff       (20)     4134 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0004_auto_20160414_1120.py
--rw-r--r--   0 phil       (501) staff       (20)     7502 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0005_auto_20160414_1427.py
--rw-r--r--   0 phil       (501) staff       (20)      556 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/flickr/migrations/0006_auto_20160414_1459.py
--rw-r--r--   0 phil       (501) staff       (20)      703 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0007_auto_20160414_1637.py
--rw-r--r--   0 phil       (501) staff       (20)     4347 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0008_auto_20160429_1559.py
--rw-r--r--   0 phil       (501) staff       (20)      584 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/flickr/migrations/0009_photoset_fetch_time.py
--rw-r--r--   0 phil       (501) staff       (20)      463 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/flickr/migrations/0010_photo_photosets.py
--rw-r--r--   0 phil       (501) staff       (20)     1042 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0011_auto_20160502_1645.py
--rw-r--r--   0 phil       (501) staff       (20)     1205 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/flickr/migrations/0012_auto_20160503_1457.py
--rw-r--r--   0 phil       (501) staff       (20)      539 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/flickr/migrations/0013_photoset_photos_raw.py
--rw-r--r--   0 phil       (501) staff       (20)      569 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0014_photo_original_file.py
--rw-r--r--   0 phil       (501) staff       (20)      572 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0015_auto_20160514_1456.py
--rw-r--r--   0 phil       (501) staff       (20)      662 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0016_photo_video_original_file.py
--rw-r--r--   0 phil       (501) staff       (20)      856 2023-12-11 19:05:06.000000 django-ditto-3.2.0/ditto/flickr/migrations/0017_auto_20160524_1350.py
--rw-r--r--   0 phil       (501) staff       (20)      681 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/flickr/migrations/0018_auto_20160525_1011.py
--rw-r--r--   0 phil       (501) staff       (20)      585 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/flickr/migrations/0019_auto_20160713_1127.py
--rw-r--r--   0 phil       (501) staff       (20)      981 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/flickr/migrations/0020_auto_20161117_1622.py
--rw-r--r--   0 phil       (501) staff       (20)      941 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/flickr/migrations/0021_photo_post_year.py
--rw-r--r--   0 phil       (501) staff       (20)      979 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/flickr/migrations/0022_photo_taken_year.py
--rw-r--r--   0 phil       (501) staff       (20)      598 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0023_auto_20180104_1457.py
--rw-r--r--   0 phil       (501) staff       (20)     1708 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/migrations/0024_auto_20201119_1539.py
--rw-r--r--   0 phil       (501) staff       (20)     1908 2020-11-19 17:05:34.000000 django-ditto-3.2.0/ditto/flickr/migrations/0025_backfill_photo_sizes.py
--rw-r--r--   0 phil       (501) staff       (20)      983 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/migrations/0026_alter_taggedphoto_content_object_and_more.py
--rw-r--r--   0 phil       (501) staff       (20)      724 2022-03-24 08:27:58.000000 django-ditto-3.2.0/ditto/flickr/migrations/0027_alter_user_photos_url_alter_user_profile_url.py
--rw-r--r--   0 phil       (501) staff       (20)      418 2022-03-24 08:27:58.000000 django-ditto-3.2.0/ditto/flickr/migrations/0028_alter_user_iconfarm.py
--rw-r--r--   0 phil       (501) staff       (20)      533 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/migrations/0029_alter_user_options_alter_user_realname.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.2.0/ditto/flickr/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    32880 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/models.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.580013 django-ditto-3.2.0/ditto/flickr/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.607572 django-ditto-3.2.0/ditto/flickr/templates/flickr/
--rw-r--r--   0 phil       (501) staff       (20)      291 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/base.html
--rw-r--r--   0 phil       (501) staff       (20)     1686 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.608689 django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/
--rw-r--r--   0 phil       (501) staff       (20)      858 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/annual_photo_counts.html
--rw-r--r--   0 phil       (501) staff       (20)     1572 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/nav_tabs.html
--rw-r--r--   0 phil       (501) staff       (20)     1102 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/photo.html
--rw-r--r--   0 phil       (501) staff       (20)     2551 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/photo_columns.html
--rw-r--r--   0 phil       (501) staff       (20)      457 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/photoset_counts.html
--rw-r--r--   0 phil       (501) staff       (20)     1456 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/photoset_list.html
--rw-r--r--   0 phil       (501) staff       (20)      836 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/sorting.html
--rw-r--r--   0 phil       (501) staff       (20)     1896 2022-03-24 08:27:58.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/user.html
--rw-r--r--   0 phil       (501) staff       (20)    10445 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/photo_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     2615 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/photoset_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1560 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/photoset_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1781 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/tag_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1326 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/tag_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1194 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/user_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1167 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/user_photoset_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1966 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/flickr/templates/flickr/user_tag_detail.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.608995 django-ditto-3.2.0/ditto/flickr/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.2.0/ditto/flickr/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     3897 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/templatetags/ditto_flickr.py
--rw-r--r--   0 phil       (501) staff       (20)     1175 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/flickr/urls.py
--rw-r--r--   0 phil       (501) staff       (20)     9349 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/flickr/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.611562 django-ditto-3.2.0/ditto/lastfm/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:37.000000 django-ditto-3.2.0/ditto/lastfm/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     4354 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/lastfm/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      237 2021-04-07 17:01:57.000000 django-ditto-3.2.0/ditto/lastfm/apps.py
--rw-r--r--   0 phil       (501) staff       (20)     1590 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/lastfm/factories.py
--rw-r--r--   0 phil       (501) staff       (20)    11445 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/lastfm/fetch.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.580362 django-ditto-3.2.0/ditto/lastfm/management/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.612010 django-ditto-3.2.0/ditto/lastfm/management/commands/
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.2.0/ditto/lastfm/management/commands/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     1872 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/lastfm/management/commands/fetch_lastfm_scrobbles.py
--rw-r--r--   0 phil       (501) staff       (20)     5901 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/lastfm/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.614193 django-ditto-3.2.0/ditto/lastfm/migrations/
--rw-r--r--   0 phil       (501) staff       (20)    11231 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/lastfm/migrations/0001_initial.py
--rw-r--r--   0 phil       (501) staff       (20)      616 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/lastfm/migrations/0002_auto_20161012_1012.py
--rw-r--r--   0 phil       (501) staff       (20)     1536 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/lastfm/migrations/0003_auto_20161026_1539.py
--rw-r--r--   0 phil       (501) staff       (20)     2292 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/lastfm/migrations/0004_auto_20161026_1540.py
--rw-r--r--   0 phil       (501) staff       (20)      987 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/lastfm/migrations/0005_auto_20161117_1622.py
--rw-r--r--   0 phil       (501) staff       (20)      947 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/lastfm/migrations/0006_scrobble_post_year.py
--rw-r--r--   0 phil       (501) staff       (20)      669 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/lastfm/migrations/0007_set_post_year.py
--rw-r--r--   0 phil       (501) staff       (20)      607 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/lastfm/migrations/0008_auto_20180104_1457.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.2.0/ditto/lastfm/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    10986 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/lastfm/models.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.580597 django-ditto-3.2.0/ditto/lastfm/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.616618 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/
--rw-r--r--   0 phil       (501) staff       (20)     1755 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/album_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1187 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/album_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1286 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/artist_albums.html
--rw-r--r--   0 phil       (501) staff       (20)     1171 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/artist_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1191 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/artist_list.html
--rw-r--r--   0 phil       (501) staff       (20)      292 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/base.html
--rw-r--r--   0 phil       (501) staff       (20)     2006 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.618161 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/
--rw-r--r--   0 phil       (501) staff       (20)     1569 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/album_sidebar.html
--rw-r--r--   0 phil       (501) staff       (20)      891 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/annual_scrobble_counts.html
--rw-r--r--   0 phil       (501) staff       (20)     1718 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/artist_sidebar.html
--rw-r--r--   0 phil       (501) staff       (20)     3033 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/chart.html
--rw-r--r--   0 phil       (501) staff       (20)      729 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/day_filter.html
--rw-r--r--   0 phil       (501) staff       (20)      679 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/nav_tabs.html
--rw-r--r--   0 phil       (501) staff       (20)     2964 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/page_navigation.html
--rw-r--r--   0 phil       (501) staff       (20)     1338 2017-02-09 11:48:12.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/scrobble.html
--rw-r--r--   0 phil       (501) staff       (20)     1741 2017-02-09 11:48:12.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/scrobble_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1593 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/track_sidebar.html
--rw-r--r--   0 phil       (501) staff       (20)     1047 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/scrobble_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1485 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/track_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1187 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/track_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1341 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/user_album_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1345 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/user_artist_list.html
--rw-r--r--   0 phil       (501) staff       (20)     2223 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/user_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1201 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/user_scrobble_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1341 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/templates/lastfm/user_track_list.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.618377 django-ditto-3.2.0/ditto/lastfm/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.2.0/ditto/lastfm/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    10691 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/lastfm/templatetags/ditto_lastfm.py
--rw-r--r--   0 phil       (501) staff       (20)     2146 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/lastfm/urls.py
--rw-r--r--   0 phil       (501) staff       (20)      746 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/lastfm/utils.py
--rw-r--r--   0 phil       (501) staff       (20)    10239 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/lastfm/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.620557 django-ditto-3.2.0/ditto/pinboard/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:41.000000 django-ditto-3.2.0/ditto/pinboard/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     3158 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/pinboard/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      355 2021-04-07 17:02:04.000000 django-ditto-3.2.0/ditto/pinboard/apps.py
--rw-r--r--   0 phil       (501) staff       (20)      854 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/pinboard/checks.py
--rw-r--r--   0 phil       (501) staff       (20)     1025 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/pinboard/factories.py
--rw-r--r--   0 phil       (501) staff       (20)    10402 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/pinboard/fetch.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.620739 django-ditto-3.2.0/ditto/pinboard/management/
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-20 14:31:00.000000 django-ditto-3.2.0/ditto/pinboard/management/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.620912 django-ditto-3.2.0/ditto/pinboard/management/commands/
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-20 14:31:06.000000 django-ditto-3.2.0/ditto/pinboard/management/commands/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     2980 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/pinboard/management/commands/fetch_pinboard_bookmarks.py
--rw-r--r--   0 phil       (501) staff       (20)     1842 2023-05-09 14:30:15.000000 django-ditto-3.2.0/ditto/pinboard/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.625842 django-ditto-3.2.0/ditto/pinboard/migrations/
--rw-r--r--   0 phil       (501) staff       (20)     4338 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0001_initial.py
--rw-r--r--   0 phil       (501) staff       (20)      568 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0002_auto_20150626_1521.py
--rw-r--r--   0 phil       (501) staff       (20)      377 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0003_auto_20150626_1558.py
--rw-r--r--   0 phil       (501) staff       (20)      469 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0004_auto_20150626_1603.py
--rw-r--r--   0 phil       (501) staff       (20)      608 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0005_auto_20150626_1702.py
--rw-r--r--   0 phil       (501) staff       (20)      897 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0006_auto_20150723_1322.py
--rw-r--r--   0 phil       (501) staff       (20)     2239 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0007_auto_20150724_1957.py
--rw-r--r--   0 phil       (501) staff       (20)      643 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0008_bookmark_tags.py
--rw-r--r--   0 phil       (501) staff       (20)      531 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0009_auto_20150729_1056.py
--rw-r--r--   0 phil       (501) staff       (20)      709 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0010_auto_20150730_1112.py
--rw-r--r--   0 phil       (501) staff       (20)     4132 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0011_auto_20151002_1525.py
--rw-r--r--   0 phil       (501) staff       (20)      492 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0012_account_is_active.py
--rw-r--r--   0 phil       (501) staff       (20)     3773 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0013_auto_20151026_1546.py
--rw-r--r--   0 phil       (501) staff       (20)      733 2022-08-08 11:31:11.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0014_auto_20151028_1556.py
--rw-r--r--   0 phil       (501) staff       (20)      574 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0015_auto_20151110_1308.py
--rw-r--r--   0 phil       (501) staff       (20)      862 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0016_auto_20151119_1702.py
--rw-r--r--   0 phil       (501) staff       (20)      540 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0017_auto_20160413_0906.py
--rw-r--r--   0 phil       (501) staff       (20)      711 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0018_auto_20160414_1637.py
--rw-r--r--   0 phil       (501) staff       (20)      903 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0019_auto_20160428_1525.py
--rw-r--r--   0 phil       (501) staff       (20)      579 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0020_auto_20160428_1526.py
--rw-r--r--   0 phil       (501) staff       (20)      637 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0021_auto_20160428_1533.py
--rw-r--r--   0 phil       (501) staff       (20)      827 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0022_auto_20160428_1542.py
--rw-r--r--   0 phil       (501) staff       (20)      989 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0023_auto_20161117_1622.py
--rw-r--r--   0 phil       (501) staff       (20)      954 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0024_bookmark_post_year.py
--rw-r--r--   0 phil       (501) staff       (20)     1291 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0025_auto_20201223_1509.py
--rw-r--r--   0 phil       (501) staff       (20)     1041 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0026_alter_taggedbookmark_content_type_and_more.py
--rw-r--r--   0 phil       (501) staff       (20)      497 2022-11-28 14:50:18.000000 django-ditto-3.2.0/ditto/pinboard/migrations/0027_alter_bookmarktag_slug.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-16 18:14:06.000000 django-ditto-3.2.0/ditto/pinboard/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     8167 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/pinboard/models.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.581171 django-ditto-3.2.0/ditto/pinboard/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.627618 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/
--rw-r--r--   0 phil       (501) staff       (20)     1097 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/account_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1925 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/account_tag_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1707 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/account_toread.html
--rw-r--r--   0 phil       (501) staff       (20)      297 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/base.html
--rw-r--r--   0 phil       (501) staff       (20)     2388 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/bookmark_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1399 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.628773 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/
--rw-r--r--   0 phil       (501) staff       (20)     1086 2017-08-22 13:41:35.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/account.html
--rw-r--r--   0 phil       (501) staff       (20)      904 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/annual_bookmark_counts.html
--rw-r--r--   0 phil       (501) staff       (20)     2229 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/bookmark.html
--rw-r--r--   0 phil       (501) staff       (20)      963 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/bookmark_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1153 2017-02-09 11:48:12.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/nav_tabs.html
--rw-r--r--   0 phil       (501) staff       (20)      757 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/popular_tags.html
--rw-r--r--   0 phil       (501) staff       (20)     2542 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/tag_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1339 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/tag_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1372 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/pinboard/templates/pinboard/toread_list.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.628979 django-ditto-3.2.0/ditto/pinboard/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-10-14 14:00:53.000000 django-ditto-3.2.0/ditto/pinboard/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     2048 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/pinboard/templatetags/ditto_pinboard.py
--rw-r--r--   0 phil       (501) staff       (20)     1014 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/pinboard/urls.py
--rw-r--r--   0 phil       (501) staff       (20)     5293 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/pinboard/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.629210 django-ditto-3.2.0/ditto/scripts/
--rw-r--r--   0 phil       (501) staff       (20)     1091 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/scripts/flickr_authorize.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.631988 django-ditto-3.2.0/ditto/twitter/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:45.000000 django-ditto-3.2.0/ditto/twitter/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     8717 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      351 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/app_settings.py
--rw-r--r--   0 phil       (501) staff       (20)      239 2021-04-07 17:02:14.000000 django-ditto-3.2.0/ditto/twitter/apps.py
--rw-r--r--   0 phil       (501) staff       (20)     3847 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/factories.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.632670 django-ditto-3.2.0/ditto/twitter/fetch/
--rw-r--r--   0 phil       (501) staff       (20)       38 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/fetch/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    17953 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/fetch/fetch.py
--rw-r--r--   0 phil       (501) staff       (20)     7852 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/fetch/fetchers.py
--rw-r--r--   0 phil       (501) staff       (20)    14761 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/fetch/savers.py
--rw-r--r--   0 phil       (501) staff       (20)     1346 2020-05-23 18:57:17.000000 django-ditto-3.2.0/ditto/twitter/imagegenerators.py
--rw-r--r--   0 phil       (501) staff       (20)    11516 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/ingest.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.632943 django-ditto-3.2.0/ditto/twitter/management/
--rw-r--r--   0 phil       (501) staff       (20)        0 2020-05-23 16:03:25.000000 django-ditto-3.2.0/ditto/twitter/management/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.634072 django-ditto-3.2.0/ditto/twitter/management/commands/
--rw-r--r--   0 phil       (501) staff       (20)     3138 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/management/commands/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     1591 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/management/commands/fetch_twitter_accounts.py
--rw-r--r--   0 phil       (501) staff       (20)      793 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/management/commands/fetch_twitter_favorites.py
--rw-r--r--   0 phil       (501) staff       (20)     1002 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/management/commands/fetch_twitter_files.py
--rw-r--r--   0 phil       (501) staff       (20)      783 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/management/commands/fetch_twitter_tweets.py
--rw-r--r--   0 phil       (501) staff       (20)     1419 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/management/commands/generate_twitter_tweet_html.py
--rw-r--r--   0 phil       (501) staff       (20)     3148 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/management/commands/import_twitter_tweets.py
--rw-r--r--   0 phil       (501) staff       (20)      540 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/management/commands/update_twitter_tweets.py
--rw-r--r--   0 phil       (501) staff       (20)      533 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/management/commands/update_twitter_users.py
--rw-r--r--   0 phil       (501) staff       (20)     2163 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.645188 django-ditto-3.2.0/ditto/twitter/migrations/
--rw-r--r--   0 phil       (501) staff       (20)     1589 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0001_initial.py
--rw-r--r--   0 phil       (501) staff       (20)      913 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0002_auto_20150729_1704.py
--rw-r--r--   0 phil       (501) staff       (20)    12119 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0003_auto_20150730_1112.py
--rw-r--r--   0 phil       (501) staff       (20)     1640 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0004_auto_20150730_1116.py
--rw-r--r--   0 phil       (501) staff       (20)      780 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0005_auto_20150730_1350.py
--rw-r--r--   0 phil       (501) staff       (20)      480 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0006_auto_20150730_1450.py
--rw-r--r--   0 phil       (501) staff       (20)     1303 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0007_auto_20150807_1432.py
--rw-r--r--   0 phil       (501) staff       (20)      350 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0008_remove_user_twitter_id_str.py
--rw-r--r--   0 phil       (501) staff       (20)      556 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0009_account_last_fetch_id.py
--rw-r--r--   0 phil       (501) staff       (20)      344 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0010_remove_tweet_text.py
--rw-r--r--   0 phil       (501) staff       (20)      445 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0011_tweet_text.py
--rw-r--r--   0 phil       (501) staff       (20)      942 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0012_auto_20150814_1730.py
--rw-r--r--   0 phil       (501) staff       (20)      475 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0013_user_favorites.py
--rw-r--r--   0 phil       (501) staff       (20)     1175 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0014_auto_20150819_1342.py
--rw-r--r--   0 phil       (501) staff       (20)      893 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0015_auto_20150819_1349.py
--rw-r--r--   0 phil       (501) staff       (20)    10191 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0016_auto_20151002_1525.py
--rw-r--r--   0 phil       (501) staff       (20)      488 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0017_account_is_active.py
--rw-r--r--   0 phil       (501) staff       (20)      482 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0018_tweet_text_html.py
--rw-r--r--   0 phil       (501) staff       (20)     4357 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0019_auto_20151028_1556.py
--rw-r--r--   0 phil       (501) staff       (20)      482 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0020_auto_20151028_1611.py
--rw-r--r--   0 phil       (501) staff       (20)     5411 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0021_video.py
--rw-r--r--   0 phil       (501) staff       (20)      986 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0022_auto_20151104_0840.py
--rw-r--r--   0 phil       (501) staff       (20)     5483 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0023_media.py
--rw-r--r--   0 phil       (501) staff       (20)      846 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0024_auto_20151104_1157.py
--rw-r--r--   0 phil       (501) staff       (20)      682 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0025_auto_20151109_1651.py
--rw-r--r--   0 phil       (501) staff       (20)      542 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0026_auto_20151110_1131.py
--rw-r--r--   0 phil       (501) staff       (20)      353 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0027_remove_user_profile_image_url.py
--rw-r--r--   0 phil       (501) staff       (20)      407 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0028_auto_20151110_1139.py
--rw-r--r--   0 phil       (501) staff       (20)      891 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0029_auto_20151110_1308.py
--rw-r--r--   0 phil       (501) staff       (20)      538 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0030_auto_20151119_1649.py
--rw-r--r--   0 phil       (501) staff       (20)      782 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0031_auto_20160413_0906.py
--rw-r--r--   0 phil       (501) staff       (20)      704 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0032_auto_20160414_1637.py
--rw-r--r--   0 phil       (501) staff       (20)     3113 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0033_auto_20160421_1602.py
--rw-r--r--   0 phil       (501) staff       (20)      495 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0034_user_description_html.py
--rw-r--r--   0 phil       (501) staff       (20)      665 2020-05-23 18:57:18.000000 django-ditto-3.2.0/ditto/twitter/migrations/0035_auto_20160505_1137.py
--rw-r--r--   0 phil       (501) staff       (20)     1383 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0036_auto_20160505_1156.py
--rw-r--r--   0 phil       (501) staff       (20)      604 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0037_user_avatar.py
--rw-r--r--   0 phil       (501) staff       (20)      548 2020-05-23 18:57:18.000000 django-ditto-3.2.0/ditto/twitter/migrations/0038_tweet_retweeted_status_id.py
--rw-r--r--   0 phil       (501) staff       (20)      794 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0039_auto_20160603_1301.py
--rw-r--r--   0 phil       (501) staff       (20)      767 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0040_auto_20160603_1302.py
--rw-r--r--   0 phil       (501) staff       (20)      390 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0041_remove_media_tweet.py
--rw-r--r--   0 phil       (501) staff       (20)      482 2020-05-23 18:57:18.000000 django-ditto-3.2.0/ditto/twitter/migrations/0042_auto_20160603_1422.py
--rw-r--r--   0 phil       (501) staff       (20)      395 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0043_remove_media_is_private.py
--rw-r--r--   0 phil       (501) staff       (20)      439 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0044_auto_20160613_1600.py
--rw-r--r--   0 phil       (501) staff       (20)      579 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0045_media_original_image_file.py
--rw-r--r--   0 phil       (501) staff       (20)      649 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0046_auto_20160615_1038.py
--rw-r--r--   0 phil       (501) staff       (20)      669 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0047_media_video_file.py
--rw-r--r--   0 phil       (501) staff       (20)      761 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/migrations/0048_auto_20160615_1045.py
--rw-r--r--   0 phil       (501) staff       (20)      989 2020-05-23 18:57:18.000000 django-ditto-3.2.0/ditto/twitter/migrations/0049_auto_20160713_1127.py
--rw-r--r--   0 phil       (501) staff       (20)      663 2020-05-23 18:57:18.000000 django-ditto-3.2.0/ditto/twitter/migrations/0050_auto_20160713_1400.py
--rw-r--r--   0 phil       (501) staff       (20)      613 2020-05-23 18:57:18.000000 django-ditto-3.2.0/ditto/twitter/migrations/0051_auto_20160713_1444.py
--rw-r--r--   0 phil       (501) staff       (20)      982 2020-05-23 18:57:18.000000 django-ditto-3.2.0/ditto/twitter/migrations/0052_auto_20161117_1622.py
--rw-r--r--   0 phil       (501) staff       (20)      940 2020-05-23 18:57:18.000000 django-ditto-3.2.0/ditto/twitter/migrations/0053_tweet_post_year.py
--rw-r--r--   0 phil       (501) staff       (20)      476 2020-05-23 18:57:18.000000 django-ditto-3.2.0/ditto/twitter/migrations/0054_auto_20171113_1001.py
--rw-r--r--   0 phil       (501) staff       (20)      584 2020-05-23 18:57:18.000000 django-ditto-3.2.0/ditto/twitter/migrations/0055_re_save_tweets_for_new_html.py
--rw-r--r--   0 phil       (501) staff       (20)      616 2022-08-08 11:24:44.000000 django-ditto-3.2.0/ditto/twitter/migrations/0056_add_count_index.py
--rw-r--r--   0 phil       (501) staff       (20)     1142 2022-02-14 11:48:22.000000 django-ditto-3.2.0/ditto/twitter/migrations/0057_alter_account_access_token_and_more.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-07-29 16:20:01.000000 django-ditto-3.2.0/ditto/twitter/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    28022 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/models.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.581883 django-ditto-3.2.0/ditto/twitter/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.646456 django-ditto-3.2.0/ditto/twitter/templates/twitter/
--rw-r--r--   0 phil       (501) staff       (20)     1406 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/account_favorite_list.html
--rw-r--r--   0 phil       (501) staff       (20)      294 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/base.html
--rw-r--r--   0 phil       (501) staff       (20)     1421 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/favorite_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1294 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.647595 django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/
--rw-r--r--   0 phil       (501) staff       (20)     1248 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/annual_tweet_counts.html
--rw-r--r--   0 phil       (501) staff       (20)     2799 2022-02-13 12:12:56.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/media.html
--rw-r--r--   0 phil       (501) staff       (20)     1175 2016-05-07 11:14:06.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/nav_tabs.html
--rw-r--r--   0 phil       (501) staff       (20)     4156 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/tweet.html
--rw-r--r--   0 phil       (501) staff       (20)     1106 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/tweet_list.html
--rw-r--r--   0 phil       (501) staff       (20)     2437 2017-08-22 13:41:35.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/user.html
--rw-r--r--   0 phil       (501) staff       (20)     2680 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/tweet_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1255 2022-08-08 11:24:43.000000 django-ditto-3.2.0/ditto/twitter/templates/twitter/user_detail.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.647831 django-ditto-3.2.0/ditto/twitter/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-10-16 16:15:35.000000 django-ditto-3.2.0/ditto/twitter/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     4787 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/templatetags/ditto_twitter.py
--rw-r--r--   0 phil       (501) staff       (20)      673 2022-08-08 11:24:45.000000 django-ditto-3.2.0/ditto/twitter/urls.py
--rw-r--r--   0 phil       (501) staff       (20)     5800 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/utils.py
--rw-r--r--   0 phil       (501) staff       (20)     3918 2023-12-12 14:20:03.000000 django-ditto-3.2.0/ditto/twitter/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-12-13 12:05:50.648757 django-ditto-3.2.0/django_ditto.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)     3733 2023-12-13 12:05:50.000000 django-ditto-3.2.0/django_ditto.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)    14941 2023-12-13 12:05:50.000000 django-ditto-3.2.0/django_ditto.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-12-13 12:05:50.000000 django-ditto-3.2.0/django_ditto.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       47 2016-04-25 12:13:07.000000 django-ditto-3.2.0/django_ditto.egg-info/pbr.json
--rw-r--r--   0 phil       (501) staff       (20)      376 2023-12-13 12:05:50.000000 django-ditto-3.2.0/django_ditto.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        6 2023-12-13 12:05:50.000000 django-ditto-3.2.0/django_ditto.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)      889 2023-12-12 14:20:03.000000 django-ditto-3.2.0/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-12-13 12:05:50.649129 django-ditto-3.2.0/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     4150 2023-12-12 14:20:03.000000 django-ditto-3.2.0/setup.py
--rw-r--r--   0 phil       (501) staff       (20)     1414 2023-12-13 11:47:01.000000 django-ditto-3.2.0/tox.ini
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.058215 django-ditto-3.2.1/
+-rw-r--r--   0 phil       (501) staff       (20)     1083 2021-10-22 16:10:52.000000 django-ditto-3.2.1/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      326 2022-03-25 12:40:03.000000 django-ditto-3.2.1/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)     3733 2024-04-08 15:05:16.058087 django-ditto-3.2.1/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     2282 2023-12-12 14:20:03.000000 django-ditto-3.2.1/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.018427 django-ditto-3.2.1/ditto/
+-rw-r--r--   0 phil       (501) staff       (20)      196 2024-04-08 14:44:57.000000 django-ditto-3.2.1/ditto/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.019425 django-ditto-3.2.1/ditto/core/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:28.000000 django-ditto-3.2.1/ditto/core/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)      263 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/core/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      708 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/core/app_settings.py
+-rw-r--r--   0 phil       (501) staff       (20)     1785 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/core/apps.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.014182 django-ditto-3.2.1/ditto/core/management/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.019570 django-ditto-3.2.1/ditto/core/management/commands/
+-rw-r--r--   0 phil       (501) staff       (20)     1976 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/core/management/commands/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)      272 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/core/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.019683 django-ditto-3.2.1/ditto/core/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2020-05-23 15:29:03.000000 django-ditto-3.2.1/ditto/core/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     5446 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/core/models.py
+-rw-r--r--   0 phil       (501) staff       (20)    11629 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/core/paginator.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.014411 django-ditto-3.2.1/ditto/core/static/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.014602 django-ditto-3.2.1/ditto/core/static/ditto-core/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.019965 django-ditto-3.2.1/ditto/core/static/ditto-core/css/
+-rw-rw-r--   0 phil       (501) staff       (20)   162264 2022-07-19 15:13:44.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/css/bootstrap.min.css
+-rw-rw-r--   0 phil       (501) staff       (20)   654593 2022-07-19 15:13:44.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/css/bootstrap.min.css.map
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.020669 django-ditto-3.2.1/ditto/core/static/ditto-core/img/
+-rw-r--r--   0 phil       (501) staff       (20)      142 2016-09-06 12:05:37.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/img/default_avatar.png
+-rw-r--r--   0 phil       (501) staff       (20)     3520 2016-09-06 12:05:37.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/img/original_error.jpg
+-rw-r--r--   0 phil       (501) staff       (20)     3309 2016-09-06 12:05:37.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/img/original_missing.jpg
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.021246 django-ditto-3.2.1/ditto/core/static/ditto-core/js/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.022063 django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/
+-rw-rw-r--   0 phil       (501) staff       (20)    20871 2022-07-19 15:13:44.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/carousel.js
+-rw-rw-r--   0 phil       (501) staff       (20)    38793 2022-07-19 15:13:44.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/carousel.js.map
+-rw-rw-r--   0 phil       (501) staff       (20)    13394 2022-07-19 15:13:44.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/collapse.js
+-rw-rw-r--   0 phil       (501) staff       (20)    24048 2022-07-19 15:13:44.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/collapse.js.map
+-rw-rw-r--   0 phil       (501) staff       (20)     6631 2022-07-19 15:13:44.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/util.js
+-rw-rw-r--   0 phil       (501) staff       (20)    12040 2022-07-19 15:13:44.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/util.js.map
+-rw-r--r--   0 phil       (501) staff       (20)    72380 2020-05-24 12:52:06.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.js
+-rw-r--r--   0 phil       (501) staff       (20)   110382 2020-05-24 12:52:06.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.map
+-rw-r--r--   0 phil       (501) staff       (20)    21233 2020-11-19 17:03:58.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/js/popper.min.js
+-rw-r--r--   0 phil       (501) staff       (20)   117179 2018-04-16 15:41:13.000000 django-ditto-3.2.1/ditto/core/static/ditto-core/js/popper.min.js.map
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.014789 django-ditto-3.2.1/ditto/core/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.022656 django-ditto-3.2.1/ditto/core/templates/ditto/
+-rw-r--r--   0 phil       (501) staff       (20)     2230 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/core/templates/ditto/archive_day.html
+-rw-r--r--   0 phil       (501) staff       (20)     4738 2020-08-10 13:47:31.000000 django-ditto-3.2.1/ditto/core/templates/ditto/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     1029 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/core/templates/ditto/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.023300 django-ditto-3.2.1/ditto/core/templates/ditto/includes/
+-rw-r--r--   0 phil       (501) staff       (20)      643 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/core/templates/ditto/includes/account_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1180 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/core/templates/ditto/includes/item_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1760 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/core/templates/ditto/includes/item_lists.html
+-rw-r--r--   0 phil       (501) staff       (20)     1108 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/core/templates/ditto/includes/pager.html
+-rw-r--r--   0 phil       (501) staff       (20)     2478 2017-08-22 13:41:35.000000 django-ditto-3.2.1/ditto/core/templates/ditto/includes/pagination.html
+-rw-r--r--   0 phil       (501) staff       (20)     2272 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/core/templates/ditto/includes/variety_nav.html
+-rw-r--r--   0 phil       (501) staff       (20)      681 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/core/templates/ditto/tag_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)      399 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/core/templates/ditto/tag_list.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.023486 django-ditto-3.2.1/ditto/core/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.2.1/ditto/core/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     5119 2024-04-08 13:24:52.000000 django-ditto-3.2.1/ditto/core/templatetags/ditto_core.py
+-rw-r--r--   0 phil       (501) staff       (20)      620 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/core/urls.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.023728 django-ditto-3.2.1/ditto/core/utils/
+-rw-r--r--   0 phil       (501) staff       (20)     3477 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/core/utils/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     3543 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/core/utils/downloader.py
+-rw-r--r--   0 phil       (501) staff       (20)    23879 2024-04-08 13:25:37.000000 django-ditto-3.2.1/ditto/core/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.025087 django-ditto-3.2.1/ditto/flickr/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:33.000000 django-ditto-3.2.1/ditto/flickr/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    12068 2024-04-08 13:27:39.000000 django-ditto-3.2.1/ditto/flickr/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      444 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/app_settings.py
+-rw-r--r--   0 phil       (501) staff       (20)      345 2021-04-07 17:01:46.000000 django-ditto-3.2.1/ditto/flickr/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)      845 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/checks.py
+-rw-r--r--   0 phil       (501) staff       (20)     4051 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/factories.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.025699 django-ditto-3.2.1/ditto/flickr/fetch/
+-rw-r--r--   0 phil       (501) staff       (20)       38 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/fetch/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    20415 2024-04-08 13:28:21.000000 django-ditto-3.2.1/ditto/flickr/fetch/fetchers.py
+-rw-r--r--   0 phil       (501) staff       (20)     4752 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/fetch/filesfetchers.py
+-rw-r--r--   0 phil       (501) staff       (20)     4604 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/fetch/multifetchers.py
+-rw-r--r--   0 phil       (501) staff       (20)    16297 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/fetch/savers.py
+-rw-r--r--   0 phil       (501) staff       (20)     3065 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/imagegenerators.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.015256 django-ditto-3.2.1/ditto/flickr/management/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.026253 django-ditto-3.2.1/ditto/flickr/management/commands/
+-rw-r--r--   0 phil       (501) staff       (20)     2953 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/management/commands/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     2721 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/management/commands/fetch_flickr_account_user.py
+-rw-r--r--   0 phil       (501) staff       (20)     1448 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/management/commands/fetch_flickr_originals.py
+-rw-r--r--   0 phil       (501) staff       (20)     1451 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/management/commands/fetch_flickr_photos.py
+-rw-r--r--   0 phil       (501) staff       (20)      866 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/management/commands/fetch_flickr_photosets.py
+-rw-r--r--   0 phil       (501) staff       (20)     1927 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.029608 django-ditto-3.2.1/ditto/flickr/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)    23757 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0001_initial.py
+-rw-r--r--   0 phil       (501) staff       (20)      426 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0002_auto_20160406_1548.py
+-rw-r--r--   0 phil       (501) staff       (20)     1069 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0003_auto_20160413_0906.py
+-rw-r--r--   0 phil       (501) staff       (20)     4134 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0004_auto_20160414_1120.py
+-rw-r--r--   0 phil       (501) staff       (20)     7502 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0005_auto_20160414_1427.py
+-rw-r--r--   0 phil       (501) staff       (20)      556 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/flickr/migrations/0006_auto_20160414_1459.py
+-rw-r--r--   0 phil       (501) staff       (20)      703 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0007_auto_20160414_1637.py
+-rw-r--r--   0 phil       (501) staff       (20)     4347 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0008_auto_20160429_1559.py
+-rw-r--r--   0 phil       (501) staff       (20)      584 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/flickr/migrations/0009_photoset_fetch_time.py
+-rw-r--r--   0 phil       (501) staff       (20)      463 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/flickr/migrations/0010_photo_photosets.py
+-rw-r--r--   0 phil       (501) staff       (20)     1042 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0011_auto_20160502_1645.py
+-rw-r--r--   0 phil       (501) staff       (20)     1205 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/flickr/migrations/0012_auto_20160503_1457.py
+-rw-r--r--   0 phil       (501) staff       (20)      539 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/flickr/migrations/0013_photoset_photos_raw.py
+-rw-r--r--   0 phil       (501) staff       (20)      569 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0014_photo_original_file.py
+-rw-r--r--   0 phil       (501) staff       (20)      572 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0015_auto_20160514_1456.py
+-rw-r--r--   0 phil       (501) staff       (20)      662 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0016_photo_video_original_file.py
+-rw-r--r--   0 phil       (501) staff       (20)      856 2023-12-11 19:05:06.000000 django-ditto-3.2.1/ditto/flickr/migrations/0017_auto_20160524_1350.py
+-rw-r--r--   0 phil       (501) staff       (20)      681 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/flickr/migrations/0018_auto_20160525_1011.py
+-rw-r--r--   0 phil       (501) staff       (20)      585 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/flickr/migrations/0019_auto_20160713_1127.py
+-rw-r--r--   0 phil       (501) staff       (20)      981 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/flickr/migrations/0020_auto_20161117_1622.py
+-rw-r--r--   0 phil       (501) staff       (20)      941 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/flickr/migrations/0021_photo_post_year.py
+-rw-r--r--   0 phil       (501) staff       (20)      979 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/flickr/migrations/0022_photo_taken_year.py
+-rw-r--r--   0 phil       (501) staff       (20)      598 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0023_auto_20180104_1457.py
+-rw-r--r--   0 phil       (501) staff       (20)     1708 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/migrations/0024_auto_20201119_1539.py
+-rw-r--r--   0 phil       (501) staff       (20)     1908 2020-11-19 17:05:34.000000 django-ditto-3.2.1/ditto/flickr/migrations/0025_backfill_photo_sizes.py
+-rw-r--r--   0 phil       (501) staff       (20)      983 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/migrations/0026_alter_taggedphoto_content_object_and_more.py
+-rw-r--r--   0 phil       (501) staff       (20)      724 2022-03-24 08:27:58.000000 django-ditto-3.2.1/ditto/flickr/migrations/0027_alter_user_photos_url_alter_user_profile_url.py
+-rw-r--r--   0 phil       (501) staff       (20)      418 2022-03-24 08:27:58.000000 django-ditto-3.2.1/ditto/flickr/migrations/0028_alter_user_iconfarm.py
+-rw-r--r--   0 phil       (501) staff       (20)      533 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/migrations/0029_alter_user_options_alter_user_realname.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.2.1/ditto/flickr/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    32861 2024-04-08 13:54:03.000000 django-ditto-3.2.1/ditto/flickr/models.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.015457 django-ditto-3.2.1/ditto/flickr/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.030723 django-ditto-3.2.1/ditto/flickr/templates/flickr/
+-rw-r--r--   0 phil       (501) staff       (20)      291 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     1686 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.031639 django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/
+-rw-r--r--   0 phil       (501) staff       (20)      858 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/annual_photo_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)     1572 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/nav_tabs.html
+-rw-r--r--   0 phil       (501) staff       (20)     1102 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/photo.html
+-rw-r--r--   0 phil       (501) staff       (20)     2551 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/photo_columns.html
+-rw-r--r--   0 phil       (501) staff       (20)      457 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/photoset_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)     1456 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/photoset_list.html
+-rw-r--r--   0 phil       (501) staff       (20)      836 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/sorting.html
+-rw-r--r--   0 phil       (501) staff       (20)     1896 2022-03-24 08:27:58.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/user.html
+-rw-r--r--   0 phil       (501) staff       (20)    10445 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/photo_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     2615 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/photoset_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1560 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/photoset_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1781 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/tag_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1326 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/tag_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1194 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/user_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1167 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/user_photoset_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1966 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/flickr/templates/flickr/user_tag_detail.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.031835 django-ditto-3.2.1/ditto/flickr/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.2.1/ditto/flickr/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     3869 2024-04-08 13:47:18.000000 django-ditto-3.2.1/ditto/flickr/templatetags/ditto_flickr.py
+-rw-r--r--   0 phil       (501) staff       (20)     1175 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/flickr/urls.py
+-rw-r--r--   0 phil       (501) staff       (20)     9349 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/flickr/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.032916 django-ditto-3.2.1/ditto/lastfm/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:37.000000 django-ditto-3.2.1/ditto/lastfm/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     4354 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/lastfm/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      237 2021-04-07 17:01:57.000000 django-ditto-3.2.1/ditto/lastfm/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)     1590 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/lastfm/factories.py
+-rw-r--r--   0 phil       (501) staff       (20)    11445 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/lastfm/fetch.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.015911 django-ditto-3.2.1/ditto/lastfm/management/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.033119 django-ditto-3.2.1/ditto/lastfm/management/commands/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.2.1/ditto/lastfm/management/commands/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     1872 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/lastfm/management/commands/fetch_lastfm_scrobbles.py
+-rw-r--r--   0 phil       (501) staff       (20)     5901 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/lastfm/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.034063 django-ditto-3.2.1/ditto/lastfm/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)    11231 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/lastfm/migrations/0001_initial.py
+-rw-r--r--   0 phil       (501) staff       (20)      616 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/lastfm/migrations/0002_auto_20161012_1012.py
+-rw-r--r--   0 phil       (501) staff       (20)     1536 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/lastfm/migrations/0003_auto_20161026_1539.py
+-rw-r--r--   0 phil       (501) staff       (20)     2292 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/lastfm/migrations/0004_auto_20161026_1540.py
+-rw-r--r--   0 phil       (501) staff       (20)      987 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/lastfm/migrations/0005_auto_20161117_1622.py
+-rw-r--r--   0 phil       (501) staff       (20)      947 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/lastfm/migrations/0006_scrobble_post_year.py
+-rw-r--r--   0 phil       (501) staff       (20)      669 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/lastfm/migrations/0007_set_post_year.py
+-rw-r--r--   0 phil       (501) staff       (20)      607 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/lastfm/migrations/0008_auto_20180104_1457.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.2.1/ditto/lastfm/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    10932 2024-04-08 13:33:25.000000 django-ditto-3.2.1/ditto/lastfm/models.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.016210 django-ditto-3.2.1/ditto/lastfm/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.035949 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/
+-rw-r--r--   0 phil       (501) staff       (20)     1755 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/album_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1187 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/album_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1286 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/artist_albums.html
+-rw-r--r--   0 phil       (501) staff       (20)     1171 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/artist_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1191 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/artist_list.html
+-rw-r--r--   0 phil       (501) staff       (20)      292 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     2006 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.037233 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/
+-rw-r--r--   0 phil       (501) staff       (20)     1569 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/album_sidebar.html
+-rw-r--r--   0 phil       (501) staff       (20)      891 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/annual_scrobble_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)     1718 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/artist_sidebar.html
+-rw-r--r--   0 phil       (501) staff       (20)     3033 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/chart.html
+-rw-r--r--   0 phil       (501) staff       (20)      729 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/day_filter.html
+-rw-r--r--   0 phil       (501) staff       (20)      679 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/nav_tabs.html
+-rw-r--r--   0 phil       (501) staff       (20)     2964 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/page_navigation.html
+-rw-r--r--   0 phil       (501) staff       (20)     1338 2017-02-09 11:48:12.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/scrobble.html
+-rw-r--r--   0 phil       (501) staff       (20)     1741 2017-02-09 11:48:12.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/scrobble_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1593 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/track_sidebar.html
+-rw-r--r--   0 phil       (501) staff       (20)     1047 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/scrobble_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1485 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/track_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1187 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/track_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1341 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/user_album_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1345 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/user_artist_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     2223 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/user_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1201 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/user_scrobble_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1341 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/templates/lastfm/user_track_list.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.037449 django-ditto-3.2.1/ditto/lastfm/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.2.1/ditto/lastfm/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    10691 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/lastfm/templatetags/ditto_lastfm.py
+-rw-r--r--   0 phil       (501) staff       (20)     2146 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/lastfm/urls.py
+-rw-r--r--   0 phil       (501) staff       (20)      746 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/lastfm/utils.py
+-rw-r--r--   0 phil       (501) staff       (20)    10239 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/lastfm/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.038685 django-ditto-3.2.1/ditto/pinboard/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:41.000000 django-ditto-3.2.1/ditto/pinboard/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     3158 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/pinboard/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      355 2021-04-07 17:02:04.000000 django-ditto-3.2.1/ditto/pinboard/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)      854 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/pinboard/checks.py
+-rw-r--r--   0 phil       (501) staff       (20)     1025 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/pinboard/factories.py
+-rw-r--r--   0 phil       (501) staff       (20)    10402 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/pinboard/fetch.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.038869 django-ditto-3.2.1/ditto/pinboard/management/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-20 14:31:00.000000 django-ditto-3.2.1/ditto/pinboard/management/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.039101 django-ditto-3.2.1/ditto/pinboard/management/commands/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-20 14:31:06.000000 django-ditto-3.2.1/ditto/pinboard/management/commands/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     2980 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/pinboard/management/commands/fetch_pinboard_bookmarks.py
+-rw-r--r--   0 phil       (501) staff       (20)     1842 2023-05-09 14:30:15.000000 django-ditto-3.2.1/ditto/pinboard/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.042683 django-ditto-3.2.1/ditto/pinboard/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)     4338 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0001_initial.py
+-rw-r--r--   0 phil       (501) staff       (20)      568 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0002_auto_20150626_1521.py
+-rw-r--r--   0 phil       (501) staff       (20)      377 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0003_auto_20150626_1558.py
+-rw-r--r--   0 phil       (501) staff       (20)      469 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0004_auto_20150626_1603.py
+-rw-r--r--   0 phil       (501) staff       (20)      608 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0005_auto_20150626_1702.py
+-rw-r--r--   0 phil       (501) staff       (20)      897 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0006_auto_20150723_1322.py
+-rw-r--r--   0 phil       (501) staff       (20)     2239 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0007_auto_20150724_1957.py
+-rw-r--r--   0 phil       (501) staff       (20)      643 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0008_bookmark_tags.py
+-rw-r--r--   0 phil       (501) staff       (20)      531 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0009_auto_20150729_1056.py
+-rw-r--r--   0 phil       (501) staff       (20)      709 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0010_auto_20150730_1112.py
+-rw-r--r--   0 phil       (501) staff       (20)     4132 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0011_auto_20151002_1525.py
+-rw-r--r--   0 phil       (501) staff       (20)      492 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0012_account_is_active.py
+-rw-r--r--   0 phil       (501) staff       (20)     3773 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0013_auto_20151026_1546.py
+-rw-r--r--   0 phil       (501) staff       (20)      733 2022-08-08 11:31:11.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0014_auto_20151028_1556.py
+-rw-r--r--   0 phil       (501) staff       (20)      574 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0015_auto_20151110_1308.py
+-rw-r--r--   0 phil       (501) staff       (20)      862 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0016_auto_20151119_1702.py
+-rw-r--r--   0 phil       (501) staff       (20)      540 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0017_auto_20160413_0906.py
+-rw-r--r--   0 phil       (501) staff       (20)      711 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0018_auto_20160414_1637.py
+-rw-r--r--   0 phil       (501) staff       (20)      903 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0019_auto_20160428_1525.py
+-rw-r--r--   0 phil       (501) staff       (20)      579 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0020_auto_20160428_1526.py
+-rw-r--r--   0 phil       (501) staff       (20)      637 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0021_auto_20160428_1533.py
+-rw-r--r--   0 phil       (501) staff       (20)      827 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0022_auto_20160428_1542.py
+-rw-r--r--   0 phil       (501) staff       (20)      989 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0023_auto_20161117_1622.py
+-rw-r--r--   0 phil       (501) staff       (20)      954 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0024_bookmark_post_year.py
+-rw-r--r--   0 phil       (501) staff       (20)     1291 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0025_auto_20201223_1509.py
+-rw-r--r--   0 phil       (501) staff       (20)     1041 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0026_alter_taggedbookmark_content_type_and_more.py
+-rw-r--r--   0 phil       (501) staff       (20)      497 2022-11-28 14:50:18.000000 django-ditto-3.2.1/ditto/pinboard/migrations/0027_alter_bookmarktag_slug.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-16 18:14:06.000000 django-ditto-3.2.1/ditto/pinboard/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     8167 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/pinboard/models.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.016770 django-ditto-3.2.1/ditto/pinboard/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.043946 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/
+-rw-r--r--   0 phil       (501) staff       (20)     1097 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/account_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1925 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/account_tag_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1707 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/account_toread.html
+-rw-r--r--   0 phil       (501) staff       (20)      297 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     2388 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/bookmark_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1399 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.044736 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/
+-rw-r--r--   0 phil       (501) staff       (20)     1086 2017-08-22 13:41:35.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/account.html
+-rw-r--r--   0 phil       (501) staff       (20)      904 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/annual_bookmark_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)     2229 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/bookmark.html
+-rw-r--r--   0 phil       (501) staff       (20)      963 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/bookmark_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1153 2017-02-09 11:48:12.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/nav_tabs.html
+-rw-r--r--   0 phil       (501) staff       (20)      757 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/popular_tags.html
+-rw-r--r--   0 phil       (501) staff       (20)     2542 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/tag_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1339 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/tag_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1372 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/pinboard/templates/pinboard/toread_list.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.044968 django-ditto-3.2.1/ditto/pinboard/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-10-14 14:00:53.000000 django-ditto-3.2.1/ditto/pinboard/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     2048 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/pinboard/templatetags/ditto_pinboard.py
+-rw-r--r--   0 phil       (501) staff       (20)     1014 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/pinboard/urls.py
+-rw-r--r--   0 phil       (501) staff       (20)     5293 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/pinboard/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.045103 django-ditto-3.2.1/ditto/scripts/
+-rw-r--r--   0 phil       (501) staff       (20)     1091 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/scripts/flickr_authorize.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.046605 django-ditto-3.2.1/ditto/twitter/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:45.000000 django-ditto-3.2.1/ditto/twitter/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     8601 2024-04-08 13:38:45.000000 django-ditto-3.2.1/ditto/twitter/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      351 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/app_settings.py
+-rw-r--r--   0 phil       (501) staff       (20)      239 2021-04-07 17:02:14.000000 django-ditto-3.2.1/ditto/twitter/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)     3847 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/factories.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.047167 django-ditto-3.2.1/ditto/twitter/fetch/
+-rw-r--r--   0 phil       (501) staff       (20)       38 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/fetch/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    17953 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/fetch/fetch.py
+-rw-r--r--   0 phil       (501) staff       (20)     7852 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/fetch/fetchers.py
+-rw-r--r--   0 phil       (501) staff       (20)    14761 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/fetch/savers.py
+-rw-r--r--   0 phil       (501) staff       (20)     1346 2020-05-23 18:57:17.000000 django-ditto-3.2.1/ditto/twitter/imagegenerators.py
+-rw-r--r--   0 phil       (501) staff       (20)    11516 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/ingest.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.047303 django-ditto-3.2.1/ditto/twitter/management/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2020-05-23 16:03:25.000000 django-ditto-3.2.1/ditto/twitter/management/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.048393 django-ditto-3.2.1/ditto/twitter/management/commands/
+-rw-r--r--   0 phil       (501) staff       (20)     3138 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/management/commands/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     1591 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/management/commands/fetch_twitter_accounts.py
+-rw-r--r--   0 phil       (501) staff       (20)      793 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/management/commands/fetch_twitter_favorites.py
+-rw-r--r--   0 phil       (501) staff       (20)     1002 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/management/commands/fetch_twitter_files.py
+-rw-r--r--   0 phil       (501) staff       (20)      783 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/management/commands/fetch_twitter_tweets.py
+-rw-r--r--   0 phil       (501) staff       (20)     1419 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/management/commands/generate_twitter_tweet_html.py
+-rw-r--r--   0 phil       (501) staff       (20)     3148 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/management/commands/import_twitter_tweets.py
+-rw-r--r--   0 phil       (501) staff       (20)      540 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/management/commands/update_twitter_tweets.py
+-rw-r--r--   0 phil       (501) staff       (20)      533 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/management/commands/update_twitter_users.py
+-rw-r--r--   0 phil       (501) staff       (20)     2163 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.055627 django-ditto-3.2.1/ditto/twitter/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)     1589 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0001_initial.py
+-rw-r--r--   0 phil       (501) staff       (20)      913 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0002_auto_20150729_1704.py
+-rw-r--r--   0 phil       (501) staff       (20)    12119 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0003_auto_20150730_1112.py
+-rw-r--r--   0 phil       (501) staff       (20)     1640 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0004_auto_20150730_1116.py
+-rw-r--r--   0 phil       (501) staff       (20)      780 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0005_auto_20150730_1350.py
+-rw-r--r--   0 phil       (501) staff       (20)      480 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0006_auto_20150730_1450.py
+-rw-r--r--   0 phil       (501) staff       (20)     1303 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0007_auto_20150807_1432.py
+-rw-r--r--   0 phil       (501) staff       (20)      350 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0008_remove_user_twitter_id_str.py
+-rw-r--r--   0 phil       (501) staff       (20)      556 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0009_account_last_fetch_id.py
+-rw-r--r--   0 phil       (501) staff       (20)      344 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0010_remove_tweet_text.py
+-rw-r--r--   0 phil       (501) staff       (20)      445 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0011_tweet_text.py
+-rw-r--r--   0 phil       (501) staff       (20)      942 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0012_auto_20150814_1730.py
+-rw-r--r--   0 phil       (501) staff       (20)      475 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0013_user_favorites.py
+-rw-r--r--   0 phil       (501) staff       (20)     1175 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0014_auto_20150819_1342.py
+-rw-r--r--   0 phil       (501) staff       (20)      893 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0015_auto_20150819_1349.py
+-rw-r--r--   0 phil       (501) staff       (20)    10191 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0016_auto_20151002_1525.py
+-rw-r--r--   0 phil       (501) staff       (20)      488 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0017_account_is_active.py
+-rw-r--r--   0 phil       (501) staff       (20)      482 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0018_tweet_text_html.py
+-rw-r--r--   0 phil       (501) staff       (20)     4357 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0019_auto_20151028_1556.py
+-rw-r--r--   0 phil       (501) staff       (20)      482 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0020_auto_20151028_1611.py
+-rw-r--r--   0 phil       (501) staff       (20)     5411 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0021_video.py
+-rw-r--r--   0 phil       (501) staff       (20)      986 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0022_auto_20151104_0840.py
+-rw-r--r--   0 phil       (501) staff       (20)     5483 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0023_media.py
+-rw-r--r--   0 phil       (501) staff       (20)      846 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0024_auto_20151104_1157.py
+-rw-r--r--   0 phil       (501) staff       (20)      682 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0025_auto_20151109_1651.py
+-rw-r--r--   0 phil       (501) staff       (20)      542 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0026_auto_20151110_1131.py
+-rw-r--r--   0 phil       (501) staff       (20)      353 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0027_remove_user_profile_image_url.py
+-rw-r--r--   0 phil       (501) staff       (20)      407 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0028_auto_20151110_1139.py
+-rw-r--r--   0 phil       (501) staff       (20)      891 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0029_auto_20151110_1308.py
+-rw-r--r--   0 phil       (501) staff       (20)      538 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0030_auto_20151119_1649.py
+-rw-r--r--   0 phil       (501) staff       (20)      782 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0031_auto_20160413_0906.py
+-rw-r--r--   0 phil       (501) staff       (20)      704 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0032_auto_20160414_1637.py
+-rw-r--r--   0 phil       (501) staff       (20)     3113 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0033_auto_20160421_1602.py
+-rw-r--r--   0 phil       (501) staff       (20)      495 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0034_user_description_html.py
+-rw-r--r--   0 phil       (501) staff       (20)      665 2020-05-23 18:57:18.000000 django-ditto-3.2.1/ditto/twitter/migrations/0035_auto_20160505_1137.py
+-rw-r--r--   0 phil       (501) staff       (20)     1383 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0036_auto_20160505_1156.py
+-rw-r--r--   0 phil       (501) staff       (20)      604 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0037_user_avatar.py
+-rw-r--r--   0 phil       (501) staff       (20)      548 2020-05-23 18:57:18.000000 django-ditto-3.2.1/ditto/twitter/migrations/0038_tweet_retweeted_status_id.py
+-rw-r--r--   0 phil       (501) staff       (20)      794 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0039_auto_20160603_1301.py
+-rw-r--r--   0 phil       (501) staff       (20)      767 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0040_auto_20160603_1302.py
+-rw-r--r--   0 phil       (501) staff       (20)      390 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0041_remove_media_tweet.py
+-rw-r--r--   0 phil       (501) staff       (20)      482 2020-05-23 18:57:18.000000 django-ditto-3.2.1/ditto/twitter/migrations/0042_auto_20160603_1422.py
+-rw-r--r--   0 phil       (501) staff       (20)      395 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0043_remove_media_is_private.py
+-rw-r--r--   0 phil       (501) staff       (20)      439 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0044_auto_20160613_1600.py
+-rw-r--r--   0 phil       (501) staff       (20)      579 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0045_media_original_image_file.py
+-rw-r--r--   0 phil       (501) staff       (20)      649 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0046_auto_20160615_1038.py
+-rw-r--r--   0 phil       (501) staff       (20)      669 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0047_media_video_file.py
+-rw-r--r--   0 phil       (501) staff       (20)      761 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/migrations/0048_auto_20160615_1045.py
+-rw-r--r--   0 phil       (501) staff       (20)      989 2020-05-23 18:57:18.000000 django-ditto-3.2.1/ditto/twitter/migrations/0049_auto_20160713_1127.py
+-rw-r--r--   0 phil       (501) staff       (20)      663 2020-05-23 18:57:18.000000 django-ditto-3.2.1/ditto/twitter/migrations/0050_auto_20160713_1400.py
+-rw-r--r--   0 phil       (501) staff       (20)      613 2020-05-23 18:57:18.000000 django-ditto-3.2.1/ditto/twitter/migrations/0051_auto_20160713_1444.py
+-rw-r--r--   0 phil       (501) staff       (20)      982 2020-05-23 18:57:18.000000 django-ditto-3.2.1/ditto/twitter/migrations/0052_auto_20161117_1622.py
+-rw-r--r--   0 phil       (501) staff       (20)      940 2020-05-23 18:57:18.000000 django-ditto-3.2.1/ditto/twitter/migrations/0053_tweet_post_year.py
+-rw-r--r--   0 phil       (501) staff       (20)      476 2020-05-23 18:57:18.000000 django-ditto-3.2.1/ditto/twitter/migrations/0054_auto_20171113_1001.py
+-rw-r--r--   0 phil       (501) staff       (20)      584 2020-05-23 18:57:18.000000 django-ditto-3.2.1/ditto/twitter/migrations/0055_re_save_tweets_for_new_html.py
+-rw-r--r--   0 phil       (501) staff       (20)      616 2022-08-08 11:24:44.000000 django-ditto-3.2.1/ditto/twitter/migrations/0056_add_count_index.py
+-rw-r--r--   0 phil       (501) staff       (20)     1142 2022-02-14 11:48:22.000000 django-ditto-3.2.1/ditto/twitter/migrations/0057_alter_account_access_token_and_more.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-07-29 16:20:01.000000 django-ditto-3.2.1/ditto/twitter/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    28017 2024-04-08 13:35:24.000000 django-ditto-3.2.1/ditto/twitter/models.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.017430 django-ditto-3.2.1/ditto/twitter/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.056256 django-ditto-3.2.1/ditto/twitter/templates/twitter/
+-rw-r--r--   0 phil       (501) staff       (20)     1406 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/account_favorite_list.html
+-rw-r--r--   0 phil       (501) staff       (20)      294 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     1421 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/favorite_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1294 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.057004 django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/
+-rw-r--r--   0 phil       (501) staff       (20)     1248 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/annual_tweet_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)     2799 2022-02-13 12:12:56.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/media.html
+-rw-r--r--   0 phil       (501) staff       (20)     1175 2016-05-07 11:14:06.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/nav_tabs.html
+-rw-r--r--   0 phil       (501) staff       (20)     4156 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/tweet.html
+-rw-r--r--   0 phil       (501) staff       (20)     1106 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/tweet_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     2437 2017-08-22 13:41:35.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/user.html
+-rw-r--r--   0 phil       (501) staff       (20)     2680 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/tweet_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1255 2022-08-08 11:24:43.000000 django-ditto-3.2.1/ditto/twitter/templates/twitter/user_detail.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.057198 django-ditto-3.2.1/ditto/twitter/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-10-16 16:15:35.000000 django-ditto-3.2.1/ditto/twitter/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     4787 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/templatetags/ditto_twitter.py
+-rw-r--r--   0 phil       (501) staff       (20)      673 2022-08-08 11:24:45.000000 django-ditto-3.2.1/ditto/twitter/urls.py
+-rw-r--r--   0 phil       (501) staff       (20)     5800 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/utils.py
+-rw-r--r--   0 phil       (501) staff       (20)     3918 2023-12-12 14:20:03.000000 django-ditto-3.2.1/ditto/twitter/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-08 15:05:16.057902 django-ditto-3.2.1/django_ditto.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)     3733 2024-04-08 15:05:15.000000 django-ditto-3.2.1/django_ditto.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)    14941 2024-04-08 15:05:16.000000 django-ditto-3.2.1/django_ditto.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2024-04-08 15:05:15.000000 django-ditto-3.2.1/django_ditto.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       47 2016-04-25 12:13:07.000000 django-ditto-3.2.1/django_ditto.egg-info/pbr.json
+-rw-r--r--   0 phil       (501) staff       (20)      376 2024-04-08 15:05:15.000000 django-ditto-3.2.1/django_ditto.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        6 2024-04-08 15:05:15.000000 django-ditto-3.2.1/django_ditto.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)      889 2024-04-08 10:50:19.000000 django-ditto-3.2.1/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2024-04-08 15:05:16.058251 django-ditto-3.2.1/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     4150 2023-12-12 14:20:03.000000 django-ditto-3.2.1/setup.py
+-rw-r--r--   0 phil       (501) staff       (20)     1406 2024-04-08 14:15:37.000000 django-ditto-3.2.1/tox.ini
```

### Comparing `django-ditto-3.2.0/LICENSE` & `django-ditto-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/PKG-INFO` & `django-ditto-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ditto
-Version: 3.2.0
+Version: 3.2.1
 Summary: A Django app to copy stuff from your accounts on Flickr, Last.fm, Pinboard and Twitter.
 Home-page: https://github.com/philgyford/django-ditto
 Author: Phil Gyford
 Author-email: phil@gyford.com
 License: MIT
 Project-URL: Blog posts, https://www.gyford.com/phil/writing/tags/django-ditto/
 Project-URL: Bug Reports, https://github.com/philgyford/django-ditto/issues
```

### Comparing `django-ditto-3.2.0/README.md` & `django-ditto-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/app_settings.py` & `django-ditto-3.2.1/ditto/core/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/apps.py` & `django-ditto-3.2.1/ditto/core/apps.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/management/commands/__init__.py` & `django-ditto-3.2.1/ditto/core/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/models.py` & `django-ditto-3.2.1/ditto/core/models.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/paginator.py` & `django-ditto-3.2.1/ditto/core/paginator.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/css/bootstrap.min.css` & `django-ditto-3.2.1/ditto/core/static/ditto-core/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/css/bootstrap.min.css.map` & `django-ditto-3.2.1/ditto/core/static/ditto-core/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/img/original_error.jpg` & `django-ditto-3.2.1/ditto/core/static/ditto-core/img/original_error.jpg`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/img/original_missing.jpg` & `django-ditto-3.2.1/ditto/core/static/ditto-core/img/original_missing.jpg`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/carousel.js` & `django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/carousel.js`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/carousel.js.map` & `django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/carousel.js.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/collapse.js` & `django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/collapse.js`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/collapse.js.map` & `django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/collapse.js.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/util.js` & `django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/util.js`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/js/bootstrap/util.js.map` & `django-ditto-3.2.1/ditto/core/static/ditto-core/js/bootstrap/util.js.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.js` & `django-ditto-3.2.1/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.map` & `django-ditto-3.2.1/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/js/popper.min.js` & `django-ditto-3.2.1/ditto/core/static/ditto-core/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/static/ditto-core/js/popper.min.js.map` & `django-ditto-3.2.1/ditto/core/static/ditto-core/js/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/templates/ditto/archive_day.html` & `django-ditto-3.2.1/ditto/core/templates/ditto/archive_day.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/templates/ditto/base.html` & `django-ditto-3.2.1/ditto/core/templates/ditto/base.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/templates/ditto/home.html` & `django-ditto-3.2.1/ditto/core/templates/ditto/home.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/templates/ditto/includes/account_list.html` & `django-ditto-3.2.1/ditto/core/templates/ditto/includes/account_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/templates/ditto/includes/item_list.html` & `django-ditto-3.2.1/ditto/core/templates/ditto/includes/item_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/templates/ditto/includes/item_lists.html` & `django-ditto-3.2.1/ditto/core/templates/ditto/includes/item_lists.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/templates/ditto/includes/pager.html` & `django-ditto-3.2.1/ditto/core/templates/ditto/includes/pager.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/templates/ditto/includes/pagination.html` & `django-ditto-3.2.1/ditto/core/templates/ditto/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/templates/ditto/includes/variety_nav.html` & `django-ditto-3.2.1/ditto/core/templates/ditto/includes/variety_nav.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/templates/ditto/tag_detail.html` & `django-ditto-3.2.1/ditto/core/templates/ditto/tag_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/templatetags/ditto_core.py` & `django-ditto-3.2.1/ditto/core/templatetags/ditto_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,12 +156,11 @@
         {% current_url_name as url_name %}
 
         <a href="#"{% if url_name == 'myapp:home' %} class="active"{% endif %}">Home</a>
 
     """
     url_name = False
     if context.request.resolver_match:
-        url_name = "{}:{}".format(
-            context.request.resolver_match.namespace,
-            context.request.resolver_match.url_name,
-        )
+        namespace = context.request.resolver_match.namespace
+        name = context.request.resolver_match.url_name
+        url_name = f"{namespace}:{name}"
     return url_name
```

### Comparing `django-ditto-3.2.0/ditto/core/urls.py` & `django-ditto-3.2.1/ditto/core/urls.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/utils/__init__.py` & `django-ditto-3.2.1/ditto/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/utils/downloader.py` & `django-ditto-3.2.1/ditto/core/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/core/views.py` & `django-ditto-3.2.1/ditto/core/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,16 +236,17 @@
             self.app_name = self.get_app_name_from_slug(app_slug)
 
             if self.is_valid_variety_slug(app_slug, variety_slug):
                 self.variety_name = self.get_variety_name_from_slugs(
                     app_slug, variety_slug
                 )
             elif variety_slug:
-                msg = "'{}' is not a valid variety slug for the '{}' app slug.".format(
-                    variety_slug, app_slug
+                msg = (
+                    f"'{variety_slug}' is not a valid variety slug for "
+                    f"the '{app_slug}' app slug."
                 )
                 raise Http404(msg)
         elif app_slug:
             raise Http404("'%s' is not a valid app slug." % app_slug)
 
         self.app_slug = app_slug
         self.variety_slug = variety_slug
```

### Comparing `django-ditto-3.2.0/ditto/flickr/admin.py` & `django-ditto-3.2.1/ditto/flickr/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -437,28 +437,26 @@
     inlines = [
         TaggedPhotoInline,
     ]
     raw_id_fields = ("user",)
 
     def show_thumb(self, instance):
         return mark_safe(
-            '<img src="{}" width="{}" height="{}" />'.format(
-                instance.thumbnail_url,
-                instance.thumbnail_width,
-                instance.thumbnail_height,
-            )
+            f'<img src="{instance.thumbnail_url}" '
+            f'width="{instance.thumbnail_width}" '
+            f'height="{instance.thumbnail_height}" />'
         )
 
     show_thumb.short_description = "Thumbnail"
 
     def show_image(self, instance):
         return mark_safe(
-            '<img src="{}" width="{}" height="{}" />'.format(
-                instance.small_url, instance.small_width, instance.small_height
-            )
+            f'<img src="{instance.small_url}" '
+            f'width="{instance.small_width}" '
+            f'height="{instance.small_height}" />'
         )
 
     show_image.short_description = "Small image"
 
     def taken_year_str(self, instance):
         "So Admin doesn't add a comma, like '2,016'."
         return str(instance.taken_year)
```

### Comparing `django-ditto-3.2.0/ditto/flickr/checks.py` & `django-ditto-3.2.1/ditto/flickr/checks.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/factories.py` & `django-ditto-3.2.1/ditto/flickr/factories.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/fetch/fetchers.py` & `django-ditto-3.2.1/ditto/flickr/fetch/fetchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -547,16 +547,17 @@
                 results = self.api.photosets.getPhotos(
                     photoset_id=photoset_id,
                     user_id=self.account.user.nsid,
                     per_page=self.items_per_page,
                     page=page_number,
                 )
             except FlickrError as err:
-                msg = "Error when fetching photos in photoset {} (page {}): {}".format(
-                    photoset_id, page_number, err
+                msg = (
+                    f"Error when fetching photos in photoset {photoset_id} "
+                    f"(page {page_number}): {err}"
                 )
                 raise FetchError(msg) from err
 
             if "photoset" in results and "photo" in results["photoset"]:
                 total_pages = results["photoset"]["pages"]
                 photos += results["photoset"]["photo"]
```

### Comparing `django-ditto-3.2.0/ditto/flickr/fetch/filesfetchers.py` & `django-ditto-3.2.1/ditto/flickr/fetch/filesfetchers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/fetch/multifetchers.py` & `django-ditto-3.2.1/ditto/flickr/fetch/multifetchers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/fetch/savers.py` & `django-ditto-3.2.1/ditto/flickr/fetch/savers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/imagegenerators.py` & `django-ditto-3.2.1/ditto/flickr/imagegenerators.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/management/commands/__init__.py` & `django-ditto-3.2.1/ditto/flickr/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/management/commands/fetch_flickr_account_user.py` & `django-ditto-3.2.1/ditto/flickr/management/commands/fetch_flickr_account_user.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/management/commands/fetch_flickr_originals.py` & `django-ditto-3.2.1/ditto/flickr/management/commands/fetch_flickr_originals.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/management/commands/fetch_flickr_photos.py` & `django-ditto-3.2.1/ditto/flickr/management/commands/fetch_flickr_photos.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/management/commands/fetch_flickr_photosets.py` & `django-ditto-3.2.1/ditto/flickr/management/commands/fetch_flickr_photosets.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/managers.py` & `django-ditto-3.2.1/ditto/flickr/managers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0001_initial.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0003_auto_20160413_0906.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0003_auto_20160413_0906.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0004_auto_20160414_1120.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0004_auto_20160414_1120.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0005_auto_20160414_1427.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0005_auto_20160414_1427.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0006_auto_20160414_1459.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0006_auto_20160414_1459.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0007_auto_20160414_1637.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0007_auto_20160414_1637.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0008_auto_20160429_1559.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0008_auto_20160429_1559.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0009_photoset_fetch_time.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0009_photoset_fetch_time.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0011_auto_20160502_1645.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0011_auto_20160502_1645.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0012_auto_20160503_1457.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0012_auto_20160503_1457.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0013_photoset_photos_raw.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0013_photoset_photos_raw.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0014_photo_original_file.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0014_photo_original_file.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0015_auto_20160514_1456.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0015_auto_20160514_1456.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0016_photo_video_original_file.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0016_photo_video_original_file.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0017_auto_20160524_1350.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0017_auto_20160524_1350.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0018_auto_20160525_1011.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0018_auto_20160525_1011.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0019_auto_20160713_1127.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0019_auto_20160713_1127.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0020_auto_20161117_1622.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0020_auto_20161117_1622.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0021_photo_post_year.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0021_photo_post_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0022_photo_taken_year.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0022_photo_taken_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0023_auto_20180104_1457.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0023_auto_20180104_1457.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0024_auto_20201119_1539.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0024_auto_20201119_1539.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0025_backfill_photo_sizes.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0025_backfill_photo_sizes.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0026_alter_taggedphoto_content_object_and_more.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0026_alter_taggedphoto_content_object_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0027_alter_user_photos_url_alter_user_profile_url.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0027_alter_user_photos_url_alter_user_profile_url.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/migrations/0029_alter_user_options_alter_user_realname.py` & `django-ditto-3.2.1/ditto/flickr/migrations/0029_alter_user_options_alter_user_realname.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/models.py` & `django-ditto-3.2.1/ditto/flickr/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         if self.user:
             return reverse("flickr:user_detail", kwargs={"nsid": self.user.nsid})
         else:
             return ""
 
     def has_credentials(self):
         "Does this at least have something in its API fields? True or False"
-        return self.api_key and self.api_secret
+        return bool(self.api_key and self.api_secret)
 
 
 class TaggedPhoto(TaggedItemBase):
     """
     Describes the relationship between a django-taggit Tag and a Photo.
     Flickr has various fields which are unique to this relationship, rather
     than the Tag itself.
@@ -491,14 +491,17 @@
         default="",
         help_text="Only present for Videos.",
     )
 
     class Meta:
         ordering = ("-post_time",)
 
+    def __str__(self):
+        return super().__str__()
+
     def save(self, *args, **kwargs):
         if self.taken_time:
             self.taken_year = self.taken_time.year
         else:
             self.taken_year = None
         super().save(*args, **kwargs)
 
@@ -677,20 +680,17 @@
                 self.original_format,
             )
         else:
             size_ext = ""
             # Medium size doesn't have a letter suffix.
             if self.PHOTO_SIZES[size]["suffix"]:
                 size_ext = "_{}".format(self.PHOTO_SIZES[size]["suffix"])
-            return "https://farm{}.static.flickr.com/{}/{}_{}{}.jpg".format(
-                self.farm,
-                self.server,
-                self.flickr_id,
-                self.secret,
-                size_ext,
+            return (
+                f"https://farm{self.farm}.static.flickr.com/{self.server}/"
+                f"{self.flickr_id}_{self.secret}{size_ext}.jpg"
             )
 
     def _video_url(self, size):
         return self._remote_video_url(size)
 
     # def _local_video_url(self, size):
     # """One day, if we work out how to translate our downloaded original
@@ -908,14 +908,13 @@
         except ValueError:
             return static("ditto-core/img/default_avatar.png")
 
     @property
     def original_icon_url(self):
         """URL of the avatar/profile pic at Flickr."""
         if self.iconserver:
-            return "https://farm{}.staticflickr.com/{}/buddyicons/{}.jpg".format(
-                self.iconfarm,
-                self.iconserver,
-                self.nsid,
+            return (
+                f"https://farm{self.iconfarm}.staticflickr.com/{self.iconserver}"
+                f"/buddyicons/{self.nsid}.jpg"
             )
         else:
             return "https://www.flickr.com/images/buddyicon.gif"
```

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/home.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/home.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/annual_photo_counts.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/annual_photo_counts.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/nav_tabs.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/nav_tabs.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/photo.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/photo.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/photo_columns.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/photo_columns.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/photoset_list.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/photoset_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/sorting.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/sorting.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/includes/user.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/includes/user.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/photo_detail.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/photo_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/photoset_detail.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/photoset_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/photoset_list.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/photoset_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/tag_detail.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/tag_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/tag_list.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/tag_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/user_detail.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/user_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/user_photoset_list.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/user_photoset_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templates/flickr/user_tag_detail.html` & `django-ditto-3.2.1/ditto/flickr/templates/flickr/user_tag_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/templatetags/ditto_flickr.py` & `django-ditto-3.2.1/ditto/flickr/templatetags/ditto_flickr.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,17 +81,16 @@
     Will probably be an HTML link to more info.
     """
     licenses = {x: y for x, y in Photo.LICENSES}
 
     if n in licenses:
         if n in Photo.LICENSE_URLS and Photo.LICENSE_URLS[n] != "":
             return format_html(
-                '<a href="{}" title="More about permissions">{}</a>'.format(
-                    Photo.LICENSE_URLS[n], licenses[n]
-                )
+                f'<a href="{Photo.LICENSE_URLS[n]}" title="More about permissions">'
+                f"{licenses[n]}</a>"
             )
         else:
             return licenses[n]
     else:
         return "[missing]"
```

### Comparing `django-ditto-3.2.0/ditto/flickr/urls.py` & `django-ditto-3.2.1/ditto/flickr/urls.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/flickr/views.py` & `django-ditto-3.2.1/ditto/flickr/views.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/admin.py` & `django-ditto-3.2.1/ditto/lastfm/admin.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/factories.py` & `django-ditto-3.2.1/ditto/lastfm/factories.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/fetch.py` & `django-ditto-3.2.1/ditto/lastfm/fetch.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/management/commands/fetch_lastfm_scrobbles.py` & `django-ditto-3.2.1/ditto/lastfm/management/commands/fetch_lastfm_scrobbles.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/managers.py` & `django-ditto-3.2.1/ditto/lastfm/managers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/migrations/0001_initial.py` & `django-ditto-3.2.1/ditto/lastfm/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/migrations/0002_auto_20161012_1012.py` & `django-ditto-3.2.1/ditto/lastfm/migrations/0002_auto_20161012_1012.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/migrations/0003_auto_20161026_1539.py` & `django-ditto-3.2.1/ditto/lastfm/migrations/0003_auto_20161026_1539.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/migrations/0004_auto_20161026_1540.py` & `django-ditto-3.2.1/ditto/lastfm/migrations/0004_auto_20161026_1540.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/migrations/0005_auto_20161117_1622.py` & `django-ditto-3.2.1/ditto/lastfm/migrations/0005_auto_20161117_1622.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/migrations/0006_scrobble_post_year.py` & `django-ditto-3.2.1/ditto/lastfm/migrations/0006_scrobble_post_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/migrations/0007_set_post_year.py` & `django-ditto-3.2.1/ditto/lastfm/migrations/0007_set_post_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/migrations/0008_auto_20180104_1457.py` & `django-ditto-3.2.1/ditto/lastfm/migrations/0008_auto_20180104_1457.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/models.py` & `django-ditto-3.2.1/ditto/lastfm/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,18 +107,16 @@
             "lastfm:album_detail",
             kwargs={"artist_slug": self.artist.slug, "album_slug": self.slug},
         )
 
     @property
     def permalink(self):
         "The Album's URL at Last.fm."
-        return "{}/music/{}/{}".format(
-            LASTFM_URL_ROOT,
-            self.artist.original_slug,
-            self.original_slug,
+        return (
+            f"{LASTFM_URL_ROOT}/music/{self.artist.original_slug}/{self.original_slug}"
         )
 
     @property
     def musicbrainz_url(self):
         if self.mbid:
             return f"{MUSICBRAINZ_URL_ROOT}/release/{self.mbid}"
         else:
@@ -335,18 +333,17 @@
             "lastfm:track_detail",
             kwargs={"artist_slug": self.artist.slug, "track_slug": self.slug},
         )
 
     @property
     def permalink(self):
         "The Track's URL at Last.fm."
-        return "{}/music/{}/_/{}".format(
-            LASTFM_URL_ROOT,
-            self.artist.original_slug,
-            self.original_slug,
+        return (
+            f"{LASTFM_URL_ROOT}/music/{self.artist.original_slug}/_/"
+            f"{self.original_slug}"
         )
 
     @property
     def musicbrainz_url(self):
         if self.mbid:
             return f"{MUSICBRAINZ_URL_ROOT}/recording/{self.mbid}"
         else:
```

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/album_detail.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/album_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/album_list.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/album_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/artist_albums.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/artist_albums.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/artist_detail.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/artist_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/artist_list.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/artist_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/home.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/home.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/album_sidebar.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/album_sidebar.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/annual_scrobble_counts.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/annual_scrobble_counts.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/artist_sidebar.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/artist_sidebar.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/chart.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/chart.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/day_filter.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/day_filter.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/nav_tabs.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/nav_tabs.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/page_navigation.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/page_navigation.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/scrobble.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/scrobble.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/scrobble_list.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/scrobble_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/includes/track_sidebar.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/includes/track_sidebar.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/scrobble_list.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/scrobble_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/track_detail.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/track_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/track_list.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/track_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/user_album_list.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/user_album_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/user_artist_list.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/user_artist_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/user_detail.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/user_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/user_scrobble_list.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/user_scrobble_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templates/lastfm/user_track_list.html` & `django-ditto-3.2.1/ditto/lastfm/templates/lastfm/user_track_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/templatetags/ditto_lastfm.py` & `django-ditto-3.2.1/ditto/lastfm/templatetags/ditto_lastfm.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/urls.py` & `django-ditto-3.2.1/ditto/lastfm/urls.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/utils.py` & `django-ditto-3.2.1/ditto/lastfm/utils.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/lastfm/views.py` & `django-ditto-3.2.1/ditto/lastfm/views.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/admin.py` & `django-ditto-3.2.1/ditto/pinboard/admin.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/checks.py` & `django-ditto-3.2.1/ditto/pinboard/checks.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/factories.py` & `django-ditto-3.2.1/ditto/pinboard/factories.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/fetch.py` & `django-ditto-3.2.1/ditto/pinboard/fetch.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/management/commands/fetch_pinboard_bookmarks.py` & `django-ditto-3.2.1/ditto/pinboard/management/commands/fetch_pinboard_bookmarks.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/managers.py` & `django-ditto-3.2.1/ditto/pinboard/managers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0001_initial.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0002_auto_20150626_1521.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0002_auto_20150626_1521.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0005_auto_20150626_1702.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0005_auto_20150626_1702.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0006_auto_20150723_1322.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0006_auto_20150723_1322.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0007_auto_20150724_1957.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0007_auto_20150724_1957.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0008_bookmark_tags.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0008_bookmark_tags.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0009_auto_20150729_1056.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0009_auto_20150729_1056.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0010_auto_20150730_1112.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0010_auto_20150730_1112.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0011_auto_20151002_1525.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0011_auto_20151002_1525.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0013_auto_20151026_1546.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0013_auto_20151026_1546.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0014_auto_20151028_1556.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0014_auto_20151028_1556.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0015_auto_20151110_1308.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0015_auto_20151110_1308.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0016_auto_20151119_1702.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0016_auto_20151119_1702.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0017_auto_20160413_0906.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0017_auto_20160413_0906.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0018_auto_20160414_1637.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0018_auto_20160414_1637.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0019_auto_20160428_1525.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0019_auto_20160428_1525.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0020_auto_20160428_1526.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0020_auto_20160428_1526.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0021_auto_20160428_1533.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0021_auto_20160428_1533.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0022_auto_20160428_1542.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0022_auto_20160428_1542.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0023_auto_20161117_1622.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0023_auto_20161117_1622.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0024_bookmark_post_year.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0024_bookmark_post_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0025_auto_20201223_1509.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0025_auto_20201223_1509.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/migrations/0026_alter_taggedbookmark_content_type_and_more.py` & `django-ditto-3.2.1/ditto/pinboard/migrations/0026_alter_taggedbookmark_content_type_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/models.py` & `django-ditto-3.2.1/ditto/pinboard/models.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/account_detail.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/account_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/account_tag_detail.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/account_tag_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/account_toread.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/account_toread.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/bookmark_detail.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/bookmark_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/home.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/home.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/account.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/account.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/annual_bookmark_counts.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/annual_bookmark_counts.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/bookmark.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/bookmark.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/bookmark_list.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/bookmark_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/nav_tabs.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/nav_tabs.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/includes/popular_tags.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/includes/popular_tags.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/tag_detail.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/tag_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/tag_list.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/tag_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templates/pinboard/toread_list.html` & `django-ditto-3.2.1/ditto/pinboard/templates/pinboard/toread_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/templatetags/ditto_pinboard.py` & `django-ditto-3.2.1/ditto/pinboard/templatetags/ditto_pinboard.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/urls.py` & `django-ditto-3.2.1/ditto/pinboard/urls.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/pinboard/views.py` & `django-ditto-3.2.1/ditto/pinboard/views.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/scripts/flickr_authorize.py` & `django-ditto-3.2.1/ditto/scripts/flickr_authorize.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/admin.py` & `django-ditto-3.2.1/ditto/twitter/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -151,37 +151,32 @@
         "time_created",
         "time_modified",
     )
     exclude = ("tweets",)
 
     def show_thumb(self, instance):
         return mark_safe(
-            '<img src="{}" width="{}" height="{}" />'.format(
-                instance.thumbnail_url,
-                instance.thumbnail_w,
-                instance.thumbnail_h,
-            )
+            f'<img src="{instance.thumbnail_url}" width="{instance.thumbnail_w}" '
+            f'height="{instance.thumbnail_h}" />'
         )
 
     show_thumb.short_description = ""
 
     def show_image(self, instance):
         if instance.media_type == "photo":
-            html = '<img src="{}" width="{}" height="{}" />'.format(
-                instance.small_url,
-                instance.small_w,
-                instance.small_h,
+            html = (
+                f'<img src="{instance.small_url}" width="{instance.small_w}" '
+                f'height="{instance.small_h}" />'
             )
         else:
-            html = '<video width="{}" height="{}" poster="{}" controls preload="metadata"><source src="{}" type="{}"></video>'.format(  # noqa: E501
-                instance.small_w,
-                instance.small_h,
-                instance.small_url,
-                instance.video_url,
-                instance.video_mime_type,
+            html = (
+                f'<video width="{instance.small_w}" height="{instance.small_h}" '
+                f'poster="{instance.small_url}" controls preload="metadata">'
+                f'<source src="{instance.video_url}" type="{instance.video_mime_type}">'
+                "</video>"
             )
         return mark_safe(html)
 
     show_image.short_description = "Image"
 
 
 @admin.register(Tweet)
```

### Comparing `django-ditto-3.2.0/ditto/twitter/factories.py` & `django-ditto-3.2.1/ditto/twitter/factories.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/fetch/fetch.py` & `django-ditto-3.2.1/ditto/twitter/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/fetch/fetchers.py` & `django-ditto-3.2.1/ditto/twitter/fetch/fetchers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/fetch/savers.py` & `django-ditto-3.2.1/ditto/twitter/fetch/savers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/imagegenerators.py` & `django-ditto-3.2.1/ditto/twitter/imagegenerators.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/ingest.py` & `django-ditto-3.2.1/ditto/twitter/ingest.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/management/commands/__init__.py` & `django-ditto-3.2.1/ditto/twitter/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/management/commands/fetch_twitter_accounts.py` & `django-ditto-3.2.1/ditto/twitter/management/commands/fetch_twitter_accounts.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/management/commands/fetch_twitter_favorites.py` & `django-ditto-3.2.1/ditto/twitter/management/commands/fetch_twitter_favorites.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/management/commands/fetch_twitter_files.py` & `django-ditto-3.2.1/ditto/twitter/management/commands/fetch_twitter_files.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/management/commands/fetch_twitter_tweets.py` & `django-ditto-3.2.1/ditto/twitter/management/commands/fetch_twitter_tweets.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/management/commands/generate_twitter_tweet_html.py` & `django-ditto-3.2.1/ditto/twitter/management/commands/generate_twitter_tweet_html.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/management/commands/import_twitter_tweets.py` & `django-ditto-3.2.1/ditto/twitter/management/commands/import_twitter_tweets.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/management/commands/update_twitter_tweets.py` & `django-ditto-3.2.1/ditto/twitter/management/commands/update_twitter_tweets.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/management/commands/update_twitter_users.py` & `django-ditto-3.2.1/ditto/twitter/management/commands/update_twitter_users.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/managers.py` & `django-ditto-3.2.1/ditto/twitter/managers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0001_initial.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0002_auto_20150729_1704.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0002_auto_20150729_1704.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0003_auto_20150730_1112.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0003_auto_20150730_1112.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0004_auto_20150730_1116.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0004_auto_20150730_1116.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0005_auto_20150730_1350.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0005_auto_20150730_1350.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0007_auto_20150807_1432.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0007_auto_20150807_1432.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0009_account_last_fetch_id.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0009_account_last_fetch_id.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0012_auto_20150814_1730.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0012_auto_20150814_1730.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0014_auto_20150819_1342.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0014_auto_20150819_1342.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0015_auto_20150819_1349.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0015_auto_20150819_1349.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0016_auto_20151002_1525.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0016_auto_20151002_1525.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0019_auto_20151028_1556.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0019_auto_20151028_1556.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0021_video.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0021_video.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0022_auto_20151104_0840.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0022_auto_20151104_0840.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0023_media.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0023_media.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0024_auto_20151104_1157.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0024_auto_20151104_1157.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0025_auto_20151109_1651.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0025_auto_20151109_1651.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0026_auto_20151110_1131.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0026_auto_20151110_1131.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0029_auto_20151110_1308.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0029_auto_20151110_1308.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0030_auto_20151119_1649.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0030_auto_20151119_1649.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0031_auto_20160413_0906.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0031_auto_20160413_0906.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0032_auto_20160414_1637.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0032_auto_20160414_1637.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0033_auto_20160421_1602.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0033_auto_20160421_1602.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0035_auto_20160505_1137.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0035_auto_20160505_1137.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0036_auto_20160505_1156.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0036_auto_20160505_1156.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0037_user_avatar.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0037_user_avatar.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0038_tweet_retweeted_status_id.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0038_tweet_retweeted_status_id.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0039_auto_20160603_1301.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0039_auto_20160603_1301.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0040_auto_20160603_1302.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0040_auto_20160603_1302.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0045_media_original_image_file.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0045_media_original_image_file.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0046_auto_20160615_1038.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0046_auto_20160615_1038.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0047_media_video_file.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0047_media_video_file.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0048_auto_20160615_1045.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0048_auto_20160615_1045.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0049_auto_20160713_1127.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0049_auto_20160713_1127.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0050_auto_20160713_1400.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0050_auto_20160713_1400.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0051_auto_20160713_1444.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0051_auto_20160713_1444.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0052_auto_20161117_1622.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0052_auto_20161117_1622.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0053_tweet_post_year.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0053_tweet_post_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0055_re_save_tweets_for_new_html.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0055_re_save_tweets_for_new_html.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0056_add_count_index.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0056_add_count_index.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/migrations/0057_alter_account_access_token_and_more.py` & `django-ditto-3.2.1/ditto/twitter/migrations/0057_alter_account_access_token_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/models.py` & `django-ditto-3.2.1/ditto/twitter/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,17 +603,17 @@
     def is_reply(self):
         return self.in_reply_to_screen_name != ""
 
     @property
     def in_reply_to_url(self):
         "If it's a reply, the link to the tweet replied to."
         if self.is_reply:
-            return "https://twitter.com/{}/status/{}".format(
-                self.in_reply_to_screen_name,
-                self.in_reply_to_status_id,
+            return (
+                f"https://twitter.com/{self.in_reply_to_screen_name}/"
+                f"status/{self.in_reply_to_status_id}"
             )
         else:
             return ""
 
     @property
     def place(self):
         return ", ".join(
```

### Comparing `django-ditto-3.2.0/ditto/twitter/templates/twitter/account_favorite_list.html` & `django-ditto-3.2.1/ditto/twitter/templates/twitter/account_favorite_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/templates/twitter/favorite_list.html` & `django-ditto-3.2.1/ditto/twitter/templates/twitter/favorite_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/templates/twitter/home.html` & `django-ditto-3.2.1/ditto/twitter/templates/twitter/home.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/annual_tweet_counts.html` & `django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/annual_tweet_counts.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/media.html` & `django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/media.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/nav_tabs.html` & `django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/nav_tabs.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/tweet.html` & `django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/tweet.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/tweet_list.html` & `django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/tweet_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/templates/twitter/includes/user.html` & `django-ditto-3.2.1/ditto/twitter/templates/twitter/includes/user.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/templates/twitter/tweet_detail.html` & `django-ditto-3.2.1/ditto/twitter/templates/twitter/tweet_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/templates/twitter/user_detail.html` & `django-ditto-3.2.1/ditto/twitter/templates/twitter/user_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/templatetags/ditto_twitter.py` & `django-ditto-3.2.1/ditto/twitter/templatetags/ditto_twitter.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/urls.py` & `django-ditto-3.2.1/ditto/twitter/urls.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/utils.py` & `django-ditto-3.2.1/ditto/twitter/utils.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/ditto/twitter/views.py` & `django-ditto-3.2.1/ditto/twitter/views.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/django_ditto.egg-info/PKG-INFO` & `django-ditto-3.2.1/django_ditto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ditto
-Version: 3.2.0
+Version: 3.2.1
 Summary: A Django app to copy stuff from your accounts on Flickr, Last.fm, Pinboard and Twitter.
 Home-page: https://github.com/philgyford/django-ditto
 Author: Phil Gyford
 Author-email: phil@gyford.com
 License: MIT
 Project-URL: Blog posts, https://www.gyford.com/phil/writing/tags/django-ditto/
 Project-URL: Bug Reports, https://github.com/philgyford/django-ditto/issues
```

### Comparing `django-ditto-3.2.0/django_ditto.egg-info/SOURCES.txt` & `django-ditto-3.2.1/django_ditto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/pyproject.toml` & `django-ditto-3.2.1/pyproject.toml`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 omit = ["*/migrations/*.py"]
 
 [tool.ruff]
 extend-exclude = [
   "*/migrations/*",
 ]
 line-length = 88
+target-version = "py39"
+
+[tool.ruff.lint]
+ignore = []
 select = [
   # Reference: https://docs.astral.sh/ruff/rules/
   "B",    # flake8-bugbear
   "E",    # pycodestyle
   "F",    # Pyflakes
   "G",    # flake8-logging-format
   "I",    # isort
@@ -32,11 +36,7 @@
   "SIM",  # flake8-simplify
   "T20",  # flake8-print
   "TID",  # flake8-tidy-imports
   "UP",   # pyupgrade
   "RUF100", # unused-noqa
   "RUF200", # invalid-pyproject-toml
 ]
-target-version = "py39"
-
-[tool.ruff.lint]
-ignore = []
```

### Comparing `django-ditto-3.2.0/setup.py` & `django-ditto-3.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.2.0/tox.ini` & `django-ditto-3.2.1/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tox]
 ; Minimum version of Tox
 minversion = 1.8
 
 envlist =
     ruff
     py39-django{41,42}
-    py310-django{41,42,50,main}
-    py311-django{41,42,50,main}
-    py312-django{42,50,main}
+    py310-django{41,42,50}
+    py311-django{41,42,50}
+    py312-django{42,50}
 
 [gh-actions]
 ; Maps GitHub Actions python version numbers to tox env vars:
 python =
     3.9: py39
     3.10: py310
     3.11: py311
@@ -49,8 +49,8 @@
     ; would run that single test (in all environments)
     coverage run --branch --source=ditto --omit=*/migrations/*.py {envbindir}/django-admin test {posargs:}
     coverage report -m
 
 [testenv:ruff]
 skip_install = true
 deps = ruff
-commands = ruff check {posargs:--show-source .}
+commands = ruff check {posargs:--output-format=full .}
```

