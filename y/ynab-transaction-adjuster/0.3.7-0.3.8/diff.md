# Comparing `tmp/ynab_transaction_adjuster-0.3.7.tar.gz` & `tmp/ynab_transaction_adjuster-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_transaction_adjuster-0.3.7.tar", max compression
+gzip compressed data, was "ynab_transaction_adjuster-0.3.8.tar", max compression
```

## Comparing `ynab_transaction_adjuster-0.3.7.tar` & `ynab_transaction_adjuster-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35148 2024-04-07 08:02:34.526925 ynab_transaction_adjuster-0.3.7/LICENSE
--rw-r--r--   0        0        0     3462 2024-04-07 08:02:34.526925 ynab_transaction_adjuster-0.3.7/README.md
--rw-r--r--   0        0        0      680 2024-04-07 08:02:49.139138 ynab_transaction_adjuster-0.3.7/pyproject.toml
--rw-r--r--   0        0        0       84 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/__init__.py
--rw-r--r--   0        0        0     1942 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/adjuster.py
--rw-r--r--   0        0        0     2481 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/client.py
--rw-r--r--   0        0        0      903 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/exceptions.py
--rw-r--r--   0        0        0      358 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/__init__.py
--rw-r--r--   0        0        0      246 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/category.py
--rw-r--r--   0        0        0      621 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/categorygroup.py
--rw-r--r--   0        0        0     3209 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/modifiedtransaction.py
--rw-r--r--   0        0        0      602 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/originalsubtransaction.py
--rw-r--r--   0        0        0     2865 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/originaltransaction.py
--rw-r--r--   0        0        0      586 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/payee.py
--rw-r--r--   0        0        0     1244 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/subtransaction.py
--rw-r--r--   0        0        0     1860 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/transactionmodifier.py
--rw-r--r--   0        0        0       72 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/repos/__init__.py
--rw-r--r--   0        0        0     1918 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/repos/categoryrepo.py
--rw-r--r--   0        0        0     1723 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/repos/payeerepo.py
--rw-r--r--   0        0        0     4337 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/ynabtransactionadjuster.py
--rw-r--r--   0        0        0     4252 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/LICENSE
+-rw-r--r--   0        0        0     3462 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/README.md
+-rw-r--r--   0        0        0      680 2024-04-08 08:57:18.496879 ynab_transaction_adjuster-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/__init__.py
+-rw-r--r--   0        0        0     1942 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/adjuster.py
+-rw-r--r--   0        0        0     2481 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/client.py
+-rw-r--r--   0        0        0      903 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/exceptions.py
+-rw-r--r--   0        0        0      358 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/category.py
+-rw-r--r--   0        0        0      621 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/categorygroup.py
+-rw-r--r--   0        0        0     3209 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/modifiedtransaction.py
+-rw-r--r--   0        0        0      602 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/originalsubtransaction.py
+-rw-r--r--   0        0        0     2865 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/originaltransaction.py
+-rw-r--r--   0        0        0      586 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/payee.py
+-rw-r--r--   0        0        0     1244 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/subtransaction.py
+-rw-r--r--   0        0        0     1860 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/transactionmodifier.py
+-rw-r--r--   0        0        0       72 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/repos/__init__.py
+-rw-r--r--   0        0        0     1918 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/repos/categoryrepo.py
+-rw-r--r--   0        0        0     1723 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/repos/payeerepo.py
+-rw-r--r--   0        0        0     4357 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/ynabtransactionadjuster.py
+-rw-r--r--   0        0        0     4252 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-0.3.8/PKG-INFO
```

### Comparing `ynab_transaction_adjuster-0.3.7/LICENSE` & `ynab_transaction_adjuster-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/README.md` & `ynab_transaction_adjuster-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/pyproject.toml` & `ynab_transaction_adjuster-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ynab-transaction-adjuster"
-version = "0.3.7"
+version = "0.3.8"
 description = "Library to adjust transactions in YNAB based on custom patterns"
 authors = ["Daniel Basta <ynab@basta.info>"]
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabtransactionadjuster'}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/adjuster.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/adjuster.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/client.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/client.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/exceptions.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/exceptions.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/categorygroup.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/categorygroup.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/modifiedtransaction.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/modifiedtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/originalsubtransaction.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/originalsubtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/originaltransaction.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/originaltransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/payee.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/payee.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/subtransaction.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/subtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/transactionmodifier.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/transactionmodifier.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/repos/categoryrepo.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/repos/categoryrepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/repos/payeerepo.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/repos/payeerepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/ynabtransactionadjuster.py` & `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/ynabtransactionadjuster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import abstractmethod
 from typing import List
 
 from ynabtransactionadjuster.adjuster import Adjuster
 from ynabtransactionadjuster.client import Client
-from ynabtransactionadjuster.models import OriginalTransaction, ModifiedTransaction
+from ynabtransactionadjuster.models import OriginalTransaction
 from ynabtransactionadjuster.models import TransactionModifier
 from ynabtransactionadjuster.repos import CategoryRepo
 from ynabtransactionadjuster.repos import PayeeRepo
 
 
 class YnabTransactionAdjuster:
 	"""Abstract class which modifies transactions according to concrete implementation. You need to create your own
@@ -36,16 +36,18 @@
 		:raises AdjustError: if there is any error during the adjust process
 		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
 		"""
 		transactions = self._client.fetch_transactions()
 		filtered_transactions = self.filter(transactions)
 		adjuster = Adjuster(transactions=filtered_transactions, adjust_func=self.adjust, categories=self.categories)
 		modified_transactions = adjuster.run()
-		updated = self._client.update_transactions(modified_transactions)
-		return updated
+		if modified_transactions:
+			updated = self._client.update_transactions(modified_transactions)
+			return updated
+		return 0
 
 	def test(self) -> List[dict]:
 		"""Tests the adjuster. It will fetch transactions from the YNAB account, filter & adjust them as per
 		implementation of the two methods. This function doesn't update records in YNAB but returns the modified
 		transactions so that they can be inspected. `#! select * from source`
 
 		The returned dicts have the following structure:
```

### Comparing `ynab_transaction_adjuster-0.3.7/PKG-INFO` & `ynab_transaction_adjuster-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynab-transaction-adjuster
-Version: 0.3.7
+Version: 0.3.8
 Summary: Library to adjust transactions in YNAB based on custom patterns
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

