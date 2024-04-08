# Comparing `tmp/opus_protobuf-1.0.56.tar.gz` & `tmp/opus_protobuf-1.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opus_protobuf-1.0.56.tar", last modified: Thu Apr  4 02:25:46 2024, max compression
+gzip compressed data, was "opus_protobuf-1.0.57.tar", last modified: Mon Apr  8 02:54:39 2024, max compression
```

## Comparing `opus_protobuf-1.0.56.tar` & `opus_protobuf-1.0.57.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:25:46.594499 opus_protobuf-1.0.56/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-04 02:25:46.594499 opus_protobuf-1.0.56/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:25:46.594499 opus_protobuf-1.0.56/opus_protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/authentication_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/authentication_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26314 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/authentication_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/notification_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/notification_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15162 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/notification_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/payment_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/payment_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/payment_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/score_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/score_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/score_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/statistic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/statistic_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    47097 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/statistic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/web_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/web_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-04 02:25:46.374500 opus_protobuf-1.0.56/opus_protobuf/web_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-04 02:25:46.386500 opus_protobuf-1.0.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:54:39.968906 opus_protobuf-1.0.57/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-08 02:54:39.968906 opus_protobuf-1.0.57/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:54:39.968906 opus_protobuf-1.0.57/opus_protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/authentication_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/authentication_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26314 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/authentication_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/notification_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/notification_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15162 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/notification_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/payment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/payment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/payment_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/score_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/score_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-08 02:54:39.888906 opus_protobuf-1.0.57/opus_protobuf/score_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-04-08 02:54:39.892906 opus_protobuf-1.0.57/opus_protobuf/statistic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-08 02:54:39.892906 opus_protobuf-1.0.57/opus_protobuf/statistic_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    48759 2024-04-08 02:54:39.892906 opus_protobuf-1.0.57/opus_protobuf/statistic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-08 02:54:39.892906 opus_protobuf-1.0.57/opus_protobuf/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-08 02:54:39.892906 opus_protobuf-1.0.57/opus_protobuf/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-04-08 02:54:39.892906 opus_protobuf-1.0.57/opus_protobuf/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-08 02:54:39.892906 opus_protobuf-1.0.57/opus_protobuf/web_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-08 02:54:39.892906 opus_protobuf-1.0.57/opus_protobuf/web_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-08 02:54:39.892906 opus_protobuf-1.0.57/opus_protobuf/web_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-08 02:54:39.900906 opus_protobuf-1.0.57/setup.py
```

### Comparing `opus_protobuf-1.0.56/PKG-INFO` & `opus_protobuf-1.0.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: opus_protobuf
-Version: 1.0.56
+Version: 1.0.57
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/user/reponame
 Author: YOUR NAME
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `opus_protobuf-1.0.56/opus_protobuf/authentication_pb2.py` & `opus_protobuf-1.0.57/opus_protobuf/authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/authentication_pb2.pyi` & `opus_protobuf-1.0.57/opus_protobuf/authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/authentication_pb2_grpc.py` & `opus_protobuf-1.0.57/opus_protobuf/authentication_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/common_pb2.py` & `opus_protobuf-1.0.57/opus_protobuf/common_pb2.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/common_pb2.pyi` & `opus_protobuf-1.0.57/opus_protobuf/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/notification_pb2.py` & `opus_protobuf-1.0.57/opus_protobuf/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/notification_pb2.pyi` & `opus_protobuf-1.0.57/opus_protobuf/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/notification_pb2_grpc.py` & `opus_protobuf-1.0.57/opus_protobuf/notification_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/payment_pb2.py` & `opus_protobuf-1.0.57/opus_protobuf/payment_pb2.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/payment_pb2_grpc.py` & `opus_protobuf-1.0.57/opus_protobuf/payment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/score_pb2.py` & `opus_protobuf-1.0.57/opus_protobuf/score_pb2.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/score_pb2.pyi` & `opus_protobuf-1.0.57/opus_protobuf/score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/score_pb2_grpc.py` & `opus_protobuf-1.0.57/opus_protobuf/score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/statistic_pb2.py` & `opus_protobuf-1.0.57/opus_protobuf/statistic_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,39 +10,40 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from opus_protobuf import common_pb2 as opus__protobuf_dot_common__pb2
+from opus_protobuf import web_pb2 as opus__protobuf_dot_web__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dopus_protobuf/statistic.proto\x12\tstatistic\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1aopus_protobuf/common.proto\"e\n\x14UploadPictureRequest\x12\x13\n\x06userId\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\n\n\x02id\x18\x02 \x01(\t\x12!\n\x07picture\x18\x03 \x01(\x0b\x32\x10.common.DocumentB\t\n\x07_userId\"\x1b\n\x0b\x44\x61taRequest\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"\x82\x01\n\x0f\x41\x63\x63\x65ssInstagram\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\x0f\n\x02id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\x04user\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x03url\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\tB\x05\n\x03_idB\x07\n\x05_userB\x06\n\x04_url\"_\n\x1bInstagramControllerResponse\x12-\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x1f.statistic.InstagramApiResponse\x12\x11\n\thave_mean\x18\x02 \x01(\x08\"[\n\x14InstagramApiResponse\x12\r\n\x05value\x18\x01 \x01(\x05\x12\x10\n\x08metadata\x18\x02 \x01(\t\x12\x15\n\x08\x65nd_time\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_end_time\"b\n\x18GetInstagramLikesRequest\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x1a.statistic.AccessInstagram\x12\x12\n\x05\x62roke\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_broke\"!\n\x11LinkTikTokRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xce\x01\n\x17LinkTensorSocialRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x11\n\tlast_name\x18\x04 \x01(\t\x12\x0e\n\x06tenant\x18\x05 \x01(\t\x12\x10\n\x08industry\x18\x06 \x01(\t\x12\x18\n\x10industry_segment\x18\x07 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x08 \x01(\t\x12\x10\n\x08\x62irthday\x18\t \x01(\t\x12\x0c\n\x04\x63ity\x18\n \x01(\t\"\x8c\x01\n\rTalentProfile\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x02 \x01(\t\x12\x0e\n\x06tenant\x18\x03 \x01(\t\x12\x10\n\x08industry\x18\x04 \x01(\t\x12\x10\n\x08\x62irthday\x18\x05 \x01(\t\x12\x18\n\x10industry_segment\x18\x06 \x01(\t\x12\x0e\n\x06gender\x18\x07 \x01(\t\"\xad\x01\n\x0bTalentMedia\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\x04user\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\x05title\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04link\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x12\n\x05order\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x1e\n\x04\x66ile\x18\x06 \x01(\x0b\x32\x10.common.DocumentB\x07\n\x05_userB\x08\n\x06_titleB\x07\n\x05_linkB\x08\n\x06_order2\xd3\x10\n\x13StatisticController\x12\x37\n\x0bHealthCheck\x12\x16.google.protobuf.Empty\x1a\x0e.common.Health\"\x00\x12G\n\x10uploadSkuPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12>\n\x13UserConnectAyrshare\x12\x13.common.GetItemByID\x1a\x10.common.Response\"\x00\x12>\n\x10GetInstagramInfo\x12\x16.statistic.DataRequest\x1a\x10.common.Response\"\x00\x12]\n\x15GetInstagramFollowers\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12[\n\x13GetInstagramFollows\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x1aGetInstagramAudienceGender\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12`\n\x18GetInstagramAudienceCity\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x63\n\x1bGetInstagramAudienceCountry\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12Y\n\x11GetInstagramReach\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12`\n\x18GetInstagramInteractions\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x11GetInstagramLikes\x12#.statistic.GetInstagramLikesRequest\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x1aGetInstagramEngagementRate\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x41\n\x13UpdateSocialNetwork\x12\x16.statistic.DataRequest\x1a\x10.common.Response\"\x00\x12I\n\x17\x43reateAudienceInstagram\x12\x1a.statistic.AccessInstagram\x1a\x10.common.Response\"\x00\x12I\n\x12UploadBrandPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12M\n\x16UploadOpportunityImage\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12Q\n\x1aUploadOpportunityTreatment\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12L\n\x15UploadInterestPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12>\n\nLinkTikTok\x12\x1c.statistic.LinkTikTokRequest\x1a\x10.common.Response\"\x00\x12J\n\x10LinkTensorSocial\x12\".statistic.LinkTensorSocialRequest\x1a\x10.common.Response\"\x00\x12\x33\n\x0bReadCsvUser\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12M\n\x16UploadCoverListPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12?\n\x0fTalentUpdateOne\x12\x18.statistic.TalentProfile\x1a\x10.common.Response\"\x00\x12<\n\x0eResyncAllUsers\x12\x16.google.protobuf.Empty\x1a\x10.common.Response\"\x00\x12?\n\x11UploadTalentMedia\x12\x16.statistic.TalentMedia\x1a\x10.common.Response\"\x00\x12\x35\n\x07\x41\x64\x64Post\x12\x16.google.protobuf.Empty\x1a\x10.common.Response\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dopus_protobuf/statistic.proto\x12\tstatistic\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1aopus_protobuf/common.proto\x1a\x17opus_protobuf/web.proto\"e\n\x14UploadPictureRequest\x12\x13\n\x06userId\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\n\n\x02id\x18\x02 \x01(\t\x12!\n\x07picture\x18\x03 \x01(\x0b\x32\x10.common.DocumentB\t\n\x07_userId\"\x1b\n\x0b\x44\x61taRequest\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"\x82\x01\n\x0f\x41\x63\x63\x65ssInstagram\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\x0f\n\x02id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\x04user\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x03url\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x05 \x01(\tB\x05\n\x03_idB\x07\n\x05_userB\x06\n\x04_url\"_\n\x1bInstagramControllerResponse\x12-\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x1f.statistic.InstagramApiResponse\x12\x11\n\thave_mean\x18\x02 \x01(\x08\"[\n\x14InstagramApiResponse\x12\r\n\x05value\x18\x01 \x01(\x05\x12\x10\n\x08metadata\x18\x02 \x01(\t\x12\x15\n\x08\x65nd_time\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_end_time\"b\n\x18GetInstagramLikesRequest\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x1a.statistic.AccessInstagram\x12\x12\n\x05\x62roke\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_broke\"!\n\x11LinkTikTokRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xce\x01\n\x17LinkTensorSocialRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x11\n\tlast_name\x18\x04 \x01(\t\x12\x0e\n\x06tenant\x18\x05 \x01(\t\x12\x10\n\x08industry\x18\x06 \x01(\t\x12\x18\n\x10industry_segment\x18\x07 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x08 \x01(\t\x12\x10\n\x08\x62irthday\x18\t \x01(\t\x12\x0c\n\x04\x63ity\x18\n \x01(\t\"\x8c\x01\n\rTalentProfile\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x02 \x01(\t\x12\x0e\n\x06tenant\x18\x03 \x01(\t\x12\x10\n\x08industry\x18\x04 \x01(\t\x12\x10\n\x08\x62irthday\x18\x05 \x01(\t\x12\x18\n\x10industry_segment\x18\x06 \x01(\t\x12\x0e\n\x06gender\x18\x07 \x01(\t\"\xad\x01\n\x0bTalentMedia\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\x04user\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\x05title\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x11\n\x04link\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x12\n\x05order\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x1e\n\x04\x66ile\x18\x06 \x01(\x0b\x32\x10.common.DocumentB\x07\n\x05_userB\x08\n\x06_titleB\x07\n\x05_linkB\x08\n\x06_order2\x84\x11\n\x13StatisticController\x12\x37\n\x0bHealthCheck\x12\x16.google.protobuf.Empty\x1a\x0e.common.Health\"\x00\x12G\n\x10uploadSkuPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12>\n\x13UserConnectAyrshare\x12\x13.common.GetItemByID\x1a\x10.common.Response\"\x00\x12>\n\x10GetInstagramInfo\x12\x16.statistic.DataRequest\x1a\x10.common.Response\"\x00\x12]\n\x15GetInstagramFollowers\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12[\n\x13GetInstagramFollows\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x1aGetInstagramAudienceGender\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12`\n\x18GetInstagramAudienceCity\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x63\n\x1bGetInstagramAudienceCountry\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12Y\n\x11GetInstagramReach\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12`\n\x18GetInstagramInteractions\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x11GetInstagramLikes\x12#.statistic.GetInstagramLikesRequest\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x62\n\x1aGetInstagramEngagementRate\x12\x1a.statistic.AccessInstagram\x1a&.statistic.InstagramControllerResponse\"\x00\x12\x41\n\x13UpdateSocialNetwork\x12\x16.statistic.DataRequest\x1a\x10.common.Response\"\x00\x12I\n\x17\x43reateAudienceInstagram\x12\x1a.statistic.AccessInstagram\x1a\x10.common.Response\"\x00\x12I\n\x12UploadBrandPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12M\n\x16UploadOpportunityImage\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12Q\n\x1aUploadOpportunityTreatment\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12L\n\x15UploadInterestPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12>\n\nLinkTikTok\x12\x1c.statistic.LinkTikTokRequest\x1a\x10.common.Response\"\x00\x12J\n\x10LinkTensorSocial\x12\".statistic.LinkTensorSocialRequest\x1a\x10.common.Response\"\x00\x12\x33\n\x0bReadCsvUser\x12\x10.common.Document\x1a\x10.common.Response\"\x00\x12M\n\x16UploadCoverListPicture\x12\x1f.statistic.UploadPictureRequest\x1a\x10.common.Response\"\x00\x12?\n\x0fTalentUpdateOne\x12\x18.statistic.TalentProfile\x1a\x10.common.Response\"\x00\x12<\n\x0eResyncAllUsers\x12\x16.google.protobuf.Empty\x1a\x10.common.Response\"\x00\x12?\n\x11UploadTalentMedia\x12\x16.statistic.TalentMedia\x1a\x10.common.Response\"\x00\x12\x35\n\x07\x41\x64\x64Post\x12\x16.google.protobuf.Empty\x1a\x10.common.Response\"\x00\x12/\n\x0eLinkUserTensor\x12\t.web.User\x1a\x10.common.Response\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'opus_protobuf.statistic_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_UPLOADPICTUREREQUEST']._serialized_start=101
-  _globals['_UPLOADPICTUREREQUEST']._serialized_end=202
-  _globals['_DATAREQUEST']._serialized_start=204
-  _globals['_DATAREQUEST']._serialized_end=231
-  _globals['_ACCESSINSTAGRAM']._serialized_start=234
-  _globals['_ACCESSINSTAGRAM']._serialized_end=364
-  _globals['_INSTAGRAMCONTROLLERRESPONSE']._serialized_start=366
-  _globals['_INSTAGRAMCONTROLLERRESPONSE']._serialized_end=461
-  _globals['_INSTAGRAMAPIRESPONSE']._serialized_start=463
-  _globals['_INSTAGRAMAPIRESPONSE']._serialized_end=554
-  _globals['_GETINSTAGRAMLIKESREQUEST']._serialized_start=556
-  _globals['_GETINSTAGRAMLIKESREQUEST']._serialized_end=654
-  _globals['_LINKTIKTOKREQUEST']._serialized_start=656
-  _globals['_LINKTIKTOKREQUEST']._serialized_end=689
-  _globals['_LINKTENSORSOCIALREQUEST']._serialized_start=692
-  _globals['_LINKTENSORSOCIALREQUEST']._serialized_end=898
-  _globals['_TALENTPROFILE']._serialized_start=901
-  _globals['_TALENTPROFILE']._serialized_end=1041
-  _globals['_TALENTMEDIA']._serialized_start=1044
-  _globals['_TALENTMEDIA']._serialized_end=1217
-  _globals['_STATISTICCONTROLLER']._serialized_start=1220
-  _globals['_STATISTICCONTROLLER']._serialized_end=3351
+  _globals['_UPLOADPICTUREREQUEST']._serialized_start=126
+  _globals['_UPLOADPICTUREREQUEST']._serialized_end=227
+  _globals['_DATAREQUEST']._serialized_start=229
+  _globals['_DATAREQUEST']._serialized_end=256
+  _globals['_ACCESSINSTAGRAM']._serialized_start=259
+  _globals['_ACCESSINSTAGRAM']._serialized_end=389
+  _globals['_INSTAGRAMCONTROLLERRESPONSE']._serialized_start=391
+  _globals['_INSTAGRAMCONTROLLERRESPONSE']._serialized_end=486
+  _globals['_INSTAGRAMAPIRESPONSE']._serialized_start=488
+  _globals['_INSTAGRAMAPIRESPONSE']._serialized_end=579
+  _globals['_GETINSTAGRAMLIKESREQUEST']._serialized_start=581
+  _globals['_GETINSTAGRAMLIKESREQUEST']._serialized_end=679
+  _globals['_LINKTIKTOKREQUEST']._serialized_start=681
+  _globals['_LINKTIKTOKREQUEST']._serialized_end=714
+  _globals['_LINKTENSORSOCIALREQUEST']._serialized_start=717
+  _globals['_LINKTENSORSOCIALREQUEST']._serialized_end=923
+  _globals['_TALENTPROFILE']._serialized_start=926
+  _globals['_TALENTPROFILE']._serialized_end=1066
+  _globals['_TALENTMEDIA']._serialized_start=1069
+  _globals['_TALENTMEDIA']._serialized_end=1242
+  _globals['_STATISTICCONTROLLER']._serialized_start=1245
+  _globals['_STATISTICCONTROLLER']._serialized_end=3425
 # @@protoc_insertion_point(module_scope)
```

### Comparing `opus_protobuf-1.0.56/opus_protobuf/statistic_pb2.pyi` & `opus_protobuf-1.0.57/opus_protobuf/statistic_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from google.protobuf import empty_pb2 as _empty_pb2
 from opus_protobuf import common_pb2 as _common_pb2
+from opus_protobuf import web_pb2 as _web_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
```

### Comparing `opus_protobuf-1.0.56/opus_protobuf/statistic_pb2_grpc.py` & `opus_protobuf-1.0.57/opus_protobuf/statistic_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from opus_protobuf import common_pb2 as opus__protobuf_dot_common__pb2
 from opus_protobuf import statistic_pb2 as opus__protobuf_dot_statistic__pb2
+from opus_protobuf import web_pb2 as opus__protobuf_dot_web__pb2
 
 
 class StatisticControllerStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
@@ -147,14 +148,19 @@
                 response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
                 )
         self.AddPost = channel.unary_unary(
                 '/statistic.StatisticController/AddPost',
                 request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                 response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
                 )
+        self.LinkUserTensor = channel.unary_unary(
+                '/statistic.StatisticController/LinkUserTensor',
+                request_serializer=opus__protobuf_dot_web__pb2.User.SerializeToString,
+                response_deserializer=opus__protobuf_dot_common__pb2.Response.FromString,
+                )
 
 
 class StatisticControllerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def HealthCheck(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -314,14 +320,20 @@
 
     def AddPost(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def LinkUserTensor(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_StatisticControllerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'HealthCheck': grpc.unary_unary_rpc_method_handler(
                     servicer.HealthCheck,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=opus__protobuf_dot_common__pb2.Health.SerializeToString,
@@ -452,14 +464,19 @@
                     response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
             ),
             'AddPost': grpc.unary_unary_rpc_method_handler(
                     servicer.AddPost,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
             ),
+            'LinkUserTensor': grpc.unary_unary_rpc_method_handler(
+                    servicer.LinkUserTensor,
+                    request_deserializer=opus__protobuf_dot_web__pb2.User.FromString,
+                    response_serializer=opus__protobuf_dot_common__pb2.Response.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'statistic.StatisticController', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -920,7 +937,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/statistic.StatisticController/AddPost',
             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             opus__protobuf_dot_common__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def LinkUserTensor(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/statistic.StatisticController/LinkUserTensor',
+            opus__protobuf_dot_web__pb2.User.SerializeToString,
+            opus__protobuf_dot_common__pb2.Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `opus_protobuf-1.0.56/opus_protobuf/user_pb2.py` & `opus_protobuf-1.0.57/opus_protobuf/user_pb2.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/user_pb2.pyi` & `opus_protobuf-1.0.57/opus_protobuf/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/user_pb2_grpc.py` & `opus_protobuf-1.0.57/opus_protobuf/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/web_pb2.py` & `opus_protobuf-1.0.57/opus_protobuf/web_pb2.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/web_pb2.pyi` & `opus_protobuf-1.0.57/opus_protobuf/web_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/opus_protobuf/web_pb2_grpc.py` & `opus_protobuf-1.0.57/opus_protobuf/web_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opus_protobuf-1.0.56/setup.py` & `opus_protobuf-1.0.57/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'opus_protobuf',         # How you named your package folder (MyLib)
   packages = ['opus_protobuf'],   # Chose the same as "name"
-  version = '1.0.56',      # Start with a small number and increase it with every change you make
+  version = '1.0.57',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'YOUR NAME',                   # Type in your name
   author_email = 'your.email@domain.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
```

