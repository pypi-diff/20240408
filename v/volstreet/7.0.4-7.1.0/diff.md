# Comparing `tmp/volstreet-7.0.4.tar.gz` & `tmp/volstreet-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-7.0.4.tar", last modified: Fri Apr  5 08:06:17 2024, max compression
+gzip compressed data, was "volstreet-7.1.0.tar", last modified: Mon Apr  8 03:37:26 2024, max compression
```

## Comparing `volstreet-7.0.4.tar` & `volstreet-7.1.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 08:06:17.622201 volstreet-7.0.4/
--rw-rw-rw-   0        0        0     1260 2024-04-05 08:06:17.622201 volstreet-7.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.0.4/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     1085 2024-04-05 08:06:17.625009 volstreet-7.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 08:06:17.519978 volstreet-7.0.4/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.0.4/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:06:17.546102 volstreet-7.0.4/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.0.4/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.0.4/volstreet/angel_interface/access_rate_handlers.py
--rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2600 2024-04-03 08:06:51.000000 volstreet-7.0.4/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    13980 2024-04-05 08:03:07.000000 volstreet-7.0.4/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     3534 2024-03-27 14:07:30.000000 volstreet-7.0.4/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    28910 2024-03-28 11:04:55.000000 volstreet-7.0.4/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.0.4/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:06:17.568468 volstreet-7.0.4/volstreet/backtests/
--rw-rw-rw-   0        0        0      187 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     8882 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/backtests/data_handling.py
--rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.0.4/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    47182 2024-03-26 10:23:44.000000 volstreet-7.0.4/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5397 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.0.4/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15721 2024-03-26 10:23:44.000000 volstreet-7.0.4/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     1628 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    18739 2024-03-14 09:00:56.000000 volstreet-7.0.4/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     6010 2024-04-05 07:34:15.000000 volstreet-7.0.4/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:06:17.583552 volstreet-7.0.4/volstreet/datamodule/
--rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.0.4/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.0.4/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.0.4/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:06:17.584619 volstreet-7.0.4/volstreet/historical_info/
--rw-rw-rw-   0        0        0    18338 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-05 05:24:39.000000 volstreet-7.0.4/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:06:17.593804 volstreet-7.0.4/volstreet/strategies/
--rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0     5684 2024-04-03 08:06:51.000000 volstreet-7.0.4/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    27021 2024-04-05 08:02:01.000000 volstreet-7.0.4/volstreet/strategies/execution.py
--rw-rw-rw-   0        0        0    58696 2024-04-05 07:07:47.000000 volstreet-7.0.4/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     9310 2024-04-05 02:48:44.000000 volstreet-7.0.4/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    89782 2024-04-05 04:35:38.000000 volstreet-7.0.4/volstreet/strategies/strats.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:06:17.602825 volstreet-7.0.4/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      256 2024-04-03 08:06:51.000000 volstreet-7.0.4/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26065 2024-04-04 11:05:16.000000 volstreet-7.0.4/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0     9797 2024-04-05 07:44:33.000000 volstreet-7.0.4/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    11666 2024-04-05 07:34:15.000000 volstreet-7.0.4/volstreet/trade_interface/order_placement.py
--rw-rw-rw-   0        0        0    20048 2024-04-03 08:06:51.000000 volstreet-7.0.4/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:06:17.613973 volstreet-7.0.4/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     2963 2024-04-05 02:45:53.000000 volstreet-7.0.4/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13047 2024-03-28 07:00:26.000000 volstreet-7.0.4/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.0.4/volstreet/vectorized_blackscholes.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:06:17.619385 volstreet-7.0.4/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.0.4/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.0.4/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.0.4/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.0.4/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0      599 2024-03-28 11:16:14.000000 volstreet-7.0.4/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:06:17.622201 volstreet-7.0.4/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1260 2024-04-05 08:06:17.000000 volstreet-7.0.4/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2374 2024-04-05 08:06:17.000000 volstreet-7.0.4/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 08:06:17.000000 volstreet-7.0.4/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      443 2024-04-05 08:06:17.000000 volstreet-7.0.4/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 08:06:17.000000 volstreet-7.0.4/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.316458 volstreet-7.1.0/
+-rw-rw-rw-   0        0        0     1293 2024-04-08 03:37:26.315148 volstreet-7.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.1.0/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1104 2024-04-08 03:37:26.317702 volstreet-7.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.141221 volstreet-7.1.0/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.1.0/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.177564 volstreet-7.1.0/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.1.0/volstreet/angel_interface/access_rate_handlers.py
+-rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2600 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    13980 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.1.0/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    28910 2024-03-28 11:04:55.000000 volstreet-7.1.0/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.1.0/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.214992 volstreet-7.1.0/volstreet/backtests/
+-rw-rw-rw-   0        0        0      187 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     8882 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/data_handling.py
+-rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    47225 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5397 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15721 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1628 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    18739 2024-03-14 09:00:56.000000 volstreet-7.1.0/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     6003 2024-04-08 03:36:49.000000 volstreet-7.1.0/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.238386 volstreet-7.1.0/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.241378 volstreet-7.1.0/volstreet/historical_info/
+-rw-rw-rw-   0        0        0    18338 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.272314 volstreet-7.1.0/volstreet/strategies/
+-rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0     5684 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    27021 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/strategies/execution.py
+-rw-rw-rw-   0        0        0    56666 2024-04-08 03:36:49.000000 volstreet-7.1.0/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0    13100 2024-04-08 03:26:20.000000 volstreet-7.1.0/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0    89977 2024-04-06 06:44:48.000000 volstreet-7.1.0/volstreet/strategies/strats.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.289067 volstreet-7.1.0/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      256 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26077 2024-04-06 06:58:33.000000 volstreet-7.1.0/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0     9797 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    11666 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/trade_interface/order_placement.py
+-rw-rw-rw-   0        0        0    20048 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.300528 volstreet-7.1.0/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     2963 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    13047 2024-03-28 07:00:26.000000 volstreet-7.1.0/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/vectorized_blackscholes.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.312618 volstreet-7.1.0/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.1.0/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.1.0/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0      599 2024-03-28 11:16:14.000000 volstreet-7.1.0/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.313648 volstreet-7.1.0/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-04-08 03:37:26.000000 volstreet-7.1.0/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2374 2024-04-08 03:37:26.000000 volstreet-7.1.0/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 03:37:26.000000 volstreet-7.1.0/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-04-08 03:37:26.000000 volstreet-7.1.0/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 03:37:26.000000 volstreet-7.1.0/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-7.0.4/PKG-INFO` & `volstreet-7.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.0.4
+Version: 7.1.0
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -13,14 +13,15 @@
 Requires-Dist: BeautifulSoup4<5.0,>=4.12.3
 Requires-Dist: eod<1.0,>=0.2.1
 Requires-Dist: fuzzywuzzy<1.0,>=0.18.0
 Requires-Dist: joblib<2.0,>=1.3.2
 Requires-Dist: logzero<2.0,>=1.7.0
 Requires-Dist: numpy<2.0,>=1.26.4
 Requires-Dist: pandas<3.0,>=2.0.1
+Requires-Dist: pulp<3.0,>=2.8.0
 Requires-Dist: pyotp<3.0,>=2.8.0
 Requires-Dist: python-Levenshtein<1.0,>=0.25.0
 Requires-Dist: requests<3.0,>=2.28.2
 Requires-Dist: scikit-learn<2.0,>=1.2.2
 Requires-Dist: scipy<2.0,>=1.12.0
 Requires-Dist: six<2.0,>=1.16.0
 Requires-Dist: smartapi-python<1.5.0,>=1.4.7
```

### Comparing `volstreet-7.0.4/setup.cfg` & `volstreet-7.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 372e 302e 340d 0a61  rsion = 7.0.4..a
+00000020: 7273 696f 6e20 3d20 372e 312e 300d 0a61  rsion = 7.1.0..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
@@ -36,33 +36,34 @@
 00000230: 2e32 2e31 2c3c 312e 300d 0a09 6675 7a7a  .2.1,<1.0...fuzz
 00000240: 7977 757a 7a79 3e3d 302e 3138 2e30 2c3c  ywuzzy>=0.18.0,<
 00000250: 312e 300d 0a09 6a6f 626c 6962 3e3d 312e  1.0...joblib>=1.
 00000260: 332e 322c 3c32 2e30 0d0a 096c 6f67 7a65  3.2,<2.0...logze
 00000270: 726f 3e3d 312e 372e 302c 3c32 2e30 0d0a  ro>=1.7.0,<2.0..
 00000280: 096e 756d 7079 3e3d 312e 3236 2e34 2c3c  .numpy>=1.26.4,<
 00000290: 322e 300d 0a09 7061 6e64 6173 3e3d 322e  2.0...pandas>=2.
-000002a0: 302e 312c 3c33 2e30 0d0a 0970 796f 7470  0.1,<3.0...pyotp
-000002b0: 3e3d 322e 382e 302c 3c33 2e30 0d0a 0970  >=2.8.0,<3.0...p
-000002c0: 7974 686f 6e2d 4c65 7665 6e73 6874 6569  ython-Levenshtei
-000002d0: 6e3e 3d30 2e32 352e 302c 3c31 2e30 0d0a  n>=0.25.0,<1.0..
-000002e0: 0972 6571 7565 7374 733e 3d32 2e32 382e  .requests>=2.28.
-000002f0: 322c 3c33 2e30 0d0a 0973 6369 6b69 742d  2,<3.0...scikit-
-00000300: 6c65 6172 6e3e 3d31 2e32 2e32 2c3c 322e  learn>=1.2.2,<2.
-00000310: 300d 0a09 7363 6970 793e 3d31 2e31 322e  0...scipy>=1.12.
-00000320: 302c 3c32 2e30 0d0a 0973 6978 3e3d 312e  0,<2.0...six>=1.
-00000330: 3136 2e30 2c3c 322e 300d 0a09 736d 6172  16.0,<2.0...smar
-00000340: 7461 7069 2d70 7974 686f 6e3e 3d31 2e34  tapi-python>=1.4
-00000350: 2e37 2c3c 312e 352e 300d 0a09 7371 6c61  .7,<1.5.0...sqla
-00000360: 6c63 6865 6d79 3e3d 322e 302e 3230 2c3c  lchemy>=2.0.20,<
-00000370: 332e 300d 0a09 7477 696c 696f 3e3d 382e  3.0...twilio>=8.
-00000380: 3131 2e31 2c3c 392e 300d 0a09 7572 6c6c  11.1,<9.0...urll
-00000390: 6962 333e 3d31 2e32 362e 3134 2c3c 322e  ib3>=1.26.14,<2.
-000003a0: 300d 0a09 7765 6273 6f63 6b65 742d 636c  0...websocket-cl
-000003b0: 6965 6e74 3e3d 312e 352e 312c 3c32 2e30  ient>=1.5.1,<2.0
-000003c0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-000003d0: 6b61 6765 5f64 6174 615d 0d0a 766f 6c73  kage_data]..vols
-000003e0: 7472 6565 7420 3d20 6869 7374 6f72 6963  treet = historic
-000003f0: 616c 5f69 6e66 6f2f 2a2e 706b 6c2c 2076  al_info/*.pkl, v
-00000400: 736c 6f67 6769 6e67 2f2a 2e6a 736f 6e0d  slogging/*.json.
-00000410: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000420: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000430: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+000002a0: 302e 312c 3c33 2e30 0d0a 0970 756c 703e  0.1,<3.0...pulp>
+000002b0: 3d32 2e38 2e30 2c3c 332e 300d 0a09 7079  =2.8.0,<3.0...py
+000002c0: 6f74 703e 3d32 2e38 2e30 2c3c 332e 300d  otp>=2.8.0,<3.0.
+000002d0: 0a09 7079 7468 6f6e 2d4c 6576 656e 7368  ..python-Levensh
+000002e0: 7465 696e 3e3d 302e 3235 2e30 2c3c 312e  tein>=0.25.0,<1.
+000002f0: 300d 0a09 7265 7175 6573 7473 3e3d 322e  0...requests>=2.
+00000300: 3238 2e32 2c3c 332e 300d 0a09 7363 696b  28.2,<3.0...scik
+00000310: 6974 2d6c 6561 726e 3e3d 312e 322e 322c  it-learn>=1.2.2,
+00000320: 3c32 2e30 0d0a 0973 6369 7079 3e3d 312e  <2.0...scipy>=1.
+00000330: 3132 2e30 2c3c 322e 300d 0a09 7369 783e  12.0,<2.0...six>
+00000340: 3d31 2e31 362e 302c 3c32 2e30 0d0a 0973  =1.16.0,<2.0...s
+00000350: 6d61 7274 6170 692d 7079 7468 6f6e 3e3d  martapi-python>=
+00000360: 312e 342e 372c 3c31 2e35 2e30 0d0a 0973  1.4.7,<1.5.0...s
+00000370: 716c 616c 6368 656d 793e 3d32 2e30 2e32  qlalchemy>=2.0.2
+00000380: 302c 3c33 2e30 0d0a 0974 7769 6c69 6f3e  0,<3.0...twilio>
+00000390: 3d38 2e31 312e 312c 3c39 2e30 0d0a 0975  =8.11.1,<9.0...u
+000003a0: 726c 6c69 6233 3e3d 312e 3236 2e31 342c  rllib3>=1.26.14,
+000003b0: 3c32 2e30 0d0a 0977 6562 736f 636b 6574  <2.0...websocket
+000003c0: 2d63 6c69 656e 743e 3d31 2e35 2e31 2c3c  -client>=1.5.1,<
+000003d0: 322e 300d 0a0d 0a5b 6f70 7469 6f6e 732e  2.0....[options.
+000003e0: 7061 636b 6167 655f 6461 7461 5d0d 0a76  package_data]..v
+000003f0: 6f6c 7374 7265 6574 203d 2068 6973 746f  olstreet = histo
+00000400: 7269 6361 6c5f 696e 666f 2f2a 2e70 6b6c  rical_info/*.pkl
+00000410: 2c20 7673 6c6f 6767 696e 672f 2a2e 6a73  , vslogging/*.js
+00000420: 6f6e 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  on....[egg_info]
+00000430: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000440: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `volstreet-7.0.4/volstreet/angel_interface/access_rate_handlers.py` & `volstreet-7.1.0/volstreet/angel_interface/access_rate_handlers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/angel_interface/async_interface.py` & `volstreet-7.1.0/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/angel_interface/base_websocket.py` & `volstreet-7.1.0/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/angel_interface/interface.py` & `volstreet-7.1.0/volstreet/angel_interface/interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/angel_interface/login.py` & `volstreet-7.1.0/volstreet/angel_interface/login.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import pyotp
 from time import sleep
 import os
-import logging
 import functools
-from datetime import datetime
 from volstreet.config import logger
 from volstreet.utils import current_time, notifier, set_error_notification_settings
 from volstreet.angel_interface.smart_connect import AsyncSmartConnect
 from volstreet.angel_interface.active_session import ActiveSession
 
 
 def login(user, pin, apikey, authkey, webhook_url=None, re_login=False):
@@ -36,40 +34,18 @@
         login_data.update(
             {"user": user, "pin": pin, "apikey": apikey, "authkey": authkey}
         )
         user_dir = f"{obj.userId}"
         if not os.path.exists(user_dir):
             os.makedirs(user_dir)
 
-        today = datetime.now().strftime("%Y-%m-%d")
-        info_log_filename = f"{obj.userId}-info-{today}.log"
-        error_log_filename = f"{obj.userId}-error-{today}.log"
-        info_log_filename = os.path.join(user_dir, info_log_filename)
-        error_log_filename = os.path.join(user_dir, error_log_filename)
-        formatter = logging.Formatter("%(asctime)s:%(levelname)s:%(message)s")
-
         # Set obj and login_data in config
         ActiveSession.obj = obj
         ActiveSession.login_data = login_data
 
-        # Edit file handlers
-        for handler in logger.handlers[:]:
-            if isinstance(handler, logging.FileHandler):
-                logger.removeHandler(handler)
-
-        info_handler = logging.FileHandler(info_log_filename)
-        info_handler.setLevel(logging.INFO)
-        info_handler.setFormatter(formatter)
-        logger.addHandler(info_handler)
-
-        error_handler = logging.FileHandler(error_log_filename)
-        error_handler.setLevel(logging.ERROR)
-        error_handler.setFormatter(formatter)
-        logger.addHandler(error_handler)
-
         set_error_notification_settings("user", obj.userId)
         notifier(
             f'Date: {current_time().strftime("%d %b %Y %H:%M:%S")}\nLogged in successfully.',
             webhook_url,
             "CRUCIAL",
         )
     else:
```

### Comparing `volstreet-7.0.4/volstreet/angel_interface/order_websocket.py` & `volstreet-7.1.0/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/angel_interface/price_websocket.py` & `volstreet-7.1.0/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/angel_interface/smart_connect.py` & `volstreet-7.1.0/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/backtests/data_handling.py` & `volstreet-7.1.0/volstreet/backtests/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/backtests/database.py` & `volstreet-7.1.0/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/backtests/delta_hedging.py` & `volstreet-7.1.0/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/backtests/delta_optimizer.py` & `volstreet-7.1.0/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/backtests/framework.py` & `volstreet-7.1.0/volstreet/backtests/framework.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,18 @@
         strike_offset: float = 1,
         call_strike_offset: float | None = None,
         put_strike_offset: float | None = None,
         from_date: str | datetime = "2019-04-01",
         to_date: str | datetime = None,
         only_expiry: bool = False,
     ):
-        """This function is intended to replace the overnight and quick straddle skeleton"""
+        """
+        This function is intended to replace the overnight and quick straddle skeleton
+        Offsets should be of the format of a multiplier. 1.02 for 2%, 0.98 for -2%
+        """
 
         underlying_prices_full = self.fetch_index_prices(
             underlying.name, from_timestamp=from_date, to_timestamp=to_date
         )
         underlying_prices_full = underlying_prices_full.set_index("timestamp")
         if only_expiry:
             expiry_dates_set = set(underlying.expiry_dates.date)
@@ -1170,14 +1173,15 @@
 
 
 def calculate_atm_ivs(
     backtester: BackTester,
     underlying: UnderlyingInfo,
     from_timestamp: str | datetime,
     to_timestamp: str | datetime,
+    **kwargs,
 ) -> pd.DataFrame:
     def _calculate_averages(group):
         # Calculate the average 'r', 'call_iv', and 'put_iv', ignoring missing values
         avg_r = group["r"].mean(skipna=True)
         avg_call_iv = group["call_iv"].mean(skipna=True)
         avg_put_iv = group["put_iv"].mean(skipna=True)
 
@@ -1186,38 +1190,36 @@
             {
                 "r": avg_r,
                 "call_iv": avg_call_iv,
                 "put_iv": avg_put_iv,
             }
         )
 
-        day_averages = day_averages.interpolate(method="linear")
-        day_averages = day_averages.fillna(method="ffill").fillna(method="bfill")
-
         return day_averages
 
     option_chain = backtester.build_option_chain(
-        underlying, from_timestamp, to_timestamp
+        underlying, from_timestamp, to_timestamp, **kwargs
     )
     option_chain["r"] = calculate_moving_interest_rate(option_chain)
     df = add_greeks_to_dataframe(option_chain, r_col="r")
     averages = df.groupby(["timestamp", "expiry"]).apply(_calculate_averages)
     averages["atm_iv"] = np.mean(averages[["call_iv", "put_iv"]], axis=1)
+    averages["atm_iv"] = averages["atm_iv"].ffill().bfill()
     averages["underlying"] = underlying.name
     averages = averages.reset_index()
     averages = averages.drop(columns=["call_iv", "put_iv"])
     return averages
 
 
 def store_atm_ivs(*args, **kwargs):
     ivs = calculate_atm_ivs(*args, **kwargs)
     underlying = ivs.underlying[0]
     from_timestamp = ivs.timestamp.min()
     to_timestamp = ivs.timestamp.max()
-    directory = f"data\\atm_ivs\\{underlying}"
+    directory = f"data\\atm_ivs_new\\{underlying}"
     file_name = f"{underlying}_atm_ivs_{from_timestamp.strftime('%Y-%m-%d')}_{to_timestamp.strftime('%Y-%m-%d')}.csv"
     full_path = f"{directory}\\{file_name}"
     make_directory_if_needed(full_path)
     ivs.to_csv(full_path)
 
 
 def calculate_moving_interest_rate(
```

### Comparing `volstreet-7.0.4/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-7.1.0/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/backtests/tools.py` & `volstreet-7.1.0/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/backtests/trend.py` & `volstreet-7.1.0/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/backtests/underlying_info.py` & `volstreet-7.1.0/volstreet/backtests/underlying_info.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/blackscholes.py` & `volstreet-7.1.0/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/config.py` & `volstreet-7.1.0/volstreet/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import urllib
 import requests
 import pandas as pd
 import pickle
 import os
 import joblib
 from pathlib import Path
-from threading import local, Event
+from threading import local
 from bs4 import BeautifulSoup
 from twilio.rest import Client as TwilioClient
 from io import StringIO
 import logging
 from importlib.resources import files
 from volstreet.vslogging import setup_logging
```

### Comparing `volstreet-7.0.4/volstreet/database_connection.py` & `volstreet-7.1.0/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/datamodule/analysis.py` & `volstreet-7.1.0/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/datamodule/archive.py` & `volstreet-7.1.0/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/datamodule/eod_client.py` & `volstreet-7.1.0/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/datamodule/gambling.py` & `volstreet-7.1.0/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/datamodule/intraday_data.py` & `volstreet-7.1.0/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/datamodule/stockmock.py` & `volstreet-7.1.0/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/datamodule/trading_assistance.py` & `volstreet-7.1.0/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/dealingroom.py` & `volstreet-7.1.0/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/decorators.py` & `volstreet-7.1.0/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/discord_bot.py` & `volstreet-7.1.0/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/exceptions.py` & `volstreet-7.1.0/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/historical_info/index_expiries.pkl` & `volstreet-7.1.0/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/parallelization.py` & `volstreet-7.1.0/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/performance_tracking.py` & `volstreet-7.1.0/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/strategies/error_handling.py` & `volstreet-7.1.0/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/strategies/execution.py` & `volstreet-7.1.0/volstreet/strategies/execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/strategies/helpers.py` & `volstreet-7.1.0/volstreet/strategies/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 from attrs import define, field, validators
 from datetime import datetime, timedelta, time
 from time import sleep
 from itertools import product
 import inspect
 import traceback
 from typing import Callable
+from pulp import LpStatus
 from volstreet import config
-from volstreet.exceptions import OptimizationError
 from volstreet.config import logger
 from volstreet.blackscholes import Greeks
 from volstreet.utils.core import (
     time_to_expiry,
     current_time,
-    dynamic_ceil,
-    dynamic_floor,
     round_shares_to_lot_size,
     filter_orderbook_by_time,
 )
 from volstreet.utils.communication import notifier
 from volstreet.utils.data_io import load_json_data, load_combine_save_json_data
 from volstreet.angel_interface.interface import (
     ActiveSession,
@@ -36,15 +34,15 @@
     OptionType,
     execute_instructions,
     place_option_order_and_notify,
     cancel_pending_orders,
 )
 from volstreet.strategies.optimization import (
     filter_greeks_frame,
-    optimize_option_weights,
+    delta_neutral_optimization_lp,
 )
 from volstreet.strategies.error_handling import log_error
 
 
 @define(slots=False, repr=False, eq=False)
 class ActiveOption(Option):
     """An extension of Option for more flexibility.
@@ -148,14 +146,18 @@
         self._premium_received = value
 
     @property
     def premium_outstanding(self):
         return self.active_qty * self.current_ltp
 
     @property
+    def mtm(self):
+        return self.premium_outstanding - self.premium_received
+
+    @property
     def position_greeks(self) -> Greeks:
         return self.current_greeks * self.active_qty
 
     @property
     def current_ltp(self) -> float:
         """The difference between this function and the parent function is that
         this function will set cached ltp."""
@@ -622,136 +624,136 @@
             greeks,
             0.65,
             self.underlying.get_synthetic_future_price(self.expiry),
             is_call,
         )
         return greeks
 
-    def set_recommendation_for_first_side(
-        self,
-        options: list[Option],
-        is_call: bool,
-    ) -> tuple[tuple[float, float], tuple[float, float]]:
-        greeks = self.prepare_greek_frame_with_options(options, is_call)
-
-        # Finding the gamma of the option whose delta is closest to 0.1
-        idx = np.abs(greeks[:, 2] - 0.1).argmin()
-        target_gamma = greeks[idx, 3]
-        gamma_floor = dynamic_floor(target_gamma)
-        gamma_ceil = dynamic_ceil(target_gamma)
-
-        for attempt in range(3):
-            try:
-                weights = optimize_option_weights(
-                    greeks[:, 2],
-                    greeks[:, 3],
-                    0.09,
-                    0.6,
-                    gamma_floor,
-                    gamma_ceil,
-                )
-                break
-            except OptimizationError as e:
-                if attempt == 2:
-                    raise e
-                gamma_floor *= 0.95
-                gamma_ceil *= 1.05
-            except Exception as e:
-                logger.error(
-                    f"Error in optimization: {e}, Traceback: {traceback.format_exc()}"
-                )
-                raise e
-
-        # noinspection PyUnboundLocalVariable
-        for option, weight in zip(greeks[:, -1], weights):
-            option.recommended_qty = round_shares_to_lot_size(
-                weight * self.base_exposure_qty, option.lot_size
-            )
-
-        # Return the weighted delta which will be used to configure the other side
-        calibrated_delta = np.dot(weights, greeks[:, 2])
-        target_deltas = (abs(calibrated_delta) - 0.01, abs(calibrated_delta) + 0.01)
-        target_gammas = (gamma_floor, gamma_ceil)
-        return target_deltas, target_gammas
-
-    def set_recommendation_for_second_side(
-        self,
-        options: list[Option],
-        is_call: bool,
-        target_deltas: tuple[float, float],
-        target_gammas: tuple[float, float],
-    ) -> None:
-        greeks = self.prepare_greek_frame_with_options(options, is_call)
-
-        for attempt in range(3):
-            try:
-                # This will try with multiple gamma scalers within itself,
-                # if all fails, it will raise an OptimizationError
-                weights = optimize_option_weights(
-                    greeks[:, 2], greeks[:, 3], *target_deltas, *target_gammas
-                )
-                break
-            except OptimizationError:
-                if attempt == 2:
-                    raise OptimizationError("Second side optimization failed")
-                elif attempt == 1:
-                    target_gammas = (-10000, 10000)  # Use the entire range
-                else:
-                    target_gammas = (target_gammas[0] * 0.75, target_gammas[1] * 1.25)
-            except Exception as e:
-                logger.error(
-                    f"Error in optimization: {e}, Traceback: {traceback.format_exc()}"
-                )
-                raise OptimizationError("Second side optimization failed")
-
-        # noinspection PyUnboundLocalVariable
-        for option, weight in zip(greeks[:, -1], weights):
-            option.recommended_qty = round_shares_to_lot_size(
-                weight * self.base_exposure_qty, option.lot_size
-            )
-
-    def set_optimized_recommended_qty(self) -> None:
-        self.reset_options()
-        try:
-            target_deltas, target_gammas = self.set_recommendation_for_first_side(
-                self.prospective_calls, is_call=True
-            )
-            self.set_recommendation_for_second_side(
-                self.prospective_puts,
-                is_call=False,
-                target_deltas=target_deltas,
-                target_gammas=target_gammas,
-            )
-        except Exception as e:
-            if "Second side optimization failed" in str(e):
-                notifier(
-                    f"Second side optimization failed for {self.underlying.name}. "
-                    f"Trying to calibrate again in reverse order.",
-                    self.notifier_url,
-                    "ERROR",
-                )
-                self.reset_options()  # CRUCIAL TO RESET THE OPTIONS
-
-                # Reverse the order of calibration
-                target_deltas, target_gammas = self.set_recommendation_for_first_side(
-                    self.prospective_puts, is_call=False
-                )
-                self.set_recommendation_for_second_side(
-                    self.prospective_calls,
-                    is_call=True,
-                    target_deltas=target_deltas,
-                    target_gammas=target_gammas,
-                )
-            else:
-                notifier(
-                    f"Optimization failed for {self.underlying.name}.",
-                    self.notifier_url,
-                    "ERROR",
-                )
-                raise e
+    # def set_recommendation_for_first_side(
+    #     self,
+    #     options: list[Option],
+    #     is_call: bool,
+    # ) -> tuple[tuple[float, float], tuple[float, float]]:
+    #     greeks = self.prepare_greek_frame_with_options(options, is_call)
+    #
+    #     # Finding the gamma of the option whose delta is closest to 0.1
+    #     idx = np.abs(greeks[:, 2] - 0.1).argmin()
+    #     target_gamma = greeks[idx, 3]
+    #     gamma_floor = dynamic_floor(target_gamma)
+    #     gamma_ceil = dynamic_ceil(target_gamma)
+    #
+    #     for attempt in range(3):
+    #         try:
+    #             weights = optimize_option_weights(
+    #                 greeks[:, 2],
+    #                 greeks[:, 3],
+    #                 0.09,
+    #                 0.6,
+    #                 gamma_floor,
+    #                 gamma_ceil,
+    #             )
+    #             break
+    #         except OptimizationError as e:
+    #             if attempt == 2:
+    #                 raise e
+    #             gamma_floor *= 0.95
+    #             gamma_ceil *= 1.05
+    #         except Exception as e:
+    #             logger.error(
+    #                 f"Error in optimization: {e}, Traceback: {traceback.format_exc()}"
+    #             )
+    #             raise e
+    #
+    #     # noinspection PyUnboundLocalVariable
+    #     for option, weight in zip(greeks[:, -1], weights):
+    #         option.recommended_qty = round_shares_to_lot_size(
+    #             weight * self.base_exposure_qty, option.lot_size
+    #         )
+    #
+    #     # Return the weighted delta which will be used to configure the other side
+    #     calibrated_delta = np.dot(weights, greeks[:, 2])
+    #     target_deltas = (abs(calibrated_delta) - 0.01, abs(calibrated_delta) + 0.01)
+    #     target_gammas = (gamma_floor, gamma_ceil)
+    #     return target_deltas, target_gammas
+    #
+    # def set_recommendation_for_second_side(
+    #     self,
+    #     options: list[Option],
+    #     is_call: bool,
+    #     target_deltas: tuple[float, float],
+    #     target_gammas: tuple[float, float],
+    # ) -> None:
+    #     greeks = self.prepare_greek_frame_with_options(options, is_call)
+    #
+    #     for attempt in range(3):
+    #         try:
+    #             # This will try with multiple gamma scalers within itself,
+    #             # if all fails, it will raise an OptimizationError
+    #             weights = optimize_option_weights(
+    #                 greeks[:, 2], greeks[:, 3], *target_deltas, *target_gammas
+    #             )
+    #             break
+    #         except OptimizationError:
+    #             if attempt == 2:
+    #                 raise OptimizationError("Second side optimization failed")
+    #             elif attempt == 1:
+    #                 target_gammas = (-10000, 10000)  # Use the entire range
+    #             else:
+    #                 target_gammas = (target_gammas[0] * 0.75, target_gammas[1] * 1.25)
+    #         except Exception as e:
+    #             logger.error(
+    #                 f"Error in optimization: {e}, Traceback: {traceback.format_exc()}"
+    #             )
+    #             raise OptimizationError("Second side optimization failed")
+    #
+    #     # noinspection PyUnboundLocalVariable
+    #     for option, weight in zip(greeks[:, -1], weights):
+    #         option.recommended_qty = round_shares_to_lot_size(
+    #             weight * self.base_exposure_qty, option.lot_size
+    #         )
+    #
+    # def set_optimized_recommended_qty(self) -> None:
+    #     self.reset_options()
+    #     try:
+    #         target_deltas, target_gammas = self.set_recommendation_for_first_side(
+    #             self.prospective_calls, is_call=True
+    #         )
+    #         self.set_recommendation_for_second_side(
+    #             self.prospective_puts,
+    #             is_call=False,
+    #             target_deltas=target_deltas,
+    #             target_gammas=target_gammas,
+    #         )
+    #     except Exception as e:
+    #         if "Second side optimization failed" in str(e):
+    #             notifier(
+    #                 f"Second side optimization failed for {self.underlying.name}. "
+    #                 f"Trying to calibrate again in reverse order.",
+    #                 self.notifier_url,
+    #                 "ERROR",
+    #             )
+    #             self.reset_options()  # CRUCIAL TO RESET THE OPTIONS
+    #
+    #             # Reverse the order of calibration
+    #             target_deltas, target_gammas = self.set_recommendation_for_first_side(
+    #                 self.prospective_puts, is_call=False
+    #             )
+    #             self.set_recommendation_for_second_side(
+    #                 self.prospective_calls,
+    #                 is_call=True,
+    #                 target_deltas=target_deltas,
+    #                 target_gammas=target_gammas,
+    #             )
+    #         else:
+    #             notifier(
+    #                 f"Optimization failed for {self.underlying.name}.",
+    #                 self.notifier_url,
+    #                 "ERROR",
+    #             )
+    #             raise e
 
     def set_recommended_qty_backup(
         self, target_delta: float = None, attempt_no: int = 0
     ):
         self.reset_options()
 
         if target_delta > 0.7 or attempt_no > 5:
@@ -778,14 +780,44 @@
             )
 
         if not success_calls or not success_puts:
             self.set_recommended_qty_backup(
                 target_delta=target_delta + 0.1, attempt_no=attempt_no + 1
             )
 
+    def set_optimized_recommended_qty(self):
+        self.reset_options()
+        call_greeks = self.prepare_greek_frame_with_options(
+            self.prospective_calls, True
+        )
+        put_greeks = self.prepare_greek_frame_with_options(self.prospective_puts, False)
+        all_greeks = np.concatenate([call_greeks, put_greeks])
+        # At this point all_greeks has the following columns:
+        # [strike, ltp, delta, gamma, theta, vega, option]
+
+        # Hardcoded gamma scaler 1000 since we are optimizing theta which is very high relative to gamma
+        all_greeks[:, 3] = all_greeks[:, 3] * 1000
+
+        prob, weights = delta_neutral_optimization_lp(
+            all_greeks[:, 2:6]
+        )  # Using delta, gamma, theta, vega
+
+        if prob.status != 1:
+            logger.warning(
+                f"Optimization failed with status {LpStatus[prob.status]}. "
+                f"Check earlier messages from logs for more details."
+            )
+            raise Exception(f"Optimization failed with status {LpStatus[prob.status]}")
+
+        # noinspection PyUnboundLocalVariable
+        for option, weight in zip(all_greeks[:, -1], weights):
+            option.recommended_qty = round_shares_to_lot_size(
+                weight * self.base_exposure_qty, option.lot_size
+            )
+
     def set_recommended_qty(self, target_delta: float, optimized: bool) -> None:
         if optimized:
             try:
                 self.set_optimized_recommended_qty()
             except Exception as e:
                 notifier(
                     f"{self.underlying.name} Error while setting optimized recommended qty: {e}\n"
@@ -917,14 +949,21 @@
                     "premium_received": option.premium_received,
                     "current_ltp": option.current_ltp,
                     "current_greeks": option.current_greeks.as_dict(),
                 }
                 for option in self.active_put_options
             ],
             "aggregate_greeks": self.aggregate_greeks().as_dict(),
+            "total_premium_received": sum(
+                [option.premium_received for option in self.active_options]
+            ),
+            "total_premium_outstanding": sum(
+                [option.premium_outstanding for option in self.active_options]
+            ),
+            "mtm": sum([option.mtm for option in self.active_options]),
             "exit_triggers": self.exit_triggers,
         }
 
         load_combine_save_json_data(position_status, file_path, default_structure=list)
 
 
 def generate_optimized_result(
@@ -1241,150 +1280,14 @@
 
     return {
         strangle: (max(np.abs(deltas[strangle])) / min(np.abs(deltas[strangle])))
         for strangle in deltas
     }
 
 
-def is_in_final_stage(
-    underlying: Index,
-    strangle: Strangle,
-    itm_steps: int,
-) -> bool:
-    """Equal delta helper function"""
-    return (strangle.put_strike - strangle.call_strike) == (itm_steps * underlying.base)
-
-
-def check_for_universal_exit(
-    strangle: Strangle,
-    call_avg: float,
-    put_avg: float,
-    final_sl: float,
-    final_stage: bool,
-) -> bool:
-    """Equal delta helper function"""
-    if final_stage:
-        move = check_for_move(strangle, call_avg, put_avg, final_sl)
-        if move:
-            return True
-        else:
-            return False
-    else:
-        return False
-
-
-def check_for_move(
-    strangle: Strangle, call_avg: float, put_avg: float, sl: float
-) -> bool | Option:
-    """Equal delta helper function"""
-    call_ltp, put_ltp = strangle.fetch_ltp()
-    call_move = (call_ltp / call_avg) - 1
-    put_move = (put_ltp / put_avg) - 1
-    if call_move > sl:
-        return strangle.put_option
-    elif put_move > sl:
-        return strangle.call_option
-    else:
-        return False
-
-
-def identify_new_option(
-    underlying: Index, strangle: Strangle, option_to_buy: Option
-) -> bool | Option:
-    """Equal delta helper function"""
-    counter_part = (
-        strangle.put_option
-        if option_to_buy.option_type == OptionType.CALL
-        else strangle.call_option
-    )
-
-    strike_range = underlying.get_active_strikes(10)
-
-    prospective_sell_options = [
-        Option(strike, option_to_buy.option_type, underlying.name, strangle.expiry)
-        for strike in strike_range
-    ]
-
-    counter_part_ltp = counter_part.fetch_ltp()
-
-    prospective_sell_options = efficient_ltp_for_options(prospective_sell_options)
-
-    # The new option should be such that its price is closest to the counterparts price
-    new_option = min(
-        prospective_sell_options,
-        key=lambda x: abs(prospective_sell_options[x] - counter_part_ltp),
-    )
-
-    return new_option
-
-
-def check_for_overlap(
-    underlying: Index, new_option: Option, strangle: Strangle, itm_steps: int
-) -> bool:
-    """Equal delta helper function"""
-    counter_part = (
-        strangle.put_option
-        if new_option.option_type == OptionType.CALL
-        else strangle.call_option
-    )
-    overlap = (
-        counter_part.strike - new_option.strike
-        if new_option.option_type == OptionType.CALL
-        else new_option.strike - counter_part.strike
-    )
-    return overlap > (
-        itm_steps * underlying.base
-    )  # Is the new option more than n steps ITM?
-
-
-def move_one_leg(
-    underlying: Index,
-    strangle: Strangle,
-    option_to_buy: Option,
-    new_option: Option,
-    number_of_lots: int,
-    strategy_tag: str,
-    notification_url: str,
-) -> tuple[Strangle, float]:
-    """Equal delta helper function"""
-    if option_to_buy == new_option:
-        notifier(
-            f"Option to buy and new option are the same. No trade required",
-            notification_url,
-        )
-        return strangle, new_option.fetch_ltp()
-
-    place_option_order_and_notify(
-        option_to_buy,
-        "BUY",
-        number_of_lots,
-        "LIMIT",
-        order_tag=strategy_tag,
-        webhook_url=notification_url,
-    )
-    _avg_price = place_option_order_and_notify(
-        new_option,
-        "SELL",
-        number_of_lots,
-        "LIMIT",
-        order_tag=strategy_tag,
-        webhook_url=notification_url,
-        return_avg_price=True,
-    )
-    call_strike, put_strike = (
-        (new_option.strike, strangle.put_strike)
-        if option_to_buy.option_type == OptionType.CALL
-        else (strangle.call_strike, new_option.strike)
-    )
-    return (
-        Strangle(call_strike, put_strike, underlying.name, strangle.expiry),
-        _avg_price,
-    )
-
-
 def calculate_pnl_for_strategy(
     data: list[dict],
     strategy_name: str,
     underlying: str = "",
     flexible_matching: bool = False,
     after_time: datetime | None = None,
 ) -> float:
@@ -1454,34 +1357,30 @@
     notifier(
         f"{underlying.name} strategy {strategy_name} exited. Total pnl: {total_pnl}. {additional_info}",
         notification_url,
         "INFO",
     )
 
 
-def load_current_straddle(
+def load_current_strangle(
     underlying_str, user_id: str, file_appendix: str
 ) -> tuple[Straddle | None, int]:
     """Load current position for a given underlying, user and strategy (file_appendix)."""
 
     # Loading current position
     trade_data = load_json_data(
         f"{user_id}\\{underlying_str}_{file_appendix}.json",
         default_structure=dict,
     )
     trade_data = trade_data.get(underlying_str, {})
-    buy_strike = trade_data.get("strike", None)
-    buy_expiry = trade_data.get("expiry", None)
+    buy_strangle = trade_data.get("strangle", None)
     buy_quantity = trade_data.get("quantity", 0)
-    buy_straddle = (
-        Straddle(strike=buy_strike, underlying=underlying_str, expiry=buy_expiry)
-        if buy_strike is not None and buy_expiry is not None
-        else None
-    )
-    return buy_straddle, buy_quantity
+    if buy_strangle:
+        buy_strangle = eval(buy_strangle)
+    return buy_strangle, buy_quantity
 
 
 def sleep_until_next_action(
     interval_minutes: int,
     exit_time: tuple[int, int],
     special_condition: Callable = lambda: False,
     tasks_to_perform: list[Callable] = None,
```

### Comparing `volstreet-7.0.4/volstreet/strategies/optimization.py` & `volstreet-7.1.0/volstreet/strategies/optimization.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,113 @@
 from scipy.optimize import minimize, dual_annealing
 import numpy as np
 from volstreet import logger, OptimizationError
+from pulp import LpProblem, LpMaximize, LpVariable, lpSum, lpDot, LpStatus, value
+
+
+def delta_neutral_optimization_lp(greeks: np.ndarray) -> tuple[LpProblem, np.ndarray]:
+
+    logger.info(f"Starting delta neutral optimization for greeks: {greeks}")
+
+    call_greeks = greeks[np.argwhere(greeks[:, 0] > 0).flatten()]
+    put_greeks = greeks[np.argwhere(greeks[:, 0] < 0).flatten()]
+
+    call_delta = call_greeks[:, 0]
+    call_gamma = call_greeks[:, 1]
+    call_theta = call_greeks[:, 2]
+
+    put_delta = put_greeks[:, 0]
+    put_gamma = put_greeks[:, 1]
+    put_theta = put_greeks[:, 2]
+
+    # Create a new LP problem
+    prob = LpProblem("Delta_Neutral_Optimization", LpMaximize)
+
+    # Define decision variables
+    x = [
+        LpVariable(f"call_{i}", cat="Continuous", upBound=1, lowBound=-1)
+        for i in range(len(call_greeks))
+    ]
+    y = [
+        LpVariable(f"put_{i}", cat="Continuous", upBound=1, lowBound=-1)
+        for i in range(len(put_greeks))
+    ]
+
+    abs_x = [
+        LpVariable(f"abs_call_{i}", cat="Continuous", upBound=1, lowBound=0)
+        for i in range(len(x))
+    ]
+    abs_y = [
+        LpVariable(f"abs_put_{i}", cat="Continuous", upBound=1, lowBound=0)
+        for i in range(len(y))
+    ]
+
+    call_total_delta = lpDot(x, call_delta)
+    call_total_theta = lpDot(x, call_theta)
+    call_total_gamma = lpDot(x, call_gamma)
+
+    put_total_delta = lpDot(y, put_delta)
+    put_total_theta = lpDot(y, put_theta)
+    put_total_gamma = lpDot(y, put_gamma)
+
+    # Set objective function
+    prob += lpSum(
+        [(call_total_theta + put_total_theta), (call_total_gamma + put_total_gamma)]
+    )
+
+    # Add constraints
+
+    # DELTA CONSTRAINTS
+    prob += lpSum([call_total_delta, put_total_delta]) <= 0.005  # Delta constraint
+    prob += lpSum([call_total_delta, put_total_delta]) >= -0.005  # Delta constraint
+
+    # QUANTITY CONSTRAINTS
+    prob += lpSum(x) == 0  # Total quantity of calls should be 0
+    prob += lpSum(y) == 0  # Total quantity of puts should be 0
+
+    for i in range(len(x)):
+        prob += abs_x[i] >= x[i]
+        prob += abs_x[i] >= -x[i]
+
+    for i in range(len(y)):
+        prob += abs_y[i] >= y[i]
+        prob += abs_y[i] >= -y[i]
+
+    prob += lpSum(abs_x) >= 1.99  # Total abs quantity of calls should be 2
+    prob += lpSum(abs_x) <= 2  # Total abs quantity of calls should be 2
+
+    prob += lpSum(abs_y) >= 1.99  # Total abs quantity of puts should be 2
+    prob += lpSum(abs_y) <= 2  # Total abs quantity of puts should be 2
+
+    # GAMMA CONSTRAINT
+
+    # Hardcoded that our gamma should be less than the 25th percentile of the gamma values
+    gamma_percentile_25_call = np.percentile(call_gamma, 25)
+    gamma_percentile_25_put = np.percentile(put_gamma, 25)
+    total_threshold = gamma_percentile_25_call + gamma_percentile_25_put
+    prob += -1 * lpSum([call_total_gamma, put_total_gamma]) <= total_threshold
+
+    # Solve the problem
+    prob.solve()
+
+    call_weights = np.array([v.varValue for v in x])
+    put_weights = np.array([v.varValue for v in y])
+
+    combined_weights = np.concatenate([call_weights, put_weights])
+
+    logger.info(
+        f"Status of optimization: {LpStatus[prob.status]}, "
+        f"Objective value: {value(prob.objective)}. "
+        f"Call Delta, Theta, Gamma: {value(call_total_delta)}, {value(call_total_theta)}, {value(call_total_gamma)}. "
+        f"Put Delta, Theta, Gamma: {value(put_total_delta)}, {value(put_total_theta)}, {value(put_total_gamma)}. "
+        f"Total Delta, Theta, Gamma: {value(call_total_delta + put_total_delta)}, "
+        f"{value(call_total_theta + put_total_theta)}, {value(call_total_gamma + put_total_gamma)}"
+    )
+
+    return prob, combined_weights
 
 
 def generate_constraints(
     deltas: np.ndarray,
     gammas: np.ndarray,
     max_delta: float,
     min_delta: float,
@@ -19,15 +122,15 @@
         {"type": "eq", "fun": lambda x: sum(x)},
         {"type": "ineq", "fun": lambda x: -np.dot(x, deltas) - min_delta},
         {"type": "ineq", "fun": lambda x: np.dot(x, deltas) + max_delta},
         {"type": "ineq", "fun": lambda x: -np.dot(x, gammas) - min_gamma},
         {"type": "ineq", "fun": lambda x: np.dot(x, gammas) + max_gamma},
         {"type": "ineq", "fun": lambda x: 2 - sum(abs(x))},
         {"type": "ineq", "fun": lambda x: sum(abs(x)) - 1.99},
-        # {"type": "ineq", "fun": lambda x: min(abs(x)) - 0.01}, commented out and using recursive optimization in practice
+        # {"type": "ineq", "fun": lambda x: min(abs(x)) - 0.01}, commented out. Using recursive optimization in practice
     ]
     return constraints if full else constraints[-1]
 
 
 def generate_x0_and_bounds(n: int):
     x0 = np.zeros(n)
     bounds = [(-1, 1) for _ in range(n)]
```

### Comparing `volstreet-7.0.4/volstreet/strategies/strats.py` & `volstreet-7.1.0/volstreet/strategies/strats.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 )
 from volstreet.strategies.helpers import (
     sleep_until_next_action,
     round_shares_to_lot_size,
     most_equal_strangle,
     DeltaPosition,
     PositionMonitor,
-    load_current_straddle,
+    load_current_strangle,
     approve_execution,
     notify_pnl,
     process_stop_loss_order_statuses,
 )
 from volstreet.strategies.error_handling import exit_on_error
 
 
@@ -443,25 +443,27 @@
     )
 
 
 @exit_on_error
 def overnight_straddle(
     underlying: Index | Stock,
     exposure: int | float,
-    strike_offset: Optional[float] = 1,
+    call_strike_offset: Optional[float] = 0.02,
+    put_strike_offset: Optional[float] = -0.02,
     take_avg_price: Optional[bool] = False,
     avg_till: Optional[tuple] = (15, 28),
     notification_url: Optional[str] = None,
     strategy_tag: Optional[str] = "Overnight straddle",
 ):
     """Rollover overnight short straddle to the next expiry.
     Args:
         underlying (Index | Stock): Underlying object.
         exposure (int | float): Exposure in rupees.
-        strike_offset (float): Strike offset from the current strike.
+        call_strike_offset (float): Call strike offset in percentage terms. eg 0.02 for 2% above current price.
+        put_strike_offset (float): Put strike offset in percentage terms. eg -0.02 for 2% below current price.
         take_avg_price (bool): Take average price of the index over 5m timeframes.
         avg_till (tuple): Time till which to average the price.
         notification_url (str): Webhook URL to send notifications.
         strategy_tag (str): Tag to identify the strategy in the notification.
     """
 
     def is_next_day_expiry(tte: float) -> bool:
@@ -540,145 +542,143 @@
     # Assigning vix
     vix = IndiaVix.fetch_ltp()
 
     # Initializing the straddle if eligible
     if eligible_for_short:
         # Assigning straddle with strike and expiry
         ltp = avg_ltp if avg_ltp else underlying.fetch_ltp()
-        sell_strike = find_strike(ltp * strike_offset, underlying.base)
+        call_strike = find_strike(ltp, base=underlying.base, offset=call_strike_offset)
+        put_strike = find_strike(ltp, base=underlying.base, offset=put_strike_offset)
         expiry_to_trade = get_expiry_to_trade_for_overnight_straddle(
             effective_time_to_expiry
         )
-        sell_straddle = Straddle(
-            strike=sell_strike, underlying=underlying.name, expiry=expiry_to_trade
+        sell_strangle = Strangle(
+            call_strike, put_strike, underlying.name, expiry_to_trade
         )
-        call_iv, put_iv, iv = sell_straddle.fetch_ivs()
+        call_iv, put_iv, iv = sell_strangle.fetch_ivs()
         iv = iv * 100
         notifier(
-            f"{underlying.name} Deploying overnight short straddle with {sell_straddle}. IV: {iv}, VIX: {vix}",
+            f"{underlying.name} Deploying overnight short straddle with {sell_strangle}. IV: {iv}, VIX: {vix}",
             notification_url,
             "INFO",
         )
     else:
-        sell_strike = None
-        expiry_to_trade = None
-        sell_straddle = None
+        sell_strangle = None
         quantity_in_lots = 0
         notifier(
             f"{underlying.name} No straddle eligible for overnight short. VIX: {vix}",
             notification_url,
             "INFO",
         )
 
     # Loading current position
-    buy_straddle, buy_quantity_in_lots = load_current_straddle(
+    buy_strangle, buy_quantity_in_lots = load_current_strangle(
         underlying_str=underlying.name,
         user_id=ActiveSession.obj.userId,
         file_appendix="overnight_positions",
     )
 
     trade_info_dict = {
         "Date": current_time().strftime("%d-%m-%Y %H:%M:%S"),
         "Underlying": underlying.name,
     }
 
     call_buy_avg, put_buy_avg = np.nan, np.nan
     call_sell_avg, put_sell_avg = np.nan, np.nan
 
     # Placing orders
-    if buy_straddle is None and sell_straddle is None:
+    if buy_strangle is None and sell_strangle is None:
         notifier(f"{underlying.name} No trade required.", notification_url, "INFO")
-    elif sell_straddle is None:  # only exiting current position
+    elif sell_strangle is None:  # only exiting current position
         notifier(
-            f"{underlying.name} Exiting current position on {buy_straddle}.",
+            f"{underlying.name} Exiting current position on {buy_strangle}.",
             notification_url,
             "INFO",
         )
         execution_details = execute_instructions(
             {
-                buy_straddle: {
+                buy_strangle: {
                     "action": Action.BUY,
                     "quantity_in_lots": buy_quantity_in_lots,
                     "order_tag": strategy_tag,
                 }
             }
         )
-        call_buy_avg, put_buy_avg = execution_details[buy_straddle]
+        call_buy_avg, put_buy_avg = execution_details[buy_strangle]
 
-    elif buy_straddle is None:  # only entering new position
+    elif buy_strangle is None:  # only entering new position
         notifier(
-            f"{underlying.name} Entering new position on {sell_straddle}.",
+            f"{underlying.name} Entering new position on {buy_strangle}.",
             notification_url,
             "INFO",
         )
         execution_details = execute_instructions(
             {
-                sell_straddle: {
+                sell_strangle: {
                     "action": Action.SELL,
                     "quantity_in_lots": quantity_in_lots,
                     "order_tag": strategy_tag,
                 }
             }
         )
-        call_sell_avg, put_sell_avg = execution_details[sell_straddle]
+        call_sell_avg, put_sell_avg = execution_details[sell_strangle]
 
     else:  # both entering and exiting positions
-        if buy_straddle == sell_straddle:
+        if buy_strangle == sell_strangle:
             notifier(
                 f"{underlying.name} Same straddle. No trade required.",
                 notification_url,
                 "INFO",
             )
-            call_ltp, put_ltp = sell_straddle.fetch_ltp()
+            call_ltp, put_ltp = sell_strangle.fetch_ltp()
             call_buy_avg, put_buy_avg, call_sell_avg, put_sell_avg = (
                 call_ltp,
                 put_ltp,
                 call_ltp,
                 put_ltp,
             )
         else:
             notifier(
-                f"{underlying.name} Buying {buy_straddle} and selling {sell_straddle}.",
+                f"{underlying.name} Buying {buy_strangle} and selling {sell_strangle}.",
                 notification_url,
                 "INFO",
             )
             execution_details = execute_instructions(
                 {
-                    buy_straddle: {
+                    buy_strangle: {
                         "action": Action.BUY,
                         "quantity_in_lots": buy_quantity_in_lots,
                         "order_tag": strategy_tag,
                     },
-                    sell_straddle: {
+                    sell_strangle: {
                         "action": Action.SELL,
                         "quantity_in_lots": quantity_in_lots,
                         "order_tag": strategy_tag,
                     },
                 }
             )
-            call_buy_avg, put_buy_avg = execution_details[buy_straddle]
-            call_sell_avg, put_sell_avg = execution_details[sell_straddle]
+            call_buy_avg, put_buy_avg = execution_details[buy_strangle]
+            call_sell_avg, put_sell_avg = execution_details[sell_strangle]
 
     trade_info_dict.update(
         {
-            "Buy Straddle": buy_straddle,
+            "Buy Straddle": buy_strangle,
             "Buy Call Price": call_buy_avg,
             "Buy Put Price": put_buy_avg,
             "Buy Total Price": call_buy_avg + put_buy_avg,
-            "Sell Straddle": sell_straddle,
+            "Sell Straddle": sell_strangle,
             "Sell Call Price": call_sell_avg,
             "Sell Put Price": put_sell_avg,
             "Sell Total Price": call_sell_avg + put_sell_avg,
         }
     )
 
     trade_data = {
         underlying.name: {
-            "strike": sell_strike,
-            "expiry": expiry_to_trade,
+            "strangle": sell_strangle,
             "quantity": quantity_in_lots,
         }
     }
     save_json_data(
         trade_data,
         f"{ActiveSession.obj.userId}\\{underlying.name}_overnight_positions.json",
     )  # Currently overwriting the file with the new data. Can be changed to use load_combine_save_json_data
@@ -786,15 +786,15 @@
             f"{underlying.name} not eligible for biweekly straddle since it is not expiry day",
             notification_url,
             "INFO",
         )
         return
 
     # Loading current position
-    buy_straddle = load_current_straddle(
+    buy_straddle = load_current_strangle(
         underlying_str=underlying.name,
         user_id=ActiveSession.obj.userId,
         file_appendix="biweekly_position",
     )
 
     # Initializing new position
     ltp = underlying.fetch_ltp()
@@ -826,15 +826,15 @@
         "order_tag": strategy_tag,
     }
 
     execution_details = execute_instructions(order_instructions)
     call_sell_avg, put_sell_avg = execution_details[sell_straddle]
     call_buy_avg, put_buy_avg = execution_details.get(buy_straddle, (np.nan, np.nan))
 
-    position_to_save = {underlying.name: {"strike": strike, "expiry": expiry}}
+    position_to_save = {underlying.name: {"strangle": sell_straddle}}
     save_json_data(
         position_to_save,
         f"{ActiveSession.obj.userId}\\{underlying.name}_biweekly_position.json",
     )  # Currently overwriting the file with the new data. Can use load_combine_save_json_data in the future
     # to append the new data to the existing data. (Use case: multiple indices using the same file)
 
     trade_info_dict = {
```

### Comparing `volstreet-7.0.4/volstreet/trade_interface/instruments.py` & `volstreet-7.1.0/volstreet/trade_interface/instruments.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,16 +57,16 @@
             self.underlying, self.expiry, self.strike, self.option_type.value
         )
         self.lot_size = get_lot_size(self.underlying, expiry=self.expiry)
         _set_underlying_attributes(self, self.underlying)
 
     def __repr__(self):
         return (
-            f"{self.__class__.__name__}(strike={self.strike}, option_type={self.option_type.value}, "
-            f"underlying={self.underlying}, expiry={self.expiry})"
+            f"{self.__class__.__name__}(strike={self.strike}, option_type='{self.option_type.value}', "
+            f"underlying='{self.underlying}', expiry='{self.expiry}')"
         )
 
     def __hash__(self):
         return hash((self.strike, self.option_type.value, self.underlying, self.expiry))
 
     def __eq__(self, other):
         if not isinstance(other, _Option):
@@ -302,16 +302,16 @@
         self.call_symbol, self.call_token = self.call_option.fetch_symbol_token()
         self.put_symbol, self.put_token = self.put_option.fetch_symbol_token()
         self.lot_size = self.call_option.lot_size
         _set_underlying_attributes(self, self.underlying)
 
     def __repr__(self):
         return (
-            f"{self.__class__.__name__}(callstrike={self.call_option.strike}, putstrike={self.put_option.strike}, "
-            f"underlying={self.underlying}, expiry={self.expiry})"
+            f"{self.__class__.__name__}(call_strike={self.call_option.strike}, put_strike={self.put_option.strike}, "
+            f"underlying='{self.underlying}', expiry='{self.expiry}')"
         )
 
     def __hash__(self):
         return hash((self.call_strike, self.put_strike, self.underlying, self.expiry))
 
     def __eq__(self, other):
         return (
```

### Comparing `volstreet-7.0.4/volstreet/trade_interface/order_execution.py` & `volstreet-7.1.0/volstreet/trade_interface/order_execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/trade_interface/order_placement.py` & `volstreet-7.1.0/volstreet/trade_interface/order_placement.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/trade_interface/underlyings.py` & `volstreet-7.1.0/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/utils/change_config.py` & `volstreet-7.1.0/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/utils/communication.py` & `volstreet-7.1.0/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/utils/core.py` & `volstreet-7.1.0/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/utils/data_io.py` & `volstreet-7.1.0/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/utils/scrip_processing.py` & `volstreet-7.1.0/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/vectorized_blackscholes.py` & `volstreet-7.1.0/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/vslogging/formatters.py` & `volstreet-7.1.0/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/vslogging/logging_config.json` & `volstreet-7.1.0/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/vslogging/logging_setup.py` & `volstreet-7.1.0/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet/vslogging/parsing.py` & `volstreet-7.1.0/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.0.4/volstreet.egg-info/PKG-INFO` & `volstreet-7.1.0/volstreet.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.0.4
+Version: 7.1.0
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -13,14 +13,15 @@
 Requires-Dist: BeautifulSoup4<5.0,>=4.12.3
 Requires-Dist: eod<1.0,>=0.2.1
 Requires-Dist: fuzzywuzzy<1.0,>=0.18.0
 Requires-Dist: joblib<2.0,>=1.3.2
 Requires-Dist: logzero<2.0,>=1.7.0
 Requires-Dist: numpy<2.0,>=1.26.4
 Requires-Dist: pandas<3.0,>=2.0.1
+Requires-Dist: pulp<3.0,>=2.8.0
 Requires-Dist: pyotp<3.0,>=2.8.0
 Requires-Dist: python-Levenshtein<1.0,>=0.25.0
 Requires-Dist: requests<3.0,>=2.28.2
 Requires-Dist: scikit-learn<2.0,>=1.2.2
 Requires-Dist: scipy<2.0,>=1.12.0
 Requires-Dist: six<2.0,>=1.16.0
 Requires-Dist: smartapi-python<1.5.0,>=1.4.7
```

### Comparing `volstreet-7.0.4/volstreet.egg-info/SOURCES.txt` & `volstreet-7.1.0/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

