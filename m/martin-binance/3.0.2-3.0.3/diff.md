# Comparing `tmp/martin_binance-3.0.2.tar.gz` & `tmp/martin_binance-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin_binance-3.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "martin_binance-3.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `martin_binance-3.0.2.tar` & `martin_binance-3.0.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1079 2024-04-03 15:51:58.716420 martin_binance-3.0.2/LICENSE
--rwxr-xr-x   0        0        0     3854 2024-04-03 15:51:58.716420 martin_binance-3.0.2/README.md
--rwxr-xr-x   0        0        0     2104 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/__init__.py
--rw-r--r--   0        0        0     5007 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2786 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    13214 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/backtest/exchange_simulator.py
--rwxr-xr-x   0        0        0     4419 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/backtest/optimizer.py
--rw-r--r--   0        0        0     7181 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     7182 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     7187 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rwxr-xr-x   0        0        0     7176 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/cli_3_BTCUSDT.py.template
--rw-r--r--   0        0        0     4752 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/client.py
--rw-r--r--   0        0        0     6895 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/db_utils.py
--rwxr-xr-x   0        0        0   139781 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/funds_rate.db.template
--rw-r--r--   0        0        0    15709 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/lib.py
--rw-r--r--   0        0        0     1723 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0     2253 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/params.py
--rw-r--r--   0        0        0      485 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    14650 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1269 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/relaunch.service
--rw-r--r--   0        0        0    82004 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/strategy_base.py
--rw-r--r--   0        0        0     7151 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/telegram_utils.py
--rw-r--r--   0        0        0     1424 2024-04-03 15:51:58.756420 martin_binance-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     5154 1970-01-01 00:00:00.000000 martin_binance-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-08 19:04:25.470012 martin_binance-3.0.3/LICENSE
+-rwxr-xr-x   0        0        0     3854 2024-04-08 19:04:25.470012 martin_binance-3.0.3/README.md
+-rwxr-xr-x   0        0        0     2076 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/__init__.py
+-rw-r--r--   0        0        0     5007 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2786 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    13214 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/backtest/exchange_simulator.py
+-rwxr-xr-x   0        0        0     4381 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/backtest/optimizer.py
+-rw-r--r--   0        0        0     4752 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/client.py
+-rw-r--r--   0        0        0     6935 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/db_utils.py
+-rwxr-xr-x   0        0        0   139916 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/executor.py
+-rw-r--r--   0        0        0    15709 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/lib.py
+-rw-r--r--   0        0        0     2253 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/params.py
+-rw-r--r--   0        0        0      485 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    14650 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1269 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/relaunch.service
+-rw-r--r--   0        0        0    82004 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/strategy_base.py
+-rw-r--r--   0        0        0     7151 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/telegram_utils.py
+-rw-r--r--   0        0        0     7181 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/cli_0_BTCUSDT.py
+-rw-r--r--   0        0        0     7182 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/cli_1_BTCUSDT.py
+-rw-r--r--   0        0        0     7187 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py
+-rwxr-xr-x   0        0        0     7176 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/cli_3_BTCUSDT.py
+-rw-r--r--   0        0        0   237568 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/funds_rate.db
+-rw-r--r--   0        0        0     1723 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/ms_cfg.toml
+-rw-r--r--   0        0        0      639 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/trial_params.json
+-rw-r--r--   0        0        0     1424 2024-04-08 19:04:25.506012 martin_binance-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5154 1970-01-01 00:00:00.000000 martin_binance-3.0.3/PKG-INFO
```

### Comparing `martin_binance-3.0.2/LICENSE` & `martin_binance-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/README.md` & `martin_binance-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/backtest/OoTSP.py` & `martin_binance-3.0.3/martin_binance/backtest/OoTSP.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/backtest/VCoSEL.py` & `martin_binance-3.0.3/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/backtest/exchange_simulator.py` & `martin_binance-3.0.3/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/backtest/optimizer.py` & `martin_binance-3.0.3/martin_binance/backtest/optimizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Searches for optimal parameters for a strategy under given conditions
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2024 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1"
+__version__ = "3.0.3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 
 import asyncio
 import importlib.util as iu
 import logging.handlers
@@ -18,15 +18,15 @@
 import sys
 from decimal import Decimal
 from pathlib import Path
 
 import optuna
 import ujson as json
 
-from martin_binance import LOG_PATH
+from martin_binance import LOG_PATH, TRIAL_PARAMS
 
 OPTIMIZER = Path(__file__).absolute()
 OPTIMIZER.chmod(OPTIMIZER.stat().st_mode | stat.S_IEXEC)
 PARAMS_FLOAT = ['KBB']
 STRATEGY = None
 
 
@@ -50,31 +50,33 @@
     return float(mbs.ex.SESSION_RESULT.get('profit', 0)) + float(mbs.ex.SESSION_RESULT.get('free', 0))
 
 
 def optimize(study_name, cli, n_trials, storage_name=None, _prm_best=None, skip_log=True, show_progress_bar=False):
     sys.excepthook = notify_exception
     optuna.logging.set_verbosity(optuna.logging.WARNING)
 
+    # Load parameter definitions from JSON file
+    with open(TRIAL_PARAMS) as f:
+        param_defs = json.load(f)
+
     spec = iu.spec_from_file_location("strategy", cli)
     mbs = iu.module_from_spec(spec)
     spec.loader.exec_module(mbs)
 
     def objective(_trial):
-        params = {
-            'GRID_MAX_COUNT': _trial.suggest_int('GRID_MAX_COUNT', 3, 5),
-            'PRICE_SHIFT': _trial.suggest_float('PRICE_SHIFT', 0, 0.05, step=0.01),
-            'PROFIT': _trial.suggest_float('PROFIT', 0.05, 0.2, step=0.05),
-            'PROFIT_MAX': _trial.suggest_float('PROFIT_MAX', 0.4, 1.0, step=0.05),
-            'OVER_PRICE': _trial.suggest_float('OVER_PRICE', 0.1, 1, step=0.1),
-            'ORDER_Q': _trial.suggest_int('ORDER_Q', 6, 12),
-            'MARTIN': _trial.suggest_float('MARTIN', 5, 15, step=1),
-            'SHIFT_GRID_DELAY': _trial.suggest_int('SHIFT_GRID_DELAY', 10, 150, step=10),
-            'KBB': _trial.suggest_float('KBB', 0.5, 4, step=0.5),
-            'LINEAR_GRID_K': _trial.suggest_int('LINEAR_GRID_K', 0, 500, step=50),
-        }
+        params = {}
+        for param_name, param_props in param_defs.items():
+            if param_props['type'] == 'int':
+                params[param_name] = _trial.suggest_int(
+                    param_name, *param_props['range'], step=param_props.get('step', 1)
+                )
+            elif param_props['type'] == 'float':
+                params[param_name] = _trial.suggest_float(
+                    param_name, *param_props['range'], step=param_props.get('step', 0.1)
+                )
         return try_trade(mbs, skip_log, **params)
 
     # noinspection PyArgumentList
     _study = optuna.create_study(study_name=study_name, storage=storage_name, direction="maximize")
 
     if _prm_best:
         logger.info(f"Previous best params: {_prm_best}")
@@ -113,14 +115,19 @@
     except KeyboardInterrupt:
         pass  # ignore
     except Exception as ex:
         logger.info(f"optimizer: {ex}")
     else:
         new_value = round(study.best_value, ndigits=6)
         bp = {k: int(any2str(v)) if isinstance(v, int) else float(any2str(v)) for k, v in study.best_params.items()}
+
         logger.info(f"Optimal parameters: {bp} for get {new_value}")
+        if new_value:
+            logger.info(f"Importance parameters: {optuna.importance.get_param_importances(study)}")
+
         _value = round(study.get_trials()[0].value, ndigits=6)
+
         if not prm_best or new_value > _value:
             bp |= {'new_value': any2str(new_value), '_value': any2str(_value)}
             print(json.dumps(bp))
         else:
             print(json.dumps({}))
```

### Comparing `martin_binance-3.0.2/martin_binance/cli_0_BTCUSDT.py.template` & `martin_binance-3.0.3/martin_binance/templates/cli_0_BTCUSDT.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1"
+__version__ = "3.0.3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 """
 ##################################################################
 Disclaimer
 
 All risks and possible losses associated with use of this strategy lie with you.
```

### Comparing `martin_binance-3.0.2/martin_binance/cli_1_BTCUSDT.py.template` & `martin_binance-3.0.3/martin_binance/templates/cli_1_BTCUSDT.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1"
+__version__ = "3.0.3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 """
 ##################################################################
 Disclaimer
 
 All risks and possible losses associated with use of this strategy lie with you.
```

### Comparing `martin_binance-3.0.2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin_binance-3.0.3/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1"
+__version__ = "3.0.3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 """
 ##################################################################
 Disclaimer
 
 All risks and possible losses associated with use of this strategy lie with you.
```

### Comparing `martin_binance-3.0.2/martin_binance/cli_3_BTCUSDT.py.template` & `martin_binance-3.0.3/martin_binance/templates/cli_3_BTCUSDT.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1"
+__version__ = "3.0.3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 """
 ##################################################################
 Disclaimer
 
 All risks and possible losses associated with use of this strategy lie with you.
```

### Comparing `martin_binance-3.0.2/martin_binance/client.py` & `martin_binance-3.0.3/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/db_utils.py` & `martin_binance-3.0.3/martin_binance/db_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Functions for managing and saving data to a SQLite database from martin-binance strategy
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.0"
+__version__ = "3.0.3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import contextlib
 import sqlite3
-from datetime import datetime
+from datetime import datetime, timezone
 import logging
 
 from martin_binance import DB_FILE
 
 logger = logging.getLogger('logger')
 
 
@@ -88,15 +88,15 @@
                                              float(data.get('s_funds')),
                                              float(data.get('avg_rate')),
                                              data.get('cycle_buy'),
                                              float(data.get('f_depo')),
                                              float(data.get('s_depo')),
                                              float(data.get('f_profit')),
                                              float(data.get('s_profit')),
-                                             datetime.utcnow(),
+                                             datetime.now(timezone.utc).replace(tzinfo=None),
                                              float(data.get('PRICE_SHIFT')),
                                              float(data.get('PROFIT')),
                                              float(data.get('over_price')),
                                              data.get('order_q'),
                                              float(data.get('MARTIN')),
                                              data.get('LINEAR_GRID_K'),
                                              data.get('ADAPTIVE_TRADE_CONDITION'),
```

### Comparing `martin_binance-3.0.2/martin_binance/executor.py` & `martin_binance-3.0.3/martin_binance/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Cyclic grid strategy based on martingale
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 import traceback
@@ -320,15 +320,16 @@
         if self.command == 'restart':
             self.stop()
             os.execv(sys.executable, [sys.executable] + [sys.argv[0]] + ['1'])
 
     def event_report(self):
         is_time_for_report_update = STATUS_DELAY and (self.get_time() - self.status_time) / 60 > STATUS_DELAY
         if self.command == 'status' or is_time_for_report_update:
-            self.command = None
+            if self.command == 'status':
+                self.command = None
             last_price = self.get_buffered_ticker().last_price
             ticker_update = int(self.get_time()) - self.last_ticker_update
             if self.cycle_time:
                 ct = str(datetime.now(timezone.utc).replace(tzinfo=None) - self.cycle_time).rsplit('.')[0]
             else:
                 self.message_log("save_strategy_state: cycle_time is None!", log_level=logging.DEBUG)
                 ct = str(datetime.now(timezone.utc)).rsplit('.')[0]
@@ -388,15 +389,16 @@
                               f"Second: {self.sum_profit_second}\n"
                               f"Summary: {sum_profit}\n"
                               f"{self.get_free_assets(mode='free')[3]}"
                               )
                 self.message_log(f"{header}\n"
                                  f"{'*** Shift grid mode ***' if self.shift_grid_threshold else '* **  **  ** *'}\n"
                                  f"{'Buy' if self.cycle_buy else 'Sell'}{' Reverse' if self.reverse else ''}"
-                                 f"{' Hold reverse' if self.reverse_hold else ''} {MODE}-cycle with"
+                                 f"{' Hold reverse' if self.reverse_hold else ''} "
+                                 f"{MODE}{'-SO' if MODE == 'TC' and SELF_OPTIMIZATION else ''}-cycle with"
                                  f" {order_buy} buy and {order_sell} sell active orders.\n"
                                  f"{order_hold or 'No'} hold grid orders\n"
                                  f"Over price: {self.over_price:.2f}%\n"
                                  f"Last ticker price: {last_price}\n"
                                  f"ver: {HEAD_VERSION}+{__version__}+{msb_ver}\n"
                                  f"From start {ct}\n"
                                  f"WSS status: {ticker_update}s\n"
```

### Comparing `martin_binance-3.0.2/martin_binance/funds_rate.db.template` & `martin_binance-3.0.3/martin_binance/templates/funds_rate.db`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/lib.py` & `martin_binance-3.0.3/martin_binance/lib.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/ms_cfg.toml.template` & `martin_binance-3.0.3/martin_binance/templates/ms_cfg.toml`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/params.py` & `martin_binance-3.0.3/martin_binance/params.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/service/funds_rate_exporter.py` & `martin_binance-3.0.3/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/service/grafana.json` & `martin_binance-3.0.3/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/service/relaunch.py` & `martin_binance-3.0.3/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/strategy_base.py` & `martin_binance-3.0.3/martin_binance/strategy_base.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/martin_binance/telegram_utils.py` & `martin_binance-3.0.3/martin_binance/telegram_utils.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.2/pyproject.toml` & `martin_binance-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.9"
 
 dependencies = [
-    "exchanges-wrapper==2.1.7",
+    "exchanges-wrapper==2.1.8",
     "jsonpickle==3.0.2",
     "psutil==5.9.6",
     "requests==2.31.0",
     "libtmux==0.23.2",
     "colorama==0.4.6",
     "prometheus-client==0.18.0",
     "optuna==3.4.0",
```

### Comparing `martin_binance-3.0.2/PKG-INFO` & `martin_binance-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 3.0.2
+Version: 3.0.3
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper==2.1.7
+Requires-Dist: exchanges-wrapper==2.1.8
 Requires-Dist: jsonpickle==3.0.2
 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0
 Requires-Dist: libtmux==0.23.2
 Requires-Dist: colorama==0.4.6
 Requires-Dist: prometheus-client==0.18.0
 Requires-Dist: optuna==3.4.0
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 3.0.2 Summary: Free trading
+Metadata-Version: 2.1 Name: martin-binance Version: 3.0.3 Summary: Free trading
 system for Binance SPOT API Author-email: Jerry Fedorenko
 yahoo.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: MacOS Requires-Dist: exchanges-
-wrapper==2.1.7 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
+wrapper==2.1.8 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0 Requires-Dist: libtmux==0.23.2 Requires-Dist:
 colorama==0.4.6 Requires-Dist: prometheus-client==0.18.0 Requires-Dist:
 optuna==3.4.0 Requires-Dist: plotly==5.18.0 Requires-Dist: pandas==2.1.2
 Requires-Dist: dash>=2.15.0 Requires-Dist: future==0.18.3 Requires-Dist:
 inquirer==3.1.3 Requires-Dist: scikit-learn==1.3.2 Requires-Dist: tqdm==4.66.1
 Requires-Dist: ujson~=5.9.0 Requires-Dist: orjson~=3.9.15 Requires-Dist:
 pyarrow~=14.0.2 Requires-Dist: shortuuid~=1.0.11 Requires-Dist: numpy~=1.23.4
```

