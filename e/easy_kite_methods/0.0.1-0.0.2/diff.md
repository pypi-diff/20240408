# Comparing `tmp/easy_kite_methods-0.0.1.tar.gz` & `tmp/easy_kite_methods-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_kite_methods-0.0.1.tar", max compression
+gzip compressed data, was "easy_kite_methods-0.0.2.tar", max compression
```

## Comparing `easy_kite_methods-0.0.1.tar` & `easy_kite_methods-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3025 2024-04-08 06:00:20.915413 easy_kite_methods-0.0.1/README.md
--rw-r--r--   0        0        0      510 2024-04-08 06:19:05.831494 easy_kite_methods-0.0.1/easy_kite_methods/__init__.py
--rw-r--r--   0        0        0     1627 2024-04-08 05:46:27.884702 easy_kite_methods-0.0.1/easy_kite_methods/kite_login.py
--rw-r--r--   0        0        0     8196 2024-04-08 06:19:05.832632 easy_kite_methods-0.0.1/easy_kite_methods/order_placement.py
--rw-r--r--   0        0        0      555 2024-04-08 06:19:24.350440 easy_kite_methods-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3645 1970-01-01 00:00:00.000000 easy_kite_methods-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3025 2024-04-08 06:23:56.009908 easy_kite_methods-0.0.2/README.md
+-rw-r--r--   0        0        0      510 2024-04-08 06:19:05.831494 easy_kite_methods-0.0.2/easy_kite_methods/__init__.py
+-rw-r--r--   0        0        0     1627 2024-04-08 05:46:27.884702 easy_kite_methods-0.0.2/easy_kite_methods/kite_login.py
+-rw-r--r--   0        0        0     8196 2024-04-08 06:19:05.832632 easy_kite_methods-0.0.2/easy_kite_methods/order_placement.py
+-rw-r--r--   0        0        0      555 2024-04-08 06:25:04.114956 easy_kite_methods-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3645 1970-01-01 00:00:00.000000 easy_kite_methods-0.0.2/PKG-INFO
```

### Comparing `easy_kite_methods-0.0.1/README.md` & `easy_kite_methods-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-# just_design_phase
+# easy_kite_methods
 
-The `just_design_phase` package provides a seamless interface for interacting with the Kite Connect API for stock trading on the Zerodha platform.
+The `easy_kite_methods` package provides a seamless interface for interacting with the Kite Connect API for stock trading on the Zerodha platform.
 
 ## Installation
 
-To install the `just_design_phase` package, run the following command:
+To install the `easy_kite_methods` package, run the following command:
 
 ```bash
-pip install just_design_phase
+pip install easy_kite_methods
 ```
 
 ## Configuration
 
-Before using the `just_design_phase` package, you must configure your environment with necessary API keys and secrets. Follow these steps to set up your environment:
+Before using the `easy_kite_methods` package, you must configure your environment with necessary API keys and secrets. Follow these steps to set up your environment:
 
 1. **Environment Variables**: Store your Kite Connect API key and secret in a `.env` file at the root of your project. This file should contain:
 
     ```
     KITE_API_KEY=your_api_key_here
     KITE_API_SECRET=your_api_secret_here
     ```
 
 ## Usage
 
-Import the package using the alias `jdp` and utilize its functions for interacting with the Zerodha Kite Connect API.
+Import the package using the alias `ekm` and utilize its functions for interacting with the Zerodha Kite Connect API.
 
 ### Example Imports
 
 ```python
-import just_design_phase as jdp
+import easy_kite_methods as ekm
 ```
 
 ### Placing Orders
 
 -   **Place a Normal Order**:
 
     ```python
-    order_id = jdp.place_normal_order(stock_name="RELIANCE", quantity=1, order_type="BUY")
+    order_id = ekm.place_normal_order(stock_name="RELIANCE", quantity=1, order_type="BUY")
     ```
 
 -   **Place a Limit Order**:
 
     ```python
-    order_id = jdp.place_limit_order(stock_name="TCS", quantity=2, price=3500, order_type="SELL")
+    order_id = ekm.place_limit_order(stock_name="TCS", quantity=2, price=3500, order_type="SELL")
     ```
 
 ### Modifying Orders
 
 -   **Modify an Order**:
 
     ```python
-    modified_order_id = jdp.modify_order(variety="regular", orderId="your_order_id_here", quantity=2, price=3550)
+    modified_order_id = ekm.modify_order(variety="regular", orderId="your_order_id_here", quantity=2, price=3550)
     ```
 
 ### Fetching Account Details
 
 -   **Fetch Holdings**:
 
     ```python
-    holdings = jdp.get_holdings()
+    holdings = ekm.get_holdings()
     ```
 
 -   **Fetch Positions**:
 
     ```python
-    positions = jdp.get_positions()
+    positions = ekm.get_positions()
     ```
 
 ### Additional Methods
 
 Include more comprehensive functionalities for trading:
 
 -   **Get Stock Price**:
 
     ```python
-    stock_price = jdp.get_stock_price(name="RELIANCE")
+    stock_price = ekm.get_stock_price(name="RELIANCE")
     ```
 
 -   **Get Stock Instrument Token**:
 
     ```python
-    token = jdp.get_stock_instrument_token(stock_name="RELIANCE")
+    token = ekm.get_stock_instrument_token(stock_name="RELIANCE")
     ```
 
 -   **Buy/Sell Intraday Normal Order**:
 
     ```python
-    order_id = jdp.buy_intraday_normal_order(stock_name="INFY", quantity=10)
+    order_id = ekm.buy_intraday_normal_order(stock_name="INFY", quantity=10)
     ```
 
     ```python
-    order_id = jdp.sell_intraday_normal_order(stock_name="INFY", quantity=5)
+    order_id = ekm.sell_intraday_normal_order(stock_name="INFY", quantity=5)
     ```
 
 -   **Buy/Sell Intraday Limit Order**:
 
     ```python
-    order_id = jdp.buy_intraday_limit_order(stock_name="INFY", quantity=10, price=1500)
+    order_id = ekm.buy_intraday_limit_order(stock_name="INFY", quantity=10, price=1500)
     ```
 
     ```python
-    order_id = jdp.sell_intraday_limit_order(stock_name="INFY", quantity=5, price=1500)
+    order_id = ekm.sell_intraday_limit_order(stock_name="INFY", quantity=5, price=1500)
     ```
 
 -   **Place Stop Loss Market Order**:
 
     ```python
-    order_id = jdp.place_slm_order(stock_name="INFY", quantity=10, order_type="BUY", price=1500)
+    order_id = ekm.place_slm_order(stock_name="INFY", quantity=10, order_type="BUY", price=1500)
     ```
 
 -   **Modify Order Properties**:
 
     ```python
-    new_order_id = jdp.modify_order_quantity(variety="regular", order_id="order123", quantity=15)
+    new_order_id = ekm.modify_order_quantity(variety="regular", order_id="order123", quantity=15)
     ```
 
     ```python
-    new_order_id = jdp.modify_order_price(variety="regular", order_id="order123", price=1520)
+    new_order_id = ekm.modify_order_price(variety="regular", order_id="order123", price=1520)
     ```
 
 -   **Cancel or Exit Orders**:
 
     ```python
-    jdp.cancel_order(order_id="order123")
+    ekm.cancel_order(order_id="order123")
     ```
 
     ```python
-    jdp.exit_orders(order_id="order123")
+    ekm.exit_orders(order_id="order123")
     ```
```

### Comparing `easy_kite_methods-0.0.1/easy_kite_methods/kite_login.py` & `easy_kite_methods-0.0.2/easy_kite_methods/kite_login.py`

 * *Files identical despite different names*

### Comparing `easy_kite_methods-0.0.1/easy_kite_methods/order_placement.py` & `easy_kite_methods-0.0.2/easy_kite_methods/order_placement.py`

 * *Files identical despite different names*

### Comparing `easy_kite_methods-0.0.1/pyproject.toml` & `easy_kite_methods-0.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_kite_methods"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Vivek Patel <vivekkvhpatel@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 kiteconnect = "^5.0.1"
```

