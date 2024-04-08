# Comparing `tmp/optrabot-0.8.1.tar.gz` & `tmp/optrabot-0.8.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optrabot-0.8.1.tar", max compression
+gzip compressed data, was "optrabot-0.8.1a0.tar", max compression
```

## Comparing `optrabot-0.8.1.tar` & `optrabot-0.8.1a0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.8.1/optrabot/__init__.py
--rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.8.1/optrabot/alembic/README
--rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.8.1/optrabot/alembic/env.py
--rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.8.1/optrabot/alembic/script.py.mako
--rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.8.1/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
--rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.8.1/optrabot/alembic.ini
--rw-r--r--   0        0        0    11822 2024-03-29 23:18:40.612397 optrabot-0.8.1/optrabot/config.py
--rw-r--r--   0        0        0     2804 2024-02-22 12:22:44.564924 optrabot-0.8.1/optrabot/crud.py
--rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.8.1/optrabot/database.py
--rw-r--r--   0        0        0     2323 2024-02-22 12:22:44.565504 optrabot-0.8.1/optrabot/main.py
--rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.8.1/optrabot/marketdatatype.py
--rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.8.1/optrabot/models.py
--rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.8.1/optrabot/optionhelper.py
--rw-r--r--   0        0        0    10372 2024-04-08 05:50:20.192018 optrabot-0.8.1/optrabot/optrabot.py
--rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.8.1/optrabot/schemas.py
--rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.8.1/optrabot/stoplossadjuster.py
--rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.8.1/optrabot/tradehelper.py
--rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.8.1/optrabot/tradetemplate/__init__.py
--rw-r--r--   0        0        0      177 2024-02-22 12:22:44.567811 optrabot-0.8.1/optrabot/tradetemplate/ironfly.py
--rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.8.1/optrabot/tradetemplate/putspread.py
--rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.8.1/optrabot/tradetemplate/template.py
--rw-r--r--   0        0        0     2273 2024-03-19 15:36:19.405141 optrabot-0.8.1/optrabot/tradetemplate/templatefactory.py
--rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.8.1/optrabot/tradetemplate/templatetrigger.py
--rw-r--r--   0        0        0    35316 2024-04-05 19:26:08.611580 optrabot-0.8.1/optrabot/tradinghubclient.py
--rw-r--r--   0        0        0      819 2024-04-08 05:53:11.432625 optrabot-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1840 1970-01-01 00:00:00.000000 optrabot-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.8.1a0/README.md
+-rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.8.1a0/optrabot/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.8.1a0/optrabot/alembic/README
+-rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.8.1a0/optrabot/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.8.1a0/optrabot/alembic/script.py.mako
+-rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.8.1a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
+-rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.8.1a0/optrabot/alembic.ini
+-rw-r--r--   0        0        0    11822 2024-03-29 23:18:40.612397 optrabot-0.8.1a0/optrabot/config.py
+-rw-r--r--   0        0        0     2804 2024-02-22 12:22:44.564924 optrabot-0.8.1a0/optrabot/crud.py
+-rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.8.1a0/optrabot/database.py
+-rw-r--r--   0        0        0     2323 2024-02-22 12:22:44.565504 optrabot-0.8.1a0/optrabot/main.py
+-rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.8.1a0/optrabot/marketdatatype.py
+-rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.8.1a0/optrabot/models.py
+-rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.8.1a0/optrabot/optionhelper.py
+-rw-r--r--   0        0        0     9791 2024-04-05 07:43:33.069681 optrabot-0.8.1a0/optrabot/optrabot.py
+-rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.8.1a0/optrabot/schemas.py
+-rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.8.1a0/optrabot/stoplossadjuster.py
+-rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.8.1a0/optrabot/tradehelper.py
+-rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.8.1a0/optrabot/tradetemplate/__init__.py
+-rw-r--r--   0        0        0      177 2024-02-22 12:22:44.567811 optrabot-0.8.1a0/optrabot/tradetemplate/ironfly.py
+-rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.8.1a0/optrabot/tradetemplate/putspread.py
+-rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.8.1a0/optrabot/tradetemplate/template.py
+-rw-r--r--   0        0        0     2273 2024-03-19 15:36:19.405141 optrabot-0.8.1a0/optrabot/tradetemplate/templatefactory.py
+-rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.8.1a0/optrabot/tradetemplate/templatetrigger.py
+-rw-r--r--   0        0        0    35316 2024-04-05 07:43:42.185859 optrabot-0.8.1a0/optrabot/tradinghubclient.py
+-rw-r--r--   0        0        0      821 2024-04-05 07:45:05.901663 optrabot-0.8.1a0/pyproject.toml
+-rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 optrabot-0.8.1a0/PKG-INFO
```

### Comparing `optrabot-0.8.1/README.md` & `optrabot-0.8.1a0/README.md`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/alembic/env.py` & `optrabot-0.8.1a0/optrabot/alembic/env.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/alembic/script.py.mako` & `optrabot-0.8.1a0/optrabot/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py` & `optrabot-0.8.1a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/alembic.ini` & `optrabot-0.8.1a0/optrabot/alembic.ini`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/config.py` & `optrabot-0.8.1a0/optrabot/config.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/crud.py` & `optrabot-0.8.1a0/optrabot/crud.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/database.py` & `optrabot-0.8.1a0/optrabot/database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/main.py` & `optrabot-0.8.1a0/optrabot/main.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/marketdatatype.py` & `optrabot-0.8.1a0/optrabot/marketdatatype.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/models.py` & `optrabot-0.8.1a0/optrabot/models.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/optionhelper.py` & `optrabot-0.8.1a0/optrabot/optionhelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/optrabot.py` & `optrabot-0.8.1a0/optrabot/optrabot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import array
 from collections import OrderedDict
 import asyncio
 import datetime as dt
-import json
 from fastapi import FastAPI
 from ib_insync import *
 from loguru import logger
 from sqlalchemy.orm import Session
 from optrabot import schemas
 from optrabot.marketdatatype import MarketDataType
 from optrabot.optionhelper import OptionHelper
@@ -40,18 +38,15 @@
 		self['config'] = conf
 		conf.logConfigurationData()
 		conf.readTemplates()
 		updateDatabase()
 		self.thc = TradinghubClient(self)
 		try:
 			logger.info('Connecting to OptraBot Hub ...')
-			additional_data = {
-				'accounts': self._getConfiguredAccounts()
-			}
-			await self.thc.reportAction(action='SU', additional_data=json.dumps(additional_data))
+			await self.thc.reportAction(action='SU')
 		except Exception as excp:
 			logger.error('Problem on Startup: {}', excp)
 			logger.error('OptraBot halted!')
 			return
 		
 		logger.info('Sucessfully connected to OptraBot Hub')
 		await self.connect_ib()
@@ -254,29 +249,14 @@
 		self._tradingEnabled = True
 
 	def isTradingEnabled(self) -> bool:
 		""" Returns true if trading is enabled after market data subscription checks have passed.
 		"""
 		return self._tradingEnabled
 	
-	def _getConfiguredAccounts(self) -> list:
-		""" 
-		Returns a list of configured accounts
-		"""
-		conf: Config = self['config']
-		configuredAccounts = None
-		for item in conf.getTemplates():
-			template : Template = item
-			if configuredAccounts == None:
-				configuredAccounts = [template.account]
-			else:
-				if not template.account in configuredAccounts:
-					configuredAccounts.append(template.account)
-		return configuredAccounts
-
 	@logger.catch
 	def handleTaskDone(self, task: asyncio.Task):
 		if not task.cancelled():
 			taskException = task.exception()
 			if taskException != None:
 				logger.error('Task Exception occured!')
 				raise taskException
```

### Comparing `optrabot-0.8.1/optrabot/schemas.py` & `optrabot-0.8.1a0/optrabot/schemas.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/stoplossadjuster.py` & `optrabot-0.8.1a0/optrabot/stoplossadjuster.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/tradehelper.py` & `optrabot-0.8.1a0/optrabot/tradehelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/tradetemplate/template.py` & `optrabot-0.8.1a0/optrabot/tradetemplate/template.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/tradetemplate/templatefactory.py` & `optrabot-0.8.1a0/optrabot/tradetemplate/templatefactory.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/tradetemplate/templatetrigger.py` & `optrabot-0.8.1a0/optrabot/tradetemplate/templatetrigger.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.1/optrabot/tradinghubclient.py` & `optrabot-0.8.1a0/optrabot/tradinghubclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,15 +676,15 @@
 				else:
 					self._ironFlyStopPrice = adjustedStopLossPrice
 					logger.info('Performing stop loss adjustment. New Stop Loss price: {}', self._ironFlyStopPrice)
 			else:
 				logger.debug('Stoploss adjustment has been performed already.')
 		else:
 			logger.debug('No StopLoss adjustment configured.')
-		desiredStopPrice = OptionHelper.roundToTickSize(self._ironFlyStopPrice + longLegsValue)
+		desiredStopPrice = OptionHelper.roundToTickSize(self._ironFlyStopPrice - longLegsValue)
 		if not self._slShortTrade and self._position == True:
 			logger.error('Caution: Stop Loss order for Short Strikes is missing. Please check in TWS!')
 			return
 		currentStopPrice = OptionHelper.roundToTickSize(self._slShortTrade.order.auxPrice)
 		logger.debug('Long Legs value {} Current Short SL Price: {} Desired Short SL Pice: {}', round(longLegsValue,2), currentStopPrice, desiredStopPrice)
 		openTrades = await ib.reqOpenOrdersAsync()
 		if self._slShortTrade in openTrades and self._slShortTrade.isActive():
```

### Comparing `optrabot-0.8.1/pyproject.toml` & `optrabot-0.8.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optrabot"
-version = "0.8.1"
+version = "0.8.1a0"
 description = "QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account."
 authors = ["QuantX GmbH"]
 readme = "README.md"
 license = "MIT"
 homepage = "http://www.optrabot.com"
 keywords = ["tws"]
 packages =  [{include = "optrabot"}]
```

### Comparing `optrabot-0.8.1/PKG-INFO` & `optrabot-0.8.1a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optrabot
-Version: 0.8.1
+Version: 0.8.1a0
 Summary: QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account.
 Home-page: http://www.optrabot.com
 License: MIT
 Keywords: tws
 Author: QuantX GmbH
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

