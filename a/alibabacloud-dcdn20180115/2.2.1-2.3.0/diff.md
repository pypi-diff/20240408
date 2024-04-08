# Comparing `tmp/alibabacloud_dcdn20180115-2.2.1.tar.gz` & `tmp/alibabacloud_dcdn20180115-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dcdn20180115-2.2.1.tar", last modified: Thu Mar 21 17:13:52 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dcdn20180115-2.3.0.tar", last modified: Mon Apr  8 17:08:33 2024, max compression
```

## Comparing `alibabacloud_dcdn20180115-2.2.1.tar` & `alibabacloud_dcdn20180115-2.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:52.000000 alibabacloud_dcdn20180115-2.2.1/
--rw-r--r--   0 root         (0) root         (0)     3953 2024-03-21 17:13:51.000000 alibabacloud_dcdn20180115-2.2.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-21 17:13:51.000000 alibabacloud_dcdn20180115-2.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-21 17:13:51.000000 alibabacloud_dcdn20180115-2.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2408 2024-03-21 17:13:52.000000 alibabacloud_dcdn20180115-2.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2024-03-21 17:13:51.000000 alibabacloud_dcdn20180115-2.2.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1184 2024-03-21 17:13:51.000000 alibabacloud_dcdn20180115-2.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:52.000000 alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-21 17:13:51.000000 alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1046408 2024-03-21 17:13:51.000000 alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115/client.py
--rw-r--r--   0 root         (0) root         (0)  1405734 2024-03-21 17:13:51.000000 alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:52.000000 alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2408 2024-03-21 17:13:52.000000 alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2024-03-21 17:13:52.000000 alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 17:13:52.000000 alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-21 17:13:52.000000 alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-03-21 17:13:52.000000 alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-21 17:13:52.000000 alibabacloud_dcdn20180115-2.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2616 2024-03-21 17:13:51.000000 alibabacloud_dcdn20180115-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)     4098 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1059206 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/client.py
+-rw-r--r--   0 root         (0) root         (0)  1418866 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/setup.py
```

### Comparing `alibabacloud_dcdn20180115-2.2.1/ChangeLog.md` & `alibabacloud_dcdn20180115-2.3.0/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-03-21 Version: 2.2.1
+- Update API DescribeDcdnKvNamespace: update response param.
+- Update API PutDcdnKvNamespace: update response param.
+
+
 2024-01-08 Version: 2.2.0
 - Generated python 2018-01-15 for dcdn.
 
 2023-12-27 Version: 2.1.0
 - Generated python 2018-01-15 for dcdn.
 
 2023-12-08 Version: 2.0.0
```

### Comparing `alibabacloud_dcdn20180115-2.2.1/LICENSE` & `alibabacloud_dcdn20180115-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115-2.2.1/PKG-INFO` & `alibabacloud_dcdn20180115-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dcdn20180115
-Version: 2.2.1
+Version: 2.3.0
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115-2.2.1/README-CN.md` & `alibabacloud_dcdn20180115-2.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115-2.2.1/README.md` & `alibabacloud_dcdn20180115-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115/client.py` & `alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -757,14 +757,174 @@
         
         @param request: BatchDeleteDcdnDomainConfigsRequest
         @return: BatchDeleteDcdnDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_delete_dcdn_domain_configs_with_options_async(request, runtime)
 
+    def batch_delete_dcdn_kv_with_options(
+        self,
+        tmp_req: dcdn_20180115_models.BatchDeleteDcdnKvRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dcdn_20180115_models.BatchDeleteDcdnKvResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dcdn_20180115_models.BatchDeleteDcdnKvShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.keys):
+            request.keys_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.keys, 'Keys', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.namespace):
+            query['Namespace'] = request.namespace
+        body = {}
+        if not UtilClient.is_unset(request.keys_shrink):
+            body['Keys'] = request.keys_shrink
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchDeleteDcdnKv',
+            version='2018-01-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dcdn_20180115_models.BatchDeleteDcdnKvResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def batch_delete_dcdn_kv_with_options_async(
+        self,
+        tmp_req: dcdn_20180115_models.BatchDeleteDcdnKvRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dcdn_20180115_models.BatchDeleteDcdnKvResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dcdn_20180115_models.BatchDeleteDcdnKvShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.keys):
+            request.keys_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.keys, 'Keys', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.namespace):
+            query['Namespace'] = request.namespace
+        body = {}
+        if not UtilClient.is_unset(request.keys_shrink):
+            body['Keys'] = request.keys_shrink
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchDeleteDcdnKv',
+            version='2018-01-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dcdn_20180115_models.BatchDeleteDcdnKvResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def batch_delete_dcdn_kv(
+        self,
+        request: dcdn_20180115_models.BatchDeleteDcdnKvRequest,
+    ) -> dcdn_20180115_models.BatchDeleteDcdnKvResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.batch_delete_dcdn_kv_with_options(request, runtime)
+
+    async def batch_delete_dcdn_kv_async(
+        self,
+        request: dcdn_20180115_models.BatchDeleteDcdnKvRequest,
+    ) -> dcdn_20180115_models.BatchDeleteDcdnKvResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.batch_delete_dcdn_kv_with_options_async(request, runtime)
+
+    def batch_delete_dcdn_kv_with_high_capacity_with_options(
+        self,
+        request: dcdn_20180115_models.BatchDeleteDcdnKvWithHighCapacityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dcdn_20180115_models.BatchDeleteDcdnKvWithHighCapacityResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.namespace):
+            query['Namespace'] = request.namespace
+        if not UtilClient.is_unset(request.url):
+            query['Url'] = request.url
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='BatchDeleteDcdnKvWithHighCapacity',
+            version='2018-01-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dcdn_20180115_models.BatchDeleteDcdnKvWithHighCapacityResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def batch_delete_dcdn_kv_with_high_capacity_with_options_async(
+        self,
+        request: dcdn_20180115_models.BatchDeleteDcdnKvWithHighCapacityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dcdn_20180115_models.BatchDeleteDcdnKvWithHighCapacityResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.namespace):
+            query['Namespace'] = request.namespace
+        if not UtilClient.is_unset(request.url):
+            query['Url'] = request.url
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='BatchDeleteDcdnKvWithHighCapacity',
+            version='2018-01-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dcdn_20180115_models.BatchDeleteDcdnKvWithHighCapacityResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def batch_delete_dcdn_kv_with_high_capacity(
+        self,
+        request: dcdn_20180115_models.BatchDeleteDcdnKvWithHighCapacityRequest,
+    ) -> dcdn_20180115_models.BatchDeleteDcdnKvWithHighCapacityResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.batch_delete_dcdn_kv_with_high_capacity_with_options(request, runtime)
+
+    async def batch_delete_dcdn_kv_with_high_capacity_async(
+        self,
+        request: dcdn_20180115_models.BatchDeleteDcdnKvWithHighCapacityRequest,
+    ) -> dcdn_20180115_models.BatchDeleteDcdnKvWithHighCapacityResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.batch_delete_dcdn_kv_with_high_capacity_with_options_async(request, runtime)
+
     def batch_delete_dcdn_waf_rules_with_options(
         self,
         request: dcdn_20180115_models.BatchDeleteDcdnWafRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchDeleteDcdnWafRulesResponse:
         """
         You can call this operation up to 20 times per second per account.
@@ -968,20 +1128,22 @@
     ) -> dcdn_20180115_models.BatchPutDcdnKvResponse:
         UtilClient.validate_model(tmp_req)
         request = dcdn_20180115_models.BatchPutDcdnKvShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.kv_list):
             request.kv_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.kv_list, 'KvList', 'json')
         query = {}
-        if not UtilClient.is_unset(request.kv_list_shrink):
-            query['KvList'] = request.kv_list_shrink
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
+        body = {}
+        if not UtilClient.is_unset(request.kv_list_shrink):
+            body['KvList'] = request.kv_list_shrink
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='BatchPutDcdnKv',
             version='2018-01-15',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -1002,20 +1164,22 @@
     ) -> dcdn_20180115_models.BatchPutDcdnKvResponse:
         UtilClient.validate_model(tmp_req)
         request = dcdn_20180115_models.BatchPutDcdnKvShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.kv_list):
             request.kv_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.kv_list, 'KvList', 'json')
         query = {}
-        if not UtilClient.is_unset(request.kv_list_shrink):
-            query['KvList'] = request.kv_list_shrink
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
+        body = {}
+        if not UtilClient.is_unset(request.kv_list_shrink):
+            body['KvList'] = request.kv_list_shrink
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='BatchPutDcdnKv',
             version='2018-01-15',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -1039,14 +1203,88 @@
     async def batch_put_dcdn_kv_async(
         self,
         request: dcdn_20180115_models.BatchPutDcdnKvRequest,
     ) -> dcdn_20180115_models.BatchPutDcdnKvResponse:
         runtime = util_models.RuntimeOptions()
         return await self.batch_put_dcdn_kv_with_options_async(request, runtime)
 
+    def batch_put_dcdn_kv_with_high_capacity_with_options(
+        self,
+        request: dcdn_20180115_models.BatchPutDcdnKvWithHighCapacityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dcdn_20180115_models.BatchPutDcdnKvWithHighCapacityResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.namespace):
+            query['Namespace'] = request.namespace
+        if not UtilClient.is_unset(request.url):
+            query['Url'] = request.url
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='BatchPutDcdnKvWithHighCapacity',
+            version='2018-01-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dcdn_20180115_models.BatchPutDcdnKvWithHighCapacityResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def batch_put_dcdn_kv_with_high_capacity_with_options_async(
+        self,
+        request: dcdn_20180115_models.BatchPutDcdnKvWithHighCapacityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dcdn_20180115_models.BatchPutDcdnKvWithHighCapacityResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.namespace):
+            query['Namespace'] = request.namespace
+        if not UtilClient.is_unset(request.url):
+            query['Url'] = request.url
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='BatchPutDcdnKvWithHighCapacity',
+            version='2018-01-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dcdn_20180115_models.BatchPutDcdnKvWithHighCapacityResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def batch_put_dcdn_kv_with_high_capacity(
+        self,
+        request: dcdn_20180115_models.BatchPutDcdnKvWithHighCapacityRequest,
+    ) -> dcdn_20180115_models.BatchPutDcdnKvWithHighCapacityResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.batch_put_dcdn_kv_with_high_capacity_with_options(request, runtime)
+
+    async def batch_put_dcdn_kv_with_high_capacity_async(
+        self,
+        request: dcdn_20180115_models.BatchPutDcdnKvWithHighCapacityRequest,
+    ) -> dcdn_20180115_models.BatchPutDcdnKvWithHighCapacityResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.batch_put_dcdn_kv_with_high_capacity_with_options_async(request, runtime)
+
     def batch_set_dcdn_domain_certificate_with_options(
         self,
         request: dcdn_20180115_models.BatchSetDcdnDomainCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.BatchSetDcdnDomainCertificateResponse:
         """
         > You can call this operation up to 10 times per second per account.
@@ -20619,14 +20857,92 @@
     async def put_dcdn_kv_namespace_async(
         self,
         request: dcdn_20180115_models.PutDcdnKvNamespaceRequest,
     ) -> dcdn_20180115_models.PutDcdnKvNamespaceResponse:
         runtime = util_models.RuntimeOptions()
         return await self.put_dcdn_kv_namespace_with_options_async(request, runtime)
 
+    def put_dcdn_kv_with_high_capacity_with_options(
+        self,
+        request: dcdn_20180115_models.PutDcdnKvWithHighCapacityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dcdn_20180115_models.PutDcdnKvWithHighCapacityResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.key):
+            query['Key'] = request.key
+        if not UtilClient.is_unset(request.namespace):
+            query['Namespace'] = request.namespace
+        if not UtilClient.is_unset(request.url):
+            query['Url'] = request.url
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='PutDcdnKvWithHighCapacity',
+            version='2018-01-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dcdn_20180115_models.PutDcdnKvWithHighCapacityResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def put_dcdn_kv_with_high_capacity_with_options_async(
+        self,
+        request: dcdn_20180115_models.PutDcdnKvWithHighCapacityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dcdn_20180115_models.PutDcdnKvWithHighCapacityResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.key):
+            query['Key'] = request.key
+        if not UtilClient.is_unset(request.namespace):
+            query['Namespace'] = request.namespace
+        if not UtilClient.is_unset(request.url):
+            query['Url'] = request.url
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='PutDcdnKvWithHighCapacity',
+            version='2018-01-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dcdn_20180115_models.PutDcdnKvWithHighCapacityResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def put_dcdn_kv_with_high_capacity(
+        self,
+        request: dcdn_20180115_models.PutDcdnKvWithHighCapacityRequest,
+    ) -> dcdn_20180115_models.PutDcdnKvWithHighCapacityResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.put_dcdn_kv_with_high_capacity_with_options(request, runtime)
+
+    async def put_dcdn_kv_with_high_capacity_async(
+        self,
+        request: dcdn_20180115_models.PutDcdnKvWithHighCapacityRequest,
+    ) -> dcdn_20180115_models.PutDcdnKvWithHighCapacityResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.put_dcdn_kv_with_high_capacity_with_options_async(request, runtime)
+
     def refresh_dcdn_object_caches_with_options(
         self,
         request: dcdn_20180115_models.RefreshDcdnObjectCachesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.RefreshDcdnObjectCachesResponse:
         """
         DCDN supports POST requests in which parameters are sent as a form.
```

### Comparing `alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115/models.py` & `alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -895,14 +895,273 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = BatchDeleteDcdnDomainConfigsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BatchDeleteDcdnKvRequest(TeaModel):
+    def __init__(
+        self,
+        keys: List[str] = None,
+        namespace: str = None,
+    ):
+        self.keys = keys
+        self.namespace = namespace
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.keys is not None:
+            result['Keys'] = self.keys
+        if self.namespace is not None:
+            result['Namespace'] = self.namespace
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Keys') is not None:
+            self.keys = m.get('Keys')
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        return self
+
+
+class BatchDeleteDcdnKvShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        keys_shrink: str = None,
+        namespace: str = None,
+    ):
+        self.keys_shrink = keys_shrink
+        self.namespace = namespace
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.keys_shrink is not None:
+            result['Keys'] = self.keys_shrink
+        if self.namespace is not None:
+            result['Namespace'] = self.namespace
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Keys') is not None:
+            self.keys_shrink = m.get('Keys')
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        return self
+
+
+class BatchDeleteDcdnKvResponseBody(TeaModel):
+    def __init__(
+        self,
+        fail_keys: List[str] = None,
+        request_id: str = None,
+        success_keys: List[str] = None,
+    ):
+        self.fail_keys = fail_keys
+        self.request_id = request_id
+        self.success_keys = success_keys
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.fail_keys is not None:
+            result['FailKeys'] = self.fail_keys
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success_keys is not None:
+            result['SuccessKeys'] = self.success_keys
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FailKeys') is not None:
+            self.fail_keys = m.get('FailKeys')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('SuccessKeys') is not None:
+            self.success_keys = m.get('SuccessKeys')
+        return self
+
+
+class BatchDeleteDcdnKvResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: BatchDeleteDcdnKvResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = BatchDeleteDcdnKvResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class BatchDeleteDcdnKvWithHighCapacityRequest(TeaModel):
+    def __init__(
+        self,
+        namespace: str = None,
+        url: str = None,
+    ):
+        self.namespace = namespace
+        self.url = url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.namespace is not None:
+            result['Namespace'] = self.namespace
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
+class BatchDeleteDcdnKvWithHighCapacityResponseBody(TeaModel):
+    def __init__(
+        self,
+        fail_keys: List[str] = None,
+        request_id: str = None,
+        success_keys: List[str] = None,
+    ):
+        self.fail_keys = fail_keys
+        self.request_id = request_id
+        self.success_keys = success_keys
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.fail_keys is not None:
+            result['FailKeys'] = self.fail_keys
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success_keys is not None:
+            result['SuccessKeys'] = self.success_keys
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FailKeys') is not None:
+            self.fail_keys = m.get('FailKeys')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('SuccessKeys') is not None:
+            self.success_keys = m.get('SuccessKeys')
+        return self
+
+
+class BatchDeleteDcdnKvWithHighCapacityResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: BatchDeleteDcdnKvWithHighCapacityResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = BatchDeleteDcdnKvWithHighCapacityResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class BatchDeleteDcdnWafRulesRequest(TeaModel):
     def __init__(
         self,
         rule_ids: str = None,
     ):
         # The IDs of the protection rules that you want to delete. Separate multiple IDs with commas (,).
         self.rule_ids = rule_ids
@@ -1104,21 +1363,17 @@
     def __init__(
         self,
         expiration: int = None,
         expiration_ttl: int = None,
         key: str = None,
         value: str = None,
     ):
-        # The expiration time. The value is a timestamp in seconds. The expiration time cannot be earlier than the current time. If you specify Expiration and ExpirationTtl, only ExpirationTtl takes effect.
         self.expiration = expiration
-        # The relative expiration time. Unit: seconds. If you specify Expiration and ExpirationTtl, only ExpirationTtl takes effect.
         self.expiration_ttl = expiration_ttl
-        # The key. The key can be up to 512 characters in length and cannot contain spaces.
         self.key = key
-        # The value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1151,15 +1406,14 @@
 
 class BatchPutDcdnKvRequest(TeaModel):
     def __init__(
         self,
         kv_list: List[BatchPutDcdnKvRequestKvList] = None,
         namespace: str = None,
     ):
-        # The key-value pairs. The key-value pairs can be up to 2 MB in size.
         self.kv_list = kv_list
         # The name of the namespace.
         self.namespace = namespace
 
     def validate(self):
         if self.kv_list:
             for k in self.kv_list:
@@ -1194,15 +1448,14 @@
 
 class BatchPutDcdnKvShrinkRequest(TeaModel):
     def __init__(
         self,
         kv_list_shrink: str = None,
         namespace: str = None,
     ):
-        # The key-value pairs. The key-value pairs can be up to 2 MB in size.
         self.kv_list_shrink = kv_list_shrink
         # The name of the namespace.
         self.namespace = namespace
 
     def validate(self):
         pass
 
@@ -1306,14 +1559,127 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = BatchPutDcdnKvResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BatchPutDcdnKvWithHighCapacityRequest(TeaModel):
+    def __init__(
+        self,
+        namespace: str = None,
+        url: str = None,
+    ):
+        self.namespace = namespace
+        self.url = url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.namespace is not None:
+            result['Namespace'] = self.namespace
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
+class BatchPutDcdnKvWithHighCapacityResponseBody(TeaModel):
+    def __init__(
+        self,
+        fail_keys: List[str] = None,
+        request_id: str = None,
+        success_keys: List[str] = None,
+    ):
+        self.fail_keys = fail_keys
+        self.request_id = request_id
+        self.success_keys = success_keys
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.fail_keys is not None:
+            result['FailKeys'] = self.fail_keys
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success_keys is not None:
+            result['SuccessKeys'] = self.success_keys
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FailKeys') is not None:
+            self.fail_keys = m.get('FailKeys')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('SuccessKeys') is not None:
+            self.success_keys = m.get('SuccessKeys')
+        return self
+
+
+class BatchPutDcdnKvWithHighCapacityResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: BatchPutDcdnKvWithHighCapacityResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = BatchPutDcdnKvWithHighCapacityResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class BatchSetDcdnDomainCertificateRequest(TeaModel):
     def __init__(
         self,
         cert_name: str = None,
         cert_type: str = None,
         domain_name: str = None,
         owner_id: int = None,
@@ -38712,14 +39078,133 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PutDcdnKvNamespaceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PutDcdnKvWithHighCapacityRequest(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        namespace: str = None,
+        url: str = None,
+    ):
+        self.key = key
+        self.namespace = namespace
+        self.url = url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.namespace is not None:
+            result['Namespace'] = self.namespace
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
+class PutDcdnKvWithHighCapacityResponseBody(TeaModel):
+    def __init__(
+        self,
+        length: int = None,
+        request_id: str = None,
+        value: str = None,
+    ):
+        self.length = length
+        self.request_id = request_id
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.length is not None:
+            result['Length'] = self.length
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Length') is not None:
+            self.length = m.get('Length')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class PutDcdnKvWithHighCapacityResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PutDcdnKvWithHighCapacityResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = PutDcdnKvWithHighCapacityResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RefreshDcdnObjectCachesRequest(TeaModel):
     def __init__(
         self,
         force: bool = None,
         object_path: str = None,
         object_type: str = None,
         owner_id: int = None,
```

### Comparing `alibabacloud_dcdn20180115-2.2.1/alibabacloud_dcdn20180115.egg-info/PKG-INFO` & `alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dcdn20180115
-Version: 2.2.1
+Version: 2.3.0
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115-2.2.1/setup.py` & `alibabacloud_dcdn20180115-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dcdn20180115.
 
-Created on 21/03/2024
+Created on 08/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dcdn20180115"
 NAME = "alibabacloud_dcdn20180115" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dcdn (20180115) SDK Library for Python"
```

