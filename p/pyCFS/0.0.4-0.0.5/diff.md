# Comparing `tmp/pyCFS-0.0.4.tar.gz` & `tmp/pyCFS-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCFS-0.0.4.tar", last modified: Mon Mar 25 21:35:56 2024, max compression
+gzip compressed data, was "pyCFS-0.0.5.tar", last modified: Mon Apr  8 15:22:17 2024, max compression
```

## Comparing `pyCFS-0.0.4.tar` & `pyCFS-0.0.5.tar`

### file list

```diff
@@ -1,131 +1,144 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.402034 pyCFS-0.0.4/
--rw-rw-rw-   0 root         (0) root         (0)     1012 2024-03-25 21:34:58.000000 pyCFS-0.0.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1278 2024-03-25 21:34:58.000000 pyCFS-0.0.4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     2074 2024-03-25 21:34:58.000000 pyCFS-0.0.4/Changelog.md
--rw-rw-rw-   0 root         (0) root         (0)     1264 2024-03-25 21:34:58.000000 pyCFS-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3796 2024-03-25 21:35:56.402034 pyCFS-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      366 2024-03-25 21:34:58.000000 pyCFS-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.370033 pyCFS-0.0.4/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.371033 pyCFS-0.0.4/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.371033 pyCFS-0.0.4/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)     6346 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/source/_static/pycfslogo-full-no-text-small.png
--rw-rw-rw-   0 root         (0) root         (0)    65714 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/source/_static/pycfslogo-full-no-text.png
--rw-rw-rw-   0 root         (0) root         (0)     1915 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/source/dev_notes.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.372033 pyCFS-0.0.4/docs/source/dev_source/
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/source/dev_source/conventions.md
--rw-rw-rw-   0 root         (0) root         (0)     2194 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/source/dev_source/data_handling.md
--rw-rw-rw-   0 root         (0) root         (0)     1853 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/source/dev_source/dev_notes_main.md
--rw-rw-rw-   0 root         (0) root         (0)      437 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1859 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/source/installation.md
--rw-rw-rw-   0 root         (0) root         (0)     2502 2024-03-25 21:34:58.000000 pyCFS-0.0.4/docs/source/pycfs_data.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.372033 pyCFS-0.0.4/pyCFS/
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.374034 pyCFS-0.0.4/pyCFS/data/
--rw-rw-rw-   0 root         (0) root         (0)      342 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.376033 pyCFS-0.0.4/pyCFS/data/extras/
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/extras/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21177 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/extras/ansys_io.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/extras/ansys_to_cfs_element_types.py
--rw-rw-rw-   0 root         (0) root         (0)    10335 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/extras/ensight_io.py
--rw-rw-rw-   0 root         (0) root         (0)     3038 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/extras/nihu_io.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/extras/nihu_to_cfs_element_types.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/extras/nihu_types.py
--rw-rw-rw-   0 root         (0) root         (0)    20494 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/extras/psv_io.py
--rw-rw-rw-   0 root         (0) root         (0)     5106 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/extras/vtk_to_cfs_element_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/extras/vtk_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.378033 pyCFS-0.0.4/pyCFS/data/io/
--rw-rw-rw-   0 root         (0) root         (0)     9850 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/io/CFSArray.py
--rw-rw-rw-   0 root         (0) root         (0)    55808 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/io/CFSMeshData.py
--rw-rw-rw-   0 root         (0) root         (0)    32969 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/io/CFSReader.py
--rw-rw-rw-   0 root         (0) root         (0)    20860 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/io/CFSResultData.py
--rw-rw-rw-   0 root         (0) root         (0)    36426 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/io/CFSWriter.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/io/cfs_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.379033 pyCFS-0.0.4/pyCFS/data/operators/
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/operators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9849 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/operators/fit_geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     7597 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/operators/interpolators.py
--rw-rw-rw-   0 root         (0) root         (0)    13237 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/operators/projection_interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)    18907 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/util.py
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/data/v_def.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    42644 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/pyCFS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.380034 pyCFS-0.0.4/pyCFS/util/
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/cli_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     4213 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/hdf5_io.py
--rw-rw-rw-   0 root         (0) root         (0)      930 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/lib_types.py
--rw-rw-rw-   0 root         (0) root         (0)     3751 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/setup_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.381034 pyCFS-0.0.4/pyCFS/util/templates/
--rw-rw-rw-   0 root         (0) root         (0)      757 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/templates/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/templates/mat.xml
--rw-rw-rw-   0 root         (0) root         (0)      237 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/templates/run_sim.py
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/templates/sim.jou
--rw-rw-rw-   0 root         (0) root         (0)      338 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/templates/sim.xml
--rw-rw-rw-   0 root         (0) root         (0)     1408 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/templates/sim_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2280 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyCFS/util/templates/sim_setup_opti.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.374034 pyCFS-0.0.4/pyCFS.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3796 2024-03-25 21:35:56.000000 pyCFS-0.0.4/pyCFS.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3358 2024-03-25 21:35:56.000000 pyCFS-0.0.4/pyCFS.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 21:35:56.000000 pyCFS-0.0.4/pyCFS.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-03-25 21:35:56.000000 pyCFS-0.0.4/pyCFS.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      385 2024-03-25 21:35:56.000000 pyCFS-0.0.4/pyCFS.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-25 21:35:56.000000 pyCFS-0.0.4/pyCFS.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2966 2024-03-25 21:34:58.000000 pyCFS-0.0.4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.382034 pyCFS-0.0.4/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-03-25 21:34:58.000000 pyCFS-0.0.4/requirements/common.txt
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-03-25 21:34:58.000000 pyCFS-0.0.4/requirements/data_extra.txt
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-03-25 21:34:58.000000 pyCFS-0.0.4/requirements/dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-03-25 21:35:56.402034 pyCFS-0.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-03-25 21:34:58.000000 pyCFS-0.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.384034 pyCFS-0.0.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.368033 pyCFS-0.0.4/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.367033 pyCFS-0.0.4/tests/data/extras/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.384034 pyCFS-0.0.4/tests/data/extras/ansys_io/
--rw-rw-rw-   0 root         (0) root         (0)   720896 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/ansys_io/ansys_io.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.390034 pyCFS-0.0.4/tests/data/extras/ensight_io/
--rw-rw-rw-   0 root         (0) root         (0)   970336 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/ensight_io/ensight_io.0000.U
--rw-rw-rw-   0 root         (0) root         (0)  4523376 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/ensight_io/ensight_io.0000.mesh
--rw-rw-rw-   0 root         (0) root         (0)   323936 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/ensight_io/ensight_io.0000.p
--rw-rw-rw-   0 root         (0) root         (0)      422 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/ensight_io/ensight_io.case
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.390034 pyCFS-0.0.4/tests/data/extras/ensight_io/poly/
--rw-rw-rw-   0 root         (0) root         (0)      782 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/ensight_io/poly/data.case
--rw-rw-rw-   0 root         (0) root         (0)    75544 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/ensight_io/poly/data00001.geo
--rw-rw-rw-   0 root         (0) root         (0)     3200 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/ensight_io/poly/data00001.scl1
--rw-rw-rw-   0 root         (0) root         (0)     7152 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/ensight_io/poly/data00001.vel
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.392034 pyCFS-0.0.4/tests/data/extras/nihu_io/
--rw-rw-rw-   0 root         (0) root         (0)  1381491 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/nihu_io/result_field.mat
--rw-rw-rw-   0 root         (0) root         (0)   894200 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/nihu_io/result_surface.mat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.395034 pyCFS-0.0.4/tests/data/extras/psv_io/
--rw-rw-rw-   0 root         (0) root         (0)      758 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/psv_io/line.npy
--rw-rw-rw-   0 root         (0) root         (0)   356352 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/psv_io/line.svd
--rw-rw-rw-   0 root         (0) root         (0)   158436 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/psv_io/line_h2_accelerance.unv
--rw-rw-rw-   0 root         (0) root         (0)   634880 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/psv_io/surface.svd
--rw-rw-rw-   0 root         (0) root         (0)     1241 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/psv_io/surface_dist.npy
--rw-rw-rw-   0 root         (0) root         (0)   394047 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/extras/psv_io/surface_h1_receptance.unv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.367033 pyCFS-0.0.4/tests/data/operators/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.396034 pyCFS-0.0.4/tests/data/operators/fit_geometry/
--rw-rw-rw-   0 root         (0) root         (0)   146369 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/operators/fit_geometry/fit_geometry_src.cfs
--rw-rw-rw-   0 root         (0) root         (0)    86438 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/operators/fit_geometry/fit_geometry_target.cfs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.398034 pyCFS-0.0.4/tests/data/operators/interpolators/
--rw-rw-rw-   0 root         (0) root         (0)   165563 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/operators/interpolators/interpolators.cfs
--rw-rw-rw-   0 root         (0) root         (0)  2051052 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/operators/interpolators/nn_elem.cfs
--rwxrwxrwx   0 root         (0) root         (0)    73117 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/operators/interpolators/nn_source.cfs
--rwxrwxrwx   0 root         (0) root         (0)    74841 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/operators/interpolators/nn_target.cfs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.400034 pyCFS-0.0.4/tests/data/operators/projection_interpolation/
--rw-rw-rw-   0 root         (0) root         (0)   981634 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/operators/projection_interpolation/source.cfs
--rw-rw-rw-   0 root         (0) root         (0)    44589 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/operators/projection_interpolation/target.cfs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 21:35:56.400034 pyCFS-0.0.4/tests/data/sim_io/
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/data/sim_io/elecFieldIntensity-sensor-positions-0.csv-1
--rw-rw-rw-   0 root         (0) root         (0)     3181 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/pycfs_data_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     7353 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/pycfs_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     8345 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/test_pycfs_core.py
--rw-rw-rw-   0 root         (0) root         (0)     8060 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/test_pycfs_data_extras.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/test_pycfs_data_io.py
--rw-rw-rw-   0 root         (0) root         (0)     8449 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/test_pycfs_data_operators.py
--rw-rw-rw-   0 root         (0) root         (0)     2574 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/test_pycfs_data_util.py
--rw-rw-rw-   0 root         (0) root         (0)     2074 2024-03-25 21:34:58.000000 pyCFS-0.0.4/tests/test_pycfs_sim_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.521576 pyCFS-0.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2024-04-08 15:21:18.000000 pyCFS-0.0.5/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.477577 pyCFS-0.0.5/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.483577 pyCFS-0.0.5/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      374 2024-04-08 15:21:18.000000 pyCFS-0.0.5/.gitlab/issue_templates/Default.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.484577 pyCFS-0.0.5/.gitlab/merge_request_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-08 15:21:18.000000 pyCFS-0.0.5/.gitlab/merge_request_templates/Default.md
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2024-04-08 15:21:18.000000 pyCFS-0.0.5/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2770 2024-04-08 15:21:18.000000 pyCFS-0.0.5/Changelog.md
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2024-04-08 15:21:18.000000 pyCFS-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-04-08 15:22:17.521576 pyCFS-0.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      366 2024-04-08 15:21:18.000000 pyCFS-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.484577 pyCFS-0.0.5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.486577 pyCFS-0.0.5/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.486577 pyCFS-0.0.5/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     6346 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/_static/pycfslogo-full-no-text-small.png
+-rw-rw-rw-   0 root         (0) root         (0)    65714 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/_static/pycfslogo-full-no-text.png
+-rw-rw-rw-   0 root         (0) root         (0)     1929 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/dev_notes.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.487577 pyCFS-0.0.5/docs/source/dev_source/
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/dev_source/conventions.md
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/dev_source/data_handling.md
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/dev_source/dev_notes_main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.478577 pyCFS-0.0.5/docs/source/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.488577 pyCFS-0.0.5/docs/source/examples/basics/
+-rw-rw-rw-   0 root         (0) root         (0)     4498 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/examples/basics/a_first_simulation.md
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/examples/basics/cli_tool.md
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/examples/basics/data_processing.md
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/examples/basics/introduction.md
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/examples/basics/result_handling.md
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/getting_started.md
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/installation.md
+-rw-rw-rw-   0 root         (0) root         (0)     2502 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/pycfs_data.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.489577 pyCFS-0.0.5/pyCFS/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.491577 pyCFS-0.0.5/pyCFS/data/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.493577 pyCFS-0.0.5/pyCFS/data/extras/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21452 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/ansys_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/ansys_to_cfs_element_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    10358 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/ensight_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     3038 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/nihu_io.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/nihu_to_cfs_element_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/nihu_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    20514 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/psv_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     5106 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/vtk_to_cfs_element_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/vtk_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.495577 pyCFS-0.0.5/pyCFS/data/io/
+-rw-rw-rw-   0 root         (0) root         (0)     9850 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/CFSArray.py
+-rw-rw-rw-   0 root         (0) root         (0)    56029 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/CFSMeshData.py
+-rw-rw-rw-   0 root         (0) root         (0)    32969 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/CFSReader.py
+-rw-rw-rw-   0 root         (0) root         (0)    21568 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/CFSResultData.py
+-rw-rw-rw-   0 root         (0) root         (0)    36590 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/CFSWriter.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/cfs_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.496577 pyCFS-0.0.5/pyCFS/data/operators/
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9849 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/operators/fit_geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)    11029 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/operators/interpolators.py
+-rw-rw-rw-   0 root         (0) root         (0)    13188 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/operators/projection_interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)    18909 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/util.py
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/v_def.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    48873 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/pyCFS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.497577 pyCFS-0.0.5/pyCFS/util/
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4213 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/hdf5_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/lib_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5658 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/setup_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.498577 pyCFS-0.0.5/pyCFS/util/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      757 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/mat.xml
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/run_sim.py
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/sim.jou
+-rw-rw-rw-   0 root         (0) root         (0)      338 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/sim.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/sim_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2280 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/sim_setup_opti.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.490577 pyCFS-0.0.5/pyCFS.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3720 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2966 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.499577 pyCFS-0.0.5/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-08 15:21:18.000000 pyCFS-0.0.5/requirements/common.txt
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-08 15:21:18.000000 pyCFS-0.0.5/requirements/data_extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-08 15:21:18.000000 pyCFS-0.0.5/requirements/dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-08 15:22:17.522576 pyCFS-0.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-08 15:21:18.000000 pyCFS-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.501577 pyCFS-0.0.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.481577 pyCFS-0.0.5/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.480577 pyCFS-0.0.5/tests/data/extras/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.501577 pyCFS-0.0.5/tests/data/extras/ansys_io/
+-rw-rw-rw-   0 root         (0) root         (0)   720896 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ansys_io/ansys_io.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.507577 pyCFS-0.0.5/tests/data/extras/ensight_io/
+-rw-rw-rw-   0 root         (0) root         (0)   970336 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.U
+-rw-rw-rw-   0 root         (0) root         (0)  4523376 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.mesh
+-rw-rw-rw-   0 root         (0) root         (0)   323936 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.p
+-rw-rw-rw-   0 root         (0) root         (0)      422 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.case
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.508576 pyCFS-0.0.5/tests/data/extras/ensight_io/poly/
+-rw-rw-rw-   0 root         (0) root         (0)      782 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data.case
+-rw-rw-rw-   0 root         (0) root         (0)    75544 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.geo
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.scl1
+-rw-rw-rw-   0 root         (0) root         (0)     7152 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.vel
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.510577 pyCFS-0.0.5/tests/data/extras/nihu_io/
+-rw-rw-rw-   0 root         (0) root         (0)  1381491 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/nihu_io/result_field.mat
+-rw-rw-rw-   0 root         (0) root         (0)   894200 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/nihu_io/result_surface.mat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.513576 pyCFS-0.0.5/tests/data/extras/psv_io/
+-rw-rw-rw-   0 root         (0) root         (0)      758 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/line.npy
+-rw-rw-rw-   0 root         (0) root         (0)   356352 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/line.svd
+-rw-rw-rw-   0 root         (0) root         (0)   158436 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/line_h2_accelerance.unv
+-rw-rw-rw-   0 root         (0) root         (0)   634880 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/surface.svd
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/surface_dist.npy
+-rw-rw-rw-   0 root         (0) root         (0)   236016 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/surface_h1_receptance.npy
+-rw-rw-rw-   0 root         (0) root         (0)   394047 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/surface_h1_receptance.unv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.481577 pyCFS-0.0.5/tests/data/operators/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.514577 pyCFS-0.0.5/tests/data/operators/fit_geometry/
+-rw-rw-rw-   0 root         (0) root         (0)   146369 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/fit_geometry/fit_geometry_src.cfs
+-rw-rw-rw-   0 root         (0) root         (0)    86438 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/fit_geometry/fit_geometry_target.cfs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.517576 pyCFS-0.0.5/tests/data/operators/interpolators/
+-rw-rw-rw-   0 root         (0) root         (0)   165563 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/interpolators/interpolators.cfs
+-rw-rw-rw-   0 root         (0) root         (0)  2051052 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/interpolators/nn_elem.cfs
+-rwxrwxrwx   0 root         (0) root         (0)    73117 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/interpolators/nn_source.cfs
+-rwxrwxrwx   0 root         (0) root         (0)    74841 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/interpolators/nn_target.cfs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.519576 pyCFS-0.0.5/tests/data/operators/projection_interpolation/
+-rw-rw-rw-   0 root         (0) root         (0)   981634 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/projection_interpolation/source.cfs
+-rw-rw-rw-   0 root         (0) root         (0)    44589 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/projection_interpolation/target.cfs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.519576 pyCFS-0.0.5/tests/data/sim_io/
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/sim_io/elecFieldIntensity-sensor-positions-0.csv-1
+-rw-rw-rw-   0 root         (0) root         (0)     3181 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/pycfs_data_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     7353 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/pycfs_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     8345 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     8434 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_data_extras.py
+-rw-rw-rw-   0 root         (0) root         (0)     8105 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_data_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     8526 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_data_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2574 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_data_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_sim_io.py
```

### Comparing `pyCFS-0.0.4/.gitignore` & `pyCFS-0.0.5/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 .pytest_cache/
 .mypy_cache/
 docs/build/latex/
 docs/build/html/
 docs/build/doctrees/
 
 # temporary : 
-examples/
+examples/capacitor_3d*/
+examples/clean_capacitor_3d*/
 data_tmp
 temp*.*
 
 # Environments
 .env
 .venv
 env/
```

### Comparing `pyCFS-0.0.4/.gitlab-ci.yml` & `pyCFS-0.0.5/.gitlab-ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,16 @@
   - pip install --upgrade pip
   - pip install -r requirements/dev.txt
 
 # build and deploy documentation on gitlab pages : 
 # runs only on 'main' branch if docs were changed
 pages:
   stage: build-docs
-  script: 
+  script:
+    - python -m pip install .
     - sphinx-build -M html docs/source/ docs/build/
     - mv docs/build/html public/
   artifacts:
     paths:
       - public
   rules:
     - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
```

### Comparing `pyCFS-0.0.4/Changelog.md` & `pyCFS-0.0.5/Changelog.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,119 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [0.0.4] - 2023-03-25
+## [Unreleased]
 
-### Added 
-- Possibility to read Meshes with groups/regions that have only Nodes defined. (As occuring when defining a nodeList) 
-in an openCFS simulation.
+### Added
+
+- ( new features )
+
+### Changed
+
+- ( changes in existing functionality )
+
+### Deprecated
+
+- ( soon-to-be removed features )
+
+### Removed
+
+- ( now removed features )
+
+### Fixed
+
+- ( any bug fixes )
+
+### Security
+
+- ( in case of vulnerabilities )
+
+## [0.0.5] - 2024-04-08
+
+### Added
+
+- Support for Reading/Writing MultiStepIDs other than 1.
+- Support for Reading MultiStep with unsorted StepValues (requires sort before writing)
+
+### Changed
+
+- CFSResultData to contain data of a single MultiStep only.
+- Improved testing using numpy.testing
+- Improved import for better usability of data submodule
+- Renamed nearest neighbor interpolator based on search direction
+
+## [0.0.4] - 2024-03-25
+
+### Added
+
+- Possibility to read Meshes with groups/regions that have only Nodes defined. (As occuring when defining a nodeList)
+  in an openCFS simulation.
 - Method to find closest node/element for CFSMeshData objects
 - Warning when element quality and centroids are not computed automatically due to size.
 
 ### Changed
+
 - Website URL to openCFS Homepage.
 - Testing of CFSReader to check read mesh and data values
 
-### Fixed 
+### Fixed
+
 - Critical bug when reading MultiStepData
 
-## [0.0.3] - 2023-03-20
+## [0.0.3] - 2024-03-20
+
+### Added
 
-### Added 
 - Possibility to just run the meshing for the given parameters.
 - Additional meshing setup control with `remeshing_on` and `mesh_present`
 - `track_results` property to choose which results from the hdf file to track.
 - Getter functions for hdf and sensor array results.
 
 ### Changed
+
 - Running simulations in parallel does not do an initial mesh generation if `remeshing_on = False`.
 
 ### Removed
+
 - `init_params` that needed to be passed to the `pyCFS` constructor, it is no longer used.
 
-### Fixed 
+### Fixed
+
 - Data module import.
 
-## [0.0.2] - 2023-03-18
+## [0.0.2] - 2024-03-18
 
 ### Added
 
 - `pyCFS.data` package
-  - code, tests and doc
-- Sensor array result support 
-  - Because CFS currently does not write SA results into the `hdf` file
+    - code, tests and doc
+- Sensor array result support
+    - Because CFS currently does not write SA results into the `hdf` file
 
 ### Changed
 
 - Extended dependencies to accommodate `pyCFS.data` package
 
-## [0.0.1] - 2023-03-12
+## [0.0.1] - 2024-03-12
 
-### Added 
+### Added
 
 - Old `pycfs` package code (refactored)
-- CI pipeline for automated testing 
+- CI pipeline for automated testing
 - GitLab pages for documentation
-  
-### Fixed 
+
+### Fixed
 
 - Parallelization when meshing
 - Type hints
 
-### Removed 
+### Removed
 
-- History results are no longer supported 
-  - These are now to be written into the `hdf` file
-- Sensor array results are the only exception 
-  - When CFS can directly write these to the `hdf` file this package will change accordingly 
-  - Users should not see much difference in behavior
+- History results are no longer supported
+    - These are now to be written into the `hdf` file
+- Sensor array results are the only exception
+    - When CFS can directly write these to the `hdf` file this package will change accordingly
+    - Users should not see much difference in behavior
```

### Comparing `pyCFS-0.0.4/LICENSE` & `pyCFS-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/PKG-INFO` & `pyCFS-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCFS
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library for automating and data handling tasks for openCFS.
 Author-email: IGTE <igte.gitlab@gmail.com>, Eniz Mušeljić <eniz.m@outlook.com>, Andreas Wurzinger <andreas.wurzinger@tugraz.at>
 License: MIT License
         
         Copyright (c) 2024 Verein zur Förderung der Software openCFS
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyCFS-0.0.4/docs/Makefile` & `pyCFS-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/docs/make.bat` & `pyCFS-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/docs/source/_static/pycfslogo-full-no-text-small.png` & `pyCFS-0.0.5/docs/source/_static/pycfslogo-full-no-text-small.png`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/docs/source/_static/pycfslogo-full-no-text.png` & `pyCFS-0.0.5/docs/source/_static/pycfslogo-full-no-text.png`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/docs/source/conf.py` & `pyCFS-0.0.5/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pyCFS
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = pyCFS.__name__
 copyright = "2024, Verein zur Förderung der Software openCFS"
-author = pyCFS.__author__
+author = " and ".join(pyCFS.__author__)
 release = pyCFS.__version__
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.duration",
```

### Comparing `pyCFS-0.0.4/docs/source/dev_source/data_handling.md` & `pyCFS-0.0.5/docs/source/dev_source/data_handling.md`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/docs/source/installation.md` & `pyCFS-0.0.5/docs/source/installation.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,75 @@
-# Installation 
+# Installation
 
-## Environment setup 
+## Environment setup
 
-This section covers the setup of the environment used for running the library. Please make sure that you follow the instructions in the given order. 
+This section covers the setup of the environment used for running the library. Please make sure that you follow the
+instructions in the given order.
 
 :::{important}
-If you are a developer just set up the conda environment as below and follow with the [developer install](#developer-install).
+If you are a developer just set up the conda/virtual environment as below (step 1) and follow with
+the [developer install](#developer-install).
 :::
 
-1. Install python version 3.12. It is recommended to install [anaconda](https://www.anaconda.com/download) or [miniconda](https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html). After doing so, open the command prompt and follow the next steps.
-   - Create a new environment with : 
-   ```bash
-    conda create --name pycfs python=3.12
-    ```
-   - Switch to new environment with : 
-    ```bash
-    conda activate pycfs
-    ```
-2. Install *pyCFS* 
-   - If you are using conda as suggested just run :
-    ```bash
-    python -m pip install --upgrade pycfs
-    ```
-   - If you are using your system python :
-    ```bash
-    pip install --upgrade pycfs
-    ```
+1. Install python version  >= 3.10.
+    1. (Recommended) Install [anaconda](https://www.anaconda.com/download)
+       or [miniconda](https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html). After doing so, open
+       the command prompt and follow the next steps.
+        - Create a new environment with :
+       ```bash
+        conda create --name pycfs python=3.12
+        ```
+        - Switch to new environment with :
+        ```bash
+        conda activate pycfs
+        ```
+    2. (Alternatively) Create a virtual environment in your project root directory (`~`) with :
+       - Create a new environment with :
+            ```bash
+            python3.10 -m venv ~/.venv/pycfs
+            ```
+            (requires locally installed python>=3.10)
+        - Switch to new environment with :
+        
+            - Linux bash: 
+                ```bash
+                source ~/.venv/pycfs/bin/activate
+                ```
+
+            - Windows PowerShell
+                ```powershell
+                ~\.venv\pycfs\Scripts\Activate.ps1
+                ```
+2. Install *pyCFS*
+    - Install via pip :
+        ```bash
+        python -m pip install --upgrade pycfs
+        ```
+3. Install *openCFS* and *coreform cubit* :
+    - Follow [this tutorial](https://opencfs.gitlab.io/userdocu/Installation/)
+
+## Developer install
 
-## Developer install 
+First you will need to clone the repository and `cd` into the repository root. As a developer you will need to install
+a few dependencies more than what is needed to just use the package.
 
-First you will need to clone the repository and `cd` into the repository root. As a developer you will need to install 
-a few dependencies more than what is needed to just use the package. 
+1. Setup up your python environment using anaconda or virtual environment.
 
-1. Install the requirements by running : 
+2. Install the requirements by running :
    ```bash
    python -m pip install -r requirements/dev.txt
    ```
-2. To install the package make sure you're in the root directory. If you are 
-using an anaconda distribution just run : 
-```
-$ python -m pip install -e .
-```
-the `-e` flag (editable install) applies the changes you make while developing directly to the package so that you can easily test it while developing in this source directory.
-
-3. If you are using the system python run : 
-```
-pip3 install -r requirements/dev.txt
-pip3 install -e .
-```
-This will install the required packages and then the `pyCFS` package itself.
+3. To install the package make sure you're in the root directory. Make sure you have activated your
+   conda environment or virtual environment, and then run:
+
+   ```bash
+   python -m pip install -e .
+   ```
+
+   the `-e` flag (editable install) applies the changes you make while developing directly to the package so that you can
+   easily test it while developing in this source directory.
+
+This will install the required packages and then the `pyCFS` package itself. You can test your installation by running :
+
+```bash
+pytest
+```
```

### Comparing `pyCFS-0.0.4/docs/source/pycfs_data.md` & `pyCFS-0.0.5/docs/source/pycfs_data.md`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS/data/extras/ansys_io.py` & `pyCFS-0.0.5/pyCFS/data/extras/ansys_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 """
 Module containing data processing utilities for reading Ansys RST files
 """
 
 from __future__ import annotations
 
+import importlib.util
 import numpy as np
+
+if importlib.util.find_spec("ansys") is None:
+    raise ModuleNotFoundError(
+        "Missing dependency for submodule pyCFS.data.extras.ansys_io. "
+        "To install pyCFS with all required dependencies run 'pip install -U pyCFS[data]'"
+    )
+
 from ansys.dpf import core as dpf
 from typing import List, Tuple, Dict
 
 from pyCFS.data.extras import ansys_to_cfs_element_types
 from pyCFS.data import io, v_def
 from pyCFS.data.io import cfs_types
 from pyCFS.data.extras.vtk_to_cfs_element_types import vtk_to_cfs_elem_type
@@ -76,19 +84,18 @@
         elif e.type == dpf.element_types.Point1:
             self.Num_POINT += 1
         else:
             raise Exception(f"Type {e.type} needs to be added to 'update_with_element' method")
 
 
 class CFSMeshData(io.CFSMeshData):
-
     def __init__(self, include_skin=True, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.MeshInfo: CFSMeshInfo = CFSMeshInfo()
-        if self.Coordinates.shape and self.Types.shape:
+        if self.Coordinates.size > 0 and self.Types.size > 0:
             self.update_info()
 
         self.ElemIDs: np.ndarray | None = None
         self.NodeIDs: np.ndarray | None = None
         self._ElemIDs_vol: np.ndarray | None = None
         self._ElemIDs_skin: np.ndarray | None = None
         self._include_skin = include_skin
```

### Comparing `pyCFS-0.0.4/pyCFS/data/extras/ansys_to_cfs_element_types.py` & `pyCFS-0.0.5/pyCFS/data/extras/nihu_to_cfs_element_types.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import numpy as np
-from ansys.dpf import core as dpf
+from pyCFS.data.extras.nihu_types import nihu_element_type
 from pyCFS.data.io.cfs_types import cfs_element_type
 
-type_link_ansys_cfs = {
-    dpf.element_types.Tet10: cfs_element_type.TET10,
-    dpf.element_types.Hex20: cfs_element_type.HEXA20,
-    dpf.element_types.Wedge15: cfs_element_type.WEDGE15,
-    dpf.element_types.Pyramid13: cfs_element_type.PYRA13,
-    dpf.element_types.Tri6: cfs_element_type.TRIA6,
-    dpf.element_types.Quad8: cfs_element_type.QUAD8,
-    dpf.element_types.Tet4: cfs_element_type.TET4,
-    dpf.element_types.Hex8: cfs_element_type.HEXA8,
-    dpf.element_types.Wedge6: cfs_element_type.WEDGE6,
-    dpf.element_types.Pyramid5: cfs_element_type.PYRA5,
-    dpf.element_types.Tri3: cfs_element_type.TRIA3,
-    dpf.element_types.Quad4: cfs_element_type.QUAD4,
-    dpf.element_types.Line2: cfs_element_type.LINE2,
-    dpf.element_types.Point1: cfs_element_type.POINT,
+type_link_nihu_cfs = {
+    nihu_element_type.UNDEF: cfs_element_type.UNDEF,
+    nihu_element_type.ConstantPoint: cfs_element_type.POINT,
+    nihu_element_type.LinearLine: cfs_element_type.LINE2,
+    nihu_element_type.LinearTria: cfs_element_type.TRIA3,
+    nihu_element_type.LinearQuad: cfs_element_type.QUAD4,
+    nihu_element_type.QuadraticLine: cfs_element_type.LINE3,
+    nihu_element_type.QuadraticTria: cfs_element_type.TRIA6,
+    nihu_element_type.QuadraticQuad: cfs_element_type.QUAD8,
+    nihu_element_type.QuadraticQuadMid: cfs_element_type.QUAD9,
+    nihu_element_type.LinearTetra: cfs_element_type.TET4,
+    nihu_element_type.LinearHexa: cfs_element_type.HEXA8,
 }
 
 
-# mapping ansys dpf element types array to cfs element types array
-def dpf_to_cfs_elem_type(ansys_elem_types: np.ndarray):
-    return np.vectorize(type_link_ansys_cfs.get)(ansys_elem_types)
+# mapping nihu element types array to cfs element types array
+def nihu_to_cfs_elem_type(nihu_elem_types: np.ndarray):
+    return np.vectorize(type_link_nihu_cfs.get)(nihu_elem_types)
```

### Comparing `pyCFS-0.0.4/pyCFS/data/extras/ensight_io.py` & `pyCFS-0.0.5/pyCFS/data/extras/ensight_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,19 @@
      - 'fieldNames' (list): List of field names (meaning cell and point arrays).
      - 'fieldDataTypes' (list): List of field data types (types: 'Cell' or 'Point').
      - 'numSteps' (int): Number of time steps.
      - 'timeRange' (tuple): start and end point of the time values.
      - 'timeSteps' (numpy array) : one-dimensional array of time steps.
 
     Args:
+    -----
         reader (vtk.vtkEnSightGoldBinaryReader): The EnSight reader object.
 
     Returns:
+    --------
         dict: A dictionary containing the retrieved information.
 
     """
 
     field_name_list = []
     field_data_type_list = []
```

### Comparing `pyCFS-0.0.4/pyCFS/data/extras/nihu_io.py` & `pyCFS-0.0.5/pyCFS/data/extras/nihu_io.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS/data/extras/psv_io.py` & `pyCFS-0.0.5/pyCFS/data/extras/psv_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,25 +166,31 @@
 
         if entry["id2"] == id2_str:
             data_frf["data"].append(entry["data"])
 
     return data_frf
 
 
-def convert_frf_form(frf_data: Dict, frf_form: str):
+def convert_frf_form(frf_data: Dict, frf_form: str) -> Dict:
+    # noinspection LongLine
     """
     Converts frf_data of type 'receptance', 'mobility', or 'accelerance' to another one of these.
-    :param frf_data: dict with keys: 'Coordinates', 'Connectivity', 'elem_types', 'frequency',
-                                  'frf_form', 'frf_type', 'data_frf', 'ref_channel'
-    :param frf_form: form of frf:
-        'receptance' = displacement/force,
-        'mobility' = velocity/force,
-        'accelerance' = acceleration/force,
-    :return frf_data: dict with keys: 'Coordinates', 'Connectivity', 'elem_types', 'frequency',
-                                  'frf_form', 'frf_type', 'data_frf', 'ref_channel'
+
+    Parameters
+    ----------
+    frf_data : dict
+        dict with keys: 'Coordinates', 'Connectivity', 'elem_types', 'frequency', 'frf_form', 'frf_type', 'data_frf', 'ref_channel'
+    frf_form : str
+        form of frf: 'receptance' = displacement/force, 'mobility' = velocity/force, 'accelerance' = acceleration/force,
+
+    Returns
+    -------
+    frf_data : dict
+        dict with keys: 'Coordinates', 'Connectivity', 'elem_types', 'frequency', 'frf_form', 'frf_type', 'data_frf', 'ref_channel'
+
     """
     if frf_form not in ["receptance", "mobility", "accelerance"]:
         raise Exception('conversion only supports "receptance", "mobility", "accelerance" as target form!')
 
     if frf_data["frf_form"] == "receptance":
         if frf_form == "mobility":
             # noinspection PyMissingOrEmptyDocstring
```

### Comparing `pyCFS-0.0.4/pyCFS/data/extras/vtk_to_cfs_element_types.py` & `pyCFS-0.0.5/pyCFS/data/extras/vtk_to_cfs_element_types.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS/data/extras/vtk_types.py` & `pyCFS-0.0.5/pyCFS/data/extras/vtk_types.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS/data/io/CFSArray.py` & `pyCFS-0.0.5/pyCFS/data/io/CFSArray.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS/data/io/CFSMeshData.py` & `pyCFS-0.0.5/pyCFS/data/io/CFSMeshData.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,31 +283,31 @@
     >>> mesh = CFSMeshData(coordinates=coordinates, connectivity=connectivity, ElementTypes=ElementTypes,
     >>>                    regions=region_data)
 
     """
 
     def __init__(
         self,
-        coordinates=np.empty(()),
-        connectivity=np.empty(()),
+        coordinates=np.empty((0, 3)),
+        connectivity=np.empty((0, 1)),
         types=np.empty(0),
         regions: List[CFSRegData] | None = None,
         verbosity=v_def.release,
     ) -> None:
         """Initializes a CFSMeshData object. If both Coordinates and types are provided,
         also updates mesh attributes."""
         if regions is None:
             regions = []
         self._Verbosity = verbosity
         self.Coordinates = coordinates
         self.Connectivity = connectivity
         self.Types: np.ndarray = types
         self.MeshInfo: CFSMeshInfo = CFSMeshInfo()
         self.Regions: List[CFSRegData] = regions
-        if self.Coordinates.shape and self.Types.shape:
+        if self.Coordinates.size > 0 and self.Types.size > 0:
             self.update_info()
         self.check_add_point_elements()
         self._flag_warn_element_centroid = True
         self._flag_warn_element_quality = True
         self._ElementCentroids: np.ndarray | None = None
         self._Quality: np.ndarray | None = None
 
@@ -430,15 +430,15 @@
                         coordinates=self.Coordinates,
                     ),
                     el_idx_it,
                 )
             ):
                 mesh_centroids[i] = res
         vprint(
-            f" | Elapsed time: {datetime.timedelta(seconds=int(time.time() - t_start))}",
+            f" | Elapsed time: {datetime.timedelta(seconds=round(time.time() - t_start))}",
             verbose=self._Verbosity >= v_def.debug,
         )
         return mesh_centroids
 
     @property
     def Quality(self) -> np.ndarray | None:
         """
@@ -660,15 +660,15 @@
                 # Define Element IDs
                 reg.Elements = np.arange(reg.Nodes.size, dtype=np.int32) + self.Connectivity.shape[0] + 1
                 # Add elements to connectivity and types
                 conn_add = np.zeros((reg.Nodes.size, self.Connectivity.shape[1]))
                 conn_add[:, 0] = reg.Nodes
                 el_types_add = np.array([cfs_element_type.POINT for _ in range(reg.Nodes.size)], dtype=np.int32)
                 self.Connectivity = np.vstack((self.Connectivity, conn_add))
-                self.Types = np.vstack((self.Types, el_types_add))
+                self.Types = np.hstack((self.Types, el_types_add))
 
     def drop_unused_nodes_elements(self, reg_data_list: List[CFSRegData]):
         """
         Drop nodes and elements that are not used in the given list of groups/regions.
 
         Parameters
         ----------
@@ -990,44 +990,49 @@
         if result_data is not None:
             # TODO: Adapt element result data
             raise NotImplementedError("Adapting result data not implemented!")
             return result_data
 
         return None
 
-    def get_region_nodes(self, region: str) -> np.ndarray:
-        reg_obj = list_search(self.Regions, region)
+    def get_region(self, region: str | CFSRegData) -> CFSRegData:
+        return list_search(self.Regions, region)
+
+    def get_region_nodes(self, region: str | CFSRegData) -> np.ndarray:
+        reg_obj = self.get_region(region=region)
         return reg_obj.Nodes
 
-    def get_region_elements(self, region: str) -> np.ndarray:
-        reg_obj = list_search(self.Regions, region)
+    def get_region_elements(self, region: str | CFSRegData) -> np.ndarray:
+        reg_obj = self.get_region(region=region)
         return reg_obj.Elements
 
-    def get_region_coordinates(self, region: str) -> np.ndarray:
-        reg_obj = list_search(self.Regions, region)
+    def get_region_coordinates(self, region: str | CFSRegData) -> np.ndarray:
+        reg_obj = self.get_region(region=region)
         return self.Coordinates[reg_obj.Nodes - 1]
 
-    def get_region_connectivity(self, region: str) -> np.ndarray:
-        reg_obj = list_search(self.Regions, region)
+    def get_region_connectivity(self, region: str | CFSRegData) -> np.ndarray:
+        reg_obj = self.get_region(region=region)
         return self.Connectivity[reg_obj.Elements - 1]
 
-    def get_region_centroids(self, region: str, processes: int | None = None) -> np.ndarray:
-        reg_obj = list_search(self.Regions, region)
+    def get_region_centroids(self, region: str | CFSRegData, processes: int | None = None) -> np.ndarray:
+        reg_obj = self.get_region(region=region)
         return self.get_mesh_centroids(el_idx=reg_obj.Elements - 1, processes=processes)
 
-    def get_closest_node(self, coordinate: np.ndarray, region: str | None = None, eps: float = 1e-3) -> np.ndarray:
+    def get_closest_node(
+        self, coordinate: np.ndarray, region: str | CFSRegData | None = None, eps: float = 1e-3
+    ) -> np.ndarray:
         """
         Return node ids of closest nodes to coordinate array.
 
         Parameters
         ----------
 
         coordinate: np.ndarray
             Coordinate array (Nx3, N is the number of query points)
-        region : str, optional
+        region : str or CFSRegData, optional
             Name of the group/region. The default is ``None``, in which case the global mesh will be used instead.
         eps : float, optional
             Show warning if distance of closest node exceeds the specified value. The default value is ``1e-3``.
         Returns
         -------
         np.ndarray
             Array of node ids (starting from 0) of the closest node to the respective coordinate. If region is passed,
@@ -1182,16 +1187,16 @@
     >>>                    regions=region_data)
 
     """
 
     def __init__(
         self,
         name: str,
-        elements=np.empty(()),
-        nodes=np.empty(()),
+        elements=np.empty(0),
+        nodes=np.empty(0),
         dimension=-1,
         is_group=False,
         verbosity=v_def.release,
     ):
         self._Elements = np.empty(0)
         self._Nodes = np.empty(0)
```

### Comparing `pyCFS-0.0.4/pyCFS/data/io/CFSReader.py` & `pyCFS-0.0.5/pyCFS/data/io/CFSReader.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS/data/io/CFSResultData.py` & `pyCFS-0.0.5/pyCFS/data/io/CFSResultData.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,25 @@
         self,
         analysis_type=cfs_analysis_type.NO_ANALYSIS,
         multi_step_id=1,
         data: List[CFSResultArray] | None = None,
         verbosity=v_def.release,
     ):
         self._Verbosity = verbosity
-        self.AnalysisType = analysis_type
-        self.MultiStepID = multi_step_id
+        self._AnalysisType = cfs_analysis_type.NO_ANALYSIS
+        self._MultiStepID = 1
         self.Data: List[CFSResultArray] = []  # List of Result Data Arrays
         if data is not None:
             if isinstance(data, list):
                 for item in data:
                     self.add_data_array(item)
             else:
                 raise TypeError("'data' must be a list of CFSResultArray objects!")
+        self.AnalysisType = analysis_type
+        self.MultiStepID = multi_step_id
 
     def __repr__(self) -> str:
         return f"""MultiStep {self.MultiStepID}: {self.AnalysisType}, {self.StepValues.size} steps"""
 
     # noinspection PyArgumentList
     def __str__(self) -> str:
         info_str = str().join([str(ri) for ri in self.ResultInfo])
@@ -126,42 +128,45 @@
             [
                 data_equality,
                 self.AnalysisType == other.AnalysisType,
                 self.MultiStepID == other.MultiStepID,
             ]
         )
 
-    # @property
-    # def MultiStepID(self) -> Set[int]:
-    #     """
-    #     Set of MultiStep IDs (property from ResultInfo).
-    #     """
-    #     if self.ResultInfo:
-    #         id_collection = [r_info.MultiStepID for r_info in self.ResultInfo]
-    #         return set(id_collection)
-    #
-    # @MultiStepID.setter
-    # def MultiStepID(self, multi_step_id: int):
-    #     for r_info in self.ResultInfo:
-    #         r_info.MultiStepID = multi_step_id
-    #
-    # @property
-    # def AnalysisType(self) -> Set[cfs_analysis_type]:
-    #     """
-    #     Set of analysis types (property from ResultInfo).
-    #     """
-    #     if self.ResultInfo:
-    #         analysis_type_collection = [r_info.AnalysisType for r_info in self.ResultInfo]
-    #         return set(analysis_type_collection)
-    #
-    # @AnalysisType.setter
-    # def AnalysisType(self, AnalysisType: cfs_analysis_type):
-    #     if self.ResultInfo:
-    #         for r_info in self.ResultInfo:
-    #             r_info.AnalysisType = AnalysisType
+    @property
+    def MultiStepID(self) -> int:
+        """
+        MultiStep ID (CFSResultData can contain data from only one MultiStep currently!)
+        """
+        return self._MultiStepID
+        # if self.ResultInfo:
+        #     id_collection = [r_info.MultiStepID for r_info in self.ResultInfo]
+        #     return set(id_collection)
+
+    @MultiStepID.setter
+    def MultiStepID(self, multi_step_id: int):
+        self._MultiStepID = multi_step_id
+        for r_array in self.Data:
+            r_array.MultiStepID = multi_step_id
+
+    @property
+    def AnalysisType(self) -> cfs_analysis_type:
+        """
+        Analysis type of MultiStepData (CFSResultData can contain data from only one MultiStep currently!)
+        """
+        return self._AnalysisType
+        # if self.ResultInfo:
+        #     analysis_type_collection = [r_info.AnalysisType for r_info in self.ResultInfo]
+        #     return set(analysis_type_collection)
+
+    @AnalysisType.setter
+    def AnalysisType(self, analysis_type: cfs_analysis_type):
+        self._AnalysisType = analysis_type
+        for r_info in self.ResultInfo:
+            r_info.AnalysisType = analysis_type
 
     @property
     def ResultInfo(self) -> List[CFSResultInfo]:
         """
         Structure containing information about the corresponding CFSResultArray object in self.Data
 
         Returns
@@ -175,18 +180,18 @@
                 result_info.append(r_array.ResultInfo)
 
         return result_info
 
     @property
     def StepValues(self) -> np.ndarray:
         """
-        Step Values of MultiStep 1 (property from ResultInfo). All data sets of one MultiStep must have the same
+        Step Values of MultiStep property. All data sets of one MultiStep must have the same
         step values currently!
         """
-        return self.get_multi_step_step_values()
+        return self.get_multi_step_step_values(multi_step_id=self.MultiStepID)
 
     @StepValues.setter
     def StepValues(self, step_values: np.ndarray | List[float]):
         self.set_multi_step_step_values(step_values)
 
     def get_multi_step_step_values(self, multi_step_id=1) -> np.ndarray:
         for item in self.Data:
@@ -272,16 +277,16 @@
             Name of the region on which the result is defined.
         restype : pyCFS.data.io.cfs_types.cfs_result_type, optional
             Type of the result data. The default is ``None`` in which case the result type is identified automatically.
             Only works, if there are not multiple result types specified.
 
         Returns
         -------
-        list[pyCFS.data.io.CFSArray]
-            List of extracted result data arrays.
+        pyCFS.data.io.CFSResultArray
+            Extracted result data arrays.
 
         Examples
         --------
         >>> from pyCFS.data.io import CFSReader
         >>> with CFSReader('file.cfs') as f:
         >>>     result_data = f.MultiStepData
         >>> result_array = result_data.get_data_array(quantity='quantity', region='region')
@@ -518,14 +523,33 @@
                 res_type=restype,
                 is_complex=is_complex,
                 multi_step_id=multi_step_id,
                 analysis_type=analysis_type,
             )
         )
 
+    def sort_steps(self, return_idx=False) -> None | np.ndarray:
+        """
+        Sort data arrays by increasing step values.
+
+        Returns
+        -------
+        np.ndarray
+            index array used for sorting.
+        """
+        idx_sort = np.argsort(self.StepValues)
+        for item in self.Data:
+            item[:] = item[idx_sort, :, :]
+            item.StepValues[:].sort()
+
+        if return_idx:
+            return idx_sort
+        else:
+            return None
+
     def _get_result_info(
         self,
         multi_step_id=1,
         quantity: str | None = None,
         region: str | None = None,
         res_type: cfs_result_type | None = None,
     ) -> List[CFSResultInfo]:
```

### Comparing `pyCFS-0.0.4/pyCFS/data/io/CFSWriter.py` & `pyCFS-0.0.5/pyCFS/data/io/CFSWriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,32 +372,32 @@
             grp_result_mesh.attrs.create("ExternalFiles", data=externalFiles, dtype=np.dtype("int32"))
 
         return grp_result_mesh
 
     @staticmethod
     def create_multistep(
         grp_result_mesh: h5py.Group,
-        stepNr=1,
-        analysisType=cfs_analysis_type.NO_ANALYSIS,
+        multi_step_id=1,
+        analysis_type=cfs_analysis_type.NO_ANALYSIS,
     ) -> Tuple[h5py.Group, h5py.Group]:
         """
         Create MultiStep
         :param grp_result_mesh:
-        :param stepNr:
-        :param analysisType:
+        :param multi_step_id:
+        :param analysis_type:
         :return: 'MultiStep' and 'ResultsDescription' object of opened HDF5 file_src
         """
-        if f"MultiStep_{stepNr}" in grp_result_mesh:
-            grp_multi_step = grp_result_mesh[f"MultiStep_{stepNr}"]
+        if f"MultiStep_{multi_step_id}" in grp_result_mesh:
+            grp_multi_step = grp_result_mesh[f"MultiStep_{multi_step_id}"]
             grp_result_description = grp_result_mesh["ResultDescription"]
         else:
-            if analysisType == cfs_analysis_type.NO_ANALYSIS:
-                print(f"WARNING: Created MultiStep result with analysis type {analysisType}")
-            grp_multi_step = grp_result_mesh.require_group(f"MultiStep_{stepNr}")
-            grp_multi_step.attrs.create("AnalysisType", analysisType, dtype=h5py.special_dtype(vlen=bytes))
+            if analysis_type == cfs_analysis_type.NO_ANALYSIS:
+                print(f"WARNING: Created MultiStep result with analysis type {analysis_type}")
+            grp_multi_step = grp_result_mesh.require_group(f"MultiStep_{multi_step_id}")
+            grp_multi_step.attrs.create("AnalysisType", analysis_type, dtype=h5py.special_dtype(vlen=bytes))
             grp_multi_step.attrs.create("LastStepNum", data=0, dtype=np.dtype("uint32"))
             grp_multi_step.attrs.create("LastStepValue", data=0, dtype=np.dtype("float64"))
 
             grp_result_description = grp_multi_step.require_group("ResultDescription")
 
         return grp_multi_step, grp_result_description
 
@@ -681,30 +681,30 @@
         )
 
         return f_external
 
     def prepare_write_multistep(
         self,
         res_info: List[CFSResultInfo],
-        multiStep=1,
+        multi_step_id=1,
         analysis_type=cfs_analysis_type.NO_ANALYSIS,
     ):
         """
         Write ResultDescription and create datasets (needs to be done a priori in case of parallel write)
         :param pyCFS.data.io.CFSResultInfo res_info: needs to contain single MultiStep results only!
         :param dict res_shape_dict:
-        :param int multiStep:
+        :param int multi_step_id:
         :param pyCFS.data.io.cfs_types.cfs_analysis_type analysis_type:
         """
 
         # Create Result
         with h5py.File(self._filename, "r+", driver=self._h5driver) as f:
             grp_result_mesh = CFSWriter.create_result(f["Results"])
             grp_multi_step, grp_result_description = CFSWriter.create_multistep(
-                grp_result_mesh, stepNr=multiStep, analysisType=analysis_type
+                grp_result_mesh, multi_step_id=multi_step_id, analysis_type=analysis_type
             )
             q_set = set()
             for r_info in res_info:
                 vprint(
                     f"Initializing result: {r_info}",
                     verbose=self._Verbosity >= v_def.debug,
                 )
@@ -762,19 +762,21 @@
                         r_info.Region,
                         r_info.ResType,
                         r_info.DataShape[1:],
                         is_complex=r_info.IsComplex,
                         compression_lvl=self.CompressionLvl,
                     )
 
-    def perform_write_multistep(self, result_data: CFSResultData):
+    def perform_write_multistep(self, result_data: CFSResultData, multi_step_id: int | None = None):
         """
         Write data to MultiStep
         :param pyCFS.data.io.CFSResultData result_data:
         """
+        if multi_step_id is None:
+            multi_step_id = result_data.MultiStepID
         with h5py.File(self._filename, "r+", driver=self._h5driver) as f:
             for stepnum in progressbar(
                 range(len(result_data.StepValues)),
                 "Writing Step:  ",
                 40,
                 verbose=self._Verbosity >= v_def.release,
             ):
@@ -784,34 +786,34 @@
                     q_name = data.Quantity
                     reg = data.Region
                     res_type = data.ResType
                     dname = "Real"
                     data_write = data[stepnum, :, :].real
                     # noinspection LongLine
                     dset = f[
-                        f"Results/Mesh/MultiStep_{result_data.MultiStepID}/Step_{stepnum + 1}/{q_name}/{reg}/{res_type}/{dname}"
+                        f"Results/Mesh/MultiStep_{multi_step_id}/Step_{stepnum + 1}/{q_name}/{reg}/{res_type}/{dname}"
                     ]
 
                     CFSWriter.write_step_result(dset, data_write)
 
                     if data.IsComplex:
                         dname = "Imag"
                         data_write = data[stepnum, :, :].imag
                         # noinspection LongLine
                         dset = f[
-                            f"Results/Mesh/MultiStep_{result_data.MultiStepID}/Step_{stepnum + 1}/{q_name}/{reg}/{res_type}/{dname}"
+                            f"Results/Mesh/MultiStep_{multi_step_id}/Step_{stepnum + 1}/{q_name}/{reg}/{res_type}/{dname}"
                         ]
 
                         CFSWriter.write_step_result(dset, data_write)
 
-    def finalize_write_multistep(self, res_info: List[CFSResultInfo], multiStep=1):
+    def finalize_write_multistep(self, res_info: List[CFSResultInfo], multi_step_id=1):
         """
         Write datasets to ResultsDescription that need to be written after the data (in case of parallel write)
         :param res_info:
-        :param multiStep:
+        :param multi_step_id:
         """
         reg_dict: Dict[str, List[str]] = dict()
         dim_names_dict: Dict[str, List[str]] = dict()
         for r_info in res_info:
             if r_info.Quantity is None or r_info.Region is None:
                 raise ValueError(f"Region {r_info.__repr__()} not properly defined!")
             if r_info.Quantity in reg_dict:
@@ -825,15 +827,15 @@
         with h5py.File(self._filename, "r+") as f:
             for q_name in reg_dict:
                 vprint(
                     f"Finalizing result: {q_name}",
                     verbose=self._Verbosity >= v_def.debug,
                 )
                 CFSWriter.finalize_result_description(
-                    f[f"Results/Mesh/MultiStep_{multiStep}/ResultDescription/{q_name}"],
+                    f[f"Results/Mesh/MultiStep_{multi_step_id}/ResultDescription/{q_name}"],
                     reg_dict[q_name],
                     dim_names_dict[q_name],
                 )
 
     def write_multistep(self, result_data: CFSResultData, multi_step_id: int | None = None):
         """
         Write ResultDescription and create datasets, write data to multistep and write datasets to ResultsDescription
@@ -852,13 +854,11 @@
         >>> with CFSWriter('file.cfs') as f:
         >>>     f.write_multistep(result_data=results)
 
         """
         if multi_step_id is None:
             multi_step_id = result_data.MultiStepID
         self.prepare_write_multistep(
-            res_info=result_data.ResultInfo,
-            multiStep=result_data.MultiStepID,
-            analysis_type=result_data.AnalysisType,
+            res_info=result_data.ResultInfo, multi_step_id=multi_step_id, analysis_type=result_data.AnalysisType
         )
-        self.perform_write_multistep(result_data=result_data)
-        self.finalize_write_multistep(res_info=result_data.ResultInfo, multiStep=result_data.MultiStepID)
+        self.perform_write_multistep(result_data=result_data, multi_step_id=multi_step_id)
+        self.finalize_write_multistep(res_info=result_data.ResultInfo, multi_step_id=multi_step_id)
```

### Comparing `pyCFS-0.0.4/pyCFS/data/io/cfs_types.py` & `pyCFS-0.0.5/pyCFS/data/io/cfs_types.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS/data/operators/fit_geometry.py` & `pyCFS-0.0.5/pyCFS/data/operators/fit_geometry.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS/data/operators/interpolators.py` & `pyCFS-0.0.5/pyCFS/data/operators/interpolators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from typing import Optional
+
 import numpy as np
 import scipy
 from scipy.spatial import KDTree
 
 from pyCFS.data.io import cfs_types
 from pyCFS.data import io
 from pyCFS.data.util import progressbar
@@ -64,25 +66,93 @@
     row_ptr = np.array(row_ptr_lst)
     interpolation_matrix = scipy.sparse.csr_array(
         (val.flatten(), col_ind.flatten(), row_ptr), matrix_shape, dtype=float
     )
     return interpolation_matrix
 
 
-def interpolation_matrix_nearest_neighbor_inverse(
+def interpolation_matrix_nearest_neighbor(
+    source_coord: np.ndarray,
+    target_coord: np.ndarray,
+    num_neighbors=20,
+    interpolation_exp=2.0,
+    max_distance: float | None = None,
+    formulation: Optional[str] = None,
+) -> scipy.sparse.csr_array | scipy.sparse.csc_array:
+    """
+    Computes interpolation matrix based on nearest neighbor search with inverse distance weighting (Shepard's method)
+    (see https://opencfs.gitlab.io/userdocu/DataExplanations/NN/). Nearest neighbors are searched for each point on the
+    source (forward) or target (backward) grid.
+
+
+    Parameters
+    ----------
+    source_coord: np.ndarray
+        Coordinate array of m source points. Expected shape (m, 3)
+    target_coord: np.ndarray
+        Coordinates of n target points. Expected shape (n, 3)
+    num_neighbors: int
+        Number of neighbors considered for nearest neighbor search
+    interpolation_exp: float, optional
+        Exponent of inverse distance weighting (Shepard's method)
+    max_distance: str, optional
+        Set interpolation weights to zero if max_distance is exceeded.
+    formulation: str, optional
+        Search direction for nearest neighbor search. By default, direction is chosen automatically based on number of
+        source and target points.
+        'forward': Nearest neighbors are searched for each point on the (coarser) target grid. Leads to checkerboard
+        if the target grid is finer than the source grid.
+        'bakcward': Nearest neighbors are searched for each point on the (coarser) source grid. Leads to overprediction
+        if the source grid is finer than the target grid.
+
+    Returns
+    -------
+    scipy.sparse.csr_array or scipy.sparse.csc_array
+        Sparse operator matrix. Type depends on formulation. 'forward' returns csc_array, 'backward' returns csr_array.
+    """
+    if formulation is None:
+        if source_coord.shape[0] < target_coord.shape[0]:
+            print(
+                "Detected fine target grid (based on number of points). "
+                "Automatically selected 'forward' nearest neighbor search. This can lead to checkerboard structures. "
+                "Please check the result, "
+                " 'backward' formulation yields better results for coarse target grids."
+            )
+            formulation = "forward"
+        else:
+            print(
+                "Detected coarse target grid (based on number of points). "
+                "Automatically selected 'backward' nearest neighbor search. This can lead to overprediction. "
+                "Please check the result, "
+                " 'forward' formulation yields better results for coarse target grids."
+            )
+            formulation = "backward"
+    if formulation == "forward":
+        return _interpolation_matrix_nearest_neighbor_forward(
+            source_coord, target_coord, num_neighbors, interpolation_exp, max_distance
+        )
+    elif formulation == "backward":
+        return _interpolation_matrix_nearest_neighbor_backward(
+            source_coord, target_coord, num_neighbors, interpolation_exp, max_distance
+        )
+    else:
+        raise ValueError("formulation argument has to be one of: None, 'forward', or 'backward'")
+
+
+def _interpolation_matrix_nearest_neighbor_backward(
     source_coord: np.ndarray,
     target_coord: np.ndarray,
     num_neighbors=20,
-    interpolation_exp=2,
+    interpolation_exp=2.0,
     max_distance: float | None = None,
 ) -> scipy.sparse.csr_array:
     """
     Computes interpolation matrix based on nearest neighbor search with inverse distance weighting (Shepard's method)
-    (see https://opencfs.gitlab.io/userdocu/DataExplanations/NN/) Nearest neighbors are searched for each point on the
-    (finer) target grid.
+    (see https://opencfs.gitlab.io/userdocu/DataExplanations/NN/). Nearest neighbors are searched for each point on the
+    (coarser) target grid. Leads to checkerboard if the target grid is finer than the source grid.
     """
     # Calculate weights
     source_coord_kdtree = KDTree(source_coord)
     d, idx_list = source_coord_kdtree.query(target_coord, num_neighbors, workers=-1)
 
     matrix_shape = (target_coord.shape[0], source_coord.shape[0])
 
@@ -119,25 +189,25 @@
     interpolation_matrix = scipy.sparse.csr_array(
         (val, np.array(col_ind).flatten(), np.array(row_ptr)), matrix_shape, dtype=float
     )
 
     return interpolation_matrix
 
 
-def interpolation_matrix_nearest_neighbor(
+def _interpolation_matrix_nearest_neighbor_forward(
     source_coord: np.ndarray,
     target_coord: np.ndarray,
     num_neighbors=20,
     interpolation_exp=2.0,
     max_distance: float | None = None,
 ) -> scipy.sparse.csc_array:
     """
     Computes interpolation matrix based on nearest neighbor search with inverse distance weighting (Shepard's method)
     (see https://opencfs.gitlab.io/userdocu/DataExplanations/NN/). Nearest neighbors are searched for each point on the
-    (finer) source grid.
+    (coarser) source grid. Leads to overprediction if the source grid is finer than the target grid.
     """
     # Calculate weights
     target_coord_kdtree = KDTree(target_coord)
     d, idx_list = target_coord_kdtree.query(source_coord, num_neighbors, workers=-1)
 
     matrix_shape = (target_coord.shape[0], source_coord.shape[0])
 
@@ -175,40 +245,38 @@
         (val, np.array(row_ind).flatten(), np.array(col_ptr)), matrix_shape, dtype=float
     )
 
     return interpolation_matrix
 
 
 def apply_interpolation(
-    result_data: io.CFSResultData,
+    result_array: io.CFSResultArray,
     interpolation_matrix: scipy.sparse.csr_array | scipy.sparse.csc_array,
-    quantity: str,
-    region: str,
-    restype: cfs_types.cfs_result_type,
-    restype_out: cfs_types.cfs_result_type,
-    quantity_out: str | None = None,
-    region_out: str | None = None,
-):
+    restype_out: Optional[cfs_types.cfs_result_type] = None,
+    quantity_out: Optional[str] = None,
+    region_out: Optional[str] = None,
+) -> io.CFSResultArray:
     """
     Performs interpolation based on sparse interpolation matrix for all data steps.
     """
     if quantity_out is None:
-        quantity_out = quantity
+        quantity_out = result_array.Quantity
     if region_out is None:
-        region_out = region
+        region_out = result_array.Region
+    if restype_out is None:
+        restype_out = result_array.ResType
 
-    step_values = result_data.StepValues
-    data_in = result_data.get_data_array(quantity=quantity, region=region)
-    data_out = io.CFSResultArray(
+    step_values = result_array.StepValues
+    result_array_out = io.CFSResultArray(
         np.empty(
-            (data_in.shape[0], interpolation_matrix.shape[0], data_in.shape[2]),
-            dtype=data_in.dtype,
+            (result_array.shape[0], interpolation_matrix.shape[0], result_array.shape[2]),
+            dtype=result_array.dtype,
         )
     )
-    data_out.MetaData = data_in.MetaData
+    result_array_out.MetaData = result_array.MetaData
+    result_array_out.Quantity = quantity_out
+    result_array_out.Region = region_out
+    result_array_out.ResType = restype_out
     for i in progressbar(range(len(step_values)), prefix="Performing interpolation:"):
-        data_out[i, :, :] = interpolation_matrix.dot(data_in[i, :, :])
-
-    result_data_out = io.CFSResultData()
-    result_data_out.add_data_array(data=data_out, quantity=quantity_out, region=region_out, restype=restype_out)
+        result_array_out[i, :, :] = interpolation_matrix.dot(result_array[i, :, :])
 
-    return result_data_out
+    return result_array_out
```

### Comparing `pyCFS-0.0.4/pyCFS/data/operators/projection_interpolation.py` & `pyCFS-0.0.5/pyCFS/data/operators/projection_interpolation.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import time
 from itertools import repeat
 from multiprocessing import Pool
 
 import numpy as np
 from scipy import sparse
 from skspatial.objects import Point, Vector, Line, Plane, Triangle
-from typing import List, Dict
+from typing import List, Dict, Optional
 
 from pyCFS.data import io
-from pyCFS.data.io import cfs_types
+from pyCFS.data.io import cfs_types, CFSResultData
 from pyCFS.data.operators import interpolators
 from pyCFS.data.util import progressbar, vecnorm
 
 
 ###############################################
 # class PointVal is an extension of the class Point to add values and IDs
 # to the Coordinates and generate a point-value pair with an ID
@@ -122,75 +122,60 @@
             )
         )
         j += 1
     return triangle_list
 
 
 def interp_matrix(
-    trgt_point_list,
-    src_point_list,
-    triangle_list,
-    proj_direction: List[np.ndarray] | np.ndarray,
-    max_proj_distance,
-    search_radius=None,
-    eps=-1e-9,
-):
-    interpolation_matrix = np.zeros([len(trgt_point_list), len(src_point_list)])
-
-    if type(proj_direction) is np.ndarray:
-        proj_direction = [proj_direction for _ in range(len(trgt_point_list))]
-
-    for idx, point in enumerate(progressbar(trgt_point_list, prefix="Building interpolation matrix: ", size=25)):
-        res = interp_matrix_point(
-            point,
-            triangle_list,
-            proj_direction[idx],
-            max_proj_distance,
-            search_radius,
-            eps,
-        )
-        if res is not None:
-            interpolation_matrix[point.id, res[0]] = res[1]
-
-    return interpolation_matrix
-
-
-def interp_matrix_parallel(
     trgt_point_list: List,
     src_point_list: List,
     triangle_list: List,
     proj_direction: List[np.ndarray] | np.ndarray,
     max_proj_distance: float,
     search_radius: float | None = None,
     eps=-1e-9,
+    workers: Optional[int] = None,
 ):
     interpolation_matrix = np.zeros([len(trgt_point_list), len(src_point_list)])
 
     if type(proj_direction) is np.ndarray:
         proj_direction = [proj_direction for _ in range(len(trgt_point_list))]
 
-    print("Building interpolation matrix", end="")
-    with Pool() as pool:
-        t_start = time.time()
-        for idx, res in enumerate(
-            pool.starmap(
-                interp_matrix_point,
-                zip(
-                    trgt_point_list,
-                    repeat(triangle_list),
-                    proj_direction,
-                    repeat(max_proj_distance),
-                    repeat(search_radius),
-                    repeat(eps),
-                ),
+    if workers is None or workers > 1:
+        print("Building interpolation matrix", end="")
+        with Pool(processes=workers) as pool:
+            t_start = time.time()
+            for idx, res in enumerate(
+                pool.starmap(
+                    interp_matrix_point,
+                    zip(
+                        trgt_point_list,
+                        repeat(triangle_list),
+                        proj_direction,
+                        repeat(max_proj_distance),
+                        repeat(search_radius),
+                        repeat(eps),
+                    ),
+                )
+            ):
+                if res is not None:
+                    interpolation_matrix[trgt_point_list[idx].id, res[0]] = res[1]
+        print(f" | Elapsed time: {datetime.timedelta(seconds=int(time.time() - t_start))}")
+    else:
+        for idx, point in enumerate(progressbar(trgt_point_list, prefix="Building interpolation matrix: ", size=25)):
+            res = interp_matrix_point(
+                point,
+                triangle_list,
+                proj_direction[idx],
+                max_proj_distance,
+                search_radius,
+                eps,
             )
-        ):
             if res is not None:
-                interpolation_matrix[trgt_point_list[idx].id, res[0]] = res[1]
-    print(f" | Elapsed time: {datetime.timedelta(seconds=int(time.time() - t_start))}")
+                interpolation_matrix[point.id, res[0]] = res[1]
 
     return interpolation_matrix
 
 
 def interp_matrix_point(
     point: Point | PointVal,
     triangle_list: List,
@@ -226,14 +211,15 @@
     trgt_coord: np.ndarray,
     trgt_conn: np.ndarray,
     trgt_reg_node: np.ndarray,
     trgt_reg_elem: np.ndarray,
     proj_direction: np.ndarray | List[np.ndarray] | None = None,
     max_distance=0.03,
     search_radius: float | None = None,
+    workers: Optional[int] = None,
 ):
     """
     Interpolation matrix for projection-based interpolation. Points of the target mesh are projected onto the
     source mesh and evaluated based on linear FE basis functions.
     """
     src_coord_reg = src_coord[src_reg_node - 1]
     src_conn_reg = src_conn[src_reg_elem - 1, :]
@@ -259,21 +245,16 @@
         for el_id, tria in enumerate(trgt_triangle_list):
             vn[el_id, :] = tria.normal_vector()
 
         for k in range(len(trgt_point_list)):
             el_idx = np.where(trgt_conn_reg_mapped == k)[0]
             proj_direction.append(vecnorm(np.mean(vn[el_idx], axis=0)))
 
-    interpolation_matrix = interp_matrix_parallel(
-        trgt_point_list,
-        src_point_list,
-        src_triangle_list,
-        proj_direction,
-        max_distance,
-        search_radius,
+    interpolation_matrix = interp_matrix(
+        trgt_point_list, src_point_list, src_triangle_list, proj_direction, max_distance, search_radius, workers=workers
     )
 
     interpolation_matrix_sparse = sparse.csr_matrix(interpolation_matrix)
 
     return interpolation_matrix_sparse
 
 
@@ -283,24 +264,25 @@
     region_src_target_dict: Dict,
     quantity_name: str,
     dim_names=None,
     is_complex=None,
     projection_direction: np.ndarray | None = None,
     max_projection_distance=0.1,
     search_radius=None,
+    workers: Optional[int] = None,
 ) -> io.CFSResultData:
     """
     max_projection_distance: Lower values speed up interpolation matrix build and prevent projecting onto far surfaces.
     search_radius            Should be chosed at least to the maximum element size of the target grid.
     """
     with io.CFSReader(file_src) as h5reader:
         src_mesh = h5reader.MeshData
         src_data = h5reader.MultiStepData
 
-    result_data_list = []
+    result_array_list = []
     for src_region_name in region_src_target_dict:
         # Convert quads to triangles in src mesh
         src_mesh.convert_quad2tria()
         src_region = src_mesh.Regions[src_mesh.Regions.index(src_region_name)]
 
         target_region_list = []
         with io.CFSReader(file_target) as h5reader:
@@ -333,24 +315,25 @@
                 target_coord,
                 target_connectivity,
                 target_reg_nodes,
                 target_reg_elems,
                 proj_direction=projection_direction,
                 max_distance=max_projection_distance,
                 search_radius=search_radius,
+                workers=workers,
             )
 
             # Perform interpolation
-            result_data = interpolators.apply_interpolation(
-                src_data,
-                interpolation_matrix,
-                quantity_name,
-                src_region_name,
-                cfs_types.cfs_result_type.NODE,
-                cfs_types.cfs_result_type.NODE,
+            src_array = src_data.get_data_array(
+                quantity=quantity_name, region=src_region_name, restype=cfs_types.cfs_result_type.NODE
+            )
+            result_array = interpolators.apply_interpolation(
+                result_array=src_array,
+                interpolation_matrix=interpolation_matrix,
+                restype_out=cfs_types.cfs_result_type.NODE,
                 region_out=target_region.Name,
             )
 
             # # Perform interpolation
             # step_value_list = src_data.StepValues
             # data_write = []
             # for i in progressbar(range(step_value_list.shape[0]), 'Performing interpolation: '):
@@ -360,14 +343,12 @@
             #
             # # Write Data object
             # result_data = io.CFSResultData(analysis_type=cfs_types.cfs_analysis_type.HARMONIC)
             # result_data.add_data(data_write, step_values=step_value_list, quantity=quantity_name,
             #                      region=target_region.Name, restype=cfs_types.cfs_result_type.NODE, dim_names=dim_names,
             #                      is_complex=is_complex)
             #
-            result_data_list.append(result_data)
+            result_array_list.append(result_array)
 
-    return_data = result_data_list[0]
-    for i in range(1, len(result_data_list)):
-        return_data.combine_with(result_data_list[i])
-
-    return return_data
+    return CFSResultData(
+        analysis_type=src_data.AnalysisType, multi_step_id=src_data.MultiStepID, data=result_array_list
+    )
```

### Comparing `pyCFS-0.0.4/pyCFS/data/util.py` & `pyCFS-0.0.5/pyCFS/data/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                     connectivity_list=connectivity_list,
                 ),
                 range(n_cells),
             )
         ):
             connectivity[i, 0 : res[0]] = res[1]
     vprint(
-        f" | Elapsed time: {datetime.timedelta(seconds=int(time.time() - t_start))}",
+        f" | Elapsed time: {datetime.timedelta(seconds=round(time.time() - t_start))}",
         verbose=verbose,
     )
 
     return connectivity
 
 
 def list_search(obj: List, item):
```

### Comparing `pyCFS-0.0.4/pyCFS/pyCFS.py` & `pyCFS-0.0.5/pyCFS/pyCFS.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import re
+import time
 from glob import glob
 from tqdm.auto import tqdm
 from multiprocessing import Pool
 import numpy as np
 import numpy.typing as npt
-from typing import List, Callable, Optional, TypeAlias
+from typing import List, Callable, Optional, TypeAlias, Dict
 
 from .util import hdf5_io as h5io
 from .util.lib_types import (
     pyCFSparamVec,
     pyCFSparam,
     nestedResultDict,
     resultVec,
@@ -23,20 +24,26 @@
 N_PARAM_GROUPS = 4
 CFS_EXT = "cfs"
 XML_EXT = "xml"
 JOU_EXT = "jou"
 CDB_EXT = "cdb"
 SA_NAME_SEPARATOR = "-"
 SA_COORD_KEYS = ["origElemNum", "globCoord", "locCoord"]
+LAST_EXEC_START = "last_exec_start"
+LAST_EXEC_STOP = "last_exec_stop"
+
+INFO_BOX_WIDTH = 90
+INFO_BOX_CHAR = "#"
 
 # Paths :
 RESULTS_HDF_DIR = "results_hdf5"
 HISTORY_DIR = "history"
 LOGS_DIR = "logs"
-SA_STORAGE_PATH = f"./{HISTORY_DIR}/"
+SA_STORAGE_DIR = f"{HISTORY_DIR}"
+DATA_DUMP_DIR = "data_dump"
 
 
 class pyCFS:
     def __init__(
         self,
         project_name: str,
         cfs_install_dir: str,
@@ -56,14 +63,15 @@
         save_hdf_results: bool = False,
         array_fill_value: pyCFSparam = np.nan,
         parallelize: bool = False,
         remeshing_on: bool = False,
         n_jobs_max: int = 1000,
         testing: bool = False,
         track_results: Optional[List[str]] = None,
+        dump_results: bool = False,
     ):
         """
 
         OpenCFS and Trelis/CoreformCubit python interfacing package. The main
         goal of this module is to make an easy to use interface which provides
         a class that handles the automatic simulation setup from given CFS and
         Trelis parameters and the result storage.
@@ -119,14 +127,17 @@
 
             testing (bool): If true will indicate to not create any directories or leave
                             footprints. Used for clean automated testing.
 
             track_results (List[str], optional): List of results which are to be tracked from
                                                  the main hdf file. If `None` then all results
                                                  are tracked. (default = None).
+
+            dump_results (bool, optional): If True then after each run the tracked results are
+                                           saved to disk. (default = False).
         """
 
         self.pyCFSobj: TypeAlias = pyCFS
 
         # Set init params from args :
         self.project_name = project_name
         self.sim_file = cfs_proj_path + project_name
@@ -144,14 +155,15 @@
         self.n_jobs_max = n_jobs_max
         self.mat_file_name = mat_file_name
         self.init_file_extension = init_file_extension
         self.res_manip_fun = res_manip_fun
         self.trelis_version = trelis_version
         self.testing = testing
         self.track_results = track_results
+        self.dump_results = dump_results
 
         self.trelis_params_names = trelis_params_names
         self.n_trelis_params = len(trelis_params_names)
 
         self.mat_params_names = material_params_names
         self.n_mat_params = len(material_params_names)
 
@@ -175,14 +187,17 @@
 
         # Set functions -> less branches in code :
         self._init_functions()
 
         # Init sensor array setup :
         self._init_sensor_array_setup()
 
+        # Print status report :
+        self._print_init_status_report()
+
     def __call__(self, X: pyCFSparamVec, mesh_only: bool = False, mesh_present: bool = False) -> None:
         """
 
         Simulation forward function. Performs the simulation for the passed
         parameter combinations. Does not return anything as the results are
         stored in the self.results dictionary.
 
@@ -195,49 +210,70 @@
             mesh_only (bool): If true only mesh files are generated for the
                              given parameters. (default = False).
 
         Returns:
             None
         """
 
-        self.mesh_present = mesh_present
+        self._set_mesh_present_status(mesh_present)
 
         # check parameter shape :
         self._check_given_params(X)
 
+        # record start time :
+        self._record_time(LAST_EXEC_START)
+
         # run meshing only if True :
         if mesh_only:
             self._generate_meshes(X)
         # else run whole pipeline :
         else:
             self._forward(X)  # type: ignore[attr-defined]
 
+        # record finish time :
+        self._record_time(LAST_EXEC_STOP)
+
+        # dump results if on :
+        self._contruct_run_metadata(X)
+        self._dump_results_if_on()
+
+        # print run status report :
+        self._print_run_status_report()
+
     # * ------------------ Init methods ------------------
     def _init_placeholders(self) -> None:
         self.files: List[str] = []
         self.sim_files: List[str] = []
         self.params_changed: npt.NDArray[np.bool_] = np.ones((N_PARAM_GROUPS,), dtype=bool)
 
         self._init_results()
         self.results_keys: List[str] = []
         self.result_regions: Optional[List[str]] = None
-        self.ind = 0
-        self.mesh_present = False
+        self.ind: int = 0
+        self.mesh_present: bool = False
+        self.time: Dict[str, str] = {
+            LAST_EXEC_START: "",
+            LAST_EXEC_STOP: "",
+            "init_time": time.ctime(time.time()),
+        }
+        self.result_dump_path: str = ""
 
     def _init_paths(self) -> None:
         """
 
         Initializes path variables and generates result paths if not present.
 
         """
 
         self.hdf_res_path = f"{self.cfs_proj_path}{RESULTS_HDF_DIR}/{self.project_name}/"
         self.hdf_file_path = f"{self.cfs_proj_path}{RESULTS_HDF_DIR}/{self.project_name}.{CFS_EXT}"
         self.logs_path = f"{self.cfs_proj_path}{LOGS_DIR}/"
         self.history_path = f"{self.cfs_proj_path}{HISTORY_DIR}/"
+        self.data_dump_path = f"{self.cfs_proj_path}{DATA_DUMP_DIR}/"
+        self.sa_storage_path = f"{self.cfs_proj_path}{SA_STORAGE_DIR}/"
 
         if not self.testing:
 
             if not os.path.exists(self.history_path):
                 os.makedirs(self.history_path)
 
             if not os.path.exists(self.hdf_res_path):
@@ -245,14 +281,20 @@
 
             if not os.path.exists(self.hdf_res_path):
                 os.makedirs(self.hdf_res_path)
 
             if not os.path.exists(self.logs_path):
                 os.makedirs(self.logs_path)
 
+            if not os.path.exists(self.data_dump_path):
+                os.makedirs(self.data_dump_path)
+
+            if not os.path.exists(self.sa_storage_path):
+                os.makedirs(self.sa_storage_path)
+
     def _init_param_setup(self) -> None:
         """
 
         Initializes the parameters by splitting these into the main groups.
 
         """
 
@@ -326,15 +368,15 @@
         )
         self._clean_sim_files_parallel_if_on: Callable[[], None] = (
             self._clean_sim_files_parallel if self.clean_finish else self.dummy_fun_noarg
         )
         self._clean_hdf_results_parallel_if_on: Callable[[], None] = (
             self._clean_hdf_results_parallel if not self.save_hdf_results else self.dummy_fun_noarg
         )
-        # self.print_init_info: Callable[[], None] = self._print_hdf_info
+        self._dump_results_if_on: Callable[[], None] = self._dump_results if self.dump_results else self.dummy_fun_noarg
 
     def _init_results(self) -> None:
         """
 
         Initializes an empty list for storing the hdf file results into.
 
         """
@@ -370,14 +412,17 @@
 
             # extract sensor arrays :
             self._extract_sensor_array_info(cfs_xml_content)
 
             # init file names :
             self._init_sa_file_names()
 
+    def _set_mesh_present_status(self, present: bool) -> None:
+        self.mesh_present = present
+
     # * ------------------ Execution methods ------------------
     def _forward_serial(self: "pyCFS", X: pyCFSparamVec) -> None:
         """
 
         Performs the forward pass over all data. Determines number of parameter
         combinations N. Allocates the result arrays and stores the results
         of the performed calculations.
@@ -586,25 +631,56 @@
             bool: Indicates if meshing should be performed.
         """
         return (self.params_changed[2] and (ind is None) and not self.mesh_present) or (
             self.remeshing_on and self.parallelize and not self.mesh_present
         )
 
     # * ------------------ Result handler methods ------------------
+    def _generate_data_dump_path(self) -> str:
+        t = time.ctime(time.time())
+        t = t.replace(" ", "_").replace(":", "-")
+        return f"{self.data_dump_path}data_dump_run_{t}.npy"
+
+    def _contruct_run_metadata(self, X: pyCFSparamVec) -> None:
+        file_paths = glob(f"{self.cfs_proj_path}/**/*.csv", recursive=True) + glob(
+            f"{self.cfs_proj_path}/**/*.py", recursive=True
+        )
+        other_files = {k: pyCFS.read_file_contents(k) for k in file_paths}
+        self.run_metadata = {
+            "xml_template": pyCFS.read_file_contents(self.cfs_file_init),
+            "mat_template": pyCFS.read_file_contents(self.mat_file_init),
+            "jou_template": pyCFS.read_file_contents(self.jou_file_init),
+            "other_files": other_files,
+            "X": X,
+            "run_start": self.time[LAST_EXEC_START],
+            "run_finish": self.time[LAST_EXEC_STOP],
+            "note": "",
+        }
+
+    def _dump_results(self) -> None:
+        result_packet = {
+            "results_hdf": self.results,
+            "results_sensor_array": self.sa_results,
+            "meta_data": self.run_metadata,
+        }
+
+        self.result_dump_path = self._generate_data_dump_path()
+        np.save(self.result_dump_path, result_packet, allow_pickle=True)  # type: ignore[arg-type]
+
     def _handle_sa_results(self, ind: Optional[int] = None) -> None:
 
         # init sa results :
         sa_results: sensorArrayResultPacket = {}
 
         # currently only handling the sensor array outputs :
         sa_file_names = self._make_sa_output_paths(ind, for_reading=True)
 
         # read sensor array outputs :
         for sa_file in sa_file_names:
-            name_parts = pyCFS._split_sa_result_name(sa_file)
+            name_parts = pyCFS._split_sa_result_name(sa_file, self.sa_storage_path)
             sa_results[name_parts[0]] = pyCFS._read_sa_result(sa_file)
 
         self.sa_results.append(sa_results)
 
     @staticmethod
     def _read_sa_result(sa_file: str) -> sensorArrayResult:
         # read the first line to acquire column names :
@@ -616,16 +692,16 @@
 
         # read the content :
         data = np.loadtxt(sa_file, dtype=np.float64, skiprows=1, delimiter=",")
 
         return {"data": data, "columns": col_names}
 
     @staticmethod
-    def _split_sa_result_name(res_name: str) -> List[str]:
-        res_name = res_name.removeprefix(SA_STORAGE_PATH)
+    def _split_sa_result_name(res_name: str, storage_path: str) -> List[str]:
+        res_name = res_name.removeprefix(storage_path)
         return res_name.split(SA_NAME_SEPARATOR)
 
     def _get_hdf_curr_package(self, ind: Optional[int] = None) -> nestedResultDict:
         """
 
         Gets the hdf package for the current simulation run by extracting all
         results from the hdf file for the result regions defined in the inital
@@ -913,15 +989,15 @@
     def _make_sa_output_paths(self, ind: Optional[int], for_reading: bool = False) -> List[str]:
 
         sarrays_output_paths = []
         ind_ext = "" if ind is None else f"{SA_NAME_SEPARATOR}{ind}"
         step_ext = "-1" if for_reading else ""
 
         for out_name in self.output_names:
-            sarrays_output_paths.append(f"{SA_STORAGE_PATH}{out_name}{ind_ext}.csv{step_ext}")
+            sarrays_output_paths.append(f"{self.sa_storage_path}{out_name}{ind_ext}.csv{step_ext}")
 
         return sarrays_output_paths
 
     def _fill_sensor_array_setup(self, xml_content: str, ind: Optional[int] = None) -> str:
 
         output_names = self._make_sa_output_paths(ind)
 
@@ -1176,14 +1252,82 @@
 
         return cfs_options
 
     def _get_console_output_options(self, ind: Optional[int] = None, is_sim: bool = True) -> str:
         run_name = "sim" if is_sim else "mesher"
         return f" >> ./logs/{run_name}_output.log" if ind is None else f" >> ./logs/{run_name}_output_{ind}.log"
 
+    # * ------------------ Time methods ------------------
+    def _record_time(self, time_id: str) -> None:
+        self.time[time_id] = time.ctime(time.time())
+
+    # * ------------------ Report methods ------------------
+    @staticmethod
+    def _print_one_line_box(
+        line_content: str = "", padding: bool = False, header: bool = False, n_times: int = 1, n_pads: int = 1
+    ) -> None:
+
+        pad = " " * n_pads if padding else ""
+        filler = INFO_BOX_CHAR if header else " "
+        padded_content = f"{pad}{line_content}{pad}"
+
+        for _ in range(n_times):
+            print(f"{INFO_BOX_CHAR}{padded_content:{filler}^{INFO_BOX_WIDTH - 2}}{INFO_BOX_CHAR}")
+
+    def _print_init_status_report(self) -> None:
+        pyCFS._print_one_line_box(header=True)
+        title = f"Project : {self.project_name}"
+        pyCFS._print_one_line_box(title, header=True, padding=True, n_pads=10)
+        pyCFS._print_one_line_box(header=True)
+        pyCFS._print_one_line_box(n_times=2)
+
+        init_time = self.time["init_time"]
+        pyCFS._print_one_line_box(f"Init at : {init_time}", padding=True)
+        pyCFS._print_one_line_box()
+        pyCFS._print_one_line_box(f"- Number of parameters : {self.n_params}", padding=True)
+        pyCFS._print_one_line_box()
+        pyCFS._print_one_line_box(f"- CFS parameters : {self.n_cfs_params}", padding=True)
+        p_names = ", ".join(self.cfs_params_names)
+        pyCFS._print_one_line_box(f"[{p_names}]", padding=True)
+        pyCFS._print_one_line_box()
+        pyCFS._print_one_line_box(f"- MAT parameters : {self.n_mat_params}", padding=True)
+        p_names = ", ".join(self.mat_params_names)
+        pyCFS._print_one_line_box(f"[{p_names}]", padding=True)
+        pyCFS._print_one_line_box()
+        pyCFS._print_one_line_box(f"- JOU parameters : {self.n_trelis_params}", padding=True)
+        p_names = ", ".join(self.trelis_params_names)
+        pyCFS._print_one_line_box(f"[{p_names}]", padding=True)
+        pyCFS._print_one_line_box()
+        pyCFS._print_one_line_box(f"- Tracked results : {self.track_results}", padding=True)
+        pyCFS._print_one_line_box(f"- Parallelize : {self.parallelize}", padding=True)
+        pyCFS._print_one_line_box(f"- Remeshing on : {self.remeshing_on}", padding=True)
+
+        pyCFS._print_one_line_box(n_times=2)
+        pyCFS._print_one_line_box(header=True)
+
+    def _print_run_status_report(self) -> None:
+        pyCFS._print_one_line_box(header=True)
+        title = f"Run report : {self.project_name}"
+        pyCFS._print_one_line_box(title, header=True, padding=True, n_pads=10)
+        pyCFS._print_one_line_box(header=True)
+        pyCFS._print_one_line_box(n_times=2)
+
+        pyCFS._print_one_line_box(f" Start at : {self.time[LAST_EXEC_START]}", padding=True)
+        pyCFS._print_one_line_box(f"Finish at : {self.time[LAST_EXEC_STOP]}", padding=True)
+
+        pyCFS._print_one_line_box(n_times=2)
+        pyCFS._print_one_line_box(f"- Total runs : {self.N}", padding=True)
+        pyCFS._print_one_line_box()
+        pyCFS._print_one_line_box(f"- Data dumped : {self.dump_results}", padding=True)
+        if self.dump_results:
+            pyCFS._print_one_line_box(f"@ : {self.result_dump_path}", padding=True)
+
+        pyCFS._print_one_line_box(n_times=2)
+        pyCFS._print_one_line_box(header=True)
+
     # * ------------------ I/O methods ------------------
     @staticmethod
     def read_file_contents(file_path: str) -> str:
 
         file = open(file_path, "r")
         contents = file.read()
         file.close()
```

### Comparing `pyCFS-0.0.4/pyCFS/util/hdf5_io.py` & `pyCFS-0.0.5/pyCFS/util/hdf5_io.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS/util/lib_types.py` & `pyCFS-0.0.5/pyCFS/util/lib_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,32 @@
 class sensorArrayResult(TypedDict):
     data: resultVec
     columns: List[str]
 
 
 sensorArrayResultPacket = Dict[str, sensorArrayResult]
 
+
+class runMetaData(TypedDict):
+    xml_template: str
+    mat_template: str
+    jou_template: str
+    other_files: Dict[str, str]
+    X: pyCFSparamVec
+    run_start: str
+    run_finish: str
+    note: str
+
+
+class resultDump(TypedDict):
+    results_hdf: List[nestedResultDict]
+    results_sensor_array: List[sensorArrayResultPacket]
+    meta_data: runMetaData
+
+
 __all__ = [
     "pyCFSparam",
     "pyCFSparamVec",
     "resultVec",
     "resultDict",
     "nestedResultDict",
     "sensorArrayResult",
```

### Comparing `pyCFS-0.0.4/pyCFS/util/setup_generator.py` & `pyCFS-0.0.5/pyCFS/util/setup_generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import os
 import shutil
+import numpy as np
 from typing import List
 from tap import Tap
 from typing import TypeAlias
 
 
 class pyCFSParser(Tap):
-    setup_type: str  # Which setup to generate. ('newsim' or 'newopti')
+    setup_type: str  # Which setup to generate. ('newsim', 'newopti', 'extract-snapshot')
     simulation_name: str = "my_simulation"  # Simulation name to be used.
+    source_path: str = "./"  # Path to the source file (for snapshot extraction).
     config_file: str = "config.yaml"  # Name of yaml config file to use.
     cfs_path: str = "CFS_PATH"  # Path to OpenCFS on your system.
     mesher_alias: str = "MESHER_ALIAS"  # Path to mesher.
     opt: bool = False  # Flag to decide if sim or opt setup.
 
+    def configure(self) -> None:
+        self.add_argument("setup_type")
+        self.add_argument("-n", "--simulation_name")
+        self.add_argument("-s", "--source_path")
+
 
 pyCFSParserArgs: TypeAlias = pyCFSParser
 
 # Consts def :
 TEMPLATES_DIR_NAME = "templates"
 MAIN_XML_TEMPLATE_PATH = __file__[:-18] + "templates/sim.xml"
 MAT_XML_TEMPLATE_PATH = __file__[:-18] + "templates/mat.xml"
@@ -31,14 +38,21 @@
 OPTIMIZATION_DIR_NAME = "optimization"
 
 PROJECT_NAME_TOKEN = "PROJECT_NAME"
 CFS_PATH_TOKEN = "CFS_PATH"
 MESHER_ALIAS_TOKEN = "MESHER_ALIAS"
 
 
+def write_file_contents(file_path: str, contents: str) -> None:
+
+    file = open(file_path, "w")
+    file.write(contents)
+    file.close()
+
+
 def generate(args: pyCFSParserArgs) -> None:
     generators = {
         "newsim": sim_setup_generator,
         "newopti": opti_setup_generator,
     }
 
     generators[args.setup_type](args)
@@ -103,15 +117,52 @@
 
 def generate_dirs(dir_paths: List[str]) -> None:
     for path in dir_paths:
         if not os.path.exists(path):
             os.mkdir(path)
 
 
+def extract_snapshot(args: pyCFSParserArgs) -> None:
+    snapshot_path = args.source_path
+    extraction_path = args.simulation_name
+
+    snapshot = np.load(snapshot_path, allow_pickle=True)[()]
+
+    # extract infos :
+    sim_name = extraction_path.split("/")[-1]
+    extraction_path += "/" if extraction_path[-1] != "/" else ""
+    templates_path = f"{extraction_path}/templates/"
+
+    # generate directories :
+    if os.path.exists(extraction_path):
+        raise FileExistsError(
+            "The given path already exists - aborting extraction \
+                              files might get overwritten!"
+        )
+    else:
+        os.makedirs(templates_path)
+
+        write_file_contents(f"{templates_path}{sim_name}_init.xml", snapshot["meta_data"]["xml_template"])
+        write_file_contents(f"{templates_path}mat_init.xml", snapshot["meta_data"]["mat_template"])
+        write_file_contents(f"{templates_path}{sim_name}_init.jou", snapshot["meta_data"]["jou_template"])
+
+        for file, content in snapshot["meta_data"]["other_files"].items():
+            f_path = file.replace("./", extraction_path)
+            f_path_parts = f_path.split("/")
+            f_path_parts.pop(-1)
+            f_dir_path = "/".join(f_path_parts) + "/"
+
+            if not os.path.exists(f_dir_path):
+                os.makedirs(f_dir_path)
+
+            if not os.path.exists(f_path):
+                write_file_contents(f_path, content)
+
+
 def main() -> None:
 
     # make functions dict
-    functions = {"newsim": generate, "newopti": generate}
+    functions = {"newsim": generate, "newopti": generate, "extract-snapshot": extract_snapshot}
 
     args = pyCFSParser().parse_args()
 
     functions[args.setup_type](args)
```

### Comparing `pyCFS-0.0.4/pyCFS/util/templates/config.yaml` & `pyCFS-0.0.5/pyCFS/util/templates/config.yaml`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS/util/templates/sim_setup.py` & `pyCFS-0.0.5/pyCFS/util/templates/sim_setup.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS/util/templates/sim_setup_opti.py` & `pyCFS-0.0.5/pyCFS/util/templates/sim_setup_opti.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/pyCFS.egg-info/PKG-INFO` & `pyCFS-0.0.5/pyCFS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCFS
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library for automating and data handling tasks for openCFS.
 Author-email: IGTE <igte.gitlab@gmail.com>, Eniz Mušeljić <eniz.m@outlook.com>, Andreas Wurzinger <andreas.wurzinger@tugraz.at>
 License: MIT License
         
         Copyright (c) 2024 Verein zur Förderung der Software openCFS
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyCFS-0.0.4/pyCFS.egg-info/SOURCES.txt` & `pyCFS-0.0.5/pyCFS.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -2,26 +2,34 @@
 .gitlab-ci.yml
 Changelog.md
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+.gitlab/issue_templates/Default.md
+.gitlab/merge_request_templates/Default.md
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/dev_notes.md
+docs/source/getting_started.md
 docs/source/index.rst
 docs/source/installation.md
 docs/source/pycfs_data.md
 docs/source/_static/pycfslogo-full-no-text-small.png
 docs/source/_static/pycfslogo-full-no-text.png
 docs/source/dev_source/conventions.md
 docs/source/dev_source/data_handling.md
 docs/source/dev_source/dev_notes_main.md
+docs/source/examples/basics/a_first_simulation.md
+docs/source/examples/basics/cli_tool.md
+docs/source/examples/basics/data_processing.md
+docs/source/examples/basics/introduction.md
+docs/source/examples/basics/result_handling.md
 pyCFS/__init__.py
 pyCFS/py.typed
 pyCFS/pyCFS.py
 pyCFS.egg-info/PKG-INFO
 pyCFS.egg-info/SOURCES.txt
 pyCFS.egg-info/dependency_links.txt
 pyCFS.egg-info/entry_points.txt
@@ -48,15 +56,14 @@
 pyCFS/data/io/__init__.py
 pyCFS/data/io/cfs_types.py
 pyCFS/data/operators/__init__.py
 pyCFS/data/operators/fit_geometry.py
 pyCFS/data/operators/interpolators.py
 pyCFS/data/operators/projection_interpolation.py
 pyCFS/util/__init__.py
-pyCFS/util/cli_handler.py
 pyCFS/util/hdf5_io.py
 pyCFS/util/lib_types.py
 pyCFS/util/setup_generator.py
 pyCFS/util/templates/config.yaml
 pyCFS/util/templates/mat.xml
 pyCFS/util/templates/run_sim.py
 pyCFS/util/templates/sim.jou
@@ -87,14 +94,15 @@
 tests/data/extras/nihu_io/result_field.mat
 tests/data/extras/nihu_io/result_surface.mat
 tests/data/extras/psv_io/line.npy
 tests/data/extras/psv_io/line.svd
 tests/data/extras/psv_io/line_h2_accelerance.unv
 tests/data/extras/psv_io/surface.svd
 tests/data/extras/psv_io/surface_dist.npy
+tests/data/extras/psv_io/surface_h1_receptance.npy
 tests/data/extras/psv_io/surface_h1_receptance.unv
 tests/data/operators/fit_geometry/fit_geometry_src.cfs
 tests/data/operators/fit_geometry/fit_geometry_target.cfs
 tests/data/operators/interpolators/interpolators.cfs
 tests/data/operators/interpolators/nn_elem.cfs
 tests/data/operators/interpolators/nn_source.cfs
 tests/data/operators/interpolators/nn_target.cfs
```

### Comparing `pyCFS-0.0.4/pyproject.toml` & `pyCFS-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/ansys_io/ansys_io.rst` & `pyCFS-0.0.5/tests/data/extras/ansys_io/ansys_io.rst`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/ensight_io/ensight_io.0000.U` & `pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.U`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/ensight_io/ensight_io.0000.mesh` & `pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.mesh`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/ensight_io/ensight_io.0000.p` & `pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.p`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/ensight_io/poly/data.case` & `pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data.case`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/ensight_io/poly/data00001.geo` & `pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.geo`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/ensight_io/poly/data00001.scl1` & `pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.scl1`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/ensight_io/poly/data00001.vel` & `pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.vel`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/nihu_io/result_field.mat` & `pyCFS-0.0.5/tests/data/extras/nihu_io/result_field.mat`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/nihu_io/result_surface.mat` & `pyCFS-0.0.5/tests/data/extras/nihu_io/result_surface.mat`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/psv_io/line.npy` & `pyCFS-0.0.5/tests/data/extras/psv_io/line.npy`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/psv_io/line.svd` & `pyCFS-0.0.5/tests/data/extras/psv_io/line.svd`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/psv_io/line_h2_accelerance.unv` & `pyCFS-0.0.5/tests/data/extras/psv_io/line_h2_accelerance.unv`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/psv_io/surface.svd` & `pyCFS-0.0.5/tests/data/extras/psv_io/surface.svd`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/psv_io/surface_dist.npy` & `pyCFS-0.0.5/tests/data/extras/psv_io/surface_dist.npy`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/extras/psv_io/surface_h1_receptance.unv` & `pyCFS-0.0.5/tests/data/extras/psv_io/surface_h1_receptance.unv`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/operators/fit_geometry/fit_geometry_src.cfs` & `pyCFS-0.0.5/tests/data/operators/fit_geometry/fit_geometry_src.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/operators/fit_geometry/fit_geometry_target.cfs` & `pyCFS-0.0.5/tests/data/operators/fit_geometry/fit_geometry_target.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/operators/interpolators/interpolators.cfs` & `pyCFS-0.0.5/tests/data/operators/interpolators/interpolators.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/operators/interpolators/nn_elem.cfs` & `pyCFS-0.0.5/tests/data/operators/interpolators/nn_elem.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/operators/interpolators/nn_source.cfs` & `pyCFS-0.0.5/tests/data/operators/interpolators/nn_source.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/operators/interpolators/nn_target.cfs` & `pyCFS-0.0.5/tests/data/operators/interpolators/nn_target.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/operators/projection_interpolation/source.cfs` & `pyCFS-0.0.5/tests/data/operators/projection_interpolation/source.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/operators/projection_interpolation/target.cfs` & `pyCFS-0.0.5/tests/data/operators/projection_interpolation/target.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/data/sim_io/elecFieldIntensity-sensor-positions-0.csv-1` & `pyCFS-0.0.5/tests/data/sim_io/elecFieldIntensity-sensor-positions-0.csv-1`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/pycfs_data_fixtures.py` & `pyCFS-0.0.5/tests/pycfs_data_fixtures.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/pycfs_fixtures.py` & `pyCFS-0.0.5/tests/pycfs_fixtures.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/test_pycfs_core.py` & `pyCFS-0.0.5/tests/test_pycfs_core.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/test_pycfs_data_extras.py` & `pyCFS-0.0.5/tests/test_pycfs_data_extras.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import importlib.util
 import time
 
 import numpy as np
 import pytest
-import importlib
 
 from pyCFS.data import v_def
 from pyCFS.data.extras import ensight_io, nihu_io, psv_io
 from pyCFS.data.extras.vtk_to_cfs_element_types import vtk_to_cfs_elem_type
 from pyCFS.data.io import mesh_from_coordinates_connectivity, CFSResultData, cfs_types, CFSWriter, CFSResultInfo
 from pyCFS.data.util import list_search
 
@@ -48,14 +47,15 @@
     meshData.drop_unused_nodes_elements(regData_keep)
 
     # Create Result
     with CFSWriter(filename_out) as h5writer:
         h5writer.create_file(mesh_data=meshData, result_data=result_data)
 
 
+@pytest.mark.skipif(importlib.util.find_spec("vtk") is None, reason="requires vtk>=9.3.0")
 def test_ensight_read(working_directory="."):
     file = f"{working_directory}/tests/data/extras/ensight_io/ensight_io.case"
     step = 2
     quantity = "U"
 
     filename_cfs = f"{working_directory}/tests/data_tmp/extras/ensight_io/ensight_io.cfs"
 
@@ -88,14 +88,15 @@
         dim_names=["x", "y", "z"],
     )
 
     with CFSWriter(filename_cfs) as writer:
         writer.create_file(mesh_data=mesh, result_data=result)
 
 
+@pytest.mark.skipif(importlib.util.find_spec("vtk") is None, reason="requires vtk>=9.3.0")
 def test_ensight_read_poly(working_directory="."):
     file = f"{working_directory}/tests/data/extras/ensight_io/poly/data.case"
     quantities = ["pressure", "velocity"]
     regions = {"rigid": 1}
 
     filename_cfs = f"{working_directory}/tests/data_tmp/extras/ensight_io/poly/data.cfs"
 
@@ -133,32 +134,36 @@
 
     with CFSWriter(file_out) as h5writer:
         h5writer.create_file(mesh_data=mesh_write, result_data=result_write)
 
 
 @pytest.fixture
 def psv_frf_data_obj(working_directory="."):
+    frf_data = np.load(
+        f"{working_directory}/tests/data/extras/psv_io/surface_h1_receptance.npy", allow_pickle=True
+    ).item()
+
+    return frf_data
+
+
+def test_psv_read(psv_frf_data_obj, working_directory="."):
     filename = f"{working_directory}/tests/data/extras/psv_io/surface_h1_receptance.unv"
     distfile = f"{working_directory}/tests/data/extras/psv_io/surface_dist.npy"
 
     frf_data = psv_io.read_frf(
         file_path=filename,
         frf_form="receptance",
         frf_type="H1",
         ref_channel=1,
         read_coordinates=True,
         read_elements=True,
         dist_file=distfile,
     )
 
-    return frf_data
-
-
-def test_psv_read(psv_frf_data_obj):
-    pass
+    np.testing.assert_equal(psv_frf_data_obj, frf_data)
 
 
 def test_psv_interpolate(psv_frf_data_obj):
     node_ids_interpolate = [10, 15]
     frf_data_interpolated = psv_io.interpolate_data_points(
         frf_data=psv_frf_data_obj, nodes_interpolate=node_ids_interpolate
     )
```

### Comparing `pyCFS-0.0.4/tests/test_pycfs_data_io.py` & `pyCFS-0.0.5/tests/test_pycfs_data_io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Module containing data processing utilities for writing HDF5 files in openCFS format
 """
 
+import copy
 from copy import deepcopy
 
 import h5py
 import numpy as np
 from pyCFS.data import io, v_def
+from pyCFS.data.io.cfs_types import cfs_analysis_type
 from .pycfs_data_fixtures import dummy_CFSMeshData_obj, dummy_CFSResultData_obj
 
 
 def test_CFSMeshData(dummy_CFSMeshData_obj):
 
     print(dummy_CFSMeshData_obj.Quality)
 
@@ -26,14 +28,30 @@
     file = f"{working_directory}/tests/data_tmp/pycfs_data_io.cfs"
 
     print("Write demo file")
     with io.CFSWriter(file, verbosity=v_def.all) as h5writer:
         h5writer.create_file(mesh_data=dummy_CFSMeshData_obj, result_data=dummy_CFSResultData_obj)
 
 
+def test_read_write_multistep2(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory="."):
+    file = f"{working_directory}/tests/data_tmp/pycfs_data_io.cfs"
+
+    test_write(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory)
+
+    dummy_CFSResultData_obj2 = copy.deepcopy(dummy_CFSResultData_obj)
+    dummy_CFSResultData_obj2.MultiStepID = 2
+    dummy_CFSResultData_obj2.AnalysisType = cfs_analysis_type.HARMONIC
+
+    with io.CFSWriter(file, verbosity=v_def.all) as h5writer:
+        h5writer.write_multistep(result_data=dummy_CFSResultData_obj2, multi_step_id=2)
+
+    with io.CFSReader(file, multistep_id=2, verbosity=v_def.all) as h5reader:
+        np.testing.assert_equal(h5reader.MultiStepData, dummy_CFSResultData_obj2)
+
+
 def test_read_mesh(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory="."):
     file = f"{working_directory}/tests/data_tmp/pycfs_data_io.cfs"
 
     test_write(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory)
 
     print("Read demo file")
     with io.CFSReader(file, verbosity=v_def.all) as h5reader:
@@ -46,41 +64,41 @@
         # Check Read Mesh Data
         print("Check Written/Read Mesh")
         print(f" - Mesh Info: {dummy_CFSMeshData_obj.MeshInfo == mesh_data_read.MeshInfo}")
         print(f" - Mesh Data: {dummy_CFSMeshData_obj == mesh_data_read}")
         for reg_read in reg_info_read:
             print(f" - Region {reg_read.Name}: {reg_read in dummy_CFSMeshData_obj.Regions}")
 
-        assert dummy_CFSMeshData_obj == mesh_data_read
+        np.testing.assert_equal(dummy_CFSMeshData_obj, mesh_data_read)
 
 
 def test_read_data(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory="."):
     file = f"{working_directory}/tests/data_tmp/pycfs_data_io.cfs"
 
     test_write(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory)
 
     print("Read demo file")
     with io.CFSReader(file, verbosity=v_def.all) as h5reader:
         # Read Mesh
         print("Read Demo Mesh")
         mesh_data_read = h5reader.MeshData
 
         # Read Data
-        assert h5reader.MultiStepData == dummy_CFSResultData_obj
+        np.testing.assert_equal(h5reader.MultiStepData, dummy_CFSResultData_obj)
 
         node_id = h5reader.get_closest_node(coordinate=np.array([[0.1, 0, 0], [0, 0, 1]]), region="Vol")
-        assert np.all(
-            mesh_data_read.get_closest_node(coordinate=np.array([[0.1, 0, 0], [0, 0, 1]]), region="Vol") == node_id
+        np.testing.assert_equal(
+            mesh_data_read.get_closest_node(coordinate=np.array([[0.1, 0, 0], [0, 0, 1]]), region="Vol"), node_id
         )
         result_data_1 = [
             h5reader.get_single_data_steps(quantity="quantity", region="Vol", entity_id=node_id[i]) for i in node_id
         ]
         el_id = h5reader.get_closest_element(coordinate=np.array([[1, 1, 1], [0, 0, 0]]), region="Surf1")
-        assert np.all(
-            mesh_data_read.get_closest_element(coordinate=np.array([[1, 1, 1], [0, 0, 0]]), region="Surf1") == el_id
+        np.testing.assert_equal(
+            mesh_data_read.get_closest_element(coordinate=np.array([[1, 1, 1], [0, 0, 0]]), region="Surf1"), el_id
         )
         result_data_1_3 = [
             h5reader.get_single_data_steps(quantity="quantity3", region="Surf1", entity_id=el_id[i]) for i in el_id
         ]
 
 
 def test_read_group_wo_elements(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory="."):
@@ -98,14 +116,26 @@
     with io.CFSReader(file, verbosity=v_def.all) as h5reader:
         mesh_data_read = h5reader.MeshData
         result_data_read = h5reader.MultiStepData
 
     test_write(mesh_data_read, result_data_read, working_directory)
 
 
+def test_sort_result_data(dummy_CFSResultData_obj):
+    # Write unsorted StepValues
+    step_values = dummy_CFSResultData_obj.StepValues
+    unsort_idx = np.arange(start=len(step_values) - 1, stop=-1, step=-1)
+    step_values = step_values[unsort_idx]
+    dummy_CFSResultData_obj.StepValues = step_values
+
+    # Sort ResultData by StepValues
+    sort_idx = dummy_CFSResultData_obj.sort_steps(return_idx=True)
+    np.testing.assert_array_equal(sort_idx, unsort_idx)
+
+
 def test_reorient(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory="."):
     file = f"{working_directory}/tests/data_tmp/pycfs_data_io.cfs"
 
     dummy_CFSMeshData_obj.reorient_region("Surf1")
     dummy_CFSMeshData_obj.reorient_region("Surf2")
     with io.CFSWriter(file, verbosity=v_def.all) as h5writer:
         h5writer.create_file(mesh_data=dummy_CFSMeshData_obj, result_data=dummy_CFSResultData_obj)
```

### Comparing `pyCFS-0.0.4/tests/test_pycfs_data_operators.py` & `pyCFS-0.0.5/tests/test_pycfs_data_operators.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from pyCFS.data.io import CFSReader, cfs_types, CFSWriter
-from pyCFS.data.io.cfs_types import cfs_result_type
+from pyCFS.data.io import CFSReader, cfs_types, CFSWriter, CFSResultData
 from pyCFS.data.operators import interpolators
 
 
 def test_fit_coordinates(working_directory="."):
     from pyCFS.data.operators.fit_geometry import fit_coordinates
 
     filename_src = f"{working_directory}/tests/data/operators/fit_geometry/fit_geometry_src.cfs"
@@ -39,38 +38,34 @@
         mesh_data = h5r.MeshData
         result_data_read = h5r.MultiStepData
 
         reg_coord = h5r.get_mesh_region_coordinates(reg_name)
         reg_conn = h5r.get_mesh_region_connectivity(reg_name)
 
     m_interp = interpolators.interpolation_matrix_node_to_cell(reg_coord, reg_conn)
-    result_data_N2C = interpolators.apply_interpolation(
-        result_data_read,
-        m_interp,
-        quantity,
-        reg_name,
-        cfs_types.cfs_result_type.NODE,
-        cfs_types.cfs_result_type.ELEMENT,
+    r_array = result_data_read.get_data_array(quantity, reg_name, cfs_types.cfs_result_type.NODE)
+    r_array_N2C = interpolators.apply_interpolation(
+        result_array=r_array,
+        interpolation_matrix=m_interp,
+        restype_out=cfs_types.cfs_result_type.ELEMENT,
         quantity_out="quantity_N2C",
     )
 
     m_interp = interpolators.interpolation_matrix_cell_to_node(reg_coord, reg_conn).tocsr()
 
-    result_data_C2N = interpolators.apply_interpolation(
-        result_data_N2C,
-        m_interp,
-        "quantity_N2C",
-        reg_name,
-        cfs_types.cfs_result_type.ELEMENT,
-        cfs_types.cfs_result_type.NODE,
+    r_array_C2N = interpolators.apply_interpolation(
+        result_array=r_array_N2C,
+        interpolation_matrix=m_interp,
+        restype_out=cfs_types.cfs_result_type.NODE,
         quantity_out="quantity_C2N",
     )
 
-    result_data_write = result_data_N2C
-    result_data_write.combine_with(result_data_C2N)
+    result_data_write = CFSResultData(
+        analysis_type=cfs_types.cfs_analysis_type.TRANSIENT, data=[r_array_C2N, r_array_N2C]
+    )
 
     with CFSWriter(file_out) as h5w:
         h5w.create_file(mesh_data, result_data_write)
 
 
 def test_interpolators_nearest_neighbor_elem(working_directory="."):
     # TODO Unit test for Nearest Neighbor interpolation
@@ -85,48 +80,47 @@
     with CFSReader(source_file) as h5r:
         result_data_src = h5r.MultiStepData
         mesh_data_src = h5r.MeshData
 
     with CFSReader(source_file) as h5r:
         mesh_data = h5r.MeshData
 
-    result_data_nn = []
+    result_array_lst_nn = []
     for src_region_name in region_src_target_dict:
         source_coord = mesh_data_src.get_region_centroids(src_region_name)
 
         target_coord = []
         for reg_name in region_src_target_dict[src_region_name]:
             target_coord.append(mesh_data.get_region_centroids(reg_name))
 
         for i, reg_name in enumerate(region_src_target_dict[src_region_name]):
             m_interp = interpolators.interpolation_matrix_nearest_neighbor(
                 source_coord,
                 target_coord[i],
                 num_neighbors=1,
                 interpolation_exp=1,
                 max_distance=1e-6,
+                formulation="forward",
+            )
+            m_interp = interpolators.interpolation_matrix_nearest_neighbor(
+                source_coord, target_coord[i], num_neighbors=1, max_distance=1e-6, formulation="backward"
             )
-            m_interp = interpolators.interpolation_matrix_nearest_neighbor_inverse(
-                source_coord, target_coord[i], num_neighbors=1, max_distance=1e-6
+            result_array_src = result_data_src.get_data_array(
+                quantity=quantity, region=src_region_name, restype=cfs_types.cfs_result_type.ELEMENT
             )
-            result_data_nn.append(
+            result_array_lst_nn.append(
                 interpolators.apply_interpolation(
-                    result_data_src,
-                    m_interp,
-                    quantity=quantity,
-                    region=src_region_name,
+                    result_array=result_array_src,
+                    interpolation_matrix=m_interp,
                     region_out=reg_name,
-                    restype=cfs_result_type.ELEMENT,
-                    restype_out=cfs_result_type.ELEMENT,
+                    restype_out=cfs_types.cfs_result_type.ELEMENT,
                 )
             )
 
-    result_data_disp = result_data_nn[0]
-    for i in range(1, len(result_data_nn)):
-        result_data_disp.combine_with(result_data_nn[i])
+    result_data_disp = CFSResultData(analysis_type=cfs_types.cfs_analysis_type.TRANSIENT, data=result_array_lst_nn)
 
     with CFSWriter(interpolated_sim) as h5w:
         h5w.create_file(mesh_data, result_data_disp)
 
 
 def test_interpolators_nearest_neighbor_node(working_directory="."):
     # NN Example
@@ -144,54 +138,48 @@
 
     with CFSReader(target_file) as h5r:
         mesh_data = h5r.MeshData
         target_coord = []
         for reg_name in reg_name_target:
             target_coord.append(h5r.get_mesh_region_coordinates(reg_name))
 
-    result_data_nn = []
-    result_data_nn_inverse = []
+    result_array_lst_nn = []
+    result_array_lst_nn_inverse = []
     for i, reg_name in enumerate(reg_name_target):
         m_interp = interpolators.interpolation_matrix_nearest_neighbor(
             source_coord, target_coord[i], num_neighbors=10, interpolation_exp=2
         )
-        m_interp_inverse = interpolators.interpolation_matrix_nearest_neighbor_inverse(
-            source_coord, target_coord[i], num_neighbors=10, interpolation_exp=2
+        m_interp_inverse = interpolators.interpolation_matrix_nearest_neighbor(
+            source_coord, target_coord[i], num_neighbors=10, interpolation_exp=2, formulation="backward"
         )
-        result_data_nn.append(
+        result_array_src = result_data_src.get_data_array(
+            quantity=quantity, region=reg_name_source, restype=cfs_types.cfs_result_type.NODE
+        )
+        result_array_lst_nn.append(
             interpolators.apply_interpolation(
-                result_data_src,
-                m_interp,
-                quantity=quantity,
+                result_array=result_array_src,
+                interpolation_matrix=m_interp,
                 quantity_out=f"{quantity}_interpolated",
-                region=reg_name_source,
                 region_out=reg_name,
-                restype=cfs_result_type.NODE,
-                restype_out=cfs_result_type.NODE,
+                restype_out=cfs_types.cfs_result_type.NODE,
             )
         )
-        result_data_nn_inverse.append(
+        result_array_lst_nn_inverse.append(
             interpolators.apply_interpolation(
-                result_data_src,
-                m_interp_inverse,
-                quantity=quantity,
+                result_array=result_array_src,
+                interpolation_matrix=m_interp_inverse,
                 quantity_out=f"{quantity}_interpolated_inverse",
-                region=reg_name_source,
                 region_out=reg_name,
-                restype=cfs_result_type.NODE,
-                restype_out=cfs_result_type.NODE,
+                restype_out=cfs_types.cfs_result_type.NODE,
             )
         )
 
-    result_data_write = result_data_nn[0]
-    for i in range(1, len(result_data_nn)):
-        result_data_write.combine_with(result_data_nn[i])
-
-    for i in range(len(result_data_nn_inverse)):
-        result_data_write.combine_with(result_data_nn_inverse[i])
+    result_data_write = CFSResultData(
+        cfs_types.cfs_analysis_type.TRANSIENT, data=result_array_lst_nn + result_array_lst_nn_inverse
+    )
 
     with CFSWriter(out_file) as h5w:
         h5w.create_file(mesh_data=mesh_data, result_data=result_data_write)
 
 
 def test_projection_interpolation(working_directory="."):
     from pyCFS.data.operators.projection_interpolation import interpolate_region
```

### Comparing `pyCFS-0.0.4/tests/test_pycfs_data_util.py` & `pyCFS-0.0.5/tests/test_pycfs_data_util.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.4/tests/test_pycfs_sim_io.py` & `pyCFS-0.0.5/tests/test_pycfs_sim_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def test_read_sa_result(sensor_array_result_file):
     sa_result = pyCFS._read_sa_result(sensor_array_result_file["file"])
     assert sa_result["columns"] == sensor_array_result_file["columns"]
     assert np.all(sa_result["data"] == sensor_array_result_file["data"])
 
 
 def test_split_sa_result_name(sensor_array_result_file):
-    name_split = pyCFS._split_sa_result_name(sensor_array_result_file["file"])
+    name_split = pyCFS._split_sa_result_name(sensor_array_result_file["file"], "")
     assert name_split == sensor_array_result_file["file_split"]
 
 
 def test_is_coord_col():
     assert pyCFS._is_coord_col("origElemNum") == True
     assert pyCFS._is_coord_col("globCoord-x") == True
     assert pyCFS._is_coord_col("globCoord-y") == True
```

