# Comparing `tmp/alibabacloud_linkedmall20230930-2.1.2.tar.gz` & `tmp/alibabacloud_linkedmall20230930-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_linkedmall20230930-2.1.2.tar", last modified: Fri Mar 29 17:20:07 2024, max compression
+gzip compressed data, was "dist/alibabacloud_linkedmall20230930-2.1.3.tar", last modified: Mon Apr  8 04:23:55 2024, max compression
```

## Comparing `alibabacloud_linkedmall20230930-2.1.2.tar` & `alibabacloud_linkedmall20230930-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/
--rw-r--r--   0 root         (0) root         (0)      365 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2450 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1123 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1208 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63190 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930/client.py
--rw-r--r--   0 root         (0) root         (0)   157226 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2450 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2024-03-29 17:20:07.000000 alibabacloud_linkedmall20230930-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/
+-rw-r--r--   0 root         (0) root         (0)      454 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63190 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/client.py
+-rw-r--r--   0 root         (0) root         (0)   157477 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/setup.py
```

### Comparing `alibabacloud_linkedmall20230930-2.1.2/LICENSE` & `alibabacloud_linkedmall20230930-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.2/PKG-INFO` & `alibabacloud_linkedmall20230930-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_linkedmall20230930
-Version: 2.1.2
+Version: 2.1.3
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930-2.1.2/README-CN.md` & `alibabacloud_linkedmall20230930-2.1.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.2/README.md` & `alibabacloud_linkedmall20230930-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930/client.py` & `alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930/models.py` & `alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1781,14 +1781,15 @@
         fuzzy_quantity: str = None,
         mark_price: int = None,
         pic_url: str = None,
         platform_price: int = None,
         price: int = None,
         product_id: str = None,
         quantity: int = None,
+        rank_value: int = None,
         shop_id: str = None,
         sku_id: str = None,
         sku_specs: List[SkuSpec] = None,
         sku_specs_code: str = None,
         sku_status: str = None,
         title: str = None,
     ):
@@ -1798,14 +1799,15 @@
         self.fuzzy_quantity = fuzzy_quantity
         self.mark_price = mark_price
         self.pic_url = pic_url
         self.platform_price = platform_price
         self.price = price
         self.product_id = product_id
         self.quantity = quantity
+        self.rank_value = rank_value
         self.shop_id = shop_id
         self.sku_id = sku_id
         self.sku_specs = sku_specs
         self.sku_specs_code = sku_specs_code
         self.sku_status = sku_status
         self.title = title
 
@@ -1837,14 +1839,16 @@
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
@@ -1875,14 +1879,16 @@
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

### Comparing `alibabacloud_linkedmall20230930-2.1.2/alibabacloud_linkedmall20230930.egg-info/PKG-INFO` & `alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-linkedmall20230930
-Version: 2.1.2
+Version: 2.1.3
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930-2.1.2/setup.py` & `alibabacloud_linkedmall20230930-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_linkedmall20230930.
 
-Created on 29/03/2024
+Created on 08/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_linkedmall20230930"
 NAME = "alibabacloud_linkedmall20230930" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud linkedmall (20230930) SDK Library for Python"
```

