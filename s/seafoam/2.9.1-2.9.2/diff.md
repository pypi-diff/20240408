# Comparing `tmp/seafoam-2.9.1.tar.gz` & `tmp/seafoam-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seafoam-2.9.1.tar", last modified: Sun Jul 16 04:35:32 2023, max compression
+gzip compressed data, was "seafoam-2.9.2.tar", last modified: Tue Mar  5 04:57:31 2024, max compression
```

## Comparing `seafoam-2.9.1.tar` & `seafoam-2.9.2.tar`

### file list

```diff
@@ -1,158 +1,157 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.959628 seafoam-2.9.1/
--rw-rw-rw-   0        0        0     1133 2023-07-11 04:35:00.000000 seafoam-2.9.1/LICENSE.txt
--rw-rw-rw-   0        0        0      180 2023-07-11 04:35:00.000000 seafoam-2.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0    30907 2023-07-16 04:35:32.959628 seafoam-2.9.1/PKG-INFO
--rw-rw-rw-   0        0        0    29488 2023-07-14 18:03:53.000000 seafoam-2.9.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.773487 seafoam-2.9.1/docs/
--rw-rw-rw-   0        0        0    10252 2023-07-16 04:32:30.000000 seafoam-2.9.1/docs/CHANGELOG.rst
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.762817 seafoam-2.9.1/pelican/
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.762817 seafoam-2.9.1/pelican/plugins/
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.773487 seafoam-2.9.1/pelican/plugins/seafoam/
--rw-rw-rw-   0        0        0      829 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/__init__.py
--rw-rw-rw-   0        0        0      504 2023-07-16 04:35:10.000000 seafoam-2.9.1/pelican/plugins/seafoam/constants.py
--rw-rw-rw-   0        0        0     1005 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/formatting.py
--rw-rw-rw-   0        0        0     7606 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/initialize.py
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.763332 seafoam-2.9.1/pelican/plugins/seafoam/static/
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.773487 seafoam-2.9.1/pelican/plugins/seafoam/static/css/
--rw-rw-rw-   0        0        0   236433 2023-07-12 04:11:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css
--rw-rw-rw-   0        0        0   236036 2023-07-12 04:11:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.784029 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/
--rw-rw-rw-   0        0        0   134808 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/FontAwesome.otf
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.804750 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/
--rw-rw-rw-   0        0        0     2104 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt
--rw-rw-rw-   0        0        0     4460 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt
--rw-rw-rw-   0        0        0    18413 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot
--rw-rw-rw-   0        0        0    50449 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg
--rw-rw-rw-   0        0        0    35472 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf
--rw-rw-rw-   0        0        0    19444 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff
--rw-rw-rw-   0        0        0    15168 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2
--rw-rw-rw-   0        0        0    19294 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot
--rw-rw-rw-   0        0        0    56250 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg
--rw-rw-rw-   0        0        0    35176 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf
--rw-rw-rw-   0        0        0    20280 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff
--rw-rw-rw-   0        0        0    15856 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2
--rw-rw-rw-   0        0        0    19408 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot
--rw-rw-rw-   0        0        0    56028 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg
--rw-rw-rw-   0        0        0    35356 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf
--rw-rw-rw-   0        0        0    20416 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff
--rw-rw-rw-   0        0        0    16020 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2
--rw-rw-rw-   0        0        0    18842 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot
--rw-rw-rw-   0        0        0    50436 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg
--rw-rw-rw-   0        0        0    35700 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf
--rw-rw-rw-   0        0        0    19916 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff
--rw-rw-rw-   0        0        0    15476 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.816342 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/
--rw-rw-rw-   0        0        0    24884 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot
--rw-rw-rw-   0        0        0   128830 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg
--rw-rw-rw-   0        0        0    49124 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf
--rw-rw-rw-   0        0        0    25788 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff
--rw-rw-rw-   0        0        0    21932 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2
--rw-rw-rw-   0        0        0    25468 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot
--rw-rw-rw-   0        0        0   128299 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg
--rw-rw-rw-   0        0        0    47480 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf
--rw-rw-rw-   0        0        0    26508 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff
--rw-rw-rw-   0        0        0    22480 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2
--rw-rw-rw-   0        0        0    23567 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot
--rw-rw-rw-   0        0        0   127687 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg
--rw-rw-rw-   0        0        0    47032 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf
--rw-rw-rw-   0        0        0    24808 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff
--rw-rw-rw-   0        0        0    21020 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2
--rw-rw-rw-   0        0        0    23239 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot
--rw-rw-rw-   0        0        0   128551 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg
--rw-rw-rw-   0        0        0    48900 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf
--rw-rw-rw-   0        0        0    24304 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff
--rw-rw-rw-   0        0        0    20512 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.816342 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/
--rw-rw-rw-   0        0        0     4499 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt
--rw-rw-rw-   0        0        0    11207 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot
--rw-rw-rw-   0        0        0    60057 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg
--rw-rw-rw-   0        0        0    18564 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf
--rw-rw-rw-   0        0        0    13008 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff
--rw-rw-rw-   0        0        0    10084 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2
--rw-rw-rw-   0        0        0   165742 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0    20127 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0   109025 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    45404 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23424 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0        0        0    18028 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.825416 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/
--rw-rw-rw-   0        0        0    30028 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot
--rw-rw-rw-   0        0        0    81305 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg
--rw-rw-rw-   0        0        0    78804 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf
--rw-rw-rw-   0        0        0    36788 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff
--rw-rw-rw-   0        0        0    30116 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.846005 seafoam-2.9.1/pelican/plugins/seafoam/static/js/
--rw-rw-rw-   0        0        0    72084 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/bootstrap.js
--rw-rw-rw-   0        0        0    37051 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     2512 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/comments.js
--rw-rw-rw-   0        0        0     1520 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/github.js
--rw-rw-rw-   0        0        0     2558 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/jXHR.js
--rw-rw-rw-   0        0        0    86713 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/jquery.min.js
--rw-rw-rw-   0        0        0     4381 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/respond.min.js
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.866708 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.866708 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/img/
--rw-rw-rw-   0        0        0      368 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/img/search.png
--rw-rw-rw-   0        0        0     5901 2023-07-16 04:29:02.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css
--rw-rw-rw-   0        0        0    33641 2023-07-16 04:29:52.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js
--rw-rw-rw-   0        0        0    10697 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js
--rw-rw-rw-   0        0        0     4537 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js
--rw-rw-rw-   0        0        0     3670 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.876870 seafoam-2.9.1/pelican/plugins/seafoam/templates/
--rw-rw-rw-   0        0        0     1110 2023-07-16 04:24:25.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/404.html
--rw-rw-rw-   0        0        0     5875 2023-07-12 01:08:09.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/archives.html
--rw-rw-rw-   0        0        0     4860 2023-07-16 04:17:25.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/article.html
--rw-rw-rw-   0        0        0     1551 2023-07-12 03:05:35.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/article_list.html
--rw-rw-rw-   0        0        0      761 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/author.html
--rw-rw-rw-   0        0        0      857 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/authors.html
--rw-rw-rw-   0        0        0    15825 2023-07-13 02:15:55.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/base.html
--rw-rw-rw-   0        0        0     2053 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/categories.html
--rw-rw-rw-   0        0        0      738 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/category.html
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.938896 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/
--rw-rw-rw-   0        0        0      196 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/aboutme.html
--rw-rw-rw-   0        0        0      618 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/addthis.html
--rw-rw-rw-   0        0        0     1711 2023-07-16 03:57:48.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/article_info.html
--rw-rw-rw-   0        0        0     3389 2023-07-12 04:29:59.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/article_listing.html
--rw-rw-rw-   0        0        0      996 2023-07-16 04:30:06.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/assets-css.html
--rw-rw-rw-   0        0        0      219 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/assets-js.html
--rw-rw-rw-   0        0        0     4405 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/cc-license.html
--rw-rw-rw-   0        0        0      559 2023-07-16 04:30:14.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/comment_count.html
--rw-rw-rw-   0        0        0     1640 2023-07-16 04:30:31.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/comments-js.html
--rw-rw-rw-   0        0        0     7976 2023-07-16 04:30:55.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/comments.html
--rw-rw-rw-   0        0        0      741 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/disqus_script.html
--rw-rw-rw-   0        0        0     3869 2023-07-12 00:31:05.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/footer.html
--rw-rw-rw-   0        0        0     1818 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/ga.html
--rw-rw-rw-   0        0        0     1308 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/github-js.html
--rw-rw-rw-   0        0        0      442 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/github.html
--rw-rw-rw-   0        0        0      434 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/links.html
--rw-rw-rw-   0        0        0     3418 2023-07-16 04:19:58.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/neighbors.html
--rw-rw-rw-   0        0        0     2955 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/pagination.html
--rw-rw-rw-   0        0        0      872 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/piwik.html
--rw-rw-rw-   0        0        0      564 2023-07-16 04:30:40.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/prjct.html
--rw-rw-rw-   0        0        0      357 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/related-posts.html
--rw-rw-rw-   0        0        0     3533 2023-07-16 04:22:30.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/sidebar.html
--rw-rw-rw-   0        0        0      319 2023-07-16 04:22:45.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/taglist.html
--rw-rw-rw-   0        0        0      329 2023-07-16 04:30:47.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/translations.html
--rw-rw-rw-   0        0        0      703 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/twitter_timeline.html
--rw-rw-rw-   0        0        0      796 2023-07-12 03:06:56.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/index.html
--rw-rw-rw-   0        0        0     2474 2023-07-13 02:04:28.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/page.html
--rw-rw-rw-   0        0        0     7104 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/period_archives.html
--rw-rw-rw-   0        0        0     4517 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/prjct.html
--rw-rw-rw-   0        0        0     1507 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/search.html
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.938896 seafoam-2.9.1/pelican/plugins/seafoam/templates/strathcona/
--rw-rw-rw-   0        0        0     8939 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html
--rw-rw-rw-   0        0        0     5443 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/strathcona/pricing.html
--rw-rw-rw-   0        0        0      795 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/tag.html
--rw-rw-rw-   0        0        0     2036 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/tags.html
--rw-rw-rw-   0        0        0      429 2023-07-11 04:35:00.000000 seafoam-2.9.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.959628 seafoam-2.9.1/seafoam.egg-info/
--rw-rw-rw-   0        0        0    30907 2023-07-16 04:35:32.000000 seafoam-2.9.1/seafoam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8286 2023-07-16 04:35:32.000000 seafoam-2.9.1/seafoam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 04:35:32.000000 seafoam-2.9.1/seafoam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-07-16 04:35:32.000000 seafoam-2.9.1/seafoam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       41 2023-07-16 04:35:32.000000 seafoam-2.9.1/seafoam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-07-16 04:35:32.959628 seafoam-2.9.1/setup.cfg
--rw-rw-rw-   0        0        0     4767 2023-07-11 04:35:00.000000 seafoam-2.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.226488 seafoam-2.9.2/
+-rw-rw-rw-   0        0        0     1133 2023-07-11 04:35:00.000000 seafoam-2.9.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      180 2023-07-11 04:35:00.000000 seafoam-2.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    31434 2024-03-05 04:57:31.226488 seafoam-2.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0    29488 2023-07-14 18:03:53.000000 seafoam-2.9.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.119391 seafoam-2.9.2/docs/
+-rw-rw-rw-   0        0        0    10623 2024-03-05 04:43:27.000000 seafoam-2.9.2/docs/CHANGELOG.rst
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.111383 seafoam-2.9.2/pelican/
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.112384 seafoam-2.9.2/pelican/plugins/
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.121392 seafoam-2.9.2/pelican/plugins/seafoam/
+-rw-rw-rw-   0        0        0      829 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/__init__.py
+-rw-rw-rw-   0        0        0      504 2024-03-05 04:57:28.000000 seafoam-2.9.2/pelican/plugins/seafoam/constants.py
+-rw-rw-rw-   0        0        0     1005 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/formatting.py
+-rw-rw-rw-   0        0        0     7606 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/initialize.py
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.113385 seafoam-2.9.2/pelican/plugins/seafoam/static/
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.123394 seafoam-2.9.2/pelican/plugins/seafoam/static/css/
+-rw-rw-rw-   0        0        0   248572 2024-03-05 02:47:01.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css
+-rw-rw-rw-   0        0        0   248175 2024-03-05 02:47:01.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.131401 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/FontAwesome.otf
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.146415 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/
+-rw-rw-rw-   0        0        0     2104 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt
+-rw-rw-rw-   0        0        0     4460 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt
+-rw-rw-rw-   0        0        0    18413 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot
+-rw-rw-rw-   0        0        0    50449 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg
+-rw-rw-rw-   0        0        0    35472 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf
+-rw-rw-rw-   0        0        0    19444 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff
+-rw-rw-rw-   0        0        0    15168 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2
+-rw-rw-rw-   0        0        0    19294 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot
+-rw-rw-rw-   0        0        0    56250 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg
+-rw-rw-rw-   0        0        0    35176 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf
+-rw-rw-rw-   0        0        0    20280 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff
+-rw-rw-rw-   0        0        0    15856 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2
+-rw-rw-rw-   0        0        0    19408 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot
+-rw-rw-rw-   0        0        0    56028 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg
+-rw-rw-rw-   0        0        0    35356 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf
+-rw-rw-rw-   0        0        0    20416 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff
+-rw-rw-rw-   0        0        0    16020 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2
+-rw-rw-rw-   0        0        0    18842 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot
+-rw-rw-rw-   0        0        0    50436 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg
+-rw-rw-rw-   0        0        0    35700 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf
+-rw-rw-rw-   0        0        0    19916 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff
+-rw-rw-rw-   0        0        0    15476 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.161429 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/
+-rw-rw-rw-   0        0        0    24884 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot
+-rw-rw-rw-   0        0        0   128830 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg
+-rw-rw-rw-   0        0        0    49124 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf
+-rw-rw-rw-   0        0        0    25788 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff
+-rw-rw-rw-   0        0        0    21932 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2
+-rw-rw-rw-   0        0        0    25468 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot
+-rw-rw-rw-   0        0        0   128299 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg
+-rw-rw-rw-   0        0        0    47480 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf
+-rw-rw-rw-   0        0        0    26508 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff
+-rw-rw-rw-   0        0        0    22480 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2
+-rw-rw-rw-   0        0        0    23567 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot
+-rw-rw-rw-   0        0        0   127687 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg
+-rw-rw-rw-   0        0        0    47032 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf
+-rw-rw-rw-   0        0        0    24808 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff
+-rw-rw-rw-   0        0        0    21020 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2
+-rw-rw-rw-   0        0        0    23239 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot
+-rw-rw-rw-   0        0        0   128551 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg
+-rw-rw-rw-   0        0        0    48900 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf
+-rw-rw-rw-   0        0        0    24304 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff
+-rw-rw-rw-   0        0        0    20512 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.165432 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/
+-rw-rw-rw-   0        0        0     4499 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt
+-rw-rw-rw-   0        0        0    11207 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot
+-rw-rw-rw-   0        0        0    60057 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg
+-rw-rw-rw-   0        0        0    18564 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf
+-rw-rw-rw-   0        0        0    13008 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff
+-rw-rw-rw-   0        0        0    10084 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2
+-rw-rw-rw-   0        0        0   165742 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0    20127 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0   109025 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    45404 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23424 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0        0        0    18028 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.169435 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/vidaloka/
+-rw-rw-rw-   0        0        0    30028 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot
+-rw-rw-rw-   0        0        0    81305 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg
+-rw-rw-rw-   0        0        0    78804 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf
+-rw-rw-rw-   0        0        0    36788 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff
+-rw-rw-rw-   0        0        0    30116 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.173440 seafoam-2.9.2/pelican/plugins/seafoam/static/js/
+-rw-rw-rw-   0        0        0    72084 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/js/bootstrap.js
+-rw-rw-rw-   0        0        0    37051 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     2512 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/js/comments.js
+-rw-rw-rw-   0        0        0     1520 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/js/github.js
+-rw-rw-rw-   0        0        0     2558 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/js/jXHR.js
+-rw-rw-rw-   0        0        0    86713 2024-03-05 04:41:01.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/js/jquery.min.js
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.177443 seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.178444 seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/img/
+-rw-rw-rw-   0        0        0      368 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/img/search.png
+-rw-rw-rw-   0        0        0     5901 2023-07-16 04:29:02.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css
+-rw-rw-rw-   0        0        0    33641 2023-07-16 04:29:52.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js
+-rw-rw-rw-   0        0        0    10697 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js
+-rw-rw-rw-   0        0        0     4537 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js
+-rw-rw-rw-   0        0        0     3670 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.188453 seafoam-2.9.2/pelican/plugins/seafoam/templates/
+-rw-rw-rw-   0        0        0     1110 2023-07-16 04:24:25.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/404.html
+-rw-rw-rw-   0        0        0     5875 2023-07-12 01:08:09.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/archives.html
+-rw-rw-rw-   0        0        0     4860 2023-07-16 04:17:25.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/article.html
+-rw-rw-rw-   0        0        0     1551 2023-07-12 03:05:35.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/article_list.html
+-rw-rw-rw-   0        0        0      761 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/author.html
+-rw-rw-rw-   0        0        0      857 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/authors.html
+-rw-rw-rw-   0        0        0    15825 2024-03-05 04:41:01.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/base.html
+-rw-rw-rw-   0        0        0     2053 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/categories.html
+-rw-rw-rw-   0        0        0      738 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/category.html
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.205468 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/
+-rw-rw-rw-   0        0        0      196 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/aboutme.html
+-rw-rw-rw-   0        0        0      618 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/addthis.html
+-rw-rw-rw-   0        0        0     1715 2024-03-05 03:36:25.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/article_info.html
+-rw-rw-rw-   0        0        0     3389 2023-07-12 04:29:59.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/article_listing.html
+-rw-rw-rw-   0        0        0      996 2023-07-16 04:30:06.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/assets-css.html
+-rw-rw-rw-   0        0        0      219 2024-03-05 04:41:01.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/assets-js.html
+-rw-rw-rw-   0        0        0     4405 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/cc-license.html
+-rw-rw-rw-   0        0        0      559 2023-07-16 04:30:14.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/comment_count.html
+-rw-rw-rw-   0        0        0     1640 2024-03-05 04:41:01.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/comments-js.html
+-rw-rw-rw-   0        0        0     7976 2023-07-16 04:30:55.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/comments.html
+-rw-rw-rw-   0        0        0      741 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/disqus_script.html
+-rw-rw-rw-   0        0        0     3869 2023-07-12 00:31:05.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/footer.html
+-rw-rw-rw-   0        0        0     1818 2024-03-05 04:41:01.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/ga.html
+-rw-rw-rw-   0        0        0     1308 2024-03-05 04:41:01.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/github-js.html
+-rw-rw-rw-   0        0        0      442 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/github.html
+-rw-rw-rw-   0        0        0      434 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/links.html
+-rw-rw-rw-   0        0        0     3447 2024-03-05 02:48:35.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/neighbors.html
+-rw-rw-rw-   0        0        0     2955 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/pagination.html
+-rw-rw-rw-   0        0        0      872 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/piwik.html
+-rw-rw-rw-   0        0        0      564 2023-07-16 04:30:40.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/prjct.html
+-rw-rw-rw-   0        0        0      357 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/related-posts.html
+-rw-rw-rw-   0        0        0     3533 2023-07-16 04:22:30.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/sidebar.html
+-rw-rw-rw-   0        0        0      319 2024-03-05 03:38:24.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/taglist.html
+-rw-rw-rw-   0        0        0      329 2023-07-16 04:30:47.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/translations.html
+-rw-rw-rw-   0        0        0      703 2024-03-05 04:41:01.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/twitter_timeline.html
+-rw-rw-rw-   0        0        0      796 2023-07-12 03:06:56.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/index.html
+-rw-rw-rw-   0        0        0     2474 2023-07-13 02:04:28.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/page.html
+-rw-rw-rw-   0        0        0     7104 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/period_archives.html
+-rw-rw-rw-   0        0        0     4517 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/prjct.html
+-rw-rw-rw-   0        0        0     1507 2024-03-05 04:41:01.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/search.html
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.206469 seafoam-2.9.2/pelican/plugins/seafoam/templates/strathcona/
+-rw-rw-rw-   0        0        0     8939 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html
+-rw-rw-rw-   0        0        0     5443 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/strathcona/pricing.html
+-rw-rw-rw-   0        0        0      795 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/tag.html
+-rw-rw-rw-   0        0        0     2036 2023-07-11 04:35:00.000000 seafoam-2.9.2/pelican/plugins/seafoam/templates/tags.html
+-rw-rw-rw-   0        0        0      429 2023-07-11 04:35:00.000000 seafoam-2.9.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-03-05 04:57:31.224486 seafoam-2.9.2/seafoam.egg-info/
+-rw-rw-rw-   0        0        0    31434 2024-03-05 04:57:31.000000 seafoam-2.9.2/seafoam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8237 2024-03-05 04:57:31.000000 seafoam-2.9.2/seafoam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-05 04:57:31.000000 seafoam-2.9.2/seafoam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2024-03-05 04:57:31.000000 seafoam-2.9.2/seafoam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       41 2024-03-05 04:57:31.000000 seafoam-2.9.2/seafoam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2024-03-05 04:57:31.230491 seafoam-2.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     4767 2023-07-11 04:35:00.000000 seafoam-2.9.2/setup.py
```

### Comparing `seafoam-2.9.1/LICENSE.txt` & `seafoam-2.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/PKG-INFO` & `seafoam-2.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seafoam
-Version: 2.9.1
+Version: 2.9.2
 Summary: Pelican theme, first used for Minchin.ca.
 Home-page: http://blog.minchin.ca/label/seafoam/
 Author: W. Minchin
 Author-email: w_minchin@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/seafoam/issues
 Project-URL: Changelog, https://github.com/MinchinWeb/seafoam/blob/master/docs/changelog.rst
@@ -22,21 +22,34 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: pelican
+Requires-Dist: pelican-image-process>=2.1.1
+Requires-Dist: pelican-jinja-filters>=2.1.0
+Requires-Dist: semantic_version
+Requires-Dist: beautifulsoup4
 Provides-Extra: lxml
+Requires-Dist: lxml; extra == "lxml"
 Provides-Extra: build
+Requires-Dist: minchin.releaser>=0.8.2; extra == "build"
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: dev
+Requires-Dist: markdown; extra == "dev"
+Requires-Dist: invoke; extra == "dev"
 Provides-Extra: all
-License-File: LICENSE.txt
+Requires-Dist: lxml; extra == "all"
+Requires-Dist: minchin.releaser>=0.8.2; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: invoke; extra == "all"
 
 =======
 Seafoam
 =======
 
 .. image:: https://raw.githubusercontent.com/MinchinWeb/seafoam/master/docs/seafoam-logo-4x.png
     :align: center
```

### Comparing `seafoam-2.9.1/README.rst` & `seafoam-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/docs/CHANGELOG.rst` & `seafoam-2.9.2/docs/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 Changelog
 =========
 
 .. Added, Changed, Depreciated, Removed, Fixed, Security
 
+- :release:`2.9.2 <2024-03-04>`
+- :support:`- minor` remove ``respond.js``. This was initially added to support
+  Internet Explorer 6 to 8, which have since faded away. Plus it was throwing
+  an Javascript error.
+- :bug:`-` fix missing icons (micropost category next link) and icon spacing
+  (readtime and tags in article details).
+- :release:`2.9.1 <2023-07-15>`
 - :support:`- minor` convert indentation to spaces
 - :bug:`-` better display of micropost links
 - :release:`2.9.0 <2023-07-14>`
 - :feature:`-` add support for *microblogging*, through my `microblogging
   plugin <https://blog.minchin.ca/label/microblogging-pelican/>`_.
   c.f. `blog.minchin.ca Issue #105
   <https://github.com/MinchinWeb/blog.minchin.ca/issues/105>`_.
```

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/__init__.py` & `seafoam-2.9.2/pelican/plugins/seafoam/__init__.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/formatting.py` & `seafoam-2.9.2/pelican/plugins/seafoam/formatting.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/initialize.py` & `seafoam-2.9.2/pelican/plugins/seafoam/initialize.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/FontAwesome.otf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2` & `seafoam-2.9.2/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/js/bootstrap.js` & `seafoam-2.9.2/pelican/plugins/seafoam/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/js/bootstrap.min.js` & `seafoam-2.9.2/pelican/plugins/seafoam/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/js/comments.js` & `seafoam-2.9.2/pelican/plugins/seafoam/static/js/comments.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/js/github.js` & `seafoam-2.9.2/pelican/plugins/seafoam/static/js/github.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/js/jXHR.js` & `seafoam-2.9.2/pelican/plugins/seafoam/static/js/jXHR.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/js/jquery.min.js` & `seafoam-2.9.2/pelican/plugins/seafoam/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css` & `seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js` & `seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js` & `seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js` & `seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js` & `seafoam-2.9.2/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/404.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/404.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/archives.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/archives.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/article.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/article.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/article_list.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/article_list.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/author.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/author.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/authors.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/authors.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/base.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/base.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/categories.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/categories.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/category.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/category.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/addthis.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/addthis.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/article_info.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/article_info.html`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,17 @@
     {#{% if article.author %}#}
     {#<span class="label">By</span>#}
     {#<a href="{{ SITEURL -}} / {{- article.author.url }}"><i class="fa fa-user"></i> {{ article.author }}</a>#}
     {#{% endif -%}-#}
 
     {%- if not article.micro -%}
         {%- if article.readtime_minutes -%}
-            <span class="label label-default">Reading Time</span>
-            <i class="fa fa-clock-o"></i> ~{{ article.readtime_minutes }} min
+            <span class="label label-default">Reading Time</span>&nbsp;<i class="fa fa-clock-o"></i>&nbsp;~{{ article.readtime_minutes }}&nbsp;min
         {%- elif article.stats -%}
-            <span class="label label-default">Reading Time</span>
-            <i class="fa fa-clock-o"></i> ~{{ article.stats['read_mins'] }} min
+            <span class="label label-default">Reading Time</span>&nbsp;<i class="fa fa-clock-o"></i>&nbsp;~{{ article.stats['read_mins'] }}&nbsp;min
         {%- endif -%}
     {%- endif -%}
 
     {#- Uncomment if you want to show Categories#}
     {#<span class="label label-default">Category</span>#}
     {#<a href="{{ SITEURL -}} / {{- article.category.url }}">{{ article.category }}</a>-#}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 Published {{ article.date | article_date }} {% if article.micro %} at {
 { article.date | datetime("%H:%M") }} {% endif -%} {# Uncomment if you want the
 author shown #} {#{% if article.author %}#} {#By#} {#
  _{_{_ _a_r_t_i_c_l_e_._a_u_t_h_o_r_ _}_}
 #} {#{% endif -%}-#} {%- if not article.micro -%} {%- if
-article.readtime_minutes -%} Reading Time ~{{ article.readtime_minutes }} min
-{%- elif article.stats -%} Reading Time ~{{ article.stats['read_mins'] }} min
+article.readtime_minutes -%} Reading Time  ~{{ article.readtime_minutes }} min
+{%- elif article.stats -%} Reading Time  ~{{ article.stats['read_mins'] }} min
 {%- endif -%} {%- endif -%} {#- Uncomment if you want to show Categories#}
 {#Category#} {#_{_{_ _a_r_t_i_c_l_e_._c_a_t_e_g_o_r_y_ _}_}-#} {%- if PDF_PROCESSOR %} _P_D_F {% endif -
 %} {%- include 'includes/taglist.html' %} {% import 'includes/
 translations.html' as translations with context %} {
 { translations.translations_for(article) }}
```

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/article_listing.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/article_listing.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/assets-css.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/assets-css.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/cc-license.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/cc-license.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/comment_count.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/comment_count.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/comments-js.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/comments-js.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/comments.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/comments.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/disqus_script.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/disqus_script.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/footer.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/footer.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/ga.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/ga.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/github-js.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/github-js.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/neighbors.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/neighbors.html`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,17 @@
                 {% endif %}
                 {% if article.next_article_in_category %}
                     <li class="next">
                         <a href="{{ SITEURL -}} / {{- article.next_article_in_category.url }}">
                             {%- if article.next_article_in_category.micro %}
                                 {{- article.next_article_in_category.date | datetime("%B %d, %Y at %H:%M") }}
                             {%- else %}
-                                {{- article.next_article_in_category.title }} <i class="fa fa-arrow-circle-right"></i>
+                                {{- article.next_article_in_category.title }}
                             {%- endif %}
+                            <i class="fa fa-arrow-circle-right"></i>
                         </a>
                     </li>
                 {% endif %}
             </ul>
         {% else %}
             <!-- no other articles in category {{ article.category }}, skipping... -->
         {% endif %}
```

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/pagination.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/piwik.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/piwik.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/prjct.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/prjct.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/sidebar.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/sidebar.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/twitter_timeline.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/includes/twitter_timeline.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/index.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/index.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/page.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/page.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/period_archives.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/period_archives.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/prjct.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/prjct.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/search.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/search.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/strathcona/pricing.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/strathcona/pricing.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/tag.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/tag.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/pelican/plugins/seafoam/templates/tags.html` & `seafoam-2.9.2/pelican/plugins/seafoam/templates/tags.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.1/seafoam.egg-info/PKG-INFO` & `seafoam-2.9.2/seafoam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seafoam
-Version: 2.9.1
+Version: 2.9.2
 Summary: Pelican theme, first used for Minchin.ca.
 Home-page: http://blog.minchin.ca/label/seafoam/
 Author: W. Minchin
 Author-email: w_minchin@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/seafoam/issues
 Project-URL: Changelog, https://github.com/MinchinWeb/seafoam/blob/master/docs/changelog.rst
@@ -22,21 +22,34 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: pelican
+Requires-Dist: pelican-image-process>=2.1.1
+Requires-Dist: pelican-jinja-filters>=2.1.0
+Requires-Dist: semantic_version
+Requires-Dist: beautifulsoup4
 Provides-Extra: lxml
+Requires-Dist: lxml; extra == "lxml"
 Provides-Extra: build
+Requires-Dist: minchin.releaser>=0.8.2; extra == "build"
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: dev
+Requires-Dist: markdown; extra == "dev"
+Requires-Dist: invoke; extra == "dev"
 Provides-Extra: all
-License-File: LICENSE.txt
+Requires-Dist: lxml; extra == "all"
+Requires-Dist: minchin.releaser>=0.8.2; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: invoke; extra == "all"
 
 =======
 Seafoam
 =======
 
 .. image:: https://raw.githubusercontent.com/MinchinWeb/seafoam/master/docs/seafoam-logo-4x.png
     :align: center
```

### Comparing `seafoam-2.9.1/seafoam.egg-info/SOURCES.txt` & `seafoam-2.9.2/seafoam.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
 pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2
 pelican/plugins/seafoam/static/js/bootstrap.js
 pelican/plugins/seafoam/static/js/bootstrap.min.js
 pelican/plugins/seafoam/static/js/comments.js
 pelican/plugins/seafoam/static/js/github.js
 pelican/plugins/seafoam/static/js/jXHR.js
 pelican/plugins/seafoam/static/js/jquery.min.js
-pelican/plugins/seafoam/static/js/respond.min.js
 pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css
 pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js
 pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js
 pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js
 pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js
 pelican/plugins/seafoam/static/tipuesearch/img/search.png
 pelican/plugins/seafoam/templates/404.html
```

### Comparing `seafoam-2.9.1/setup.py` & `seafoam-2.9.2/setup.py`

 * *Files identical despite different names*

