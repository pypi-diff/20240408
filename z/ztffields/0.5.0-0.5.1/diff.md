# Comparing `tmp/ztffields-0.5.0.tar.gz` & `tmp/ztffields-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztffields-0.5.0.tar", last modified: Thu Feb 29 10:01:05 2024, max compression
+gzip compressed data, was "ztffields-0.5.1.tar", last modified: Mon Apr  8 13:14:47 2024, max compression
```

## Comparing `ztffields-0.5.0.tar` & `ztffields-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-02-29 10:01:05.574269 ztffields-0.5.0/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-12-09 18:53:25.000000 ztffields-0.5.0/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)     1027 2024-02-29 10:01:05.574205 ztffields-0.5.0/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      432 2022-12-13 14:52:32.000000 ztffields-0.5.0/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)     1128 2024-02-29 10:01:05.574578 ztffields-0.5.0/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2022-12-11 14:43:45.000000 ztffields-0.5.0/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-02-29 10:01:05.571191 ztffields-0.5.0/ztffields/
--rw-r--r--   0 rigault   (2358) staff       (20)       95 2024-02-29 10:00:50.000000 ztffields-0.5.0/ztffields/__init__.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-02-29 10:01:05.572701 ztffields-0.5.0/ztffields/data/
--rwxr-xr-x   0 rigault   (2358) staff       (20)     1419 2022-12-11 14:44:47.000000 ztffields-0.5.0/ztffields/data/ztf_ccd_layout.tbl
--rwxr-xr-x   0 rigault   (2358) staff       (20)     6230 2022-12-11 14:44:47.000000 ztffields-0.5.0/ztffields/data/ztf_ccd_quad_layout.tbl
--rwxr-xr-x   0 rigault   (2358) staff       (20)   123430 2022-12-11 14:44:47.000000 ztffields-0.5.0/ztffields/data/ztf_fields.txt
--rw-r--r--   0 rigault   (2358) staff       (20)    20296 2023-06-29 08:00:51.000000 ztffields-0.5.0/ztffields/fields.py
--rw-r--r--   0 rigault   (2358) staff       (20)      175 2022-12-11 14:47:26.000000 ztffields-0.5.0/ztffields/io.py
--rw-r--r--   0 rigault   (2358) staff       (20)    28985 2023-09-04 19:35:33.000000 ztffields-0.5.0/ztffields/plotting.py
--rw-r--r--   0 rigault   (2358) staff       (20)    14179 2024-02-29 09:59:33.000000 ztffields-0.5.0/ztffields/projection.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2268 2023-02-12 07:53:02.000000 ztffields-0.5.0/ztffields/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-02-29 10:01:05.573803 ztffields-0.5.0/ztffields.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)     1027 2024-02-29 10:01:05.000000 ztffields-0.5.0/ztffields.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      458 2024-02-29 10:01:05.000000 ztffields-0.5.0/ztffields.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2024-02-29 10:01:05.000000 ztffields-0.5.0/ztffields.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2022-12-11 14:44:59.000000 ztffields-0.5.0/ztffields.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)      132 2024-02-29 10:01:05.000000 ztffields-0.5.0/ztffields.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2024-02-29 10:01:05.000000 ztffields-0.5.0/ztffields.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-04-08 13:14:47.930210 ztffields-0.5.1/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-12-09 18:53:25.000000 ztffields-0.5.1/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)     1027 2024-04-08 13:14:47.930153 ztffields-0.5.1/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      432 2022-12-13 14:52:32.000000 ztffields-0.5.1/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)     1128 2024-04-08 13:14:47.930519 ztffields-0.5.1/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2022-12-11 14:43:45.000000 ztffields-0.5.1/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-04-08 13:14:47.928472 ztffields-0.5.1/ztffields/
+-rw-r--r--   0 rigault   (2358) staff       (20)       95 2024-03-26 14:18:31.000000 ztffields-0.5.1/ztffields/__init__.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-04-08 13:14:47.929545 ztffields-0.5.1/ztffields/data/
+-rwxr-xr-x   0 rigault   (2358) staff       (20)     1419 2022-12-11 14:44:47.000000 ztffields-0.5.1/ztffields/data/ztf_ccd_layout.tbl
+-rwxr-xr-x   0 rigault   (2358) staff       (20)     6230 2022-12-11 14:44:47.000000 ztffields-0.5.1/ztffields/data/ztf_ccd_quad_layout.tbl
+-rwxr-xr-x   0 rigault   (2358) staff       (20)   123430 2022-12-11 14:44:47.000000 ztffields-0.5.1/ztffields/data/ztf_fields.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)    20296 2023-06-29 08:00:51.000000 ztffields-0.5.1/ztffields/fields.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      175 2022-12-11 14:47:26.000000 ztffields-0.5.1/ztffields/io.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    28985 2023-09-04 19:35:33.000000 ztffields-0.5.1/ztffields/plotting.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    15102 2024-03-26 14:21:58.000000 ztffields-0.5.1/ztffields/projection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2317 2024-02-29 14:30:53.000000 ztffields-0.5.1/ztffields/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-04-08 13:14:47.929769 ztffields-0.5.1/ztffields.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)     1027 2024-04-08 13:14:47.000000 ztffields-0.5.1/ztffields.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      458 2024-04-08 13:14:47.000000 ztffields-0.5.1/ztffields.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2024-04-08 13:14:47.000000 ztffields-0.5.1/ztffields.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2022-12-11 14:44:59.000000 ztffields-0.5.1/ztffields.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)      132 2024-04-08 13:14:47.000000 ztffields-0.5.1/ztffields.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2024-04-08 13:14:47.000000 ztffields-0.5.1/ztffields.egg-info/top_level.txt
```

### Comparing `ztffields-0.5.0/LICENSE` & `ztffields-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.0/PKG-INFO` & `ztffields-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ztffields
-Version: 0.5.0
+Version: 0.5.1
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/ztffields
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ztffields-0.5.0/setup.cfg` & `ztffields-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.0/ztffields/data/ztf_ccd_layout.tbl` & `ztffields-0.5.1/ztffields/data/ztf_ccd_layout.tbl`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.0/ztffields/data/ztf_ccd_quad_layout.tbl` & `ztffields-0.5.1/ztffields/data/ztf_ccd_quad_layout.tbl`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.0/ztffields/data/ztf_fields.txt` & `ztffields-0.5.1/ztffields/data/ztf_fields.txt`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.0/ztffields/fields.py` & `ztffields-0.5.1/ztffields/fields.py`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.0/ztffields/plotting.py` & `ztffields-0.5.1/ztffields/plotting.py`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.0/ztffields/projection.py` & `ztffields-0.5.1/ztffields/projection.py`

 * *Files 3% similar despite different names*

```diff
@@ -312,18 +312,41 @@
     @classmethod
     def radec_to_fieldid(cls, radec, level="focalplane", explode=True):
         """ """
         this = cls(radec=radec, level=level)
         return this.get_target_fields(explode=explode)
         
     @classmethod
-    def fieldid_to_radec(cls, radec, level="focalplane", explode=True):
+    def fieldid_to_radec(cls, fieldid=None, level="focalplane", as_shapely=False):
         """ """
-        this = cls(radec=radec, level=level)
-        return this.get_field_targets(explode=explode)
+        this = cls(level=level)
+        geo_df = this.get_geoseries(level).to_frame("geometry").copy()
+
+        # build the geodataframe of centroid
+        if level == "focalplane":
+            geocentroid = geo_df["geometry"].centroid
+            if fieldid is not None:
+                geocentroid = geocentroid.loc[fieldid] # single-index
+                
+            
+        elif level == "ccd" or "quadrant":
+            key = "ccdid" if level == "ccd" else "rcid"
+            fieldid, levelid = np.vstack(geo_df.index.str.split("_")).astype("int32").T
+            geo_df["fieldid"], geo_df[key] = fieldid, levelid
+            geocentroid = geo_df.set_index(["fieldid", key]).centroid
+            if fieldid is not None:
+                geocentroid = geocentroid.loc[fieldid,:] # multi-index
+            
+        else:
+            raise ValueError(f"level={level} is not accepted.")
+
+        if as_shapely:
+            return geocentroid
+        
+        return geocentroid.map(lambda x: np.hstack(x.xy))
         
     # ============= #
     #  Methods      #
     # ============= #        
     # - Top Level
     def get_target_fields(self, explode=False):
         """ """
```

### Comparing `ztffields-0.5.0/ztffields/utils.py` & `ztffields-0.5.1/ztffields/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,14 @@
         [r, theta, phi]
     """
     v_rot = rot_xz( sph2cart([1,l,b]), theta)
     return cart2sph(v_rot)[1:]
 
 def ccdid_qid_to_rcid(ccdid, qid):
     """ provides the rcid corresponding to the ccdid and qid """
-    return 4*(ccdid - 1) + qid - 1
+    return np.asarray(4*(ccdid - 1) + qid - 1, dtype="int")
 
 def rcid_to_ccdid_qid(rcid):
     """ gets the ccdid and qid for the given rcid """
     qid = (rcid%4)+1
-    ccdid  = int((rcid-(qid - 1))/4 +1)
-    return ccdid, qid
+    ccdid  = ((rcid-(qid - 1))/4 +1)
+    return np.asarray([ccdid, qid], dtype="int")
```

### Comparing `ztffields-0.5.0/ztffields.egg-info/PKG-INFO` & `ztffields-0.5.1/ztffields.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ztffields
-Version: 0.5.0
+Version: 0.5.1
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/ztffields
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

