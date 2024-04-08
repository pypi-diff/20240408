# Comparing `tmp/pyserilog-0.2.0a4-py3-none-any.whl.zip` & `tmp/pyserilog-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 70586 bytes, number of entries: 113
+Zip file size: 73893 bytes, number of entries: 118
 -rw-rw-rw-  2.0 fat       97 b- defN 23-Mar-25 04:26 pyserilog/__init__.py
 -rw-rw-rw-  2.0 fat      194 b- defN 23-Mar-25 04:26 pyserilog/guard.py
 -rw-rw-rw-  2.0 fat     5466 b- defN 24-Apr-04 12:41 pyserilog/ilogger.py
 -rw-rw-rw-  2.0 fat     9312 b- defN 23-Mar-26 15:34 pyserilog/logger_configuration.py
 -rw-rw-rw-  2.0 fat      298 b- defN 23-Mar-25 04:26 pyserilog/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-25 04:26 pyserilog/capturing/__init__.py
 -rw-rw-rw-  2.0 fat     2211 b- defN 23-Mar-26 15:34 pyserilog/capturing/depth_limiter.py
@@ -19,15 +19,15 @@
 -rw-rw-rw-  2.0 fat     3621 b- defN 23-Mar-25 04:26 pyserilog/configuration/logger_minimum_level_configuration.py
 -rw-rw-rw-  2.0 fat     1175 b- defN 23-Mar-25 11:29 pyserilog/configuration/logger_settings_configuration.py
 -rw-rw-rw-  2.0 fat     5520 b- defN 23-Mar-26 15:34 pyserilog/configuration/logger_sink_configuration.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-04 12:56 pyserilog/context/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Apr-04 13:02 pyserilog/context/log_context.py
 -rw-rw-rw-  2.0 fat      423 b- defN 24-Apr-04 13:02 pyserilog/context/log_context_enricher.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-25 04:26 pyserilog/core/__init__.py
--rw-rw-rw-  2.0 fat       70 b- defN 23-Mar-25 04:26 pyserilog/core/constants.py
+-rw-rw-rw-  2.0 fat       71 b- defN 24-Apr-08 06:23 pyserilog/core/constants.py
 -rw-rw-rw-  2.0 fat      435 b- defN 23-Mar-26 07:21 pyserilog/core/idestructuring_policy.py
 -rw-rw-rw-  2.0 fat      329 b- defN 23-Mar-26 07:21 pyserilog/core/ilog_event_enricher.py
 -rw-rw-rw-  2.0 fat      534 b- defN 23-Mar-26 10:16 pyserilog/core/ilog_event_filter.py
 -rw-rw-rw-  2.0 fat      733 b- defN 23-Mar-25 04:26 pyserilog/core/ilog_event_property_factory.py
 -rw-rw-rw-  2.0 fat      305 b- defN 23-Mar-25 04:26 pyserilog/core/ilog_event_property_value_factory.py
 -rw-rw-rw-  2.0 fat      198 b- defN 23-Mar-26 07:23 pyserilog/core/ilog_event_sink.py
 -rw-rw-rw-  2.0 fat      228 b- defN 23-Mar-25 04:26 pyserilog/core/imessage_template_parser.py
@@ -104,12 +104,17 @@
 -rw-rw-rw-  2.0 fat      674 b- defN 23-Mar-27 16:33 pyserilog/rendering/padding.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-04 13:26 pyserilog/settings/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-04 13:26 pyserilog/settings/key_value_paies/__init__.py
 -rw-rw-rw-  2.0 fat     1642 b- defN 23-Mar-26 11:28 pyserilog/settings/key_value_paies/callable_configuration_method_finder.py
 -rw-rw-rw-  2.0 fat    13526 b- defN 23-Mar-26 15:34 pyserilog/settings/key_value_paies/key_value_pair_settings.py
 -rw-rw-rw-  2.0 fat     1652 b- defN 23-Mar-25 10:33 pyserilog/settings/key_value_paies/setting_value_conversions.py
 -rw-rw-rw-  2.0 fat     5630 b- defN 24-Apr-04 13:49 pyserilog/settings/key_value_paies/surrogate_configuration_methods.py
--rw-rw-rw-  2.0 fat      628 b- defN 24-Apr-04 13:50 pyserilog-0.2.0a4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-04 13:50 pyserilog-0.2.0a4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-04 13:50 pyserilog-0.2.0a4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    10841 b- defN 24-Apr-04 13:50 pyserilog-0.2.0a4.dist-info/RECORD
-113 files, 185360 bytes uncompressed, 52844 bytes compressed:  71.5%
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-07 13:41 pyserilog/sinks/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-07 13:43 pyserilog/sinks/periodic_batching/__init__.py
+-rw-rw-rw-  2.0 fat     1644 b- defN 24-Apr-08 06:07 pyserilog/sinks/periodic_batching/failure_aware_batch_scheduler.py
+-rw-rw-rw-  2.0 fat      822 b- defN 24-Apr-07 15:33 pyserilog/sinks/periodic_batching/options.py
+-rw-rw-rw-  2.0 fat     5069 b- defN 24-Apr-08 05:40 pyserilog/sinks/periodic_batching/periodic_batching_sink.py
+-rw-rw-rw-  2.0 fat      594 b- defN 24-Apr-08 06:24 pyserilog-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 06:24 pyserilog-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-08 06:24 pyserilog-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    11352 b- defN 24-Apr-08 06:24 pyserilog-0.3.0.dist-info/RECORD
+118 files, 193373 bytes uncompressed, 55305 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -321,20 +321,35 @@
 
 Filename: pyserilog/settings/key_value_paies/setting_value_conversions.py
 Comment: 
 
 Filename: pyserilog/settings/key_value_paies/surrogate_configuration_methods.py
 Comment: 
 
-Filename: pyserilog-0.2.0a4.dist-info/METADATA
+Filename: pyserilog/sinks/__init__.py
 Comment: 
 
-Filename: pyserilog-0.2.0a4.dist-info/WHEEL
+Filename: pyserilog/sinks/periodic_batching/__init__.py
 Comment: 
 
-Filename: pyserilog-0.2.0a4.dist-info/top_level.txt
+Filename: pyserilog/sinks/periodic_batching/failure_aware_batch_scheduler.py
 Comment: 
 
-Filename: pyserilog-0.2.0a4.dist-info/RECORD
+Filename: pyserilog/sinks/periodic_batching/options.py
+Comment: 
+
+Filename: pyserilog/sinks/periodic_batching/periodic_batching_sink.py
+Comment: 
+
+Filename: pyserilog-0.3.0.dist-info/METADATA
+Comment: 
+
+Filename: pyserilog-0.3.0.dist-info/WHEEL
+Comment: 
+
+Filename: pyserilog-0.3.0.dist-info/top_level.txt
+Comment: 
+
+Filename: pyserilog-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyserilog/core/constants.py

```diff
@@ -1,2 +1,2 @@
 class Constants:
-    SOURCE_CONTEXT_PROPERTY_NAME = "SourceContext"
+    SOURCE_CONTEXT_PROPERTY_NAME = "source_context"
```

## Comparing `pyserilog-0.2.0a4.dist-info/RECORD` & `pyserilog-0.3.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 pyserilog/configuration/logger_minimum_level_configuration.py,sha256=ATXEZxxWIrHNEbhLiaEJiCswzE2ViD4fxme2U0c0Na8,3621
 pyserilog/configuration/logger_settings_configuration.py,sha256=ga1d627Aux4SZ3baWspuT9YOj3yatxYHV8aoPo5Thmg,1175
 pyserilog/configuration/logger_sink_configuration.py,sha256=zW--arx1AW-P-KmXQmxDrssW0XQRkpxXV0mHrYkT9rs,5520
 pyserilog/context/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyserilog/context/log_context.py,sha256=lCsBGRAnyi4GtmkNsr5U7FbuYkkVtKkII5nhW54pooE,27
 pyserilog/context/log_context_enricher.py,sha256=O-Zpl8Q5-05-nTml8vHgc_hr3h8fMrXN_sYCxyvchz0,423
 pyserilog/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pyserilog/core/constants.py,sha256=igmr52v5WrAUA_IKUsOCHdUgosmOM8KgdydFRqdV5is,70
+pyserilog/core/constants.py,sha256=UnemeY-GlbClJAtpzVBS9u972WsDF04XfgBf7mIwVvo,71
 pyserilog/core/idestructuring_policy.py,sha256=P-2of9oL7DZqmYs16AGbtrPhwibv4e3c75OF0l5HFVc,435
 pyserilog/core/ilog_event_enricher.py,sha256=FFOs47T6XDkDbrpZHHxSvvRnPp2tG-c2zbPWOKcGdvo,329
 pyserilog/core/ilog_event_filter.py,sha256=_JIsds01JV5QTny8yJjPXw5YUo6e7QtnE6l0nhphe5k,534
 pyserilog/core/ilog_event_property_factory.py,sha256=-0iVxS_MB5KgWQpamaqIBwuWUh7Z7uv-0lzvwRHcTCE,733
 pyserilog/core/ilog_event_property_value_factory.py,sha256=6nUSwQhQTDP0eviut0BcqGEJsY3KWiCO2w-Wos2OJVA,305
 pyserilog/core/ilog_event_sink.py,sha256=AdLuZJrpKrzpXSNnPEKXZQoElj5FGiNhCiX6ZzPZsf8,198
 pyserilog/core/imessage_template_parser.py,sha256=Es4WcE4xvZFBTPsYrWEtwkIwL2bcYAZsjQ_PSTeVWCg,228
@@ -103,11 +103,16 @@
 pyserilog/rendering/padding.py,sha256=T6rCLbmZC2P1BUhX5SEqN0nILXOf-Red-V2KVcCtKbI,674
 pyserilog/settings/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyserilog/settings/key_value_paies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyserilog/settings/key_value_paies/callable_configuration_method_finder.py,sha256=nVM5Vw-PL1-ZuE10Bh_Hx4vgKt3sGQBGQvKFreD3ee4,1642
 pyserilog/settings/key_value_paies/key_value_pair_settings.py,sha256=6HsKeOqYAw4biKQ1ftJxpGjEAVfA9WuPD5fF4KdxxAs,13526
 pyserilog/settings/key_value_paies/setting_value_conversions.py,sha256=VuL5eS3jbvRLsaSL1idEGvm3gCxQZOCvR6LuC7CL5EI,1652
 pyserilog/settings/key_value_paies/surrogate_configuration_methods.py,sha256=HkOe5rahROzt3596pq1sxh8HAhX9vAtzACVl29GokhI,5630
-pyserilog-0.2.0a4.dist-info/METADATA,sha256=lOnYf4Ypu3PAG551xLWRFj43rVCchd_WkBxzb_7LZGI,628
-pyserilog-0.2.0a4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyserilog-0.2.0a4.dist-info/top_level.txt,sha256=hPeO21itJn_SAW-X2aIdIo_cgIiyUrxcxrYpP7xQu88,10
-pyserilog-0.2.0a4.dist-info/RECORD,,
+pyserilog/sinks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+pyserilog/sinks/periodic_batching/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+pyserilog/sinks/periodic_batching/failure_aware_batch_scheduler.py,sha256=-4pQGfKjSm7bDfwBrXdr5Vgglj7cbv7Qh15PP-HvbmA,1644
+pyserilog/sinks/periodic_batching/options.py,sha256=_fjUNb8gqAQcnyEeUr4WJ1yg6zHBtayrIpJiTnCpHR0,822
+pyserilog/sinks/periodic_batching/periodic_batching_sink.py,sha256=VQSbRRBSJXv3-d05WjmkEeKYGakRktPVjIYMsgh2aVQ,5069
+pyserilog-0.3.0.dist-info/METADATA,sha256=b7D9h3mHpf7iYxfQV4y1pjxUIOvemGOzwElcusHsxYM,594
+pyserilog-0.3.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+pyserilog-0.3.0.dist-info/top_level.txt,sha256=hPeO21itJn_SAW-X2aIdIo_cgIiyUrxcxrYpP7xQu88,10
+pyserilog-0.3.0.dist-info/RECORD,,
```

