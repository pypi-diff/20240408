# Comparing `tmp/interferometer-1.1.tar.gz` & `tmp/interferometer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interferometer-1.1.tar", last modified: Tue Jun 21 20:50:56 2022, max compression
+gzip compressed data, was "interferometer-1.1.1.tar", last modified: Mon Apr  8 17:38:22 2024, max compression
```

## Comparing `interferometer-1.1.tar` & `interferometer-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2022-06-21 20:50:56.510123 interferometer-1.1/
--rw-rw-r--   0 william   (1000) william   (1000)     1082 2022-04-08 18:45:01.000000 interferometer-1.1/LICENSE
--rw-rw-r--   0 william   (1000) william   (1000)     2367 2022-06-21 20:50:56.510123 interferometer-1.1/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)     1710 2022-06-21 19:30:23.000000 interferometer-1.1/README.md
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2022-06-21 20:50:56.510123 interferometer-1.1/interferometer/
--rw-rw-r--   0 william   (1000) william   (1000)      122 2022-06-21 19:36:25.000000 interferometer-1.1/interferometer/__init__.py
--rw-rw-r--   0 william   (1000) william   (1000)    11823 2022-06-21 20:03:09.000000 interferometer-1.1/interferometer/main.py
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2022-06-21 20:50:56.510123 interferometer-1.1/interferometer.egg-info/
--rw-rw-r--   0 william   (1000) william   (1000)     2367 2022-06-21 20:50:56.000000 interferometer-1.1/interferometer.egg-info/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)      271 2022-06-21 20:50:56.000000 interferometer-1.1/interferometer.egg-info/SOURCES.txt
--rw-rw-r--   0 william   (1000) william   (1000)        1 2022-06-21 20:50:56.000000 interferometer-1.1/interferometer.egg-info/dependency_links.txt
--rw-rw-r--   0 william   (1000) william   (1000)       17 2022-06-21 20:50:56.000000 interferometer-1.1/interferometer.egg-info/requires.txt
--rw-rw-r--   0 william   (1000) william   (1000)       15 2022-06-21 20:50:56.000000 interferometer-1.1/interferometer.egg-info/top_level.txt
--rw-rw-r--   0 william   (1000) william   (1000)      819 2022-06-21 20:49:41.000000 interferometer-1.1/pyproject.toml
--rw-rw-r--   0 william   (1000) william   (1000)       38 2022-06-21 20:50:56.510123 interferometer-1.1/setup.cfg
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-08 17:38:22.102784 interferometer-1.1.1/
+-rw-rw-r--   0 william   (1000) william   (1000)     1082 2024-04-07 12:57:36.000000 interferometer-1.1.1/LICENSE
+-rw-r--r--   0 william   (1000) william   (1000)     2416 2024-04-08 17:38:22.102784 interferometer-1.1.1/PKG-INFO
+-rw-rw-r--   0 william   (1000) william   (1000)     1710 2024-04-07 12:57:36.000000 interferometer-1.1.1/README.md
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-08 17:38:22.098784 interferometer-1.1.1/interferometer/
+-rw-rw-r--   0 william   (1000) william   (1000)      122 2024-04-07 12:57:36.000000 interferometer-1.1.1/interferometer/__init__.py
+-rw-rw-r--   0 william   (1000) william   (1000)    12044 2024-04-07 13:29:05.000000 interferometer-1.1.1/interferometer/main.py
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-08 17:38:22.102784 interferometer-1.1.1/interferometer.egg-info/
+-rw-r--r--   0 william   (1000) william   (1000)     2416 2024-04-08 17:38:22.000000 interferometer-1.1.1/interferometer.egg-info/PKG-INFO
+-rw-rw-r--   0 william   (1000) william   (1000)      300 2024-04-08 17:38:22.000000 interferometer-1.1.1/interferometer.egg-info/SOURCES.txt
+-rw-rw-r--   0 william   (1000) william   (1000)        1 2024-04-08 17:38:22.000000 interferometer-1.1.1/interferometer.egg-info/dependency_links.txt
+-rw-rw-r--   0 william   (1000) william   (1000)       17 2024-04-08 17:38:22.000000 interferometer-1.1.1/interferometer.egg-info/requires.txt
+-rw-rw-r--   0 william   (1000) william   (1000)       15 2024-04-08 17:38:22.000000 interferometer-1.1.1/interferometer.egg-info/top_level.txt
+-rw-rw-r--   0 william   (1000) william   (1000)      821 2024-04-08 17:31:44.000000 interferometer-1.1.1/pyproject.toml
+-rw-rw-r--   0 william   (1000) william   (1000)       38 2024-04-08 17:38:22.102784 interferometer-1.1.1/setup.cfg
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-08 17:38:22.098784 interferometer-1.1.1/tests/
+-rw-rw-r--   0 william   (1000) william   (1000)      559 2024-04-07 12:57:36.000000 interferometer-1.1.1/tests/test_interferometer.py
```

### Comparing `interferometer-1.1/LICENSE` & `interferometer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `interferometer-1.1/PKG-INFO` & `interferometer-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: interferometer
-Version: 1.1
+Version: 1.1.1
 Summary: Algorithms for universal interferometers
 Author-email: "William R. Clements" <mail@william-clements.com>
 Project-URL: Homepage, https://github.com/clementsw/interferometer
 Project-URL: Bug Tracker, https://github.com/clementsw/interferometer/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
 
 # Interferometer package
 
 The ability to implement arbitrary interference between any number of optical inputs is useful for both classical and quantum optics. This package provides implementations of the following two papers:
 
 - Reck, Michael, et al. "Experimental realization of any discrete unitary operator." Physical review letters 73.1 (1994): 58.
 - Clements, William R., et al. "Optimal design for universal multiport interferometers." Optica 3.12 (2016): 1460-1465.
```

### Comparing `interferometer-1.1/README.md` & `interferometer-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `interferometer-1.1/interferometer/main.py` & `interferometer-1.1.1/interferometer/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,16 +181,16 @@
         an Interferometer instance
     """
     I = Interferometer()
     N = int(np.sqrt(U.size))
     for ii in range(N-1):
         for jj in range(N-1-ii):
             modes = [N - jj - 1, N - jj]
-            theta = np.arctan(abs(U[ii, N - 1 - jj] / U[ii, N - 2 - jj]))
-            phi = -np.angle(-U[ii, N - 1 - jj] / U[ii, N - 2 - jj])
+            theta = custom_arctan(U[ii, N - 1 - jj], U[ii, N - 2 - jj])
+            phi = -custom_angle(-U[ii, N - 1 - jj], U[ii, N - 2 - jj])
             invT = np.eye(N, dtype=np.complex_)
             invT[modes[0]-1, modes[0]-1] = np.exp(-1j * phi) * np.cos(theta)
             invT[modes[0]-1, modes[1]-1] = np.exp(-1j * phi) * np.sin(theta)
             invT[modes[1]-1, modes[0]-1] = -np.sin(theta)
             invT[modes[1]-1, modes[1]-1] = np.cos(theta)
             U = np.matmul(U, invT)
             I.BS_list.append(Beamsplitter(modes[0], modes[1], theta, phi))
@@ -212,28 +212,28 @@
     I = Interferometer()
     N = int(np.sqrt(U.size))
     left_T = []
     for ii in range(N-1):
         if np.mod(ii, 2) == 0:
             for jj in range(ii+1):
                 modes = [ii - jj + 1, ii + 2 - jj]
-                theta = np.arctan(abs(U[N-1-jj, ii-jj] / U[N-1-jj, ii-jj+1]))
-                phi = np.angle(U[N-1-jj, ii-jj] / U[N-1-jj, ii-jj+1])
+                theta = custom_arctan(U[N-1-jj, ii-jj], U[N-1-jj, ii-jj+1])
+                phi = custom_angle(U[N-1-jj, ii-jj], U[N-1-jj, ii-jj+1])
                 invT = np.eye(N, dtype=np.complex_)
                 invT[modes[0]-1, modes[0]-1] = np.exp(-1j * phi) * np.cos(theta)
                 invT[modes[0]-1, modes[1]-1] = np.exp(-1j * phi) * np.sin(theta)
                 invT[modes[1]-1, modes[0]-1] = -np.sin(theta)
                 invT[modes[1]-1, modes[1]-1] = np.cos(theta)
                 U = np.matmul(U, invT)
                 I.BS_list.append(Beamsplitter(modes[0], modes[1], theta, phi))
         else:
             for jj in range(ii+1):
                 modes = [N+jj-ii-1, N+jj-ii]
-                theta = np.arctan(abs(U[N+jj-ii-1, jj] / U[N+jj-ii-2, jj]))
-                phi = np.angle(-U[N+jj-ii-1, jj] / U[N+jj-ii-2, jj])
+                theta = custom_arctan(U[N+jj-ii-1, jj], U[N+jj-ii-2, jj])
+                phi = custom_angle(-U[N+jj-ii-1, jj], U[N+jj-ii-2, jj])
                 T = np.eye(N, dtype=np.complex_)
                 T[modes[0]-1, modes[0]-1] = np.exp(1j * phi) * np.cos(theta)
                 T[modes[0]-1, modes[1]-1] = -np.sin(theta)
                 T[modes[1]-1, modes[0]-1] = np.exp(1j * phi) * np.sin(theta)
                 T[modes[1]-1, modes[1]-1] = np.cos(theta)
                 U = np.matmul(T, U)         
                 left_T.append(Beamsplitter(modes[0], modes[1], theta, phi))
@@ -242,16 +242,16 @@
         modes = [int(BS.mode1), int(BS.mode2)]
         invT = np.eye(N, dtype=np.complex_)
         invT[modes[0]-1, modes[0]-1] = np.exp(-1j * BS.phi) * np.cos(BS.theta)
         invT[modes[0]-1, modes[1]-1] = np.exp(-1j * BS.phi) * np.sin(BS.theta)
         invT[modes[1]-1, modes[0]-1] = -np.sin(BS.theta)
         invT[modes[1]-1, modes[1]-1] = np.cos(BS.theta)
         U = np.matmul(invT, U)
-        theta = np.arctan(abs(U[modes[1]-1, modes[0]-1]/U[modes[1]-1, modes[1]-1]))
-        phi = np.angle(U[modes[1]-1, modes[0]-1] / U[modes[1]-1, modes[1]-1])
+        theta = custom_arctan(U[modes[1]-1, modes[0]-1], U[modes[1]-1, modes[1]-1])
+        phi = custom_angle(U[modes[1]-1, modes[0]-1], U[modes[1]-1, modes[1]-1])
         invT[modes[0]-1, modes[0]-1] = np.exp(-1j * phi) * np.cos(theta)
         invT[modes[0]-1, modes[1]-1] = np.exp(-1j * phi) * np.sin(theta)
         invT[modes[1]-1, modes[0]-1] = -np.sin(theta)
         invT[modes[1]-1, modes[1]-1] = np.cos(theta)
         U = np.matmul(U, invT) 
         I.BS_list.append(Beamsplitter(modes[0], modes[1], theta, phi))
     phases = np.diag(U)
@@ -277,7 +277,19 @@
             X[ii, jj] = (np.random.normal() + 1j * np.random.normal()) / np.sqrt(2)
 
     q, r = np.linalg.qr(X)
     r = np.diag(np.divide(np.diag(r), abs(np.diag(r))))
     U = np.matmul(q, r)
 
     return U
+
+def custom_arctan(x1, x2):
+    if x2 != 0:
+        return np.arctan(abs(x1/x2))
+    else:
+        return np.pi/2
+
+def custom_angle(x1, x2):
+    if x2 != 0:
+        return np.angle(x1/x2)
+    else:
+        return 0
```

### Comparing `interferometer-1.1/interferometer.egg-info/PKG-INFO` & `interferometer-1.1.1/interferometer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: interferometer
-Version: 1.1
+Version: 1.1.1
 Summary: Algorithms for universal interferometers
 Author-email: "William R. Clements" <mail@william-clements.com>
 Project-URL: Homepage, https://github.com/clementsw/interferometer
 Project-URL: Bug Tracker, https://github.com/clementsw/interferometer/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
 
 # Interferometer package
 
 The ability to implement arbitrary interference between any number of optical inputs is useful for both classical and quantum optics. This package provides implementations of the following two papers:
 
 - Reck, Michael, et al. "Experimental realization of any discrete unitary operator." Physical review letters 73.1 (1994): 58.
 - Clements, William R., et al. "Optimal design for universal multiport interferometers." Optica 3.12 (2016): 1460-1465.
```

### Comparing `interferometer-1.1/pyproject.toml` & `interferometer-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "interferometer"
-version = "1.1"
+version = "1.1.1"
 authors = [
   { name="William R. Clements", email="mail@william-clements.com" },
 ]
 description = "Algorithms for universal interferometers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

