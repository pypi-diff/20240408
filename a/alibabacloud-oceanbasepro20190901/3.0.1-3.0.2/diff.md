# Comparing `tmp/alibabacloud_oceanbasepro20190901-3.0.1.tar.gz` & `tmp/alibabacloud_oceanbasepro20190901-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901-3.0.1.tar", last modified: Mon Mar 25 12:42:18 2024, max compression
+gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901-3.0.2.tar", last modified: Mon Apr  8 12:13:31 2024, max compression
```

## Comparing `alibabacloud_oceanbasepro20190901-3.0.1.tar` & `alibabacloud_oceanbasepro20190901-3.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/
--rw-r--r--   0 root         (0) root         (0)     2219 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2464 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1131 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1216 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   426822 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901/client.py
--rw-r--r--   0 root         (0) root         (0)  1648565 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2464 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      492 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2656 2024-03-25 12:42:18.000000 alibabacloud_oceanbasepro20190901-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 12:13:31.000000 alibabacloud_oceanbasepro20190901-3.0.2/
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901-3.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901-3.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901-3.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2464 2024-04-08 12:13:31.000000 alibabacloud_oceanbasepro20190901-3.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901-3.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1216 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901-3.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 12:13:31.000000 alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   427692 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901/client.py
+-rw-r--r--   0 root         (0) root         (0)  1666488 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 12:13:31.000000 alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2464 2024-04-08 12:13:31.000000 alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      492 2024-04-08 12:13:31.000000 alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 12:13:31.000000 alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-08 12:13:31.000000 alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-08 12:13:31.000000 alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-08 12:13:31.000000 alibabacloud_oceanbasepro20190901-3.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2656 2024-04-08 12:13:30.000000 alibabacloud_oceanbasepro20190901-3.0.2/setup.py
```

### Comparing `alibabacloud_oceanbasepro20190901-3.0.1/ChangeLog.md` & `alibabacloud_oceanbasepro20190901-3.0.2/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-03-25 Version: 3.0.1
+- Generated python 2019-09-01 for OceanBasePro.
+
 2024-03-20 Version: 3.0.0
 - Delete API CreateOmsOpenAPIProject.
 - Delete API DeleteOmsOpenAPIProject.
 - Delete API DescribeOmsOpenAPIProject.
 - Delete API DescribeOmsOpenAPIProjectSteps.
 - Delete API ReleaseOmsOpenAPIProject.
 - Delete API ResetOmsOpenAPIProject.
```

### Comparing `alibabacloud_oceanbasepro20190901-3.0.1/LICENSE` & `alibabacloud_oceanbasepro20190901-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-3.0.1/PKG-INFO` & `alibabacloud_oceanbasepro20190901-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_oceanbasepro20190901
-Version: 3.0.1
+Version: 3.0.2
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901-3.0.1/README-CN.md` & `alibabacloud_oceanbasepro20190901-3.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-3.0.1/README.md` & `alibabacloud_oceanbasepro20190901-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901/client.py` & `alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -875,14 +875,16 @@
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
@@ -904,14 +906,16 @@
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
@@ -953,14 +957,16 @@
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
@@ -982,14 +988,16 @@
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

### Comparing `alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901/models.py` & `alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2458,19 +2458,27 @@
 class CreateProjectRequestFullTransferConfig(TeaModel):
     def __init__(
         self,
         allow_dest_table_not_empty: bool = None,
         full_transfer_speed_mode: str = None,
         full_verify_speed_mode: str = None,
         none_pk_uk_truncate_dst_table: bool = None,
+        read_worker_num: int = None,
+        throttle_iops: int = None,
+        throttle_rps: int = None,
+        write_worker_num: int = None,
     ):
         self.allow_dest_table_not_empty = allow_dest_table_not_empty
         self.full_transfer_speed_mode = full_transfer_speed_mode
         self.full_verify_speed_mode = full_verify_speed_mode
         self.none_pk_uk_truncate_dst_table = none_pk_uk_truncate_dst_table
+        self.read_worker_num = read_worker_num
+        self.throttle_iops = throttle_iops
+        self.throttle_rps = throttle_rps
+        self.write_worker_num = write_worker_num
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -2481,45 +2489,67 @@
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         enable_incr_sync_statistics: bool = None,
         enable_sequencing_within_txn: bool = None,
         incr_sync_concurrency: int = None,
         record_type_white_list: List[str] = None,
         start_timestamp: str = None,
         store_log_kept_hour: int = None,
+        support_ddltypes: List[str] = None,
+        throttle_iops: int = None,
+        throttle_rps: int = None,
     ):
         self.enable_incr_sync_statistics = enable_incr_sync_statistics
         self.enable_sequencing_within_txn = enable_sequencing_within_txn
         self.incr_sync_concurrency = incr_sync_concurrency
         self.record_type_white_list = record_type_white_list
         self.start_timestamp = start_timestamp
         self.store_log_kept_hour = store_log_kept_hour
+        self.support_ddltypes = support_ddltypes
+        self.throttle_iops = throttle_iops
+        self.throttle_rps = throttle_rps
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -2534,14 +2564,20 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('EnableIncrSyncStatistics') is not None:
             self.enable_incr_sync_statistics = m.get('EnableIncrSyncStatistics')
         if m.get('EnableSequencingWithinTxn') is not None:
@@ -2550,14 +2586,95 @@
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
+    def __init__(
+        self,
+        enable_incr_sync_statistics: bool = None,
+        enable_sequencing_within_txn: bool = None,
+        incr_sync_concurrency: int = None,
+        record_type_white_list: List[str] = None,
+        start_timestamp: str = None,
+        store_log_kept_hour: int = None,
+        support_ddltypes: List[str] = None,
+        throttle_iops: int = None,
+        throttle_rps: int = None,
+    ):
+        self.enable_incr_sync_statistics = enable_incr_sync_statistics
+        self.enable_sequencing_within_txn = enable_sequencing_within_txn
+        self.incr_sync_concurrency = incr_sync_concurrency
+        self.record_type_white_list = record_type_white_list
+        self.start_timestamp = start_timestamp
+        self.store_log_kept_hour = store_log_kept_hour
+        self.support_ddltypes = support_ddltypes
+        self.throttle_iops = throttle_iops
+        self.throttle_rps = throttle_rps
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         byte_char_convert_strategy: str = None,
@@ -3769,14 +3886,15 @@
         enable_struct_transfer: bool = None,
         full_transfer_config: CreateProjectRequestFullTransferConfig = None,
         id: str = None,
         incr_transfer_config: CreateProjectRequestIncrTransferConfig = None,
         label_ids: List[str] = None,
         name: str = None,
         oss_key: str = None,
+        reverse_incr_transfer_config: CreateProjectRequestReverseIncrTransferConfig = None,
         sink_endpoint_id: str = None,
         source_endpoint_id: str = None,
         struct_transfer_config: CreateProjectRequestStructTransferConfig = None,
         transfer_mapping: CreateProjectRequestTransferMapping = None,
         type: str = None,
         use_oss: bool = None,
         worker_grade_id: str = None,
@@ -3789,14 +3907,15 @@
         self.enable_struct_transfer = enable_struct_transfer
         self.full_transfer_config = full_transfer_config
         self.id = id
         self.incr_transfer_config = incr_transfer_config
         self.label_ids = label_ids
         self.name = name
         self.oss_key = oss_key
+        self.reverse_incr_transfer_config = reverse_incr_transfer_config
         self.sink_endpoint_id = sink_endpoint_id
         self.source_endpoint_id = source_endpoint_id
         self.struct_transfer_config = struct_transfer_config
         self.transfer_mapping = transfer_mapping
         self.type = type
         self.use_oss = use_oss
         self.worker_grade_id = worker_grade_id
@@ -3804,14 +3923,16 @@
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
         _map = super().to_map()
@@ -3839,14 +3960,16 @@
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
@@ -3884,14 +4007,17 @@
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
@@ -3918,14 +4044,15 @@
         enable_struct_transfer: bool = None,
         full_transfer_config_shrink: str = None,
         id: str = None,
         incr_transfer_config_shrink: str = None,
         label_ids_shrink: str = None,
         name: str = None,
         oss_key: str = None,
+        reverse_incr_transfer_config_shrink: str = None,
         sink_endpoint_id: str = None,
         source_endpoint_id: str = None,
         struct_transfer_config_shrink: str = None,
         transfer_mapping_shrink: str = None,
         type: str = None,
         use_oss: bool = None,
         worker_grade_id: str = None,
@@ -3938,14 +4065,15 @@
         self.enable_struct_transfer = enable_struct_transfer
         self.full_transfer_config_shrink = full_transfer_config_shrink
         self.id = id
         self.incr_transfer_config_shrink = incr_transfer_config_shrink
         self.label_ids_shrink = label_ids_shrink
         self.name = name
         self.oss_key = oss_key
+        self.reverse_incr_transfer_config_shrink = reverse_incr_transfer_config_shrink
         self.sink_endpoint_id = sink_endpoint_id
         self.source_endpoint_id = source_endpoint_id
         self.struct_transfer_config_shrink = struct_transfer_config_shrink
         self.transfer_mapping_shrink = transfer_mapping_shrink
         self.type = type
         self.use_oss = use_oss
         self.worker_grade_id = worker_grade_id
@@ -3979,14 +4107,16 @@
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
@@ -4021,14 +4151,16 @@
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
@@ -13160,25 +13292,29 @@
         instance_id: str = None,
         instance_name: str = None,
         page_number: int = None,
         page_size: int = None,
         resource_group_id: str = None,
         search_key: str = None,
     ):
-        # The number of CPU cores used in the cluster.
+        # The ID of the OceanBase cluster.
         self.instance_id = instance_id
-        # The size of used memory in the cluster, in GB.
+        # The name of the OceanBase cluster. It must be 1 to 20 characters in length. If this parameter is not specified, the value is the instance ID of the cluster by default.
         self.instance_name = instance_name
-        # The total memory size of the cluster, in GB.
+        # The number of the page to return.
+        # - Pages start from page 1.
+        # - Default value: 1.
         self.page_number = page_number
-        # The information about the memory resources of the cluster.
+        # The number of rows to return on each page.
+        # - Maximum value: 100.
+        # - Default value: 10.
         self.page_size = page_size
-        # The number of CPU cores of each replica node in the cluster.
+        # The ID of the resource group. If you do not specify this parameter, all resources are returned.
         self.resource_group_id = resource_group_id
-        # The memory size of each replica node in the cluster, in GB.
+        # The keyword for fuzzy search, which can be an instance ID, instance name, tenant ID, or tenant name.
         self.search_key = search_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13225,21 +13361,29 @@
         scale_step_in_merge: int = None,
         scale_step_in_normal: int = None,
         upper_merge_threshold: int = None,
         upper_scale_strategy: str = None,
         upper_threshold: int = None,
         upperbound: int = None,
     ):
+        # Specifies whether to enable the automatic scaling of the data disk.
         self.auto_scale = auto_scale
+        # The maximum size of the disk, in GB.
         self.max_disk_size = max_disk_size
+        # The size of scaling step during a major compaction.
         self.scale_step_in_merge = scale_step_in_merge
+        # The size of scaling step during daily use.
         self.scale_step_in_normal = scale_step_in_normal
+        # The maximum usage of the data disk, in percentage, that triggers the scaling of the data disk for major compactions.
         self.upper_merge_threshold = upper_merge_threshold
+        # The scale-out strategy. Valid values: RAW and PERCENTAGE.
         self.upper_scale_strategy = upper_scale_strategy
+        # The maximum usage of the data disk, in percentage, that triggers the scaling of the data disk for daily use.
         self.upper_threshold = upper_threshold
+        # The maximum space, in GB, to which the data disk can be scaled.
         self.upperbound = upperbound
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13289,16 +13433,19 @@
 class DescribeInstancesResponseBodyInstancesResourceCapacityUnit(TeaModel):
     def __init__(
         self,
         max_capacity_unit: int = None,
         min_capacity_unit: int = None,
         used_capacity_unit: int = None,
     ):
+        # The maximum number of capacity units.
         self.max_capacity_unit = max_capacity_unit
+        # The minimum number of capacity units.
         self.min_capacity_unit = min_capacity_unit
+        # The number of used capacity units.
         self.used_capacity_unit = used_capacity_unit
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13329,26 +13476,21 @@
     def __init__(
         self,
         original_total_cpu: int = None,
         total_cpu: int = None,
         unit_cpu: int = None,
         used_cpu: int = None,
     ):
+        # The number of original CPU cores in the cluster.
         self.original_total_cpu = original_total_cpu
-        # The name of the OceanBase cluster.    
-        # It must be 1 to 20 characters in length.   
-        # If this parameter is not specified, the value is the instance ID of the cluster by default.
+        # The total number of CPU cores of the cluster.
         self.total_cpu = total_cpu
-        # The data replica distribution mode of the cluster. Valid values:    
-        # 
-        # - n: indicates the single-IDC mode.  
-        # - n-n: indicates the dual-IDC mode.  
-        # - n-n-n: indicates the multi-IDC mode. The integer n represents the number of OBServer nodes in each IDC.
+        # The number of CPU cores of each replica node in the cluster.
         self.unit_cpu = unit_cpu
-        # The search keyword.
+        # The number of CPU cores used in the cluster.
         self.used_cpu = used_cpu
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13383,20 +13525,21 @@
     def __init__(
         self,
         original_total_disk_size: int = None,
         total_disk_size: int = None,
         unit_disk_size: int = None,
         used_disk_size: int = None,
     ):
+        # The original size of the disk.
         self.original_total_disk_size = original_total_disk_size
-        # The request ID.
+        # The total storage space of the cluster, in GB.
         self.total_disk_size = total_disk_size
-        # Example 1
+        # The storage space of each replica node in the cluster, in GB.
         self.unit_disk_size = unit_disk_size
-        # $.parameters[7].schema.example
+        # The size of used storage space of the cluster, in GB.
         self.used_disk_size = used_disk_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13431,18 +13574,19 @@
     def __init__(
         self,
         original_total_memory: int = None,
         total_memory: int = None,
         unit_memory: int = None,
         used_memory: int = None,
     ):
+        # The original memory size of the cluster, in GB.
         self.original_total_memory = original_total_memory
-        # The number of CPU cores of the cluster.
+        # The total memory size of the cluster, in GB.
         self.total_memory = total_memory
-        # The size of used storage space of the cluster, in GB.
+        # The memory size of each replica node in the cluster, in GB.
         self.unit_memory = unit_memory
         # The size of used memory in the cluster, in GB.
         self.used_memory = used_memory
 
     def validate(self):
         pass
 
@@ -13480,36 +13624,23 @@
         self,
         capacity_unit: DescribeInstancesResponseBodyInstancesResourceCapacityUnit = None,
         cpu: DescribeInstancesResponseBodyInstancesResourceCpu = None,
         disk_size: DescribeInstancesResponseBodyInstancesResourceDiskSize = None,
         memory: DescribeInstancesResponseBodyInstancesResourceMemory = None,
         unit_count: int = None,
     ):
+        # The information about capacity units.
         self.capacity_unit = capacity_unit
-        # Indicates whether new nodes can be added.
+        # The information about the CPU resources of the cluster.
         self.cpu = cpu
-        # The time elapsed since the expiration of the cluster, in seconds.
+        # The information about the storage resources of the cluster.
         self.disk_size = disk_size
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
         self.memory = memory
+        # The number of resource units in the cluster.
         self.unit_count = unit_count
 
     def validate(self):
         if self.capacity_unit:
             self.capacity_unit.validate()
         if self.cpu:
             self.cpu.validate()
@@ -13585,72 +13716,134 @@
         resource_group_id: str = None,
         series: str = None,
         state: str = None,
         used_disk_size: int = None,
         version: str = None,
         vpc_id: str = None,
     ):
-        # The time in UTC when the cluster expires.
+        # The information about the zone in which the cluster is deployed.
         self.available_zones = available_zones
-        # The storage space of each replica node in the cluster, in GB.
-        self.commodity_code = commodity_code
         # The product code of the OceanBase cluster.   
         # - oceanbase_oceanbasepre_public_cn: indicates an OceanBase cluster that is billed based on the subscription plan and that is deployed in a China site.  
         # - oceanbase_oceanbasepost_public_cn: indicates an OceanBase cluster that is billed based on the pay-as-you-go plan and that is deployed in a China site.  
         # - oceanbase_obpre_public_intl: indicates an OceanBase cluster that is billed based on the subscription plan and that is deployed in an international site.
+        self.commodity_code = commodity_code
+        # The number of CPU cores of the cluster.
         self.cpu = cpu
+        # The CPU architecture of the cluster.
         self.cpu_architecture = cpu_architecture
-        # The number of OceanBase clusters queried.
+        # The time in UTC when the cluster was created.
         self.create_time = create_time
+        # Specifies parameters for the automatic scaling of the data disk.
         self.data_disk_auto_scale_config = data_disk_auto_scale_config
-        # The request ID.
+        # The data replica distribution mode of the cluster. The value is in the n-n-n format, where n is the number of OBServer nodes in each IDC.
         self.deploy_mode = deploy_mode
-        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
+        # The deployment type of the cluster. Valid values:   
+        # - multiple: multi-IDC deployment  
+        # - single: single-IDC deployment  
+        # - dual: dual-IDC deployment
         self.deploy_type = deploy_type
-        # The information about the memory resources of the cluster.
+        # The size of the storage space, in GB.
         self.disk_size = disk_size
-        # The number of CPU cores used in the cluster.
+        # The type of the storage disk where the cluster is deployed.   
+        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
         self.disk_type = disk_type
+        # Indicates whether the cluster supports read-only replicas.
         self.enable_read_only_replica_management = enable_read_only_replica_management
-        # The ID of the OceanBase cluster.
+        # Indicates whether new nodes can be added.
         self.enable_upgrade_nodes = enable_upgrade_nodes
-        # The whitelist information of the cluster.
+        # The time elapsed since the expiration of the cluster, in seconds. 
+        # > In subscription mode, if the cluster has not expired, this parameter indicates the remaining validity period of the cluster. If the cluster has expired, this parameter indicates the time elapsed since the expiration.
         self.expire_seconds = expire_seconds
-        # The information about the storage resources of the cluster.
+        # The time in UTC when the cluster expires. 
+        # > This parameter is valid only for subscription instances.
         self.expire_time = expire_time
+        # Specifies whether to indicate the temporary status of the capacity.
         self.in_temp_capacity_status = in_temp_capacity_status
-        # The instance type.
+        # The specifications of the cluster.  You can specify one of the following four plans:  
+        # - 8C32G: indicates 8 CPU cores and 32 GB of memory.  
+        # - 14C70G: indicates 14 CPU cores and 70 GB of memory.  
+        # - 30C180G: indicates 30 CPU cores and 180 GB of memory.  
+        # - 62C400G: indicates 62 CPU cores and 400 GB of memory.
         self.instance_class = instance_class
-        # The total storage space of the cluster, in GB.
+        # The ID of the OceanBase cluster.
         self.instance_id = instance_id
-        # The return result of the request.
+        # The name of the OceanBase cluster.
         self.instance_name = instance_name
+        # The role of the instance.
         self.instance_role = instance_role
-        # You can call this operation to obtain the list of OceanBase clusters.
+        # The instance type.
+        # - cluster: indicates a cluster instance.
+        # - mtenant: indicates a tenant instance in MySQL mode.
+        # - mtenant_serverless: indicates a serverless instance in MySQL mode.
         self.instance_type = instance_type
-        # The return result of the request.
+        # The time period in UTC for the daily routine maintenance of the cluster.
         self.maintain_time = maintain_time
-        # The information about the CPU resources of the cluster.
+        # The memory size of the instance, in GB.
         self.mem = mem
-        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
-        self.pay_type = pay_type
-        # The type of the storage disk where the cluster is deployed.   
-        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
-        self.resource = resource
-        # The number of OceanBase clusters queried.
-        self.resource_group_id = resource_group_id
         # The billing method for the OceanBase cluster. Valid values:  
         # - PREPAY: the subscription billing method.  
         # - POSTPAY: the pay-as-you-go billing method.
+        self.pay_type = pay_type
+        # The information about cluster resources.
+        self.resource = resource
+        # The ID of the resource group.
+        self.resource_group_id = resource_group_id
+        # The series of the OceanBase cluster. Valid values:   
+        # - NORMAL: the high availability edition.   
+        # - BASIC: the basic edition.
         self.series = series
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
         self.state = state
-        # The number of resource units in the cluster.
+        # The size of used storage space of the cluster, in GB.
         self.used_disk_size = used_disk_size
-        # The total number of CPU cores of the cluster.
+        # The OBServer version.
         self.version = version
         # vpcId
         self.vpc_id = vpc_id
 
     def validate(self):
         if self.data_disk_auto_scale_config:
             self.data_disk_auto_scale_config.validate()
@@ -13795,17 +13988,19 @@
 class DescribeInstancesResponseBody(TeaModel):
     def __init__(
         self,
         instances: List[DescribeInstancesResponseBodyInstances] = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The total storage space of the cluster, in GB.
+        # The information of the OceanBase cluster.
         self.instances = instances
+        # The request ID.
         self.request_id = request_id
+        # The number of OceanBase clusters queried.
         self.total_count = total_count
 
     def validate(self):
         if self.instances:
             for k in self.instances:
                 if k:
                     k.validate()
@@ -19871,19 +20066,27 @@
 class DescribeProjectResponseBodyDataFullTransferConfig(TeaModel):
     def __init__(
         self,
         allow_dest_table_not_empty: bool = None,
         full_transfer_speed_mode: str = None,
         full_verify_speed_mode: str = None,
         none_pk_uk_truncate_dst_table: bool = None,
+        read_worker_num: int = None,
+        throttle_iops: int = None,
+        throttle_rps: int = None,
+        write_worker_num: int = None,
     ):
         self.allow_dest_table_not_empty = allow_dest_table_not_empty
         self.full_transfer_speed_mode = full_transfer_speed_mode
         self.full_verify_speed_mode = full_verify_speed_mode
         self.none_pk_uk_truncate_dst_table = none_pk_uk_truncate_dst_table
+        self.read_worker_num = read_worker_num
+        self.throttle_iops = throttle_iops
+        self.throttle_rps = throttle_rps
+        self.write_worker_num = write_worker_num
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -19894,45 +20097,67 @@
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         enable_incr_sync_statistics: bool = None,
         enable_sequencing_within_txn: bool = None,
         incr_sync_concurrency: int = None,
         record_type_white_list: List[str] = None,
         start_timestamp: int = None,
         store_log_kept_hour: int = None,
+        support_ddltypes: List[str] = None,
+        throttle_iops: int = None,
+        throttle_rps: int = None,
     ):
         self.enable_incr_sync_statistics = enable_incr_sync_statistics
         self.enable_sequencing_within_txn = enable_sequencing_within_txn
         self.incr_sync_concurrency = incr_sync_concurrency
         self.record_type_white_list = record_type_white_list
         self.start_timestamp = start_timestamp
         self.store_log_kept_hour = store_log_kept_hour
+        self.support_ddltypes = support_ddltypes
+        self.throttle_iops = throttle_iops
+        self.throttle_rps = throttle_rps
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -19947,14 +20172,20 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('EnableIncrSyncStatistics') is not None:
             self.enable_incr_sync_statistics = m.get('EnableIncrSyncStatistics')
         if m.get('EnableSequencingWithinTxn') is not None:
@@ -19963,14 +20194,20 @@
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
     def __init__(
         self,
         id: str = None,
@@ -19999,14 +20236,89 @@
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         return self
 
 
+class DescribeProjectResponseBodyDataReverseIncrTransferConfig(TeaModel):
+    def __init__(
+        self,
+        enable_incr_sync_statistics: bool = None,
+        enable_sequencing_within_txn: bool = None,
+        incr_sync_concurrency: int = None,
+        record_type_white_list: List[str] = None,
+        start_timestamp: int = None,
+        store_log_kept_hour: int = None,
+        support_ddltypes: List[str] = None,
+        throttle_iops: int = None,
+        throttle_rps: int = None,
+    ):
+        self.enable_incr_sync_statistics = enable_incr_sync_statistics
+        self.enable_sequencing_within_txn = enable_sequencing_within_txn
+        self.incr_sync_concurrency = incr_sync_concurrency
+        self.record_type_white_list = record_type_white_list
+        self.start_timestamp = start_timestamp
+        self.store_log_kept_hour = store_log_kept_hour
+        self.support_ddltypes = support_ddltypes
+        self.throttle_iops = throttle_iops
+        self.throttle_rps = throttle_rps
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         charset: str = None,
         conn_extra_attributes: Any = None,
         connection_info: str = None,
         db_engine: str = None,
@@ -21840,14 +22152,15 @@
         incr_transfer_config: DescribeProjectResponseBodyDataIncrTransferConfig = None,
         is_merging: bool = None,
         is_modifying: bool = None,
         is_sub_project: bool = None,
         labels: List[DescribeProjectResponseBodyDataLabels] = None,
         name: str = None,
         owner: str = None,
+        reverse_incr_transfer_config: DescribeProjectResponseBodyDataReverseIncrTransferConfig = None,
         sink_connect_info: DescribeProjectResponseBodyDataSinkConnectInfo = None,
         sink_endpoint_type: str = None,
         source_connect_info: DescribeProjectResponseBodyDataSourceConnectInfo = None,
         source_endpoint_type: str = None,
         status: str = None,
         steps: List[DescribeProjectResponseBodyDataSteps] = None,
         struct_transfer_config: DescribeProjectResponseBodyDataStructTransferConfig = None,
@@ -21876,14 +22189,15 @@
         self.incr_transfer_config = incr_transfer_config
         self.is_merging = is_merging
         self.is_modifying = is_modifying
         self.is_sub_project = is_sub_project
         self.labels = labels
         self.name = name
         self.owner = owner
+        self.reverse_incr_transfer_config = reverse_incr_transfer_config
         self.sink_connect_info = sink_connect_info
         self.sink_endpoint_type = sink_endpoint_type
         self.source_connect_info = source_connect_info
         self.source_endpoint_type = source_endpoint_type
         self.status = status
         self.steps = steps
         self.struct_transfer_config = struct_transfer_config
@@ -21903,14 +22217,16 @@
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
@@ -21974,14 +22290,16 @@
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
@@ -22058,14 +22376,17 @@
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

### Comparing `alibabacloud_oceanbasepro20190901-3.0.1/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO` & `alibabacloud_oceanbasepro20190901-3.0.2/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-oceanbasepro20190901
-Version: 3.0.1
+Version: 3.0.2
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901-3.0.1/setup.py` & `alibabacloud_oceanbasepro20190901-3.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_oceanbasepro20190901.
 
-Created on 25/03/2024
+Created on 08/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_oceanbasepro20190901"
 NAME = "alibabacloud_oceanbasepro20190901" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OceanBasePro (20190901) SDK Library for Python"
```

