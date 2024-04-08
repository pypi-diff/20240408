# Comparing `tmp/alibabacloud_dcdn20180115_py2-2.2.0.tar.gz` & `tmp/alibabacloud_dcdn20180115_py2-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dcdn20180115_py2-2.2.0.tar", last modified: Thu Mar 21 17:13:45 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dcdn20180115_py2-2.3.0.tar", last modified: Mon Apr  8 17:07:44 2024, max compression
```

## Comparing `alibabacloud_dcdn20180115_py2-2.2.0.tar` & `alibabacloud_dcdn20180115_py2-2.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:45.000000 alibabacloud_dcdn20180115_py2-2.2.0/
--rw-r--r--   0 root         (0) root         (0)     3676 2024-03-21 17:13:44.000000 alibabacloud_dcdn20180115_py2-2.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-21 17:13:44.000000 alibabacloud_dcdn20180115_py2-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-21 17:13:44.000000 alibabacloud_dcdn20180115_py2-2.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2024-03-21 17:13:45.000000 alibabacloud_dcdn20180115_py2-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2024-03-21 17:13:44.000000 alibabacloud_dcdn20180115_py2-2.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2024-03-21 17:13:44.000000 alibabacloud_dcdn20180115_py2-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:45.000000 alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-21 17:13:44.000000 alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115/__init__.py
--rw-r--r--   0 root         (0) root         (0)   454804 2024-03-21 17:13:44.000000 alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115/client.py
--rw-r--r--   0 root         (0) root         (0)  1423742 2024-03-21 17:13:44.000000 alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:45.000000 alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2024-03-21 17:13:45.000000 alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2024-03-21 17:13:45.000000 alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 17:13:45.000000 alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-21 17:13:45.000000 alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-03-21 17:13:45.000000 alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-21 17:13:45.000000 alibabacloud_dcdn20180115_py2-2.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2024-03-21 17:13:44.000000 alibabacloud_dcdn20180115_py2-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)     3915 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   459855 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/client.py
+-rw-r--r--   0 root         (0) root         (0)  1437036 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/setup.py
```

### Comparing `alibabacloud_dcdn20180115_py2-2.2.0/ChangeLog.md` & `alibabacloud_dcdn20180115_py2-2.3.0/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+2024-03-21 Version: 2.2.0
+- Support API CreateDcdnCertificateSigningRequest.
+- Support API SetDcdnDomainCSRCertificate.
+- Update API DescribeDcdnKvNamespace: update response param.
+- Update API PutDcdnKvNamespace: update response param.
+
+
 2023-12-27 Version: 2.1.0
 - Generated python2 2018-01-15 for dcdn.
 
 2023-12-08 Version: 2.0.0
 - Generated python2 2018-01-15 for dcdn.
 
 2023-11-23 Version: 1.10.0
```

### Comparing `alibabacloud_dcdn20180115_py2-2.2.0/LICENSE` & `alibabacloud_dcdn20180115_py2-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-2.2.0/PKG-INFO` & `alibabacloud_dcdn20180115_py2-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dcdn20180115_py2
-Version: 2.2.0
+Version: 2.3.0
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115_py2-2.2.0/README-CN.md` & `alibabacloud_dcdn20180115_py2-2.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-2.2.0/README.md` & `alibabacloud_dcdn20180115_py2-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115/client.py` & `alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,14 +404,80 @@
         @param request: BatchDeleteDcdnDomainConfigsRequest
 
         @return: BatchDeleteDcdnDomainConfigsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_delete_dcdn_domain_configs_with_options(request, runtime)
 
+    def batch_delete_dcdn_kv_with_options(self, tmp_req, runtime):
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
+    def batch_delete_dcdn_kv(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.batch_delete_dcdn_kv_with_options(request, runtime)
+
+    def batch_delete_dcdn_kv_with_high_capacity_with_options(self, request, runtime):
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
+    def batch_delete_dcdn_kv_with_high_capacity(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.batch_delete_dcdn_kv_with_high_capacity_with_options(request, runtime)
+
     def batch_delete_dcdn_waf_rules_with_options(self, request, runtime):
         """
         You can call this operation up to 20 times per second per account.
         *   Alibaba Cloud Dynamic Content Delivery Network (DCDN) supports POST requests.
         
 
         @param request: BatchDeleteDcdnWafRulesRequest
@@ -507,20 +573,22 @@
     def batch_put_dcdn_kv_with_options(self, tmp_req, runtime):
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
@@ -534,14 +602,44 @@
             self.call_api(params, req, runtime)
         )
 
     def batch_put_dcdn_kv(self, request):
         runtime = util_models.RuntimeOptions()
         return self.batch_put_dcdn_kv_with_options(request, runtime)
 
+    def batch_put_dcdn_kv_with_high_capacity_with_options(self, request, runtime):
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
+    def batch_put_dcdn_kv_with_high_capacity(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.batch_put_dcdn_kv_with_high_capacity_with_options(request, runtime)
+
     def batch_set_dcdn_domain_certificate_with_options(self, request, runtime):
         """
         > You can call this operation up to 10 times per second per account.
         
 
         @param request: BatchSetDcdnDomainCertificateRequest
 
@@ -9824,14 +9922,46 @@
             self.call_api(params, req, runtime)
         )
 
     def put_dcdn_kv_namespace(self, request):
         runtime = util_models.RuntimeOptions()
         return self.put_dcdn_kv_namespace_with_options(request, runtime)
 
+    def put_dcdn_kv_with_high_capacity_with_options(self, request, runtime):
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
+    def put_dcdn_kv_with_high_capacity(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.put_dcdn_kv_with_high_capacity_with_options(request, runtime)
+
     def refresh_dcdn_object_caches_with_options(self, request, runtime):
         """
         DCDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshDcdnObjectCaches](~~130620~~) operation to refresh content and call the [PreloadDcdnObjectCaches](~~130636~~) operation to prefetch content.
         *   By default, each Alibaba Cloud account can refresh content from a maximum of 10,000 URLs and 100 directories per day, including subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. DCDN evaluates your application based on your workloads.
         *   You can specify up to 1,000 URLs or 100 directories that you want to refresh in each request.
         *   You can refresh a maximum of 1,000 URLs per minute for each domain name.
```

### Comparing `alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115/models.py` & `alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -793,14 +793,241 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = BatchDeleteDcdnDomainConfigsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BatchDeleteDcdnKvRequest(TeaModel):
+    def __init__(self, keys=None, namespace=None):
+        self.keys = keys  # type: list[str]
+        self.namespace = namespace  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BatchDeleteDcdnKvRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Keys') is not None:
+            self.keys = m.get('Keys')
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        return self
+
+
+class BatchDeleteDcdnKvShrinkRequest(TeaModel):
+    def __init__(self, keys_shrink=None, namespace=None):
+        self.keys_shrink = keys_shrink  # type: str
+        self.namespace = namespace  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BatchDeleteDcdnKvShrinkRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Keys') is not None:
+            self.keys_shrink = m.get('Keys')
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        return self
+
+
+class BatchDeleteDcdnKvResponseBody(TeaModel):
+    def __init__(self, fail_keys=None, request_id=None, success_keys=None):
+        self.fail_keys = fail_keys  # type: list[str]
+        self.request_id = request_id  # type: str
+        self.success_keys = success_keys  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BatchDeleteDcdnKvResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: BatchDeleteDcdnKvResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(BatchDeleteDcdnKvResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, namespace=None, url=None):
+        self.namespace = namespace  # type: str
+        self.url = url  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BatchDeleteDcdnKvWithHighCapacityRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
+class BatchDeleteDcdnKvWithHighCapacityResponseBody(TeaModel):
+    def __init__(self, fail_keys=None, request_id=None, success_keys=None):
+        self.fail_keys = fail_keys  # type: list[str]
+        self.request_id = request_id  # type: str
+        self.success_keys = success_keys  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BatchDeleteDcdnKvWithHighCapacityResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: BatchDeleteDcdnKvWithHighCapacityResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(BatchDeleteDcdnKvWithHighCapacityResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, rule_ids=None):
         # The IDs of the protection rules that you want to delete. Separate multiple IDs with commas (,).
         self.rule_ids = rule_ids  # type: str
 
     def validate(self):
         pass
@@ -973,21 +1200,17 @@
             temp_model = BatchModifyDcdnWafRulesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BatchPutDcdnKvRequestKvList(TeaModel):
     def __init__(self, expiration=None, expiration_ttl=None, key=None, value=None):
-        # The expiration time. The value is a timestamp in seconds. The expiration time cannot be earlier than the current time. If you specify Expiration and ExpirationTtl, only ExpirationTtl takes effect.
         self.expiration = expiration  # type: long
-        # The relative expiration time. Unit: seconds. If you specify Expiration and ExpirationTtl, only ExpirationTtl takes effect.
         self.expiration_ttl = expiration_ttl  # type: long
-        # The key. The key can be up to 512 characters in length and cannot contain spaces.
         self.key = key  # type: str
-        # The value.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchPutDcdnKvRequestKvList, self).to_map()
@@ -1016,15 +1239,14 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class BatchPutDcdnKvRequest(TeaModel):
     def __init__(self, kv_list=None, namespace=None):
-        # The key-value pairs. The key-value pairs can be up to 2 MB in size.
         self.kv_list = kv_list  # type: list[BatchPutDcdnKvRequestKvList]
         # The name of the namespace.
         self.namespace = namespace  # type: str
 
     def validate(self):
         if self.kv_list:
             for k in self.kv_list:
@@ -1055,15 +1277,14 @@
         if m.get('Namespace') is not None:
             self.namespace = m.get('Namespace')
         return self
 
 
 class BatchPutDcdnKvShrinkRequest(TeaModel):
     def __init__(self, kv_list_shrink=None, namespace=None):
-        # The key-value pairs. The key-value pairs can be up to 2 MB in size.
         self.kv_list_shrink = kv_list_shrink  # type: str
         # The name of the namespace.
         self.namespace = namespace  # type: str
 
     def validate(self):
         pass
 
@@ -1157,14 +1378,113 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = BatchPutDcdnKvResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BatchPutDcdnKvWithHighCapacityRequest(TeaModel):
+    def __init__(self, namespace=None, url=None):
+        self.namespace = namespace  # type: str
+        self.url = url  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BatchPutDcdnKvWithHighCapacityRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
+class BatchPutDcdnKvWithHighCapacityResponseBody(TeaModel):
+    def __init__(self, fail_keys=None, request_id=None, success_keys=None):
+        self.fail_keys = fail_keys  # type: list[str]
+        self.request_id = request_id  # type: str
+        self.success_keys = success_keys  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BatchPutDcdnKvWithHighCapacityResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: BatchPutDcdnKvWithHighCapacityResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(BatchPutDcdnKvWithHighCapacityResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, cert_name=None, cert_type=None, domain_name=None, owner_id=None, region=None, sslpri=None,
                  sslprotocol=None, sslpub=None, security_token=None):
         # The name of the certificate.
         self.cert_name = cert_name  # type: str
         # The type of the certificate. Valid values:
         # 
@@ -34468,14 +34788,118 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PutDcdnKvNamespaceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PutDcdnKvWithHighCapacityRequest(TeaModel):
+    def __init__(self, key=None, namespace=None, url=None):
+        self.key = key  # type: str
+        self.namespace = namespace  # type: str
+        self.url = url  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(PutDcdnKvWithHighCapacityRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, length=None, request_id=None, value=None):
+        self.length = length  # type: int
+        self.request_id = request_id  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(PutDcdnKvWithHighCapacityResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: PutDcdnKvWithHighCapacityResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(PutDcdnKvWithHighCapacityResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, force=None, object_path=None, object_type=None, owner_id=None, security_token=None):
         # Specifies whether to refresh resources in a directory if the resources are different from the resources in the same directory in the origin server. Default value: false.
         # 
         # *   **true**: refresh all resources in the directory.
         # *   **false**: refresh the changed resources in the directory.
         self.force = force  # type: bool
```

### Comparing `alibabacloud_dcdn20180115_py2-2.2.0/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO` & `alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dcdn20180115-py2
-Version: 2.2.0
+Version: 2.3.0
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115_py2-2.2.0/setup.py` & `alibabacloud_dcdn20180115_py2-2.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dcdn20180115_py2.
 
-Created on 21/03/2024
+Created on 08/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dcdn20180115"
 NAME = "alibabacloud_dcdn20180115_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dcdn (20180115) SDK Library for Python2"
```

