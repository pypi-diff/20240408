# Comparing `tmp/MinecraftMotionTools-1.8.1.tar.gz` & `tmp/MinecraftMotionTools-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MinecraftMotionTools-1.8.1.tar", last modified: Sun Apr  7 09:34:41 2024, max compression
+gzip compressed data, was "MinecraftMotionTools-1.8.2.tar", last modified: Mon Apr  8 12:36:15 2024, max compression
```

## Comparing `MinecraftMotionTools-1.8.1.tar` & `MinecraftMotionTools-1.8.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-07 09:34:41.341058 MinecraftMotionTools-1.8.1/
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     1083 2024-04-07 09:33:06.000000 MinecraftMotionTools-1.8.1/LICENSE
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6889 2024-04-07 09:34:41.331228 MinecraftMotionTools-1.8.1/PKG-INFO
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6581 2024-04-07 09:33:06.000000 MinecraftMotionTools-1.8.1/README.md
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      481 2024-04-07 09:34:02.000000 MinecraftMotionTools-1.8.1/pyproject.toml
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       38 2024-04-07 09:34:41.343066 MinecraftMotionTools-1.8.1/setup.cfg
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-07 09:34:41.000787 MinecraftMotionTools-1.8.1/src/
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-07 09:34:41.319168 MinecraftMotionTools-1.8.1/src/MinecraftMotionTools.egg-info/
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6889 2024-04-07 09:34:40.000000 MinecraftMotionTools-1.8.1/src/MinecraftMotionTools.egg-info/PKG-INFO
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      392 2024-04-07 09:34:40.000000 MinecraftMotionTools-1.8.1/src/MinecraftMotionTools.egg-info/SOURCES.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        1 2024-04-07 09:34:40.000000 MinecraftMotionTools-1.8.1/src/MinecraftMotionTools.egg-info/dependency_links.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       14 2024-04-07 09:34:40.000000 MinecraftMotionTools-1.8.1/src/MinecraftMotionTools.egg-info/requires.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       23 2024-04-07 09:34:40.000000 MinecraftMotionTools-1.8.1/src/MinecraftMotionTools.egg-info/top_level.txt
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-07 09:34:41.284145 MinecraftMotionTools-1.8.1/src/minecraft_motion_tools/
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      669 2024-04-07 09:33:06.000000 MinecraftMotionTools-1.8.1/src/minecraft_motion_tools/__init__.py
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    12044 2024-04-07 09:33:57.000000 MinecraftMotionTools-1.8.1/src/minecraft_motion_tools/acceleration.py
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    10267 2024-04-07 09:33:06.000000 MinecraftMotionTools-1.8.1/src/minecraft_motion_tools/velocity.py
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-08 12:36:15.029439 MinecraftMotionTools-1.8.2/
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     1083 2024-04-08 11:39:56.000000 MinecraftMotionTools-1.8.2/LICENSE
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6889 2024-04-08 12:36:15.020782 MinecraftMotionTools-1.8.2/PKG-INFO
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6581 2024-04-08 11:39:56.000000 MinecraftMotionTools-1.8.2/README.md
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      481 2024-04-08 11:40:04.000000 MinecraftMotionTools-1.8.2/pyproject.toml
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       38 2024-04-08 12:36:15.030513 MinecraftMotionTools-1.8.2/setup.cfg
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-08 12:36:14.748809 MinecraftMotionTools-1.8.2/src/
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-08 12:36:15.007479 MinecraftMotionTools-1.8.2/src/MinecraftMotionTools.egg-info/
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6889 2024-04-08 12:36:14.000000 MinecraftMotionTools-1.8.2/src/MinecraftMotionTools.egg-info/PKG-INFO
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      392 2024-04-08 12:36:14.000000 MinecraftMotionTools-1.8.2/src/MinecraftMotionTools.egg-info/SOURCES.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        1 2024-04-08 12:36:14.000000 MinecraftMotionTools-1.8.2/src/MinecraftMotionTools.egg-info/dependency_links.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       14 2024-04-08 12:36:14.000000 MinecraftMotionTools-1.8.2/src/MinecraftMotionTools.egg-info/requires.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       23 2024-04-08 12:36:14.000000 MinecraftMotionTools-1.8.2/src/MinecraftMotionTools.egg-info/top_level.txt
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-08 12:36:14.975062 MinecraftMotionTools-1.8.2/src/minecraft_motion_tools/
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      669 2024-04-08 11:39:56.000000 MinecraftMotionTools-1.8.2/src/minecraft_motion_tools/__init__.py
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    12743 2024-04-08 12:33:38.000000 MinecraftMotionTools-1.8.2/src/minecraft_motion_tools/acceleration.py
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    10267 2024-04-08 11:39:56.000000 MinecraftMotionTools-1.8.2/src/minecraft_motion_tools/velocity.py
```

### Comparing `MinecraftMotionTools-1.8.1/LICENSE` & `MinecraftMotionTools-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MinecraftMotionTools-1.8.1/PKG-INFO` & `MinecraftMotionTools-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinecraftMotionTools
-Version: 1.8.1
+Version: 1.8.2
 Summary: A library to compute entities' motion in Minecraft.
 Author: OrHy3
 Project-URL: Homepage, https://github.com/OrHy3/MinecraftMotionTools
 Project-URL: Issues, https://github.com/OrHy3/MinecraftMotionTools/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MinecraftMotionTools-1.8.1/README.md` & `MinecraftMotionTools-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `MinecraftMotionTools-1.8.1/src/MinecraftMotionTools.egg-info/PKG-INFO` & `MinecraftMotionTools-1.8.2/src/MinecraftMotionTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinecraftMotionTools
-Version: 1.8.1
+Version: 1.8.2
 Summary: A library to compute entities' motion in Minecraft.
 Author: OrHy3
 Project-URL: Homepage, https://github.com/OrHy3/MinecraftMotionTools
 Project-URL: Issues, https://github.com/OrHy3/MinecraftMotionTools/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MinecraftMotionTools-1.8.1/src/minecraft_motion_tools/__init__.py` & `MinecraftMotionTools-1.8.2/src/minecraft_motion_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `MinecraftMotionTools-1.8.1/src/minecraft_motion_tools/acceleration.py` & `MinecraftMotionTools-1.8.2/src/minecraft_motion_tools/acceleration.py`

 * *Files 6% similar despite different names*

```diff
@@ -250,14 +250,17 @@
             return None
         return (a,)
     if after:
         k /= 1 - d
     if 1 + k * d == 0:
         return None
     a = solve_equation(1, v1 * d, v2 * d, (1 - d) ** ((v2 - v1 + (p2 - p1) * d) / (1 + k * d)))
+    for i in range(len(a) - 1, -1):
+        if math.log(1 - d) * (v1 / a + 1 / d) / (1 + k * d) * (1 - d) ** (((v1 + p1 * d) / a + 1 / d) / (1 + k * d)) * math.e < -1 or math.log(1 - d) * (v2 / a + 1 / d) / (1 + k * d) * (1 - d) ** (((v2 + p2 * d) / a + 1 / d) / (1 + k * d)) * math.e < -1:
+            a.pop(i)
     if a == []:
         return None
     if after:
         a = [sol / (1 - d) for sol in a]
     return tuple(a)
 
 def a_from_v_t_p_t(first: tuple, second: tuple, d=0.050000011920928955, after=True, k=0):
@@ -322,14 +325,17 @@
         return tuple(a)
     if after:
         k /= 1 - d
     if 1 + k * d == 0:
         return None
     gamma = (1 - d) ** (((1 - d) ** -t1 - 1) / d / (1 + k * d) - t1)
     a = solve_equation(gamma, gamma * v1 * d, v2 * d, (1 - d) ** ((v2 - v1 * (1 - d) ** -t1 + p2 * d) / (1 + k * d)))
+    for i in range(len(a) - 1, -1):
+        if math.log(1 - d) * (v2 / a + 1 / d) / (1 + k * d) * (1 - d) ** (((v2 + p2 * d) / a + 1 / d) / (1 + k * d)) * math.e < -1:
+            a.pop(i)
     if a == []:
         return None
     if after:
         a = [sol / (1 - d) for sol in a]
     return tuple(a)
 
 def a_from_p_t_v_p(first: tuple, second: tuple, d=0.050000011920928955, after=True, k=0):
@@ -366,12 +372,15 @@
     if 1 + k * d == 0:
         return None
     arg = 1 - (1 - d) ** t1
     if arg == 0:
         return None
     gamma = (1 - d) ** (t1 / arg - 1 / d / (1 + k * d)) * d / arg
     a = solve_equation(gamma * (1 + k * d) * t1, gamma * p1 * d, v2 * d, (1 - d) ** ((v2 + (p2 - p1 / arg) * d) / (1 + k * d)))
+    for i in range(len(a) - 1, -1):
+        if math.log(1 - d) * (v2 / a + 1 / d) / (1 + k * d) * (1 - d) ** (((v2 + p2 * d) / a + 1 / d) / (1 + k * d)) * math.e < -1:
+            a.pop(i)
     if a == []:
         return None
     if after:
         a = [sol / (1 - d) for sol in a]
     return tuple(a)
```

### Comparing `MinecraftMotionTools-1.8.1/src/minecraft_motion_tools/velocity.py` & `MinecraftMotionTools-1.8.2/src/minecraft_motion_tools/velocity.py`

 * *Files identical despite different names*
