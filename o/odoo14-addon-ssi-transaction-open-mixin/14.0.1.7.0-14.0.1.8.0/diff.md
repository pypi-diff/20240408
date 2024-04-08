# Comparing `tmp/odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 54357 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1256 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_open_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_open_mixin/__init__.py
--rw-r--r--  2.0 unx      537 b- defN 23-Dec-30 14:53 odoo/addons/ssi_transaction_open_mixin/__manifest__.py
--rw-r--r--  2.0 unx      197 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_open_mixin/models/__init__.py
--rw-r--r--  2.0 unx     6205 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_open_mixin/models/mixin_transaction_open.py
--rw-r--r--  2.0 unx    48333 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_open_mixin/static/description/icon.png
--rw-r--r--  2.0 unx      496 b- defN 23-Dec-30 14:51 odoo/addons/ssi_transaction_open_mixin/templates/mixin_transaction_open_templates.xml
--rw-r--r--  2.0 unx     1826 b- defN 23-Dec-30 14:56 odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-30 14:56 odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Dec-30 14:56 odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1273 b- defN 23-Dec-30 14:56 odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/RECORD
-11 files, 60401 bytes uncompressed, 52083 bytes compressed:  13.8%
+Zip file size: 54640 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1256 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/__init__.py
+-rw-r--r--  2.0 unx      537 b- defN 24-Apr-08 04:44 odoo/addons/ssi_transaction_open_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      197 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/models/__init__.py
+-rw-r--r--  2.0 unx     7266 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/models/mixin_transaction_open.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx      697 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_open_mixin/templates/mixin_transaction_open_templates.xml
+-rw-r--r--  2.0 unx     1824 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1273 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/RECORD
+11 files, 61661 bytes uncompressed, 52366 bytes compressed:  15.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_transaction_open_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_transaction_open_mixin/templates/mixin_transaction_open_templates.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_transaction_open_mixin/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "Transaction Mixin - In Progress State",
-    "version": "14.0.1.7.0",
+    "version": "14.0.1.8.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [
         "ssi_transaction_mixin",
     ],
```

## odoo/addons/ssi_transaction_open_mixin/models/mixin_transaction_open.py

```diff
@@ -2,15 +2,18 @@
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 
 from inspect import getmembers
 
 from lxml import etree
 
-from odoo import api, fields, models
+from odoo import _, api, fields, models
+from odoo.exceptions import UserError
+
+from odoo.addons.ssi_decorator import ssi_decorator
 
 
 class MixinTransactionOpen(models.AbstractModel):
     _name = "mixin.transaction_open"
     _inherit = [
         "mixin.transaction",
     ]
@@ -92,20 +95,38 @@
             if self.is_decorator(func, "_post_open_action"):
                 methods.append(func)
         if methods:
             self.run_decorator_method(methods)
 
     def action_open(self):
         for record in self.sudo():
+            record._check_open_policy()
             record._run_pre_open_check()
             record._run_pre_open_action()
             record.write(record._prepare_open_data())
             record._run_post_open_check()
             record._run_post_open_action()
 
+    def _check_open_policy(self):
+        self.ensure_one()
+        if self.env.context.get("bypass_open_policy", False):
+            return True
+
+        if not self.open_ok:
+            error_message = """
+                Context: Start %s
+                Database ID: %s
+                Problem: Document is not allowed to start
+                Solution: Check start policy prerequisite
+                """ % (
+                self._description.lower(),
+                self.id,
+            )
+            raise UserError(_(error_message))
+
     @api.model
     def fields_view_get(
         self, view_id=None, view_type="form", toolbar=False, submenu=False
     ):
         result = super().fields_view_get(
             view_id=view_id, view_type=view_type, toolbar=toolbar, submenu=submenu
         )
@@ -174,7 +195,18 @@
             view_arch = self._add_view_element(
                 view_arch,
                 "ssi_transaction_open_mixin.open_filter",
                 self._state_filter_xpath,
                 "after",
             )
         return view_arch
+
+    @ssi_decorator.insert_on_tree_view()
+    def _01_view_add_tree_open_button(self, view_arch):
+        if self._automatically_insert_open_button:
+            view_arch = self._add_view_element(
+                view_arch,
+                "ssi_transaction_open_mixin.tree_button_open",
+                "/tree/header",
+                "inside",
+            )
+        return view_arch
```

## odoo/addons/ssi_transaction_open_mixin/templates/mixin_transaction_open_templates.xml

### odoo/addons/ssi_transaction_open_mixin/templates/mixin_transaction_open_templates.xml

```diff
@@ -2,11 +2,14 @@
 <odoo>
   <template id="open_policy_field">
     <field name="open_ok"/>
   </template>
   <template id="button_open">
     <button name="action_open" string="Start" type="object" class="oe_highlight" attrs="{'invisible':[('open_ok','!=',True)]}"/>
   </template>
+  <template id="tree_button_open">
+    <button name="action_open" string="Start" type="object" confirm="Start data. Are you sure?"/>
+  </template>
   <template id="open_filter">
     <filter name="dom_open" string="In Progress" domain="[('state', '=', 'open')]"/>
   </template>
 </odoo>
```

## Comparing `odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/METADATA` & `odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-transaction-open-mixin
-Version: 14.0.1.7.0
+Version: 14.0.1.8.0
 Summary: Transaction Mixin - In Progress State
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
 
 =====================================
 Transaction Mixin - In Progress State
```

## Comparing `odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/RECORD` & `odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/ssi_transaction_open_mixin/README.rst,sha256=LsaB-c6GP16LpNgw-0pN-2ylD3Q_d3TCg6dHy79wuB8,1256
 odoo/addons/ssi_transaction_open_mixin/__init__.py,sha256=_euh7OtzMTDmyHY0E3tvYRWTi0ufnrMCH3IH8ZLtu0s,181
-odoo/addons/ssi_transaction_open_mixin/__manifest__.py,sha256=7CzGQXGW8ZEzA4sNf7Q6reYM8k07VTNcEJC8lddcdxY,537
+odoo/addons/ssi_transaction_open_mixin/__manifest__.py,sha256=Hpp9IYzGPWRj62fNEsuMd-1PmCck8xoE9BD8LBDPapM,537
 odoo/addons/ssi_transaction_open_mixin/models/__init__.py,sha256=9Xi4MfyVO72dwQ8dVtgQqU2p4Q6v4223KpaiAf3pS3o,197
-odoo/addons/ssi_transaction_open_mixin/models/mixin_transaction_open.py,sha256=wxLFg8nWshI9NwJ6ijnUz2R8zrAeY7QHDBjiO6RnIDo,6205
+odoo/addons/ssi_transaction_open_mixin/models/mixin_transaction_open.py,sha256=qrZoNTzO7ZDFZ0mtNuLCehkkVrq-21CmX366COML71I,7266
 odoo/addons/ssi_transaction_open_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo/addons/ssi_transaction_open_mixin/templates/mixin_transaction_open_templates.xml,sha256=jvvM_PryBC15uyehRHHYaaoDr-KA228INOZ3GQknc4g,496
-odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/METADATA,sha256=rmx2z61QvHcVUNIuaxhLdgx_8_e8_ooV0ikJVw6I600,1826
-odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_transaction_open_mixin-14.0.1.7.0.dist-info/RECORD,,
+odoo/addons/ssi_transaction_open_mixin/templates/mixin_transaction_open_templates.xml,sha256=hjtYoBYPwswPncZPs4s9SqszrHZuC64BhTYgQ4McBso,697
+odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/METADATA,sha256=MkjJFQyGtzf7SfcwN_V6RhU0g9rd6Uo_tVhAKOpbq_E,1824
+odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_transaction_open_mixin-14.0.1.8.0.dist-info/RECORD,,
```

