# Comparing `tmp/easy_kite_methods-0.0.2.tar.gz` & `tmp/easy_kite_methods-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_kite_methods-0.0.2.tar", max compression
+gzip compressed data, was "easy_kite_methods-0.0.3.tar", max compression
```

## Comparing `easy_kite_methods-0.0.2.tar` & `easy_kite_methods-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3025 2024-04-08 06:23:56.009908 easy_kite_methods-0.0.2/README.md
--rw-r--r--   0        0        0      510 2024-04-08 06:19:05.831494 easy_kite_methods-0.0.2/easy_kite_methods/__init__.py
--rw-r--r--   0        0        0     1627 2024-04-08 05:46:27.884702 easy_kite_methods-0.0.2/easy_kite_methods/kite_login.py
--rw-r--r--   0        0        0     8196 2024-04-08 06:19:05.832632 easy_kite_methods-0.0.2/easy_kite_methods/order_placement.py
--rw-r--r--   0        0        0      555 2024-04-08 06:25:04.114956 easy_kite_methods-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3645 1970-01-01 00:00:00.000000 easy_kite_methods-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3640 2024-04-08 09:17:23.806185 easy_kite_methods-0.0.3/README.md
+-rw-r--r--   0        0        0      510 2024-04-08 06:19:05.831494 easy_kite_methods-0.0.3/easy_kite_methods/__init__.py
+-rw-r--r--   0        0        0     1627 2024-04-08 05:46:27.884702 easy_kite_methods-0.0.3/easy_kite_methods/kite_login.py
+-rw-r--r--   0        0        0     9773 2024-04-08 09:17:23.807237 easy_kite_methods-0.0.3/easy_kite_methods/order_placement.py
+-rw-r--r--   0        0        0      555 2024-04-08 09:20:43.857391 easy_kite_methods-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 easy_kite_methods-0.0.3/PKG-INFO
```

### Comparing `easy_kite_methods-0.0.2/easy_kite_methods/kite_login.py` & `easy_kite_methods-0.0.3/easy_kite_methods/kite_login.py`

 * *Files identical despite different names*

### Comparing `easy_kite_methods-0.0.2/easy_kite_methods/order_placement.py` & `easy_kite_methods-0.0.3/easy_kite_methods/order_placement.py`

 * *Files 17% similar despite different names*

```diff
@@ -131,52 +131,106 @@
                                 order_type=kite.ORDER_TYPE_MARKET)
     return order_id
 
 
 def modify_order_quantity(variety, order_id, quantity):
     """
     order_id : This is the id of order executed
-    variety : Variety can be [VARIETY_AMO 
-                            VARIETY_REGULAR ]
+    variety : Variety can be [AMO ,REGULAR , BO,CO]
     quantity : Total number of orders                        
     """
-    order_id = kite.modify_order(variety=variety, order_id=order_id,
+
+    if variety.upper() is "REGULAR" :
+         order_id = kite.modify_order(variety=kite.VARIETY_REGULAR, order_id=order_id,
                                  quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
     return order_id
 
+    if variety.upper() is "CO" :
+         order_id = kite.modify_order(variety=kite.VARIETY_CO, order_id=order_id,
+                                 quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
+    return order_id
+
+     if variety.upper() is "AMO" :
+         order_id = kite.modify_order(variety=kite.VARIETY_AMO, order_id=order_id,
+                                 quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
+    return order_id
+
+     if variety.upper() is "BO" :
+         order_id = kite.modify_order(variety=kite.VARIETY_BO, order_id=order_id,
+                                 quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
+    return order_id
+
+      
+
 
 def modify_order_price(variety, order_id, price):
     """
     order_id : This is the id of order executed
     variety : Variety can be [VARIETY_AMO 
                             VARIETY_REGULAR ]
     price : Modified price of order                      
     """
+    if variety.upper() is "REGULAR" :
+         variety = kite.VARIETY_REGULAR
+
+    if variety.upper() is "CO" :
+         variety = kite.VARIETY_CO
+  
+    if variety.upper() is "AMO" :
+        variety = kite.VARIETY_AMO
+
+     if variety.upper() is "BO" :
+        variety = kite.VARIETY_BO
+         
     order_id = kite.modify_order(variety=variety, order_id=order_id,
                                  price=price, order_type=kite.ORDER_TYPE_MARKET)
     return order_id
 
 
 def modify_order_to_sell(variety, order_id):
     """
     order_id : This is the id of order executed
     variety : Variety can be [VARIETY_AMO 
                             VARIETY_REGULAR ]                    
     """
+    if variety.upper() is "REGULAR" :
+         variety = kite.VARIETY_REGULAR
+
+    if variety.upper() is "CO" :
+         variety = kite.VARIETY_CO
+  
+    if variety.upper() is "AMO" :
+        variety = kite.VARIETY_AMO
+
+     if variety.upper() is "BO" :
+        variety = kite.VARIETY_BO
+
     order_id = kite.modify_order(
         variety=variety, order_id=order_id, order_type=kite.TRANSACTION_TYPE_SELL)
     return order_id
 
 
 def modify_order_to_buy(variety, order_id):
     """
     order_id : This is the id of order executed
     variety : Variety can be [VARIETY_AMO 
                             VARIETY_REGULAR ]                    
     """
+    if variety.upper() is "REGULAR" :
+         variety = kite.VARIETY_REGULAR
+
+    if variety.upper() is "CO" :
+         variety = kite.VARIETY_CO
+  
+    if variety.upper() is "AMO" :
+        variety = kite.VARIETY_AMO
+
+     if variety.upper() is "BO" :
+        variety = kite.VARIETY_BO
+
     order_id = kite.modify_order(
         variety=variety, order_id=order_id, order_type=kite.TRANSACTION_TYPE_BUY)
     return order_id
 
 
 def get_holdings():
     return kite.holdings()
```

### Comparing `easy_kite_methods-0.0.2/pyproject.toml` & `easy_kite_methods-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_kite_methods"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Vivek Patel <vivekkvhpatel@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 kiteconnect = "^5.0.1"
```

