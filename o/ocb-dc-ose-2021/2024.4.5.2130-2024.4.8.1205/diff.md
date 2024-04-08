# Comparing `tmp/ocb-dc-ose-2021-2024.4.5.2130.tar.gz` & `tmp/ocb-dc-ose-2021-2024.4.8.1205.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocb-dc-ose-2021-2024.4.5.2130.tar", last modified: Fri Apr  5 19:30:35 2024, max compression
+gzip compressed data, was "ocb-dc-ose-2021-2024.4.8.1205.tar", last modified: Mon Apr  8 10:05:08 2024, max compression
```

## Comparing `ocb-dc-ose-2021-2024.4.5.2130.tar` & `ocb-dc-ose-2021-2024.4.8.1205.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:30:35.587246 ocb-dc-ose-2021-2024.4.5.2130/
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1071 2024-03-30 21:52:11.000000 ocb-dc-ose-2021-2024.4.5.2130/LICENSE
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      272 2024-04-05 19:30:35.587246 ocb-dc-ose-2021-2024.4.5.2130/PKG-INFO
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1607 2024-04-05 14:34:37.000000 ocb-dc-ose-2021-2024.4.5.2130/README.md
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:30:35.583246 ocb-dc-ose-2021-2024.4.5.2130/datachallenge/
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:30:35.583246 ocb-dc-ose-2021-2024.4.5.2130/datachallenge/scripts/
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      439 2024-04-04 07:47:54.000000 ocb-dc-ose-2021-2024.4.5.2130/datachallenge/scripts/format_metrics.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      286 2024-04-04 07:47:54.000000 ocb-dc-ose-2021-2024.4.5.2130/datachallenge/scripts/wrap_yaml.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:30:35.583246 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)       81 2024-04-05 16:51:06.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/__init__.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:30:35.587246 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-30 21:52:11.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/__init__.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1357 2024-04-05 14:34:04.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/cmems_get.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3042 2024-04-05 14:33:56.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/interp_on_track.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     5267 2024-04-05 14:33:36.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/lambdax.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     2504 2024-04-05 14:33:23.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/mu.py
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3582 2024-04-05 19:24:49.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/prepare_track.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:30:35.587246 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/pipelines/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-30 21:53:54.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/pipelines/__init__.py
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     2614 2024-04-05 18:21:13.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/pipelines/input_data.py
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     3320 2024-04-05 17:20:42.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/pipelines/metrics.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 19:30:35.587246 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021.egg-info/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      272 2024-04-05 19:30:35.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021.egg-info/PKG-INFO
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      690 2024-04-05 19:30:35.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021.egg-info/SOURCES.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        1 2024-04-05 19:30:35.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021.egg-info/dependency_links.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      162 2024-04-05 19:30:35.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021.egg-info/entry_points.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       22 2024-04-05 19:30:35.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021.egg-info/requires.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       48 2024-04-05 19:30:35.000000 ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021.egg-info/top_level.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      637 2024-04-05 19:29:18.000000 ocb-dc-ose-2021-2024.4.5.2130/pyproject.toml
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       38 2024-04-05 19:30:35.587246 ocb-dc-ose-2021-2024.4.5.2130/setup.cfg
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 10:05:08.794914 ocb-dc-ose-2021-2024.4.8.1205/
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1071 2024-03-30 21:52:11.000000 ocb-dc-ose-2021-2024.4.8.1205/LICENSE
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      272 2024-04-08 10:05:08.794914 ocb-dc-ose-2021-2024.4.8.1205/PKG-INFO
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1607 2024-04-05 14:34:37.000000 ocb-dc-ose-2021-2024.4.8.1205/README.md
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 10:05:08.790914 ocb-dc-ose-2021-2024.4.8.1205/datachallenge/
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 10:05:08.790914 ocb-dc-ose-2021-2024.4.8.1205/datachallenge/scripts/
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      439 2024-04-04 07:47:54.000000 ocb-dc-ose-2021-2024.4.8.1205/datachallenge/scripts/format_metrics.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      286 2024-04-04 07:47:54.000000 ocb-dc-ose-2021-2024.4.8.1205/datachallenge/scripts/wrap_yaml.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 10:05:08.790914 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)       81 2024-04-05 16:51:06.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/__init__.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 10:05:08.794914 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-30 21:52:11.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/__init__.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     1357 2024-04-05 14:34:04.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/cmems_get.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3042 2024-04-05 14:33:56.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/interp_on_track.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     5267 2024-04-05 14:33:36.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/lambdax.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     2504 2024-04-05 14:33:23.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/mu.py
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)     3667 2024-04-08 09:53:22.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/prepare_track.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 10:05:08.794914 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/pipelines/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-30 21:53:54.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/pipelines/__init__.py
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     2614 2024-04-05 18:21:13.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/pipelines/input_data.py
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     3320 2024-04-05 17:20:42.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/pipelines/metrics.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-08 10:05:08.794914 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021.egg-info/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      272 2024-04-08 10:05:08.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021.egg-info/PKG-INFO
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      690 2024-04-08 10:05:08.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021.egg-info/SOURCES.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        1 2024-04-08 10:05:08.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021.egg-info/dependency_links.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      162 2024-04-08 10:05:08.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021.egg-info/entry_points.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       22 2024-04-08 10:05:08.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021.egg-info/requires.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       48 2024-04-08 10:05:08.000000 ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021.egg-info/top_level.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      637 2024-04-08 08:32:30.000000 ocb-dc-ose-2021-2024.4.8.1205/pyproject.toml
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       38 2024-04-08 10:05:08.794914 ocb-dc-ose-2021-2024.4.8.1205/setup.cfg
```

### Comparing `ocb-dc-ose-2021-2024.4.5.2130/LICENSE` & `ocb-dc-ose-2021-2024.4.8.1205/LICENSE`

 * *Files identical despite different names*

### Comparing `ocb-dc-ose-2021-2024.4.5.2130/README.md` & `ocb-dc-ose-2021-2024.4.8.1205/README.md`

 * *Files identical despite different names*

### Comparing `ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/cmems_get.py` & `ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/cmems_get.py`

 * *Files identical despite different names*

### Comparing `ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/interp_on_track.py` & `ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/interp_on_track.py`

 * *Files identical despite different names*

### Comparing `ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/lambdax.py` & `ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/lambdax.py`

 * *Files identical despite different names*

### Comparing `ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/mu.py` & `ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/mu.py`

 * *Files identical despite different names*

### Comparing `ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/mods/prepare_track.py` & `ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/mods/prepare_track.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,57 +67,54 @@
     log.debug(f"Returning {ds=}")
     return ds
 
 
 def prepare_track(
     input_paths: str | Sequence[str],
     output_path: str,
-    preprocess: Callable[xr.Dataset, xr.Dataset],
+    preprocess: Callable[[xr.Dataset], xr.Dataset],
+    sort_paths: bool = True,
 ):
     """
     Open multifile dataset to be contatenated by time apply processing and write output
 
     Args:
         input_paths (str | Path | Sequence): path(s) to input netcdf file(s)
         output_path (str): path where to write the output
         preprocess (callable): function to apply to each netcdf
+        sort_paths (bool): whether to sort input_paths before concatenation
     """
     Path(output_path).parent.mkdir(parents=True, exist_ok=True)
     log.info(f"Starting")
+    if sort_paths:
+        log.debug(f"Sorting {input_paths=}")
+        input_paths = sorted(input_paths)
     log.debug(f"Opening {input_paths=}")
     log.debug(f"Applying preprocessing {preprocess}")
     log.debug(f"{getattr(preprocess, '__doc__', '')}")
-    xr.open_mfdataset(
+    ds = xr.open_mfdataset(
         input_paths,
         preprocess=preprocess,
         combine="nested",
         concat_dim="time",
-    ).to_netcdf(output_path)
+    )
+    log.debug(f"Writing to {output_path}")
+    ds.to_netcdf(output_path)
     log.info("Done")
 
 
-def sorted_glob(pathname: str):
-    """
-
-    Args:
-        pathname: file pattern to select
-
-    Returns: Sorted list of files matching pathname
-
-    """
-    return sorted(glob.glob(pathname=pathname, recursive=True))
-
-
 b = hydra_zen.make_custom_builds_fn(populate_full_signature=True)
 pb = hydra_zen.make_custom_builds_fn(zen_partial=True, populate_full_signature=True)
 
 run, cfg = aprl.part.register(
     prepare_track,
     base_args=dict(
-        input_paths=b(sorted_glob, pathname="data/downloads/ref/**/*.nc"),
+        input_paths=b(
+            glob.iglob, pathname="data/downloads/ref/**/*.nc", recursive=True
+        ),
         output_path="data/prepared/ref/default.nc",
         preprocess=pb(
             preprocess_track,
             min_lon=-65,
             max_lon=-55,
             min_lat=33,
             max_lat=43,
```

### Comparing `ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/pipelines/input_data.py` & `ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/pipelines/input_data.py`

 * *Files identical despite different names*

### Comparing `ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021/pipelines/metrics.py` & `ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021/pipelines/metrics.py`

 * *Files identical despite different names*

### Comparing `ocb-dc-ose-2021-2024.4.5.2130/ocb_dc_ose_2021.egg-info/SOURCES.txt` & `ocb-dc-ose-2021-2024.4.8.1205/ocb_dc_ose_2021.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocb-dc-ose-2021-2024.4.5.2130/pyproject.toml` & `ocb-dc-ose-2021-2024.4.8.1205/pyproject.toml`

 * *Files identical despite different names*

