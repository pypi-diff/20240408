# Comparing `tmp/pynocaptcha-1.8.6.tar.gz` & `tmp/pynocaptcha-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynocaptcha-1.8.6.tar", last modified: Thu Apr  4 16:00:28 2024, max compression
+gzip compressed data, was "pynocaptcha-1.8.7.tar", last modified: Mon Apr  8 01:17:52 2024, max compression
```

## Comparing `pynocaptcha-1.8.6.tar` & `pynocaptcha-1.8.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-04 16:00:28.697966 pynocaptcha-1.8.6/
--rw-r--r--   0 esbiya     (501) staff       (20)     1074 2023-03-15 06:31:13.000000 pynocaptcha-1.8.6/LICENSE
--rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-04 16:00:28.697784 pynocaptcha-1.8.6/PKG-INFO
--rw-r--r--   0 esbiya     (501) staff       (20)       38 2023-03-15 09:37:56.000000 pynocaptcha-1.8.6/README.md
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-04 16:00:28.694585 pynocaptcha-1.8.6/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)     1095 2024-03-28 09:20:29.000000 pynocaptcha-1.8.6/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-04 16:00:28.697496 pynocaptcha-1.8.6/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     1054 2023-11-15 10:37:10.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)      668 2024-04-04 15:59:57.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/aws.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5258 2024-03-30 04:19:25.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1061 2024-02-27 06:17:10.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)      744 2023-08-14 02:01:08.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/discord.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1221 2023-07-03 06:08:01.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2088 2024-01-15 06:49:23.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1559 2024-03-30 04:01:26.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/perimeterx.py
--rw-r--r--   0 esbiya     (501) staff       (20)     3077 2023-12-13 01:23:55.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/tls.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-04 16:00:28.695256 pynocaptcha-1.8.6/pynocaptcha.egg-info/
--rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/PKG-INFO
--rw-r--r--   0 esbiya     (501) staff       (20)      577 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/not-zip-safe
--rw-r--r--   0 esbiya     (501) staff       (20)       15 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/requires.txt
--rw-r--r--   0 esbiya     (501) staff       (20)       33 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/top_level.txt
--rw-r--r--   0 esbiya     (501) staff       (20)       38 2024-04-04 16:00:28.698004 pynocaptcha-1.8.6/setup.cfg
--rw-r--r--   0 esbiya     (501) staff       (20)      845 2024-04-04 16:00:21.000000 pynocaptcha-1.8.6/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-08 01:17:52.072888 pynocaptcha-1.8.7/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1074 2023-03-15 06:31:13.000000 pynocaptcha-1.8.7/LICENSE
+-rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-08 01:17:52.072744 pynocaptcha-1.8.7/PKG-INFO
+-rw-r--r--   0 esbiya     (501) staff       (20)       38 2023-03-15 09:37:56.000000 pynocaptcha-1.8.7/README.md
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-08 01:17:52.071203 pynocaptcha-1.8.7/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1095 2024-03-28 09:20:29.000000 pynocaptcha-1.8.7/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-08 01:17:52.072589 pynocaptcha-1.8.7/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1054 2023-11-15 10:37:10.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      668 2024-04-04 15:59:57.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/aws.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5116 2024-04-08 01:16:56.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1061 2024-02-27 06:17:10.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      744 2023-08-14 02:01:08.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/discord.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1221 2023-07-03 06:08:01.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2088 2024-01-15 06:49:23.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1559 2024-03-30 04:01:26.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/perimeterx.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     3077 2023-12-13 01:23:55.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/tls.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-08 01:17:52.071698 pynocaptcha-1.8.7/pynocaptcha.egg-info/
+-rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 esbiya     (501) staff       (20)      577 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/not-zip-safe
+-rw-r--r--   0 esbiya     (501) staff       (20)       15 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/requires.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)       33 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/top_level.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)       38 2024-04-08 01:17:52.072917 pynocaptcha-1.8.7/setup.cfg
+-rw-r--r--   0 esbiya     (501) staff       (20)      845 2024-04-08 01:16:25.000000 pynocaptcha-1.8.7/setup.py
```

### Comparing `pynocaptcha-1.8.6/LICENSE` & `pynocaptcha-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/PKG-INFO` & `pynocaptcha-1.8.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynocaptcha
-Version: 1.8.6
+Version: 1.8.7
 Summary: nocaptcha.io api
 License: MIT
 Keywords: nocaptcha
 Platform: all
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `pynocaptcha-1.8.6/pynocaptcha/__init__.py` & `pynocaptcha-1.8.7/pynocaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.8.7/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/pynocaptcha/crackers/aws.py` & `pynocaptcha-1.8.7/pynocaptcha/crackers/aws.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/pynocaptcha/crackers/base.py` & `pynocaptcha-1.8.7/pynocaptcha/crackers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         # cookies: dict = {},
         # proxy: str = None, 
         # timeout: int = 30,
         # debug: bool = False,
         # check_useful: bool = False,
         # max_retry_times: int = 3,
         # internal=True,
-        # internal_api=True,
         # auth=False,
         **kwargs
     ) -> None:
         """
         :param user_token: nocaptcha.io 用户 token
         :param developer_id: nocaptcha.io 用户上级代理 token
         :param user_agent: 请求流程使用 ua
@@ -63,15 +62,14 @@
         self.cookies = kwargs.get("cookies") or {}
         self.user_agent = kwargs.get("user_agent")
         self.proxy = kwargs.get("proxy")
         self.timeout = kwargs.get("timeout") or 30
         self.debug = kwargs.get("debug", False)
         self.check_useful = kwargs.get("check_useful", False)
         self.max_retry_times = kwargs.get("max_retry_times", 3)
-        self.internal_api = kwargs.get('internal_api', True)
         self.wanda_args = {
             "internal": kwargs.get('internal', True),
             "is_auth": kwargs.get('auth', False),
             "timeout": self.timeout
         }
         for k in self.must_check_params:
             _v = kwargs.get(k)
@@ -117,15 +115,15 @@
             self.wanda_args["proxy"] = self.proxy
 
         retry_times = 0        
         resp = {}
         while retry_times < self.max_retry_times:
             try:
                 resp = requests.post(
-                    f"http://{'xn--fjqs46frol.com' if self.internal_api else 'api.nocaptcha.io' }/api/wanda/{self.cracker_name}/{self.cracker_version}", 
+                    f"http://api.nocaptcha.io/api/wanda/{self.cracker_name}/{self.cracker_version}", 
                     headers=headers, json=self.wanda_args, timeout=self.timeout
                 ).json()
                 if self.debug:
                     logger.info(resp)
                 break
             except Exception as e:
                 if self.debug:
```

### Comparing `pynocaptcha-1.8.6/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.8.7/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/pynocaptcha/crackers/discord.py` & `pynocaptcha-1.8.7/pynocaptcha/crackers/discord.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.8.7/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.8.7/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/pynocaptcha/crackers/perimeterx.py` & `pynocaptcha-1.8.7/pynocaptcha/crackers/perimeterx.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.8.7/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/pynocaptcha/crackers/tls.py` & `pynocaptcha-1.8.7/pynocaptcha/crackers/tls.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/pynocaptcha.egg-info/PKG-INFO` & `pynocaptcha-1.8.7/pynocaptcha.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynocaptcha
-Version: 1.8.6
+Version: 1.8.7
 Summary: nocaptcha.io api
 License: MIT
 Keywords: nocaptcha
 Platform: all
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `pynocaptcha-1.8.6/pynocaptcha.egg-info/SOURCES.txt` & `pynocaptcha-1.8.7/pynocaptcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.6/setup.py` & `pynocaptcha-1.8.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 setup(
     name='pynocaptcha',
-    version='1.8.6',
+    version='1.8.7',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

