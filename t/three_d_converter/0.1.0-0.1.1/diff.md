# Comparing `tmp/three_d_converter-0.1.0.tar.gz` & `tmp/three_d_converter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "three_d_converter-0.1.0.tar", max compression
+gzip compressed data, was "three_d_converter-0.1.1.tar", max compression
```

## Comparing `three_d_converter-0.1.0.tar` & `three_d_converter-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0        0 2024-03-25 09:14:32.209732 three_d_converter-0.1.0/README.md
--rw-r--r--   0        0        0      340 2024-04-05 00:43:52.679294 three_d_converter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-04 13:52:25.329765 three_d_converter-0.1.0/three_d_converter/.DS_Store
--rw-r--r--   0        0        0       75 2024-03-27 09:28:17.451540 three_d_converter-0.1.0/three_d_converter/__init__.py
--rw-r--r--   0        0        0     1886 2024-03-25 11:28:49.087664 three_d_converter-0.1.0/three_d_converter/blender_installation.py
--rw-r--r--   0        0        0        0 2024-03-26 16:33:43.145406 three_d_converter-0.1.0/three_d_converter/blender_scripts/__init__.py
--rw-r--r--   0        0        0      187 2024-03-27 09:22:16.615625 three_d_converter-0.1.0/three_d_converter/blender_scripts/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-03-26 16:34:01.604872 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__init__.py
--rw-r--r--   0        0        0      196 2024-03-27 09:22:16.633256 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      869 2024-03-27 14:18:41.066530 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1381 2024-04-01 19:05:36.697671 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc
--rw-r--r--   0        0        0      841 2024-04-04 14:37:52.250202 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc
--rw-r--r--   0        0        0      949 2024-03-27 14:35:58.192056 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc
--rw-r--r--   0        0        0      868 2024-03-27 14:35:58.192389 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc
--rw-r--r--   0        0        0      885 2024-03-27 14:35:58.192751 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc
--rw-r--r--   0        0        0     1910 2024-03-30 21:41:27.622542 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc
--rw-r--r--   0        0        0      841 2024-03-27 14:35:58.193147 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc
--rw-r--r--   0        0        0      332 2024-03-27 14:18:37.671207 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/base.py
--rw-r--r--   0        0        0     1163 2024-03-30 22:41:07.584587 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/factory.py
--rw-r--r--   0        0        0      432 2024-04-01 19:13:29.237259 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/fbx.py
--rw-r--r--   0        0        0      584 2024-03-27 14:35:22.912067 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/gltf_glb.py
--rw-r--r--   0        0        0      480 2024-03-27 14:35:27.665691 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/obj.py
--rw-r--r--   0        0        0      499 2024-03-27 14:35:30.763033 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/stl.py
--rw-r--r--   0        0        0     1970 2024-03-30 21:41:24.635318 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/usdz.py
--rw-r--r--   0        0        0      431 2024-03-27 14:35:36.527341 three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/x3d.py
--rw-r--r--   0        0        0        0 2024-03-26 16:34:00.638176 three_d_converter-0.1.0/three_d_converter/blender_scripts/filehandler/__init__.py
--rw-r--r--   0        0        0      199 2024-03-27 09:22:16.616322 three_d_converter-0.1.0/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1400 2024-03-30 21:35:19.640244 three_d_converter-0.1.0/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc
--rw-r--r--   0        0        0      969 2024-03-30 21:30:39.900357 three_d_converter-0.1.0/three_d_converter/blender_scripts/filehandler/filehandler.py
--rw-r--r--   0        0        0        0 2024-03-26 16:33:58.724687 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__init__.py
--rw-r--r--   0        0        0      196 2024-03-27 09:21:41.584714 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      841 2024-03-27 09:22:16.618618 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1381 2024-03-27 09:21:41.585181 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc
--rw-r--r--   0        0        0      812 2024-03-27 09:22:16.619044 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc
--rw-r--r--   0        0        0      843 2024-03-27 09:22:16.619394 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc
--rw-r--r--   0        0        0      812 2024-03-27 09:22:16.619759 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc
--rw-r--r--   0        0        0      811 2024-03-27 09:22:16.620105 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc
--rw-r--r--   0        0        0     1404 2024-03-30 20:50:55.073448 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc
--rw-r--r--   0        0        0      812 2024-03-27 09:22:16.632941 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc
--rw-r--r--   0        0        0      314 2024-03-26 15:59:12.658481 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/base.py
--rw-r--r--   0        0        0     1162 2024-03-26 16:08:17.690705 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/factory.py
--rw-r--r--   0        0        0      410 2024-03-26 16:00:47.363524 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/fbx.py
--rw-r--r--   0        0        0      449 2024-03-26 16:00:54.064417 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/gltf_glb.py
--rw-r--r--   0        0        0      409 2024-03-26 16:00:57.882675 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/obj.py
--rw-r--r--   0        0        0      408 2024-03-26 16:01:00.538346 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/stl.py
--rw-r--r--   0        0        0     1373 2024-03-30 20:50:28.446058 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/usdz.py
--rw-r--r--   0        0        0      409 2024-03-26 16:01:07.761750 three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/x3d.py
--rw-r--r--   0        0        0     1830 2024-03-27 16:49:47.021033 three_d_converter-0.1.0/three_d_converter/blender_scripts/main.py
--rw-r--r--   0        0        0      525 2024-03-30 20:57:37.029462 three_d_converter-0.1.0/three_d_converter/converter.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 three_d_converter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-25 09:14:32.209732 three_d_converter-0.1.1/README.md
+-rw-r--r--   0        0        0      340 2024-04-08 10:45:44.452356 three_d_converter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-08 08:17:05.466098 three_d_converter-0.1.1/three_d_converter/.DS_Store
+-rw-r--r--   0        0        0       75 2024-03-27 09:28:17.451540 three_d_converter-0.1.1/three_d_converter/__init__.py
+-rw-r--r--   0        0        0     1886 2024-03-25 11:28:49.087664 three_d_converter-0.1.1/three_d_converter/blender_installation.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:33:43.145406 three_d_converter-0.1.1/three_d_converter/blender_scripts/__init__.py
+-rw-r--r--   0        0        0      187 2024-03-27 09:22:16.615625 three_d_converter-0.1.1/three_d_converter/blender_scripts/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-03-26 16:34:01.604872 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-27 09:22:16.633256 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      869 2024-03-27 14:18:41.066530 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1381 2024-04-01 19:05:36.697671 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0      841 2024-04-04 14:37:52.250202 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc
+-rw-r--r--   0        0        0      949 2024-03-27 14:35:58.192056 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc
+-rw-r--r--   0        0        0      868 2024-03-27 14:35:58.192389 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc
+-rw-r--r--   0        0        0      885 2024-03-27 14:35:58.192751 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc
+-rw-r--r--   0        0        0     1910 2024-03-30 21:41:27.622542 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc
+-rw-r--r--   0        0        0      841 2024-03-27 14:35:58.193147 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc
+-rw-r--r--   0        0        0      332 2024-03-27 14:18:37.671207 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/base.py
+-rw-r--r--   0        0        0     1163 2024-03-30 22:41:07.584587 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/factory.py
+-rw-r--r--   0        0        0      432 2024-04-01 19:13:29.237259 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/fbx.py
+-rw-r--r--   0        0        0      584 2024-03-27 14:35:22.912067 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/gltf_glb.py
+-rw-r--r--   0        0        0      480 2024-03-27 14:35:27.665691 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/obj.py
+-rw-r--r--   0        0        0      499 2024-03-27 14:35:30.763033 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/stl.py
+-rw-r--r--   0        0        0     1970 2024-03-30 21:41:24.635318 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/usdz.py
+-rw-r--r--   0        0        0      431 2024-03-27 14:35:36.527341 three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/x3d.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:34:00.638176 three_d_converter-0.1.1/three_d_converter/blender_scripts/filehandler/__init__.py
+-rw-r--r--   0        0        0      199 2024-03-27 09:22:16.616322 three_d_converter-0.1.1/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1400 2024-04-08 09:33:12.714318 three_d_converter-0.1.1/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc
+-rw-r--r--   0        0        0      969 2024-04-08 09:32:50.673912 three_d_converter-0.1.1/three_d_converter/blender_scripts/filehandler/filehandler.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:33:58.724687 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-27 09:21:41.584714 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      841 2024-03-27 09:22:16.618618 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1381 2024-03-27 09:21:41.585181 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0      737 2024-04-08 09:50:34.382104 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc
+-rw-r--r--   0        0        0      768 2024-04-08 10:19:37.443510 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc
+-rw-r--r--   0        0        0      737 2024-04-08 09:50:34.382832 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc
+-rw-r--r--   0        0        0      736 2024-04-08 09:58:56.168458 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc
+-rw-r--r--   0        0        0     1368 2024-04-08 10:08:42.662397 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc
+-rw-r--r--   0        0        0      737 2024-04-08 10:34:59.977397 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc
+-rw-r--r--   0        0        0      314 2024-03-26 15:59:12.658481 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/base.py
+-rw-r--r--   0        0        0     1162 2024-03-26 16:08:17.690705 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/factory.py
+-rw-r--r--   0        0        0      278 2024-04-08 10:40:55.468143 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/fbx.py
+-rw-r--r--   0        0        0      317 2024-04-08 10:40:07.913312 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/gltf_glb.py
+-rw-r--r--   0        0        0      277 2024-04-08 10:39:59.167677 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/obj.py
+-rw-r--r--   0        0        0      276 2024-04-08 10:40:12.287369 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/stl.py
+-rw-r--r--   0        0        0     1319 2024-04-08 10:08:39.158994 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/usdz.py
+-rw-r--r--   0        0        0      277 2024-04-08 10:40:15.167928 three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/x3d.py
+-rw-r--r--   0        0        0     1830 2024-03-27 16:49:47.021033 three_d_converter-0.1.1/three_d_converter/blender_scripts/main.py
+-rw-r--r--   0        0        0      525 2024-03-30 20:57:37.029462 three_d_converter-0.1.1/three_d_converter/converter.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 three_d_converter-0.1.1/PKG-INFO
```

### Comparing `three_d_converter-0.1.0/three_d_converter/.DS_Store` & `three_d_converter-0.1.1/three_d_converter/.DS_Store`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_installation.py` & `three_d_converter-0.1.1/three_d_converter/blender_installation.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/factory.py` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/factory.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/gltf_glb.py` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/gltf_glb.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/exporter/usdz.py` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/exporter/usdz.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Mar 30 21:30:39 2024 UTC, .py size: 969 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7f84 0866 c903 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 c2b9 1366 c903 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 8302 5a04 6401 5300 2905 e900  ..d...Z.d.S.)...
 00000060: 0000 004e 2901 da05 7575 6964 3463 0000  ...N)...uuid4c..
 00000070: 0000 0000 0000 0000 0000 0000 0000 0500  ................
```

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/filehandler/filehandler.py` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/filehandler/filehandler.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 26 16:00:54 2024 UTC, .py size: 449 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,47 @@
-00000000: 6f0d 0d0a 0000 0000 36f1 0266 c101 0000  o.......6..f....
+00000000: 6f0d 0d0a 0000 0000 c7bd 1366 2001 0000  o..........f ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6502 8303  Z.G.d.d...d.e...
 00000060: 5a05 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000070: da0d 4d6f 6465 6c49 6d70 6f72 7465 7263  ..ModelImporterc
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0400 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
 000000a0: 0164 005a 0264 0165 036a 0464 0264 0366  .d.Z.d.e.j.d.d.f
 000000b0: 0464 0464 0584 045a 0564 0353 0029 06da  .d.d...Z.d.S.)..
-000000c0: 0f47 4c54 4647 4c42 496d 706f 7274 6572  .GLTFGLBImporter
-000000d0: da09 6669 6c65 5f70 6174 68da 0672 6574  ..file_path..ret
-000000e0: 7572 6e4e 6302 0000 0000 0000 0000 0000  urnNc...........
-000000f0: 0002 0000 0006 0000 0043 0000 0073 3e00  .........C...s>.
-00000100: 0000 7c01 6a00 6401 6b02 730a 7c01 6a00  ..|.j.d.k.s.|.j.
-00000110: 6402 6b02 721d 7401 6a02 6a03 6a04 7405  d.k.r.t.j.j.j.t.
-00000120: 6a06 a007 7c00 6a08 6a09 740a 7c01 8301  j...|.j.j.t.|...
-00000130: a102 6403 8d01 0100 6400 5300 6400 5300  ..d.....d.S.d.S.
-00000140: 2904 4e7a 052e 676c 7466 7a04 2e67 6c62  ).Nz..gltfz..glb
-00000150: 2901 da08 6669 6c65 7061 7468 290b da06  )...filepath)...
-00000160: 7375 6666 6978 da03 6270 79da 036f 7073  suffix..bpy..ops
-00000170: da0c 696d 706f 7274 5f73 6365 6e65 5a04  ..import_sceneZ.
-00000180: 676c 7466 da02 6f73 da04 7061 7468 da04  gltf..os..path..
-00000190: 6a6f 696e da0c 6669 6c65 5f68 616e 646c  join..file_handl
-000001a0: 6572 da14 7061 7468 5f74 6f5f 6669 6c65  er..path_to_file
-000001b0: 735f 696e 5f74 6d70 da03 7374 7229 02da  s_in_tmp..str)..
-000001c0: 0473 656c 6672 0400 0000 a900 7212 0000  .selfr......r...
-000001d0: 00fa 672f 5573 6572 732f 6665 7268 6174  ..g/Users/ferhat
-000001e0: 7465 6b65 722f 6968 6b5f 7072 6f6a 656b  teker/ihk_projek
-000001f0: 742f 7468 7265 655f 645f 636f 6e76 6572  t/three_d_conver
-00000200: 7465 722f 7468 7265 655f 645f 636f 6e76  ter/three_d_conv
-00000210: 6572 7465 722f 626c 656e 6465 725f 7363  erter/blender_sc
-00000220: 7269 7074 732f 696d 706f 7274 6572 2f67  ripts/importer/g
-00000230: 6c74 665f 676c 622e 7079 da0b 696d 706f  ltf_glb.py..impo
-00000240: 7274 5f66 696c 6507 0000 0073 0e00 0000  rt_file....s....
-00000250: 1401 0801 0601 0c01 02ff 0aff 04ff 7a1b  ..............z.
-00000260: 474c 5446 474c 4249 6d70 6f72 7465 722e  GLTFGLBImporter.
-00000270: 696d 706f 7274 5f66 696c 6529 06da 085f  import_file)..._
-00000280: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000290: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000002a0: 5fda 0770 6174 686c 6962 da04 5061 7468  _..pathlib..Path
-000002b0: 7214 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-000002c0: 1200 0000 7213 0000 0072 0300 0000 0600  ....r....r......
-000002d0: 0000 7304 0000 0008 0018 0172 0300 0000  ..s........r....
-000002e0: 2906 7218 0000 00da 1d62 6c65 6e64 6572  ).r......blender
-000002f0: 5f73 6372 6970 7473 2e69 6d70 6f72 7465  _scripts.importe
-00000300: 722e 6261 7365 7202 0000 0072 0b00 0000  r.baser....r....
-00000310: 7208 0000 0072 0300 0000 7212 0000 0072  r....r....r....r
-00000320: 1200 0000 7212 0000 0072 1300 0000 da08  ....r....r......
-00000330: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
-00000340: 0008 000c 0108 0108 0114 02              ...........
+000000c0: 0b46 4258 496d 706f 7274 6572 da09 6669  .FBXImporter..fi
+000000d0: 6c65 5f70 6174 68da 0672 6574 7572 6e4e  le_path..returnN
+000000e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000000f0: 0003 0000 0043 0000 0073 2600 0000 7c01  .....C...s&...|.
+00000100: 6a00 6401 6b02 7211 7401 6a02 6a03 6a04  j.d.k.r.t.j.j.j.
+00000110: 7405 7c01 8301 6402 8d01 0100 6400 5300  t.|...d.....d.S.
+00000120: 6400 5300 2903 4e7a 042e 6662 7829 01da  d.S.).Nz..fbx)..
+00000130: 0866 696c 6570 6174 6829 06da 0673 7566  .filepath)...suf
+00000140: 6669 78da 0362 7079 da03 6f70 735a 0c69  fix..bpy..opsZ.i
+00000150: 6d70 6f72 745f 7363 656e 655a 0366 6278  mport_sceneZ.fbx
+00000160: da03 7374 7229 02da 0473 656c 6672 0400  ..str)...selfr..
+00000170: 0000 a900 720c 0000 00fa 622f 5573 6572  ....r.....b/User
+00000180: 732f 6665 7268 6174 7465 6b65 722f 6968  s/ferhatteker/ih
+00000190: 6b5f 7072 6f6a 656b 742f 7468 7265 655f  k_projekt/three_
+000001a0: 645f 636f 6e76 6572 7465 722f 7468 7265  d_converter/thre
+000001b0: 655f 645f 636f 6e76 6572 7465 722f 626c  e_d_converter/bl
+000001c0: 656e 6465 725f 7363 7269 7074 732f 696d  ender_scripts/im
+000001d0: 706f 7274 6572 2f66 6278 2e70 79da 0b69  porter/fbx.py..i
+000001e0: 6d70 6f72 745f 6669 6c65 0800 0000 7306  mport_file....s.
+000001f0: 0000 000a 0118 0104 ff7a 1746 4258 496d  .........z.FBXIm
+00000200: 706f 7274 6572 2e69 6d70 6f72 745f 6669  porter.import_fi
+00000210: 6c65 2906 da08 5f5f 6e61 6d65 5f5f da0a  le)...__name__..
+00000220: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000230: 616c 6e61 6d65 5f5f da07 7061 7468 6c69  alname__..pathli
+00000240: 62da 0450 6174 6872 0e00 0000 720c 0000  b..Pathr....r...
+00000250: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000260: 7203 0000 0007 0000 0073 0400 0000 0800  r........s......
+00000270: 1801 7203 0000 0029 0672 1200 0000 da1d  ..r....).r......
+00000280: 626c 656e 6465 725f 7363 7269 7074 732e  blender_scripts.
+00000290: 696d 706f 7274 6572 2e62 6173 6572 0200  importer.baser..
+000002a0: 0000 da02 6f73 7208 0000 0072 0300 0000  ....osr....r....
+000002b0: 720c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+000002c0: 0d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000002d0: 0000 730a 0000 0008 000c 0108 0108 0114  ..s.............
+000002e0: 03                                       .
```

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 26 16:00:57 2024 UTC, .py size: 409 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,47 @@
-00000000: 6f0d 0d0a 0000 0000 39f1 0266 9901 0000  o.......9..f....
+00000000: 6f0d 0d0a 0000 0000 ddbd 1366 1f01 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6502 8303  Z.G.d.d...d.e...
 00000060: 5a05 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000070: da0d 4d6f 6465 6c49 6d70 6f72 7465 7263  ..ModelImporterc
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0400 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
 000000a0: 0164 005a 0264 0165 036a 0464 0264 0366  .d.Z.d.e.j.d.d.f
 000000b0: 0464 0464 0584 045a 0564 0353 0029 06da  .d.d...Z.d.S.)..
 000000c0: 0b4f 424a 496d 706f 7274 6572 da09 6669  .OBJImporter..fi
 000000d0: 6c65 5f70 6174 68da 0672 6574 7572 6e4e  le_path..returnN
 000000e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000000f0: 0006 0000 0043 0000 0073 3400 0000 7c01  .....C...s4...|.
-00000100: 6a00 6401 6b02 7218 7401 6a02 6a03 6a04  j.d.k.r.t.j.j.j.
-00000110: 7405 6a06 a007 7c00 6a08 6a09 740a 7c01  t.j...|.j.j.t.|.
-00000120: 8301 a102 6402 8d01 0100 6400 5300 6400  ....d.....d.S.d.
-00000130: 5300 2903 4e7a 042e 6f62 6a29 01da 0866  S.).Nz..obj)...f
-00000140: 696c 6570 6174 6829 0bda 0673 7566 6669  ilepath)...suffi
-00000150: 78da 0362 7079 da03 6f70 73da 0c69 6d70  x..bpy..ops..imp
-00000160: 6f72 745f 7363 656e 65da 036f 626a da02  ort_scene..obj..
-00000170: 6f73 da04 7061 7468 da04 6a6f 696e da0c  os..path..join..
-00000180: 6669 6c65 5f68 616e 646c 6572 da14 7061  file_handler..pa
-00000190: 7468 5f74 6f5f 6669 6c65 735f 696e 5f74  th_to_files_in_t
-000001a0: 6d70 da03 7374 7229 02da 0473 656c 6672  mp..str)...selfr
-000001b0: 0400 0000 a900 7213 0000 00fa 622f 5573  ......r.....b/Us
-000001c0: 6572 732f 6665 7268 6174 7465 6b65 722f  ers/ferhatteker/
-000001d0: 6968 6b5f 7072 6f6a 656b 742f 7468 7265  ihk_projekt/thre
-000001e0: 655f 645f 636f 6e76 6572 7465 722f 7468  e_d_converter/th
-000001f0: 7265 655f 645f 636f 6e76 6572 7465 722f  ree_d_converter/
-00000200: 626c 656e 6465 725f 7363 7269 7074 732f  blender_scripts/
-00000210: 696d 706f 7274 6572 2f6f 626a 2e70 79da  importer/obj.py.
-00000220: 0b69 6d70 6f72 745f 6669 6c65 0700 0000  .import_file....
-00000230: 730e 0000 000a 0108 0106 010c 0102 ff0a  s...............
-00000240: ff04 ff7a 174f 424a 496d 706f 7274 6572  ...z.OBJImporter
-00000250: 2e69 6d70 6f72 745f 6669 6c65 2906 da08  .import_file)...
-00000260: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000270: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000280: 5f5f da07 7061 7468 6c69 62da 0450 6174  __..pathlib..Pat
-00000290: 6872 1500 0000 7213 0000 0072 1300 0000  hr....r....r....
-000002a0: 7213 0000 0072 1400 0000 7203 0000 0006  r....r....r.....
-000002b0: 0000 0073 0400 0000 0800 1801 7203 0000  ...s........r...
-000002c0: 0029 0672 1900 0000 da1d 626c 656e 6465  .).r......blende
-000002d0: 725f 7363 7269 7074 732e 696d 706f 7274  r_scripts.import
-000002e0: 6572 2e62 6173 6572 0200 0000 720c 0000  er.baser....r...
-000002f0: 0072 0800 0000 7203 0000 0072 1300 0000  .r....r....r....
-00000300: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-00000310: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
-00000320: 0000 0800 0c01 0801 0801 1402            ............
+000000f0: 0003 0000 0043 0000 0073 2600 0000 7c01  .....C...s&...|.
+00000100: 6a00 6401 6b02 7211 7401 6a02 6a03 6a04  j.d.k.r.t.j.j.j.
+00000110: 7405 7c01 8301 6402 8d01 0100 6400 5300  t.|...d.....d.S.
+00000120: 6400 5300 2903 4e7a 042e 6f62 6a29 01da  d.S.).Nz..obj)..
+00000130: 0866 696c 6570 6174 6829 06da 0673 7566  .filepath)...suf
+00000140: 6669 78da 0362 7079 da03 6f70 73da 0c69  fix..bpy..ops..i
+00000150: 6d70 6f72 745f 7363 656e 65da 036f 626a  mport_scene..obj
+00000160: da03 7374 7229 02da 0473 656c 6672 0400  ..str)...selfr..
+00000170: 0000 a900 720e 0000 00fa 622f 5573 6572  ....r.....b/User
+00000180: 732f 6665 7268 6174 7465 6b65 722f 6968  s/ferhatteker/ih
+00000190: 6b5f 7072 6f6a 656b 742f 7468 7265 655f  k_projekt/three_
+000001a0: 645f 636f 6e76 6572 7465 722f 7468 7265  d_converter/thre
+000001b0: 655f 645f 636f 6e76 6572 7465 722f 626c  e_d_converter/bl
+000001c0: 656e 6465 725f 7363 7269 7074 732f 696d  ender_scripts/im
+000001d0: 706f 7274 6572 2f6f 626a 2e70 79da 0b69  porter/obj.py..i
+000001e0: 6d70 6f72 745f 6669 6c65 0700 0000 7306  mport_file....s.
+000001f0: 0000 000a 0118 0104 ff7a 174f 424a 496d  .........z.OBJIm
+00000200: 706f 7274 6572 2e69 6d70 6f72 745f 6669  porter.import_fi
+00000210: 6c65 2906 da08 5f5f 6e61 6d65 5f5f da0a  le)...__name__..
+00000220: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000230: 616c 6e61 6d65 5f5f da07 7061 7468 6c69  alname__..pathli
+00000240: 62da 0450 6174 6872 1000 0000 720e 0000  b..Pathr....r...
+00000250: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000260: 7203 0000 0006 0000 0073 0400 0000 0800  r........s......
+00000270: 1801 7203 0000 0029 0672 1400 0000 da1d  ..r....).r......
+00000280: 626c 656e 6465 725f 7363 7269 7074 732e  blender_scripts.
+00000290: 696d 706f 7274 6572 2e62 6173 6572 0200  importer.baser..
+000002a0: 0000 da02 6f73 7208 0000 0072 0300 0000  ....osr....r....
+000002b0: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+000002c0: 0f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000002d0: 0000 730a 0000 0008 000c 0108 0108 0114  ..s.............
+000002e0: 02                                       .
```

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 26 16:01:00 2024 UTC, .py size: 408 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,48 @@
-00000000: 6f0d 0d0a 0000 0000 3cf1 0266 9801 0000  o.......<..f....
+00000000: 6f0d 0d0a 0000 0000 88c4 1366 4701 0000  o..........fG...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6502 8303  Z.G.d.d...d.e...
 00000060: 5a05 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000070: da0d 4d6f 6465 6c49 6d70 6f72 7465 7263  ..ModelImporterc
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0400 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
 000000a0: 0164 005a 0264 0165 036a 0464 0264 0366  .d.Z.d.e.j.d.d.f
 000000b0: 0464 0464 0584 045a 0564 0353 0029 06da  .d.d...Z.d.S.)..
-000000c0: 0b53 544c 496d 706f 7274 6572 da09 6669  .STLImporter..fi
-000000d0: 6c65 5f70 6174 68da 0672 6574 7572 6e4e  le_path..returnN
-000000e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000000f0: 0006 0000 0043 0000 0073 3400 0000 7c01  .....C...s4...|.
-00000100: 6a00 6401 6b02 7218 7401 6a02 6a03 6a04  j.d.k.r.t.j.j.j.
-00000110: 7405 6a06 a007 7c00 6a08 6a09 740a 7c01  t.j...|.j.j.t.|.
-00000120: 8301 a102 6402 8d01 0100 6400 5300 6400  ....d.....d.S.d.
-00000130: 5300 2903 4e7a 042e 7374 6c29 01da 0866  S.).Nz..stl)...f
-00000140: 696c 6570 6174 6829 0bda 0673 7566 6669  ilepath)...suffi
-00000150: 78da 0362 7079 da03 6f70 735a 0b69 6d70  x..bpy..opsZ.imp
-00000160: 6f72 745f 6d65 7368 5a03 7374 6cda 026f  ort_meshZ.stl..o
-00000170: 73da 0470 6174 68da 046a 6f69 6eda 0c66  s..path..join..f
-00000180: 696c 655f 6861 6e64 6c65 72da 1470 6174  ile_handler..pat
-00000190: 685f 746f 5f66 696c 6573 5f69 6e5f 746d  h_to_files_in_tm
-000001a0: 70da 0373 7472 2902 da04 7365 6c66 7204  p..str)...selfr.
-000001b0: 0000 00a9 0072 1100 0000 fa62 2f55 7365  .....r.....b/Use
-000001c0: 7273 2f66 6572 6861 7474 656b 6572 2f69  rs/ferhatteker/i
-000001d0: 686b 5f70 726f 6a65 6b74 2f74 6872 6565  hk_projekt/three
-000001e0: 5f64 5f63 6f6e 7665 7274 6572 2f74 6872  _d_converter/thr
-000001f0: 6565 5f64 5f63 6f6e 7665 7274 6572 2f62  ee_d_converter/b
-00000200: 6c65 6e64 6572 5f73 6372 6970 7473 2f69  lender_scripts/i
-00000210: 6d70 6f72 7465 722f 7374 6c2e 7079 da0b  mporter/stl.py..
-00000220: 696d 706f 7274 5f66 696c 6507 0000 0073  import_file....s
-00000230: 0e00 0000 0a01 0801 0601 0c01 02ff 0aff  ................
-00000240: 04ff 7a17 5354 4c49 6d70 6f72 7465 722e  ..z.STLImporter.
-00000250: 696d 706f 7274 5f66 696c 6529 06da 085f  import_file)..._
-00000260: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000270: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000280: 5fda 0770 6174 686c 6962 da04 5061 7468  _..pathlib..Path
-00000290: 7213 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-000002a0: 1100 0000 7212 0000 0072 0300 0000 0600  ....r....r......
-000002b0: 0000 7304 0000 0008 0018 0172 0300 0000  ..s........r....
-000002c0: 2906 7217 0000 00da 1d62 6c65 6e64 6572  ).r......blender
-000002d0: 5f73 6372 6970 7473 2e69 6d70 6f72 7465  _scripts.importe
-000002e0: 722e 6261 7365 7202 0000 0072 0a00 0000  r.baser....r....
-000002f0: 7208 0000 0072 0300 0000 7211 0000 0072  r....r....r....r
-00000300: 1100 0000 7211 0000 0072 1200 0000 da08  ....r....r......
-00000310: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
-00000320: 0008 000c 0108 0108 0114 02              ...........
+000000c0: 0f47 4c54 4647 4c42 496d 706f 7274 6572  .GLTFGLBImporter
+000000d0: da09 6669 6c65 5f70 6174 68da 0672 6574  ..file_path..ret
+000000e0: 7572 6e4e 6302 0000 0000 0000 0000 0000  urnNc...........
+000000f0: 0002 0000 0003 0000 0043 0000 0073 3000  .........C...s0.
+00000100: 0000 7c01 6a00 6401 6b02 730a 7c01 6a00  ..|.j.d.k.s.|.j.
+00000110: 6402 6b02 7216 7401 6a02 6a03 6a04 7405  d.k.r.t.j.j.j.t.
+00000120: 7c01 8301 6403 8d01 0100 6400 5300 6400  |...d.....d.S.d.
+00000130: 5300 2904 4e7a 052e 676c 7466 7a04 2e67  S.).Nz..gltfz..g
+00000140: 6c62 2901 da08 6669 6c65 7061 7468 2906  lb)...filepath).
+00000150: da06 7375 6666 6978 da03 6270 79da 036f  ..suffix..bpy..o
+00000160: 7073 da0c 696d 706f 7274 5f73 6365 6e65  ps..import_scene
+00000170: 5a04 676c 7466 da03 7374 7229 02da 0473  Z.gltf..str)...s
+00000180: 656c 6672 0400 0000 a900 720d 0000 00fa  elfr......r.....
+00000190: 672f 5573 6572 732f 6665 7268 6174 7465  g/Users/ferhatte
+000001a0: 6b65 722f 6968 6b5f 7072 6f6a 656b 742f  ker/ihk_projekt/
+000001b0: 7468 7265 655f 645f 636f 6e76 6572 7465  three_d_converte
+000001c0: 722f 7468 7265 655f 645f 636f 6e76 6572  r/three_d_conver
+000001d0: 7465 722f 626c 656e 6465 725f 7363 7269  ter/blender_scri
+000001e0: 7074 732f 696d 706f 7274 6572 2f67 6c74  pts/importer/glt
+000001f0: 665f 676c 622e 7079 da0b 696d 706f 7274  f_glb.py..import
+00000200: 5f66 696c 6507 0000 0073 0600 0000 1401  _file....s......
+00000210: 1801 04ff 7a1b 474c 5446 474c 4249 6d70  ....z.GLTFGLBImp
+00000220: 6f72 7465 722e 696d 706f 7274 5f66 696c  orter.import_fil
+00000230: 6529 06da 085f 5f6e 616d 655f 5fda 0a5f  e)...__name__.._
+00000240: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000250: 6c6e 616d 655f 5fda 0770 6174 686c 6962  lname__..pathlib
+00000260: da04 5061 7468 720f 0000 0072 0d00 0000  ..Pathr....r....
+00000270: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00000280: 0300 0000 0600 0000 7304 0000 0008 0018  ........s.......
+00000290: 0172 0300 0000 2906 7213 0000 00da 1d62  .r....).r......b
+000002a0: 6c65 6e64 6572 5f73 6372 6970 7473 2e69  lender_scripts.i
+000002b0: 6d70 6f72 7465 722e 6261 7365 7202 0000  mporter.baser...
+000002c0: 00da 026f 7372 0800 0000 7203 0000 0072  ...osr....r....r
+000002d0: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+000002e0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000002f0: 0073 0a00 0000 0800 0c01 0801 0801 1402  .s..............
```

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Mar 30 20:50:28 2024 UTC, .py size: 1373 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 147b 0866 5d05 0000  o........{.f]...
+00000000: 6f0d 0d0a 0000 0000 27c2 1366 2705 0000  o.......'..f'...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 6400 6403 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6401 6c07 5a07 6400 6401 6c08 5a08 4700  d.l.Z.d.d.l.Z.G.
 00000070: 6404 6405 8400 6405 6506 8303 5a09 6401  d.d...d.e...Z.d.
@@ -12,77 +12,75 @@
 000000b0: 0000 0000 0004 0000 0040 0000 0073 2000  .........@...s .
 000000c0: 0000 6500 5a01 6400 5a02 6401 6503 6a04  ..e.Z.d.Z.d.e.j.
 000000d0: 6402 6403 6604 6404 6405 8404 5a05 6403  d.d.f.d.d...Z.d.
 000000e0: 5300 2906 da0c 5553 445a 496d 706f 7274  S.)...USDZImport
 000000f0: 6572 da09 6669 6c65 5f70 6174 68da 0672  er..file_path..r
 00000100: 6574 7572 6e4e 6302 0000 0000 0000 0000  eturnNc.........
 00000110: 0000 0005 0000 0009 0000 0043 0000 0073  ...........C...s
-00000120: e400 0000 7400 7401 8300 8301 7d02 7402  ....t.t.....}.t.
-00000130: a003 7404 6a05 a006 7c00 6a07 6a08 7400  ..t.j...|.j.j.t.
-00000140: 7c01 8301 a102 7404 6a05 a006 7c00 6a07  |.....t.j...|.j.
-00000150: 6a09 7c02 6401 1700 a102 a102 0100 740a  j.|.d.........t.
-00000160: a00b 7400 7c01 8301 6402 a102 8f13 7d03  ..t.|...d.....}.
-00000170: 7c03 a00c 7404 6a05 a006 7c00 6a07 6a0d  |...t.j...|.j.j.
-00000180: a101 a101 0100 5700 6400 0400 0400 8303  ......W.d.......
-00000190: 0100 6e08 3100 733b 7701 0100 0100 0100  ..n.1.s;w.......
-000001a0: 5900 0100 7404 a00e 7c00 6a07 6a0d a101  Y...t...|.j.j...
-000001b0: 4400 5d28 7d04 7c04 a00f 6403 a101 7353  D.](}.|...d...sS
-000001c0: 7c04 a00f 6404 a101 7268 7410 6a11 6a12  |...d...rht.j.j.
-000001d0: 6a13 7404 6a05 a006 7c00 6a07 6a0d 7c04  j.t.j...|.j.j.|.
-000001e0: a102 6405 6405 6405 6405 6406 6407 8d06  ..d.d.d.d.d.d...
-000001f0: 0100 7147 7414 6408 7c04 9b00 9d02 8301  ..qGt.d.|.......
-00000200: 0100 7147 6400 5300 2909 4e7a 052e 7573  ..qGd.S.).Nz..us
-00000210: 647a da01 727a 052e 7573 6463 7a05 2e75  dz..rz..usdcz..u
-00000220: 7364 6154 5a12 5245 4645 5245 4e43 455f  sdaTZ.REFERENCE_
-00000230: 4558 4953 5449 4e47 2906 da08 6669 6c65  EXISTING)...file
-00000240: 7061 7468 5a10 696d 706f 7274 5f6d 6174  pathZ.import_mat
-00000250: 6572 6961 6c73 5a12 696d 706f 7274 5f75  erialsZ.import_u
-00000260: 7364 5f70 7265 7669 6577 5a0d 696d 706f  sd_previewZ.impo
-00000270: 7274 5f73 7562 6469 765a 1072 6561 645f  rt_subdivZ.read_
-00000280: 6d65 7368 5f63 6f6c 6f72 735a 176d 746c  mesh_colorsZ.mtl
-00000290: 5f6e 616d 655f 636f 6c6c 6973 696f 6e5f  _name_collision_
-000002a0: 6d6f 6465 7a18 556e 7375 7070 6f72 7465  modez.Unsupporte
-000002b0: 6420 6669 6c65 2066 6f72 6d61 7420 2915  d file format ).
-000002c0: da03 7374 7272 0200 0000 da06 7368 7574  ..strr......shut
-000002d0: 696c da05 636f 7079 32da 026f 73da 0470  il..copy2..os..p
-000002e0: 6174 68da 046a 6f69 6eda 0c66 696c 655f  ath..join..file_
-000002f0: 6861 6e64 6c65 72da 1470 6174 685f 746f  handler..path_to
-00000300: 5f66 696c 6573 5f69 6e5f 746d 70da 1570  _files_in_tmp..p
-00000310: 6174 685f 746f 5f70 7562 6c69 635f 6d6f  ath_to_public_mo
-00000320: 6465 6c73 da07 7a69 7066 696c 65da 075a  dels..zipfile..Z
-00000330: 6970 4669 6c65 da0a 6578 7472 6163 7461  ipFile..extracta
-00000340: 6c6c da14 6d6f 6465 6c5f 746d 705f 7061  ll..model_tmp_pa
-00000350: 7468 5f75 6e7a 6970 da07 6c69 7374 6469  th_unzip..listdi
-00000360: 72da 0865 6e64 7377 6974 68da 0362 7079  r..endswith..bpy
-00000370: da03 6f70 73da 0277 6d5a 0a75 7364 5f69  ..ops..wmZ.usd_i
-00000380: 6d70 6f72 74da 0570 7269 6e74 2905 da04  mport..print)...
-00000390: 7365 6c66 7205 0000 005a 0c6e 6577 6669  selfr....Z.newfi
-000003a0: 6c65 5f70 6174 685a 0d75 7364 7a5f 756e  le_pathZ.usdz_un
-000003b0: 7a69 7070 6564 da09 6669 6c65 5f6e 616d  zipped..file_nam
-000003c0: 65a9 0072 1e00 0000 fa63 2f55 7365 7273  e..r.....c/Users
-000003d0: 2f66 6572 6861 7474 656b 6572 2f69 686b  /ferhatteker/ihk
-000003e0: 5f70 726f 6a65 6b74 2f74 6872 6565 5f64  _projekt/three_d
-000003f0: 5f63 6f6e 7665 7274 6572 2f74 6872 6565  _converter/three
-00000400: 5f64 5f63 6f6e 7665 7274 6572 2f62 6c65  _d_converter/ble
-00000410: 6e64 6572 5f73 6372 6970 7473 2f69 6d70  nder_scripts/imp
-00000420: 6f72 7465 722f 7573 647a 2e70 79da 0b69  orter/usdz.py..i
-00000430: 6d70 6f72 745f 6669 6c65 0a00 0000 7334  mport_file....s4
-00000440: 0000 000a 0104 0114 0106 010c 0102 ff04  ................
-00000450: fe12 0704 010e 0106 ff1c ff12 0514 0108  ................
-00000460: 0106 0108 0102 ff02 0302 0102 0102 0102  ................
-00000470: 0108 f810 0b04 f37a 1855 5344 5a49 6d70  .......z.USDZImp
-00000480: 6f72 7465 722e 696d 706f 7274 5f66 696c  orter.import_fil
-00000490: 6529 06da 085f 5f6e 616d 655f 5fda 0a5f  e)...__name__.._
-000004a0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000004b0: 6c6e 616d 655f 5fda 0770 6174 686c 6962  lname__..pathlib
-000004c0: da04 5061 7468 7220 0000 0072 1e00 0000  ..Pathr ...r....
-000004d0: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-000004e0: 0400 0000 0900 0000 7304 0000 0008 0018  ........s.......
-000004f0: 0172 0400 0000 290a 7224 0000 0072 0a00  .r....).r$...r..
-00000500: 0000 da04 7575 6964 7202 0000 0072 1200  ....uuidr....r..
-00000510: 0000 da1d 626c 656e 6465 725f 7363 7269  ....blender_scri
-00000520: 7074 732e 696d 706f 7274 6572 2e62 6173  pts.importer.bas
-00000530: 6572 0300 0000 720c 0000 0072 1800 0000  er....r....r....
-00000540: 7204 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
-00000550: 1e00 0000 721f 0000 00da 083c 6d6f 6475  ....r......<modu
-00000560: 6c65 3e01 0000 0073 1000 0000 0800 0801  le>....s........
-00000570: 0c01 0801 0c01 0801 0801 1402            ............
+00000120: d600 0000 7400 7401 8300 8301 7d02 7402  ....t.t.....}.t.
+00000130: a003 7400 7c01 8301 7404 6a05 a006 7c00  ..t.|...t.j...|.
+00000140: 6a07 6a08 7c02 6401 1700 a102 a102 0100  j.j.|.d.........
+00000150: 7409 a00a 7400 7c01 8301 6402 a102 8f13  t...t.|...d.....
+00000160: 7d03 7c03 a00b 7404 6a05 a006 7c00 6a07  }.|...t.j...|.j.
+00000170: 6a0c a101 a101 0100 5700 6400 0400 0400  j.......W.d.....
+00000180: 8303 0100 6e08 3100 7334 7701 0100 0100  ....n.1.s4w.....
+00000190: 0100 5900 0100 7404 a00d 7c00 6a07 6a0c  ..Y...t...|.j.j.
+000001a0: a101 4400 5d28 7d04 7c04 a00e 6403 a101  ..D.](}.|...d...
+000001b0: 734c 7c04 a00e 6404 a101 7261 740f 6a10  sL|...d...rat.j.
+000001c0: 6a11 6a12 7404 6a05 a006 7c00 6a07 6a0c  j.j.t.j...|.j.j.
+000001d0: 7c04 a102 6405 6405 6405 6405 6406 6407  |...d.d.d.d.d.d.
+000001e0: 8d06 0100 7140 7413 6408 7c04 9b00 9d02  ....q@t.d.|.....
+000001f0: 8301 0100 7140 6400 5300 2909 4e7a 052e  ....q@d.S.).Nz..
+00000200: 7573 647a da01 727a 052e 7573 6463 7a05  usdz..rz..usdcz.
+00000210: 2e75 7364 6154 5a12 5245 4645 5245 4e43  .usdaTZ.REFERENC
+00000220: 455f 4558 4953 5449 4e47 2906 da08 6669  E_EXISTING)...fi
+00000230: 6c65 7061 7468 5a10 696d 706f 7274 5f6d  lepathZ.import_m
+00000240: 6174 6572 6961 6c73 5a12 696d 706f 7274  aterialsZ.import
+00000250: 5f75 7364 5f70 7265 7669 6577 5a0d 696d  _usd_previewZ.im
+00000260: 706f 7274 5f73 7562 6469 765a 1072 6561  port_subdivZ.rea
+00000270: 645f 6d65 7368 5f63 6f6c 6f72 735a 176d  d_mesh_colorsZ.m
+00000280: 746c 5f6e 616d 655f 636f 6c6c 6973 696f  tl_name_collisio
+00000290: 6e5f 6d6f 6465 7a18 556e 7375 7070 6f72  n_modez.Unsuppor
+000002a0: 7465 6420 6669 6c65 2066 6f72 6d61 7420  ted file format 
+000002b0: 2914 da03 7374 7272 0200 0000 da06 7368  )...strr......sh
+000002c0: 7574 696c da05 636f 7079 32da 026f 73da  util..copy2..os.
+000002d0: 0470 6174 68da 046a 6f69 6eda 0c66 696c  .path..join..fil
+000002e0: 655f 6861 6e64 6c65 72da 1570 6174 685f  e_handler..path_
+000002f0: 746f 5f70 7562 6c69 635f 6d6f 6465 6c73  to_public_models
+00000300: da07 7a69 7066 696c 65da 075a 6970 4669  ..zipfile..ZipFi
+00000310: 6c65 da0a 6578 7472 6163 7461 6c6c da14  le..extractall..
+00000320: 6d6f 6465 6c5f 746d 705f 7061 7468 5f75  model_tmp_path_u
+00000330: 6e7a 6970 da07 6c69 7374 6469 72da 0865  nzip..listdir..e
+00000340: 6e64 7377 6974 68da 0362 7079 da03 6f70  ndswith..bpy..op
+00000350: 73da 0277 6d5a 0a75 7364 5f69 6d70 6f72  s..wmZ.usd_impor
+00000360: 74da 0570 7269 6e74 2905 da04 7365 6c66  t..print)...self
+00000370: 7205 0000 005a 0c6e 6577 6669 6c65 5f70  r....Z.newfile_p
+00000380: 6174 685a 0d75 7364 7a5f 756e 7a69 7070  athZ.usdz_unzipp
+00000390: 6564 da09 6669 6c65 5f6e 616d 65a9 0072  ed..file_name..r
+000003a0: 1d00 0000 fa63 2f55 7365 7273 2f66 6572  .....c/Users/fer
+000003b0: 6861 7474 656b 6572 2f69 686b 5f70 726f  hatteker/ihk_pro
+000003c0: 6a65 6b74 2f74 6872 6565 5f64 5f63 6f6e  jekt/three_d_con
+000003d0: 7665 7274 6572 2f74 6872 6565 5f64 5f63  verter/three_d_c
+000003e0: 6f6e 7665 7274 6572 2f62 6c65 6e64 6572  onverter/blender
+000003f0: 5f73 6372 6970 7473 2f69 6d70 6f72 7465  _scripts/importe
+00000400: 722f 7573 647a 2e70 79da 0b69 6d70 6f72  r/usdz.py..impor
+00000410: 745f 6669 6c65 0a00 0000 7334 0000 000a  t_file....s4....
+00000420: 0104 0106 0106 010c 0102 ff04 fe12 0704  ................
+00000430: 010e 0106 ff1c ff12 0514 0108 0106 0108  ................
+00000440: 0102 ff02 0302 0102 0102 0102 0108 f810  ................
+00000450: 0b04 f37a 1855 5344 5a49 6d70 6f72 7465  ...z.USDZImporte
+00000460: 722e 696d 706f 7274 5f66 696c 6529 06da  r.import_file)..
+00000470: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000480: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000490: 655f 5fda 0770 6174 686c 6962 da04 5061  e__..pathlib..Pa
+000004a0: 7468 721f 0000 0072 1d00 0000 721d 0000  thr....r....r...
+000004b0: 0072 1d00 0000 721e 0000 0072 0400 0000  .r....r....r....
+000004c0: 0900 0000 7304 0000 0008 0018 0172 0400  ....s........r..
+000004d0: 0000 290a 7223 0000 0072 0a00 0000 da04  ..).r#...r......
+000004e0: 7575 6964 7202 0000 0072 1100 0000 da1d  uuidr....r......
+000004f0: 626c 656e 6465 725f 7363 7269 7074 732e  blender_scripts.
+00000500: 696d 706f 7274 6572 2e62 6173 6572 0300  importer.baser..
+00000510: 0000 720c 0000 0072 1700 0000 7204 0000  ..r....r....r...
+00000520: 0072 1d00 0000 721d 0000 0072 1d00 0000  .r....r....r....
+00000530: 721e 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000540: 0000 0073 1000 0000 0800 0801 0c01 0801  ...s............
+00000550: 0c01 0801 0801 1402                      ........
```

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 26 16:01:07 2024 UTC, .py size: 409 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,47 @@
-00000000: 6f0d 0d0a 0000 0000 43f1 0266 9901 0000  o.......C..f....
+00000000: 6f0d 0d0a 0000 0000 51c8 1366 1f01 0000  o.......Q..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6502 8303  Z.G.d.d...d.e...
 00000060: 5a05 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000070: da0d 4d6f 6465 6c49 6d70 6f72 7465 7263  ..ModelImporterc
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0400 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
 000000a0: 0164 005a 0264 0165 036a 0464 0264 0366  .d.Z.d.e.j.d.d.f
 000000b0: 0464 0464 0584 045a 0564 0353 0029 06da  .d.d...Z.d.S.)..
 000000c0: 0b58 3344 496d 706f 7274 6572 da09 6669  .X3DImporter..fi
 000000d0: 6c65 5f70 6174 68da 0672 6574 7572 6e4e  le_path..returnN
 000000e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000000f0: 0006 0000 0043 0000 0073 3400 0000 7c01  .....C...s4...|.
-00000100: 6a00 6401 6b02 7218 7401 6a02 6a03 6a04  j.d.k.r.t.j.j.j.
-00000110: 7405 6a06 a007 7c00 6a08 6a09 740a 7c01  t.j...|.j.j.t.|.
-00000120: 8301 a102 6402 8d01 0100 6400 5300 6400  ....d.....d.S.d.
-00000130: 5300 2903 4e7a 042e 7833 6429 01da 0866  S.).Nz..x3d)...f
-00000140: 696c 6570 6174 6829 0bda 0673 7566 6669  ilepath)...suffi
-00000150: 78da 0362 7079 da03 6f70 73da 0c69 6d70  x..bpy..ops..imp
-00000160: 6f72 745f 7363 656e 655a 0378 3364 da02  ort_sceneZ.x3d..
-00000170: 6f73 da04 7061 7468 da04 6a6f 696e da0c  os..path..join..
-00000180: 6669 6c65 5f68 616e 646c 6572 da14 7061  file_handler..pa
-00000190: 7468 5f74 6f5f 6669 6c65 735f 696e 5f74  th_to_files_in_t
-000001a0: 6d70 da03 7374 7229 02da 0473 656c 6672  mp..str)...selfr
-000001b0: 0400 0000 a900 7212 0000 00fa 622f 5573  ......r.....b/Us
-000001c0: 6572 732f 6665 7268 6174 7465 6b65 722f  ers/ferhatteker/
-000001d0: 6968 6b5f 7072 6f6a 656b 742f 7468 7265  ihk_projekt/thre
-000001e0: 655f 645f 636f 6e76 6572 7465 722f 7468  e_d_converter/th
-000001f0: 7265 655f 645f 636f 6e76 6572 7465 722f  ree_d_converter/
-00000200: 626c 656e 6465 725f 7363 7269 7074 732f  blender_scripts/
-00000210: 696d 706f 7274 6572 2f78 3364 2e70 79da  importer/x3d.py.
-00000220: 0b69 6d70 6f72 745f 6669 6c65 0700 0000  .import_file....
-00000230: 730e 0000 000a 0108 0106 010c 0102 ff0a  s...............
-00000240: ff04 ff7a 1758 3344 496d 706f 7274 6572  ...z.X3DImporter
-00000250: 2e69 6d70 6f72 745f 6669 6c65 2906 da08  .import_file)...
-00000260: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000270: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000280: 5f5f da07 7061 7468 6c69 62da 0450 6174  __..pathlib..Pat
-00000290: 6872 1400 0000 7212 0000 0072 1200 0000  hr....r....r....
-000002a0: 7212 0000 0072 1300 0000 7203 0000 0006  r....r....r.....
-000002b0: 0000 0073 0400 0000 0800 1801 7203 0000  ...s........r...
-000002c0: 0029 0672 1800 0000 da1d 626c 656e 6465  .).r......blende
-000002d0: 725f 7363 7269 7074 732e 696d 706f 7274  r_scripts.import
-000002e0: 6572 2e62 6173 6572 0200 0000 720b 0000  er.baser....r...
-000002f0: 0072 0800 0000 7203 0000 0072 1200 0000  .r....r....r....
-00000300: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00000310: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
-00000320: 0000 0800 0c01 0801 0801 1402            ............
+000000f0: 0003 0000 0043 0000 0073 2600 0000 7c01  .....C...s&...|.
+00000100: 6a00 6401 6b02 7211 7401 6a02 6a03 6a04  j.d.k.r.t.j.j.j.
+00000110: 7405 7c01 8301 6402 8d01 0100 6400 5300  t.|...d.....d.S.
+00000120: 6400 5300 2903 4e7a 042e 7833 6429 01da  d.S.).Nz..x3d)..
+00000130: 0866 696c 6570 6174 6829 06da 0673 7566  .filepath)...suf
+00000140: 6669 78da 0362 7079 da03 6f70 73da 0c69  fix..bpy..ops..i
+00000150: 6d70 6f72 745f 7363 656e 655a 0378 3364  mport_sceneZ.x3d
+00000160: da03 7374 7229 02da 0473 656c 6672 0400  ..str)...selfr..
+00000170: 0000 a900 720d 0000 00fa 622f 5573 6572  ....r.....b/User
+00000180: 732f 6665 7268 6174 7465 6b65 722f 6968  s/ferhatteker/ih
+00000190: 6b5f 7072 6f6a 656b 742f 7468 7265 655f  k_projekt/three_
+000001a0: 645f 636f 6e76 6572 7465 722f 7468 7265  d_converter/thre
+000001b0: 655f 645f 636f 6e76 6572 7465 722f 626c  e_d_converter/bl
+000001c0: 656e 6465 725f 7363 7269 7074 732f 696d  ender_scripts/im
+000001d0: 706f 7274 6572 2f78 3364 2e70 79da 0b69  porter/x3d.py..i
+000001e0: 6d70 6f72 745f 6669 6c65 0700 0000 7306  mport_file....s.
+000001f0: 0000 000a 0118 0104 ff7a 1758 3344 496d  .........z.X3DIm
+00000200: 706f 7274 6572 2e69 6d70 6f72 745f 6669  porter.import_fi
+00000210: 6c65 2906 da08 5f5f 6e61 6d65 5f5f da0a  le)...__name__..
+00000220: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000230: 616c 6e61 6d65 5f5f da07 7061 7468 6c69  alname__..pathli
+00000240: 62da 0450 6174 6872 0f00 0000 720d 0000  b..Pathr....r...
+00000250: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00000260: 7203 0000 0006 0000 0073 0400 0000 0800  r........s......
+00000270: 1801 7203 0000 0029 0672 1300 0000 da1d  ..r....).r......
+00000280: 626c 656e 6465 725f 7363 7269 7074 732e  blender_scripts.
+00000290: 696d 706f 7274 6572 2e62 6173 6572 0200  importer.baser..
+000002a0: 0000 da02 6f73 7208 0000 0072 0300 0000  ....osr....r....
+000002b0: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+000002c0: 0e00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000002d0: 0000 730a 0000 0008 000c 0108 0108 0114  ..s.............
+000002e0: 02                                       .
```

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/factory.py` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/factory.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/importer/usdz.py` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/importer/usdz.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import bpy
 
 class USDZImporter(ModelImporter):
     def import_file(self, file_path: pathlib.Path) -> None:
         newfile_path: str = str(uuid4())
         shutil.copy2(
-            os.path.join(self.file_handler.path_to_files_in_tmp, str(file_path)),
+            str(file_path),
             os.path.join(
                 self.file_handler.path_to_public_models, newfile_path + ".usdz"
             ),
         )
 
         with zipfile.ZipFile(str(file_path), "r") as usdz_unzipped:
             usdz_unzipped.extractall(
```

### Comparing `three_d_converter-0.1.0/three_d_converter/blender_scripts/main.py` & `three_d_converter-0.1.1/three_d_converter/blender_scripts/main.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.0/three_d_converter/converter.py` & `three_d_converter-0.1.1/three_d_converter/converter.py`

 * *Files identical despite different names*

