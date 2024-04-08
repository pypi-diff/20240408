# Comparing `tmp/jianyingdraft_py-0.1.8.tar.gz` & `tmp/jianyingdraft_py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianyingdraft_py-0.1.8.tar", max compression
+gzip compressed data, was "jianyingdraft_py-0.1.9.tar", max compression
```

## Comparing `jianyingdraft_py-0.1.8.tar` & `jianyingdraft_py-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-0.1.8/JianYingDraft/__init__.py
--rw-r--r--   0        0        0      159 2024-03-24 09:09:33.984726 jianyingdraft_py-0.1.8/JianYingDraft/core/__init__.py
--rw-r--r--   0        0        0     9156 2024-03-30 04:44:45.919428 jianyingdraft_py-0.1.8/JianYingDraft/core/draft.py
--rw-r--r--   0        0        0     7174 2024-03-29 05:25:41.499997 jianyingdraft_py-0.1.8/JianYingDraft/core/media.py
--rw-r--r--   0        0        0     1387 2024-03-29 05:25:48.612581 jianyingdraft_py-0.1.8/JianYingDraft/core/mediaAudio.py
--rw-r--r--   0        0        0     1364 2024-03-29 05:26:30.317548 jianyingdraft_py-0.1.8/JianYingDraft/core/mediaFactory.py
--rw-r--r--   0        0        0     1507 2024-03-29 05:26:00.190295 jianyingdraft_py-0.1.8/JianYingDraft/core/mediaImage.py
--rw-r--r--   0        0        0     1520 2024-03-29 05:26:08.208537 jianyingdraft_py-0.1.8/JianYingDraft/core/mediaText.py
--rw-r--r--   0        0        0     1530 2024-03-29 05:26:20.813825 jianyingdraft_py-0.1.8/JianYingDraft/core/mediaVideo.py
--rw-r--r--   0        0        0     9469 2024-03-29 05:26:20.773543 jianyingdraft_py-0.1.8/JianYingDraft/core/template.py
--rw-r--r--   0        0        0     3151 2024-03-24 09:08:48.975245 jianyingdraft_py-0.1.8/JianYingDraft/template/draft_content.json
--rw-r--r--   0        0        0     1591 2024-03-24 09:08:52.740696 jianyingdraft_py-0.1.8/JianYingDraft/template/draft_meta_info.json
--rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-0.1.8/JianYingDraft/utils/__init__.py
--rw-r--r--   0        0        0      866 2024-03-29 02:21:54.415368 jianyingdraft_py-0.1.8/JianYingDraft/utils/tools.py
--rw-r--r--   0        0        0     1066 2024-03-24 09:07:42.089208 jianyingdraft_py-0.1.8/LICENSE
--rw-r--r--   0        0        0      546 2024-03-30 10:53:29.079121 jianyingdraft_py-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1550 2024-03-29 15:44:39.369561 jianyingdraft_py-0.1.8/README.md
--rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 jianyingdraft_py-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-0.1.9/JianYingDraft/__init__.py
+-rw-r--r--   0        0        0      159 2024-03-24 09:09:33.984726 jianyingdraft_py-0.1.9/JianYingDraft/core/__init__.py
+-rw-r--r--   0        0        0     9306 2024-03-30 11:43:51.292222 jianyingdraft_py-0.1.9/JianYingDraft/core/draft.py
+-rw-r--r--   0        0        0     7174 2024-03-29 05:25:41.499997 jianyingdraft_py-0.1.9/JianYingDraft/core/media.py
+-rw-r--r--   0        0        0     1387 2024-03-29 05:25:48.612581 jianyingdraft_py-0.1.9/JianYingDraft/core/mediaAudio.py
+-rw-r--r--   0        0        0     1364 2024-03-29 05:26:30.317548 jianyingdraft_py-0.1.9/JianYingDraft/core/mediaFactory.py
+-rw-r--r--   0        0        0     1507 2024-03-29 05:26:00.190295 jianyingdraft_py-0.1.9/JianYingDraft/core/mediaImage.py
+-rw-r--r--   0        0        0     1520 2024-03-29 05:26:08.208537 jianyingdraft_py-0.1.9/JianYingDraft/core/mediaText.py
+-rw-r--r--   0        0        0     1530 2024-03-29 05:26:20.813825 jianyingdraft_py-0.1.9/JianYingDraft/core/mediaVideo.py
+-rw-r--r--   0        0        0     9469 2024-03-29 05:26:20.773543 jianyingdraft_py-0.1.9/JianYingDraft/core/template.py
+-rw-r--r--   0        0        0     3151 2024-03-24 09:08:48.975245 jianyingdraft_py-0.1.9/JianYingDraft/template/draft_content.json
+-rw-r--r--   0        0        0     1591 2024-03-24 09:08:52.740696 jianyingdraft_py-0.1.9/JianYingDraft/template/draft_meta_info.json
+-rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-0.1.9/JianYingDraft/utils/__init__.py
+-rw-r--r--   0        0        0      866 2024-03-29 02:21:54.415368 jianyingdraft_py-0.1.9/JianYingDraft/utils/tools.py
+-rw-r--r--   0        0        0     1066 2024-03-24 09:07:42.089208 jianyingdraft_py-0.1.9/LICENSE
+-rw-r--r--   0        0        0      546 2024-03-30 11:44:15.873229 jianyingdraft_py-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1550 2024-03-29 15:44:39.369561 jianyingdraft_py-0.1.9/README.md
+-rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 jianyingdraft_py-0.1.9/PKG-INFO
```

### Comparing `jianyingdraft_py-0.1.8/JianYingDraft/core/draft.py` & `jianyingdraft_py-0.1.9/JianYingDraft/core/draft.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,20 @@
 
         # 将媒体信息添加到draft的轨道库
         self.__add_media_to_content_tracks(media)
 
         # 将媒体信息添加到draft的元数据库
         self.__add_media_to_meta_info(media)
 
+    def get_draft_duration(self):
+        """
+        获取（通过计算）草稿的时长
+        """
+        self.__get_track_duration("video")
+
     def save(self):
         """
         保存草稿
         """
         # 校准时长信息
         self.__calc_duration()
```

### Comparing `jianyingdraft_py-0.1.8/JianYingDraft/core/media.py` & `jianyingdraft_py-0.1.9/JianYingDraft/core/media.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/JianYingDraft/core/mediaAudio.py` & `jianyingdraft_py-0.1.9/JianYingDraft/core/mediaAudio.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/JianYingDraft/core/mediaFactory.py` & `jianyingdraft_py-0.1.9/JianYingDraft/core/mediaFactory.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/JianYingDraft/core/mediaImage.py` & `jianyingdraft_py-0.1.9/JianYingDraft/core/mediaImage.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/JianYingDraft/core/mediaText.py` & `jianyingdraft_py-0.1.9/JianYingDraft/core/mediaText.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/JianYingDraft/core/mediaVideo.py` & `jianyingdraft_py-0.1.9/JianYingDraft/core/mediaVideo.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/JianYingDraft/core/template.py` & `jianyingdraft_py-0.1.9/JianYingDraft/core/template.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/JianYingDraft/template/draft_content.json` & `jianyingdraft_py-0.1.9/JianYingDraft/template/draft_content.json`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/JianYingDraft/template/draft_meta_info.json` & `jianyingdraft_py-0.1.9/JianYingDraft/template/draft_meta_info.json`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/JianYingDraft/utils/tools.py` & `jianyingdraft_py-0.1.9/JianYingDraft/utils/tools.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/LICENSE` & `jianyingdraft_py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/pyproject.toml` & `jianyingdraft_py-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "JianYingDraft.PY"
-version = "0.1.8"
+version = "0.1.9"
 description = "帮助剪映快速生成草稿的方案"
 authors = ["解大劦 <develope@163.com>"]
 readme = "README.md"
 packages = [{ include = "JianYingDraft" }]
 include = ["README.md", "LICENSE"]
 license = "MIT"
```

### Comparing `jianyingdraft_py-0.1.8/README.md` & `jianyingdraft_py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.8/PKG-INFO` & `jianyingdraft_py-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JianYingDraft.PY
-Version: 0.1.8
+Version: 0.1.9
 Summary: 帮助剪映快速生成草稿的方案
 License: MIT
 Author: 解大劦
 Author-email: develope@163.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

