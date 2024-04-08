# Comparing `tmp/pyrsig-0.7.0.tar.gz` & `tmp/pyrsig-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsig-0.7.0.tar", last modified: Wed Nov 22 12:40:08 2023, max compression
+gzip compressed data, was "pyrsig-0.8.2.tar", last modified: Mon Apr  8 16:54:44 2024, max compression
```

## Comparing `pyrsig-0.7.0.tar` & `pyrsig-0.8.2.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-11-22 12:40:08.932036 pyrsig-0.7.0/
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.7.0/LICENSE
--rw-r--r--   0 bhenders (83225) romo       (131)     3517 2023-11-22 12:40:08.931694 pyrsig-0.7.0/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)     3019 2023-11-16 21:15:29.000000 pyrsig-0.7.0/README.md
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-11-22 12:40:08.924207 pyrsig-0.7.0/pyrsig/
--rw-r--r--   0 bhenders (83225) romo       (131)    64690 2023-11-20 21:09:07.000000 pyrsig-0.7.0/pyrsig/__init__.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-11-22 12:40:08.931243 pyrsig-0.7.0/pyrsig/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.7.0/pyrsig/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.7.0/pyrsig/tests/test_api.py
--rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.7.0/pyrsig/tests/test_coards.py
--rw-r--r--   0 bhenders (83225) romo       (131)     3129 2023-06-08 20:39:38.000000 pyrsig-0.7.0/pyrsig/tests/test_dataframes.py
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-11-16 19:56:26.000000 pyrsig-0.7.0/pyrsig/tests/test_gui.py
--rw-r--r--   0 bhenders (83225) romo       (131)     3576 2023-10-10 18:23:29.000000 pyrsig-0.7.0/pyrsig/tests/test_ioapi.py
--rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.7.0/pyrsig/tests/test_misc.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-11-22 12:40:08.927181 pyrsig-0.7.0/pyrsig.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)     3517 2023-11-22 12:40:08.925037 pyrsig-0.7.0/pyrsig.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-11-22 12:40:08.925598 pyrsig-0.7.0/pyrsig.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-11-22 12:40:08.926164 pyrsig-0.7.0/pyrsig.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-11-22 12:40:08.926656 pyrsig-0.7.0/pyrsig.egg-info/requires.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-11-22 12:40:08.927257 pyrsig-0.7.0/pyrsig.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-11-22 12:40:08.932318 pyrsig-0.7.0/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-11-16 20:59:18.000000 pyrsig-0.7.0/setup.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-08 16:54:44.709510 pyrsig-0.8.2/
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.8.2/LICENSE
+-rw-r--r--   0 bhenders (83225) romo       (131)     3678 2024-04-08 16:54:44.709256 pyrsig-0.8.2/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)     3180 2024-04-08 16:48:39.000000 pyrsig-0.8.2/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-08 16:54:44.701291 pyrsig-0.8.2/pyrsig/
+-rw-r--r--   0 bhenders (83225) romo       (131)    53734 2024-04-08 16:48:46.000000 pyrsig-0.8.2/pyrsig/__init__.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-08 16:54:44.705100 pyrsig-0.8.2/pyrsig/cmaq/
+-rw-r--r--   0 bhenders (83225) romo       (131)     7162 2024-03-07 22:09:38.000000 pyrsig-0.8.2/pyrsig/cmaq/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     5581 2024-03-11 19:31:34.000000 pyrsig-0.8.2/pyrsig/cmaq/pair.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-08 16:54:44.708890 pyrsig-0.8.2/pyrsig/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.8.2/pyrsig/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-12-14 22:29:06.000000 pyrsig-0.8.2/pyrsig/tests/test_api.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.8.2/pyrsig/tests/test_coards.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3129 2023-06-08 20:39:38.000000 pyrsig-0.8.2/pyrsig/tests/test_dataframes.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-11-16 19:56:26.000000 pyrsig-0.8.2/pyrsig/tests/test_gui.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3576 2023-10-10 18:23:29.000000 pyrsig-0.8.2/pyrsig/tests/test_ioapi.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.8.2/pyrsig/tests/test_misc.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     8301 2024-03-11 21:02:29.000000 pyrsig-0.8.2/pyrsig/utils.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    20959 2024-04-08 13:39:40.000000 pyrsig-0.8.2/pyrsig/xdr.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-08 16:54:44.704062 pyrsig-0.8.2/pyrsig.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)     3678 2024-04-08 16:54:44.701941 pyrsig-0.8.2/pyrsig.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)      456 2024-04-08 16:54:44.702486 pyrsig-0.8.2/pyrsig.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2024-04-08 16:54:44.703028 pyrsig-0.8.2/pyrsig.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       23 2024-04-08 16:54:44.703596 pyrsig-0.8.2/pyrsig.egg-info/requires.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        7 2024-04-08 16:54:44.704138 pyrsig-0.8.2/pyrsig.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2024-04-08 16:54:44.709732 pyrsig-0.8.2/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-11-16 20:59:18.000000 pyrsig-0.8.2/setup.py
```

### Comparing `pyrsig-0.7.0/LICENSE` & `pyrsig-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsig-0.7.0/PKG-INFO` & `pyrsig-0.8.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.7.0
+Version: 0.8.2
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
@@ -105,14 +105,17 @@
 # 3875
 ```
 
 ## Change Log
 
 Not all changes are listed, but notable changes are itemized for ease of review.
 
+* v0.8.2: Added xdr CALIPSO 1.0 format capability.
+* v0.8.1: Added xdr Point 1.0 format capability.
+* v0.8.0: Restructuring module code and adding CMAQ pairing.
 * v0.7.0: Added offline descriptions for review of space/time coverage.
 * v0.7.0: Added TEMPO options for screening
 * v0.6.0: Added latitude longitude grid pass thru support.
 * v0.5.1: Added convenience function for opening many IOAPI files at once.
 * v0.5.1: Updated TEMPO proxy naming.
 * v0.4.6: Added support for legacy TLS servers (e.g, ofmpub and maple)
 * v0.4.5: Updated TEMPO proxy naming
```

### Comparing `pyrsig-0.7.0/README.md` & `pyrsig-0.8.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,17 @@
 # 3875
 ```
 
 ## Change Log
 
 Not all changes are listed, but notable changes are itemized for ease of review.
 
+* v0.8.2: Added xdr CALIPSO 1.0 format capability.
+* v0.8.1: Added xdr Point 1.0 format capability.
+* v0.8.0: Restructuring module code and adding CMAQ pairing.
 * v0.7.0: Added offline descriptions for review of space/time coverage.
 * v0.7.0: Added TEMPO options for screening
 * v0.6.0: Added latitude longitude grid pass thru support.
 * v0.5.1: Added convenience function for opening many IOAPI files at once.
 * v0.5.1: Updated TEMPO proxy naming.
 * v0.4.6: Added support for legacy TLS servers (e.g, ofmpub and maple)
 * v0.4.5: Updated TEMPO proxy naming
```

### Comparing `pyrsig-0.7.0/pyrsig/__init__.py` & `pyrsig-0.8.2/pyrsig/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,15 @@
-__all__ = ['RsigApi', 'RsigGui', 'open_ioapi', 'open_mfioapi']
-__version__ = '0.7.0'
+__all__ = ['RsigApi', 'RsigGui', 'open_ioapi', 'open_mfioapi', 'cmaq']
+__version__ = '0.8.2'
 
+from . import cmaq
+from .cmaq import open_ioapi, open_mfioapi
 import pandas as pd
 import requests
-
-_def_grid_kw = {
-    '12US1': dict(
-        GDNAM='12US1', GDTYP=2, NCOLS=459, NROWS=299,
-        XORIG=-2556000.0, YORIG=-1728000.0, XCELL=12000., YCELL=12000.,
-        P_ALP=33., P_BET=45., P_GAM=-97., XCENT=-97., YCENT=40.
-    ),
-    '4US1': dict(
-        GDNAM='4US1', GDTYP=2, NCOLS=459 * 3, NROWS=299 * 3,
-        XORIG=-2556000.0, YORIG=-1728000.0, XCELL=4000., YCELL=4000.,
-        P_ALP=33., P_BET=45., P_GAM=-97., XCENT=-97., YCENT=40.
-    ),
-    '1US1': dict(
-        GDNAM='1US1', GDTYP=2, NCOLS=459 * 12, NROWS=299 * 12,
-        XORIG=-2556000.0, YORIG=-1728000.0, XCELL=1000., YCELL=1000.,
-        P_ALP=33., P_BET=45., P_GAM=-97., XCENT=-97., YCENT=40.
-    ),
-    '12US2': dict(
-        GDNAM='12US2', GDTYP=2, NCOLS=396, NROWS=246,
-        XORIG=-2412000.0, YORIG=-1620000.0, XCELL=12000., YCELL=12000.,
-        P_ALP=33., P_BET=45., P_GAM=-97., XCENT=-97., YCENT=40.
-    ),
-    '4US2': dict(
-        GDNAM='4US2', GDTYP=2, NCOLS=396 * 3, NROWS=246 * 3,
-        XORIG=-2412000.0, YORIG=-1620000.0, XCELL=4000., YCELL=4000.,
-        P_ALP=33., P_BET=45., P_GAM=-97., XCENT=-97., YCENT=40.
-    ),
-    '1US2': dict(
-        GDNAM='1US2', GDTYP=2, NCOLS=396 * 12, NROWS=246 * 12,
-        XORIG=-2412000.0, YORIG=-1620000.0, XCELL=1000., YCELL=1000.,
-        P_ALP=33., P_BET=45., P_GAM=-97., XCENT=-97., YCENT=40.
-    ),
-    '36US3': dict(
-        GDNAM='36US3', GDTYP=2, NCOLS=172, NROWS=148,
-        XORIG=-2952000.0, YORIG=-2772000.0, XCELL=36000., YCELL=36000.,
-        P_ALP=33., P_BET=45., P_GAM=-97., XCENT=-97., YCENT=40.
-    ),
-    '108NHEMI2': dict(
-        GDNAM='108NHEMI2', GDTYP=6, NCOLS=187, NROWS=187,
-        XORIG=-10098000.0, YORIG=-10098000.0, XCELL=108000., YCELL=108000.,
-        P_ALP=1., P_BET=45., P_GAM=-98., XCENT=-98., YCENT=90.
-    ),
-    '36NHEMI2': dict(
-        GDNAM='36NHEMI2', GDTYP=6, NCOLS=187 * 3, NROWS=187 * 3,
-        XORIG=-10098000.0, YORIG=-10098000.0, XCELL=36000., YCELL=36000.,
-        P_ALP=1., P_BET=45., P_GAM=-98., XCENT=-98., YCENT=90.
-    ),
-    'NORTHSOUTHAM': dict(
-        GDNAM='NORTHSOUTHAM', GDTYP=7, NCOLS=179, NROWS=154,
-        XORIG=251759.25, YORIG=-1578187., XCELL=27000., YCELL=27000.,
-        P_ALP=0., P_BET=0., P_GAM=-98., XCENT=-98., YCENT=0.
-    ),
-    'global_1pt0': dict(
-        GDNAM='GLOBAL', GDTYP=1, NCOLS=360, NROWS=180,
-        XORIG=-180, YORIG=-90, XCELL=1., YCELL=1.,
-        P_ALP=0., P_BET=0., P_GAM=0., XCENT=0., YCENT=0.
-    ),
-    'global_0pt1': dict(
-        GDNAM='GLOBAL', GDTYP=1, NCOLS=3600, NROWS=1800,
-        XORIG=-180, YORIG=-90, XCELL=0.1, YCELL=0.1,
-        P_ALP=0., P_BET=0., P_GAM=0., XCENT=0., YCENT=0.
-    ),
-}
-
-_shared_grid_kw = dict(
-    VGTYP=7, VGTOP=5000., NLAYS=35, earth_radius=6370000., g=9.81, R=287.04,
-    A=50., T0=290, P0=1000e2, REGRID_AGGREGATE='None'
-)
-
-for key in _def_grid_kw:
-    for pk, pv in _shared_grid_kw.items():
-        _def_grid_kw[key].setdefault(pk, pv)
+from .utils import customize_grid, def_grid_kw as _def_grid_kw
 
 # Used to shorten pandora names for 80 character PEP
 _trvca = 'tropospheric_vertical_column_amount'
 
 _keys = (
     'airnow.pm25', 'airnow.pm10', 'airnow.ozone', 'airnow.no', 'airnow.no2',
     'airnow.nox', 'airnow.so2', 'airnow.co', 'airnow.temperature',
@@ -102,15 +33,15 @@
     'nesdis.nh3', 'nesdis.nox', 'nesdis.so2', 'nesdis.tnmhc',
     'pandora.ozone'
     f'pandora.L2_rfuh5p1_8.formaldehyde_{_trvca}',
     f'pandora.L2_rfuh5p1_8.formaldehyde_{_trvca}_uncertainty',
     'pandora.L2_rfus5p1_8.direct_formaldehyde_air_mass_factor',
     'pandora.L2_rfus5p1_8.direct_formaldehyde_air_mass_factor_uncertainty',
     'pandora.L2_rfus5p1_8.formaldehyde_total_vertical_column_amount',
-    'pandora.L2_rfus5p1_8.formaldehyde_vertical_column_amount_uncertainty'
+    'pandora.L2_rfus5p1_8.formaldehyde_vertical_column_amount_uncertainty',
     f'pandora.L2_rnvh3p1_8.water_vapor_{_trvca}',
     f'pandora.L2_rnvh3p1_8.water_vapor_{_trvca}_uncertainty',
     'pandora.L2_rnvs3p1_8.nitrogen_dioxide_vertical_column_amount',
     'pandora.L2_rnvh3p1_8.tropospheric_nitrogen_dioxide',
     'pandora.L2_rnvh3p1_8.tropospheric_nitrogen_dioxide_uncertainty',
     'pandora.L2_rnvs3p1_8.direct_nitrogen_dioxide_air_mass_factor',
     'pandora.L2_rnvs3p1_8.direct_nitrogen_dioxide_air_mass_factor_uncertainty',
@@ -160,15 +91,16 @@
     'tropomi.offl.co.carbonmonoxide_total_column',
     'tropomi.offl.ch4.methane_mixing_ratio',
     'tropomi.offl.ch4.methane_mixing_ratio_bias_corrected',
     'viirsnoaa.jrraod.AOD550', 'viirsnoaa.vaooo.AerosolOpticalDepth_at_550nm',
 )
 
 _nocorner_prefixes = (
-    'airnow', 'aqs', 'purpleair', 'pandora', 'cmaq', 'regridded'
+    'airnow', 'aqs', 'purpleair', 'pandora', 'cmaq', 'regridded',
+    'calipso'
 )
 _nolonlats_prefixes = ('cmaq', 'regridded')
 _noregrid_prefixes = ('cmaq', 'regridded')
 
 
 def _actionf(msg, action, ErrorTyp=None):
     """
@@ -304,30 +236,44 @@
 
 
 class LegacyAdapter(requests.adapters.HTTPAdapter):
     # "Transport adapter" that allows us to use custom ssl_context.
 
     def __init__(self, **kwargs):
         import ssl
+        def_ctx = ssl._create_default_https_context
+        ssl._create_default_https_context = _create_unverified_tls_context
         ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
         ctx.options |= 0x4  # OP_LEGACY_SERVER_CONNECT
         self.ssl_context = ctx
+        ssl._create_default_https_context = def_ctx
         super().__init__(**kwargs)
 
     def init_poolmanager(self, connections, maxsize, block=False):
         import urllib3
         self.poolmanager = urllib3.poolmanager.PoolManager(
             num_pools=connections, maxsize=maxsize,
             block=block, ssl_context=self.ssl_context)
 
 
-def legacy_get(*args, **kwds):
+def legacy_get(url, *args, **kwds):
+    import copy
     session = requests.session()
-    session.mount('https://', LegacyAdapter())
-    return session.get(*args, **kwds)
+    la = LegacyAdapter()
+
+    # Maple has a bad certificate, so here if you are using maple
+    # I disable the certificate, but no the warning
+    if 'maple' in url:
+        la.ssl_context.check_hostname = False
+        kwds = copy.copy(kwds)
+        kwds.setdefault('verify', False)
+
+    session.mount('https://', la)
+
+    return session.get(url, *args, **kwds)
 
 
 def _getfile(url, outpath, maxtries=5, verbose=1, overwrite=False):
     """
     Download file from RSIG using fault tolerance and optional caching
     when overwrite is False.
 
@@ -400,366 +346,19 @@
 
         if verbose > 0:
             print('')
 
     ssl._create_default_https_context = _def_https_context
 
 
-def get_proj4(attrs, earth_radius=6370000.):
-    """
-    Create a proj4 formatted grid definition using IOAPI attrs and earth_radius
-
-    Arguments
-    ---------
-    attrs : dict-like
-        Mappable of IOAPI properties that supports the items method
-    earth_radius : float
-        Assumed radius of the earth. 6370000 is the WRF default.
-
-    Returns
-    -------
-    projstr : str
-        proj4 formatted string such that the domain southwest corner starts at
-        (0, 0) and ends at (NCOLS, NROWS)
-    """
-    props = {k: v for k, v in attrs.items()}
-    props['x_0'] = -props['XORIG']
-    props['y_0'] = -props['YORIG']
-    props.setdefault('earth_radius', earth_radius)
-
-    if props['GDTYP'] == 1:
-        projstr = '+proj=lonlat +R={earth_radius}'.format(**props)
-    elif props['GDTYP'] == 2:
-        projstr = (
-            '+proj=lcc +lat_1={P_ALP} +lat_2={P_BET} +lat_0={YCENT}'
-            ' +lon_0={XCENT} +R={earth_radius} +x_0={x_0} +y_0={y_0}'
-            ' +to_meter={XCELL} +no_defs'
-        ).format(**props)
-    elif props['GDTYP'] == 6:
-        projstr = (
-            '+proj=stere +lat_0={lat_0} +lat_ts={P_BET} +lon_0={XCENT}'
-            + ' +x_0={x_0} +y_0={y_0} +R={earth_radius} +to_meter={XCELL}'
-            + ' +no_defs'
-        ).format(lat_0=props['P_ALP'] * 90, **props)
-    elif props['GDTYP'] == 7:
-        projstr = (
-            '+proj=merc +R={earth_radius} +lat_ts=0 +lon_0={XCENT}'
-            + ' +x_0={x_0} +y_0={y_0} +to_meter={XCELL}'
-            + ' +no_defs'
-        ).format(**props)
-    else:
-        raise ValueError('GDTYPE {GDTYP} not implemented'.format(**props))
-
-    return projstr
-
-
-def customize_grid(grid_kw, bbox, clip=True):
-    """
-    Redefine grid_kw to cover bbox by removing extra rows and columns and
-    redefining XORIG, YORIG, NCOLS and NROWS.
-
-    Arguments
-    ---------
-    grid_kw : dict or str
-        If str, must be a known grid in default grids.
-        If dict, must include all IOAPI grid metadata properties
-    bbox : tuple
-        wlon, slat, elon, nlat in decimal degrees (-180 to 180)
-    clip : bool
-        If True, limit grid to original grid bounds
-
-    Returns
-    -------
-    ogrid_kw : dict
-        IOAPI grid metadata properties with XORIG/YORIG and NCOLS/NROWS
-        adjusted such that it only covers bbox or (if clip) only covers
-        the portion of bbox covered by the original grid_kw.
-    """
-    import pyproj
-    import numpy as np
-
-    if isinstance(grid_kw, str):
-        grid_kw = _def_grid_kw[grid_kw]
-
-    ogrid_kw = {k: v for k, v in grid_kw.items()}
-    # Lonlat box must be treated separately
-    if ogrid_kw['GDTYP'] == 1:
-        llx, lly = bbox[:2]
-        urx, ury = bbox[2:]
-        ncols = int(np.ceil((urx - llx) / ogrid_kw['XCELL']) + 4)
-        nrows = int(np.ceil((ury - lly) / ogrid_kw['YCELL']) + 4)
-        xorig = (int(llx / ogrid_kw['XCELL']) - 1) * ogrid_kw['XCELL']
-        yorig = (int(lly / ogrid_kw['YCELL']) - 1) * ogrid_kw['YCELL']
-        ogrid_kw['NCOLS'] = ncols
-        ogrid_kw['NROWS'] = nrows
-        ogrid_kw['XORIG'] = xorig
-        ogrid_kw['YORIG'] = yorig
-        return ogrid_kw
-
-    proj4str = get_proj4(grid_kw)
-    proj = pyproj.Proj(proj4str)
-    llx, lly = proj(*bbox[:2])
-    urx, ury = proj(*bbox[2:])
-    midx, midy = proj((bbox[0] + bbox[2]) / 2, (bbox[1] + bbox[3]) / 2)
-    maxy = np.max([lly, ury, midy])
-    miny = np.min([lly, ury, midy])
-    maxx = np.max([llx, urx, midx])
-    minx = np.min([llx, urx, midx])
-
-    lli, llj = np.floor([minx, miny]).astype('i')
-    uri, urj = np.ceil([maxx, maxy]).astype('i')
-    if clip:
-        lli, llj = np.maximum(0, [lli, llj])
-        uri = np.minimum(grid_kw['NCOLS'], uri)
-        urj = np.minimum(grid_kw['NROWS'], urj)
-    ogrid_kw['XORIG'] = grid_kw['XORIG'] + lli * grid_kw['XCELL']
-    ogrid_kw['YORIG'] = grid_kw['YORIG'] + llj * grid_kw['YCELL']
-    ogrid_kw['NCOLS'] = uri - lli
-    ogrid_kw['NROWS'] = urj - llj
-    return ogrid_kw
-
-
-def save_ioapi(ds, path, format='NETCDF3_CLASSIC', **kwds):
-    """
-    Providing a function to clean-up meta-data for IOAPI.
-
-    Arguments
-    ---------
-    ds : xr.Dataset
-        Dataset that should be saved as IOAPI. Dimensions and coordinates
-        must support the conversion.
-    path : str
-        Path to save ioapi file
-    format : str
-        'NETCDF3_CLASSIC' or 'NETCDF4_CLASSIC'
-    kwds :
-        Passed to xr.Dataset.to_netcdf
-
-    Returns
-    -------
-    ds.to_netcdf
-        Saved file
-    """
-    import pandas as pd
-    import xarray as xr
-    import numpy as np
-
-    ods = ds[[]].copy(deep=True)
-    props = ods.attrs
-    props.update(ds.attrs)
-    outkeys = [
-        vk for vk, vv in ds.data_vars.items()
-        if 'PERIM' in vv.dims or 'ROW' in vv.dims
-    ]
-    nv = len(outkeys)
-    if 'ROW' in ds[outkeys[0]].dims:
-        ods.attrs['FTYPE'] = 1
-    elif 'PERIM' in ds[outkeys[0]].dims:
-        ods.attrs['FTYPE'] = 2
-
-    assert len(set([k[:16] for k in outkeys])) == nv
-    varlist = ''.join([k[:16].ljust(16) for k in outkeys])
-    dates = pd.to_datetime(ds.TSTEP.values)
-    dt = np.diff(dates).astype('d').max() / 1e9
-
-    dth = dt // 3600
-    dtm = (dt % 3600) // 60
-    dts = (dt % 60) // 1
-    timec = pd.to_datetime(
-        ds.TSTEP.min().values
-        + np.arange(len(dates)) * pd.to_timedelta(dt, unit='s')
-    )
-    jdays = timec.strftime('%Y%j').astype('i')
-    hms = timec.strftime('%H%M%S').astype('i')
-    ods['TFLAG'] = xr.DataArray(
-        np.array([jdays, hms]).T, name='TFLAG', dims=('TSTEP', 'DATE-TIME'),
-        attrs=dict(
-            long_name='TFLAG'.ljust(16), units='<YYYYJJJ,HHMMSS>',
-            var_desc='Time flag'.ljust(80)
-        )
-    ).expand_dims(VAR=nv).transpose('TSTEP', 'VAR', 'DATE-TIME')
-    ods.attrs['SDATE'] = int(ods['TFLAG'][0, 0, 0])
-    ods.attrs['STIME'] = int(ods['TFLAG'][0, 0, 1])
-    ods.attrs['TSTEP'] = int(f'{dth:.0f}{dtm:02.0f}{dts:02.0f}')
-
-    for dk in outkeys:
-        ok = dk[:16]
-        ods[ok] = ds[dk].copy()
-        vprops = ods[ok].attrs
-        vprops['long_name'] = vprops.get('long_name', ok)[:16].ljust(16)
-        vprops['var_desc'] = vprops.get('var_desc', ok)[:80].ljust(80)
-        vprops['units'] = vprops.get('units', 'unknown')[:16].ljust(16)
-
-    now = pd.to_datetime('now', utc=True)
-    props['CDATE'] = props['WDATE'] = int(now.strftime('%Y%j'))
-    props['CTIME'] = props['WTIME'] = int(now.strftime('%H%M%S'))
-    props['NCOLS'], props['NROWS'] = ds.dims['COL'], ds.dims['ROW']
-    props['NLAYS'], props['NVARS'] = ds.dims['LAY'], ods.dims['VAR']
-    props['XORIG'] = float(props['XORIG'] + ds.COL.min() - 0.5)
-    props['YORIG'] = float(props['YORIG'] + ds.COL.min() - 0.5)
-    s = [1]
-    for i, sm in enumerate(ods.LAY):
-        s.append(2 * sm - s[-1])
-
-    props['VAR-LIST'] = varlist
-    props['VGLVLS'] = np.array(s, dtype='f')
-    props['UPNAM'] = f'pyrsig {__version__}'.ljust(16)
-    defprops = {
-        'IOAPI_VERSION': 'not applicable'.ljust(16), 'EXEC_ID': '?'.ljust(80),
-        'FTYPE': 1, 'NTHIK': 1, 'GDTYP': 2, 'P_ALP': 33.0, 'P_BET': 45.0,
-        'P_GAM': -97.0, 'XCENT': -97.0, 'YCENT': 40.0,
-        'VGTYP': -9999, 'VGTOP': np.float32(5000.0),
-        'GDNAM': f'{"UNKNOWN":16s}'.ljust(16), 'metadata': ''
-    }
-
-    for pk, pdef in defprops.items():
-        ods.attrs.setdefault(pk, pdef)
-
-    return ods.to_netcdf(path, format=format, **kwds)
-
-
-def open_ioapi(path, metapath=None, earth_radius=6370000.):
-    """
-    Open an IOAPI file, add coordinate data, and optionally add RSIG metadata.
-
-    Arguments
-    ---------
-    path : str
-        Path to IOAPI formatted files.
-    metapath : str
-        Path to metadata associated with the RSIG query. The metadata will be
-        added as metadata global property.
-    earth_radius : float
-        Assumed radius of the earth. 6370000 is the WRF default.
-
-    Returns
-    -------
-    ds : xarray.Dataset
-        Dataset with IOAPI metadata
-    """
-    import xarray as xr
-
-    f = xr.open_dataset(path, engine='netcdf4')
-    f = add_ioapi_meta(
-        f, path=path, metapath=metapath, earth_radius=earth_radius
-    )
-    return f
-
-
-def add_ioapi_meta(ds, metapath=None, earth_radius=6370000., path=''):
-    """
-    Open an IOAPI file, add coordinate data, and optionally add RSIG metadata.
-
-    Arguments
-    ---------
-    ds : xr.Dataset
-        IOAPI dataset Path to IOAPI formatted files.
-    metapath : str
-        Path to metadata associated with the RSIG query. The metadata will be
-        added as metadata global property.
-    earth_radius : float
-        Assumed radius of the earth. 6370000 is the WRF default.
-
-    Returns
-    -------
-    outds : xarray.Dataset
-        Dataset with IOAPI metadata
-    """
-    import numpy as np
-    import warnings
-    f = ds
-    lvls = f.attrs['VGLVLS']
-    tflag = f['TFLAG'].astype('i').values[:, 0, :]
-    yyyyjjj = tflag[:, 0]
-    yyyyjjj = np.where(yyyyjjj < 1, 1970001, yyyyjjj)
-    HHMMSS = tflag[:, 1]
-    tstrs = []
-    for j, t in zip(yyyyjjj, HHMMSS):
-        tstrs.append(f'{j:07d}T{t:06d}')
-
-    try:
-        time = pd.to_datetime(tstrs, format='%Y%jT%H%M%S')
-        f.coords['TSTEP'] = time
-    except Exception:
-        pass
-
-    f.coords['LAY'] = (lvls[:-1] + lvls[1:]) / 2.
-    f.coords['ROW'] = np.arange(f.attrs['NROWS']) + 0.5
-    f.coords['COL'] = np.arange(f.attrs['NCOLS']) + 0.5
-    try:
-        proj4str = get_proj4(f.attrs, earth_radius=earth_radius)
-        f.attrs['crs_proj4'] = proj4str
-    except ValueError as e:
-        warnings.warn(str(e))
-
-    if metapath is None:
-        import os
-        if os.path.exists(path + '.txt'):
-            metapath = path + '.txt'
-
-    if metapath is False:
-        metapath = None
-
-    if metapath is not None:
-        with open(metapath, 'r') as metaf:
-            metatxt = metaf.read()
-        f.attrs['metadata'] = metatxt
-
-    return f
-
-
-def open_mfioapi(
-    paths, metapaths=None, earth_radius=6370000., **kwargs
-):
-    """
-    Minimal version of open_mfdataset that is compatible with open_ioapi.
-    preprocess :  keyword defaults to add_ioapi_meta
-    concat_dim :  keyword defaults to 'TSTEP'
-
-    Arguments
-    ---------
-    paths : iterable
-        Paths to ioapi files to be opened.
-    metapaths : iterable
-        Paths to be added as a string metadata
-    earth_radius : float
-        Radius of the earth for projection.
-    kwargs :
-        See xr.open_mfdataset
-
-    Returns
-    -------
-
-    """
-    import xarray as xr
-    import functools
-
-    addio = functools.partial(add_ioapi_meta, earth_radius=earth_radius)
-    kwargs.setdefault('concat_dim', 'TSTEP')
-    kwargs.setdefault('preprocess', addio)
-    outf = xr.open_mfdataset(paths, **kwargs)
-    if metapaths is None:
-        metapaths = []
-    elif isinstance(metapaths, str):
-        metapaths = [metapaths]
-
-    metastr = ''
-    for metapath in metapaths:
-        with open(metapath, 'r') as mf:
-            metastr += metapath + ':\n' + mf.read()
-
-    outf.attrs['metadata'] = metastr
-
-    return outf
-
-
 class RsigApi:
     def __init__(
         self, key=None, bdate=None, edate=None, bbox=None, grid_kw=None,
         tropomi_kw=None, purpleair_kw=None, viirsnoaa_kw=None, tempo_kw=None,
+        pandora_kw=None, calipso_kw=None,
         server='ofmpub.epa.gov', compress=1, corners=1, encoding=None,
         overwrite=False, workdir='.', gridfit=False
     ):
         """
         RsigApi is a python-based interface to RSIG's web-based API
 
         Arguments
@@ -775,30 +374,37 @@
           wlon, slat, elon, nlat in decimal degrees (-180 to 180)
         grid_kw : str or dict
           If str, must be 12US1, 1US1, 12US2, 1US2, 36US3, 108NHEMI2, 36NHEMI2
           and will be used to set parameters based on EPA domains. If dict,
           IOAPI mapping parameters see default for details.
         viirsnoaa_kw : dict
           Dictionary of VIIRS NOAA filter parameters default
-          {'minimum_quality': 'high'} options include 'high' or 'medium')
+          {'minimum_quality': 'high'} other options 'medium' or 'low'
         tropomi_kw : dict
           Dictionary of TropOMI filter parameters default
           {'minimum_quality': 75, 'maximum_cloud_fraction': 1.0} options
           are 0-100 and 0-1.
         purpleair_kw : dict
           Dictionary of purpleair filter parameters and api_key.
             'out_in_flag': 0, # options 0, 2, ''
-            'freq': 'hourly', # options hourly, daily, monthly, yearly
+            'freq': 'hourly', # options hourly, daily, monthly, yearly, none
             'maximum_difference': 5, # integer
             'maximum_ratio': 0.70, # float
             'agg_pct': 75, # 0-100
-            'api_key': '<your key here>'
+            'default_humidity': 50,
+            'api_key': 'your_key_here'
         tempo_kw : dict
           Dictionary of TEMPO filter parameters default
-            'api_key': '<your password>' # 'password'
+            'api_key': 'your_key_here' # 'password'
+        pandora_kw : dict
+          Dictionary of Pandora filter parameters default
+          {'minimum_quality': 'high'} other options 'medium' or 'low'
+        calipso_kw : dict
+          Dictionary of Calipso filter parameters default
+          {'MINIMUM_CAD': 20, 'MAXIMUM_UNCERTAINTY': 99}
         server : str
           'ofmpub.epa.gov' for external  users
           'maple.hesc.epa.gov' for on EPA VPN users
         compress : int
           1 to transfer files with gzip compression
           0 to transfer uncompressed files (slow)
         encoding : dict
@@ -874,37 +480,63 @@
 
         if gridfit:
             grid_kw = customize_grid(grid_kw, self.bbox)
 
         self.grid_kw = grid_kw
 
         if tropomi_kw is None:
-            tropomi_kw = {'minimum_quality': 75, 'maximum_cloud_fraction': 1.0}
+            tropomi_kw = {}
+
+        tropomi_kw.setdefault('minimum_quality', 75)
+        tropomi_kw.setdefault('maximum_cloud_fraction', 1.0)
 
         self.tropomi_kw = tropomi_kw
 
         if tempo_kw is None:
             tempo_kw = {}
-            tempo_kw['minimum_quality'] = 'normal'
-            tempo_kw['maximum_cloud_fraction'] = 1.0
-            tempo_kw['api_key'] = '<your password>'
+
+        tempo_kw.setdefault('minimum_quality', 'normal')
+        tempo_kw.setdefault('maximum_cloud_fraction', 1.0)
+        tempo_kw.setdefault('api_key', 'your_key_here')
 
         self.tempo_kw = tempo_kw
 
         if viirsnoaa_kw is None:
-            viirsnoaa_kw = {'minimum_quality': 'high'}
+            viirsnoaa_kw = {}
+
+        viirsnoaa_kw.setdefault('minimum_quality', 'high')
 
         self.viirsnoaa_kw = viirsnoaa_kw
 
+        if pandora_kw is None:
+            pandora_kw = {}
+
+        pandora_kw.setdefault('minimum_quality', 'high')
+
+        self.pandora_kw = pandora_kw
+
+        if calipso_kw is None:
+            calipso_kw = {}
+
+        calipso_kw.setdefault('MINIMUM_CAD', 20)
+        calipso_kw.setdefault('MAXIMUM_UNCERTAINTY', 99)
+
+        self.calipso_kw = calipso_kw
+
         if purpleair_kw is None:
-            purpleair_kw = {
-                'out_in_flag': 0, 'freq': 'hourly',
-                'maximum_difference': 5, 'maximum_ratio': 0.70,
-                'agg_pct': 75, 'api_key': '<your key here>'
-            }
+            purpleair_kw = {}
+
+        defpurp_kw = {
+            'out_in_flag': 0, 'freq': 'hourly',
+            'maximum_difference': 5, 'maximum_ratio': 0.70,
+            'agg_pct': 75, 'api_key': 'your_key_here',
+            'default_humidity': 50.000000
+        }
+        for k, v in defpurp_kw.items():
+            purpleair_kw.setdefault(k, v)
 
         self.purpleair_kw = purpleair_kw
 
     def set_grid_kw(self, grid_kw):
         if isinstance(grid_kw, str):
             if grid_kw not in _def_grid_kw:
                 raise KeyError('unknown grid, you must specify properites')
@@ -1060,14 +692,15 @@
             flags=re.MULTILINE + re.DOTALL
         )
 
         # Regex, replacement
         resubsdesc = [
             (descmidre, ''),  # concated coverages have extra open/close tags
             (re.compile('<='), '&lt;='),  # associated with <= 32 in Modis
+            (re.compile('qa_value <'), 'qa_value &lt;'),  # w/ tropomi.ntri
             (
                 mismatchtempre,
                 '</lonLatEnvelope><domainSet><spatialDomain></spatialDomain>',
             ),  # Missing open block for spatialDomain in goes (eg imager.calb)
             (
                 re.compile(r'</CoverageOffering>\s+</CoverageOfferingBrief>'),
                 '</CoverageOffering>',
@@ -1168,16 +801,16 @@
 
     def capabilities(self, as_dataframe=True, refresh=False, verbose=0):
         """
         At this time, the capabilities does not list cmaq.*
         """
         import re
         import pandas as pd
-        import warnings
         import os
+        import io
 
         cappath = os.path.expanduser('~/.pyrsig/GetCapabilities.csv')
         if not refresh and as_dataframe:
             if self._capabilitiesdf is not None:
                 return self._capabilitiesdf
             elif os.path.exists(cappath):
                 self._capabilitiesdf = pd.read_csv(cappath)
@@ -1193,44 +826,50 @@
             os.makedirs(os.path.dirname(cappath), exist_ok=True)
             cre = re.compile(
                 '<CoverageOfferingBrief>.+?</CoverageOfferingBrief>',
                 re.DOTALL + re.M
             )
             gre = re.compile(
                 r'<lonLatEnvelope srsName="WGS84\(DD\)">\s*<gml:pos>(.+?)'
-                + r'</gml:pos>\s*<gml:pos>(.+?)</gml:pos>\s*</lonLatEnvelope>'
-            , re.M)
-            tre = re.compile('>\s+<', re.M)
+                + r'</gml:pos>\s*<gml:pos>(.+?)</gml:pos>\s*</lonLatEnvelope>',
+                re.M
+            )
+            tre = re.compile(r'>\s+<', re.M)
             ctext = self._capabilities.text
             ctext = '\n'.join(cre.findall(ctext))
             ctext = gre.sub(r'<bbox_str>\1 \2</bbox_str>', ctext)
             ctext = tre.sub(r'><', ctext)
             # Cleanup... for known issues
             ctext = ctext.replace('>yyy', '>')
             ctext = ctext.replace('<=', 'less than or equal to ')
+            ctext = ctext.replace('qa_value < 0', 'qa_value less than 0')
             ctext = ctext.replace('>0=', 'greater than 0 =')
             ctext = ctext.replace('<0=', 'less than 0 = ')
             # version 1.5
             if hasattr(pd, 'read_xml'):
                 ctext = f"""<?xml version="1.0" encoding="UTF-8" ?>
                 <WCS_Capabilities>
                 {ctext}
                 </WCS_Capabilities>"""
                 capabilitiesdf = pd.read_xml(io.StringIO(ctext))
             else:
                 ccsv = ctext.replace('"', '\'')
                 ccsv = ccsv.replace('</name><label>', '","')
                 ccsv = ccsv.replace('</label><description>', '","')
                 ccsv = ccsv.replace('</description><bbox_str>', '","')
-                ccsv = ccsv.replace('</bbox_str></CoverageOfferingBrief>', '"\n')
+                ccsv = ccsv.replace(
+                    '</bbox_str></CoverageOfferingBrief>', '"\n'
+                )
                 ccsv = ccsv.replace('<CoverageOfferingBrief><name>', '"')
                 ccsv = 'name,label,description,bbox_str\n' + ccsv
                 capabilitiesdf = pd.read_csv(io.StringIO(ccsv))
 
-            capabilitiesdf['prefix'] = capabilitiesdf['name'].apply(lambda x: x.split('.')[0])
+            capabilitiesdf['prefix'] = capabilitiesdf['name'].apply(
+                lambda x: x.split('.')[0]
+            )
             capabilitiesdf.to_csv(cappath, index=False)
             self._capabilitiesdf = capabilitiesdf
             return self._capabilitiesdf
 
         return self._capabilities
 
     def keys(self, offline=True):
@@ -1241,18 +880,15 @@
             If True, uses small cached set of tested coverages.
             If False, finds all coverages from capabilities service.
 
         """
         if offline:
             keys = tuple(_keys)
         else:
-            keys = []
-            for line in self.capabilities().text.split('\n'):
-                if line.startswith('            <name>'):
-                    keys.append(line.split('name')[1][1:-2])
+            keys = sorted(self.capabilities(refresh=True).name.unique())
 
         return keys
 
     def get_file(
         self, formatstr, key=None, bdate=None, edate=None, bbox=None,
         grid=False, request='GetCoverage', compress=0, overwrite=None,
         verbose=0
@@ -1324,14 +960,16 @@
 
         corners = self.corners
         grid_kw = self.grid_kw
         purpleair_kw = self.purpleair_kw
         tropomi_kw = self.tropomi_kw
         tempo_kw = self.tempo_kw
         viirsnoaa_kw = self.viirsnoaa_kw
+        pandora_kw = self.pandora_kw
+        calipso_kw = self.calipso_kw
         if compress is None:
             compress = self.compress
 
         wlon, slat, elon, nlat = bbox
 
         # If already gridded, do not use grid keywords
         nogridkw = any([key.startswith(pre) for pre in _noregrid_prefixes])
@@ -1344,36 +982,57 @@
         if key.startswith('viirsnoaa'):
             viirsnoaastr = '&MINIMUM_QUALITY={minimum_quality}'.format(
                 **viirsnoaa_kw
             )
         else:
             viirsnoaastr = ''
 
+        if key.startswith('pandora'):
+            pandorastr = '&MINIMUM_QUALITY={minimum_quality}'.format(
+                **pandora_kw
+            )
+        else:
+            pandorastr = ''
+
+        if key.startswith('calipso'):
+            calipsostr = (
+                '&MINIMUM_CAD={MINIMUM_CAD}'
+                + '&MAXIMUM_UNCERTAINTY={MAXIMUM_UNCERTAINTY}'
+            ).format(**calipso_kw)
+        else:
+            calipsostr = ''
+
         if key.startswith('tropomi'):
             tropomistr = (
                 '&MINIMUM_QUALITY={minimum_quality}'
                 '&MAXIMUM_CLOUD_FRACTION={maximum_cloud_fraction}'
             ).format(**tropomi_kw)
         else:
             tropomistr = ''
 
         if key.startswith('tempo.l2'):
+            if tempo_kw['api_key'] == 'your_key_here':
+                raise ValueError('''You must set the tempo_kw api_key
+(e.g., api.tempo_kw["api_key"] = "...") before submitting a query.''')
             tempostr = (
                 '&MAXIMUM_CLOUD_FRACTION={maximum_cloud_fraction}'
                 '&MINIMUM_QUALITY={minimum_quality}&KEY={api_key}'
             ).format(**tempo_kw)
         else:
             tempostr = ''
 
         if key.startswith('purpleair'):
+            if purpleair_kw['api_key'] == 'your_key_here':
+                raise ValueError('''You must set the purpleair_kw api_key
+(e.g., api.purpleair_kw["api_key"] = "9...") before submitting a query.''')
             purpleairstr = (
                 '&OUT_IN_FLAG={out_in_flag}&MAXIMUM_DIFFERENCE='
                 '{maximum_difference}&MAXIMUM_RATIO={maximum_ratio}'
                 '&AGGREGATE={freq}&MINIMUM_AGGREGATION_COUNT_PERCENTAGE='
-                '{agg_pct}&KEY={api_key}'
+                '{agg_pct}&DEFAULT_HUMIDITY={default_humidity}&KEY={api_key}'
             ).format(**purpleair_kw)
         else:
             purpleairstr = ''
 
         if any([key.startswith(pre) for pre in _nocorner_prefixes]):
             cornerstr = ''
         else:
@@ -1388,16 +1047,16 @@
             f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION=1.0.0'
             f'&REQUEST={request}&FORMAT={formatstr}'
             f'&TIME={bdate:%Y-%m-%dT%H:%M:%SZ}/{edate:%Y-%m-%dT%H:%M:%SZ}'
             f'&BBOX={wlon},{slat},{elon},{nlat}'
             f'&COVERAGE={key}'
             f'&COMPRESS={compress}'
         ) + (
-            purpleairstr + viirsnoaastr + tropomistr + tempostr + gridstr
-            + cornerstr + nolonlatsstr
+            purpleairstr + viirsnoaastr + tropomistr + tempostr + pandorastr
+            + calipsostr + gridstr + cornerstr + nolonlatsstr
         )
 
         outpath = (
             f'{self.workdir}/{key}_{bdate:%Y-%m-%dT%H%M%SZ}'
             f'_{edate:%Y-%m-%dT%H%M%SZ}'
         )
 
@@ -1443,15 +1102,15 @@
         if grid_kw.get('REGRID_AGGREGATE', 'None').strip() != 'None':
             gridstr += "&REGRID_AGGREGATE={REGRID_AGGREGATE}"
 
         return gridstr.format(**grid_kw)
 
     def to_dataframe(
         self, key=None, bdate=None, edate=None, bbox=None, unit_keys=True,
-        parse_dates=False, withmeta=False, verbose=0
+        parse_dates=False, withmeta=False, verbose=0, backend='ascii'
     ):
         """
         All arguments default to those provided during initialization.
 
         Arguments
         ---------
         key : str
@@ -1477,20 +1136,26 @@
 
         Returns
         -------
         df : pandas.DataFrame
             Results from download
 
         """
+        from . import xdr
+        assert backend in {'ascii', 'xdr'}
         outpath = self.get_file(
-            'ascii', key=key, bdate=bdate, edate=edate, bbox=bbox,
+            backend, key=key, bdate=bdate, edate=edate, bbox=bbox,
             grid=False, verbose=verbose,
             compress=1
         )
-        df = pd.read_csv(outpath, delimiter='\t', na_values=[-9999., -999])
+        if backend == 'ascii':
+            df = pd.read_csv(outpath, delimiter='\t', na_values=[-9999., -999])
+        else:
+            df = xdr.from_xdrfile(outpath, na_values=[-9999., -999])
+
         if withmeta:
             metapath = self.get_file(
                 'ascii', key=key, bdate=bdate, edate=edate, bbox=bbox,
                 grid=False, verbose=verbose, request='GetMetadata',
                 compress=1
             )
             metatxt = open(metapath, 'r').read()
```

### Comparing `pyrsig-0.7.0/pyrsig/tests/test_api.py` & `pyrsig-0.8.2/pyrsig/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.7.0/pyrsig/tests/test_coards.py` & `pyrsig-0.8.2/pyrsig/tests/test_coards.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.7.0/pyrsig/tests/test_dataframes.py` & `pyrsig-0.8.2/pyrsig/tests/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.7.0/pyrsig/tests/test_gui.py` & `pyrsig-0.8.2/pyrsig/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.7.0/pyrsig/tests/test_ioapi.py` & `pyrsig-0.8.2/pyrsig/tests/test_ioapi.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.7.0/pyrsig.egg-info/PKG-INFO` & `pyrsig-0.8.2/pyrsig.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.7.0
+Version: 0.8.2
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
@@ -105,14 +105,17 @@
 # 3875
 ```
 
 ## Change Log
 
 Not all changes are listed, but notable changes are itemized for ease of review.
 
+* v0.8.2: Added xdr CALIPSO 1.0 format capability.
+* v0.8.1: Added xdr Point 1.0 format capability.
+* v0.8.0: Restructuring module code and adding CMAQ pairing.
 * v0.7.0: Added offline descriptions for review of space/time coverage.
 * v0.7.0: Added TEMPO options for screening
 * v0.6.0: Added latitude longitude grid pass thru support.
 * v0.5.1: Added convenience function for opening many IOAPI files at once.
 * v0.5.1: Updated TEMPO proxy naming.
 * v0.4.6: Added support for legacy TLS servers (e.g, ofmpub and maple)
 * v0.4.5: Updated TEMPO proxy naming
```

### Comparing `pyrsig-0.7.0/setup.py` & `pyrsig-0.8.2/setup.py`

 * *Files identical despite different names*

