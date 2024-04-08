# Comparing `tmp/alibabacloud_linkedmall20230930_py2-2.1.2.tar.gz` & `tmp/alibabacloud_linkedmall20230930_py2-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_linkedmall20230930_py2-2.1.2.tar", last modified: Fri Mar 29 17:27:46 2024, max compression
+gzip compressed data, was "dist/alibabacloud_linkedmall20230930_py2-2.1.3.tar", last modified: Mon Apr  8 04:23:49 2024, max compression
```

## Comparing `alibabacloud_linkedmall20230930_py2-2.1.2.tar` & `alibabacloud_linkedmall20230930_py2-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/
--rw-r--r--   0 root         (0) root         (0)      370 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2514 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1054 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27155 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930/client.py
--rw-r--r--   0 root         (0) root         (0)   157159 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2514 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2938 2024-03-29 17:27:46.000000 alibabacloud_linkedmall20230930_py2-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/
+-rw-r--r--   0 root         (0) root         (0)      548 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27155 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930/client.py
+-rw-r--r--   0 root         (0) root         (0)   157409 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2938 2024-04-08 04:23:49.000000 alibabacloud_linkedmall20230930_py2-2.1.3/setup.py
```

### Comparing `alibabacloud_linkedmall20230930_py2-2.1.2/LICENSE` & `alibabacloud_linkedmall20230930_py2-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930_py2-2.1.2/PKG-INFO` & `alibabacloud_linkedmall20230930_py2-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_linkedmall20230930_py2
-Version: 2.1.2
+Version: 2.1.3
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930_py2-2.1.2/README-CN.md` & `alibabacloud_linkedmall20230930_py2-2.1.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930_py2-2.1.2/README.md` & `alibabacloud_linkedmall20230930_py2-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930/client.py` & `alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930/models.py` & `alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2851,26 +2851,27 @@
         if m.get('total') is not None:
             self.total = m.get('total')
         return self
 
 
 class Sku(TeaModel):
     def __init__(self, barcode=None, can_sell=None, division_code=None, fuzzy_quantity=None, mark_price=None,
-                 pic_url=None, platform_price=None, price=None, product_id=None, quantity=None, shop_id=None, sku_id=None,
-                 sku_specs=None, sku_specs_code=None, sku_status=None, title=None):
+                 pic_url=None, platform_price=None, price=None, product_id=None, quantity=None, rank_value=None,
+                 shop_id=None, sku_id=None, sku_specs=None, sku_specs_code=None, sku_status=None, title=None):
         self.barcode = barcode  # type: str
         self.can_sell = can_sell  # type: bool
         self.division_code = division_code  # type: str
         self.fuzzy_quantity = fuzzy_quantity  # type: str
         self.mark_price = mark_price  # type: long
         self.pic_url = pic_url  # type: str
         self.platform_price = platform_price  # type: long
         self.price = price  # type: long
         self.product_id = product_id  # type: str
         self.quantity = quantity  # type: long
+        self.rank_value = rank_value  # type: long
         self.shop_id = shop_id  # type: str
         self.sku_id = sku_id  # type: str
         self.sku_specs = sku_specs  # type: list[SkuSpec]
         self.sku_specs_code = sku_specs_code  # type: str
         self.sku_status = sku_status  # type: str
         self.title = title  # type: str
 
@@ -2902,14 +2903,16 @@
             result['platformPrice'] = self.platform_price
         if self.price is not None:
             result['price'] = self.price
         if self.product_id is not None:
             result['productId'] = self.product_id
         if self.quantity is not None:
             result['quantity'] = self.quantity
+        if self.rank_value is not None:
+            result['rankValue'] = self.rank_value
         if self.shop_id is not None:
             result['shopId'] = self.shop_id
         if self.sku_id is not None:
             result['skuId'] = self.sku_id
         result['skuSpecs'] = []
         if self.sku_specs is not None:
             for k in self.sku_specs:
@@ -2940,14 +2943,16 @@
             self.platform_price = m.get('platformPrice')
         if m.get('price') is not None:
             self.price = m.get('price')
         if m.get('productId') is not None:
             self.product_id = m.get('productId')
         if m.get('quantity') is not None:
             self.quantity = m.get('quantity')
+        if m.get('rankValue') is not None:
+            self.rank_value = m.get('rankValue')
         if m.get('shopId') is not None:
             self.shop_id = m.get('shopId')
         if m.get('skuId') is not None:
             self.sku_id = m.get('skuId')
         self.sku_specs = []
         if m.get('skuSpecs') is not None:
             for k in m.get('skuSpecs'):
```

### Comparing `alibabacloud_linkedmall20230930_py2-2.1.2/alibabacloud_linkedmall20230930_py2.egg-info/PKG-INFO` & `alibabacloud_linkedmall20230930_py2-2.1.3/alibabacloud_linkedmall20230930_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-linkedmall20230930-py2
-Version: 2.1.2
+Version: 2.1.3
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930_py2-2.1.2/setup.py` & `alibabacloud_linkedmall20230930_py2-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_linkedmall20230930_py2.
 
-Created on 29/03/2024
+Created on 08/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_linkedmall20230930"
 NAME = "alibabacloud_linkedmall20230930_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud linkedmall (20230930) SDK Library for Python2"
```

