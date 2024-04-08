# Comparing `tmp/widget_bzvisualizer-0.2.3.tar.gz` & `tmp/widget_bzvisualizer-0.2.4.tar.gz`

## Comparing `widget_bzvisualizer-0.2.3.tar` & `widget_bzvisualizer-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/__init__.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/utils.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/static/widget.css
--rw-r--r--   0        0        0   484471 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/static/widget.js
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/.gitignore
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/README.md
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/__init__.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/utils.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/static/widget.css
+-rw-r--r--   0        0        0   484471 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/static/widget.js
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/README.md
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 widget_bzvisualizer-0.2.4/PKG-INFO
```

### Comparing `widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/utils.py` & `widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import numpy as np
 import seekpath
 from seekpath.brillouinzone.brillouinzone import get_BZ
 
 
-def get_seekpath_data_for_visualizer(cell, relcoords, atomic_numbers):
-    system = (np.array(cell), np.array(relcoords), np.array(atomic_numbers))
+def get_seekpath_data_for_visualizer(system):
+    system = (
+        np.array(system["cell"]),
+        np.array(system["rel_coords"]),
+        np.array(system["atom_numbers"]),
+    )
     res = seekpath.get_explicit_k_path(system, with_time_reversal=False)
 
     b1, b2, b3 = res["reciprocal_primitive_lattice"]
     faces_data = get_BZ(b1=b1, b2=b2, b3=b3)
 
     kpoints_rel = res["point_coords"]
     kpoints_abs = {
```

### Comparing `widget_bzvisualizer-0.2.3/src/widget_bzvisualizer/static/widget.js` & `widget_bzvisualizer-0.2.4/src/widget_bzvisualizer/static/widget.js`

 * *Files identical despite different names*

### Comparing `widget_bzvisualizer-0.2.3/README.md` & `widget_bzvisualizer-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `widget_bzvisualizer-0.2.3/pyproject.toml` & `widget_bzvisualizer-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "widget-bzvisualizer"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
   "anywidget~=0.9.3",
   "numpy~=1.21",
   "scipy~=1.10",
   "seekpath~=2.1",
 ]
 readme = "README.md"
@@ -37,15 +37,15 @@
 dependencies = ["hatch-jupyter-builder>=0.5.0"]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 npm = "npm"
 build_cmd = "build"
 
 [tool.bumpver]
-current_version = "v0.2.3"
+current_version = "v0.2.4"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `widget_bzvisualizer-0.2.3/PKG-INFO` & `widget_bzvisualizer-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: widget-bzvisualizer
-Version: 0.2.3
+Version: 0.2.4
 Requires-Dist: anywidget~=0.9.3
 Requires-Dist: numpy~=1.21
 Requires-Dist: scipy~=1.10
 Requires-Dist: seekpath~=2.1
 Provides-Extra: dev
 Requires-Dist: ase; extra == 'dev'
 Requires-Dist: bumpver==2023.1129; extra == 'dev'
```

