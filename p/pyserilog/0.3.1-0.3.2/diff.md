# Comparing `tmp/pyserilog-0.3.1-py3-none-any.whl.zip` & `tmp/pyserilog-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 73881 bytes, number of entries: 118
+Zip file size: 73934 bytes, number of entries: 118
 -rw-rw-rw-  2.0 fat       97 b- defN 23-Mar-25 04:26 pyserilog/__init__.py
 -rw-rw-rw-  2.0 fat      194 b- defN 23-Mar-25 04:26 pyserilog/guard.py
 -rw-rw-rw-  2.0 fat     5466 b- defN 24-Apr-04 12:41 pyserilog/ilogger.py
 -rw-rw-rw-  2.0 fat     9312 b- defN 23-Mar-26 15:34 pyserilog/logger_configuration.py
 -rw-rw-rw-  2.0 fat      298 b- defN 23-Mar-25 04:26 pyserilog/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-25 04:26 pyserilog/capturing/__init__.py
 -rw-rw-rw-  2.0 fat     2211 b- defN 23-Mar-26 15:34 pyserilog/capturing/depth_limiter.py
@@ -107,14 +107,14 @@
 -rw-rw-rw-  2.0 fat     1642 b- defN 23-Mar-26 11:28 pyserilog/settings/key_value_paies/callable_configuration_method_finder.py
 -rw-rw-rw-  2.0 fat    13526 b- defN 23-Mar-26 15:34 pyserilog/settings/key_value_paies/key_value_pair_settings.py
 -rw-rw-rw-  2.0 fat     1652 b- defN 23-Mar-25 10:33 pyserilog/settings/key_value_paies/setting_value_conversions.py
 -rw-rw-rw-  2.0 fat     5630 b- defN 24-Apr-04 13:49 pyserilog/settings/key_value_paies/surrogate_configuration_methods.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-07 13:41 pyserilog/sinks/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-07 13:43 pyserilog/sinks/periodic_batching/__init__.py
 -rw-rw-rw-  2.0 fat     1644 b- defN 24-Apr-08 06:07 pyserilog/sinks/periodic_batching/failure_aware_batch_scheduler.py
--rw-rw-rw-  2.0 fat      822 b- defN 24-Apr-07 15:33 pyserilog/sinks/periodic_batching/options.py
+-rw-rw-rw-  2.0 fat     1156 b- defN 24-Apr-08 13:55 pyserilog/sinks/periodic_batching/options.py
 -rw-rw-rw-  2.0 fat     4875 b- defN 24-Apr-08 12:55 pyserilog/sinks/periodic_batching/periodic_batching_sink.py
--rw-rw-rw-  2.0 fat      594 b- defN 24-Apr-08 12:55 pyserilog-0.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 12:55 pyserilog-0.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-08 12:55 pyserilog-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    11352 b- defN 24-Apr-08 12:55 pyserilog-0.3.1.dist-info/RECORD
-118 files, 193179 bytes uncompressed, 55293 bytes compressed:  71.4%
+-rw-rw-rw-  2.0 fat      594 b- defN 24-Apr-08 13:55 pyserilog-0.3.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 13:55 pyserilog-0.3.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-08 13:55 pyserilog-0.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    11353 b- defN 24-Apr-08 13:55 pyserilog-0.3.2.dist-info/RECORD
+118 files, 193514 bytes uncompressed, 55346 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -336,20 +336,20 @@
 
 Filename: pyserilog/sinks/periodic_batching/options.py
 Comment: 
 
 Filename: pyserilog/sinks/periodic_batching/periodic_batching_sink.py
 Comment: 
 
-Filename: pyserilog-0.3.1.dist-info/METADATA
+Filename: pyserilog-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: pyserilog-0.3.1.dist-info/WHEEL
+Filename: pyserilog-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyserilog-0.3.1.dist-info/top_level.txt
+Filename: pyserilog-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyserilog-0.3.1.dist-info/RECORD
+Filename: pyserilog-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyserilog/sinks/periodic_batching/options.py

```diff
@@ -1,24 +1,28 @@
 from typing import Optional
 
 
 class PeriodicBatchingSinkOptions:
-    eagerly_emit_first_event: bool = True
-    """
-    Eagerly emit a batch containing the first received event, regardless of the target batch size or batching time.
-     This helps with perceived "liveness" when running/debugging applications interactively. The default is `True`.
-    """
+    def __init__(self, eagerly_emit_first_event: bool = True,
+                 batch_size_limit: int = 1000,
+                 period: float = 2,
+                 queue_limit: Optional[int] = 100000):
+        self.eagerly_emit_first_event: bool = eagerly_emit_first_event
+        """
+        Eagerly emit a batch containing the first received event, regardless of the target batch size or batching time.
+         This helps with perceived "liveness" when running/debugging applications interactively. The default is `True`.
+        """
 
-    batch_size_limit: int = 1000
-    """
-    The maximum number of events to include in a single batch. The default is `1000`.
-    """
+        self.batch_size_limit: int = batch_size_limit
+        """
+        The maximum number of events to include in a single batch. The default is `1000`.
+        """
 
-    period: float = 2
-    """
-    The maximum buffering delay between event batches. The default is `two` seconds.
-    """
+        self.period: float = period
+        """
+        The maximum buffering delay between event batches. The default is `two` seconds.
+        """
 
-    queue_limit: Optional[int] = 100000
-    """
-    Maximum number of events to hold in the sink's internal queue, or `null` for an unbounded queue. The default is `100000`.
-    """
+        self.queue_limit: Optional[int] = queue_limit
+        """
+        Maximum number of events to hold in the sink's internal queue, or `null` for an unbounded queue. The default is `100000`.
+        """
```

## Comparing `pyserilog-0.3.1.dist-info/METADATA` & `pyserilog-0.3.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyserilog
-Version: 0.3.1
+Version: 0.3.2
 Summary: python version of serilog a structured logging library
 Author: Reza Sadeghi
 Author-email: rezasadeghikhas@gmail.com
 License: Apache2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
```

## Comparing `pyserilog-0.3.1.dist-info/RECORD` & `pyserilog-0.3.2.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -106,13 +106,13 @@
 pyserilog/settings/key_value_paies/callable_configuration_method_finder.py,sha256=nVM5Vw-PL1-ZuE10Bh_Hx4vgKt3sGQBGQvKFreD3ee4,1642
 pyserilog/settings/key_value_paies/key_value_pair_settings.py,sha256=6HsKeOqYAw4biKQ1ftJxpGjEAVfA9WuPD5fF4KdxxAs,13526
 pyserilog/settings/key_value_paies/setting_value_conversions.py,sha256=VuL5eS3jbvRLsaSL1idEGvm3gCxQZOCvR6LuC7CL5EI,1652
 pyserilog/settings/key_value_paies/surrogate_configuration_methods.py,sha256=HkOe5rahROzt3596pq1sxh8HAhX9vAtzACVl29GokhI,5630
 pyserilog/sinks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyserilog/sinks/periodic_batching/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyserilog/sinks/periodic_batching/failure_aware_batch_scheduler.py,sha256=-4pQGfKjSm7bDfwBrXdr5Vgglj7cbv7Qh15PP-HvbmA,1644
-pyserilog/sinks/periodic_batching/options.py,sha256=_fjUNb8gqAQcnyEeUr4WJ1yg6zHBtayrIpJiTnCpHR0,822
+pyserilog/sinks/periodic_batching/options.py,sha256=OpSMbVznQ919vaP-wtmSZpzDwzrS89IpIHWohbfs6K4,1156
 pyserilog/sinks/periodic_batching/periodic_batching_sink.py,sha256=IPUmOr-p4QrPFS7JGZ0tgkR3qyJz7GD9VDYDsdl05H0,4875
-pyserilog-0.3.1.dist-info/METADATA,sha256=xY_XFytLiWWpZHGDYJUY1PmBdrfVb_gN6DvLXw8tvXk,594
-pyserilog-0.3.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-pyserilog-0.3.1.dist-info/top_level.txt,sha256=hPeO21itJn_SAW-X2aIdIo_cgIiyUrxcxrYpP7xQu88,10
-pyserilog-0.3.1.dist-info/RECORD,,
+pyserilog-0.3.2.dist-info/METADATA,sha256=OgaJD7Bo8tt_XEx-ge2pymKcaqjR5EphsqSo2dayrus,594
+pyserilog-0.3.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+pyserilog-0.3.2.dist-info/top_level.txt,sha256=hPeO21itJn_SAW-X2aIdIo_cgIiyUrxcxrYpP7xQu88,10
+pyserilog-0.3.2.dist-info/RECORD,,
```

