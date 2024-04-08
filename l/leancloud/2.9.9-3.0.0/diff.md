# Comparing `tmp/leancloud-2.9.9.tar.gz` & `tmp/leancloud-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leancloud-2.9.9.tar", last modified: Tue Dec 14 08:29:31 2021, max compression
+gzip compressed data, was "leancloud-3.0.0.tar", last modified: Mon Apr  8 06:38:47 2024, max compression
```

## Comparing `leancloud-2.9.9.tar` & `leancloud-3.0.0.tar`

### file list

```diff
@@ -1,42 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 08:29:31.678484 leancloud-2.9.9/
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2021-12-14 08:29:22.000000 leancloud-2.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      639 2021-12-14 08:29:31.678484 leancloud-2.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2021-12-14 08:29:22.000000 leancloud-2.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 08:29:31.678484 leancloud-2.9.9/leancloud/
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3644 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/acl.py
--rw-r--r--   0 runner    (1001) docker     (121)     2090 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/app_router.py
--rw-r--r--   0 runner    (1001) docker     (121)     7238 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5019 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     4113 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 08:29:31.678484 leancloud-2.9.9/leancloud/engine/
--rw-r--r--   0 runner    (1001) docker     (121)     6709 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/engine/authorization.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/engine/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     4352 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/engine/cookie_session.py
--rw-r--r--   0 runner    (1001) docker     (121)     3106 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/engine/cors.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/engine/https_redirect_middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)    18614 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/engine/leanengine.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    10105 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/file_.py
--rw-r--r--   0 runner    (1001) docker     (121)     3481 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/geo_point.py
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/message.py
--rw-r--r--   0 runner    (1001) docker     (121)    19183 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/object_.py
--rw-r--r--   0 runner    (1001) docker     (121)    11182 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/operation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3607 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/push.py
--rw-r--r--   0 runner    (1001) docker     (121)    22855 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     2999 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/role.py
--rw-r--r--   0 runner    (1001) docker     (121)     3895 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/sys_message.py
--rw-r--r--   0 runner    (1001) docker     (121)    12426 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     6863 2021-12-14 08:29:22.000000 leancloud-2.9.9/leancloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 08:29:31.678484 leancloud-2.9.9/leancloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      639 2021-12-14 08:29:31.000000 leancloud-2.9.9/leancloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      868 2021-12-14 08:29:31.000000 leancloud-2.9.9/leancloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-14 08:29:31.000000 leancloud-2.9.9/leancloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      328 2021-12-14 08:29:31.000000 leancloud-2.9.9/leancloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-14 08:29:31.000000 leancloud-2.9.9/leancloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-12-14 08:29:31.678484 leancloud-2.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2021-12-14 08:29:22.000000 leancloud-2.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:38:47.905838 leancloud-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-08 06:38:39.000000 leancloud-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-08 06:38:47.905838 leancloud-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-08 06:38:39.000000 leancloud-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:38:47.901838 leancloud-3.0.0/leancloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/app_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:38:47.901838 leancloud-3.0.0/leancloud/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/engine/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/engine/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/engine/cookie_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/engine/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/engine/https_redirect_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18614 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/engine/leanengine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/file_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/geo_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19183 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/object_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/push.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22855 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/sys_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-08 06:38:39.000000 leancloud-3.0.0/leancloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:38:47.905838 leancloud-3.0.0/leancloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-08 06:38:47.000000 leancloud-3.0.0/leancloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-08 06:38:47.000000 leancloud-3.0.0/leancloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:38:47.000000 leancloud-3.0.0/leancloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 06:38:47.000000 leancloud-3.0.0/leancloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 06:38:47.000000 leancloud-3.0.0/leancloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 06:38:47.909838 leancloud-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-08 06:38:39.000000 leancloud-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:38:47.905838 leancloud-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21454 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_geo_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10074 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15403 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_sys_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-08 06:38:39.000000 leancloud-3.0.0/tests/test_util.py
```

### Comparing `leancloud-2.9.9/LICENSE` & `leancloud-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/README.md` & `leancloud-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/__init__.py` & `leancloud-3.0.0/leancloud/__init__.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/acl.py` & `leancloud-3.0.0/leancloud/acl.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/app_router.py` & `leancloud-3.0.0/leancloud/app_router.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,32 +18,37 @@
         self.region = region
         self.hosts = {}
         self.session = requests.Session()
         self.lock = threading.Lock()
         self.expired_at = 0
 
         prefix = app_id[:8].lower()
-        domain = "lncld.net"
+        is_cn_n1 = False
 
         if region == "US":
             domain = "lncldglobal.com"
         elif region == "CN":
             if app_id.endswith("-9Nh9j0Va"):
                 domain = "lncldapi.com"
             elif app_id.endswith("-MdYXbMMI"):
                 domain = "lncldglobal.com"
             else:
-                domain = "lncld.net"
+                domain = "{}.lc-cn-n1-shared.com".format(prefix)
+                is_cn_n1 = True
         else:
             raise RuntimeError("invalid region: {}".format(region))
 
-        self.hosts["api"] = "{}.api.{}".format(prefix, domain)
-        self.hosts["engine"] = "{}.engine.{}".format(prefix, domain)
-        self.hosts["stats"] = "{}.stats.{}".format(prefix, domain)
-        self.hosts["push"] = "{}.push.{}".format(prefix, domain)
+        if is_cn_n1:
+            self.hosts.update(dict.fromkeys(
+                ["api", "engine", "stats", "push"], domain))
+        else:
+            self.hosts["api"] = "{}.api.{}".format(prefix, domain)
+            self.hosts["engine"] = "{}.engine.{}".format(prefix, domain)
+            self.hosts["stats"] = "{}.stats.{}".format(prefix, domain)
+            self.hosts["push"] = "{}.push.{}".format(prefix, domain)
 
     def get(self, type_):
         with self.lock:
             if time.time() > self.expired_at:
                 self.expired_at += 600
                 threading.Thread(target=self.refresh).start()
             return self.hosts[type_]
```

### Comparing `leancloud-2.9.9/leancloud/client.py` & `leancloud-3.0.0/leancloud/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         return func(headers=headers, *args, **kwargs)
 
     return new_func
 
 
 def get_url(part):
     # try to use the base URL from environ
-    url = os.environ.get("LC_API_SERVER") or os.environ.get("LEANCLOUD_API_SERVER")
+    url = os.environ.get("LEANCLOUD_API_SERVER") or os.environ.get("LC_API_SERVER")
     if url:
         return "{}/{}{}".format(url, SERVER_VERSION, part)
 
     global app_router
     if app_router is None:
         app_router = AppRouter(APP_ID, REGION)
```

### Comparing `leancloud-2.9.9/leancloud/cloud.py` & `leancloud-3.0.0/leancloud/cloud.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/conversation.py` & `leancloud-3.0.0/leancloud/conversation.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/engine/__init__.py` & `leancloud-3.0.0/leancloud/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/engine/authorization.py` & `leancloud-3.0.0/leancloud/engine/authorization.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/engine/context.py` & `leancloud-3.0.0/leancloud/engine/context.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/engine/cookie_session.py` & `leancloud-3.0.0/leancloud/engine/cookie_session.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/engine/cors.py` & `leancloud-3.0.0/leancloud/engine/cors.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/engine/https_redirect_middleware.py` & `leancloud-3.0.0/leancloud/engine/https_redirect_middleware.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/engine/leanengine.py` & `leancloud-3.0.0/leancloud/engine/leanengine.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/engine/utils.py` & `leancloud-3.0.0/leancloud/engine/utils.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/errors.py` & `leancloud-3.0.0/leancloud/errors.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/file_.py` & `leancloud-3.0.0/leancloud/file_.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/geo_point.py` & `leancloud-3.0.0/leancloud/geo_point.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/message.py` & `leancloud-3.0.0/leancloud/message.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/object_.py` & `leancloud-3.0.0/leancloud/object_.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/operation.py` & `leancloud-3.0.0/leancloud/operation.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/push.py` & `leancloud-3.0.0/leancloud/push.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/query.py` & `leancloud-3.0.0/leancloud/query.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/relation.py` & `leancloud-3.0.0/leancloud/relation.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/role.py` & `leancloud-3.0.0/leancloud/role.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/status.py` & `leancloud-3.0.0/leancloud/status.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/sys_message.py` & `leancloud-3.0.0/leancloud/sys_message.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/leancloud/user.py` & `leancloud-3.0.0/leancloud/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,16 +331,16 @@
     def request_password_reset_by_sms_code(cls, phone_number, validate_token=None):
         params = {"mobilePhoneNumber": phone_number}
         if validate_token is not None:
             params["validate_token"] = validate_token
         client.post("/requestPasswordResetBySmsCode", params)
 
     @classmethod
-    def reset_password_by_sms_code(cls, sms_code, new_password):
-        params = {"password": new_password}
+    def reset_password_by_sms_code(cls, sms_code, new_password, phone_number):
+        params = {"password": new_password, "mobilePhoneNumber": phone_number}
         client.put("/resetPasswordBySmsCode/" + sms_code, params)
 
     # This should be an instance method.
     # However, to be consistent with other similar methods (`request_password_reset_by_sms_code`),
     # it is implemented as a class method.
     @classmethod
     def request_change_phone_number(cls, phone_number, ttl=None, validate_token=None):
@@ -355,16 +355,17 @@
     # but it is implemented as a class method for the same reason as above.
     @classmethod
     def change_phone_number(cls, sms_code, phone_number):
         params = {"mobilePhoneNumber": phone_number, "code": sms_code}
         client.post("/changePhoneNumber", params)
 
     @classmethod
-    def verify_mobile_phone_number(cls, sms_code):
-        client.post("/verfyMobilePhone/" + sms_code, {})
+    def verify_mobile_phone_number(cls, sms_code, phone_number):
+        params = {"mobilePhoneNumber": phone_number}
+        client.post("/verifyMobilePhone/" + sms_code, params)
 
     @classmethod
     def request_login_sms_code(cls, phone_number, validate_token=None):
         params = {"mobilePhoneNumber": phone_number}
         if validate_token is not None:
             params["validate_token"] = validate_token
         client.post("/requestLoginSmsCode", params)
```

### Comparing `leancloud-2.9.9/leancloud/utils.py` & `leancloud-3.0.0/leancloud/utils.py`

 * *Files identical despite different names*

### Comparing `leancloud-2.9.9/setup.py` & `leancloud-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,34 +10,35 @@
     "arrow>=1.0.0,<2.0.0; python_version >= '3.6'",
     'iso8601>=0.1.14',
     'six>=1.11.0',
     'qiniu==7.3.1',
     'requests>=2.25.1',
     'Werkzeug>=0.16.0,<2.0.0',
     'secure-cookie>=0.1.0,<1.0.0',
-    'gevent>=21.1.0,<22.0.0',
-    "typing; python_version < '3.5'"
+    'gevent>=22.10.2,<23.0.0',
+    "typing; python_version < '3.5'",
+    'markupsafe<=2.0.1',
 ]
 
 setup(
     name='leancloud',
-    version='2.9.9',
+    version='3.0.0',
     description='LeanCloud Python SDK',
     url='https://leancloud.cn/',
     author='asaka',
     author_email='lan@leancloud.rocks',
     license='LGPL',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.9',
     ],
     keywords='Leancloud SDK',
     packages=find_packages(exclude=['docs', 'tests*']),
     test_suite='nose.collector',
     install_requires=install_requires,
     extras_require={
         'dev': ['sphinx', 'sphinx_rtd_theme'],
```

