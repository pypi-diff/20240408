# Comparing `tmp/eon_collective_docs_theme-0.0.1.dev0.tar.gz` & `tmp/eon_collective_docs_theme-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eon_collective_docs_theme-0.0.1.dev0.tar", last modified: Mon Apr  8 12:45:15 2024, max compression
+gzip compressed data, was "eon_collective_docs_theme-0.0.2.dev0.tar", last modified: Mon Apr  8 14:00:44 2024, max compression
```

## Comparing `eon_collective_docs_theme-0.0.1.dev0.tar` & `eon_collective_docs_theme-0.0.2.dev0.tar`

### file list

```diff
@@ -1,77 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:15.137470 eon_collective_docs_theme-0.0.1.dev0/
--rw-rw-rw-   0        0        0     1126 2024-04-07 14:47:16.000000 eon_collective_docs_theme-0.0.1.dev0/LICENSE
--rw-rw-rw-   0        0        0      213 2024-04-07 13:13:06.000000 eon_collective_docs_theme-0.0.1.dev0/MANIFEST.in
--rw-rw-rw-   0        0        0     2087 2024-04-08 12:45:15.138497 eon_collective_docs_theme-0.0.1.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2024-04-07 12:24:54.000000 eon_collective_docs_theme-0.0.1.dev0/README.md
--rw-rw-rw-   0        0        0      759 2024-04-07 12:15:21.000000 eon_collective_docs_theme-0.0.1.dev0/USAGE.rst
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:15.021711 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:15.036753 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/UNKNOWN.egg-info/
--rw-rw-rw-   0        0        0      123 2024-04-08 12:30:36.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/UNKNOWN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 12:30:36.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/UNKNOWN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-08 12:30:36.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/UNKNOWN.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2284 2024-04-08 01:13:17.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:15.039923 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/__pycache__/
--rw-rw-rw-   0        0        0     3728 2024-04-08 01:13:25.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      411 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/breadcrumbs.html
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:15.042884 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/dist/
--rw-rw-rw-   0        0        0      562 2024-04-08 12:30:36.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/dist/UNKNOWN-0.0.0.tar.gz
--rw-rw-rw-   0        0        0     1896 2024-04-07 14:41:44.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/domainindex.html
--rw-rw-rw-   0        0        0     1385 2024-04-07 14:42:59.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/extensions.html
--rw-rw-rw-   0        0        0     1707 2024-04-07 14:46:15.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/footer.html
--rw-rw-rw-   0        0        0     2035 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/genindex-single.html
--rw-rw-rw-   0        0        0     1166 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/genindex-split.html
--rw-rw-rw-   0        0        0     2554 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/genindex.html
--rw-rw-rw-   0        0        0      413 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/globaltoc.html
--rw-rw-rw-   0        0        0     9449 2024-04-08 11:16:06.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/layout.html
--rw-rw-rw-   0        0        0       76 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/page.html
--rw-rw-rw-   0        0        0      513 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/pager.html
--rw-rw-rw-   0        0        0     1093 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/search.html
--rw-rw-rw-   0        0        0      789 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/searchbox.html
--rw-rw-rw-   0        0        0      701 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/searchresults.html
--rw-rw-rw-   0        0        0      450 2024-04-08 00:43:14.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/sitemap.html
--rw-rw-rw-   0        0        0      275 2024-04-07 22:44:38.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/source-buttons.html
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:14.970941 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:15.074887 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:15.122512 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/
--rw-rw-rw-   0        0        0   134346 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.eot
--rw-rw-rw-   0        0        0   747545 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.svg
--rw-rw-rw-   0        0        0   134040 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.ttf
--rw-rw-rw-   0        0        0    90060 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.woff
--rw-rw-rw-   0        0        0    76764 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    34034 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.eot
--rw-rw-rw-   0        0        0   144714 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.svg
--rw-rw-rw-   0        0        0    33736 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    16276 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.woff
--rw-rw-rw-   0        0        0    13276 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   203030 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.eot
--rw-rw-rw-   0        0        0   918991 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.svg
--rw-rw-rw-   0        0        0   202744 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.ttf
--rw-rw-rw-   0        0        0   101652 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.woff
--rw-rw-rw-   0        0        0    78196 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.woff2
--rw-rw-rw-   0        0        0     2737 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/blocking.js
--rw-rw-rw-   0        0        0     4374 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/blocking.js.map
--rw-rw-rw-   0        0        0    73757 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/fontawesome.css
--rw-rw-rw-   0        0        0   289108 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/fontawesome.css.map
--rw-rw-rw-   0        0        0     1026 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/fontawesome.js
--rw-rw-rw-   0        0        0      799 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/fontawesome.js.map
--rw-rw-rw-   0        0        0   208107 2024-04-08 11:52:38.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/theme.css
--rw-rw-rw-   0        0        0   553935 2024-04-08 11:23:12.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/theme.css.map
--rw-rw-rw-   0        0        0    13314 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/theme.js
--rw-rw-rw-   0        0        0    17191 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/theme.js.map
--rw-rw-rw-   0        0        0   533995 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/vendor.js
--rw-rw-rw-   0        0        0   666226 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/vendor.js.map
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:15.128508 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/img/
--rw-rw-rw-   0        0        0     2735 2024-04-08 01:00:26.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/img/eon-white-full.png
--rw-rw-rw-   0        0        0     5665 2024-04-08 01:01:55.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/img/eon-white-full.svg
--rw-rw-rw-   0        0        0      351 2024-04-08 01:07:56.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/theme.conf
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:15.030780 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme.egg-info/
--rw-rw-rw-   0        0        0     2087 2024-04-08 12:45:14.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3062 2024-04-08 12:45:14.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 12:45:14.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-08 12:45:14.000000 eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1274 2024-04-08 12:45:15.141469 eon_collective_docs_theme-0.0.1.dev0/setup.cfg
--rw-rw-rw-   0        0        0      417 2024-04-07 12:23:24.000000 eon_collective_docs_theme-0.0.1.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:45:15.135468 eon_collective_docs_theme-0.0.1.dev0/tests/
--rw-rw-rw-   0        0        0       50 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/tests/__init__.py
--rw-rw-rw-   0        0        0      288 2024-04-07 14:02:09.000000 eon_collective_docs_theme-0.0.1.dev0/tests/test_python_sphinx_wagtail_theme.py
--rw-rw-rw-   0        0        0     2166 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.1.dev0/tests/test_visual_regression.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:44.002843 eon_collective_docs_theme-0.0.2.dev0/
+-rw-rw-rw-   0        0        0     1126 2024-04-07 14:47:16.000000 eon_collective_docs_theme-0.0.2.dev0/LICENSE
+-rw-rw-rw-   0        0        0      213 2024-04-07 13:13:06.000000 eon_collective_docs_theme-0.0.2.dev0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2071 2024-04-08 14:00:44.002843 eon_collective_docs_theme-0.0.2.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     1108 2024-04-08 13:12:40.000000 eon_collective_docs_theme-0.0.2.dev0/README.md
+-rw-rw-rw-   0        0        0      759 2024-04-07 12:15:21.000000 eon_collective_docs_theme-0.0.2.dev0/USAGE.rst
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:43.932235 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/
+-rw-rw-rw-   0        0        0     2128 2024-04-08 13:48:17.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/__init__.py
+-rw-rw-rw-   0        0        0      411 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/breadcrumbs.html
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:43.942237 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/dist/
+-rw-rw-rw-   0        0        0      562 2024-04-08 12:30:36.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/dist/UNKNOWN-0.0.0.tar.gz
+-rw-rw-rw-   0        0        0     1896 2024-04-07 14:41:44.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/domainindex.html
+-rw-rw-rw-   0        0        0     1385 2024-04-07 14:42:59.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/extensions.html
+-rw-rw-rw-   0        0        0     1707 2024-04-07 14:46:15.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/footer.html
+-rw-rw-rw-   0        0        0     2035 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/genindex-single.html
+-rw-rw-rw-   0        0        0     1166 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/genindex-split.html
+-rw-rw-rw-   0        0        0     2554 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/genindex.html
+-rw-rw-rw-   0        0        0      413 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/globaltoc.html
+-rw-rw-rw-   0        0        0     9449 2024-04-08 11:16:06.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/layout.html
+-rw-rw-rw-   0        0        0       76 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/page.html
+-rw-rw-rw-   0        0        0      513 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/pager.html
+-rw-rw-rw-   0        0        0     1093 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/search.html
+-rw-rw-rw-   0        0        0      789 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/searchbox.html
+-rw-rw-rw-   0        0        0      701 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/searchresults.html
+-rw-rw-rw-   0        0        0      450 2024-04-08 00:43:14.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/sitemap.html
+-rw-rw-rw-   0        0        0      275 2024-04-07 22:44:38.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/source-buttons.html
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:43.880334 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:43.964241 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:43.995242 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/
+-rw-rw-rw-   0        0        0   134346 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.eot
+-rw-rw-rw-   0        0        0   747545 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.svg
+-rw-rw-rw-   0        0        0   134040 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0    90060 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.woff
+-rw-rw-rw-   0        0        0    76764 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    34034 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.eot
+-rw-rw-rw-   0        0        0   144714 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.svg
+-rw-rw-rw-   0        0        0    33736 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    16276 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.woff
+-rw-rw-rw-   0        0        0    13276 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   203030 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.eot
+-rw-rw-rw-   0        0        0   918991 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.svg
+-rw-rw-rw-   0        0        0   202744 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0   101652 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.woff
+-rw-rw-rw-   0        0        0    78196 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.woff2
+-rw-rw-rw-   0        0        0     2737 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/blocking.js
+-rw-rw-rw-   0        0        0     4374 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/blocking.js.map
+-rw-rw-rw-   0        0        0    73757 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/fontawesome.css
+-rw-rw-rw-   0        0        0   289108 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/fontawesome.css.map
+-rw-rw-rw-   0        0        0     1026 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/fontawesome.js
+-rw-rw-rw-   0        0        0      799 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/fontawesome.js.map
+-rw-rw-rw-   0        0        0   208107 2024-04-08 11:52:38.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/theme.css
+-rw-rw-rw-   0        0        0   553935 2024-04-08 11:23:12.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/theme.css.map
+-rw-rw-rw-   0        0        0    13314 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/theme.js
+-rw-rw-rw-   0        0        0    17191 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/theme.js.map
+-rw-rw-rw-   0        0        0   533995 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/vendor.js
+-rw-rw-rw-   0        0        0   666226 2024-04-07 17:36:45.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/vendor.js.map
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:43.998235 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/img/
+-rw-rw-rw-   0        0        0     2735 2024-04-08 01:00:26.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/img/eon-white-full.png
+-rw-rw-rw-   0        0        0     5665 2024-04-08 01:01:55.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/img/eon-white-full.svg
+-rw-rw-rw-   0        0        0      351 2024-04-08 01:07:56.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/theme.conf
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:43.939236 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme.egg-info/
+-rw-rw-rw-   0        0        0     2071 2024-04-08 14:00:43.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2823 2024-04-08 14:00:43.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 14:00:43.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-08 14:00:43.000000 eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1274 2024-04-08 14:00:44.005240 eon_collective_docs_theme-0.0.2.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      417 2024-04-07 12:23:24.000000 eon_collective_docs_theme-0.0.2.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:00:44.001784 eon_collective_docs_theme-0.0.2.dev0/tests/
+-rw-rw-rw-   0        0        0       50 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/tests/__init__.py
+-rw-rw-rw-   0        0        0      288 2024-04-07 14:02:09.000000 eon_collective_docs_theme-0.0.2.dev0/tests/test_python_sphinx_wagtail_theme.py
+-rw-rw-rw-   0        0        0     2166 2024-04-06 21:26:52.000000 eon_collective_docs_theme-0.0.2.dev0/tests/test_visual_regression.py
```

### Comparing `eon_collective_docs_theme-0.0.1.dev0/LICENSE` & `eon_collective_docs_theme-0.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/PKG-INFO` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eon_collective_docs_theme
-Version: 0.0.1.dev0
+Name: eon-collective-docs-theme
+Version: 0.0.2.dev0
 Summary: The theme used to render documentation
 Home-page: https://github.com/janerose-njogu/eon-collective-docs-theme
 Author: Janerose Njogu
 Author-email: janerose.njogu@eoncllective.com
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 3 - Alpha
@@ -34,24 +34,22 @@
 This guide assumes that you have set up Sphinx in your project. All you need to do is install this theme and include it within your conf.py file.
 
 It is also assumed that you understand Sphinx.
 
 ## Installation
 
 ```sh
-# TODO
 pip install eon-collective-docs-theme
 ```
 
 ## Usage
 
 In your conf.py file of a Sphinx documentation, specify the "Eon Collective Documentation theme" as an extension.
 
 ```python
-# TODO
 # include the theme in the list of extensions to be loaded
 extensions = ['eon_collective_docs_theme', …]
 
 # select the theme
 html_theme = 'eon_collective_docs_theme'
 ```
```

### Comparing `eon_collective_docs_theme-0.0.1.dev0/README.md` & `eon_collective_docs_theme-0.0.2.dev0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,24 +11,22 @@
 This guide assumes that you have set up Sphinx in your project. All you need to do is install this theme and include it within your conf.py file.
 
 It is also assumed that you understand Sphinx.
 
 ## Installation
 
 ```sh
-# TODO
 pip install eon-collective-docs-theme
 ```
 
 ## Usage
 
 In your conf.py file of a Sphinx documentation, specify the "Eon Collective Documentation theme" as an extension.
 
 ```python
-# TODO
 # include the theme in the list of extensions to be loaded
 extensions = ['eon_collective_docs_theme', …]
 
 # select the theme
 html_theme = 'eon_collective_docs_theme'
 ```
```

### Comparing `eon_collective_docs_theme-0.0.1.dev0/USAGE.rst` & `eon_collective_docs_theme-0.0.2.dev0/USAGE.rst`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/__init__.py` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,19 +31,15 @@
     file `sitemap.html` for this page instead of the default template file
     `page.html`.
 
     """
     context["theme_version"] = __version__
     parent_dir = os.path.dirname(os.path.dirname(__file__))
     docs_dir = os.path.join(parent_dir, "docs")
-    config_file_path = docs_dir
-    if os.path.isdir(os.path.join(docs_dir, "source")):
-        config_file_path = os.path.join(docs_dir,"source")
-
-    config_values = Config.read(confdir=config_file_path)._raw_config
+    config_values = Config.read(confdir=docs_dir)._raw_config
     if(config_values.get("repository")):
         context["repository"] = config_values["repository"]
     return app.builder.env.metadata.get(pagename, {}).get("template")
 
 def setup(app):
     """Setup functionality called by Sphinx"""
     app.connect("html-page-context", update_context)
```

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/dist/UNKNOWN-0.0.0.tar.gz` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/dist/UNKNOWN-0.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/domainindex.html` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/extensions.html` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/extensions.html`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/footer.html` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/footer.html`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/genindex-single.html` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/genindex-single.html`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/genindex-split.html` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/genindex-split.html`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/genindex.html` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/layout.html` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/layout.html`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/pager.html` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/pager.html`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/search.html` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/search.html`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/searchbox.html` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/searchresults.html` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/searchresults.html`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.eot` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.svg` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.ttf` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.woff` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.woff2` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.eot` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.svg` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.ttf` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.woff` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.woff2` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.eot` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.svg` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.ttf` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.woff` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.woff2` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/assets/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/blocking.js` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/blocking.js`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/blocking.js.map` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/blocking.js.map`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/fontawesome.css` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/fontawesome.css`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/fontawesome.css.map` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/fontawesome.css.map`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/fontawesome.js` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/fontawesome.js`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/fontawesome.js.map` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/fontawesome.js.map`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/theme.css` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/theme.css`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/theme.css.map` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/theme.css.map`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/theme.js` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/theme.js`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/theme.js.map` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/theme.js.map`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/vendor.js` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/vendor.js`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/dist/vendor.js.map` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/dist/vendor.js.map`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/img/eon-white-full.png` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/img/eon-white-full.png`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme/static/img/eon-white-full.svg` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme/static/img/eon-white-full.svg`

 * *Files identical despite different names*

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme.egg-info/PKG-INFO` & `eon_collective_docs_theme-0.0.2.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eon-collective-docs-theme
-Version: 0.0.1.dev0
+Name: eon_collective_docs_theme
+Version: 0.0.2.dev0
 Summary: The theme used to render documentation
 Home-page: https://github.com/janerose-njogu/eon-collective-docs-theme
 Author: Janerose Njogu
 Author-email: janerose.njogu@eoncllective.com
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 3 - Alpha
@@ -34,24 +34,22 @@
 This guide assumes that you have set up Sphinx in your project. All you need to do is install this theme and include it within your conf.py file.
 
 It is also assumed that you understand Sphinx.
 
 ## Installation
 
 ```sh
-# TODO
 pip install eon-collective-docs-theme
 ```
 
 ## Usage
 
 In your conf.py file of a Sphinx documentation, specify the "Eon Collective Documentation theme" as an extension.
 
 ```python
-# TODO
 # include the theme in the list of extensions to be loaded
 extensions = ['eon_collective_docs_theme', …]
 
 # select the theme
 html_theme = 'eon_collective_docs_theme'
 ```
```

### Comparing `eon_collective_docs_theme-0.0.1.dev0/eon_collective_docs_theme.egg-info/SOURCES.txt` & `eon_collective_docs_theme-0.0.2.dev0/eon_collective_docs_theme.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 eon_collective_docs_theme/sitemap.html
 eon_collective_docs_theme/source-buttons.html
 eon_collective_docs_theme/theme.conf
 eon_collective_docs_theme.egg-info/PKG-INFO
 eon_collective_docs_theme.egg-info/SOURCES.txt
 eon_collective_docs_theme.egg-info/dependency_links.txt
 eon_collective_docs_theme.egg-info/top_level.txt
-eon_collective_docs_theme/UNKNOWN.egg-info/SOURCES.txt
-eon_collective_docs_theme/UNKNOWN.egg-info/dependency_links.txt
-eon_collective_docs_theme/UNKNOWN.egg-info/top_level.txt
-eon_collective_docs_theme/__pycache__/__init__.cpython-311.pyc
 eon_collective_docs_theme/dist/UNKNOWN-0.0.0.tar.gz
 eon_collective_docs_theme/static/dist/blocking.js
 eon_collective_docs_theme/static/dist/blocking.js.map
 eon_collective_docs_theme/static/dist/fontawesome.css
 eon_collective_docs_theme/static/dist/fontawesome.css.map
 eon_collective_docs_theme/static/dist/fontawesome.js
 eon_collective_docs_theme/static/dist/fontawesome.js.map
```

### Comparing `eon_collective_docs_theme-0.0.1.dev0/setup.cfg` & `eon_collective_docs_theme-0.0.2.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6f6e 5f63 6f6c 6c65 6374 6976   = eon_collectiv
 00000020: 655f 646f 6373 5f74 6865 6d65 0d0a 7665  e_docs_theme..ve
-00000030: 7273 696f 6e20 3d20 302e 302e 312e 6465  rsion = 0.0.1.de
+00000030: 7273 696f 6e20 3d20 302e 302e 322e 6465  rsion = 0.0.2.de
 00000040: 7630 0d0a 6175 7468 6f72 203d 204a 616e  v0..author = Jan
 00000050: 6572 6f73 6520 4e6a 6f67 750d 0a61 7574  erose Njogu..aut
 00000060: 686f 725f 656d 6169 6c20 3d20 6a61 6e65  hor_email = jane
 00000070: 726f 7365 2e6e 6a6f 6775 4065 6f6e 636c  rose.njogu@eoncl
 00000080: 6c65 6374 6976 652e 636f 6d0d 0a64 6573  lective.com..des
 00000090: 6372 6970 7469 6f6e 203d 2054 6865 2074  cription = The t
 000000a0: 6865 6d65 2075 7365 6420 746f 2072 656e  heme used to ren
```

### Comparing `eon_collective_docs_theme-0.0.1.dev0/tests/test_visual_regression.py` & `eon_collective_docs_theme-0.0.2.dev0/tests/test_visual_regression.py`

 * *Files identical despite different names*

