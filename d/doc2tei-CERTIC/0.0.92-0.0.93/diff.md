# Comparing `tmp/doc2tei-CERTIC-0.0.92.tar.gz` & `tmp/doc2tei-CERTIC-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc2tei-CERTIC-0.0.92.tar", last modified: Thu Mar 28 17:14:57 2024, max compression
+gzip compressed data, was "doc2tei-CERTIC-0.0.93.tar", last modified: Mon Apr  8 15:45:04 2024, max compression
```

## Comparing `doc2tei-CERTIC-0.0.92.tar` & `doc2tei-CERTIC-0.0.93.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.972764 doc2tei-CERTIC-0.0.92/
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      537 2024-03-28 17:14:57.972764 doc2tei-CERTIC-0.0.92/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1710 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.952763 doc2tei-CERTIC-0.0.92/doc2tei/
--rw-rw-rw-   0 root         (0) root         (0)    21029 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1518 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.952763 doc2tei-CERTIC-0.0.92/doc2tei/resources/
--rwxrwxrwx   0 root         (0) root         (0)  5046534 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/saxon9.jar
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.960763 doc2tei-CERTIC-0.0.92/doc2tei/resources/schema/
--rw-rw-rw-   0 root         (0) root         (0)   359005 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/schema/metopes.rng
--rw-rw-rw-   0 root         (0) root         (0)   176870 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/schema/openedition.rng
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.964763 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/
--rw-rw-rw-   0 root         (0) root         (0)     4312 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl
--rw-rw-rw-   0 root         (0) root         (0)     8141 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4404 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl
--rw-rw-rw-   0 root         (0) root         (0)    33329 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3098 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/cleanup.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.964763 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-02-normalisation/
--rw-rw-rw-   0 root         (0) root         (0)     3431 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl
--rw-rw-rw-   0 root         (0) root         (0)     8617 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl
--rw-rw-rw-   0 root         (0) root         (0)     7762 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4904 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4086 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.964763 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-03-enrich/
--rw-rw-rw-   0 root         (0) root         (0)     3552 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-03-enrich/enrich.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.964763 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/
--rw-rw-rw-   0 root         (0) root         (0)     4975 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-cit.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3685 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-figure-grp.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3689 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-figure.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4093 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-floatingText.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3746 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-review.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4045 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-sp.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4248 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl
--rw-rw-rw-   0 root         (0) root         (0)     5996 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/hierarchize-review.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.968764 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-05-control/
--rw-rw-rw-   0 root         (0) root         (0)     2648 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-05-control/control-errors.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4036 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-05-control/control-hierarchy.xsl
--rw-rw-rw-   0 root         (0) root         (0)    10640 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-05-control/control-styles-id.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.968764 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-06-hierarchize/
--rw-rw-rw-   0 root         (0) root         (0)     4873 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.968764 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-07-organise/
--rw-rw-rw-   0 root         (0) root         (0)     8786 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-07-organise/organise.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.968764 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/
--rw-rw-rw-   0 root         (0) root         (0)     4102 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/back.xsl
--rw-rw-rw-   0 root         (0) root         (0)    14220 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_cit.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4026 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_code.xsl
--rw-rw-rw-   0 root         (0) root         (0)     7816 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_div-para.xsl
--rw-rw-rw-   0 root         (0) root         (0)    12266 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_figure.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3771 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_linking.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4335 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_list.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3468 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_note.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3592 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_typo.xsl
--rw-rw-rw-   0 root         (0) root         (0)    12185 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/front.xsl
--rw-rw-rw-   0 root         (0) root         (0)    33916 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/teiHeader.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3499 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/totei.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.968764 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-09-toOpenedition/
--rwxrwxrwx   0 root         (0) root         (0)     8845 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:14:57.972764 doc2tei-CERTIC-0.0.92/doc2tei_CERTIC.egg-info/
--rw-r--r--   0 root         (0) root         (0)      537 2024-03-28 17:14:57.000000 doc2tei-CERTIC-0.0.92/doc2tei_CERTIC.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2286 2024-03-28 17:14:57.000000 doc2tei-CERTIC-0.0.92/doc2tei_CERTIC.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 17:14:57.000000 doc2tei-CERTIC-0.0.92/doc2tei_CERTIC.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-03-28 17:14:57.000000 doc2tei-CERTIC-0.0.92/doc2tei_CERTIC.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-28 17:14:57.000000 doc2tei-CERTIC-0.0.92/doc2tei_CERTIC.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-28 17:14:57.000000 doc2tei-CERTIC-0.0.92/doc2tei_CERTIC.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-28 17:14:57.972764 doc2tei-CERTIC-0.0.92/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      832 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.92/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.908650 doc2tei-CERTIC-0.0.93/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      537 2024-04-08 15:45:04.908650 doc2tei-CERTIC-0.0.93/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.836646 doc2tei-CERTIC-0.0.93/doc2tei/
+-rw-rw-rw-   0 root         (0) root         (0)    21029 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.836646 doc2tei-CERTIC-0.0.93/doc2tei/resources/
+-rwxrwxrwx   0 root         (0) root         (0)  5046534 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/saxon9.jar
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.892649 doc2tei-CERTIC-0.0.93/doc2tei/resources/schema/
+-rw-rw-rw-   0 root         (0) root         (0)   355944 2024-03-28 17:16:57.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/schema/metopes.rng
+-rw-rw-rw-   0 root         (0) root         (0)   176870 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/schema/openedition.rng
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.892649 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/
+-rw-rw-rw-   0 root         (0) root         (0)     4312 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     8141 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    33450 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/cleanup.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.896650 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-02-normalisation/
+-rw-rw-rw-   0 root         (0) root         (0)     3431 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     8617 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4904 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4086 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.896650 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-03-enrich/
+-rw-rw-rw-   0 root         (0) root         (0)     3552 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-03-enrich/enrich.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.900650 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-cit.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3685 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-figure-grp.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3689 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-figure.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4093 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-floatingText.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3746 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-review.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-sp.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4248 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     5996 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/hierarchize-review.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.900650 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-05-control/
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-05-control/control-errors.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4036 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-05-control/control-hierarchy.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    10640 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-05-control/control-styles-id.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.900650 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-06-hierarchize/
+-rw-rw-rw-   0 root         (0) root         (0)     5073 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.900650 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-07-organise/
+-rw-rw-rw-   0 root         (0) root         (0)     8786 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-07-organise/organise.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.904650 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/
+-rw-rw-rw-   0 root         (0) root         (0)     4102 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/back.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    14220 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_cit.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4026 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_code.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     8280 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_div-para.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    12266 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_figure.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_linking.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4335 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_list.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3468 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_note.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3592 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_typo.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    12206 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/front.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    33916 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/teiHeader.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3499 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/totei.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.904650 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-09-toOpenedition/
+-rwxrwxrwx   0 root         (0) root         (0)     8845 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:45:04.908650 doc2tei-CERTIC-0.0.93/doc2tei_CERTIC.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      537 2024-04-08 15:45:04.000000 doc2tei-CERTIC-0.0.93/doc2tei_CERTIC.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-04-08 15:45:04.000000 doc2tei-CERTIC-0.0.93/doc2tei_CERTIC.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:45:04.000000 doc2tei-CERTIC-0.0.93/doc2tei_CERTIC.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-08 15:45:04.000000 doc2tei-CERTIC-0.0.93/doc2tei_CERTIC.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-08 15:45:04.000000 doc2tei-CERTIC-0.0.93/doc2tei_CERTIC.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 15:45:04.000000 doc2tei-CERTIC-0.0.93/doc2tei_CERTIC.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 15:45:04.908650 doc2tei-CERTIC-0.0.93/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.93/setup.py
```

### Comparing `doc2tei-CERTIC-0.0.92/PKG-INFO` & `doc2tei-CERTIC-0.0.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc2tei-CERTIC
-Version: 0.0.92
+Version: 0.0.93
 Summary: Convert ODT and DOCX files to TEI
 Home-page: https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doc2tei-CERTIC-0.0.92/README.md` & `doc2tei-CERTIC-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/__init__.py` & `doc2tei-CERTIC-0.0.93/doc2tei/__init__.py`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/__main__.py` & `doc2tei-CERTIC-0.0.93/doc2tei/__main__.py`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/saxon9.jar` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/saxon9.jar`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/schema/metopes.rng` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/schema/metopes.rng`

 * *Files 0% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/schema/metopes.rng` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/schema/metopes.rng`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <grammar xmlns="http://relaxng.org/ns/structure/1.0" xmlns:tei="http://www.tei-c.org/ns/1.0" xmlns:teix="http://www.tei-c.org/ns/Examples" xmlns:xlink="http://www.w3.org/1999/xlink" datatypeLibrary="http://www.w3.org/2001/XMLSchema-datatypes" ns="http://www.tei-c.org/ns/1.0">
   <!--
-Schema generated from ODD source 2024-02-03T20:04:28Z. .
+Schema generated from ODD source 2024-02-24T14:28:08Z. .
 TEI Edition: 
 TEI Edition Location: https://www.tei-c.org/Vault/P5//
   
 -->
   <!---->
   <div datatypeLibrary="http://www.w3.org/2001/XMLSchema-datatypes">
     <div>
@@ -4053,62 +4053,62 @@
           </data>
         </choice>
       </attribute>
     </optional>
   </define>
   <define name="model.nameLike.agent">
     <choice>
+      <ref name="name"/>
       <ref name="orgName"/>
       <ref name="persName"/>
-      <ref name="name"/>
     </choice>
   </define>
   <define name="model.nameLike.agent_alternation">
     <choice>
+      <ref name="name"/>
       <ref name="orgName"/>
       <ref name="persName"/>
-      <ref name="name"/>
     </choice>
   </define>
   <define name="model.nameLike.agent_sequence">
+    <ref name="name"/>
     <ref name="orgName"/>
     <ref name="persName"/>
-    <ref name="name"/>
   </define>
   <define name="model.nameLike.agent_sequenceOptional">
     <optional>
-      <ref name="orgName"/>
+      <ref name="name"/>
     </optional>
     <optional>
-      <ref name="persName"/>
+      <ref name="orgName"/>
     </optional>
     <optional>
-      <ref name="name"/>
+      <ref name="persName"/>
     </optional>
   </define>
   <define name="model.nameLike.agent_sequenceOptionalRepeatable">
     <zeroOrMore>
-      <ref name="orgName"/>
+      <ref name="name"/>
     </zeroOrMore>
     <zeroOrMore>
-      <ref name="persName"/>
+      <ref name="orgName"/>
     </zeroOrMore>
     <zeroOrMore>
-      <ref name="name"/>
+      <ref name="persName"/>
     </zeroOrMore>
   </define>
   <define name="model.nameLike.agent_sequenceRepeatable">
     <oneOrMore>
-      <ref name="orgName"/>
+      <ref name="name"/>
     </oneOrMore>
     <oneOrMore>
-      <ref name="persName"/>
+      <ref name="orgName"/>
     </oneOrMore>
     <oneOrMore>
-      <ref name="name"/>
+      <ref name="persName"/>
     </oneOrMore>
   </define>
   <define name="model.segLike">
     <choice>
       <ref name="seg"/>
     </choice>
   </define>
@@ -5222,17 +5222,17 @@
       <ref name="floatingText"/>
     </oneOrMore>
   </define>
   <define name="model.respLike">
     <choice>
       <ref name="author"/>
       <ref name="editor"/>
+      <ref name="sponsor"/>
       <ref name="funder"/>
       <ref name="respStmt"/>
-      <ref name="sponsor"/>
     </choice>
   </define>
   <define name="model.divWrapper">
     <choice>
       <ref name="argument"/>
       <ref name="epigraph"/>
       <ref name="byline"/>
@@ -5269,16 +5269,16 @@
       <ref name="model.divBottomPart"/>
     </choice>
   </define>
   <define name="model.imprintPart">
     <choice>
       <ref name="biblScope"/>
       <ref name="distributor"/>
-      <ref name="pubPlace"/>
       <ref name="publisher"/>
+      <ref name="pubPlace"/>
     </choice>
   </define>
   <define name="model.addressLike">
     <choice>
       <ref name="email"/>
       <ref name="affiliation"/>
       <ref name="address"/>
@@ -5437,15 +5437,14 @@
       <ref name="extent"/>
     </choice>
   </define>
   <define name="model.frontPart">
     <choice>
       <ref name="model.frontPart.drama"/>
       <ref name="listBibl"/>
-      <ref name="titlePage"/>
     </choice>
   </define>
   <define name="model.pPart.data">
     <choice>
       <ref name="model.dateLike"/>
       <ref name="model.measureLike"/>
       <ref name="model.addressLike"/>
@@ -5628,15 +5627,15 @@
       <ref name="att.global.attribute.xmlbase"/>
       <ref name="att.global.attribute.xmlspace"/>
       <ref name="att.global.rendition.attribute.rendition"/>
       <optional>
         <attribute name="rend">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
           <data type="token">
-            <param name="pattern">(Vol_.*)|(editor-[\w]*)|(author(ity|ities)?(-|_)?[\w]*)|(title-[\w]*)|(TEI_local[\w]*)|(unkown:[\w]*)|(break|answer|question|consecutive|caption|credits|#rtl|#ltr|docTitle|titlePart|docAuthor|affiliation|email|sponsor)</param>
+            <param name="pattern">(archeo_.*)|(Vol_.*)|(editor-[\w]*)|(author(ity|ities)?(-|_)?[\w]*)|(title-[\w]*)|(TEI_local[\w]*)|(unkown:[\w]*)|(break|answer|question|consecutive|caption|credits|#rtl|#ltr|docTitle|titlePart|docAuthor|affiliation|email|sponsor|signature)</param>
           </data>
         </attribute>
       </optional>
       <optional>
         <attribute name="select">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
           <data type="anyURI">
@@ -5783,18 +5782,39 @@
       <ref name="att.global.rendition.attribute.rend"/>
       <ref name="att.global.rendition.attribute.rendition"/>
       <ref name="att.typed.attribute.type"/>
       <ref name="att.canonical.attributes"/>
       <empty/>
     </element>
   </define>
+  <define name="name">
+    <element name="name">
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(name, proper noun) contains a proper noun or noun phrase. [3.6.1. Referring Strings]</a:documentation>
+      <ref name="macro.phraseSeq"/>
+      <ref name="att.datable.attributes"/>
+      <optional>
+        <attribute name="type">
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">Sample values include: 1] speaker</a:documentation>
+          <text/>
+        </attribute>
+      </optional>
+      <empty/>
+    </element>
+  </define>
   <define name="email">
     <element name="email">
       <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(electronic mail address) contains an email address identifying a location to which email messages can be delivered. [3.6.2. Addresses]</a:documentation>
       <ref name="macro.phraseSeq"/>
+      <optional>
+        <attribute name="xml:id">
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+          <text/>
+        </attribute>
+      </optional>
+      <empty/>
     </element>
   </define>
   <define name="num">
     <element name="num">
       <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(number) contains a number, written in any form. [3.6.3. Numbers and
 Measures]</a:documentation>
       <ref name="macro.phraseSeq"/>
@@ -6020,25 +6040,16 @@
               </choice>
             </oneOrMore>
           </list>
         </attribute>
       </optional>
       <optional>
         <attribute name="type">
-          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">characterizes the element in some sense, using any convenient classification scheme or typology.</a:documentation>
-          <choice>
-            <value>aut</value>
-            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
-            <value>biography</value>
-            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
-            <value>pbl</value>
-            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
-            <value>trl</value>
-            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
-          </choice>
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">Sample values include:</a:documentation>
+          <text/>
         </attribute>
       </optional>
       <empty/>
     </element>
   </define>
   <define name="graphic">
     <element name="graphic">
@@ -6265,14 +6276,24 @@
             </oneOrMore>
           </list>
         </attribute>
       </optional>
       <empty/>
     </element>
   </define>
+  <define name="resp">
+    <element name="resp">
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(responsibility) [Métopes] contient une expression décrivant la nature de la responsabilité intellectuelle d'une personne. [3.12.2.2. Titles, Authors, and Editors 2.2.1. The Title Statement 2.2.2. The Edition Statement 2.2.5. The Series Statement]</a:documentation>
+      <ref name="macro.phraseSeq.limited"/>
+      <ref name="att.global.attributes"/>
+      <ref name="att.canonical.attributes"/>
+      <ref name="att.datable.attributes"/>
+      <empty/>
+    </element>
+  </define>
   <define name="title">
     <element name="title">
       <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(title) contains a title for any kind of work. [3.12.2.2. Titles, Authors, and Editors 2.2.1. The Title Statement 2.2.5. The Series Statement]</a:documentation>
       <ref name="macro.paraContent"/>
       <ref name="att.global.attribute.xmlid"/>
       <ref name="att.global.attribute.n"/>
       <ref name="att.global.attribute.xmllang"/>
@@ -6394,33 +6415,53 @@
       <ref name="att.typed.attribute.type"/>
       <optional>
         <attribute name="rend">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(rendition) indicates how the element in question was rendered or presented in the source text.</a:documentation>
           <list>
             <oneOrMore>
               <choice>
-                <value>block</value>
-                <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
                 <value>inline</value>
                 <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+                <value>bold</value>
+                <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+                <value>italic</value>
+                <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+                <value>small-caps</value>
+                <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+                <value>strikethrough</value>
+                <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+                <value>sup</value>
+                <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+                <value>sub</value>
+                <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+                <value>underline</value>
+                <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+                <value>uppercase</value>
+                <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
               </choice>
             </oneOrMore>
           </list>
         </attribute>
       </optional>
       <optional>
         <attribute name="target">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
           <text/>
         </attribute>
       </optional>
       <optional>
         <attribute name="n">
-          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(number) gives a number (or other label) for an element, which is not necessarily unique within the document.</a:documentation>
-          <data type="string"/>
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+          <text/>
+        </attribute>
+      </optional>
+      <optional>
+        <attribute name="sameAs">
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+          <text/>
         </attribute>
       </optional>
       <empty/>
     </element>
   </define>
   <define name="biblStruct">
     <element name="biblStruct">
@@ -6701,14 +6742,24 @@
         </oneOrMore>
         <zeroOrMore>
           <ref name="model.respLike"/>
         </zeroOrMore>
       </group>
     </element>
   </define>
+  <define name="sponsor">
+    <element name="sponsor">
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(sponsor) [Métopes] indique le nom d’une institution ou d’un organisme partenaires. [2.2.1. The Title Statement]</a:documentation>
+      <ref name="macro.phraseSeq.limited"/>
+      <ref name="att.global.attributes"/>
+      <ref name="att.canonical.attributes"/>
+      <ref name="att.datable.attributes"/>
+      <empty/>
+    </element>
+  </define>
   <define name="funder">
     <element name="funder">
       <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(funding body) specifies the name of an individual, institution, or organization responsible for the funding of a project or text. [2.2.1. The Title Statement]</a:documentation>
       <oneOrMore>
         <choice>
           <ref name="orgName"/>
           <ref name="idno"/>
@@ -7672,16 +7723,14 @@
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>gallery</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>abbreviations</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>catalogue</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
-            <value>compte-rendu</value>
-            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>chronique</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>epigraph</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>biographical-note</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>translator-note</value>
@@ -8121,15 +8170,15 @@
   <define name="model.addrPart">
     <choice>
       <ref name="addrLine"/>
     </choice>
   </define>
   <define name="ab">
     <element name="ab">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(anonymous block) contains any component-level unit of text, acting as a container for phrase or inter level elements analogous to, but without the same constraints as, a paragraph. []</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(anonymous block) [Métopes] contient une unité de texte quelconque, de niveau &quot;composant&quot;, faisant office de contenant anonyme pour une expression ou des éléments de niveau intermédiaire, analogue à un paragraphe mais sans sa portée sémantique. []</a:documentation>
       <zeroOrMore>
         <choice>
           <ref name="address"/>
           <ref name="bibl"/>
           <ref name="date"/>
           <ref name="desc"/>
           <ref name="dim"/>
@@ -8164,14 +8213,16 @@
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>expression</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>digital_download</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>digital_online</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>CUP</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
           </choice>
         </attribute>
       </optional>
       <optional>
         <attribute name="subtype">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(subtype) provides a sub-categorization of the element, if needed
 Sample values include: 1] EPUB; 2] PDF; 3] HTML</a:documentation>
@@ -8181,15 +8232,15 @@
         </attribute>
       </optional>
       <empty/>
     </element>
   </define>
   <define name="abstract">
     <element name="abstract">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">contains a summary or formal abstract prefixed to an existing source document by the encoder. []</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">[Métopes] contains a summary or formal abstract prefixed to an existing source document by the encoder. []</a:documentation>
       <oneOrMore>
         <choice>
           <ref name="model.pLike"/>
           <ref name="model.listLike"/>
           <ref name="listBibl"/>
         </choice>
       </oneOrMore>
@@ -8212,25 +8263,17 @@
             </oneOrMore>
           </list>
         </attribute>
       </optional>
       <empty/>
     </element>
   </define>
-  <define name="addrLine">
-    <element name="addrLine">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(address line) contains one line of a postal address. [  ]</a:documentation>
-      <ref name="macro.phraseSeq"/>
-      <ref name="att.global.attributes"/>
-      <empty/>
-    </element>
-  </define>
   <define name="address">
     <element name="address">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(address) contains a postal address, for example of a publisher, an organization, or an individual. [  ]</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(address) [Métopes] contient une adresse postale ou d'un autre type, par exemple l'adresse d'un éditeur, d'un organisme ou d'une personne. [  ]</a:documentation>
       <group>
         <zeroOrMore>
           <ref name="model.global"/>
         </zeroOrMore>
         <oneOrMore>
           <group>
             <ref name="model.addrPart"/>
@@ -8240,49 +8283,65 @@
           </group>
         </oneOrMore>
       </group>
       <ref name="att.global.attributes"/>
       <empty/>
     </element>
   </define>
+  <define name="addrLine">
+    <element name="addrLine">
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(address line) [Métopes] contient une ligne d'adresse postale. [  ]</a:documentation>
+      <ref name="macro.phraseSeq"/>
+      <ref name="att.global.attributes"/>
+      <empty/>
+    </element>
+  </define>
   <define name="byline">
     <element name="byline">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(byline) contains the primary statement of responsibility given for a work on its title page or at the head or end of the work. [ ]</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(byline) [Métopes] indique la responsabilité principale pour une œuvre donnée sur la page de titre ou au début ou à la fin de l’œuvre. [ ]</a:documentation>
       <zeroOrMore>
         <choice>
           <text/>
           <ref name="model.gLike"/>
           <ref name="model.phrase"/>
           <ref name="model.global"/>
         </choice>
       </zeroOrMore>
       <ref name="att.global.attributes"/>
       <empty/>
     </element>
   </define>
   <define name="depth">
     <element name="depth">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">
-        (depth) contains a measurement from the front to the back of an object, perpendicular to the measurement given by the
-        <code xmlns="http://www.w3.org/1999/xhtml">&lt;width&gt;</code>
-        element. []
-      </a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(depth) [Métopes] contient une dimension mesurée sur le dos du manuscrit. []</a:documentation>
       <ref name="att.global.attributes"/>
       <optional>
         <attribute name="unit">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
           <text/>
         </attribute>
       </optional>
+      <optional>
+        <attribute name="quantity">
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+          <choice>
+            <data type="double"/>
+            <data type="token">
+              <param name="pattern">(\-?[\d]+/\-?[\d]+)</param>
+            </data>
+            <data type="decimal"/>
+          </choice>
+        </attribute>
+      </optional>
       <empty/>
     </element>
   </define>
   <define name="dim">
     <element name="dim">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">contains any single measurement forming part of a dimensional specification of some sort. []</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">[Métopes] contains any single measurement forming part of a dimensional specification of some sort. []</a:documentation>
       <zeroOrMore>
         <choice>
           <text/>
         </choice>
       </zeroOrMore>
       <ref name="att.global.attributes"/>
       <ref name="att.typed.attributes"/>
@@ -8299,15 +8358,15 @@
         </attribute>
       </optional>
       <empty/>
     </element>
   </define>
   <define name="dimensions">
     <element name="dimensions">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(dimensions) contains a dimensional specification. []</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(dimensions) [Métopes] contient une spécification des dimensions. []</a:documentation>
       <zeroOrMore>
         <choice>
           <ref name="depth"/>
           <ref name="height"/>
           <ref name="width"/>
         </choice>
       </zeroOrMore>
@@ -8348,15 +8407,15 @@
         </attribute>
       </optional>
       <empty/>
     </element>
   </define>
   <define name="editionStmt">
     <element name="editionStmt">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(edition statement) groups information relating to one edition of a text. [ ]</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(edition statement) [Métopes] regroupe les informations relatives à l’édition d’un texte. [ ]</a:documentation>
       <choice>
         <oneOrMore>
           <ref name="model.pLike"/>
         </oneOrMore>
         <group>
           <ref name="edition"/>
           <zeroOrMore>
@@ -8366,28 +8425,28 @@
       </choice>
       <ref name="att.global.attributes"/>
       <empty/>
     </element>
   </define>
   <define name="editorialDecl">
     <element name="editorialDecl">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(editorial practice declaration) provides details of editorial principles and practices applied during the encoding of a text. [  ]</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(editorial practice declaration) [Métopes] donne des précisions sur les pratiques et les principes éditoriaux appliqués au cours de l’encodage du texte. [  ]</a:documentation>
       <oneOrMore>
         <choice>
           <ref name="model.pLike"/>
           <ref name="model.editorialDeclPart"/>
         </choice>
       </oneOrMore>
       <ref name="att.global.attributes"/>
       <empty/>
     </element>
   </define>
   <define name="extent">
     <element name="extent">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(extent) describes the approximate size of a text stored on some carrier medium or of some other object, digital or non-digital, specified in any convenient units. [   ]</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(extent) [Métopes] décrit la taille approximative d’un texte stocké sur son support, numérique ou non numérique, exprimé dans une unité quelconque appropriée. [   ]</a:documentation>
       <ref name="macro.phraseSeq"/>
       <ref name="att.global.attribute.xmlid"/>
       <ref name="att.global.attribute.n"/>
       <ref name="att.global.attribute.xmllang"/>
       <ref name="att.global.attribute.xmlbase"/>
       <ref name="att.global.attribute.xmlspace"/>
       <ref name="att.global.rendition.attribute.rendition"/>
@@ -8406,23 +8465,23 @@
         </attribute>
       </optional>
       <empty/>
     </element>
   </define>
   <define name="foreign">
     <element name="foreign">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(foreign) identifies a word or phrase as belonging to some language other than that of the surrounding text. []</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(foreign) [Métopes] reconnaît un mot ou une expression comme appartenant à une langue différente de celle du contexte. []</a:documentation>
       <ref name="macro.phraseSeq"/>
       <ref name="att.global.attributes"/>
       <empty/>
     </element>
   </define>
   <define name="group">
     <element name="group">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(group) contains the body of a composite text, grouping together a sequence of distinct texts (or groups of such texts) which are regarded as a unit for some purpose, for example the collected works of an author, a sequence of prose essays, etc. [  ]</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(group) [Métopes] contient un ensemble de textes distincts (ou des groupes de textes de ce type), considérés comme formant une unité, par exemple pour présenter les œuvres complètes d’un auteur, une suite d’essais en prose, etc. [  ]</a:documentation>
       <zeroOrMore>
         <choice>
           <ref name="include"/>
           <ref name="group"/>
           <ref name="text"/>
           <ref name="head"/>
         </choice>
@@ -8430,49 +8489,67 @@
       <ref name="att.global.attributes"/>
       <ref name="att.typed.attributes"/>
       <empty/>
     </element>
   </define>
   <define name="height">
     <element name="height">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(height) contains a measurement measured along the axis at a right angle to the bottom of the object. []</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(height) [Métopes] contient une dimension prise sur l'axe parallèle au dos du manuscrit.  []</a:documentation>
       <ref name="att.global.attributes"/>
       <optional>
         <attribute name="unit">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
           <text/>
         </attribute>
       </optional>
+      <optional>
+        <attribute name="quantity">
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+          <choice>
+            <data type="double"/>
+            <data type="token">
+              <param name="pattern">(\-?[\d]+/\-?[\d]+)</param>
+            </data>
+            <data type="decimal"/>
+          </choice>
+        </attribute>
+      </optional>
       <empty/>
     </element>
   </define>
   <define name="index">
     <element name="index">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(index entry) marks a location to be indexed for whatever purpose. []</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(index entry) [Métopes] marque un emplacement à indexer dans un but quelconque. []</a:documentation>
       <zeroOrMore>
         <group>
           <ref name="term"/>
           <optional>
             <ref name="index"/>
           </optional>
         </group>
       </zeroOrMore>
       <ref name="att.global.attributes"/>
       <optional>
+        <attribute name="source">
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+          <text/>
+        </attribute>
+      </optional>
+      <optional>
         <attribute name="indexName">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">a single word which follows the rules defining a legal XML name (see ), supplying a name to specify which index (of several) the index entry belongs to.</a:documentation>
           <data type="string"/>
         </attribute>
       </optional>
       <empty/>
     </element>
   </define>
   <define name="measure">
     <element name="measure">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(measure) contains a word or phrase referring to some quantity of an object or commodity, usually comprising a number, a unit, and a commodity name. []</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(measure) [Métopes] contient un mot ou une expression faisant référence à la quantité d'un objet ou d'un produit, comprenant en général un nombre, une unité et le nom d'un produit. []</a:documentation>
       <ref name="macro.phraseSeq"/>
       <ref name="att.global.attributes"/>
       <ref name="att.typed.attribute.subtype"/>
       <optional>
         <attribute name="type">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">specifies the type of measurement in any convenient typology.</a:documentation>
           <data type="token">
@@ -8485,50 +8562,17 @@
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
           <text/>
         </attribute>
       </optional>
       <empty/>
     </element>
   </define>
-  <define name="name">
-    <element name="name">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(name, proper noun) contains a proper noun or noun phrase. []</a:documentation>
-      <ref name="macro.phraseSeq"/>
-      <ref name="att.global.attributes"/>
-      <ref name="att.datable.attributes"/>
-      <ref name="att.typed.attributes"/>
-      <optional>
-        <attribute name="calendar">
-          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">indicates one or more systems or calendars to which the date represented by the content of this element belongs.</a:documentation>
-          <list>
-            <oneOrMore>
-              <data type="anyURI">
-                <param name="pattern">\S+</param>
-              </data>
-            </oneOrMore>
-          </list>
-        </attribute>
-      </optional>
-      <pattern xmlns="http://purl.oclc.org/dsdl/schematron" id="commons-publishing-metopes-name-calendar-calendar-check-name-constraint-rule-10">
-        <sch:rule xmlns="http://www.tei-c.org/ns/1.0" xmlns:m="http://www.w3.org/1998/Math/MathML" xmlns:rng="http://relaxng.org/ns/structure/1.0" xmlns:sch="http://purl.oclc.org/dsdl/schematron" xmlns:xi="http://www.w3.org/2001/XInclude" xmlns:xs="http://www.w3.org/2001/XMLSchema" context="tei:*[@calendar]">
-          <sch:assert test="string-length( normalize-space(.) ) gt 0">
-            @calendar indicates one or more
-                        systems or calendars to which the date represented by the content of this element belongs,
-                        but this
-            <sch:name/>
-            element has no textual content.
-          </sch:assert>
-        </sch:rule>
-      </pattern>
-      <empty/>
-    </element>
-  </define>
   <define name="normalization">
     <element name="normalization">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(normalization) indicates the extent of normalization or regularization of the original source carried out in converting it to electronic form. [ ]</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(normalization) [Métopes] indique l'extension de la normalisation ou de la régularisation effectuée sur le texte source dans sa conversion vers sa forme électronique. [ ]</a:documentation>
       <oneOrMore>
         <ref name="model.pLike"/>
       </oneOrMore>
       <ref name="att.global.attributes"/>
       <optional>
         <attribute xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0" name="method" a:defaultValue="silent">
           <a:documentation>indicates the method adopted to indicate normalizations within the text.</a:documentation>
@@ -8539,35 +8583,35 @@
             <a:documentation>normalization represented using markup</a:documentation>
           </choice>
         </attribute>
       </optional>
       <empty/>
     </element>
   </define>
-  <define name="pubPlace">
-    <element name="pubPlace">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(publication place) contains the name of the place where a bibliographic item was published. []</a:documentation>
+  <define name="publisher">
+    <element name="publisher">
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(publisher) [Métopes] donne le nom de l'organisme responsable de la publication ou de la distribution d'un élément de la bibliographie. [ ]</a:documentation>
       <ref name="macro.phraseSeq"/>
       <ref name="att.global.attributes"/>
-      <ref name="att.naming.attributes"/>
+      <ref name="att.canonical.attributes"/>
       <empty/>
     </element>
   </define>
-  <define name="publisher">
-    <element name="publisher">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(publisher) provides the name of the organization responsible for the publication or distribution of a bibliographic item. [ ]</a:documentation>
+  <define name="pubPlace">
+    <element name="pubPlace">
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(publication place) [Métopes] contient le nom du lieu d'une publication. []</a:documentation>
       <ref name="macro.phraseSeq"/>
       <ref name="att.global.attributes"/>
-      <ref name="att.canonical.attributes"/>
+      <ref name="att.naming.attributes"/>
       <empty/>
     </element>
   </define>
   <define name="respStmt">
     <element name="respStmt">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(statement of responsibility) supplies a statement of responsibility for the intellectual content of a text, edition, recording, or series, where the specialized elements for authors, editors, etc. do not suffice or do not apply. May also be used to encode information about individuals or organizations which have played a role in the production or distribution of a bibliographic work. [   ]</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(statement of responsibility) [Métopes] indique la responsabilité quant au contenu intellectuel d'un texte, d'une édition, d'un enregistrement ou d'une publication en série, lorsque les éléments spécifiques relatifs aux auteurs, éditeurs, etc. ne suffisent pas ou ne s'appliquent pas. [   ]</a:documentation>
       <group>
         <choice>
           <group>
             <oneOrMore>
               <ref name="resp"/>
             </oneOrMore>
             <oneOrMore>
@@ -8588,113 +8632,36 @@
         </zeroOrMore>
       </group>
       <ref name="att.global.attributes"/>
       <ref name="att.canonical.attributes"/>
       <empty/>
     </element>
   </define>
-  <define name="resp">
-    <element name="resp">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(responsibility) contains a phrase describing the nature of a person's intellectual responsibility, or an organization's role in the production or distribution of a work. [   ]</a:documentation>
-      <ref name="macro.phraseSeq.limited"/>
-      <ref name="att.global.attributes"/>
-      <ref name="att.canonical.attributes"/>
-      <ref name="att.datable.attributes"/>
-      <optional>
-        <attribute name="calendar">
-          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">indicates one or more systems or calendars to which the date represented by the content of this element belongs.</a:documentation>
-          <list>
-            <oneOrMore>
-              <data type="anyURI">
-                <param name="pattern">\S+</param>
-              </data>
-            </oneOrMore>
-          </list>
-        </attribute>
-      </optional>
-      <pattern xmlns="http://purl.oclc.org/dsdl/schematron" id="commons-publishing-metopes-resp-calendar-calendar-check-resp-constraint-rule-11">
-        <sch:rule xmlns="http://www.tei-c.org/ns/1.0" xmlns:m="http://www.w3.org/1998/Math/MathML" xmlns:rng="http://relaxng.org/ns/structure/1.0" xmlns:sch="http://purl.oclc.org/dsdl/schematron" xmlns:xi="http://www.w3.org/2001/XInclude" xmlns:xs="http://www.w3.org/2001/XMLSchema" context="tei:*[@calendar]">
-          <sch:assert test="string-length( normalize-space(.) ) gt 0">
-            @calendar indicates one or more
-                        systems or calendars to which the date represented by the content of this element belongs,
-                        but this
-            <sch:name/>
-            element has no textual content.
-          </sch:assert>
-        </sch:rule>
-      </pattern>
-      <empty/>
-    </element>
-  </define>
-  <define name="sponsor">
-    <element name="sponsor">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(sponsor) specifies the name of a sponsoring organization or institution. []</a:documentation>
-      <ref name="macro.phraseSeq.limited"/>
-      <ref name="att.global.attributes"/>
-      <ref name="att.canonical.attributes"/>
-      <ref name="att.datable.attributes"/>
-      <optional>
-        <attribute name="calendar">
-          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">indicates one or more systems or calendars to which the date represented by the content of this element belongs.</a:documentation>
-          <list>
-            <oneOrMore>
-              <data type="anyURI">
-                <param name="pattern">\S+</param>
-              </data>
-            </oneOrMore>
-          </list>
-        </attribute>
-      </optional>
-      <pattern xmlns="http://purl.oclc.org/dsdl/schematron" id="commons-publishing-metopes-sponsor-calendar-calendar-check-sponsor-constraint-rule-12">
-        <sch:rule xmlns="http://www.tei-c.org/ns/1.0" xmlns:m="http://www.w3.org/1998/Math/MathML" xmlns:rng="http://relaxng.org/ns/structure/1.0" xmlns:sch="http://purl.oclc.org/dsdl/schematron" xmlns:xi="http://www.w3.org/2001/XInclude" xmlns:xs="http://www.w3.org/2001/XMLSchema" context="tei:*[@calendar]">
-          <sch:assert test="string-length( normalize-space(.) ) gt 0">
-            @calendar indicates one or more
-                        systems or calendars to which the date represented by the content of this element belongs,
-                        but this
-            <sch:name/>
-            element has no textual content.
-          </sch:assert>
-        </sch:rule>
-      </pattern>
-      <empty/>
-    </element>
-  </define>
-  <define name="titlePage">
-    <element name="titlePage">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(title page) contains the title page of a text, appearing within the front or back matter. []</a:documentation>
-      <group>
-        <zeroOrMore>
-          <choice>
-            <ref name="model.global"/>
-          </choice>
-        </zeroOrMore>
-      </group>
-      <ref name="att.global.attributes"/>
-      <ref name="att.typed.attribute.subtype"/>
-      <optional>
-        <attribute name="type">
-          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">classifies the title page according to any convenient typology.</a:documentation>
-          <data type="token">
-            <param name="pattern">[^\p{C}\p{Z}]+</param>
-          </data>
-        </attribute>
-      </optional>
-      <empty/>
-    </element>
-  </define>
   <define name="width">
     <element name="width">
-      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(width) contains a measurement of an object along the axis parallel to its bottom, e.g. perpendicular to the spine of a book or codex. []</a:documentation>
+      <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(width) [Métopes] contient une dimension mesurée sur l'axe perpendiculaire au dos du manuscrit. []</a:documentation>
       <ref name="att.global.attributes"/>
       <optional>
         <attribute name="unit">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
           <text/>
         </attribute>
       </optional>
+      <optional>
+        <attribute name="quantity">
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+          <choice>
+            <data type="double"/>
+            <data type="token">
+              <param name="pattern">(\-?[\d]+/\-?[\d]+)</param>
+            </data>
+            <data type="decimal"/>
+          </choice>
+        </attribute>
+      </optional>
       <empty/>
     </element>
   </define>
   <define name="include">
     <element name="include" ns="http://www.w3.org/2001/XInclude">
       <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
       <optional>
```

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/schema/openedition.rng` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/schema/openedition.rng`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl`

 * *Files 2% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl`

```diff
@@ -319,16 +319,16 @@
                 </xsl:otherwise>
               </xsl:choose>
               <xsl:apply-templates/>
             </xsl:element>
           </xsl:otherwise>
         </xsl:choose>
       </xsl:when>
-      <!-- surcharge alignement table -->
-      <xsl:when test="$currentElementName='text:p' and parent::table:table-cell and //style:style[@style:name=$currentStyle]/style:paragraph-properties/@fo:text-align">
+      <!-- surcharge alignement table (sur paragraphes normaux) -->
+      <xsl:when test="$currentElementName='text:p' and //style:style[@style:name=$currentStyle][starts-with(@style:parent-style-name,'Standard')] and parent::table:table-cell and //style:style[@style:name=$currentStyle]/style:paragraph-properties/@fo:text-align">
         <xsl:element name="{$currentElementName}">
           <xsl:copy-of select="@*"/>
           <xsl:attribute name="text:style-name">
             <xsl:choose>
               <xsl:when test="matches($currentStyle,'[P]\d{1,2}')">
                 <xsl:value-of select="//style:style[@style:name=$currentStyle]/@style:parent-style-name"/>
               </xsl:when>
```

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-01-cleanup/cleanup.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-01-cleanup/cleanup.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-03-enrich/enrich.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-03-enrich/enrich.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-cit.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-cit.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-figure-grp.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-figure-grp.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-figure.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-figure.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-floatingText.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-floatingText.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-review.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-review.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/group-sp.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/group-sp.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-04-group/hierarchize-review.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-04-group/hierarchize-review.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-05-control/control-errors.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-05-control/control-errors.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-05-control/control-hierarchy.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-05-control/control-hierarchy.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-05-control/control-styles-id.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-05-control/control-styles-id.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl`

 * *Files 3% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl`

```diff
@@ -42,14 +42,19 @@
                   <xsl:value-of select="concat('section',$level -1)"/>
                 </xsl:when>
                 <xsl:otherwise>
                   <xsl:value-of select="concat('section',$level)"/>
                 </xsl:otherwise>
               </xsl:choose>
             </xsl:attribute>
+            <xsl:if test="contains(@text:style-name,'+')">
+              <xsl:attribute name="subtype">
+                <xsl:value-of select="substring-after(@text:style-name,'+')"/>
+              </xsl:attribute>
+            </xsl:if>
             <xsl:call-template name="addDiv">
               <xsl:with-param name="level" select="$level+1"/>
               <xsl:with-param name="currentGroup" select="current-group()"/>
             </xsl:call-template>
           </div>
         </xsl:when>
         <xsl:otherwise>
```

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-07-organise/organise.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-07-organise/organise.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/back.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/back.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_cit.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_cit.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_code.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_code.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_div-para.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_div-para.xsl`

 * *Files 2% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_div-para.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_div-para.xsl`

```diff
@@ -158,14 +158,21 @@
               <xsl:apply-templates/>
             </bibl>
           </body>
         </xsl:otherwise>
       </xsl:choose>
     </floatingText>
   </xsl:template>
+  <!-- ### archeo CHR ### -->
+  <xsl:template match="text:p[@text:style-name='TEI_archeoCHR_fieldwork-method']|text:p[@text:style-name='TEI_archeoCHR_fieldwork-year']|text:p[@text:style-name='TEI_archeoCHR_type']|text:p[starts-with(@text:style-name,'TEI_archeoCHR_keywords')]">
+    <p rend="{concat('archeo_',substring-after(@text:style-name,'TEI_archeoCHR_'))}">
+      <xsl:copy-of select="@rendition"/>
+      <xsl:apply-templates/>
+    </p>
+  </xsl:template>
   <!-- ### bibl ### -->
   <xsl:template match="text:p[@text:style-name='TEI_bibl_reference']">
     <!--    <xsl:comment>traitement générique des bibl</xsl:comment>-->
     <bibl>
       <xsl:copy-of select="@* except(@text:style-name)"/>
       <xsl:apply-templates/>
     </bibl>
```

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_figure.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_figure.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_linking.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_linking.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_list.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_list.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_note.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_note.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/core_typo.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/core_typo.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/front.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/front.xsl`

 * *Files 0% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/front.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/front.xsl`

```diff
@@ -208,26 +208,26 @@
   </xsl:template>
   <xsl:template match="text:span[@text:style-name='TEI_reviewed_date-inline']" mode="reviewSemantic">
     <date>
       <xsl:apply-templates select=".//text()"/>
     </date>
   </xsl:template>
   <!-- archéo -->
-  <xsl:template match="*:p[starts-with(@text:style-name,'TEI_archeo')][not(preceding-sibling::*:p[starts-with(@text:style-name,'TEI_archeo')])]">
+  <xsl:template match="*:p[starts-with(@text:style-name,'TEI_archeoART')][not(preceding-sibling::*:p[starts-with(@text:style-name,'TEI_archeoART')])]">
     <div type="archeo">
-      <p rend="{concat('archeo_',substring-after(@text:style-name,'TEI_archeo_'))}">
+      <p rend="{concat('archeo_',substring-after(@text:style-name,'TEI_archeoART_'))}">
         <xsl:apply-templates/>
       </p>
-      <xsl:for-each select="following-sibling::*:p[starts-with(@text:style-name,'TEI_archeo')]">
-        <p rend="{concat('archeo_',substring-after(@text:style-name,'TEI_archeo_'))}">
+      <xsl:for-each select="following-sibling::*:p[starts-with(@text:style-name,'TEI_archeoART')]">
+        <p rend="{concat('archeo_',substring-after(@text:style-name,'TEI_archeoART_'))}">
           <xsl:apply-templates select="node()"/>
         </p>
       </xsl:for-each>
     </div>
   </xsl:template>
   <!-- suppression -->
   <xsl:template match="*:p[starts-with(@text:style-name,'TEI_acknowledgment')][preceding-sibling::*:p[starts-with(@text:style-name,'TEI_acknowledgment')]]"/>
   <xsl:template match="*:p[starts-with(@text:style-name,'TEI_dedication')][preceding-sibling::*:p[starts-with(@text:style-name,'TEI_dedication')]]"/>
   <xsl:template match="*:p[starts-with(@text:style-name,'TEI_paragraph_lead')][preceding-sibling::*:p[starts-with(@text:style-name,'TEI_paragraph_lead')]]"/>
   <xsl:template match="*:p[starts-with(@text:style-name,'TEI_erratum')][preceding-sibling::*:p[starts-with(@text:style-name,'TEI_erratum')]]"/>
-  <xsl:template match="*:p[starts-with(@text:style-name,'TEI_archeo')][preceding-sibling::*:p[starts-with(@text:style-name,'TEI_archeo')]]"/>
+  <xsl:template match="*:p[starts-with(@text:style-name,'TEI_archeoART')][preceding-sibling::*:p[starts-with(@text:style-name,'TEI_archeoART')]]"/>
 </xsl:stylesheet>
```

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/teiHeader.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/teiHeader.xsl`

 * *Files 0% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/teiHeader.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/teiHeader.xsl`

```diff
@@ -257,15 +257,15 @@
               <xsl:value-of select="//meta:user-defined[@meta:name='tplVersion']"/>
             </xsl:attribute>
             <label>Word template</label>
             <desc>Version of MS Word template used</desc>
             <!-- todo : lien vers le code publié -->
             <ref target="#"/>
           </application>
-          <application version="0.0.92">
+          <application version="0.0.93">
             <xsl:attribute name="ident" select="concat('circe-',$source)"/>
             <label>Circé</label>
             <desc>Document converted into TEI using Circé application (doc2tei pipeline)</desc>
             <!-- todo : lien vers le code publié -->
             <ref target="#"/>
           </application>
         </appInfo>
```

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-08-totei/totei.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-08-totei/totei.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl` & `doc2tei-CERTIC-0.0.93/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei_CERTIC.egg-info/PKG-INFO` & `doc2tei-CERTIC-0.0.93/doc2tei_CERTIC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc2tei-CERTIC
-Version: 0.0.92
+Version: 0.0.93
 Summary: Convert ODT and DOCX files to TEI
 Home-page: https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doc2tei-CERTIC-0.0.92/doc2tei_CERTIC.egg-info/SOURCES.txt` & `doc2tei-CERTIC-0.0.93/doc2tei_CERTIC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.92/setup.py` & `doc2tei-CERTIC-0.0.93/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="doc2tei-CERTIC",
-    version="0.0.92",
+    version="0.0.93",
     author="Mickaël Desfrênes",
     author_email="mickael.desfrenes@unicaen.fr",
     description="Convert ODT and DOCX files to TEI",
     long_description="Convert ODT and DOCX files to TEI",
     long_description_content_type="text/plain",
     url="https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe",
     packages=setuptools.find_packages(),
```

