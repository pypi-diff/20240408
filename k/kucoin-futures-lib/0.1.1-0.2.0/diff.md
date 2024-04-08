# Comparing `tmp/kucoin_futures_lib-0.1.1.tar.gz` & `tmp/kucoin_futures_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kucoin_futures_lib-0.1.1.tar", max compression
+gzip compressed data, was "kucoin_futures_lib-0.2.0.tar", max compression
```

## Comparing `kucoin_futures_lib-0.1.1.tar` & `kucoin_futures_lib-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/LICENSE
--rw-r--r--   0        0        0       52 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/README.md
--rw-r--r--   0        0        0      719 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/__init__.py
--rw-r--r--   0        0        0     2329 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/factory.py
--rw-r--r--   0        0        0      251 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/__init__.py
--rw-r--r--   0        0        0      961 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/base.py
--rw-r--r--   0        0        0     1920 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/entry.py
--rw-r--r--   0        0        0     2508 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/oco.py
--rw-r--r--   0        0        0     1419 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/helper.py
--rw-r--r--   0        0        0     2464 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/kucoinf.py
--rw-r--r--   0        0        0     3117 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/market.py
--rw-r--r--   0        0        0    12864 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/trade.py
--rw-r--r--   0        0        0     1068 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/user.py
--rw-r--r--   0        0        0     2732 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/websocket.py
--rw-r--r--   0        0        0      455 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/LICENSE
+-rw-r--r--   0        0        0       52 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/README.md
+-rw-r--r--   0        0        0      719 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/factory.py
+-rw-r--r--   0        0        0      251 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/base.py
+-rw-r--r--   0        0        0     1920 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/entry.py
+-rw-r--r--   0        0        0     2499 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/oco.py
+-rw-r--r--   0        0        0     1419 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/helper.py
+-rw-r--r--   0        0        0     2464 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/kucoinf.py
+-rw-r--r--   0        0        0     3117 2024-04-08 18:45:50.316869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/market.py
+-rw-r--r--   0        0        0    12864 2024-04-08 18:45:50.316869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/trade.py
+-rw-r--r--   0        0        0     1068 2024-04-08 18:45:50.316869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/user.py
+-rw-r--r--   0        0        0     2732 2024-04-08 18:45:50.316869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/websocket.py
+-rw-r--r--   0        0        0      455 2024-04-08 18:45:50.316869 kucoin_futures_lib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.2.0/PKG-INFO
```

### Comparing `kucoin_futures_lib-0.1.1/LICENSE` & `kucoin_futures_lib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.1/kucoin_futures_lib/__init__.py` & `kucoin_futures_lib-0.2.0/kucoin_futures_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.1/kucoin_futures_lib/factory.py` & `kucoin_futures_lib-0.2.0/kucoin_futures_lib/factory.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/base.py` & `kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/entry.py` & `kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/entry.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/oco.py` & `kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/oco.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,22 +47,23 @@
     async def handle(self, msg: Dict):
         """Handle the trade order message from
         :param msg: The trade order message.
         https://www.kucoin.com/docs/websocket/futures-trading/private-channels/trade-orders
         """
         trade_order = msg.get("data", {})
         order_id = trade_order.get("orderId", "")
-        message_type = trade_order.get("type", "")
+        status = trade_order.get("status", "")
 
-        if order_id == self.limit_order_id and message_type == "filled":
-            logger.info("Limit order %s is done.", self.limit_order_id)
-            await self.cancel_order(self.market_order_id)
-        elif order_id == self.market_order_id and message_type == "filled":
-            logger.info("Market order %s is done.", self.market_order_id)
-            self._canceled.set()
+        if status == "done":
+            if order_id == self.limit_order_id:
+                logger.info("Limit order %s is done.", self.limit_order_id)
+                await self.cancel_order(self.market_order_id)
+            elif order_id == self.market_order_id:
+                logger.info("Market order %s is done.", self.market_order_id)
+                self._canceled.set()
 
     async def cancel_order(self, order_id: str) -> None:
         """Cancel the order based on its type (sync or async)."""
         if inspect.isawaitable(self._cancel_order) or isinstance(
             self._cancel_order, AsyncMock  # For testing
         ):
             await self._cancel_order(order_id)
```

### Comparing `kucoin_futures_lib-0.1.1/kucoin_futures_lib/helper.py` & `kucoin_futures_lib-0.2.0/kucoin_futures_lib/helper.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.1/kucoin_futures_lib/kucoinf.py` & `kucoin_futures_lib-0.2.0/kucoin_futures_lib/kucoinf.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.1/kucoin_futures_lib/market.py` & `kucoin_futures_lib-0.2.0/kucoin_futures_lib/market.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.1/kucoin_futures_lib/trade.py` & `kucoin_futures_lib-0.2.0/kucoin_futures_lib/trade.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.1/kucoin_futures_lib/user.py` & `kucoin_futures_lib-0.2.0/kucoin_futures_lib/user.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.1/kucoin_futures_lib/websocket.py` & `kucoin_futures_lib-0.2.0/kucoin_futures_lib/websocket.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.1/PKG-INFO` & `kucoin_futures_lib-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kucoin-futures-lib
-Version: 0.1.1
+Version: 0.2.0
 Summary: Kucoin Futures wrapper library
 License: Apache-2.0
 Author: Evgeny Aleshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

