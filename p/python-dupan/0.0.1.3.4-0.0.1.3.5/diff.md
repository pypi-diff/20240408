# Comparing `tmp/python_dupan-0.0.1.3.4.tar.gz` & `tmp/python_dupan-0.0.1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dupan-0.0.1.3.4.tar", max compression
+gzip compressed data, was "python_dupan-0.0.1.3.5.tar", max compression
```

## Comparing `python_dupan-0.0.1.3.4.tar` & `python_dupan-0.0.1.3.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rwxr-xr-x   0        0        0     1100 2023-12-31 13:16:43.902936 python_dupan-0.0.1.3.4/LICENSE
--rw-r--r--   0        0        0    97252 2024-01-17 12:43:04.316136 python_dupan-0.0.1.3.4/dupan/__init__.py
--rw-r--r--   0        0        0       61 2024-01-01 10:28:23.372962 python_dupan-0.0.1.3.4/dupan/util/__init__.py
--rw-r--r--   0        0        0    13106 2024-01-13 08:28:56.453139 python_dupan-0.0.1.3.4/dupan/util/file.py
--rw-r--r--   0        0        0     1795 2023-12-14 11:01:07.350145 python_dupan-0.0.1.3.4/dupan/util/property.py
--rw-r--r--   0        0        0     2751 2023-12-29 05:26:01.836028 python_dupan-0.0.1.3.4/dupan/util/response.py
--rw-r--r--   0        0        0     6295 2024-01-16 04:33:26.963104 python_dupan-0.0.1.3.4/dupan/util/text.py
--rw-r--r--   0        0        0     2114 2023-12-10 10:45:36.285664 python_dupan-0.0.1.3.4/dupan/util/urlopen.py
--rw-r--r--   0        0        0     1249 2024-01-17 12:42:57.284799 python_dupan-0.0.1.3.4/pyproject.toml
--rw-r--r--   0        0        0    10836 2024-01-17 04:31:26.628554 python_dupan-0.0.1.3.4/readme.md
--rw-r--r--   0        0        0    12069 1970-01-01 00:00:00.000000 python_dupan-0.0.1.3.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-12-31 13:16:43.902936 python_dupan-0.0.1.3.5/LICENSE
+-rw-r--r--   0        0        0    97504 2024-04-08 06:45:01.992933 python_dupan-0.0.1.3.5/dupan/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_dupan-0.0.1.3.5/dupan/py.typed
+-rw-r--r--   0        0        0       61 2024-01-01 10:28:23.372962 python_dupan-0.0.1.3.5/dupan/util/__init__.py
+-rw-r--r--   0        0        0    13103 2024-01-19 04:25:53.949786 python_dupan-0.0.1.3.5/dupan/util/file.py
+-rw-r--r--   0        0        0     1795 2023-12-14 11:01:07.350145 python_dupan-0.0.1.3.5/dupan/util/property.py
+-rw-r--r--   0        0        0     2751 2023-12-29 05:26:01.836028 python_dupan-0.0.1.3.5/dupan/util/response.py
+-rw-r--r--   0        0        0     6295 2024-01-16 04:33:26.963104 python_dupan-0.0.1.3.5/dupan/util/text.py
+-rw-r--r--   0        0        0     2114 2023-12-10 10:45:36.285664 python_dupan-0.0.1.3.5/dupan/util/urlopen.py
+-rw-r--r--   0        0        0     1249 2024-04-08 06:45:59.111697 python_dupan-0.0.1.3.5/pyproject.toml
+-rw-r--r--   0        0        0    10836 2024-01-17 04:31:26.628554 python_dupan-0.0.1.3.5/readme.md
+-rw-r--r--   0        0        0    12069 1970-01-01 00:00:00.000000 python_dupan-0.0.1.3.5/PKG-INFO
```

### Comparing `python_dupan-0.0.1.3.4/LICENSE` & `python_dupan-0.0.1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.4/dupan/__init__.py` & `python_dupan-0.0.1.3.5/dupan/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -925,15 +925,18 @@
         if urlp.netloc and urlp.netloc != "pan.baidu.com":
             raise ValueError(f"url 的域名必须是 'pan.baidu.com'，收到 {urlp.netloc!r}")
         path = urlp.path
         query = dict(parse_qsl(urlp.query))
         if path == "/share/link":
             shorturl = ""
         elif path == "/share/init":
-            shorturl = query["surl"]
+            try:
+                shorturl = query["surl"]
+            except KeyError:
+                shorturl = ""
         elif path.startswith("/s/1"):
             shorturl = path.removeprefix("/s/1")
             idx = shorturl.find("&")
             if idx > -1:
                 shorturl = shorturl[:idx]
         elif "/" not in path:
             shorturl = path
@@ -988,15 +991,21 @@
     @cached_property
     def yundata(self, /):
         self.list_index()
         return self.__dict__["yundata"]
 
     def verify(self, /, use_vcode: bool = False):
         api = "https://pan.baidu.com/share/verify"
-        params: dict[str, int | str] = {"surl": self.shorturl, "web": 1, "clienttype": 0}
+        params: dict[str, int | str]
+        if self.shorturl:
+            params = {"surl": self.shorturl, "web": 1, "clienttype": 0}
+        else:
+            params = {"web": 1, "clienttype": 0}
+            params.update(parse_qsl(urlparse(self.url).query))
+
         data = {"pwd": self.password}
         if use_vcode:
             data.update(cast(dict[str, str], decaptcha()))
         post = self.session.post
         while True:
             with post(api, params=params, data=data) as resp:
                 resp.raise_for_status()
```

### Comparing `python_dupan-0.0.1.3.4/dupan/util/file.py` & `python_dupan-0.0.1.3.5/dupan/util/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
         url = self.url
         response = self.urlopen(
             url() if callable(url) else url, 
             headers={**self.headers, "Range": f"bytes={start}-"}
         )
         length_new = get_total_length(response)
         if self.length != length_new:
-            raise OSError(errno.EIO, "file size changed: %s -> %s", self.length, length_new)
+            raise OSError(errno.EIO, f"file size changed: {self.length} -> {length_new}")
         self.__dict__.update(
             response=response, 
             start=start, 
             closed=False, 
         )
         return start
```

### Comparing `python_dupan-0.0.1.3.4/dupan/util/property.py` & `python_dupan-0.0.1.3.5/dupan/util/property.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.4/dupan/util/response.py` & `python_dupan-0.0.1.3.5/dupan/util/response.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.4/dupan/util/text.py` & `python_dupan-0.0.1.3.5/dupan/util/text.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.4/dupan/util/urlopen.py` & `python_dupan-0.0.1.3.5/dupan/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.4/pyproject.toml` & `python_dupan-0.0.1.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-dupan"
-version = "0.0.1.3.4"
+version = "0.0.1.3.5"
 description = "Python wrapper for `baidu webdisk <https://pan.baidu.com>`."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-dupan-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-dupan-client"
 keywords = ["nas", "dupan", "百度网盘"]
```

### Comparing `python_dupan-0.0.1.3.4/readme.md` & `python_dupan-0.0.1.3.5/readme.md`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.4/PKG-INFO` & `python_dupan-0.0.1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dupan
-Version: 0.0.1.3.4
+Version: 0.0.1.3.5
 Summary: Python wrapper for `baidu webdisk <https://pan.baidu.com>`.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-dupan-client
 License: MIT
 Keywords: nas,dupan,百度网盘
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

