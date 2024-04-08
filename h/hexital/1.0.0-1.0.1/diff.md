# Comparing `tmp/hexital-1.0.0.tar.gz` & `tmp/hexital-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexital-1.0.0.tar", max compression
+gzip compressed data, was "hexital-1.0.1.tar", max compression
```

## Comparing `hexital-1.0.0.tar` & `hexital-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     4665 2024-02-11 12:42:38.991346 hexital-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1067 2024-02-11 12:42:38.991346 hexital-1.0.0/LICENSE
--rw-r--r--   0        0        0    12008 2024-02-11 12:42:38.991346 hexital-1.0.0/README.md
--rw-r--r--   0        0        0      249 2024-02-11 12:42:38.991346 hexital-1.0.0/hexital/__init__.py
--rw-r--r--   0        0        0      747 2024-02-11 12:42:38.991346 hexital-1.0.0/hexital/analysis/__init__.py
--rw-r--r--   0        0        0    12248 2024-02-11 12:42:38.991346 hexital-1.0.0/hexital/analysis/movement.py
--rw-r--r--   0        0        0     2538 2024-02-11 12:42:38.991346 hexital-1.0.0/hexital/analysis/patterns.py
--rw-r--r--   0        0        0     1378 2024-02-11 12:42:38.991346 hexital-1.0.0/hexital/analysis/utils.py
--rw-r--r--   0        0        0       80 2024-02-11 12:42:38.991346 hexital-1.0.0/hexital/candlesticks/__init__.py
--rw-r--r--   0        0        0      719 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/candlesticks/heikinashi.py
--rw-r--r--   0        0        0        0 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/core/__init__.py
--rw-r--r--   0        0        0     5984 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/core/candle.py
--rw-r--r--   0        0        0     7829 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/core/candle_manager.py
--rw-r--r--   0        0        0      958 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/core/candlestick_type.py
--rw-r--r--   0        0        0    14482 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/core/hexital.py
--rw-r--r--   0        0        0    13487 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/core/indicator.py
--rw-r--r--   0        0        0      839 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/exceptions.py
--rw-r--r--   0        0        0      761 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/__init__.py
--rw-r--r--   0        0        0     3970 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/adx.py
--rw-r--r--   0        0        0     2188 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/amorph.py
--rw-r--r--   0        0        0     1069 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/atr.py
--rw-r--r--   0        0        0     1295 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/ema.py
--rw-r--r--   0        0        0      426 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/hla.py
--rw-r--r--   0        0        0     1613 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/kc.py
--rw-r--r--   0        0        0     2860 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/macd.py
--rw-r--r--   0        0        0      818 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/obv.py
--rw-r--r--   0        0        0     1413 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/rma.py
--rw-r--r--   0        0        0      676 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/roc.py
--rw-r--r--   0        0        0     2589 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/rsi.py
--rw-r--r--   0        0        0     1168 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/sma.py
--rw-r--r--   0        0        0     2801 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/stoch.py
--rw-r--r--   0        0        0     2555 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/supertrend.py
--rw-r--r--   0        0        0      802 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/tr.py
--rw-r--r--   0        0        0     1452 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/vwap.py
--rw-r--r--   0        0        0      906 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/vwma.py
--rw-r--r--   0        0        0      962 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/indicators/wma.py
--rw-r--r--   0        0        0       89 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/utils/__init__.py
--rw-r--r--   0        0        0     2960 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/utils/candles.py
--rw-r--r--   0        0        0      585 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/utils/candlesticks.py
--rw-r--r--   0        0        0     1088 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/utils/indexing.py
--rw-r--r--   0        0        0     2792 2024-02-11 12:42:38.995346 hexital-1.0.0/hexital/utils/timeframe.py
--rw-r--r--   0        0        0     1503 2024-02-11 12:42:38.995346 hexital-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    13019 1970-01-01 00:00:00.000000 hexital-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4747 2024-04-08 21:11:50.558715 hexital-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2024-04-08 21:11:50.558715 hexital-1.0.1/LICENSE
+-rw-r--r--   0        0        0    12008 2024-04-08 21:11:50.558715 hexital-1.0.1/README.md
+-rw-r--r--   0        0        0      249 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/analysis/__init__.py
+-rw-r--r--   0        0        0    12248 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/analysis/movement.py
+-rw-r--r--   0        0        0     2538 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/analysis/patterns.py
+-rw-r--r--   0        0        0     1378 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/analysis/utils.py
+-rw-r--r--   0        0        0       80 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/candlesticks/__init__.py
+-rw-r--r--   0        0        0      719 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/candlesticks/heikinashi.py
+-rw-r--r--   0        0        0        0 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/__init__.py
+-rw-r--r--   0        0        0     5984 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/candle.py
+-rw-r--r--   0        0        0     7829 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/candle_manager.py
+-rw-r--r--   0        0        0      958 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/candlestick_type.py
+-rw-r--r--   0        0        0    15017 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/hexital.py
+-rw-r--r--   0        0        0    13487 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/indicator.py
+-rw-r--r--   0        0        0      839 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/exceptions.py
+-rw-r--r--   0        0        0      761 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/__init__.py
+-rw-r--r--   0        0        0     3970 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/adx.py
+-rw-r--r--   0        0        0     2188 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/amorph.py
+-rw-r--r--   0        0        0     1069 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/atr.py
+-rw-r--r--   0        0        0     1295 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/ema.py
+-rw-r--r--   0        0        0      426 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/hla.py
+-rw-r--r--   0        0        0     1613 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/kc.py
+-rw-r--r--   0        0        0     2860 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/macd.py
+-rw-r--r--   0        0        0      818 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/obv.py
+-rw-r--r--   0        0        0     1413 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/rma.py
+-rw-r--r--   0        0        0      676 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/roc.py
+-rw-r--r--   0        0        0     2589 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/rsi.py
+-rw-r--r--   0        0        0     1168 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/sma.py
+-rw-r--r--   0        0        0     2801 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/stoch.py
+-rw-r--r--   0        0        0     2555 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/supertrend.py
+-rw-r--r--   0        0        0      802 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/tr.py
+-rw-r--r--   0        0        0     1452 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/vwap.py
+-rw-r--r--   0        0        0      906 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/vwma.py
+-rw-r--r--   0        0        0      962 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/wma.py
+-rw-r--r--   0        0        0       89 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/utils/__init__.py
+-rw-r--r--   0        0        0     2960 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/utils/candles.py
+-rw-r--r--   0        0        0      585 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/utils/candlesticks.py
+-rw-r--r--   0        0        0     1088 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/utils/indexing.py
+-rw-r--r--   0        0        0     2792 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/utils/timeframe.py
+-rw-r--r--   0        0        0     1503 2024-04-08 21:11:50.558715 hexital-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    13019 1970-01-01 00:00:00.000000 hexital-1.0.1/PKG-INFO
```

### Comparing `hexital-1.0.0/CHANGELOG.md` & `hexital-1.0.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.0.1 - 2024-04-08
+- Fixed #12 Inaccurate verify_indicators method in Hexital
+
 ## 1.0.0 - 2024-02-11
 - Moving Into BETA
 - Added CandleManager
   - CandleManger replaces List[Candle] to manage Candles and controls CandlestickTypes, timeframes and lifespan
 - Added CandlestickType
   - CandlestickType modular parent to convert candlesticks to alt types,
   - E.G Auto convert candles to heikin-ashi
```

### Comparing `hexital-1.0.0/LICENSE` & `hexital-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/README.md` & `hexital-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/analysis/__init__.py` & `hexital-1.0.1/hexital/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/analysis/movement.py` & `hexital-1.0.1/hexital/analysis/movement.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/analysis/patterns.py` & `hexital-1.0.1/hexital/analysis/patterns.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/analysis/utils.py` & `hexital-1.0.1/hexital/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/candlesticks/heikinashi.py` & `hexital-1.0.1/hexital/candlesticks/heikinashi.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/core/candle.py` & `hexital-1.0.1/hexital/core/candle.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/core/candle_manager.py` & `hexital-1.0.1/hexital/core/candle_manager.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/core/candlestick_type.py` & `hexital-1.0.1/hexital/core/candlestick_type.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/core/hexital.py` & `hexital-1.0.1/hexital/core/hexital.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,22 +240,40 @@
 
     def recalculate(self, name: Optional[str] = None):
         """Purge's all indicator reading's and re-calculates them all,
         ideal for changing an indicator parameters midway."""
         self.purge(name)
         self.calculate(name)
 
+    def _find_indicator(self, indicator: str) -> CandleManager | None:
+        for manager in self._candles.values():
+            if not manager.candles:
+                return manager
+            elif manager.find_indicator(indicator):
+                return manager
+
+        return None
+
     def _verify_indicators(
         self, indicator: str, indicator_two: Optional[str] = None
     ) -> List[Candle]:
-        if indicator and not indicator_two:
-            for manager in self._candles.values():
-                if manager.find_indicator(indicator):
-                    return manager.candles
-            raise MissingIndicator(f"Cannot find {indicator}")
+        manager = self._find_indicator(indicator)
+
+        if not manager and indicator in self._indicators:
+            return []
+        elif manager and not indicator_two:
+            return manager.candles
+
+        if not indicator_two or not manager:
+            raise MissingIndicator("Cannot find Indicator: %s" % indicator)
+
+        manager_two = self._find_indicator(indicator_two)
+
+        if not manager_two:
+            raise MissingIndicator("Cannot find Indicator: %s" % indicator_two)
 
         for manager in self._candles.values():
             if manager.find_indicator(indicator) and manager.find_indicator(indicator_two):
                 return manager.candles
 
         raise MixedTimeframes(
             "Cannot find {%s} and {%s} within same timeframe" % (indicator, indicator_two)
```

### Comparing `hexital-1.0.0/hexital/core/indicator.py` & `hexital-1.0.1/hexital/core/indicator.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/exceptions.py` & `hexital-1.0.1/hexital/exceptions.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/__init__.py` & `hexital-1.0.1/hexital/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/adx.py` & `hexital-1.0.1/hexital/indicators/adx.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/amorph.py` & `hexital-1.0.1/hexital/indicators/amorph.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/atr.py` & `hexital-1.0.1/hexital/indicators/atr.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/ema.py` & `hexital-1.0.1/hexital/indicators/ema.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/kc.py` & `hexital-1.0.1/hexital/indicators/kc.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/macd.py` & `hexital-1.0.1/hexital/indicators/macd.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/obv.py` & `hexital-1.0.1/hexital/indicators/obv.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/rma.py` & `hexital-1.0.1/hexital/indicators/rma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/roc.py` & `hexital-1.0.1/hexital/indicators/roc.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/rsi.py` & `hexital-1.0.1/hexital/indicators/rsi.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/sma.py` & `hexital-1.0.1/hexital/indicators/sma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/stoch.py` & `hexital-1.0.1/hexital/indicators/stoch.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/supertrend.py` & `hexital-1.0.1/hexital/indicators/supertrend.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/tr.py` & `hexital-1.0.1/hexital/indicators/tr.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/vwap.py` & `hexital-1.0.1/hexital/indicators/vwap.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/vwma.py` & `hexital-1.0.1/hexital/indicators/vwma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/indicators/wma.py` & `hexital-1.0.1/hexital/indicators/wma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/utils/candles.py` & `hexital-1.0.1/hexital/utils/candles.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/utils/candlesticks.py` & `hexital-1.0.1/hexital/utils/candlesticks.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/utils/indexing.py` & `hexital-1.0.1/hexital/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/hexital/utils/timeframe.py` & `hexital-1.0.1/hexital/utils/timeframe.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.0/pyproject.toml` & `hexital-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hexital"
-version = "1.0.0"
+version = "1.0.1"
 description = "Hex Incremental Technical Analysis Library"
 readme = "README.md"
 license = "MIT"
 authors = ["Merlin Roe <merlin.roe@hotmail.co.uk>"]
 homepage = "https://github.com/MerlinR/Hexital"
 repository = "https://github.com/MerlinR/Hexital"
 documentation = "https://github.com/MerlinR/Hexital"
```

### Comparing `hexital-1.0.0/PKG-INFO` & `hexital-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexital
-Version: 1.0.0
+Version: 1.0.1
 Summary: Hex Incremental Technical Analysis Library
 Home-page: https://github.com/MerlinR/Hexital
 License: MIT
 Keywords: trading,quant,indicators
 Author: Merlin Roe
 Author-email: merlin.roe@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
```

