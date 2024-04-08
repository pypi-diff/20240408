# Comparing `tmp/kiwi_booster-0.3.6.tar.gz` & `tmp/kiwi_booster-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwi_booster-0.3.6.tar", max compression
+gzip compressed data, was "kiwi_booster-0.3.7.tar", max compression
```

## Comparing `kiwi_booster-0.3.6.tar` & `kiwi_booster-0.3.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-05-10 16:09:22.014857 kiwi_booster-0.3.6/LICENSE
--rw-r--r--   0        0        0     9196 2024-03-29 18:18:01.069091 kiwi_booster-0.3.6/README.md
--rw-r--r--   0        0        0        0 2023-05-14 15:53:32.721294 kiwi_booster-0.3.6/kiwi_booster/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 16:06:23.304697 kiwi_booster-0.3.6/kiwi_booster/common_utils/__init__.py
--rw-r--r--   0        0        0     1199 2024-03-01 18:03:31.363100 kiwi_booster-0.3.6/kiwi_booster/common_utils/geographic.py
--rw-r--r--   0        0        0      578 2024-03-01 18:03:31.363100 kiwi_booster-0.3.6/kiwi_booster/common_utils/json.py
--rw-r--r--   0        0        0     1748 2023-05-14 16:09:16.985180 kiwi_booster-0.3.6/kiwi_booster/common_utils/loggers.py
--rw-r--r--   0        0        0        0 2023-05-11 22:59:08.795321 kiwi_booster-0.3.6/kiwi_booster/common_utils/requests.py
--rw-r--r--   0        0        0     3444 2024-03-01 18:04:06.915726 kiwi_booster-0.3.6/kiwi_booster/common_utils/time.py
--rw-r--r--   0        0        0     1460 2024-03-17 01:39:10.338452 kiwi_booster-0.3.6/kiwi_booster/common_utils/video.py
--rw-r--r--   0        0        0     1794 2024-03-17 16:55:20.021796 kiwi_booster-0.3.6/kiwi_booster/decorators.py
--rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.3.6/kiwi_booster/gcp_utils/__init__.py
--rw-r--r--   0        0        0      569 2024-02-22 20:14:01.692745 kiwi_booster-0.3.6/kiwi_booster/gcp_utils/bigquery.py
--rw-r--r--   0        0        0     1312 2024-03-17 01:49:02.412758 kiwi_booster-0.3.6/kiwi_booster/gcp_utils/kfp.py
--rw-r--r--   0        0        0     2070 2024-02-23 17:29:39.403328 kiwi_booster-0.3.6/kiwi_booster/gcp_utils/secrets.py
--rw-r--r--   0        0        0     3995 2024-03-01 18:04:06.915726 kiwi_booster-0.3.6/kiwi_booster/gcp_utils/storage.py
--rw-r--r--   0        0        0        0 2024-03-01 18:03:31.363100 kiwi_booster-0.3.6/kiwi_booster/mcap_utils/__init__.py
--rw-r--r--   0        0        0    11694 2024-03-29 18:00:31.624861 kiwi_booster-0.3.6/kiwi_booster/mcap_utils/decode.py
--rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.3.6/kiwi_booster/ml_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 23:00:22.783840 kiwi_booster-0.3.6/kiwi_booster/ml_utils/benchmarks.py
--rw-r--r--   0        0        0        0 2023-05-11 23:00:10.175752 kiwi_booster-0.3.6/kiwi_booster/ml_utils/prediction.py
--rw-r--r--   0        0        0     4110 2024-03-01 18:03:31.363100 kiwi_booster-0.3.6/kiwi_booster/slack_utils.py
--rw-r--r--   0        0        0     2986 2024-03-29 18:21:02.960189 kiwi_booster-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    10607 1970-01-01 00:00:00.000000 kiwi_booster-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-10 16:09:22.014857 kiwi_booster-0.3.7/LICENSE
+-rw-r--r--   0        0        0     9196 2024-04-08 20:09:19.938677 kiwi_booster-0.3.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-14 15:53:32.721294 kiwi_booster-0.3.7/kiwi_booster/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 16:06:23.304697 kiwi_booster-0.3.7/kiwi_booster/common_utils/__init__.py
+-rw-r--r--   0        0        0     1199 2024-03-01 18:03:31.363100 kiwi_booster-0.3.7/kiwi_booster/common_utils/geographic.py
+-rw-r--r--   0        0        0      578 2024-03-01 18:03:31.363100 kiwi_booster-0.3.7/kiwi_booster/common_utils/json.py
+-rw-r--r--   0        0        0     1748 2023-05-14 16:09:16.985180 kiwi_booster-0.3.7/kiwi_booster/common_utils/loggers.py
+-rw-r--r--   0        0        0        0 2023-05-11 22:59:08.795321 kiwi_booster-0.3.7/kiwi_booster/common_utils/requests.py
+-rw-r--r--   0        0        0     3444 2024-03-01 18:04:06.915726 kiwi_booster-0.3.7/kiwi_booster/common_utils/time.py
+-rw-r--r--   0        0        0     3018 2024-04-08 20:09:58.331136 kiwi_booster-0.3.7/kiwi_booster/common_utils/video.py
+-rw-r--r--   0        0        0     1794 2024-04-08 20:09:19.942677 kiwi_booster-0.3.7/kiwi_booster/decorators.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.3.7/kiwi_booster/gcp_utils/__init__.py
+-rw-r--r--   0        0        0      569 2024-02-22 20:14:01.692745 kiwi_booster-0.3.7/kiwi_booster/gcp_utils/bigquery.py
+-rw-r--r--   0        0        0     1312 2024-04-08 20:09:19.942677 kiwi_booster-0.3.7/kiwi_booster/gcp_utils/kfp.py
+-rw-r--r--   0        0        0     2070 2024-02-23 17:29:39.403328 kiwi_booster-0.3.7/kiwi_booster/gcp_utils/secrets.py
+-rw-r--r--   0        0        0     3995 2024-03-01 18:04:06.915726 kiwi_booster-0.3.7/kiwi_booster/gcp_utils/storage.py
+-rw-r--r--   0        0        0        0 2024-03-01 18:03:31.363100 kiwi_booster-0.3.7/kiwi_booster/mcap_utils/__init__.py
+-rw-r--r--   0        0        0    11933 2024-04-08 20:09:19.942677 kiwi_booster-0.3.7/kiwi_booster/mcap_utils/decode.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.3.7/kiwi_booster/ml_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:00:22.783840 kiwi_booster-0.3.7/kiwi_booster/ml_utils/benchmarks.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:00:10.175752 kiwi_booster-0.3.7/kiwi_booster/ml_utils/prediction.py
+-rw-r--r--   0        0        0     4110 2024-03-01 18:03:31.363100 kiwi_booster-0.3.7/kiwi_booster/slack_utils.py
+-rw-r--r--   0        0        0     3116 2024-04-08 20:42:07.330728 kiwi_booster-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    10629 1970-01-01 00:00:00.000000 kiwi_booster-0.3.7/PKG-INFO
```

### Comparing `kiwi_booster-0.3.6/LICENSE` & `kiwi_booster-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/README.md` & `kiwi_booster-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/kiwi_booster/common_utils/geographic.py` & `kiwi_booster-0.3.7/kiwi_booster/common_utils/geographic.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/kiwi_booster/common_utils/json.py` & `kiwi_booster-0.3.7/kiwi_booster/common_utils/json.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/kiwi_booster/common_utils/loggers.py` & `kiwi_booster-0.3.7/kiwi_booster/common_utils/loggers.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/kiwi_booster/common_utils/time.py` & `kiwi_booster-0.3.7/kiwi_booster/common_utils/time.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/kiwi_booster/decorators.py` & `kiwi_booster-0.3.7/kiwi_booster/decorators.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/kiwi_booster/gcp_utils/bigquery.py` & `kiwi_booster-0.3.7/kiwi_booster/gcp_utils/bigquery.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/kiwi_booster/gcp_utils/kfp.py` & `kiwi_booster-0.3.7/kiwi_booster/gcp_utils/kfp.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/kiwi_booster/gcp_utils/secrets.py` & `kiwi_booster-0.3.7/kiwi_booster/gcp_utils/secrets.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/kiwi_booster/gcp_utils/storage.py` & `kiwi_booster-0.3.7/kiwi_booster/gcp_utils/storage.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/kiwi_booster/mcap_utils/decode.py` & `kiwi_booster-0.3.7/kiwi_booster/mcap_utils/decode.py`

 * *Files 3% similar despite different names*

```diff
@@ -285,23 +285,29 @@
                 "z": msg.twist.twist.angular.z,
             },
         },
         "covariance": msg.ros_msg.pose.covariance,
     }
 
 
-def decode_image_marker(msg: Any) -> Tuple[np.ndarray, np.ndarray, dict]:
+def decode_image_marker(msg: Any) -> Tuple[dict, dict, dict]:
     """
-    Decodes a visualization_msgs/msg/ImageMarker message into a tuple of the markers and some metadata.
+    Decodes a visualization_msgs/msg/ImageMarker message into a tuple of the markers and
+    some metadata.
 
     Args:
         msg (ImageMarker): The ImageMarker message to decode.
 
     Returns:
-        Tuple[np.ndarray, np.ndarray, dict]: The position, points as Numpy arrays and the following metadata:
+        Tuple[dict, dict, dict]: The position, points as dictionaries with the "x" and "y"
+        points and the following metadata:
+            - timestamp: The timestamp of the message as a datetime object.
+            - frame_id: The frame id of the message.
+            - type: The type of the message.
+            - action: The action of the message.
     """
 
     position = {
         "x": msg.position.x,
         "y": msg.position.y,
         # "z": msg.position.z, # z is always 0
     }
```

### Comparing `kiwi_booster-0.3.6/kiwi_booster/slack_utils.py` & `kiwi_booster-0.3.7/kiwi_booster/slack_utils.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.6/pyproject.toml` & `kiwi_booster-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kiwi-booster"
-version = "0.3.6"
+version = "0.3.7"
 description = "Python utility functions and classes for KiwiBot AI&Robotics team"
 authors = ["Sebastian Hernandez <juan.hernandez@kiwibot.con>"]
 readme = "README.md"
 packages = [{include = "kiwi_booster"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13.0"
@@ -25,16 +25,24 @@
 mcap-ros2-support = "^0.5.3"
 ipregistry = "^3.2.0"
 pillow = "^10.2.0"
 protobuf = "^3.20.0"
 kfp = "^2.4.0"
 python-path = "^0.1.3"
 
-[tool.poetry.group.dev.dependencies]
-slack-sdk = "^3.21.3"
+[tool.poetry.group.video]
+optional = true
+
+[tool.poetry.group.video.dependencies]
+opencv-python = "^4.9.0.80"
+moviepy = "^1.0.3"
+
+[tool.poetry.extras]
+video = ["opencv-python", "moviepy"]
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
```

### Comparing `kiwi_booster-0.3.6/PKG-INFO` & `kiwi_booster-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: kiwi-booster
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python utility functions and classes for KiwiBot AI&Robotics team
 Author: Sebastian Hernandez
 Author-email: juan.hernandez@kiwibot.con
 Requires-Python: >=3.8,<3.13.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: video
 Requires-Dist: google-auth (>=2.18.0,<3.0.0)
 Requires-Dist: google-cloud-bigquery (>=3.10.0,<4.0.0)
 Requires-Dist: google-cloud-secret-manager (>=2.16.1,<3.0.0)
 Requires-Dist: google-cloud-storage (>=2.9.0,<3.0.0)
 Requires-Dist: google-crc32c (>=1.5.0,<2.0.0)
 Requires-Dist: ipregistry (>=3.2.0,<4.0.0)
 Requires-Dist: kfp (>=2.4.0,<3.0.0)
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: kiwi-booster Version: 0.3.6 Summary: Python utility
+Metadata-Version: 2.1 Name: kiwi-booster Version: 0.3.7 Summary: Python utility
 functions and classes for KiwiBot AI&Robotics team Author: Sebastian Hernandez
 Author-email: juan.hernandez@kiwibot.con Requires-Python: >=3.8,<3.13.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: google-auth (>=2.18.0,<3.0.0) Requires-Dist: google-cloud-
-bigquery (>=3.10.0,<4.0.0) Requires-Dist: google-cloud-secret-manager
-(>=2.16.1,<3.0.0) Requires-Dist: google-cloud-storage (>=2.9.0,<3.0.0)
-Requires-Dist: google-crc32c (>=1.5.0,<2.0.0) Requires-Dist: ipregistry
-(>=3.2.0,<4.0.0) Requires-Dist: kfp (>=2.4.0,<3.0.0) Requires-Dist: mcap
-(>=1.1.1,<2.0.0) Requires-Dist: mcap-ros2-support (>=0.5.3,<0.6.0) Requires-
-Dist: numpy (>=1.19,<2.0) ; python_version < "3.9" Requires-Dist: numpy
-(>=1.23,<2.0) ; python_version >= "3.9" Requires-Dist: pillow
+Provides-Extra: video Requires-Dist: google-auth (>=2.18.0,<3.0.0) Requires-
+Dist: google-cloud-bigquery (>=3.10.0,<4.0.0) Requires-Dist: google-cloud-
+secret-manager (>=2.16.1,<3.0.0) Requires-Dist: google-cloud-storage
+(>=2.9.0,<3.0.0) Requires-Dist: google-crc32c (>=1.5.0,<2.0.0) Requires-Dist:
+ipregistry (>=3.2.0,<4.0.0) Requires-Dist: kfp (>=2.4.0,<3.0.0) Requires-Dist:
+mcap (>=1.1.1,<2.0.0) Requires-Dist: mcap-ros2-support (>=0.5.3,<0.6.0)
+Requires-Dist: numpy (>=1.19,<2.0) ; python_version < "3.9" Requires-Dist:
+numpy (>=1.23,<2.0) ; python_version >= "3.9" Requires-Dist: pillow
 (>=10.2.0,<11.0.0) Requires-Dist: protobuf (>=3.20.0,<4.0.0) Requires-Dist:
 python-path (>=0.1.3,<0.2.0) Requires-Dist: slack-sdk (>=3.21.3,<4.0.0)
 Requires-Dist: structlog (>=23.1.0,<24.0.0) Requires-Dist: timezonefinder
 (==4.4.1) Requires-Dist: tzlocal (>=5.2,<6.0) Description-Content-Type: text/
 markdown
 
                                     _[_L_o_g_o_]
```

