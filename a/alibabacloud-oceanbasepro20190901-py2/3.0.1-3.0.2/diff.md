# Comparing `tmp/alibabacloud_oceanbasepro20190901_py2-3.0.1.tar.gz` & `tmp/alibabacloud_oceanbasepro20190901_py2-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901_py2-3.0.1.tar", last modified: Mon Mar 25 12:41:36 2024, max compression
+gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901_py2-3.0.2.tar", last modified: Mon Apr  8 12:13:30 2024, max compression
```

## Comparing `alibabacloud_oceanbasepro20190901_py2-3.0.1.tar` & `alibabacloud_oceanbasepro20190901_py2-3.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:41:36.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/
--rw-r--r--   0 root         (0) root         (0)     2137 2024-03-25 12:41:35.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-25 12:41:35.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-25 12:41:35.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2526 2024-03-25 12:41:36.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1060 2024-03-25 12:41:35.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2024-03-25 12:41:35.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:41:36.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 12:41:35.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   173631 2024-03-25 12:41:35.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901/client.py
--rw-r--r--   0 root         (0) root         (0)  1664278 2024-03-25 12:41:35.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:41:36.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2526 2024-03-25 12:41:36.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2024-03-25 12:41:36.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 12:41:36.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-25 12:41:36.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-03-25 12:41:36.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 12:41:36.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2948 2024-03-25 12:41:35.000000 alibabacloud_oceanbasepro20190901_py2-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   174066 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901/client.py
+-rw-r--r--   0 root         (0) root         (0)  1682352 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2948 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901_py2-3.0.2/setup.py
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-3.0.1/ChangeLog.md` & `alibabacloud_oceanbasepro20190901_py2-3.0.2/ChangeLog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-03-25 Version: 3.0.1
+- Generated python2 2019-09-01 for OceanBasePro.
+
 2024-03-20 Version: 3.0.0
 - Delete API CreateOmsOpenAPIProject.
 - Delete API DeleteOmsOpenAPIProject.
 - Delete API DescribeOmsOpenAPIProject.
 - Delete API DescribeOmsOpenAPIProjectSteps.
 - Delete API ReleaseOmsOpenAPIProject.
 - Delete API ResetOmsOpenAPIProject.
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-3.0.1/LICENSE` & `alibabacloud_oceanbasepro20190901_py2-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-3.0.1/PKG-INFO` & `alibabacloud_oceanbasepro20190901_py2-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_oceanbasepro20190901_py2
-Version: 3.0.1
+Version: 3.0.2
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-3.0.1/README-CN.md` & `alibabacloud_oceanbasepro20190901_py2-3.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-3.0.1/README.md` & `alibabacloud_oceanbasepro20190901_py2-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901/client.py` & `alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,14 +398,16 @@
             request.common_transfer_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.common_transfer_config, 'CommonTransferConfig', 'json')
         if not UtilClient.is_unset(tmp_req.full_transfer_config):
             request.full_transfer_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.full_transfer_config, 'FullTransferConfig', 'json')
         if not UtilClient.is_unset(tmp_req.incr_transfer_config):
             request.incr_transfer_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.incr_transfer_config, 'IncrTransferConfig', 'json')
         if not UtilClient.is_unset(tmp_req.label_ids):
             request.label_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.label_ids, 'LabelIds', 'json')
+        if not UtilClient.is_unset(tmp_req.reverse_incr_transfer_config):
+            request.reverse_incr_transfer_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.reverse_incr_transfer_config, 'ReverseIncrTransferConfig', 'json')
         if not UtilClient.is_unset(tmp_req.struct_transfer_config):
             request.struct_transfer_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.struct_transfer_config, 'StructTransferConfig', 'json')
         if not UtilClient.is_unset(tmp_req.transfer_mapping):
             request.transfer_mapping_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.transfer_mapping, 'TransferMapping', 'json')
         body = {}
         if not UtilClient.is_unset(request.common_transfer_config_shrink):
             body['CommonTransferConfig'] = request.common_transfer_config_shrink
@@ -427,14 +429,16 @@
             body['IncrTransferConfig'] = request.incr_transfer_config_shrink
         if not UtilClient.is_unset(request.label_ids_shrink):
             body['LabelIds'] = request.label_ids_shrink
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.oss_key):
             body['OssKey'] = request.oss_key
+        if not UtilClient.is_unset(request.reverse_incr_transfer_config_shrink):
+            body['ReverseIncrTransferConfig'] = request.reverse_incr_transfer_config_shrink
         if not UtilClient.is_unset(request.sink_endpoint_id):
             body['SinkEndpointId'] = request.sink_endpoint_id
         if not UtilClient.is_unset(request.source_endpoint_id):
             body['SourceEndpointId'] = request.source_endpoint_id
         if not UtilClient.is_unset(request.struct_transfer_config_shrink):
             body['StructTransferConfig'] = request.struct_transfer_config_shrink
         if not UtilClient.is_unset(request.transfer_mapping_shrink):
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901/models.py` & `alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2155,19 +2155,24 @@
         if m.get('TableCategory') is not None:
             self.table_category = m.get('TableCategory')
         return self
 
 
 class CreateProjectRequestFullTransferConfig(TeaModel):
     def __init__(self, allow_dest_table_not_empty=None, full_transfer_speed_mode=None,
-                 full_verify_speed_mode=None, none_pk_uk_truncate_dst_table=None):
+                 full_verify_speed_mode=None, none_pk_uk_truncate_dst_table=None, read_worker_num=None, throttle_iops=None,
+                 throttle_rps=None, write_worker_num=None):
         self.allow_dest_table_not_empty = allow_dest_table_not_empty  # type: bool
         self.full_transfer_speed_mode = full_transfer_speed_mode  # type: str
         self.full_verify_speed_mode = full_verify_speed_mode  # type: str
         self.none_pk_uk_truncate_dst_table = none_pk_uk_truncate_dst_table  # type: bool
+        self.read_worker_num = read_worker_num  # type: int
+        self.throttle_iops = throttle_iops  # type: int
+        self.throttle_rps = throttle_rps  # type: int
+        self.write_worker_num = write_worker_num  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateProjectRequestFullTransferConfig, self).to_map()
         if _map is not None:
@@ -2178,38 +2183,58 @@
             result['AllowDestTableNotEmpty'] = self.allow_dest_table_not_empty
         if self.full_transfer_speed_mode is not None:
             result['FullTransferSpeedMode'] = self.full_transfer_speed_mode
         if self.full_verify_speed_mode is not None:
             result['FullVerifySpeedMode'] = self.full_verify_speed_mode
         if self.none_pk_uk_truncate_dst_table is not None:
             result['NonePkUkTruncateDstTable'] = self.none_pk_uk_truncate_dst_table
+        if self.read_worker_num is not None:
+            result['ReadWorkerNum'] = self.read_worker_num
+        if self.throttle_iops is not None:
+            result['ThrottleIOPS'] = self.throttle_iops
+        if self.throttle_rps is not None:
+            result['ThrottleRps'] = self.throttle_rps
+        if self.write_worker_num is not None:
+            result['WriteWorkerNum'] = self.write_worker_num
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AllowDestTableNotEmpty') is not None:
             self.allow_dest_table_not_empty = m.get('AllowDestTableNotEmpty')
         if m.get('FullTransferSpeedMode') is not None:
             self.full_transfer_speed_mode = m.get('FullTransferSpeedMode')
         if m.get('FullVerifySpeedMode') is not None:
             self.full_verify_speed_mode = m.get('FullVerifySpeedMode')
         if m.get('NonePkUkTruncateDstTable') is not None:
             self.none_pk_uk_truncate_dst_table = m.get('NonePkUkTruncateDstTable')
+        if m.get('ReadWorkerNum') is not None:
+            self.read_worker_num = m.get('ReadWorkerNum')
+        if m.get('ThrottleIOPS') is not None:
+            self.throttle_iops = m.get('ThrottleIOPS')
+        if m.get('ThrottleRps') is not None:
+            self.throttle_rps = m.get('ThrottleRps')
+        if m.get('WriteWorkerNum') is not None:
+            self.write_worker_num = m.get('WriteWorkerNum')
         return self
 
 
 class CreateProjectRequestIncrTransferConfig(TeaModel):
     def __init__(self, enable_incr_sync_statistics=None, enable_sequencing_within_txn=None,
-                 incr_sync_concurrency=None, record_type_white_list=None, start_timestamp=None, store_log_kept_hour=None):
+                 incr_sync_concurrency=None, record_type_white_list=None, start_timestamp=None, store_log_kept_hour=None,
+                 support_ddltypes=None, throttle_iops=None, throttle_rps=None):
         self.enable_incr_sync_statistics = enable_incr_sync_statistics  # type: bool
         self.enable_sequencing_within_txn = enable_sequencing_within_txn  # type: bool
         self.incr_sync_concurrency = incr_sync_concurrency  # type: int
         self.record_type_white_list = record_type_white_list  # type: list[str]
         self.start_timestamp = start_timestamp  # type: str
         self.store_log_kept_hour = store_log_kept_hour  # type: int
+        self.support_ddltypes = support_ddltypes  # type: list[str]
+        self.throttle_iops = throttle_iops  # type: int
+        self.throttle_rps = throttle_rps  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateProjectRequestIncrTransferConfig, self).to_map()
         if _map is not None:
@@ -2224,14 +2249,20 @@
             result['IncrSyncConcurrency'] = self.incr_sync_concurrency
         if self.record_type_white_list is not None:
             result['RecordTypeWhiteList'] = self.record_type_white_list
         if self.start_timestamp is not None:
             result['StartTimestamp'] = self.start_timestamp
         if self.store_log_kept_hour is not None:
             result['StoreLogKeptHour'] = self.store_log_kept_hour
+        if self.support_ddltypes is not None:
+            result['SupportDDLTypes'] = self.support_ddltypes
+        if self.throttle_iops is not None:
+            result['ThrottleIOPS'] = self.throttle_iops
+        if self.throttle_rps is not None:
+            result['ThrottleRps'] = self.throttle_rps
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('EnableIncrSyncStatistics') is not None:
             self.enable_incr_sync_statistics = m.get('EnableIncrSyncStatistics')
         if m.get('EnableSequencingWithinTxn') is not None:
@@ -2240,14 +2271,86 @@
             self.incr_sync_concurrency = m.get('IncrSyncConcurrency')
         if m.get('RecordTypeWhiteList') is not None:
             self.record_type_white_list = m.get('RecordTypeWhiteList')
         if m.get('StartTimestamp') is not None:
             self.start_timestamp = m.get('StartTimestamp')
         if m.get('StoreLogKeptHour') is not None:
             self.store_log_kept_hour = m.get('StoreLogKeptHour')
+        if m.get('SupportDDLTypes') is not None:
+            self.support_ddltypes = m.get('SupportDDLTypes')
+        if m.get('ThrottleIOPS') is not None:
+            self.throttle_iops = m.get('ThrottleIOPS')
+        if m.get('ThrottleRps') is not None:
+            self.throttle_rps = m.get('ThrottleRps')
+        return self
+
+
+class CreateProjectRequestReverseIncrTransferConfig(TeaModel):
+    def __init__(self, enable_incr_sync_statistics=None, enable_sequencing_within_txn=None,
+                 incr_sync_concurrency=None, record_type_white_list=None, start_timestamp=None, store_log_kept_hour=None,
+                 support_ddltypes=None, throttle_iops=None, throttle_rps=None):
+        self.enable_incr_sync_statistics = enable_incr_sync_statistics  # type: bool
+        self.enable_sequencing_within_txn = enable_sequencing_within_txn  # type: bool
+        self.incr_sync_concurrency = incr_sync_concurrency  # type: int
+        self.record_type_white_list = record_type_white_list  # type: list[str]
+        self.start_timestamp = start_timestamp  # type: str
+        self.store_log_kept_hour = store_log_kept_hour  # type: int
+        self.support_ddltypes = support_ddltypes  # type: list[str]
+        self.throttle_iops = throttle_iops  # type: int
+        self.throttle_rps = throttle_rps  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateProjectRequestReverseIncrTransferConfig, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enable_incr_sync_statistics is not None:
+            result['EnableIncrSyncStatistics'] = self.enable_incr_sync_statistics
+        if self.enable_sequencing_within_txn is not None:
+            result['EnableSequencingWithinTxn'] = self.enable_sequencing_within_txn
+        if self.incr_sync_concurrency is not None:
+            result['IncrSyncConcurrency'] = self.incr_sync_concurrency
+        if self.record_type_white_list is not None:
+            result['RecordTypeWhiteList'] = self.record_type_white_list
+        if self.start_timestamp is not None:
+            result['StartTimestamp'] = self.start_timestamp
+        if self.store_log_kept_hour is not None:
+            result['StoreLogKeptHour'] = self.store_log_kept_hour
+        if self.support_ddltypes is not None:
+            result['SupportDDLTypes'] = self.support_ddltypes
+        if self.throttle_iops is not None:
+            result['ThrottleIOPS'] = self.throttle_iops
+        if self.throttle_rps is not None:
+            result['ThrottleRps'] = self.throttle_rps
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('EnableIncrSyncStatistics') is not None:
+            self.enable_incr_sync_statistics = m.get('EnableIncrSyncStatistics')
+        if m.get('EnableSequencingWithinTxn') is not None:
+            self.enable_sequencing_within_txn = m.get('EnableSequencingWithinTxn')
+        if m.get('IncrSyncConcurrency') is not None:
+            self.incr_sync_concurrency = m.get('IncrSyncConcurrency')
+        if m.get('RecordTypeWhiteList') is not None:
+            self.record_type_white_list = m.get('RecordTypeWhiteList')
+        if m.get('StartTimestamp') is not None:
+            self.start_timestamp = m.get('StartTimestamp')
+        if m.get('StoreLogKeptHour') is not None:
+            self.store_log_kept_hour = m.get('StoreLogKeptHour')
+        if m.get('SupportDDLTypes') is not None:
+            self.support_ddltypes = m.get('SupportDDLTypes')
+        if m.get('ThrottleIOPS') is not None:
+            self.throttle_iops = m.get('ThrottleIOPS')
+        if m.get('ThrottleRps') is not None:
+            self.throttle_rps = m.get('ThrottleRps')
         return self
 
 
 class CreateProjectRequestStructTransferConfig(TeaModel):
     def __init__(self, byte_char_convert_strategy=None, defer_index_creation=None):
         self.byte_char_convert_strategy = byte_char_convert_strategy  # type: str
         self.defer_index_creation = defer_index_creation  # type: bool
@@ -3313,29 +3416,30 @@
             self.table_and_view_white_list = m.get('TableAndViewWhiteList')
         return self
 
 
 class CreateProjectRequest(TeaModel):
     def __init__(self, common_transfer_config=None, enable_full_transfer=None, enable_full_verify=None,
                  enable_incr_transfer=None, enable_reverse_incr_transfer=None, enable_struct_transfer=None, full_transfer_config=None,
-                 id=None, incr_transfer_config=None, label_ids=None, name=None, oss_key=None, sink_endpoint_id=None,
-                 source_endpoint_id=None, struct_transfer_config=None, transfer_mapping=None, type=None, use_oss=None,
-                 worker_grade_id=None):
+                 id=None, incr_transfer_config=None, label_ids=None, name=None, oss_key=None,
+                 reverse_incr_transfer_config=None, sink_endpoint_id=None, source_endpoint_id=None, struct_transfer_config=None,
+                 transfer_mapping=None, type=None, use_oss=None, worker_grade_id=None):
         self.common_transfer_config = common_transfer_config  # type: CreateProjectRequestCommonTransferConfig
         self.enable_full_transfer = enable_full_transfer  # type: bool
         self.enable_full_verify = enable_full_verify  # type: bool
         self.enable_incr_transfer = enable_incr_transfer  # type: bool
         self.enable_reverse_incr_transfer = enable_reverse_incr_transfer  # type: bool
         self.enable_struct_transfer = enable_struct_transfer  # type: bool
         self.full_transfer_config = full_transfer_config  # type: CreateProjectRequestFullTransferConfig
         self.id = id  # type: str
         self.incr_transfer_config = incr_transfer_config  # type: CreateProjectRequestIncrTransferConfig
         self.label_ids = label_ids  # type: list[str]
         self.name = name  # type: str
         self.oss_key = oss_key  # type: str
+        self.reverse_incr_transfer_config = reverse_incr_transfer_config  # type: CreateProjectRequestReverseIncrTransferConfig
         self.sink_endpoint_id = sink_endpoint_id  # type: str
         self.source_endpoint_id = source_endpoint_id  # type: str
         self.struct_transfer_config = struct_transfer_config  # type: CreateProjectRequestStructTransferConfig
         self.transfer_mapping = transfer_mapping  # type: CreateProjectRequestTransferMapping
         self.type = type  # type: str
         self.use_oss = use_oss  # type: bool
         self.worker_grade_id = worker_grade_id  # type: str
@@ -3343,14 +3447,16 @@
     def validate(self):
         if self.common_transfer_config:
             self.common_transfer_config.validate()
         if self.full_transfer_config:
             self.full_transfer_config.validate()
         if self.incr_transfer_config:
             self.incr_transfer_config.validate()
+        if self.reverse_incr_transfer_config:
+            self.reverse_incr_transfer_config.validate()
         if self.struct_transfer_config:
             self.struct_transfer_config.validate()
         if self.transfer_mapping:
             self.transfer_mapping.validate()
 
     def to_map(self):
         _map = super(CreateProjectRequest, self).to_map()
@@ -3378,14 +3484,16 @@
             result['IncrTransferConfig'] = self.incr_transfer_config.to_map()
         if self.label_ids is not None:
             result['LabelIds'] = self.label_ids
         if self.name is not None:
             result['Name'] = self.name
         if self.oss_key is not None:
             result['OssKey'] = self.oss_key
+        if self.reverse_incr_transfer_config is not None:
+            result['ReverseIncrTransferConfig'] = self.reverse_incr_transfer_config.to_map()
         if self.sink_endpoint_id is not None:
             result['SinkEndpointId'] = self.sink_endpoint_id
         if self.source_endpoint_id is not None:
             result['SourceEndpointId'] = self.source_endpoint_id
         if self.struct_transfer_config is not None:
             result['StructTransferConfig'] = self.struct_transfer_config.to_map()
         if self.transfer_mapping is not None:
@@ -3423,14 +3531,17 @@
             self.incr_transfer_config = temp_model.from_map(m['IncrTransferConfig'])
         if m.get('LabelIds') is not None:
             self.label_ids = m.get('LabelIds')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('OssKey') is not None:
             self.oss_key = m.get('OssKey')
+        if m.get('ReverseIncrTransferConfig') is not None:
+            temp_model = CreateProjectRequestReverseIncrTransferConfig()
+            self.reverse_incr_transfer_config = temp_model.from_map(m['ReverseIncrTransferConfig'])
         if m.get('SinkEndpointId') is not None:
             self.sink_endpoint_id = m.get('SinkEndpointId')
         if m.get('SourceEndpointId') is not None:
             self.source_endpoint_id = m.get('SourceEndpointId')
         if m.get('StructTransferConfig') is not None:
             temp_model = CreateProjectRequestStructTransferConfig()
             self.struct_transfer_config = temp_model.from_map(m['StructTransferConfig'])
@@ -3446,28 +3557,29 @@
         return self
 
 
 class CreateProjectShrinkRequest(TeaModel):
     def __init__(self, common_transfer_config_shrink=None, enable_full_transfer=None, enable_full_verify=None,
                  enable_incr_transfer=None, enable_reverse_incr_transfer=None, enable_struct_transfer=None,
                  full_transfer_config_shrink=None, id=None, incr_transfer_config_shrink=None, label_ids_shrink=None, name=None, oss_key=None,
-                 sink_endpoint_id=None, source_endpoint_id=None, struct_transfer_config_shrink=None, transfer_mapping_shrink=None,
-                 type=None, use_oss=None, worker_grade_id=None):
+                 reverse_incr_transfer_config_shrink=None, sink_endpoint_id=None, source_endpoint_id=None, struct_transfer_config_shrink=None,
+                 transfer_mapping_shrink=None, type=None, use_oss=None, worker_grade_id=None):
         self.common_transfer_config_shrink = common_transfer_config_shrink  # type: str
         self.enable_full_transfer = enable_full_transfer  # type: bool
         self.enable_full_verify = enable_full_verify  # type: bool
         self.enable_incr_transfer = enable_incr_transfer  # type: bool
         self.enable_reverse_incr_transfer = enable_reverse_incr_transfer  # type: bool
         self.enable_struct_transfer = enable_struct_transfer  # type: bool
         self.full_transfer_config_shrink = full_transfer_config_shrink  # type: str
         self.id = id  # type: str
         self.incr_transfer_config_shrink = incr_transfer_config_shrink  # type: str
         self.label_ids_shrink = label_ids_shrink  # type: str
         self.name = name  # type: str
         self.oss_key = oss_key  # type: str
+        self.reverse_incr_transfer_config_shrink = reverse_incr_transfer_config_shrink  # type: str
         self.sink_endpoint_id = sink_endpoint_id  # type: str
         self.source_endpoint_id = source_endpoint_id  # type: str
         self.struct_transfer_config_shrink = struct_transfer_config_shrink  # type: str
         self.transfer_mapping_shrink = transfer_mapping_shrink  # type: str
         self.type = type  # type: str
         self.use_oss = use_oss  # type: bool
         self.worker_grade_id = worker_grade_id  # type: str
@@ -3501,14 +3613,16 @@
             result['IncrTransferConfig'] = self.incr_transfer_config_shrink
         if self.label_ids_shrink is not None:
             result['LabelIds'] = self.label_ids_shrink
         if self.name is not None:
             result['Name'] = self.name
         if self.oss_key is not None:
             result['OssKey'] = self.oss_key
+        if self.reverse_incr_transfer_config_shrink is not None:
+            result['ReverseIncrTransferConfig'] = self.reverse_incr_transfer_config_shrink
         if self.sink_endpoint_id is not None:
             result['SinkEndpointId'] = self.sink_endpoint_id
         if self.source_endpoint_id is not None:
             result['SourceEndpointId'] = self.source_endpoint_id
         if self.struct_transfer_config_shrink is not None:
             result['StructTransferConfig'] = self.struct_transfer_config_shrink
         if self.transfer_mapping_shrink is not None:
@@ -3543,14 +3657,16 @@
             self.incr_transfer_config_shrink = m.get('IncrTransferConfig')
         if m.get('LabelIds') is not None:
             self.label_ids_shrink = m.get('LabelIds')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('OssKey') is not None:
             self.oss_key = m.get('OssKey')
+        if m.get('ReverseIncrTransferConfig') is not None:
+            self.reverse_incr_transfer_config_shrink = m.get('ReverseIncrTransferConfig')
         if m.get('SinkEndpointId') is not None:
             self.sink_endpoint_id = m.get('SinkEndpointId')
         if m.get('SourceEndpointId') is not None:
             self.source_endpoint_id = m.get('SourceEndpointId')
         if m.get('StructTransferConfig') is not None:
             self.struct_transfer_config_shrink = m.get('StructTransferConfig')
         if m.get('TransferMapping') is not None:
@@ -11623,25 +11739,29 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstancesRequest(TeaModel):
     def __init__(self, instance_id=None, instance_name=None, page_number=None, page_size=None,
                  resource_group_id=None, search_key=None):
-        # The number of CPU cores used in the cluster.
+        # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
-        # The size of used memory in the cluster, in GB.
+        # The name of the OceanBase cluster. It must be 1 to 20 characters in length. If this parameter is not specified, the value is the instance ID of the cluster by default.
         self.instance_name = instance_name  # type: str
-        # The total memory size of the cluster, in GB.
+        # The number of the page to return.
+        # - Pages start from page 1.
+        # - Default value: 1.
         self.page_number = page_number  # type: int
-        # The information about the memory resources of the cluster.
+        # The number of rows to return on each page.
+        # - Maximum value: 100.
+        # - Default value: 10.
         self.page_size = page_size  # type: int
-        # The number of CPU cores of each replica node in the cluster.
+        # The ID of the resource group. If you do not specify this parameter, all resources are returned.
         self.resource_group_id = resource_group_id  # type: str
-        # The memory size of each replica node in the cluster, in GB.
+        # The keyword for fuzzy search, which can be an instance ID, instance name, tenant ID, or tenant name.
         self.search_key = search_key  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstancesRequest, self).to_map()
@@ -11679,21 +11799,29 @@
             self.search_key = m.get('SearchKey')
         return self
 
 
 class DescribeInstancesResponseBodyInstancesDataDiskAutoScaleConfig(TeaModel):
     def __init__(self, auto_scale=None, max_disk_size=None, scale_step_in_merge=None, scale_step_in_normal=None,
                  upper_merge_threshold=None, upper_scale_strategy=None, upper_threshold=None, upperbound=None):
+        # Specifies whether to enable the automatic scaling of the data disk.
         self.auto_scale = auto_scale  # type: bool
+        # The maximum size of the disk, in GB.
         self.max_disk_size = max_disk_size  # type: long
+        # The size of scaling step during a major compaction.
         self.scale_step_in_merge = scale_step_in_merge  # type: long
+        # The size of scaling step during daily use.
         self.scale_step_in_normal = scale_step_in_normal  # type: long
+        # The maximum usage of the data disk, in percentage, that triggers the scaling of the data disk for major compactions.
         self.upper_merge_threshold = upper_merge_threshold  # type: long
+        # The scale-out strategy. Valid values: RAW and PERCENTAGE.
         self.upper_scale_strategy = upper_scale_strategy  # type: str
+        # The maximum usage of the data disk, in percentage, that triggers the scaling of the data disk for daily use.
         self.upper_threshold = upper_threshold  # type: long
+        # The maximum space, in GB, to which the data disk can be scaled.
         self.upperbound = upperbound  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstancesResponseBodyInstancesDataDiskAutoScaleConfig, self).to_map()
@@ -11738,16 +11866,19 @@
         if m.get('Upperbound') is not None:
             self.upperbound = m.get('Upperbound')
         return self
 
 
 class DescribeInstancesResponseBodyInstancesResourceCapacityUnit(TeaModel):
     def __init__(self, max_capacity_unit=None, min_capacity_unit=None, used_capacity_unit=None):
+        # The maximum number of capacity units.
         self.max_capacity_unit = max_capacity_unit  # type: int
+        # The minimum number of capacity units.
         self.min_capacity_unit = min_capacity_unit  # type: int
+        # The number of used capacity units.
         self.used_capacity_unit = used_capacity_unit  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstancesResponseBodyInstancesResourceCapacityUnit, self).to_map()
@@ -11772,26 +11903,21 @@
         if m.get('UsedCapacityUnit') is not None:
             self.used_capacity_unit = m.get('UsedCapacityUnit')
         return self
 
 
 class DescribeInstancesResponseBodyInstancesResourceCpu(TeaModel):
     def __init__(self, original_total_cpu=None, total_cpu=None, unit_cpu=None, used_cpu=None):
+        # The number of original CPU cores in the cluster.
         self.original_total_cpu = original_total_cpu  # type: long
-        # The name of the OceanBase cluster.    
-        # It must be 1 to 20 characters in length.   
-        # If this parameter is not specified, the value is the instance ID of the cluster by default.
+        # The total number of CPU cores of the cluster.
         self.total_cpu = total_cpu  # type: long
-        # The data replica distribution mode of the cluster. Valid values:    
-        # 
-        # - n: indicates the single-IDC mode.  
-        # - n-n: indicates the dual-IDC mode.  
-        # - n-n-n: indicates the multi-IDC mode. The integer n represents the number of OBServer nodes in each IDC.
+        # The number of CPU cores of each replica node in the cluster.
         self.unit_cpu = unit_cpu  # type: long
-        # The search keyword.
+        # The number of CPU cores used in the cluster.
         self.used_cpu = used_cpu  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstancesResponseBodyInstancesResourceCpu, self).to_map()
@@ -11821,20 +11947,21 @@
             self.used_cpu = m.get('UsedCpu')
         return self
 
 
 class DescribeInstancesResponseBodyInstancesResourceDiskSize(TeaModel):
     def __init__(self, original_total_disk_size=None, total_disk_size=None, unit_disk_size=None,
                  used_disk_size=None):
+        # The original size of the disk.
         self.original_total_disk_size = original_total_disk_size  # type: long
-        # The request ID.
+        # The total storage space of the cluster, in GB.
         self.total_disk_size = total_disk_size  # type: long
-        # Example 1
+        # The storage space of each replica node in the cluster, in GB.
         self.unit_disk_size = unit_disk_size  # type: long
-        # $.parameters[7].schema.example
+        # The size of used storage space of the cluster, in GB.
         self.used_disk_size = used_disk_size  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstancesResponseBodyInstancesResourceDiskSize, self).to_map()
@@ -11863,18 +11990,19 @@
         if m.get('UsedDiskSize') is not None:
             self.used_disk_size = m.get('UsedDiskSize')
         return self
 
 
 class DescribeInstancesResponseBodyInstancesResourceMemory(TeaModel):
     def __init__(self, original_total_memory=None, total_memory=None, unit_memory=None, used_memory=None):
+        # The original memory size of the cluster, in GB.
         self.original_total_memory = original_total_memory  # type: long
-        # The number of CPU cores of the cluster.
+        # The total memory size of the cluster, in GB.
         self.total_memory = total_memory  # type: long
-        # The size of used storage space of the cluster, in GB.
+        # The memory size of each replica node in the cluster, in GB.
         self.unit_memory = unit_memory  # type: long
         # The size of used memory in the cluster, in GB.
         self.used_memory = used_memory  # type: long
 
     def validate(self):
         pass
 
@@ -11905,36 +12033,23 @@
         if m.get('UsedMemory') is not None:
             self.used_memory = m.get('UsedMemory')
         return self
 
 
 class DescribeInstancesResponseBodyInstancesResource(TeaModel):
     def __init__(self, capacity_unit=None, cpu=None, disk_size=None, memory=None, unit_count=None):
+        # The information about capacity units.
         self.capacity_unit = capacity_unit  # type: DescribeInstancesResponseBodyInstancesResourceCapacityUnit
-        # Indicates whether new nodes can be added.
+        # The information about the CPU resources of the cluster.
         self.cpu = cpu  # type: DescribeInstancesResponseBodyInstancesResourceCpu
-        # The time elapsed since the expiration of the cluster, in seconds.
+        # The information about the storage resources of the cluster.
         self.disk_size = disk_size  # type: DescribeInstancesResponseBodyInstancesResourceDiskSize
-        # The status of the cluster. Valid values:   
-        # - PENDING_CREATE: The cluster is being created.  
-        # - ONLINE: The cluster is running.  
-        # - TENANT_CREATING: The tenant is being created.  
-        # - TENANT_SPEC_MODIFYING: The tenant specifications are being modified.  
-        # - EXPANDING: Nodes are being added to the cluster to increase its capacity.  
-        # - REDUCING: Nodes are being removed from the cluster to reduce its capacity.  
-        # - SPEC_UPGRADING: The service plan is being upgraded.  
-        # - DISK_UPGRADING: The storage space is being expanded.  
-        # - WHITE_LIST_MODIFYING: The whitelist is being modified.  
-        # - PARAMETER_MODIFYING: Parameters are being modified.  
-        # - SSL_MODIFYING: The SSL certificate is being changed.  
-        # - PREPAID_EXPIRE_CLOSED: The payment is overdue. This parameter is valid for a cluster whose billing method is set to PREPAY.  
-        # - ARREARS_CLOSED: The payment is overdue. This parameter is valid for a cluster whose billing method is set to POSTPAY.  
-        # - PENDING_DELETE: The cluster is being deleted.   
-        # Generally, the cluster is in the ONLINE state.
+        # The information about the memory resources of the cluster.
         self.memory = memory  # type: DescribeInstancesResponseBodyInstancesResourceMemory
+        # The number of resource units in the cluster.
         self.unit_count = unit_count  # type: long
 
     def validate(self):
         if self.capacity_unit:
             self.capacity_unit.validate()
         if self.cpu:
             self.cpu.validate()
@@ -11983,72 +12098,134 @@
 class DescribeInstancesResponseBodyInstances(TeaModel):
     def __init__(self, available_zones=None, commodity_code=None, cpu=None, cpu_architecture=None, create_time=None,
                  data_disk_auto_scale_config=None, deploy_mode=None, deploy_type=None, disk_size=None, disk_type=None,
                  enable_read_only_replica_management=None, enable_upgrade_nodes=None, expire_seconds=None, expire_time=None,
                  in_temp_capacity_status=None, instance_class=None, instance_id=None, instance_name=None, instance_role=None,
                  instance_type=None, maintain_time=None, mem=None, pay_type=None, resource=None, resource_group_id=None,
                  series=None, state=None, used_disk_size=None, version=None, vpc_id=None):
-        # The time in UTC when the cluster expires.
+        # The information about the zone in which the cluster is deployed.
         self.available_zones = available_zones  # type: list[str]
-        # The storage space of each replica node in the cluster, in GB.
-        self.commodity_code = commodity_code  # type: str
         # The product code of the OceanBase cluster.   
         # - oceanbase_oceanbasepre_public_cn: indicates an OceanBase cluster that is billed based on the subscription plan and that is deployed in a China site.  
         # - oceanbase_oceanbasepost_public_cn: indicates an OceanBase cluster that is billed based on the pay-as-you-go plan and that is deployed in a China site.  
         # - oceanbase_obpre_public_intl: indicates an OceanBase cluster that is billed based on the subscription plan and that is deployed in an international site.
+        self.commodity_code = commodity_code  # type: str
+        # The number of CPU cores of the cluster.
         self.cpu = cpu  # type: int
+        # The CPU architecture of the cluster.
         self.cpu_architecture = cpu_architecture  # type: str
-        # The number of OceanBase clusters queried.
+        # The time in UTC when the cluster was created.
         self.create_time = create_time  # type: str
+        # Specifies parameters for the automatic scaling of the data disk.
         self.data_disk_auto_scale_config = data_disk_auto_scale_config  # type: DescribeInstancesResponseBodyInstancesDataDiskAutoScaleConfig
-        # The request ID.
+        # The data replica distribution mode of the cluster. The value is in the n-n-n format, where n is the number of OBServer nodes in each IDC.
         self.deploy_mode = deploy_mode  # type: str
-        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
+        # The deployment type of the cluster. Valid values:   
+        # - multiple: multi-IDC deployment  
+        # - single: single-IDC deployment  
+        # - dual: dual-IDC deployment
         self.deploy_type = deploy_type  # type: str
-        # The information about the memory resources of the cluster.
+        # The size of the storage space, in GB.
         self.disk_size = disk_size  # type: str
-        # The number of CPU cores used in the cluster.
+        # The type of the storage disk where the cluster is deployed.   
+        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
         self.disk_type = disk_type  # type: str
+        # Indicates whether the cluster supports read-only replicas.
         self.enable_read_only_replica_management = enable_read_only_replica_management  # type: bool
-        # The ID of the OceanBase cluster.
+        # Indicates whether new nodes can be added.
         self.enable_upgrade_nodes = enable_upgrade_nodes  # type: bool
-        # The whitelist information of the cluster.
+        # The time elapsed since the expiration of the cluster, in seconds. 
+        # > In subscription mode, if the cluster has not expired, this parameter indicates the remaining validity period of the cluster. If the cluster has expired, this parameter indicates the time elapsed since the expiration.
         self.expire_seconds = expire_seconds  # type: int
-        # The information about the storage resources of the cluster.
+        # The time in UTC when the cluster expires. 
+        # > This parameter is valid only for subscription instances.
         self.expire_time = expire_time  # type: str
+        # Specifies whether to indicate the temporary status of the capacity.
         self.in_temp_capacity_status = in_temp_capacity_status  # type: bool
-        # The instance type.
+        # The specifications of the cluster.  You can specify one of the following four plans:  
+        # - 8C32G: indicates 8 CPU cores and 32 GB of memory.  
+        # - 14C70G: indicates 14 CPU cores and 70 GB of memory.  
+        # - 30C180G: indicates 30 CPU cores and 180 GB of memory.  
+        # - 62C400G: indicates 62 CPU cores and 400 GB of memory.
         self.instance_class = instance_class  # type: str
-        # The total storage space of the cluster, in GB.
+        # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
-        # The return result of the request.
+        # The name of the OceanBase cluster.
         self.instance_name = instance_name  # type: str
+        # The role of the instance.
         self.instance_role = instance_role  # type: str
-        # You can call this operation to obtain the list of OceanBase clusters.
+        # The instance type.
+        # - cluster: indicates a cluster instance.
+        # - mtenant: indicates a tenant instance in MySQL mode.
+        # - mtenant_serverless: indicates a serverless instance in MySQL mode.
         self.instance_type = instance_type  # type: str
-        # The return result of the request.
+        # The time period in UTC for the daily routine maintenance of the cluster.
         self.maintain_time = maintain_time  # type: str
-        # The information about the CPU resources of the cluster.
+        # The memory size of the instance, in GB.
         self.mem = mem  # type: long
-        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
-        self.pay_type = pay_type  # type: str
-        # The type of the storage disk where the cluster is deployed.   
-        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
-        self.resource = resource  # type: DescribeInstancesResponseBodyInstancesResource
-        # The number of OceanBase clusters queried.
-        self.resource_group_id = resource_group_id  # type: str
         # The billing method for the OceanBase cluster. Valid values:  
         # - PREPAY: the subscription billing method.  
         # - POSTPAY: the pay-as-you-go billing method.
+        self.pay_type = pay_type  # type: str
+        # The information about cluster resources.
+        self.resource = resource  # type: DescribeInstancesResponseBodyInstancesResource
+        # The ID of the resource group.
+        self.resource_group_id = resource_group_id  # type: str
+        # The series of the OceanBase cluster. Valid values:   
+        # - NORMAL: the high availability edition.   
+        # - BASIC: the basic edition.
         self.series = series  # type: str
-        # The number of resource units in the cluster.
+        # The status of the cluster. Valid values:   
+        # - ONLINE: The cluster is running.  
+        # - PENDING_CREATE: The cluster is being created.  
+        # - ARREARS_CLOSED("arrears_closed"): The cluster is suspended due to insufficient balance.
+        # - PREPAID_EXPIRE_CLOSED("prepaid_expire_closed"): The cluster is suspended because the subscription has expired.
+        # - WHITE_LIST_MODIFYING("white_list_modifying"): The allowlist of the cluster is being modified.
+        # - SSL_MODIFYING("ssl_modifying"): The Secure Sockets Layer (SSL) settings of the cluster are being modified.
+        # - PARAMETER_MODIFYING("parameter_modifying"): Parameters of the cluster are being modified.
+        # - TENANT_CREATING("tenant_creating"): A tenant is being created in the cluster.
+        # - TENANT_SPEC_MODIFYING("tenant_spec_modifying"): The specifications of a tenant in the cluster are being modified.
+        # - EXPANDING("expanding"): Nodes are being added to the cluster.
+        # - REDUCING("reducing"): Nodes are being removed from the cluster.
+        # - ZONE_CHANGING("zone_changing"): Zones of the cluster are being modified.
+        # - SPEC_UPGRADING: The service plan is being upgraded.
+        # - SPEC_DOWNGRADING("spec_downgrading"): The plan specification is being downgraded.
+        # - DISK_UPGRADING: The storage space is being expanded.
+        # - UPGRADING("upgrading"): The version of the cluster is being upgraded.
+        # - PENDING_DELETE("pending_delete"): The cluster is being deleted.
+        # - DELETED("deleted"): The cluster has been deleted.
+        # - ABNORMAL("abnormal"): The cluster is abnormal.
+        # - OFFLINE("offline"): The cluster is offline.
+        # - STANDBY_CREATING("standby_creating"): A standby cluster is being created for the cluster.
+        # - STANDBY_DELETING("standby_deleting"): A standby cluster of the cluster is being deleted.
+        # - SWITCHOVER_SWITCHING("switchover_switching"): The cluster is undergoing a primary/standby switchover.
+        # - STANDBY_DISCONNECTING("standby_disconnecting"): The cluster is being decoupled from its standby cluster.
+        # - LOG_DISK_UPGRADING("log_disk_upgrading"): The log disk of the cluster is being scaled out.
+        # - ISOLATION_OPTIMIZATION_MODIFYING("isolation_optimization_modifying"): The isolation optimization settings of the cluster are being modified.
+        # - DISKTYPE_MODIFYING("disktype_modifying"): The data disk type of the cluster is being modified.
+        # - PROXY_SERVICE_CREATING("proxy_service_creating"): The proxy service is being enabled for the cluster.
+        # - PROXY_SERVICE_DELETING("proxy_service_deleting"): The proxy service is being disabled for the cluster.
+        # - PROXY_SERVICE_SPEC_MODIFYING("proxy_service_spec_modifying"): The proxy service specification is being modified for the cluster.
+        # - READONLY_ADD_NODE("readonly_add_node"): A read-only node is being added to the cluster.
+        # - READONLY_REDUCE_NODE("readonly_reduce_node"): A read-only node is being removed from the cluster.
+        # - READONLY_REDUCE_ZONE("readonly_reduce_zone"): A read-only zone is being removed from the cluster.
+        # - READONLY_ADD_ZONE("readonly_add_zone"): A read-only zone is being added to the cluster.
+        # - READONLY_UPGRADE_SPEC("readonly_upgrade_spec"): The specification of read-only replicas is being upgraded.
+        # - READONLY_UPGRADE_DISK("readonly_upgrade_disk"): The disk space of read-only replicas is being scaled out.
+        # - READONLY_DOWNGRADE_SPEC("readonly_downgrade_spec"): The specification of read-only replicas is being downgraded.
+        # - READONLY_DOWNGRADE_DISK("readonly_downgrade_disk"): The disk space of read-only replicas is being scaled in.
+        # - CREATING_TENANT_READONLY_REPLICA("creating_tenant_readonly_replica"): A read-only replica is being created for a tenant in the cluster.
+        # - DELETING_TENANT_READONLY_REPLICA("deleting_tenant_readonly_replica"): A read-only replica is being deleted for a tenant in the cluster.
+        # - DISK_DOWNGRADING("disk_downgrading"): The disk space of the cluster is being scaled in.
+        # - DEPLOY_MODE_MODIFYING("deploy_mode_modifying"): The deployment mode of the cluster is being modified.
+        # > Generally, the cluster is in the ONLINE state.
         self.state = state  # type: str
-        # The number of resource units in the cluster.
+        # The size of used storage space of the cluster, in GB.
         self.used_disk_size = used_disk_size  # type: long
-        # The total number of CPU cores of the cluster.
+        # The OBServer version.
         self.version = version  # type: str
         # vpcId
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         if self.data_disk_auto_scale_config:
             self.data_disk_auto_scale_config.validate()
@@ -12188,17 +12365,19 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeInstancesResponseBody(TeaModel):
     def __init__(self, instances=None, request_id=None, total_count=None):
-        # The total storage space of the cluster, in GB.
+        # The information of the OceanBase cluster.
         self.instances = instances  # type: list[DescribeInstancesResponseBodyInstances]
+        # The request ID.
         self.request_id = request_id  # type: str
+        # The number of OceanBase clusters queried.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.instances:
             for k in self.instances:
                 if k:
                     k.validate()
@@ -17561,19 +17740,24 @@
         if m.get('SyncDelaySampleTimestamp') is not None:
             self.sync_delay_sample_timestamp = m.get('SyncDelaySampleTimestamp')
         return self
 
 
 class DescribeProjectResponseBodyDataFullTransferConfig(TeaModel):
     def __init__(self, allow_dest_table_not_empty=None, full_transfer_speed_mode=None,
-                 full_verify_speed_mode=None, none_pk_uk_truncate_dst_table=None):
+                 full_verify_speed_mode=None, none_pk_uk_truncate_dst_table=None, read_worker_num=None, throttle_iops=None,
+                 throttle_rps=None, write_worker_num=None):
         self.allow_dest_table_not_empty = allow_dest_table_not_empty  # type: bool
         self.full_transfer_speed_mode = full_transfer_speed_mode  # type: str
         self.full_verify_speed_mode = full_verify_speed_mode  # type: str
         self.none_pk_uk_truncate_dst_table = none_pk_uk_truncate_dst_table  # type: bool
+        self.read_worker_num = read_worker_num  # type: int
+        self.throttle_iops = throttle_iops  # type: int
+        self.throttle_rps = throttle_rps  # type: int
+        self.write_worker_num = write_worker_num  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeProjectResponseBodyDataFullTransferConfig, self).to_map()
         if _map is not None:
@@ -17584,38 +17768,58 @@
             result['AllowDestTableNotEmpty'] = self.allow_dest_table_not_empty
         if self.full_transfer_speed_mode is not None:
             result['FullTransferSpeedMode'] = self.full_transfer_speed_mode
         if self.full_verify_speed_mode is not None:
             result['FullVerifySpeedMode'] = self.full_verify_speed_mode
         if self.none_pk_uk_truncate_dst_table is not None:
             result['NonePkUkTruncateDstTable'] = self.none_pk_uk_truncate_dst_table
+        if self.read_worker_num is not None:
+            result['ReadWorkerNum'] = self.read_worker_num
+        if self.throttle_iops is not None:
+            result['ThrottleIOPS'] = self.throttle_iops
+        if self.throttle_rps is not None:
+            result['ThrottleRps'] = self.throttle_rps
+        if self.write_worker_num is not None:
+            result['WriteWorkerNum'] = self.write_worker_num
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AllowDestTableNotEmpty') is not None:
             self.allow_dest_table_not_empty = m.get('AllowDestTableNotEmpty')
         if m.get('FullTransferSpeedMode') is not None:
             self.full_transfer_speed_mode = m.get('FullTransferSpeedMode')
         if m.get('FullVerifySpeedMode') is not None:
             self.full_verify_speed_mode = m.get('FullVerifySpeedMode')
         if m.get('NonePkUkTruncateDstTable') is not None:
             self.none_pk_uk_truncate_dst_table = m.get('NonePkUkTruncateDstTable')
+        if m.get('ReadWorkerNum') is not None:
+            self.read_worker_num = m.get('ReadWorkerNum')
+        if m.get('ThrottleIOPS') is not None:
+            self.throttle_iops = m.get('ThrottleIOPS')
+        if m.get('ThrottleRps') is not None:
+            self.throttle_rps = m.get('ThrottleRps')
+        if m.get('WriteWorkerNum') is not None:
+            self.write_worker_num = m.get('WriteWorkerNum')
         return self
 
 
 class DescribeProjectResponseBodyDataIncrTransferConfig(TeaModel):
     def __init__(self, enable_incr_sync_statistics=None, enable_sequencing_within_txn=None,
-                 incr_sync_concurrency=None, record_type_white_list=None, start_timestamp=None, store_log_kept_hour=None):
+                 incr_sync_concurrency=None, record_type_white_list=None, start_timestamp=None, store_log_kept_hour=None,
+                 support_ddltypes=None, throttle_iops=None, throttle_rps=None):
         self.enable_incr_sync_statistics = enable_incr_sync_statistics  # type: bool
         self.enable_sequencing_within_txn = enable_sequencing_within_txn  # type: bool
         self.incr_sync_concurrency = incr_sync_concurrency  # type: int
         self.record_type_white_list = record_type_white_list  # type: list[str]
         self.start_timestamp = start_timestamp  # type: long
         self.store_log_kept_hour = store_log_kept_hour  # type: int
+        self.support_ddltypes = support_ddltypes  # type: list[str]
+        self.throttle_iops = throttle_iops  # type: int
+        self.throttle_rps = throttle_rps  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeProjectResponseBodyDataIncrTransferConfig, self).to_map()
         if _map is not None:
@@ -17630,14 +17834,20 @@
             result['IncrSyncConcurrency'] = self.incr_sync_concurrency
         if self.record_type_white_list is not None:
             result['RecordTypeWhiteList'] = self.record_type_white_list
         if self.start_timestamp is not None:
             result['StartTimestamp'] = self.start_timestamp
         if self.store_log_kept_hour is not None:
             result['StoreLogKeptHour'] = self.store_log_kept_hour
+        if self.support_ddltypes is not None:
+            result['SupportDDLTypes'] = self.support_ddltypes
+        if self.throttle_iops is not None:
+            result['ThrottleIOPS'] = self.throttle_iops
+        if self.throttle_rps is not None:
+            result['ThrottleRps'] = self.throttle_rps
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('EnableIncrSyncStatistics') is not None:
             self.enable_incr_sync_statistics = m.get('EnableIncrSyncStatistics')
         if m.get('EnableSequencingWithinTxn') is not None:
@@ -17646,14 +17856,20 @@
             self.incr_sync_concurrency = m.get('IncrSyncConcurrency')
         if m.get('RecordTypeWhiteList') is not None:
             self.record_type_white_list = m.get('RecordTypeWhiteList')
         if m.get('StartTimestamp') is not None:
             self.start_timestamp = m.get('StartTimestamp')
         if m.get('StoreLogKeptHour') is not None:
             self.store_log_kept_hour = m.get('StoreLogKeptHour')
+        if m.get('SupportDDLTypes') is not None:
+            self.support_ddltypes = m.get('SupportDDLTypes')
+        if m.get('ThrottleIOPS') is not None:
+            self.throttle_iops = m.get('ThrottleIOPS')
+        if m.get('ThrottleRps') is not None:
+            self.throttle_rps = m.get('ThrottleRps')
         return self
 
 
 class DescribeProjectResponseBodyDataLabels(TeaModel):
     def __init__(self, id=None, name=None):
         self.id = id  # type: str
         self.name = name  # type: str
@@ -17678,14 +17894,80 @@
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         return self
 
 
+class DescribeProjectResponseBodyDataReverseIncrTransferConfig(TeaModel):
+    def __init__(self, enable_incr_sync_statistics=None, enable_sequencing_within_txn=None,
+                 incr_sync_concurrency=None, record_type_white_list=None, start_timestamp=None, store_log_kept_hour=None,
+                 support_ddltypes=None, throttle_iops=None, throttle_rps=None):
+        self.enable_incr_sync_statistics = enable_incr_sync_statistics  # type: bool
+        self.enable_sequencing_within_txn = enable_sequencing_within_txn  # type: bool
+        self.incr_sync_concurrency = incr_sync_concurrency  # type: int
+        self.record_type_white_list = record_type_white_list  # type: list[str]
+        self.start_timestamp = start_timestamp  # type: long
+        self.store_log_kept_hour = store_log_kept_hour  # type: int
+        self.support_ddltypes = support_ddltypes  # type: list[str]
+        self.throttle_iops = throttle_iops  # type: int
+        self.throttle_rps = throttle_rps  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeProjectResponseBodyDataReverseIncrTransferConfig, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enable_incr_sync_statistics is not None:
+            result['EnableIncrSyncStatistics'] = self.enable_incr_sync_statistics
+        if self.enable_sequencing_within_txn is not None:
+            result['EnableSequencingWithinTxn'] = self.enable_sequencing_within_txn
+        if self.incr_sync_concurrency is not None:
+            result['IncrSyncConcurrency'] = self.incr_sync_concurrency
+        if self.record_type_white_list is not None:
+            result['RecordTypeWhiteList'] = self.record_type_white_list
+        if self.start_timestamp is not None:
+            result['StartTimestamp'] = self.start_timestamp
+        if self.store_log_kept_hour is not None:
+            result['StoreLogKeptHour'] = self.store_log_kept_hour
+        if self.support_ddltypes is not None:
+            result['SupportDDLTypes'] = self.support_ddltypes
+        if self.throttle_iops is not None:
+            result['ThrottleIOPS'] = self.throttle_iops
+        if self.throttle_rps is not None:
+            result['ThrottleRps'] = self.throttle_rps
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('EnableIncrSyncStatistics') is not None:
+            self.enable_incr_sync_statistics = m.get('EnableIncrSyncStatistics')
+        if m.get('EnableSequencingWithinTxn') is not None:
+            self.enable_sequencing_within_txn = m.get('EnableSequencingWithinTxn')
+        if m.get('IncrSyncConcurrency') is not None:
+            self.incr_sync_concurrency = m.get('IncrSyncConcurrency')
+        if m.get('RecordTypeWhiteList') is not None:
+            self.record_type_white_list = m.get('RecordTypeWhiteList')
+        if m.get('StartTimestamp') is not None:
+            self.start_timestamp = m.get('StartTimestamp')
+        if m.get('StoreLogKeptHour') is not None:
+            self.store_log_kept_hour = m.get('StoreLogKeptHour')
+        if m.get('SupportDDLTypes') is not None:
+            self.support_ddltypes = m.get('SupportDDLTypes')
+        if m.get('ThrottleIOPS') is not None:
+            self.throttle_iops = m.get('ThrottleIOPS')
+        if m.get('ThrottleRps') is not None:
+            self.throttle_rps = m.get('ThrottleRps')
+        return self
+
+
 class DescribeProjectResponseBodyDataSinkConnectInfo(TeaModel):
     def __init__(self, charset=None, conn_extra_attributes=None, connection_info=None, db_engine=None,
                  endpoint_id=None, endpoint_name=None, endpoint_side=None, host=None, id=None, nls_length_semantics=None,
                  ocp_name=None, operating_system=None, owner=None, port=None, region=None, resource_owner=None, timezone=None,
                  username=None, version=None):
         self.charset = charset  # type: str
         self.conn_extra_attributes = conn_extra_attributes  # type: any
@@ -19283,17 +19565,18 @@
 
 
 class DescribeProjectResponseBodyData(TeaModel):
     def __init__(self, alarm_stats=None, common_transfer_config=None, dest_conn_id=None, enable_full_transfer=None,
                  enable_full_verify=None, enable_incr_transfer=None, enable_incr_verify=None, enable_reverse_incr_transfer=None,
                  enable_struct_transfer=None, extra_info=None, full_transfer_config=None, gmt_create=None, gmt_finish=None,
                  gmt_modified=None, gmt_start=None, id=None, importance=None, incr_transfer_config=None, is_merging=None,
-                 is_modifying=None, is_sub_project=None, labels=None, name=None, owner=None, sink_connect_info=None,
-                 sink_endpoint_type=None, source_connect_info=None, source_endpoint_type=None, status=None, steps=None,
-                 struct_transfer_config=None, transfer_mapping=None, type=None, worker_grade_id=None, worker_grade_info=None):
+                 is_modifying=None, is_sub_project=None, labels=None, name=None, owner=None, reverse_incr_transfer_config=None,
+                 sink_connect_info=None, sink_endpoint_type=None, source_connect_info=None, source_endpoint_type=None, status=None,
+                 steps=None, struct_transfer_config=None, transfer_mapping=None, type=None, worker_grade_id=None,
+                 worker_grade_info=None):
         self.alarm_stats = alarm_stats  # type: DescribeProjectResponseBodyDataAlarmStats
         self.common_transfer_config = common_transfer_config  # type: DescribeProjectResponseBodyDataCommonTransferConfig
         self.dest_conn_id = dest_conn_id  # type: str
         self.enable_full_transfer = enable_full_transfer  # type: bool
         self.enable_full_verify = enable_full_verify  # type: bool
         self.enable_incr_transfer = enable_incr_transfer  # type: bool
         self.enable_incr_verify = enable_incr_verify  # type: bool
@@ -19310,14 +19593,15 @@
         self.incr_transfer_config = incr_transfer_config  # type: DescribeProjectResponseBodyDataIncrTransferConfig
         self.is_merging = is_merging  # type: bool
         self.is_modifying = is_modifying  # type: bool
         self.is_sub_project = is_sub_project  # type: bool
         self.labels = labels  # type: list[DescribeProjectResponseBodyDataLabels]
         self.name = name  # type: str
         self.owner = owner  # type: str
+        self.reverse_incr_transfer_config = reverse_incr_transfer_config  # type: DescribeProjectResponseBodyDataReverseIncrTransferConfig
         self.sink_connect_info = sink_connect_info  # type: DescribeProjectResponseBodyDataSinkConnectInfo
         self.sink_endpoint_type = sink_endpoint_type  # type: str
         self.source_connect_info = source_connect_info  # type: DescribeProjectResponseBodyDataSourceConnectInfo
         self.source_endpoint_type = source_endpoint_type  # type: str
         self.status = status  # type: str
         self.steps = steps  # type: list[DescribeProjectResponseBodyDataSteps]
         self.struct_transfer_config = struct_transfer_config  # type: DescribeProjectResponseBodyDataStructTransferConfig
@@ -19337,14 +19621,16 @@
             self.full_transfer_config.validate()
         if self.incr_transfer_config:
             self.incr_transfer_config.validate()
         if self.labels:
             for k in self.labels:
                 if k:
                     k.validate()
+        if self.reverse_incr_transfer_config:
+            self.reverse_incr_transfer_config.validate()
         if self.sink_connect_info:
             self.sink_connect_info.validate()
         if self.source_connect_info:
             self.source_connect_info.validate()
         if self.steps:
             for k in self.steps:
                 if k:
@@ -19408,14 +19694,16 @@
         if self.labels is not None:
             for k in self.labels:
                 result['Labels'].append(k.to_map() if k else None)
         if self.name is not None:
             result['Name'] = self.name
         if self.owner is not None:
             result['Owner'] = self.owner
+        if self.reverse_incr_transfer_config is not None:
+            result['ReverseIncrTransferConfig'] = self.reverse_incr_transfer_config.to_map()
         if self.sink_connect_info is not None:
             result['SinkConnectInfo'] = self.sink_connect_info.to_map()
         if self.sink_endpoint_type is not None:
             result['SinkEndpointType'] = self.sink_endpoint_type
         if self.source_connect_info is not None:
             result['SourceConnectInfo'] = self.source_connect_info.to_map()
         if self.source_endpoint_type is not None:
@@ -19492,14 +19780,17 @@
             for k in m.get('Labels'):
                 temp_model = DescribeProjectResponseBodyDataLabels()
                 self.labels.append(temp_model.from_map(k))
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Owner') is not None:
             self.owner = m.get('Owner')
+        if m.get('ReverseIncrTransferConfig') is not None:
+            temp_model = DescribeProjectResponseBodyDataReverseIncrTransferConfig()
+            self.reverse_incr_transfer_config = temp_model.from_map(m['ReverseIncrTransferConfig'])
         if m.get('SinkConnectInfo') is not None:
             temp_model = DescribeProjectResponseBodyDataSinkConnectInfo()
             self.sink_connect_info = temp_model.from_map(m['SinkConnectInfo'])
         if m.get('SinkEndpointType') is not None:
             self.sink_endpoint_type = m.get('SinkEndpointType')
         if m.get('SourceConnectInfo') is not None:
             temp_model = DescribeProjectResponseBodyDataSourceConnectInfo()
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO` & `alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-oceanbasepro20190901-py2
-Version: 3.0.1
+Version: 3.0.2
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-3.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt` & `alibabacloud_oceanbasepro20190901_py2-3.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-3.0.1/setup.py` & `alibabacloud_oceanbasepro20190901_py2-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_oceanbasepro20190901_py2.
 
-Created on 25/03/2024
+Created on 08/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_oceanbasepro20190901"
 NAME = "alibabacloud_oceanbasepro20190901_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2"
```

