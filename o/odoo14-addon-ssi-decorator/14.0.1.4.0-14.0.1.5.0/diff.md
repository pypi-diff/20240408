# Comparing `tmp/odoo14_addon_ssi_decorator-14.0.1.4.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_decorator-14.0.1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 53880 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1179 b- defN 23-Dec-30 14:51 odoo/addons/ssi_decorator/README.rst
--rw-r--r--  2.0 unx      180 b- defN 23-Dec-30 14:51 odoo/addons/ssi_decorator/__init__.py
--rw-r--r--  2.0 unx      414 b- defN 23-Dec-30 14:53 odoo/addons/ssi_decorator/__manifest__.py
--rw-r--r--  2.0 unx     3869 b- defN 23-Dec-30 14:51 odoo/addons/ssi_decorator/ssi_decorator.py
--rw-r--r--  2.0 unx      193 b- defN 23-Dec-30 14:51 odoo/addons/ssi_decorator/models/__init__.py
--rw-r--r--  2.0 unx     3917 b- defN 23-Dec-30 14:51 odoo/addons/ssi_decorator/models/ssi_decorator_mixin.py
--rw-r--r--  2.0 unx    48333 b- defN 23-Dec-30 14:51 odoo/addons/ssi_decorator/static/description/icon.png
--rw-r--r--  2.0 unx     1664 b- defN 23-Dec-30 14:55 odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-30 14:55 odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Dec-30 14:55 odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1098 b- defN 23-Dec-30 14:55 odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/RECORD
-11 files, 60944 bytes uncompressed, 51958 bytes compressed:  14.7%
+Zip file size: 53913 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1179 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/README.rst
+-rw-r--r--  2.0 unx      180 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/__init__.py
+-rw-r--r--  2.0 unx      414 b- defN 24-Apr-08 04:44 odoo/addons/ssi_decorator/__manifest__.py
+-rw-r--r--  2.0 unx     4197 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/ssi_decorator.py
+-rw-r--r--  2.0 unx      193 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/models/__init__.py
+-rw-r--r--  2.0 unx     3917 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/models/ssi_decorator_mixin.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/static/description/icon.png
+-rw-r--r--  2.0 unx     1662 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1098 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/RECORD
+11 files, 61270 bytes uncompressed, 51991 bytes compressed:  15.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_decorator/models/ssi_decorator_mixin.py
 Comment: 
 
 Filename: odoo/addons/ssi_decorator/static/description/icon.png
 Comment: 
 
-Filename: odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_decorator/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "SSI - Decorator",
-    "version": "14.0.1.4.0",
+    "version": "14.0.1.5.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [],
     "data": [],
 }
```

## odoo/addons/ssi_decorator/ssi_decorator.py

```diff
@@ -71,14 +71,31 @@
     return attrsetter("_pre_open_action", args)
 
 
 def post_open_action(*args):
     return attrsetter("_post_open_action", args)
 
 
+# READY
+def pre_ready_check(*args):
+    return attrsetter("_pre_ready_check", args)
+
+
+def post_ready_check(*args):
+    return attrsetter("_post_ready_check", args)
+
+
+def pre_ready_action(*args):
+    return attrsetter("_pre_ready_action", args)
+
+
+def post_ready_action(*args):
+    return attrsetter("_post_ready_action", args)
+
+
 # DONE
 def pre_done_check(*args):
     return attrsetter("_pre_done_check", args)
 
 
 def post_done_check(*args):
     return attrsetter("_post_done_check", args)
```

## Comparing `odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/METADATA` & `odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-decorator
-Version: 14.0.1.4.0
+Version: 14.0.1.5.0
 Summary: SSI - Decorator
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
-Requires-Dist: odoo (<14.1dev,>=14.0a)
+Requires-Dist: odoo <14.1dev,>=14.0a
 
 .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
    :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
    :alt: License: AGPL-3
 
 ===============
 SSI - Decorator
```

## Comparing `odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/RECORD` & `odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/ssi_decorator/README.rst,sha256=x3j1DGfpwl-LURwTV8POFMvtSKYhEvN23dbLS_6xV_c,1179
 odoo/addons/ssi_decorator/__init__.py,sha256=tzITx23QOcikJV4zQ1mAV0fGGi0rhMaF3ksZb9m8FVQ,180
-odoo/addons/ssi_decorator/__manifest__.py,sha256=i4XmFyw3pKNwdHt0DuoP4EVkLByMJjdioRUP1DuXXCs,414
-odoo/addons/ssi_decorator/ssi_decorator.py,sha256=Eg4uIwlYQS8pypR3c-0fy-Lkz7-3Rx9dLDrsP2QyM9o,3869
+odoo/addons/ssi_decorator/__manifest__.py,sha256=E2AQQNA59DYvNRFEsQrLOshZ_9tqfSR3XMx6zA-X9Fo,414
+odoo/addons/ssi_decorator/ssi_decorator.py,sha256=Z8FpIXGKZNKX9SOedUDpelZ39dofpTQ8PUPv1jxFEU4,4197
 odoo/addons/ssi_decorator/models/__init__.py,sha256=YbUtBI9pRkCEdMYdeZg_cyMUx23l346q6-paMBMWF-U,193
 odoo/addons/ssi_decorator/models/ssi_decorator_mixin.py,sha256=9lmUHQAJIEFcEXicPvArGdOISPQ0RU8klm4mPGucWuA,3917
 odoo/addons/ssi_decorator/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/METADATA,sha256=4OEp8GyF_LzCiEU-nUyKbey-WyzlsnWxCJCSXXE7AkA,1664
-odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_decorator-14.0.1.4.0.dist-info/RECORD,,
+odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/METADATA,sha256=wqfHuHX5V8fQ-zvCKR-yb-NPcsDMzrOM0YKdDrUYPv8,1662
+odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/RECORD,,
```

