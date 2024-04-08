# Comparing `tmp/scPANTHEON-0.5.5.tar.gz` & `tmp/scPANTHEON-0.5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.5.5.tar", last modified: Mon Apr  8 14:56:24 2024, max compression
+gzip compressed data, was "scPANTHEON-0.5.5.1.tar", last modified: Mon Apr  8 14:57:43 2024, max compression
```

## Comparing `scPANTHEON-0.5.5.tar` & `scPANTHEON-0.5.5.1.tar`

### file list

```diff
@@ -1,329 +1,329 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.726164 scPANTHEON-0.5.5/
--rw-rw-rw-   0        0        0      132 2024-03-24 08:59:16.000000 scPANTHEON-0.5.5/.gitattributes
--rw-rw-rw-   0        0        0       66 2024-04-02 11:16:17.000000 scPANTHEON-0.5.5/.gitignore
--rw-rw-rw-   0        0        0   837120 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/10k-genomics.png
--rw-rw-rw-   0        0        0      238 2024-04-08 14:56:24.725164 scPANTHEON-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-01-02 19:33:04.000000 scPANTHEON-0.5.5/README.md
--rw-rw-rw-   0        0        0        0 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.191603 scPANTHEON-0.5.5/__pycache__/
--rw-rw-rw-   0        0        0      143 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      689 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5/__pycache__/main.cpython-39.pyc
--rw-rw-rw-   0        0        0     3789 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5/__pycache__/qt.cpython-39.pyc
--rw-rw-rw-   0        0        0      363 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5/__pycache__/run.cpython-39.pyc
--rw-rw-rw-   0        0        0    35541 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5/__pycache__/source.cpython-36.pyc
--rw-rw-rw-   0        0        0    35243 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5/__pycache__/source.cpython-38.pyc
--rw-rw-rw-   0        0        0    35200 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5/__pycache__/source.cpython-39.pyc
--rw-rw-rw-   0        0        0    37871 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5/__pycache__/sourceqt.cpython-39.pyc
--rw-rw-rw-   0        0        0      631 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5/__pycache__/transform.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.195633 scPANTHEON-0.5.5/document/
--rw-rw-rw-   0        0        0      658 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/Makefile
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.219712 scPANTHEON-0.5.5/document/build/
--rw-rw-rw-   0        0        0      234 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/.buildinfo
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.230748 scPANTHEON-0.5.5/document/build/.doctrees/
--rw-rw-rw-   0        0        0     2390 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/.doctrees/Download.doctree
--rw-rw-rw-   0        0        0     3738 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/.doctrees/Introduction.doctree
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.238780 scPANTHEON-0.5.5/document/build/.doctrees/Tutorials/
--rw-rw-rw-   0        0        0     2470 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/.doctrees/Tutorials/Clustering with sacnpy.doctree
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.240289 scPANTHEON-0.5.5/document/build/.doctrees/Tutorials/Navigation/
--rw-rw-rw-   0        0        0    19370 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/.doctrees/Tutorials/Navigation/contents.doctree
--rw-rw-rw-   0        0        0     2485 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/.doctrees/Tutorials/Preprocessing with scanpy.doctree
--rw-rw-rw-   0        0        0     2844 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/.doctrees/Tutorials/index.doctree
--rw-rw-rw-   0        0        0    19829 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/.doctrees/environment.pickle
--rw-rw-rw-   0        0        0     4036 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/.doctrees/index.doctree
--rw-rw-rw-   0        0        0     4380 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/Download.html
--rw-rw-rw-   0        0        0     4782 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/Introduction.html
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.248355 scPANTHEON-0.5.5/document/build/Tutorials/
--rw-rw-rw-   0        0        0     4758 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/Tutorials/Clustering with sacnpy.html
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.251356 scPANTHEON-0.5.5/document/build/Tutorials/Navigation/
--rw-rw-rw-   0        0        0    12677 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/Tutorials/Navigation/contents.html
--rw-rw-rw-   0        0        0     5036 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/Tutorials/Preprocessing with scanpy.html
--rw-rw-rw-   0        0        0     6225 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/Tutorials/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.278029 scPANTHEON-0.5.5/document/build/_images/
--rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/_images/1overview0.png
--rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/_images/2mouse1.png
--rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/_images/3map.png
--rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/_images/3map1.png
--rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5/document/build/_images/3map2.png
--rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_images/3map3.png
--rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_images/4plot1.png
--rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_images/5group1.png
--rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_images/6cluster1.png
--rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_images/6cluster2.png
--rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_images/7hlg1.png
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.285051 scPANTHEON-0.5.5/document/build/_sources/
--rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_sources/Download.rst.txt
--rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_sources/Introduction.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.291051 scPANTHEON-0.5.5/document/build/_sources/Tutorials/
--rw-rw-rw-   0        0        0       46 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_sources/Tutorials/Clustering with sacnpy.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.293567 scPANTHEON-0.5.5/document/build/_sources/Tutorials/Navigation/
--rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_sources/Tutorials/Navigation/contents.rst.txt
--rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_sources/Tutorials/Preprocessing with scanpy.rst.txt
--rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_sources/Tutorials/index.rst.txt
--rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.328078 scPANTHEON-0.5.5/document/build/_static/
--rw-rw-rw-   0        0        0     4552 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-rw-   0        0        0    11885 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/alabaster.css
--rw-rw-rw-   0        0        0    15519 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/basic.css
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.332076 scPANTHEON-0.5.5/document/build/_static/css/
--rw-rw-rw-   0        0        0     3275 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/badge_only.css
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.372235 scPANTHEON-0.5.5/document/build/_static/css/fonts/
--rw-rw-rw-   0        0        0    87624 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-rw-   0        0        0    67312 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-rw-   0        0        0    86288 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-rw-   0        0        0    66444 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-rw-   0        0        0   165742 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0   323344 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-bold-italic.woff
--rw-rw-rw-   0        0        0   193308 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-rw-   0        0        0   309728 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-bold.woff
--rw-rw-rw-   0        0        0   184912 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-bold.woff2
--rw-rw-rw-   0        0        0   328412 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-normal-italic.woff
--rw-rw-rw-   0        0        0   195704 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-rw-   0        0        0   309192 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-normal.woff
--rw-rw-rw-   0        0        0   182708 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-normal.woff2
--rw-rw-rw-   0        0        0   129677 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/css/theme.css
--rw-rw-rw-   0        0        0       43 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/custom.css
--rw-rw-rw-   0        0        0     8435 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/doctools.js
--rw-rw-rw-   0        0        0      433 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/file.png
--rw-rw-rw-   0        0        0   299461 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/jquery-3.6.0.js
--rw-rw-rw-   0        0        0    89503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/jquery.js
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.380268 scPANTHEON-0.5.5/document/build/_static/js/
--rw-rw-rw-   0        0        0      934 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/js/badge_only.js
--rw-rw-rw-   0        0        0     4373 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/js/html5shiv-printshiv.min.js
--rw-rw-rw-   0        0        0     2737 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/js/html5shiv.min.js
--rw-rw-rw-   0        0        0     5023 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/js/theme.js
--rw-rw-rw-   0        0        0     4957 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/plus.png
--rw-rw-rw-   0        0        0     4892 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/pygments.css
--rw-rw-rw-   0        0        0    17650 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/searchtools.js
--rw-rw-rw-   0        0        0    70462 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/underscore-1.13.1.js
--rw-rw-rw-   0        0        0    19535 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/_static/underscore.js
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.388290 scPANTHEON-0.5.5/document/build/doctrees/
--rw-rw-rw-   0        0        0     2390 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/doctrees/Download.doctree
--rw-rw-rw-   0        0        0     3738 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/doctrees/Introduction.doctree
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.393289 scPANTHEON-0.5.5/document/build/doctrees/Tutorials/
--rw-rw-rw-   0        0        0     2470 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/doctrees/Tutorials/Clustering with sacnpy.doctree
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.395102 scPANTHEON-0.5.5/document/build/doctrees/Tutorials/Navigation/
--rw-rw-rw-   0        0        0    19370 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/doctrees/Tutorials/Navigation/contents.doctree
--rw-rw-rw-   0        0        0     2485 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/doctrees/Tutorials/Preprocessing with scanpy.doctree
--rw-rw-rw-   0        0        0     2844 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/doctrees/Tutorials/index.doctree
--rw-rw-rw-   0        0        0    19803 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/doctrees/environment.pickle
--rw-rw-rw-   0        0        0     4036 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/doctrees/index.doctree
--rw-rw-rw-   0        0        0     3491 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/genindex.html
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.410244 scPANTHEON-0.5.5/document/build/html/
--rw-rw-rw-   0        0        0      234 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/.buildinfo
--rw-rw-rw-   0        0        0     4380 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/Download.html
--rw-rw-rw-   0        0        0     4782 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/Introduction.html
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.416042 scPANTHEON-0.5.5/document/build/html/Tutorials/
--rw-rw-rw-   0        0        0     4758 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/Tutorials/Clustering with sacnpy.html
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.418040 scPANTHEON-0.5.5/document/build/html/Tutorials/Navigation/
--rw-rw-rw-   0        0        0    12248 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/Tutorials/Navigation/contents.html
--rw-rw-rw-   0        0        0     5036 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/Tutorials/Preprocessing with scanpy.html
--rw-rw-rw-   0        0        0     6225 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/Tutorials/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.439077 scPANTHEON-0.5.5/document/build/html/_images/
--rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_images/1overview0.png
--rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_images/2mouse1.png
--rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_images/3map.png
--rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_images/3map1.png
--rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_images/3map2.png
--rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_images/3map3.png
--rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_images/4plot1.png
--rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_images/5group1.png
--rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_images/6cluster1.png
--rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_images/6cluster2.png
--rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_images/7hlg1.png
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.445149 scPANTHEON-0.5.5/document/build/html/_sources/
--rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_sources/Download.rst.txt
--rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_sources/Introduction.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.451182 scPANTHEON-0.5.5/document/build/html/_sources/Tutorials/
--rw-rw-rw-   0        0        0       46 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_sources/Tutorials/Clustering with sacnpy.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.453181 scPANTHEON-0.5.5/document/build/html/_sources/Tutorials/Navigation/
--rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_sources/Tutorials/Navigation/contents.rst.txt
--rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_sources/Tutorials/Preprocessing with scanpy.rst.txt
--rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_sources/Tutorials/index.rst.txt
--rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.480013 scPANTHEON-0.5.5/document/build/html/_static/
--rw-rw-rw-   0        0        0     4552 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-rw-   0        0        0    15519 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/basic.css
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.483009 scPANTHEON-0.5.5/document/build/html/_static/css/
--rw-rw-rw-   0        0        0     3275 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/badge_only.css
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.527284 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/
--rw-rw-rw-   0        0        0    87624 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-rw-   0        0        0    67312 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-rw-   0        0        0    86288 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-rw-   0        0        0    66444 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-rw-   0        0        0   165742 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0   323344 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-rw-rw-   0        0        0   193308 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-rw-   0        0        0   309728 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-bold.woff
--rw-rw-rw-   0        0        0   184912 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-bold.woff2
--rw-rw-rw-   0        0        0   328412 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-rw-rw-   0        0        0   195704 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-rw-   0        0        0   309192 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-normal.woff
--rw-rw-rw-   0        0        0   182708 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-normal.woff2
--rw-rw-rw-   0        0        0   129677 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/css/theme.css
--rw-rw-rw-   0        0        0     8435 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/doctools.js
--rw-rw-rw-   0        0        0      433 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/file.png
--rw-rw-rw-   0        0        0   299461 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/jquery-3.6.0.js
--rw-rw-rw-   0        0        0    89503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/jquery.js
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.536003 scPANTHEON-0.5.5/document/build/html/_static/js/
--rw-rw-rw-   0        0        0      934 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/js/badge_only.js
--rw-rw-rw-   0        0        0     4373 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/js/html5shiv-printshiv.min.js
--rw-rw-rw-   0        0        0     2737 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/js/html5shiv.min.js
--rw-rw-rw-   0        0        0     5023 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/js/theme.js
--rw-rw-rw-   0        0        0     4957 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/plus.png
--rw-rw-rw-   0        0        0     4892 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/pygments.css
--rw-rw-rw-   0        0        0    17650 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/searchtools.js
--rw-rw-rw-   0        0        0    70462 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/underscore-1.13.1.js
--rw-rw-rw-   0        0        0    19535 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/_static/underscore.js
--rw-rw-rw-   0        0        0     3491 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/genindex.html
--rw-rw-rw-   0        0        0     6035 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/index.html
--rw-rw-rw-   0        0        0      382 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/objects.inv
--rw-rw-rw-   0        0        0     3905 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/search.html
--rw-rw-rw-   0        0        0     3080 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/html/searchindex.js
--rw-rw-rw-   0        0        0     6035 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/index.html
--rw-rw-rw-   0        0        0      382 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/objects.inv
--rw-rw-rw-   0        0        0     3905 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/search.html
--rw-rw-rw-   0        0        0     3339 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/build/searchindex.js
--rwxrwxrwx   0        0        0      804 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/make.bat
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.543021 scPANTHEON-0.5.5/document/source/
--rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Download.rst
--rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Introduction.rst
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.550140 scPANTHEON-0.5.5/document/source/Tutorials/
--rw-rw-rw-   0        0        0       46 2024-03-23 11:22:01.000000 scPANTHEON-0.5.5/document/source/Tutorials/Clustering with sacnpy.rst
--rw-rw-rw-   0        0        0       46 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5/document/source/Tutorials/Clustering with scanpy.rst
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.552141 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/
--rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/contents.rst
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.580080 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/
--rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/1overview0.png
--rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/2mouse1.png
--rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/3map.png
--rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/3map1.png
--rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/3map2.png
--rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/3map3.png
--rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/4plot1.png
--rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/5group1.png
--rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/6cluster1.png
--rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/6cluster2.png
--rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/7hlg1.png
--rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/Preprocessing with scanpy.rst
--rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/Tutorials/index.rst
--rw-rw-rw-   0        0        0      951 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/conf.py
--rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/document/source/index.rst
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.138971 scPANTHEON-0.5.5/extension/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.582080 scPANTHEON-0.5.5/extension/Change_Color/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.590110 scPANTHEON-0.5.5/extension/Change_Color/__pycache__/
--rw-rw-rw-   0        0        0     3990 2024-04-02 11:01:10.000000 scPANTHEON-0.5.5/extension/Change_Color/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     2348 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Change_Color/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     1691 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Change_Color/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     2363 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Change_Color/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1741 2024-03-24 09:06:41.000000 scPANTHEON-0.5.5/extension/Change_Color/module.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.592107 scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.600937 scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0     7058 2024-04-02 11:01:17.000000 scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     3901 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     2896 2024-03-24 09:05:36.000000 scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     3911 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     3354 2024-03-24 09:06:53.000000 scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.601935 scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.609972 scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/__pycache__/
--rw-rw-rw-   0        0        0    11487 2024-04-02 11:01:13.000000 scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     6104 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     4423 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5975 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     5670 2024-03-24 09:06:59.000000 scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/module.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.611971 scPANTHEON-0.5.5/extension/Find_Marker_Gene/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.619004 scPANTHEON-0.5.5/extension/Find_Marker_Gene/__pycache__/
--rw-rw-rw-   0        0        0     9696 2024-04-02 11:01:11.000000 scPANTHEON-0.5.5/extension/Find_Marker_Gene/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     5101 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Find_Marker_Gene/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     3786 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5037 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     4839 2024-03-24 09:07:32.000000 scPANTHEON-0.5.5/extension/Find_Marker_Gene/module.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.621006 scPANTHEON-0.5.5/extension/Plot_Histogram/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.628331 scPANTHEON-0.5.5/extension/Plot_Histogram/__pycache__/
--rw-rw-rw-   0        0        0      172 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Plot_Histogram/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8022 2024-04-02 10:04:39.000000 scPANTHEON-0.5.5/extension/Plot_Histogram/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     4379 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Plot_Histogram/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     4412 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Plot_Histogram/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     5244 2024-04-02 10:04:06.000000 scPANTHEON-0.5.5/extension/Plot_Histogram/module.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.629328 scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.637284 scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0    16100 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     7921 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     5877 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     7827 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     8155 2024-03-24 09:07:39.000000 scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.639284 scPANTHEON-0.5.5/extension/R_UMAP/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.641731 scPANTHEON-0.5.5/extension/R_UMAP/__pycache__/
--rw-rw-rw-   0        0        0    18998 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/R_UMAP/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0    10979 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/R_UMAP/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0    12580 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/R_UMAP/module.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.644245 scPANTHEON-0.5.5/extension/TOMAS/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.651687 scPANTHEON-0.5.5/extension/TOMAS/__pycache__/
--rw-rw-rw-   0        0        0    20982 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/TOMAS/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0    10490 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/TOMAS/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     7544 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/TOMAS/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0    10206 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5/extension/TOMAS/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0    11454 2024-03-24 09:07:45.000000 scPANTHEON-0.5.5/extension/TOMAS/module.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.663280 scPANTHEON-0.5.5/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      238 2024-04-08 14:56:22.000000 scPANTHEON-0.5.5/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12232 2024-04-08 14:56:23.000000 scPANTHEON-0.5.5/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 14:56:22.000000 scPANTHEON-0.5.5/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-08 14:56:22.000000 scPANTHEON-0.5.5/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2024-04-08 14:56:22.000000 scPANTHEON-0.5.5/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-08 14:56:22.000000 scPANTHEON-0.5.5/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.668031 scPANTHEON-0.5.5/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5/scpantheon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.684202 scPANTHEON-0.5.5/scpantheon/__pycache__/
--rw-rw-rw-   0        0        0   106928 2024-02-18 02:45:28.000000 scPANTHEON-0.5.5/scpantheon/__pycache__/aaa.cpython-311.pyc
--rw-rw-rw-   0        0        0     1405 2023-03-11 01:52:14.000000 scPANTHEON-0.5.5/scpantheon/__pycache__/anndata.cpython-39.pyc
--rw-rw-rw-   0        0        0     2701 2023-07-06 11:39:42.000000 scPANTHEON-0.5.5/scpantheon/__pycache__/bokeh_qt.cpython-39.pyc
--rw-rw-rw-   0        0        0     4877 2023-09-07 14:04:21.000000 scPANTHEON-0.5.5/scpantheon/__pycache__/data_qt.cpython-39.pyc
--rw-rw-rw-   0        0        0     4144 2023-04-20 04:56:49.000000 scPANTHEON-0.5.5/scpantheon/__pycache__/qt.cpython-39.pyc
--rw-rw-rw-   0        0        0   105802 2024-04-08 14:46:50.000000 scPANTHEON-0.5.5/scpantheon/__pycache__/source.cpython-311.pyc
--rw-rw-rw-   0        0        0    35550 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/scpantheon/__pycache__/source.cpython-38.pyc
--rw-rw-rw-   0        0        0    50207 2023-08-04 11:20:46.000000 scPANTHEON-0.5.5/scpantheon/__pycache__/source.cpython-39.pyc
--rw-rw-rw-   0        0        0      643 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5/scpantheon/__pycache__/transform.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.688456 scPANTHEON-0.5.5/scpantheon/app/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5/scpantheon/app/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.697971 scPANTHEON-0.5.5/scpantheon/app/__pycache__/
--rw-rw-rw-   0        0        0      179 2024-02-24 08:42:01.000000 scPANTHEON-0.5.5/scpantheon/app/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      161 2023-07-14 08:17:56.000000 scPANTHEON-0.5.5/scpantheon/app/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5557 2024-03-24 08:26:36.000000 scPANTHEON-0.5.5/scpantheon/app/__pycache__/bokeh_qt.cpython-311.pyc
--rw-rw-rw-   0        0        0     2705 2023-07-10 06:20:31.000000 scPANTHEON-0.5.5/scpantheon/app/__pycache__/bokeh_qt.cpython-39.pyc
--rw-rw-rw-   0        0        0    49472 2023-07-12 11:46:18.000000 scPANTHEON-0.5.5/scpantheon/app/__pycache__/source.cpython-39.pyc
--rw-rw-rw-   0        0        0     2978 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5/scpantheon/app/bokeh_qt.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.707283 scPANTHEON-0.5.5/scpantheon/front_end/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5/scpantheon/front_end/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.721370 scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/
--rw-rw-rw-   0        0        0      185 2023-11-20 22:01:18.000000 scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      167 2023-07-14 08:17:56.000000 scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    20629 2024-04-08 14:46:54.000000 scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/data_qt.cpython-311.pyc
--rw-rw-rw-   0        0        0     4722 2023-07-13 13:25:20.000000 scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/data_qt.cpython-39.pyc
--rw-rw-rw-   0        0        0     7822 2024-03-24 05:59:04.000000 scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/extensions_qt.cpython-311.pyc
--rw-rw-rw-   0        0        0     7846 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/load_qt.cpython-311.pyc
--rw-rw-rw-   0        0        0     7576 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/save_qt.cpython-311.pyc
--rw-rw-rw-   0        0        0     3473 2023-07-10 13:34:08.000000 scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/save_qt.cpython-39.pyc
--rw-rw-rw-   0        0        0    13255 2024-04-08 14:46:15.000000 scPANTHEON-0.5.5/scpantheon/front_end/data_qt.py
--rw-rw-rw-   0        0        0     4227 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5/scpantheon/front_end/extensions_qt.py
--rw-rw-rw-   0        0        0     4567 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5/scpantheon/front_end/load_qt.py
--rw-rw-rw-   0        0        0     4899 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5/scpantheon/front_end/save_qt.py
--rw-rw-rw-   0        0        0     1276 2024-04-08 14:46:38.000000 scPANTHEON-0.5.5/scpantheon/main.py
--rw-rw-rw-   0        0        0    66684 2024-04-02 11:00:55.000000 scPANTHEON-0.5.5/scpantheon/source.py
--rw-rw-rw-   0        0        0       42 2024-04-08 14:56:24.726164 scPANTHEON-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1138 2024-04-08 14:56:05.000000 scPANTHEON-0.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:56:24.723371 scPANTHEON-0.5.5/tests/
--rw-rw-rw-   0        0        0      294 2024-04-02 14:13:56.000000 scPANTHEON-0.5.5/tests/test_data.py
--rw-rw-rw-   0        0        0   104067 2024-01-02 19:33:04.000000 scPANTHEON-0.5.5/zhijiang.png
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.913108 scPANTHEON-0.5.5.1/
+-rw-rw-rw-   0        0        0      132 2024-03-24 08:59:16.000000 scPANTHEON-0.5.5.1/.gitattributes
+-rw-rw-rw-   0        0        0       66 2024-04-02 11:16:17.000000 scPANTHEON-0.5.5.1/.gitignore
+-rw-rw-rw-   0        0        0   837120 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/10k-genomics.png
+-rw-rw-rw-   0        0        0      240 2024-04-08 14:57:43.911602 scPANTHEON-0.5.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-01-02 19:33:04.000000 scPANTHEON-0.5.5.1/README.md
+-rw-rw-rw-   0        0        0        0 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.335957 scPANTHEON-0.5.5.1/__pycache__/
+-rw-rw-rw-   0        0        0      143 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.1/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      689 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.1/__pycache__/main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3789 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.1/__pycache__/qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      363 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.1/__pycache__/run.cpython-39.pyc
+-rw-rw-rw-   0        0        0    35541 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.1/__pycache__/source.cpython-36.pyc
+-rw-rw-rw-   0        0        0    35243 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.1/__pycache__/source.cpython-38.pyc
+-rw-rw-rw-   0        0        0    35200 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.1/__pycache__/source.cpython-39.pyc
+-rw-rw-rw-   0        0        0    37871 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.1/__pycache__/sourceqt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      631 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.1/__pycache__/transform.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.339958 scPANTHEON-0.5.5.1/document/
+-rw-rw-rw-   0        0        0      658 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.356411 scPANTHEON-0.5.5.1/document/build/
+-rw-rw-rw-   0        0        0      234 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/.buildinfo
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.364920 scPANTHEON-0.5.5.1/document/build/.doctrees/
+-rw-rw-rw-   0        0        0     2390 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/.doctrees/Download.doctree
+-rw-rw-rw-   0        0        0     3738 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/.doctrees/Introduction.doctree
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.371924 scPANTHEON-0.5.5.1/document/build/.doctrees/Tutorials/
+-rw-rw-rw-   0        0        0     2470 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/.doctrees/Tutorials/Clustering with sacnpy.doctree
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.374958 scPANTHEON-0.5.5.1/document/build/.doctrees/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0    19370 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/.doctrees/Tutorials/Navigation/contents.doctree
+-rw-rw-rw-   0        0        0     2485 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/.doctrees/Tutorials/Preprocessing with scanpy.doctree
+-rw-rw-rw-   0        0        0     2844 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/.doctrees/Tutorials/index.doctree
+-rw-rw-rw-   0        0        0    19829 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/.doctrees/environment.pickle
+-rw-rw-rw-   0        0        0     4036 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/.doctrees/index.doctree
+-rw-rw-rw-   0        0        0     4380 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/Download.html
+-rw-rw-rw-   0        0        0     4782 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/Introduction.html
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.380957 scPANTHEON-0.5.5.1/document/build/Tutorials/
+-rw-rw-rw-   0        0        0     4758 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/Tutorials/Clustering with sacnpy.html
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.383463 scPANTHEON-0.5.5.1/document/build/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0    12677 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/Tutorials/Navigation/contents.html
+-rw-rw-rw-   0        0        0     5036 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/Tutorials/Preprocessing with scanpy.html
+-rw-rw-rw-   0        0        0     6225 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/Tutorials/index.html
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.407039 scPANTHEON-0.5.5.1/document/build/_images/
+-rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/_images/1overview0.png
+-rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/_images/2mouse1.png
+-rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/_images/3map.png
+-rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/_images/3map1.png
+-rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.1/document/build/_images/3map2.png
+-rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_images/3map3.png
+-rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_images/4plot1.png
+-rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_images/5group1.png
+-rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_images/6cluster1.png
+-rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_images/6cluster2.png
+-rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_images/7hlg1.png
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.414049 scPANTHEON-0.5.5.1/document/build/_sources/
+-rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_sources/Download.rst.txt
+-rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_sources/Introduction.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.422063 scPANTHEON-0.5.5.1/document/build/_sources/Tutorials/
+-rw-rw-rw-   0        0        0       46 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_sources/Tutorials/Clustering with sacnpy.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.424258 scPANTHEON-0.5.5.1/document/build/_sources/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_sources/Tutorials/Navigation/contents.rst.txt
+-rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_sources/Tutorials/Preprocessing with scanpy.rst.txt
+-rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_sources/Tutorials/index.rst.txt
+-rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.464389 scPANTHEON-0.5.5.1/document/build/_static/
+-rw-rw-rw-   0        0        0     4552 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-rw-   0        0        0    11885 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/alabaster.css
+-rw-rw-rw-   0        0        0    15519 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/basic.css
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.468906 scPANTHEON-0.5.5.1/document/build/_static/css/
+-rw-rw-rw-   0        0        0     3275 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/badge_only.css
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.512146 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/
+-rw-rw-rw-   0        0        0    87624 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-rw-   0        0        0    67312 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-rw-   0        0        0    86288 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-rw-   0        0        0    66444 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-rw-   0        0        0   165742 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0   323344 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-rw-   0        0        0   193308 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-rw-   0        0        0   309728 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-bold.woff
+-rw-rw-rw-   0        0        0   184912 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-bold.woff2
+-rw-rw-rw-   0        0        0   328412 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-rw-   0        0        0   195704 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-rw-   0        0        0   309192 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-normal.woff
+-rw-rw-rw-   0        0        0   182708 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-normal.woff2
+-rw-rw-rw-   0        0        0   129677 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/css/theme.css
+-rw-rw-rw-   0        0        0       43 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/custom.css
+-rw-rw-rw-   0        0        0     8435 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/doctools.js
+-rw-rw-rw-   0        0        0      433 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/file.png
+-rw-rw-rw-   0        0        0   299461 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/jquery-3.6.0.js
+-rw-rw-rw-   0        0        0    89503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/jquery.js
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.543217 scPANTHEON-0.5.5.1/document/build/_static/js/
+-rw-rw-rw-   0        0        0      934 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/js/badge_only.js
+-rw-rw-rw-   0        0        0     4373 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/js/html5shiv-printshiv.min.js
+-rw-rw-rw-   0        0        0     2737 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/js/html5shiv.min.js
+-rw-rw-rw-   0        0        0     5023 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/js/theme.js
+-rw-rw-rw-   0        0        0     4957 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/plus.png
+-rw-rw-rw-   0        0        0     4892 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/pygments.css
+-rw-rw-rw-   0        0        0    17650 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/searchtools.js
+-rw-rw-rw-   0        0        0    70462 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    19535 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/_static/underscore.js
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.554994 scPANTHEON-0.5.5.1/document/build/doctrees/
+-rw-rw-rw-   0        0        0     2390 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/doctrees/Download.doctree
+-rw-rw-rw-   0        0        0     3738 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/doctrees/Introduction.doctree
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.560997 scPANTHEON-0.5.5.1/document/build/doctrees/Tutorials/
+-rw-rw-rw-   0        0        0     2470 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/doctrees/Tutorials/Clustering with sacnpy.doctree
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.561993 scPANTHEON-0.5.5.1/document/build/doctrees/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0    19370 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/doctrees/Tutorials/Navigation/contents.doctree
+-rw-rw-rw-   0        0        0     2485 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/doctrees/Tutorials/Preprocessing with scanpy.doctree
+-rw-rw-rw-   0        0        0     2844 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/doctrees/Tutorials/index.doctree
+-rw-rw-rw-   0        0        0    19803 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/doctrees/environment.pickle
+-rw-rw-rw-   0        0        0     4036 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/doctrees/index.doctree
+-rw-rw-rw-   0        0        0     3491 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/genindex.html
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.580135 scPANTHEON-0.5.5.1/document/build/html/
+-rw-rw-rw-   0        0        0      234 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/.buildinfo
+-rw-rw-rw-   0        0        0     4380 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/Download.html
+-rw-rw-rw-   0        0        0     4782 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/Introduction.html
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.587001 scPANTHEON-0.5.5.1/document/build/html/Tutorials/
+-rw-rw-rw-   0        0        0     4758 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/Tutorials/Clustering with sacnpy.html
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.588003 scPANTHEON-0.5.5.1/document/build/html/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0    12248 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/Tutorials/Navigation/contents.html
+-rw-rw-rw-   0        0        0     5036 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/Tutorials/Preprocessing with scanpy.html
+-rw-rw-rw-   0        0        0     6225 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/Tutorials/index.html
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.610262 scPANTHEON-0.5.5.1/document/build/html/_images/
+-rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_images/1overview0.png
+-rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_images/2mouse1.png
+-rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_images/3map.png
+-rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_images/3map1.png
+-rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_images/3map2.png
+-rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_images/3map3.png
+-rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_images/4plot1.png
+-rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_images/5group1.png
+-rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_images/6cluster1.png
+-rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_images/6cluster2.png
+-rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_images/7hlg1.png
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.618286 scPANTHEON-0.5.5.1/document/build/html/_sources/
+-rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_sources/Download.rst.txt
+-rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_sources/Introduction.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.624353 scPANTHEON-0.5.5.1/document/build/html/_sources/Tutorials/
+-rw-rw-rw-   0        0        0       46 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_sources/Tutorials/Clustering with sacnpy.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.626364 scPANTHEON-0.5.5.1/document/build/html/_sources/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_sources/Tutorials/Navigation/contents.rst.txt
+-rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_sources/Tutorials/Preprocessing with scanpy.rst.txt
+-rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_sources/Tutorials/index.rst.txt
+-rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.670734 scPANTHEON-0.5.5.1/document/build/html/_static/
+-rw-rw-rw-   0        0        0     4552 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-rw-   0        0        0    15519 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/basic.css
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.675317 scPANTHEON-0.5.5.1/document/build/html/_static/css/
+-rw-rw-rw-   0        0        0     3275 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/badge_only.css
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.714842 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/
+-rw-rw-rw-   0        0        0    87624 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-rw-   0        0        0    67312 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-rw-   0        0        0    86288 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-rw-   0        0        0    66444 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-rw-   0        0        0   165742 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0   323344 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-rw-   0        0        0   193308 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-rw-   0        0        0   309728 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-bold.woff
+-rw-rw-rw-   0        0        0   184912 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-bold.woff2
+-rw-rw-rw-   0        0        0   328412 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-rw-   0        0        0   195704 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-rw-   0        0        0   309192 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-normal.woff
+-rw-rw-rw-   0        0        0   182708 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-normal.woff2
+-rw-rw-rw-   0        0        0   129677 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/css/theme.css
+-rw-rw-rw-   0        0        0     8435 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      433 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/file.png
+-rw-rw-rw-   0        0        0   299461 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/jquery-3.6.0.js
+-rw-rw-rw-   0        0        0    89503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/jquery.js
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.722360 scPANTHEON-0.5.5.1/document/build/html/_static/js/
+-rw-rw-rw-   0        0        0      934 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/js/badge_only.js
+-rw-rw-rw-   0        0        0     4373 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-rw-rw-   0        0        0     2737 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/js/html5shiv.min.js
+-rw-rw-rw-   0        0        0     5023 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/js/theme.js
+-rw-rw-rw-   0        0        0     4957 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4892 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    17650 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0    70462 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    19535 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/_static/underscore.js
+-rw-rw-rw-   0        0        0     3491 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/genindex.html
+-rw-rw-rw-   0        0        0     6035 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/index.html
+-rw-rw-rw-   0        0        0      382 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/objects.inv
+-rw-rw-rw-   0        0        0     3905 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/search.html
+-rw-rw-rw-   0        0        0     3080 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/html/searchindex.js
+-rw-rw-rw-   0        0        0     6035 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/index.html
+-rw-rw-rw-   0        0        0      382 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/objects.inv
+-rw-rw-rw-   0        0        0     3905 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/search.html
+-rw-rw-rw-   0        0        0     3339 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/build/searchindex.js
+-rwxrwxrwx   0        0        0      804 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/make.bat
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.730009 scPANTHEON-0.5.5.1/document/source/
+-rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Download.rst
+-rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Introduction.rst
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.736958 scPANTHEON-0.5.5.1/document/source/Tutorials/
+-rw-rw-rw-   0        0        0       46 2024-03-23 11:22:01.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Clustering with sacnpy.rst
+-rw-rw-rw-   0        0        0       46 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Clustering with scanpy.rst
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.738957 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/contents.rst
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.760507 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/
+-rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/1overview0.png
+-rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/2mouse1.png
+-rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/3map.png
+-rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/3map1.png
+-rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/3map2.png
+-rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/3map3.png
+-rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/4plot1.png
+-rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/5group1.png
+-rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/6cluster1.png
+-rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/6cluster2.png
+-rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/7hlg1.png
+-rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/Preprocessing with scanpy.rst
+-rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/Tutorials/index.rst
+-rw-rw-rw-   0        0        0      951 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/conf.py
+-rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/document/source/index.rst
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.291799 scPANTHEON-0.5.5.1/extension/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.763010 scPANTHEON-0.5.5.1/extension/Change_Color/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.770001 scPANTHEON-0.5.5.1/extension/Change_Color/__pycache__/
+-rw-rw-rw-   0        0        0     3990 2024-04-02 11:01:10.000000 scPANTHEON-0.5.5.1/extension/Change_Color/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2348 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Change_Color/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1691 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Change_Color/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2363 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Change_Color/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1741 2024-03-24 09:06:41.000000 scPANTHEON-0.5.5.1/extension/Change_Color/module.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.772003 scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.779025 scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/__pycache__/
+-rw-rw-rw-   0        0        0     7058 2024-04-02 11:01:17.000000 scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3901 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2896 2024-03-24 09:05:36.000000 scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3911 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3354 2024-03-24 09:06:53.000000 scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/module.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.780026 scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.788184 scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/__pycache__/
+-rw-rw-rw-   0        0        0    11487 2024-04-02 11:01:13.000000 scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6104 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4423 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5975 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5670 2024-03-24 09:06:59.000000 scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/module.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.790183 scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.798118 scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/__pycache__/
+-rw-rw-rw-   0        0        0     9696 2024-04-02 11:01:11.000000 scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5101 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3786 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5037 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4839 2024-03-24 09:07:32.000000 scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/module.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.800117 scPANTHEON-0.5.5.1/extension/Plot_Histogram/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.809184 scPANTHEON-0.5.5.1/extension/Plot_Histogram/__pycache__/
+-rw-rw-rw-   0        0        0      172 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Plot_Histogram/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8022 2024-04-02 10:04:39.000000 scPANTHEON-0.5.5.1/extension/Plot_Histogram/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4379 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Plot_Histogram/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4412 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Plot_Histogram/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5244 2024-04-02 10:04:06.000000 scPANTHEON-0.5.5.1/extension/Plot_Histogram/module.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.810184 scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.819354 scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/__pycache__/
+-rw-rw-rw-   0        0        0    16100 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7921 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     5877 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     7827 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8155 2024-03-24 09:07:39.000000 scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/module.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.820354 scPANTHEON-0.5.5.1/extension/R_UMAP/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.824241 scPANTHEON-0.5.5.1/extension/R_UMAP/__pycache__/
+-rw-rw-rw-   0        0        0    18998 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/R_UMAP/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10979 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/R_UMAP/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0    12580 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/R_UMAP/module.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.826244 scPANTHEON-0.5.5.1/extension/TOMAS/
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.834313 scPANTHEON-0.5.5.1/extension/TOMAS/__pycache__/
+-rw-rw-rw-   0        0        0    20982 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/TOMAS/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10490 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/TOMAS/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7544 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/TOMAS/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0    10206 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.1/extension/TOMAS/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11454 2024-03-24 09:07:45.000000 scPANTHEON-0.5.5.1/extension/TOMAS/module.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.846357 scPANTHEON-0.5.5.1/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      240 2024-04-08 14:57:41.000000 scPANTHEON-0.5.5.1/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12232 2024-04-08 14:57:43.000000 scPANTHEON-0.5.5.1/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 14:57:41.000000 scPANTHEON-0.5.5.1/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-08 14:57:41.000000 scPANTHEON-0.5.5.1/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-08 14:57:41.000000 scPANTHEON-0.5.5.1/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-08 14:57:41.000000 scPANTHEON-0.5.5.1/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.852355 scPANTHEON-0.5.5.1/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5.1/scpantheon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.870106 scPANTHEON-0.5.5.1/scpantheon/__pycache__/
+-rw-rw-rw-   0        0        0   106928 2024-02-18 02:45:28.000000 scPANTHEON-0.5.5.1/scpantheon/__pycache__/aaa.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1405 2023-03-11 01:52:14.000000 scPANTHEON-0.5.5.1/scpantheon/__pycache__/anndata.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2701 2023-07-06 11:39:42.000000 scPANTHEON-0.5.5.1/scpantheon/__pycache__/bokeh_qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4877 2023-09-07 14:04:21.000000 scPANTHEON-0.5.5.1/scpantheon/__pycache__/data_qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4144 2023-04-20 04:56:49.000000 scPANTHEON-0.5.5.1/scpantheon/__pycache__/qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0   105802 2024-04-08 14:46:50.000000 scPANTHEON-0.5.5.1/scpantheon/__pycache__/source.cpython-311.pyc
+-rw-rw-rw-   0        0        0    35550 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/scpantheon/__pycache__/source.cpython-38.pyc
+-rw-rw-rw-   0        0        0    50207 2023-08-04 11:20:46.000000 scPANTHEON-0.5.5.1/scpantheon/__pycache__/source.cpython-39.pyc
+-rw-rw-rw-   0        0        0      643 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.1/scpantheon/__pycache__/transform.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.873970 scPANTHEON-0.5.5.1/scpantheon/app/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5.1/scpantheon/app/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.883488 scPANTHEON-0.5.5.1/scpantheon/app/__pycache__/
+-rw-rw-rw-   0        0        0      179 2024-02-24 08:42:01.000000 scPANTHEON-0.5.5.1/scpantheon/app/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      161 2023-07-14 08:17:56.000000 scPANTHEON-0.5.5.1/scpantheon/app/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5557 2024-03-24 08:26:36.000000 scPANTHEON-0.5.5.1/scpantheon/app/__pycache__/bokeh_qt.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2705 2023-07-10 06:20:31.000000 scPANTHEON-0.5.5.1/scpantheon/app/__pycache__/bokeh_qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0    49472 2023-07-12 11:46:18.000000 scPANTHEON-0.5.5.1/scpantheon/app/__pycache__/source.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2978 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.1/scpantheon/app/bokeh_qt.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.893013 scPANTHEON-0.5.5.1/scpantheon/front_end/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.908603 scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/
+-rw-rw-rw-   0        0        0      185 2023-11-20 22:01:18.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      167 2023-07-14 08:17:56.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    20629 2024-04-08 14:46:54.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/data_qt.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4722 2023-07-13 13:25:20.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/data_qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7822 2024-03-24 05:59:04.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/extensions_qt.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7846 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/load_qt.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7576 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/save_qt.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3473 2023-07-10 13:34:08.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/save_qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0    13255 2024-04-08 14:46:15.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/data_qt.py
+-rw-rw-rw-   0        0        0     4227 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/extensions_qt.py
+-rw-rw-rw-   0        0        0     4567 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/load_qt.py
+-rw-rw-rw-   0        0        0     4899 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.1/scpantheon/front_end/save_qt.py
+-rw-rw-rw-   0        0        0     1314 2024-04-08 14:57:19.000000 scPANTHEON-0.5.5.1/scpantheon/main.py
+-rw-rw-rw-   0        0        0    66684 2024-04-02 11:00:55.000000 scPANTHEON-0.5.5.1/scpantheon/source.py
+-rw-rw-rw-   0        0        0       42 2024-04-08 14:57:43.913108 scPANTHEON-0.5.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1140 2024-04-08 14:57:29.000000 scPANTHEON-0.5.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:57:43.910603 scPANTHEON-0.5.5.1/tests/
+-rw-rw-rw-   0        0        0      294 2024-04-02 14:13:56.000000 scPANTHEON-0.5.5.1/tests/test_data.py
+-rw-rw-rw-   0        0        0   104067 2024-01-02 19:33:04.000000 scPANTHEON-0.5.5.1/zhijiang.png
```

### Comparing `scPANTHEON-0.5.5/10k-genomics.png` & `scPANTHEON-0.5.5.1/10k-genomics.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/__pycache__/main.cpython-39.pyc` & `scPANTHEON-0.5.5.1/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/__pycache__/qt.cpython-39.pyc` & `scPANTHEON-0.5.5.1/__pycache__/qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/__pycache__/source.cpython-36.pyc` & `scPANTHEON-0.5.5.1/__pycache__/source.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/__pycache__/source.cpython-38.pyc` & `scPANTHEON-0.5.5.1/__pycache__/source.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/__pycache__/source.cpython-39.pyc` & `scPANTHEON-0.5.5.1/__pycache__/source.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/__pycache__/sourceqt.cpython-39.pyc` & `scPANTHEON-0.5.5.1/__pycache__/sourceqt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/__pycache__/transform.cpython-39.pyc` & `scPANTHEON-0.5.5.1/__pycache__/transform.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/Makefile` & `scPANTHEON-0.5.5.1/document/Makefile`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/.doctrees/Download.doctree` & `scPANTHEON-0.5.5.1/document/build/.doctrees/Download.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/.doctrees/Introduction.doctree` & `scPANTHEON-0.5.5.1/document/build/.doctrees/Introduction.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/.doctrees/Tutorials/Clustering with sacnpy.doctree` & `scPANTHEON-0.5.5.1/document/build/.doctrees/Tutorials/Clustering with sacnpy.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/.doctrees/Tutorials/Navigation/contents.doctree` & `scPANTHEON-0.5.5.1/document/build/.doctrees/Tutorials/Navigation/contents.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/.doctrees/Tutorials/Preprocessing with scanpy.doctree` & `scPANTHEON-0.5.5.1/document/build/.doctrees/Tutorials/Preprocessing with scanpy.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/.doctrees/Tutorials/index.doctree` & `scPANTHEON-0.5.5.1/document/build/.doctrees/Tutorials/index.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/.doctrees/environment.pickle` & `scPANTHEON-0.5.5.1/document/build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/.doctrees/index.doctree` & `scPANTHEON-0.5.5.1/document/build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/Download.html` & `scPANTHEON-0.5.5.1/document/build/Download.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/Introduction.html` & `scPANTHEON-0.5.5.1/document/build/Introduction.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/Tutorials/Clustering with sacnpy.html` & `scPANTHEON-0.5.5.1/document/build/Tutorials/Clustering with sacnpy.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/Tutorials/Navigation/contents.html` & `scPANTHEON-0.5.5.1/document/build/Tutorials/Navigation/contents.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/Tutorials/Preprocessing with scanpy.html` & `scPANTHEON-0.5.5.1/document/build/Tutorials/Preprocessing with scanpy.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/Tutorials/index.html` & `scPANTHEON-0.5.5.1/document/build/Tutorials/index.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_images/1overview0.png` & `scPANTHEON-0.5.5.1/document/build/_images/1overview0.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_images/2mouse1.png` & `scPANTHEON-0.5.5.1/document/build/_images/2mouse1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_images/3map.png` & `scPANTHEON-0.5.5.1/document/build/_images/3map.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_images/3map1.png` & `scPANTHEON-0.5.5.1/document/build/_images/3map1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_images/3map2.png` & `scPANTHEON-0.5.5.1/document/build/_images/3map2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_images/3map3.png` & `scPANTHEON-0.5.5.1/document/build/_images/3map3.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_images/4plot1.png` & `scPANTHEON-0.5.5.1/document/build/_images/4plot1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_images/5group1.png` & `scPANTHEON-0.5.5.1/document/build/_images/5group1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_images/6cluster1.png` & `scPANTHEON-0.5.5.1/document/build/_images/6cluster1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_images/6cluster2.png` & `scPANTHEON-0.5.5.1/document/build/_images/6cluster2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_images/7hlg1.png` & `scPANTHEON-0.5.5.1/document/build/_images/7hlg1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_sources/Tutorials/Navigation/contents.rst.txt` & `scPANTHEON-0.5.5.1/document/build/_sources/Tutorials/Navigation/contents.rst.txt`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/_sphinx_javascript_frameworks_compat.js` & `scPANTHEON-0.5.5.1/document/build/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/alabaster.css` & `scPANTHEON-0.5.5.1/document/build/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/basic.css` & `scPANTHEON-0.5.5.1/document/build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/badge_only.css` & `scPANTHEON-0.5.5.1/document/build/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/Roboto-Slab-Bold.woff` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/Roboto-Slab-Bold.woff2` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/Roboto-Slab-Regular.woff` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/Roboto-Slab-Regular.woff2` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/fontawesome-webfont.eot` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/fontawesome-webfont.svg` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/fontawesome-webfont.ttf` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/fontawesome-webfont.woff` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/fontawesome-webfont.woff2` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-bold-italic.woff` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-bold-italic.woff2` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-bold.woff` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-bold.woff2` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-normal-italic.woff` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-normal-italic.woff2` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-normal.woff` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/fonts/lato-normal.woff2` & `scPANTHEON-0.5.5.1/document/build/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/css/theme.css` & `scPANTHEON-0.5.5.1/document/build/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/doctools.js` & `scPANTHEON-0.5.5.1/document/build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/jquery-3.6.0.js` & `scPANTHEON-0.5.5.1/document/build/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/jquery.js` & `scPANTHEON-0.5.5.1/document/build/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/js/badge_only.js` & `scPANTHEON-0.5.5.1/document/build/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/js/html5shiv-printshiv.min.js` & `scPANTHEON-0.5.5.1/document/build/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/js/html5shiv.min.js` & `scPANTHEON-0.5.5.1/document/build/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/js/theme.js` & `scPANTHEON-0.5.5.1/document/build/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/language_data.js` & `scPANTHEON-0.5.5.1/document/build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/pygments.css` & `scPANTHEON-0.5.5.1/document/build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/searchtools.js` & `scPANTHEON-0.5.5.1/document/build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/underscore-1.13.1.js` & `scPANTHEON-0.5.5.1/document/build/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/_static/underscore.js` & `scPANTHEON-0.5.5.1/document/build/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/doctrees/Download.doctree` & `scPANTHEON-0.5.5.1/document/build/doctrees/Download.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/doctrees/Introduction.doctree` & `scPANTHEON-0.5.5.1/document/build/doctrees/Introduction.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/doctrees/Tutorials/Clustering with sacnpy.doctree` & `scPANTHEON-0.5.5.1/document/build/doctrees/Tutorials/Clustering with sacnpy.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/doctrees/Tutorials/Navigation/contents.doctree` & `scPANTHEON-0.5.5.1/document/build/doctrees/Tutorials/Navigation/contents.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/doctrees/Tutorials/Preprocessing with scanpy.doctree` & `scPANTHEON-0.5.5.1/document/build/doctrees/Tutorials/Preprocessing with scanpy.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/doctrees/Tutorials/index.doctree` & `scPANTHEON-0.5.5.1/document/build/doctrees/Tutorials/index.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/doctrees/environment.pickle` & `scPANTHEON-0.5.5.1/document/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/doctrees/index.doctree` & `scPANTHEON-0.5.5.1/document/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/genindex.html` & `scPANTHEON-0.5.5.1/document/build/genindex.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/Download.html` & `scPANTHEON-0.5.5.1/document/build/html/Download.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/Introduction.html` & `scPANTHEON-0.5.5.1/document/build/html/Introduction.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/Tutorials/Clustering with sacnpy.html` & `scPANTHEON-0.5.5.1/document/build/html/Tutorials/Clustering with sacnpy.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/Tutorials/Navigation/contents.html` & `scPANTHEON-0.5.5.1/document/build/html/Tutorials/Navigation/contents.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/Tutorials/Preprocessing with scanpy.html` & `scPANTHEON-0.5.5.1/document/build/html/Tutorials/Preprocessing with scanpy.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/Tutorials/index.html` & `scPANTHEON-0.5.5.1/document/build/html/Tutorials/index.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_images/1overview0.png` & `scPANTHEON-0.5.5.1/document/build/html/_images/1overview0.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_images/2mouse1.png` & `scPANTHEON-0.5.5.1/document/build/html/_images/2mouse1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_images/3map.png` & `scPANTHEON-0.5.5.1/document/build/html/_images/3map.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_images/3map1.png` & `scPANTHEON-0.5.5.1/document/build/html/_images/3map1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_images/3map2.png` & `scPANTHEON-0.5.5.1/document/build/html/_images/3map2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_images/3map3.png` & `scPANTHEON-0.5.5.1/document/build/html/_images/3map3.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_images/4plot1.png` & `scPANTHEON-0.5.5.1/document/build/html/_images/4plot1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_images/5group1.png` & `scPANTHEON-0.5.5.1/document/build/html/_images/5group1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_images/6cluster1.png` & `scPANTHEON-0.5.5.1/document/build/html/_images/6cluster1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_images/6cluster2.png` & `scPANTHEON-0.5.5.1/document/build/html/_images/6cluster2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_images/7hlg1.png` & `scPANTHEON-0.5.5.1/document/build/html/_images/7hlg1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_sources/Tutorials/Navigation/contents.rst.txt` & `scPANTHEON-0.5.5.1/document/build/html/_sources/Tutorials/Navigation/contents.rst.txt`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/basic.css` & `scPANTHEON-0.5.5.1/document/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/badge_only.css` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/fontawesome-webfont.eot` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/fontawesome-webfont.svg` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/fontawesome-webfont.woff` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-bold-italic.woff` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-bold-italic.woff2` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-bold.woff` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-bold.woff2` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-normal-italic.woff` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-normal-italic.woff2` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-normal.woff` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/fonts/lato-normal.woff2` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/css/theme.css` & `scPANTHEON-0.5.5.1/document/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/doctools.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/jquery-3.6.0.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/jquery.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/js/badge_only.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/js/html5shiv-printshiv.min.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/js/html5shiv.min.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/js/theme.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/language_data.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/pygments.css` & `scPANTHEON-0.5.5.1/document/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/searchtools.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/underscore-1.13.1.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/_static/underscore.js` & `scPANTHEON-0.5.5.1/document/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/genindex.html` & `scPANTHEON-0.5.5.1/document/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/index.html` & `scPANTHEON-0.5.5.1/document/build/html/index.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/search.html` & `scPANTHEON-0.5.5.1/document/build/html/search.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/html/searchindex.js` & `scPANTHEON-0.5.5.1/document/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/index.html` & `scPANTHEON-0.5.5.1/document/build/index.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/search.html` & `scPANTHEON-0.5.5.1/document/build/search.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/build/searchindex.js` & `scPANTHEON-0.5.5.1/document/build/searchindex.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/make.bat` & `scPANTHEON-0.5.5.1/document/make.bat`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/contents.rst` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/contents.rst`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/1overview0.png` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/1overview0.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/2mouse1.png` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/2mouse1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/3map.png` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/3map.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/3map1.png` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/3map1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/3map2.png` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/3map2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/3map3.png` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/3map3.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/4plot1.png` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/4plot1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/5group1.png` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/5group1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/6cluster1.png` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/6cluster1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/6cluster2.png` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/6cluster2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/Tutorials/Navigation/image/7hlg1.png` & `scPANTHEON-0.5.5.1/document/source/Tutorials/Navigation/image/7hlg1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/document/source/conf.py` & `scPANTHEON-0.5.5.1/document/source/conf.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Change_Color/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.1/extension/Change_Color/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Change_Color/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.1/extension/Change_Color/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Change_Color/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.1/extension/Change_Color/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Change_Color/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.1/extension/Change_Color/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Change_Color/module.py` & `scPANTHEON-0.5.5.1/extension/Change_Color/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Clustering_with_Scanpy/module.py` & `scPANTHEON-0.5.5.1/extension/Clustering_with_Scanpy/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Differential_Expression_Analysis/module.py` & `scPANTHEON-0.5.5.1/extension/Differential_Expression_Analysis/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Find_Marker_Gene/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Find_Marker_Gene/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Find_Marker_Gene/module.py` & `scPANTHEON-0.5.5.1/extension/Find_Marker_Gene/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Plot_Histogram/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.1/extension/Plot_Histogram/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Plot_Histogram/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.1/extension/Plot_Histogram/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Plot_Histogram/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.1/extension/Plot_Histogram/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Plot_Histogram/module.py` & `scPANTHEON-0.5.5.1/extension/Plot_Histogram/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/Preprocessing_with_Scanpy/module.py` & `scPANTHEON-0.5.5.1/extension/Preprocessing_with_Scanpy/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/R_UMAP/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.1/extension/R_UMAP/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/R_UMAP/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.1/extension/R_UMAP/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/R_UMAP/module.py` & `scPANTHEON-0.5.5.1/extension/R_UMAP/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/TOMAS/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.1/extension/TOMAS/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/TOMAS/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.1/extension/TOMAS/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/TOMAS/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.1/extension/TOMAS/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/TOMAS/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.1/extension/TOMAS/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/extension/TOMAS/module.py` & `scPANTHEON-0.5.5.1/extension/TOMAS/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scPANTHEON.egg-info/SOURCES.txt` & `scPANTHEON-0.5.5.1/scPANTHEON.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/__pycache__/aaa.cpython-311.pyc` & `scPANTHEON-0.5.5.1/scpantheon/__pycache__/aaa.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/__pycache__/anndata.cpython-39.pyc` & `scPANTHEON-0.5.5.1/scpantheon/__pycache__/anndata.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/__pycache__/bokeh_qt.cpython-39.pyc` & `scPANTHEON-0.5.5.1/scpantheon/__pycache__/bokeh_qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/__pycache__/data_qt.cpython-39.pyc` & `scPANTHEON-0.5.5.1/scpantheon/__pycache__/data_qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/__pycache__/qt.cpython-39.pyc` & `scPANTHEON-0.5.5.1/scpantheon/__pycache__/qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/__pycache__/source.cpython-311.pyc` & `scPANTHEON-0.5.5.1/scpantheon/__pycache__/source.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/__pycache__/source.cpython-38.pyc` & `scPANTHEON-0.5.5.1/scpantheon/__pycache__/source.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/__pycache__/source.cpython-39.pyc` & `scPANTHEON-0.5.5.1/scpantheon/__pycache__/source.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/__pycache__/transform.cpython-38.pyc` & `scPANTHEON-0.5.5.1/scpantheon/__pycache__/transform.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/app/__pycache__/bokeh_qt.cpython-311.pyc` & `scPANTHEON-0.5.5.1/scpantheon/app/__pycache__/bokeh_qt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/app/__pycache__/bokeh_qt.cpython-39.pyc` & `scPANTHEON-0.5.5.1/scpantheon/app/__pycache__/bokeh_qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/app/__pycache__/source.cpython-39.pyc` & `scPANTHEON-0.5.5.1/scpantheon/app/__pycache__/source.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/app/bokeh_qt.py` & `scPANTHEON-0.5.5.1/scpantheon/app/bokeh_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/data_qt.cpython-311.pyc` & `scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/data_qt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/data_qt.cpython-39.pyc` & `scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/data_qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/extensions_qt.cpython-311.pyc` & `scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/extensions_qt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/load_qt.cpython-311.pyc` & `scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/load_qt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/save_qt.cpython-311.pyc` & `scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/save_qt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/front_end/__pycache__/save_qt.cpython-39.pyc` & `scPANTHEON-0.5.5.1/scpantheon/front_end/__pycache__/save_qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/front_end/data_qt.py` & `scPANTHEON-0.5.5.1/scpantheon/front_end/data_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/front_end/extensions_qt.py` & `scPANTHEON-0.5.5.1/scpantheon/front_end/extensions_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/front_end/load_qt.py` & `scPANTHEON-0.5.5.1/scpantheon/front_end/load_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/front_end/save_qt.py` & `scPANTHEON-0.5.5.1/scpantheon/front_end/save_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/scpantheon/main.py` & `scPANTHEON-0.5.5.1/scpantheon/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from multiprocessing import freeze_support
 
 import multiprocessing
 import pkg_resources, subprocess
 try:
-    import source
-    from app import bokeh_qt
-    from front_end import data_qt
+    from scpantheon import source
+    from scpantheon.app import bokeh_qt
+    from scpantheon.front_end import data_qt
     version = pkg_resources.get_distribution("scpantheon").version
 except:
     print("pip install scpantheon")
     subprocess.check_call(['pip', 'install', "scpantheon"])
     from scpantheon import source
     from scpantheon.app import bokeh_qt
     from scpantheon.front_end import data_qt
```

### Comparing `scPANTHEON-0.5.5/scpantheon/source.py` & `scPANTHEON-0.5.5.1/scpantheon/source.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5/setup.py` & `scPANTHEON-0.5.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.5.5',#版本
+    version='0.5.5.1',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon', 'scpantheon.app', 'scpantheon.front_end'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
                        'appdirs','requests','leidenalg', 'setuptools_scm'], # 依赖包,如果没有,可以不要 rpy2
```

### Comparing `scPANTHEON-0.5.5/zhijiang.png` & `scPANTHEON-0.5.5.1/zhijiang.png`

 * *Files identical despite different names*

