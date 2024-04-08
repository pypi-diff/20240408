# Comparing `tmp/satkit-0.2.5.tar.gz` & `tmp/satkit-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satkit-0.2.5.tar", last modified: Sat Mar 23 20:45:05 2024, max compression
+gzip compressed data, was "satkit-0.2.6.tar", last modified: Mon Apr  8 15:30:44 2024, max compression
```

## Comparing `satkit-0.2.5.tar` & `satkit-0.2.6.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.478888 satkit-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-23 20:40:55.000000 satkit-0.2.5/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-23 20:40:55.000000 satkit-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-23 20:40:55.000000 satkit-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-03-23 20:45:05.478888 satkit-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-03-23 20:40:55.000000 satkit-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-23 20:40:55.000000 satkit-0.2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.462888 satkit-0.2.5/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.462888 satkit-0.2.5/python/satkit/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38128 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.462888 satkit-0.2.5/python/satkit/astro-data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/astro-data/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.466888 satkit-0.2.5/python/satkit/density/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/density/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/density/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.466888 satkit-0.2.5/python/satkit/frametransform/
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/frametransform/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/frametransform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.466888 satkit-0.2.5/python/satkit/jplephem/
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/jplephem/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/jplephem/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.466888 satkit-0.2.5/python/satkit/moon/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/moon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/moon/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.466888 satkit-0.2.5/python/satkit/satprop/
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/satprop/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/satprop/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.466888 satkit-0.2.5/python/satkit/sun/
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/sun/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/sun/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.466888 satkit-0.2.5/python/satkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 20:40:55.000000 satkit-0.2.5/python/satkit/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.478888 satkit-0.2.5/python/satkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-03-23 20:45:05.000000 satkit-0.2.5/python/satkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-03-23 20:45:05.000000 satkit-0.2.5/python/satkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 20:45:05.000000 satkit-0.2.5/python/satkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-23 20:45:05.000000 satkit-0.2.5/python/satkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-23 20:45:05.000000 satkit-0.2.5/python/satkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.466888 satkit-0.2.5/python/test/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-23 20:40:55.000000 satkit-0.2.5/python/test/download_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-23 20:40:55.000000 satkit-0.2.5/python/test/download_from_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-23 20:40:55.000000 satkit-0.2.5/python/test/download_testvecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-23 20:40:55.000000 satkit-0.2.5/python/test/orbitprop_gps_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-23 20:40:55.000000 satkit-0.2.5/python/test/sp3file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23703 2024-03-23 20:40:55.000000 satkit-0.2.5/python/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 20:45:05.478888 satkit-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.470888 satkit-0.2.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)    25250 2024-03-23 20:40:55.000000 satkit-0.2.5/src/astrotime.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-23 20:40:55.000000 satkit-0.2.5/src/consts.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-03-23 20:40:55.000000 satkit-0.2.5/src/duration.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-03-23 20:40:55.000000 satkit-0.2.5/src/earth_orientation_params.rs
--rw-r--r--   0 runner    (1001) docker     (127)    22770 2024-03-23 20:40:55.000000 satkit-0.2.5/src/earthgravity.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.470888 satkit-0.2.5/src/frametransform/
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-03-23 20:40:55.000000 satkit-0.2.5/src/frametransform/ierstable.rs
--rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-03-23 20:40:55.000000 satkit-0.2.5/src/frametransform/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-03-23 20:40:55.000000 satkit-0.2.5/src/frametransform/qcirs2gcrs.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21770 2024-03-23 20:40:55.000000 satkit-0.2.5/src/itrfcoord.rs
--rw-r--r--   0 runner    (1001) docker     (127)    25758 2024-03-23 20:40:55.000000 satkit-0.2.5/src/jplephem.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-03-23 20:40:55.000000 satkit-0.2.5/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.470888 satkit-0.2.5/src/lpephem/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-23 20:40:55.000000 satkit-0.2.5/src/lpephem/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-03-23 20:40:55.000000 satkit-0.2.5/src/lpephem/moon.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-03-23 20:40:55.000000 satkit-0.2.5/src/lpephem/sun.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-03-23 20:40:55.000000 satkit-0.2.5/src/nrlmsise.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.474888 satkit-0.2.5/src/ode/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/harmonic_oscillator.rs
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/nalgebra.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rk_adaptive.rs
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rk_adaptive_settings.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rk_explicit.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rkf45.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rkts54.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rkv65.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rkv65_table.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rkv87.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rkv87_table.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rkv98.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rkv98_nointerp.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rkv98_nointerp_table.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/rkv98_table.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-03-23 20:40:55.000000 satkit-0.2.5/src/ode/types.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.474888 satkit-0.2.5/src/orbitprop/
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-03-23 20:40:55.000000 satkit-0.2.5/src/orbitprop/drag.rs
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-23 20:40:55.000000 satkit-0.2.5/src/orbitprop/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-23 20:40:55.000000 satkit-0.2.5/src/orbitprop/point_gravity.rs
--rw-r--r--   0 runner    (1001) docker     (127)    27157 2024-03-23 20:40:55.000000 satkit-0.2.5/src/orbitprop/propagator.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-23 20:40:55.000000 satkit-0.2.5/src/orbitprop/satproperties.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-03-23 20:40:55.000000 satkit-0.2.5/src/orbitprop/satstate.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-23 20:40:55.000000 satkit-0.2.5/src/orbitprop/settings.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.478888 satkit-0.2.5/src/pybindings/
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/mod_utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)    22773 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pyastrotime.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pyconsts.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pydensity.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pyduration.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pyframetransform.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pygravity.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pyitrfcoord.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pyjplephem.rs
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pylpephem_moon.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pylpephem_sun.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pynrlmsise.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pypropagate.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pypropsettings.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pyquaternion.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pysatproperties.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pysatstate.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pysgp4.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pysolarsystem.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pytle.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-23 20:40:55.000000 satkit-0.2.5/src/pybindings/pyutils.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.478888 satkit-0.2.5/src/sgp4/
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-03-23 20:40:55.000000 satkit-0.2.5/src/sgp4/dpper.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-03-23 20:40:55.000000 satkit-0.2.5/src/sgp4/dscom.rs
--rw-r--r--   0 runner    (1001) docker     (127)    12980 2024-03-23 20:40:55.000000 satkit-0.2.5/src/sgp4/dsinit.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-03-23 20:40:55.000000 satkit-0.2.5/src/sgp4/dspace.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-23 20:40:55.000000 satkit-0.2.5/src/sgp4/getgravconst.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-03-23 20:40:55.000000 satkit-0.2.5/src/sgp4/initl.rs
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-23 20:40:55.000000 satkit-0.2.5/src/sgp4/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-03-23 20:40:55.000000 satkit-0.2.5/src/sgp4/satrec.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-03-23 20:40:55.000000 satkit-0.2.5/src/sgp4/sgp4.rs
--rw-r--r--   0 runner    (1001) docker     (127)    15524 2024-03-23 20:40:55.000000 satkit-0.2.5/src/sgp4/sgp4_lowlevel.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21970 2024-03-23 20:40:55.000000 satkit-0.2.5/src/sgp4/sgp4init.rs
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-23 20:40:55.000000 satkit-0.2.5/src/solarsystem.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-03-23 20:40:55.000000 satkit-0.2.5/src/spaceweather.rs
--rw-r--r--   0 runner    (1001) docker     (127)    15457 2024-03-23 20:40:55.000000 satkit-0.2.5/src/tle.rs
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-23 20:40:55.000000 satkit-0.2.5/src/types.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:45:05.478888 satkit-0.2.5/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-23 20:40:55.000000 satkit-0.2.5/src/utils/datadir.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-23 20:40:55.000000 satkit-0.2.5/src/utils/download.rs
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-23 20:40:55.000000 satkit-0.2.5/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-23 20:40:55.000000 satkit-0.2.5/src/utils/skerror.rs
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-23 20:40:55.000000 satkit-0.2.5/src/utils/test.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-03-23 20:40:55.000000 satkit-0.2.5/src/utils/update_data.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.536245 satkit-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-08 15:26:42.000000 satkit-0.2.6/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 15:26:42.000000 satkit-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-08 15:26:42.000000 satkit-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-08 15:30:44.536245 satkit-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-08 15:26:42.000000 satkit-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-08 15:26:42.000000 satkit-0.2.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.512245 satkit-0.2.6/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.516245 satkit-0.2.6/python/satkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38208 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.516245 satkit-0.2.6/python/satkit/astro-data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/astro-data/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.516245 satkit-0.2.6/python/satkit/density/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/density/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/density/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.516245 satkit-0.2.6/python/satkit/frametransform/
+-rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/frametransform/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/frametransform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.516245 satkit-0.2.6/python/satkit/jplephem/
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/jplephem/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/jplephem/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.516245 satkit-0.2.6/python/satkit/moon/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/moon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/moon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.516245 satkit-0.2.6/python/satkit/satprop/
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/satprop/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/satprop/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.516245 satkit-0.2.6/python/satkit/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/sun/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/sun/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.516245 satkit-0.2.6/python/satkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:26:42.000000 satkit-0.2.6/python/satkit/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.536245 satkit-0.2.6/python/satkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-08 15:30:44.000000 satkit-0.2.6/python/satkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-08 15:30:44.000000 satkit-0.2.6/python/satkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:30:44.000000 satkit-0.2.6/python/satkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 15:30:44.000000 satkit-0.2.6/python/satkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 15:30:44.000000 satkit-0.2.6/python/satkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.520245 satkit-0.2.6/python/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-08 15:26:42.000000 satkit-0.2.6/python/test/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 15:26:42.000000 satkit-0.2.6/python/test/download_from_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-08 15:26:42.000000 satkit-0.2.6/python/test/download_testvecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-08 15:26:42.000000 satkit-0.2.6/python/test/orbitprop_gps_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-08 15:26:42.000000 satkit-0.2.6/python/test/sp3file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25177 2024-04-08 15:26:42.000000 satkit-0.2.6/python/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:30:44.536245 satkit-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.520245 satkit-0.2.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    25250 2024-04-08 15:26:42.000000 satkit-0.2.6/src/astrotime.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-08 15:26:42.000000 satkit-0.2.6/src/consts.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-08 15:26:42.000000 satkit-0.2.6/src/duration.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-08 15:26:42.000000 satkit-0.2.6/src/earth_orientation_params.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    22770 2024-04-08 15:26:42.000000 satkit-0.2.6/src/earthgravity.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.520245 satkit-0.2.6/src/frametransform/
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-08 15:26:42.000000 satkit-0.2.6/src/frametransform/ierstable.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-04-08 15:26:42.000000 satkit-0.2.6/src/frametransform/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-08 15:26:42.000000 satkit-0.2.6/src/frametransform/qcirs2gcrs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21770 2024-04-08 15:26:42.000000 satkit-0.2.6/src/itrfcoord.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    25758 2024-04-08 15:26:42.000000 satkit-0.2.6/src/jplephem.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-08 15:26:42.000000 satkit-0.2.6/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.524245 satkit-0.2.6/src/lpephem/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 15:26:42.000000 satkit-0.2.6/src/lpephem/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-08 15:26:42.000000 satkit-0.2.6/src/lpephem/moon.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-08 15:26:42.000000 satkit-0.2.6/src/lpephem/sun.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-08 15:26:42.000000 satkit-0.2.6/src/nrlmsise.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.524245 satkit-0.2.6/src/ode/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/harmonic_oscillator.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/nalgebra.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rk_adaptive.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rk_adaptive_settings.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rk_explicit.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rkf45.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rkts54.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rkv65.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rkv65_table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rkv87.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rkv87_table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rkv98.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rkv98_nointerp.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rkv98_nointerp_table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/rkv98_table.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-08 15:26:42.000000 satkit-0.2.6/src/ode/types.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.528245 satkit-0.2.6/src/orbitprop/
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-08 15:26:42.000000 satkit-0.2.6/src/orbitprop/drag.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-08 15:26:42.000000 satkit-0.2.6/src/orbitprop/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-08 15:26:42.000000 satkit-0.2.6/src/orbitprop/point_gravity.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    27157 2024-04-08 15:26:42.000000 satkit-0.2.6/src/orbitprop/propagator.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-08 15:26:42.000000 satkit-0.2.6/src/orbitprop/satproperties.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-08 15:26:42.000000 satkit-0.2.6/src/orbitprop/satstate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-08 15:26:42.000000 satkit-0.2.6/src/orbitprop/settings.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.532245 satkit-0.2.6/src/pybindings/
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/mod_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    23930 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pyastrotime.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pyconsts.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pydensity.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pyduration.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pyframetransform.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pygravity.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pyitrfcoord.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pyjplephem.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pylpephem_moon.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pylpephem_sun.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pynrlmsise.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pypropagate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pypropsettings.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pyquaternion.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pysatproperties.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pysatstate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pysgp4.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pysolarsystem.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pytle.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-04-08 15:26:42.000000 satkit-0.2.6/src/pybindings/pyutils.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.532245 satkit-0.2.6/src/sgp4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-04-08 15:26:42.000000 satkit-0.2.6/src/sgp4/dpper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-08 15:26:42.000000 satkit-0.2.6/src/sgp4/dscom.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    12980 2024-04-08 15:26:42.000000 satkit-0.2.6/src/sgp4/dsinit.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-08 15:26:42.000000 satkit-0.2.6/src/sgp4/dspace.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-08 15:26:42.000000 satkit-0.2.6/src/sgp4/getgravconst.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-08 15:26:42.000000 satkit-0.2.6/src/sgp4/initl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-08 15:26:42.000000 satkit-0.2.6/src/sgp4/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-08 15:26:42.000000 satkit-0.2.6/src/sgp4/satrec.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-04-08 15:26:42.000000 satkit-0.2.6/src/sgp4/sgp4.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    15524 2024-04-08 15:26:42.000000 satkit-0.2.6/src/sgp4/sgp4_lowlevel.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21970 2024-04-08 15:26:42.000000 satkit-0.2.6/src/sgp4/sgp4init.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-08 15:26:42.000000 satkit-0.2.6/src/solarsystem.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-08 15:26:42.000000 satkit-0.2.6/src/spaceweather.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    15457 2024-04-08 15:26:42.000000 satkit-0.2.6/src/tle.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 15:26:42.000000 satkit-0.2.6/src/types.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:30:44.532245 satkit-0.2.6/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-08 15:26:42.000000 satkit-0.2.6/src/utils/datadir.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-08 15:26:42.000000 satkit-0.2.6/src/utils/download.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-08 15:26:42.000000 satkit-0.2.6/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-08 15:26:42.000000 satkit-0.2.6/src/utils/skerror.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-08 15:26:42.000000 satkit-0.2.6/src/utils/test.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-08 15:26:42.000000 satkit-0.2.6/src/utils/update_data.rs
```

### Comparing `satkit-0.2.5/Cargo.toml` & `satkit-0.2.6/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "satkit"
-version = "0.2.5"
+version = "0.2.6"
 edition = "2021"
 description = "Satellite Toolkit"
 readme = "README.md"
 licence = "MIT"
 license-file = "LICENSE"
 homepage = "https://github.com/ssmichael1/satkit"
 repository = "https://github.com/ssmichael1/satkit"
```

### Comparing `satkit-0.2.5/LICENSE` & `satkit-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/PKG-INFO` & `satkit-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satkit
-Version: 0.2.5
+Version: 0.2.6
 Summary: Satellite Orbital Dynamics Toolkit
 Author-email: Steven Michael <ssmichael@gmail.com>
 Maintainer-email: Steven Michael <ssmichael@gmail.com>
 Keywords: satellite,orbit,astrodynamics,SGP4,TLE,JPL,Ephemeris
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `satkit-0.2.5/README.md` & `satkit-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/pyproject.toml` & `satkit-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-rust"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "satkit"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = ["numpy>=1.20.0"]
 requires-python = ">= 3.8"
 authors = [{ name = "Steven Michael", email = "ssmichael@gmail.com" }]
 maintainers = [{ name = "Steven Michael", email = "ssmichael@gmail.com" }]
 readme = "README.md"
 description = "Satellite Orbital Dynamics Toolkit"
 keywords = [
@@ -39,64 +39,64 @@
 ]
 
 [tool.setuptools.packages]
 find = { where = ["python"] }
 
 [tool.cibuildwheel]
 build = ["cp312-*", "cp311-* cp310-* cp39-* cp38-*"]
+test-skip = "*-macosx_arm64 *-macosx_universal2:arm64"
+skip = ["pp*", "*_i686", "*_s390x", "*_aarch64", "*_ppc64le", "*-musllinux*"]
+
 
 [tool.cibuildwheel.macos]
 archs = ["x86_64", "arm64"]
 before-build = [
     "pip install -U setuptools-rust",
     "rustup default stable",
     "rustup target add aarch64-apple-darwin",
     "rustup show",
 ]
 environment = { PATH = "$PATH:$HOME/.cargo/bin" }
 # Skip trying to test arm64 builds on Intel Macs
-test-skip = "*-macosx_arm64 *-macosx_universal2:arm64"
 test-requires = "pytest"
 test-command = [
-    "ASTRO_DATA={package}/astro-data SATKIT_TESTVEC_ROOT={package}/satkit-testvecs pytest {project}/python/test/test.py",
+    "SATKIT_DATA={package}/astro-data SATKIT_TESTVEC_ROOT={package}/satkit-testvecs pytest {project}/python/test/test.py",
 ]
 
 
 [tool.cibuildwheel.linux]
 environment = { PATH = "$PATH:$HOME/.cargo/bin" }
 archs = ["x86_64"]
-skip = ["pp*", "*_i686", "*_s390x", "*_aarch64", "*_ppc64le", "*-musllinux*"]
 before-build = [
     "pip install -U setuptools-rust",
     "curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain=stable --profile=minimal -y",
     "rustup show",
 ]
 test-requires = "pytest"
 test-command = [
-    "ASTRO_DATA={package}/astro-data SATKIT_TESTVEC_ROOT={package}/satkit-testvecs pytest {project}/python/test/test.py",
+    "SATKIT_DATA={package}/astro-data SATKIT_TESTVEC_ROOT={package}/satkit-testvecs pytest {project}/python/test/test.py",
 ]
 
 [tool.cibuildwheel.windows]
 environment = { PATH = '$UserProfile\.cargo\bin;$PATH' }
 before-build = [
     "pip install -U setuptools-rust",
     "rustup toolchain install stable-x86_64-pc-windows-msvc",
     "rustup default stable-x86_64-pc-windows-msvc",
     "rustup override set stable-x86_64-pc-windows-msvc",
     "rustup show",
 ]
 archs = ["AMD64"]
-skip = ["pp*"]
 test-requires = "pytest"
 before-test = [
-    "set ASTRO_DATA={package}\\astro-data",
+    "set SATKIT_DATA={package}\\astro-data",
     "set SATKIT_TESTVEC_ROOT={package}\\satkit-testvecs",
 ]
 test-command = [
-    "set ASTRO_DATA={package}\\astro-data&&set SATKIT_TESTVEC_ROOT={package}\\satkit-testvecs&&pytest {project}\\python\\test\\test.py",
+    "set SATKIT_DATA={package}\\astro-data&&set SATKIT_TESTVEC_ROOT={package}\\satkit-testvecs&&pytest {project}\\python\\test\\test.py",
 ]
 
 
 [[tool.setuptools-rust.ext-modules]]
 features = ["pybindings"]
 args = ["--crate-type", "cdylib"]
 target = "satkit/satkit"
```

### Comparing `satkit-0.2.5/python/satkit/__init__.pyi` & `satkit-0.2.6/python/satkit/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -533,16 +533,16 @@
     Specify time scale used to represent or convert between the "satkit.time"
     representation of time
 
     Most of the time, these are not needed directly, but various time scales
     are needed to compute precise rotations between various inertial and
     Earth-fixed coordinate frames
 
-    For details, see:
-    https://stjarnhimlen.se/comp/time.html
+    For an excellent overview, see:
+    https://spsweb.fltops.jpl.nasa.gov/portaldataops/mpg/MPG_Docs/MPG%20Book/Release/Chapter2-TimeScales.pdf
 
     # Options:
 
     * Invalid: Invalid time scale
     * UTC: Universal Time Coordinate
     * TT: Terrestrial Time
     * UT1: UT1
```

### Comparing `satkit-0.2.5/python/satkit/density/__init__.pyi` & `satkit-0.2.6/python/satkit/density/__init__.pyi`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/python/satkit/frametransform/__init__.pyi` & `satkit-0.2.6/python/satkit/frametransform/__init__.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -15,102 +15,147 @@
 import numpy.typing as npt
 import numpy as np
 
 import satkit
 import datetime
 
 def gmst(
-    tm: satkit.time | npt.ArrayLike[satkit.time],
+    tm: satkit.time | npt.ArrayLike[satkit.time] | datetime.datetime | npt.ArrayLike[datetime.datetime],
 ) -> float | npt.ArrayLike[np.float]:
     """
     Greenwich Mean Sidereal Time
-
+    
     Vallado algorithm 15:
-
-    GMST = 67310.5481 + (876600h + 8640184.812866) * tᵤₜ₁ * (0.983104 + tᵤₜ₁ * -6.2e-6)
-
-    Input is satkit.time object or list or numpy array of satkit.time objects.
-
-    Output is float or numpy array of floats with GMST in radians matched element-wise
-    to the input times.
+    
+    GMST = 67310.5481 + (876600h + 8640184.812866) * tᵤₜ₁ * (0.983104 + tᵤₜ₁ * −6.2e−6)
+    
+    
+    # Arguments
+    
+      * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+              representing time at which to calculate output
+    
+    # Returns
+    
+    * Greenwich Mean Sideral Time, radians, at intput time(s)
+    
     """
 
 def gast(
-    tm: satkit.time | npt.ArrayLike[satkit.time],
+    tm: satkit.time | npt.ArrayLike[satkit.time] | datetime.datetime | npt.ArrayLike[datetime.datetime],
 ) -> float | npt.ArrayLike[np.float]:
     """
-    Greenwich Apparent Sidereal Time
-
-    Input is satkit.time object or list or numpy array of satkit.time objects.
-
-    Output is float or numpy array of floats with GAST in radians matched element-wise
-    to the input times.
+    Greenwich apparant sidereal time, radians
+    
+    # Arguments:
+    
+      * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+              representing time at which to calculate output
+    
+    # Returns:
+    
+     * Greenwich apparant sidereal time, radians, at input time(s)
+    
     """
 
 def earth_rotation_angle(
-    tm: satkit.time | npt.ArrayLike[satkit.time],
+    tm: satkit.time | npt.ArrayLike[satkit.time] | datetime.datetime | npt.ArrayLike[datetime.datetime],
 ) -> float | npt.ArrayLike[np.float]:
     """
-    Earth rotation angle
-
-    See:
-    https://www.iers.org/SharedDocs/Publikationen/EN/IERS/Publications/tn/TechnNote36/tn36_043.pdf?__blob=publicationFile&v=1
-
+    Earth Rotation Angle
+    
+    See
+    [IERS Technical Note 36, Chapter 5](https://www.iers.org/SharedDocs/Publikationen/EN/IERS/Publications/tn/TechnNote36/tn36_043.pdf?__blob=publicationFile&v=1)
     Equation 5.15
-
-    Input is satkit.time object or list or numpy array of satkit.time objects.
-
-    Output is float or numpy array of floats with Earth Rotation Angle in radians
-    matched element-wise to the input times.
+    
+    # Arguments:
+    
+     * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+             representing time at which to calculate output
+    
+    # Returns:
+    
+     * Earth rotation angle, in radians, at input time(s)
+    
+    # Calculation Details
+    
+    * Let t be UT1 Julian date
+    * let f be fractional component of t (fraction of day)
+    * ERA = 2𝜋 ((0.7790572732640 + f + 0.00273781191135448 * (t − 2451545.0))
+    
     """
 
 def qitrf2tirs(
-    tm: satkit.time | npt.ArrayLike[satkit.time],
+    tm: satkit.time | npt.ArrayLike[satkit.time] | datetime.datetime | npt.ArrayLike[datetime.datetime],
 ) -> satkit.quaternion | npt.ArrayLike[satkit.quaternion]:
     """
-    Rotation from International Terrestrial Reference Frame
-    (ITRF) to the Terrestrial Intermediate Reference System (TIRS)
-    represented as satkit.quaterinion object
-
-    Input is satkit.time object or list or numpy array of satkit.time objects.
-
-    Output is satkit.quaternion or numpy array of satkit.quaternion representiong
-    rotations from itrf to tirs matched element-wise to the input times
+    Rotation from Terrestrial Intermediate Reference System to
+    Celestial Intermediate Reference Systems
+    
+    # Arguments:
+    
+     * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+             representing time at which to calculate output
+    
+    # Returns:
+    
+     * Quaternion representing rotation from TIRS to CIRS at input time(s)
+    
     """
 
 @typing.overload
-def qcirs2gcrf(tm: satkit.time) -> satkit.quaternion:
-    """
-    Rotate from Celestial Intermediate Reference System
+def qcirs2gcrf(tm: satkit.time | datetime.datetime) -> satkit.quaternion:
+    """  
+    Rotation from Celestial Intermediate Reference System
     to Geocentric Celestial Reference Frame
+    
+    # Arguments:
+    
+     * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+             representing time at which to calculate output
+    
+    # Returns:
+    
+     * Quaternion representing rotation from CIRS to GCRF at input time(s)
+    
     """
 
 @typing.overload
-def qcirs2gcrf(tm: npt.ArrayLike[satkit.time]) -> npt.ArrayLike[satkit.quaternion]:
+def qcirs2gcrf(tm: npt.ArrayLike[satkit.time] | npt.ArrayLike[datetime.datetime]) -> npt.ArrayLike[satkit.quaternion]:
     """
-    Rotate from Celestial Intermediate Reference System
+    Rotation from Celestial Intermediate Reference System
     to Geocentric Celestial Reference Frame
+    
+    # Arguments:
+    
+     * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+             representing time at which to calculate output
+    
+    # Returns:
+    
+     * Quaternion representing rotation from CIRS to GCRF at input time(s)
+    
     """
 
 def qtirs2cirs(
-    tm: satkit.time | npt.ArrayLike[satkit.time],
+    tm: satkit.time | npt.ArrayLike[satkit.time] | datetime.datetime | npt.ArrayLike[datetime.datetime],
 ) -> satkit.quaternion | npt.ArrayLike[satkit.quaternion]:
     """
     Rotation from Terrestrial Intermediate Reference System (TIRS)
     to the Celestial Intermediate Reference System (CIRS)
 
 
     Input is satkit.time object or list or numpy array of satkit.time objects.
 
     Output is satkit.quaternion or numpy array of satkit.quaternion representiong
     rotations from itrf to tirs matched element-wise to the input times
     """
 
 def qgcrf2itrf_approx(
-    tm: satkit.time | npt.ArrayLike[satkit.time],
+    tm: satkit.time | npt.ArrayLike[satkit.time] | datetime.datetime | npt.ArrayLike[datetime.datetime],
 ) -> satkit.quaternion | npt.ArrayLike[satkit.quaternion]:
     """
     Quaternion representing approximate rotation from the
     Geocentric Celestial Reference Frame (GCRF)
     to the International Terrestrial Reference Frame (ITRF)
 
     # Notes:
@@ -124,15 +169,15 @@
     # Outputs:
 
         * satkit.quaternion or numpy array of satkit.quaternion representiong
         rotations from gcrf to itrf matched element-wise to the input times
     """
 
 def qitrf2gcrf_approx(
-    tm: satkit.time | npt.ArrayLike[satkit.time],
+    tm: satkit.time | npt.ArrayLike[satkit.time] | datetime.datetime | npt.ArrayLike[datetime.datetime],
 ) -> satkit.quaternion | npt.ArrayLike[satkit.quaternion]:
     """
     Quaternion representing approximate rotation from the
     International Terrestrial Reference Frame (ITRF)
     to the Geocentric Celestial Reference Frame (GCRF)
 
     # Notes:
@@ -171,15 +216,15 @@
     # Outputs:
 
         * satkit.quaternion or numpy array of satkit.quaternion representiong
         rotations from gcrf to itrf matched element-wise to the input times
     """
 
 def qitrf2gcrf(
-    tm: satkit.time | npt.ArrayLike[satkit.time],
+    tm: satkit.time | npt.ArrayLike[satkit.time] | datetime.datetime | npt.ArrayLike[datetime.datetime],
 ) -> satkit.quaternion | npt.ArrayLike[satkit.quaternion]:
     """
     Quaternion representing rotation from the
     International Terrestrial Reference Frame (ITRF)
     to the Geocentric Celestial Reference Frame (GCRF)
 
     Uses full IAU2006 Reduction
@@ -196,15 +241,15 @@
     # Outputs:
 
         * satkit.quaternion or numpy array of satkit.quaternion representiong
         rotations from itrf to gcrf matched element-wise to the input times
     """
 
 def qteme2itrf(
-    tm: satkit.time | npt.ArrayLike[satkit.time],
+    tm: satkit.time | npt.ArrayLike[satkit.time] | datetime.datetime | npt.ArrayLike[datetime.datetime],
 ) -> satkit.quaternion | npt.ArrayLike[satkit.quaternion]:
     """
     Quaternion representing rotation from the
     True Equator Mean Equinox (TEME) frame
     to the International Terrestrial Reference Frame (ITRF)
 
     This is equation 3-90 in Vallado
```

### Comparing `satkit-0.2.5/python/satkit/jplephem/__init__.pyi` & `satkit-0.2.6/python/satkit/jplephem/__init__.pyi`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/python/satkit/moon/__init__.py` & `satkit-0.2.6/python/satkit/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/python/satkit/satprop/__init__.pyi` & `satkit-0.2.6/python/satkit/satprop/__init__.pyi`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/python/satkit/sun/__init__.pyi` & `satkit-0.2.6/python/satkit/sun/__init__.pyi`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/python/satkit/utils/__init__.pyi` & `satkit-0.2.6/python/satkit/utils/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     JPL Ephemeris, etc..
 
     Data directory is 1st of following directories search that contains
     the data files listed in "update_datafiles"
 
     MacOS:
 
-    1. Directory pointed to by "ASTRO_DATA" environment variable
+    1. Directory pointed to by "SATKIT_DATA" environment variable
     2. $HOME/LIBRARY/Application\ Support/astro-data
     3. $HOME/.astro-data
     4. $HOME
     5. /usr/share/astro-data
     6. /Library/Application\ Support/astro-data
 
     Linux:
```

### Comparing `satkit-0.2.5/python/satkit.egg-info/PKG-INFO` & `satkit-0.2.6/python/satkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satkit
-Version: 0.2.5
+Version: 0.2.6
 Summary: Satellite Orbital Dynamics Toolkit
 Author-email: Steven Michael <ssmichael@gmail.com>
 Maintainer-email: Steven Michael <ssmichael@gmail.com>
 Keywords: satellite,orbit,astrodynamics,SGP4,TLE,JPL,Ephemeris
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `satkit-0.2.5/python/satkit.egg-info/SOURCES.txt` & `satkit-0.2.6/python/satkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/python/test/download_data.py` & `satkit-0.2.6/python/test/download_data.py`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/python/test/download_from_json.py` & `satkit-0.2.6/python/test/download_from_json.py`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/python/test/download_testvecs.py` & `satkit-0.2.6/python/test/download_testvecs.py`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/python/test/orbitprop_gps_fit.py` & `satkit-0.2.6/python/test/orbitprop_gps_fit.py`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/python/test/sp3file.py` & `satkit-0.2.6/python/test/sp3file.py`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/python/test/test.py` & `satkit-0.2.6/python/test/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,58 @@
 # %%
 import satkit as sk
 import pytest
 import numpy as np
 import math as m
 import os
 from sp3file import read_sp3file
-
+from datetime import datetime, timezone
 
 testvec_dir = os.getenv(
             "SATKIT_TESTVEC_ROOT", default="." + os.path.sep + "satkit-testvecs" + os.path.sep
         )
 
+class TestDateTime:
+    """
+    Check that function calls with satkit.time and datetime.datetime return 
+    the same result
+    """
+    def test_scalar_times(self):
+
+        # Create times and show that they are equal
+        tm1 = sk.time(2023, 3, 4, 12, 5, 6)
+        tm2 = datetime(2023, 3, 4, 12, 5, 6, tzinfo=timezone.utc)
+
+
+        assert(tm1.datetime() == tm2)
+        # Check that function calls work
+        # Pick gmst as the test function call for time
+        # it can be anything since under the hood the same function call is used
+        # to get time inputs for all python functions in package
+        g1 = sk.frametransform.gmst(tm1)
+        g2 = sk.frametransform.gmst(tm2)
+        assert g1 == pytest.approx(g2, rel=1e-10)
+
+    def test_list_times(self):
+        timearr = range(10)
+        tm1 = [sk.time(2023, 3, x+1, 12, 0, 0) for x in timearr]
+        tm2 = [datetime(2023, 3, x+1, 12, 0, 0, tzinfo=timezone.utc) for x in timearr]
+        g1 = sk.frametransform.gmst(tm1)
+        g2 = sk.frametransform.gmst(tm2)
+        assert g1 == pytest.approx(g2)
+
+    def test_numpy_times(self):
+        timearr = range(10)
+        tm1 = np.array([sk.time(2023, 3, x+1, 12, 0, 0) for x in timearr])
+        tm2 = np.array([datetime(2023, 3, x+1, 12, 0, 0, tzinfo=timezone.utc) for x in timearr])
+        g1 = sk.frametransform.gmst(tm1)
+        g2 = sk.frametransform.gmst(tm2)
+        assert g1 == pytest.approx(g2)   
+
+
 class TestTime:
     def test_mjd(self):
         """
         Test MJD conversion
         """
         t = sk.time(2021, 1, 1, 0, 0, 0)
         mjd = t.to_mjd(sk.timescale.UTC)
```

### Comparing `satkit-0.2.5/src/astrotime.rs` & `satkit-0.2.6/src/astrotime.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/consts.rs` & `satkit-0.2.6/src/consts.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #[allow(non_upper_case_globals)]
-///  WGS-84 semiparameter, in meters */
+///  WGS-84 semiparameter, in meters
 pub const WGS84_A: f64 = 6378137.0;
-///  WGS-84 flattening */
+///  WGS-84 flattening
 pub const WGS84_F: f64 = 0.003352810664747;
 /// WGS-84 Earth radius, meters
 pub const EARTH_RADIUS: f64 = WGS84_A;
-///  Gravitational parameter of Earth, m^3/s^2 */
+///  Gravitational parameter of Earth, m^3/s^2
 pub const MU_EARTH: f64 = 3.986004418E14;
-///  Gravitational parameter of Moon, m^3/s^2 */
+///  Gravitational parameter of Moon, m^3/s^2
 pub const MU_MOON: f64 = 4.9048695E12;
-///  Gravitational parameter of Sun, m^3/s^2 */
+///  Gravitational parameter of Sun, m^3/s^2
 pub const MU_SUN: f64 = 1.32712440018E20;
-///  Alternate name for gravitational parameter */
+///  Alternate name for gravitational parameter
 pub const GM: f64 = MU_EARTH;
-///  Earth rotation rate, radians / second */
+///  Earth rotation rate, radians / second
 pub const OMEGA_EARTH: f64 = 7.292115090E-5;
-///  speed of light, m/s */
+///  speed of light, m/s
 pub const C: f64 = 299792458.0;
-///  Astronomical unit, meters */
+///  Astronomical unit, meters
 pub const AU: f64 = 1.4959787069999998807907104492E11;
-///  Sun radius in meters */
+///  Sun radius in meters
 pub const SUN_RADIUS: f64 = 695500000.0;
-///  Moon radius, meters */
+///  Moon radius, meters
 pub const MOON_RADIUS: f64 = 1737400.0;
-///  Ratio of earth mass to moon mass */
+///  Ratio of earth mass to moon mass
 pub const EARTH_MOON_MASS_RATIO: f64 = 81.30056822149721540427;
-///  Geosynchronous Distance */
+///  Geosynchronous Distance
 pub const GEO_R: f64 = 42164172.58422766;
-///  JGM3 Gravitational parameter of Earth, m^3/s^2 */
+///  JGM3 Gravitational parameter of Earth, m^3/s^2
 pub const JGM3_MU: f64 = 0.3986004415E+15;
-///  JGM3 Semimajor axis of Earth, m */
+///  JGM3 Semimajor axis of Earth, m
 pub const JGM3_A: f64 = 0.6378136300E+07;
-///  JGM3 J2 term */
+///  JGM3 J2 term
 pub const JGM3_J2: f64 = -0.0010826360229829945;
 //jgm3_J2:f64 = -sqrt(5.) * -0.484169548456e-03;
```

### Comparing `satkit-0.2.5/src/duration.rs` & `satkit-0.2.6/src/duration.rs`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,17 @@
             sign = String::from("-");
             secs = -1.0 * secs;
         }
         // add 5e-4 seconds so that display will round correctly,
         // e.g. if seconds = 59.999..., rather than round up and
         // display "seconds" in second field, show 0 and increment
         // minutes...
-        secs = secs + 5.0e-4;
+        if secs % 60.0  > 59.9995 {
+            secs = secs + 5.0e-4;
+        }
 
         if secs < 1.0 {
             format!("Duration: {}{:.3} microseconds", sign, (secs % 1.0) * 1.0e6)
         } else {
             let days = (secs / 86400.0) as usize;
             let hours = ((secs % 86400.0) / 3600.0) as usize;
             let minutes = ((secs % 3600.0) / 60.0) as usize;
```

### Comparing `satkit-0.2.5/src/earth_orientation_params.rs` & `satkit-0.2.6/src/earth_orientation_params.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/earthgravity.rs` & `satkit-0.2.6/src/earthgravity.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/frametransform/ierstable.rs` & `satkit-0.2.6/src/frametransform/ierstable.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/frametransform/mod.rs` & `satkit-0.2.6/src/frametransform/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         + tut1 * ((876600.0 * 3600.0 + 8640184.812866) + tut1 * (0.093104 + tut1 * -6.2e-6));
 
     gmst = (gmst % 86400.0) / 240.0 * PI / 180.0;
     return gmst;
 }
 
 /// Equation of Equinoxes
+/// Equation of the equinoxes
 pub fn eqeq(tm: &AstroTime) -> f64 {
     let d: f64 = tm.to_mjd(Scale::TT) - 51544.5;
     let omega = PI / 180.0 * (125.04 - 0.052954 * d);
     let l = (280.47 + 0.98565 * d) * PI / 180.0;
     let epsilon = (23.4393 - 0.0000004 * d) * PI / 180.0;
     let d_psi = (-0.000319 * f64::sin(omega) - 0.000024 * f64::sin(2.0 * l)) * 15.0 * PI / 180.0;
     d_psi * f64::cos(epsilon)
```

### Comparing `satkit-0.2.5/src/frametransform/qcirs2gcrs.rs` & `satkit-0.2.6/src/frametransform/qcirs2gcrs.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/itrfcoord.rs` & `satkit-0.2.6/src/itrfcoord.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/jplephem.rs` & `satkit-0.2.6/src/jplephem.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/lib.rs` & `satkit-0.2.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/lpephem/moon.rs` & `satkit-0.2.6/src/lpephem/moon.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/lpephem/sun.rs` & `satkit-0.2.6/src/lpephem/sun.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/nrlmsise.rs` & `satkit-0.2.6/src/nrlmsise.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/mod.rs` & `satkit-0.2.6/src/ode/mod.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/nalgebra.rs` & `satkit-0.2.6/src/ode/nalgebra.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rk_adaptive.rs` & `satkit-0.2.6/src/ode/rk_adaptive.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rk_adaptive_settings.rs` & `satkit-0.2.6/src/ode/rk_adaptive_settings.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rk_explicit.rs` & `satkit-0.2.6/src/ode/rk_explicit.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rkf45.rs` & `satkit-0.2.6/src/ode/rkf45.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rkts54.rs` & `satkit-0.2.6/src/ode/rkts54.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rkv65.rs` & `satkit-0.2.6/src/ode/rkv65.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rkv65_table.rs` & `satkit-0.2.6/src/ode/rkv65_table.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rkv87.rs` & `satkit-0.2.6/src/ode/rkv87.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rkv87_table.rs` & `satkit-0.2.6/src/ode/rkv87_table.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rkv98.rs` & `satkit-0.2.6/src/ode/rkv98.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rkv98_nointerp.rs` & `satkit-0.2.6/src/ode/rkv98_nointerp.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rkv98_nointerp_table.rs` & `satkit-0.2.6/src/ode/rkv98_nointerp_table.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/rkv98_table.rs` & `satkit-0.2.6/src/ode/rkv98_table.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/ode/types.rs` & `satkit-0.2.6/src/ode/types.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/orbitprop/drag.rs` & `satkit-0.2.6/src/orbitprop/drag.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/orbitprop/point_gravity.rs` & `satkit-0.2.6/src/orbitprop/point_gravity.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/orbitprop/propagator.rs` & `satkit-0.2.6/src/orbitprop/propagator.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/orbitprop/satproperties.rs` & `satkit-0.2.6/src/orbitprop/satproperties.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/orbitprop/satstate.rs` & `satkit-0.2.6/src/orbitprop/satstate.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/orbitprop/settings.rs` & `satkit-0.2.6/src/orbitprop/settings.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/mod.rs` & `satkit-0.2.6/src/pybindings/mod.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/mod_utils.rs` & `satkit-0.2.6/src/pybindings/mod_utils.rs`

 * *Files 17% similar despite different names*

```diff
@@ -50,19 +50,30 @@
 
     match crate::utils::update_datafiles(datadir, overwrite_files) {
         Err(e) => Err(pyo3::exceptions::PyRuntimeError::new_err(e.to_string())),
         Ok(_) => Ok(()),
     }
 }
 
-/// Return directory currently used to hold
-/// necessary data files for the directory
+/// Get directory where astronomy data is stored
 ///
-/// e.g., Earth Orientation Parameters, gravity coefficients,
-/// JPL Ephemeris, etc..
+/// Tries the following paths in order, and stops when the
+/// files are found
+///
+/// *  "SATKIT_DATA" environment variable
+/// *  ${HOME}/astro-data
+/// *  ${HOME}
+/// *  /usr/share/astro-data
+/// *  On Mac Only:
+///    * /Library/Application Support/astro-data
+///    * ${Home}/Library/Application Support/astro-data
+///
+/// Returns:
+///
+///  * string representing directory where files are stored
 ///
 #[pyfunction]
 fn datadir() -> PyResult<PyObject> {
     pyo3::Python::with_gil(|py| -> PyResult<PyObject> {
         match crate::utils::datadir() {
             Ok(v) => Ok(v.to_str().unwrap().to_object(py)),
             Err(_) => Ok(pyo3::types::PyNone::get(py).into_py(py)),
@@ -72,14 +83,21 @@
 
 /// Git hash of compiled library
 #[pyfunction]
 fn githash() -> PyResult<String> {
     Ok(String::from(crate::utils::githash()))
 }
 
+// Version of satkit
+#[pyfunction]
+fn version() -> PyResult<String> {
+    Ok(String::from(crate::utils::gittag()))
+}
+
+
 #[pyfunction]
 fn dylib_path() -> PyResult<PyObject> {
     pyo3::Python::with_gil(|py| -> PyResult<PyObject> {
         match process_path::get_dylib_path() {
             Some(v) => Ok(v.to_str().unwrap().to_object(py)),
             None => Ok(pyo3::types::PyNone::get(py).into_py(py)),
         }
@@ -96,10 +114,11 @@
 #[pymodule]
 pub fn utils(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(datadir, m)?).unwrap();
     m.add_function(wrap_pyfunction!(dylib_path, m)?).unwrap();
     m.add_function(wrap_pyfunction!(update_datafiles, m)?)
         .unwrap();
     m.add_function(wrap_pyfunction!(githash, m)?).unwrap();
+    m.add_function(wrap_pyfunction!(version, m)?).unwrap();
     m.add_function(wrap_pyfunction!(build_date, m)?).unwrap();
     Ok(())
 }
```

### Comparing `satkit-0.2.5/src/pybindings/pyastrotime.rs` & `satkit-0.2.6/src/pybindings/pyastrotime.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 use pyo3::prelude::*;
 use pyo3::types::timezone_utc;
 use pyo3::types::PyDateTime;
 use pyo3::types::PyTuple;
-use pyo3::types::PyTzInfo;
 
 use crate::astrotime::{self, AstroTime, Scale};
 
 use super::pyduration::PyDuration;
 
 use numpy as np;
 
 /// Specify time scale used to represent or convert between the "satkit.time"
 /// representation of time
 ///
 /// Most of the time, these are not needed directly, but various time scales
 /// are needed to compute precise rotations between various inertial and
 /// Earth-fixed coordinate frames
 ///
-/// For details, see:
-/// https://stjarnhimlen.se/comp/time.html
+/// For an excellent overview, see:
+/// https://spsweb.fltops.jpl.nasa.gov/portaldataops/mpg/MPG_Docs/MPG%20Book/Release/Chapter2-TimeScales.pdf
 ///
 /// UTC = Universal Time Coordinate
 /// TT = Terrestrial Time
 /// UT1 = Universal time, corrected for polar wandering
 /// TAI = International Atomic Time
 /// GPS = Global Positioning System Time (epoch = 1/6/1980 00:00:00)
 /// TDB = Barycentric Dynamical Time
@@ -323,18 +322,18 @@
     /// # `utc_timezone` - Optional bool indicating use UTC as timezone
     ///                    if not passed in, defaults to true
     ///
     #[pyo3(signature = (utc=true))]
     fn datetime(&self, utc: bool) -> PyResult<PyObject> {
         pyo3::Python::with_gil(|py| -> PyResult<PyObject> {
             let timestamp: f64 = self.to_unixtime();
-            let mut tz: Option<&PyTzInfo> = Some(timezone_utc(py));
-            if utc == false {
-                tz = None;
-            }
+            let tz = match utc {
+                false => None,
+                true => Some(timezone_utc(py)),
+            };
             Ok(PyDateTime::from_timestamp(py, timestamp, tz)?.into_py(py))
         })
     }
 
     /// Convert to Modified Julian date
     /// 
     /// # Arguments:
@@ -632,51 +631,70 @@
 impl ToTimeVec for &PyAny {
     fn to_time_vec(&self) -> PyResult<Vec<AstroTime>> {
         // "Scalar" time input case
         if self.is_instance_of::<PyAstroTime>() {
             let tm: PyAstroTime = self.extract().unwrap();
             Ok(vec![tm.inner.clone()])
         }
+        else if self.is_instance_of::<PyDateTime>() {
+            let dt: &PyDateTime = self.extract().unwrap();
+            Ok(vec![PyAstroTime::from_datetime(dt).unwrap().inner])
+        }
         // List case
         else if self.is_instance_of::<pyo3::types::PyList>() {
             match self.extract::<Vec<PyAstroTime>>() {
                 Ok(v) => Ok(v.iter().map(|x| x.inner).collect::<Vec<_>>()),
-                Err(e) => Err(pyo3::exceptions::PyRuntimeError::new_err(format!(
-                    "Not a list of astro::AstroTime: {e}"
-                ))),
+                Err(e) => {
+                    match self.extract::<Vec<&PyDateTime>>() {
+                        Ok(v) => Ok(v.iter().map(|x| 
+                            PyAstroTime::from_datetime(x.extract().unwrap()).unwrap().inner)
+                            .collect::<Vec<_>>()),
+                        Err(e) => {
+                            Err(pyo3::exceptions::PyTypeError::new_err(format!(
+                                "Not a list of satkit.time or datetime.datetime: {e}"
+                            )))
+                        }
+                    }
+                }
+               
             }
         }
         // numpy array case
         else if self.is_instance_of::<numpy::PyArray1<PyObject>>() {
             match self.extract::<numpy::PyReadonlyArray1<PyObject>>() {
                 Ok(v) => pyo3::Python::with_gil(|py| -> PyResult<Vec<AstroTime>> {
                     // Extract times from numpya array of objects
                     let tmarray: Result<Vec<AstroTime>, _> = v
                         .as_array()
                         .into_iter()
                         .map(|p| -> Result<AstroTime, _> {
                             match p.extract::<PyAstroTime>(py) {
                                 Ok(v2) => Ok(v2.inner),
-                                Err(v2) => Err(v2),
+                                Err(_) => match p.extract::<&PyDateTime>(py) {
+                                    Ok(v3) => Ok(PyAstroTime::from_datetime(v3.extract().unwrap()).unwrap().inner),
+                                    Err(_) => Err(pyo3::exceptions::PyTypeError::new_err(format!(
+                                        "Input numpy array must contain satkit.time elements or datetime.datetime elements"
+                                    ))),
                             }
+                        }
                         })
                         .collect();
                     if !tmarray.is_ok() {
                         Err(pyo3::exceptions::PyRuntimeError::new_err(
-                            "Invalid AstroTime input",
+                            "Invalid satkit.time input",
                         ))
                     } else {
                         Ok(tmarray.unwrap())
                     }
                 }),
 
                 Err(e) => Err(pyo3::exceptions::PyRuntimeError::new_err(format!(
-                    "Invalid AstroTime input: {e}"
+                    "Invalid satkit.time or datetime.datetime input: {e}"
                 ))),
             }
         } else {
             Err(pyo3::exceptions::PyRuntimeError::new_err(
-                "Invalid AstroTime input",
+                "Invalid satkit.time or datetime.datetime input",
             ))
         }
     }
 }
```

### Comparing `satkit-0.2.5/src/pybindings/pyconsts.rs` & `satkit-0.2.6/src/pybindings/pyconsts.rs`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     #[classattr]
     ///  WGS-84 flattening
     const wgs84_f: f64 = cconsts::WGS84_F;
     #[classattr]
     /// WGS-84 Earth radius, meters
     const earth_radius: f64 = cconsts::EARTH_RADIUS;
 
-    ///  Gravitational parameter of Earth, m^3/s^2 */
+    ///  Gravitational parameter of Earth, m^3/s^2
     #[classattr]
     const mu_earth: f64 = cconsts::MU_EARTH;
     /// Gravitational parameter of moon, m^3/s^2
     #[classattr]
     const mu_moon: f64 = cconsts::MU_MOON;
 
     /// Gravitational parameter of sun, m^3/s^2
```

### Comparing `satkit-0.2.5/src/pybindings/pydensity.rs` & `satkit-0.2.6/src/pybindings/pydensity.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pyframetransform.rs` & `satkit-0.2.6/src/pybindings/pyframetransform.rs`

 * *Files 24% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 /// Vallado algorithm 15:
 ///
 /// GMST = 67310.5481 + (876600h + 8640184.812866) * tᵤₜ₁ * (0.983104 + tᵤₜ₁ * −6.2e−6)
 ///
 ///
 /// # Arguments
 ///
-/// * tm: AstroTime object representing input time
-///
+///   * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+///           representing time at which to calculate output
+/// 
 /// # Returns
 ///
-/// * Greenwich Mean Sideral Time,  radians
+/// * Greenwich Mean Sideral Time, radians, at intput time(s)
 ///
 #[pyfunction]
 pub fn gmst(tm: &PyAny) -> PyResult<PyObject> {
     py_func_of_time_arr(ft::gmst, tm)
 }
 
 ///
@@ -33,19 +34,20 @@
 }
 
 ///
 /// Greenwich apparant sidereal time, radians
 ///
 /// # Arguments:
 ///
-///   * tm: astro.time struct representing input time
+///   * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+///           representing time at which to calculate output
 ///
 /// # Returns:
 ///
-///  * Greenwich apparant sidereal time, radians
+///  * Greenwich apparant sidereal time, radians, at input time(s)
 ///
 #[pyfunction]
 pub fn gast(tm: &PyAny) -> PyResult<PyObject> {
     py_func_of_time_arr(ft::gast, tm)
 }
 
 ///
@@ -53,54 +55,81 @@
 ///
 /// See
 /// [IERS Technical Note 36, Chapter 5](https://www.iers.org/SharedDocs/Publikationen/EN/IERS/Publications/tn/TechnNote36/tn36_043.pdf?__blob=publicationFile&v=1)
 /// Equation 5.15
 ///
 /// # Arguments:
 ///
-///   * tm: AstroTime struct representing input time
+///  * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+///          representing time at which to calculate output
 ///
 /// # Returns:
 ///
-///  * Earth rotation angle, in radians
+///  * Earth rotation angle, in radians, at input time(s)
 ///
 /// # Calculation Details
 ///
 /// * Let t be UT1 Julian date
 /// * let f be fractional component of t (fraction of day)
 /// * ERA = 2𝜋 ((0.7790572732640 + f + 0.00273781191135448 * (t − 2451545.0))
 ///
-///
 #[pyfunction]
 pub fn earth_rotation_angle(tm: &PyAny) -> PyResult<PyObject> {
     py_func_of_time_arr(ft::earth_rotation_angle, tm)
 }
 
 ///
 /// Rotation from International Terrestrial Reference Frame
 /// (ITRF) to the Terrestrial Intermediate Reference System (TIRS)
 ///
 /// # Arguments:
 ///
-///   * tm: astro.time struct representing input time
-///
+///  * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+///          representing time at which to calculate output
+/// 
 /// # Returns:
 ///
-///  * Quaternion representing rotation from ITRF to TIRS
+///  * Quaternion representing rotation from ITRF to TIRS at input time(s)
 ///
 #[pyfunction]
 pub fn qitrf2tirs(tm: &PyAny) -> PyResult<PyObject> {
     py_quat_from_time_arr(ft::qitrf2tirs, tm)
 }
 
+///
+/// Rotation from Terrestrial Intermediate Reference System to
+/// Celestial Intermediate Reference Systems
+///
+/// # Arguments:
+///
+///  * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+///          representing time at which to calculate output
+/// 
+/// # Returns:
+///
+///  * Quaternion representing rotation from TIRS to CIRS at input time(s)
+///
 #[pyfunction]
 pub fn qtirs2cirs(tm: &PyAny) -> PyResult<PyObject> {
     py_quat_from_time_arr(ft::qtirs2cirs, tm)
 }
 
+///
+/// Rotation from Celestial Intermediate Reference System
+/// to Geocentric Celestial Reference Frame
+///
+/// # Arguments:
+///
+///  * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+///          representing time at which to calculate output
+/// 
+/// # Returns:
+///
+///  * Quaternion representing rotation from CIRS to GCRF at input time(s)
+///
 #[pyfunction]
 pub fn qcirs2gcrf(tm: &PyAny) -> PyResult<PyObject> {
     py_quat_from_time_arr(ft::qcirs2gcrs, tm)
 }
 
 ///
 /// Quaternion representing rotation from the
@@ -110,19 +139,20 @@
 /// Uses full IAU2006 Reduction
 /// See IERS Technical Note 36, Chapter 5
 ///
 /// Note: Very computationally expensive
 ///
 /// # Arguments:
 ///
-///   * `tm` - astro.time struct representing input time
+///  * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+///          representing time at which to calculate output
 ///
 /// # Returns:
 ///
-///  * Quaternion representing rotation from ITRF to GCRF
+///  * Quaternion representing rotation from ITRF to GCRF at input time(s)
 ///
 #[pyfunction]
 pub fn qitrf2gcrf(tm: &PyAny) -> PyResult<PyObject> {
     py_quat_from_time_arr(ft::qitrf2gcrf, tm)
 }
 
 ///
@@ -133,19 +163,20 @@
 /// Uses full IAU2006 Reduction
 /// See IERS Technical Note 36, Chapter 5
 ///
 /// Note: Very computationally expensive
 ///
 /// # Arguments:
 ///
-///   * `tm` - astro.time struct representing input time
+///  * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+///          representing time at which to calculate output
 ///
 /// # Returns:
 ///
-///  * Quaternion representing rotation from GCRF to ITRF
+///  * Quaternion representing rotation from GCRF to ITRF at input time(s)
 ///
 #[pyfunction]
 pub fn qgcrf2itrf(tm: &PyAny) -> PyResult<PyObject> {
     py_quat_from_time_arr(ft::qgcrf2itrf, tm)
 }
 
 ///
@@ -154,19 +185,20 @@
 /// International Terrestrial Reference Frame
 ///
 /// This uses an approximation of the IAU-76/FK5 Reduction
 /// See Vallado section 3.7.3
 ///
 /// # Arguments:
 ///
-///   * `tm` - astro.time struct representing input time
+///  * `tm`: scalar, list, or numpy array of astro.time or datetime.datetime 
+///          representing time at which to calculate output
 ///
 /// # Returns:
 ///
-///  * Quaternion representing rotation from GCRF to ITRF
+///  * Quaternion representing rotation from GCRF to ITRF at input time(s)
 ///
 #[pyfunction]
 pub fn qgcrf2itrf_approx(tm: &PyAny) -> PyResult<PyObject> {
     py_quat_from_time_arr(ft::qgcrf2itrf_approx, tm)
 }
 
 #[pyfunction]
@@ -180,15 +212,15 @@
 ///
 /// Note: TEME is output frame of SGP4 propagator
 ///
 /// This is Equation 3-90 in Vallado
 ///
 /// # Arguments:
 ///
-///   * tm: astro.time struct representing input time
+///  * tm: astro.time struct representing input time
 ///
 /// # Returns:
 ///
 ///  * Quaternion representing rotation from TEME to ITRF
 ///
 #[pyfunction]
 pub fn qteme2itrf(tm: &PyAny) -> PyResult<PyObject> {
```

### Comparing `satkit-0.2.5/src/pybindings/pygravity.rs` & `satkit-0.2.6/src/pybindings/pygravity.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pyitrfcoord.rs` & `satkit-0.2.6/src/pybindings/pyitrfcoord.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pyjplephem.rs` & `satkit-0.2.6/src/pybindings/pyjplephem.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pylpephem_moon.rs` & `satkit-0.2.6/src/pybindings/pylpephem_moon.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pylpephem_sun.rs` & `satkit-0.2.6/src/pybindings/pylpephem_sun.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pynrlmsise.rs` & `satkit-0.2.6/src/pybindings/pynrlmsise.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pypropagate.rs` & `satkit-0.2.6/src/pybindings/pypropagate.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pypropsettings.rs` & `satkit-0.2.6/src/pybindings/pypropsettings.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pyquaternion.rs` & `satkit-0.2.6/src/pybindings/pyquaternion.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pysatproperties.rs` & `satkit-0.2.6/src/pybindings/pysatproperties.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pysatstate.rs` & `satkit-0.2.6/src/pybindings/pysatstate.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pysgp4.rs` & `satkit-0.2.6/src/pybindings/pysgp4.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pysolarsystem.rs` & `satkit-0.2.6/src/pybindings/pysolarsystem.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pytle.rs` & `satkit-0.2.6/src/pybindings/pytle.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/pybindings/pyutils.rs` & `satkit-0.2.6/src/pybindings/pyutils.rs`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,16 @@
                     .to_object(py))
             }),
             Err(e) => Err(pyo3::exceptions::PyRuntimeError::new_err(e.to_string())),
         },
         _ => {
             let mut pout = ndarray::Array2::<f64>::zeros([tm.len(), 3]);
             let mut vout = ndarray::Array2::<f64>::zeros([tm.len(), 3]);
+
+            
             for (i, tm) in tm.iter().enumerate() {
                 match cfunc(tm) {
                     Ok(r) => {
                         pout.row_mut(i)
                             .assign(&ndarray::Array1::from_vec(vec![r.0[0], r.0[1], r.0[2]]));
                         vout.row_mut(i)
                             .assign(&ndarray::Array1::from_vec(vec![r.1[0], r.1[1], r.1[2]]));
```

### Comparing `satkit-0.2.5/src/sgp4/dpper.rs` & `satkit-0.2.6/src/sgp4/dpper.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/sgp4/dscom.rs` & `satkit-0.2.6/src/sgp4/dscom.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/sgp4/dsinit.rs` & `satkit-0.2.6/src/sgp4/dsinit.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/sgp4/dspace.rs` & `satkit-0.2.6/src/sgp4/dspace.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/sgp4/getgravconst.rs` & `satkit-0.2.6/src/sgp4/getgravconst.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/sgp4/initl.rs` & `satkit-0.2.6/src/sgp4/initl.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/sgp4/mod.rs` & `satkit-0.2.6/src/sgp4/mod.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/sgp4/satrec.rs` & `satkit-0.2.6/src/sgp4/satrec.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/sgp4/sgp4.rs` & `satkit-0.2.6/src/sgp4/sgp4.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/sgp4/sgp4_lowlevel.rs` & `satkit-0.2.6/src/sgp4/sgp4_lowlevel.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/sgp4/sgp4init.rs` & `satkit-0.2.6/src/sgp4/sgp4init.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/solarsystem.rs` & `satkit-0.2.6/src/solarsystem.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/spaceweather.rs` & `satkit-0.2.6/src/spaceweather.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/tle.rs` & `satkit-0.2.6/src/tle.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/utils/datadir.rs` & `satkit-0.2.6/src/utils/datadir.rs`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 use std::path::Path;
 use std::path::PathBuf;
 
 pub fn testdirs() -> Vec<PathBuf> {
     let mut testdirs: Vec<PathBuf> = Vec::new();
 
     // Look for paths in environment variable
-    match std::env::var(&"ASTRO_DATA") {
+    match std::env::var(&"SATKIT_DATA") {
         Ok(val) => testdirs.push(Path::new(&val).to_path_buf()),
         Err(_) => (),
     }
 
     // Look for paths in current library directory
     #[cfg(feature = "pybindings")]
     match get_dylib_path() {
@@ -60,15 +60,15 @@
 }
 
 /// Get directory where astronomy data is stored
 ///
 /// Tries the following paths in order, and stops when the
 /// files are found
 ///
-/// *  "ASTRO_DATA" environment variable
+/// *  "SATKIT_DATA" environment variable
 /// *  ${HOME}/astro-data
 /// *  ${HOME}
 /// *  /usr/share/astro-data
 /// *  On Mac Only:
 ///    * /Library/Application Support/astro-data
 ///    * ${Home}/Library/Application Support/astro-data
 ///
```

### Comparing `satkit-0.2.5/src/utils/download.rs` & `satkit-0.2.6/src/utils/download.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/utils/mod.rs` & `satkit-0.2.6/src/utils/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -23,12 +23,19 @@
 /// Return git hash of compiled library
 ///
 pub fn githash<'a>() -> &'a str {
     env!("GIT_HASH")
 }
 
 ///
+/// Return git tag of compiled library
+/// 
+pub fn gittag<'a>() -> &'a str {
+    env!("GIT_TAG")
+}
+
+///
 /// Return libary compile date
 ///
 pub fn build_date<'a>() -> &'a str {
     env!("BUILD_DATE")
 }
```

### Comparing `satkit-0.2.5/src/utils/skerror.rs` & `satkit-0.2.6/src/utils/skerror.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/utils/test.rs` & `satkit-0.2.6/src/utils/test.rs`

 * *Files identical despite different names*

### Comparing `satkit-0.2.5/src/utils/update_data.rs` & `satkit-0.2.6/src/utils/update_data.rs`

 * *Files identical despite different names*

