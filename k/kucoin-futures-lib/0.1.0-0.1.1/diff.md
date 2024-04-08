# Comparing `tmp/kucoin_futures_lib-0.1.0.tar.gz` & `tmp/kucoin_futures_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kucoin_futures_lib-0.1.0.tar", max compression
+gzip compressed data, was "kucoin_futures_lib-0.1.1.tar", max compression
```

## Comparing `kucoin_futures_lib-0.1.0.tar` & `kucoin_futures_lib-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-04-07 23:11:35.277519 kucoin_futures_lib-0.1.0/LICENSE
--rw-r--r--   0        0        0       52 2024-04-07 23:11:35.277519 kucoin_futures_lib-0.1.0/README.md
--rw-r--r--   0        0        0      719 2024-04-07 23:11:35.277519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/__init__.py
--rw-r--r--   0        0        0     2326 2024-04-07 23:11:35.277519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/factory.py
--rw-r--r--   0        0        0      327 2024-04-07 23:11:35.277519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/handlers/__init__.py
--rw-r--r--   0        0        0      961 2024-04-07 23:11:35.277519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/handlers/base.py
--rw-r--r--   0        0        0     1920 2024-04-07 23:11:35.277519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/handlers/entry.py
--rw-r--r--   0        0        0     1378 2024-04-07 23:11:35.277519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/handlers/fill.py
--rw-r--r--   0        0        0     2508 2024-04-07 23:11:35.277519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/handlers/oco.py
--rw-r--r--   0        0        0     1419 2024-04-07 23:11:35.277519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/helper.py
--rw-r--r--   0        0        0     2470 2024-04-07 23:11:35.277519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/kucoinf.py
--rw-r--r--   0        0        0     3117 2024-04-07 23:11:35.281519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/market.py
--rw-r--r--   0        0        0    12851 2024-04-07 23:11:35.281519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/trade.py
--rw-r--r--   0        0        0     1060 2024-04-07 23:11:35.281519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/user.py
--rw-r--r--   0        0        0     3120 2024-04-07 23:11:35.281519 kucoin_futures_lib-0.1.0/kucoin_futures_lib/websocket.py
--rw-r--r--   0        0        0      430 2024-04-07 23:11:35.281519 kucoin_futures_lib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/LICENSE
+-rw-r--r--   0        0        0       52 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/README.md
+-rw-r--r--   0        0        0      719 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/factory.py
+-rw-r--r--   0        0        0      251 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/base.py
+-rw-r--r--   0        0        0     1920 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/entry.py
+-rw-r--r--   0        0        0     2508 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/oco.py
+-rw-r--r--   0        0        0     1419 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/helper.py
+-rw-r--r--   0        0        0     2464 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/kucoinf.py
+-rw-r--r--   0        0        0     3117 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/market.py
+-rw-r--r--   0        0        0    12864 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/trade.py
+-rw-r--r--   0        0        0     1068 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/user.py
+-rw-r--r--   0        0        0     2732 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/kucoin_futures_lib/websocket.py
+-rw-r--r--   0        0        0      455 2024-04-08 14:21:48.210106 kucoin_futures_lib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.1.1/PKG-INFO
```

### Comparing `kucoin_futures_lib-0.1.0/LICENSE` & `kucoin_futures_lib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.0/kucoin_futures_lib/__init__.py` & `kucoin_futures_lib-0.1.1/kucoin_futures_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.0/kucoin_futures_lib/factory.py` & `kucoin_futures_lib-0.1.1/kucoin_futures_lib/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,31 +25,31 @@
 
 
 def initialize_user(
     api_key: str, api_secret: str, api_passphrase: str
 ) -> "KucoinFuturesUser":
     """Initialize the Kucoin Futures User client using API credentials."""
     user = User(key=api_key, secret=api_secret, passphrase=api_passphrase)
-    return KucoinFuturesUser(user=user)
+    return KucoinFuturesUser(client=user)
 
 
 def initialize_market(
     api_key: str, api_secret: str, api_passphrase: str
 ) -> KucoinFuturesMarket:
     """Initialize the Kucoin Futures Market client using API credentials."""
     market = Market(key=api_key, secret=api_secret, passphrase=api_passphrase)
-    return KucoinFuturesMarket(market=market)
+    return KucoinFuturesMarket(client=market)
 
 
 def initialize_trade(
     api_key: str, api_secret: str, api_passphrase: str
 ) -> KucoinFuturesTrade:
     """Initialize the Kucoin Futures Trade client using API credentials."""
     trade = Trade(key=api_key, secret=api_secret, passphrase=api_passphrase)
-    return KucoinFuturesTrade(trade=trade)
+    return KucoinFuturesTrade(client=trade)
 
 
 def initialize_websocket(
     api_key: str,
     api_secret: str,
     api_passphrase: str,
     url="https://api-futures.kucoin.com",
```

### Comparing `kucoin_futures_lib-0.1.0/kucoin_futures_lib/handlers/base.py` & `kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.0/kucoin_futures_lib/handlers/entry.py` & `kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/entry.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.0/kucoin_futures_lib/handlers/oco.py` & `kucoin_futures_lib-0.1.1/kucoin_futures_lib/handlers/oco.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.0/kucoin_futures_lib/helper.py` & `kucoin_futures_lib-0.1.1/kucoin_futures_lib/helper.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.1.0/kucoin_futures_lib/kucoinf.py` & `kucoin_futures_lib-0.1.1/kucoin_futures_lib/kucoinf.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             instrument=instrument,
             side=side,
             size=size,
             price=price,
             leverage=leverage,
         )
 
-        await self.websocket.listen_for_fill(order_id=entry_order_id)
+        await self.trade.poll_for_fill(order_id=entry_order_id)
 
         order_ids = self.trade.create_stop_loss_and_take_profit(
             instrument=instrument,
             side=side,
             take_profit=take_profit,
             stop_loss=stop_loss,
             take_profit_type=take_profit_type,
```

### Comparing `kucoin_futures_lib-0.1.0/kucoin_futures_lib/market.py` & `kucoin_futures_lib-0.1.1/kucoin_futures_lib/market.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,39 +9,39 @@
 
 
 class KucoinFuturesMarket:
     """Kucoin Futures market wrapper class."""
 
     def __init__(
         self,
-        market: Market = None,
+        client: Market = None,
     ):
         """Initialize the Kucoin Futures client."""
-        self.market = market
+        self.client = client
 
     def get_current_price(self, instrument: str) -> float:
         """Get the current price of an instrument.
         :param instrument: The instrument symbol
         :return: The current price of the instrument"""
         logger.debug("Getting current price for: %s", instrument)
-        return float(self.market.get_ticker(instrument)["price"])
+        return float(self.client.get_ticker(instrument)["price"])
 
     def get_tick_size(self, instrument: str) -> float:  # Unused
         """Get the tick size for an instrument.
         :param instrument: The instrument symbol
         :return: The tick size"""
         logger.debug("Getting tick size for: %s", instrument)
-        return self.market.get_contract_detail(instrument)["tickSize"]
+        return self.client.get_contract_detail(instrument)["tickSize"]
 
     def get_multiplier(self, instrument: str) -> float:  # Unused
         """Get the contract multiplier for an instrument.
         :param instrument: The instrument symbol
         :return: The contract multiplier"""
         logger.debug("Getting multiplier for: %s", instrument)
-        return self.market.get_contract_detail(instrument)["multiplier"]
+        return self.client.get_contract_detail(instrument)["multiplier"]
 
     async def poll_for_entry(
         self,
         instrument: str,
         entry_low: float,
         entry_high: float,
         interval: int = 3,
```

### Comparing `kucoin_futures_lib-0.1.0/kucoin_futures_lib/trade.py` & `kucoin_futures_lib-0.1.1/kucoin_futures_lib/trade.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,41 +15,41 @@
 
 
 class KucoinFuturesTrade:
     """Kucoin Futures trade wrapper class."""
 
     def __init__(
         self,
-        trade: Trade = None,
+        client: Trade = None,
         leverage: int = 2,
     ):
         """Initialize the Kucoin Futures client."""
-        self.trade = trade
+        self.client = client
         self.leverage = leverage
 
     def get_open_orders(self, instrument: str = None) -> List[Dict[str, Any]]:  # Unused
         """https://www.kucoin.com/docs/rest/futures-trading/orders/get-order-list
         :param instrument: The instrument symbol
         :return: A dictionary containing the open orders for the instrument"""
         logger.debug("Getting open orders")
-        response = self.trade.get_order_list()
+        response = self.client.get_order_list()
         if instrument:
             open_orders = [
                 order for order in response["items"] if order["symbol"] == instrument
             ]
         else:
             open_orders = response["items"]
         return open_orders
 
     def cancel_order(self, order_id: str) -> None:
         """Cancel an order by order id.
         https://www.kucoin.com/docs/rest/futures-trading/orders/cancel-order-by-orderid
         """
         logger.debug("Cancelling order by order id: %s", order_id)
-        self.trade.cancel_order(orderId=order_id)
+        self.client.cancel_order(orderId=order_id)
         logger.info("Order %s cancel request sent.", order_id)
 
     async def cancel_order_and_wait(self, order_id: str) -> None:
         """Cancel an order by order id and wait for it to be done."""
         self.cancel_order(order_id)
         await self.poll_for_done(order_id)
         logger.info("Order %s has been cancelled", order_id)
@@ -59,15 +59,15 @@
         instrument: str,
         entry_side: str,
         tp_price: float,
     ) -> str:
         """Create a take profit order using limit order.
         https://www.kucoin.com/docs/rest/futures-trading/orders/place-order
         """
-        response = self.trade.create_limit_order(
+        response = self.client.create_limit_order(
             symbol=instrument,
             side="buy" if entry_side == "sell" else "sell",
             price=str(tp_price),
             timeInForce="GTC",
             closeOrder=True,
             lever=None,
             size=None,
@@ -83,15 +83,15 @@
         entry_side: str,
         tp_price: float,
     ) -> str:
         """Create take profit order using stop market order.
         https://www.kucoin.com/docs/rest/futures-trading/orders/place-order
         """
         side, stop = ("sell", "up") if entry_side == "buy" else ("buy", "down")
-        response = self.trade.create_market_order(
+        response = self.client.create_market_order(
             symbol=instrument,
             side=side,
             stop=stop,
             stopPriceType="TP",
             stopPrice=str(tp_price),
             timeInForce="GTC",
             closeOrder=True,
@@ -113,15 +113,15 @@
         https://www.kucoin.com/docs/rest/futures-trading/orders/place-order
         :param instrument: Instrument symbol
         :param entry_side: Entry order side (buy or sell)
         :param sl_price: Take profit price
         :return: The order id of the stop loss order
         """
         side, stop = ("sell", "down") if entry_side == "buy" else ("buy", "up")
-        response = self.trade.create_market_order(
+        response = self.client.create_market_order(
             symbol=instrument,
             side=side,
             stop=stop,
             lever=None,
             stopPriceType="TP",
             stopPrice=str(sl_price),
             timeInForce="GTC",
@@ -140,15 +140,15 @@
         https://www.kucoin.com/docs/rest/futures-trading/orders/place-order
         :param instrument: Instrument symbol
         :param entry_side: Entry order side (buy or sell)
         :param sl_price: Take profit price
         :return: The order id of the stop loss order
         """
         side, stop = ("sell", "down") if entry_side == "buy" else ("buy", "up")
-        response = self.trade.create_limit_order(
+        response = self.client.create_limit_order(
             symbol=instrument,
             side=side,
             stop=stop,
             stopPriceType="TP",
             price=str(sl_price),
             stopPrice=str(sl_price),
             timeInForce="GTC",
@@ -174,15 +174,15 @@
         :param side: The side of the order (buy or sell)
         :param size: The size of the order in lots
         :param leverage: The leverage to use
         :return: The order id of the entry order
         """
         side = side.lower()
         leverage = leverage or self.leverage
-        response = self.trade.create_market_order(
+        response = self.client.create_market_order(
             symbol=instrument, side=side, size=str(size), lever=str(leverage)
         )
         entry_order_id = response["orderId"]
         logger.info(
             "Created market %s order for %s with id %s",
             side,
             instrument,
@@ -206,15 +206,15 @@
         :param price: The limit price
         :param leverage: The leverage to use
         :return: The order id of the entry order
         """
         side = side.lower()
         leverage = leverage or self.leverage
 
-        response = self.trade.create_limit_order(
+        response = self.client.create_limit_order(
             symbol=instrument,
             side=side,
             lever=str(leverage),
             size=str(size),
             price=str(price),
         )
         entry_order_id = response.get("orderId")
@@ -289,15 +289,15 @@
         :param interval: The interval in seconds between each poll. Default is 5 seconds.
         :param max_attempts: The maximum number of attempts to make before giving up. Default is 720.
         :return: A dictionary containing the fill details of the matching order if found.
         :raises TimeoutError: If `order_id` is not found after the maximum number of attempts.
         """
         attempt = 0
         while attempt < max_attempts:
-            recent_fills = self.trade.get_recent_fills()
+            recent_fills = self.client.get_recent_fills()
             logger.debug("Recent fills: %s", json.dumps(recent_fills))
             if isinstance(recent_fills, list):
                 for fill in recent_fills:
                     if isinstance(fill, dict) and fill.get("orderId", "") == order_id:
                         logger.info("Order %s has been filled.", order_id)
                         return fill
                 logger.info("Order %s has not been filled yet.", order_id)
@@ -325,15 +325,15 @@
         :param order_id: Order ID to wait for done status.
         :param interval: The interval in seconds between each poll. Default is 1 second.
         :param max_attempts: The maximum number of attempts to make before giving up. Default is 20.
         :return: A dictionary containing the order details if the order status is done.
         """
         attempt = 0
         while attempt < max_attempts:
-            order_details = self.trade.get_order_details(order_id)
+            order_details = self.client.get_order_details(order_id)
             logger.info("Order details: %s", json.dumps(order_details))
             if order_details["status"] == "done":
                 logger.info("Order %s is done.", order_id)
                 return order_details
             attempt += 1
             logger.info(
                 "Order %s is not done yet. Attempt %s/%s",
```

### Comparing `kucoin_futures_lib-0.1.0/kucoin_futures_lib/user.py` & `kucoin_futures_lib-0.1.1/kucoin_futures_lib/user.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 logger = logging.getLogger(__name__)
 
 
 class KucoinFuturesUser:
     """Kucoin Futures user wrapper class."""
 
-    def __init__(self, user: User = None, currency: str = "USDT"):
-        self.user = user
+    def __init__(self, client: User = None, currency: str = "USDT"):
+        self.client = client
         self.currency = currency
 
     def get_account_overview(self, currency: Optional[str] = None) -> dict:
         """Get the account overview.
         :param currency: The currency to get the account overview for.
         :return: The account overview"""
         logger.debug("Getting account overview")
         currency = currency or self.currency
-        return self.user.get_account_overview(currency=currency)
+        return self.client.get_account_overview(currency=currency)
 
     def get_balance(self, currency: Optional[str] = None) -> float:
         """Get the account balance.
         :return: The account balance"""
         logger.debug("Getting account balance")
         account_overview = self.get_account_overview(currency=currency)
         return float(account_overview["accountEquity"])
```

### Comparing `kucoin_futures_lib-0.1.0/kucoin_futures_lib/websocket.py` & `kucoin_futures_lib-0.1.1/kucoin_futures_lib/websocket.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import logging
 from typing import Union, Callable, Awaitable, Optional
 
 from kucoin_futures.client import WsToken
 from kucoin_futures.ws_client import KucoinFuturesWsClient
 
-from kucoin_futures_lib.handlers import OcoHandler, EntryRangeHandler, HandlerABC, FillHandler
+from kucoin_futures_lib.handlers import OcoHandler, EntryRangeHandler, HandlerABC
 
 logger = logging.getLogger(__name__)
 
 
 class KucoinFuturesWebsocket:
     """Kucoin Futures user wrapper class."""
 
@@ -75,19 +75,7 @@
         :param entry_low: Entry low price
         :param timeout: timeout in seconds. Default is 12 hours
         """
         handler = EntryRangeHandler(
             instrument=instrument, entry_high=entry_high, entry_low=entry_low
         )
         await self.subscribe(handler, timeout)
-
-    async def listen_for_fill(
-        self,
-        order_id: str,
-        timeout: float = 60 * 60 * 12,
-    ) -> None:
-        """Listen for the order to be filled.
-        :param order_id: Order ID
-        :param timeout: timeout in seconds. Default is 12 hours
-        """
-        handler = FillHandler(order_id=order_id)
-        await self.subscribe(handler, timeout)
```

### Comparing `kucoin_futures_lib-0.1.0/PKG-INFO` & `kucoin_futures_lib-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: kucoin-futures-lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Kucoin Futures wrapper library
 License: Apache-2.0
 Author: Evgeny Aleshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: kucoin-futures-python (>=1.0.9,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # kucoin-futures-lib
 Kucoin Futures Wrapper Library
```

