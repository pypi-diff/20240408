# Comparing `tmp/PyCBA-0.4.2.tar.gz` & `tmp/PyCBA-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCBA-0.4.2.tar", last modified: Fri Mar 22 00:52:19 2024, max compression
+gzip compressed data, was "PyCBA-0.5.1.tar", last modified: Mon Apr  8 14:14:43 2024, max compression
```

## Comparing `PyCBA-0.4.2.tar` & `PyCBA-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 00:52:19.184208 PyCBA-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-22 00:52:13.000000 PyCBA-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-03-22 00:52:19.184208 PyCBA-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-22 00:52:13.000000 PyCBA-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-22 00:52:13.000000 PyCBA-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 00:52:19.184208 PyCBA-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 00:52:13.000000 PyCBA-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 00:52:19.180208 PyCBA-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 00:52:19.184208 PyCBA-0.4.2/src/PyCBA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-03-22 00:52:19.000000 PyCBA-0.4.2/src/PyCBA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-22 00:52:19.000000 PyCBA-0.4.2/src/PyCBA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 00:52:19.000000 PyCBA-0.4.2/src/PyCBA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-22 00:52:19.000000 PyCBA-0.4.2/src/PyCBA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 00:52:19.000000 PyCBA-0.4.2/src/PyCBA.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 00:52:19.184208 PyCBA-0.4.2/src/pycba/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-22 00:52:13.000000 PyCBA-0.4.2/src/pycba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-03-22 00:52:13.000000 PyCBA-0.4.2/src/pycba/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-03-22 00:52:13.000000 PyCBA-0.4.2/src/pycba/beam.py
--rw-r--r--   0 runner    (1001) docker     (127)    19409 2024-03-22 00:52:13.000000 PyCBA-0.4.2/src/pycba/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-03-22 00:52:13.000000 PyCBA-0.4.2/src/pycba/inf_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-03-22 00:52:13.000000 PyCBA-0.4.2/src/pycba/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-03-22 00:52:13.000000 PyCBA-0.4.2/src/pycba/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-03-22 00:52:13.000000 PyCBA-0.4.2/src/pycba/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-03-22 00:52:13.000000 PyCBA-0.4.2/src/pycba/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-03-22 00:52:13.000000 PyCBA-0.4.2/src/pycba/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 00:52:19.184208 PyCBA-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-03-22 00:52:13.000000 PyCBA-0.4.2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-03-22 00:52:13.000000 PyCBA-0.4.2/tests/test_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-03-22 00:52:13.000000 PyCBA-0.4.2/tests/test_inf_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:14:43.939666 PyCBA-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 14:14:38.000000 PyCBA-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-08 14:14:43.939666 PyCBA-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-08 14:14:38.000000 PyCBA-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-08 14:14:38.000000 PyCBA-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:14:43.939666 PyCBA-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 14:14:38.000000 PyCBA-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:14:43.935666 PyCBA-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:14:43.939666 PyCBA-0.5.1/src/PyCBA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-08 14:14:43.000000 PyCBA-0.5.1/src/PyCBA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-08 14:14:43.000000 PyCBA-0.5.1/src/PyCBA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:14:43.000000 PyCBA-0.5.1/src/PyCBA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 14:14:43.000000 PyCBA-0.5.1/src/PyCBA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 14:14:43.000000 PyCBA-0.5.1/src/PyCBA.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:14:43.939666 PyCBA-0.5.1/src/pycba/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-08 14:14:38.000000 PyCBA-0.5.1/src/pycba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-04-08 14:14:38.000000 PyCBA-0.5.1/src/pycba/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-04-08 14:14:38.000000 PyCBA-0.5.1/src/pycba/beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19409 2024-04-08 14:14:38.000000 PyCBA-0.5.1/src/pycba/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-08 14:14:38.000000 PyCBA-0.5.1/src/pycba/inf_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22136 2024-04-08 14:14:38.000000 PyCBA-0.5.1/src/pycba/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-08 14:14:38.000000 PyCBA-0.5.1/src/pycba/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13076 2024-04-08 14:14:38.000000 PyCBA-0.5.1/src/pycba/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-08 14:14:38.000000 PyCBA-0.5.1/src/pycba/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-04-08 14:14:38.000000 PyCBA-0.5.1/src/pycba/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:14:43.939666 PyCBA-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-04-08 14:14:38.000000 PyCBA-0.5.1/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-08 14:14:38.000000 PyCBA-0.5.1/tests/test_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-08 14:14:38.000000 PyCBA-0.5.1/tests/test_inf_lines.py
```

### Comparing `PyCBA-0.4.2/LICENSE` & `PyCBA-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCBA-0.4.2/PKG-INFO` & `PyCBA-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCBA
-Version: 0.4.2
+Version: 0.5.1
 Summary: Python Continuous Beam Analysis
 Author-email: Colin Caprani <colin.caprani@monash.edu>
 License: Apache 2.0
 Project-URL: Homepage, https://ccaprani.github.io/pycba/
 Project-URL: Documentation, https://ccaprani.github.io/pycba/
 Project-URL: Source, https://github.com/ccaprani/pycba/
 Project-URL: Tracker, https://github.com/ccaprani/pycba/issues/
```

### Comparing `PyCBA-0.4.2/README.md` & `PyCBA-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `PyCBA-0.4.2/pyproject.toml` & `PyCBA-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyCBA-0.4.2/src/PyCBA.egg-info/PKG-INFO` & `PyCBA-0.5.1/src/PyCBA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCBA
-Version: 0.4.2
+Version: 0.5.1
 Summary: Python Continuous Beam Analysis
 Author-email: Colin Caprani <colin.caprani@monash.edu>
 License: Apache 2.0
 Project-URL: Homepage, https://ccaprani.github.io/pycba/
 Project-URL: Documentation, https://ccaprani.github.io/pycba/
 Project-URL: Source, https://github.com/ccaprani/pycba/
 Project-URL: Tracker, https://github.com/ccaprani/pycba/issues/
```

### Comparing `PyCBA-0.4.2/src/pycba/analysis.py` & `PyCBA-0.5.1/src/pycba/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         """
         self._beam._set_loads()
 
         f = np.zeros(self._nDOF)
 
         for i in range(self._n):
             dof_i = 2 * i
-            fmbr = self._beam.get_cnl(i)
+            fmbr = self._beam.get_ref(i)
             # Cumulatively apply forces in opposite direction
             f[dof_i : dof_i + 4] -= fmbr
         return f
 
     def _assemble(self) -> np.ndarray:
         """
         Construct the unrestricted global stiffness matrix
```

### Comparing `PyCBA-0.4.2/src/pycba/beam.py` & `PyCBA-0.5.1/src/pycba/beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,26 +215,26 @@
 
         Returns
         -------
         no_restraints : int
             The number of restraints in the beam
         """
         return len(self._restraints)
-    
+
     @property
     def no_fixed_restraints(self):
         """
         Returns the number of fixed restraints of the beam (fully-supported DOFs)
 
         Returns
         -------
         no_fixed_restraints : int
             The number of fixed restraints in the beam
         """
-        return len(np.where(np.array(self._restraints)==-1)[0])
+        return len(np.where(np.array(self._restraints) == -1)[0])
 
     @property
     def length(self):
         """
         Returns
         -------
         length : float
@@ -276,37 +276,38 @@
             ispan = next(i - 1 for i, x in enumerate(self._terminal_coords) if x > pos)
         except StopIteration:  # at the end of the beam
             ispan = self._no_spans - 1
         pos_in_span = pos - self._terminal_coords[ispan]
 
         return ispan, pos_in_span
 
-    def get_cnl(self, i_span: int) -> LoadCNL:
+    def get_ref(self, i_span: int) -> LoadCNL:
         """
-        Returns Consistent Nodal Loads for the member
+        Returns Released End Forces for the member; that is, the Consistent Nodal Loads
+        modified for the element type (i.e. releases)
 
         Parameters
         ----------
         ispan : int
             The index (1-based) of the span in which the point of interest falls
 
         Returns
         -------
-        cnl : LoadCNL
+        ref : LoadCNL
             The totalled CNL object for the member, considering all loads.
 
         """
-        cnl = np.zeros(4)
+        ref = np.zeros(4)
         L = self.mbr_lengths[i_span]
         eType = self.mbr_eletype[i_span]
 
         for load in self._loads:
             if load.i_span == i_span:
-                cnl += load.get_cnl(L, eType)
-        return cnl
+                ref += load.get_ref(L, eType)
+        return ref
 
     def get_span_k(self, i_span: int) -> np.ndarray:
         """
         Returns the stiffness matrix for the ith span
 
         Parameters
         ----------
```

### Comparing `PyCBA-0.4.2/src/pycba/bridge.py` & `PyCBA-0.5.1/src/pycba/bridge.py`

 * *Files identical despite different names*

### Comparing `PyCBA-0.4.2/src/pycba/inf_lines.py` & `PyCBA-0.5.1/src/pycba/inf_lines.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,52 +115,80 @@
         (x,eta) : tuple(np.ndarray,np.ndarray)
             A tuple of the vectors of abcissa and influence ordinates.
         """
         if not self.vResults:
             self.create_ils()
 
         x = self.vResults[0].results.x
-        dx = x[2] - x[1]
-        idx = np.where(np.abs(x - poi) <= dx * 1e-6)[0][0]
-        #idx = np.abs(x - poi).argmin()
-        
         npts = len(self.vResults)
         eta = np.zeros(npts)
-        
-        #
-        # Getting the correct vertical reaction is tricky
-        # Should be relatively easy to extend to get moment reactions too.
+
+        # Preparations for reaction ILs
         #
         # Get vector of the node locations
         node_locations = np.cumsum(np.insert(self.ba.beam.mbr_lengths, 0, 0))
-        # The indices of the supported vertical DOFs wrt the node locations vector
-        vert_sup_dof_idx = np.where(np.array(self.ba._beam.restraints)[::2]==-1)[0]
-        # The locations then of these vertical supports
-        vert_sup_locs = node_locations[vert_sup_dof_idx]
-        # The index of the closest vertical support
-        closest_vert_sup_idx = np.abs(vert_sup_locs-poi).argmin()
-        # And its value
-        closest_vert_sup = vert_sup_locs[closest_vert_sup_idx]
-        # And now the indixe of this support in the node locations vector
-        node_idx = np.where(node_locations==closest_vert_sup)[0][0]
-        # And hence its index in the overall DOFs vector
-        dof_idx = 2*node_idx
-        
-        # Now we must link the supported DOF to the index in the BeamAnalysis reactions vector
+        # Link the supported DOF to the index in the BeamAnalysis reactions vector
         idx_mask = np.zeros_like(self.ba._beam.restraints)
-        idx_mask[np.where(np.array(self.ba._beam.restraints)==-1)] = np.arange(self.ba.beam.no_fixed_restraints)
-        # And finally the index of the vertical support nearest the POI in the reactions vector
-        vert_sup_idx = idx_mask[dof_idx]
+        idx_mask[np.where(np.array(self.ba._beam.restraints) == -1)] = np.arange(
+            self.ba.beam.no_fixed_restraints
+        )
 
-        for i, res in enumerate(self.vResults):
-            if load_effect == "V":
+        # idx = np.abs(x - poi).argmin()
+
+        if load_effect.upper() == "V":
+            dx = x[2] - x[1]
+            idx = np.where(np.abs(x - poi) <= dx * 1e-6)[0][0]
+            for i, res in enumerate(self.vResults):
                 eta[i] = res.results.V[idx]
-            elif load_effect == "R":
+
+        elif load_effect.upper() == "R":
+            #
+            # Getting the correct reaction is tricky
+            #
+            # The indices of the supported DOFs wrt the node locations vector
+            vert_sups_dof_idx = np.where(np.array(self.ba._beam.restraints)[::2] == -1)[
+                0
+            ]
+            # The locations then of these supports
+            vert_sups_locs = node_locations[vert_sups_dof_idx]
+            # The index of the closest support
+            closest_vert_sup_idx = np.abs(vert_sups_locs - poi).argmin()
+            # And its value
+            closest_vert_sup = vert_sups_locs[closest_vert_sup_idx]
+            # And now the index of this support in the node locations vector
+            vert_sup_node_idx = np.where(node_locations == closest_vert_sup)[0][0]
+            # And hence its index in the overall DOFs vector
+            vert_sup_dof_idx = 2 * vert_sup_node_idx
+            # And finally the index of the support nearest the POI in the reactions vector
+            vert_sup_idx = idx_mask[vert_sup_dof_idx]
+
+            for i, res in enumerate(self.vResults):
                 eta[i] = res.R[vert_sup_idx]
-            else:
+
+        elif load_effect.upper() == "MR":
+            #
+            # Follows the same logic for the vertical reaction
+            #
+            mt_sups_dof_idx = np.where(np.array(self.ba._beam.restraints)[1::2] == -1)[
+                0
+            ]
+            mt_sups_locs = node_locations[mt_sups_dof_idx]
+            closest_mt_sup_idx = np.abs(mt_sups_locs - poi).argmin()
+            closest_mt_sup = mt_sups_locs[closest_mt_sup_idx]
+            mt_sup_node_idx = np.where(node_locations == closest_mt_sup)[0][0]
+            mt_sup_dof_idx = 2 * mt_sup_node_idx + 1
+            mt_sup_idx = idx_mask[mt_sup_dof_idx]
+
+            for i, res in enumerate(self.vResults):
+                eta[i] = res.R[mt_sup_idx]
+
+        else:
+            dx = x[2] - x[1]
+            idx = np.where(np.abs(x - poi) <= dx * 1e-6)[0][0]
+            for i, res in enumerate(self.vResults):
                 eta[i] = res.results.M[idx]
 
         return (np.array(self.pos), eta)
 
     def plot_il(self, poi: float, load_effect: str, ax: Optional[plt.Axes] = None):
         """
         Retrieves and plots the IL on either a supplied or new axes.
```

### Comparing `PyCBA-0.4.2/src/pycba/load.py` & `PyCBA-0.5.1/src/pycba/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         Parameters
         ----------
         i_span : int
             The index of the span (or member), 1-based
         """
         self.i_span = i_span
 
-    def get_cnl(self, L, eType):
+    def get_cnl(self, L):
         # Enforce virtual base class
         raise NotImplementedError
 
     def get_mbr_results(self, x, L):
         raise NotImplementedError
 
     def MB(self, v: np.ndarray) -> np.ndarray:
@@ -211,55 +211,52 @@
             The vector to which the Heaviside function will be applied
         value : float
             The value of the Heaviside function at zero, usually 0, but sometimes
             0.5 (average of adjacent values) or 1.0.
         """
         return np.heaviside(v, value)
 
-    def released_end_forces(self, cnl: LoadCNL, L: float, eType: int) -> LoadCNL:
+    def get_ref(self, L: float, eType: int) -> LoadCNL:
         """
-        The released end forces for each element type: converts the Consistent Nodal
-        Loads of the applied loading to the correct nodal loading depending on the
-        element type.
+        Returns the Released End Forces for a span of length L of element eType:
+        converts the Consistent Nodal Loads of the applied loading to the correct nodal
+        loading depending on the element type.
 
         Parameters
         ----------
-        cnl : LoadCNL
-            The nodal loading statically consistent with the externally applied loads.
         L : float
-            The length of the member.
+            The length of the member
         eType : int
-            The element type.
+            The member element type
 
         Returns
         -------
         LoadCNL
-            The nodal loads to be applied in the analysis, consistent with the element
-            type.
-
+            Released End Forces for this load type: the nodal loads to be applied in
+            the analysis, consistent with the element type.
         """
-
+        cnl = self.get_cnl(L, eType)
         ref = np.zeros(4)
         fm = 6 / (4 * L)  # flexibility coeff for moment
 
         if eType == 2:  # DOF = moment at j node
             ref[0] = fm * cnl.Mb
             ref[1] = 0.5 * cnl.Mb
             ref[2] = -fm * cnl.Mb
             ref[3] = 1.0 * cnl.Mb
         elif eType == 3:  # DOF = moment at i node
             ref[0] = fm * cnl.Ma
-            ref[1] = 0.5 * cnl.Ma
+            ref[1] = 1.0 * cnl.Ma
             ref[2] = -fm * cnl.Ma
-            ref[3] = 1.0 * cnl.Ma
+            ref[3] = 0.5 * cnl.Ma
         elif eType == 4:  # keep only vertical, remove moments
-            ref[0] = 0
-            ref[1] = 1.0 * cnl.Va
-            ref[2] = 0
-            ref[3] = 1.0 * cnl.Va
+            ref[0] = -(cnl.Ma + cnl.Mb) / L
+            ref[1] = 1.0 * cnl.Ma
+            ref[2] = (cnl.Ma + cnl.Mb) / L
+            ref[3] = 1.0 * cnl.Mb
         else:
             # no nothing if it is FF
             pass
         # now superimpose the released forces
         return LoadCNL(
             Va=cnl.Va - ref[0],
             Ma=cnl.Ma - ref[1],
@@ -315,16 +312,15 @@
             # Shears
             Va=w * L / 2.0,
             Vb=w * L / 2.0,
             # Moments
             Ma=w * L**2 / 12.0,
             Mb=-w * L**2 / 12.0,
         )
-
-        return self.released_end_forces(cnl, L, eType)
+        return cnl
 
     def get_mbr_results(self, x: np.ndarray, L: float) -> MemberResults:
         """
         Results along the member from UDL
 
         Parameters
         ----------
@@ -412,16 +408,15 @@
             # Shears
             Va=P / L**3 * (b * L**2 - a**2 * b + a * b**2),
             Vb=P / L**3 * (a * L**2 + a**2 * b - a * b**2),
             # Moments
             Ma=P * a * b**2 / L**2,
             Mb=-P * a**2 * b / L**2,
         )
-        # implicit conversion to tuple in correct order
-        return self.released_end_forces(cnl, L, eType)
+        return cnl
 
     def get_mbr_results(self, x: np.ndarray, L: float) -> MemberResults:
         """
         Results along the member from this load
 
         Parameters
         ----------
@@ -508,15 +503,15 @@
             Va=(w * c / L**3) * ((2 * s + L) * t**2 + (s - t) * c**2 / 4),
             Vb=w * c - (w * c / L**3) * ((2 * s + L) * t**2 + (s - t) * c**2 / 4),
             # Moments
             Ma=(w * c / L**2) * (s * t**2 + (s - 2 * t) * c**2 / 12),
             Mb=-(w * c / L**2) * (t * s**2 + (t - 2 * s) * c**2 / 12),
         )
         # implicit conversion to tuple in correct order
-        return self.released_end_forces(cnl, L, eType)
+        return cnl
 
     def get_mbr_results(self, x: np.ndarray, L: float) -> MemberResults:
         """
         Results along the member from this load
 
         Parameters
         ----------
@@ -604,16 +599,15 @@
             # Shears
             Va=(Ma + Mb) / L,
             Vb=-(Ma + Mb) / L,
             # Moments
             Ma=Ma,
             Mb=Mb,
         )
-        # implicit conversion to tuple in correct order
-        return self.released_end_forces(cnl, L, eType)
+        return cnl
 
     def get_mbr_results(self, x: np.ndarray, L: float) -> MemberResults:
         """
         Results along the member from this load
 
         Parameters
         ----------
@@ -686,16 +680,15 @@
             # Shears
             Va=6 * m * a * b / L**3,
             Vb=-6 * m * a * b / L**3,
             # Moments
             Ma=(m * b / L**2) * (2 * a - b),
             Mb=(m * a / L**2) * (2 * b - a),
         )
-        # implicit conversion to tuple in correct order
-        return self.released_end_forces(cnl, L, eType)
+        return cnl
 
     def get_mbr_results(self, x: np.ndarray, L: float) -> MemberResults:
         """
         Results along the member from this load
 
         Parameters
         ----------
```

### Comparing `PyCBA-0.4.2/src/pycba/pattern.py` & `PyCBA-0.5.1/src/pycba/pattern.py`

 * *Files identical despite different names*

### Comparing `PyCBA-0.4.2/src/pycba/results.py` & `PyCBA-0.5.1/src/pycba/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from __future__ import annotations  # https://bit.ly/3KYiL2o
 from typing import List, Tuple
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy import integrate
 from .beam import Beam
-from .load import MemberResults, LoadMaMb
+from .load import MemberResults, LoadMaMb, LoadCNL
 from copy import deepcopy
 
 
 class BeamResults:
     """
     BeamResults Class for processing and containing the results for each member
     """
@@ -101,15 +101,15 @@
         for i in range(beam.no_spans):
             kb = beam.get_span_k(i)
             dof_i = 2 * i
             dmbr = d[dof_i : dof_i + 4]
             fmbr = np.zeros(4)
             for j in range(4):
                 fmbr[j] = np.sum(kb[j][:] * dmbr[:])
-            fmbr += beam.get_cnl(i)
+            fmbr += beam.get_ref(i)
             res = self._member_values(beam, i, fmbr, dmbr)
             # Shift x vals by location of mbr starting point
             res.x += sumL
             sumL += beam.mbr_lengths[i]
             vRes.append(res)
         return vRes
 
@@ -134,34 +134,50 @@
         Returns
         -------
         MemberResults
             The load effects values along the member.
         """
 
         L = beam.mbr_lengths[i_span]
+        EI = beam.mbr_EIs[i_span]
+        etype = beam.mbr_eletype[i_span]
+
         dx = L / self.npts
         x = np.zeros(self.npts + 3)
         x[1 : self.npts + 2] = dx * np.arange(0, self.npts + 1)
         x[self.npts + 2] = L
 
         # Get the results for the end moments alone
         MaMb = LoadMaMb(i_span=i_span, Ma=f[1], Mb=f[3])
         res = MaMb.get_mbr_results(x, L)
 
         # Now get the results for all the applied loads on a simple span
+        Ma = 0
+        Mb = 0
         for load in beam._loads:
             if load.i_span != i_span:
                 continue
             res += load.get_mbr_results(x, L)
+            cnl = load.get_cnl(L, etype)
+            Ma += cnl.Ma
+            Mb += cnl.Mb
+
+        # If no releases, the rotation at i is easy
+        R0 = d[1]
+
+        # Otherwise, check account for releases
+        if etype > 1:
+            theta = (d[2] - d[0]) / L
+            phi = (L / (3 * EI)) * (-(f[1] - 0.5 * f[3]) + (Ma - 0.5 * Mb))
+            R0 = theta - phi
 
         # And superimpose end displacements using Moment-Area
         h = L / self.npts
-        EI = beam.mbr_EIs[i_span]
 
-        R = integrate.cumtrapz(res.M[1:-1], dx=h, initial=0) / EI + d[1]
+        R = integrate.cumtrapz(res.M[1:-1], dx=h, initial=0) / EI + R0
         D = integrate.cumtrapz(R, dx=h, initial=0) + d[0]
 
         res.R[1:-1] = R
         res.D[1:-1] = D
 
         return res
```

### Comparing `PyCBA-0.4.2/src/pycba/utils.py` & `PyCBA-0.5.1/src/pycba/utils.py`

 * *Files identical despite different names*

### Comparing `PyCBA-0.4.2/src/pycba/vehicle.py` & `PyCBA-0.5.1/src/pycba/vehicle.py`

 * *Files identical despite different names*

### Comparing `PyCBA-0.4.2/tests/test_bridge.py` & `PyCBA-0.5.1/tests/test_bridge.py`

 * *Files identical despite different names*

### Comparing `PyCBA-0.4.2/tests/test_inf_lines.py` & `PyCBA-0.5.1/tests/test_inf_lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
     assert L == [30.0, 30.0, 30.0, 30.0]
     assert EI == pytest.approx([300000.0, 300000.0, 300000.0, 300000.0])
     assert R == [-1, -1, -1, 0, 0, 0, -1, 0, -1, -1]
     assert eType == [1, 2, 1, 1]
 
 
-def test_distcretization():
+def test_discretization():
     """
     Confirm that poi rounding to find the closest idx for ILs works
     """
 
     beam_str = "P7R7R"
     (L, EI, R, eType) = cba.parse_beam_string(beam_str)
```

