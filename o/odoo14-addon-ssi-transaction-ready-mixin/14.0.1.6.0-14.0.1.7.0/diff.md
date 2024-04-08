# Comparing `tmp/odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 54229 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1272 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_ready_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_ready_mixin/__init__.py
--rw-r--r--  2.0 unx      543 b- defN 23-Dec-30 14:52 odoo/addons/ssi_transaction_ready_mixin/__manifest__.py
--rw-r--r--  2.0 unx      198 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_ready_mixin/models/__init__.py
--rw-r--r--  2.0 unx     4781 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py
--rw-r--r--  2.0 unx    48333 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_ready_mixin/static/description/icon.png
--rw-r--r--  2.0 unx      553 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml
--rw-r--r--  2.0 unx     1848 b- defN 23-Dec-30 14:55 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-30 14:55 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Dec-30 14:55 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1286 b- defN 23-Dec-30 14:55 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/RECORD
-11 files, 59092 bytes uncompressed, 51929 bytes compressed:  12.1%
+Zip file size: 54694 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1272 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/__init__.py
+-rw-r--r--  2.0 unx      543 b- defN 24-Apr-08 04:44 odoo/addons/ssi_transaction_ready_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      198 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/models/__init__.py
+-rw-r--r--  2.0 unx     7310 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx      804 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml
+-rw-r--r--  2.0 unx     1846 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1286 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/RECORD
+11 files, 61870 bytes uncompressed, 52394 bytes compressed:  15.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_transaction_ready_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_transaction_ready_mixin/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "Transaction Mixin - Ready to Process State",
-    "version": "14.0.1.6.0",
+    "version": "14.0.1.7.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [
         "ssi_transaction_mixin",
     ],
```

## odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py

```diff
@@ -1,14 +1,19 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 
+from inspect import getmembers
+
 from lxml import etree
 
-from odoo import api, fields, models
+from odoo import _, api, fields, models
+from odoo.exceptions import UserError
+
+from odoo.addons.ssi_decorator import ssi_decorator
 
 
 class MixinTransactionReady(models.AbstractModel):
     _name = "mixin.transaction_ready"
     _inherit = [
         "mixin.transaction",
     ]
@@ -48,17 +53,79 @@
         result = {
             "state": self._ready_state,
         }
         if self._create_sequence_state == self._ready_state:
             self._create_sequence()
         return result
 
+    def _run_pre_ready_check(self):
+        self.ensure_one()
+        cls = type(self)
+        methods = []
+        for _attr, func in getmembers(cls):
+            if self.is_decorator(func, "_pre_ready_check"):
+                methods.append(func)
+        if methods:
+            self.run_decorator_method(methods)
+
+    def _run_post_ready_check(self):
+        self.ensure_one()
+        cls = type(self)
+        methods = []
+        for _attr, func in getmembers(cls):
+            if self.is_decorator(func, "_post_ready_check"):
+                methods.append(func)
+        if methods:
+            self.run_decorator_method(methods)
+
+    def _run_pre_ready_action(self):
+        self.ensure_one()
+        cls = type(self)
+        methods = []
+        for _attr, func in getmembers(cls):
+            if self.is_decorator(func, "_pre_ready_action"):
+                methods.append(func)
+        if methods:
+            self.run_decorator_method(methods)
+
+    def _run_post_ready_action(self):
+        self.ensure_one()
+        cls = type(self)
+        methods = []
+        for _attr, func in getmembers(cls):
+            if self.is_decorator(func, "_post_ready_action"):
+                methods.append(func)
+        if methods:
+            self.run_decorator_method(methods)
+
     def action_ready(self):
         for record in self.sudo():
+            record._check_ready_policy()
+            record._run_pre_ready_check()
+            record._run_pre_ready_action()
             record.write(record._prepare_ready_data())
+            record._run_post_ready_check()
+            record._run_post_ready_action()
+
+    def _check_ready_policy(self):
+        self.ensure_one()
+        if self.env.context.get("bypass_ready_policy", False):
+            return True
+
+        if not self.ready_ok:
+            error_message = """
+            Context: Stage %s
+            Database ID: %s
+            Problem: Document is not allowed to stage
+            Solution: Check stage policy prerequisite
+            """ % (
+                self._description.lower(),
+                self.id,
+            )
+            raise UserError(_(error_message))
 
     @api.model
     def fields_view_get(
         self, view_id=None, view_type="form", toolbar=False, submenu=False
     ):
         result = super().fields_view_get(
             view_id=view_id, view_type=view_type, toolbar=toolbar, submenu=submenu
@@ -128,7 +195,18 @@
             view_arch = self._add_view_element(
                 view_arch,
                 "ssi_transaction_ready_mixin.button_ready",
                 "/form/header/field[@name='state']",
                 "before",
             )
         return view_arch
+
+    @ssi_decorator.insert_on_tree_view()
+    def _01_view_add_tree_ready_button(self, view_arch):
+        if self._automatically_insert_ready_button:
+            view_arch = self._add_view_element(
+                view_arch,
+                "ssi_transaction_ready_mixin.tree_button_ready",
+                "/tree/header",
+                "inside",
+            )
+        return view_arch
```

## odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml

### odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml

```diff
@@ -1,12 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <template id="ready_policy_field">
     <field name="ready_ok"/>
   </template>
   <template id="button_ready">
-    <button name="action_ready" string="Stage" type="object" class="oe_highlight" attrs="{'invisible':[('ready_ok','!=',True)]}"/>
+    <button name="action_ready" string="Stage" type="object" class="oe_highlight" attrs="{'invisible':[('ready_ok','!=',True)]}" confirm="Stage data. Are you sure?"/>
+  </template>
+  <template id="tree_button_ready">
+    <button name="action_ready" string="Stage" type="object" confirm="Stage data. Are you sure?"/>
   </template>
   <template id="ready_filter">
     <filter name="dom_ready" string="Ready to Process" domain="[('state', '=', 'ready')]"/>
   </template>
 </odoo>
```

## Comparing `odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/METADATA` & `odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-transaction-ready-mixin
-Version: 14.0.1.6.0
+Version: 14.0.1.7.0
 Summary: Transaction Mixin - Ready to Process State
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
 Requires-Dist: odoo14-addon-ssi-transaction-mixin
-Requires-Dist: odoo (<14.1dev,>=14.0a)
+Requires-Dist: odoo <14.1dev,>=14.0a
 
 .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
    :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
    :alt: License: AGPL-3
 
 ==========================================
 Transaction Mixin - Ready to Process State
```

## Comparing `odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/RECORD` & `odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/ssi_transaction_ready_mixin/README.rst,sha256=Q5zmi0IIuueW7CbBTomlXKXWbnM66bVGAqh-Lg6Ma1s,1272
 odoo/addons/ssi_transaction_ready_mixin/__init__.py,sha256=_euh7OtzMTDmyHY0E3tvYRWTi0ufnrMCH3IH8ZLtu0s,181
-odoo/addons/ssi_transaction_ready_mixin/__manifest__.py,sha256=YB79BSp7_RZV8i42_yvpwFNs-sNUJZA9AUfv3Hnj_Dc,543
+odoo/addons/ssi_transaction_ready_mixin/__manifest__.py,sha256=0nUgRu5qo_catDf6BiMSwSbG2r8_sqd6NrGpxqWNoAQ,543
 odoo/addons/ssi_transaction_ready_mixin/models/__init__.py,sha256=lOfO70jrUznLOmoFqDgf3m1pEV4Qij3s_sNFeGQulLA,198
-odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py,sha256=sDDo_ULJ3SEF8n7McklAlYV3UttlRZTIzgDM9icVHBI,4781
+odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py,sha256=k1DocbpZWUF_DgYmF-BeefM7I3I6mXoEoOXM4V3RibU,7310
 odoo/addons/ssi_transaction_ready_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml,sha256=ec4Y90ZLVayxia6Z-89Dg_eMQwcsTz3VfOoBwJ3WL6I,553
-odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/METADATA,sha256=q2Be8N1QqWBgtq3KCfF4FwFDkUCHztYSva0YQQKsmxw,1848
-odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_transaction_ready_mixin-14.0.1.6.0.dist-info/RECORD,,
+odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml,sha256=Ojf_LdJpD45bIRgd4bUf7J55hNNbtrCWGYrF8aEnyGY,804
+odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/METADATA,sha256=UyC2O2FS56PEFgBk4Y8mDGK6bfj_uXEwY3LlKz3S2Io,1846
+odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/RECORD,,
```

