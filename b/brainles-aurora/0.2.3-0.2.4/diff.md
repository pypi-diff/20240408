# Comparing `tmp/brainles_aurora-0.2.3-py3-none-any.whl.zip` & `tmp/brainles_aurora-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 28828 bytes, number of entries: 17
+Zip file size: 28848 bytes, number of entries: 17
 -rw-r--r--  2.0 unx     1799 b- defN 80-Jan-01 00:00 brainles_aurora/.gitignore
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 brainles_aurora/__init__.py
 -rw-r--r--  2.0 unx       87 b- defN 80-Jan-01 00:00 brainles_aurora/inferer/__init__.py
 -rw-r--r--  2.0 unx     1360 b- defN 80-Jan-01 00:00 brainles_aurora/inferer/config.py
 -rw-r--r--  2.0 unx     2627 b- defN 80-Jan-01 00:00 brainles_aurora/inferer/constants.py
 -rw-r--r--  2.0 unx    10383 b- defN 80-Jan-01 00:00 brainles_aurora/inferer/data.py
 -rw-r--r--  2.0 unx     9471 b- defN 80-Jan-01 00:00 brainles_aurora/inferer/inferer.py
 -rw-r--r--  2.0 unx      615 b- defN 80-Jan-01 00:00 brainles_aurora/inferer/log_config.json
 -rw-r--r--  2.0 unx     8635 b- defN 80-Jan-01 00:00 brainles_aurora/inferer/model.py
 -rw-r--r--  2.0 unx       85 b- defN 80-Jan-01 00:00 brainles_aurora/utils/__init__.py
--rw-r--r--  2.0 unx      612 b- defN 80-Jan-01 00:00 brainles_aurora/utils/console_decorators.py
+-rw-r--r--  2.0 unx      657 b- defN 80-Jan-01 00:00 brainles_aurora/utils/console_decorators.py
 -rw-r--r--  2.0 unx     1291 b- defN 80-Jan-01 00:00 brainles_aurora/utils/download.py
 -rw-r--r--  2.0 unx      401 b- defN 80-Jan-01 00:00 brainles_aurora/utils/utils.py
--rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 brainles_aurora-0.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4414 b- defN 80-Jan-01 00:00 brainles_aurora-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brainles_aurora-0.2.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1491 b- defN 16-Jan-01 00:00 brainles_aurora-0.2.3.dist-info/RECORD
-17 files, 77882 bytes uncompressed, 26342 bytes compressed:  66.2%
+-rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 brainles_aurora-0.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4414 b- defN 80-Jan-01 00:00 brainles_aurora-0.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brainles_aurora-0.2.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1491 b- defN 16-Jan-01 00:00 brainles_aurora-0.2.4.dist-info/RECORD
+17 files, 77927 bytes uncompressed, 26362 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: brainles_aurora/utils/download.py
 Comment: 
 
 Filename: brainles_aurora/utils/utils.py
 Comment: 
 
-Filename: brainles_aurora-0.2.3.dist-info/LICENSE
+Filename: brainles_aurora-0.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: brainles_aurora-0.2.3.dist-info/METADATA
+Filename: brainles_aurora-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: brainles_aurora-0.2.3.dist-info/WHEEL
+Filename: brainles_aurora-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: brainles_aurora-0.2.3.dist-info/RECORD
+Filename: brainles_aurora-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## brainles_aurora/utils/console_decorators.py

```diff
@@ -1,13 +1,15 @@
+from functools import wraps
 from rich.console import Console
 
 CITATION_LINK = "https://github.com/BrainLesion/AURORA#citation"
 
 
 def citation_reminder(func):
+    @wraps(func)
     def wrapper(*args, **kwargs):
         console = Console()
         console.rule("Thank you for using [bold]AURORA[/bold]")
         console.print(
             f"Please support our development by citing the papers listed here:",
             justify="center",
         )
```

## Comparing `brainles_aurora-0.2.3.dist-info/LICENSE` & `brainles_aurora-0.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `brainles_aurora-0.2.3.dist-info/METADATA` & `brainles_aurora-0.2.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainles_aurora
-Version: 0.2.3
+Version: 0.2.4
 Summary: Segmentation models for cancer metastasis in brain MR.
 Home-page: https://github.com/BrainLesion/AURORA
 License: AGPL-3.0
 Author: Florian Kofler
 Author-email: florian.kofler@tum.de
 Maintainer: Florian Kofler
 Maintainer-email: florian.kofler@tum.de
```

## Comparing `brainles_aurora-0.2.3.dist-info/RECORD` & `brainles_aurora-0.2.4.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 brainles_aurora/inferer/config.py,sha256=Prbm3akYTsoI3z4WiEw4Z8DX5dtNAbCugpo5_-R9tNU,1360
 brainles_aurora/inferer/constants.py,sha256=oD0mU2aphC3eEZcgY39GRm5_IBrNgYndS7JyYc3ZYDE,2627
 brainles_aurora/inferer/data.py,sha256=B907tQ2_9MYrvq9XxWtBo8-gsvdbZ8dFFd2C_sp5oJU,10383
 brainles_aurora/inferer/inferer.py,sha256=Gvlo5-qyF6jYwqm7o89sFwllgF4FbdzVk95M-zTyP90,9471
 brainles_aurora/inferer/log_config.json,sha256=VjIEXQEAVVh32MqSHNK8UxmOh_SCpdiVn1s82WE2Zu8,615
 brainles_aurora/inferer/model.py,sha256=vw3tgQWvg878ugWRYjSH4q37CMhzQt_h9EMRaQss9BI,8635
 brainles_aurora/utils/__init__.py,sha256=7xxjIau-UTNATw2NUQNZzEREpO4s8JZyAv3u6kW6s0w,85
-brainles_aurora/utils/console_decorators.py,sha256=BhvfDon43XWBdLLMXcD4il__hKldn1HZrBDydStFDsc,612
+brainles_aurora/utils/console_decorators.py,sha256=81nHI60qtVe0_owstvAS-B9STIXIxiw8BkeyzJbpT8Q,657
 brainles_aurora/utils/download.py,sha256=a5Hm2SS19PxcvIpmbp6BInfySp768CxLoftmqGQbqAc,1291
 brainles_aurora/utils/utils.py,sha256=P6LnaOXImVpqTcg4y7PUVYRLWWbCDwlazkAWxxzz9dA,401
-brainles_aurora-0.2.3.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-brainles_aurora-0.2.3.dist-info/METADATA,sha256=U2kazZonLlzLgvUb4k1jznWeU3E9NMdMQ6rA-m2ZGuI,4414
-brainles_aurora-0.2.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-brainles_aurora-0.2.3.dist-info/RECORD,,
+brainles_aurora-0.2.4.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+brainles_aurora-0.2.4.dist-info/METADATA,sha256=BEqxexZpKYhGnrVNH2HvqGC525ArL-3pxLSoMpPf8Dc,4414
+brainles_aurora-0.2.4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+brainles_aurora-0.2.4.dist-info/RECORD,,
```

