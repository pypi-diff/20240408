# Comparing `tmp/prosperity2bt-0.1.4.tar.gz` & `tmp/prosperity2bt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.1.4.tar", last modified: Sun Apr  7 00:22:48 2024, max compression
+gzip compressed data, was "prosperity2bt-0.2.0.tar", last modified: Mon Apr  8 09:08:11 2024, max compression
```

## Comparing `prosperity2bt-0.1.4.tar` & `prosperity2bt-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-07 00:22:45.000000 prosperity2bt-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.940956 prosperity2bt-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-08 09:08:11.940956 prosperity2bt-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.932957 prosperity2bt-0.2.0/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9777 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.932957 prosperity2bt-0.2.0/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.932957 prosperity2bt-0.2.0/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.940956 prosperity2bt-0.2.0/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.940956 prosperity2bt-0.2.0/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-08 09:08:09.000000 prosperity2bt-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:08:11.940956 prosperity2bt-0.2.0/setup.cfg
```

### Comparing `prosperity2bt-0.1.4/LICENSE` & `prosperity2bt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.4/PKG-INFO` & `prosperity2bt-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.1.4
+Version: 0.2.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.1.4/README.md` & `prosperity2bt-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.4/prosperity2bt/core.py` & `prosperity2bt-0.2.0/prosperity2bt/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 
     return "\n" + "\n".join(sandbox_log_lines)
 
 def process_buy_order(
     timestamp: int,
     order: Order,
     order_depth: OrderDepth,
-    own_trades: dict[Symbol, list[Trade]],
     own_positions: dict[Symbol, int],
     profit_loss_by_product: dict[Symbol, float],
 ) -> list[Trade]:
     new_trades = []
 
     price_matches = sorted(price for price in order_depth.sell_orders.keys() if price <= order.price)
     for price in price_matches:
@@ -85,15 +84,14 @@
 
     return new_trades
 
 def process_sell_order(
     timestamp: int,
     order: Order,
     order_depth: OrderDepth,
-    own_trades: dict[Symbol, list[Trade]],
     own_positions: dict[Symbol, int],
     profit_loss_by_product: dict[Symbol, float],
 ) -> list[Trade]:
     new_trades = []
 
     price_matches = sorted((price for price in order_depth.buy_orders.keys() if price >= order.price), reverse=True)
     for price in price_matches:
@@ -114,23 +112,22 @@
 
     return new_trades
 
 def process_order(
     timestamp: int,
     order: Order,
     order_depths: dict[Symbol, OrderDepth],
-    own_trades: dict[Symbol, list[Trade]],
     own_positions: dict[Symbol, int],
     profit_loss_by_product: dict[Symbol, float],
 ) -> list[Trade]:
     order_depth = order_depths[order.symbol]
     if order.quantity > 0:
-        return process_buy_order(timestamp, order, order_depth, own_trades, own_positions, profit_loss_by_product)
+        return process_buy_order(timestamp, order, order_depth, own_positions, profit_loss_by_product)
     elif order.quantity < 0:
-        return process_sell_order(timestamp, order, order_depth, own_trades, own_positions, profit_loss_by_product)
+        return process_sell_order(timestamp, order, order_depth, own_positions, profit_loss_by_product)
     else:
         return []
 
 def trade_to_dict(trade: Trade) -> dict[str, Any]:
     return {
         "timestamp": trade.timestamp,
         "buyer": trade.buyer,
@@ -270,22 +267,15 @@
             "timestamp": timestamp,
         })
 
         for product in tradable_products:
             new_trades = []
 
             for order in orders_by_symbol.get(product, []):
-                new_trades.extend(process_order(
-                    timestamp,
-                    order,
-                    order_depths,
-                    own_trades,
-                    own_positions,
-                    profit_loss_by_product,
-                ))
+                new_trades.extend(process_order(timestamp, order, order_depths, own_positions, profit_loss_by_product))
 
             if len(new_trades) > 0:
                 own_trades[product] = new_trades
 
         for product, trades in trades_by_timestamp[timestamp].items():
             market_trades[product] = trades
```

### Comparing `prosperity2bt-0.1.4/prosperity2bt/data.py` & `prosperity2bt-0.2.0/prosperity2bt/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     trades = []
     with trades_file as file:
         for line in file.read_text(encoding="utf-8").splitlines()[1:]:
             columns = line.split(";")
 
             trades.append(Trade(
                 symbol=columns[3],
-                price=int(columns[5]),
+                price=int(float(columns[5])),
                 quantity=int(columns[6]),
                 buyer=columns[1],
                 seller=columns[2],
                 timestamp=int(columns[0]),
             ))
 
     return DayData(round, day, prices, trades)
```

### Comparing `prosperity2bt-0.1.4/prosperity2bt/datamodel.py` & `prosperity2bt-0.2.0/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.4/prosperity2bt/main.py` & `prosperity2bt-0.2.0/prosperity2bt/main.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.4/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.2.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.4/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.2.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.4/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.2.0/prosperity2bt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.1.4
+Version: 0.2.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.1.4/pyproject.toml` & `prosperity2bt-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.1.4"
+version = "0.2.0"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

