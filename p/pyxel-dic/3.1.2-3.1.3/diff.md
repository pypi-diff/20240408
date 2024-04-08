# Comparing `tmp/pyxel-dic-3.1.2.tar.gz` & `tmp/pyxel-dic-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxel-dic-3.1.2.tar", last modified: Thu Mar  7 16:20:58 2024, max compression
+gzip compressed data, was "pyxel-dic-3.1.3.tar", last modified: Mon Apr  8 13:09:18 2024, max compression
```

## Comparing `pyxel-dic-3.1.2.tar` & `pyxel-dic-3.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 16:20:58.108477 pyxel-dic-3.1.2/
--rw-rw-rw-   0        0        0     3197 2023-04-17 15:11:38.000000 pyxel-dic-3.1.2/LICENSE
--rw-rw-rw-   0        0        0     8950 2024-03-07 16:20:58.100463 pyxel-dic-3.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4247 2023-12-14 07:13:45.000000 pyxel-dic-3.1.2/README.md
--rw-rw-rw-   0        0        0      833 2024-03-07 16:19:53.000000 pyxel-dic-3.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      898 2024-03-07 16:20:58.112432 pyxel-dic-3.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-07 16:20:57.836589 pyxel-dic-3.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-07 16:20:58.048149 pyxel-dic-3.1.2/src/pyxel/
--rw-rw-rw-   0        0        0      409 2023-09-26 15:49:25.000000 pyxel-dic-3.1.2/src/pyxel/__init__.py
--rw-rw-rw-   0        0        0    29337 2023-10-10 15:10:56.000000 pyxel-dic-3.1.2/src/pyxel/bspline_patch.py
--rw-rw-rw-   0        0        0    41545 2023-10-10 15:14:01.000000 pyxel-dic-3.1.2/src/pyxel/bspline_routines.py
--rw-rw-rw-   0        0        0    31260 2023-12-01 13:11:54.000000 pyxel-dic-3.1.2/src/pyxel/camera.py
--rw-rw-rw-   0        0        0    25572 2024-01-24 15:55:48.000000 pyxel-dic-3.1.2/src/pyxel/dic.py
--rw-rw-rw-   0        0        0     2317 2023-12-14 15:57:00.000000 pyxel-dic-3.1.2/src/pyxel/exportpixmap.py
--rw-rw-rw-   0        0        0    15430 2024-01-23 18:19:07.000000 pyxel-dic-3.1.2/src/pyxel/image.py
--rw-rw-rw-   0        0        0     9658 2023-04-17 15:11:38.000000 pyxel-dic-3.1.2/src/pyxel/levelset.py
--rw-rw-rw-   0        0        0     5908 2024-03-06 07:09:44.000000 pyxel-dic-3.1.2/src/pyxel/material.py
--rw-rw-rw-   0        0        0   136656 2024-03-07 15:46:09.000000 pyxel-dic-3.1.2/src/pyxel/mesh.py
--rw-rw-rw-   0        0        0    24345 2024-02-09 21:11:50.000000 pyxel-dic-3.1.2/src/pyxel/mesher.py
--rw-rw-rw-   0        0        0     6859 2023-04-17 15:11:38.000000 pyxel-dic-3.1.2/src/pyxel/meshparser.py
--rw-rw-rw-   0        0        0     3926 2024-01-23 18:23:13.000000 pyxel-dic-3.1.2/src/pyxel/utils.py
--rw-rw-rw-   0        0        0    16353 2023-04-17 15:11:38.000000 pyxel-dic-3.1.2/src/pyxel/vtktools.py
-drwxrwxrwx   0        0        0        0 2024-03-07 16:20:58.093996 pyxel-dic-3.1.2/src/pyxel_dic.egg-info/
--rw-rw-rw-   0        0        0     8950 2024-03-07 16:20:57.000000 pyxel-dic-3.1.2/src/pyxel_dic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2024-03-07 16:20:57.000000 pyxel-dic-3.1.2/src/pyxel_dic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 16:20:57.000000 pyxel-dic-3.1.2/src/pyxel_dic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-03-07 16:20:57.000000 pyxel-dic-3.1.2/src/pyxel_dic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-07 16:20:57.000000 pyxel-dic-3.1.2/src/pyxel_dic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 13:09:18.807938 pyxel-dic-3.1.3/
+-rw-rw-rw-   0        0        0     3197 2023-04-17 15:11:38.000000 pyxel-dic-3.1.3/LICENSE
+-rw-rw-rw-   0        0        0     8950 2024-04-08 13:09:18.799238 pyxel-dic-3.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4247 2023-12-14 07:13:45.000000 pyxel-dic-3.1.3/README.md
+-rw-rw-rw-   0        0        0      833 2024-04-08 13:07:36.000000 pyxel-dic-3.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      898 2024-04-08 13:09:18.811027 pyxel-dic-3.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 13:09:18.540295 pyxel-dic-3.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 13:09:18.745679 pyxel-dic-3.1.3/src/pyxel/
+-rw-rw-rw-   0        0        0      409 2023-09-26 15:49:25.000000 pyxel-dic-3.1.3/src/pyxel/__init__.py
+-rw-rw-rw-   0        0        0    29337 2023-10-10 15:10:56.000000 pyxel-dic-3.1.3/src/pyxel/bspline_patch.py
+-rw-rw-rw-   0        0        0    41545 2023-10-10 15:14:01.000000 pyxel-dic-3.1.3/src/pyxel/bspline_routines.py
+-rw-rw-rw-   0        0        0    32075 2024-03-21 10:29:35.000000 pyxel-dic-3.1.3/src/pyxel/camera.py
+-rw-rw-rw-   0        0        0    25572 2024-03-20 21:54:51.000000 pyxel-dic-3.1.3/src/pyxel/dic.py
+-rw-rw-rw-   0        0        0     2317 2023-12-14 15:57:00.000000 pyxel-dic-3.1.3/src/pyxel/exportpixmap.py
+-rw-rw-rw-   0        0        0    15430 2024-01-23 18:19:07.000000 pyxel-dic-3.1.3/src/pyxel/image.py
+-rw-rw-rw-   0        0        0     9658 2023-04-17 15:11:38.000000 pyxel-dic-3.1.3/src/pyxel/levelset.py
+-rw-rw-rw-   0        0        0     5908 2024-03-06 07:09:44.000000 pyxel-dic-3.1.3/src/pyxel/material.py
+-rw-rw-rw-   0        0        0   139712 2024-04-08 13:01:41.000000 pyxel-dic-3.1.3/src/pyxel/mesh.py
+-rw-rw-rw-   0        0        0    24345 2024-02-09 21:11:50.000000 pyxel-dic-3.1.3/src/pyxel/mesher.py
+-rw-rw-rw-   0        0        0     6859 2023-04-17 15:11:38.000000 pyxel-dic-3.1.3/src/pyxel/meshparser.py
+-rw-rw-rw-   0        0        0     3926 2024-01-23 18:23:13.000000 pyxel-dic-3.1.3/src/pyxel/utils.py
+-rw-rw-rw-   0        0        0    16353 2023-04-17 15:11:38.000000 pyxel-dic-3.1.3/src/pyxel/vtktools.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:09:18.793199 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/
+-rw-rw-rw-   0        0        0     8950 2024-04-08 13:09:18.000000 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2024-04-08 13:09:18.000000 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 13:09:18.000000 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-08 13:09:18.000000 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-08 13:09:18.000000 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/top_level.txt
```

### Comparing `pyxel-dic-3.1.2/LICENSE` & `pyxel-dic-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/PKG-INFO` & `pyxel-dic-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-dic
-Version: 3.1.2
+Version: 3.1.3
 Summary: Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics
 Home-page: https://github.com/jcpassieux/pyxel
 Author: Jean-Charles Passieux
 Author-email: JC Passieux <jc.passieux@gmail.com>
 License: 
           CeCILL FREE SOFTWARE LICENSE AGREEMENT
```

### Comparing `pyxel-dic-3.1.2/README.md` & `pyxel-dic-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/pyproject.toml` & `pyxel-dic-3.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools==68.2.2",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyxel-dic"
-version = "3.1.2"
+version = "3.1.3"
 authors = [
   { name="JC Passieux", email="jc.passieux@gmail.com" },
 ]
 description = "Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyxel-dic-3.1.2/setup.cfg` & `pyxel-dic-3.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel/bspline_patch.py` & `pyxel-dic-3.1.3/src/pyxel/bspline_patch.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel/bspline_routines.py` & `pyxel-dic-3.1.3/src/pyxel/bspline_routines.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel/camera.py` & `pyxel-dic-3.1.3/src/pyxel/camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,26 +416,48 @@
         # import sympy as sp
         # f, tx, ty, rz, u0, v0, r1, X, Y = sp.symbols('f, tx, ty, rz, u0, v0, r1, X, Y', real=True)
         # u = f * (sp.sin(rz) * X - sp.cos(rz) * Y - ty)
         # v = f * (sp.cos(rz) * X + sp.sin(rz) * Y + tx)
         # rho2 = (u-u0)**2 + (v-v0)**2
         # ud = (u - u0) * (1 + r1*rho2) + u0 
         # vd = (v - v0) * (1 + r1*rho2) + v0
-        # sp.pycode(sp.diff(vd, Y))
+        # list_nulle = (sp.diff(ud, X), sp.diff(ud, Y), sp.diff(vd, X), sp.diff(vd, Y))
+        # variable_namer = sp.numbered_symbols('v')
+        # replacements, reduced = sp.cse(list_nulle, symbols=variable_namer)
+        # for key, val in replacements:
+        #     print(key, '=', sp.pycode(val))
+        # for i, r in enumerate(reduced):
+        #     print('deriv[{}]'.format(i), '=', sp.pycode(r))
         f = self.f
         tx = self.tx
         ty = self.ty
         rz = self.rz
         u0 = self.u0
         v0 = self.v0
         r1 = self.r1
-        dudx = f*(r1*((f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)**2 + (f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)**2) + 1)*np.sin(rz) + r1*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*(2*f*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*np.sin(rz) + 2*f*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*np.cos(rz))
-        dudy = -f*(r1*((f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)**2 + (f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)**2) + 1)*np.cos(rz) + r1*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*(-2*f*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*np.cos(rz) + 2*f*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*np.sin(rz))
-        dvdx = f*(r1*((f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)**2 + (f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)**2) + 1)*np.cos(rz) + r1*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*(2*f*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*np.sin(rz) + 2*f*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*np.cos(rz))
-        dvdy = f*(r1*((f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)**2 + (f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)**2) + 1)*np.sin(rz) + r1*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*(-2*f*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*np.cos(rz) + 2*f*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*np.sin(rz))
+        v0 = np.sin(rz)
+        v1 = np.cos(rz)
+        v2 = f*(X*v1 + Y*v0 + tx) - v0
+        v3 = f*(X*v0 - Y*v1 - ty) - u0
+        v4 = f*(r1*(v2**2 + v3**2) + 1)
+        v5 = v0*v4
+        v6 = 2*f
+        v7 = v3*v6
+        v8 = v0*v7 + v1*v2*v6
+        v9 = v1*v4
+        v10 = 2*f*v0*v2 - v1*v7
+        v11 = r1*v2
+        dudx = r1*v3*v8 + v5
+        dudy = r1*v10*v3 - v9
+        dvdx = v11*v8 + v9
+        dvdy = v10*v11 + v5
+        # dudx = f*(r1*((f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)**2 + (f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)**2) + 1)*np.sin(rz) + r1*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*(2*f*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*np.sin(rz) + 2*f*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*np.cos(rz))
+        # dudy = -f*(r1*((f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)**2 + (f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)**2) + 1)*np.cos(rz) + r1*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*(-2*f*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*np.cos(rz) + 2*f*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*np.sin(rz))
+        # dvdx = f*(r1*((f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)**2 + (f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)**2) + 1)*np.cos(rz) + r1*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*(2*f*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*np.sin(rz) + 2*f*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*np.cos(rz))
+        # dvdy = f*(r1*((f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)**2 + (f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)**2) + 1)*np.sin(rz) + r1*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*(-2*f*(f*(X*np.sin(rz) - Y*np.cos(rz) - ty) - u0)*np.cos(rz) + 2*f*(f*(X*np.cos(rz) + Y*np.sin(rz) + tx) - v0)*np.sin(rz))
         return dudx, dudy, dvdx, dvdy
 
     def dPdp(self, X, Y):
         """
         First order derivative of the Camera model wrt camera parameters p
 
         Parameters
```

### Comparing `pyxel-dic-3.1.2/src/pyxel/dic.py` & `pyxel-dic-3.1.3/src/pyxel/dic.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel/exportpixmap.py` & `pyxel-dic-3.1.3/src/pyxel/exportpixmap.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel/image.py` & `pyxel-dic-3.1.3/src/pyxel/image.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel/levelset.py` & `pyxel-dic-3.1.3/src/pyxel/levelset.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel/material.py` & `pyxel-dic-3.1.3/src/pyxel/material.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel/mesh.py` & `pyxel-dic-3.1.3/src/pyxel/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1424,42 +1424,52 @@
                 eet = self.e[et]
                 x1 = u[eet[:, 0]]
                 y1 = v[eet[:, 0]]
                 z1 = w[eet[:, 0]]
                 x2 = u[eet[:, 1]]
                 y2 = v[eet[:, 1]]
                 z2 = w[eet[:, 1]]
-                x3 = u[eet[:, 2]]
-                y3 = v[eet[:, 2]]
-                z3 = w[eet[:, 2]]
-                x4 = u[eet[:, 3]]
-                y4 = v[eet[:, 3]]
-                z4 = w[eet[:, 3]]
-                l1 = np.sqrt((x1-x4)**2 + (y1-y4)**2 + (z1-z4)**2)
-                l2 = np.sqrt((x1-x3)**2 + (y1-y3)**2 + (z1-z3)**2)
-                l3 = np.sqrt((x1-x2)**2 + (y1-y2)**2 + (z1-z2)**2)
-                aes = np.append(aes, np.hstack((l1, l2, l3)))
-            if method == 'max':
-                return np.mean(aes) + np.std(aes) * 0.5
-            elif method == 'min':
-                return np.mean(aes) - np.std(aes) * 0.5
-            elif method == 'mean':
-                return np.mean(aes)
+                if et != 1: # tetraedral elements
+                    x3 = u[eet[:, 2]]
+                    y3 = v[eet[:, 2]]
+                    z3 = w[eet[:, 2]]
+                    if et != 2:
+                        x4 = u[eet[:, 3]]
+                        y4 = v[eet[:, 3]]
+                        z4 = w[eet[:, 3]]
+                        l1 = np.sqrt((x1-x4)**2 + (y1-y4)**2 + (z1-z4)**2)
+                        l2 = np.sqrt((x1-x3)**2 + (y1-y3)**2 + (z1-z3)**2)
+                        l3 = np.sqrt((x1-x2)**2 + (y1-y2)**2 + (z1-z2)**2)
+                        aes = np.append(aes, np.hstack((l1, l2, l3)))
+                    else:
+                        l2 = np.sqrt((x1-x3)**2 + (y1-y3)**2 + (z1-z3)**2)
+                        l3 = np.sqrt((x1-x2)**2 + (y1-y2)**2 + (z1-z2)**2)
+                        aes = np.append(aes, np.hstack((l2, l3)))
+                else: # bar/beam elements
+                    aes = np.sqrt((x1-x2)**2 + (y1-y2)**2 + (z1-z2)**2)
+                if method == 'max':
+                    return np.mean(aes) + np.std(aes) * 0.5
+                elif method == 'min':
+                    return np.mean(aes) - np.std(aes) * 0.5
+                elif method == 'mean':
+                    return np.mean(aes)
         else:   # 2D
             if cam is None:
                 u = self.n[:, 0]
                 v = self.n[:, 1]
             else:
                 u, v = cam.P(self.n[:, 0], self.n[:, 1])
             aes = []
             for et in self.e.keys():
                 if et in [2, 9]:
                     rep = np.arange(3)
                 elif et in [3, 10, 16]:
                     rep = np.arange(4)
+                elif et in [1]:
+                    rep = np.arange(2)
                 um = u[self.e[et][:, rep]] - np.mean(u[self.e[et][:, rep]], axis=1)[:, np.newaxis]
                 vm = v[self.e[et][:, rep]] - np.mean(v[self.e[et][:, rep]], axis=1)[:, np.newaxis]
                 if method == 'max':
                     aes = np.append(aes,
                                     np.max(np.sqrt(um**2 + vm**2), axis=1)
                                     )
                 elif method == 'min':
@@ -2107,38 +2117,32 @@
         eps = 1e-12
         if gp_field.ndim == 2:  # strain or stress field with 2 or 3 components
             if self.dim == 2: # dim 2
                 wx = np.sum(m.phix, axis=0).A[0] + eps
                 wy = np.sum(m.phiy, axis=0).A[0] + eps
                 dof_field = diags(1/wx) @ m.phix.T @ gp_field[:, 0] +\
                             diags(1/wy) @ m.phiy.T @ gp_field[:, 1]
-            elif len(gp_field) == 3:  # dim 3
+            else:  # dim 3
                 wx = np.sum(m.phix, axis=0).A[0] + eps
                 wy = np.sum(m.phiy, axis=0).A[0] + eps
                 wz = np.sum(m.phiz, axis=0).A[0] + eps
                 dof_field = diags(1/wx) @ m.phix.T @ gp_field[:, 0] +\
                             diags(1/wy) @ m.phiy.T @ gp_field[:, 1] +\
                             diags(1/wz) @ m.phiz.T @ gp_field[:, 2]
         else:  # only one comp.
             wx = np.sum(m.phix, axis=0).A[0] + eps
             dof_field = diags(1/wx) @ m.phix.T @ gp_field
         return dof_field
 
     def StrainAtNodes(self, U):
         eps_normal, eps_shear = self.StrainAtGP(U)
-        if self.dim == 2:
-            eps_normal = self.GP2DOF(eps_normal)
-            eps_normal = self.DOF2Nodes(eps_normal)
-            eps_shear = self.GP2DOF(eps_shear)
-            eps_shear = self.DOF2Nodes(eps_shear)
-        else:   # dim 3
-            eps_normal = self.GP2DOF(eps_normal)
-            eps_normal = self.DOF2Nodes(eps_normal)
-            eps_shear = self.GP2DOF(eps_shear)
-            eps_shear = self.DOF2Nodes(eps_shear)
+        eps_normal = self.GP2DOF(eps_normal)
+        eps_normal = self.DOF2Nodes(eps_normal)
+        eps_shear = self.GP2DOF(eps_shear)
+        eps_shear = self.DOF2Nodes(eps_shear)
         return eps_normal, eps_shear
 
     def VTKIntegrationPoints(self, cam, f, g, U, filename="IntPts", iscale=2):
         """
         Writes a VTK Result file for vizualisation using Paraview.
         It builds a points cloud corresponding to the integration points
         where it is possible to visualize the displacement, strain,
@@ -2898,33 +2902,47 @@
 
         where  roi = f.SelectROI()
         """
         inside = self.ElemsInsideRoi(roi, cam=cam)
         for je in self.e.keys():
             self.e[je] = self.e[je][inside[je], :]
 
-    def RemoveDoubleNodes(self):
+    def RemoveDoubleNodes(self, eps=None):
         """
         Removes the double nodes thus changes connectivity
         Warning: both self.e and self.n are modified!
 
         Usage :
             m.RemoveDoubleNodes()
 
         """
-        nnew = np.unique(self.n, axis=0)
-        table = -1 * np.ones(len(self.n), dtype='int')
-        eps = 1e-5 * self.GetApproxElementSize()
-        for jn in range(len(self.n)):
-            rep, = np.where(np.linalg.norm(nnew-self.n[jn, :][np.newaxis],
-                                           axis=1) < eps)
-            table[jn] = rep
+        if eps is None:
+            eps = 1e-5 * self.GetApproxElementSize()
+        scale = 10 ** np.floor(np.log10(eps))  # tolerance between two nodes
+        nnew = np.round(self.n/scale) * scale
+        nnew, ind, inv = np.unique(nnew, axis=0, return_index=True,
+                                   return_inverse=True)
+        self.n = self.n[ind]  # keep the initial precision of remaining nodes
         for k in self.e.keys():
-            self.e[k] = table[self.e[k]]
-        self.n = nnew
+            self.e[k] = inv[self.e[k]]
+
+    def RemoveDoubleElems(self):
+        """
+        Removes elements that appear twice
+        Warning: both self.e is modified!
+
+        Usage :
+            m.RemoveDoubleElems()
+
+        """
+        for k in self.e.keys():
+            e_sort = np.sort(self.e[k], axis=1)
+            _, ind, inv = np.unique(e_sort, axis=0,
+                                   return_index=True, return_inverse=True)
+            self.e[k] = self.e[k][ind, :]
 
     def KeepElemsConnectedToThisNode(self, node_id=0):
         """
         Removes the hanging elements is case of non connexity
         Keeps the elements connected to node id node_id
         Solves a Poisson problem to find connectivity.
 
@@ -3370,8 +3388,67 @@
             elset = dict.fromkeys(self.e.keys())
             for et in self.e.keys():
                 elset[et] = np.zeros(len(self.e[et]), dtype=int)
                 elset[et][self.cell_sets[s][et]] = 1
             el_gp = self.Elem2GaussPoint(elset)
             hooke += np.kron(el_gp[np.newaxis], hooke_dict[s][np.newaxis].T)
         return hooke
-    
+
+    def FEComposition(self, mc):
+        """
+        Composition of a micro mesh by the element mappings of self mesh.
+        Only works with homogeneous element type in self.
+        
+        Parameters
+        ----------
+        mc : PYXEL.MESH
+            is a micro FE mesh defined within the parent element of self
+
+        Returns
+        -------
+        TYPE PYXEL.MESH
+          The composition of the micro and self meshes
+
+        """
+        et = list(self.e.keys())
+        if len(et) > 1:
+            raise Exception('Only one elem type in macro mesh = ' + str(et))
+        else:
+            et = et[0]
+        nelem = 0
+        nelem = len(self.e[et])
+        nnc = len(mc.n)
+        ng = np.zeros((nelem*nnc, self.dim))
+        eg = {}
+        nec = {}
+        for eti in mc.e.keys():
+            nec[eti] = len(mc.e[eti])
+            eg[eti] = np.zeros((nelem*nec[eti], mc.e[eti].shape[1]), dtype='int64')
+        ielem = 0
+        if self.dim == 2:
+            _, _, _, N, _, _ = ShapeFunctions(et)
+            for je in range(len(self.e[et])):
+                rep = np.arange(nnc) + ielem * nnc
+                phi = N(mc.n[:, 0], mc.n[:, 1])
+                ng[rep, :] = phi @ self.n[self.e[et][je]]
+                for eti in mc.e.keys():
+                    rep = np.arange(nec[eti]) + ielem * nec[eti]
+                    eg[eti][rep, :] = mc.e[eti] + ielem * nnc
+                ielem += 1
+        else:
+            _, _, _, _, N, _, _, _ = ShapeFunctions(et)
+            for je in range(len(self.e[et])):
+                rep = np.arange(nnc) + ielem * nnc
+                phi = N(mc.n[:, 0], mc.n[:, 1], mc.n[:, 2])
+                ng[rep, :] = phi @ self.n[self.e[et][je]]
+                for eti in mc.e.keys():
+                    rep = np.arange(nec[eti]) + ielem * nec[eti]
+                    eg[eti][rep, :] = mc.e[eti] + ielem * nnc
+                ielem += 1
+        mg = Mesh(eg, ng, self.dim)
+        print('Removing Unused nodes...')
+        mg.RemoveUnusedNodes()
+        print('Removing Double nodes...')
+        mg.RemoveDoubleNodes(eps=3e-5)
+        print('Removing Double Elements...')
+        mg.RemoveDoubleElems()
+        return mg
```

### Comparing `pyxel-dic-3.1.2/src/pyxel/mesher.py` & `pyxel-dic-3.1.3/src/pyxel/mesher.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel/meshparser.py` & `pyxel-dic-3.1.3/src/pyxel/meshparser.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel/utils.py` & `pyxel-dic-3.1.3/src/pyxel/utils.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel/vtktools.py` & `pyxel-dic-3.1.3/src/pyxel/vtktools.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.2/src/pyxel_dic.egg-info/PKG-INFO` & `pyxel-dic-3.1.3/src/pyxel_dic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-dic
-Version: 3.1.2
+Version: 3.1.3
 Summary: Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics
 Home-page: https://github.com/jcpassieux/pyxel
 Author: Jean-Charles Passieux
 Author-email: JC Passieux <jc.passieux@gmail.com>
 License: 
           CeCILL FREE SOFTWARE LICENSE AGREEMENT
```

### Comparing `pyxel-dic-3.1.2/src/pyxel_dic.egg-info/SOURCES.txt` & `pyxel-dic-3.1.3/src/pyxel_dic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

