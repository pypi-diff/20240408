# Comparing `tmp/QWeb-3.1.0.tar.gz` & `tmp/QWeb-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QWeb-3.1.0.tar", last modified: Fri Jan 26 12:45:34 2024, max compression
+gzip compressed data, was "QWeb-3.2.0.tar", last modified: Fri Mar  8 12:06:59 2024, max compression
```

## Comparing `QWeb-3.1.0.tar` & `QWeb-3.2.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-01-26 12:45:34.546387 QWeb-3.1.0/
--rw-rw-rw-   0        0        0    11558 2021-09-04 19:02:10.000000 QWeb-3.1.0/LICENSE
--rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11340 2024-01-26 12:45:34.547850 QWeb-3.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-01-26 12:45:34.553188 QWeb-3.1.0/QWeb/
--rw-rw-rw-   0        0        0    16564 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/__init__.py
--rw-rw-rw-   0        0        0     2283 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/__main__.py
--rw-rw-rw-   0        0        0      519 2024-01-26 12:45:34.553188 QWeb-3.1.0/QWeb/_version.py
--rw-rw-rw-   0        0        0     1408 2023-12-20 13:58:51.000000 QWeb-3.1.0/QWeb/custom_config.py
-drwxrwxrwx   0        0        0        0 2024-01-26 12:45:34.446411 QWeb-3.1.0/QWeb/internal/
--rw-rw-rw-   0        0        0       64 2021-09-04 19:02:10.000000 QWeb-3.1.0/QWeb/internal/__init__.py
--rw-rw-rw-   0        0        0    21919 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/internal/actions.py
--rw-rw-rw-   0        0        0     3840 2022-06-16 12:12:06.000000 QWeb-3.1.0/QWeb/internal/ajax.py
--rw-rw-rw-   0        0        0     1699 2022-06-16 12:12:06.000000 QWeb-3.1.0/QWeb/internal/alert.py
--rw-rw-rw-   0        0        0     3689 2022-06-16 12:12:06.000000 QWeb-3.1.0/QWeb/internal/blocks.py
-drwxrwxrwx   0        0        0        0 2024-01-26 12:45:34.468041 QWeb-3.1.0/QWeb/internal/browser/
--rw-rw-rw-   0        0        0     5495 2023-04-26 08:15:55.000000 QWeb-3.1.0/QWeb/internal/browser/__init__.py
--rw-rw-rw-   0        0        0     1581 2023-10-20 07:45:42.000000 QWeb-3.1.0/QWeb/internal/browser/android.py
--rw-rw-rw-   0        0        0     3419 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/internal/browser/bs_desktop.py
--rw-rw-rw-   0        0        0     2162 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/internal/browser/bs_mobile.py
--rw-rw-rw-   0        0        0     6161 2023-11-10 09:40:45.000000 QWeb-3.1.0/QWeb/internal/browser/chrome.py
--rw-rw-rw-   0        0        0     4108 2023-10-20 07:45:42.000000 QWeb-3.1.0/QWeb/internal/browser/edge.py
--rw-rw-rw-   0        0        0     4975 2023-10-20 07:45:42.000000 QWeb-3.1.0/QWeb/internal/browser/firefox.py
--rw-rw-rw-   0        0        0     1934 2023-12-20 13:58:51.000000 QWeb-3.1.0/QWeb/internal/browser/safari.py
--rw-rw-rw-   0        0        0     6626 2022-11-22 10:56:24.000000 QWeb-3.1.0/QWeb/internal/checkbox.py
--rw-rw-rw-   0        0        0     4118 2022-06-16 12:12:06.000000 QWeb-3.1.0/QWeb/internal/config.py
--rw-rw-rw-   0        0        0     4379 2022-06-16 12:12:06.000000 QWeb-3.1.0/QWeb/internal/config_defaults.py
--rw-rw-rw-   0        0        0     1294 2022-11-22 10:56:24.000000 QWeb-3.1.0/QWeb/internal/cookies.py
--rw-rw-rw-   0        0        0     9346 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/internal/decorators.py
--rw-rw-rw-   0        0        0     5613 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/internal/download.py
--rw-rw-rw-   0        0        0     3143 2023-10-20 07:45:42.000000 QWeb-3.1.0/QWeb/internal/dragdrop.py
--rw-rw-rw-   0        0        0     7808 2022-12-12 14:30:56.000000 QWeb-3.1.0/QWeb/internal/dropdown.py
--rw-rw-rw-   0        0        0    29245 2023-12-20 13:58:51.000000 QWeb-3.1.0/QWeb/internal/element.py
--rw-rw-rw-   0        0        0     3087 2022-06-16 12:12:06.000000 QWeb-3.1.0/QWeb/internal/exceptions.py
--rw-rw-rw-   0        0        0     3463 2022-12-09 08:03:29.000000 QWeb-3.1.0/QWeb/internal/file.py
--rw-rw-rw-   0        0        0    11931 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/internal/frame.py
--rw-rw-rw-   0        0        0     1960 2023-09-12 08:26:02.000000 QWeb-3.1.0/QWeb/internal/frame_checker.py
--rw-rw-rw-   0        0        0    20876 2023-12-20 13:58:51.000000 QWeb-3.1.0/QWeb/internal/icon.py
--rw-rw-rw-   0        0        0    11050 2023-08-02 09:59:23.000000 QWeb-3.1.0/QWeb/internal/input_.py
--rw-rw-rw-   0        0        0     7245 2023-12-15 13:19:14.000000 QWeb-3.1.0/QWeb/internal/input_handler.py
--rw-rw-rw-   0        0        0    21104 2023-09-12 08:44:36.000000 QWeb-3.1.0/QWeb/internal/javascript.py
--rw-rw-rw-   0        0        0     9479 2022-11-22 10:56:24.000000 QWeb-3.1.0/QWeb/internal/lists.py
--rw-rw-rw-   0        0        0     3194 2022-06-16 12:12:06.000000 QWeb-3.1.0/QWeb/internal/meas.py
--rw-rw-rw-   0        0        0      833 2022-06-16 12:12:06.000000 QWeb-3.1.0/QWeb/internal/platform.py
--rw-rw-rw-   0        0        0    13395 2023-09-05 13:39:03.000000 QWeb-3.1.0/QWeb/internal/screenshot.py
--rw-rw-rw-   0        0        0     6850 2022-06-16 12:12:07.000000 QWeb-3.1.0/QWeb/internal/search_strategy.py
--rw-rw-rw-   0        0        0     8673 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/internal/secrets.py
--rw-rw-rw-   0        0        0    16706 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/internal/table.py
--rw-rw-rw-   0        0        0    16852 2023-09-05 13:39:03.000000 QWeb-3.1.0/QWeb/internal/text.py
--rw-rw-rw-   0        0        0     1411 2022-06-16 12:12:07.000000 QWeb-3.1.0/QWeb/internal/user.py
--rw-rw-rw-   0        0        0    13488 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/internal/util.py
--rw-rw-rw-   0        0        0     4423 2022-06-16 12:12:07.000000 QWeb-3.1.0/QWeb/internal/window.py
--rw-rw-rw-   0        0        0     3321 2022-06-16 12:12:07.000000 QWeb-3.1.0/QWeb/internal/xhr.py
-drwxrwxrwx   0        0        0        0 2024-01-26 12:45:34.543201 QWeb-3.1.0/QWeb/keywords/
--rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.1.0/QWeb/keywords/__init__.py
--rw-rw-rw-   0        0        0     4238 2022-12-09 08:03:37.000000 QWeb-3.1.0/QWeb/keywords/ajax.py
--rw-rw-rw-   0        0        0     4920 2022-06-16 12:12:07.000000 QWeb-3.1.0/QWeb/keywords/alert.py
--rw-rw-rw-   0        0        0     5750 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/keywords/blocks.py
--rw-rw-rw-   0        0        0    24181 2023-12-20 13:58:51.000000 QWeb-3.1.0/QWeb/keywords/browser.py
--rw-rw-rw-   0        0        0    12960 2022-06-16 12:12:07.000000 QWeb-3.1.0/QWeb/keywords/checkbox.py
--rw-rw-rw-   0        0        0    36464 2023-11-13 08:47:02.000000 QWeb-3.1.0/QWeb/keywords/config.py
--rw-rw-rw-   0        0        0     2851 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/keywords/cookies.py
--rw-rw-rw-   0        0        0     2500 2022-06-16 12:12:07.000000 QWeb-3.1.0/QWeb/keywords/debug.py
--rw-rw-rw-   0        0        0     3998 2022-06-16 12:12:07.000000 QWeb-3.1.0/QWeb/keywords/download.py
--rw-rw-rw-   0        0        0     6268 2022-11-22 10:56:24.000000 QWeb-3.1.0/QWeb/keywords/dragdrop.py
--rw-rw-rw-   0        0        0    14590 2022-06-16 12:12:07.000000 QWeb-3.1.0/QWeb/keywords/dropdown.py
--rw-rw-rw-   0        0        0    27614 2023-09-05 13:39:03.000000 QWeb-3.1.0/QWeb/keywords/element.py
--rw-rw-rw-   0        0        0    12455 2023-09-05 13:39:03.000000 QWeb-3.1.0/QWeb/keywords/file.py
--rw-rw-rw-   0        0        0     4612 2022-06-16 12:12:07.000000 QWeb-3.1.0/QWeb/keywords/frame.py
--rw-rw-rw-   0        0        0     8675 2023-03-23 15:17:25.000000 QWeb-3.1.0/QWeb/keywords/icon.py
--rw-rw-rw-   0        0        0    38042 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/keywords/input_.py
--rw-rw-rw-   0        0        0     1887 2023-12-20 13:58:51.000000 QWeb-3.1.0/QWeb/keywords/javascript.py
--rw-rw-rw-   0        0        0     8703 2022-11-21 09:35:10.000000 QWeb-3.1.0/QWeb/keywords/lists.py
--rw-rw-rw-   0        0        0     2968 2023-12-20 13:58:51.000000 QWeb-3.1.0/QWeb/keywords/screenshot.py
--rw-rw-rw-   0        0        0     8486 2022-06-16 12:12:07.000000 QWeb-3.1.0/QWeb/keywords/search_strategy.py
--rw-rw-rw-   0        0        0    18917 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/keywords/table.py
--rw-rw-rw-   0        0        0    67037 2024-01-26 10:08:26.000000 QWeb-3.1.0/QWeb/keywords/text.py
--rw-rw-rw-   0        0        0    17323 2023-12-20 13:58:51.000000 QWeb-3.1.0/QWeb/keywords/window.py
-drwxrwxrwx   0        0        0        0 2024-01-26 12:45:34.352846 QWeb-3.1.0/QWeb.egg-info/
--rw-rw-rw-   0        0        0    11340 2024-01-26 12:45:34.000000 QWeb-3.1.0/QWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2024-01-26 12:45:34.000000 QWeb-3.1.0/QWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-26 12:45:34.000000 QWeb-3.1.0/QWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-09-08 09:34:25.000000 QWeb-3.1.0/QWeb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      351 2024-01-26 12:45:34.000000 QWeb-3.1.0/QWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-01-26 12:45:34.000000 QWeb-3.1.0/QWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10600 2023-10-20 07:45:42.000000 QWeb-3.1.0/README.md
--rw-rw-rw-   0        0        0     1209 2024-01-26 12:45:34.553188 QWeb-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2532 2024-01-26 10:08:26.000000 QWeb-3.1.0/setup.py
--rw-rw-rw-   0        0        0    70433 2021-09-04 19:02:10.000000 QWeb-3.1.0/versioneer.py
+drwxrwxrwx   0        0        0        0 2024-03-08 12:06:59.851325 QWeb-3.2.0/
+-rw-rw-rw-   0        0        0    11558 2021-09-04 19:02:10.000000 QWeb-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11340 2024-03-08 12:06:59.852054 QWeb-3.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-03-08 12:06:59.856782 QWeb-3.2.0/QWeb/
+-rw-rw-rw-   0        0        0    16564 2024-01-26 10:08:26.000000 QWeb-3.2.0/QWeb/__init__.py
+-rw-rw-rw-   0        0        0     2283 2024-01-26 10:08:26.000000 QWeb-3.2.0/QWeb/__main__.py
+-rw-rw-rw-   0        0        0      519 2024-03-08 12:06:59.856782 QWeb-3.2.0/QWeb/_version.py
+-rw-rw-rw-   0        0        0     1408 2023-12-20 13:58:51.000000 QWeb-3.2.0/QWeb/custom_config.py
+drwxrwxrwx   0        0        0        0 2024-03-08 12:06:59.757813 QWeb-3.2.0/QWeb/internal/
+-rw-rw-rw-   0        0        0       64 2021-09-04 19:02:10.000000 QWeb-3.2.0/QWeb/internal/__init__.py
+-rw-rw-rw-   0        0        0    21809 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/internal/actions.py
+-rw-rw-rw-   0        0        0     3840 2022-06-16 12:12:06.000000 QWeb-3.2.0/QWeb/internal/ajax.py
+-rw-rw-rw-   0        0        0     1699 2022-06-16 12:12:06.000000 QWeb-3.2.0/QWeb/internal/alert.py
+-rw-rw-rw-   0        0        0     3689 2022-06-16 12:12:06.000000 QWeb-3.2.0/QWeb/internal/blocks.py
+drwxrwxrwx   0        0        0        0 2024-03-08 12:06:59.779175 QWeb-3.2.0/QWeb/internal/browser/
+-rw-rw-rw-   0        0        0     5495 2023-04-26 08:15:55.000000 QWeb-3.2.0/QWeb/internal/browser/__init__.py
+-rw-rw-rw-   0        0        0     1581 2023-10-20 07:45:42.000000 QWeb-3.2.0/QWeb/internal/browser/android.py
+-rw-rw-rw-   0        0        0     3419 2024-01-26 10:08:26.000000 QWeb-3.2.0/QWeb/internal/browser/bs_desktop.py
+-rw-rw-rw-   0        0        0     2162 2024-01-26 10:08:26.000000 QWeb-3.2.0/QWeb/internal/browser/bs_mobile.py
+-rw-rw-rw-   0        0        0     6161 2023-11-10 09:40:45.000000 QWeb-3.2.0/QWeb/internal/browser/chrome.py
+-rw-rw-rw-   0        0        0     4108 2023-10-20 07:45:42.000000 QWeb-3.2.0/QWeb/internal/browser/edge.py
+-rw-rw-rw-   0        0        0     4975 2023-10-20 07:45:42.000000 QWeb-3.2.0/QWeb/internal/browser/firefox.py
+-rw-rw-rw-   0        0        0     1934 2023-12-20 13:58:51.000000 QWeb-3.2.0/QWeb/internal/browser/safari.py
+-rw-rw-rw-   0        0        0     6626 2022-11-22 10:56:24.000000 QWeb-3.2.0/QWeb/internal/checkbox.py
+-rw-rw-rw-   0        0        0     4329 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/internal/config.py
+-rw-rw-rw-   0        0        0     4379 2022-06-16 12:12:06.000000 QWeb-3.2.0/QWeb/internal/config_defaults.py
+-rw-rw-rw-   0        0        0     1294 2022-11-22 10:56:24.000000 QWeb-3.2.0/QWeb/internal/cookies.py
+-rw-rw-rw-   0        0        0     9346 2024-02-07 14:33:28.000000 QWeb-3.2.0/QWeb/internal/decorators.py
+-rw-rw-rw-   0        0        0     5613 2024-01-26 10:08:26.000000 QWeb-3.2.0/QWeb/internal/download.py
+-rw-rw-rw-   0        0        0     3143 2023-10-20 07:45:42.000000 QWeb-3.2.0/QWeb/internal/dragdrop.py
+-rw-rw-rw-   0        0        0     7808 2022-12-12 14:30:56.000000 QWeb-3.2.0/QWeb/internal/dropdown.py
+-rw-rw-rw-   0        0        0    29790 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/internal/element.py
+-rw-rw-rw-   0        0        0     3087 2022-06-16 12:12:06.000000 QWeb-3.2.0/QWeb/internal/exceptions.py
+-rw-rw-rw-   0        0        0     3463 2022-12-09 08:03:29.000000 QWeb-3.2.0/QWeb/internal/file.py
+-rw-rw-rw-   0        0        0    11924 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/internal/frame.py
+-rw-rw-rw-   0        0        0     1960 2023-09-12 08:26:02.000000 QWeb-3.2.0/QWeb/internal/frame_checker.py
+-rw-rw-rw-   0        0        0    20876 2023-12-20 13:58:51.000000 QWeb-3.2.0/QWeb/internal/icon.py
+-rw-rw-rw-   0        0        0    11050 2023-08-02 09:59:23.000000 QWeb-3.2.0/QWeb/internal/input_.py
+-rw-rw-rw-   0        0        0     7245 2023-12-15 13:19:14.000000 QWeb-3.2.0/QWeb/internal/input_handler.py
+-rw-rw-rw-   0        0        0    21104 2023-09-12 08:44:36.000000 QWeb-3.2.0/QWeb/internal/javascript.py
+-rw-rw-rw-   0        0        0     9479 2022-11-22 10:56:24.000000 QWeb-3.2.0/QWeb/internal/lists.py
+-rw-rw-rw-   0        0        0     3194 2022-06-16 12:12:06.000000 QWeb-3.2.0/QWeb/internal/meas.py
+-rw-rw-rw-   0        0        0      833 2022-06-16 12:12:06.000000 QWeb-3.2.0/QWeb/internal/platform.py
+-rw-rw-rw-   0        0        0    13395 2023-09-05 13:39:03.000000 QWeb-3.2.0/QWeb/internal/screenshot.py
+-rw-rw-rw-   0        0        0     7250 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/internal/search_strategy.py
+-rw-rw-rw-   0        0        0     8673 2024-01-26 10:08:26.000000 QWeb-3.2.0/QWeb/internal/secrets.py
+-rw-rw-rw-   0        0        0    17095 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/internal/table.py
+-rw-rw-rw-   0        0        0    16945 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/internal/text.py
+-rw-rw-rw-   0        0        0     1411 2022-06-16 12:12:07.000000 QWeb-3.2.0/QWeb/internal/user.py
+-rw-rw-rw-   0        0        0    13488 2024-02-12 10:35:50.000000 QWeb-3.2.0/QWeb/internal/util.py
+-rw-rw-rw-   0        0        0     4423 2022-06-16 12:12:07.000000 QWeb-3.2.0/QWeb/internal/window.py
+-rw-rw-rw-   0        0        0     3321 2022-06-16 12:12:07.000000 QWeb-3.2.0/QWeb/internal/xhr.py
+drwxrwxrwx   0        0        0        0 2024-03-08 12:06:59.848633 QWeb-3.2.0/QWeb/keywords/
+-rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.2.0/QWeb/keywords/__init__.py
+-rw-rw-rw-   0        0        0     4238 2022-12-09 08:03:37.000000 QWeb-3.2.0/QWeb/keywords/ajax.py
+-rw-rw-rw-   0        0        0     4920 2022-06-16 12:12:07.000000 QWeb-3.2.0/QWeb/keywords/alert.py
+-rw-rw-rw-   0        0        0     5750 2024-01-26 10:08:26.000000 QWeb-3.2.0/QWeb/keywords/blocks.py
+-rw-rw-rw-   0        0        0    24178 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/keywords/browser.py
+-rw-rw-rw-   0        0        0    12960 2022-06-16 12:12:07.000000 QWeb-3.2.0/QWeb/keywords/checkbox.py
+-rw-rw-rw-   0        0        0    37939 2024-03-08 11:59:59.000000 QWeb-3.2.0/QWeb/keywords/config.py
+-rw-rw-rw-   0        0        0     3053 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/keywords/cookies.py
+-rw-rw-rw-   0        0        0     2500 2022-06-16 12:12:07.000000 QWeb-3.2.0/QWeb/keywords/debug.py
+-rw-rw-rw-   0        0        0     3998 2022-06-16 12:12:07.000000 QWeb-3.2.0/QWeb/keywords/download.py
+-rw-rw-rw-   0        0        0     6268 2022-11-22 10:56:24.000000 QWeb-3.2.0/QWeb/keywords/dragdrop.py
+-rw-rw-rw-   0        0        0    14590 2022-06-16 12:12:07.000000 QWeb-3.2.0/QWeb/keywords/dropdown.py
+-rw-rw-rw-   0        0        0    27838 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/keywords/element.py
+-rw-rw-rw-   0        0        0    12455 2023-09-05 13:39:03.000000 QWeb-3.2.0/QWeb/keywords/file.py
+-rw-rw-rw-   0        0        0     4612 2022-06-16 12:12:07.000000 QWeb-3.2.0/QWeb/keywords/frame.py
+-rw-rw-rw-   0        0        0     8675 2023-03-23 15:17:25.000000 QWeb-3.2.0/QWeb/keywords/icon.py
+-rw-rw-rw-   0        0        0    38042 2024-01-26 10:08:26.000000 QWeb-3.2.0/QWeb/keywords/input_.py
+-rw-rw-rw-   0        0        0     1887 2023-12-20 13:58:51.000000 QWeb-3.2.0/QWeb/keywords/javascript.py
+-rw-rw-rw-   0        0        0     8703 2022-11-21 09:35:10.000000 QWeb-3.2.0/QWeb/keywords/lists.py
+-rw-rw-rw-   0        0        0     2968 2023-12-20 13:58:51.000000 QWeb-3.2.0/QWeb/keywords/screenshot.py
+-rw-rw-rw-   0        0        0     8486 2022-06-16 12:12:07.000000 QWeb-3.2.0/QWeb/keywords/search_strategy.py
+-rw-rw-rw-   0        0        0    20611 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/keywords/table.py
+-rw-rw-rw-   0        0        0    67923 2024-03-08 11:29:33.000000 QWeb-3.2.0/QWeb/keywords/text.py
+-rw-rw-rw-   0        0        0    17323 2023-12-20 13:58:51.000000 QWeb-3.2.0/QWeb/keywords/window.py
+drwxrwxrwx   0        0        0        0 2024-03-08 12:06:59.598890 QWeb-3.2.0/QWeb.egg-info/
+-rw-rw-rw-   0        0        0    11340 2024-03-08 12:06:59.000000 QWeb-3.2.0/QWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2024-03-08 12:06:59.000000 QWeb-3.2.0/QWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-08 12:06:59.000000 QWeb-3.2.0/QWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-09-08 09:34:25.000000 QWeb-3.2.0/QWeb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      351 2024-03-08 12:06:59.000000 QWeb-3.2.0/QWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-03-08 12:06:59.000000 QWeb-3.2.0/QWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10600 2023-10-20 07:45:42.000000 QWeb-3.2.0/README.md
+-rw-rw-rw-   0        0        0     1209 2024-03-08 12:06:59.855813 QWeb-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2532 2024-01-26 10:08:26.000000 QWeb-3.2.0/setup.py
+-rw-rw-rw-   0        0        0    70433 2021-09-04 19:02:10.000000 QWeb-3.2.0/versioneer.py
```

### Comparing `QWeb-3.1.0/LICENSE` & `QWeb-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/PKG-INFO` & `QWeb-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QWeb
-Version: 3.1.0
+Version: 3.2.0
 Summary: Keyword driven automation for the web
 Home-page: https://github.com/qentinelqi/qweb/
 Author: Qentinel Group
 Author-email: libraries@qentinel.com
 License: Apache License 2.0
 Keywords: test automation robot framework
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `QWeb-3.1.0/QWeb/__init__.py` & `QWeb-3.2.0/QWeb/__init__.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/__main__.py` & `QWeb-3.2.0/QWeb/__main__.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/custom_config.py` & `QWeb-3.2.0/QWeb/custom_config.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/actions.py` & `QWeb-3.2.0/QWeb/internal/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             input_element.send_keys(kwargs.get('key', input_handler.line_break_key))
         except ElementNotInteractableException:
             # this can happen with firefox for shadow dom elements
             # log, but do not fail the test case as value was written correctly
             logger.debug("Could not send line break key to input")
     else:
         input_handler.write(input_element, input_text, **kwargs)
-    logger.debug('Preferred text: "{}"'.format(input_text))
+    logger.debug(f'Preferred text: "{input_text}"')
 
 
 @decorators.timeout_decorator_for_actions
 def compare_input_values(
         input_element: WebElement,
         expected_value: str,
         timeout: int,  # pylint: disable=unused-argument
@@ -87,19 +87,20 @@
         real_value = input_value(input_element, timeout="0.5s", **kwargs)
         if expected_value == real_value:  # Full match
             return True
         real_value = util.get_substring(real_value, **kwargs)
         expected_value = str(util.get_substring(expected_value, **kwargs))
     except QWebValueError:
         real_value = ""
-    logger.debug('Real value: {}, expected value {}'.format(real_value, expected_value))
+    logger.debug(f'Real value: {real_value}, expected value {expected_value}')
     if fnmatch.fnmatch(str(real_value).strip(), expected_value):
         return True
-    raise QWebValueMismatchError('Expected value "{}" didn\'t match to real value "{}"'.format(
-        expected_value, real_value))
+    raise QWebValueMismatchError(
+        f"""Expected value "{expected_value}" didn\'t match to real value "{real_value}\""""
+    )
 
 
 @decorators.timeout_decorator_for_actions
 def input_value(input_element: WebElement, timeout: int, **kwargs: Any) -> str:
     blind = util.par2bool(kwargs.get('blind', CONFIG['BlindReturn']))
     shadow_dom = CONFIG['ShadowDOM']
 
@@ -107,15 +108,15 @@
         value = input_element.get_attribute('innerText')
     else:
         value = input_element.get_attribute('value')
     if value:
         return value.strip()
     if blind:
         return ''
-    raise QWebValueError('No Value found after {} sec'.format(timeout))
+    raise QWebValueError(f'No Value found after {timeout} sec')
 
 
 @decorators.timeout_decorator_for_actions
 def scroll(web_element: WebElement, timeout: int) -> None:  # pylint: disable=unused-argument
     javascript.execute_javascript('arguments[0].scrollIntoView();', web_element)
 
 
@@ -142,15 +143,15 @@
                     double_click(web_element)
             elif js:
                 js_click(web_element)
             else:
                 wd_click(web_element, **kwargs)
                 logger.debug('element clicked')
         except WebDriverException as e:
-            logger.info('Got {} when tried to click.'.format(e))
+            logger.info(f'Got {e} when tried to click.')
             if 'text' not in kwargs:
                 raise e
         if 'text' in kwargs:
             logger.debug('button clicked. Verifying expected condition..')
             try:
                 if text_appearance(kwargs['text'],
                                    text_appear=text_appear,
@@ -283,16 +284,17 @@
 
 
 @decorators.timeout_decorator_for_actions
 def is_not_in_dropdown(select: Select, option: str, **kwargs: Any) -> bool:
     """"Verifies that the selected option is not in the dropdown list"""
     option_list = get_select_options(select, **kwargs)
     if option in option_list:
-        raise QWebValueError("Found the value {} from the dropdown menu: {}.".format(
-            option, option_list))
+        raise QWebValueError(
+            f"Found the value {option} from the dropdown menu: {option_list}."
+        )
     return True
 
 
 @decorators.timeout_decorator_for_actions
 def get_selected_value(
         select: Select,  # pylint: disable=unused-argument
         expected: Optional[str] = None,
@@ -310,16 +312,17 @@
     selected = [ele.text for ele in sel_elems]
 
     txt_selected = ",".join(selected)
 
     if expected:
         if expected in selected:
             return True
-        raise QWebValueMismatchError('Expected value "{}" didn\'t match to real value "{}".'.format(
-            expected, txt_selected))
+        raise QWebValueMismatchError(
+            f"""Expected value "{expected}" didn\'t match to real value "{txt_selected}"."""
+        )
     return txt_selected
 
 
 @decorators.timeout_decorator_for_actions
 def get_select_options(
         select: Select,  # pylint: disable=unused-argument
         expected: Optional[str] = None,
@@ -327,15 +330,15 @@
     options = select.options
     if expected:
         for option in options:
             logger.debug(option.text)
             if fnmatch.fnmatch(expected, option.text):
                 return True
         raise QWebValueMismatchError(
-            'Expected value "{}" not found from selectable options'.format(expected))
+            f'Expected value "{expected}" not found from selectable options')
     # parse all options to a list and return it
     option_list = []
     for option in options:
         option_list.append(option.text)
     return option_list
 
 
@@ -386,23 +389,23 @@
 @decorators.timeout_decorator_for_actions
 def get_element_text(web_element: WebElement, expected=None, timeout: int = 0) -> Union[bool, str]:  # pylint: disable=unused-argument
     real_text = web_element.text.strip()
     if expected is not None:
         try:
             return _compare_texts(real_text, expected.strip(), timeout)
         except QWebValueMismatchError as e:
-            raise QWebValueError('Expected {}, found {}'.format(expected, real_text)) from e
+            raise QWebValueError(f'Expected {expected}, found {real_text}') from e
     if real_text is not None:
         return real_text
     raise QWebValueMismatchError('Text not found')
 
 
 def _compare_texts(text_to_compare: str, expected: str, timeout: int) -> bool:  # pylint: disable=unused-argument
     if fnmatch.fnmatch(text_to_compare, expected) is False:
-        raise QWebValueMismatchError('Expected {0}, found {1}'.format(expected, text_to_compare))
+        raise QWebValueMismatchError(f'Expected {expected}, found {text_to_compare}')
     return True
 
 
 def _ends_with_line_break(input_text: str) -> bool:
     line_break = ('\n', '\ue007', '\t', '\ue004')
     return input_text.endswith(line_break)
 
@@ -443,75 +446,82 @@
           } else {
             return getScrollParent(node.parentNode);
           }
         }
         return getScrollParent(arguments[0]);
     """
     js_element_position = "return arguments[0].scrollTop;"
-    js_element_scroll = "arguments[0].scrollBy(0, {})".format(scroll_length or '1000')
+    js_element_scroll = f"arguments[0].scrollBy(0, {scroll_length or '1000'})"
     web_element = internal_text.get_element_by_locator_text(locator, anchor)
     scrollable_element = javascript.execute_javascript(js_get_parent_element, web_element)
     current_pos = javascript.execute_javascript(js_element_position, scrollable_element)
     old_pos = None
     start = time.time()
     if not slow_mode:
         while not visible and old_pos != current_pos and time.time() < float(timeout) + start:
             old_pos = javascript.execute_javascript(js_element_position, scrollable_element)
             javascript.execute_javascript(js_element_scroll, scrollable_element)
             time.sleep(.5)
             current_pos = javascript.execute_javascript(js_element_position, scrollable_element)
             visible = internal_text.get_element_by_locator_text(text_to_find,
                                                                 allow_non_existent=True)
-            logger.info('Old pos: {}\nNew pos: {}\nVisible: {}'.format(
-                old_pos, current_pos, visible),
-                        also_console=True)
+            logger.info(
+                f'Old pos: {old_pos}\nNew pos: {current_pos}\nVisible: {visible}',
+                also_console=True,
+            )
     else:
-        logger.info('\nSlow mode is on, execution will only stop if the text "{}" is found or if '
-                    'the timeout is reached.'.format(text_to_find),
-                    also_console=True)
+        logger.info(
+            f'\nSlow mode is on, execution will only stop if the text "{text_to_find}" '
+            ' is found or if the timeout is reached.',
+            also_console=True,
+        )
         while not visible and time.time() < float(timeout) + start:
             javascript.execute_javascript(js_element_scroll, scrollable_element)
             time.sleep(.5)
             visible = internal_text.get_element_by_locator_text(text_to_find,
                                                                 allow_non_existent=True)
-            logger.info('\nVisible: {}'.format(visible), also_console=True)
+            logger.info(f'\nVisible: {visible}', also_console=True)
     if visible:
         return
-    raise QWebTextNotFoundError('Text {} not found.'.format(text_to_find))
+    raise QWebTextNotFoundError(f'Text {text_to_find} not found.')
 
 
 def scroll_dynamic_web_page(text_to_find: str, scroll_length: Optional[Union[int, str]],
                             slow_mode: bool, timeout: Union[int, float, str]) -> bool:
     visible = None
     js_browser_height = "return window.innerHeight"
     height = javascript.execute_javascript(js_browser_height)  # Length of one scroll
     js_current_pos = "return window.pageYOffset;"
-    js_scroll = 'window.scrollBy(0,{})'.format(scroll_length or height)
+    js_scroll = f'window.scrollBy(0,{scroll_length or height})'
     current_pos = javascript.execute_javascript(js_current_pos)
     old_pos = None
     start = time.time()
     if not slow_mode:
         while not visible and old_pos != current_pos and time.time() < float(timeout) + start:
             old_pos = javascript.execute_javascript(js_current_pos)
             javascript.execute_javascript(js_scroll)
             time.sleep(.5)
             current_pos = javascript.execute_javascript(js_current_pos)
             visible = internal_text.get_element_by_locator_text(text_to_find,
                                                                 allow_non_existent=True)
-            logger.info('\nOld pos: {}\nCurrent pos: {}\nVisible: {}'.format(
-                old_pos, current_pos, visible),
-                        also_console=True)
+            logger.info(
+                f'\nOld pos: {old_pos}\nCurrent pos: {current_pos}\nVisible: {visible}',
+                also_console=True,
+            )
     else:
-        logger.info('\nSlow mode is on, execution will only stop if the text "{}" is found or if '
-                    'the timeout is reached.'.format(text_to_find),
-                    also_console=True)
+        logger.info(
+            '\nSlow mode is on, execution will only stop if '
+            f'the text "{text_to_find}" is found or if the timeout is reached.',
+            also_console=True,
+        )
         while not visible and time.time() < float(timeout) + start:
             javascript.execute_javascript(js_scroll)
             time.sleep(.5)
             visible = internal_text.get_element_by_locator_text(text_to_find,
                                                                 allow_non_existent=True)
-            logger.info('\nVisible: {}'.format(visible), also_console=True)
+            logger.info(f'\nVisible: {visible}', also_console=True)
 
     if visible:
         return True
-    raise QWebTextNotFoundError('Could not find text "{}" after scrolling for {} pixels.'.format(
-        text_to_find, current_pos))
+    raise QWebTextNotFoundError(
+        f'Could not find text "{text_to_find}" after scrolling for {current_pos} pixels.'
+    )
```

### Comparing `QWeb-3.1.0/QWeb/internal/ajax.py` & `QWeb-3.2.0/QWeb/internal/ajax.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/alert.py` & `QWeb-3.2.0/QWeb/internal/alert.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/blocks.py` & `QWeb-3.2.0/QWeb/internal/blocks.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/browser/__init__.py` & `QWeb-3.2.0/QWeb/internal/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/browser/android.py` & `QWeb-3.2.0/QWeb/internal/browser/android.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/browser/bs_desktop.py` & `QWeb-3.2.0/QWeb/internal/browser/bs_desktop.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/browser/bs_mobile.py` & `QWeb-3.2.0/QWeb/internal/browser/bs_mobile.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/browser/chrome.py` & `QWeb-3.2.0/QWeb/internal/browser/chrome.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/browser/edge.py` & `QWeb-3.2.0/QWeb/internal/browser/edge.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/browser/firefox.py` & `QWeb-3.2.0/QWeb/internal/browser/firefox.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/browser/safari.py` & `QWeb-3.2.0/QWeb/internal/browser/safari.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/checkbox.py` & `QWeb-3.2.0/QWeb/internal/checkbox.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/config.py` & `QWeb-3.2.0/QWeb/internal/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,7 +98,14 @@
 
     @staticmethod
     def _clean_string(string_value: str) -> str:
         dropped_chars_dict = dict.fromkeys(Config.DROPPED_DELIMITER_CHARS)
         trans_table = str.maketrans(dropped_chars_dict)
         _string_value = string_value.lower().translate(trans_table)
         return _string_value
+
+    def enforce_direction(self) -> bool:
+        search_direction = self.get_value("SearchDirection")
+        if search_direction:
+            return search_direction.endswith("!")
+
+        return False
```

### Comparing `QWeb-3.1.0/QWeb/internal/config_defaults.py` & `QWeb-3.2.0/QWeb/internal/config_defaults.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/cookies.py` & `QWeb-3.2.0/QWeb/internal/cookies.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/decorators.py` & `QWeb-3.2.0/QWeb/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/download.py` & `QWeb-3.2.0/QWeb/internal/download.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/dragdrop.py` & `QWeb-3.2.0/QWeb/internal/dragdrop.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/dropdown.py` & `QWeb-3.2.0/QWeb/internal/dropdown.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/element.py` & `QWeb-3.2.0/QWeb/internal/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from QWeb.internal import frame
 from QWeb.internal.exceptions import QWebElementNotFoundError, QWebStalingElementError, \
     QWebValueError, QWebSearchingMode
 from QWeb.internal import browser, javascript, util
 from QWeb.internal.config_defaults import CONFIG
 
 ACTIVE_AREA_FUNCTION: Optional[Callable[..., Any]] = None
+DEFAULT_DISTANCE = 1000000.0  # Just some large number
 
 
 def is_enabled(element: WebElement) -> bool:
     """Is the element interactable?
 
     Uses the disabled attribute to determine if form element is enabled or
     not.
@@ -99,15 +100,15 @@
     Returns
     -------
     WebElement
     """
     if not candidate_elements:
         raise QWebElementNotFoundError('No elements visible')
     closest_element_list = []
-    closest_distance = 1000000.0  # Just some large number
+    closest_distance = DEFAULT_DISTANCE
     for candidate_element in candidate_elements:
         element_info = _list_info(candidate_element)
         logger.debug("Measuring distance for: {}".format(element_info))
         if _overlap(locator_element, candidate_element):
             logger.debug('Elements overlap, returning this: {}'.format(element_info))
             return candidate_element
         distance = _calculate_closest_distance(locator_element, candidate_element)
@@ -115,19 +116,25 @@
 
         if abs(distance - closest_distance) < 2:
             closest_element_list.append(candidate_element)
             closest_distance = distance
         elif distance < closest_distance:
             closest_distance = distance
             closest_element_list = [candidate_element]
+    # if search direction is "forced" and closest distance is in default value
+    # then we don't have the element on correct direction from the anchor
+    enforce_direction = CONFIG.enforce_direction()
+    if enforce_direction and closest_distance == DEFAULT_DISTANCE:
+        logger.debug(f'No elements in expected direction {CONFIG.get_value("SearchDirection")}')
+        raise QWebElementNotFoundError("No elements found in enforced direction")
 
     closest_element = _get_closest_ortho_element(locator_element, closest_element_list)
 
-    logger.debug("Closest distance found is {}".format(closest_distance))
-    logger.debug("Closest element is: {}".format(_list_info(closest_element)))
+    logger.debug(f"Closest distance found is {closest_distance}")
+    logger.debug(f"Closest element is: {_list_info(closest_element)}")
     return closest_element
 
 
 def get_unique_element_by_xpath(xpath: str,
                                 index: Union[str, int] = 0,
                                 **kwargs: Any) -> WebElement:
     """Get element if it is needed to be unique.
@@ -356,43 +363,45 @@
     Returns
     -------
     float
     """
     search_direction = CONFIG["SearchDirection"]
     corners_locations1 = _get_corners_locations(element1)
     corners_locations2 = _get_corners_locations(element2)
-    closest_distance = 1000000.0  # Some large number
+    closest_distance = DEFAULT_DISTANCE
     for corner1 in corners_locations1:
         for corner2 in corners_locations2:
             distance = _manhattan_distance(corner1['x'], corner1['y'], corner2['x'], corner2['y'])
             if search_direction != 'closest':
                 # y coordinate goes up downwards on page
                 # small y is above
                 angle = math.degrees(
                     math.atan2(corner2['y'] - corner1['y'], corner2['x'] - corner1['x']))
-            if search_direction == 'down':
+
+            if search_direction in ('down', 'down!'):
                 if not 5 < angle < 175:
                     logger.debug(
                         'Search direction is {} and element is not in arc'.format(search_direction))
-                    distance = 1000000.0
-            elif search_direction == 'up':
+                    distance = DEFAULT_DISTANCE
+            elif search_direction in ('up', 'up!'):
                 if not -175 < angle < -5:
                     logger.debug(
                         'Search direction is {} and element is not in arc'.format(search_direction))
-                    distance = 1000000.0
-            elif search_direction == 'left':
+                    distance = DEFAULT_DISTANCE
+            elif search_direction in ('left', 'left!'):
                 if not abs(angle) > 95:
                     logger.debug(
                         'Search direction is {} and element is not in arc'.format(search_direction))
-                    distance = 1000000.0
-            elif search_direction == 'right':
+                    distance = DEFAULT_DISTANCE
+            elif search_direction in ('right', 'right!'):
                 if not -85 < angle < 85:
                     logger.debug(
                         'Search direction is {} and element is not in arc'.format(search_direction))
-                    distance = 1000000.0
+                    distance = DEFAULT_DISTANCE
+
             if closest_distance > distance > 0:
                 closest_distance = distance
     return closest_distance
 
 
 def _calculate_closest_ortho_distance(element1: WebElement, element2: WebElement) -> float:
     """Returns shortest ortho  distance between locator and candidate element centers
@@ -513,15 +522,15 @@
     list_len = len(element_list)
     # pylint: disable=no-else-return
     if list_len == 1:
         return element_list[0]
     elif list_len == 0:
         raise IndexError
 
-    closest_distance = 1000000.0
+    closest_distance = DEFAULT_DISTANCE
     for candidate_element in element_list:
         distance = _calculate_closest_ortho_distance(locator_element, candidate_element)
         logger.debug("Candidate {}: horizontal distance: {}".format(candidate_element, distance))
         if distance < closest_distance:
             closest_distance = distance
             closest_element = candidate_element
```

### Comparing `QWeb-3.1.0/QWeb/internal/exceptions.py` & `QWeb-3.2.0/QWeb/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/file.py` & `QWeb-3.2.0/QWeb/internal/file.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/frame.py` & `QWeb-3.2.0/QWeb/internal/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             driver.switch_to.default_content()
     timeout = CONFIG['XHRTimeout']
     if timeout.lower() == "none":
         return
     try:
         xhr.wait_xhr(timestr_to_secs(timeout))
     except (WebDriverException, QWebDriverError) as e:
-        logger.info('Unable to check AJAX requests due error: {}'.format(e))
+        logger.debug(f'Unable to check AJAX requests due error: {e}')
 
 
 def get_raw_html() -> str:
     driver = browser.get_current_browser()
     return driver.page_source
```

### Comparing `QWeb-3.1.0/QWeb/internal/frame_checker.py` & `QWeb-3.2.0/QWeb/internal/frame_checker.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/icon.py` & `QWeb-3.2.0/QWeb/internal/icon.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/input_.py` & `QWeb-3.2.0/QWeb/internal/input_.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/input_handler.py` & `QWeb-3.2.0/QWeb/internal/input_handler.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/javascript.py` & `QWeb-3.2.0/QWeb/internal/javascript.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/lists.py` & `QWeb-3.2.0/QWeb/internal/lists.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/meas.py` & `QWeb-3.2.0/QWeb/internal/meas.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/platform.py` & `QWeb-3.2.0/QWeb/internal/platform.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/screenshot.py` & `QWeb-3.2.0/QWeb/internal/screenshot.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/search_strategy.py` & `QWeb-3.2.0/QWeb/internal/search_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------
 from typing import Any
+
 # pylint: disable=line-too-long
 import re
 import string
 
 
 class SearchStrategies:
     ALL_INPUT_ELEMENTS: str = '//input[@type="text" or @type="email" or @type="password" or @type="tel"]|//textarea'
 
     MATCHING_INPUT_ELEMENT: str = '//*[(self::input or self::textarea) and (normalize-space(@placeholder)="{0}" or normalize-space(@value)="{0}")]'
     CONTAINING_INPUT_ELEMENT: str = '//*[(self::input or self::textarea) and (contains(normalize-space(@placeholder),"{0}") or contains(normalize-space(@value),"{0}"))]'
 
-    ACTIVE_AREA_XPATH: str = '//body'
+    ACTIVE_AREA_XPATH: str = "//body"
 
     TEXT_MATCH: str = '//*[not(self::script) and normalize-space(translate(., "\u00a0", " "))="{0}" and not(descendant::*[normalize-space(translate(., "\u00a0", " "))="{0}"])]|//input[(@type="button" or @type="reset" or @type="submit" or @type="checkbox") and normalize-space(translate(@value, "\u00a0", " "))="{0}"]'
 
     CONTAINING_TEXT_MATCH_CASE_SENSITIVE: str = (
         '//*[not(self::script) and contains(normalize-space(translate(., "\u00a0", " ")), "{0}") '
         'and not(descendant::*[contains(normalize-space(translate(., "\u00a0", " ")), "{0}")])]| '
         '//input[(@type="button" or @type="reset" or @type="submit") and contains(normalize-space(translate(@value, "\u00a0", " ")), "{0}")]'
@@ -42,27 +43,27 @@
                             "abcdefghijklmnopqrstuvwxyzäöå"), translate("{0}", "ABCDEFGHIJKLMNOPQRSTUVWXYZÄÖÅ", "abcdefghijklmnopqrstuvwxyzäöå"))  \
                             and not(descendant::*[contains(translate(normalize-space(translate(., "\u00a0", " ")), "ABCDEFGHIJKLMNOPQRSTUVWXYZÄÖÅ", \
                             "abcdefghijklmnopqrstuvwxyzäöå"), translate("{0}", "ABCDEFGHIJKLMNOPQRSTUVWXYZÄÖÅ", "abcdefghijklmnopqrstuvwxyzäöå"))])]| \
                             //input[(@type="button" or @type="reset" or @type="submit") and contains(translate(normalize-space(translate(@value, "\u00a0", " ")), \
                             "ABCDEFGHIJKLMNOPQRSTUVWXYZÄÖÅ", "abcdefghijklmnopqrstuvwxyzäöå"), \
                             translate("{0}", "ABCDEFGHIJKLMNOPQRSTUVWXYZÄÖÅ", "abcdefghijklmnopqrstuvwxyzäöå"))]'
 
-    IS_MODAL_XPATH = '//body'
+    IS_MODAL_XPATH = "//body"
 
     @staticmethod
     def active_area_xpath_validation(xpath: str) -> str:
         return SearchStrategies.clear_xpath(xpath)
 
     @staticmethod
     def all_input_elements_validation(xpath: str) -> str:
         return SearchStrategies.clear_xpath(xpath)
 
     @staticmethod
     def matching_input_element_validation(xpath: str) -> str:
-        if xpath == 'containing input element':
+        if xpath == "containing input element":
             xpath = SearchStrategies.CONTAINING_INPUT_ELEMENT
         SearchStrategies.verify_format_string(xpath, 1)
         return SearchStrategies.clear_xpath(xpath)
 
     @staticmethod
     def text_match_validation(xpath: str) -> str:
         return SearchStrategies.clear_xpath(xpath)
@@ -70,31 +71,41 @@
     @staticmethod
     def containing_text_match_validation(xpath: str) -> str:
         return SearchStrategies.clear_xpath(xpath)
 
     @staticmethod
     def clear_xpath(xpath: str) -> str:
         if re.match("xpath *=", xpath, re.IGNORECASE):
-            return ''.join(xpath.split('=')[1:])
+            return "".join(xpath.split("=")[1:])
         return xpath
 
     @staticmethod
     def search_direction_validation(direction: str) -> str:
-        """ Validates the search direction configuration """
-        valid_directions = ["up", "down", "left", "right", "closest"]
+        """Validates the search direction configuration"""
+        valid_directions = [
+            "up",
+            "down",
+            "left",
+            "right",
+            "closest",
+            "up!",
+            "down!",
+            "left!",
+            "right!",
+        ]
         direction = direction.lower()
         if direction not in valid_directions:
             raise ValueError("Wrong search direction")
         return direction
 
     @staticmethod
     def _continuous_set(s: set, num: int) -> bool:
         """Verifies that a set has given number of continous values
-           starting from 0. E.g. 0,1,2,3 is 4 continuous values whereas
-           0,1,3,4 is not.
+        starting from 0. E.g. 0,1,2,3 is 4 continuous values whereas
+        0,1,3,4 is not.
         """
 
         return set.intersection(s, set(range(num))) == set(range(num))
 
     @staticmethod
     def default_timeout_validation(timeout: Any) -> Any:
         return timeout
@@ -116,28 +127,42 @@
         # Parse format string to a list of elements
         parsed = list(string.Formatter().parse(s))
         empty_placeholders = 0
         index_placeholders = set()
         continuous = False
         for elem in parsed:
             # field_name '' matches {}
-            if elem[1] == '':
+            if elem[1] == "":
                 empty_placeholders += 1
             # field_name '0' matches {0} etc.
             elif elem[1] and elem[1].isnumeric():
                 index_placeholders.add(int(elem[1]))
 
         # Position placeholders are in a set. They must start from zero
         # so that we have {0}'s, {1}'s etc.
         if index_placeholders:
-            continuous = SearchStrategies._continuous_set(index_placeholders, placeholder_num)
+            continuous = SearchStrategies._continuous_set(
+                index_placeholders, placeholder_num
+            )
 
         if placeholder_num != (empty_placeholders + len(index_placeholders)):
-            raise ValueError("xpath has invalid number of placeholders, got {}, {}".format(
-                empty_placeholders, len(index_placeholders)))
-
-        if empty_placeholders == placeholder_num or \
-           len(index_placeholders) == placeholder_num and continuous:
+            raise ValueError(
+                "xpath has invalid number of placeholders, got {}, {}".format(
+                    empty_placeholders, len(index_placeholders)
+                )
+            )
+
+        if (
+            empty_placeholders == placeholder_num
+            or len(index_placeholders) == placeholder_num
+            and continuous
+        ):
             pass
         else:
-            raise ValueError("xpath should contain {} placeholders, got {}, {}, {}".format(
-                placeholder_num, empty_placeholders, len(index_placeholders), continuous))
+            raise ValueError(
+                "xpath should contain {} placeholders, got {}, {}, {}".format(
+                    placeholder_num,
+                    empty_placeholders,
+                    len(index_placeholders),
+                    continuous,
+                )
+            )
```

### Comparing `QWeb-3.1.0/QWeb/internal/secrets.py` & `QWeb-3.2.0/QWeb/internal/secrets.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/table.py` & `QWeb-3.2.0/QWeb/internal/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,50 +125,55 @@
                 locator_element = text.get_text_using_anchor(locator, anchor)
                 table_elements = self._get_all_table_elements()
                 table_element = element.get_closest_element(locator_element, table_elements)
             else:  # Found many
                 table_element = text.get_element_using_anchor(table_elements, anchor)
         if table_element:
             return table_element
-        raise QWebElementNotFoundError('Table element not found by locator {}'.format(locator))
+        raise QWebElementNotFoundError(f'Table element not found by locator {locator}')
 
     def get_table_cell(self, coordinates: str, anchor: str, **kwargs) -> WebElement:  # pylint: disable=unused-argument
         cell = None
         try:
             if '/' in coordinates:
-                cell = self.get_using_text_in_coordinates(coordinates, anchor)
+                cell = self.get_using_text_in_coordinates(coordinates, anchor, **kwargs)
             else:
                 row, column = self._convert_coordinates(coordinates)
                 try:
                     cell = self.table.find_element(By.XPATH,
                                                    './/tr[{0}]//td[{1}]'.format(row, column))
                 except AttributeError as e:
-                    logger.debug('exception {}'.format(e))
+                    logger.debug(f'exception {e}')
                     self.update_table()
             if cell:
                 if CONFIG['SearchMode']:
                     element.draw_borders(cell)
                 return cell
         except (StaleElementReferenceException, NoSuchElementException) as e:
-            logger.debug('exception {}'.format(e))
+            logger.debug(f'exception {e}')
             self.update_table()
-        raise QWebElementNotFoundError('Cell for coords {} not found after'.format(coordinates))
-
-    def get_using_text_in_coordinates(self, coordinates: str, anchor: str) -> WebElement:
+        raise QWebElementNotFoundError(
+            f'Cell for coords {coordinates} not found after'
+        )
+
+    def get_using_text_in_coordinates(self,
+                                      coordinates: str,
+                                      anchor: str,
+                                      **kwargs) -> WebElement:
         row: Optional[int]
         column: Optional[int]
         row_elem = None
         cell = None
         locator = coordinates.split('/')
         if locator[0].startswith('r?'):
             row_elem = self.get_row(locator[0][2:], anchor)
         else:
             row, _ = self._convert_coordinates(locator[0])
         if locator[1].startswith('c?'):
-            column = self.get_cell_by_locator(locator[1][2:])
+            column = self.get_cell_by_locator(locator[1][2:], **kwargs)
         else:
             _, column = self._convert_coordinates(locator[1])
         if row_elem:
             cell = javascript.execute_javascript(
                 'return arguments[0].cells[{}]'.format(column - 1),  # type:ignore[operator]
                 row_elem)
         else:
@@ -179,40 +184,45 @@
     def get_clickable_cell(self,
                            coordinates: str,
                            anchor: str,
                            index: int = 1,
                            **kwargs) -> WebElement:
         if int(index) < 1:
             raise QWebValueError('Index should be greater than 0.')
-        table_cell = self.get_table_cell(coordinates, anchor)
+        table_cell = self.get_table_cell(coordinates, anchor, **kwargs)
         if 'tag' in kwargs:
             clickable_child = element.get_element_from_childnodes(table_cell,
                                                                   str(kwargs.get('tag')),
                                                                   dom_traversing=False)
             if int(index) > len(clickable_child):
                 raise QWebValueError('Index exceeds the number of clickable elements in cell.')
             return clickable_child[int(index) - 1]
         return table_cell
 
-    def get_cell_by_locator(self, locator: str) -> int:
+    def get_cell_by_locator(self, locator: str, **kwargs) -> int:
+        partial_match = util.par2bool(kwargs.get('partial_match', CONFIG['PartialMatch']))
         rows = self.get_all_rows()
         for i, r in enumerate(rows):  # pylint: disable=unused-variable
             cells = self.get_cells_from_row(r)
             for index, c in enumerate(cells):
                 cell_text = ""
                 if c.text:
                     cell_text += c.text
                 elif javascript.execute_javascript(
                         'return arguments[0].querySelector("input, textarea")', c):
                     value = javascript.execute_javascript('return arguments[0].value', c)
                     if value:
                         cell_text += str(value)
-                if locator in cell_text:
-                    return index + 1
-        raise QWebValueError('Matching table cell not found for locator {}.'.format(locator))
+                if partial_match:
+                    if locator in cell_text:
+                        return index + 1
+                else:
+                    if locator == cell_text:
+                        return index + 1
+        raise QWebValueError(f'Matching table cell not found for locator {locator}.')
 
     def get_row(self, locator: str, anchor: str, row_index: bool = False, **kwargs
                 ) -> Union[WebElement, int]:
         skip_header = util.par2bool(kwargs.get('skip_header', False))
         rows = self.get_all_rows()
         if locator.startswith('//last'):
             if skip_header:
@@ -221,15 +231,15 @@
         matches, index = self._get_row_by_locator_text(rows, locator, anchor)
         if row_index:
             if skip_header:
                 return index
             return index + 1
         if matches:
             return matches
-        raise QWebValueError('Matching table row not found for locator {}.'.format(locator))
+        raise QWebValueError(f'Matching table row not found for locator {locator}.')
 
     def get_all_rows(self) -> list[WebElement]:
         return javascript.execute_javascript('return arguments[0].rows', self.table)
 
     @staticmethod
     def get_cells_from_row(row: WebElement) -> list[WebElement]:
         return javascript.execute_javascript('return arguments[0].cells', row)
@@ -256,16 +266,17 @@
             if locator in row_content:
                 if anchor_text and anchor_text in row_content:
                     return row, index
                 row_index.append(index)
                 matches.append(row)
         if matches and not anchor_text:
             return matches[int(anchor)], row_index[int(anchor)]
-        raise QWebElementNotFoundError('Row that includes texts {} and {} not found'.format(
-            locator, anchor_text))
+        raise QWebElementNotFoundError(
+            f'Row that includes texts {locator} and {anchor_text} not found'
+        )
 
     def _convert_coordinates(self, coordinate_str: str) -> tuple[Optional[int], Optional[int]]:
         """Return row and column from coordinate string."""
         try:
             row = int(re.findall('r([+-]?[0-9]+)', coordinate_str)[0])
             if row < 0:
                 last_row = self.get_row('//last', self.anchor)
```

### Comparing `QWeb-3.1.0/QWeb/internal/text.py` & `QWeb-3.2.0/QWeb/internal/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             WebDriverException):
         try:
             web_element = element.get_unique_element_by_xpath(locator, index=index)
         except (QWebElementNotFoundError, InvalidSelectorException, NoSuchFrameException) as e:
             no_raise = util.par2bool(kwargs.get('allow_non_existent', False))
             if no_raise:
                 return None
-            raise QWebElementNotFoundError(e)  # pylint: disable=W0707
+            raise QWebElementNotFoundError(e) from e
     if web_element:
         if 'parent' in kwargs and kwargs['parent']:
             tag_name = kwargs['parent']
             web_element = element.get_parent_element(web_element, tag_name)
         elif 'child' in kwargs and kwargs['child']:
             tag_name = kwargs['child']
             web_element = element.get_element_from_childnodes(web_element,
@@ -197,15 +197,16 @@
     web_elements = get_all_text_elements(text, **kwargs)
 
     # filter elements by modal (dialog etc) if needed
     web_elements = filter_by_modal_ancestor(web_elements)
     if not web_elements:
         raise QWebElementNotFoundError('Webpage did not contain text "{}"'.format(text))
 
-    if len(web_elements) == 1:
+    # return directly if 1 match and direction does not need to be checked
+    if len(web_elements) == 1 and not CONFIG.enforce_direction():
         return web_elements[0]
     # Found many elements, use anchors to determine correct element
     correct_element = get_element_using_anchor(web_elements, anchor, **kwargs)
     return correct_element
 
 
 def _get_exact_text_element(text: str, **kwargs) -> Optional[list[WebElement]]:
```

### Comparing `QWeb-3.1.0/QWeb/internal/user.py` & `QWeb-3.2.0/QWeb/internal/user.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/util.py` & `QWeb-3.2.0/QWeb/internal/util.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/window.py` & `QWeb-3.2.0/QWeb/internal/window.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/internal/xhr.py` & `QWeb-3.2.0/QWeb/internal/xhr.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/ajax.py` & `QWeb-3.2.0/QWeb/keywords/ajax.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/alert.py` & `QWeb-3.2.0/QWeb/keywords/alert.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/blocks.py` & `QWeb-3.2.0/QWeb/keywords/blocks.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/browser.py` & `QWeb-3.2.0/QWeb/keywords/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,15 +508,15 @@
 
     # Set 'Headless' flag as False, since no session open anymore
     CONFIG.set_value("Headless", False)
 
 
 @keyword(tags=("Browser", "Verification"))
 def verify_links(
-    url: str = "current", log_all: bool = False, header_only: bool = True, timeout=None
+    url: str = "current", log_all: bool = False, header_only: bool = True, timeout=0
 ) -> None:
     r"""Verify that all links on a given website return good HTTP status codes.
 
     Examples
     --------
     .. code-block:: robotframework
```

### Comparing `QWeb-3.1.0/QWeb/keywords/checkbox.py` & `QWeb-3.2.0/QWeb/keywords/checkbox.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/config.py` & `QWeb-3.2.0/QWeb/keywords/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     |                     | interaction keyword. Useful for example |                |
     |                     | when there is a custom spinner that     |                |
     |                     | should be waited for                    |                |
     +---------------------+-----------------------------------------+----------------+
     | ScreenShotType_     | Log html source, screenshot or both     | screenshot     |
     +---------------------+-----------------------------------------+----------------+
     | SearchDirection_    | Set relative search direction for       | closest        |
-    |                     | element search (up, down, lef, righ,    |                |
-    |                     | closest)                                |                |
+    |                     | element search (closest, up, down, left,|                |
+    |                     | right, up!, down!, left!, right!)       |                |
     +---------------------+-----------------------------------------+----------------+
     | SearchMode_         | Options for highlighting elements found | draw           |
     |                     | by searches (None, debug, draw).        |                |
     +---------------------+-----------------------------------------+----------------+
     | ShadowDOM_          | Extend element searches to shadow DOM.  |   False        |
     +---------------------+-----------------------------------------+----------------+
     | XHRTimeout_         | Maximum wait for page to be loaded      | 30s            |
@@ -223,28 +223,58 @@
     ----
 
     Parameter: SearchDirection
     --------------------------
 
     Set search direction for element search.
 
-    Search direction is "up", "down", "left", "right" and "closest".
+    Search direction is "closest, "up", "down", "left", "right",
+    "up!", "down!", "left!", "right!".
     "Closest" is the default value.
 
     Elements are searched according to their relative position to anchor.
 
+    With this setting you can choose between two ways of searching:
+
+    - **normal mode**
+    - **strict mode** (ending with "!").
+
+    **Normal Mode**: In this mode, you start looking for something starting from a specific point
+    or direction you've chosen. If you can't find it there, the search will then try to find
+    the closest match, even if it's not exactly in the direction you started from.
+
+    **Strict Mode**: This mode is stricter. You also start searching from a specific direction,
+    but the big difference is that if what you're looking for isn't found exactly in that direction,
+    the search will fail.
+    It won't try to find the next closest thing. The search insists that the item must be found in
+    the direction you specified, or not at all.
+    It's important to note that this enforced format works only when you're searching for text
+    on a page, like when you're using commands to verify text is there (VerifyText)
+    or when you want to click on text (ClickText).
+
     Examples
     ^^^^^^^^
+
     .. code-block:: robotframework
 
-        SetConfig    SearchDirection       right
-        TypeText     MyLocator   Robot     # finds text "My Locator" on the right of text "Robot"
-        SetConfig    SearchDirection       up
-        TypeText     MyLocator   Robot     # finds text "My Locator" above of text "Robot"
-        SetConfig    SearchDirection       closest
+        *** Test Cases ***
+        SearchDirection Example
+            # finds input using text "My Locator" on the right of text "Robot"
+            SetConfig    SearchDirection       right
+            TypeText     MyLocator  Hello  Robot
+
+            # finds input using text "My Locator" above of text "Robot"
+            SetConfig    SearchDirection       up
+            TypeText     MyLocator  Hello  Robot
+
+            # When using strict mode (!), the test case fails if the locator text is
+            # not found in the correct direction from the anchor.
+            SetConfig    SearchDirection       left!
+            VerifyText   Firstname             anchor=Lastname
+            SetConfig    SearchDirection       closest
 
     .. _linebreak:
 
     ----
 
     Parameter: LineBreak
     --------------------
```

### Comparing `QWeb-3.1.0/QWeb/keywords/cookies.py` & `QWeb-3.2.0/QWeb/keywords/cookies.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,32 +43,39 @@
     ----------------
     \`ListCookies\`, \`IsCookie\`
     """
     cookies.delete_all_cookies()
 
 
 @keyword(tags=("Browser", "Getters"))
-def list_cookies() -> list[dict[str, Any]]:
+def list_cookies(log: bool = True) -> list[dict[str, Any]]:
     r"""List all cookies in browser.
 
     Cookies can be only listed when browser is open. Cookies are automatically
-    deleted when you Close All Browsers
+    deleted when you Close All Browsers.
 
     Examples
     --------
     .. code-block:: robotframework
 
         ListCookies
 
+    Parameters
+    ----------
+    log : bool
+        If true, log list of cookies to html log file. If False, only returns cookie list.
+        Default is True.
+
     Related keywords
     ----------------
     \`DeleteAllCookies\`, \`IsCookie\`
     """
     cookies_list = cookies.get_cookies()
-    logger.info(f"{cookies_list}")
+    if log:
+        logger.info(f"{cookies_list}")
     return cookies_list
 
 
 @keyword(tags=("Browser", "Verification"))
 def is_cookie(name: str, value: str) -> bool:
     r"""Return True if cookie with name and value is found.
```

### Comparing `QWeb-3.1.0/QWeb/keywords/debug.py` & `QWeb-3.2.0/QWeb/keywords/debug.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/download.py` & `QWeb-3.2.0/QWeb/keywords/download.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/dragdrop.py` & `QWeb-3.2.0/QWeb/keywords/dragdrop.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/dropdown.py` & `QWeb-3.2.0/QWeb/keywords/dropdown.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/element.py` & `QWeb-3.2.0/QWeb/keywords/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,22 +516,24 @@
                   element_type: Optional[str] = None,
                   timeout: Union[int, float, str] = 0,
                   **kwargs) -> str:
     r"""Get attribute value of an element.
 
     Examples
     --------
-    Using attributes or xpaths like with ClickElement etc. kw:s without specified
-    element_type. If element_type is not specified end result is a type of list:
+    Using xpaths like with ClickElement etc. kw:s without specified
+    element_type. Index must be given if element is not unique:
 
     .. code-block:: robotframework
 
         ${attribute_value}  GetAttribute            click_me     id         tag=button
         ${attribute_value}  GetAttribute            //*[@id\="click_me"]    id
         ${attribute_value}  GetAttribute            xpath\=//*[@id\="click_me"] name
+        # Get id attribute value from 3rd matching element
+        ${attribute_value}  GetAttribute            //button    id  index=3
 
     GetAttribute using element_type attribute to locate element.
     Text elements works as ClickText, VerifyText, GetText etc.:
 
     .. code-block:: robotframework
 
         ${attribute_value}   GetAttribute     Log In    type    element_type=text
@@ -570,15 +572,16 @@
         (available types: text, input, checkbox, item, dropdown or css).
     timeout : int
         How long we wait element to appear. Default=10 sec
     kwargs :
         |  Accepted kwargs:
         |       Any available for picked searching method.
         |       See interacting with text, item, input etc. elements from
-        |       documentation
+        |       documentation. When using xpath as locator **index** should be
+        |       specified unless xpath matches to a single element.
 
     Returns
     -------
     value : Value of attribute (true if attribute exist but does not have value)
 
     Related keywords
     ----------------
```

### Comparing `QWeb-3.1.0/QWeb/keywords/file.py` & `QWeb-3.2.0/QWeb/keywords/file.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/frame.py` & `QWeb-3.2.0/QWeb/keywords/frame.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/icon.py` & `QWeb-3.2.0/QWeb/keywords/icon.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/input_.py` & `QWeb-3.2.0/QWeb/keywords/input_.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/javascript.py` & `QWeb-3.2.0/QWeb/keywords/javascript.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/lists.py` & `QWeb-3.2.0/QWeb/keywords/lists.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/screenshot.py` & `QWeb-3.2.0/QWeb/keywords/screenshot.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/search_strategy.py` & `QWeb-3.2.0/QWeb/keywords/search_strategy.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb/keywords/table.py` & `QWeb-3.2.0/QWeb/keywords/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,15 +90,16 @@
 
 
 @keyword(tags=("Tables", "Verification"))
 @decorators.timeout_decorator
 def verify_table(coordinates: str,
                  expected: str,
                  anchor: str = "1",
-                 timeout: Union[int, float, str] = 0) -> None:
+                 timeout: Union[int, float, str] = 0,
+                 **kwargs) -> None:
     r"""Verify text in table coordinates.
 
     Reads cell value from coordinates in active table and verifies it
     against expected value.
 
     Examples
     --------
@@ -118,28 +119,42 @@
         Index number or text near the input field's locator element.
         If the page contains many places where the locator is then anchor is used
         to select the wanted item. Index number selects the item from the list
         of matching entries starting with 1. Text selects the entry with the closest
         distance.
     timeout : str | int
         How long we search before failing. Default = Search Strategy default timeout (10s)
+    kwargs :
+        |  Accepted kwargs:
+        |       **partial_match**: This argument lets you decide if you want to find column names
+        |       by looking for an exact match to your search term or if a partial match is
+        |       good enough. For example, when you're specifying which column to look at using
+        |       a text-based method (like "r1/?cRobot"), this determines whether the system should
+        |       look for an exact match to "Robot" or if it can work with columns that only partly
+        |       match the word "Robot".
+        |       It also applies to checking values: this setting controls whether a value that only
+        |       partially matches your criteria is considered okay.
+        |       Default: if partial_match is not given, the value of SetConfig PartialMatch is used.
 
     Raises
     ------
     QWebValueMismatchErr
         If the table is not defined by UseTable keyword
 
     Related keywords
     ----------------
     \`ClickCell\`, \`GetCellText\`, \`GetTableRow\`, \`UseTable\`
     """
-    table = Table.ACTIVE_TABLE.update_table()
-    if isinstance(ACTIVE_TABLE, Table) is False:
+    if not isinstance(ACTIVE_TABLE, Table):
         raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
-    table_cell = table.ACTIVE_TABLE.get_table_cell(coordinates, anchor)
+    table = Table.ACTIVE_TABLE.update_table()
+
+    table_cell = table.ACTIVE_TABLE.get_table_cell(coordinates, anchor, **kwargs)
+    partial_match = util.par2bool(kwargs.get('partial_match', CONFIG['PartialMatch']))
+    expected = f"{expected}*" if partial_match else expected
     actions.get_element_text(table_cell, expected=expected, timeout=timeout)
 
 
 @keyword(tags=("Tables", "Getters"))
 @decorators.timeout_decorator
 def get_cell_text(coordinates: str,
                   anchor: str = "1",
@@ -183,17 +198,18 @@
     QWebValueError
         If the table is not defined by UseTable keyword
 
     Related keywords
     ----------------
     \`ClickCell\`, \`GetTableRow\`, \`UseTable\`, \`VerifyTable\`
     """
-    table = Table.ACTIVE_TABLE.update_table()
-    if isinstance(ACTIVE_TABLE, Table) is False:
+    if not isinstance(ACTIVE_TABLE, Table):
         raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+    table = Table.ACTIVE_TABLE.update_table()
+
     table_cell = table.get_table_cell(coordinates, anchor)
     try:
         text = actions.get_element_text(table_cell, timeout=timeout)
         return util.get_substring(text, **kwargs)
     except QWebTimeoutError:
         return ""
 
@@ -231,27 +247,38 @@
       If row is located by text which is not unique, use anchor to point correct one.
       Anchor can be some other text in same row or index. Default = 1
     timeout : str | int
        How long we search before failing. Default = Search Strategy default timeout (10s)
     index : int
        Use index when table cell contains more than one clickable element and preferred one
        is not the first one. Requires the use of tag and value should be > 0, default = 1.
+    kwargs :
+        |  Accepted kwargs:
+        |       **partial_match**: This argument lets you decide if you want to find column names
+        |       by looking for an exact match to your search term or if a partial match is
+        |       good enough. For example, when you're specifying which column to look at using
+        |       a text-based method (like "r1/?cRobot"), this determines whether the system should
+        |       look for an exact match to "Robot" or if it can work with columns that only partly
+        |       match the word "Robot".
+        |       Default: if partial_match is not given, the value of SetConfig PartialMatch is used.
+
 
     Raises
     ------
     QWebValueError
        If the table is not defined by UseTable keyword
 
     Related keywords
     ----------------
     \`GetCellText\`, \`GetTableRow\`, \`UseTable\`, \`VerifyTable\`
     """
-    table = Table.ACTIVE_TABLE.update_table()
-    if isinstance(ACTIVE_TABLE, Table) is False:
+    if not isinstance(ACTIVE_TABLE, Table):
         raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+    table = Table.ACTIVE_TABLE.update_table()
+
     table_cell = table.get_clickable_cell(coordinates, anchor, index, **kwargs)
     actions.execute_click_and_verify_condition(table_cell, **kwargs)
 
 
 @keyword(tags=("Tables", "Getters"))
 @decorators.timeout_decorator
 def get_table_row(
@@ -288,17 +315,18 @@
     ValueError
        If the table is not defined by UseTable keyword
 
     Related keywords
     ----------------
     \`ClickCell\`, \`GetCellText\`, \`UseTable\`, \`VerifyTable\`
     """
-    table = Table.ACTIVE_TABLE.update_table()
-    if isinstance(ACTIVE_TABLE, Table) is False:
+    if not isinstance(ACTIVE_TABLE, Table):
         raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+    table = Table.ACTIVE_TABLE.update_table()
+
     return table.get_row(locator, anchor, row_index=True, **kwargs)
 
 
 @keyword(tags=("Tables", "Getters"))
 def get_col_header_count() -> int:
     r"""Get Count of column headers in current active table.
```

### Comparing `QWeb-3.1.0/QWeb/keywords/text.py` & `QWeb-3.2.0/QWeb/keywords/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,31 @@
     r"""Verify page contains given text.
 
     Keyword waits until timeout has passed. If timeout is not specified, it
     uses default timeout that can be adjusted with DefaultTimeout keyword.
 
     VerifyText does not require for the text to be unique.
 
+    *Note: Slots are a bit unique as they do not have size/offset. This means
+    that our default visibility check will treat slots as not visible. If text is
+    directly on the slot, use visibility=False argument in VerifyText keyword. For example:*
+
+    .. code-block:: html
+
+        <slot>My Text</slot>
+
+    *The above needs visibility=False argument, as text is directly on the slot. However,
+    this one would work without turning visibility check off, since text is on a child
+    element under slot:*
+
+    .. code-block:: html
+
+        <slot><span>My Text</span></slot>
+
+
     Examples
     --------
     .. code-block:: robotframework
 
         VerifyText        Canis
 
     In the above example the test will wait until "Canis" exists on the page or default
@@ -409,15 +426,17 @@
         tag name for clickable parent.
     child : str
         tag name for clickable child.
     js : boolean
         If set to true, uses javascript instead of selenium to click element.
     Accepted kwargs:
         css=False/off: Use this to bypass css search when finding elements
-        by visible text
+        by visible text. In practise this means that also non-clickable texts
+        (e.g. spans) are considered. By default ClickText only finds texts that
+        are considered "clickable".
 
     Related keywords
     ----------------
     \`ClickElement\`, \`ClickItem\`, \`GetText\`, \`RightClick\`, \`VerifyText\`
     """
     anchor = str(anchor)
 
@@ -1209,22 +1228,25 @@
     \`HoverElement\`, \`HoverItem\`, \`HoverText\`, \`HoverTo\`, \`ScrollTo\`
     """
     web_element = internal_text.get_element_by_locator_text(text, anchor, **kwargs)
     _scroll(web_element, timeout=timeout)
 
 
 @keyword(tags=("input", "Text", "Interaction"))
-def write_text(text: str) -> None:
+def write_text(text: str, **kwargs) -> None:  # pylint: disable=W0613
     r"""Type text with single-character keys.
 
     Parameters
     ----------
     text : str
         Text to type.
 
+    Accepted kwargs:
+        delay = Time to wait (seconds) before typing.
+
     Examples
     --------
     .. code-block:: robotframework
 
         WriteText    Hello World!
 
     Related keywords
```

### Comparing `QWeb-3.1.0/QWeb/keywords/window.py` & `QWeb-3.2.0/QWeb/keywords/window.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/QWeb.egg-info/PKG-INFO` & `QWeb-3.2.0/QWeb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QWeb
-Version: 3.1.0
+Version: 3.2.0
 Summary: Keyword driven automation for the web
 Home-page: https://github.com/qentinelqi/qweb/
 Author: Qentinel Group
 Author-email: libraries@qentinel.com
 License: Apache License 2.0
 Keywords: test automation robot framework
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `QWeb-3.1.0/QWeb.egg-info/SOURCES.txt` & `QWeb-3.2.0/QWeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/README.md` & `QWeb-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/setup.cfg` & `QWeb-3.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/setup.py` & `QWeb-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.1.0/versioneer.py` & `QWeb-3.2.0/versioneer.py`

 * *Files identical despite different names*

