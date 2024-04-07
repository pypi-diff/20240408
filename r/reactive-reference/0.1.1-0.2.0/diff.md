# Comparing `tmp/reactive_reference-0.1.1.tar.gz` & `tmp/reactive_reference-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactive_reference-0.1.1.tar", max compression
+gzip compressed data, was "reactive_reference-0.2.0.tar", max compression
```

## Comparing `reactive_reference-0.1.1.tar` & `reactive_reference-0.2.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0      557 2024-03-30 18:44:25.623295 reactive_reference-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-17 18:52:53.157605 reactive_reference-0.1.1/reactive_reference/__init__.py
--rw-r--r--   0        0        0   372653 2024-03-09 15:37:55.228821 reactive_reference-0.1.1/reactive_reference/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0   162472 2024-03-09 15:37:55.220817 reactive_reference-0.1.1/reactive_reference/docs/_build/doctrees/event.doctree
--rw-r--r--   0        0        0     5089 2024-03-09 15:28:36.521180 reactive_reference-0.1.1/reactive_reference/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0     3156 2024-03-09 15:34:20.772306 reactive_reference-0.1.1/reactive_reference/docs/_build/doctrees/modules.doctree
--rw-r--r--   0        0        0    62041 2024-03-09 15:28:36.614221 reactive_reference-0.1.1/reactive_reference/docs/_build/doctrees/reference.doctree
--rw-r--r--   0        0        0      234 2024-03-09 15:37:55.454817 reactive_reference-0.1.1/reactive_reference/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0        0 2024-03-09 15:37:55.220817 reactive_reference-0.1.1/reactive_reference/docs/_build/html/.nojekyll
--rw-r--r--   0        0        0      624 2024-03-09 15:22:39.357756 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_sources/event.rst.txt
--rw-r--r--   0        0        0      501 2024-03-09 15:17:08.018220 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0      132 2024-03-09 15:34:19.544980 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      497 2024-03-09 15:25:02.696282 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_sources/reference.rst.txt
--rw-r--r--   0        0        0    11932 2024-03-09 15:37:55.265818 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/alabaster.css
--rw-r--r--   0        0        0    16018 2024-03-09 15:37:55.238817 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2024-01-02 12:56:21.197138 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2024-01-02 12:56:23.613999 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      335 2024-03-09 15:37:55.242817 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2024-01-02 12:56:23.614998 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0     4957 2024-03-09 15:37:55.244819 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2024-01-02 12:56:23.617000 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2024-01-02 12:56:23.617000 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     5470 2024-03-09 15:37:55.233818 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18732 2024-01-02 12:56:23.617998 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2024-01-02 12:56:23.617998 reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0    60076 2024-03-09 15:37:55.389822 reactive_reference-0.1.1/reactive_reference/docs/_build/html/event.html
--rw-r--r--   0        0        0    19457 2024-03-09 15:37:55.434817 reactive_reference-0.1.1/reactive_reference/docs/_build/html/genindex.html
--rw-r--r--   0        0        0     4373 2024-03-09 15:37:55.399818 reactive_reference-0.1.1/reactive_reference/docs/_build/html/index.html
--rw-r--r--   0        0        0    23299 2024-03-09 15:37:55.419818 reactive_reference-0.1.1/reactive_reference/docs/_build/html/modules.html
--rw-r--r--   0        0        0      982 2024-03-09 15:37:55.457821 reactive_reference-0.1.1/reactive_reference/docs/_build/html/objects.inv
--rw-r--r--   0        0        0     4897 2024-03-09 15:37:55.445817 reactive_reference-0.1.1/reactive_reference/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0    23349 2024-03-09 15:28:36.966982 reactive_reference-0.1.1/reactive_reference/docs/_build/html/reference.html
--rw-r--r--   0        0        0     3071 2024-03-09 15:37:55.454817 reactive_reference-0.1.1/reactive_reference/docs/_build/html/search.html
--rw-r--r--   0        0        0    13424 2024-03-09 15:37:55.456820 reactive_reference-0.1.1/reactive_reference/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0     1091 2024-03-09 15:28:12.629313 reactive_reference-0.1.1/reactive_reference/docs/conf.py
--rw-r--r--   0        0        0      624 2024-03-09 15:22:39.357756 reactive_reference-0.1.1/reactive_reference/docs/event.rst
--rw-r--r--   0        0        0      501 2024-03-09 15:17:08.018220 reactive_reference-0.1.1/reactive_reference/docs/index.rst
--rwxr-xr-x   0        0        0      800 2024-03-09 15:16:24.732157 reactive_reference-0.1.1/reactive_reference/docs/make.bat
--rw-r--r--   0        0        0      634 2024-03-09 15:16:24.731158 reactive_reference-0.1.1/reactive_reference/docs/Makefile
--rw-r--r--   0        0        0      132 2024-03-09 15:34:19.544980 reactive_reference-0.1.1/reactive_reference/docs/modules.rst
--rw-r--r--   0        0        0      497 2024-03-09 15:25:02.696282 reactive_reference-0.1.1/reactive_reference/docs/reference.rst
--rw-r--r--   0        0        0        2 2024-01-01 23:28:01.587008 reactive_reference-0.1.1/reactive_reference/errors.py
--rw-r--r--   0        0        0      686 2024-01-01 23:28:01.588003 reactive_reference-0.1.1/reactive_reference/event/__init__.py
--rw-r--r--   0        0        0      249 2024-02-24 14:20:25.120304 reactive_reference-0.1.1/reactive_reference/event/Constants.py
--rw-r--r--   0        0        0      377 2024-01-01 23:28:01.588003 reactive_reference-0.1.1/reactive_reference/event/data/Domain.py
--rw-r--r--   0        0        0      493 2024-03-09 14:48:16.794680 reactive_reference-0.1.1/reactive_reference/event/data/Entity.py
--rw-r--r--   0        0        0      449 2024-01-01 23:28:01.589006 reactive_reference-0.1.1/reactive_reference/event/data/Event.py
--rw-r--r--   0        0        0      118 2024-03-09 15:28:12.648314 reactive_reference-0.1.1/reactive_reference/event/data/EventErrors.py
--rw-r--r--   0        0        0      316 2024-03-09 15:08:02.809472 reactive_reference-0.1.1/reactive_reference/event/data/EventType.py
--rw-r--r--   0        0        0      504 2024-03-09 15:04:48.109899 reactive_reference-0.1.1/reactive_reference/event/data/LifecycleEvent.py
--rw-r--r--   0        0        0      410 2024-01-01 23:28:01.589006 reactive_reference-0.1.1/reactive_reference/event/data/Payload.py
--rw-r--r--   0        0        0      148 2024-02-24 14:20:25.114304 reactive_reference-0.1.1/reactive_reference/event/data/ReplayStrategy.py
--rw-r--r--   0        0        0    11691 2024-03-30 18:44:25.619298 reactive_reference-0.1.1/reactive_reference/event/EventStream.py
--rw-r--r--   0        0        0     2495 2024-03-09 15:28:12.669313 reactive_reference-0.1.1/reactive_reference/event/EventSubscriber.py
--rw-r--r--   0        0        0     2938 2024-02-24 14:44:59.878140 reactive_reference-0.1.1/reactive_reference/event/interfaces/IEventStream.py
--rw-r--r--   0        0        0     2468 2024-03-09 15:28:12.655312 reactive_reference-0.1.1/reactive_reference/event/interfaces/IEventSubscriber.py
--rw-r--r--   0        0        0        0 2024-01-01 23:28:01.590004 reactive_reference-0.1.1/reactive_reference/jellyfin/__init__.py
--rw-r--r--   0        0        0      656 2024-01-01 23:28:01.590004 reactive_reference-0.1.1/reactive_reference/jellyfin/common.py
--rw-r--r--   0        0        0       64 2024-01-01 23:28:01.591005 reactive_reference-0.1.1/reactive_reference/jellyfin/data/Constants.py
--rw-r--r--   0        0        0      394 2024-01-01 23:28:01.591005 reactive_reference-0.1.1/reactive_reference/jellyfin/data/Link.py
--rw-r--r--   0        0        0      297 2024-01-01 23:28:01.591005 reactive_reference-0.1.1/reactive_reference/jellyfin/data/Server.py
--rw-r--r--   0        0        0      468 2024-01-04 15:30:20.212700 reactive_reference-0.1.1/reactive_reference/jellyfin/main.py
--rw-r--r--   0        0        0      143 2024-01-01 23:28:01.592007 reactive_reference-0.1.1/reactive_reference/reference/__init__.py
--rw-r--r--   0        0        0     1280 2024-01-01 23:28:01.592007 reactive_reference-0.1.1/reactive_reference/reference/IReference.py
--rw-r--r--   0        0        0     3173 2024-01-01 23:28:01.592007 reactive_reference-0.1.1/reactive_reference/reference/Reference.py
--rw-r--r--   0        0        0     1161 2024-03-30 18:48:36.926810 reactive_reference-0.1.1/reactive_reference/utils.py
--rw-r--r--   0        0        0        0 2023-12-17 18:52:53.157605 reactive_reference-0.1.1/README.md
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 reactive_reference-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      633 2024-04-07 22:43:39.126562 reactive_reference-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-17 18:52:53.157605 reactive_reference-0.2.0/reactive_reference/__init__.py
+-rw-r--r--   0        0        0   372653 2024-03-09 15:37:55.228821 reactive_reference-0.2.0/reactive_reference/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0   162472 2024-03-09 15:37:55.220817 reactive_reference-0.2.0/reactive_reference/docs/_build/doctrees/event.doctree
+-rw-r--r--   0        0        0     5089 2024-03-09 15:28:36.521180 reactive_reference-0.2.0/reactive_reference/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0     3156 2024-03-09 15:34:20.772306 reactive_reference-0.2.0/reactive_reference/docs/_build/doctrees/modules.doctree
+-rw-r--r--   0        0        0    62041 2024-03-09 15:28:36.614221 reactive_reference-0.2.0/reactive_reference/docs/_build/doctrees/reference.doctree
+-rw-r--r--   0        0        0      234 2024-03-09 15:37:55.454817 reactive_reference-0.2.0/reactive_reference/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0        0 2024-03-09 15:37:55.220817 reactive_reference-0.2.0/reactive_reference/docs/_build/html/.nojekyll
+-rw-r--r--   0        0        0      624 2024-03-09 15:22:39.357756 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_sources/event.rst.txt
+-rw-r--r--   0        0        0      501 2024-03-09 15:17:08.018220 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0      132 2024-03-09 15:34:19.544980 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      497 2024-03-09 15:25:02.696282 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_sources/reference.rst.txt
+-rw-r--r--   0        0        0    11932 2024-03-09 15:37:55.265818 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    16018 2024-03-09 15:37:55.238817 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2024-01-02 12:56:21.197138 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2024-01-02 12:56:23.613999 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      335 2024-03-09 15:37:55.242817 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2024-01-02 12:56:23.614998 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4957 2024-03-09 15:37:55.244819 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2024-01-02 12:56:23.617000 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2024-01-02 12:56:23.617000 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     5470 2024-03-09 15:37:55.233818 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18732 2024-01-02 12:56:23.617998 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2024-01-02 12:56:23.617998 reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    60076 2024-03-09 15:37:55.389822 reactive_reference-0.2.0/reactive_reference/docs/_build/html/event.html
+-rw-r--r--   0        0        0    19457 2024-03-09 15:37:55.434817 reactive_reference-0.2.0/reactive_reference/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0     4373 2024-03-09 15:37:55.399818 reactive_reference-0.2.0/reactive_reference/docs/_build/html/index.html
+-rw-r--r--   0        0        0    23299 2024-03-09 15:37:55.419818 reactive_reference-0.2.0/reactive_reference/docs/_build/html/modules.html
+-rw-r--r--   0        0        0      982 2024-03-09 15:37:55.457821 reactive_reference-0.2.0/reactive_reference/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0     4897 2024-03-09 15:37:55.445817 reactive_reference-0.2.0/reactive_reference/docs/_build/html/py-modindex.html
+-rw-r--r--   0        0        0    23349 2024-03-09 15:28:36.966982 reactive_reference-0.2.0/reactive_reference/docs/_build/html/reference.html
+-rw-r--r--   0        0        0     3071 2024-03-09 15:37:55.454817 reactive_reference-0.2.0/reactive_reference/docs/_build/html/search.html
+-rw-r--r--   0        0        0    13424 2024-03-09 15:37:55.456820 reactive_reference-0.2.0/reactive_reference/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0     1091 2024-03-09 15:28:12.629313 reactive_reference-0.2.0/reactive_reference/docs/conf.py
+-rw-r--r--   0        0        0      624 2024-03-09 15:22:39.357756 reactive_reference-0.2.0/reactive_reference/docs/event.rst
+-rw-r--r--   0        0        0      501 2024-03-09 15:17:08.018220 reactive_reference-0.2.0/reactive_reference/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2024-03-09 15:16:24.732157 reactive_reference-0.2.0/reactive_reference/docs/make.bat
+-rw-r--r--   0        0        0      634 2024-03-09 15:16:24.731158 reactive_reference-0.2.0/reactive_reference/docs/Makefile
+-rw-r--r--   0        0        0      132 2024-03-09 15:34:19.544980 reactive_reference-0.2.0/reactive_reference/docs/modules.rst
+-rw-r--r--   0        0        0      497 2024-03-09 15:25:02.696282 reactive_reference-0.2.0/reactive_reference/docs/reference.rst
+-rw-r--r--   0        0        0        2 2024-01-01 23:28:01.587008 reactive_reference-0.2.0/reactive_reference/errors.py
+-rw-r--r--   0        0        0      686 2024-01-01 23:28:01.588003 reactive_reference-0.2.0/reactive_reference/event/__init__.py
+-rw-r--r--   0        0        0      249 2024-02-24 14:20:25.120304 reactive_reference-0.2.0/reactive_reference/event/Constants.py
+-rw-r--r--   0        0        0      377 2024-01-01 23:28:01.588003 reactive_reference-0.2.0/reactive_reference/event/data/Domain.py
+-rw-r--r--   0        0        0      493 2024-03-09 14:48:16.794680 reactive_reference-0.2.0/reactive_reference/event/data/Entity.py
+-rw-r--r--   0        0        0      449 2024-01-01 23:28:01.589006 reactive_reference-0.2.0/reactive_reference/event/data/Event.py
+-rw-r--r--   0        0        0      118 2024-03-09 15:28:12.648314 reactive_reference-0.2.0/reactive_reference/event/data/EventErrors.py
+-rw-r--r--   0        0        0      316 2024-03-09 15:08:02.809472 reactive_reference-0.2.0/reactive_reference/event/data/EventType.py
+-rw-r--r--   0        0        0      504 2024-03-09 15:04:48.109899 reactive_reference-0.2.0/reactive_reference/event/data/LifecycleEvent.py
+-rw-r--r--   0        0        0      410 2024-01-01 23:28:01.589006 reactive_reference-0.2.0/reactive_reference/event/data/Payload.py
+-rw-r--r--   0        0        0      148 2024-02-24 14:20:25.114304 reactive_reference-0.2.0/reactive_reference/event/data/ReplayStrategy.py
+-rw-r--r--   0        0        0     1406 2024-04-07 21:58:07.391451 reactive_reference-0.2.0/reactive_reference/event/EventProducer.py
+-rw-r--r--   0        0        0    12496 2024-04-07 22:12:01.062419 reactive_reference-0.2.0/reactive_reference/event/EventStream.py
+-rw-r--r--   0        0        0     2359 2024-04-07 22:14:01.340575 reactive_reference-0.2.0/reactive_reference/event/EventSubscriber.py
+-rw-r--r--   0        0        0      993 2024-04-07 21:58:07.379451 reactive_reference-0.2.0/reactive_reference/event/interfaces/IEventProducer.py
+-rw-r--r--   0        0        0     3049 2024-04-07 21:58:07.387453 reactive_reference-0.2.0/reactive_reference/event/interfaces/IEventStream.py
+-rw-r--r--   0        0        0     2123 2024-04-07 22:14:01.344577 reactive_reference-0.2.0/reactive_reference/event/interfaces/IEventSubscriber.py
+-rw-r--r--   0        0        0        0 2024-01-01 23:28:01.590004 reactive_reference-0.2.0/reactive_reference/jellyfin/__init__.py
+-rw-r--r--   0        0        0      656 2024-01-01 23:28:01.590004 reactive_reference-0.2.0/reactive_reference/jellyfin/common.py
+-rw-r--r--   0        0        0       64 2024-01-01 23:28:01.591005 reactive_reference-0.2.0/reactive_reference/jellyfin/data/Constants.py
+-rw-r--r--   0        0        0      394 2024-01-01 23:28:01.591005 reactive_reference-0.2.0/reactive_reference/jellyfin/data/Link.py
+-rw-r--r--   0        0        0      297 2024-01-01 23:28:01.591005 reactive_reference-0.2.0/reactive_reference/jellyfin/data/Server.py
+-rw-r--r--   0        0        0      468 2024-01-04 15:30:20.212700 reactive_reference-0.2.0/reactive_reference/jellyfin/main.py
+-rw-r--r--   0        0        0      143 2024-01-01 23:28:01.592007 reactive_reference-0.2.0/reactive_reference/reference/__init__.py
+-rw-r--r--   0        0        0     1280 2024-01-01 23:28:01.592007 reactive_reference-0.2.0/reactive_reference/reference/IReference.py
+-rw-r--r--   0        0        0     3173 2024-01-01 23:28:01.592007 reactive_reference-0.2.0/reactive_reference/reference/Reference.py
+-rw-r--r--   0        0        0     1161 2024-03-30 18:48:36.926810 reactive_reference-0.2.0/reactive_reference/utils.py
+-rw-r--r--   0        0        0     1031 2024-04-07 22:42:16.455257 reactive_reference-0.2.0/README.md
+-rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 reactive_reference-0.2.0/PKG-INFO
```

### Comparing `reactive_reference-0.1.1/pyproject.toml` & `reactive_reference-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "reactive-reference"
-version = "0.1.1"
-description = ""
-authors = ["Carlos Silva <cmiguelrsilva@gmail.com>"]
+version = "0.2.0"
+description = "A collection of mini projects for a reactive programming approach"
+authors = ["Carlos Silva <carlos.miguel.silva@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pre-commit = "^3.6.0"
```

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/doctrees/environment.pickle` & `reactive_reference-0.2.0/reactive_reference/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/doctrees/event.doctree` & `reactive_reference-0.2.0/reactive_reference/docs/_build/doctrees/event.doctree`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/doctrees/index.doctree` & `reactive_reference-0.2.0/reactive_reference/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/doctrees/modules.doctree` & `reactive_reference-0.2.0/reactive_reference/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/doctrees/reference.doctree` & `reactive_reference-0.2.0/reactive_reference/docs/_build/doctrees/reference.doctree`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/_sources/event.rst.txt` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/_sources/event.rst.txt`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/alabaster.css` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/basic.css` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/doctools.js` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/language_data.js` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/pygments.css` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/searchtools.js` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/_static/sphinx_highlight.js` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/event.html` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/event.html`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/genindex.html` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/index.html` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/modules.html` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/objects.inv` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/py-modindex.html` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/reference.html` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/reference.html`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/search.html` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/_build/html/searchindex.js` & `reactive_reference-0.2.0/reactive_reference/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/conf.py` & `reactive_reference-0.2.0/reactive_reference/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/event.rst` & `reactive_reference-0.2.0/reactive_reference/docs/event.rst`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/make.bat` & `reactive_reference-0.2.0/reactive_reference/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/docs/Makefile` & `reactive_reference-0.2.0/reactive_reference/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/event/__init__.py` & `reactive_reference-0.2.0/reactive_reference/event/__init__.py`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/event/EventStream.py` & `reactive_reference-0.2.0/reactive_reference/event/EventStream.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from reactive_reference.event.data.Domain import Domain
 from reactive_reference.event.data.Entity import Entity
 from reactive_reference.event.data.Event import Event
 from reactive_reference.event.data.EventType import EventType
 from reactive_reference.event.data.LifecycleEvent import LifecycleEvent
 from reactive_reference.event.data.Payload import Payload
 from reactive_reference.event.data.ReplayStrategy import ReplayStrategy
+from reactive_reference.event.interfaces.IEventProducer import IEventProducer
 from reactive_reference.event.interfaces.IEventStream import IEventStream
 from reactive_reference.event.interfaces.IEventSubscriber import IEventSubscriber
 from reactive_reference.utils import Singleton, md5_hash, random_string
 
 
 class EventStream(IEventStream, Singleton):
     def __init__(
@@ -28,14 +29,15 @@
         :param exclusive: Set the mode of the stream to exclusive. If True, will only notify those of the same domain
         :param limit: If not set stream has no limit for how many values to store. Otherwise, oldest are dropped
         """
         self.__id = md5_hash("Stream")
         self.__values: List[Event] = []
         self.__lifecycle_events: List[LifecycleEvent] = []
         self.__subscribers: Dict[str, Entity] = {}
+        self.__producers: Dict[str, Entity] = {}
         self.__exclusive = exclusive
         self.__notifications: Dict[str, dict] = {}
         self.__limit = limit
         self.__emit_lifecycle_event(EventType.ON_START, Payload("Stream Started"), None)
         self.__alive = True
 
     @property
@@ -58,14 +60,18 @@
         exclusive: bool = False,
     ) -> NoReturn:
         async def runner(runners: List[Callable]) -> NoReturn:
             await asyncio.gather(*runners)
 
         if not self.__alive:
             return
+        if not isinstance(entity.instance, IEventProducer):
+            return
+        if entity.id not in self.__producers.keys():
+            return
         if isinstance(data, EventType):
             if data.KILL:
                 self.__alive = False
                 self.__emit_lifecycle_event(EventType.KILL, Payload("Stream Kill"), entity)
                 return
         e = Event(
             md5_hash(data),
@@ -82,15 +88,15 @@
             for sub in self.__get_other_instances(entity):
                 coroutines.append(sub.instance.on_event_receive(e))
         else:
             for sub in self.__get_instances_for_domain(entity, domain, exclusive):
                 coroutines.append(sub.instance.on_event_receive(e))
         asyncio.run(runner(coroutines))
 
-    def get(self, _filter: Union[Callable, None] = None) -> List[Event]:
+    def get(self, _filter: Union[Callable[[Event], bool], None] = None) -> List[Event]:
         if _filter:
             return [_ for _ in self.__values if _filter(_)]
         return self.__values
 
     def follow(self, entity: Entity, domain: Domain) -> bool:
         if entity.domain == domain:
             self.__emit_lifecycle_event(
@@ -136,37 +142,47 @@
         self.__emit_lifecycle_event(
             EventType.ON_UNFOLLOW, Payload("Failed to unfollow"), entity
         )
         return False
 
     def register(
         self,
-        instance: IEventSubscriber,
+        instance: IEventSubscriber | IEventProducer,
         domain: Domain = Constants.DefaultDomain,
     ) -> Entity:
         _entity = Entity(md5_hash(random_string(15)), instance, domain)
         if self.__alive:
-            self.__subscribers[_entity.id] = _entity
-            self.__emit_lifecycle_event(
-                EventType.ON_SUBSCRIBE, Payload("New entity subscribed"), _entity
-            )
-            self.__replay_events_on_subscribe(instance)
-            self.__emit_lifecycle_event(
-                EventType.ON_SUBSCRIBE,
-                Payload(
-                    f"Executed {_entity.instance.strategy.name} ReplayStrategy on {_entity.id}"
-                ),
-                _entity,
-            )
+            if isinstance(instance, IEventSubscriber):
+                self.__subscribers[_entity.id] = _entity
+                self.__emit_lifecycle_event(
+                    EventType.ON_SUBSCRIBE, Payload("New entity subscribed"), _entity
+                )
+                self.__replay_events_on_subscribe(instance)
+                self.__emit_lifecycle_event(
+                    EventType.ON_SUBSCRIBE,
+                    Payload(
+                        f"Executed {_entity.instance.strategy.name} ReplayStrategy on {_entity.id}"
+                    ),
+                    _entity,
+                )
+            elif isinstance(instance, IEventProducer):
+                self.__producers[_entity.id] = _entity
         return _entity
 
     def unregister(self, entity: Entity) -> bool:
-        _ = self.__subscribers.get(entity.id, None)
+        _ = (
+            self.__subscribers.get(entity.id, None)
+            if isinstance(entity.instance, IEventSubscriber)
+            else self.__producers.get(entity.id)
+        )
         if _:
-            del self.__subscribers[entity.id]
+            if isinstance(entity.instance, IEventSubscriber):
+                del self.__subscribers[entity.id]
+            else:
+                del self.__producers[entity.id]
             self.__emit_lifecycle_event(
                 EventType.ON_UNSUBSCRIBE,
                 Payload(f"Entity {entity.id} unsubscribed"),
                 entity,
             )
             return True
         self.__emit_lifecycle_event(
```

### Comparing `reactive_reference-0.1.1/reactive_reference/event/EventSubscriber.py` & `reactive_reference-0.2.0/reactive_reference/event/EventSubscriber.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABCMeta, abstractmethod
-from typing import Any, Callable, List, NoReturn, Union
+from typing import Callable, List, NoReturn, Union
 
 from reactive_reference.event.Constants import Constants
 from reactive_reference.event.data.Domain import Domain
 from reactive_reference.event.data.Event import Event
 from reactive_reference.event.data.LifecycleEvent import LifecycleEvent
 from reactive_reference.event.data.ReplayStrategy import ReplayStrategy
 from reactive_reference.event.interfaces.IEventStream import IEventStream
@@ -42,18 +42,15 @@
     @abstractmethod
     async def on_event_receive(self, data: Event) -> NoReturn:
         ...
 
     async def on_lifecycle_event(self, event: LifecycleEvent) -> NoReturn:
         ...
 
-    def emit(self, data: Any, exclusive: bool = False) -> NoReturn:
-        self.__stream.emit(self.__entity, data, self.__domain, exclusive)
-
-    def get(self, _filter: Union[Callable, None] = None) -> List[Event]:
+    def get(self, _filter: Union[Callable[[Event], bool], None] = None) -> List[Event]:
         return self.__stream.get(_filter)
 
     def unregister(self) -> bool:
         return self.__stream.unregister(self.__entity)
 
     def follow(self, domain: Domain) -> bool:
         return self.__stream.follow(self.__entity, domain)
```

### Comparing `reactive_reference-0.1.1/reactive_reference/event/interfaces/IEventStream.py` & `reactive_reference-0.2.0/reactive_reference/event/interfaces/IEventStream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Callable, List, Any, NoReturn, Union
 
 from reactive_reference.event.Constants import Constants
 from reactive_reference.event.data.Domain import Domain
 from reactive_reference.event.data.Entity import Entity
 from reactive_reference.event.data.Event import Event
+from reactive_reference.event.interfaces.IEventProducer import IEventProducer
 from reactive_reference.event.interfaces.IEventSubscriber import IEventSubscriber
 
 
 class IEventStream:
     __name__ = "EventStream"
 
     latest: Event
@@ -26,15 +27,15 @@
         :param data: Structured payload for the Event Stream
         :param domain: Domain to which the data is binded to
         :param exclusive: Set the mode of the message to exclusive. If True, will only notify those of the same domain
         :return: None
         """
         ...
 
-    def get(self, _filter: Union[Callable, None] = None) -> List[Event]:
+    def get(self, _filter: Union[Callable[[Event], bool], None] = None) -> List[Event]:
         """
         Retrieve all events
         :param _filter: Function to allow filtering of events
         :return: List with all applicable Events
         """
         ...
 
@@ -54,15 +55,15 @@
         :param domain: Domain to unfollow from the stream
         :return: True if was correctly unfollowed, False otherwise or if already unfollowed
         """
         ...
 
     def register(
         self,
-        instance: IEventSubscriber,
+        instance: IEventSubscriber | IEventProducer,
         domain: Domain = Constants.DefaultDomain,
     ) -> Entity:
         """
         Register class for Event updates
         :param instance: Class instance that extends from EventSubscriber
         :param domain: Domain to subscribe for updates. If no domain is given class will subscribe to every update
         :return: Entity object
```

### Comparing `reactive_reference-0.1.1/reactive_reference/event/interfaces/IEventSubscriber.py` & `reactive_reference-0.2.0/reactive_reference/event/interfaces/IEventSubscriber.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, List, NoReturn, Union
+from typing import Callable, List, NoReturn, Union
 
 from reactive_reference.event.data.Domain import Domain
 from reactive_reference.event.data.Event import Event
 from reactive_reference.event.data.LifecycleEvent import LifecycleEvent
 from reactive_reference.event.data.ReplayStrategy import ReplayStrategy
 
 
@@ -25,24 +25,15 @@
         """
         Triggered by the event stream when new Events are posted in the Stream
         :param event: Lifecycle event sent by the stream
         :return: None
         """
         ...
 
-    def emit(self, data: Any, exclusive: bool = False) -> NoReturn:
-        """
-        Sends data to the Event Stream
-        :param data: Structured payload for the Event Stream
-        :param exclusive: Set the mode of the message to exclusive. If True, will only notify those of the same domain
-        :return: None
-        """
-        ...
-
-    def get(self, _filter: Union[Callable, None] = None) -> List[Event]:
+    def get(self, _filter: Union[Callable[[Event], bool], None] = None) -> List[Event]:
         """
         Retrieve all events
         :param _filter: Function to allow filtering of events
         :return: List with all applicable Events
         """
         ...
```

### Comparing `reactive_reference-0.1.1/reactive_reference/jellyfin/common.py` & `reactive_reference-0.2.0/reactive_reference/jellyfin/common.py`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/reference/IReference.py` & `reactive_reference-0.2.0/reactive_reference/reference/IReference.py`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/reference/Reference.py` & `reactive_reference-0.2.0/reactive_reference/reference/Reference.py`

 * *Files identical despite different names*

### Comparing `reactive_reference-0.1.1/reactive_reference/utils.py` & `reactive_reference-0.2.0/reactive_reference/utils.py`

 * *Files identical despite different names*

