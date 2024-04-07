# Comparing `tmp/triple-barrier-0.4.2rc0.tar.gz` & `tmp/triple-barrier-0.4.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triple-barrier-0.4.2rc0.tar", last modified: Wed Mar 27 16:05:22 2024, max compression
+gzip compressed data, was "triple-barrier-0.4.3rc0.tar", last modified: Sun Apr  7 23:57:01 2024, max compression
```

## Comparing `triple-barrier-0.4.2rc0.tar` & `triple-barrier-0.4.3rc0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mchiuminatto  (1000) mchiuminatto  (1000)        0 2024-03-27 16:05:22.735878 triple-barrier-0.4.2rc0/
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     1077 2024-02-25 14:27:49.000000 triple-barrier-0.4.2rc0/LICENSE
--rw-r--r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     5043 2024-03-27 16:05:22.731878 triple-barrier-0.4.2rc0/PKG-INFO
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     4311 2024-03-27 16:01:36.000000 triple-barrier-0.4.2rc0/README.md
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)      886 2024-03-27 16:01:36.000000 triple-barrier-0.4.2rc0/pyproject.toml
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)       38 2024-03-27 16:05:22.735878 triple-barrier-0.4.2rc0/setup.cfg
-drwxrwxr-x   0 mchiuminatto  (1000) mchiuminatto  (1000)        0 2024-03-27 16:05:22.731878 triple-barrier-0.4.2rc0/triple_barrier/
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)        0 2024-02-11 20:42:31.000000 triple-barrier-0.4.2rc0/triple_barrier/__init__.py
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)      440 2024-03-27 00:02:18.000000 triple-barrier-0.4.2rc0/triple_barrier/constants.py
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     6001 2024-03-27 00:02:18.000000 triple-barrier-0.4.2rc0/triple_barrier/multi_barrier_box.py
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     1142 2024-03-27 00:02:18.000000 triple-barrier-0.4.2rc0/triple_barrier/multi_barrier_types.py
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     8495 2024-03-27 00:02:18.000000 triple-barrier-0.4.2rc0/triple_barrier/plots.py
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)    10668 2024-03-27 00:02:18.000000 triple-barrier-0.4.2rc0/triple_barrier/triple_barrier.py
-drwxrwxr-x   0 mchiuminatto  (1000) mchiuminatto  (1000)        0 2024-03-27 16:05:22.731878 triple-barrier-0.4.2rc0/triple_barrier.egg-info/
--rw-r--r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     5043 2024-03-27 16:05:22.000000 triple-barrier-0.4.2rc0/triple_barrier.egg-info/PKG-INFO
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)      407 2024-03-27 16:05:22.000000 triple-barrier-0.4.2rc0/triple_barrier.egg-info/SOURCES.txt
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)        1 2024-03-27 16:05:22.000000 triple-barrier-0.4.2rc0/triple_barrier.egg-info/dependency_links.txt
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)       84 2024-03-27 16:05:22.000000 triple-barrier-0.4.2rc0/triple_barrier.egg-info/requires.txt
--rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)       15 2024-03-27 16:05:22.000000 triple-barrier-0.4.2rc0/triple_barrier.egg-info/top_level.txt
+drwxrwxr-x   0 mchiuminatto  (1000) mchiuminatto  (1000)        0 2024-04-07 23:57:01.630569 triple-barrier-0.4.3rc0/
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     1077 2024-02-25 14:27:49.000000 triple-barrier-0.4.3rc0/LICENSE
+-rw-r--r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     5439 2024-04-07 23:57:01.630569 triple-barrier-0.4.3rc0/PKG-INFO
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     4707 2024-04-07 23:54:58.000000 triple-barrier-0.4.3rc0/README.md
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)      886 2024-04-07 23:36:42.000000 triple-barrier-0.4.3rc0/pyproject.toml
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)       38 2024-04-07 23:57:01.630569 triple-barrier-0.4.3rc0/setup.cfg
+drwxrwxr-x   0 mchiuminatto  (1000) mchiuminatto  (1000)        0 2024-04-07 23:57:01.630569 triple-barrier-0.4.3rc0/triple_barrier/
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)        0 2024-02-11 20:42:31.000000 triple-barrier-0.4.3rc0/triple_barrier/__init__.py
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)      440 2024-03-27 00:02:18.000000 triple-barrier-0.4.3rc0/triple_barrier/constants.py
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     6144 2024-04-07 21:26:52.000000 triple-barrier-0.4.3rc0/triple_barrier/orders.py
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     8325 2024-04-07 23:42:21.000000 triple-barrier-0.4.3rc0/triple_barrier/plots.py
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)    10587 2024-04-07 21:43:14.000000 triple-barrier-0.4.3rc0/triple_barrier/trade_labeling.py
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     1173 2024-04-07 23:39:30.000000 triple-barrier-0.4.3rc0/triple_barrier/types.py
+drwxrwxr-x   0 mchiuminatto  (1000) mchiuminatto  (1000)        0 2024-04-07 23:57:01.630569 triple-barrier-0.4.3rc0/triple_barrier.egg-info/
+-rw-r--r--   0 mchiuminatto  (1000) mchiuminatto  (1000)     5439 2024-04-07 23:57:01.000000 triple-barrier-0.4.3rc0/triple_barrier.egg-info/PKG-INFO
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)      382 2024-04-07 23:57:01.000000 triple-barrier-0.4.3rc0/triple_barrier.egg-info/SOURCES.txt
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)        1 2024-04-07 23:57:01.000000 triple-barrier-0.4.3rc0/triple_barrier.egg-info/dependency_links.txt
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)       84 2024-04-07 23:57:01.000000 triple-barrier-0.4.3rc0/triple_barrier.egg-info/requires.txt
+-rw-rw-r--   0 mchiuminatto  (1000) mchiuminatto  (1000)       15 2024-04-07 23:57:01.000000 triple-barrier-0.4.3rc0/triple_barrier.egg-info/top_level.txt
```

### Comparing `triple-barrier-0.4.2rc0/LICENSE` & `triple-barrier-0.4.3rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `triple-barrier-0.4.2rc0/PKG-INFO` & `triple-barrier-0.4.3rc0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triple-barrier
-Version: 0.4.2rc0
+Version: 0.4.3rc0
 Summary: Back-testing and machine learning pipelines trades labeling utility
 Author-email: Marcello Chiuminatto <mch@thequantick.net>
 Project-URL: Homepage, https://github.com/mchiuminatto/triple_barrier
 Project-URL: Issues, https://github.com/mchiuminatto/triple_barrier/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,99 +19,120 @@
 
 # WARNING:
 
 This is a work in progress DO NOT USE IT FOR PRODUCTION PURPOSES
 
 # Overview
 
-Triple Barrier is a trade labeler that con be used in the context of back-testing or machine learning trading and
-validating process. It records for each trade when, at what price level and why a trade was closed.
+Triple Barrier is a trade labeler that can be used for algorithmic trading back-testing or machine learning training and
+validating pipelines. It records for each trade when, at what price level and why a position was closed.
 
 ![](./docs/images/trades-table.png)
 
-Includes features to plot the triple for a particular trade and the closing event:
+It includes features to plot the triple for a particular trade and the closing event:
 
 ![](./docs/images/trade_example_1.png)
 
 Other features:
 
 - Built
-  upon [pandas](https://pandas.pydata.org/), [numpy](https://numpy.org/), [mplfinance](https://github.com/matplotlib/mplfinance).
-- Works semi vectorized, meaning that can be used with a pandas apply function.
+  upon [pandas](https://pandas.pydata.org/), [numpy](https://numpy.org/), [matplotlib](https://matplotlib.org/) [mplfinance](https://github.com/matplotlib/mplfinance).
+- It can be used to label single trades or semi vectorized, meaning that can be used with a pandas apply function.
 
 ## Why?
 
-This project emerges from repeated trading strategy back-testing process where I was caught again and again copying and
-pasting from previous pipelines the code to perform a vectorized (semi-vectorized to be more accurate) labeling of
-trades. To avoid this DRY routine is that I decide to move this code to a library.
+This project emerges from a repeated trading strategy back-testing process where I was caught again and again copying 
+and pasting from previous pipelines the code to perform a vectorized (semi-vectorized to be more accurate) labeling of 
+trades. To avoid this DRY (Do not Repeat Yourself) routine, that is why I decided to move this code to a library.
 
-The name and core idea is inspired in an algorithm found in the book: Advances in Financial Machine Learning, by Marcos
+The name and core idea were inspired by an algorithm found in the book: Advances in Financial Machine Learning, by Marcos
 Lopez de Prado.
 
-Before going moving further into library details a little bit of context.
+Before moving further into the library details a little bit of context.
 
 ### Trading Strategies
 
-A trading strategy describes the logic for opening trades, managing and closing positions.
+A trading strategy describes the logic for opening, managing and closing positions.
 
-Depending on the trading strategy, after a position is opened, four events will determine how the position ends:
+Depending on the trading strategy, once a position is opened, four events can determine how the position ends:
 
 1. Stop loss hit: The price hit the stop loss, which is the maximum tolerable loss (Limit Order)
 2. Take profit hit: The price hit the take profit, which is the estimated maximum profit the position can reach (Limit
    Order)
 3. Expiration time reached: The position has reached a specific expiration time (Good Til Time or GTT orders)
-4. A custom condition: Any custom condition that can maximize the position profit. These conditions depend on price
-   action whuile the position is opened
+4. A custom condition: Any custom condition that can trigger the position closing. These conditions depend on price
+   action while the position is opened
 
 ![](./docs/images/triple-barrier-long.png)
 
-To determine if strategy is potentially profitable before live trading, it is necessary to collect a large sample of
-trades to
-analyze the effectiveness of the strategy in terms of profits, mean profits, profits distributions, draw-downs or any
-metric you prefer.
+To determine if a strategy is potentially profitable before live trading, it is necessary to collect a large sample of
+trades to analyze the effectiveness of the strategy in terms of profits, mean profits, profits distributions, drawdowns
+or any metric you prefer.
 
 Doing this analysis process manually is not recommended at all, considering the amount of data you need to analyze, the
 volume of trades required to determine if the strategy is significantly profitable and the human error, to name a few
-reasons. Suppose you have
-ten trading strategy models, each one with ten permutations of parameter values (this can lead to over-fitting, I know)
-and
-suppose you want to collect samples over ten years at a frequency (time-frame) of 5 minutes, impossible, isn't it?
+reasons. 
 
-## Enter Algorithmic Trading
+## Algorithmic Trading and Triple Barrier
 
-In simple terms, through algorithmic trading is using software to automate all the process described above: Open, manage
+In simple terms, algorithmic trading is using software to automate all the processes described above: Open, manage
 and Close trading positions.
 
 But before running live a trading algorithm that implements a trading model you need to perform some research and
-analyze the algorithm behavior on historic data to understand whether the algorithm is able to generalize and
-potentially behave similarly on unseen or future data, this process is called back-testing.
+analyze the algorithm behavior on historic data to understand whether the algorithm is able to generalize well and
+ behave similarly on unseen or future data, this process is called back-testing.
 
-Is in back-testing where you need to identify: when positions where opened, when and why they were closed.
+Is in back-testing where you need to identify: when positions were opened, when and why they were closed, so you can 
+calculate all required performance metrics and that is why Triple Barrier was built for.
 
-## Enter Triple Barrier
-
-So Triple Barrier automates the recording of trades in the context of back-testing or machine learning as well
-to label trade profit/loss, closing event or any other value you can calculate from the data provided by triple barrier.
 
 ## How?
 
-For now please refer to the tests to understand how triple barrier works:
+### How to install
+
+```commandline
+pip install triple-barrier==0.4.3rc0
+```
+
 
 [Triple barrier test](./tests/triple_barrier/integration/test_triple_barrier_apply_happy_path.py)
 
 Or to this Jupyter Notebook that combines triple barrier calculation with plotting.
 
 [Triple Barrier Jupyter Notebook](./docs/plot-method-tests.ipynb)
 
-In the future extensive amount of examples will be used.
 
 ### How to install
 
 As of now, the latest version (Release candidate) is 0.4.1rc and can be installed as follows:
 
 ```commandline
 pip install triple-barrier==0.4.2rc0
 ```
 
+### Examples
+
+This is a work in progress, but you can find some examples here:
+
+You can see use case examples in this [folder](./docs/examples)
+
+## TODO
+
+This project is its final stages of testing, documentation and CLEANing.
+
+Besides that, there are some identified tasks that need to be done before the first release.
+
+- Add string representations for some classes
+- Provide an out-of-the-box function that can be easily used by pandas apply . Currently, you need to build one.
+- Refactor list of barriers hits (OrderBoxHits.barriers) as dictionary, currently is a list which
+is not much actionable.
+- Plotting: Add possibility to plot oscillators in a panel below
+- Add trailing stops
+
+
+## Other Documentation
+
+[Uml models](./docs/models.md)
+
 # References
 
 [Why numpy is fast](https://numpy.org/doc/stable/user/whatisnumpy.html#why-is-numpy-fast)
```

### Comparing `triple-barrier-0.4.2rc0/README.md` & `triple-barrier-0.4.3rc0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,119 @@
 # WARNING:
 
 This is a work in progress DO NOT USE IT FOR PRODUCTION PURPOSES
 
 # Overview
 
-Triple Barrier is a trade labeler that con be used in the context of back-testing or machine learning trading and
-validating process. It records for each trade when, at what price level and why a trade was closed.
+Triple Barrier is a trade labeler that can be used for algorithmic trading back-testing or machine learning training and
+validating pipelines. It records for each trade when, at what price level and why a position was closed.
 
 ![](./docs/images/trades-table.png)
 
-Includes features to plot the triple for a particular trade and the closing event:
+It includes features to plot the triple for a particular trade and the closing event:
 
 ![](./docs/images/trade_example_1.png)
 
 Other features:
 
 - Built
-  upon [pandas](https://pandas.pydata.org/), [numpy](https://numpy.org/), [mplfinance](https://github.com/matplotlib/mplfinance).
-- Works semi vectorized, meaning that can be used with a pandas apply function.
+  upon [pandas](https://pandas.pydata.org/), [numpy](https://numpy.org/), [matplotlib](https://matplotlib.org/) [mplfinance](https://github.com/matplotlib/mplfinance).
+- It can be used to label single trades or semi vectorized, meaning that can be used with a pandas apply function.
 
 ## Why?
 
-This project emerges from repeated trading strategy back-testing process where I was caught again and again copying and
-pasting from previous pipelines the code to perform a vectorized (semi-vectorized to be more accurate) labeling of
-trades. To avoid this DRY routine is that I decide to move this code to a library.
+This project emerges from a repeated trading strategy back-testing process where I was caught again and again copying 
+and pasting from previous pipelines the code to perform a vectorized (semi-vectorized to be more accurate) labeling of 
+trades. To avoid this DRY (Do not Repeat Yourself) routine, that is why I decided to move this code to a library.
 
-The name and core idea is inspired in an algorithm found in the book: Advances in Financial Machine Learning, by Marcos
+The name and core idea were inspired by an algorithm found in the book: Advances in Financial Machine Learning, by Marcos
 Lopez de Prado.
 
-Before going moving further into library details a little bit of context.
+Before moving further into the library details a little bit of context.
 
 ### Trading Strategies
 
-A trading strategy describes the logic for opening trades, managing and closing positions.
+A trading strategy describes the logic for opening, managing and closing positions.
 
-Depending on the trading strategy, after a position is opened, four events will determine how the position ends:
+Depending on the trading strategy, once a position is opened, four events can determine how the position ends:
 
 1. Stop loss hit: The price hit the stop loss, which is the maximum tolerable loss (Limit Order)
 2. Take profit hit: The price hit the take profit, which is the estimated maximum profit the position can reach (Limit
    Order)
 3. Expiration time reached: The position has reached a specific expiration time (Good Til Time or GTT orders)
-4. A custom condition: Any custom condition that can maximize the position profit. These conditions depend on price
-   action whuile the position is opened
+4. A custom condition: Any custom condition that can trigger the position closing. These conditions depend on price
+   action while the position is opened
 
 ![](./docs/images/triple-barrier-long.png)
 
-To determine if strategy is potentially profitable before live trading, it is necessary to collect a large sample of
-trades to
-analyze the effectiveness of the strategy in terms of profits, mean profits, profits distributions, draw-downs or any
-metric you prefer.
+To determine if a strategy is potentially profitable before live trading, it is necessary to collect a large sample of
+trades to analyze the effectiveness of the strategy in terms of profits, mean profits, profits distributions, drawdowns
+or any metric you prefer.
 
 Doing this analysis process manually is not recommended at all, considering the amount of data you need to analyze, the
 volume of trades required to determine if the strategy is significantly profitable and the human error, to name a few
-reasons. Suppose you have
-ten trading strategy models, each one with ten permutations of parameter values (this can lead to over-fitting, I know)
-and
-suppose you want to collect samples over ten years at a frequency (time-frame) of 5 minutes, impossible, isn't it?
+reasons. 
 
-## Enter Algorithmic Trading
+## Algorithmic Trading and Triple Barrier
 
-In simple terms, through algorithmic trading is using software to automate all the process described above: Open, manage
+In simple terms, algorithmic trading is using software to automate all the processes described above: Open, manage
 and Close trading positions.
 
 But before running live a trading algorithm that implements a trading model you need to perform some research and
-analyze the algorithm behavior on historic data to understand whether the algorithm is able to generalize and
-potentially behave similarly on unseen or future data, this process is called back-testing.
+analyze the algorithm behavior on historic data to understand whether the algorithm is able to generalize well and
+ behave similarly on unseen or future data, this process is called back-testing.
 
-Is in back-testing where you need to identify: when positions where opened, when and why they were closed.
+Is in back-testing where you need to identify: when positions were opened, when and why they were closed, so you can 
+calculate all required performance metrics and that is why Triple Barrier was built for.
 
-## Enter Triple Barrier
-
-So Triple Barrier automates the recording of trades in the context of back-testing or machine learning as well
-to label trade profit/loss, closing event or any other value you can calculate from the data provided by triple barrier.
 
 ## How?
 
-For now please refer to the tests to understand how triple barrier works:
+### How to install
+
+```commandline
+pip install triple-barrier==0.4.3rc0
+```
+
 
 [Triple barrier test](./tests/triple_barrier/integration/test_triple_barrier_apply_happy_path.py)
 
 Or to this Jupyter Notebook that combines triple barrier calculation with plotting.
 
 [Triple Barrier Jupyter Notebook](./docs/plot-method-tests.ipynb)
 
-In the future extensive amount of examples will be used.
 
 ### How to install
 
 As of now, the latest version (Release candidate) is 0.4.1rc and can be installed as follows:
 
 ```commandline
 pip install triple-barrier==0.4.2rc0
 ```
 
+### Examples
+
+This is a work in progress, but you can find some examples here:
+
+You can see use case examples in this [folder](./docs/examples)
+
+## TODO
+
+This project is its final stages of testing, documentation and CLEANing.
+
+Besides that, there are some identified tasks that need to be done before the first release.
+
+- Add string representations for some classes
+- Provide an out-of-the-box function that can be easily used by pandas apply . Currently, you need to build one.
+- Refactor list of barriers hits (OrderBoxHits.barriers) as dictionary, currently is a list which
+is not much actionable.
+- Plotting: Add possibility to plot oscillators in a panel below
+- Add trailing stops
+
+
+## Other Documentation
+
+[Uml models](./docs/models.md)
+
 # References
 
 [Why numpy is fast](https://numpy.org/doc/stable/user/whatisnumpy.html#why-is-numpy-fast)
```

### Comparing `triple-barrier-0.4.2rc0/pyproject.toml` & `triple-barrier-0.4.3rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "triple-barrier"
-version = "0.4.2rc"
+version = "0.4.3rc"
 authors = [
     {name="Marcello Chiuminatto", email="mch@thequantick.net"},
 ]
 description = "Back-testing and machine learning pipelines trades labeling utility"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `triple-barrier-0.4.2rc0/triple_barrier/multi_barrier_types.py` & `triple-barrier-0.4.3rc0/triple_barrier/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from datetime import datetime
 
 
-class BarrierType(Enum):
+class OrderType(Enum):
     TAKE_PROFIT = "take-profit"
     STOP_LOSS = "stop-loss"
-    TIME_BARRIER = "time-barrier"
+    TIME_EXPIRATION = "time-expiration"
     DYNAMIC = "dynamic"
 
 
 class ExitType(Enum):
     TAKE_PROFIT_HIT = "take-profit-hit"
     STOP_LOSS_HIT = "stop-loss-hit"
     TIME_BARRIER_HIT = "tme-barrier-hit"
@@ -17,31 +17,33 @@
 
 
 class TradeSide(Enum):
     BUY = 1
     SELL = -1
 
 
-class BarrierHit:
+class OrderHit:
 
     def __init__(self,
                  level: float | None = None,
                  hit_datetime: datetime | None = None,
-                 barrier_type: BarrierType | None = None
+                 order_type: OrderType | None = None
                  ):
         self.level: float = level
         self.hit_datetime: datetime = hit_datetime
-        self.barrier_type: BarrierType = barrier_type
+        self.order_type: OrderType = order_type
 
     def __str__(self):
         output: str = f"""
-        Datetime: {self.hit_datetime} 
-        Level: {self.level} 
-        Type: {self.barrier_type.value}
+        Datetime: {self.hit_datetime}
+        Level: {self.level}
+        Type: {self.order_type.value}
         """
         return output
 
 
-class MultiBarrierHit:
+class OrderBoxHits:
     def __init__(self) -> None:
-        self.barriers: list[BarrierHit] = []
-        self.first_hit: BarrierHit = BarrierHit()
+        self.barriers: list[OrderHit] = []
+        self.first_hit: OrderHit = OrderHit()
+
+    # TODO: Implement a good string representation
```

### Comparing `triple-barrier-0.4.2rc0/triple_barrier/plots.py` & `triple-barrier-0.4.3rc0/triple_barrier/plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import numpy as np
 import pandas as pd
 
 import matplotlib.pyplot as plt
 import mplfinance as mpf
 
-from triple_barrier.triple_barrier import BarrierHit
-from triple_barrier.triple_barrier import MultiBarrier
+from triple_barrier.trade_labeling import OrderHit
+from triple_barrier.trade_labeling import Labeler
 
 from triple_barrier import constants
 
 
 class PlotTripleBarrier:
 
     def __init__(self,
@@ -50,33 +50,33 @@
                              "high": high_price,
                              "low": low_price,
                              "close": close_price},
                             columns=["open", "high", "low", "close"])
         return ohlc
 
     def plot_multi_barrier(self,
-                           multi_barrier: MultiBarrier):
+                           multi_barrier: Labeler):
         self._plot(
             entry_period=multi_barrier.multi_barrier_box.open_datetime,
             take_profit_level=multi_barrier.multi_barrier_box.take_profit,
             stop_loss_level=multi_barrier.multi_barrier_box.stop_loss,
             time_barrier_datetime=multi_barrier.multi_barrier_box.time_limit,
             periods_to_plot=self._periods_to_plot,
             dynamic_exit_price=None,
-            closing_event=multi_barrier.multi_barrier_hit.first_hit
+            closing_event=multi_barrier.orders_hit.first_hit
         )
 
     def _plot(self,
               entry_period: datetime,
               take_profit_level: float,
               stop_loss_level: float,
               time_barrier_datetime: datetime,
               periods_to_plot: int = 50,
               dynamic_exit_price: float | None = None,
-              closing_event: BarrierHit | None = None
+              closing_event: OrderHit | None = None
               ):
 
         date_from: datetime = entry_period
         date_to: datetime = self.ohlc[entry_period:].index[periods_to_plot - 1]
 
         if len(self.ohlc[date_from: date_to]) == 0:
             raise ValueError("No data to process")
@@ -120,21 +120,21 @@
         plt.show()
 
         # TODO: store binary image in a file to compare with a stored one for testing purposes
 
     def _add_closing_event_hit(self,
                                date_from: datetime,
                                date_to: datetime,
-                               closing_event: BarrierHit) -> dict:
+                               closing_event: OrderHit) -> dict:
 
         # move this logic to a function that returns the make_addplot object
         self.ohlc["temp-dynamic"] = np.nan
-        high = self.ohlc.loc[closing_event.hit_datetime, "high"] + (
-                self.ohlc.loc[closing_event.hit_datetime, "high"] -
-                self.ohlc.loc[closing_event.hit_datetime, "low"]) * 1.05
+        high = (self.ohlc.loc[closing_event.hit_datetime, "high"]
+                + (self.ohlc.loc[closing_event.hit_datetime, "high"]
+                   - self.ohlc.loc[closing_event.hit_datetime, "low"]) * 1.05)
         self.ohlc.loc[closing_event.hit_datetime, "temp-dynamic"] = high
 
         return mpf.make_addplot(self.ohlc[date_from: date_to]["temp-dynamic"],
                                 type="scatter",
                                 marker="v",
                                 markersize=75,
                                 color="red"
@@ -150,19 +150,19 @@
         open_price: float = barrier[constants.OPEN_PRICE]
         time_limit: datetime = barrier[constants.TIME_LIMIT]
         dynamic_close: float = barrier[constants.DYNAMIC_CLOSE]
 
         top_line_level: float = max(take_profit, stop_loss, -float("inf") if dynamic_close is None else dynamic_close)
         bottom_line_level: float = min(take_profit, stop_loss, float("inf") if dynamic_close is None else dynamic_close)
 
-        take_profit_line: list[tuple, tuple] = [(date_from, take_profit), (time_limit, take_profit)]
-        stop_loss_line: list[tuple, tuple] = [(date_from, stop_loss), (time_limit, stop_loss)]
-        open_vertical_line: list[tuple, tuple] = [(date_from, bottom_line_level), (date_from, top_line_level)]
-        time_barrier_vertical_line: list[tuple, tuple] = [(time_limit, bottom_line_level), (time_limit, top_line_level)]
-        open_line: list[tuple, tuple] = [(date_from, open_price), (time_limit, open_price)]
+        take_profit_line: list = [(date_from, take_profit), (time_limit, take_profit)]
+        stop_loss_line: list = [(date_from, stop_loss), (time_limit, stop_loss)]
+        open_vertical_line: list = [(date_from, bottom_line_level), (date_from, top_line_level)]
+        time_barrier_vertical_line: list = [(time_limit, bottom_line_level), (time_limit, top_line_level)]
+        open_line: list = [(date_from, open_price), (time_limit, open_price)]
 
         barrier_lines = [
             take_profit_line,
             stop_loss_line,
             time_barrier_vertical_line,
             open_vertical_line,
             open_line
@@ -189,15 +189,14 @@
         font = {"family": "serif",
                 "color": "black",
                 "weight": "normal",
                 "size": 10,
                 "backgroundcolor": "white"
                 }
 
-        last_index: int = self.ohlc.index.get_loc(barrier[constants.TIME_LIMIT])
         time_limit_index = self.ohlc[date_from:date_to].index.get_loc(barrier[constants.TIME_LIMIT]) + 1
         axis[0].text(time_limit_index,
                      barrier[constants.OPEN_PRICE],
                      "open",
                      fontdict=font)
 
         font["color"] = "green"
```

### Comparing `triple-barrier-0.4.2rc0/triple_barrier/triple_barrier.py` & `triple-barrier-0.4.3rc0/triple_barrier/trade_labeling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,120 @@
 from datetime import datetime
-from enum import Enum
 
 import pandas as pd
 import numpy as np
 
 from triple_barrier import constants
-from triple_barrier.multi_barrier_box import BoxBuilder
-from triple_barrier.multi_barrier_box import MultiBarrierParameters
-from triple_barrier.multi_barrier_box import MultiBarrierBox
-from triple_barrier.multi_barrier_types import MultiBarrierHit
-from triple_barrier.multi_barrier_types import BarrierHit
-from triple_barrier.multi_barrier_types import BarrierType
-from triple_barrier.multi_barrier_types import TradeSide
+from triple_barrier.orders import BoxBuilder
+from triple_barrier.orders import Orders
+from triple_barrier.orders import OrdersBox
+from triple_barrier.types import OrderBoxHits
+from triple_barrier.types import OrderHit
+from triple_barrier.types import OrderType
+from triple_barrier.types import TradeSide
 
 
-class MultiBarrier:
+class Labeler:
 
     def __init__(self,
                  open_price: pd.Series,
                  high_price: pd.Series,
                  low_price: pd.Series,
                  close_price: pd.Series,
-                 box_setup: MultiBarrierParameters,
+                 box_setup: Orders,
                  dynamic_exit: pd.Series | None = None
                  ) -> None:
 
         self.open: pd.Series = open_price
         self.high: pd.Series = high_price
         self.low: pd.Series = low_price
         self.close: pd.Series = close_price
         self.dynamic_exit: pd.Series = dynamic_exit
 
         box_builder: BoxBuilder = BoxBuilder()
-        self.multi_barrier_box: MultiBarrierBox = box_builder.build_multi_barrier_box(box_setup)
+        self.multi_barrier_box: OrdersBox = box_builder.build_multi_barrier_box(box_setup)
 
-        self.multi_barrier_hit: MultiBarrierHit = MultiBarrierHit()
+        self.orders_hit: OrderBoxHits = OrderBoxHits()
+
+        self._take_profit_barrier: TakeProfit | None = None
+        self._stop_loss_barrier: StopLoss | None = None
+        self._time_barrier: TimeBarrier | None = None
+        self._dynamic_barrier: DynamicOrder | None = None
+
+        self._do_initializations()
+
+    def _do_initializations(self):
+        self._take_profit_barrier = TakeProfit(open_price=self.open,
+                                               high_price=self.high,
+                                               low_price=self.low,
+                                               close_price=self.close,
+                                               open_datetime=self.multi_barrier_box.open_datetime,
+                                               trade_side=self.multi_barrier_box.trade_side,
+                                               pip_decimal_position=self.multi_barrier_box.pip_decimal_position,
+                                               take_profit=self.multi_barrier_box.take_profit
+                                               )
+        self._stop_loss_barrier = StopLoss(open_price=self.open,
+                                           high_price=self.high,
+                                           low_price=self.low,
+                                           close_price=self.close,
+                                           open_datetime=self.multi_barrier_box.open_datetime,
+                                           trade_side=self.multi_barrier_box.trade_side,
+                                           pip_decimal_position=self.multi_barrier_box.pip_decimal_position,
+                                           stop_loss=self.multi_barrier_box.stop_loss
+                                           )
+        self._time_barrier = TimeBarrier(open_price=self.open,
+                                         time_limit_date=self.multi_barrier_box.time_limit,
+                                         open_datetime=self.multi_barrier_box.open_datetime
+                                         )
+        self._dynamic_barrier = DynamicOrder(open_price=self.open,
+                                             exit_signals=self.dynamic_exit,
+                                             open_datetime=self.multi_barrier_box.open_datetime
+                                             )
 
     def compute(self):
         try:
             self._compute_take_profit_barrier()
             self._compute_stop_loss_barrier()
             self._compute_time_barrier()
             if self.dynamic_exit is not None:
                 self._compute_dynamic_barrier()
             self._select_first_hit()
-            return self.multi_barrier_hit
+            return self.orders_hit
         except Exception as error_instance:
             raise Exception(str(error_instance))
 
     def _compute_take_profit_barrier(self):
-        take_profit_barrier: TakeProfit = TakeProfit(open_price=self.open,
-                                                     high_price=self.high,
-                                                     low_price=self.low,
-                                                     close_price=self.close,
-                                                     open_datetime=self.multi_barrier_box.open_datetime,
-                                                     trade_side=self.multi_barrier_box.trade_side,
-                                                     pip_decimal_position=self.multi_barrier_box.pip_decimal_position,
-                                                     take_profit=self.multi_barrier_box.take_profit
-                                                     )
-        take_profit_barrier.compute()
-        self.multi_barrier_hit.barriers.append(take_profit_barrier.barrier)
+
+        self._take_profit_barrier.compute()
+        self.orders_hit.barriers.append(self._take_profit_barrier.barrier)
 
     def _compute_stop_loss_barrier(self):
-        stop_loss_barrier: StopLoss = StopLoss(open_price=self.open,
-                                               high_price=self.high,
-                                               low_price=self.low,
-                                               close_price=self.close,
-                                               open_datetime=self.multi_barrier_box.open_datetime,
-                                               trade_side=self.multi_barrier_box.trade_side,
-                                               pip_decimal_position=self.multi_barrier_box.pip_decimal_position,
-                                               stop_loss=self.multi_barrier_box.stop_loss
-                                               )
-        stop_loss_barrier.compute()
-        self.multi_barrier_hit.barriers.append(stop_loss_barrier.barrier)
+
+        self._stop_loss_barrier.compute()
+        self.orders_hit.barriers.append(self._stop_loss_barrier.barrier)
 
     def _compute_time_barrier(self):
-        time_barrier: TimeBarrier = TimeBarrier(open_price=self.open,
-                                                time_limit_date=self.multi_barrier_box.time_limit,
-                                                open_datetime=self.multi_barrier_box.open_datetime
-                                                )
-        time_barrier.compute()
-        self.multi_barrier_hit.barriers.append(time_barrier.barrier)
+
+        self._time_barrier.compute()
+        self.orders_hit.barriers.append(self._time_barrier.barrier)
 
     def _compute_dynamic_barrier(self):
-        dynamic_barrier: DynamicBarrier = DynamicBarrier(open_price=self.open,
-                                                         exit_signals=self.dynamic_exit,
-                                                         open_datetime=self.multi_barrier_box.open_datetime
-                                                         )
-        dynamic_barrier.compute()
-        self.multi_barrier_hit.barriers.append(dynamic_barrier.barrier)
+
+        self._dynamic_barrier.compute()
+        self.orders_hit.barriers.append(self._dynamic_barrier.barrier)
 
     def _select_first_hit(self):
-        first_hit: BarrierHit | None = None
-        for barrier in self.multi_barrier_hit.barriers:
+        first_hit: OrderHit | None = None
+        for barrier in self.orders_hit.barriers:
             if first_hit is None:
                 first_hit = barrier
             else:
                 if barrier.hit_datetime < first_hit.hit_datetime:
                     first_hit = barrier
-        self.multi_barrier_hit.first_hit = first_hit
+        self.orders_hit.first_hit = first_hit
 
 
 class TakeProfit:
 
     def __init__(self,
                  open_price: pd.Series,
                  high_price: pd.Series,
@@ -118,16 +130,16 @@
         self._high_price: pd.Series = high_price
         self._low_price: pd.Series = low_price
         self._close_price: pd.Series = close_price
         self._open_datetime: datetime = open_datetime
         self._trade_side: TradeSide = trade_side
         self._pip_decimal_position: int = pip_decimal_position
 
-        self.barrier: BarrierHit = BarrierHit(barrier_type=BarrierType.TAKE_PROFIT,
-                                              level=take_profit)
+        self.barrier: OrderHit = OrderHit(order_type=OrderType.TAKE_PROFIT,
+                                          level=take_profit)
 
     def compute(self):
         self._compute_next_take_profit_hit()
 
     def _compute_next_take_profit_hit(self):
 
         hit_date: datetime | None = constants.INFINITE_DATE
@@ -166,16 +178,16 @@
         self._high_price: pd.Series = high_price
         self._low_price: pd.Series = low_price
         self._close_price: pd.Series = close_price
         self._open_datetime: datetime = open_datetime
         self._trade_side: TradeSide = trade_side
         self._pip_decimal_position: int = pip_decimal_position
 
-        self.barrier: BarrierHit = BarrierHit(barrier_type=BarrierType.STOP_LOSS,
-                                              level=stop_loss)
+        self.barrier: OrderHit = OrderHit(order_type=OrderType.STOP_LOSS,
+                                          level=stop_loss)
 
     def compute(self):
         self._compute_next_level_hit()
 
     def _compute_next_level_hit(self):
 
         hit_datetime: datetime = constants.INFINITE_DATE
@@ -202,41 +214,41 @@
     def __init__(self,
                  open_price: pd.Series,
                  time_limit_date: datetime,
                  open_datetime: datetime):
         self.open_price: pd.Series = open_price
         self.open_datetime: datetime = open_datetime
 
-        self.barrier = BarrierHit(barrier_type=BarrierType.TIME_BARRIER, hit_datetime=time_limit_date)
+        self.barrier = OrderHit(order_type=OrderType.TIME_EXPIRATION, hit_datetime=time_limit_date)
 
     def compute(self):
         self._compute_hit_level()
 
     def _compute_hit_level(self):
         hit_level: float = np.inf
 
         open_price = self.open_price[self.open_datetime:]
         if self.barrier.hit_datetime != constants.INFINITE_DATE:
             hit_level = open_price[self.barrier.hit_datetime:].iloc[1]
 
         self.barrier.level = hit_level
 
 
-class DynamicBarrier:
+class DynamicOrder:
 
     def __init__(self,
                  open_price: pd.Series,
                  exit_signals: pd.Series,
                  open_datetime: datetime,
                  ):
         self.open_price = open_price
         self.open_datetime: datetime = open_datetime
         self.exit_signals: pd.Series = exit_signals
 
-        self.barrier: BarrierHit = BarrierHit(barrier_type=BarrierType.DYNAMIC)
+        self.barrier: OrderHit = OrderHit(order_type=OrderType.DYNAMIC)
 
     def compute(self):
         self._compute_hit_datetime()
         self._compute_hit_level()
 
     def _compute_hit_datetime(self):
```

### Comparing `triple-barrier-0.4.2rc0/triple_barrier.egg-info/PKG-INFO` & `triple-barrier-0.4.3rc0/triple_barrier.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triple-barrier
-Version: 0.4.2rc0
+Version: 0.4.3rc0
 Summary: Back-testing and machine learning pipelines trades labeling utility
 Author-email: Marcello Chiuminatto <mch@thequantick.net>
 Project-URL: Homepage, https://github.com/mchiuminatto/triple_barrier
 Project-URL: Issues, https://github.com/mchiuminatto/triple_barrier/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,99 +19,120 @@
 
 # WARNING:
 
 This is a work in progress DO NOT USE IT FOR PRODUCTION PURPOSES
 
 # Overview
 
-Triple Barrier is a trade labeler that con be used in the context of back-testing or machine learning trading and
-validating process. It records for each trade when, at what price level and why a trade was closed.
+Triple Barrier is a trade labeler that can be used for algorithmic trading back-testing or machine learning training and
+validating pipelines. It records for each trade when, at what price level and why a position was closed.
 
 ![](./docs/images/trades-table.png)
 
-Includes features to plot the triple for a particular trade and the closing event:
+It includes features to plot the triple for a particular trade and the closing event:
 
 ![](./docs/images/trade_example_1.png)
 
 Other features:
 
 - Built
-  upon [pandas](https://pandas.pydata.org/), [numpy](https://numpy.org/), [mplfinance](https://github.com/matplotlib/mplfinance).
-- Works semi vectorized, meaning that can be used with a pandas apply function.
+  upon [pandas](https://pandas.pydata.org/), [numpy](https://numpy.org/), [matplotlib](https://matplotlib.org/) [mplfinance](https://github.com/matplotlib/mplfinance).
+- It can be used to label single trades or semi vectorized, meaning that can be used with a pandas apply function.
 
 ## Why?
 
-This project emerges from repeated trading strategy back-testing process where I was caught again and again copying and
-pasting from previous pipelines the code to perform a vectorized (semi-vectorized to be more accurate) labeling of
-trades. To avoid this DRY routine is that I decide to move this code to a library.
+This project emerges from a repeated trading strategy back-testing process where I was caught again and again copying 
+and pasting from previous pipelines the code to perform a vectorized (semi-vectorized to be more accurate) labeling of 
+trades. To avoid this DRY (Do not Repeat Yourself) routine, that is why I decided to move this code to a library.
 
-The name and core idea is inspired in an algorithm found in the book: Advances in Financial Machine Learning, by Marcos
+The name and core idea were inspired by an algorithm found in the book: Advances in Financial Machine Learning, by Marcos
 Lopez de Prado.
 
-Before going moving further into library details a little bit of context.
+Before moving further into the library details a little bit of context.
 
 ### Trading Strategies
 
-A trading strategy describes the logic for opening trades, managing and closing positions.
+A trading strategy describes the logic for opening, managing and closing positions.
 
-Depending on the trading strategy, after a position is opened, four events will determine how the position ends:
+Depending on the trading strategy, once a position is opened, four events can determine how the position ends:
 
 1. Stop loss hit: The price hit the stop loss, which is the maximum tolerable loss (Limit Order)
 2. Take profit hit: The price hit the take profit, which is the estimated maximum profit the position can reach (Limit
    Order)
 3. Expiration time reached: The position has reached a specific expiration time (Good Til Time or GTT orders)
-4. A custom condition: Any custom condition that can maximize the position profit. These conditions depend on price
-   action whuile the position is opened
+4. A custom condition: Any custom condition that can trigger the position closing. These conditions depend on price
+   action while the position is opened
 
 ![](./docs/images/triple-barrier-long.png)
 
-To determine if strategy is potentially profitable before live trading, it is necessary to collect a large sample of
-trades to
-analyze the effectiveness of the strategy in terms of profits, mean profits, profits distributions, draw-downs or any
-metric you prefer.
+To determine if a strategy is potentially profitable before live trading, it is necessary to collect a large sample of
+trades to analyze the effectiveness of the strategy in terms of profits, mean profits, profits distributions, drawdowns
+or any metric you prefer.
 
 Doing this analysis process manually is not recommended at all, considering the amount of data you need to analyze, the
 volume of trades required to determine if the strategy is significantly profitable and the human error, to name a few
-reasons. Suppose you have
-ten trading strategy models, each one with ten permutations of parameter values (this can lead to over-fitting, I know)
-and
-suppose you want to collect samples over ten years at a frequency (time-frame) of 5 minutes, impossible, isn't it?
+reasons. 
 
-## Enter Algorithmic Trading
+## Algorithmic Trading and Triple Barrier
 
-In simple terms, through algorithmic trading is using software to automate all the process described above: Open, manage
+In simple terms, algorithmic trading is using software to automate all the processes described above: Open, manage
 and Close trading positions.
 
 But before running live a trading algorithm that implements a trading model you need to perform some research and
-analyze the algorithm behavior on historic data to understand whether the algorithm is able to generalize and
-potentially behave similarly on unseen or future data, this process is called back-testing.
+analyze the algorithm behavior on historic data to understand whether the algorithm is able to generalize well and
+ behave similarly on unseen or future data, this process is called back-testing.
 
-Is in back-testing where you need to identify: when positions where opened, when and why they were closed.
+Is in back-testing where you need to identify: when positions were opened, when and why they were closed, so you can 
+calculate all required performance metrics and that is why Triple Barrier was built for.
 
-## Enter Triple Barrier
-
-So Triple Barrier automates the recording of trades in the context of back-testing or machine learning as well
-to label trade profit/loss, closing event or any other value you can calculate from the data provided by triple barrier.
 
 ## How?
 
-For now please refer to the tests to understand how triple barrier works:
+### How to install
+
+```commandline
+pip install triple-barrier==0.4.3rc0
+```
+
 
 [Triple barrier test](./tests/triple_barrier/integration/test_triple_barrier_apply_happy_path.py)
 
 Or to this Jupyter Notebook that combines triple barrier calculation with plotting.
 
 [Triple Barrier Jupyter Notebook](./docs/plot-method-tests.ipynb)
 
-In the future extensive amount of examples will be used.
 
 ### How to install
 
 As of now, the latest version (Release candidate) is 0.4.1rc and can be installed as follows:
 
 ```commandline
 pip install triple-barrier==0.4.2rc0
 ```
 
+### Examples
+
+This is a work in progress, but you can find some examples here:
+
+You can see use case examples in this [folder](./docs/examples)
+
+## TODO
+
+This project is its final stages of testing, documentation and CLEANing.
+
+Besides that, there are some identified tasks that need to be done before the first release.
+
+- Add string representations for some classes
+- Provide an out-of-the-box function that can be easily used by pandas apply . Currently, you need to build one.
+- Refactor list of barriers hits (OrderBoxHits.barriers) as dictionary, currently is a list which
+is not much actionable.
+- Plotting: Add possibility to plot oscillators in a panel below
+- Add trailing stops
+
+
+## Other Documentation
+
+[Uml models](./docs/models.md)
+
 # References
 
 [Why numpy is fast](https://numpy.org/doc/stable/user/whatisnumpy.html#why-is-numpy-fast)
```

