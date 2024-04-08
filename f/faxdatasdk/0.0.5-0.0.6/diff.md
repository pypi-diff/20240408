# Comparing `tmp/faxdatasdk-0.0.5.tar.gz` & `tmp/faxdatasdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faxdatasdk-0.0.5.tar", last modified: Mon Apr  8 13:29:20 2024, max compression
+gzip compressed data, was "faxdatasdk-0.0.6.tar", last modified: Mon Apr  8 13:59:16 2024, max compression
```

## Comparing `faxdatasdk-0.0.5.tar` & `faxdatasdk-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 13:29:20.665510 faxdatasdk-0.0.5/
--rw-rw-rw-   0        0        0    11558 2023-07-09 16:17:28.000000 faxdatasdk-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3484 2024-04-08 13:29:20.662509 faxdatasdk-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2770 2024-01-06 09:53:52.000000 faxdatasdk-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 13:29:20.631509 faxdatasdk-0.0.5/faxdatasdk/
--rw-rw-rw-   0        0        0     1294 2024-04-07 13:47:56.000000 faxdatasdk-0.0.5/faxdatasdk/__init__.py
--rw-rw-rw-   0        0        0    14421 2024-04-08 10:48:31.000000 faxdatasdk-0.0.5/faxdatasdk/api.py
--rw-rw-rw-   0        0        0     9605 2024-04-07 14:10:47.000000 faxdatasdk-0.0.5/faxdatasdk/client.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:29:20.661508 faxdatasdk-0.0.5/faxdatasdk/compat/
--rw-rw-rw-   0        0        0        0 2023-07-09 16:17:28.000000 faxdatasdk-0.0.5/faxdatasdk/compat/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-07-09 16:17:28.000000 faxdatasdk-0.0.5/faxdatasdk/compat/pickle_compat.py
--rw-rw-rw-   0        0        0      175 2023-07-09 16:17:28.000000 faxdatasdk-0.0.5/faxdatasdk/exceptions.py
--rw-rw-rw-   0        0        0     3417 2023-12-29 07:30:25.000000 faxdatasdk-0.0.5/faxdatasdk/logger.py
--rw-rw-rw-   0        0        0     2216 2023-12-30 10:25:49.000000 faxdatasdk-0.0.5/faxdatasdk/request.py
--rw-rw-rw-   0        0        0      811 2024-04-07 14:11:07.000000 faxdatasdk-0.0.5/faxdatasdk/thrift_client.py
--rw-rw-rw-   0        0        0      590 2023-12-30 02:20:26.000000 faxdatasdk-0.0.5/faxdatasdk/utils.py
--rw-rw-rw-   0        0        0      438 2024-04-08 13:28:36.000000 faxdatasdk-0.0.5/faxdatasdk/version.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:29:20.646508 faxdatasdk-0.0.5/faxdatasdk.egg-info/
--rw-rw-rw-   0        0        0     3484 2024-04-08 13:29:20.000000 faxdatasdk-0.0.5/faxdatasdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2024-04-08 13:29:20.000000 faxdatasdk-0.0.5/faxdatasdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 13:29:20.000000 faxdatasdk-0.0.5/faxdatasdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-08 13:29:20.000000 faxdatasdk-0.0.5/faxdatasdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      151 2024-04-08 13:29:20.000000 faxdatasdk-0.0.5/faxdatasdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-08 13:29:20.000000 faxdatasdk-0.0.5/faxdatasdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 13:29:20.665510 faxdatasdk-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1966 2024-04-07 14:26:19.000000 faxdatasdk-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:59:16.471497 faxdatasdk-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2023-07-09 16:17:28.000000 faxdatasdk-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3484 2024-04-08 13:59:16.471497 faxdatasdk-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2770 2024-01-06 09:53:52.000000 faxdatasdk-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 13:59:16.455494 faxdatasdk-0.0.6/faxdatasdk/
+-rw-rw-rw-   0        0        0     1294 2024-04-07 13:47:56.000000 faxdatasdk-0.0.6/faxdatasdk/__init__.py
+-rw-rw-rw-   0        0        0    14720 2024-04-08 13:57:06.000000 faxdatasdk-0.0.6/faxdatasdk/api.py
+-rw-rw-rw-   0        0        0     9605 2024-04-07 14:10:47.000000 faxdatasdk-0.0.6/faxdatasdk/client.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:59:16.470497 faxdatasdk-0.0.6/faxdatasdk/compat/
+-rw-rw-rw-   0        0        0        0 2023-07-09 16:17:28.000000 faxdatasdk-0.0.6/faxdatasdk/compat/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-07-09 16:17:28.000000 faxdatasdk-0.0.6/faxdatasdk/compat/pickle_compat.py
+-rw-rw-rw-   0        0        0      175 2023-07-09 16:17:28.000000 faxdatasdk-0.0.6/faxdatasdk/exceptions.py
+-rw-rw-rw-   0        0        0     3417 2023-12-29 07:30:25.000000 faxdatasdk-0.0.6/faxdatasdk/logger.py
+-rw-rw-rw-   0        0        0     2216 2023-12-30 10:25:49.000000 faxdatasdk-0.0.6/faxdatasdk/request.py
+-rw-rw-rw-   0        0        0      811 2024-04-07 14:11:07.000000 faxdatasdk-0.0.6/faxdatasdk/thrift_client.py
+-rw-rw-rw-   0        0        0      590 2023-12-30 02:20:26.000000 faxdatasdk-0.0.6/faxdatasdk/utils.py
+-rw-rw-rw-   0        0        0      438 2024-04-08 13:58:44.000000 faxdatasdk-0.0.6/faxdatasdk/version.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:59:16.469497 faxdatasdk-0.0.6/faxdatasdk.egg-info/
+-rw-rw-rw-   0        0        0     3484 2024-04-08 13:59:16.000000 faxdatasdk-0.0.6/faxdatasdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2024-04-08 13:59:16.000000 faxdatasdk-0.0.6/faxdatasdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 13:59:16.000000 faxdatasdk-0.0.6/faxdatasdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-08 13:59:16.000000 faxdatasdk-0.0.6/faxdatasdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      151 2024-04-08 13:59:16.000000 faxdatasdk-0.0.6/faxdatasdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-08 13:59:16.000000 faxdatasdk-0.0.6/faxdatasdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 13:59:16.471497 faxdatasdk-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1966 2024-04-07 14:26:19.000000 faxdatasdk-0.0.6/setup.py
```

### Comparing `faxdatasdk-0.0.5/LICENSE` & `faxdatasdk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.5/PKG-INFO` & `faxdatasdk-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faxdatasdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Data SDK for stock analysis.
 Home-page: https://www.faxframework.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 License: Apache License v2
```

### Comparing `faxdatasdk-0.0.5/README.md` & `faxdatasdk-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.5/faxdatasdk/__init__.py` & `faxdatasdk-0.0.6/faxdatasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.5/faxdatasdk/api.py` & `faxdatasdk-0.0.6/faxdatasdk/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,9 +355,22 @@
 
 
 @assert_auth
 def get_news_content(start_date: str, end_date: str, sec_code_list: list = None):
     return FaxDataClient.instance().get_news_content(**locals())
 
 
+@assert_auth
+def get_stock_info(fields=None, stock_lst: list = None, stock_pool: list = None):
+    """
+    获取股票基础信息。
+
+    :param stock_pool:
+    :param stock_lst:
+    :param fields:
+    :return:
+    """
+    return FaxDataClient.instance().get_stock_info(**locals())
+
+
 __all__ = []
 __all__.extend([name for name in globals().keys() if name.startswith("get")])
```

### Comparing `faxdatasdk-0.0.5/faxdatasdk/client.py` & `faxdatasdk-0.0.6/faxdatasdk/client.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.5/faxdatasdk/compat/pickle_compat.py` & `faxdatasdk-0.0.6/faxdatasdk/compat/pickle_compat.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.5/faxdatasdk/logger.py` & `faxdatasdk-0.0.6/faxdatasdk/logger.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.5/faxdatasdk/request.py` & `faxdatasdk-0.0.6/faxdatasdk/request.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.5/faxdatasdk/thrift_client.py` & `faxdatasdk-0.0.6/faxdatasdk/thrift_client.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.5/faxdatasdk/utils.py` & `faxdatasdk-0.0.6/faxdatasdk/utils.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.5/faxdatasdk.egg-info/PKG-INFO` & `faxdatasdk-0.0.6/faxdatasdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faxdatasdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Data SDK for stock analysis.
 Home-page: https://www.faxframework.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 License: Apache License v2
```

### Comparing `faxdatasdk-0.0.5/setup.py` & `faxdatasdk-0.0.6/setup.py`

 * *Files identical despite different names*

