# Comparing `tmp/exchanges_wrapper-2.1.7.tar.gz` & `tmp/exchanges_wrapper-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges_wrapper-2.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "exchanges_wrapper-2.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `exchanges_wrapper-2.1.7.tar` & `exchanges_wrapper-2.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1114 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/LICENSE.md
--rw-r--r--   0        0        0     7003 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/README.md
--rwxr-xr-x   0        0        0     1516 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    19230 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0    15978 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/bybit_parser.py
--rw-r--r--   0        0        0    78029 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2768 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12512 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    36432 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     5597 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    13216 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    14390 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/huobi_parser.py
--rwxr-xr-x   0        0        0     2500 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/lib.py
--rw-r--r--   0        0        0    53745 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/martin/__init__.py
--rw-r--r--   0        0        0    16228 2024-04-03 15:41:45.792099 exchanges_wrapper-2.1.7/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    10683 2024-04-03 15:41:45.796099 exchanges_wrapper-2.1.7/exchanges_wrapper/proto/martin.proto
--rw-r--r--   0        0        0    27723 2024-04-03 15:41:45.796099 exchanges_wrapper-2.1.7/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0     1227 2024-04-03 15:41:45.796099 exchanges_wrapper-2.1.7/pyproject.toml
--rw-r--r--   0        0        0     8020 1970-01-01 00:00:00.000000 exchanges_wrapper-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-04-08 17:59:39.823769 exchanges_wrapper-2.1.8/LICENSE.md
+-rw-r--r--   0        0        0     7003 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/README.md
+-rwxr-xr-x   0        0        0     1516 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    78383 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2768 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12512 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    36649 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     5597 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    13216 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/http_client.py
+-rwxr-xr-x   0        0        0     2500 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/lib.py
+-rw-r--r--   0        0        0    53745 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/martin/__init__.py
+-rw-r--r--   0        0        0    19230 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/bitfinex_parser.py
+-rw-r--r--   0        0        0    16028 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/bybit_parser.py
+-rw-r--r--   0        0        0    14390 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/huobi_parser.py
+-rw-r--r--   0        0        0    16228 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/okx_parser.py
+-rw-r--r--   0        0        0    10683 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/proto/martin.proto
+-rw-r--r--   0        0        0    27755 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0     1227 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0     8020 1970-01-01 00:00:00.000000 exchanges_wrapper-2.1.8/PKG-INFO
```

### Comparing `exchanges_wrapper-2.1.7/LICENSE.md` & `exchanges_wrapper-2.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/README.md` & `exchanges_wrapper-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/__init__.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "2.1.7"
+__version__ = "2.1.8"
 
 from pathlib import Path
 import shutil
 
 from grpclib.server import Server, GRPCError, Status
 from grpclib.client import Channel
 from grpclib.utils import graceful_exit
```

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/bitfinex_parser.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/bitfinex_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/bybit_parser.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/bybit_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,15 +370,20 @@
     cumulative_filled_quantity = res.get("cumExecQty", str(order_quantity - leaves_qty))
     cumulative_quote_asset = res.get("cumExecValue", str(Decimal(cumulative_filled_quantity) * order_price))
 
     last_executed_quantity = res.get("execQty", cumulative_filled_quantity)
     last_executed_price = res.get("execPrice", res.get("avgPrice"))
     last_quote_asset_transacted = res.get("execValue", cumulative_quote_asset)
 
-    status = 'NEW' if leaves_qty == order_quantity else 'PARTIALLY_FILLED' if leaves_qty > 0 else 'FILLED'
+    if leaves_qty == order_quantity:
+        status = 'NEW'
+    elif leaves_qty > 0:
+        status = 'PARTIALLY_FILLED'
+    else:
+        status = 'FILLED'
 
     return {
         "e": "executionReport",
         "E": int(res.get("execTime", res.get("updatedTime"))),
         "s": res["symbol"],
         "c": res["orderLinkId"],
         "S": res["side"].upper(),
```

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/client.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     MarketEventsDataStream, \
     BfxPrivateEventsDataStream, \
     HbpPrivateEventsDataStream, \
     OkxPrivateEventsDataStream, \
     BBTPrivateEventsDataStream
 from exchanges_wrapper.definitions import OrderType
 from exchanges_wrapper.events import Events
-import exchanges_wrapper.bitfinex_parser as bfx
-import exchanges_wrapper.huobi_parser as hbp
-import exchanges_wrapper.okx_parser as okx
-import exchanges_wrapper.bybit_parser as bbt
+import exchanges_wrapper.parsers.bitfinex_parser as bfx
+import exchanges_wrapper.parsers.huobi_parser as hbp
+import exchanges_wrapper.parsers.okx_parser as okx
+import exchanges_wrapper.parsers.bybit_parser as bbt
 from crypto_ws_api.ws_session import UserWSSession
 
 logger = logging.getLogger(__name__)
 
 STATUS_TIMEOUT = 5  # sec, also use for lifetime limit for inactive order (Bitfinex) as 60 * STATUS_TIMEOUT
 
 
@@ -113,14 +113,15 @@
         res = None
         while res is None:
             await asyncio.sleep(0.05)
             res = self.wss_buffer.pop(key, None)
         return res
 
     async def load(self, symbol):
+        logger.info(f"Try load {self.exchange}:{symbol} info...")
         infos = await self.fetch_exchange_info(symbol)
         if not infos.get('serverTime'):
             raise UserWarning("Can't get exchange info, check availability and operational status of the exchange")
         self.ts_start[symbol] = int(time.time() * 1000)
         # load available symbols
         self.highest_precision = 8
         original_symbol_infos = infos["symbols"]
@@ -140,14 +141,15 @@
             if self.main_account_uid == '0':
                 logger.info(f"It is main ByBit account, UID: {self.account_uid}")
             else:
                 logger.info(f"Main ByBit account UID: {self.main_account_uid}, sub-UID: {self.account_uid}")
         # load rate limits
         self.rate_limits = infos["rateLimits"]
         self.loaded = True
+        logger.info(f"Info for {self.exchange}:{symbol} loaded success")
 
     async def close(self):
         await self.session.close()
 
     @property
     def events(self):
         if not hasattr(self, "_events"):
@@ -1173,26 +1175,27 @@
                         signed=True,
                     )
             )
         elif self.exchange == 'bitfinex':
             orders = await self.fetch_open_orders(trade_id, symbol, receive_window=receive_window, response_type=True)
             orders_id = [order.get('orderId') for order in orders]
             params = {'id': orders_id}
-            res = (
-                    await self.user_wss_session.handle_request(trade_id, "oc_multi", _params=params)
-                    or await self.http.send_api_call(
+            res = await self.user_wss_session.handle_request(trade_id, "oc_multi", _params=params)
+            if res is None or (res and isinstance(res, list) and res[6] == 'ERROR'):
+                logger.debug(f"cancel_all_orders.bitfinex {orders_id}: res1: {res}")
+                res = await self.http.send_api_call(
                         "v2/auth/w/order/cancel/multi",
                         method="POST",
                         signed=True,
-                        **params,
-                    )
-            )
-            if res and res[6] == 'SUCCESS':
-                return bfx.orders(res[4], response_type=True, cancelled=True)
-            logger.debug(f"bitfinex: cancel_all_orders.res: {res}")
+                        **params
+                )
+            if res and isinstance(res, list) and res[6] == 'SUCCESS':
+                binance_res = bfx.orders(res[4], response_type=True, cancelled=True)
+            else:
+                logger.debug(f"bitfinex: cancel_all_orders.res: {res}")
 
         elif self.exchange == 'huobi':
             orders = await self.fetch_open_orders(trade_id, symbol, receive_window=receive_window, response_type=True)
             orders_id = [str(order.get('orderId')) for order in orders]
             params = {'order-ids': orders_id}
             res = await self.http.send_api_call(
                 "v1/order/orders/batchcancel",
```

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/definitions.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/definitions.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/errors.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/events.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/exch_srv.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/exch_srv.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,17 +156,19 @@
                 sleep_duration = rate_limit_interval - ts_diff
                 await asyncio.sleep(sleep_duration)
 
     async def open_client_connection(self, request: mr.OpenClientConnectionRequest) -> mr.OpenClientConnectionId:
         logger.info(f"OpenClientConnection start trade: {request.account_name}:{request.trade_id}")
         client_id = OpenClient.get_id(request.account_name)
         if client_id:
+            logger.debug(f"OpenClientConnection: {request.account_name}:{request.trade_id}:{client_id}")
             open_client = OpenClient.get_client(client_id)
             open_client.client.http.rate_limit_reached = False
         else:
+            logger.debug(f"OpenClientConnection: {request.account_name}:{request.trade_id}: set new client_id")
             try:
                 open_client = OpenClient(request.account_name)
                 client_id = id(open_client)
                 if open_client.client.master_name == 'Huobi':
                     # For HuobiPro get master account uid and account_id
                     main_account = get_account(open_client.client.master_name)
                     main_client = Client(*main_account)
```

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges_wrapper-2.1.8/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/http_client.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/http_client.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/huobi_parser.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/huobi_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/lib.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/lib.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/martin/__init__.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/martin/__init__.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/okx_parser.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/okx_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/proto/martin.proto` & `exchanges_wrapper-2.1.8/exchanges_wrapper/proto/martin.proto`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/exchanges_wrapper/web_sockets.py` & `exchanges_wrapper-2.1.8/exchanges_wrapper/web_sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import time
 from decimal import Decimal
 import gzip
 from datetime import datetime, timezone
 from urllib.parse import urlencode, urlparse
 import websockets
 
-import exchanges_wrapper.bitfinex_parser as bfx
-import exchanges_wrapper.huobi_parser as hbp
-import exchanges_wrapper.okx_parser as okx
-import exchanges_wrapper.bybit_parser as bbt
+import exchanges_wrapper.parsers.bitfinex_parser as bfx
+import exchanges_wrapper.parsers.huobi_parser as hbp
+import exchanges_wrapper.parsers.okx_parser as okx
+import exchanges_wrapper.parsers.bybit_parser as bbt
 from crypto_ws_api.ws_session import generate_signature
 from exchanges_wrapper import LOG_PATH
 
 logger = logging.getLogger('exch_srv_logger')
 
 logger_ws = logging.getLogger(__name__)
 logger_ws.level = logging.INFO
```

### Comparing `exchanges_wrapper-2.1.7/pyproject.toml` & `exchanges_wrapper-2.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.7/PKG-INFO` & `exchanges_wrapper-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 2.1.7
+Version: 2.1.8
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 2.1.7 Summary: REST API
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 2.1.8 Summary: REST API
 and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
 email: Thomas Marchand
 tuta.io>, Jerry Fedorenko
 yahoo.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
```

