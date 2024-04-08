# Comparing `tmp/ccdt-2.1.93.tar.gz` & `tmp/ccdt-2.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.1.93.tar", last modified: Sat Mar  9 03:01:27 2024, max compression
+gzip compressed data, was "ccdt-2.1.94.tar", last modified: Mon Apr  8 09:54:32 2024, max compression
```

## Comparing `ccdt-2.1.93.tar` & `ccdt-2.1.94.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 03:01:27.870984 ccdt-2.1.93/
--rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.93/LICENSE
--rw-rw-rw-   0        0        0     4806 2024-03-09 03:01:27.869986 ccdt-2.1.93/PKG-INFO
--rw-rw-rw-   0        0        0     3979 2023-06-26 09:05:42.000000 ccdt-2.1.93/README.md
-drwxrwxrwx   0        0        0        0 2024-03-09 03:01:27.839069 ccdt-2.1.93/ccdt/
--rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.93/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 03:01:27.849043 ccdt-2.1.93/ccdt/dataset/
--rw-rw-rw-   0        0        0      248 2023-07-31 10:14:46.000000 ccdt-2.1.93/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 03:01:27.851037 ccdt-2.1.93/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.93/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    34221 2024-03-09 02:58:35.000000 ccdt-2.1.93/ccdt/dataset/base_coco/base_coco.py
-drwxrwxrwx   0        0        0        0 2024-03-09 03:01:27.854029 ccdt-2.1.93/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.93/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0    15199 2023-11-27 03:47:20.000000 ccdt-2.1.93/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0   115258 2024-03-07 07:48:12.000000 ccdt-2.1.93/ccdt/dataset/base_labelme/base_labelme.py
-drwxrwxrwx   0        0        0        0 2024-03-09 03:01:27.859016 ccdt-2.1.93/ccdt/dataset/base_voc/
--rw-rw-rw-   0        0        0      326 2023-11-07 09:53:48.000000 ccdt-2.1.93/ccdt/dataset/base_voc/__init__.py
--rw-rw-rw-   0        0        0     4862 2023-11-27 03:47:20.000000 ccdt-2.1.93/ccdt/dataset/base_voc/base_sys.py
--rw-rw-rw-   0        0        0     3834 2023-10-14 07:34:34.000000 ccdt-2.1.93/ccdt/dataset/base_voc/base_txt.py
--rw-rw-rw-   0        0        0     3430 2023-07-31 13:32:48.000000 ccdt-2.1.93/ccdt/dataset/base_voc/base_voc.py
--rw-rw-rw-   0        0        0    13391 2023-11-10 05:14:34.000000 ccdt-2.1.93/ccdt/dataset/base_voc/coco_to_labelme.py
--rw-rw-rw-   0        0        0    23667 2024-03-07 03:40:15.000000 ccdt-2.1.93/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2024-03-09 03:01:27.862008 ccdt-2.1.93/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      221 2023-06-26 08:16:17.000000 ccdt-2.1.93/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.93/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    27068 2024-02-02 07:58:30.000000 ccdt-2.1.93/ccdt/dataset/utils/labelme_load.py
-drwxrwxrwx   0        0        0        0 2024-03-09 03:01:27.866994 ccdt-2.1.93/ccdt/video_tool/
--rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.93/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1726 2023-07-05 09:01:01.000000 ccdt-2.1.93/ccdt/video_tool/intercept.py
--rw-rw-rw-   0        0        0     5367 2024-03-02 06:01:23.000000 ccdt-2.1.93/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     6301 2023-08-18 09:59:56.000000 ccdt-2.1.93/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2024-03-09 03:01:27.868989 ccdt-2.1.93/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4806 2024-03-09 03:01:27.000000 ccdt-2.1.93/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      851 2024-03-09 03:01:27.000000 ccdt-2.1.93/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 03:01:27.000000 ccdt-2.1.93/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-03-09 03:01:27.000000 ccdt-2.1.93/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2024-03-09 03:01:27.000000 ccdt-2.1.93/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-09 03:01:27.000000 ccdt-2.1.93/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-09 03:01:27.871981 ccdt-2.1.93/setup.cfg
--rw-rw-rw-   0        0        0     2524 2024-03-09 03:01:14.000000 ccdt-2.1.93/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-09 03:01:27.867992 ccdt-2.1.93/test/
--rw-rw-rw-   0        0        0     8178 2023-06-09 06:33:20.000000 ccdt-2.1.93/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.854778 ccdt-2.1.94/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.94/LICENSE
+-rw-rw-rw-   0        0        0     4806 2024-04-08 09:54:32.853781 ccdt-2.1.94/PKG-INFO
+-rw-rw-rw-   0        0        0     3979 2023-06-26 09:05:42.000000 ccdt-2.1.94/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.643366 ccdt-2.1.94/ccdt/
+-rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.94/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.657307 ccdt-2.1.94/ccdt/dataset/
+-rw-rw-rw-   0        0        0      248 2023-07-31 10:14:46.000000 ccdt-2.1.94/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.660299 ccdt-2.1.94/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.94/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    34384 2024-03-09 03:14:32.000000 ccdt-2.1.94/ccdt/dataset/base_coco/base_coco.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.706211 ccdt-2.1.94/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.94/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0    15199 2023-11-27 03:47:20.000000 ccdt-2.1.94/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0   115258 2024-03-07 07:48:12.000000 ccdt-2.1.94/ccdt/dataset/base_labelme/base_labelme.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.772036 ccdt-2.1.94/ccdt/dataset/base_voc/
+-rw-rw-rw-   0        0        0      326 2023-11-07 09:53:48.000000 ccdt-2.1.94/ccdt/dataset/base_voc/__init__.py
+-rw-rw-rw-   0        0        0     4862 2023-11-27 03:47:20.000000 ccdt-2.1.94/ccdt/dataset/base_voc/base_sys.py
+-rw-rw-rw-   0        0        0     3834 2023-10-14 07:34:34.000000 ccdt-2.1.94/ccdt/dataset/base_voc/base_txt.py
+-rw-rw-rw-   0        0        0     3430 2023-07-31 13:32:48.000000 ccdt-2.1.94/ccdt/dataset/base_voc/base_voc.py
+-rw-rw-rw-   0        0        0    14450 2024-04-08 09:36:39.000000 ccdt-2.1.94/ccdt/dataset/base_voc/coco_to_labelme.py
+-rw-rw-rw-   0        0        0    23667 2024-03-07 03:40:15.000000 ccdt-2.1.94/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.778982 ccdt-2.1.94/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      221 2023-06-26 08:16:17.000000 ccdt-2.1.94/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.94/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    27068 2024-02-02 07:58:30.000000 ccdt-2.1.94/ccdt/dataset/utils/labelme_load.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.825856 ccdt-2.1.94/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.94/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1726 2023-07-05 09:01:01.000000 ccdt-2.1.94/ccdt/video_tool/intercept.py
+-rw-rw-rw-   0        0        0     5367 2024-03-02 06:01:23.000000 ccdt-2.1.94/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     6301 2023-08-18 09:59:56.000000 ccdt-2.1.94/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.851790 ccdt-2.1.94/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4806 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 09:54:32.855777 ccdt-2.1.94/setup.cfg
+-rw-rw-rw-   0        0        0     2524 2024-04-08 09:54:17.000000 ccdt-2.1.94/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.840817 ccdt-2.1.94/test/
+-rw-rw-rw-   0        0        0     8178 2023-06-09 06:33:20.000000 ccdt-2.1.94/test/test.py
```

### Comparing `ccdt-2.1.93/LICENSE` & `ccdt-2.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/PKG-INFO` & `ccdt-2.1.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.93
+Version: 2.1.94
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.93/README.md` & `ccdt-2.1.94/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt/dataset/base_coco/base_coco.py` & `ccdt-2.1.94/ccdt/dataset/base_coco/base_coco.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,15 @@
                     continue
             if structure_shape_key is None and self.parameter.coco_to_bbox is not True:  # 处理不打组的数据，即分组键为None，只有矩形框未分组的可以转coco注释
                 # 一张图像如果标注都没有打组，就会直接把所有标注shape进行迭代
                 self.shape_processing(structure_shape_value, dataset, one_img_ann_list, point_list, rebuild_polygon_point_shape)
                 convert_segmentation = sum(segmentation, point_list)  # 把列表中存储的多个元组元素，合并成一个列表且保持原有排列顺序
                 rebuild_polygon_point_shape.update({'segmentation': convert_segmentation})  # 新增关键点列表，按照左上、右上、右下、左下的顺序排序
                 one_img_ann_list.append(rebuild_polygon_point_shape)  # 把标注shape追加到转coco时的迭代列表集合中
-            if self.parameter.coco_to_bbox:  # 处理多边形转coco为bbox，矩形框转coco为bbox
+            if self.parameter.coco_to_bbox:  # 处理多边形转coco为bbox且points同时转换为segmentation，矩形框转coco为bbox
                 for shape in structure_shape_value:
                     if shape.setdefault('shape_type') == 'polygon' and self.parameter.coco_to_bbox is True:
                         polygon = self.polygon_shape_bbox(shape, dataset)
                         one_img_ann_list.extend(polygon)
                     if shape.setdefault('shape_type') == 'rectangle':  # 目前存在组合：1、多边形和矩形框组合。2、点和矩形框组合
                         rectangle = self.rectangle_shape_bbox(shape)
                         one_img_ann_list.extend(rectangle)
@@ -496,15 +496,15 @@
     #         # clamp_y1 = np.clip(y1, 0, dataset.get('image_height'))
     #         # clamp_x2 = np.clip(x2, 0, dataset.get('image_width'))
     #         # clamp_y2 = np.clip(y2, 0, dataset.get('image_height'))
     #         # dataset.update({'output_dir': dataset.get('out_of_bounds_path')})
     #         return True
     def polygon_shape_bbox(self, shape, dataset):
         """
-        把多边形转为矩形框
+        把多边形转为矩形框，同时把shape['points']，使用列表解析和itertools.chain.from_iterable()来快速将子列表展开为单个列表。
         @param shape:
         @param dataset:
         """
         one_img_ann_list = list()
         file_path = dataset.get('full_path')
         rebuild_polygon_point_shape = {}  # 存储shape重构为coco标注属性字典变量
         if len(shape['points']) == 4:
```

### Comparing `ccdt-2.1.93/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.1.94/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.1.94/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt/dataset/base_voc/base_sys.py` & `ccdt-2.1.94/ccdt/dataset/base_voc/base_sys.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt/dataset/base_voc/base_txt.py` & `ccdt-2.1.94/ccdt/dataset/base_voc/base_txt.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt/dataset/base_voc/base_voc.py` & `ccdt-2.1.94/ccdt/dataset/base_voc/base_voc.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt/dataset/base_voc/coco_to_labelme.py` & `ccdt-2.1.94/ccdt/dataset/base_voc/coco_to_labelme.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import ast
 import json
 from ccdt.dataset import *
 from collections import defaultdict
 import time
 import itertools
 import hashlib
-
+import ccdt.dataset.utils.labelme_load
 
 def _isArrayLike(obj):
     return hasattr(obj, '__iter__') and hasattr(obj, '__len__')
 
 
 class CocoToLabelme(BaseLabelme):
     # 当前设计的coco转labelme，主要是图像文件没有对应的注释，注释都在coco文件中
@@ -74,15 +74,15 @@
                 dataset.update({'imagePath': relative_path})
                 dataset.update({'image_width': image_width})
                 dataset.update({'image_height': image_height})
                 dataset.update({'labelme_file': json_name})
                 dataset.update({'image_file': image_attr.get("file_name")})
                 full_path = os.path.join(dataset.get('input_dir'), dataset.get('image_dir'), dataset.get('image_file'))
                 json_path = os.path.join(dataset.get('input_dir'), dataset.get('labelme_dir'), dataset.get('labelme_file'))
-                md5value = self.calculate_file_md5(full_path)
+                md5value = self.calculate_file_md5(full_path, dataset)
                 dataset.update({'full_path': full_path})
                 dataset.update({'json_path': json_path})
                 dataset.update({'md5_value': md5value})
                 labelme_data = dict(
                     version='4.5.9',
                     flags={},
                     shapes=[],
@@ -254,20 +254,36 @@
             ids = []
         if _isArrayLike(ids):
             return [self.cats[id] for id in ids]
         elif type(ids) == int:
             return [self.cats[ids]]
 
     @staticmethod
-    def calculate_file_md5(file_path):
+    def calculate_file_md5(file_path, dataset):
         """
         functools.lru_cache装饰器对文件的MD5值进行了缓存，暂时没有用
         采用最近最少使用的缓存策略，最多缓存128个不同的文件的MD5值
         这样可以大大减少重复计算MD5值的次数，节约计算资源，提高程序性能。
         """
-        with open(file_path, 'rb') as f:
-            hasher = hashlib.md5()
-            buf = f.read(8192)
-            while buf:
-                hasher.update(buf)
+
+        # import ccdt.dataset.utils.labelme_load
+        # from ccdt.dataset.utils.labelme_load import calculate_sha3_512
+        # content = utils.labelme_load.LabelmeLoad.read_file(file_path)
+        # sha3_512 = utils.labelme_load.LabelmeLoad.calculate_sha3_512(content)
+        # print(sha3_512)
+        try:
+            with open(file_path, 'rb') as f:
+                hasher = hashlib.sha3_512()
                 buf = f.read(8192)
-            return hasher.hexdigest()
+                while buf:
+                    hasher.update(buf)
+                    buf = f.read(8192)
+                return hasher.hexdigest()
+        except Exception as e:
+            print(e)
+            print("图片存放目录不存在00.images目录，该目录为标准，必须手动创建后把图像移动到00.images目录中，再次重新执行指令")
+            images_path = os.path.join(dataset.get('input_dir'), dataset.get('image_dir'))
+            json_path = os.path.join(dataset.get('input_dir'), dataset.get('labelme_dir'))
+            os.makedirs(images_path, exist_ok=True)
+            os.makedirs(json_path, exist_ok=True)
+            print("请在此{}".format(dataset.get('input_dir')) + "   路径下移动图像到00.images目录")
+            exit()
```

### Comparing `ccdt-2.1.93/ccdt/dataset/main.py` & `ccdt-2.1.94/ccdt/dataset/main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt/dataset/utils/encoder.py` & `ccdt-2.1.94/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.1.94/ccdt/dataset/utils/labelme_load.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt/video_tool/intercept.py` & `ccdt-2.1.94/ccdt/video_tool/intercept.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt/video_tool/split.py` & `ccdt-2.1.94/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt/video_tool/video_main.py` & `ccdt-2.1.94/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/ccdt.egg-info/PKG-INFO` & `ccdt-2.1.94/ccdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.93
+Version: 2.1.94
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.93/ccdt.egg-info/SOURCES.txt` & `ccdt-2.1.94/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.93/setup.py` & `ccdt-2.1.94/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.1.93',
+    version='2.1.94',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ccdt-2.1.93/test/test.py` & `ccdt-2.1.94/test/test.py`

 * *Files identical despite different names*

