# Comparing `tmp/semanticsdp-0.1.0b6.tar.gz` & `tmp/semanticsdp-0.1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semanticsdp-0.1.0b6.tar", max compression
+gzip compressed data, was "semanticsdp-0.1.0b7.tar", max compression
```

## Comparing `semanticsdp-0.1.0b6.tar` & `semanticsdp-0.1.0b7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rwxr-xr-x   0        0        0     1064 2024-02-29 18:15:55.583279 semanticsdp-0.1.0b6/LICENSE
--rwxr-xr-x   0        0        0      104 2024-03-03 18:23:24.882601 semanticsdp-0.1.0b6/README.md
--rwxr-xr-x   0        0        0      354 2024-03-18 14:42:03.126519 semanticsdp-0.1.0b6/pyproject.toml
--rwxr-xr-x   0        0        0     1076 2024-02-29 17:57:17.013925 semanticsdp-0.1.0b6/semanticsdp/__init__.py
--rwxr-xr-x   0        0        0      324 2024-03-18 14:39:43.646557 semanticsdp-0.1.0b6/semanticsdp/_base.py
--rwxr-xr-x   0        0        0      117 2024-03-18 14:39:13.931524 semanticsdp-0.1.0b6/semanticsdp/_dataclass_fix.py
--rwxr-xr-x   0        0        0      410 2024-03-18 14:41:44.093397 semanticsdp-0.1.0b6/semanticsdp/candidate_info.py
--rwxr-xr-x   0        0        0     2235 2024-03-18 14:41:43.230583 semanticsdp-0.1.0b6/semanticsdp/codec_info.py
--rwxr-xr-x   0        0        0      291 2024-03-18 14:41:44.168968 semanticsdp-0.1.0b6/semanticsdp/crypto_info.py
--rwxr-xr-x   0        0        0      264 2024-03-18 14:41:43.941830 semanticsdp-0.1.0b6/semanticsdp/datachannel_info.py
--rwxr-xr-x   0        0        0      490 2024-02-29 17:52:52.438580 semanticsdp-0.1.0b6/semanticsdp/direction.py
--rwxr-xr-x   0        0        0      339 2024-02-29 17:52:52.509166 semanticsdp-0.1.0b6/semanticsdp/direction_way.py
--rwxr-xr-x   0        0        0      565 2024-03-18 14:41:43.872864 semanticsdp-0.1.0b6/semanticsdp/dtls_info.py
--rwxr-xr-x   0        0        0      460 2024-03-18 14:41:44.237125 semanticsdp-0.1.0b6/semanticsdp/ice_info.py
--rwxr-xr-x   0        0        0     5474 2024-03-18 14:43:58.147873 semanticsdp-0.1.0b6/semanticsdp/media_info.py
--rwxr-xr-x   0        0        0      925 2024-03-18 14:41:43.361248 semanticsdp-0.1.0b6/semanticsdp/rid_info.py
--rwxr-xr-x   0        0        0      674 2024-03-18 14:41:43.672600 semanticsdp-0.1.0b6/semanticsdp/rtcp_feedback_info.py
--rwxr-xr-x   0        0        0    21677 2024-03-18 14:41:42.905708 semanticsdp-0.1.0b6/semanticsdp/sdp_info.py
--rwxr-xr-x   0        0        0      552 2024-02-29 14:38:18.185577 semanticsdp-0.1.0b6/semanticsdp/setup.py
--rwxr-xr-x   0        0        0     1133 2024-03-18 14:41:44.374328 semanticsdp-0.1.0b6/semanticsdp/simulcast_info.py
--rwxr-xr-x   0        0        0      257 2024-03-18 14:41:44.312252 semanticsdp-0.1.0b6/semanticsdp/simulcast_stream_info.py
--rwxr-xr-x   0        0        0      597 2024-03-18 14:41:43.003732 semanticsdp-0.1.0b6/semanticsdp/source_group_info.py
--rwxr-xr-x   0        0        0      327 2024-03-18 14:41:43.464698 semanticsdp-0.1.0b6/semanticsdp/source_info.py
--rwxr-xr-x   0        0        0      739 2024-03-18 14:41:44.013137 semanticsdp-0.1.0b6/semanticsdp/stream_info.py
--rwxr-xr-x   0        0        0      974 2024-03-18 14:41:43.099634 semanticsdp-0.1.0b6/semanticsdp/track_encoding_info.py
--rwxr-xr-x   0        0        0     1510 2024-03-18 14:41:43.762987 semanticsdp-0.1.0b6/semanticsdp/track_info.py
--rwxr-xr-x   0        0        0      101 2024-03-01 10:13:28.649034 semanticsdp-0.1.0b6/semanticsdp/transform/__init__.py
--rwxr-xr-x   0        0        0    13325 2024-03-01 10:54:49.304989 semanticsdp-0.1.0b6/semanticsdp/transform/sdp_grammar.py
--rwxr-xr-x   0        0        0     2882 2024-03-12 16:01:10.245802 semanticsdp-0.1.0b6/semanticsdp/transform/sdp_parser.py
--rwxr-xr-x   0        0        0     2175 2024-03-12 16:01:10.074962 semanticsdp-0.1.0b6/semanticsdp/transform/sdp_writer.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 semanticsdp-0.1.0b6/PKG-INFO
+-rwxr-xr-x   0        0        0     1064 2024-02-29 18:15:55.583279 semanticsdp-0.1.0b7/LICENSE
+-rwxr-xr-x   0        0        0      104 2024-03-03 18:23:24.882601 semanticsdp-0.1.0b7/README.md
+-rwxr-xr-x   0        0        0      354 2024-04-08 16:30:51.830709 semanticsdp-0.1.0b7/pyproject.toml
+-rwxr-xr-x   0        0        0     1076 2024-02-29 17:57:17.013925 semanticsdp-0.1.0b7/semanticsdp/__init__.py
+-rwxr-xr-x   0        0        0      324 2024-03-18 14:39:43.646557 semanticsdp-0.1.0b7/semanticsdp/_base.py
+-rwxr-xr-x   0        0        0      117 2024-03-18 14:39:13.931524 semanticsdp-0.1.0b7/semanticsdp/_dataclass_fix.py
+-rwxr-xr-x   0        0        0      410 2024-03-18 14:41:44.093397 semanticsdp-0.1.0b7/semanticsdp/candidate_info.py
+-rwxr-xr-x   0        0        0     2235 2024-03-18 14:41:43.230583 semanticsdp-0.1.0b7/semanticsdp/codec_info.py
+-rwxr-xr-x   0        0        0      291 2024-03-18 14:41:44.168968 semanticsdp-0.1.0b7/semanticsdp/crypto_info.py
+-rwxr-xr-x   0        0        0      264 2024-03-18 14:41:43.941830 semanticsdp-0.1.0b7/semanticsdp/datachannel_info.py
+-rwxr-xr-x   0        0        0      490 2024-02-29 17:52:52.438580 semanticsdp-0.1.0b7/semanticsdp/direction.py
+-rwxr-xr-x   0        0        0      339 2024-02-29 17:52:52.509166 semanticsdp-0.1.0b7/semanticsdp/direction_way.py
+-rwxr-xr-x   0        0        0      565 2024-03-18 14:41:43.872864 semanticsdp-0.1.0b7/semanticsdp/dtls_info.py
+-rwxr-xr-x   0        0        0      460 2024-03-18 14:41:44.237125 semanticsdp-0.1.0b7/semanticsdp/ice_info.py
+-rwxr-xr-x   0        0        0     5474 2024-03-18 14:43:58.147873 semanticsdp-0.1.0b7/semanticsdp/media_info.py
+-rwxr-xr-x   0        0        0      925 2024-03-18 14:41:43.361248 semanticsdp-0.1.0b7/semanticsdp/rid_info.py
+-rwxr-xr-x   0        0        0      674 2024-03-18 14:41:43.672600 semanticsdp-0.1.0b7/semanticsdp/rtcp_feedback_info.py
+-rwxr-xr-x   0        0        0    21675 2024-04-08 16:30:26.728835 semanticsdp-0.1.0b7/semanticsdp/sdp_info.py
+-rwxr-xr-x   0        0        0      552 2024-02-29 14:38:18.185577 semanticsdp-0.1.0b7/semanticsdp/setup.py
+-rwxr-xr-x   0        0        0     1133 2024-03-18 14:41:44.374328 semanticsdp-0.1.0b7/semanticsdp/simulcast_info.py
+-rwxr-xr-x   0        0        0      257 2024-03-18 14:41:44.312252 semanticsdp-0.1.0b7/semanticsdp/simulcast_stream_info.py
+-rwxr-xr-x   0        0        0      597 2024-03-18 14:41:43.003732 semanticsdp-0.1.0b7/semanticsdp/source_group_info.py
+-rwxr-xr-x   0        0        0      327 2024-03-18 14:41:43.464698 semanticsdp-0.1.0b7/semanticsdp/source_info.py
+-rwxr-xr-x   0        0        0      739 2024-03-18 14:41:44.013137 semanticsdp-0.1.0b7/semanticsdp/stream_info.py
+-rwxr-xr-x   0        0        0      974 2024-03-18 14:41:43.099634 semanticsdp-0.1.0b7/semanticsdp/track_encoding_info.py
+-rwxr-xr-x   0        0        0     1510 2024-03-18 14:41:43.762987 semanticsdp-0.1.0b7/semanticsdp/track_info.py
+-rwxr-xr-x   0        0        0      101 2024-03-01 10:13:28.649034 semanticsdp-0.1.0b7/semanticsdp/transform/__init__.py
+-rwxr-xr-x   0        0        0    13325 2024-03-01 10:54:49.304989 semanticsdp-0.1.0b7/semanticsdp/transform/sdp_grammar.py
+-rwxr-xr-x   0        0        0     2882 2024-03-12 16:01:10.245802 semanticsdp-0.1.0b7/semanticsdp/transform/sdp_parser.py
+-rwxr-xr-x   0        0        0     2175 2024-03-12 16:01:10.074962 semanticsdp-0.1.0b7/semanticsdp/transform/sdp_writer.py
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 semanticsdp-0.1.0b7/PKG-INFO
```

### Comparing `semanticsdp-0.1.0b6/LICENSE` & `semanticsdp-0.1.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/__init__.py` & `semanticsdp-0.1.0b7/semanticsdp/__init__.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/codec_info.py` & `semanticsdp-0.1.0b7/semanticsdp/codec_info.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/dtls_info.py` & `semanticsdp-0.1.0b7/semanticsdp/dtls_info.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/media_info.py` & `semanticsdp-0.1.0b7/semanticsdp/media_info.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/rid_info.py` & `semanticsdp-0.1.0b7/semanticsdp/rid_info.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/rtcp_feedback_info.py` & `semanticsdp-0.1.0b7/semanticsdp/rtcp_feedback_info.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/sdp_info.py` & `semanticsdp-0.1.0b7/semanticsdp/sdp_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,15 +447,15 @@
 
             for ssrc in media.get("ssrcs", {}):
                 if not (source := sources.get(ssrc["id"])):
                     sources[ssrc["id"]] = (source := SourceInfo(ssrc["id"]))
 
                 if ssrc["attribute"].lower() == "cname":
                     source.cname = ssrc["value"]
-                elif ssrc["attribute"].lower() != "msid":
+                if ssrc["attribute"].lower() != "msid":
                     continue
 
                 source.stream_id, source.track_id = ssrc["value"].split(" ")
                 if not (stream := sdpInfo.streams.get(source.stream_id)):
                     stream = StreamInfo(source.stream_id)
                     sdpInfo.streams[source.stream_id] = stream
```

### Comparing `semanticsdp-0.1.0b6/semanticsdp/setup.py` & `semanticsdp-0.1.0b7/semanticsdp/setup.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/simulcast_info.py` & `semanticsdp-0.1.0b7/semanticsdp/simulcast_info.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/source_group_info.py` & `semanticsdp-0.1.0b7/semanticsdp/source_group_info.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/stream_info.py` & `semanticsdp-0.1.0b7/semanticsdp/stream_info.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/track_encoding_info.py` & `semanticsdp-0.1.0b7/semanticsdp/track_encoding_info.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/track_info.py` & `semanticsdp-0.1.0b7/semanticsdp/track_info.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/transform/sdp_grammar.py` & `semanticsdp-0.1.0b7/semanticsdp/transform/sdp_grammar.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/transform/sdp_parser.py` & `semanticsdp-0.1.0b7/semanticsdp/transform/sdp_parser.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/semanticsdp/transform/sdp_writer.py` & `semanticsdp-0.1.0b7/semanticsdp/transform/sdp_writer.py`

 * *Files identical despite different names*

### Comparing `semanticsdp-0.1.0b6/PKG-INFO` & `semanticsdp-0.1.0b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semanticsdp
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: Python port of medooze/semantic-sdp-js
 Author: RuslanUC
 Author-email: dev_ruslan_uc@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

