# Comparing `tmp/pycitysim-1.12.1.tar.gz` & `tmp/pycitysim-1.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycitysim-1.12.1.tar", last modified: Sun Apr  7 14:04:27 2024, max compression
+gzip compressed data, was "pycitysim-1.12.2.tar", last modified: Mon Apr  8 03:53:56 2024, max compression
```

## Comparing `pycitysim-1.12.1.tar` & `pycitysim-1.12.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.887297 pycitysim-1.12.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-07 14:04:19.000000 pycitysim-1.12.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-07 14:04:27.887297 pycitysim-1.12.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-07 14:04:19.000000 pycitysim-1.12.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.879298 pycitysim-1.12.1/pycitysim/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.883298 pycitysim-1.12.1/pycitysim/apphub/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/apphub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/apphub/apphub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.883298 pycitysim-1.12.1/pycitysim/map/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35545 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/map/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.883298 pycitysim-1.12.1/pycitysim/routing/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/routing/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.883298 pycitysim-1.12.1/pycitysim/sidecar/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sidecar/sidecar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.887297 pycitysim-1.12.1/pycitysim/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/aoi_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/clock_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/economy_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/lane_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/light_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/person_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/road_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/social_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.887297 pycitysim-1.12.1/pycitysim/urbankg/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/urbankg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/urbankg/kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.887297 pycitysim-1.12.1/pycitysim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/utils/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/utils/grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/utils/protobuf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.887297 pycitysim-1.12.1/pycitysim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-07 14:04:27.000000 pycitysim-1.12.1/pycitysim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-07 14:04:27.000000 pycitysim-1.12.1/pycitysim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:04:27.000000 pycitysim-1.12.1/pycitysim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-07 14:04:27.000000 pycitysim-1.12.1/pycitysim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 14:04:27.000000 pycitysim-1.12.1/pycitysim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:04:27.887297 pycitysim-1.12.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.763809 pycitysim-1.12.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 03:53:49.000000 pycitysim-1.12.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-08 03:53:56.763809 pycitysim-1.12.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-08 03:53:49.000000 pycitysim-1.12.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.755808 pycitysim-1.12.2/pycitysim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.759809 pycitysim-1.12.2/pycitysim/apphub/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/apphub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/apphub/apphub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.759809 pycitysim-1.12.2/pycitysim/map/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35545 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/map/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.759809 pycitysim-1.12.2/pycitysim/routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/routing/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.759809 pycitysim-1.12.2/pycitysim/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sidecar/sidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.763809 pycitysim-1.12.2/pycitysim/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/aoi_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/clock_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/economy_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/lane_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/light_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/person_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/road_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/social_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.763809 pycitysim-1.12.2/pycitysim/urbankg/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/urbankg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/urbankg/kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.763809 pycitysim-1.12.2/pycitysim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/utils/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/utils/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/utils/protobuf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.763809 pycitysim-1.12.2/pycitysim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-08 03:53:56.000000 pycitysim-1.12.2/pycitysim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-08 03:53:56.000000 pycitysim-1.12.2/pycitysim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:53:56.000000 pycitysim-1.12.2/pycitysim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 03:53:56.000000 pycitysim-1.12.2/pycitysim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 03:53:56.000000 pycitysim-1.12.2/pycitysim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 03:53:56.763809 pycitysim-1.12.2/setup.cfg
```

### Comparing `pycitysim-1.12.1/LICENSE` & `pycitysim-1.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/PKG-INFO` & `pycitysim-1.12.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycitysim
-Version: 1.12.1
+Version: 1.12.2
 Summary: City Simulator and OpenCity Databases Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycitysim-1.12.1/README.md` & `pycitysim-1.12.2/README.md`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/__init__.py` & `pycitysim-1.12.2/pycitysim/__init__.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/apphub/apphub.py` & `pycitysim-1.12.2/pycitysim/apphub/apphub.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,23 +168,24 @@
         - agent_id: 绑定后的agent ID。the bound agent ID.
 
         Raises:
         - Exception: 绑定失败。Binding failed.
         """
         return self._bind(org_id, "org", name, avatar)
     
-    def bind_func(self, name:str, avatar:Image):
+    def bind_func(self, func_id:int, name:str, avatar:Image):
         """
         插入非模拟器相关的智能体——func类型智能体
 
         Args:
+        - func_id (str): 该智能体的编号——唯一
         - name (str): 该智能体的名字
         - avatar (Image): 该智能体的头像
         """
-        return self._bind(-1, "func", name, avatar)
+        return self._bind(func_id+10000000, "func", name, avatar)
 
     def release_agent(self, agent_id: int) -> bool:
         """
         释放agent(person/org), 释放后agent将不再被访问并允许其他app绑定
         Release the agent (person/org). After the release, the agent will no longer be accessed and allows other apps to bind.
 
         Args:
```

### Comparing `pycitysim-1.12.1/pycitysim/map/map.py` & `pycitysim-1.12.2/pycitysim/map/map.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/routing/client.py` & `pycitysim-1.12.2/pycitysim/routing/client.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sidecar/sidecar.py` & `pycitysim-1.12.2/pycitysim/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sim/__init__.py` & `pycitysim-1.12.2/pycitysim/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sim/aoi_service.py` & `pycitysim-1.12.2/pycitysim/sim/aoi_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sim/client.py` & `pycitysim-1.12.2/pycitysim/sim/client.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sim/clock_service.py` & `pycitysim-1.12.2/pycitysim/sim/clock_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sim/economy_services.py` & `pycitysim-1.12.2/pycitysim/sim/economy_services.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sim/event_service.py` & `pycitysim-1.12.2/pycitysim/sim/event_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sim/lane_service.py` & `pycitysim-1.12.2/pycitysim/sim/lane_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sim/light_service.py` & `pycitysim-1.12.2/pycitysim/sim/light_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sim/person_service.py` & `pycitysim-1.12.2/pycitysim/sim/person_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sim/road_service.py` & `pycitysim-1.12.2/pycitysim/sim/road_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/sim/social_service.py` & `pycitysim-1.12.2/pycitysim/sim/social_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/urbankg/kg.py` & `pycitysim-1.12.2/pycitysim/urbankg/kg.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/utils/geojson.py` & `pycitysim-1.12.2/pycitysim/utils/geojson.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/utils/grpc.py` & `pycitysim-1.12.2/pycitysim/utils/grpc.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim/utils/protobuf.py` & `pycitysim-1.12.2/pycitysim/utils/protobuf.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pycitysim.egg-info/PKG-INFO` & `pycitysim-1.12.2/pycitysim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycitysim
-Version: 1.12.1
+Version: 1.12.2
 Summary: City Simulator and OpenCity Databases Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycitysim-1.12.1/pycitysim.egg-info/SOURCES.txt` & `pycitysim-1.12.2/pycitysim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.1/pyproject.toml` & `pycitysim-1.12.2/pyproject.toml`

 * *Files identical despite different names*

