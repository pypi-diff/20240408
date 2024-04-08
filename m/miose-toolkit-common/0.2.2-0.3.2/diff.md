# Comparing `tmp/miose_toolkit_common-0.2.2.tar.gz` & `tmp/miose_toolkit_common-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miose_toolkit_common-0.2.2.tar", max compression
+gzip compressed data, was "miose_toolkit_common-0.3.2.tar", max compression
```

## Comparing `miose_toolkit_common-0.2.2.tar` & `miose_toolkit_common-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      525 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      660 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/__init__.py
--rw-r--r--   0        0        0    12915 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/command.py
--rw-r--r--   0        0        0     1673 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/common.py
--rw-r--r--   0        0        0     5217 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/config.py
--rw-r--r--   0        0        0      510 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/convert.py
--rw-r--r--   0        0        0      267 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/dict.py
--rw-r--r--   0        0        0      109 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/exceptions.py
--rw-r--r--   0        0        0     1809 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/fetch.py
--rw-r--r--   0        0        0     1560 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/file.py
--rw-r--r--   0        0        0     3680 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/funny.py
--rw-r--r--   0        0        0     2074 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/list.py
--rw-r--r--   0        0        0     6057 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/mxios.py
--rw-r--r--   0        0        0     1300 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/retry.py
--rw-r--r--   0        0        0     1115 2024-03-21 02:55:08.550101 miose_toolkit_common-0.2.2/src/miose_toolkit_common/url.py
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 miose_toolkit_common-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      525 2024-04-08 06:09:33.766204 miose_toolkit_common-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      702 2024-04-08 06:09:33.766204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/__init__.py
+-rw-r--r--   0        0        0    12915 2024-04-08 06:09:33.766204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/command.py
+-rw-r--r--   0        0        0     1673 2024-04-08 06:09:33.766204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/common.py
+-rw-r--r--   0        0        0     5217 2024-04-08 06:09:33.766204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/config.py
+-rw-r--r--   0        0        0      510 2024-04-08 06:09:33.766204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/convert.py
+-rw-r--r--   0        0        0      267 2024-04-08 06:09:33.766204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/dict.py
+-rw-r--r--   0        0        0      109 2024-04-08 06:09:33.766204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/exceptions.py
+-rw-r--r--   0        0        0     4441 2024-04-08 06:09:33.766204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/fetch.py
+-rw-r--r--   0        0        0     1560 2024-04-08 06:09:33.770204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/file.py
+-rw-r--r--   0        0        0     3680 2024-04-08 06:09:33.770204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/funny.py
+-rw-r--r--   0        0        0     2074 2024-04-08 06:09:33.770204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/list.py
+-rw-r--r--   0        0        0    11361 2024-04-08 06:09:33.770204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/mxios.py
+-rw-r--r--   0        0        0     1300 2024-04-08 06:09:33.770204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/retry.py
+-rw-r--r--   0        0        0     1411 2024-04-08 06:09:33.770204 miose_toolkit_common-0.3.2/src/miose_toolkit_common/url.py
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 miose_toolkit_common-0.3.2/PKG-INFO
```

### Comparing `miose_toolkit_common-0.2.2/pyproject.toml` & `miose_toolkit_common-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miose-toolkit-common"
-version = "0.2.2"
+version = "0.3.2"
 description = "Miose Toolkit 通用模块"
 authors = ["KroMiose <li_xiangff@163.com>"]
 packages = [{ include = "miose_toolkit_common", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 aiohttp = "^3.9.2"
```

### Comparing `miose_toolkit_common-0.2.2/src/miose_toolkit_common/__init__.py` & `miose_toolkit_common-0.3.2/src/miose_toolkit_common/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 from .list import (
     advance_split,
     drop_empty_from_list,
     json_list_stringify_limit,
     quick_value,
     split_and_drop_empty,
 )
-from .mxios import Mxios
+from .mxios import AioResponse, Mxios, Response
 from .retry import async_retry, retry
 from .url import (
     drop_url_anchor,
+    gen_proxy_url,
     get_url_domain,
     get_url_params,
     get_url_path,
     is_relative_url,
 )
```

### Comparing `miose_toolkit_common-0.2.2/src/miose_toolkit_common/command.py` & `miose_toolkit_common-0.3.2/src/miose_toolkit_common/command.py`

 * *Files identical despite different names*

### Comparing `miose_toolkit_common-0.2.2/src/miose_toolkit_common/common.py` & `miose_toolkit_common-0.3.2/src/miose_toolkit_common/common.py`

 * *Files identical despite different names*

### Comparing `miose_toolkit_common-0.2.2/src/miose_toolkit_common/config.py` & `miose_toolkit_common-0.3.2/src/miose_toolkit_common/config.py`

 * *Files identical despite different names*

### Comparing `miose_toolkit_common-0.2.2/src/miose_toolkit_common/file.py` & `miose_toolkit_common-0.3.2/src/miose_toolkit_common/file.py`

 * *Files identical despite different names*

### Comparing `miose_toolkit_common-0.2.2/src/miose_toolkit_common/funny.py` & `miose_toolkit_common-0.3.2/src/miose_toolkit_common/funny.py`

 * *Files identical despite different names*

### Comparing `miose_toolkit_common-0.2.2/src/miose_toolkit_common/list.py` & `miose_toolkit_common-0.3.2/src/miose_toolkit_common/list.py`

 * *Files identical despite different names*

### Comparing `miose_toolkit_common-0.2.2/src/miose_toolkit_common/retry.py` & `miose_toolkit_common-0.3.2/src/miose_toolkit_common/retry.py`

 * *Files identical despite different names*

### Comparing `miose_toolkit_common-0.2.2/src/miose_toolkit_common/url.py` & `miose_toolkit_common-0.3.2/src/miose_toolkit_common/url.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,65 @@
-from urllib.parse import quote, unquote
+from urllib.parse import quote, unquote, urlparse
 
 
 def get_url_domain(url: str) -> str:
     """获取url的域名"""
 
     try:
         return url.split("//")[1].split("/")[0]
     except Exception:
         return ""
 
+
 def get_url_path(url: str) -> str:
     """获取url的路径"""
 
     path = url.split("//")[1].split("/", 1)  # Split only once
     if len(path) > 1:
         return "/" + path[1]
     return "/"
 
+
 def get_url_params(url: str, use_unquote: bool = True) -> dict:
     """获取url的参数"""
 
     try:
         params = {}
         for param in url.split("?")[1].split("&"):
             k, v = param.split("=")
             params[k] = v if not use_unquote else unquote(v)
     except Exception:
         return {}
     else:
         return params
 
+
 def drop_url_anchor(url: str) -> str:
     """去除url中的锚点"""
 
     if url.startswith("#"):
         return ""
     return url.split("#")[0]
 
+
 def is_relative_url(url: str) -> bool:
     """判断url是否为相对路径"""
 
     return url.startswith(("/", "#"))
 
+
 def trans_str_to_url(s: str) -> str:
     """将字符串转换为url"""
 
     return quote(s, safe="")
+
+
+def gen_proxy_url(
+    proxy_host: str,
+    proxy_port: int,
+    proxy_username: str = "",
+    proxy_password: str = "",
+    protocol: str = "http",
+) -> str:
+    return urlparse(
+        f"{protocol}//{proxy_username}:{proxy_password}@{proxy_host}:{proxy_port}",
+    ).geturl()
```

### Comparing `miose_toolkit_common-0.2.2/PKG-INFO` & `miose_toolkit_common-0.3.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miose-toolkit-common
-Version: 0.2.2
+Version: 0.3.2
 Summary: Miose Toolkit 通用模块
 Author: KroMiose
 Author-email: li_xiangff@163.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

