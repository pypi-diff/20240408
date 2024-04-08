# Comparing `tmp/erlab-1.6.5.tar.gz` & `tmp/erlab-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-1.6.5.tar", last modified: Wed Apr  3 08:40:33 2024, max compression
+gzip compressed data, was "erlab-2.0.0.tar", last modified: Mon Apr  8 13:43:45 2024, max compression
```

## Comparing `erlab-1.6.5.tar` & `erlab-2.0.0.tar`

### file list

```diff
@@ -1,161 +1,170 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.764332 erlab-1.6.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.724332 erlab-1.6.5/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.732332 erlab-1.6.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-03 08:40:28.000000 erlab-1.6.5/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-03 08:40:28.000000 erlab-1.6.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.732332 erlab-1.6.5/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-03 08:40:28.000000 erlab-1.6.5/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-03 08:40:28.000000 erlab-1.6.5/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-03 08:40:28.000000 erlab-1.6.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-03 08:40:28.000000 erlab-1.6.5/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      796 2024-04-03 08:40:28.000000 erlab-1.6.5/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)    97287 2024-04-03 08:40:30.000000 erlab-1.6.5/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-03 08:40:28.000000 erlab-1.6.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    46708 2024-04-03 08:40:33.764332 erlab-1.6.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-03 08:40:28.000000 erlab-1.6.5/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     4414 2024-04-03 08:40:28.000000 erlab-1.6.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.732332 erlab-1.6.5/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      752 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      540 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.736332 erlab-1.6.5/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    10762 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    13410 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/development.rst
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/erlab.characterization.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     2888 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.744332 erlab-1.6.5/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     2497 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.744332 erlab-1.6.5/docs/source/notebooks/
--rw-r--r--   0 root         (0) root         (0)   189769 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/notebooks/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)     1582 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/notebooks/io.ipynb
--rw-r--r--   0 root         (0) root         (0)   379528 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/notebooks/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    15761 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/notebooks/plotting.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.744332 erlab-1.6.5/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2579 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/refs.bib
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-03 08:40:28.000000 erlab-1.6.5/docs/source/userguide.rst
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-03 08:40:28.000000 erlab-1.6.5/environment.yml
--rw-r--r--   0 root         (0) root         (0)      990 2024-04-03 08:40:28.000000 erlab-1.6.5/environment_apple.yml
--rw-r--r--   0 root         (0) root         (0)      876 2024-04-03 08:40:28.000000 erlab-1.6.5/environment_nogit.yml
--rw-r--r--   0 root         (0) root         (0)      848 2024-04-03 08:40:28.000000 erlab-1.6.5/environment_nogit_mkl.yml
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-03 08:40:28.000000 erlab-1.6.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      334 2024-04-03 08:40:28.000000 erlab-1.6.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 08:40:33.764332 erlab-1.6.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.728332 erlab-1.6.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.748332 erlab-1.6.5/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-03 08:40:30.000000 erlab-1.6.5/src/erlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35539 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/accessors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.748332 erlab-1.6.5/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      748 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.752332 erlab-1.6.5/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      459 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.752332 erlab-1.6.5/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      812 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8766 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     6026 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    10689 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    13862 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10344 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.752332 erlab-1.6.5/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     2768 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7810 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     8332 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.752332 erlab-1.6.5/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)     2115 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.756332 erlab-1.6.5/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      601 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13943 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    20820 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    22076 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    19528 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)     9458 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/exampledata.py
--rw-r--r--   0 root         (0) root         (0)    19072 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.756332 erlab-1.6.5/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19391 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.756332 erlab-1.6.5/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52076 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114751 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27081 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    53776 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    11483 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    23195 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    16658 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     3341 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    52417 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.756332 erlab-1.6.5/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     1937 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30047 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6780 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.760332 erlab-1.6.5/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3674 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     7448 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7745 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     5630 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.760332 erlab-1.6.5/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.764332 erlab-1.6.5/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     1857 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29010 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18275 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4294 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    32411 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    30998 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.764332 erlab-1.6.5/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-03 08:40:28.000000 erlab-1.6.5/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.764332 erlab-1.6.5/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    46708 2024-04-03 08:40:33.000000 erlab-1.6.5/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4265 2024-04-03 08:40:33.000000 erlab-1.6.5/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:40:33.000000 erlab-1.6.5/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      321 2024-04-03 08:40:33.000000 erlab-1.6.5/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-03 08:40:33.000000 erlab-1.6.5/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:40:33.764332 erlab-1.6.5/tests/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-03 08:40:28.000000 erlab-1.6.5/tests/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-03 08:40:28.000000 erlab-1.6.5/tests/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2419 2024-04-03 08:40:28.000000 erlab-1.6.5/tests/test_kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.578651 erlab-2.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.538651 erlab-2.0.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.542651 erlab-2.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-08 13:43:39.000000 erlab-2.0.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-08 13:43:39.000000 erlab-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.542651 erlab-2.0.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 13:43:39.000000 erlab-2.0.0/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-08 13:43:39.000000 erlab-2.0.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-08 13:43:39.000000 erlab-2.0.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-08 13:43:39.000000 erlab-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-08 13:43:39.000000 erlab-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)    98753 2024-04-08 13:43:41.000000 erlab-2.0.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-08 13:43:39.000000 erlab-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    46760 2024-04-08 13:43:45.578651 erlab-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-08 13:43:39.000000 erlab-2.0.0/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     4414 2024-04-08 13:43:39.000000 erlab-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.546651 erlab-2.0.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      655 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.546651 erlab-2.0.0/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    13912 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    13410 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/development.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.characterization.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     2888 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.554651 erlab-2.0.0/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.558651 erlab-2.0.0/docs/source/notebooks/
+-rw-r--r--   0 root         (0) root         (0)   189769 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/notebooks/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)     1582 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/notebooks/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)   379533 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/notebooks/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    15761 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/notebooks/plotting.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.558651 erlab-2.0.0/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2579 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     2356 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/refs.bib
+-rw-r--r--   0 root         (0) root         (0)     1259 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/userguide.rst
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-08 13:43:39.000000 erlab-2.0.0/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-08 13:43:39.000000 erlab-2.0.0/environment_apple.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-08 13:43:39.000000 erlab-2.0.0/environment_nogit.yml
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-08 13:43:39.000000 erlab-2.0.0/environment_nogit_mkl.yml
+-rw-r--r--   0 root         (0) root         (0)     4351 2024-04-08 13:43:39.000000 erlab-2.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-08 13:43:39.000000 erlab-2.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 13:43:45.578651 erlab-2.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.538651 erlab-2.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.558651 erlab-2.0.0/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-08 13:43:41.000000 erlab-2.0.0/src/erlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35543 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/accessors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.562651 erlab-2.0.0/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.562651 erlab-2.0.0/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      459 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.562651 erlab-2.0.0/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      840 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9632 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     6026 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)     9818 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    15394 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    17273 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10359 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.562651 erlab-2.0.0/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     2775 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7810 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     8659 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.562651 erlab-2.0.0/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.566651 erlab-2.0.0/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13943 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    20867 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    22451 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    14901 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)     9458 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.566651 erlab-2.0.0/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    19391 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.566651 erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52076 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114751 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27081 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    54122 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    13907 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25375 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    16658 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     3341 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    52417 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.570651 erlab-2.0.0/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30047 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6780 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.570651 erlab-2.0.0/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3674 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     7448 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7745 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     5630 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.570651 erlab-2.0.0/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.574651 erlab-2.0.0/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     1857 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29010 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18275 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    32411 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    31070 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.574651 erlab-2.0.0/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.578651 erlab-2.0.0/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    46760 2024-04-08 13:43:45.000000 erlab-2.0.0/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4487 2024-04-08 13:43:45.000000 erlab-2.0.0/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 13:43:45.000000 erlab-2.0.0/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      370 2024-04-08 13:43:45.000000 erlab-2.0.0/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-08 13:43:45.000000 erlab-2.0.0/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.574651 erlab-2.0.0/templates/
+-rw-r--r--   0 root         (0) root         (0)      971 2024-04-08 13:43:39.000000 erlab-2.0.0/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-08 13:43:39.000000 erlab-2.0.0/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-08 13:43:39.000000 erlab-2.0.0/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.578651 erlab-2.0.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4485 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     5229 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_image.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_utilities.py
```

### Comparing `erlab-1.6.5/.github/ISSUE_TEMPLATE/feature_request.md` & `erlab-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/.github/workflows/pr.yml` & `erlab-2.0.0/.github/workflows/pr.yml`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,14 @@
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install pytest and dependencies
         run: |
           sudo apt update && sudo apt install -y libegl1-mesa-dev
           python -m pip install --upgrade pip
-          python -m pip install -v . pytest pytest-xdist
           python -m pip install -r requirements.txt
+          python -m pip install -v . pytest pytest-xdist
 
 
       - name: Test with pytest
         run: |
           pytest -v -n auto
```

### Comparing `erlab-1.6.5/.github/workflows/release.yml` & `erlab-2.0.0/.github/workflows/release.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install pytest and dependencies
         run: |
           sudo apt update && sudo apt install -y libegl1-mesa-dev
           python -m pip install --upgrade pip
-          python -m pip install -v . pytest pytest-xdist
           python -m pip install -r requirements.txt
+          python -m pip install -v . pytest pytest-xdist
 
 
       - name: Test with pytest
         run: |
           pytest -v -n auto
 
   release:
```

### Comparing `erlab-1.6.5/.gitignore` & `erlab-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/.pre-commit-config.yaml` & `erlab-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/.readthedocs.yaml` & `erlab-2.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/CHANGELOG.md` & `erlab-2.0.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,1535 +1,1620 @@
 # CHANGELOG
 
 
 
+## v2.0.0 (2024-04-08)
+
+### Breaking
+
+* **fit** unify dynamic function names ([`20d784c`](https://github.com/kmnhan/erlabpy/commit/20d784c1d8fdcd786ab73b3ae03d3e331dc04df5))
+
+  BREAKING CHANGE: `PolyFunc` is now `PolynomialFunction`, and `FermiEdge2dFunc` is now `FermiEdge2dFunction`. The corresponding model names are unchanged.
+
+* **fit** directly base models on lmfit.Model ([`59163d5`](https://github.com/kmnhan/erlabpy/commit/59163d5f0e000d65aa53690a51b6db82df1ce5f1))
+
+  BREAKING CHANGE: This change disables the use of guess_fit. All fitting must be performed in the syntax recommended by lmfit. Addition of a accessor or a convenience function for coordinate-aware fitting is planned in the next release.
+
+### Build
+
+* add templates for changelog and release notes ([`be72b24`](https://github.com/kmnhan/erlabpy/commit/be72b245f1194d1bd894bd12c845f68eedbb8f3b))
+
+### Chore
+
+* add setuptools_scm configuration ([`506faa6`](https://github.com/kmnhan/erlabpy/commit/506faa6bcb63b03bbce4add7fd5a7b5a4f761320))
+
+* **deps** update dependency to use igor2&gt;=0.5.6 now on conda-forge ([`b59fc5a`](https://github.com/kmnhan/erlabpy/commit/b59fc5a75071191e199c20424df6b76860d69029))
+
+* **deps** remove igor2 direct dependency from requirements.txt ([`bfb5518`](https://github.com/kmnhan/erlabpy/commit/bfb551893d7858ed1816a376b25ef6aba5004b3b))
+
+* **deps** remove importlib metadata ([`b5718e7`](https://github.com/kmnhan/erlabpy/commit/b5718e7aeb988b1cfe8e5026358640d49481db61))
+
+* **deps** update minimum versions and env configurations ([`18a3d67`](https://github.com/kmnhan/erlabpy/commit/18a3d67becacbfe2b907c206490917a85541df2c))
+
+* **deps** update dependencies ([`b3e2494`](https://github.com/kmnhan/erlabpy/commit/b3e249460d99f429c403cdaad01d7f3ea16084e9))
+
+* **deps** remove importlib ([`8a6b818`](https://github.com/kmnhan/erlabpy/commit/8a6b818a1c38e87e648bdc80a82148d31083bf0d))
+
+### Ci
+
+* **github** swap pip installation order ([`afa4722`](https://github.com/kmnhan/erlabpy/commit/afa472259a564019c3d8e78fee158277eed9c923))
+
+### Documentation
+
+* fix typo ([`dc8204a`](https://github.com/kmnhan/erlabpy/commit/dc8204aa67488e6efc29d50ccf73f8b0babc0f9c))
+
+* update conf.py ([`3f092c4`](https://github.com/kmnhan/erlabpy/commit/3f092c472ae5312dee18ab9be98d080124f02edc))
+
+* update bibliography ([`8e32515`](https://github.com/kmnhan/erlabpy/commit/8e325159b7f8f4e631dece557028f94527481cfd))
+
+* improve readability ([`bd8049d`](https://github.com/kmnhan/erlabpy/commit/bd8049d1060791f5df22ef6b610fe26a700c14cc))
+
+* update minimum gradient documentation ([`a8df0f3`](https://github.com/kmnhan/erlabpy/commit/a8df0f3ba04e979f0a8d6fb9b2598c65b28767e1))
+
+### Feature
+
+* **itool** add copy code to PlotItem vb menu ([`7b4f30a`](https://github.com/kmnhan/erlabpy/commit/7b4f30ada21c5accc1d3824ad3d0f8097f9a99c1))
+
+  For each plot in imagetool, a new &#39;copy selection code&#39; button has been added to the right-click menu that copies the code that can slice the data to recreate the data shown in the plot.
+
+* add 2D curvature, finally closes #14 ([`7fe95ff`](https://github.com/kmnhan/erlabpy/commit/7fe95ffcdf0531e456cfc97ae605467e4ae433c0))
+
+* **plotting** add N argument to plot_array_2d ([`2cd79f7`](https://github.com/kmnhan/erlabpy/commit/2cd79f7ee007058da09aff244cd75748698444ee))
+
+* add scaled laplace ([`079e1d2`](https://github.com/kmnhan/erlabpy/commit/079e1d21201c7523877b06a0f04f7640027b0614))
+
+* add gaussian filter and laplacian ([`8628d33`](https://github.com/kmnhan/erlabpy/commit/8628d336ff5b4219e4fd382293736e4cbf026d56))
+
+* add derivative module with minimum gradient implementation ([`e0eabde`](https://github.com/kmnhan/erlabpy/commit/e0eabde60e6860c3827959b45be6d4f491918363))
+
+### Fix
+
+* **dynamic** properly broadcast xarray input ([`2f6672f`](https://github.com/kmnhan/erlabpy/commit/2f6672f3b003792ecd98b4fbc99fb11fcc0efb8b))
+
+* **fit.functions** polynomial function now works for xarray input ([`3eb80de`](https://github.com/kmnhan/erlabpy/commit/3eb80dea31b6414fa9a694049b92b7334a4e10f5))
+
+* **analysis.image** remove critical typo ([`fb7de0f`](https://github.com/kmnhan/erlabpy/commit/fb7de0fc3ba9049c488a90bef8ee3c4feb935341))
+
+* **analysis.image** dtype safety of cfunc ([`b4f9b17`](https://github.com/kmnhan/erlabpy/commit/b4f9b17656c64be4cff876843ed0f3491d8310d4))
+
+* set autodownsample off for colorbar ([`256bf2d`](https://github.com/kmnhan/erlabpy/commit/256bf2dc8c368d093a3578d7f9279b1ee4653534))
+
+* disable itool downsample ([`e626bba`](https://github.com/kmnhan/erlabpy/commit/e626bba9fcd4fd31387ca3a07a9a33b7690f3645))
+
+### Performance
+
+* **itool** add explicit signatures to fastbinning ([`62e1d51`](https://github.com/kmnhan/erlabpy/commit/62e1d516f0260f661fe9cd8f1fae9cb81afbcabe))
+
+  Speedup initial binning by providing explicit signatures.
+
+### Refactor
+
+* update dtool to use new functions ([`a6e46bb`](https://github.com/kmnhan/erlabpy/commit/a6e46bb8b19512e438291afbbd5e0e9a4eb4fe87))
+
+* **analysis.image** add documentation and reorder functions ([`340665d`](https://github.com/kmnhan/erlabpy/commit/340665dc507a99acc7d56c46a2a2326fbb56b1e3))
+
+* rename module to image and add citation ([`b74a654`](https://github.com/kmnhan/erlabpy/commit/b74a654e07d9f4522cee2db0b897f1ffcdb86e94))
+
+* **dtool** cleanup unused code ([`f4abd34`](https://github.com/kmnhan/erlabpy/commit/f4abd34bbf3130c0ec0fd2f9c830c8da43849f13))
+
+### Unknown
+
+* tests: reduce test time by specifying explicit path ([`60fb0d0`](https://github.com/kmnhan/erlabpy/commit/60fb0d0cedd9f0aaeca7101dddf0848f8872ccc3))
+
+  
+  This will not trigger directory recursion, so tests will run a bit faster
+
+* tests: add tests for fitting functions ([`4992251`](https://github.com/kmnhan/erlabpy/commit/499225149346e970d00b60dcb5ca39af5e5ddb47))
+
+* tests: add tests for image and shift ([`7e4daeb`](https://github.com/kmnhan/erlabpy/commit/7e4daeb5aea9689aadfe3eedb561d313e217684c))
+
+
 ## v1.6.5 (2024-04-03)
 
 ### Fix
 
-* fix: make imports work without optional pip dependencies ([`b8ac11d`](https://github.com/kmnhan/erlabpy/commit/b8ac11d8fb4379f70a39c817332382c352391a64))
+* make imports work without optional pip dependencies ([`b8ac11d`](https://github.com/kmnhan/erlabpy/commit/b8ac11d8fb4379f70a39c817332382c352391a64))
 
 
 ## v1.6.4 (2024-04-03)
 
 ### Fix
 
-* fix: load colormaps only when igor2 is  available ([`7927c7d`](https://github.com/kmnhan/erlabpy/commit/7927c7db264bedb1a27b980d820d352f779b64c9))
+* load colormaps only when igor2 is  available ([`7927c7d`](https://github.com/kmnhan/erlabpy/commit/7927c7db264bedb1a27b980d820d352f779b64c9))
 
 
 ## v1.6.3 (2024-04-03)
 
 ### Fix
 
-* fix: leave out type annotation for passing tests ([`eb25008`](https://github.com/kmnhan/erlabpy/commit/eb2500838820172529ee751b5d8a624c950f66d2))
+* leave out type annotation for passing tests ([`eb25008`](https://github.com/kmnhan/erlabpy/commit/eb2500838820172529ee751b5d8a624c950f66d2))
 
 
 ## v1.6.2 (2024-04-03)
 
 ### Fix
 
-* fix: igor2 does not have to be installed on import time ([`186727a`](https://github.com/kmnhan/erlabpy/commit/186727ac8d50b662efeba8bee567cf1013ca936a))
+* igor2 does not have to be installed on import time ([`186727a`](https://github.com/kmnhan/erlabpy/commit/186727ac8d50b662efeba8bee567cf1013ca936a))
 
 
 ## v1.6.1 (2024-04-03)
 
 ### Chore
 
-* chore(deps): add pre-commit to dev dependency ([`3a2fccd`](https://github.com/kmnhan/erlabpy/commit/3a2fccd978d23d806d2088ebd9ef60c7a2b20902))
+* **deps** add pre-commit to dev dependency ([`3a2fccd`](https://github.com/kmnhan/erlabpy/commit/3a2fccd978d23d806d2088ebd9ef60c7a2b20902))
 
-* chore: make csaps optional ([`db31b06`](https://github.com/kmnhan/erlabpy/commit/db31b064c1f46edef7743fdd1c3ab7984e170b3c))
+* make csaps optional ([`db31b06`](https://github.com/kmnhan/erlabpy/commit/db31b064c1f46edef7743fdd1c3ab7984e170b3c))
 
-* chore: update issue templates ([`dfc2ab0`](https://github.com/kmnhan/erlabpy/commit/dfc2ab0fdfcf1fd5ab83dac2c9d6473b4d2cb7e1))
+* update issue templates ([`dfc2ab0`](https://github.com/kmnhan/erlabpy/commit/dfc2ab0fdfcf1fd5ab83dac2c9d6473b4d2cb7e1))
 
 ### Ci
 
-* ci(github): remove linting, let pre-commit handle it ([`b209ecb`](https://github.com/kmnhan/erlabpy/commit/b209ecbb3c0a35d2bbeba8155bea3da9ffa58fe1))
+* **github** remove linting, let pre-commit handle it ([`b209ecb`](https://github.com/kmnhan/erlabpy/commit/b209ecbb3c0a35d2bbeba8155bea3da9ffa58fe1))
 
-* ci(pre-commit): add hooks ([`9b401c3`](https://github.com/kmnhan/erlabpy/commit/9b401c328bb3ff18dddcce40b935afa2b6e2624a))
+* **pre-commit** add hooks ([`9b401c3`](https://github.com/kmnhan/erlabpy/commit/9b401c328bb3ff18dddcce40b935afa2b6e2624a))
 
 ### Documentation
 
-* docs: rephrase kconv guide ([`dd2c022`](https://github.com/kmnhan/erlabpy/commit/dd2c022e42e692c2af640a1fc8d21c3e429781b2))
+* rephrase kconv guide ([`dd2c022`](https://github.com/kmnhan/erlabpy/commit/dd2c022e42e692c2af640a1fc8d21c3e429781b2))
 
-* docs: add ipykernel dependency to resolve failing builds ([`e5774a5`](https://github.com/kmnhan/erlabpy/commit/e5774a51c14ef6df190eb9f6198c274d2061cdd5))
+* add ipykernel dependency to resolve failing builds ([`e5774a5`](https://github.com/kmnhan/erlabpy/commit/e5774a51c14ef6df190eb9f6198c274d2061cdd5))
 
-* docs: add hvplot example ([`6997020`](https://github.com/kmnhan/erlabpy/commit/69970208ba6658f15e900ee6b9367177fcd86d29))
+* add hvplot example ([`6997020`](https://github.com/kmnhan/erlabpy/commit/69970208ba6658f15e900ee6b9367177fcd86d29))
 
 ### Fix
 
-* fix: remove all pypi dependencies from pyproject.toml ([`1b2fd55`](https://github.com/kmnhan/erlabpy/commit/1b2fd5594f00bba8367419cd00919eba45cde5a7))
+* remove all pypi dependencies from pyproject.toml ([`1b2fd55`](https://github.com/kmnhan/erlabpy/commit/1b2fd5594f00bba8367419cd00919eba45cde5a7))
 
 ### Refactor
 
-* refactor: remove ktool_old ([`18ea072`](https://github.com/kmnhan/erlabpy/commit/18ea0723fdf538bdbf2789ca73b2b962839ca3e5))
+* remove ktool_old ([`18ea072`](https://github.com/kmnhan/erlabpy/commit/18ea0723fdf538bdbf2789ca73b2b962839ca3e5))
 
 ### Style
 
-* style: apply ruff to deprecated imagetools ([`b2c7596`](https://github.com/kmnhan/erlabpy/commit/b2c7596ed12d89edaa2be3fe2923388014c68007))
+* apply ruff to deprecated imagetools ([`b2c7596`](https://github.com/kmnhan/erlabpy/commit/b2c7596ed12d89edaa2be3fe2923388014c68007))
 
-* style: apply pre-commit fixes ([`12b6441`](https://github.com/kmnhan/erlabpy/commit/12b6441419ed6c4ff4da921790c57a599032dba7))
+* apply pre-commit fixes ([`12b6441`](https://github.com/kmnhan/erlabpy/commit/12b6441419ed6c4ff4da921790c57a599032dba7))
 
 
 ## v1.6.0 (2024-04-02)
 
 ### Ci
 
-* ci: speedup tests ([`618851e`](https://github.com/kmnhan/erlabpy/commit/618851e74d94301ec4f85a46facd46d3b6272571))
+* speedup tests ([`618851e`](https://github.com/kmnhan/erlabpy/commit/618851e74d94301ec4f85a46facd46d3b6272571))
 
-* ci: parallelize tests ([`232301a`](https://github.com/kmnhan/erlabpy/commit/232301a0ab26c9c32a355af11b5458395a1cd832))
+* parallelize tests ([`232301a`](https://github.com/kmnhan/erlabpy/commit/232301a0ab26c9c32a355af11b5458395a1cd832))
 
-* ci: migrate from pylint to ruff ([`2acd5e3`](https://github.com/kmnhan/erlabpy/commit/2acd5e3177f97f196d94644d75e3566a2714bf40))
+* migrate from pylint to ruff ([`2acd5e3`](https://github.com/kmnhan/erlabpy/commit/2acd5e3177f97f196d94644d75e3566a2714bf40))
 
-* ci: add pre-commit configuration ([`063067d`](https://github.com/kmnhan/erlabpy/commit/063067dfdedefefc47e55096d310a4df54a5b999))
+* add pre-commit configuration ([`063067d`](https://github.com/kmnhan/erlabpy/commit/063067dfdedefefc47e55096d310a4df54a5b999))
 
 ### Documentation
 
-* docs: add pre-commit ci status badge ([`ae39d3d`](https://github.com/kmnhan/erlabpy/commit/ae39d3dbb0a058b59493b97507f88576f6b1737a))
+* add pre-commit ci status badge ([`ae39d3d`](https://github.com/kmnhan/erlabpy/commit/ae39d3dbb0a058b59493b97507f88576f6b1737a))
 
-* docs: add pre-commit badges ([`1b6702b`](https://github.com/kmnhan/erlabpy/commit/1b6702b9615c9881afb86883466f3e8846a2db12))
+* add pre-commit badges ([`1b6702b`](https://github.com/kmnhan/erlabpy/commit/1b6702b9615c9881afb86883466f3e8846a2db12))
 
-* docs: replace black with ruff ([`cb1a4b5`](https://github.com/kmnhan/erlabpy/commit/cb1a4b56a1b11b6d4630e5a36307befc48270294))
+* replace black with ruff ([`cb1a4b5`](https://github.com/kmnhan/erlabpy/commit/cb1a4b56a1b11b6d4630e5a36307befc48270294))
 
 ### Feature
 
-* feat: add mdctool ([`a4976f9`](https://github.com/kmnhan/erlabpy/commit/a4976f93cde51a41d667321a93dc2a90f23bddc3))
+* add mdctool ([`a4976f9`](https://github.com/kmnhan/erlabpy/commit/a4976f93cde51a41d667321a93dc2a90f23bddc3))
 
 ### Refactor
 
-* refactor: remove deprecated function and dependencies ([`4b9c7b1`](https://github.com/kmnhan/erlabpy/commit/4b9c7b1629d99fbf0108ca33791d1bfd59632199))
+* remove deprecated function and dependencies ([`4b9c7b1`](https://github.com/kmnhan/erlabpy/commit/4b9c7b1629d99fbf0108ca33791d1bfd59632199))
 
 ### Style
 
-* style: remove unnecessary dict call ([`ea0e0e8`](https://github.com/kmnhan/erlabpy/commit/ea0e0e822f8487ec5238b651f3d72aafac5c6bcb))
+* remove unnecessary dict call ([`ea0e0e8`](https://github.com/kmnhan/erlabpy/commit/ea0e0e822f8487ec5238b651f3d72aafac5c6bcb))
 
-* style: apply formatting ([`12e3a16`](https://github.com/kmnhan/erlabpy/commit/12e3a1649ce03792f79df8220f70572ff0ecc97a))
+* apply formatting ([`12e3a16`](https://github.com/kmnhan/erlabpy/commit/12e3a1649ce03792f79df8220f70572ff0ecc97a))
 
-* style: remove implicit optionals and apply more linter suggestions ([`798508c`](https://github.com/kmnhan/erlabpy/commit/798508c6a65ac439be70f9b7cc32c801ae8632cb))
+* remove implicit optionals and apply more linter suggestions ([`798508c`](https://github.com/kmnhan/erlabpy/commit/798508c6a65ac439be70f9b7cc32c801ae8632cb))
 
-* style: reduce indentation ([`274a330`](https://github.com/kmnhan/erlabpy/commit/274a33037b0155b82d8f9eb5ec542568c54da1db))
+* reduce indentation ([`274a330`](https://github.com/kmnhan/erlabpy/commit/274a33037b0155b82d8f9eb5ec542568c54da1db))
 
-* style: move imports to type-checking block ([`e1f4005`](https://github.com/kmnhan/erlabpy/commit/e1f400516dcbc220979346f25a7dcfe4018df906))
+* move imports to type-checking block ([`e1f4005`](https://github.com/kmnhan/erlabpy/commit/e1f400516dcbc220979346f25a7dcfe4018df906))
 
-* style: cleanup kwargs and unnecessary pass statements ([`7867623`](https://github.com/kmnhan/erlabpy/commit/7867623e779636531cdf1e0675846d22d0045249))
+* cleanup kwargs and unnecessary pass statements ([`7867623`](https://github.com/kmnhan/erlabpy/commit/7867623e779636531cdf1e0675846d22d0045249))
 
-* style: make collections literal ([`74a8878`](https://github.com/kmnhan/erlabpy/commit/74a887853c2e84f315d45e52844a9c0fa7b46e28))
+* make collections literal ([`74a8878`](https://github.com/kmnhan/erlabpy/commit/74a887853c2e84f315d45e52844a9c0fa7b46e28))
 
-* style: rewrite unnecessary dict calls as literal ([`10637f6`](https://github.com/kmnhan/erlabpy/commit/10637f622b29703a02b4666c5712e8cf03a96066))
+* rewrite unnecessary dict calls as literal ([`10637f6`](https://github.com/kmnhan/erlabpy/commit/10637f622b29703a02b4666c5712e8cf03a96066))
 
-* style: format with ruff ([`64f3fed`](https://github.com/kmnhan/erlabpy/commit/64f3fed42e4766c1fe70d6a9488b75179a905314))
+* format with ruff ([`64f3fed`](https://github.com/kmnhan/erlabpy/commit/64f3fed42e4766c1fe70d6a9488b75179a905314))
 
-* style: fix flake8-bugbear violations ([`4aade97`](https://github.com/kmnhan/erlabpy/commit/4aade97013cea63e20895fb39b43c04953a67984))
+* fix flake8-bugbear violations ([`4aade97`](https://github.com/kmnhan/erlabpy/commit/4aade97013cea63e20895fb39b43c04953a67984))
 
-* style: apply ruff unsafe fixes ([`a1a7d9a`](https://github.com/kmnhan/erlabpy/commit/a1a7d9ae79d3afa88cffe7423bb942aca29bfd09))
+* apply ruff unsafe fixes ([`a1a7d9a`](https://github.com/kmnhan/erlabpy/commit/a1a7d9ae79d3afa88cffe7423bb942aca29bfd09))
 
-* style: lint with pyupgrade and ruff ([`244e053`](https://github.com/kmnhan/erlabpy/commit/244e05305ce2e0b72c54e3eb7c96befb97762f87))
+* lint with pyupgrade and ruff ([`244e053`](https://github.com/kmnhan/erlabpy/commit/244e05305ce2e0b72c54e3eb7c96befb97762f87))
 
-* style: apply linter suggestions ([`7295cbc`](https://github.com/kmnhan/erlabpy/commit/7295cbc5b08065d75447f80ab1d84eb1c15255f3))
+* apply linter suggestions ([`7295cbc`](https://github.com/kmnhan/erlabpy/commit/7295cbc5b08065d75447f80ab1d84eb1c15255f3))
 
 ### Unknown
 
-* [pre-commit.ci] auto fixes from pre-commit.com hooks
+* [pre-commit.ci] auto fixes from pre-commit.com hooks ([`b86c995`](https://github.com/kmnhan/erlabpy/commit/b86c9952be94b4b7f5e5918ed28cbf39b750ef09))
 
-for more information, see https://pre-commit.ci ([`b86c995`](https://github.com/kmnhan/erlabpy/commit/b86c9952be94b4b7f5e5918ed28cbf39b750ef09))
+  
+  for more information, see https://pre-commit.ci
 
 
 ## v1.5.2 (2024-04-01)
 
 ### Documentation
 
-* docs: update user guide notebooks ([`80ab771`](https://github.com/kmnhan/erlabpy/commit/80ab7717539e95c2cfe4a15f0713f259dfe04da3))
+* update user guide notebooks ([`80ab771`](https://github.com/kmnhan/erlabpy/commit/80ab7717539e95c2cfe4a15f0713f259dfe04da3))
 
-* docs: update docstring ([`b262765`](https://github.com/kmnhan/erlabpy/commit/b2627651648066dc8b98f023c5028c11f2929426))
+* update docstring ([`b262765`](https://github.com/kmnhan/erlabpy/commit/b2627651648066dc8b98f023c5028c11f2929426))
 
-* docs: update documentation ([`9051ed8`](https://github.com/kmnhan/erlabpy/commit/9051ed8d406c06ae4a037b65ed648a16843a0655))
+* update documentation ([`9051ed8`](https://github.com/kmnhan/erlabpy/commit/9051ed8d406c06ae4a037b65ed648a16843a0655))
 
 ### Fix
 
-* fix: set values after setting bounds ([`ab6d682`](https://github.com/kmnhan/erlabpy/commit/ab6d682d0afafefcaec4c1ab6d673a39a75f40a6))
+* set values after setting bounds ([`ab6d682`](https://github.com/kmnhan/erlabpy/commit/ab6d682d0afafefcaec4c1ab6d673a39a75f40a6))
 
-* fix: proper patch all interpolator selection functions ([`b91834e`](https://github.com/kmnhan/erlabpy/commit/b91834e1b0be200bafb86ed3581f08cf1a5d42ef))
+* proper patch all interpolator selection functions ([`b91834e`](https://github.com/kmnhan/erlabpy/commit/b91834e1b0be200bafb86ed3581f08cf1a5d42ef))
 
-* fix: make bz voronoi robust ([`8259760`](https://github.com/kmnhan/erlabpy/commit/8259760249be45892cd32f143b1b83aefe166c49))
+* make bz voronoi robust ([`8259760`](https://github.com/kmnhan/erlabpy/commit/8259760249be45892cd32f143b1b83aefe166c49))
 
 ### Refactor
 
-* refactor: remove debug print statement in FastInterpolator class ([`712bd2c`](https://github.com/kmnhan/erlabpy/commit/712bd2ce90ad3534212d8a63c3fe10d780e243f5))
+* remove debug print statement in FastInterpolator class ([`712bd2c`](https://github.com/kmnhan/erlabpy/commit/712bd2ce90ad3534212d8a63c3fe10d780e243f5))
 
-* refactor: add edge correction ([`87adcef`](https://github.com/kmnhan/erlabpy/commit/87adceffda2364f404de0860bfe8bf36b4cc1394))
+* add edge correction ([`87adcef`](https://github.com/kmnhan/erlabpy/commit/87adceffda2364f404de0860bfe8bf36b4cc1394))
 
-* refactor: change variable name ([`b68949e`](https://github.com/kmnhan/erlabpy/commit/b68949ec59fd6bd7d7dad4ff9cc232b0e1ce4fba))
+* change variable name ([`b68949e`](https://github.com/kmnhan/erlabpy/commit/b68949ec59fd6bd7d7dad4ff9cc232b0e1ce4fba))
 
-* refactor: make rotation transformations try fast interpolator first ([`e0a7908`](https://github.com/kmnhan/erlabpy/commit/e0a790833025f0c7e952ad17d120f46de3100555))
+* make rotation transformations try fast interpolator first ([`e0a7908`](https://github.com/kmnhan/erlabpy/commit/e0a790833025f0c7e952ad17d120f46de3100555))
 
-* refactor: update warning message ([`af67c1a`](https://github.com/kmnhan/erlabpy/commit/af67c1a507be35348b58862b6b51b92fac52781b))
+* update warning message ([`af67c1a`](https://github.com/kmnhan/erlabpy/commit/af67c1a507be35348b58862b6b51b92fac52781b))
 
-* refactor: add several new accessors ([`664e92a`](https://github.com/kmnhan/erlabpy/commit/664e92a3e171512be26ea957df945e84134c880a))
+* add several new accessors ([`664e92a`](https://github.com/kmnhan/erlabpy/commit/664e92a3e171512be26ea957df945e84134c880a))
 
-* refactor: use new accessors and attrs ([`8e1dee2`](https://github.com/kmnhan/erlabpy/commit/8e1dee22d9d716f7e9bce29a1be3e68311494aa1))
+* use new accessors and attrs ([`8e1dee2`](https://github.com/kmnhan/erlabpy/commit/8e1dee22d9d716f7e9bce29a1be3e68311494aa1))
 
-* refactor: add qplot accessor ([`cb9aa01`](https://github.com/kmnhan/erlabpy/commit/cb9aa017bebd2ee6661f4eb87b988509d28a37a5))
+* add qplot accessor ([`cb9aa01`](https://github.com/kmnhan/erlabpy/commit/cb9aa017bebd2ee6661f4eb87b988509d28a37a5))
 
-* refactor: remove annotate_cuts ([`004ee80`](https://github.com/kmnhan/erlabpy/commit/004ee808dab13073cb3d2021d331767f6c28388a))
+* remove annotate_cuts ([`004ee80`](https://github.com/kmnhan/erlabpy/commit/004ee808dab13073cb3d2021d331767f6c28388a))
 
-* refactor: dataloader cleanup ([`fd97780`](https://github.com/kmnhan/erlabpy/commit/fd977800a504256afd6018e9991b2d1e996277df))
+* dataloader cleanup ([`fd97780`](https://github.com/kmnhan/erlabpy/commit/fd977800a504256afd6018e9991b2d1e996277df))
 
 
 ## v1.5.1 (2024-03-28)
 
 ### Documentation
 
-* docs: update README screenshots ([`04d6b44`](https://github.com/kmnhan/erlabpy/commit/04d6b443dc077cbf056dae9b2bf9630284e707ee))
+* update README screenshots ([`04d6b44`](https://github.com/kmnhan/erlabpy/commit/04d6b443dc077cbf056dae9b2bf9630284e707ee))
 
-* docs: use svg plots ([`aaa4842`](https://github.com/kmnhan/erlabpy/commit/aaa48420f69c71eb08180934ef2051819df92c03))
+* use svg plots ([`aaa4842`](https://github.com/kmnhan/erlabpy/commit/aaa48420f69c71eb08180934ef2051819df92c03))
 
-* docs: improve momentum conversion documentation ([`c315a1a`](https://github.com/kmnhan/erlabpy/commit/c315a1a6e4d6365a6cc02e861dae84daf9e0cc14))
+* improve momentum conversion documentation ([`c315a1a`](https://github.com/kmnhan/erlabpy/commit/c315a1a6e4d6365a6cc02e861dae84daf9e0cc14))
 
-* docs: update dev docs ([`7406308`](https://github.com/kmnhan/erlabpy/commit/740630899108d562bcc542bd6ae9d147b893c27d))
+* update dev docs ([`7406308`](https://github.com/kmnhan/erlabpy/commit/740630899108d562bcc542bd6ae9d147b893c27d))
 
 ### Fix
 
-* fix: restore argname detection that was broken with namespace changes ([`863b702`](https://github.com/kmnhan/erlabpy/commit/863b702b6373f9a219a1e770aa49c71145371681))
+* restore argname detection that was broken with namespace changes ([`863b702`](https://github.com/kmnhan/erlabpy/commit/863b702b6373f9a219a1e770aa49c71145371681))
 
-* fix: namespace collision ([`10edcdc`](https://github.com/kmnhan/erlabpy/commit/10edcdc8b06425c380ca6caa2d3f5f2be5c13733))
+* namespace collision ([`10edcdc`](https://github.com/kmnhan/erlabpy/commit/10edcdc8b06425c380ca6caa2d3f5f2be5c13733))
 
-* fix: followup namespace change ([`4c5222c`](https://github.com/kmnhan/erlabpy/commit/4c5222cc93196f0b6a75a0101107a37e73748eeb))
+* followup namespace change ([`4c5222c`](https://github.com/kmnhan/erlabpy/commit/4c5222cc93196f0b6a75a0101107a37e73748eeb))
 
 ### Refactor
 
-* refactor: allow offsetview upate chaining
+* allow offsetview upate chaining ([`8d5ca4f`](https://github.com/kmnhan/erlabpy/commit/8d5ca4f5b12c7d7060ea444773a9851f23db9850))
 
-This also means that _repr_html_ is automatically displayed when update or reset is called. ([`8d5ca4f`](https://github.com/kmnhan/erlabpy/commit/8d5ca4f5b12c7d7060ea444773a9851f23db9850))
+  This also means that _repr_html_ is automatically displayed when update or reset is called.
 
-* refactor: improve consistency in accessors
+* improve consistency in accessors ([`9596fd7`](https://github.com/kmnhan/erlabpy/commit/9596fd723206f3e992fe00990f73364a61604cd6))
 
-Added setter method for configuration too. ([`9596fd7`](https://github.com/kmnhan/erlabpy/commit/9596fd723206f3e992fe00990f73364a61604cd6))
+  Added setter method for configuration too.
 
-* refactor: make prints consistent ([`0021302`](https://github.com/kmnhan/erlabpy/commit/002130224e3efc01615948a6443516e29d333cf5))
+* make prints consistent ([`0021302`](https://github.com/kmnhan/erlabpy/commit/002130224e3efc01615948a6443516e29d333cf5))
 
-* refactor: change module names to prevent conflict with function names
+* change module names to prevent conflict with function names ([`493a5aa`](https://github.com/kmnhan/erlabpy/commit/493a5aab19c0d66851ca068e286a6aec92131e33))
 
-Cleanup erplot namespace and move tools to interactive. ([`493a5aa`](https://github.com/kmnhan/erlabpy/commit/493a5aab19c0d66851ca068e286a6aec92131e33))
+  Cleanup erplot namespace and move tools to interactive.
 
-* refactor: follow class naming conventions ([`efb9610`](https://github.com/kmnhan/erlabpy/commit/efb9610a864ef637f424c2f1b2871add7324b090))
+* follow class naming conventions ([`efb9610`](https://github.com/kmnhan/erlabpy/commit/efb9610a864ef637f424c2f1b2871add7324b090))
 
 
 ## v1.5.0 (2024-03-27)
 
 ### Chore
 
-* chore: remove unnecessary dependency on colorcet, cmasher, cmocean and seaborn ([`5fd2d61`](https://github.com/kmnhan/erlabpy/commit/5fd2d614f97e8bba4f34a9277c70835214a95be7))
+* remove unnecessary dependency on colorcet, cmasher, cmocean and seaborn ([`5fd2d61`](https://github.com/kmnhan/erlabpy/commit/5fd2d614f97e8bba4f34a9277c70835214a95be7))
 
-* chore: add isort profile to project configuration ([`df269a9`](https://github.com/kmnhan/erlabpy/commit/df269a990e642135c76a60bfd19e0a6767974a40))
+* add isort profile to project configuration ([`df269a9`](https://github.com/kmnhan/erlabpy/commit/df269a990e642135c76a60bfd19e0a6767974a40))
 
-* chore: update dependencies and environment files
+* update dependencies and environment files ([`6ec32dd`](https://github.com/kmnhan/erlabpy/commit/6ec32ddedb342d0556aacec0625c889b01f18b62))
 
-Fix python version and remove editable installs ([`6ec32dd`](https://github.com/kmnhan/erlabpy/commit/6ec32ddedb342d0556aacec0625c889b01f18b62))
+  Fix python version and remove editable installs
 
-* chore: change pyclip dependency to pyperclip
+* change pyclip dependency to pyperclip ([`db78f8e`](https://github.com/kmnhan/erlabpy/commit/db78f8e5a8be47ca4f23aa560e8aef88efb58c5b))
 
-Although pyclip supports copying bytes, it&#39;s not on conda-forge. Using pyperclip instead. ([`db78f8e`](https://github.com/kmnhan/erlabpy/commit/db78f8e5a8be47ca4f23aa560e8aef88efb58c5b))
+  Although pyclip supports copying bytes, it&#39;s not on conda-forge. Using pyperclip instead.
 
 ### Documentation
 
-* docs: add momentum conversion documentation draft ([`5410763`](https://github.com/kmnhan/erlabpy/commit/54107632edd5a7a911a1c8d06c663fc48d5217a0))
+* add momentum conversion documentation draft ([`5410763`](https://github.com/kmnhan/erlabpy/commit/54107632edd5a7a911a1c8d06c663fc48d5217a0))
 
-* docs: add installation and contribution information ([`93a4e7c`](https://github.com/kmnhan/erlabpy/commit/93a4e7c4f43a8133f3f2149eb638261a9d56cfe6))
+* add installation and contribution information ([`93a4e7c`](https://github.com/kmnhan/erlabpy/commit/93a4e7c4f43a8133f3f2149eb638261a9d56cfe6))
 
-* docs: fix typo in README ([`2b5e2cf`](https://github.com/kmnhan/erlabpy/commit/2b5e2cf3d5dd9e93d34da578e5689f14d490405b))
+* fix typo in README ([`2b5e2cf`](https://github.com/kmnhan/erlabpy/commit/2b5e2cf3d5dd9e93d34da578e5689f14d490405b))
 
 ### Feature
 
-* feat: add interactive tool to kspace accessor ([`fb91cdb`](https://github.com/kmnhan/erlabpy/commit/fb91cdb50229154c070df8dfaa80cddc8520ae6d))
+* add interactive tool to kspace accessor ([`fb91cdb`](https://github.com/kmnhan/erlabpy/commit/fb91cdb50229154c070df8dfaa80cddc8520ae6d))
 
 ### Refactor
 
-* refactor: accessors are now registered upon package import ([`d79fee2`](https://github.com/kmnhan/erlabpy/commit/d79fee2a28dd5ee59bfc6bd1ce224a44c5f40a24))
+* accessors are now registered upon package import ([`d79fee2`](https://github.com/kmnhan/erlabpy/commit/d79fee2a28dd5ee59bfc6bd1ce224a44c5f40a24))
 
 ### Style
 
-* style: apply linter suggestions ([`fe35da9`](https://github.com/kmnhan/erlabpy/commit/fe35da9a3494af28420ead2d8d40c5339788ac80))
+* apply linter suggestions ([`fe35da9`](https://github.com/kmnhan/erlabpy/commit/fe35da9a3494af28420ead2d8d40c5339788ac80))
 
 
 ## v1.4.1 (2024-03-26)
 
 ### Fix
 
-* fix: update package metadata
+* update package metadata ([`ecfb88f`](https://github.com/kmnhan/erlabpy/commit/ecfb88f2c23a7681e12d6f2dedcc316a28aa22c7))
 
-This should be classified as chore, but commiting as a fix to trigger CI ([`ecfb88f`](https://github.com/kmnhan/erlabpy/commit/ecfb88f2c23a7681e12d6f2dedcc316a28aa22c7))
+  This should be classified as chore, but commiting as a fix to trigger CI
 
 
 ## v1.4.0 (2024-03-26)
 
 ### Chore
 
-* chore: update workflow triggers ([`fb158f3`](https://github.com/kmnhan/erlabpy/commit/fb158f3a6b6ded4ed2d573f4d33f85fbd36809b5))
+* update workflow triggers ([`fb158f3`](https://github.com/kmnhan/erlabpy/commit/fb158f3a6b6ded4ed2d573f4d33f85fbd36809b5))
 
-* chore: update build command ([`a22b8e5`](https://github.com/kmnhan/erlabpy/commit/a22b8e58bb744d02c2e0214af6185da8c66cbe29))
+* update build command ([`a22b8e5`](https://github.com/kmnhan/erlabpy/commit/a22b8e58bb744d02c2e0214af6185da8c66cbe29))
 
-* chore: update CI/CD badge urls ([`db61b29`](https://github.com/kmnhan/erlabpy/commit/db61b29fa0d92f54f7134ce5bd1c021aacfae647))
+* update CI/CD badge urls ([`db61b29`](https://github.com/kmnhan/erlabpy/commit/db61b29fa0d92f54f7134ce5bd1c021aacfae647))
 
-* chore: make pyproject.toml compatible
+* make pyproject.toml compatible ([`959f687`](https://github.com/kmnhan/erlabpy/commit/959f6874f421ddd7bdf816f96c78d1533081b24d))
 
-README file link fixed, and remove direct dependencies.
-Add build command for automatic building ([`959f687`](https://github.com/kmnhan/erlabpy/commit/959f6874f421ddd7bdf816f96c78d1533081b24d))
+  README file link fixed, and remove direct dependencies. Add build command for automatic building
 
-* chore: update workflows to upload to pypi ([`2902b68`](https://github.com/kmnhan/erlabpy/commit/2902b683051ce651be6d5e38c6bdf6e55a9681f1))
+* update workflows to upload to pypi ([`2902b68`](https://github.com/kmnhan/erlabpy/commit/2902b683051ce651be6d5e38c6bdf6e55a9681f1))
 
 ### Documentation
 
-* docs: update docstring and apply linter suggestions ([`de3ee01`](https://github.com/kmnhan/erlabpy/commit/de3ee01dd35973186d69125f24d9527cfa8abd94))
+* update docstring and apply linter suggestions ([`de3ee01`](https://github.com/kmnhan/erlabpy/commit/de3ee01dd35973186d69125f24d9527cfa8abd94))
 
-* docs: update README ([`8bd239f`](https://github.com/kmnhan/erlabpy/commit/8bd239f562d2d2345178c339a455ec23a5aa8082))
+* update README ([`8bd239f`](https://github.com/kmnhan/erlabpy/commit/8bd239f562d2d2345178c339a455ec23a5aa8082))
 
 ### Feature
 
-* feat: calculate kz in MomentumAccessor
+* calculate kz in MomentumAccessor ([`46979f9`](https://github.com/kmnhan/erlabpy/commit/46979f907b120e5a4a88fdacd7d74a4b9dd41d6d))
 
-Add method that calculates kz array from given photon energy float ([`46979f9`](https://github.com/kmnhan/erlabpy/commit/46979f907b120e5a4a88fdacd7d74a4b9dd41d6d))
+  Add method that calculates kz array from given photon energy float
 
-* feat: make momentum conversion functions xarray compatible ([`a7aa34b`](https://github.com/kmnhan/erlabpy/commit/a7aa34ba983d3159c555ed66579d46eaf9e993aa))
+* make momentum conversion functions xarray compatible ([`a7aa34b`](https://github.com/kmnhan/erlabpy/commit/a7aa34ba983d3159c555ed66579d46eaf9e993aa))
 
 
 ## v1.3.1 (2024-03-25)
 
 ### Documentation
 
-* docs: update documentation
+* update documentation ([`69a02fa`](https://github.com/kmnhan/erlabpy/commit/69a02fa3591720cf79b01289fd9dfb9cf55c26db))
 
-- Move rst README contents to docs, replace with newly written markdown.
-- Add screenshot images to  documentation and README ([`69a02fa`](https://github.com/kmnhan/erlabpy/commit/69a02fa3591720cf79b01289fd9dfb9cf55c26db))
+  - Move rst README contents to docs, replace with newly written markdown. - Add screenshot images to  documentation and README
 
-* docs: update README ([`15f61bf`](https://github.com/kmnhan/erlabpy/commit/15f61bfe7a1734cece17479064c6d7946e2701f9))
+* update README ([`15f61bf`](https://github.com/kmnhan/erlabpy/commit/15f61bfe7a1734cece17479064c6d7946e2701f9))
 
 ### Fix
 
-* fix: fixes #12 ([`02b49a1`](https://github.com/kmnhan/erlabpy/commit/02b49a1da7550ae2b07819e6ccde3dcf750fc527))
+* fixes #12 ([`02b49a1`](https://github.com/kmnhan/erlabpy/commit/02b49a1da7550ae2b07819e6ccde3dcf750fc527))
 
 
 ## v1.3.0 (2024-03-25)
 
 ### Chore
 
-* chore: fix wrong branch name in release workflow ([`76a51b8`](https://github.com/kmnhan/erlabpy/commit/76a51b87180065631b6f5ca0678a87dfaa7e267e))
+* fix wrong branch name in release workflow ([`76a51b8`](https://github.com/kmnhan/erlabpy/commit/76a51b87180065631b6f5ca0678a87dfaa7e267e))
 
-* chore: configure semantic release ([`3ebdecb`](https://github.com/kmnhan/erlabpy/commit/3ebdecb45b510ed5e45e25fbc10d58ebc0b4ce20))
+* configure semantic release ([`3ebdecb`](https://github.com/kmnhan/erlabpy/commit/3ebdecb45b510ed5e45e25fbc10d58ebc0b4ce20))
 
-* chore: bump version to 1.2.1 ([`30ec306`](https://github.com/kmnhan/erlabpy/commit/30ec3065234b6f727ed8f74daa1a866b82b0abc7))
+* bump version to 1.2.1 ([`30ec306`](https://github.com/kmnhan/erlabpy/commit/30ec3065234b6f727ed8f74daa1a866b82b0abc7))
 
 ### Documentation
 
-* docs: update README ([`79ba5b4`](https://github.com/kmnhan/erlabpy/commit/79ba5b42f5089d9fd81ccfc69dadda21914b42a7))
+* update README ([`79ba5b4`](https://github.com/kmnhan/erlabpy/commit/79ba5b42f5089d9fd81ccfc69dadda21914b42a7))
 
 ### Feature
 
-* feat(io): add new data loader plugin for DA30 + SES ([`7a27a2f`](https://github.com/kmnhan/erlabpy/commit/7a27a2f27d9658f1091aaa48bcc78dea562898d8))
+* **io** add new data loader plugin for DA30 + SES ([`7a27a2f`](https://github.com/kmnhan/erlabpy/commit/7a27a2f27d9658f1091aaa48bcc78dea562898d8))
 
 ### Fix
 
-* fix(io): properly handle registry getattr
+* **io** properly handle registry getattr ([`499526f`](https://github.com/kmnhan/erlabpy/commit/499526fc1705bfbfbf8d3b80d50d65450dec7eae))
 
-This fixes an issue where _repr_html_ will fallback to __repr__.
-Additionally, `get` will now raise a KeyError instead of a ValueError. ([`499526f`](https://github.com/kmnhan/erlabpy/commit/499526fc1705bfbfbf8d3b80d50d65450dec7eae))
+  This fixes an issue where _repr_html_ will fallback to __repr__. Additionally, `get` will now raise a KeyError instead of a ValueError.
 
 ### Style
 
-* style: adjust loader registry repr ([`1fc31af`](https://github.com/kmnhan/erlabpy/commit/1fc31af083654a6c093bf343a881fcab37f9fbe2))
+* adjust loader registry repr ([`1fc31af`](https://github.com/kmnhan/erlabpy/commit/1fc31af083654a6c093bf343a881fcab37f9fbe2))
 
-* style: remove incorrect type annotation ([`69dbf8a`](https://github.com/kmnhan/erlabpy/commit/69dbf8a1041ab22ea5d928623adae497b5ecd919))
+* remove incorrect type annotation ([`69dbf8a`](https://github.com/kmnhan/erlabpy/commit/69dbf8a1041ab22ea5d928623adae497b5ecd919))
 
 
 ## v1.2.1 (2024-03-25)
 
 ### Build
 
-* build: drop python 3.10 support ([`183769f`](https://github.com/kmnhan/erlabpy/commit/183769f9af371f5e3a910976356ac2ac384c9ebb))
+* drop python 3.10 support ([`183769f`](https://github.com/kmnhan/erlabpy/commit/183769f9af371f5e3a910976356ac2ac384c9ebb))
 
-* build: update pyproject.toml to properly include dependencies ([`d39e69e`](https://github.com/kmnhan/erlabpy/commit/d39e69e7f5a6cf1b9b6088689f1f7756e25edc4f))
+* update pyproject.toml to properly include dependencies ([`d39e69e`](https://github.com/kmnhan/erlabpy/commit/d39e69e7f5a6cf1b9b6088689f1f7756e25edc4f))
 
-* build: update requirements.txt ([`91cac05`](https://github.com/kmnhan/erlabpy/commit/91cac05fdade8c5ce21a9e28d311159f57351ac9))
+* update requirements.txt ([`91cac05`](https://github.com/kmnhan/erlabpy/commit/91cac05fdade8c5ce21a9e28d311159f57351ac9))
 
-* build: update requirements.txt ([`bf2e534`](https://github.com/kmnhan/erlabpy/commit/bf2e5346d4c3030a4ef8061e5f463491725e9f9c))
+* update requirements.txt ([`bf2e534`](https://github.com/kmnhan/erlabpy/commit/bf2e5346d4c3030a4ef8061e5f463491725e9f9c))
 
-* build: bump version ([`a68a6ea`](https://github.com/kmnhan/erlabpy/commit/a68a6ea1e061ffbb6c4ae966a6b23c6710175744))
+* bump version ([`a68a6ea`](https://github.com/kmnhan/erlabpy/commit/a68a6ea1e061ffbb6c4ae966a6b23c6710175744))
 
-* build: bump version to 1.1.0 ([`791af02`](https://github.com/kmnhan/erlabpy/commit/791af027a4e3ebf3cbad4bcb9af490986a2be2c0))
+* bump version to 1.1.0 ([`791af02`](https://github.com/kmnhan/erlabpy/commit/791af027a4e3ebf3cbad4bcb9af490986a2be2c0))
 
-* build: bump setuptools minver ([`b55da17`](https://github.com/kmnhan/erlabpy/commit/b55da17c30ec94e897cf2ee8abf151796f3f78b7))
+* bump setuptools minver ([`b55da17`](https://github.com/kmnhan/erlabpy/commit/b55da17c30ec94e897cf2ee8abf151796f3f78b7))
 
-* build: try automatic discovery ([`05040e3`](https://github.com/kmnhan/erlabpy/commit/05040e3f98b6094258d4a7be7a33feeefa1fd44b))
+* try automatic discovery ([`05040e3`](https://github.com/kmnhan/erlabpy/commit/05040e3f98b6094258d4a7be7a33feeefa1fd44b))
 
-* build: modify to updated directory structure ([`625ffcf`](https://github.com/kmnhan/erlabpy/commit/625ffcf2eb5a2914024efd815de40a910b1ae040))
+* modify to updated directory structure ([`625ffcf`](https://github.com/kmnhan/erlabpy/commit/625ffcf2eb5a2914024efd815de40a910b1ae040))
 
-* build: add setuptools-scm as build dependency ([`4ff4791`](https://github.com/kmnhan/erlabpy/commit/4ff47910022571d0d37ddc923755705dfa8a549e))
+* add setuptools-scm as build dependency ([`4ff4791`](https://github.com/kmnhan/erlabpy/commit/4ff47910022571d0d37ddc923755705dfa8a549e))
 
-* build: fix typo in requirements.txt ([`29571de`](https://github.com/kmnhan/erlabpy/commit/29571de3bec9a9bbbcdff850b34e6caec167a109))
+* fix typo in requirements.txt ([`29571de`](https://github.com/kmnhan/erlabpy/commit/29571de3bec9a9bbbcdff850b34e6caec167a109))
 
-* build: update README, remove setup.cfg and update pyproject.toml ([`3736f46`](https://github.com/kmnhan/erlabpy/commit/3736f4629621d036ec071f27b0660bf7e99f8e86))
+* update README, remove setup.cfg and update pyproject.toml ([`3736f46`](https://github.com/kmnhan/erlabpy/commit/3736f4629621d036ec071f27b0660bf7e99f8e86))
 
-* build: add reqquirements.txt ([`dacd5be`](https://github.com/kmnhan/erlabpy/commit/dacd5be9985e28d1c67ac46d2badd24f148d4062))
+* add reqquirements.txt ([`dacd5be`](https://github.com/kmnhan/erlabpy/commit/dacd5be9985e28d1c67ac46d2badd24f148d4062))
 
-* build: add yml file for intel ([`4844091`](https://github.com/kmnhan/erlabpy/commit/48440915782e1e8b918c88e4d9dce38b9703e43c))
+* add yml file for intel ([`4844091`](https://github.com/kmnhan/erlabpy/commit/48440915782e1e8b918c88e4d9dce38b9703e43c))
 
-* build: update readme type ([`40cf807`](https://github.com/kmnhan/erlabpy/commit/40cf807e522a59e9aad8ff6196788fe58846584b))
+* update readme type ([`40cf807`](https://github.com/kmnhan/erlabpy/commit/40cf807e522a59e9aad8ff6196788fe58846584b))
 
-* build: update dependencies ([`e1bb13a`](https://github.com/kmnhan/erlabpy/commit/e1bb13ae6a350adf51e1b08ebe83f2732d1797f8))
+* update dependencies ([`e1bb13a`](https://github.com/kmnhan/erlabpy/commit/e1bb13ae6a350adf51e1b08ebe83f2732d1797f8))
 
-* build: update instructions, cleanup dependencies ([`66d0e25`](https://github.com/kmnhan/erlabpy/commit/66d0e25d07393dc4b16a4d5e5994ea4fa822dd33))
+* update instructions, cleanup dependencies ([`66d0e25`](https://github.com/kmnhan/erlabpy/commit/66d0e25d07393dc4b16a4d5e5994ea4fa822dd33))
 
-* build: add yml for intel ([`8db3b26`](https://github.com/kmnhan/erlabpy/commit/8db3b269544c2f086f98fa302beb594f10573f65))
+* add yml for intel ([`8db3b26`](https://github.com/kmnhan/erlabpy/commit/8db3b269544c2f086f98fa302beb594f10573f65))
 
-* build: update dependencies ([`21e8fab`](https://github.com/kmnhan/erlabpy/commit/21e8fabc2896d2b1fac5d2567eecf2df63047fe4))
+* update dependencies ([`21e8fab`](https://github.com/kmnhan/erlabpy/commit/21e8fabc2896d2b1fac5d2567eecf2df63047fe4))
 
-* build: update dependencies ([`88a0170`](https://github.com/kmnhan/erlabpy/commit/88a01706b4f49d3b56f017badfd69af63df897f9))
+* update dependencies ([`88a0170`](https://github.com/kmnhan/erlabpy/commit/88a01706b4f49d3b56f017badfd69af63df897f9))
 
-* build: update dependencies
-dropped python 3.9 support (temporary) ([`832e1ed`](https://github.com/kmnhan/erlabpy/commit/832e1ed25c299f7838dee1bc3d862a43ffe0bbb7))
+* update dependencies ([`832e1ed`](https://github.com/kmnhan/erlabpy/commit/832e1ed25c299f7838dee1bc3d862a43ffe0bbb7))
 
-* build: update requirements ([`fe26fc2`](https://github.com/kmnhan/erlabpy/commit/fe26fc2d17e4c107ef9b9a2773ce6c6318e18b2e))
+* update requirements ([`fe26fc2`](https://github.com/kmnhan/erlabpy/commit/fe26fc2d17e4c107ef9b9a2773ce6c6318e18b2e))
 
-* build: refactor requirements ([`81d3038`](https://github.com/kmnhan/erlabpy/commit/81d3038b03a717cf18fff655dba4224a7e67570a))
+* refactor requirements ([`81d3038`](https://github.com/kmnhan/erlabpy/commit/81d3038b03a717cf18fff655dba4224a7e67570a))
 
-* build: add environment.yml for conda env ([`ea7bbf4`](https://github.com/kmnhan/erlabpy/commit/ea7bbf4309efeecd0ed1dcbd1791e482ab4d3ced))
+* add environment.yml for conda env ([`ea7bbf4`](https://github.com/kmnhan/erlabpy/commit/ea7bbf4309efeecd0ed1dcbd1791e482ab4d3ced))
 
-* build: fix dependencies ([`e344f99`](https://github.com/kmnhan/erlabpy/commit/e344f990e55e7ddcc7e6ef5c87999d2c777b44a5))
+* fix dependencies ([`e344f99`](https://github.com/kmnhan/erlabpy/commit/e344f990e55e7ddcc7e6ef5c87999d2c777b44a5))
 
-* build: fix dependencies ([`5a6e38c`](https://github.com/kmnhan/erlabpy/commit/5a6e38c8de1f554819aa74d9e9e5a4f4524a2f6f))
+* fix dependencies ([`5a6e38c`](https://github.com/kmnhan/erlabpy/commit/5a6e38c8de1f554819aa74d9e9e5a4f4524a2f6f))
 
 ### Chore
 
-* chore: update .gitignore ([`a4b2cbc`](https://github.com/kmnhan/erlabpy/commit/a4b2cbc322a4e031d75db87e87e7d532c585709f))
+* update .gitignore ([`a4b2cbc`](https://github.com/kmnhan/erlabpy/commit/a4b2cbc322a4e031d75db87e87e7d532c585709f))
 
-* chore: update .gitignore ([`221b623`](https://github.com/kmnhan/erlabpy/commit/221b6232a6dc39b42ac1a3fd1a5abd0e2f1441d4))
+* update .gitignore ([`221b623`](https://github.com/kmnhan/erlabpy/commit/221b6232a6dc39b42ac1a3fd1a5abd0e2f1441d4))
 
-* chore: add some type hints remove deprecated ([`79d7349`](https://github.com/kmnhan/erlabpy/commit/79d7349953a1747e177796d14da44dbed5b02874))
+* add some type hints remove deprecated ([`79d7349`](https://github.com/kmnhan/erlabpy/commit/79d7349953a1747e177796d14da44dbed5b02874))
 
 ### Ci
 
-* ci: update flake8 args ([`d720ee2`](https://github.com/kmnhan/erlabpy/commit/d720ee2b27df60fb42eca954ae7691641669828d))
+* update flake8 args ([`d720ee2`](https://github.com/kmnhan/erlabpy/commit/d720ee2b27df60fb42eca954ae7691641669828d))
 
-* ci: install qt runtime dependency ([`9e18d14`](https://github.com/kmnhan/erlabpy/commit/9e18d1499cddf987f8d267d8f358646b2a23ae32))
+* install qt runtime dependency ([`9e18d14`](https://github.com/kmnhan/erlabpy/commit/9e18d1499cddf987f8d267d8f358646b2a23ae32))
 
-* ci: create test.yml ([`c788eef`](https://github.com/kmnhan/erlabpy/commit/c788eef6025382a744d944e9e64c38b935324158))
+* create test.yml ([`c788eef`](https://github.com/kmnhan/erlabpy/commit/c788eef6025382a744d944e9e64c38b935324158))
 
 ### Documentation
 
-* docs: update docstring
+* update docstring ([`f7bf9cb`](https://github.com/kmnhan/erlabpy/commit/f7bf9cb2f51fc8a57aa9a84b2c690b06cd029ec8))
 
-Changed configuration so that type annotations appear in both the signature and the description. ([`f7bf9cb`](https://github.com/kmnhan/erlabpy/commit/f7bf9cb2f51fc8a57aa9a84b2c690b06cd029ec8))
+  Changed configuration so that type annotations appear in both the signature and the description.
 
-* docs: update plotting examples with display_expand_data=False ([`79117c4`](https://github.com/kmnhan/erlabpy/commit/79117c4814d66dd5dc3d7cfc85af8f9b662651bf))
+* update plotting examples with display_expand_data=False ([`79117c4`](https://github.com/kmnhan/erlabpy/commit/79117c4814d66dd5dc3d7cfc85af8f9b662651bf))
 
-* docs: update dosctring ([`2eccbf3`](https://github.com/kmnhan/erlabpy/commit/2eccbf3b18b7c52250b52c958cf5899fd05ea9a4))
+* update dosctring ([`2eccbf3`](https://github.com/kmnhan/erlabpy/commit/2eccbf3b18b7c52250b52c958cf5899fd05ea9a4))
 
-* docs: update docstring ([`4e8be19`](https://github.com/kmnhan/erlabpy/commit/4e8be19c1153d816e06d41d446bef7d057a4eb9b))
+* update docstring ([`4e8be19`](https://github.com/kmnhan/erlabpy/commit/4e8be19c1153d816e06d41d446bef7d057a4eb9b))
 
-* docs: add link to api reference in guide ([`e750519`](https://github.com/kmnhan/erlabpy/commit/e750519f3936ad4b7d4d532daebbe72c1b35f3d3))
+* add link to api reference in guide ([`e750519`](https://github.com/kmnhan/erlabpy/commit/e750519f3936ad4b7d4d532daebbe72c1b35f3d3))
 
-* docs: add update instructions ([`71bb0c6`](https://github.com/kmnhan/erlabpy/commit/71bb0c66815eef6acf1222c1f6e1081b753db493))
+* add update instructions ([`71bb0c6`](https://github.com/kmnhan/erlabpy/commit/71bb0c66815eef6acf1222c1f6e1081b753db493))
 
-* docs: update installation instructions ([`64f9a3b`](https://github.com/kmnhan/erlabpy/commit/64f9a3bf39a4c0ef49fd23ead37e34bf7a94f620))
+* update installation instructions ([`64f9a3b`](https://github.com/kmnhan/erlabpy/commit/64f9a3bf39a4c0ef49fd23ead37e34bf7a94f620))
 
-* docs: update README ([`428ea67`](https://github.com/kmnhan/erlabpy/commit/428ea671748f7062872533603b954ed27933a72a))
+* update README ([`428ea67`](https://github.com/kmnhan/erlabpy/commit/428ea671748f7062872533603b954ed27933a72a))
 
-* docs: cleanup top-level headers ([`39e9fcf`](https://github.com/kmnhan/erlabpy/commit/39e9fcf8962f0282902a90595d52a7d576fe35dd))
+* cleanup top-level headers ([`39e9fcf`](https://github.com/kmnhan/erlabpy/commit/39e9fcf8962f0282902a90595d52a7d576fe35dd))
 
-* docs: update documentation
+* update documentation ([`32ca369`](https://github.com/kmnhan/erlabpy/commit/32ca369ee6238696792229b63a29c27aa4060ddc))
 
-Cleanup header styles and add cards to index page ([`32ca369`](https://github.com/kmnhan/erlabpy/commit/32ca369ee6238696792229b63a29c27aa4060ddc))
+  Cleanup header styles and add cards to index page
 
-* docs: update docstrings for some functions ([`d6a8e7d`](https://github.com/kmnhan/erlabpy/commit/d6a8e7d408d795586bd6b6bc6fc6d4f48443a853))
+* update docstrings for some functions ([`d6a8e7d`](https://github.com/kmnhan/erlabpy/commit/d6a8e7d408d795586bd6b6bc6fc6d4f48443a853))
 
-* docs: cleanup conf.py ([`eab5e60`](https://github.com/kmnhan/erlabpy/commit/eab5e6078850de71c447cc1aa42b266bc10caf3b))
+* cleanup conf.py ([`eab5e60`](https://github.com/kmnhan/erlabpy/commit/eab5e6078850de71c447cc1aa42b266bc10caf3b))
 
-* docs: update documentation ([`e03d118`](https://github.com/kmnhan/erlabpy/commit/e03d1182f294ef909b03ff04ea3d805349304bc1))
+* update documentation ([`e03d118`](https://github.com/kmnhan/erlabpy/commit/e03d1182f294ef909b03ff04ea3d805349304bc1))
 
-* docs: update to use bibtex ([`c571b11`](https://github.com/kmnhan/erlabpy/commit/c571b11774c2dc2c152ccace4953976ad29600ef))
+* update to use bibtex ([`c571b11`](https://github.com/kmnhan/erlabpy/commit/c571b11774c2dc2c152ccace4953976ad29600ef))
 
-* docs: update accessor docstring ([`d32f352`](https://github.com/kmnhan/erlabpy/commit/d32f35283208b6fbc72264a8f966beef4c39e0c9))
+* update accessor docstring ([`d32f352`](https://github.com/kmnhan/erlabpy/commit/d32f35283208b6fbc72264a8f966beef4c39e0c9))
 
-* docs: update documentation ([`ec7a47e`](https://github.com/kmnhan/erlabpy/commit/ec7a47e28eee265ec01a66419fd32412ed565ba2))
+* update documentation ([`ec7a47e`](https://github.com/kmnhan/erlabpy/commit/ec7a47e28eee265ec01a66419fd32412ed565ba2))
 
-* docs: update documentation ([`0390eb3`](https://github.com/kmnhan/erlabpy/commit/0390eb37d758459a83cbb20b9d567d6f4937619d))
+* update documentation ([`0390eb3`](https://github.com/kmnhan/erlabpy/commit/0390eb37d758459a83cbb20b9d567d6f4937619d))
 
-* docs: update documentation ([`a7bfea2`](https://github.com/kmnhan/erlabpy/commit/a7bfea28f2f9cef1a32d591d3ebbf32c0d968450))
+* update documentation ([`a7bfea2`](https://github.com/kmnhan/erlabpy/commit/a7bfea28f2f9cef1a32d591d3ebbf32c0d968450))
 
-* docs: update docstring to use PEP annotation ([`fc496df`](https://github.com/kmnhan/erlabpy/commit/fc496df1a9efe0ca345a183decdddaf54cdb0cc6))
+* update docstring to use PEP annotation ([`fc496df`](https://github.com/kmnhan/erlabpy/commit/fc496df1a9efe0ca345a183decdddaf54cdb0cc6))
 
-* docs: add copybutton ([`5e14247`](https://github.com/kmnhan/erlabpy/commit/5e142478568d17e4160f7ea52b99fa4b15a75b0d))
+* add copybutton ([`5e14247`](https://github.com/kmnhan/erlabpy/commit/5e142478568d17e4160f7ea52b99fa4b15a75b0d))
 
-* docs: update docstring ([`9b9eaff`](https://github.com/kmnhan/erlabpy/commit/9b9eaff437f39e4b684a2e1ef1f0d91a2762507b))
+* update docstring ([`9b9eaff`](https://github.com/kmnhan/erlabpy/commit/9b9eaff437f39e4b684a2e1ef1f0d91a2762507b))
 
-* docs: use default font for docs plot generation ([`d36ce1d`](https://github.com/kmnhan/erlabpy/commit/d36ce1d5687168958da9cd33c9e225a52443c6ef))
+* use default font for docs plot generation ([`d36ce1d`](https://github.com/kmnhan/erlabpy/commit/d36ce1d5687168958da9cd33c9e225a52443c6ef))
 
-* docs: revert to pip due to slow build time, keep at py311 until 3.12.2 is available ([`954f357`](https://github.com/kmnhan/erlabpy/commit/954f3573e578da9a73a3256011b9016df01f6f30))
+* revert to pip due to slow build time, keep at py311 until 3.12.2 is available ([`954f357`](https://github.com/kmnhan/erlabpy/commit/954f3573e578da9a73a3256011b9016df01f6f30))
 
-* docs: build with conda ([`d2b8c40`](https://github.com/kmnhan/erlabpy/commit/d2b8c408d75c5d1dcedef6f7cfbdd12d93a57d34))
+* build with conda ([`d2b8c40`](https://github.com/kmnhan/erlabpy/commit/d2b8c408d75c5d1dcedef6f7cfbdd12d93a57d34))
 
-* docs: retry build with py312 ([`bb12503`](https://github.com/kmnhan/erlabpy/commit/bb12503c5c6d67166a78de986df70778902c65cf))
+* retry build with py312 ([`bb12503`](https://github.com/kmnhan/erlabpy/commit/bb12503c5c6d67166a78de986df70778902c65cf))
 
-* docs: update requirements.txt ([`0b2eaad`](https://github.com/kmnhan/erlabpy/commit/0b2eaad96ff270d688f7b0549f57f8a753730b38))
+* update requirements.txt ([`0b2eaad`](https://github.com/kmnhan/erlabpy/commit/0b2eaad96ff270d688f7b0549f57f8a753730b38))
 
-* docs: Add varname to requirements.txt ([`90df11e`](https://github.com/kmnhan/erlabpy/commit/90df11e1dd07ac8c3ea009b0b6c98d42014910d7))
+* Add varname to requirements.txt ([`90df11e`](https://github.com/kmnhan/erlabpy/commit/90df11e1dd07ac8c3ea009b0b6c98d42014910d7))
 
-* docs: Add h5netcdf to requirements.txt ([`6be918c`](https://github.com/kmnhan/erlabpy/commit/6be918c905f463dc171c9df63065f0e87bd1811f))
+* Add h5netcdf to requirements.txt ([`6be918c`](https://github.com/kmnhan/erlabpy/commit/6be918c905f463dc171c9df63065f0e87bd1811f))
 
-* docs: try build with py311 ([`233553d`](https://github.com/kmnhan/erlabpy/commit/233553d56d7d83692c4b9a9e7a35848554e21846))
+* try build with py311 ([`233553d`](https://github.com/kmnhan/erlabpy/commit/233553d56d7d83692c4b9a9e7a35848554e21846))
 
-* docs: comment out code for latex generation and add new dependencies ([`ad9b974`](https://github.com/kmnhan/erlabpy/commit/ad9b97470ea45c7f1abc3e3ccaeccc5f761e5fc1))
+* comment out code for latex generation and add new dependencies ([`ad9b974`](https://github.com/kmnhan/erlabpy/commit/ad9b97470ea45c7f1abc3e3ccaeccc5f761e5fc1))
 
-* docs: update requirements ([`fde56f2`](https://github.com/kmnhan/erlabpy/commit/fde56f2c7ac7c146dac0a28e76decfc250d400dc))
+* update requirements ([`fde56f2`](https://github.com/kmnhan/erlabpy/commit/fde56f2c7ac7c146dac0a28e76decfc250d400dc))
 
-* docs: Add Sphinx documentation dependencies ([`11d200e`](https://github.com/kmnhan/erlabpy/commit/11d200e113a54c047acaccd430f90da6e9c19f1f))
+* Add Sphinx documentation dependencies ([`11d200e`](https://github.com/kmnhan/erlabpy/commit/11d200e113a54c047acaccd430f90da6e9c19f1f))
 
-* docs: Add .readthedocs.yaml and docs/requirements.txt files ([`9296c71`](https://github.com/kmnhan/erlabpy/commit/9296c710fb082442bc4226b82f383e4e6fddf45c))
+* Add .readthedocs.yaml and docs/requirements.txt files ([`9296c71`](https://github.com/kmnhan/erlabpy/commit/9296c710fb082442bc4226b82f383e4e6fddf45c))
 
-* docs: update documentation ([`fd5fc1a`](https://github.com/kmnhan/erlabpy/commit/fd5fc1a616e4b76b6cd37e3065f58e49e94b53b5))
+* update documentation ([`fd5fc1a`](https://github.com/kmnhan/erlabpy/commit/fd5fc1a616e4b76b6cd37e3065f58e49e94b53b5))
 
-* docs: Add figmpl_directive to extensions in conf.py ([`3ca728f`](https://github.com/kmnhan/erlabpy/commit/3ca728f0aa2d6904c8bf31791275992b27ce1ebe))
+* Add figmpl_directive to extensions in conf.py ([`3ca728f`](https://github.com/kmnhan/erlabpy/commit/3ca728f0aa2d6904c8bf31791275992b27ce1ebe))
 
-* docs: update documentation ([`fa312c0`](https://github.com/kmnhan/erlabpy/commit/fa312c05cc9dabb858d9268808b3efd2bead1a3e))
+* update documentation ([`fa312c0`](https://github.com/kmnhan/erlabpy/commit/fa312c05cc9dabb858d9268808b3efd2bead1a3e))
 
-* docs: update documentation ([`2e4e573`](https://github.com/kmnhan/erlabpy/commit/2e4e5736cec670f51e55e81db603c82b98a9e78b))
+* update documentation ([`2e4e573`](https://github.com/kmnhan/erlabpy/commit/2e4e5736cec670f51e55e81db603c82b98a9e78b))
 
-* docs: add some comments ([`e66bc31`](https://github.com/kmnhan/erlabpy/commit/e66bc31cd9f9905a16a94f3b491170556b29adbc))
+* add some comments ([`e66bc31`](https://github.com/kmnhan/erlabpy/commit/e66bc31cd9f9905a16a94f3b491170556b29adbc))
 
-* docs(itool): improve tooltip ([`97ad19b`](https://github.com/kmnhan/erlabpy/commit/97ad19b1581613b6eb7012d4e04d79209f12075d))
+* **itool** improve tooltip ([`97ad19b`](https://github.com/kmnhan/erlabpy/commit/97ad19b1581613b6eb7012d4e04d79209f12075d))
 
-* docs: update docstring ([`700a9a3`](https://github.com/kmnhan/erlabpy/commit/700a9a3982ddcd16756efacb53bd5be861f7ed18))
+* update docstring ([`700a9a3`](https://github.com/kmnhan/erlabpy/commit/700a9a3982ddcd16756efacb53bd5be861f7ed18))
 
-* docs: update documentation ([`e12b9af`](https://github.com/kmnhan/erlabpy/commit/e12b9afc1750823db4edb8034f4b225e51460cca))
+* update documentation ([`e12b9af`](https://github.com/kmnhan/erlabpy/commit/e12b9afc1750823db4edb8034f4b225e51460cca))
 
-* docs: update docstring and formatting ([`dc8e544`](https://github.com/kmnhan/erlabpy/commit/dc8e54415fd26090782075847fd78fa942f7efca))
+* update docstring and formatting ([`dc8e544`](https://github.com/kmnhan/erlabpy/commit/dc8e54415fd26090782075847fd78fa942f7efca))
 
-* docs: update docstring ([`9d7139c`](https://github.com/kmnhan/erlabpy/commit/9d7139ceb90676189e300479d7775c26a4c107ed))
+* update docstring ([`9d7139c`](https://github.com/kmnhan/erlabpy/commit/9d7139ceb90676189e300479d7775c26a4c107ed))
 
-* docs: update README ([`8ca11fe`](https://github.com/kmnhan/erlabpy/commit/8ca11fec492fd1b29737cec5df3dc8535e23b9bb))
+* update README ([`8ca11fe`](https://github.com/kmnhan/erlabpy/commit/8ca11fec492fd1b29737cec5df3dc8535e23b9bb))
 
-* docs: update documentation ([`dc857f7`](https://github.com/kmnhan/erlabpy/commit/dc857f73931413a40eb1b14cced16dda9fe5f4c8))
+* update documentation ([`dc857f7`](https://github.com/kmnhan/erlabpy/commit/dc857f73931413a40eb1b14cced16dda9fe5f4c8))
 
-* docs: update documentation ([`dec0b39`](https://github.com/kmnhan/erlabpy/commit/dec0b39a4d6182af688f7030f88e747cab7b255d))
+* update documentation ([`dec0b39`](https://github.com/kmnhan/erlabpy/commit/dec0b39a4d6182af688f7030f88e747cab7b255d))
 
-* docs: update documentation ([`01d0cb4`](https://github.com/kmnhan/erlabpy/commit/01d0cb4a868076e4e60851a58606df6d5b00ba4e))
+* update documentation ([`01d0cb4`](https://github.com/kmnhan/erlabpy/commit/01d0cb4a868076e4e60851a58606df6d5b00ba4e))
 
-* docs: update documentation ([`cd914c6`](https://github.com/kmnhan/erlabpy/commit/cd914c650b651ad97ce6f4083c999c5251be02fc))
+* update documentation ([`cd914c6`](https://github.com/kmnhan/erlabpy/commit/cd914c650b651ad97ce6f4083c999c5251be02fc))
 
-* docs: update documentation ([`1944109`](https://github.com/kmnhan/erlabpy/commit/194410948df009ea56c91b4fbacafd5dd07f6537))
+* update documentation ([`1944109`](https://github.com/kmnhan/erlabpy/commit/194410948df009ea56c91b4fbacafd5dd07f6537))
 
-* docs: update documentation ([`83615f6`](https://github.com/kmnhan/erlabpy/commit/83615f67bc27ee8d1bf9dcf2a2fd3a9e62b1ef51))
+* update documentation ([`83615f6`](https://github.com/kmnhan/erlabpy/commit/83615f67bc27ee8d1bf9dcf2a2fd3a9e62b1ef51))
 
-* docs: update documentation ([`c28e6c4`](https://github.com/kmnhan/erlabpy/commit/c28e6c4e52817ed2cdec7f7902529bb7f99b829a))
+* update documentation ([`c28e6c4`](https://github.com/kmnhan/erlabpy/commit/c28e6c4e52817ed2cdec7f7902529bb7f99b829a))
 
-* docs: update documentation ([`0577134`](https://github.com/kmnhan/erlabpy/commit/05771342c12225536328c5bb959ff4bc1898ee34))
+* update documentation ([`0577134`](https://github.com/kmnhan/erlabpy/commit/05771342c12225536328c5bb959ff4bc1898ee34))
 
-* docs: update README ([`ccd3c05`](https://github.com/kmnhan/erlabpy/commit/ccd3c05c9a46110b3b740ea0ee061cf8ba595661))
+* update README ([`ccd3c05`](https://github.com/kmnhan/erlabpy/commit/ccd3c05c9a46110b3b740ea0ee061cf8ba595661))
 
-* docs: update documentation ([`e4df36f`](https://github.com/kmnhan/erlabpy/commit/e4df36f98c0031cd5a25738fa4698fd77836e79b))
+* update documentation ([`e4df36f`](https://github.com/kmnhan/erlabpy/commit/e4df36f98c0031cd5a25738fa4698fd77836e79b))
 
-* docs: update documentation ([`5388383`](https://github.com/kmnhan/erlabpy/commit/5388383fd27be899d9e749e3cf3423c3e9a07e0c))
+* update documentation ([`5388383`](https://github.com/kmnhan/erlabpy/commit/5388383fd27be899d9e749e3cf3423c3e9a07e0c))
 
-* docs: update docstring ([`793f1de`](https://github.com/kmnhan/erlabpy/commit/793f1de1b1be734343f7c67a2d59f93a955adeac))
+* update docstring ([`793f1de`](https://github.com/kmnhan/erlabpy/commit/793f1de1b1be734343f7c67a2d59f93a955adeac))
 
-* docs: update documentation ([`1ff5855`](https://github.com/kmnhan/erlabpy/commit/1ff5855f70b33e47034c03347e6d531f5553b431))
+* update documentation ([`1ff5855`](https://github.com/kmnhan/erlabpy/commit/1ff5855f70b33e47034c03347e6d531f5553b431))
 
-* docs: update documentation ([`d01edcb`](https://github.com/kmnhan/erlabpy/commit/d01edcbffeb38d0e9473e865053f52d646bfda55))
+* update documentation ([`d01edcb`](https://github.com/kmnhan/erlabpy/commit/d01edcbffeb38d0e9473e865053f52d646bfda55))
 
-* docs: update docstring ([`d9df4f6`](https://github.com/kmnhan/erlabpy/commit/d9df4f67d596cde8efed7bb5a07451be2eb8924b))
+* update docstring ([`d9df4f6`](https://github.com/kmnhan/erlabpy/commit/d9df4f67d596cde8efed7bb5a07451be2eb8924b))
 
-* docs: update documentation ([`00a9472`](https://github.com/kmnhan/erlabpy/commit/00a947298a42c857574a0f1fa0c8a10c1e02dd27))
+* update documentation ([`00a9472`](https://github.com/kmnhan/erlabpy/commit/00a947298a42c857574a0f1fa0c8a10c1e02dd27))
 
-* docs: update README ([`7f62e74`](https://github.com/kmnhan/erlabpy/commit/7f62e7416ad2514372379f0d8a0a33c2946848af))
+* update README ([`7f62e74`](https://github.com/kmnhan/erlabpy/commit/7f62e7416ad2514372379f0d8a0a33c2946848af))
 
-* docs: update README ([`f774da7`](https://github.com/kmnhan/erlabpy/commit/f774da73f7bf11cc2b2c6740552fb6f53acb2bb9))
+* update README ([`f774da7`](https://github.com/kmnhan/erlabpy/commit/f774da73f7bf11cc2b2c6740552fb6f53acb2bb9))
 
-* docs: update README ([`e1aa11d`](https://github.com/kmnhan/erlabpy/commit/e1aa11dedba93636431b761160d883e36189050e))
+* update README ([`e1aa11d`](https://github.com/kmnhan/erlabpy/commit/e1aa11dedba93636431b761160d883e36189050e))
 
-* docs: update docstring ([`ee31e1f`](https://github.com/kmnhan/erlabpy/commit/ee31e1fe997c245981057c59a602fe1b7a253501))
+* update docstring ([`ee31e1f`](https://github.com/kmnhan/erlabpy/commit/ee31e1fe997c245981057c59a602fe1b7a253501))
 
-* docs: update docstring ([`b32e92f`](https://github.com/kmnhan/erlabpy/commit/b32e92f0cee5c5aa2b7793a17d95c21ff49ce94d))
+* update docstring ([`b32e92f`](https://github.com/kmnhan/erlabpy/commit/b32e92f0cee5c5aa2b7793a17d95c21ff49ce94d))
 
 ### Feature
 
-* feat(gold): apply automatic weights proportional to sqrt(count) on edge fit ([`717b9c8`](https://github.com/kmnhan/erlabpy/commit/717b9c814ce6fd38567695adb515973e6097ec50))
+* **gold** apply automatic weights proportional to sqrt(count) on edge fit ([`717b9c8`](https://github.com/kmnhan/erlabpy/commit/717b9c814ce6fd38567695adb515973e6097ec50))
 
-* feat: add class to handle momentum conversion offsets ([`15416e5`](https://github.com/kmnhan/erlabpy/commit/15416e5aeca748225e35659c65dcc07b82b40007))
+* add class to handle momentum conversion offsets ([`15416e5`](https://github.com/kmnhan/erlabpy/commit/15416e5aeca748225e35659c65dcc07b82b40007))
 
-* feat: add translation layer between lmfit models and iminuit ([`0f2f894`](https://github.com/kmnhan/erlabpy/commit/0f2f894994a00714e50e934dd4d5b518540539df))
+* add translation layer between lmfit models and iminuit ([`0f2f894`](https://github.com/kmnhan/erlabpy/commit/0f2f894994a00714e50e934dd4d5b518540539df))
 
-* feat: include all cmaps by default ([`3afe72e`](https://github.com/kmnhan/erlabpy/commit/3afe72ece2474c9adcfb89cb5037c50af2e2f0e5))
+* include all cmaps by default ([`3afe72e`](https://github.com/kmnhan/erlabpy/commit/3afe72ece2474c9adcfb89cb5037c50af2e2f0e5))
 
-* feat: change default colormap to CET-L20 ([`274122a`](https://github.com/kmnhan/erlabpy/commit/274122a4b2e582a24385c4dd748206ae0165b4b8))
+* change default colormap to CET-L20 ([`274122a`](https://github.com/kmnhan/erlabpy/commit/274122a4b2e582a24385c4dd748206ae0165b4b8))
 
-* feat(goldtool): can access fit result after window close ([`4c9f232`](https://github.com/kmnhan/erlabpy/commit/4c9f232adfde874d975f033dc9bdcc8bf4969787))
+* **goldtool** can access fit result after window close ([`4c9f232`](https://github.com/kmnhan/erlabpy/commit/4c9f232adfde874d975f033dc9bdcc8bf4969787))
 
-* feat(io): style summary ([`6919929`](https://github.com/kmnhan/erlabpy/commit/6919929815401aa5d6ee4a37398c0593fab3657d))
+* **io** style summary ([`6919929`](https://github.com/kmnhan/erlabpy/commit/6919929815401aa5d6ee4a37398c0593fab3657d))
 
-* feat(io): summarize will now default to set directory ([`ca5b65a`](https://github.com/kmnhan/erlabpy/commit/ca5b65a0e850058837945b7f53864cfc6b32e933))
+* **io** summarize will now default to set directory ([`ca5b65a`](https://github.com/kmnhan/erlabpy/commit/ca5b65a0e850058837945b7f53864cfc6b32e933))
 
-* feat(constants): add neutron mass ([`379ef37`](https://github.com/kmnhan/erlabpy/commit/379ef3705eb2f952121c92c9b653f2ca715618ee))
+* **constants** add neutron mass ([`379ef37`](https://github.com/kmnhan/erlabpy/commit/379ef3705eb2f952121c92c9b653f2ca715618ee))
 
-* feat(io): make loaders accessible with __getattr__ ([`b4884e4`](https://github.com/kmnhan/erlabpy/commit/b4884e4989c3565fdeccb8e18ec6a840cc67a7d2))
+* **io** make loaders accessible with __getattr__ ([`b4884e4`](https://github.com/kmnhan/erlabpy/commit/b4884e4989c3565fdeccb8e18ec6a840cc67a7d2))
 
-* feat(io): add loader plugin for SSRL Beamline 5-2 ([`67ced64`](https://github.com/kmnhan/erlabpy/commit/67ced64352e0f071fad5ebe441348108b6834784))
+* **io** add loader plugin for SSRL Beamline 5-2 ([`67ced64`](https://github.com/kmnhan/erlabpy/commit/67ced64352e0f071fad5ebe441348108b6834784))
 
-* feat(io): show full table on summary in ipython ([`985046f`](https://github.com/kmnhan/erlabpy/commit/985046f8a13911dc2c0be7cc68e530e93de37683))
+* **io** show full table on summary in ipython ([`985046f`](https://github.com/kmnhan/erlabpy/commit/985046f8a13911dc2c0be7cc68e530e93de37683))
 
-* feat(io.dataloader): allow loaders to specify mapping dictionary on cut postprocessing ([`73abb0d`](https://github.com/kmnhan/erlabpy/commit/73abb0d1a078779130e6f82fadc9f44e62619799))
+* **io.dataloader** allow loaders to specify mapping dictionary on cut postprocessing ([`73abb0d`](https://github.com/kmnhan/erlabpy/commit/73abb0d1a078779130e6f82fadc9f44e62619799))
 
-* feat(io): new arg to get_files ([`a9be216`](https://github.com/kmnhan/erlabpy/commit/a9be2165b61082956d5118c328e6484bdd0694c5))
+* **io** new arg to get_files ([`a9be216`](https://github.com/kmnhan/erlabpy/commit/a9be2165b61082956d5118c328e6484bdd0694c5))
 
-* feat(io.igor): remove dependency on find_first_file ([`1d95292`](https://github.com/kmnhan/erlabpy/commit/1d95292ff4ba1c6ad5fcc95cae2d36c452d52ecf))
+* **io.igor** remove dependency on find_first_file ([`1d95292`](https://github.com/kmnhan/erlabpy/commit/1d95292ff4ba1c6ad5fcc95cae2d36c452d52ecf))
 
-* feat(io): dataloader now preserves more attributes ([`f1157ba`](https://github.com/kmnhan/erlabpy/commit/f1157ba7afcb0b259932062edb0dc2138c749c55))
+* **io** dataloader now preserves more attributes ([`f1157ba`](https://github.com/kmnhan/erlabpy/commit/f1157ba7afcb0b259932062edb0dc2138c749c55))
 
-* feat(io): new data loader!
+* **io** new data loader! ([`6c85cba`](https://github.com/kmnhan/erlabpy/commit/6c85cba810936403734cfeefa65b005e2d2e329e))
 
-Implemented  new class-based data loader. Currently only implemented for ALS BL4.0.3. ([`6c85cba`](https://github.com/kmnhan/erlabpy/commit/6c85cba810936403734cfeefa65b005e2d2e329e))
+  Implemented  new class-based data loader. Currently only implemented for ALS BL4.0.3.
 
-* feat(io): add new utility function ([`a27a9f8`](https://github.com/kmnhan/erlabpy/commit/a27a9f89ce56b35a7a35fd1014c01269378a8148))
+* **io** add new utility function ([`a27a9f8`](https://github.com/kmnhan/erlabpy/commit/a27a9f89ce56b35a7a35fd1014c01269378a8148))
 
-* feat(igor): remove attribute renaming, keep original attribute as much as possible ([`912376c`](https://github.com/kmnhan/erlabpy/commit/912376c0216c901e85dd68b03817cbc8b85522a7))
+* **igor** remove attribute renaming, keep original attribute as much as possible ([`912376c`](https://github.com/kmnhan/erlabpy/commit/912376c0216c901e85dd68b03817cbc8b85522a7))
 
-* feat: show elapsed time for momentum conversion ([`8889737`](https://github.com/kmnhan/erlabpy/commit/8889737aa6a8c5da2ef2ba17e5201816c99c574b))
+* show elapsed time for momentum conversion ([`8889737`](https://github.com/kmnhan/erlabpy/commit/8889737aa6a8c5da2ef2ba17e5201816c99c574b))
 
-* feat: add sample data generation in angles ([`1d2600d`](https://github.com/kmnhan/erlabpy/commit/1d2600d37b7fe323adb016a1daf2b9811d6f4593))
+* add sample data generation in angles ([`1d2600d`](https://github.com/kmnhan/erlabpy/commit/1d2600d37b7fe323adb016a1daf2b9811d6f4593))
 
-* feat(constants): add electron rest energy mc^2 ([`8e46445`](https://github.com/kmnhan/erlabpy/commit/8e46445efd3fa5fe623e2ab65ee939039b4dc149))
+* **constants** add electron rest energy mc^2 ([`8e46445`](https://github.com/kmnhan/erlabpy/commit/8e46445efd3fa5fe623e2ab65ee939039b4dc149))
 
-* feat(ktool): full kz support
+* **ktool** full kz support ([`c3284f7`](https://github.com/kmnhan/erlabpy/commit/c3284f785484b5f506bd2025afa57661ac947eec))
 
-Added inner potential spinbox and projected BZ overlay ([`c3284f7`](https://github.com/kmnhan/erlabpy/commit/c3284f785484b5f506bd2025afa57661ac947eec))
+  Added inner potential spinbox and projected BZ overlay
 
-* feat(bz): add BZ extending ([`cbbb11a`](https://github.com/kmnhan/erlabpy/commit/cbbb11ac8997951cda17ec976fe321b8699d1eff))
+* **bz** add BZ extending ([`cbbb11a`](https://github.com/kmnhan/erlabpy/commit/cbbb11ac8997951cda17ec976fe321b8699d1eff))
 
-* feat(itool): allow different label maximum widths
+* **itool** allow different label maximum widths ([`3467ae1`](https://github.com/kmnhan/erlabpy/commit/3467ae1720363ebfc026e3f5fc4f9517a342a448))
 
-The controls took up too much space if one of the dim names was long ([`3467ae1`](https://github.com/kmnhan/erlabpy/commit/3467ae1720363ebfc026e3f5fc4f9517a342a448))
+  The controls took up too much space if one of the dim names was long
 
-* feat: change transpose button order for 4D data ([`018002c`](https://github.com/kmnhan/erlabpy/commit/018002cd5606a091a528f866b2edcff051ce7570))
+* change transpose button order for 4D data ([`018002c`](https://github.com/kmnhan/erlabpy/commit/018002cd5606a091a528f866b2edcff051ce7570))
 
-* feat: add support for automatic cut and hv-dependent momentum conversion ([`f5be05f`](https://github.com/kmnhan/erlabpy/commit/f5be05fb80a4e5dc4f2b976e8894bddc07d43d91))
+* add support for automatic cut and hv-dependent momentum conversion ([`f5be05f`](https://github.com/kmnhan/erlabpy/commit/f5be05fb80a4e5dc4f2b976e8894bddc07d43d91))
 
-* feat: add bz masking function ([`f3a7d21`](https://github.com/kmnhan/erlabpy/commit/f3a7d21c44784e4191011e8e95202889afc15ccc))
+* add bz masking function ([`f3a7d21`](https://github.com/kmnhan/erlabpy/commit/f3a7d21c44784e4191011e8e95202889afc15ccc))
 
-* feat(interpolate): add more checks and warnings ([`f1c223f`](https://github.com/kmnhan/erlabpy/commit/f1c223fbce27d65ed196fafd196c8b9c28d978dd))
+* **interpolate** add more checks and warnings ([`f1c223f`](https://github.com/kmnhan/erlabpy/commit/f1c223fbce27d65ed196fafd196c8b9c28d978dd))
 
-* feat(ktool): frontend tweaks
+* **ktool** frontend tweaks ([`d0050d0`](https://github.com/kmnhan/erlabpy/commit/d0050d02270c5ad8e51af281cb7a9f7a1cb89913))
 
-Added wait dialog for showing imagetool and make labels prettier ([`d0050d0`](https://github.com/kmnhan/erlabpy/commit/d0050d02270c5ad8e51af281cb7a9f7a1cb89913))
+  Added wait dialog for showing imagetool and make labels prettier
 
-* feat: add new momentum conversion tool ([`dfa96fe`](https://github.com/kmnhan/erlabpy/commit/dfa96fe9f20b57699d43d3d23755c663c3793d30))
+* add new momentum conversion tool ([`dfa96fe`](https://github.com/kmnhan/erlabpy/commit/dfa96fe9f20b57699d43d3d23755c663c3793d30))
 
-* feat: implement new momentum conversion functions. Currently only supports kxky and kxkyE conversion. ([`956a0bd`](https://github.com/kmnhan/erlabpy/commit/956a0bd8e034754d0b208a7c654d77e690491b98))
+* implement new momentum conversion functions. Currently only supports kxky and kxkyE conversion. ([`956a0bd`](https://github.com/kmnhan/erlabpy/commit/956a0bd8e034754d0b208a7c654d77e690491b98))
 
-* feat: switch data loaders and plotting functions to new angle coordinate convention.
+* switch data loaders and plotting functions to new angle coordinate convention. ([`b5734df`](https://github.com/kmnhan/erlabpy/commit/b5734df4a4c0009131b0510645f4cb28eff702cb))
 
-Adopts the angle convention given by Y. Ishida and S. Shin, Rev. Sci. Instrum. 89, 043903 (2018). This is a breakin change, and momentum conversion will be entirely re-written.
-All angles are now given in degrees, goodbye to radians. ([`b5734df`](https://github.com/kmnhan/erlabpy/commit/b5734df4a4c0009131b0510645f4cb28eff702cb))
+  Adopts the angle convention given by Y. Ishida and S. Shin, Rev. Sci. Instrum. 89, 043903 (2018). This is a breakin change, and momentum conversion will be entirely re-written. All angles are now given in degrees, goodbye to radians.
 
-* feat: misc. changes to momentum conversion tool ([`1221fd0`](https://github.com/kmnhan/erlabpy/commit/1221fd0403977b840e650221111ae3a72a69cb65))
+* misc. changes to momentum conversion tool ([`1221fd0`](https://github.com/kmnhan/erlabpy/commit/1221fd0403977b840e650221111ae3a72a69cb65))
 
-* feat: load new resistance data ([`782cdf8`](https://github.com/kmnhan/erlabpy/commit/782cdf82c8b6b12d15c3f964dfe4a924131e5d4a))
+* load new resistance data ([`782cdf8`](https://github.com/kmnhan/erlabpy/commit/782cdf82c8b6b12d15c3f964dfe4a924131e5d4a))
 
-* feat: add spline module (work in progress) ([`69f8e4c`](https://github.com/kmnhan/erlabpy/commit/69f8e4c60cd147fc677f27aee927607153db3ac6))
+* add spline module (work in progress) ([`69f8e4c`](https://github.com/kmnhan/erlabpy/commit/69f8e4c60cd147fc677f27aee927607153db3ac6))
 
-* feat(goldtool): scale roi initial position to data ([`65f71d2`](https://github.com/kmnhan/erlabpy/commit/65f71d2c3ec1888f8e8fecb84b0e98189859f191))
+* **goldtool** scale roi initial position to data ([`65f71d2`](https://github.com/kmnhan/erlabpy/commit/65f71d2c3ec1888f8e8fecb84b0e98189859f191))
 
-* feat(goldtool): add remaining time to progress bar ([`348aaf7`](https://github.com/kmnhan/erlabpy/commit/348aaf7acde9421156bb6027bc0853a4142f166f))
+* **goldtool** add remaining time to progress bar ([`348aaf7`](https://github.com/kmnhan/erlabpy/commit/348aaf7acde9421156bb6027bc0853a4142f166f))
 
-* feat: add atom plotting module ([`2fcf012`](https://github.com/kmnhan/erlabpy/commit/2fcf012c2866b598a82741961b9ad29602a63748))
+* add atom plotting module ([`2fcf012`](https://github.com/kmnhan/erlabpy/commit/2fcf012c2866b598a82741961b9ad29602a63748))
 
-* feat: minor tweaks to mplstyle ([`10972b8`](https://github.com/kmnhan/erlabpy/commit/10972b8f70c041835d0c8274448e53be67172d18))
+* minor tweaks to mplstyle ([`10972b8`](https://github.com/kmnhan/erlabpy/commit/10972b8f70c041835d0c8274448e53be67172d18))
 
-* feat: add crop to  plot_array ([`36d8536`](https://github.com/kmnhan/erlabpy/commit/36d85366ffd1c84298df79d6721b26f17d8cf031))
+* add crop to  plot_array ([`36d8536`](https://github.com/kmnhan/erlabpy/commit/36d85366ffd1c84298df79d6721b26f17d8cf031))
 
-* feat(colors): make axes not required for nice_colorbar ([`48af74b`](https://github.com/kmnhan/erlabpy/commit/48af74b45e926f5ff9f2c0c717d27d05987837b8))
+* **colors** make axes not required for nice_colorbar ([`48af74b`](https://github.com/kmnhan/erlabpy/commit/48af74b45e926f5ff9f2c0c717d27d05987837b8))
 
-* feat(goldtool): add diffev to list of methods ([`d21c915`](https://github.com/kmnhan/erlabpy/commit/d21c915f7993c66f1a79dc7cfa28b06b63cc89f8))
+* **goldtool** add diffev to list of methods ([`d21c915`](https://github.com/kmnhan/erlabpy/commit/d21c915f7993c66f1a79dc7cfa28b06b63cc89f8))
 
-* feat(itool): plot class customization ([`fee3913`](https://github.com/kmnhan/erlabpy/commit/fee39133c4208e7733a18b31d77a7898ac4b5713))
+* **itool** plot class customization ([`fee3913`](https://github.com/kmnhan/erlabpy/commit/fee39133c4208e7733a18b31d77a7898ac4b5713))
 
-* feat: better cache management for slicer ([`9f49374`](https://github.com/kmnhan/erlabpy/commit/9f49374ee98fb2cc101974292d959ee0f6898a9a))
+* better cache management for slicer ([`9f49374`](https://github.com/kmnhan/erlabpy/commit/9f49374ee98fb2cc101974292d959ee0f6898a9a))
 
-* feat(betterspinbox): make keyboardTracking off by default ([`753ddcd`](https://github.com/kmnhan/erlabpy/commit/753ddcd344ff6859ff44cecaff4fb641e4e981dd))
+* **betterspinbox** make keyboardTracking off by default ([`753ddcd`](https://github.com/kmnhan/erlabpy/commit/753ddcd344ff6859ff44cecaff4fb641e4e981dd))
 
-* feat(annotation): add axis unit scaling ([`a61b8f3`](https://github.com/kmnhan/erlabpy/commit/a61b8f38165828d3f118c682cbfe05325c413e22))
+* **annotation** add axis unit scaling ([`a61b8f3`](https://github.com/kmnhan/erlabpy/commit/a61b8f38165828d3f118c682cbfe05325c413e22))
 
-* feat(itool): add option to decouple colors ([`3e2f132`](https://github.com/kmnhan/erlabpy/commit/3e2f1325baa1011540b29f1f36fd8b12a7770114))
+* **itool** add option to decouple colors ([`3e2f132`](https://github.com/kmnhan/erlabpy/commit/3e2f1325baa1011540b29f1f36fd8b12a7770114))
 
-* feat(style): update poster style ([`da58226`](https://github.com/kmnhan/erlabpy/commit/da582267a69fea8efb86e93478c398d70c7e411c))
+* **style** update poster style ([`da58226`](https://github.com/kmnhan/erlabpy/commit/da582267a69fea8efb86e93478c398d70c7e411c))
 
-* feat(accessor): use pyarpes for 2d kconv ([`9cbe422`](https://github.com/kmnhan/erlabpy/commit/9cbe422d19bb95e17a13b4757b8239d08069d850))
+* **accessor** use pyarpes for 2d kconv ([`9cbe422`](https://github.com/kmnhan/erlabpy/commit/9cbe422d19bb95e17a13b4757b8239d08069d850))
 
-* feat: improve extendability ([`ded8841`](https://github.com/kmnhan/erlabpy/commit/ded884139e25cea9549fd3e3e7b0519c03b1d447))
+* improve extendability ([`ded8841`](https://github.com/kmnhan/erlabpy/commit/ded884139e25cea9549fd3e3e7b0519c03b1d447))
 
-* feat(itool): pass parent ([`c8feac4`](https://github.com/kmnhan/erlabpy/commit/c8feac43871fba3a0c12db56d33c819efdfd3e41))
+* **itool** pass parent ([`c8feac4`](https://github.com/kmnhan/erlabpy/commit/c8feac43871fba3a0c12db56d33c819efdfd3e41))
 
-* feat(itool): add base imagetool with only controls ([`fdb8a6b`](https://github.com/kmnhan/erlabpy/commit/fdb8a6b0e52f83c05441d03a06bd15d83b8a261a))
+* **itool** add base imagetool with only controls ([`fdb8a6b`](https://github.com/kmnhan/erlabpy/commit/fdb8a6b0e52f83c05441d03a06bd15d83b8a261a))
 
-* feat: add option to return individual regions ([`7c5b081`](https://github.com/kmnhan/erlabpy/commit/7c5b08181f0cfc6d727fafe6a8789ec952ac895f))
+* add option to return individual regions ([`7c5b081`](https://github.com/kmnhan/erlabpy/commit/7c5b08181f0cfc6d727fafe6a8789ec952ac895f))
 
-* feat(colors): add function to unify color limits ([`33d571f`](https://github.com/kmnhan/erlabpy/commit/33d571f4dfcdecec02d536f5f5a4cd9af349d2df))
+* **colors** add function to unify color limits ([`33d571f`](https://github.com/kmnhan/erlabpy/commit/33d571f4dfcdecec02d536f5f5a4cd9af349d2df))
 
-* feat(colors): add function that combines colormaps ([`f19d87c`](https://github.com/kmnhan/erlabpy/commit/f19d87ca5c3de53ca8623d7954a280b7050f2d15))
+* **colors** add function that combines colormaps ([`f19d87c`](https://github.com/kmnhan/erlabpy/commit/f19d87ca5c3de53ca8623d7954a280b7050f2d15))
 
-* feat: add new colormap! ([`474ad52`](https://github.com/kmnhan/erlabpy/commit/474ad521c3c5726341c17b9b4759ee501661ce73))
+* add new colormap! ([`474ad52`](https://github.com/kmnhan/erlabpy/commit/474ad521c3c5726341c17b9b4759ee501661ce73))
 
-* feat: k range freedom in sample data generation ([`9dd5b00`](https://github.com/kmnhan/erlabpy/commit/9dd5b0025aaf52ef0bf4685ef5e380ccd5a72ac4))
+* k range freedom in sample data generation ([`9dd5b00`](https://github.com/kmnhan/erlabpy/commit/9dd5b0025aaf52ef0bf4685ef5e380ccd5a72ac4))
 
-* feat: make BZ plotter standalone ([`3bec642`](https://github.com/kmnhan/erlabpy/commit/3bec64218de70cabf8a43b78bf6728bef6402b49))
+* make BZ plotter standalone ([`3bec642`](https://github.com/kmnhan/erlabpy/commit/3bec64218de70cabf8a43b78bf6728bef6402b49))
 
-* feat(igorinterface): add to load wave menu ([`da704c5`](https://github.com/kmnhan/erlabpy/commit/da704c5c083a41db3999b031a5676bb69e33f46a))
+* **igorinterface** add to load wave menu ([`da704c5`](https://github.com/kmnhan/erlabpy/commit/da704c5c083a41db3999b031a5676bb69e33f46a))
 
-* feat(io): add DA30 loader ([`9afd149`](https://github.com/kmnhan/erlabpy/commit/9afd149ddfb21a64564f4d9d2bb1ccb6dcd6d808))
+* **io** add DA30 loader ([`9afd149`](https://github.com/kmnhan/erlabpy/commit/9afd149ddfb21a64564f4d9d2bb1ccb6dcd6d808))
 
-* feat(goldtool): add fit abort ([`693b1e4`](https://github.com/kmnhan/erlabpy/commit/693b1e474ebbc4989dba6ed900f85cad62b5cfcc))
+* **goldtool** add fit abort ([`693b1e4`](https://github.com/kmnhan/erlabpy/commit/693b1e474ebbc4989dba6ed900f85cad62b5cfcc))
 
-* feat: pass kwargs to broadcast_model ([`82d11f2`](https://github.com/kmnhan/erlabpy/commit/82d11f24b6412f8c774264f5941863eaff7cef6b))
+* pass kwargs to broadcast_model ([`82d11f2`](https://github.com/kmnhan/erlabpy/commit/82d11f24b6412f8c774264f5941863eaff7cef6b))
 
-* feat: autolevel colorbar ([`f116155`](https://github.com/kmnhan/erlabpy/commit/f1161551fbf4665b65287d27a2312b3b052c1948))
+* autolevel colorbar ([`f116155`](https://github.com/kmnhan/erlabpy/commit/f1161551fbf4665b65287d27a2312b3b052c1948))
 
-* feat: set colorbar width ([`b13b5d2`](https://github.com/kmnhan/erlabpy/commit/b13b5d2abd89e98bee6e55d5aeba135a16b3fb50))
+* set colorbar width ([`b13b5d2`](https://github.com/kmnhan/erlabpy/commit/b13b5d2abd89e98bee6e55d5aeba135a16b3fb50))
 
-* feat(gold): fully integrate spline fitting ([`d5b345c`](https://github.com/kmnhan/erlabpy/commit/d5b345cb5efc6e1e889c272d437e646935ff12e1))
+* **gold** fully integrate spline fitting ([`d5b345c`](https://github.com/kmnhan/erlabpy/commit/d5b345cb5efc6e1e889c272d437e646935ff12e1))
 
-* feat: add lattice module ([`bafe36b`](https://github.com/kmnhan/erlabpy/commit/bafe36b7ab89f004f7ac0ac1d4aa2d1b5137698a))
+* add lattice module ([`bafe36b`](https://github.com/kmnhan/erlabpy/commit/bafe36b7ab89f004f7ac0ac1d4aa2d1b5137698a))
 
-* feat: estimate k resolution from data ([`457edc7`](https://github.com/kmnhan/erlabpy/commit/457edc72ffa755ffc2e8d3fee039df97bab53ae0))
+* estimate k resolution from data ([`457edc7`](https://github.com/kmnhan/erlabpy/commit/457edc72ffa755ffc2e8d3fee039df97bab53ae0))
 
-* feat: add kspace conversion accessor ([`56da9e0`](https://github.com/kmnhan/erlabpy/commit/56da9e09c0dedc9cb066fbd641b5a92eca5b8635))
+* add kspace conversion accessor ([`56da9e0`](https://github.com/kmnhan/erlabpy/commit/56da9e09c0dedc9cb066fbd641b5a92eca5b8635))
 
-* feat(itool): save individual plot as hdf5 ([`a5a88b9`](https://github.com/kmnhan/erlabpy/commit/a5a88b9402b5d538386547083b8d7dcc2335e032))
+* **itool** save individual plot as hdf5 ([`a5a88b9`](https://github.com/kmnhan/erlabpy/commit/a5a88b9402b5d538386547083b8d7dcc2335e032))
 
-* feat: add ZT image view for 4D ([`bf66dfb`](https://github.com/kmnhan/erlabpy/commit/bf66dfbc948bbf585dde392b23b0e5586b2a1d35))
+* add ZT image view for 4D ([`bf66dfb`](https://github.com/kmnhan/erlabpy/commit/bf66dfbc948bbf585dde392b23b0e5586b2a1d35))
 
-* feat: add igor procedure to load dataarrays ([`f8b93e0`](https://github.com/kmnhan/erlabpy/commit/f8b93e0e79adc6052e577304dd856a146de0c521))
+* add igor procedure to load dataarrays ([`f8b93e0`](https://github.com/kmnhan/erlabpy/commit/f8b93e0e79adc6052e577304dd856a146de0c521))
 
-* feat(itool): enable sync across multiple windows! ([`d3a5056`](https://github.com/kmnhan/erlabpy/commit/d3a50561bd38c9040b9aae3b6c1b82453df1423b))
+* **itool** enable sync across multiple windows! ([`d3a5056`](https://github.com/kmnhan/erlabpy/commit/d3a50561bd38c9040b9aae3b6c1b82453df1423b))
 
-* feat(gold): automatic crop for corrected gold ([`dad4bb8`](https://github.com/kmnhan/erlabpy/commit/dad4bb886799fd11d5ecf6c8c18c4a118858d15f))
+* **gold** automatic crop for corrected gold ([`dad4bb8`](https://github.com/kmnhan/erlabpy/commit/dad4bb886799fd11d5ecf6c8c18c4a118858d15f))
 
-* feat(io): improve BL4 data loading, add basic log generator ([`e283262`](https://github.com/kmnhan/erlabpy/commit/e283262f138bc509d9f4481efd835626060f8b62))
+* **io** improve BL4 data loading, add basic log generator ([`e283262`](https://github.com/kmnhan/erlabpy/commit/e283262f138bc509d9f4481efd835626060f8b62))
 
-* feat(interp): improve interpolator syntax ([`c7b322b`](https://github.com/kmnhan/erlabpy/commit/c7b322b6bf4106320270b39b4aa423d94ffa94be))
+* **interp** improve interpolator syntax ([`c7b322b`](https://github.com/kmnhan/erlabpy/commit/c7b322b6bf4106320270b39b4aa423d94ffa94be))
 
-* feat(gold): configurable covariance matrix scaling ([`d051864`](https://github.com/kmnhan/erlabpy/commit/d051864da1dd2e3f5101d33743fa04720fab5411))
+* **gold** configurable covariance matrix scaling ([`d051864`](https://github.com/kmnhan/erlabpy/commit/d051864da1dd2e3f5101d33743fa04720fab5411))
 
-* feat(fit): add step function edge ([`3a7bc03`](https://github.com/kmnhan/erlabpy/commit/3a7bc03c666a946813ce79e95002475efb446046))
+* **fit** add step function edge ([`3a7bc03`](https://github.com/kmnhan/erlabpy/commit/3a7bc03c666a946813ce79e95002475efb446046))
 
-* feat: handle rad2deg automatically ([`aea4a62`](https://github.com/kmnhan/erlabpy/commit/aea4a62d047cca0be231e0256ad3f519ef54eb0e))
+* handle rad2deg automatically ([`aea4a62`](https://github.com/kmnhan/erlabpy/commit/aea4a62d047cca0be231e0256ad3f519ef54eb0e))
 
-* feat(bz): add option for clip path ([`52daa2a`](https://github.com/kmnhan/erlabpy/commit/52daa2afa4fe98acb1c5ac39dfe6362d348d2e11))
+* **bz** add option for clip path ([`52daa2a`](https://github.com/kmnhan/erlabpy/commit/52daa2afa4fe98acb1c5ac39dfe6362d348d2e11))
 
-* feat: add fast trilinear interpolation ([`ae77bee`](https://github.com/kmnhan/erlabpy/commit/ae77bee8050b3a80e5ab24bef447911d2e6a4ccd))
+* add fast trilinear interpolation ([`ae77bee`](https://github.com/kmnhan/erlabpy/commit/ae77bee8050b3a80e5ab24bef447911d2e6a4ccd))
 
-* feat(io): add function for pxp debugging ([`1802e09`](https://github.com/kmnhan/erlabpy/commit/1802e099689062bf7e7f531b726ea8ce7ada91e0))
+* **io** add function for pxp debugging ([`1802e09`](https://github.com/kmnhan/erlabpy/commit/1802e099689062bf7e7f531b726ea8ce7ada91e0))
 
-* feat: add W to ph/s conversion ([`a64039d`](https://github.com/kmnhan/erlabpy/commit/a64039d3ca2971b5a434a451fc8e956e40fa2e9b))
+* add W to ph/s conversion ([`a64039d`](https://github.com/kmnhan/erlabpy/commit/a64039d3ca2971b5a434a451fc8e956e40fa2e9b))
 
-* feat: add 2D fermi edge fitting function ([`90c65de`](https://github.com/kmnhan/erlabpy/commit/90c65de986074dcce3ba658a0ec9ce1581da1dd2))
+* add 2D fermi edge fitting function ([`90c65de`](https://github.com/kmnhan/erlabpy/commit/90c65de986074dcce3ba658a0ec9ce1581da1dd2))
 
-* feat(itool): keep manual limits under transpose ([`bdec7e5`](https://github.com/kmnhan/erlabpy/commit/bdec7e5abe935072f91570af9fc58bb2f19582cb))
+* **itool** keep manual limits under transpose ([`bdec7e5`](https://github.com/kmnhan/erlabpy/commit/bdec7e5abe935072f91570af9fc58bb2f19582cb))
 
-* feat: add more colortables from igor ([`03a615f`](https://github.com/kmnhan/erlabpy/commit/03a615f2ffbbf522bc8421757b7def3db037eab4))
+* add more colortables from igor ([`03a615f`](https://github.com/kmnhan/erlabpy/commit/03a615f2ffbbf522bc8421757b7def3db037eab4))
 
-* feat: add interactive brillouin zone plot ([`85f844f`](https://github.com/kmnhan/erlabpy/commit/85f844f5f7461489f924f8cf5096416791dec525))
+* add interactive brillouin zone plot ([`85f844f`](https://github.com/kmnhan/erlabpy/commit/85f844f5f7461489f924f8cf5096416791dec525))
 
-* feat: update style files ([`5278c6c`](https://github.com/kmnhan/erlabpy/commit/5278c6c04213ce4230797bc34028d8befa2923af))
+* update style files ([`5278c6c`](https://github.com/kmnhan/erlabpy/commit/5278c6c04213ce4230797bc34028d8befa2923af))
 
-* feat: modernize plot_array ([`c5e7321`](https://github.com/kmnhan/erlabpy/commit/c5e7321dbbc124ae99d55b3959c020f59b1a2b7d))
+* modernize plot_array ([`c5e7321`](https://github.com/kmnhan/erlabpy/commit/c5e7321dbbc124ae99d55b3959c020f59b1a2b7d))
 
-* feat(io): igor-compatible output ([`2a654e2`](https://github.com/kmnhan/erlabpy/commit/2a654e26fb0e53f79b705bb62db437f5d16e5735))
+* **io** igor-compatible output ([`2a654e2`](https://github.com/kmnhan/erlabpy/commit/2a654e26fb0e53f79b705bb62db437f5d16e5735))
 
-* feat(io): rewrite igor related backend ([`8739bef`](https://github.com/kmnhan/erlabpy/commit/8739befc3f30661e4d2ffd680888c3b06f3230cb))
+* **io** rewrite igor related backend ([`8739bef`](https://github.com/kmnhan/erlabpy/commit/8739befc3f30661e4d2ffd680888c3b06f3230cb))
 
-* feat: polynomial model now takes positional args ([`a3000d5`](https://github.com/kmnhan/erlabpy/commit/a3000d55eca86fe2c1c1d8f7d468ab4051ceef08))
+* polynomial model now takes positional args ([`a3000d5`](https://github.com/kmnhan/erlabpy/commit/a3000d55eca86fe2c1c1d8f7d468ab4051ceef08))
 
-* feat(goldtool): add smoothing spline fit ([`b25cd7c`](https://github.com/kmnhan/erlabpy/commit/b25cd7c19ced68c028f63cd3fbac533ae7a026b3))
+* **goldtool** add smoothing spline fit ([`b25cd7c`](https://github.com/kmnhan/erlabpy/commit/b25cd7c19ced68c028f63cd3fbac533ae7a026b3))
 
-* feat(itool): add performance benchmarks ([`9634af0`](https://github.com/kmnhan/erlabpy/commit/9634af0232afbf7f845b9694a03739b9111d516f))
+* **itool** add performance benchmarks ([`9634af0`](https://github.com/kmnhan/erlabpy/commit/9634af0232afbf7f845b9694a03739b9111d516f))
 
-* feat: default cmap for analysis is now terrain ([`c1cc21c`](https://github.com/kmnhan/erlabpy/commit/c1cc21c2e7660245d1d0bcd1c3e4a5f45b757e15))
+* default cmap for analysis is now terrain ([`c1cc21c`](https://github.com/kmnhan/erlabpy/commit/c1cc21c2e7660245d1d0bcd1c3e4a5f45b757e15))
 
-* feat: example dataset generator ([`6b6cadf`](https://github.com/kmnhan/erlabpy/commit/6b6cadf19d536dea990daacd687739953a33a2d1))
+* example dataset generator ([`6b6cadf`](https://github.com/kmnhan/erlabpy/commit/6b6cadf19d536dea990daacd687739953a33a2d1))
 
-* feat: add curve fitting tool (alpha) ([`68356ab`](https://github.com/kmnhan/erlabpy/commit/68356ab6d7fc4ecb6653d36213acc8c22ef4f23b))
+* add curve fitting tool (alpha) ([`68356ab`](https://github.com/kmnhan/erlabpy/commit/68356ab6d7fc4ecb6653d36213acc8c22ef4f23b))
 
-* feat: add new module for curve fitting ([`20c8be9`](https://github.com/kmnhan/erlabpy/commit/20c8be92116a0ce95f1dd55a2de131a1a9a16efe))
+* add new module for curve fitting ([`20c8be9`](https://github.com/kmnhan/erlabpy/commit/20c8be92116a0ce95f1dd55a2de131a1a9a16efe))
 
-* feat: added boltzmann const. at constants ([`038930e`](https://github.com/kmnhan/erlabpy/commit/038930ebd9a48c000990c006ca794f8fc34b3d94))
+* added boltzmann const. at constants ([`038930e`](https://github.com/kmnhan/erlabpy/commit/038930ebd9a48c000990c006ca794f8fc34b3d94))
 
-* feat: add module for 3D plotting ([`4ec1bd2`](https://github.com/kmnhan/erlabpy/commit/4ec1bd2c81b17c775321d7b8197fe7ca84f1d03b))
+* add module for 3D plotting ([`4ec1bd2`](https://github.com/kmnhan/erlabpy/commit/4ec1bd2c81b17c775321d7b8197fe7ca84f1d03b))
 
-* feat(itool): add copy index action ([`6f25677`](https://github.com/kmnhan/erlabpy/commit/6f25677d2ba5d8cf1172a937d3370f67a7220781))
+* **itool** add copy index action ([`6f25677`](https://github.com/kmnhan/erlabpy/commit/6f25677d2ba5d8cf1172a937d3370f67a7220781))
 
-* feat: parallelize multidimensional mean ([`7cfae81`](https://github.com/kmnhan/erlabpy/commit/7cfae816761e3169d1eb52b24d7adbbe8aeef848))
+* parallelize multidimensional mean ([`7cfae81`](https://github.com/kmnhan/erlabpy/commit/7cfae816761e3169d1eb52b24d7adbbe8aeef848))
 
-* feat: add 2D colormap ([`f5799d8`](https://github.com/kmnhan/erlabpy/commit/f5799d8d389ddf9c8cb03d7bfd05e9daa5331de0))
+* add 2D colormap ([`f5799d8`](https://github.com/kmnhan/erlabpy/commit/f5799d8d389ddf9c8cb03d7bfd05e9daa5331de0))
 
-* feat(itool): intuitive transpose for 4D data ([`38315f8`](https://github.com/kmnhan/erlabpy/commit/38315f83f98fa92313c8f7857c5b100f1b6f4fed))
+* **itool** intuitive transpose for 4D data ([`38315f8`](https://github.com/kmnhan/erlabpy/commit/38315f83f98fa92313c8f7857c5b100f1b6f4fed))
 
-* feat(polygon): add convenience function ([`a9e64c7`](https://github.com/kmnhan/erlabpy/commit/a9e64c7213952754c2ad70c2f7b92c73a4a1a45d))
+* **polygon** add convenience function ([`a9e64c7`](https://github.com/kmnhan/erlabpy/commit/a9e64c7213952754c2ad70c2f7b92c73a4a1a45d))
 
-* feat: gradient fill under line plot ([`6a951c1`](https://github.com/kmnhan/erlabpy/commit/6a951c10060d454c8f5335d9081d1764881d1fc2))
+* gradient fill under line plot ([`6a951c1`](https://github.com/kmnhan/erlabpy/commit/6a951c10060d454c8f5335d9081d1764881d1fc2))
 
-* feat: plot 1D slices ([`36dee17`](https://github.com/kmnhan/erlabpy/commit/36dee178b9ffaa37216f74a4bf7810ff3021354c))
+* plot 1D slices ([`36dee17`](https://github.com/kmnhan/erlabpy/commit/36dee178b9ffaa37216f74a4bf7810ff3021354c))
 
-* feat(io): add convenience function for BL4 data loading ([`0f3a4ea`](https://github.com/kmnhan/erlabpy/commit/0f3a4eac22e4738fe860117c6474bdab7923b959))
+* **io** add convenience function for BL4 data loading ([`0f3a4ea`](https://github.com/kmnhan/erlabpy/commit/0f3a4eac22e4738fe860117c6474bdab7923b959))
 
-* feat: add igor colormaps ([`4bfcceb`](https://github.com/kmnhan/erlabpy/commit/4bfcceb8cca35df3fcb775743f73b127a7c48239))
+* add igor colormaps ([`4bfcceb`](https://github.com/kmnhan/erlabpy/commit/4bfcceb8cca35df3fcb775743f73b127a7c48239))
 
-* feat: new module for some common constants ([`c6aaede`](https://github.com/kmnhan/erlabpy/commit/c6aaede496725cb59548e26fff45f933f71883da))
+* new module for some common constants ([`c6aaede`](https://github.com/kmnhan/erlabpy/commit/c6aaede496725cb59548e26fff45f933f71883da))
 
-* feat: update erplot ([`4bdbc10`](https://github.com/kmnhan/erlabpy/commit/4bdbc10e9556105df9f0250aeb1554ea3b862581))
+* update erplot ([`4bdbc10`](https://github.com/kmnhan/erlabpy/commit/4bdbc10e9556105df9f0250aeb1554ea3b862581))
 
-* feat: add some annotations ([`4a37666`](https://github.com/kmnhan/erlabpy/commit/4a37666dcbd732f8c14c95c2ac1a2c24dee46e3b))
+* add some annotations ([`4a37666`](https://github.com/kmnhan/erlabpy/commit/4a37666dcbd732f8c14c95c2ac1a2c24dee46e3b))
 
-* feat(io): add load functions ([`c654c44`](https://github.com/kmnhan/erlabpy/commit/c654c4444fd78ae64222b25559a881bdca1b6321))
+* **io** add load functions ([`c654c44`](https://github.com/kmnhan/erlabpy/commit/c654c4444fd78ae64222b25559a881bdca1b6321))
 
-* feat(itool): copy cursor position ([`cc39829`](https://github.com/kmnhan/erlabpy/commit/cc398299fb1d25ac1164a216cf68f68ec2e80555))
+* **itool** copy cursor position ([`cc39829`](https://github.com/kmnhan/erlabpy/commit/cc398299fb1d25ac1164a216cf68f68ec2e80555))
 
-* feat: attempt better colorbar... this is probably stupid, fix later ([`2b26a3c`](https://github.com/kmnhan/erlabpy/commit/2b26a3c12e52c11d0468fa1268611b58ecf82b19))
+* attempt better colorbar... this is probably stupid, fix later ([`2b26a3c`](https://github.com/kmnhan/erlabpy/commit/2b26a3c12e52c11d0468fa1268611b58ecf82b19))
 
-* feat: fast peak fitting with broadened step edge ([`dc30094`](https://github.com/kmnhan/erlabpy/commit/dc300944a2ec0f25e0e4f16540b1edb42af0b154))
+* fast peak fitting with broadened step edge ([`dc30094`](https://github.com/kmnhan/erlabpy/commit/dc300944a2ec0f25e0e4f16540b1edb42af0b154))
 
-* feat: AxisItem scientific labeling
-feat: increased degree of freedom for ParameterGroup
-fix: wrong colorbar levels ([`42b8860`](https://github.com/kmnhan/erlabpy/commit/42b8860a722dc4e20206b835e7fccb926975c460))
+* AxisItem scientific labeling ([`42b8860`](https://github.com/kmnhan/erlabpy/commit/42b8860a722dc4e20206b835e7fccb926975c460))
 
-* feat: add diverging colormap normalizations ([`b085946`](https://github.com/kmnhan/erlabpy/commit/b085946ab554c6a4aaef19b4aa13d1071114dc3b))
+* add diverging colormap normalizations ([`b085946`](https://github.com/kmnhan/erlabpy/commit/b085946ab554c6a4aaef19b4aa13d1071114dc3b))
 
-* feat(itool): add working colorbar ([`c326727`](https://github.com/kmnhan/erlabpy/commit/c326727c126c5081f1d7e60c2ce806699b8fb36f))
+* **itool** add working colorbar ([`c326727`](https://github.com/kmnhan/erlabpy/commit/c326727c126c5081f1d7e60c2ce806699b8fb36f))
 
-* feat(itool): full support for non-uniform coords ([`d3eface`](https://github.com/kmnhan/erlabpy/commit/d3eface36de9c15d788ab479d0f0a6860b36c9c8))
+* **itool** full support for non-uniform coords ([`d3eface`](https://github.com/kmnhan/erlabpy/commit/d3eface36de9c15d788ab479d0f0a6860b36c9c8))
 
-* feat(itool): auto-convert non-uniform dimensions to indices ([`1ad940d`](https://github.com/kmnhan/erlabpy/commit/1ad940d8bbc2b430cc54b7d9228ddc87e5235432))
+* **itool** auto-convert non-uniform dimensions to indices ([`1ad940d`](https://github.com/kmnhan/erlabpy/commit/1ad940d8bbc2b430cc54b7d9228ddc87e5235432))
 
-* feat(bz): add brillouin zone edge calculation ([`2b70d91`](https://github.com/kmnhan/erlabpy/commit/2b70d91ec8c77c27117637c1fec906a7a06c9571))
+* **bz** add brillouin zone edge calculation ([`2b70d91`](https://github.com/kmnhan/erlabpy/commit/2b70d91ec8c77c27117637c1fec906a7a06c9571))
 
-* feat(colors): add higher contrast PowerNorm ([`16b965c`](https://github.com/kmnhan/erlabpy/commit/16b965c224691103aabcfbb41c73524eb6b2244f))
+* **colors** add higher contrast PowerNorm ([`16b965c`](https://github.com/kmnhan/erlabpy/commit/16b965c224691103aabcfbb41c73524eb6b2244f))
 
-* feat(itool): add file open dialog ([`ba50354`](https://github.com/kmnhan/erlabpy/commit/ba5035491fa87ab44103d7041a81e15dee7a029e))
+* **itool** add file open dialog ([`ba50354`](https://github.com/kmnhan/erlabpy/commit/ba5035491fa87ab44103d7041a81e15dee7a029e))
 
-* feat(itool): move all cursors on drag with alt modifier ([`6ad638d`](https://github.com/kmnhan/erlabpy/commit/6ad638d9ef07c7b5dac05acc4977a39954abe96a))
+* **itool** move all cursors on drag with alt modifier ([`6ad638d`](https://github.com/kmnhan/erlabpy/commit/6ad638d9ef07c7b5dac05acc4977a39954abe96a))
 
-* feat(itool): add color limit lock and discrete cursor line ([`0929d61`](https://github.com/kmnhan/erlabpy/commit/0929d61973ef8ae62065820378d362a70cbbe110))
+* **itool** add color limit lock and discrete cursor line ([`0929d61`](https://github.com/kmnhan/erlabpy/commit/0929d61973ef8ae62065820378d362a70cbbe110))
 
-* feat(itool): parse ArrayLike input automatically ([`ce3d802`](https://github.com/kmnhan/erlabpy/commit/ce3d8027bf2ba2956ef80c8c28cbed28ab6d21be))
+* **itool** parse ArrayLike input automatically ([`ce3d802`](https://github.com/kmnhan/erlabpy/commit/ce3d8027bf2ba2956ef80c8c28cbed28ab6d21be))
 
-* feat(itool): add more menus ([`6b423eb`](https://github.com/kmnhan/erlabpy/commit/6b423eb0b56c0082ec0eee7de89761cbc56dfba5))
+* **itool** add more menus ([`6b423eb`](https://github.com/kmnhan/erlabpy/commit/6b423eb0b56c0082ec0eee7de89761cbc56dfba5))
 
-* feat: add EDC fitting tool (WIP) ([`4fceef5`](https://github.com/kmnhan/erlabpy/commit/4fceef509c63b8f51661b37cb8470f5bcf514b4b))
+* add EDC fitting tool (WIP) ([`4fceef5`](https://github.com/kmnhan/erlabpy/commit/4fceef509c63b8f51661b37cb8470f5bcf514b4b))
 
-* feat: add and modify styles ([`079f007`](https://github.com/kmnhan/erlabpy/commit/079f0070da78c1c44dcb67c46b38e84490d67f16))
+* add and modify styles ([`079f007`](https://github.com/kmnhan/erlabpy/commit/079f0070da78c1c44dcb67c46b38e84490d67f16))
 
-* feat(io): warn when modifying attrs ([`7692379`](https://github.com/kmnhan/erlabpy/commit/7692379416dda67c47a302d49b1c9a747514ef9c))
+* **io** warn when modifying attrs ([`7692379`](https://github.com/kmnhan/erlabpy/commit/7692379416dda67c47a302d49b1c9a747514ef9c))
 
-* feat(itool): add menubar ([`1614567`](https://github.com/kmnhan/erlabpy/commit/1614567a1287e3a099418190855ff54f8cadad95))
+* **itool** add menubar ([`1614567`](https://github.com/kmnhan/erlabpy/commit/1614567a1287e3a099418190855ff54f8cadad95))
 
-* feat(itool): better cursor colors ([`78dae09`](https://github.com/kmnhan/erlabpy/commit/78dae09619bfb79424eb0af930cc444467fce2c2))
+* **itool** better cursor colors ([`78dae09`](https://github.com/kmnhan/erlabpy/commit/78dae09619bfb79424eb0af930cc444467fce2c2))
 
-* feat(itool): enable handling multiple cursors ([`e971af7`](https://github.com/kmnhan/erlabpy/commit/e971af767f78d72acee064a0e87ae5764fd13d98))
+* **itool** enable handling multiple cursors ([`e971af7`](https://github.com/kmnhan/erlabpy/commit/e971af767f78d72acee064a0e87ae5764fd13d98))
 
-* feat: pretty plot gold edge fit results ([`aa621c5`](https://github.com/kmnhan/erlabpy/commit/aa621c588b733eae683494422f1330da74e09b23))
+* pretty plot gold edge fit results ([`aa621c5`](https://github.com/kmnhan/erlabpy/commit/aa621c588b733eae683494422f1330da74e09b23))
 
-* feat: add vertical Fermi energy indicators ([`80e2694`](https://github.com/kmnhan/erlabpy/commit/80e2694ed19dc18375b2dc26531fbda37525ca9e))
+* add vertical Fermi energy indicators ([`80e2694`](https://github.com/kmnhan/erlabpy/commit/80e2694ed19dc18375b2dc26531fbda37525ca9e))
 
-* feat: easier colorbar font size specification ([`5638d9c`](https://github.com/kmnhan/erlabpy/commit/5638d9c709c888fcfc24503196955e9d8df863c2))
+* easier colorbar font size specification ([`5638d9c`](https://github.com/kmnhan/erlabpy/commit/5638d9c709c888fcfc24503196955e9d8df863c2))
 
-* feat: add interactive progressbar for joblib ([`3fd24c7`](https://github.com/kmnhan/erlabpy/commit/3fd24c7dd57e2139c6f16af88fe0773323b928b4))
+* add interactive progressbar for joblib ([`3fd24c7`](https://github.com/kmnhan/erlabpy/commit/3fd24c7dd57e2139c6f16af88fe0773323b928b4))
 
-* feat(itool): add axis labels ([`96f9e76`](https://github.com/kmnhan/erlabpy/commit/96f9e76315cbff362d11e16b2b33378c5d7deab0))
+* **itool** add axis labels ([`96f9e76`](https://github.com/kmnhan/erlabpy/commit/96f9e76315cbff362d11e16b2b33378c5d7deab0))
 
-* feat(itool): minor adjustments to layout ([`c5dcbe2`](https://github.com/kmnhan/erlabpy/commit/c5dcbe2ec3c143579fe2c7969eda65dcb741e876))
+* **itool** minor adjustments to layout ([`c5dcbe2`](https://github.com/kmnhan/erlabpy/commit/c5dcbe2ec3c143579fe2c7969eda65dcb741e876))
 
-* feat(goldtool): higher order polynomials ([`5f34c35`](https://github.com/kmnhan/erlabpy/commit/5f34c3579975ed48124a5a2cf89980735f8d53a8))
+* **goldtool** higher order polynomials ([`5f34c35`](https://github.com/kmnhan/erlabpy/commit/5f34c3579975ed48124a5a2cf89980735f8d53a8))
 
-* feat(gold): get full results from Fermi edge fitting ([`ce0d853`](https://github.com/kmnhan/erlabpy/commit/ce0d853adf51df174d01098b703db21e26859882))
+* **gold** get full results from Fermi edge fitting ([`ce0d853`](https://github.com/kmnhan/erlabpy/commit/ce0d853adf51df174d01098b703db21e26859882))
 
-* feat: colorbar tick label customization ([`03e82bf`](https://github.com/kmnhan/erlabpy/commit/03e82bf100b3ca62fe781e1c82d54fce0ecab9b7))
+* colorbar tick label customization ([`03e82bf`](https://github.com/kmnhan/erlabpy/commit/03e82bf100b3ca62fe781e1c82d54fce0ecab9b7))
 
-* feat(io): improve SSRL loader ([`8fe9a46`](https://github.com/kmnhan/erlabpy/commit/8fe9a467d348225d213909a95acf9d80d93d018b))
+* **io** improve SSRL loader ([`8fe9a46`](https://github.com/kmnhan/erlabpy/commit/8fe9a467d348225d213909a95acf9d80d93d018b))
 
-* feat(itool): multicursor binning ([`bb4430c`](https://github.com/kmnhan/erlabpy/commit/bb4430ced79bfec8850ef7724c6ce752b4cd707b))
+* **itool** multicursor binning ([`bb4430c`](https://github.com/kmnhan/erlabpy/commit/bb4430ced79bfec8850ef7724c6ce752b4cd707b))
 
-* feat: add autoscale convenience function ([`36f838d`](https://github.com/kmnhan/erlabpy/commit/36f838d47bd5fdf8554e59b327b9bed9df961a0f))
+* add autoscale convenience function ([`36f838d`](https://github.com/kmnhan/erlabpy/commit/36f838d47bd5fdf8554e59b327b9bed9df961a0f))
 
-* feat: delegate font handling to different styles ([`aabf87b`](https://github.com/kmnhan/erlabpy/commit/aabf87b05be49c8bfe19afaf570bb769656c5ccb))
+* delegate font handling to different styles ([`aabf87b`](https://github.com/kmnhan/erlabpy/commit/aabf87b05be49c8bfe19afaf570bb769656c5ccb))
 
-* feat: simplify getting foreground color based on image ([`8034bfd`](https://github.com/kmnhan/erlabpy/commit/8034bfd15452f6032b0b2ff64cb14dc92d607c8b))
+* simplify getting foreground color based on image ([`8034bfd`](https://github.com/kmnhan/erlabpy/commit/8034bfd15452f6032b0b2ff64cb14dc92d607c8b))
 
-* feat: add fira font mplstyle ([`9c05702`](https://github.com/kmnhan/erlabpy/commit/9c05702d1ea822b5e138fca1e5f75c8d600397d7))
+* add fira font mplstyle ([`9c05702`](https://github.com/kmnhan/erlabpy/commit/9c05702d1ea822b5e138fca1e5f75c8d600397d7))
 
-* feat(itool): bind autorange to keyboard ([`98a236d`](https://github.com/kmnhan/erlabpy/commit/98a236deb88a9d74bc6763f49a75d465a097a264))
+* **itool** bind autorange to keyboard ([`98a236d`](https://github.com/kmnhan/erlabpy/commit/98a236deb88a9d74bc6763f49a75d465a097a264))
 
-* feat(itool): implement rad2deg ([`c074d74`](https://github.com/kmnhan/erlabpy/commit/c074d74a4ba62fda1e81e1dedf039ae939959975))
+* **itool** implement rad2deg ([`c074d74`](https://github.com/kmnhan/erlabpy/commit/c074d74a4ba62fda1e81e1dedf039ae939959975))
 
-* feat: include styles ([`5281177`](https://github.com/kmnhan/erlabpy/commit/528117714f3f7b08d253036b7492aba48dfe833b))
+* include styles ([`5281177`](https://github.com/kmnhan/erlabpy/commit/528117714f3f7b08d253036b7492aba48dfe833b))
 
-* feat: add completely reimplemented imagetool with faster slicing and multicursor support ([`af0655e`](https://github.com/kmnhan/erlabpy/commit/af0655eebb1f27199eae5270c971b206cb3edb6b))
+* add completely reimplemented imagetool with faster slicing and multicursor support ([`af0655e`](https://github.com/kmnhan/erlabpy/commit/af0655eebb1f27199eae5270c971b206cb3edb6b))
 
-* feat: added interactive gold edge fitting tool ([`c4017b6`](https://github.com/kmnhan/erlabpy/commit/c4017b699b27af76b9aa912f3231d1a19864e5e9))
+* added interactive gold edge fitting tool ([`c4017b6`](https://github.com/kmnhan/erlabpy/commit/c4017b699b27af76b9aa912f3231d1a19864e5e9))
 
-* feat: allow axes input to slice plotter ([`ab4c639`](https://github.com/kmnhan/erlabpy/commit/ab4c639c0b4d9e1cd34d03950846db2a4afdb138))
+* allow axes input to slice plotter ([`ab4c639`](https://github.com/kmnhan/erlabpy/commit/ab4c639c0b4d9e1cd34d03950846db2a4afdb138))
 
-* feat: multiple axes input to bz overlay plotter ([`9820e34`](https://github.com/kmnhan/erlabpy/commit/9820e340584299f5bbf95aea4193e6c47c026304))
+* multiple axes input to bz overlay plotter ([`9820e34`](https://github.com/kmnhan/erlabpy/commit/9820e340584299f5bbf95aea4193e6c47c026304))
 
-* feat(fermiline): support multiple axes input ([`9dc59b1`](https://github.com/kmnhan/erlabpy/commit/9dc59b1fbb6605e82ed0dcf8e7f444978c2c05df))
+* **fermiline** support multiple axes input ([`9dc59b1`](https://github.com/kmnhan/erlabpy/commit/9dc59b1fbb6605e82ed0dcf8e7f444978c2c05df))
 
-* feat: add interactive widget base classes
-refactor: subclass interactive widgets ([`e6787cf`](https://github.com/kmnhan/erlabpy/commit/e6787cf567bfd1a1cc1a131a69700143eb6e17bb))
+* add interactive widget base classes ([`e6787cf`](https://github.com/kmnhan/erlabpy/commit/e6787cf567bfd1a1cc1a131a69700143eb6e17bb))
 
-* feat(colors): add colorbar creation macro ([`811ed52`](https://github.com/kmnhan/erlabpy/commit/811ed526dc99d165f3f0cf77dd577744973cb539))
+* **colors** add colorbar creation macro ([`811ed52`](https://github.com/kmnhan/erlabpy/commit/811ed526dc99d165f3f0cf77dd577744973cb539))
 
-* feat: remove pyarpes dependency on labeling ([`71081fa`](https://github.com/kmnhan/erlabpy/commit/71081faf8404d256fb5b7f57fdc2304de6674445))
+* remove pyarpes dependency on labeling ([`71081fa`](https://github.com/kmnhan/erlabpy/commit/71081faf8404d256fb5b7f57fdc2304de6674445))
 
-* feat(io): silent loading of .pxp files ([`27d6b30`](https://github.com/kmnhan/erlabpy/commit/27d6b30fbff64237562ceaa9b3436d48b06a6e3b))
+* **io** silent loading of .pxp files ([`27d6b30`](https://github.com/kmnhan/erlabpy/commit/27d6b30fbff64237562ceaa9b3436d48b06a6e3b))
 
-* feat: parallel processing helpers wip ([`ac88e26`](https://github.com/kmnhan/erlabpy/commit/ac88e264463f4647a1195bd4eb93d617cd38c972))
+* parallel processing helpers wip ([`ac88e26`](https://github.com/kmnhan/erlabpy/commit/ac88e264463f4647a1195bd4eb93d617cd38c972))
 
-* feat: reliable gold edge and resolution fitting ([`653db58`](https://github.com/kmnhan/erlabpy/commit/653db5891f4573e069caaeb6f65edcffaa24b316))
+* reliable gold edge and resolution fitting ([`653db58`](https://github.com/kmnhan/erlabpy/commit/653db5891f4573e069caaeb6f65edcffaa24b316))
 
-* feat(annotations): better high symmetry marking ([`8e6dfcb`](https://github.com/kmnhan/erlabpy/commit/8e6dfcbc3f26f1d17a5bc1400a60512c51aa8a4d))
+* **annotations** better high symmetry marking ([`8e6dfcb`](https://github.com/kmnhan/erlabpy/commit/8e6dfcbc3f26f1d17a5bc1400a60512c51aa8a4d))
 
-* feat(mask): completely reimplement masking
-based on CGAL C++ library ([`ccfb9b6`](https://github.com/kmnhan/erlabpy/commit/ccfb9b61b75aa5e1f17e88402fc6824fe14287e8))
+* **mask** completely reimplement masking ([`ccfb9b6`](https://github.com/kmnhan/erlabpy/commit/ccfb9b61b75aa5e1f17e88402fc6824fe14287e8))
 
-* feat(io): data loading functions for igor ([`dd333e1`](https://github.com/kmnhan/erlabpy/commit/dd333e199c5e2718b0bb712b1842e37b6c099ea6))
+* **io** data loading functions for igor ([`dd333e1`](https://github.com/kmnhan/erlabpy/commit/dd333e199c5e2718b0bb712b1842e37b6c099ea6))
 
-* feat(correlation): rewrite based on scipy ([`14b1b29`](https://github.com/kmnhan/erlabpy/commit/14b1b29c1752ccb3d93d67de6de160e714606133))
+* **correlation** rewrite based on scipy ([`14b1b29`](https://github.com/kmnhan/erlabpy/commit/14b1b29c1752ccb3d93d67de6de160e714606133))
 
-* feat: add callable models for edge correction ([`3a6d8c3`](https://github.com/kmnhan/erlabpy/commit/3a6d8c3b5cc44078cd4b8f5056ccacb21d335428))
+* add callable models for edge correction ([`3a6d8c3`](https://github.com/kmnhan/erlabpy/commit/3a6d8c3b5cc44078cd4b8f5056ccacb21d335428))
 
-* feat: functions for gold edge related analysis ([`8c4941f`](https://github.com/kmnhan/erlabpy/commit/8c4941f6347c09a783b9e34ff17a132e05d16631))
+* functions for gold edge related analysis ([`8c4941f`](https://github.com/kmnhan/erlabpy/commit/8c4941f6347c09a783b9e34ff17a132e05d16631))
 
-* feat: rudimentary loader for SSRL ([`7e18e13`](https://github.com/kmnhan/erlabpy/commit/7e18e1354f95341440da2f020d992c4a38403261))
+* rudimentary loader for SSRL ([`7e18e13`](https://github.com/kmnhan/erlabpy/commit/7e18e1354f95341440da2f020d992c4a38403261))
 
-* feat(itool): better dock, improved memory usage ([`04f0047`](https://github.com/kmnhan/erlabpy/commit/04f00472ce5b507c1d467620dcfe03bdde1700c0))
+* **itool** better dock, improved memory usage ([`04f0047`](https://github.com/kmnhan/erlabpy/commit/04f00472ce5b507c1d467620dcfe03bdde1700c0))
 
-* feat(itool): support 4D input
-known issue: hiding slices are buggy with 4D ([`33a252f`](https://github.com/kmnhan/erlabpy/commit/33a252f42f88b9a0c182a3d771644b8e937d57be))
+* **itool** support 4D input ([`33a252f`](https://github.com/kmnhan/erlabpy/commit/33a252f42f88b9a0c182a3d771644b8e937d57be))
 
-* feat: add sizebar ([`21f420f`](https://github.com/kmnhan/erlabpy/commit/21f420f362dbf2bb18d1b16e34051dc11034a08a))
+* add sizebar ([`21f420f`](https://github.com/kmnhan/erlabpy/commit/21f420f362dbf2bb18d1b16e34051dc11034a08a))
 
-* feat(itool): add gamma slider ([`f5efcb7`](https://github.com/kmnhan/erlabpy/commit/f5efcb71c21696ccb9ed1e9b90b3c9e976bac01e))
+* **itool** add gamma slider ([`f5efcb7`](https://github.com/kmnhan/erlabpy/commit/f5efcb71c21696ccb9ed1e9b90b3c9e976bac01e))
 
-* feat(itool): subclass buttons for dark mode
-feat(itool): flow layout with customizable spacing
-refactor(itool): subclassed some button layouts
-refactor(itool): remove pyarpes dependency
-feat(itool): lazy load colormaps
-feat(itool): replace tabs with docks ([`e215470`](https://github.com/kmnhan/erlabpy/commit/e2154703986a8d35aa9b0b44b35a40c9dde62ec7))
+* **itool** subclass buttons for dark mode ([`e215470`](https://github.com/kmnhan/erlabpy/commit/e2154703986a8d35aa9b0b44b35a40c9dde62ec7))
 
-* feat: initial commit of general interactive tool ([`bf00956`](https://github.com/kmnhan/erlabpy/commit/bf009565f26a95ead1cda41bb000409bc435062e))
+* initial commit of general interactive tool ([`bf00956`](https://github.com/kmnhan/erlabpy/commit/bf009565f26a95ead1cda41bb000409bc435062e))
 
-* feat(itool): add axes visibility controls ([`258ff3f`](https://github.com/kmnhan/erlabpy/commit/258ff3fcecf5743adb04c82606feeff54ed828eb))
+* **itool** add axes visibility controls ([`258ff3f`](https://github.com/kmnhan/erlabpy/commit/258ff3fcecf5743adb04c82606feeff54ed828eb))
 
-* feat(itool): hide and show individual axes ([`6a8c71e`](https://github.com/kmnhan/erlabpy/commit/6a8c71e514c8fd4755c47ff521ed5f242c72056d))
+* **itool** hide and show individual axes ([`6a8c71e`](https://github.com/kmnhan/erlabpy/commit/6a8c71e514c8fd4755c47ff521ed5f242c72056d))
 
-* feat(itool): enable latex labels
-fix(itool): better grid size adjustment ([`be0b25d`](https://github.com/kmnhan/erlabpy/commit/be0b25dcad9abf49859c766668e969cc800406b9))
+* **itool** enable latex labels ([`be0b25d`](https://github.com/kmnhan/erlabpy/commit/be0b25dcad9abf49859c766668e969cc800406b9))
 
-* feat(itool):
-add joystick for cursor
-add axis stretch sliders
-add keyboard shortcuts
-changed layout margins ([`3faf410`](https://github.com/kmnhan/erlabpy/commit/3faf410676af1e85ebe27282a80d65c2d55c17a0))
+* **itool** add joystick for cursor ([`3faf410`](https://github.com/kmnhan/erlabpy/commit/3faf410676af1e85ebe27282a80d65c2d55c17a0))
 
-* feat: cursor binning ([`9b3de32`](https://github.com/kmnhan/erlabpy/commit/9b3de32f3b1ee098b646b0ad663cd8a95de02e11))
+* cursor binning ([`9b3de32`](https://github.com/kmnhan/erlabpy/commit/9b3de32f3b1ee098b646b0ad663cd8a95de02e11))
 
-* feat: new convenience function ([`e482cf6`](https://github.com/kmnhan/erlabpy/commit/e482cf6234e5b865b36ed2574c9566b199806c26))
+* new convenience function ([`e482cf6`](https://github.com/kmnhan/erlabpy/commit/e482cf6234e5b865b36ed2574c9566b199806c26))
 
-* feat: add Fermi edge correction from fit result ([`607e6ee`](https://github.com/kmnhan/erlabpy/commit/607e6eedef84b05f83cef7097c7ce0aaedbb2f97))
+* add Fermi edge correction from fit result ([`607e6ee`](https://github.com/kmnhan/erlabpy/commit/607e6eedef84b05f83cef7097c7ce0aaedbb2f97))
 
-* feat: add tool for analyzing dispersive features ([`7926238`](https://github.com/kmnhan/erlabpy/commit/792623836b77502f7d4ab065712465df007fb1ed))
+* add tool for analyzing dispersive features ([`7926238`](https://github.com/kmnhan/erlabpy/commit/792623836b77502f7d4ab065712465df007fb1ed))
 
-* feat: add pyqtgraph-based itool, WIP ([`de462c7`](https://github.com/kmnhan/erlabpy/commit/de462c7ab22d5ba47b686e05eaa0cc6558d2d4be))
+* add pyqtgraph-based itool, WIP ([`de462c7`](https://github.com/kmnhan/erlabpy/commit/de462c7ab22d5ba47b686e05eaa0cc6558d2d4be))
 
-* feat(itool): add invert colormap ([`bd616ad`](https://github.com/kmnhan/erlabpy/commit/bd616adf30cdee0f96433d9cb8ca8febedf5207c))
+* **itool** add invert colormap ([`bd616ad`](https://github.com/kmnhan/erlabpy/commit/bd616adf30cdee0f96433d9cb8ca8febedf5207c))
 
-* feat(itool): add color picker ([`cb40537`](https://github.com/kmnhan/erlabpy/commit/cb405377302855b357387a539a37f7f466b83447))
+* **itool** add color picker ([`cb40537`](https://github.com/kmnhan/erlabpy/commit/cb405377302855b357387a539a37f7f466b83447))
 
-* feat(itool): add binning ([`4d8155d`](https://github.com/kmnhan/erlabpy/commit/4d8155dd85da507ee87b09cb604ed2cba2ea7e42))
+* **itool** add binning ([`4d8155d`](https://github.com/kmnhan/erlabpy/commit/4d8155dd85da507ee87b09cb604ed2cba2ea7e42))
 
-* feat: add dark mode ([`a0dfefd`](https://github.com/kmnhan/erlabpy/commit/a0dfefdc65676b631ceb380216cfbdbdeab6f2f8))
+* add dark mode ([`a0dfefd`](https://github.com/kmnhan/erlabpy/commit/a0dfefdc65676b631ceb380216cfbdbdeab6f2f8))
 
-* feat(itool): 2d image support ([`98d0af7`](https://github.com/kmnhan/erlabpy/commit/98d0af799729884f5ccec203ffacebbffbe72f91))
+* **itool** 2d image support ([`98d0af7`](https://github.com/kmnhan/erlabpy/commit/98d0af799729884f5ccec203ffacebbffbe72f91))
 
-* feat: add toggle for cursor snap ([`d9ccfbd`](https://github.com/kmnhan/erlabpy/commit/d9ccfbdd8b36fce57655ffe04109fffda5c86189))
+* add toggle for cursor snap ([`d9ccfbd`](https://github.com/kmnhan/erlabpy/commit/d9ccfbdd8b36fce57655ffe04109fffda5c86189))
 
-* feat: add energy and resolution slider to ktool ([`94e886a`](https://github.com/kmnhan/erlabpy/commit/94e886ab02d638059311b6c6cb43957c3bbde1a9))
+* add energy and resolution slider to ktool ([`94e886a`](https://github.com/kmnhan/erlabpy/commit/94e886ab02d638059311b6c6cb43957c3bbde1a9))
 
-* feat: add qt and mpl-based interactive tools ([`823c509`](https://github.com/kmnhan/erlabpy/commit/823c50972fb5afe92f10c9409ed61a7c626971fb))
+* add qt and mpl-based interactive tools ([`823c509`](https://github.com/kmnhan/erlabpy/commit/823c50972fb5afe92f10c9409ed61a7c626971fb))
 
-* feat: added LabeledCursor ([`c970413`](https://github.com/kmnhan/erlabpy/commit/c970413dafd391c3da2e81efb1009e0452a6ec51))
+* added LabeledCursor ([`c970413`](https://github.com/kmnhan/erlabpy/commit/c970413dafd391c3da2e81efb1009e0452a6ec51))
 
-* feat: added annotation macros ([`dd36878`](https://github.com/kmnhan/erlabpy/commit/dd36878e25acd2b7cff5f34442f93b40307ff452))
+* added annotation macros ([`dd36878`](https://github.com/kmnhan/erlabpy/commit/dd36878e25acd2b7cff5f34442f93b40307ff452))
 
-* feat: Add characterization module ([`e5c56e8`](https://github.com/kmnhan/erlabpy/commit/e5c56e8903d5bcfa95d0d665186b4c1bb33c81a7))
+* Add characterization module ([`e5c56e8`](https://github.com/kmnhan/erlabpy/commit/e5c56e8903d5bcfa95d0d665186b4c1bb33c81a7))
 
 ### Fix
 
-* fix(era.fit.models): undefined name in all ([`308f525`](https://github.com/kmnhan/erlabpy/commit/308f525dd291247b631ac8a878d572ea3bfd2230))
+* **era.fit.models** undefined name in all ([`308f525`](https://github.com/kmnhan/erlabpy/commit/308f525dd291247b631ac8a878d572ea3bfd2230))
 
-* fix: invalid escape ([`a0a33b6`](https://github.com/kmnhan/erlabpy/commit/a0a33b6695471fb85060c35f17c0cb39d9a6338b))
+* invalid escape ([`a0a33b6`](https://github.com/kmnhan/erlabpy/commit/a0a33b6695471fb85060c35f17c0cb39d9a6338b))
 
-* fix(interpolate): make output shape consistent with scipy ([`0709493`](https://github.com/kmnhan/erlabpy/commit/07094935339bd29ab1c2fce5bf0a4478121a69c7))
+* **interpolate** make output shape consistent with scipy ([`0709493`](https://github.com/kmnhan/erlabpy/commit/07094935339bd29ab1c2fce5bf0a4478121a69c7))
 
-* fix: do not reset offsets on accessor initialization if exists ([`5328483`](https://github.com/kmnhan/erlabpy/commit/5328483587da21de3e11966d4baab4bc0fefce12))
+* do not reset offsets on accessor initialization if exists ([`5328483`](https://github.com/kmnhan/erlabpy/commit/5328483587da21de3e11966d4baab4bc0fefce12))
 
-* fix(itool): properly parse colorcet cmaps ([`cb81811`](https://github.com/kmnhan/erlabpy/commit/cb81811f4a1b9ea24657d2aa27a7455825fb4eff))
+* **itool** properly parse colorcet cmaps ([`cb81811`](https://github.com/kmnhan/erlabpy/commit/cb81811f4a1b9ea24657d2aa27a7455825fb4eff))
 
-* fix: add some more guess constraints, fix type ([`82825a7`](https://github.com/kmnhan/erlabpy/commit/82825a79af122602435802d3a3aab349ef2e37b7))
+* add some more guess constraints, fix type ([`82825a7`](https://github.com/kmnhan/erlabpy/commit/82825a79af122602435802d3a3aab349ef2e37b7))
 
-* fix(goldtool): round roi position to 3 decimal places ([`d83fafa`](https://github.com/kmnhan/erlabpy/commit/d83fafa0712726fee935755a0d3f816100f90666))
+* **goldtool** round roi position to 3 decimal places ([`d83fafa`](https://github.com/kmnhan/erlabpy/commit/d83fafa0712726fee935755a0d3f816100f90666))
 
-* fix(goldtool): disable memmapping for parallel fitting ([`0c8b053`](https://github.com/kmnhan/erlabpy/commit/0c8b053e2a741f28aa622a2d9ba7e847a82bd8d0))
+* **goldtool** disable memmapping for parallel fitting ([`0c8b053`](https://github.com/kmnhan/erlabpy/commit/0c8b053e2a741f28aa622a2d9ba7e847a82bd8d0))
 
-* fix: duplicated data_dir ([`4b08754`](https://github.com/kmnhan/erlabpy/commit/4b087543059e730c0085b0a656424329cf99bf08))
+* duplicated data_dir ([`4b08754`](https://github.com/kmnhan/erlabpy/commit/4b087543059e730c0085b0a656424329cf99bf08))
 
-* fix: missing import ([`a1241da`](https://github.com/kmnhan/erlabpy/commit/a1241da6cbdffb68cb9405236d0bbb40bcf16815))
+* missing import ([`a1241da`](https://github.com/kmnhan/erlabpy/commit/a1241da6cbdffb68cb9405236d0bbb40bcf16815))
 
-* fix(io): fix duplicated loader aliases ([`d832a48`](https://github.com/kmnhan/erlabpy/commit/d832a487e6e63befa24049992eed8a6fbd2a2be7))
+* **io** fix duplicated loader aliases ([`d832a48`](https://github.com/kmnhan/erlabpy/commit/d832a487e6e63befa24049992eed8a6fbd2a2be7))
 
-* fix: syntax error ([`63214f3`](https://github.com/kmnhan/erlabpy/commit/63214f35fd9009e04d7ed4299bf9327ba18f08e0))
+* syntax error ([`63214f3`](https://github.com/kmnhan/erlabpy/commit/63214f35fd9009e04d7ed4299bf9327ba18f08e0))
 
-* fix(io.plugins.merlin): files with non-standard names  are properly summarized ([`388dd02`](https://github.com/kmnhan/erlabpy/commit/388dd0266e82557a250f9d20dff3a918b139cf00))
+* **io.plugins.merlin** files with non-standard names  are properly summarized ([`388dd02`](https://github.com/kmnhan/erlabpy/commit/388dd0266e82557a250f9d20dff3a918b139cf00))
 
-* fix: move positional to keyword only ([`ae300b3`](https://github.com/kmnhan/erlabpy/commit/ae300b3a9158940e07ccd585fc76750e3652593c))
+* move positional to keyword only ([`ae300b3`](https://github.com/kmnhan/erlabpy/commit/ae300b3a9158940e07ccd585fc76750e3652593c))
 
-* fix(io): return full path for get_files ([`bbaab33`](https://github.com/kmnhan/erlabpy/commit/bbaab3328c09a385762c0d65d00e24ef50ed9273))
+* **io** return full path for get_files ([`bbaab33`](https://github.com/kmnhan/erlabpy/commit/bbaab3328c09a385762c0d65d00e24ef50ed9273))
 
-* fix: make fit result accessible ([`a40ae66`](https://github.com/kmnhan/erlabpy/commit/a40ae6616721a320eac51e69b7206ec7bf70f243))
+* make fit result accessible ([`a40ae66`](https://github.com/kmnhan/erlabpy/commit/a40ae6616721a320eac51e69b7206ec7bf70f243))
 
-* fix: typo in multipeakfunction ([`cafe6cc`](https://github.com/kmnhan/erlabpy/commit/cafe6cc405650921b0a28cc9831b53b448e620ff))
+* typo in multipeakfunction ([`cafe6cc`](https://github.com/kmnhan/erlabpy/commit/cafe6cc405650921b0a28cc9831b53b448e620ff))
 
-* fix(ktool): round angle offsets ([`31c4730`](https://github.com/kmnhan/erlabpy/commit/31c4730663b24a344ded9a658580981732445100))
+* **ktool** round angle offsets ([`31c4730`](https://github.com/kmnhan/erlabpy/commit/31c4730663b24a344ded9a658580981732445100))
 
-* fix(io): when given path to file, skip regex parsing ([`92019bb`](https://github.com/kmnhan/erlabpy/commit/92019bb56b5b8f818bc311a294150644149899ec))
+* **io** when given path to file, skip regex parsing ([`92019bb`](https://github.com/kmnhan/erlabpy/commit/92019bb56b5b8f818bc311a294150644149899ec))
 
-* fix: more realistic angle data generation ([`498e7f5`](https://github.com/kmnhan/erlabpy/commit/498e7f52ce567efe8029f2d4baec7ccb12d607db))
+* more realistic angle data generation ([`498e7f5`](https://github.com/kmnhan/erlabpy/commit/498e7f52ce567efe8029f2d4baec7ccb12d607db))
 
-* fix: return type ([`c089f44`](https://github.com/kmnhan/erlabpy/commit/c089f4404c4e63172e1da1d06d167ea75fef5841))
+* return type ([`c089f44`](https://github.com/kmnhan/erlabpy/commit/c089f4404c4e63172e1da1d06d167ea75fef5841))
 
-* fix: move doc comments to above ([`429c868`](https://github.com/kmnhan/erlabpy/commit/429c8681dd90bc3c7c890377eb37f4ad1414c3f7))
+* move doc comments to above ([`429c868`](https://github.com/kmnhan/erlabpy/commit/429c8681dd90bc3c7c890377eb37f4ad1414c3f7))
 
-* fix(docs): avoid direct import in conf.py ([`db930f0`](https://github.com/kmnhan/erlabpy/commit/db930f03f7d308f677dfa5c1385e3dd6c9bf3d0e))
+* **docs** avoid direct import in conf.py ([`db930f0`](https://github.com/kmnhan/erlabpy/commit/db930f03f7d308f677dfa5c1385e3dd6c9bf3d0e))
 
-* fix(ktool): default values and data orientation ([`1dcf1f4`](https://github.com/kmnhan/erlabpy/commit/1dcf1f4ca773c5ea5e30146a8fec927851ec54a5))
+* **ktool** default values and data orientation ([`1dcf1f4`](https://github.com/kmnhan/erlabpy/commit/1dcf1f4ca773c5ea5e30146a8fec927851ec54a5))
 
-* fix: Update ktool.py to keep up with refactoring changes ([`f23afb2`](https://github.com/kmnhan/erlabpy/commit/f23afb25c5a2141a53e7427cb0e4ea1291e008f3))
+* Update ktool.py to keep up with refactoring changes ([`f23afb2`](https://github.com/kmnhan/erlabpy/commit/f23afb25c5a2141a53e7427cb0e4ea1291e008f3))
 
-* fix: fix typo in documentation ([`5c527a4`](https://github.com/kmnhan/erlabpy/commit/5c527a4da449867231cf4ca548cd147cd7657edb))
+* fix typo in documentation ([`5c527a4`](https://github.com/kmnhan/erlabpy/commit/5c527a4da449867231cf4ca548cd147cd7657edb))
 
-* fix: properly execute in ipython ([`262b965`](https://github.com/kmnhan/erlabpy/commit/262b96518e38cecacf36141614da44d7bf7e3deb))
+* properly execute in ipython ([`262b965`](https://github.com/kmnhan/erlabpy/commit/262b96518e38cecacf36141614da44d7bf7e3deb))
 
-* fix: momentum conversion offset ([`7836ce1`](https://github.com/kmnhan/erlabpy/commit/7836ce137d12f8b68725ca333ce2536a9e0ab24c))
+* momentum conversion offset ([`7836ce1`](https://github.com/kmnhan/erlabpy/commit/7836ce137d12f8b68725ca333ce2536a9e0ab24c))
 
-* fix: Update pyproject.toml with package-dir ([`c56fe0f`](https://github.com/kmnhan/erlabpy/commit/c56fe0f28b537d7e0601d33e9f20efc3f3c87310))
+* Update pyproject.toml with package-dir ([`c56fe0f`](https://github.com/kmnhan/erlabpy/commit/c56fe0f28b537d7e0601d33e9f20efc3f3c87310))
 
-* fix: Update requirements.txt ([`6b3150a`](https://github.com/kmnhan/erlabpy/commit/6b3150a1f49feb349a8fe5e3aa5d07b53d058a00))
+* Update requirements.txt ([`6b3150a`](https://github.com/kmnhan/erlabpy/commit/6b3150a1f49feb349a8fe5e3aa5d07b53d058a00))
 
-* fix: Update docs/requirements.txt ([`5835db9`](https://github.com/kmnhan/erlabpy/commit/5835db9d53c13bc6da16d2b0f5f2e4695a5cd6fd))
+* Update docs/requirements.txt ([`5835db9`](https://github.com/kmnhan/erlabpy/commit/5835db9d53c13bc6da16d2b0f5f2e4695a5cd6fd))
 
-* fix: enable dynamic versioning ([`cc0fc96`](https://github.com/kmnhan/erlabpy/commit/cc0fc96a191abf807a80433025b243fc9d11431c))
+* enable dynamic versioning ([`cc0fc96`](https://github.com/kmnhan/erlabpy/commit/cc0fc96a191abf807a80433025b243fc9d11431c))
 
-* fix: Add packages to setuptools configuration ([`a2bbdcf`](https://github.com/kmnhan/erlabpy/commit/a2bbdcf6950de42c56c0f558d0d13c6521f7887f))
+* Add packages to setuptools configuration ([`a2bbdcf`](https://github.com/kmnhan/erlabpy/commit/a2bbdcf6950de42c56c0f558d0d13c6521f7887f))
 
-* fix: Add version number to pyproject.toml ([`0caf0c4`](https://github.com/kmnhan/erlabpy/commit/0caf0c40f3dc943f786fe06e68d54b779367edad))
+* Add version number to pyproject.toml ([`0caf0c4`](https://github.com/kmnhan/erlabpy/commit/0caf0c40f3dc943f786fe06e68d54b779367edad))
 
-* fix: update version ([`d394f20`](https://github.com/kmnhan/erlabpy/commit/d394f204387a1f3fdb18006298002d03b0a8b0d3))
+* update version ([`d394f20`](https://github.com/kmnhan/erlabpy/commit/d394f204387a1f3fdb18006298002d03b0a8b0d3))
 
-* fix: Update Sphinx configuration path in .readthedocs.yaml ([`21c1b1f`](https://github.com/kmnhan/erlabpy/commit/21c1b1f02b7e8b356d86074fe5c0f89895afbc90))
+* Update Sphinx configuration path in .readthedocs.yaml ([`21c1b1f`](https://github.com/kmnhan/erlabpy/commit/21c1b1f02b7e8b356d86074fe5c0f89895afbc90))
 
-* fix(itool): ignore zerodivision ([`97e2bf5`](https://github.com/kmnhan/erlabpy/commit/97e2bf56c6e351dcfe6bd382c5b888ef12b44f4a))
+* **itool** ignore zerodivision ([`97e2bf5`](https://github.com/kmnhan/erlabpy/commit/97e2bf56c6e351dcfe6bd382c5b888ef12b44f4a))
 
-* fix: try to make autoscale_off context more reliable, needs testing ([`3a4726a`](https://github.com/kmnhan/erlabpy/commit/3a4726a90343bee7af916490a76679a027fc6aa1))
+* try to make autoscale_off context more reliable, needs testing ([`3a4726a`](https://github.com/kmnhan/erlabpy/commit/3a4726a90343bee7af916490a76679a027fc6aa1))
 
-* fix: gradient_fill now doesn&#39;t mess with autoscale ([`040db5a`](https://github.com/kmnhan/erlabpy/commit/040db5a6aeaebbdb628a5ff05bddce53f5f825bd))
+* gradient_fill now doesn&#39;t mess with autoscale ([`040db5a`](https://github.com/kmnhan/erlabpy/commit/040db5a6aeaebbdb628a5ff05bddce53f5f825bd))
 
-* fix: proper file handler termination ([`2ca7593`](https://github.com/kmnhan/erlabpy/commit/2ca7593b3036f8c13dda8ec7ae34a18ad8ef572c))
+* proper file handler termination ([`2ca7593`](https://github.com/kmnhan/erlabpy/commit/2ca7593b3036f8c13dda8ec7ae34a18ad8ef572c))
 
-* fix: acf2 stack dimension mismatch resolved ([`8dde2da`](https://github.com/kmnhan/erlabpy/commit/8dde2da853bc756cabc79e0587b93d5f99c92efb))
+* acf2 stack dimension mismatch resolved ([`8dde2da`](https://github.com/kmnhan/erlabpy/commit/8dde2da853bc756cabc79e0587b93d5f99c92efb))
 
-* fix: validation changed, fixes #11 ([`8479814`](https://github.com/kmnhan/erlabpy/commit/84798146b8596ee4cd75e89282180f4e858176b3))
+* validation changed, fixes #11 ([`8479814`](https://github.com/kmnhan/erlabpy/commit/84798146b8596ee4cd75e89282180f4e858176b3))
 
-* fix(interactive): override copy, temporarily fixes #10 ([`4e99863`](https://github.com/kmnhan/erlabpy/commit/4e99863b2ce5b6fe82f0fbe3658cf9b024f69fb0))
+* **interactive** override copy, temporarily fixes #10 ([`4e99863`](https://github.com/kmnhan/erlabpy/commit/4e99863b2ce5b6fe82f0fbe3658cf9b024f69fb0))
 
-* fix: subclass scalarformatter for better compat ([`b69bfd6`](https://github.com/kmnhan/erlabpy/commit/b69bfd6607aa283c1e717e8183982ef1c40d9749))
+* subclass scalarformatter for better compat ([`b69bfd6`](https://github.com/kmnhan/erlabpy/commit/b69bfd6607aa283c1e717e8183982ef1c40d9749))
 
-* fix: nice horizontal colorbar ([`2766e36`](https://github.com/kmnhan/erlabpy/commit/2766e3689ef3ebe5152ec5ce8fe22373127a507b))
+* nice horizontal colorbar ([`2766e36`](https://github.com/kmnhan/erlabpy/commit/2766e3689ef3ebe5152ec5ce8fe22373127a507b))
 
-* fix(colors): handle callable segmented cmaps ([`8135d73`](https://github.com/kmnhan/erlabpy/commit/8135d73e3d11f7e8126576b7b2281a15ec6e2920))
+* **colors** handle callable segmented cmaps ([`8135d73`](https://github.com/kmnhan/erlabpy/commit/8135d73e3d11f7e8126576b7b2281a15ec6e2920))
 
-* fix(itool): keyboard modifier syntax ([`d593258`](https://github.com/kmnhan/erlabpy/commit/d5932583b6b36f288a72a5d4965c81c805c55c66))
+* **itool** keyboard modifier syntax ([`d593258`](https://github.com/kmnhan/erlabpy/commit/d5932583b6b36f288a72a5d4965c81c805c55c66))
 
-* fix(io): fix da30 loading ([`ee0615d`](https://github.com/kmnhan/erlabpy/commit/ee0615dd31fff487139350df692045b646402c03))
+* **io** fix da30 loading ([`ee0615d`](https://github.com/kmnhan/erlabpy/commit/ee0615dd31fff487139350df692045b646402c03))
 
-* fix: fix typo ([`6a84557`](https://github.com/kmnhan/erlabpy/commit/6a845573f8c0bc0d03c6003a218e6d1322c6a05e))
+* fix typo ([`6a84557`](https://github.com/kmnhan/erlabpy/commit/6a845573f8c0bc0d03c6003a218e6d1322c6a05e))
 
-* fix: load da30 map angle in radians ([`8d08c65`](https://github.com/kmnhan/erlabpy/commit/8d08c6533cbb57b225d5ee9ae99d1795ab5ec300))
+* load da30 map angle in radians ([`8d08c65`](https://github.com/kmnhan/erlabpy/commit/8d08c6533cbb57b225d5ee9ae99d1795ab5ec300))
 
-* fix: remove duplicate star ([`a018691`](https://github.com/kmnhan/erlabpy/commit/a0186915be3fc7065fbb19af5ff68d491167a468))
+* remove duplicate star ([`a018691`](https://github.com/kmnhan/erlabpy/commit/a0186915be3fc7065fbb19af5ff68d491167a468))
 
-* fix(itool): update io ([`8c082b0`](https://github.com/kmnhan/erlabpy/commit/8c082b0f2c814e101e25dd99002e5fb45fccd744))
+* **itool** update io ([`8c082b0`](https://github.com/kmnhan/erlabpy/commit/8c082b0f2c814e101e25dd99002e5fb45fccd744))
 
-* fix(itool): handle ambiguous datasets ([`9226c12`](https://github.com/kmnhan/erlabpy/commit/9226c12f93ddceb35ea5b8852989dcf15620f9c6))
+* **itool** handle ambiguous datasets ([`9226c12`](https://github.com/kmnhan/erlabpy/commit/9226c12f93ddceb35ea5b8852989dcf15620f9c6))
 
-* fix(itool): catch overflow ([`ae1afe1`](https://github.com/kmnhan/erlabpy/commit/ae1afe16e67b76789c5adc59f1e0b149010cfc2f))
+* **itool** catch overflow ([`ae1afe1`](https://github.com/kmnhan/erlabpy/commit/ae1afe16e67b76789c5adc59f1e0b149010cfc2f))
 
-* fix: patch breaking changes in lmfit 1.2.2 ([`8179fc3`](https://github.com/kmnhan/erlabpy/commit/8179fc308976d3ac8ca8575136bea7382ee85eac))
+* patch breaking changes in lmfit 1.2.2 ([`8179fc3`](https://github.com/kmnhan/erlabpy/commit/8179fc308976d3ac8ca8575136bea7382ee85eac))
 
-* fix: make colorbar more robust ([`3a4968d`](https://github.com/kmnhan/erlabpy/commit/3a4968dd5983fc4bcde43bdf3056c3cc467be070))
+* make colorbar more robust ([`3a4968d`](https://github.com/kmnhan/erlabpy/commit/3a4968dd5983fc4bcde43bdf3056c3cc467be070))
 
-* fix: resistance data loading ([`7db3c4a`](https://github.com/kmnhan/erlabpy/commit/7db3c4abae28ae2ef99d1e8a54aa2744a3bde025))
+* resistance data loading ([`7db3c4a`](https://github.com/kmnhan/erlabpy/commit/7db3c4abae28ae2ef99d1e8a54aa2744a3bde025))
 
-* fix: typo ([`a74732d`](https://github.com/kmnhan/erlabpy/commit/a74732d8429beb94a3009cbfde004387e4fae762))
+* typo ([`a74732d`](https://github.com/kmnhan/erlabpy/commit/a74732d8429beb94a3009cbfde004387e4fae762))
 
-* fix: fix critical typo ([`3e10834`](https://github.com/kmnhan/erlabpy/commit/3e10834a8f9f5f78a9a41f3567f2fb4a9d092245))
+* fix critical typo ([`3e10834`](https://github.com/kmnhan/erlabpy/commit/3e10834a8f9f5f78a9a41f3567f2fb4a9d092245))
 
-* fix: handle undetermined spectrum type ([`b59c3e9`](https://github.com/kmnhan/erlabpy/commit/b59c3e9068de1c26c1efced8ee0ffdc62c256f1c))
+* handle undetermined spectrum type ([`b59c3e9`](https://github.com/kmnhan/erlabpy/commit/b59c3e9068de1c26c1efced8ee0ffdc62c256f1c))
 
-* fix(ssrl52): improve compatibility with old data ([`135b022`](https://github.com/kmnhan/erlabpy/commit/135b022996259da7ee379a49a0bb13327182ef51))
+* **ssrl52** improve compatibility with old data ([`135b022`](https://github.com/kmnhan/erlabpy/commit/135b022996259da7ee379a49a0bb13327182ef51))
 
-* fix: remove now-redundant patches ([`687ece9`](https://github.com/kmnhan/erlabpy/commit/687ece99866628da3fbb302981d005cf57552cfb))
+* remove now-redundant patches ([`687ece9`](https://github.com/kmnhan/erlabpy/commit/687ece99866628da3fbb302981d005cf57552cfb))
 
-* fix: improve ZT image view for 4D ([`c8d07b5`](https://github.com/kmnhan/erlabpy/commit/c8d07b522216f191a94a7ef40d7beda478e46074))
+* improve ZT image view for 4D ([`c8d07b5`](https://github.com/kmnhan/erlabpy/commit/c8d07b522216f191a94a7ef40d7beda478e46074))
 
-* fix: keep slicer object for expected signal behavior ([`e0ebe85`](https://github.com/kmnhan/erlabpy/commit/e0ebe8519d972467332965be4ac097df0c26d530))
+* keep slicer object for expected signal behavior ([`e0ebe85`](https://github.com/kmnhan/erlabpy/commit/e0ebe8519d972467332965be4ac097df0c26d530))
 
-* fix: keep slicer object for expected signal behavior ([`2c401e6`](https://github.com/kmnhan/erlabpy/commit/2c401e643f08eadbf3f3c84854332ee95d89451d))
+* keep slicer object for expected signal behavior ([`2c401e6`](https://github.com/kmnhan/erlabpy/commit/2c401e643f08eadbf3f3c84854332ee95d89451d))
 
-* fix: indexerror on loading higher dimensional data ([`e068bec`](https://github.com/kmnhan/erlabpy/commit/e068bec807b8f744c5b5925ef1208130c9136c2b))
+* indexerror on loading higher dimensional data ([`e068bec`](https://github.com/kmnhan/erlabpy/commit/e068bec807b8f744c5b5925ef1208130c9136c2b))
 
-* fix: binning control order not updating on transpose ([`bdfda97`](https://github.com/kmnhan/erlabpy/commit/bdfda979475ecc8efeb1e8c80cf45a006f2ff85f))
+* binning control order not updating on transpose ([`bdfda97`](https://github.com/kmnhan/erlabpy/commit/bdfda979475ecc8efeb1e8c80cf45a006f2ff85f))
 
-* fix: labels should not displace subplots ([`43b9258`](https://github.com/kmnhan/erlabpy/commit/43b925846306b311fcd309bc14a89390a51fb99e))
+* labels should not displace subplots ([`43b9258`](https://github.com/kmnhan/erlabpy/commit/43b925846306b311fcd309bc14a89390a51fb99e))
 
-* fix: revert clean_labels ([`1316fce`](https://github.com/kmnhan/erlabpy/commit/1316fce90142b41e423b0f7464768ea8b178599e))
+* revert clean_labels ([`1316fce`](https://github.com/kmnhan/erlabpy/commit/1316fce90142b41e423b0f7464768ea8b178599e))
 
-* fix: dimension mismatch ([`68fc306`](https://github.com/kmnhan/erlabpy/commit/68fc3063294bee4c89581b252cb49e71fc40b377))
+* dimension mismatch ([`68fc306`](https://github.com/kmnhan/erlabpy/commit/68fc3063294bee4c89581b252cb49e71fc40b377))
 
-* fix: circular import ([`186cb03`](https://github.com/kmnhan/erlabpy/commit/186cb03f4a93cba01773b2a5dac848ad16a761cd))
+* circular import ([`186cb03`](https://github.com/kmnhan/erlabpy/commit/186cb03f4a93cba01773b2a5dac848ad16a761cd))
 
-* fix: make qt progressbar more accurate ([`7c83b31`](https://github.com/kmnhan/erlabpy/commit/7c83b3100d7880577c533c3b17b77d6b643759c8))
+* make qt progressbar more accurate ([`7c83b31`](https://github.com/kmnhan/erlabpy/commit/7c83b3100d7880577c533c3b17b77d6b643759c8))
 
-* fix: revert default pad ([`8e5715c`](https://github.com/kmnhan/erlabpy/commit/8e5715ce5f2c89c236ae7791820dcf5a7411fcc1))
+* revert default pad ([`8e5715c`](https://github.com/kmnhan/erlabpy/commit/8e5715ce5f2c89c236ae7791820dcf5a7411fcc1))
 
-* fix(goldtool): keyerror on code generation ([`e421719`](https://github.com/kmnhan/erlabpy/commit/e4217193441cabca6f8bce3e4001a530dea02678))
+* **goldtool** keyerror on code generation ([`e421719`](https://github.com/kmnhan/erlabpy/commit/e4217193441cabca6f8bce3e4001a530dea02678))
 
-* fix(io): make save and load work with datasets ([`a4f1a12`](https://github.com/kmnhan/erlabpy/commit/a4f1a1279fb0070f38119e80b04bdbf19739b50c))
+* **io** make save and load work with datasets ([`a4f1a12`](https://github.com/kmnhan/erlabpy/commit/a4f1a1279fb0070f38119e80b04bdbf19739b50c))
 
-* fix(style): nonzero pad on savefig ([`b21a178`](https://github.com/kmnhan/erlabpy/commit/b21a17829d95d69aee2affe4c590c082b1cb22ca))
+* **style** nonzero pad on savefig ([`b21a178`](https://github.com/kmnhan/erlabpy/commit/b21a17829d95d69aee2affe4c590c082b1cb22ca))
 
-* fix: gold fit autoscale ([`b81e4e8`](https://github.com/kmnhan/erlabpy/commit/b81e4e86f72eedbc63e256de14b70298c2c591f4))
+* gold fit autoscale ([`b81e4e8`](https://github.com/kmnhan/erlabpy/commit/b81e4e86f72eedbc63e256de14b70298c2c591f4))
 
-* fix(io): can now load BL4 pxt files ([`d318c91`](https://github.com/kmnhan/erlabpy/commit/d318c91bdaa4adc2fb54be647e5932463e84474c))
+* **io** can now load BL4 pxt files ([`d318c91`](https://github.com/kmnhan/erlabpy/commit/d318c91bdaa4adc2fb54be647e5932463e84474c))
 
-* fix: gold fit autoscaling ([`9ed8f86`](https://github.com/kmnhan/erlabpy/commit/9ed8f86f68006a648e0ed2868ff65dd451b9f2ff))
+* gold fit autoscaling ([`9ed8f86`](https://github.com/kmnhan/erlabpy/commit/9ed8f86f68006a648e0ed2868ff65dd451b9f2ff))
 
-* fix: disable covariance matrix scaling ([`a3264c7`](https://github.com/kmnhan/erlabpy/commit/a3264c70bf9d2bb502b83f7265482ff462dba11a))
+* disable covariance matrix scaling ([`a3264c7`](https://github.com/kmnhan/erlabpy/commit/a3264c70bf9d2bb502b83f7265482ff462dba11a))
 
-* fix: try to fix random segfault with numba ([`3505b42`](https://github.com/kmnhan/erlabpy/commit/3505b4291b34697732f2dccc33f81f5c32e5fcad))
+* try to fix random segfault with numba ([`3505b42`](https://github.com/kmnhan/erlabpy/commit/3505b4291b34697732f2dccc33f81f5c32e5fcad))
 
-* fix: stupid regression in plot_array ([`2ef2ad6`](https://github.com/kmnhan/erlabpy/commit/2ef2ad62227798c0ab3b72ccd9132086fd8a3e45))
+* stupid regression in plot_array ([`2ef2ad6`](https://github.com/kmnhan/erlabpy/commit/2ef2ad62227798c0ab3b72ccd9132086fd8a3e45))
 
-* fix: stupid regression on rename ([`cc37d8e`](https://github.com/kmnhan/erlabpy/commit/cc37d8e86e7a0ea36a89b265b6409aa2898c302c))
+* stupid regression on rename ([`cc37d8e`](https://github.com/kmnhan/erlabpy/commit/cc37d8e86e7a0ea36a89b265b6409aa2898c302c))
 
-* fix: wrong attributes ([`01812ba`](https://github.com/kmnhan/erlabpy/commit/01812bad65847dbe33d1afe013c564898c3c99a6))
+* wrong attributes ([`01812ba`](https://github.com/kmnhan/erlabpy/commit/01812bad65847dbe33d1afe013c564898c3c99a6))
 
-* fix: invert before gamma ([`c70bff5`](https://github.com/kmnhan/erlabpy/commit/c70bff5b59a17d59260a1289e8c3df007194b762))
+* invert before gamma ([`c70bff5`](https://github.com/kmnhan/erlabpy/commit/c70bff5b59a17d59260a1289e8c3df007194b762))
 
-* fix(io): fix livexy and livepolar loader dims ([`edcf9a8`](https://github.com/kmnhan/erlabpy/commit/edcf9a8640169bebb427f768baeb82735494ab40))
+* **io** fix livexy and livepolar loader dims ([`edcf9a8`](https://github.com/kmnhan/erlabpy/commit/edcf9a8640169bebb427f768baeb82735494ab40))
 
-* fix(itool): restore compatibility for float64 data ([`4e8baab`](https://github.com/kmnhan/erlabpy/commit/4e8baabb0f592294862bcbda41bdf1422748ab62))
+* **itool** restore compatibility for float64 data ([`4e8baab`](https://github.com/kmnhan/erlabpy/commit/4e8baabb0f592294862bcbda41bdf1422748ab62))
 
-* fix: resolve type related problems ([`4ec5bdd`](https://github.com/kmnhan/erlabpy/commit/4ec5bddc2c82076eab3e973845d21f188cf09161))
+* resolve type related problems ([`4ec5bdd`](https://github.com/kmnhan/erlabpy/commit/4ec5bddc2c82076eab3e973845d21f188cf09161))
 
-* fix: fix typo in comment ([`8cd71df`](https://github.com/kmnhan/erlabpy/commit/8cd71df415b5715a64c81dcf338f44abee21fa7d))
+* fix typo in comment ([`8cd71df`](https://github.com/kmnhan/erlabpy/commit/8cd71df415b5715a64c81dcf338f44abee21fa7d))
 
-* fix: remove type hints, were causing thread errors ([`1ed309c`](https://github.com/kmnhan/erlabpy/commit/1ed309c58ea3c8da696d352e1df0ba03903c223b))
+* remove type hints, were causing thread errors ([`1ed309c`](https://github.com/kmnhan/erlabpy/commit/1ed309c58ea3c8da696d352e1df0ba03903c223b))
 
-* fix: edge correction with callable ([`8a1052f`](https://github.com/kmnhan/erlabpy/commit/8a1052fe2678baca09042d8eb644d41a9ab48f56))
+* edge correction with callable ([`8a1052f`](https://github.com/kmnhan/erlabpy/commit/8a1052fe2678baca09042d8eb644d41a9ab48f56))
 
-* fix: default pad changed ([`a2039c2`](https://github.com/kmnhan/erlabpy/commit/a2039c2b9db91950d7d627b82614fad0a536f906))
+* default pad changed ([`a2039c2`](https://github.com/kmnhan/erlabpy/commit/a2039c2b9db91950d7d627b82614fad0a536f906))
 
-* fix: fix curve fitting on notebook ([`4126aa0`](https://github.com/kmnhan/erlabpy/commit/4126aa0fa6061c880b03d188199b3d40d64c4b84))
+* fix curve fitting on notebook ([`4126aa0`](https://github.com/kmnhan/erlabpy/commit/4126aa0fa6061c880b03d188199b3d40d64c4b84))
 
-* fix: compatibility with PyQt6 ([`01f550e`](https://github.com/kmnhan/erlabpy/commit/01f550e463ea14720d0e84cd43bf98501cf0b554))
+* compatibility with PyQt6 ([`01f550e`](https://github.com/kmnhan/erlabpy/commit/01f550e463ea14720d0e84cd43bf98501cf0b554))
 
-* fix: stupid commit ([`d3b1f53`](https://github.com/kmnhan/erlabpy/commit/d3b1f53448805691c3de358e2cdfca3cb631866a))
+* stupid commit ([`d3b1f53`](https://github.com/kmnhan/erlabpy/commit/d3b1f53448805691c3de358e2cdfca3cb631866a))
 
-* fix(io): add compatibiity check, fixes #9 ([`35c6bd7`](https://github.com/kmnhan/erlabpy/commit/35c6bd73753af06f49130dddc642baca008044e4))
+* **io** add compatibiity check, fixes #9 ([`35c6bd7`](https://github.com/kmnhan/erlabpy/commit/35c6bd73753af06f49130dddc642baca008044e4))
 
-* fix: correct color limits for new cursors ([`25e54f4`](https://github.com/kmnhan/erlabpy/commit/25e54f46bbca24ac54aa2cccf1abaacf9403ec68))
+* correct color limits for new cursors ([`25e54f4`](https://github.com/kmnhan/erlabpy/commit/25e54f46bbca24ac54aa2cccf1abaacf9403ec68))
 
-* fix: add PyQt6 compatibility ([`713cea2`](https://github.com/kmnhan/erlabpy/commit/713cea28683643f27c5b163c1aba0e332c168b30))
+* add PyQt6 compatibility ([`713cea2`](https://github.com/kmnhan/erlabpy/commit/713cea28683643f27c5b163c1aba0e332c168b30))
 
-* fix: pyqt-compatible multiple inheritance, fixes #7 ([`de37753`](https://github.com/kmnhan/erlabpy/commit/de377534db051b852d528ab8dd6abf212bf3e1a0))
+* pyqt-compatible multiple inheritance, fixes #7 ([`de37753`](https://github.com/kmnhan/erlabpy/commit/de377534db051b852d528ab8dd6abf212bf3e1a0))
 
-* fix: pyqt-compatible multiple inheritance, fixes #7 ([`7fb28d8`](https://github.com/kmnhan/erlabpy/commit/7fb28d834b149c1a7dd8bd09162d09fcf4890004))
+* pyqt-compatible multiple inheritance, fixes #7 ([`7fb28d8`](https://github.com/kmnhan/erlabpy/commit/7fb28d834b149c1a7dd8bd09162d09fcf4890004))
 
-* fix: minor fixes ([`2b4e61c`](https://github.com/kmnhan/erlabpy/commit/2b4e61cb086ae5f813aa1d784c722fbbc8613330))
+* minor fixes ([`2b4e61c`](https://github.com/kmnhan/erlabpy/commit/2b4e61cb086ae5f813aa1d784c722fbbc8613330))
 
-* fix: 2d colormap incorrect normalization ([`a425cb1`](https://github.com/kmnhan/erlabpy/commit/a425cb1bd560aa2e7047321ec2b21ecd0bc0779d))
+* 2d colormap incorrect normalization ([`a425cb1`](https://github.com/kmnhan/erlabpy/commit/a425cb1bd560aa2e7047321ec2b21ecd0bc0779d))
 
-* fix: set tol to 10x eps float32, fixes #5 ([`d4d2dc7`](https://github.com/kmnhan/erlabpy/commit/d4d2dc72fda8ece6875d50f03e337d1b9dd222de))
+* set tol to 10x eps float32, fixes #5 ([`d4d2dc7`](https://github.com/kmnhan/erlabpy/commit/d4d2dc72fda8ece6875d50f03e337d1b9dd222de))
 
-* fix: convert everything to float32, fixes #2 ([`8f2b58f`](https://github.com/kmnhan/erlabpy/commit/8f2b58f5218a4bdcb2d6fb8c8d6d8ef798c84a03))
+* convert everything to float32, fixes #2 ([`8f2b58f`](https://github.com/kmnhan/erlabpy/commit/8f2b58f5218a4bdcb2d6fb8c8d6d8ef798c84a03))
 
-* fix: fixes #3 ([`1ae6ff8`](https://github.com/kmnhan/erlabpy/commit/1ae6ff8cd58db64fc439cd034f2f93f6961bd6c9))
+* fixes #3 ([`1ae6ff8`](https://github.com/kmnhan/erlabpy/commit/1ae6ff8cd58db64fc439cd034f2f93f6961bd6c9))
 
-* fix: fixes #1 along with some memory optimization ([`a667c6a`](https://github.com/kmnhan/erlabpy/commit/a667c6a44fda268b7a450b4522d2ada193de0639))
+* fixes #1 along with some memory optimization ([`a667c6a`](https://github.com/kmnhan/erlabpy/commit/a667c6a44fda268b7a450b4522d2ada193de0639))
 
-* fix: choose nearest for zero width when plotting slices ([`6ba03da`](https://github.com/kmnhan/erlabpy/commit/6ba03da2c6054044701accc20763bac424ac3bcf))
+* choose nearest for zero width when plotting slices ([`6ba03da`](https://github.com/kmnhan/erlabpy/commit/6ba03da2c6054044701accc20763bac424ac3bcf))
 
-* fix(itool): multicursor colorbar ([`65bd992`](https://github.com/kmnhan/erlabpy/commit/65bd9923680a11e96350b8f9dab079934199bd3a))
+* **itool** multicursor colorbar ([`65bd992`](https://github.com/kmnhan/erlabpy/commit/65bd9923680a11e96350b8f9dab079934199bd3a))
 
-* fix: shift by DataArray ([`fd38eaf`](https://github.com/kmnhan/erlabpy/commit/fd38eaf479b1109f57f3dc30e7b4cc5964459bf7))
+* shift by DataArray ([`fd38eaf`](https://github.com/kmnhan/erlabpy/commit/fd38eaf479b1109f57f3dc30e7b4cc5964459bf7))
 
-* fix: force qt api ([`3613853`](https://github.com/kmnhan/erlabpy/commit/36138538c31ba1baaf6c5606372039aeb5dcfb95))
+* force qt api ([`3613853`](https://github.com/kmnhan/erlabpy/commit/36138538c31ba1baaf6c5606372039aeb5dcfb95))
 
-* fix: temperature not required when fitting with broadened step edge ([`4b83d87`](https://github.com/kmnhan/erlabpy/commit/4b83d8713044e8dfdaf605653cc60f8fe6057ea5))
+* temperature not required when fitting with broadened step edge ([`4b83d87`](https://github.com/kmnhan/erlabpy/commit/4b83d8713044e8dfdaf605653cc60f8fe6057ea5))
 
-* fix: fix colorbar conflict with multiple cursors ([`6cb35b6`](https://github.com/kmnhan/erlabpy/commit/6cb35b68b9643dc19d9e197e67554c203e5c4b99))
+* fix colorbar conflict with multiple cursors ([`6cb35b6`](https://github.com/kmnhan/erlabpy/commit/6cb35b68b9643dc19d9e197e67554c203e5c4b99))
 
-* fix: wrong sign in powernorm ([`b4df421`](https://github.com/kmnhan/erlabpy/commit/b4df42102822da0e41991b9c176a24b900220088))
+* wrong sign in powernorm ([`b4df421`](https://github.com/kmnhan/erlabpy/commit/b4df42102822da0e41991b9c176a24b900220088))
 
-* fix: rewrite pyqtgraph colormap normalization ([`e2a807e`](https://github.com/kmnhan/erlabpy/commit/e2a807e7a0c7e556a6d2750cd4052df911b5ec3c))
+* rewrite pyqtgraph colormap normalization ([`e2a807e`](https://github.com/kmnhan/erlabpy/commit/e2a807e7a0c7e556a6d2750cd4052df911b5ec3c))
 
-* fix(itool): fix misc. bugs ([`15c737c`](https://github.com/kmnhan/erlabpy/commit/15c737cd0096a27d5582ab1f084a7ad070b28bcc))
+* **itool** fix misc. bugs ([`15c737c`](https://github.com/kmnhan/erlabpy/commit/15c737cd0096a27d5582ab1f084a7ad070b28bcc))
 
-* fix: retain clipboard after window close ([`e800bc7`](https://github.com/kmnhan/erlabpy/commit/e800bc72fae148e0f9fc4df646566013bf7082b8))
+* retain clipboard after window close ([`e800bc7`](https://github.com/kmnhan/erlabpy/commit/e800bc72fae148e0f9fc4df646566013bf7082b8))
 
-* fix(bz): input reciprocal lattice vectors ([`32df4d7`](https://github.com/kmnhan/erlabpy/commit/32df4d7e673fbcfb886c959450d30c9bf1fa1d27))
+* **bz** input reciprocal lattice vectors ([`32df4d7`](https://github.com/kmnhan/erlabpy/commit/32df4d7e673fbcfb886c959450d30c9bf1fa1d27))
 
-* fix: automatic figure detection ([`f0f2ef9`](https://github.com/kmnhan/erlabpy/commit/f0f2ef9810ec637a46d316b37578bc45307ea881))
+* automatic figure detection ([`f0f2ef9`](https://github.com/kmnhan/erlabpy/commit/f0f2ef9810ec637a46d316b37578bc45307ea881))
 
-* fix(itool): regression: aspect ratio for 2D arrays ([`087ba24`](https://github.com/kmnhan/erlabpy/commit/087ba24cb99b12901ae928cd2b3288c25570c9eb))
+* **itool** regression: aspect ratio for 2D arrays ([`087ba24`](https://github.com/kmnhan/erlabpy/commit/087ba24cb99b12901ae928cd2b3288c25570c9eb))
 
-* fix(itool): better handle drag ([`23cdbf0`](https://github.com/kmnhan/erlabpy/commit/23cdbf039118980c50760a7ebf94b24b48a6b6c8))
+* **itool** better handle drag ([`23cdbf0`](https://github.com/kmnhan/erlabpy/commit/23cdbf039118980c50760a7ebf94b24b48a6b6c8))
 
-* fix: replace bitwise inversion on boolean ([`5569060`](https://github.com/kmnhan/erlabpy/commit/5569060a356aad3d1d3141b5accce61f66e78418))
+* replace bitwise inversion on boolean ([`5569060`](https://github.com/kmnhan/erlabpy/commit/5569060a356aad3d1d3141b5accce61f66e78418))
 
-* fix: works properly with integer coordinates ([`adc0074`](https://github.com/kmnhan/erlabpy/commit/adc00746668456576709b1db9525ea5bb6e5bb11))
+* works properly with integer coordinates ([`adc0074`](https://github.com/kmnhan/erlabpy/commit/adc00746668456576709b1db9525ea5bb6e5bb11))
 
-* fix: update some deprecated syntax ([`839f1a6`](https://github.com/kmnhan/erlabpy/commit/839f1a60132ff03b578224109553491e49a80aae))
+* update some deprecated syntax ([`839f1a6`](https://github.com/kmnhan/erlabpy/commit/839f1a60132ff03b578224109553491e49a80aae))
 
-* fix: patch for PySide6 6.4 ([`6e9d1b9`](https://github.com/kmnhan/erlabpy/commit/6e9d1b9ed5899cb4f639806281da55d987e01f1d))
+* patch for PySide6 6.4 ([`6e9d1b9`](https://github.com/kmnhan/erlabpy/commit/6e9d1b9ed5899cb4f639806281da55d987e01f1d))
 
-* fix: better aspect ratio for 2D arrays ([`b002350`](https://github.com/kmnhan/erlabpy/commit/b002350164c4f9c7cd233f50488937f55dff8e46))
+* better aspect ratio for 2D arrays ([`b002350`](https://github.com/kmnhan/erlabpy/commit/b002350164c4f9c7cd233f50488937f55dff8e46))
 
-* fix: regression as per pyqtgraph/pyqtgraph@cead5cd ([`74c9f81`](https://github.com/kmnhan/erlabpy/commit/74c9f8181033c9f7cfbe8eaa15b64172dc287601))
+* regression as per pyqtgraph/pyqtgraph@cead5cd ([`74c9f81`](https://github.com/kmnhan/erlabpy/commit/74c9f8181033c9f7cfbe8eaa15b64172dc287601))
 
-* fix: stupid rad2deg handling ([`4a6d629`](https://github.com/kmnhan/erlabpy/commit/4a6d629261e6bc0da286b3c687d8fe8af46ee589))
+* stupid rad2deg handling ([`4a6d629`](https://github.com/kmnhan/erlabpy/commit/4a6d629261e6bc0da286b3c687d8fe8af46ee589))
 
-* fix(goldtool): catch varname exceptions ([`aa22dd7`](https://github.com/kmnhan/erlabpy/commit/aa22dd7833e1fd7e3f1a36fa48ccee7c6420dffe))
+* **goldtool** catch varname exceptions ([`aa22dd7`](https://github.com/kmnhan/erlabpy/commit/aa22dd7833e1fd7e3f1a36fa48ccee7c6420dffe))
 
-* fix(itool): wrong signals ([`a0f0036`](https://github.com/kmnhan/erlabpy/commit/a0f00366be305f302a52e84eac5e4fc97d7d9d54))
+* **itool** wrong signals ([`a0f0036`](https://github.com/kmnhan/erlabpy/commit/a0f00366be305f302a52e84eac5e4fc97d7d9d54))
 
-* fix: colorbar aspect specification ([`456f370`](https://github.com/kmnhan/erlabpy/commit/456f370907ca163c30567992da8edbfebcf18caf))
+* colorbar aspect specification ([`456f370`](https://github.com/kmnhan/erlabpy/commit/456f370907ca163c30567992da8edbfebcf18caf))
 
-* fix: docstring and labeling ([`4bbedda`](https://github.com/kmnhan/erlabpy/commit/4bbedda90b83f7be32494cfd63bc9ac7dfb94327))
+* docstring and labeling ([`4bbedda`](https://github.com/kmnhan/erlabpy/commit/4bbedda90b83f7be32494cfd63bc9ac7dfb94327))
 
-* fix: attempts to overwrite read-only object ([`0cf8606`](https://github.com/kmnhan/erlabpy/commit/0cf8606cd69ccdeaae4d84945e181b9e2b07a846))
+* attempts to overwrite read-only object ([`0cf8606`](https://github.com/kmnhan/erlabpy/commit/0cf8606cd69ccdeaae4d84945e181b9e2b07a846))
 
-* fix(plot_array): colorbar extents ([`2fe8a93`](https://github.com/kmnhan/erlabpy/commit/2fe8a930f2cf8fd37d88958231388e4a446b1443))
+* **plot_array** colorbar extents ([`2fe8a93`](https://github.com/kmnhan/erlabpy/commit/2fe8a930f2cf8fd37d88958231388e4a446b1443))
 
-* fix: broken binning ([`f217938`](https://github.com/kmnhan/erlabpy/commit/f217938379ea7d69613fdef462b26ed41d4850cd))
+* broken binning ([`f217938`](https://github.com/kmnhan/erlabpy/commit/f217938379ea7d69613fdef462b26ed41d4850cd))
 
-* fix(itool): isocurve wrong orientation ([`dfd6aac`](https://github.com/kmnhan/erlabpy/commit/dfd6aac29b846e5b187791aa7fe2708dc95abe76))
+* **itool** isocurve wrong orientation ([`dfd6aac`](https://github.com/kmnhan/erlabpy/commit/dfd6aac29b846e5b187791aa7fe2708dc95abe76))
 
-* fix(itool): tab position ([`a70af2b`](https://github.com/kmnhan/erlabpy/commit/a70af2be59c80231be605e49304d226ed5c24f0c))
+* **itool** tab position ([`a70af2b`](https://github.com/kmnhan/erlabpy/commit/a70af2be59c80231be605e49304d226ed5c24f0c))
 
-* fix: fine-tune automatic colormap assignment ([`1d035bb`](https://github.com/kmnhan/erlabpy/commit/1d035bb6ce178f7c13b4c2cd35b20fb69342a627))
+* fine-tune automatic colormap assignment ([`1d035bb`](https://github.com/kmnhan/erlabpy/commit/1d035bb6ce178f7c13b4c2cd35b20fb69342a627))
 
-* fix(itool): smarter mouse detection ([`3032c0c`](https://github.com/kmnhan/erlabpy/commit/3032c0cc15c23a3f345300de0eb57080d31b7604))
+* **itool** smarter mouse detection ([`3032c0c`](https://github.com/kmnhan/erlabpy/commit/3032c0cc15c23a3f345300de0eb57080d31b7604))
 
-* fix: noisetool import ([`c99bfd2`](https://github.com/kmnhan/erlabpy/commit/c99bfd2980127f07fc6b361d9156e5a68be2711c))
+* noisetool import ([`c99bfd2`](https://github.com/kmnhan/erlabpy/commit/c99bfd2980127f07fc6b361d9156e5a68be2711c))
 
-* fix: invalid import ([`5fd9010`](https://github.com/kmnhan/erlabpy/commit/5fd90104cd8e2a2b8158df6acf88dfa7408bc102))
+* invalid import ([`5fd9010`](https://github.com/kmnhan/erlabpy/commit/5fd90104cd8e2a2b8158df6acf88dfa7408bc102))
 
-* fix: flickering cursor when moving ([`439157b`](https://github.com/kmnhan/erlabpy/commit/439157bf3fb3b377ebb17a9f6c7a37b87fafc905))
+* flickering cursor when moving ([`439157b`](https://github.com/kmnhan/erlabpy/commit/439157bf3fb3b377ebb17a9f6c7a37b87fafc905))
 
-* fix(itool): fix transpose ([`0b23f61`](https://github.com/kmnhan/erlabpy/commit/0b23f61dfb7c3dec8a534d5b5c7dae560418376f))
+* **itool** fix transpose ([`0b23f61`](https://github.com/kmnhan/erlabpy/commit/0b23f61dfb7c3dec8a534d5b5c7dae560418376f))
 
-* fix(itool): change wrong 2D layout ([`e04f162`](https://github.com/kmnhan/erlabpy/commit/e04f162ac0f88f1c576942e9eb820044a17ea791))
+* **itool** change wrong 2D layout ([`e04f162`](https://github.com/kmnhan/erlabpy/commit/e04f162ac0f88f1c576942e9eb820044a17ea791))
 
-* fix(itool): revert ([`ca4335a`](https://github.com/kmnhan/erlabpy/commit/ca4335a77ba467d46fa0d68e80927aa6ee8e8a24))
+* **itool** revert ([`ca4335a`](https://github.com/kmnhan/erlabpy/commit/ca4335a77ba467d46fa0d68e80927aa6ee8e8a24))
 
-* fix(itool): adjust blitting ([`0873882`](https://github.com/kmnhan/erlabpy/commit/0873882a7692da94ec05ee659030d0e26be51585))
+* **itool** adjust blitting ([`0873882`](https://github.com/kmnhan/erlabpy/commit/0873882a7692da94ec05ee659030d0e26be51585))
 
-* fix(itool): properly functioning pan &amp; zoom ([`26ce4e8`](https://github.com/kmnhan/erlabpy/commit/26ce4e8efce62eb2ab38f14b097f0121ef6205d4))
+* **itool** properly functioning pan &amp; zoom ([`26ce4e8`](https://github.com/kmnhan/erlabpy/commit/26ce4e8efce62eb2ab38f14b097f0121ef6205d4))
 
-* fix: fix offset not syncing across energy ([`7ec4072`](https://github.com/kmnhan/erlabpy/commit/7ec4072c93e1b41f24e4247afc414244a43badac))
+* fix offset not syncing across energy ([`7ec4072`](https://github.com/kmnhan/erlabpy/commit/7ec4072c93e1b41f24e4247afc414244a43badac))
 
-* fix: fix cursor issue and home resetting limits ([`f3374ab`](https://github.com/kmnhan/erlabpy/commit/f3374abaa8643aef78f33366dfab9a0994b475ce))
+* fix cursor issue and home resetting limits ([`f3374ab`](https://github.com/kmnhan/erlabpy/commit/f3374abaa8643aef78f33366dfab9a0994b475ce))
 
-* fix: simplify cursor customization ([`a5ff97f`](https://github.com/kmnhan/erlabpy/commit/a5ff97f6cffcd2cc3da0a31f44d62ac590c663e3))
+* simplify cursor customization ([`a5ff97f`](https://github.com/kmnhan/erlabpy/commit/a5ff97f6cffcd2cc3da0a31f44d62ac590c663e3))
 
-* fix: make plotting imports backwards compatible ([`82f132b`](https://github.com/kmnhan/erlabpy/commit/82f132b89ffd3c911208ae93fa8d47b1825e7928))
+* make plotting imports backwards compatible ([`82f132b`](https://github.com/kmnhan/erlabpy/commit/82f132b89ffd3c911208ae93fa8d47b1825e7928))
 
-* fix(plotting): fix UnboundLocalError ([`e4f5bca`](https://github.com/kmnhan/erlabpy/commit/e4f5bca381c881d159c9f6a09ebdc86616a4f467))
+* **plotting** fix UnboundLocalError ([`e4f5bca`](https://github.com/kmnhan/erlabpy/commit/e4f5bca381c881d159c9f6a09ebdc86616a4f467))
 
-* fix: fix typo ([`39d160a`](https://github.com/kmnhan/erlabpy/commit/39d160a15a6d8990061de48a08b431a2ff35f699))
+* fix typo ([`39d160a`](https://github.com/kmnhan/erlabpy/commit/39d160a15a6d8990061de48a08b431a2ff35f699))
 
 ### Performance
 
-* perf(interpolate): make some jitted functions always inlined ([`4624b16`](https://github.com/kmnhan/erlabpy/commit/4624b16ec926546876a98864abe3c1d47b6fc221))
+* **interpolate** make some jitted functions always inlined ([`4624b16`](https://github.com/kmnhan/erlabpy/commit/4624b16ec926546876a98864abe3c1d47b6fc221))
 
-* perf(itool): fps optimization, add proper support for nonuniform dimensions ([`6df84db`](https://github.com/kmnhan/erlabpy/commit/6df84db7156de88b2ee8d100a2ce0c45f8b2135a))
+* **itool** fps optimization, add proper support for nonuniform dimensions ([`6df84db`](https://github.com/kmnhan/erlabpy/commit/6df84db7156de88b2ee8d100a2ce0c45f8b2135a))
 
-* perf: cleanup, reduce import time ([`dbfcce3`](https://github.com/kmnhan/erlabpy/commit/dbfcce38f9b874b8532666ff7479dbc789fef657))
+* cleanup, reduce import time ([`dbfcce3`](https://github.com/kmnhan/erlabpy/commit/dbfcce38f9b874b8532666ff7479dbc789fef657))
 
-* perf(itool): add cached properties ([`0124093`](https://github.com/kmnhan/erlabpy/commit/0124093a25ba47e5bc304125fcfd62f6768beb13))
+* **itool** add cached properties ([`0124093`](https://github.com/kmnhan/erlabpy/commit/0124093a25ba47e5bc304125fcfd62f6768beb13))
 
-* perf: limit fps with SignalProxy ([`f7ce099`](https://github.com/kmnhan/erlabpy/commit/f7ce099f87e97adeb27a8e4f2d760b6ddd4f4d22))
+* limit fps with SignalProxy ([`f7ce099`](https://github.com/kmnhan/erlabpy/commit/f7ce099f87e97adeb27a8e4f2d760b6ddd4f4d22))
 
-* perf: get coords efficiently ([`5582afc`](https://github.com/kmnhan/erlabpy/commit/5582afc9e86e8306e6499da52b2f2c06604b029b))
+* get coords efficiently ([`5582afc`](https://github.com/kmnhan/erlabpy/commit/5582afc9e86e8306e6499da52b2f2c06604b029b))
 
-* perf: better min/max performance, fixes #4 ([`3c4aa13`](https://github.com/kmnhan/erlabpy/commit/3c4aa1369fbbf10fa5a2597dc958bb559e4bb26a))
+* better min/max performance, fixes #4 ([`3c4aa13`](https://github.com/kmnhan/erlabpy/commit/3c4aa1369fbbf10fa5a2597dc958bb559e4bb26a))
 
-* perf(slicer): contiguity optimizations ([`6f2b543`](https://github.com/kmnhan/erlabpy/commit/6f2b543a11d89d744961e1f1716ad542a9bab163))
+* **slicer** contiguity optimizations ([`6f2b543`](https://github.com/kmnhan/erlabpy/commit/6f2b543a11d89d744961e1f1716ad542a9bab163))
 
-* perf(itool): update only relevant axes ([`c561650`](https://github.com/kmnhan/erlabpy/commit/c5616502767e8f14425ba07bed4660355eba1203))
+* **itool** update only relevant axes ([`c561650`](https://github.com/kmnhan/erlabpy/commit/c5616502767e8f14425ba07bed4660355eba1203))
 
 ### Refactor
 
-* refactor: apply linter suggestions ([`edfc91a`](https://github.com/kmnhan/erlabpy/commit/edfc91a6712620588106471ae03975a76976f634))
+* apply linter suggestions ([`edfc91a`](https://github.com/kmnhan/erlabpy/commit/edfc91a6712620588106471ae03975a76976f634))
 
-* refactor: apply linter suggestions ([`231f794`](https://github.com/kmnhan/erlabpy/commit/231f794a3aaf6575528df63b70a4478cb9769fe8))
+* apply linter suggestions ([`231f794`](https://github.com/kmnhan/erlabpy/commit/231f794a3aaf6575528df63b70a4478cb9769fe8))
 
-* refactor: apply some linter suggestions ([`4e1f66c`](https://github.com/kmnhan/erlabpy/commit/4e1f66c6b19eb2e3674511e19309c9127d610369))
+* apply some linter suggestions ([`4e1f66c`](https://github.com/kmnhan/erlabpy/commit/4e1f66c6b19eb2e3674511e19309c9127d610369))
 
-* refactor(goldtool): ui changes ([`464d05e`](https://github.com/kmnhan/erlabpy/commit/464d05ee270cf601c322536b3dafd3c7bf0e9f7f))
+* **goldtool** ui changes ([`464d05e`](https://github.com/kmnhan/erlabpy/commit/464d05ee270cf601c322536b3dafd3c7bf0e9f7f))
 
-* refactor: rename variable ([`32a901e`](https://github.com/kmnhan/erlabpy/commit/32a901e0de1b7d0c5fb6858a275b8bf3cb69e801))
+* rename variable ([`32a901e`](https://github.com/kmnhan/erlabpy/commit/32a901e0de1b7d0c5fb6858a275b8bf3cb69e801))
 
-* refactor: cleanup namespace ([`4779e46`](https://github.com/kmnhan/erlabpy/commit/4779e46920cf88a49f211d1d7f856f61e6c84c2a))
+* cleanup namespace ([`4779e46`](https://github.com/kmnhan/erlabpy/commit/4779e46920cf88a49f211d1d7f856f61e6c84c2a))
 
-* refactor(io): minor changes to summary format ([`d26a8f7`](https://github.com/kmnhan/erlabpy/commit/d26a8f78f4d86f7b0654a0949e644d2f96652b50))
+* **io** minor changes to summary format ([`d26a8f7`](https://github.com/kmnhan/erlabpy/commit/d26a8f78f4d86f7b0654a0949e644d2f96652b50))
 
-* refactor: move functions  to submodule ([`824a2fb`](https://github.com/kmnhan/erlabpy/commit/824a2fb4847d5f29dc51f50517a51aae3709d3df))
+* move functions  to submodule ([`824a2fb`](https://github.com/kmnhan/erlabpy/commit/824a2fb4847d5f29dc51f50517a51aae3709d3df))
 
-* refactor: fit functions submodule ([`2bc555c`](https://github.com/kmnhan/erlabpy/commit/2bc555cfb050d28523f805b75053dcf836759a7f))
+* fit functions submodule ([`2bc555c`](https://github.com/kmnhan/erlabpy/commit/2bc555cfb050d28523f805b75053dcf836759a7f))
 
-* refactor(io.dataloader): fix _repr_html_ to return valid html table ([`73adb0f`](https://github.com/kmnhan/erlabpy/commit/73adb0ffffc618d28903a4c5814923dac5502186))
+* **io.dataloader** fix _repr_html_ to return valid html table ([`73adb0f`](https://github.com/kmnhan/erlabpy/commit/73adb0ffffc618d28903a4c5814923dac5502186))
 
-* refactor(io.dataloader): make reverse_mapping a staticmethod ([`983c02b`](https://github.com/kmnhan/erlabpy/commit/983c02bda02c97a7eb179c35f98d0a89c0814cd9))
+* **io.dataloader** make reverse_mapping a staticmethod ([`983c02b`](https://github.com/kmnhan/erlabpy/commit/983c02bda02c97a7eb179c35f98d0a89c0814cd9))
 
-* refactor(io): change dict format ([`a13b064`](https://github.com/kmnhan/erlabpy/commit/a13b06465f53c78b9edea538e9825d83f66b86f0))
+* **io** change dict format ([`a13b064`](https://github.com/kmnhan/erlabpy/commit/a13b06465f53c78b9edea538e9825d83f66b86f0))
 
-* refactor: add type annotation ([`7e08658`](https://github.com/kmnhan/erlabpy/commit/7e08658093fe24a383366f722f044029f097cb69))
+* add type annotation ([`7e08658`](https://github.com/kmnhan/erlabpy/commit/7e08658093fe24a383366f722f044029f097cb69))
 
-* refactor: use match-case for enum matching ([`cc9e112`](https://github.com/kmnhan/erlabpy/commit/cc9e1126f7571df3e68e568375773a3a4dce63b5))
+* use match-case for enum matching ([`cc9e112`](https://github.com/kmnhan/erlabpy/commit/cc9e1126f7571df3e68e568375773a3a4dce63b5))
 
-* refactor: change package directory structure; BREAKING CHANGE ([`5385ec7`](https://github.com/kmnhan/erlabpy/commit/5385ec70b23775ddd19b02459cbb0d0630143454))
+* change package directory structure; BREAKING CHANGE ([`5385ec7`](https://github.com/kmnhan/erlabpy/commit/5385ec70b23775ddd19b02459cbb0d0630143454))
 
-* refactor: format with black ([`1655eec`](https://github.com/kmnhan/erlabpy/commit/1655eec321bd12acc37681e1d55e21155ec34252))
+* format with black ([`1655eec`](https://github.com/kmnhan/erlabpy/commit/1655eec321bd12acc37681e1d55e21155ec34252))
 
-* refactor: remove code trying to infer spectrum from dataset
+* remove code trying to infer spectrum from dataset ([`3fa6b1b`](https://github.com/kmnhan/erlabpy/commit/3fa6b1b25dc70add644e9719488ae55df314238c))
 
-From now on all data should be strictly a xr.DataArray ([`3fa6b1b`](https://github.com/kmnhan/erlabpy/commit/3fa6b1b25dc70add644e9719488ae55df314238c))
+  From now on all data should be strictly a xr.DataArray
 
-* refactor: deprecate old ktool, replace ([`dbd972f`](https://github.com/kmnhan/erlabpy/commit/dbd972f0e56197c1796695921b6cc021b3f4d190))
+* deprecate old ktool, replace ([`dbd972f`](https://github.com/kmnhan/erlabpy/commit/dbd972f0e56197c1796695921b6cc021b3f4d190))
 
-* refactor(gold): add type annotation ([`06c39a7`](https://github.com/kmnhan/erlabpy/commit/06c39a790109e23a81e88c885a1fa0ee1f615e41))
+* **gold** add type annotation ([`06c39a7`](https://github.com/kmnhan/erlabpy/commit/06c39a790109e23a81e88c885a1fa0ee1f615e41))
 
-* refactor: Update requirements.txt so that igor2 is not editable ([`0e20bc4`](https://github.com/kmnhan/erlabpy/commit/0e20bc48d458a363b4c2e2b829a59ac6e1aba6cf))
+* Update requirements.txt so that igor2 is not editable ([`0e20bc4`](https://github.com/kmnhan/erlabpy/commit/0e20bc48d458a363b4c2e2b829a59ac6e1aba6cf))
 
-* refactor: temporarily disable annotate_cuts_erlab ([`08e4b52`](https://github.com/kmnhan/erlabpy/commit/08e4b527316b94b0a1d2912b67d1b67ea4571755))
+* temporarily disable annotate_cuts_erlab ([`08e4b52`](https://github.com/kmnhan/erlabpy/commit/08e4b527316b94b0a1d2912b67d1b67ea4571755))
 
-* refactor(itool): modify test code ([`8934fba`](https://github.com/kmnhan/erlabpy/commit/8934fba1b20cf182455d2a70e24ff835d6ca96be))
+* **itool** modify test code ([`8934fba`](https://github.com/kmnhan/erlabpy/commit/8934fba1b20cf182455d2a70e24ff835d6ca96be))
 
-* refactor(exampledata): tweak defaults ([`73eb495`](https://github.com/kmnhan/erlabpy/commit/73eb4955ff3ed7f568136efce5efaf9ab929dfba))
+* **exampledata** tweak defaults ([`73eb495`](https://github.com/kmnhan/erlabpy/commit/73eb4955ff3ed7f568136efce5efaf9ab929dfba))
 
-* refactor: cleanup ([`88b418f`](https://github.com/kmnhan/erlabpy/commit/88b418f61491917e275ec7b5cc544c157617429d))
+* cleanup ([`88b418f`](https://github.com/kmnhan/erlabpy/commit/88b418f61491917e275ec7b5cc544c157617429d))
 
-* refactor: try garbage collection, failed ([`ac75267`](https://github.com/kmnhan/erlabpy/commit/ac75267921884299970c5d78b1633835700dce6e))
+* try garbage collection, failed ([`ac75267`](https://github.com/kmnhan/erlabpy/commit/ac75267921884299970c5d78b1633835700dce6e))
 
-* refactor: typo ([`f1df9ea`](https://github.com/kmnhan/erlabpy/commit/f1df9ea0a4e128013d21e2f2b5e9a64f9acf57a3))
+* typo ([`f1df9ea`](https://github.com/kmnhan/erlabpy/commit/f1df9ea0a4e128013d21e2f2b5e9a64f9acf57a3))
 
-* refactor: reorder functions ([`ee6886f`](https://github.com/kmnhan/erlabpy/commit/ee6886fa7810c3bac26e05b1407ceebc1563ad54))
+* reorder functions ([`ee6886f`](https://github.com/kmnhan/erlabpy/commit/ee6886fa7810c3bac26e05b1407ceebc1563ad54))
 
-* refactor: organize imports ([`70b2b9b`](https://github.com/kmnhan/erlabpy/commit/70b2b9bed7e395a824ee3e1b240937b570e670ec))
+* organize imports ([`70b2b9b`](https://github.com/kmnhan/erlabpy/commit/70b2b9bed7e395a824ee3e1b240937b570e670ec))
 
-* refactor: cleanup ([`8b01e73`](https://github.com/kmnhan/erlabpy/commit/8b01e7393b7d7a6ae23b85e6f784a7f760cdd74a))
+* cleanup ([`8b01e73`](https://github.com/kmnhan/erlabpy/commit/8b01e7393b7d7a6ae23b85e6f784a7f760cdd74a))
 
-* refactor: relocate color related classes ([`b322fb8`](https://github.com/kmnhan/erlabpy/commit/b322fb8ced0b41a1ec8e7dbaf9ac50c8f7aa853c))
+* relocate color related classes ([`b322fb8`](https://github.com/kmnhan/erlabpy/commit/b322fb8ced0b41a1ec8e7dbaf9ac50c8f7aa853c))
 
-* refactor(io): cleanup imports ([`125f672`](https://github.com/kmnhan/erlabpy/commit/125f672edd3b6f94943c2a3d221e626f9a58c820))
+* **io** cleanup imports ([`125f672`](https://github.com/kmnhan/erlabpy/commit/125f672edd3b6f94943c2a3d221e626f9a58c820))
 
-* refactor: add submodules to analysis initialization ([`30ab7d0`](https://github.com/kmnhan/erlabpy/commit/30ab7d0f71a6c09633e54345c7317215934c1ca6))
+* add submodules to analysis initialization ([`30ab7d0`](https://github.com/kmnhan/erlabpy/commit/30ab7d0f71a6c09633e54345c7317215934c1ca6))
 
-* refactor: rename igor procedure file ([`92d495c`](https://github.com/kmnhan/erlabpy/commit/92d495cb114a921a8ca9d1fde81a4e6400d53089))
+* rename igor procedure file ([`92d495c`](https://github.com/kmnhan/erlabpy/commit/92d495cb114a921a8ca9d1fde81a4e6400d53089))
 
-* refactor: cleanup ([`025b39b`](https://github.com/kmnhan/erlabpy/commit/025b39bb557ab364e6c2f5ff14ddb2956ba52467))
+* cleanup ([`025b39b`](https://github.com/kmnhan/erlabpy/commit/025b39bb557ab364e6c2f5ff14ddb2956ba52467))
 
-* refactor: move colormap controls up ([`13a44fe`](https://github.com/kmnhan/erlabpy/commit/13a44febb156fe657ed39636323c124650010501))
+* move colormap controls up ([`13a44fe`](https://github.com/kmnhan/erlabpy/commit/13a44febb156fe657ed39636323c124650010501))
 
-* refactor: follow pep8 dunder names ([`f954b7b`](https://github.com/kmnhan/erlabpy/commit/f954b7ba76b877a7376b45a9a91871e9b8ea4d25))
+* follow pep8 dunder names ([`f954b7b`](https://github.com/kmnhan/erlabpy/commit/f954b7ba76b877a7376b45a9a91871e9b8ea4d25))
 
-* refactor: replace deprecated syntax ([`6d48a08`](https://github.com/kmnhan/erlabpy/commit/6d48a088f632c0a6d467067463e706c410ad8978))
+* replace deprecated syntax ([`6d48a08`](https://github.com/kmnhan/erlabpy/commit/6d48a088f632c0a6d467067463e706c410ad8978))
 
-* refactor: cleanup ([`5b24106`](https://github.com/kmnhan/erlabpy/commit/5b241068cbd60de73da420149fbd4ba2f09a1ac9))
+* cleanup ([`5b24106`](https://github.com/kmnhan/erlabpy/commit/5b241068cbd60de73da420149fbd4ba2f09a1ac9))
 
-* refactor: cleanup and add some type annotation ([`daabfb8`](https://github.com/kmnhan/erlabpy/commit/daabfb87b07fa71a618b127c2cd6a51bbc0e3e18))
+* cleanup and add some type annotation ([`daabfb8`](https://github.com/kmnhan/erlabpy/commit/daabfb87b07fa71a618b127c2cd6a51bbc0e3e18))
 
-* refactor: move DictMenuBar to utilities ([`2b3fcb1`](https://github.com/kmnhan/erlabpy/commit/2b3fcb1776115cfee987db4e74c4d34a5d679bcf))
+* move DictMenuBar to utilities ([`2b3fcb1`](https://github.com/kmnhan/erlabpy/commit/2b3fcb1776115cfee987db4e74c4d34a5d679bcf))
 
-* refactor: change gold fitting syntax ([`e6043d6`](https://github.com/kmnhan/erlabpy/commit/e6043d6ae3aa0bc3b90db2d0378c9bd3c7a7c948))
+* change gold fitting syntax ([`e6043d6`](https://github.com/kmnhan/erlabpy/commit/e6043d6ae3aa0bc3b90db2d0378c9bd3c7a7c948))
 
-* refactor: update clean_labels with matplotlib API ([`13013dd`](https://github.com/kmnhan/erlabpy/commit/13013dd7ebb16e03b1609e4e44315b22139e8f28))
+* update clean_labels with matplotlib API ([`13013dd`](https://github.com/kmnhan/erlabpy/commit/13013dd7ebb16e03b1609e4e44315b22139e8f28))
 
-* refactor: move some functions ([`866eca5`](https://github.com/kmnhan/erlabpy/commit/866eca5c5a5b0ccf38383aead2b5871903c5c50a))
+* move some functions ([`866eca5`](https://github.com/kmnhan/erlabpy/commit/866eca5c5a5b0ccf38383aead2b5871903c5c50a))
 
-* refactor: follow pep8 dunder names ([`b043701`](https://github.com/kmnhan/erlabpy/commit/b043701e428c7e1c461f64f57667d8b25642a5ce))
+* follow pep8 dunder names ([`b043701`](https://github.com/kmnhan/erlabpy/commit/b043701e428c7e1c461f64f57667d8b25642a5ce))
 
-* refactor: imagetool is now a package ([`1a39b82`](https://github.com/kmnhan/erlabpy/commit/1a39b8283582cccacd448addb3566f6f1e882744))
+* imagetool is now a package ([`1a39b82`](https://github.com/kmnhan/erlabpy/commit/1a39b8283582cccacd448addb3566f6f1e882744))
 
-* refactor: follow pep8 dunder names ([`dbdc0f6`](https://github.com/kmnhan/erlabpy/commit/dbdc0f62cb048ce5c2f248a21e112476d5ebb3df))
+* follow pep8 dunder names ([`dbdc0f6`](https://github.com/kmnhan/erlabpy/commit/dbdc0f62cb048ce5c2f248a21e112476d5ebb3df))
 
-* refactor: cleanup ([`aace486`](https://github.com/kmnhan/erlabpy/commit/aace486d8652e07ab9007f89a49a29cca3d4e1af))
+* cleanup ([`aace486`](https://github.com/kmnhan/erlabpy/commit/aace486d8652e07ab9007f89a49a29cca3d4e1af))
 
-* refactor: cleanup annotations ([`12e590c`](https://github.com/kmnhan/erlabpy/commit/12e590c2a771d089e29aff02492851448640b605))
+* cleanup annotations ([`12e590c`](https://github.com/kmnhan/erlabpy/commit/12e590c2a771d089e29aff02492851448640b605))
 
-* refactor: transition to new polynomial api ([`5461c34`](https://github.com/kmnhan/erlabpy/commit/5461c342f7a84d1ba98f924c74be6ecde16cf6e4))
+* transition to new polynomial api ([`5461c34`](https://github.com/kmnhan/erlabpy/commit/5461c342f7a84d1ba98f924c74be6ecde16cf6e4))
 
-* refactor: cleanup syntax ([`310c2ba`](https://github.com/kmnhan/erlabpy/commit/310c2babf15d7a22900806cac308643bb22f8bce))
+* cleanup syntax ([`310c2ba`](https://github.com/kmnhan/erlabpy/commit/310c2babf15d7a22900806cac308643bb22f8bce))
 
-* refactor(itool): changes to layout ([`7a684e4`](https://github.com/kmnhan/erlabpy/commit/7a684e400772036dde7af4f8a4747c8db208eb0f))
+* **itool** changes to layout ([`7a684e4`](https://github.com/kmnhan/erlabpy/commit/7a684e400772036dde7af4f8a4747c8db208eb0f))
 
-* refactor: remove dependency on darkdetect ([`81fa963`](https://github.com/kmnhan/erlabpy/commit/81fa963a91fddd1eb2b7f316fcec04eb27716d13))
+* remove dependency on darkdetect ([`81fa963`](https://github.com/kmnhan/erlabpy/commit/81fa963a91fddd1eb2b7f316fcec04eb27716d13))
 
-* refactor: format code ([`adf6cb3`](https://github.com/kmnhan/erlabpy/commit/adf6cb3cd48e494d708c79906347e3c54fcd3e20))
+* format code ([`adf6cb3`](https://github.com/kmnhan/erlabpy/commit/adf6cb3cd48e494d708c79906347e3c54fcd3e20))
 
-* refactor: remove io module, add as package ([`5d1280a`](https://github.com/kmnhan/erlabpy/commit/5d1280a3c7893bb86a42fdf2a71b6825c5db6986))
+* remove io module, add as package ([`5d1280a`](https://github.com/kmnhan/erlabpy/commit/5d1280a3c7893bb86a42fdf2a71b6825c5db6986))
 
-* refactor: try to merge commit error ([`2c61d45`](https://github.com/kmnhan/erlabpy/commit/2c61d4575bfcafe22b63527a5dc3f318147cb8c4))
+* try to merge commit error ([`2c61d45`](https://github.com/kmnhan/erlabpy/commit/2c61d4575bfcafe22b63527a5dc3f318147cb8c4))
 
-* refactor: menubar cleanup ([`f147f11`](https://github.com/kmnhan/erlabpy/commit/f147f114364bd9fab0ba456a24113d58dc549652))
+* menubar cleanup ([`f147f11`](https://github.com/kmnhan/erlabpy/commit/f147f114364bd9fab0ba456a24113d58dc549652))
 
-* refactor: organize code ([`93ebd5b`](https://github.com/kmnhan/erlabpy/commit/93ebd5b59307b8524452a3c155a5851988070923))
+* organize code ([`93ebd5b`](https://github.com/kmnhan/erlabpy/commit/93ebd5b59307b8524452a3c155a5851988070923))
 
-* refactor: rename constants ([`ebaeaa1`](https://github.com/kmnhan/erlabpy/commit/ebaeaa11a0c718266512261f640441a06e2703e1))
+* rename constants ([`ebaeaa1`](https://github.com/kmnhan/erlabpy/commit/ebaeaa11a0c718266512261f640441a06e2703e1))
 
-* refactor: cleanup ([`f29bdf3`](https://github.com/kmnhan/erlabpy/commit/f29bdf31e035fc8891f95b8479bf2c05f39ffc03))
+* cleanup ([`f29bdf3`](https://github.com/kmnhan/erlabpy/commit/f29bdf31e035fc8891f95b8479bf2c05f39ffc03))
 
-* refactor: syntax cleanup ([`2678967`](https://github.com/kmnhan/erlabpy/commit/26789677f4fb489af39edcab5b0f73714c1e52b4))
+* syntax cleanup ([`2678967`](https://github.com/kmnhan/erlabpy/commit/26789677f4fb489af39edcab5b0f73714c1e52b4))
 
-* refactor: interactive is no longer a submodule of plotting ([`3da646c`](https://github.com/kmnhan/erlabpy/commit/3da646cf4f13c717cf99ec9cc2e3e449e4d4bfdb))
+* interactive is no longer a submodule of plotting ([`3da646c`](https://github.com/kmnhan/erlabpy/commit/3da646cf4f13c717cf99ec9cc2e3e449e4d4bfdb))
 
-* refactor: remove relative imports ([`96a2095`](https://github.com/kmnhan/erlabpy/commit/96a209572843c35dff50dc383c00bf83c48eb263))
+* remove relative imports ([`96a2095`](https://github.com/kmnhan/erlabpy/commit/96a209572843c35dff50dc383c00bf83c48eb263))
 
-* refactor: lint with flake8 ([`ca34ea1`](https://github.com/kmnhan/erlabpy/commit/ca34ea1b82fccf4ed73b5fdf4f8dfedca303cfa2))
+* lint with flake8 ([`ca34ea1`](https://github.com/kmnhan/erlabpy/commit/ca34ea1b82fccf4ed73b5fdf4f8dfedca303cfa2))
 
-* refactor: remove sandbox notebook ([`504cbc9`](https://github.com/kmnhan/erlabpy/commit/504cbc9f58eb43fb142541c1a5c6b97b4ced3c64))
+* remove sandbox notebook ([`504cbc9`](https://github.com/kmnhan/erlabpy/commit/504cbc9f58eb43fb142541c1a5c6b97b4ced3c64))
 
-* refactor: minor changes ([`692fbc0`](https://github.com/kmnhan/erlabpy/commit/692fbc0d95657c2fcd0646e5a8a65aa0161d2aca))
+* minor changes ([`692fbc0`](https://github.com/kmnhan/erlabpy/commit/692fbc0d95657c2fcd0646e5a8a65aa0161d2aca))
 
-* refactor: expose property label ([`9e2dafd`](https://github.com/kmnhan/erlabpy/commit/9e2dafd4948437b3e3b308a7a53a2a331b551941))
+* expose property label ([`9e2dafd`](https://github.com/kmnhan/erlabpy/commit/9e2dafd4948437b3e3b308a7a53a2a331b551941))
 
-* refactor: syntax cleanup ([`37166af`](https://github.com/kmnhan/erlabpy/commit/37166af6b1cbb7bdebccdd8a90e4953685859ab0))
+* syntax cleanup ([`37166af`](https://github.com/kmnhan/erlabpy/commit/37166af6b1cbb7bdebccdd8a90e4953685859ab0))
 
-* refactor: syntax cleanup ([`19884df`](https://github.com/kmnhan/erlabpy/commit/19884df9909684f2352e6583cad0abb523e958de))
+* syntax cleanup ([`19884df`](https://github.com/kmnhan/erlabpy/commit/19884df9909684f2352e6583cad0abb523e958de))
 
-* refactor: syntax cleanup ([`59e2921`](https://github.com/kmnhan/erlabpy/commit/59e2921c5c7d897f3cfdb17417d46127bb95af60))
+* syntax cleanup ([`59e2921`](https://github.com/kmnhan/erlabpy/commit/59e2921c5c7d897f3cfdb17417d46127bb95af60))
 
-* refactor: change clipboard handler ([`d687499`](https://github.com/kmnhan/erlabpy/commit/d687499b43a027ea97a05243d57c88ae6f756398))
+* change clipboard handler ([`d687499`](https://github.com/kmnhan/erlabpy/commit/d687499b43a027ea97a05243d57c88ae6f756398))
 
-* refactor: some changes regarding colorbar, may be reverted ([`bc913c0`](https://github.com/kmnhan/erlabpy/commit/bc913c07dcd9bbe36f6a28112f32d5d8ff077152))
+* some changes regarding colorbar, may be reverted ([`bc913c0`](https://github.com/kmnhan/erlabpy/commit/bc913c07dcd9bbe36f6a28112f32d5d8ff077152))
 
-* refactor: deprecate old imagetool ([`26e20ec`](https://github.com/kmnhan/erlabpy/commit/26e20ec474776274b07d4221976c5d5cee3d2b8b))
+* deprecate old imagetool ([`26e20ec`](https://github.com/kmnhan/erlabpy/commit/26e20ec474776274b07d4221976c5d5cee3d2b8b))
 
-* refactor: cleanup enums ([`ec42673`](https://github.com/kmnhan/erlabpy/commit/ec4267373c9f3caf36c2ef4a5f7870e4fa205bdf))
+* cleanup enums ([`ec42673`](https://github.com/kmnhan/erlabpy/commit/ec4267373c9f3caf36c2ef4a5f7870e4fa205bdf))
 
-* refactor: cleanup ([`9eef9f9`](https://github.com/kmnhan/erlabpy/commit/9eef9f94d54badb74578fac96dd8854fcfc1f393))
+* cleanup ([`9eef9f9`](https://github.com/kmnhan/erlabpy/commit/9eef9f94d54badb74578fac96dd8854fcfc1f393))
 
-* refactor: cleanup axis labels and signals ([`3aec658`](https://github.com/kmnhan/erlabpy/commit/3aec658a2c93a3244f8053b28f27b8446fbef61e))
+* cleanup axis labels and signals ([`3aec658`](https://github.com/kmnhan/erlabpy/commit/3aec658a2c93a3244f8053b28f27b8446fbef61e))
 
-* refactor: add typing ([`4951388`](https://github.com/kmnhan/erlabpy/commit/4951388b93ec37fffaf04e44ad02ee67b6f92d6d))
+* add typing ([`4951388`](https://github.com/kmnhan/erlabpy/commit/4951388b93ec37fffaf04e44ad02ee67b6f92d6d))
 
-* refactor: change class name ([`a7d51e5`](https://github.com/kmnhan/erlabpy/commit/a7d51e5c7b5eead59f3a7a0ecd667adae6d90c3a))
+* change class name ([`a7d51e5`](https://github.com/kmnhan/erlabpy/commit/a7d51e5c7b5eead59f3a7a0ecd667adae6d90c3a))
 
-* refactor: minor improvement and cleanup ([`b2886e4`](https://github.com/kmnhan/erlabpy/commit/b2886e447737c954d01eac2a016ef68ecbfc97b6))
+* minor improvement and cleanup ([`b2886e4`](https://github.com/kmnhan/erlabpy/commit/b2886e447737c954d01eac2a016ef68ecbfc97b6))
 
-* refactor: move spinbox to utilities ([`906a0f7`](https://github.com/kmnhan/erlabpy/commit/906a0f7ed919f7f800007633f27d5be0f1f33a2a))
+* move spinbox to utilities ([`906a0f7`](https://github.com/kmnhan/erlabpy/commit/906a0f7ed919f7f800007633f27d5be0f1f33a2a))
 
-* refactor: remove dependency on pyqtgraph dock ([`35b5c3f`](https://github.com/kmnhan/erlabpy/commit/35b5c3f15e7ad2524c239e270dbbecfde5287f78))
+* remove dependency on pyqtgraph dock ([`35b5c3f`](https://github.com/kmnhan/erlabpy/commit/35b5c3f15e7ad2524c239e270dbbecfde5287f78))
 
-* refactor: preparation and cleanup for leaving pyqtgraph dock ([`5721243`](https://github.com/kmnhan/erlabpy/commit/572124321b63c805a94aefb371653918cc174b9a))
+* preparation and cleanup for leaving pyqtgraph dock ([`5721243`](https://github.com/kmnhan/erlabpy/commit/572124321b63c805a94aefb371653918cc174b9a))
 
-* refactor: cleanup ([`1ac0de1`](https://github.com/kmnhan/erlabpy/commit/1ac0de10ddd215d208eb4ca7038e35d35abd826a))
+* cleanup ([`1ac0de1`](https://github.com/kmnhan/erlabpy/commit/1ac0de10ddd215d208eb4ca7038e35d35abd826a))
 
-* refactor: remove font refresh macro
-Just delete cache... ([`3780f23`](https://github.com/kmnhan/erlabpy/commit/3780f23b4b29b271bc4a640e5c187e176f3813b8))
+* remove font refresh macro ([`3780f23`](https://github.com/kmnhan/erlabpy/commit/3780f23b4b29b271bc4a640e5c187e176f3813b8))
 
-* refactor: restructure plotting module ([`7259ab3`](https://github.com/kmnhan/erlabpy/commit/7259ab3d34ad289225f2972dacdfd6aa8a827007))
+* restructure plotting module ([`7259ab3`](https://github.com/kmnhan/erlabpy/commit/7259ab3d34ad289225f2972dacdfd6aa8a827007))
 
-* refactor: split interactive colors module
-the whole package will need a complete restructuring. ([`a06439c`](https://github.com/kmnhan/erlabpy/commit/a06439cfdb044d379df25fc6643250662dcc81c4))
+* split interactive colors module ([`a06439c`](https://github.com/kmnhan/erlabpy/commit/a06439cfdb044d379df25fc6643250662dcc81c4))
 
-* refactor: change to updated colorbar ([`cdd7a8e`](https://github.com/kmnhan/erlabpy/commit/cdd7a8ed04b1c16a3dfd293668604d00e9d3926f))
+* change to updated colorbar ([`cdd7a8e`](https://github.com/kmnhan/erlabpy/commit/cdd7a8ed04b1c16a3dfd293668604d00e9d3926f))
 
-* refactor: prevent namespace collision ([`f3599b2`](https://github.com/kmnhan/erlabpy/commit/f3599b2d465f4c56db38046f8e9127fe519c78dd))
+* prevent namespace collision ([`f3599b2`](https://github.com/kmnhan/erlabpy/commit/f3599b2d465f4c56db38046f8e9127fe519c78dd))
 
-* refactor: clean up comments and format with black ([`90d67b9`](https://github.com/kmnhan/erlabpy/commit/90d67b96448c1786a1fc7dabd5215ab7b6d0cfcb))
+* clean up comments and format with black ([`90d67b9`](https://github.com/kmnhan/erlabpy/commit/90d67b96448c1786a1fc7dabd5215ab7b6d0cfcb))
 
-* refactor: format with black ([`7f79731`](https://github.com/kmnhan/erlabpy/commit/7f7973120c674d1d34f574aa2fedc8ac240bc402))
+* format with black ([`7f79731`](https://github.com/kmnhan/erlabpy/commit/7f7973120c674d1d34f574aa2fedc8ac240bc402))
 
-* refactor: remove deprecated ([`a655778`](https://github.com/kmnhan/erlabpy/commit/a655778161208a9c2f605a27343afe82792c4218))
+* remove deprecated ([`a655778`](https://github.com/kmnhan/erlabpy/commit/a655778161208a9c2f605a27343afe82792c4218))
 
-* refactor: format with black ([`88548cb`](https://github.com/kmnhan/erlabpy/commit/88548cbeda20da21ffd02c284a4086e0e50d3bbe))
+* format with black ([`88548cb`](https://github.com/kmnhan/erlabpy/commit/88548cbeda20da21ffd02c284a4086e0e50d3bbe))
 
-* refactor: format with black ([`306e530`](https://github.com/kmnhan/erlabpy/commit/306e5304c34b3e7c648fe2ea030259fa7a892a42))
+* format with black ([`306e530`](https://github.com/kmnhan/erlabpy/commit/306e5304c34b3e7c648fe2ea030259fa7a892a42))
 
-* refactor: reduce pyarpes dependency ([`14e85fb`](https://github.com/kmnhan/erlabpy/commit/14e85fbcfa7d95df674381f8882db80f39e7bda3))
+* reduce pyarpes dependency ([`14e85fb`](https://github.com/kmnhan/erlabpy/commit/14e85fbcfa7d95df674381f8882db80f39e7bda3))
 
-* refactor: format with black ([`7696b66`](https://github.com/kmnhan/erlabpy/commit/7696b66c6ef93a04c353e8e199c096c2458794ff))
+* format with black ([`7696b66`](https://github.com/kmnhan/erlabpy/commit/7696b66c6ef93a04c353e8e199c096c2458794ff))
 
-* refactor: format with black ([`f6fc29c`](https://github.com/kmnhan/erlabpy/commit/f6fc29ce22a541d9143397ffb902c34d752cdad3))
+* format with black ([`f6fc29c`](https://github.com/kmnhan/erlabpy/commit/f6fc29ce22a541d9143397ffb902c34d752cdad3))
 
-* refactor(itool): cleanup hide buttons ([`2649fe9`](https://github.com/kmnhan/erlabpy/commit/2649fe9ae12893e719a456f0cf22b7eee097df0f))
+* **itool** cleanup hide buttons ([`2649fe9`](https://github.com/kmnhan/erlabpy/commit/2649fe9ae12893e719a456f0cf22b7eee097df0f))
 
-* refactor: format code ([`c69b9cc`](https://github.com/kmnhan/erlabpy/commit/c69b9ccca3ee911b5b07bd6393a43444ba771f33))
+* format code ([`c69b9cc`](https://github.com/kmnhan/erlabpy/commit/c69b9ccca3ee911b5b07bd6393a43444ba771f33))
 
-* refactor: trivial changes ([`6d5df90`](https://github.com/kmnhan/erlabpy/commit/6d5df9019932c4c6ad5930d952714e0bd181cacf))
+* trivial changes ([`6d5df90`](https://github.com/kmnhan/erlabpy/commit/6d5df9019932c4c6ad5930d952714e0bd181cacf))
 
-* refactor: easy import ([`b308d3d`](https://github.com/kmnhan/erlabpy/commit/b308d3d546ee92b04299d679042564149759206b))
+* easy import ([`b308d3d`](https://github.com/kmnhan/erlabpy/commit/b308d3d546ee92b04299d679042564149759206b))
 
-* refactor: cleanup and reorganize ([`136715b`](https://github.com/kmnhan/erlabpy/commit/136715b46da525bf7b8e28d2e26c306754d93e61))
+* cleanup and reorganize ([`136715b`](https://github.com/kmnhan/erlabpy/commit/136715b46da525bf7b8e28d2e26c306754d93e61))
 
-* refactor: update with new imagetool ([`6ec6f65`](https://github.com/kmnhan/erlabpy/commit/6ec6f65ca653ef1d90807c2f8448d12ae57d69c2))
+* update with new imagetool ([`6ec6f65`](https://github.com/kmnhan/erlabpy/commit/6ec6f65ca653ef1d90807c2f8448d12ae57d69c2))
 
-* refactor: deprecate mpl-based imagetool ([`5a28947`](https://github.com/kmnhan/erlabpy/commit/5a289471c08022bd4ac4502b176af73d4157c31c))
+* deprecate mpl-based imagetool ([`5a28947`](https://github.com/kmnhan/erlabpy/commit/5a289471c08022bd4ac4502b176af73d4157c31c))
 
-* refactor: sort imports ([`60f52f5`](https://github.com/kmnhan/erlabpy/commit/60f52f50feb68b48c1e3eaf965becf565129b8c0))
+* sort imports ([`60f52f5`](https://github.com/kmnhan/erlabpy/commit/60f52f50feb68b48c1e3eaf965becf565129b8c0))
 
-* refactor: cleanup code ([`58ca4ed`](https://github.com/kmnhan/erlabpy/commit/58ca4edeab44c0e665e0b272c1a42a0376d2223a))
+* cleanup code ([`58ca4ed`](https://github.com/kmnhan/erlabpy/commit/58ca4edeab44c0e665e0b272c1a42a0376d2223a))
 
-* refactor: reorganize plotting routines ([`f5ef54f`](https://github.com/kmnhan/erlabpy/commit/f5ef54f22c7a2b51c794fe00816fa8778da53060))
+* reorganize plotting routines ([`f5ef54f`](https://github.com/kmnhan/erlabpy/commit/f5ef54f22c7a2b51c794fe00816fa8778da53060))
 
 ### Style
 
-* style: format with black ([`82b2938`](https://github.com/kmnhan/erlabpy/commit/82b29382c3c01f7aea4c0ec511c3828de1177e10))
+* format with black ([`82b2938`](https://github.com/kmnhan/erlabpy/commit/82b29382c3c01f7aea4c0ec511c3828de1177e10))
 
-* style: remove relative imports ([`096a78d`](https://github.com/kmnhan/erlabpy/commit/096a78df4e09643961f358cf13d200d2428afc6f))
+* remove relative imports ([`096a78d`](https://github.com/kmnhan/erlabpy/commit/096a78df4e09643961f358cf13d200d2428afc6f))
 
-* style: remove relative imports ([`9891273`](https://github.com/kmnhan/erlabpy/commit/9891273e568c6673541866d3475990aed965fd5e))
+* remove relative imports ([`9891273`](https://github.com/kmnhan/erlabpy/commit/9891273e568c6673541866d3475990aed965fd5e))
 
-* style: add typing ([`1f16ebb`](https://github.com/kmnhan/erlabpy/commit/1f16ebb398dc29a4d0bddf77a422af926b7952da))
+* add typing ([`1f16ebb`](https://github.com/kmnhan/erlabpy/commit/1f16ebb398dc29a4d0bddf77a422af926b7952da))
 
-* style: remove unused imports ([`68ef006`](https://github.com/kmnhan/erlabpy/commit/68ef00632f75978e380c15bd6ad9040ef6565520))
+* remove unused imports ([`68ef006`](https://github.com/kmnhan/erlabpy/commit/68ef00632f75978e380c15bd6ad9040ef6565520))
 
 ### Test
 
-* test: tests initial commit
+* tests initial commit ([`fde2283`](https://github.com/kmnhan/erlabpy/commit/fde2283c646ce3b5335c6a8a2960da19380e7827))
 
-Add basic tests for fast binning, momentum conversion, and interpolation. ([`fde2283`](https://github.com/kmnhan/erlabpy/commit/fde2283c646ce3b5335c6a8a2960da19380e7827))
+  Add basic tests for fast binning, momentum conversion, and interpolation.
 
 ### Unknown
 
 * Merge branch &#39;main&#39; of https://github.com/kmnhan/erlabpy ([`ffb7de8`](https://github.com/kmnhan/erlabpy/commit/ffb7de8345100a5f935f9a97739f549f31bb014d))
 
 * Create LICENSE ([`2ee8814`](https://github.com/kmnhan/erlabpy/commit/2ee881436ded6073c889693af3e50f6124d651ce))
```

### Comparing `erlab-1.6.5/LICENSE` & `erlab-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/PKG-INFO` & `erlab-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 1.6.5
+Version: 2.0.0
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,34 +690,34 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.22.0
-Requires-Dist: numba>=0.56.2
-Requires-Dist: numbagg
-Requires-Dist: numba-progress
-Requires-Dist: joblib
-Requires-Dist: scipy>=1.8.0
-Requires-Dist: lmfit>=1.2.0
-Requires-Dist: uncertainties>=3.0.1
+Requires-Dist: h5netcdf>=1.2.0
+Requires-Dist: igor2>=0.5.6
 Requires-Dist: iminuit>=2.25.2
+Requires-Dist: joblib>=1.3.2
+Requires-Dist: lmfit>=1.2.0
 Requires-Dist: matplotlib>=3.8.0
-Requires-Dist: xarray
-Requires-Dist: h5netcdf
-Requires-Dist: varname
-Requires-Dist: tqdm
-Requires-Dist: pyperclip
-Requires-Dist: qtpy
+Requires-Dist: numba-progress>=1.0.0
+Requires-Dist: numba>=0.59.0
+Requires-Dist: numbagg>=0.8.1
+Requires-Dist: numpy>=1.26.0
+Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: pyqtgraph>=0.13.1
-Requires-Dist: qtawesome
-Requires-Dist: superqt
-Requires-Dist: importlib-metadata; python_version >= "3.11"
+Requires-Dist: qtawesome>=1.3.1
+Requires-Dist: qtpy>=2.4.1
+Requires-Dist: scipy>=1.12.0
+Requires-Dist: superqt>=0.6.2
+Requires-Dist: tqdm>=4.66.2
+Requires-Dist: uncertainties>=3.0.1
+Requires-Dist: varname>=0.13.0
+Requires-Dist: xarray>=2024.02.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # ERLabPy
```

### Comparing `erlab-1.6.5/PythonInterface.ipf` & `erlab-2.0.0/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/README.md` & `erlab-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/Makefile` & `erlab-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/environment.yml` & `erlab-2.0.0/docs/environment.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 name: erlabrtd
 channels:
   - conda-forge
 dependencies:
   - python>=3.11
   - pip>=19.3
   - ipykernel
+  - igor2>=0.5.6
   - numpy>=1.22.0
   - matplotlib>=3.8.0
   - hvplot
   - xarray
   - h5netcdf
   - varname
   - numba>=0.56.2
@@ -30,11 +31,9 @@
   - nbsphinx
   - furo
   - sphinx-design
   - pyperclip
   - pip:
     - pyqt6>=6.2.2
     - csaps
-    - igor2 @ git+https://github.com/kmnhan/igor2@master
-    - arpes @ git+https://github.com/kmnhan/arpes@master
     - -e git+https://github.com/kmnhan/erlabpy.git#egg=erlab
     - sphinx-qt-documentation
```

### Comparing `erlab-1.6.5/docs/make.bat` & `erlab-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/conf.py` & `erlab-2.0.0/docs/source/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -64,25 +64,25 @@
 
 # -- Autosummary and autodoc settings ----------------------------------------
 
 autosummary_generate = True
 autosummary_generate_overwrite = True
 
 autodoc_inherit_docstrings = False
-autodoc_typehints = "both"
+autodoc_typehints = "description"
 autodoc_typehints_format = "short"
 autodoc_class_signature = "mixed"
 autodoc_member_order = "bysource"
 autodoc_default_options = {
     "members": True,
     "undoc-members": True,
     # "exclude-members":("sigDataChanged",),
     "show-inheritance": False,
 }
-autodoc_typehints_description_target = "all"
+autodoc_typehints_description_target = "documented"
 
 # autodoc_type_aliases = {
 # "numpy.float64": "float",
 # "float64": "float",
 # }
 
 # -- Napoleon settings -------------------------------------------------------
@@ -123,15 +123,14 @@
     "numba": ("https://numba.readthedocs.io/en/stable/", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/", None),
     "lmfit": ("https://lmfit.github.io/lmfit-py/", None),
     "matplotlib": ("https://matplotlib.org/stable/", None),
     "xarray": ("https://docs.xarray.dev/en/stable/", None),
     "pandas": ("https://pandas.pydata.org/docs/", None),
     "pyqtgraph": ("https://pyqtgraph.readthedocs.io/en/latest/", None),
-    "arpes": ("https://arpes.readthedocs.io/en/latest/", None),
     "csaps": ("https://csaps.readthedocs.io/en/latest/", None),
     "iminuit": ("https://scikit-hep.org/iminuit/", None),
 }
 
 
 # -- Plot configuration ------------------------------------------------------
 
@@ -146,30 +145,71 @@
 # -- Bibliography settings ---------------------------------------------------
 
 pybtex.style.formatting.unsrt.date = pybtex.style.template.words(sep="")[
     "(", pybtex.style.template.field("year"), ")"
 ]
 
 
-class ApsStyle(pybtex.style.formatting.unsrt.Style):
+class APSStyle(pybtex.style.formatting.unsrt.Style):
     """
     APS style for BibTeX formatting, adapted from the conf.py file of the `mitiq
     library<https://github.com/unitaryfund/mitiq>`_.
     """
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.abbreviate_names = True
+
     def format_title(self, e, which_field, as_sentence=True):
         formatted_title = pybtex.style.template.field(
             which_field, apply_func=lambda text: text.capitalize()
         )
+
         formatted_title = pybtex.style.template.tag("em")[formatted_title]
         if as_sentence:
             return pybtex.style.template.sentence[formatted_title]
         else:
             return formatted_title
 
+    def format_editor(self, e, as_sentence=True):
+        editors = self.format_names("editor", as_sentence=False)
+        if "editor" not in e.persons:
+            return editors
+        result = pybtex.style.template.join(sep=" ")["edited by", editors]
+        if as_sentence:
+            return pybtex.style.template.sentence[result]
+        else:
+            return result
+
+    def format_address_organization_publisher_date(self, e, include_organization=True):
+        if include_organization:
+            organization = pybtex.style.template.optional_field("organization")
+        else:
+            organization = None
+        return pybtex.style.template.first_of[
+            pybtex.style.template.optional[
+                pybtex.style.template.join(sep=", ")[
+                    pybtex.style.template.sentence(add_period=False, sep=", ")[
+                        organization, pybtex.style.template.optional_field("publisher")
+                    ],
+                    pybtex.style.template.join(sep=", ")[
+                        pybtex.style.template.sentence(add_period=False)[
+                            pybtex.style.template.optional_field("address")
+                        ],
+                        pybtex.style.template.field("year"),
+                    ],
+                ]
+            ],
+            pybtex.style.template.join(sep=", ")[
+                organization,
+                pybtex.style.template.optional_field("publisher"),
+                pybtex.style.template.field("year"),
+            ],
+        ]
+
     def get_article_template(self, e):
         volume_and_pages = pybtex.style.template.first_of[
             # volume and pages
             pybtex.style.template.optional[
                 pybtex.style.template.join[
                     " ",
                     pybtex.style.template.tag("strong")[
@@ -248,16 +288,46 @@
                 ],
                 pybtex.style.formatting.unsrt.date,
             ],
             self.format_web_refs(e),
         ]
         return template
 
+    def get_inproceedings_template(self, e):
+        template = pybtex.style.formatting.toplevel[
+            pybtex.style.template.sentence[self.format_names("author")],
+            self.format_title(e, "title"),
+            pybtex.style.template.words[
+                "in",
+                pybtex.style.template.sentence[
+                    self.format_btitle(e, "booktitle", as_sentence=False),
+                    # self.format_volume_and_series(e, as_sentence=False),
+                    # self.format_chapter_and_pages(e),
+                    pybtex.style.template.field("year"),
+                    pybtex.style.template.sentence(add_period=False, sep=" ")[
+                        pybtex.style.template.optional[
+                            self.format_editor(e, as_sentence=False)
+                        ],
+                        pybtex.style.template.words(sep="")[
+                            "(", self.format_address_organization_publisher_date(e), ")"
+                        ],
+                    ],
+                    pybtex.style.template.sentence(add_period=True, sep=". ")[
+                        "p",
+                        pybtex.style.formatting.unsrt.pages,
+                        pybtex.style.template.optional_field("note"),
+                    ],
+                ],
+            ],
+            self.format_web_refs(e),
+        ]
+        return template
+
 
-pybtex.plugin.register_plugin("pybtex.style.formatting", "apsstyle", ApsStyle)
+pybtex.plugin.register_plugin("pybtex.style.formatting", "apsstyle", APSStyle)
 
 bibtex_bibfiles = ["refs.bib"]
 bibtex_default_style = "apsstyle"
 bibtex_footbibliography_header = ".. rubric:: References"
 
 
 # -- Options for HTML output -------------------------------------------------
@@ -292,12 +362,17 @@
     },
 }
 
 # -- LaTeX options -----------------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#latex-options
 
 latex_engine = "lualatex"
-latex_table_style = ["booktabs"]
+latex_show_pagerefs = True
+latex_show_urls = "footnote"
+latex_table_style = ["booktabs", "colorrows"]
 latex_elements = {
     "fontpkg": r"""\usepackage{fontspec,unicode-math}
-""",
+\setmainfont{DejaVu Serif}
+\setsansfont{DejaVu Sans}
+\setmonofont{DejaVu Sans Mono}
+"""
 }
```

### Comparing `erlab-1.6.5/docs/source/development.rst` & `erlab-2.0.0/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/getting-started.rst` & `erlab-2.0.0/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/images/imagetool_dark.png` & `erlab-2.0.0/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/images/imagetool_light.png` & `erlab-2.0.0/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/images/ktool_1_dark.png` & `erlab-2.0.0/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/images/ktool_1_light.png` & `erlab-2.0.0/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/images/ktool_2_dark.png` & `erlab-2.0.0/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/images/ktool_2_light.png` & `erlab-2.0.0/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/index.rst` & `erlab-2.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/notebooks/indexing.ipynb` & `erlab-2.0.0/docs/source/notebooks/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/notebooks/io.ipynb` & `erlab-2.0.0/docs/source/notebooks/io.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/notebooks/kconv.ipynb` & `erlab-2.0.0/docs/source/notebooks/kconv.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998816287878788%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(10, 'Momentum conversion in ERLabPy follows the "*

 * *            'nomenclature from :cite:t:`ishida2018kconv`. All experimental geometry are classified '*

 * *            "into 4 types. Definition of angles differ for each geometry.\\n')], delete: [10]}}}"}*

```diff
@@ -17,15 +17,15 @@
                 "Momentum conversion in ERLabPy is exact with no small angle approximation, but\n",
                 "is also very fast, thanks to the numba-accelerated trilinear interpolation in\n",
                 ":mod:`erlab.analysis.interpolate`\\ .\n",
                 "\n",
                 "Nomenclature\n",
                 "------------\n",
                 "\n",
-                "Momentum conversion in ERLabPy follows the nomenclature from :cite:t:`Ishida2018`. All experimental geometry are classified into 4 types. Definition of angles differ for each geometry.\n",
+                "Momentum conversion in ERLabPy follows the nomenclature from :cite:t:`ishida2018kconv`. All experimental geometry are classified into 4 types. Definition of angles differ for each geometry.\n",
                 "\n",
                 "For instance, image a typical Type 1 setup with a vertical slit that acquires maps by rotating about the `z` axis in the lab frame. In this case, the polar angle (rotation about `z`) is :math:`\u03b2`, and the tilt angle is :math:`\u03be`.\n",
                 "\n",
                 "In all cases, :math:`\u03b4` is the azimuthal angle that indicates in-plane rotation, and :math:`\u03b1` is the angle along the slit."
             ]
         },
         {
```

### Comparing `erlab-1.6.5/docs/source/notebooks/plotting.ipynb` & `erlab-2.0.0/docs/source/notebooks/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/pyplots/norms.py` & `erlab-2.0.0/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/reference.rst` & `erlab-2.0.0/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/docs/source/userguide.rst` & `erlab-2.0.0/docs/source/userguide.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 **********
 User Guide
 **********
 
 .. admonition:: Work in Progress
    :class: warning
 
-   The user guide is incomplete. For the full list of packages and modules provided by ERLabPy, see :doc:`reference`.
+   The user guide is incomplete. For the full list of packages and modules
+   provided by ERLabPy, see :doc:`reference`.
 
-This section contains some examples for getting started with ARPES data analysis and visualization.
+This section contains some examples for getting started with ARPES data analysis
+and visualization.
 
 
 Introduction
 ============
 
 The following documentation assumes basic python programming experience.
 
-If you are new to scientific programming in python altogether, `Scientific Python Lectures <https://github.com/jrjohansson/scientific-python-lectures>`_ is a great resource to get started.
-
-Data in ERLabPy are mostly represented by :mod:`xarray` objects. The user guide of the `xarray documentation <https://docs.xarray.dev/en/stable/index.html>`_ provides an excellent overview on data manipulation.
+If you are new to scientific programming in python altogether, `Scientific
+Python Lectures <https://github.com/jrjohansson/scientific-python-lectures>`_ is
+a great resource to get started.
+
+Data in ERLabPy are mostly represented by :mod:`xarray` objects
+:cite:p:`hoyer2017xarray`. The `xarray user guide
+<https://docs.xarray.dev/en/stable/index.html>`_ and the `xarray tutorial
+<https://tutorial.xarray.dev/>`_ are great resources to get started with xarray.
 
 .. toctree::
    notebooks/io
    notebooks/indexing
    notebooks/plotting
    notebooks/kconv
 
 Further Reading
 ===============
 
-- `Lectures on scientific computing with Python <https://github.com/jrjohansson/scientific-python-lectures>`_
-- `The beginner's guide to numpy <https://numpy.org/doc/stable/user/absolute_beginners.html>`_
+- `Lectures on scientific computing with Python
+  <https://github.com/jrjohansson/scientific-python-lectures>`_
+- `The beginner's guide to numpy
+  <https://numpy.org/doc/stable/user/absolute_beginners.html>`_
+- `Xarray tutorial <https://tutorial.xarray.dev/>`_
```

### Comparing `erlab-1.6.5/environment_nogit_mkl.yml` & `erlab-2.0.0/environment_apple.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,33 @@
 name: erlab
 channels:
   - conda-forge
 dependencies:
-  - python>=3.11
-  - ipython
-  - pip>=19.3
-  - setuptools
-  - libblas=*=*mkl
-  - libcblas=*=*mkl
-  - liblapack=*=*mkl
-  - liblapacke=*=*mkl
-  - h5netcdf
-  - varname
-  - numpy>=1.22.0
-  - scipy>=1.8.0
-  - matplotlib>=3.7.0
-  - h5py>=3.2.1
-  - netCDF4>=1.5.0
-  - astropy
-  - superqt>=0.3.1
-  - dill
-  - llvm-openmp>=13.0.0
-  - llvmlite
-  - asteval>=0.9.22
-  - xarray>=0.16.1
-  - numba>=0.56.2
-  - ase>=3.17.0
-  - bokeh>=2.0.0
-  - bottleneck>=1.3.2
-  - colorama
-  - imageio
-  - ipywidgets>=7.0.1
-  - joblib
+  - h5netcdf>=1.2.0
+  - igor2>=0.5.6
+  - iminuit>=2.25.2
+  - ipykernel
+  - joblib>=1.3.2
+  - libblas=*=*accelerate
+  - libcblas=*=*accelerate
+  - liblapack=*=*accelerate
+  - liblapacke=*=*accelerate
   - lmfit>=1.2.0
-  - pandas
-  - pint
-  - psutil
-  - pygments
+  - matplotlib>=3.8.0
+  - numba-progress>=1.0.0
+  - numba>=0.59.0
+  - numbagg>=0.8.1
+  - numpy>=1.26.0
+  - pip>=19.3
+  - pyperclip>=1.8.2
   - pyqtgraph>=0.13.1
-  - rx
-  - scikit-image
-  - scikit-learn>=0.24.0
-  - tbb
-  - titlecase
-  - tqdm
+  - python>=3.11
+  - qtawesome>=1.3.1
+  - qtpy>=2.4.1
+  - scipy>=1.12.0
+  - superqt>=0.6.2
+  - tqdm>=4.66.2
   - uncertainties>=3.0.1
-  - qtawesome
-  - numbagg
-  - numba-progress
-  - iminuit>=2.3
-  - pyperclip
+  - varname>=0.13.0
+  - xarray>=2024.02.0
   - pip:
     - pyqt6>=6.2.2
```

### Comparing `erlab-1.6.5/pyproject.toml` & `erlab-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,34 +17,34 @@
     "Topic :: Scientific/Engineering :: Visualization",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "numpy>=1.22.0",
-    "numba>=0.56.2",
-    "numbagg",
-    "numba-progress",
-    "joblib",
-    "scipy>=1.8.0",
-    "lmfit>=1.2.0",
-    "uncertainties>=3.0.1",
+    "h5netcdf>=1.2.0",
+    "igor2>=0.5.6",
     "iminuit>=2.25.2",
+    "joblib>=1.3.2",
+    "lmfit>=1.2.0",
     "matplotlib>=3.8.0",
-    "xarray",
-    "h5netcdf",
-    "varname",
-    "tqdm",
-    "pyperclip",
-    "qtpy",
+    "numba-progress>=1.0.0",
+    "numba>=0.59.0",
+    "numbagg>=0.8.1",
+    "numpy>=1.26.0",
+    "pyperclip>=1.8.2",
     "pyqtgraph>=0.13.1",
-    "qtawesome",
-    "superqt",
-    'importlib-metadata; python_version>="3.11"',
+    "qtawesome>=1.3.1",
+    "qtpy>=2.4.1",
+    "scipy>=1.12.0",
+    "superqt>=0.6.2",
+    "tqdm>=4.66.2",
+    "uncertainties>=3.0.1",
+    "varname>=0.13.0",
+    "xarray>=2024.02.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://erlabpy.readthedocs.io"
 Repository = "https://github.com/kmnhan/erlabpy.git"
 Issues = "https://github.com/kmnhan/erlabpy/issues"
@@ -55,14 +55,16 @@
 
 [tool.setuptools]
 package-dir = { "" = "src" }
 
 [tool.setuptools.dynamic]
 version = { attr = "erlab.__version__" }
 
+[tool.setuptools_scm]
+
 [tool.semantic_release]
 assets = []
 build_command = "pip install build && python -m build"
 commit_message = "{version}\n\nAutomatically generated by python-semantic-release"
 commit_parser = "angular"
 logging_use_named_masks = false
 major_on_zero = true
@@ -187,7 +189,10 @@
 skip-magic-trailing-comma = false
 line-ending = "auto"
 docstring-code-format = true
 docstring-code-line-length = "dynamic"
 
 [tool.isort]
 profile = "black"
+
+[tool.pytest.ini_options]
+testpaths = "tests"
```

### Comparing `erlab-1.6.5/src/erlab/accessors.py` & `erlab-2.0.0/src/erlab/accessors.py`

 * *Files 0% similar despite different names*

```diff
@@ -794,15 +794,15 @@
         )
 
     @property
     @only_angles
     def best_kz_resolution(self) -> float:
         r"""
         Estimates the minimum out-of-plane momentum resolution based on the mean free
-        path :cite:p:`Seah1979` and the kinetic energy.
+        path :cite:p:`seah1979imfp` and the kinetic energy.
 
         .. math:: \Delta k_z \sim 1/\lambda
 
         """
         kin = self._kinetic_energy.flatten()
         c1, c2 = 641.0, 0.096
         imfp = (c1 / (kin**2) + c2 * np.sqrt(kin)) * 10
```

### Comparing `erlab-1.6.5/src/erlab/analysis/__init__.py` & `erlab-2.0.0/src/erlab/analysis/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 .. autosummary::
    :toctree: generated
 
    fit
    mask
    correlation
    gold
+   image
    interpolate
    kspace
    transform
    utilities
 
 """
```

### Comparing `erlab-1.6.5/src/erlab/analysis/correlation.py` & `erlab-2.0.0/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.0.0/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 These functions are not limited to a single function form, and can be used to create
 complex models.
 """
 
 __all__ = [
     "get_args_kwargs",
     "DynamicFunction",
-    "PolyFunc",
+    "PolynomialFunction",
     "MultiPeakFunction",
-    "FermiEdge2dFunc",
+    "FermiEdge2dFunction",
 ]
 import functools
 import inspect
 from collections.abc import Callable
 
 import numpy as np
 import numpy.typing as npt
@@ -91,15 +91,15 @@
     def kwargs(self) -> dict[str, int | float]:
         return {}
 
     def __call__(self, x: npt.NDArray[np.float64], **params) -> npt.NDArray[np.float64]:
         raise NotImplementedError("Must be overloaded in child classes")
 
 
-class PolyFunc(DynamicFunction):
+class PolynomialFunction(DynamicFunction):
     """A callable class for a arbitrary degree polynomial.
 
     Parameters
     ----------
     degree
         The degree of the polynomial.
 
@@ -115,15 +115,17 @@
 
     def __call__(self, x, *coeffs, **params):
         if len(coeffs) != self.degree + 1:
             coeffs = [params[f"c{d}"] for d in range(self.degree + 1)]
         if isinstance(x, np.ndarray):
             return np.polynomial.polynomial.polyval(x, coeffs)
         else:
-            coeffs = xr.DataArray(coeffs, coords={"degree": np.arange(self.degree + 1)})
+            coeffs = xr.DataArray(
+                np.asarray(coeffs), coords={"degree": np.arange(self.degree + 1)}
+            )
             return xr.polyval(x, coeffs)
 
 
 class MultiPeakFunction(DynamicFunction):
     """A callable class for a multi-peak model.
 
     Parameters
@@ -257,24 +259,31 @@
             y += params["offset"]
 
         return y
 
     def __call__(
         self, x: npt.NDArray[np.float64], **params: dict
     ) -> npt.NDArray[np.float64]:
+        if isinstance(x, xr.DataArray):
+            return x * 0.0 + self.__call__(x.values, **params)
+
         if self.convolve:
+            if "resolution" not in params:
+                raise TypeError(
+                    "Missing parameter `resolution` required for convolution"
+                )
             return do_convolve(x, self.pre_call, **params)
         else:
             return self.pre_call(x, **params)
 
 
-class FermiEdge2dFunc(DynamicFunction):
+class FermiEdge2dFunction(DynamicFunction):
     def __init__(self, degree=1) -> None:
         super().__init__()
-        self.poly = PolyFunc(degree)
+        self.poly = PolynomialFunction(degree)
 
     @property
     def argnames(self) -> list[str]:
         return ["eV", "alpha"] + self.poly.argnames[1:]
 
     @property
     def kwargs(self):
@@ -292,8 +301,19 @@
             *[params.pop(f"c{i}") for i in range(self.poly.degree + 1)],
         )
         return (params["const_bkg"] - params["offset"] + params["lin_bkg"] * eV) / (
             1 + np.exp((1.0 * eV - center) / max(TINY, params["temp"] * kb_eV))
         ) + params["offset"]
 
     def __call__(self, eV, alpha, **params: dict):
+        if isinstance(eV, xr.DataArray) and isinstance(alpha, xr.DataArray):
+            out = eV * alpha * 0.0
+            return out + self.__call__(eV.values, alpha.values, **params).reshape(
+                out.shape
+            )
+        if isinstance("eV", xr.DataArray):
+            eV = eV.values
+        if isinstance("alpha", xr.DataArray):
+            alpha = alpha.values
+        if "resolution" not in params:
+            raise TypeError("Missing parameter `resolution` required for convolution")
         return do_convolve_y(eV, alpha, self.pre_call, **params).flatten()
```

### Comparing `erlab-1.6.5/src/erlab/analysis/fit/functions/general.py` & `erlab-2.0.0/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/analysis/fit/minuit.py` & `erlab-2.0.0/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/analysis/fit/models.py` & `erlab-2.0.0/src/erlab/analysis/fit/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,33 +4,25 @@
     "ExtendedAffineBroadenedFD",
     "StepEdgeModel",
     "PolynomialModel",
     "MultiPeakModel",
     "FermiEdge2dModel",
 ]
 
-
-import importlib
-
 import lmfit
 import numba
 import numpy as np
 import numpy.typing as npt
 import scipy.ndimage
 import xarray as xr
 
-if importlib.util.find_spec("arpes"):
-    from arpes.fits import XModelMixin
-else:
-    from lmfit.models import Model as XModelMixin
-
 from erlab.analysis.fit.functions import (
-    FermiEdge2dFunc,
+    FermiEdge2dFunction,
     MultiPeakFunction,
-    PolyFunc,
+    PolynomialFunction,
     fermi_dirac_linbkg_broad,
     step_linbkg_broad,
 )
 
 
 @numba.njit("f8[:,:](f8[:], i8)", cache=True)
 def _coeff_mat(x, deg):
@@ -104,94 +96,81 @@
         np.array(x[-len_fit:], dtype=np.float64),
         np.array(data[-len_fit:], dtype=np.float64),
         deg=1,
     )
     return n0, m0, n1, m1
 
 
-class ExtendedAffineBroadenedFD(XModelMixin):
+class ExtendedAffineBroadenedFD(lmfit.Model):
     """
     Fermi-dirac function with linear background above and below the fermi level,
     convolved with a gaussian kernel.
     """
 
-    guess_dataarray = True
-
     @staticmethod
     def LinearBroadFermiDirac(
         x,
-        center=0,
-        temp=30,
+        center=0.0,
+        temp=30.0,
         resolution=0.02,
-        back0=1,
-        back1=0,
-        dos0=1,
-        dos1=0,
+        back0=0.0,
+        back1=0.0,
+        dos0=1.0,
+        dos1=0.0,
     ):
         return fermi_dirac_linbkg_broad(
             x, center, temp, resolution, back0, back1, dos0, dos1
         )
 
-    def __init__(
-        self, independent_vars=("x",), prefix="", missing="raise", name=None, **kwargs
-    ):
-        """Defer to lmfit for initialization."""
-        kwargs.update(
-            {"prefix": prefix, "missing": missing, "independent_vars": independent_vars}
-        )
+    def __init__(self, **kwargs):
         super().__init__(self.LinearBroadFermiDirac, **kwargs)
         self.set_param_hint("temp", min=0.0)
         self.set_param_hint("resolution", min=0.0)
 
     def guess(self, data, x, **kwargs):
-        """Make some heuristic guesses."""
         pars = self.make_params()
 
         len_fit = max(round(len(x) * 0.05), 10)
         dos0, dos1, back0, back1 = fit_edges_linear(x, data, len_fit)
-        efermi = x[
+        efermi = np.asarray(x)[
             np.argmin(np.gradient(scipy.ndimage.gaussian_filter1d(data, 0.2 * len(x))))
         ]
 
-        temp = 30
+        temp = 30.0
         if isinstance(data, xr.DataArray):
             try:
-                temp = data.attrs["temp_sample"]
+                temp = float(data.attrs["temp_sample"])
             except KeyError:
                 pass
 
-        pars[f"{self.prefix}center"].set(value=efermi, min=x.min(), max=x.max())
+        pars[f"{self.prefix}center"].set(
+            value=efermi, min=np.asarray(x).min(), max=np.asarray(x).max()
+        )
         pars[f"{self.prefix}back0"].set(value=back0)
         pars[f"{self.prefix}back1"].set(value=back1)
         pars[f"{self.prefix}dos0"].set(value=dos0)
         pars[f"{self.prefix}dos1"].set(value=dos1)
         pars[f"{self.prefix}temp"].set(value=temp)
         pars[f"{self.prefix}resolution"].set(value=0.02)
 
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
 
     __init__.doc = lmfit.models.COMMON_INIT_DOC
     guess.__doc__ = lmfit.models.COMMON_GUESS_DOC
 
 
-class StepEdgeModel(XModelMixin):
-    guess_dataarray = True
-
-    def __init__(
-        self, independent_vars=("x",), prefix="", missing="raise", name=None, **kwargs
-    ):
-        """Defer to lmfit for initialization."""
+class StepEdgeModel(lmfit.Model):
+    def __init__(self, independent_vars=("x",), prefix="", missing="raise", **kwargs):
         kwargs.update(
             {"prefix": prefix, "missing": missing, "independent_vars": independent_vars}
         )
         super().__init__(step_linbkg_broad, **kwargs)
         self.set_param_hint("sigma", min=0.0)
 
     def guess(self, data, x, **kwargs):
-        """Make some heuristic guesses."""
         pars = self.make_params()
 
         len_fit = max(round(len(x) * 0.05), 10)
         dos0, dos1, back0, back1 = fit_edges_linear(x, data, len_fit)
         efermi = x[
             np.argmin(np.gradient(scipy.ndimage.gaussian_filter1d(data, 0.2 * len(x))))
         ]
@@ -205,18 +184,18 @@
 
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
 
     __init__.doc = lmfit.models.COMMON_INIT_DOC
     guess.__doc__ = lmfit.models.COMMON_GUESS_DOC
 
 
-class PolynomialModel(XModelMixin):
+class PolynomialModel(lmfit.Model):
     def __init__(self, degree=9, **kwargs):
         kwargs.setdefault("name", f"Poly{degree}")
-        super().__init__(PolyFunc(degree), **kwargs)
+        super().__init__(PolynomialFunction(degree), **kwargs)
 
     def guess(self, data, x=None, **kwargs):
         pars = self.make_params()
         if x is None:
             pars["c0"].set(value=data.mean())
             for i in range(1, self.func.degree + 1):
                 pars[f"{self.prefix}c{i}"].set(value=0.0)
@@ -226,44 +205,34 @@
                 pars[f"{self.prefix}c{i}"].set(value=coef)
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
 
     __init__.doc = lmfit.models.COMMON_INIT_DOC
     guess.__doc__ = lmfit.models.COMMON_GUESS_DOC
 
 
-class MultiPeakModel(XModelMixin):
+class MultiPeakModel(lmfit.Model):
     """Model for fitting multiple Gaussian or Lorentzian peaks.
 
-    Most input parameters are passed to the
-    `erlab.analysis.fit.functions.MultiPeakFunction` constructor.
+    Most input parameters are passed to the :class:`MultiPeakFunction
+    <erlab.analysis.fit.functions.MultiPeakFunction>` constructor.
     """
 
     def __init__(
         self,
         npeaks: int = 1,
         peak_shapes: list[str] | str | None = None,
         fd: bool = True,
         convolve: bool = True,
-        independent_vars=None,
-        param_names=None,
-        nan_policy="raise",
-        prefix="",
-        name=None,
-        **kws,
+        **kwargs,
     ):
         super().__init__(
             MultiPeakFunction(
                 npeaks, peak_shapes=peak_shapes, fd=fd, convolve=convolve
             ),
-            independent_vars,
-            param_names,
-            nan_policy,
-            prefix,
-            name,
-            **kws,
+            **kwargs,
         )
 
         if self.func.convolve:
             self.set_param_hint("resolution", min=0.0)
 
     def guess(self, data, x=None, **kwargs):
         pars = self.make_params()
@@ -286,15 +255,15 @@
             pars[f"{self.prefix}p{i}_width"].set(value=0.1 * xrange)
 
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
 
     guess.__doc__ = lmfit.models.COMMON_GUESS_DOC
 
 
-class FermiEdge2dModel(XModelMixin):
+class FermiEdge2dModel(lmfit.Model):
     r"""A 2D model for a polynomial Fermi edge with a linear density of states.
 
     The model function can be written as
 
     .. math::
 
         I = \left\{(a\omega + b)\left[1 + \exp\left(\frac{\omega - \sum_{i = 0}^{n} c_i
@@ -303,38 +272,25 @@
     for a :math:`n` th degree polynomial edge with coefficients :math:`c_i` with a
     linear density of states described by :math:`a\omega+b` with a constant background
     :math:`c` convolved with a gaussian, where :math:`\omega` is the binding energy and
     :math:`\alpha` is the detector angle.
 
     """
 
-    n_dims = 2
-    dimension_order = ["eV", "alpha"]
-    guess_dataarray = True
-    fit_flat = True
-
     def __init__(
         self,
-        degree=2,
+        degree: int = 2,
         independent_vars=("eV", "alpha"),
-        prefix="",
-        nan_policy="raise",
         **kwargs,
     ):
-        kwargs.update(
-            {
-                "prefix": prefix,
-                "nan_policy": nan_policy,
-                "independent_vars": independent_vars,
-            }
-        )
-        super().__init__(FermiEdge2dFunc(degree), **kwargs)
+        kwargs.update({"independent_vars": independent_vars})
+        super().__init__(FermiEdge2dFunction(degree), **kwargs)
         self.name = f"FermiEdge2dModel (deg {degree})"
 
-    def guess(self, data, eV, alpha, negative=False, **kwargs):
+    def guess(self, data, eV, alpha, **kwargs):
         pars = self.make_params()
         for i in range(self.func.poly.degree + 1):
             pars[f"{self.prefix}c{i}"].set(value=0.0)
 
         avg_edc = data.mean("alpha").values
         len_fit = max(round(len(eV) * 0.05), 10)
         dos0, dos1 = fit_poly_jit(
@@ -344,12 +300,15 @@
         )
         pars[f"{self.prefix}const_bkg"].set(value=dos0)
         pars[f"{self.prefix}lin_bkg"].set(value=dos1)
         pars[f"{self.prefix}temp"].set(value=data.attrs["temp_sample"])
 
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
 
-    def guess_fit(self, *args, **kwargs):
-        return super().guess_fit(*args, **kwargs)
+    def fit(self, data, *args, **kwargs):
+        if isinstance(data, xr.DataArray):
+            data = data.transpose("eV", "alpha").values
+        # Ensure flat fit
+        return super().fit(data.ravel(), *args, **kwargs)
 
     __init__.__doc__ = lmfit.models.COMMON_INIT_DOC.replace("['x']", "['eV', 'alpha']")
     guess.__doc__ = lmfit.models.COMMON_GUESS_DOC
```

### Comparing `erlab-1.6.5/src/erlab/analysis/fit/spline.py` & `erlab-2.0.0/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/analysis/gold.py` & `erlab-2.0.0/src/erlab/analysis/gold.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     "poly",
     "poly_from_edge",
     "spline_from_edge",
     "resolution",
     "resolution_roi",
 ]
 
-import importlib
 from collections.abc import Sequence
 
+import joblib
 import lmfit.model
 import matplotlib
 import matplotlib.figure
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
@@ -25,31 +25,30 @@
 
 from erlab.analysis.fit.models import (
     ExtendedAffineBroadenedFD,
     PolynomialModel,
     StepEdgeModel,
 )
 from erlab.analysis.utilities import correct_with_edge
+from erlab.parallel import joblib_progress
 from erlab.plotting.general import autoscale_to, figwh
 
-if importlib.util.find_spec("arpes"):
-    import arpes.fits
-
 
 def edge(
     gold: xr.DataArray | xr.Dataset,
     angle_range: tuple[float, float],
     eV_range: tuple[float, float],
     bin_size: tuple[int, int] = (1, 1),
     temp: float | None = None,
     vary_temp: bool = False,
     fast: bool = False,
     method: str = "leastsq",
     progress: bool = True,
     parallel_kw: dict | None = None,
+    parallel_obj: joblib.Parallel | None = None,
     return_full: bool = False,
     fixed_center: float | None = None,
     scale_covar: bool = True,
     **kwargs: dict,
 ) -> tuple[npt.NDArray, npt.NDArray] | xr.Dataset:
     """
     Fit a Fermi edge to the given gold data.
@@ -74,14 +73,17 @@
         `False`.
     method
         The fitting method to use, by default ``"leastsq"``.
     progress
         Whether to display the fitting progress, by default `True`.
     parallel_kw
         Additional keyword arguments for parallel fitting, by default `None`.
+    parallel_obj
+        The `joblib.Parallel` object to use for fitting, by default `None`. If provided,
+        `parallel_kw` will be ignored.
     return_full
         Whether to return the full fit results, by default `False`.
     fixed_center
         The fixed center value. If provided, the Fermi level will be fixed at the given
         value, by default `None`.
     scale_covar
         Whether to scale the covariance matrix, by default `True`.
@@ -95,65 +97,107 @@
         is `False`.
     fitresults
         A dataset containing the full fit results, returned when `return_full` is
         `True`.
 
     """
     if fast:
-        params = {}
+        params = lmfit.create_params()
         model_cls = StepEdgeModel
     else:
         if temp is None:
             temp = gold.attrs["temp_sample"]
-        params = {
-            "temp": {"value": temp, "vary": vary_temp},
-        }
+        params = lmfit.create_params(temp={"value": temp, "vary": vary_temp})
         model_cls = ExtendedAffineBroadenedFD
 
+    model = model_cls()
+
     if parallel_kw is None:
         parallel_kw = {}
 
     if fixed_center is not None:
-        params["center"] = {"value": fixed_center, "vary": False}
+        params["center"].set(value=fixed_center, vary=False)
 
     if any(b != 1 for b in bin_size):
         gold_binned = gold.coarsen(alpha=bin_size[0], eV=bin_size[1], boundary="trim")
         gold = gold_binned.mean()
 
     gold_sel = gold.sel(alpha=slice(*angle_range), eV=slice(*eV_range))
 
     # Assuming Poisson noise, the weights are the square root of the counts.
-    weights = np.sqrt(gold.sum("eV"))
+    weights = 1 / np.sqrt(gold_sel.sum("eV").values)
+
+    n_fits = len(gold_sel.alpha)
+
+    if parallel_obj is None:
+        if n_fits > 20:
+            parallel_kw.setdefault("n_jobs", -1)
+        else:
+            parallel_kw.setdefault("n_jobs", 1)
+        parallel_obj = joblib.Parallel(**parallel_kw)
+
+    def _fit(data, w):
+        pars = model.guess(data, x=data["eV"]).update(params)
+
+        res = model.fit(
+            data,
+            x=data["eV"],
+            params=pars,
+            method=method,
+            scale_covar=scale_covar,
+            weights=w,
+        )
+        return res
+
+    if progress:
+        with joblib_progress(desc="Fitting", total=n_fits) as _:
+            fitresults = parallel_obj(
+                joblib.delayed(_fit)(gold_sel.isel(alpha=i), weights[i])
+                for i in range(n_fits)
+            )
+    else:
+        fitresults = parallel_obj(
+            joblib.delayed(_fit)(gold_sel.isel(alpha=i), weights[i])
+            for i in range(n_fits)
+        )
 
-    fitresults = arpes.fits.broadcast_model(
-        model_cls,
-        gold_sel,
-        "alpha",
-        weights=weights,
-        params=params,
-        method=method,
-        progress=progress,
-        parallel_kw=parallel_kw,
-        scale_covar=scale_covar,
-        **kwargs,
-    )
     if return_full:
         return fitresults
 
-    center_arr, center_stderr = fitresults.F.p("center"), fitresults.F.s("center")
-    center_arr = center_arr.where(~center_stderr.isnull(), drop=True)
-    center_stderr = center_stderr.where(~center_stderr.isnull(), drop=True)
-    return center_arr, center_stderr
+    xval = []
+    res_vals = []
+
+    for i, r in enumerate(fitresults):
+        center_ufloat = r.uvars["center"]
+
+        if not np.isnan(center_ufloat.std_dev):
+            xval.append(gold_sel.alpha.values[i])
+            res_vals.append([center_ufloat.nominal_value, center_ufloat.std_dev])
+
+    xval = np.asarray(xval)
+    yval, yerr = np.asarray(res_vals).T
+
+    return (
+        xr.DataArray(yval, coords={"alpha": xval}),
+        xr.DataArray(yerr, coords={"alpha": xval}),
+    )
 
 
 def poly_from_edge(
     center, weights=None, degree=4, method="leastsq", scale_covar=True
 ) -> lmfit.model.ModelResult:
-    modelresult = PolynomialModel(degree=degree).guess_fit(
-        center, weights=weights, method=method, scale_covar=scale_covar
+    model = PolynomialModel(degree=degree)
+    pars = model.guess(center.values, x=center[center.dims[0]].values)
+    modelresult = model.fit(
+        center,
+        x=center[center.dims[0]].values,
+        params=pars,
+        weights=weights,
+        method=method,
+        scale_covar=scale_covar,
     )
     return modelresult
 
 
 def spline_from_edge(
     center, weights: Sequence[float] | None = None, lam: float | None = None
 ) -> scipy.interpolate.BSpline:
@@ -387,20 +431,22 @@
 
     if eV_range_fit is None:
         eV_range_fit = tuple(r - np.mean(pol.best_fit) for r in eV_range_edge)
     del pol
     gold_roi = gold_corr.sel(alpha=slice(*angle_range))
     edc_avg = gold_roi.mean("alpha").sel(eV=slice(*eV_range_fit))
 
-    params = {
-        "temp": {"value": gold.attrs["temp_sample"], "vary": False},
-        "resolution": {"value": 0.1, "vary": True, "min": 0},
-    }
-    fit = ExtendedAffineBroadenedFD().guess_fit(
-        edc_avg, params=params, method=method, scale_covar=scale_covar
+    params = lmfit.create_params(
+        temp={"value": gold_roi.attrs["temp_sample"], "vary": False},
+        resolution={"value": 0.1, "vary": True, "min": 0},
+    )
+    model = ExtendedAffineBroadenedFD()
+    params = model.guess(edc_avg, x=edc_avg["eV"]).update(params)
+    fit = ExtendedAffineBroadenedFD().fit(
+        edc_avg, x=edc_avg["eV"], params=params, method=method, scale_covar=scale_covar
     )
     if plot:
         plt.show()
         ax = plt.gca()
         gold_corr.qplot(ax=ax, cmap="copper", gamma=0.5)
         rect = mpatches.Rectangle(
             (angle_range[0], eV_range_fit[0]),
@@ -433,20 +479,23 @@
     fix_temperature: bool = True,
     method: str = "leastsq",
     plot: bool = True,
     scale_covar: bool = True,
 ) -> lmfit.model.ModelResult:
     edc_avg = gold_roi.mean("alpha").sel(eV=slice(*eV_range))
 
-    params = {
-        "temp": {"value": gold_roi.attrs["temp_sample"], "vary": not fix_temperature},
-        "resolution": {"value": 0.1, "vary": True, "min": 0},
-    }
-    fit = ExtendedAffineBroadenedFD().guess_fit(
+    params = lmfit.create_params(
+        temp={"value": gold_roi.attrs["temp_sample"], "vary": not fix_temperature},
+        resolution={"value": 0.1, "vary": True, "min": 0},
+    )
+    model = ExtendedAffineBroadenedFD()
+    params = model.guess(edc_avg, x=edc_avg["eV"]).update(params)
+    fit = model.fit(
         edc_avg,
+        x=edc_avg["eV"],
         params=params,
         method=method,
         scale_covar=scale_covar,  # weights=1 / edc_stderr
     )
     if plot:
         ax = plt.gca()
         gold_roi.qplot(ax=ax, cmap="copper", gamma=0.5)
```

### Comparing `erlab-1.6.5/src/erlab/analysis/interpolate.py` & `erlab-2.0.0/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/analysis/kspace.py` & `erlab-2.0.0/src/erlab/analysis/kspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Momentum conversion functions.
 
 Typically, the user will not have to call this module directly, but will instead use the
 :func:`erlab.accessors.MomentumAccessor.convert` method.
 
-Angle conventions and function forms are based on Ref. :cite:p:`Ishida2018`.
+Angle conventions and function forms are based on Ref. :cite:p:`ishida2018kconv`.
 
 """
 
 import enum
 from collections.abc import Callable
 
 import numpy as np
@@ -17,15 +17,15 @@
 import erlab.io
 import erlab.lattice
 
 
 class AxesConfiguration(enum.IntEnum):
     """
     Enum class representing different types of axes configurations. See Ref.
-    :cite:p:`Ishida2018`.
+    :cite:p:`ishida2018kconv`.
 
     """
 
     Type1 = 1
     Type2 = 2
     Type1DA = 3
     Type2DA = 4
@@ -63,15 +63,15 @@
         The kinetic energy in eV.
     configuration
         Experimental configuration.
     angle_params
         Dictionary of required angle parameters. If the configuration has a DA, the
         parameters should be `delta`, `chi`, `chi0`, `xi`, and `xi0`. Otherwise, they
         should be `delta`, `xi`, `xi0`, and `beta0`, following the notation in Ref.
-        :cite:p:`Ishida2018`.
+        :cite:p:`ishida2018kconv`.
 
     Returns
     -------
     forward_func : Callable
         Forward function that takes :math:`(α, β)` and returns :math:`(k_x, k_y)`.
     inverse_func : Callable
         Inverse function that takes :math:`(k_x, k_y)` or :math:`(k_x, k_y, k_z)` and
```

### Comparing `erlab-1.6.5/src/erlab/analysis/mask/__init__.py` & `erlab-2.0.0/src/erlab/analysis/mask/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Functions related to masking.
 
 Polygon masking is adapted from the `CGAL
 <https://doc.cgal.org/5.3.2/Polygon/index.html>`_ library. More information on
-point-in-polygon strategies can be found in Ref. :cite:p:`Schirra2008`.
+point-in-polygon strategies can be found in Ref. :cite:p:`schirra2008polygon`.
 
 .. currentmodule:: erlab.analysis.mask
 
 Modules
 =======
 
 .. autosummary::
```

### Comparing `erlab-1.6.5/src/erlab/analysis/mask/polygon.py` & `erlab-2.0.0/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/analysis/transform.py` & `erlab-2.0.0/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/analysis/utilities.py` & `erlab-2.0.0/src/erlab/analysis/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,20 @@
     """Shifts the values of a DataArray along a specified dimension.
 
     Parameters
     ----------
     darr
         The array to shift.
     shift
-        The amount of shift to be applied along the specified dimension. If `shift` is a
-        DataArray, different shifts can be applied to different coordinates. The
-        dimensions of `shift` must be a subset of the dimensions of `darr`. For more
-        information, see the note below. If `shift` is a `float`, the same shift is
-        applied to all values along dimension `along`. This is equivalent to providing a
-        0-dimensional DataArray.
+        The amount of shift to be applied along the specified dimension. If
+        :code:`shift` is a DataArray, different shifts can be applied to different
+        coordinates. The dimensions of :code:`shift` must be a subset of the dimensions
+        of `darr`. For more information, see the note below. If :code:`shift` is a
+        `float`, the same shift is applied to all values along dimension `along`. This
+        is equivalent to providing a 0-dimensional DataArray.
     along
         Name of the dimension along which the shift is applied.
     shift_coords
         If `True`, the coordinates of the output data will be changed so that the output
         contains all the values of the original data. If `False`, the coordinates and
         shape of the original data will be retained, and only the data will be shifted.
         Defaults to `False`.
@@ -145,36 +145,40 @@
     modelresult: lmfit.model.ModelResult | npt.NDArray[np.floating] | Callable,
     shift_coords: bool = True,
     plot: bool = False,
     plot_kw: dict | None = None,
     **shift_kwargs,
 ):
     """
-    Corrects the given data array `darr` using the edge correction method.
+    Corrects the given data array `darr` with the given values or fit result.
 
     Parameters
     ----------
     darr
         The input data array to be corrected.
     modelresult
         The model result that contains the fermi edge information. It can be an instance
-        of `lmfit.model.ModelResult`, a numpy array, or a callable function that takes
-        an array of angles and returns the corresponding energy value.
+        of `lmfit.model.ModelResult`, a numpy array containing the edge position at each
+        angle, or a callable function that takes an array of angles and returns the
+        corresponding energy value.
     shift_coords
-        Whether to shift the coordinates of the data array. Defaults to True.
+        If `True`, the coordinates of the output data will be changed so that the output
+        contains all the values of the original data. If `False`, the coordinates and
+        shape of the original data will be retained, and only the data will be shifted.
+        Defaults to `False`.
     plot
-        Whether to plot the original and corrected data arrays. Defaults to False.
+        Whether to plot the original and corrected data arrays. Defaults to `False`.
     plot_kw
-        Additional keyword arguments for the plot. Defaults to None.
+        Additional keyword arguments for the plot. Defaults to `None`.
     **shift_kwargs
-        Additional keyword arguments to `shift`.
+        Additional keyword arguments to `erlab.analysis.utilities.shift`.
 
     Returns
     -------
-    xarray.DataArray
+    corrected : xarray.DataArray
         The edge corrected data.
     """
     if plot_kw is None:
         plot_kw = {}
 
     if isinstance(modelresult, lmfit.model.ModelResult):
         if isinstance(modelresult.model, FermiEdge2dModel):
```

### Comparing `erlab-1.6.5/src/erlab/characterization/resistance.py` & `erlab-2.0.0/src/erlab/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/characterization/xrd.py` & `erlab-2.0.0/src/erlab/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/constants.py` & `erlab-2.0.0/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/interactive/__init__.py` & `erlab-2.0.0/src/erlab/interactive/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,17 +18,13 @@
    kspace
    masktool
    derivative
    utilities
 
 """
 
-__all__ = ["goldtool", "itool", "ktool", "dtool"]
-
-import importlib
+__all__ = ["dtool", "goldtool", "itool", "ktool"]
 
+from erlab.interactive.derivative import dtool
 from erlab.interactive.fermiedge import goldtool
 from erlab.interactive.imagetool import itool
 from erlab.interactive.kspace import ktool
-
-if importlib.util.find_spec("arpes"):
-    from erlab.interactive.derivative import dtool
```

### Comparing `erlab-1.6.5/src/erlab/interactive/bzplot.py` & `erlab-2.0.0/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/interactive/colors.py` & `erlab-2.0.0/src/erlab/interactive/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,17 @@
 
         self.setDefaultPadding(0)
         # self.hideButtons()
         self.setMenuEnabled(False)
         self.vb.setMouseEnabled(x=False, y=True)
 
         self._colorbar = pg.ImageItem(
-            np.linspace(0, 1, 4096).reshape((-1, 1)), axisOrder="row-major"
+            np.linspace(0, 1, 4096).reshape((-1, 1)),
+            axisOrder="row-major",
+            autoDownsample=False,
         )
         self.addItem(self._colorbar)
 
         self._span = pg.LinearRegionItem(
             (0, 1),
             "horizontal",
             swapMode="block",
```

### Comparing `erlab-1.6.5/src/erlab/interactive/curvefittingtool.py` & `erlab-2.0.0/src/erlab/interactive/curvefittingtool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 import sys
 
+import lmfit
 import pyqtgraph as pg
 import xarray as xr
 from qtpy import QtCore, QtWidgets
 
 from erlab.analysis.fit import MultiPeakModel
 from erlab.interactive.utilities import FittingParameterWidget, ParameterGroup
 
@@ -157,15 +158,15 @@
             self.param_widget.widgets["center"].setValue(pos.x())
             self.param_widget.widgets["height"].setValue(
                 self._start_height + self.mapToParent(ev.pos() - ev.buttonDownPos()).y()
             )
 
         elif QtCore.Qt.MouseButton.RightButton in ev.buttons():
             if ev.isStart():
-                self._start_width = self.param_widget.widgets["width"].value()
+                self._start_width = self.param_widgÏet.widgets["width"].value()
             ev.accept()
 
             val = self.mapToParent(ev.buttonDownPos() - ev.pos()).y()
             y0, _, y1, _ = self.boundingRect().getCoords()
             amount = val / abs(y1 - y0)
             self.param_widget.widgets["width"].setValue(self._start_width + amount)
         if ev.isFinish():
@@ -380,17 +381,21 @@
 
             curve.setData(x=self.xdata, y=model.func.eval_peak(i, self.xdata, **params))
             line.refresh_pos()
 
         self.modelplot.setData(x=self.xdata, y=model.eval(x=self.xdata, **params))
 
     def do_fit(self):
-        res = self.model.guess_fit(
-            self.data,
-            params=self.params_dict,
+        params = lmfit.create_params(**self.params_dict)
+        model = self.model
+        params = model.guess(self.data, self.data[self.data.dims[0]]).update(params)
+        res = self.model.fit(
+            self.ydata,
+            x=self.xdata,
+            params=params,
             method=self._params_init.values["Method"],
         )
         print(res.best_values)
         self.fitplot.setData(x=self.xdata, y=res.best_fit)
         self.set_params(res.best_values)
 
         self.result = res
@@ -610,17 +615,21 @@
 
             curve.setData(x=self.xdata, y=model.func.eval_peak(i, self.xdata, **params))
             line.refresh_pos()
 
         self.modelplot.setData(x=self.xdata, y=model.eval(x=self.xdata, **params))
 
     def do_fit(self):
-        res = self.model.guess_fit(
-            self.data,
-            params=self.params_dict,
+        params = lmfit.create_params(**self.params_dict)
+        model = self.model
+        params = model.guess(self.data, self.data[self.data.dims[0]]).update(params)
+        res = self.model.fit(
+            self.ydata,
+            x=self.xdata,
+            params=params,
             method=self._params_init.values["Method"],
         )
         print(res.best_values)
         self.fitplot.setData(x=self.xdata, y=res.best_fit)
         self.set_params(res.best_values)
 
         self.result = res
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `erlab-1.6.5/src/erlab/interactive/derivative.py` & `erlab-2.0.0/src/erlab/interactive/derivative.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,181 +1,18 @@
+__all__ = ["dtool"]
+
 import sys
+
 import numpy as np
 import pyqtgraph as pg
-
-from arpes.analysis.derivative import curvature, minimum_gradient
-from erlab.interactive.utilities import parse_data, AnalysisWidgetBase
-
 from qtpy import QtCore, QtWidgets
 from scipy.ndimage import gaussian_filter, uniform_filter
 
-# def move_mean_centered(a, window, min_count=None, axis=-1):
-#     w = (window - 1) // 2
-#     shift = w + 1
-#     if min_count is None:
-#         min_count = w + 1
-#     pad_width = [(0, 0)] * a.ndim
-#     pad_width[axis] = (0, shift)
-#     a = np.pad(a, pad_width, constant_values=np.nan)
-#     val = bn.move_mean(a, window, min_count=min_count, axis=axis)
-#     return val[(slice(None),) * (axis % a.ndim) + (slice(w, -1),)]
-
-
-# def move_mean_centered_multiaxis(a, window_list, min_count_list=None):
-#     w_list = [(window - 1) // 2 for window in window_list]
-#     pad_width = [(0, 0)] * a.ndim
-#     slicer = [
-#         slice(None),
-#     ] * a.ndim
-#     if min_count_list is None:
-#         min_count_list = [w + 1 for w in w_list]
-#     for axis in range(a.ndim):
-#         pad_width[axis] = (0, w_list[axis] + 1)
-#         slicer[axis] = slice(w_list[axis], -1)
-#     a = np.pad(a, pad_width, constant_values=np.nan)
-#     val = move_mean(
-#         a,
-#         numba.typed.List(window_list),
-#         numba.typed.List(min_count_list),
-#     )
-#     return val[tuple(slicer)]
-
-
-# def move_mean(a, window, min_count):
-#     if a.ndim == 3:
-#         return move_mean3d(a, window, min_count)
-#     elif a.ndim == 2:
-#         return move_mean2d(a, window, min_count)
-#     else:
-#         raise NotImplementedError
-
-
-# pg.setConfigOption('useNumba', True)
-
-__all__ = ["dtool"]
-
-
-# def boxcarfilt2(array, window_list, min_count_list=None):
-#     return move_mean_centered_multiaxis(array, window_list, min_count_list)
-
-
-def laplacian_O3(f, *varargs):
-    """
-    Third order accurate, 5-point formula. Not really laplacian, but second derivative
-    along each axis. Sum the outputs to get laplacian.
-    """
-    N = len(f.shape)  # number of dimensions
-    n = len(varargs)
-    if n == 0:
-        dx = [1.0] * N
-    elif n == 1:
-        dx = [varargs[0]] * N
-    elif n == N:
-        dx = list(varargs)
-    else:
-        raise SyntaxError("invalid number of arguments")
-
-    # use central differences on interior and first differences on endpoints
-
-    # print dx
-    outvals = []
-
-    # create slice objects --- initially all are [:, :, ..., :]
-    slice0 = [slice(None)] * N
-    slice1 = [slice(None)] * N
-    slice2 = [slice(None)] * N
-    slice3 = [slice(None)] * N
-    slice4 = [slice(None)] * N
-
-    otype = f.dtype.char
-    if otype not in ["f", "d", "F", "D"]:
-        otype = "d"
-
-    for axis in range(N):
-        # select out appropriate parts for this dimension
-        out = np.zeros(f.shape, f.dtype.char)
-
-        # http://www.sitmo.com/eq/262 (3rd order accurate)
-        slice0[axis] = slice(2, -2)
-        slice1[axis] = slice(None, -4)
-        slice2[axis] = slice(1, -3)
-        slice3[axis] = slice(3, -1)
-        slice4[axis] = slice(4, None)
-        # 1D equivalent -- out[2:-2] = (-f[:-4] + 16*f[1:-3] + -30*f[2:-2] +
-        # 16*f[3:-1] - f[4:])/12.0
-        out[slice0] = (
-            -f[slice1]
-            + 16.0 * f[slice2]
-            - 30.0 * f[slice0]
-            + 16.0 * f[slice3]
-            - f[slice4]
-        ) / 12.0
-
-        # http://www.sitmo.com/eq/260 (2nd order accurate; there's also a 3rd
-        # order accurate that requires 5 points)
-        slice0[axis] = slice(None, 2)
-        slice1[axis] = slice(3, 5)
-        slice2[axis] = slice(2, 4)
-        slice3[axis] = slice(1, 3)
-        # 1D equivalent -- out[0:2] = 2*f[0:2] - 5*f[1:3] + 4*f[2:4] - f[3:5]
-        out[slice0] = 2.0 * f[slice0] - 5.0 * f[slice3] + 4.0 * f[slice2] - f[slice1]
-
-        slice0[axis] = slice(-2, None)
-        slice1[axis] = slice(-5, -3)
-        slice2[axis] = slice(-4, -2)
-        slice3[axis] = slice(-3, -1)
-        # 1D equivalent -- out[0:2] = 2*f[0:2] - 5*f[1:3] + 4*f[2:4] - f[3:5]
-        out[slice0] = 2.0 * f[slice0] - 5.0 * f[slice3] + 4.0 * f[slice2] - f[slice1]
-
-        # divide by step size
-        axis_dx = dx[axis]
-        outvals.append(out / (axis_dx * axis_dx))
-
-        # reset the slice object in this dimension to ":"
-        slice0[axis] = slice(None)
-        slice1[axis] = slice(None)
-        slice2[axis] = slice(None)
-        slice3[axis] = slice(None)
-        slice4[axis] = slice(None)
-
-    if N == 1:
-        return outvals[0]
-    else:
-        return outvals
-
-
-class NoiseToolNew(AnalysisWidgetBase):
-    def __init__(self, data, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.set_input(data)
-
-    # def get_smoothfunc(self, amount, num, method="boxcar"):
-    #     if method == "boxcar":
-    #         def func(data):
-    #             out = data.copy(deep=True)
-    #             vals = data.values
-    #             for _ in range(num):
-    #                 vals = uniform_filter(
-    #                     vals,
-    #                     amount,
-    #                     mode="constant",
-    #                     origin=(0, 0),
-    #                 )
-    #             out.values = vals
-    #             return out
-    #     elif method == "gaussian":
-    #         def func(data):
-    #             out = data.copy(deep=True)
-    #             vals = data.values
-    #             sigma = [(amount[0] - 1) / 3, (amount[1] - 1) / 3]
-    #             for _ in range(num):
-    #                 vals = gaussian_filter(vals, sigma=sigma)
-    #             out.values = vals
-    #             return out
-    #     return func
+from erlab.analysis.image import curvature, minimum_gradient
+from erlab.interactive.utilities import parse_data
 
 
 class DerivativeTool(QtWidgets.QMainWindow):
     def __init__(self, data=None, *args, **kwargs):
         super().__init__()
 
         self._main = QtWidgets.QWidget()
@@ -269,25 +106,34 @@
         self._deriv_axis_combo = QtWidgets.QComboBox(self._deriv_group)
         self._deriv_axis_combo.addItems(["x", "y"])
         deriv_layout.addWidget(self._deriv_axis_combo, 0, 0)
 
         self._curv_group = QtWidgets.QGroupBox("Curvature")
         curv_layout = QtWidgets.QGridLayout(self._curv_group)
         self._curv_alpha_spin = QtWidgets.QDoubleSpinBox(self._curv_group)
-        self._curv_alpha_spin.setRange(-30, 30)
-        self._curv_alpha_spin.setValue(0)
-        self._curv_alpha_spin.setSingleStep(0.05)
+        self._curv_alpha_spin.setRange(0, 100)
+        self._curv_alpha_spin.setDecimals(4)
+        self._curv_alpha_spin.setValue(1.0)
+        self._curv_alpha_spin.setSingleStep(0.001)
+        self._curv_factor_spin = QtWidgets.QDoubleSpinBox(self._curv_group)
+        self._curv_factor_spin.setRange(-1, 1)
+        self._curv_factor_spin.setDecimals(4)
+        self._curv_factor_spin.setValue(1.0)
+        self._curv_factor_spin.setSingleStep(0.0001)
         curv_layout.addWidget(self._curv_alpha_spin, 0, 0)
+        curv_layout.addWidget(self._curv_factor_spin, 1, 0)
 
         self._mingrad_group = QtWidgets.QGroupBox("Minimum Gradient")
         mingrad_layout = QtWidgets.QGridLayout(self._mingrad_group)
-        self._mingrad_delta_spin = QtWidgets.QSpinBox(self._mingrad_group)
-        self._mingrad_delta_spin.setRange(1, 100)
-        self._mingrad_delta_spin.setValue(1)
-        mingrad_layout.addWidget(self._mingrad_delta_spin, 0, 0)
+        self._mingrad_btn = QtWidgets.QPushButton("Calculate")
+        # self._mingrad_delta_spin = QtWidgets.QSpinBox(self._mingrad_group)
+        # self._mingrad_delta_spin.setRange(1, 100)
+        # self._mingrad_delta_spin.setValue(1)
+        # mingrad_layout.addWidget(self._mingrad_delta_spin, 0, 0)
+        mingrad_layout.addWidget(self._mingrad_btn, 0, 0)
 
         self._deriv_tab = QtWidgets.QWidget()
         deriv_content = QtWidgets.QGridLayout(self._deriv_tab)
         deriv_content.addWidget(self._smooth2_group, 0, 0)
         deriv_content.addWidget(self._deriv_group, 0, 1)
 
         self._curv_tab = QtWidgets.QWidget()
@@ -327,20 +173,20 @@
             lambda val, ax=0: self.smooth_data(ax, val)
         )
         self._smooth_n_spin.valueChanged.connect(self.set_smooth_num)
         self._smooth2_x_spin.valueChanged.connect(lambda: self.deriv_data())
         self._smooth2_y_spin.valueChanged.connect(lambda: self.deriv_data())
         self._smooth2_n_spin.valueChanged.connect(self.set_smooth2_num)
         self._deriv_axis_combo.currentTextChanged.connect(self.deriv_data)
-        self._curv_alpha_spin.valueChanged.connect(
-            lambda beta: self.curv_data(beta=beta)
-        )
-        self._mingrad_delta_spin.valueChanged.connect(
-            lambda delta: self.mingrad_data(delta=delta)
-        )
+        self._curv_alpha_spin.valueChanged.connect(self.curv_data)
+        self._curv_factor_spin.valueChanged.connect(self.curv_data)
+        self._mingrad_btn.clicked.connect(lambda: self.mingrad_data())
+        # self._mingrad_delta_spin.valueChanged.connect(
+        #     lambda delta: self.mingrad_data(delta=delta)
+        # )
         for s in self._color_range_spin:
             s.valueChanged.connect(self._result_update_lims)
 
     def get_cutoff(self, data, cutoff=None):
         q3, q1 = np.percentile(data, [75, 25])
         ql = q1 - 1.5 * (q3 - q1)
         qu = q3 + 1.5 * (q3 - q1)
@@ -381,31 +227,35 @@
         self.smooth_num = n
         self.smooth_data()
 
     def set_smooth2_num(self, n):
         self.smooth2_num = n
         self.deriv_data()
 
-    def mingrad_data(self, delta=1):
+    # def mingrad_data(self, delta=1):
+    def mingrad_data(self):
         self.use_curv = False
         self.use_mingrad = True
         self.use_deriv = False
         # self.data_s_d = self.data_s.copy(deep=True)
-        self.data_s_d = -minimum_gradient(self.data_s, delta=delta)
+        # self.data_s_d = -minimum_gradient(self.data_s, delta=delta)
+        self.data_s_d = -minimum_gradient(self.data_s)
         self._result_update_lims()
 
-    def curv_data(self, alpha=1, beta=None):
+    def curv_data(self):
         self.use_curv = True
         self.use_deriv = False
         self.use_mingrad = False
-        if beta is None:
-            beta = self._curv_alpha_spin.value()
-        self.data_s_d = self.data_s.copy(deep=True)
-        self.data_s_d.values = curvature(
-            self.data_s / self.data_s.max(), alpha=alpha, beta=beta, values=True
+
+        # self.data_s_d = self.data_s.copy(deep=True)
+        self.data_s_d = curvature(
+            # self.data_s / self.data_s.max(), alpha=alpha, beta=beta, values=True
+            self.data_s,
+            a0=self._curv_alpha_spin.value(),
+            factor=self._curv_factor_spin.value(),
         )
         # m = self.data_s_d.max()
         # self.data_s_d /= m
         self._result_update_lims()
 
     def deriv_data(self, axis=None):
         self.use_curv = False
@@ -502,15 +352,15 @@
     app.raise_()
     qapp.exec()
 
 
 if __name__ == "__main__":
     import erlab.io
 
-    gkmk_cvs = erlab.io.load_als_bl4(
+    gkmk_cvs = erlab.io.merlin.load(
         "/Users/khan/Documents/ERLab/CsV3Sb5/2021_Dec_ALS_CV3Sb5/211217 ALS BL4/csvtisb1/f_003.pxt"
     )
     alpha_new = np.linspace(gkmk_cvs.alpha[0], gkmk_cvs.alpha[-1], 1000)
     eV_new = np.linspace(gkmk_cvs.eV[0], gkmk_cvs.eV[-1], 2000)
     gkmk_cvs = gkmk_cvs.interp(alpha=alpha_new, eV=eV_new)
     gkmk_cvs = gkmk_cvs.sel(
         alpha=slice(*np.rad2deg((-0.25, 0.25))), eV=slice(-1.25, 0.15)
```

### Comparing `erlab-1.6.5/src/erlab/interactive/exampledata.py` & `erlab-2.0.0/src/erlab/interactive/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/interactive/fermiedge.py` & `erlab-2.0.0/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.0.0/src/erlab/interactive/imagetool/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/interactive/imagetool/controls.py` & `erlab-2.0.0/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/interactive/imagetool/core.py` & `erlab-2.0.0/src/erlab/interactive/imagetool/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from __future__ import annotations
 
 __all__ = ["ImageSlicerArea"]
 
 import collections
 import functools
-import gc
 import inspect
 import os
 import time
 import weakref
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
@@ -21,15 +20,15 @@
 
 from erlab.interactive.colors import (
     BetterColorBarItem,
     BetterImageItem,
     pg_colormap_powernorm,
 )
 from erlab.interactive.imagetool.slicer import ArraySlicer
-from erlab.interactive.utilities import BetterAxisItem
+from erlab.interactive.utilities import BetterAxisItem, copy_to_clipboard
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Iterable, Sequence
 
     from pyqtgraph.graphicsItems.ViewBox import ViewBoxMenu
     from pyqtgraph.GraphicsScene import mouseEvents
 
@@ -448,15 +447,14 @@
 
     def on_close(self):
         self.array_slicer.clear_cache()
         self.data.close()
         if hasattr(self, "_data"):
             self._data.close()
             del self._data
-        gc.collect()
 
     def connect_axes_signals(self):
         for ax in self.axes:
             ax.connect_signals()
 
     def disconnect_axes_signals(self):
         for ax in self.axes:
@@ -1148,14 +1146,17 @@
         )
         for act in ["Transforms", "Downsample", "Average", "Alpha", "Points"]:
             self.setContextMenuActionVisible(act, False)
 
         save_action = self.vb.menu.addAction("Save data as HDF5")
         save_action.triggered.connect(lambda: self.save_current_data())
 
+        copy_code_action = self.vb.menu.addAction("Copy selection code")
+        copy_code_action.triggered.connect(self.copy_selection_code)
+
         for i in (0, 1):
             self.getViewBoxMenu().ctrl[i].linkCombo.setVisible(False)
             self.getViewBoxMenu().ctrl[i].label.setVisible(False)
         self.getViewBox().setCursor(QtGui.QCursor(QtCore.Qt.CursorShape.CrossCursor))
 
         self.slicer_area = slicer_area
         self._display_axis = display_axis
@@ -1304,15 +1305,15 @@
             clr_span_edge,
         ) = self.slicer_area.gen_cursor_colors(new_cursor)
 
         if self.is_image:
             item = self.image_cls(
                 self,
                 cursor=new_cursor,
-                autoDownsample=True,
+                autoDownsample=False,
                 axisOrder="row-major",
                 **self._item_kw,
             )
             if self.slicer_area.color_locked:
                 item.setLevels(self.array_slicer.limits, update=True)
         else:
             item = self.plotdata_cls(
@@ -1505,14 +1506,22 @@
         import erlab.io
 
         erlab.io.save_as_hdf5(
             self.slicer_data_items[self.slicer_area.current_cursor].sliced_data,
             fileName,
         )
 
+    @QtCore.Slot()
+    def copy_selection_code(self):
+        copy_to_clipboard(
+            self.array_slicer.qsel_code(
+                self.slicer_area.current_cursor, self.display_axis
+            )
+        )
+
     @property
     def display_axis(self) -> tuple[int, ...]:
         return self._display_axis
 
     @display_axis.setter
     def display_axis(self, value: tuple[int, ...]):
         self._display_axis = value
```

### Comparing `erlab-1.6.5/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.0.0/src/erlab/interactive/imagetool/slicer.py`

 * *Files 3% similar despite different names*

```diff
@@ -572,26 +572,89 @@
         if uniform or (axis not in self._nonuniform_axes):
             return _index_of_value(
                 axis, value, self.lims_uniform, self.incs_uniform, self._obj.shape
             )
         else:
             return _index_of_value_nonuniform(self.coords[axis], value)
 
-    def gen_selection_code(self, cursor: int, disp: Sequence[int]) -> str:
+    def isel_args(
+        self, cursor: int, disp: Sequence[int], int_if_one: bool = False
+    ) -> dict[str, slice | int]:
         axis = sorted(set(range(self._obj.ndim)) - set(disp))
-        slice_dict = {
-            self._obj.dims[ax]: self._bin_slice(cursor, ax, int_if_one=True)
-            for ax in axis
+        return {
+            self._obj.dims[ax]: self._bin_slice(cursor, ax, int_if_one) for ax in axis
         }
-        return f".isel(**{slice_dict!s}).squeeze()"
+
+    def qsel_args(self, cursor: int, disp: Sequence[int]) -> dict:
+        out: dict[str, float] = {}
+        binned = self.get_binned(cursor)
+
+        for dim, selector in self.isel_args(cursor, disp, int_if_one=True).items():
+            inc = self.incs[self._obj.dims.index(dim)]
+            order = int(-np.floor(np.log10(inc)) + 1)
+
+            if binned[self._obj.dims.index(dim)]:
+                coord = self._obj[dim][selector].values
+
+                out[dim] = np.round(coord.mean(), order)
+                width = np.round(abs(coord[-1] - coord[0]) + inc, order)
+
+                if not np.allclose(
+                    self._obj[dim]
+                    .sel({dim: slice(out[dim] - width / 2, out[dim] + width / 2)})
+                    .values,
+                    coord,
+                ):
+                    raise ValueError(
+                        "Bin does not contain the same values as the original data."
+                    )
+
+                out[dim + "_width"] = width
+
+            else:
+                out[dim] = np.round(self._obj[dim].values[selector], order)
+
+        return out
+
+    def qsel_code(self, cursor: int, disp: Sequence[int]) -> str:
+        if self._nonuniform_axes:
+            # Has non-uniform axes, fallback to isel
+            return self.isel_code(cursor, disp)
+
+        try:
+            qsel_kw = self.qsel_args(cursor, disp)
+        except ValueError:
+            return self.isel_code(cursor, disp)
+
+        dict_repr: str = ""
+        for k, v in qsel_kw.items():
+            dict_repr += f"{k}={v!s}, "
+        dict_repr = dict_repr.rstrip(", ")
+        return f".qsel({dict_repr})"
+
+    def isel_code(self, cursor: int, disp: Sequence[int]) -> str:
+        dict_repr: str = ""
+        for k, v in self.isel_args(cursor, disp, int_if_one=True).items():
+            dict_repr += f"{k}={v!s}, "
+        dict_repr = dict_repr.rstrip(", ")
+        return f".isel({dict_repr})"
 
     def xslice(self, cursor: int, disp: Sequence[int]) -> xr.DataArray:
-        axis = sorted(set(range(self._obj.ndim)) - set(disp))
-        slices = {self._obj.dims[ax]: self._bin_slice(cursor, ax) for ax in axis}
-        return self._obj.isel(**slices).squeeze()
+        isel_kw: dict[str, slice] = self.isel_args(cursor, disp, int_if_one=False)
+        binned_coord_average: dict[str, xr.DataArray] = {
+            k: self._obj[k][isel_kw[k]].mean()
+            for k, v in zip(self._obj.dims, self.get_binned(cursor))
+            if v
+        }
+        return (
+            self._obj.isel(**isel_kw)
+            .squeeze()
+            .mean(binned_coord_average.keys())
+            .assign_coords(**binned_coord_average)
+        )
 
     @QtCore.Slot(int, tuple, result=np.ndarray)
     def slice_with_coord(
         self, cursor: int, disp: Sequence[int]
     ) -> tuple[
         tuple[np.float32, np.float32, np.float32, np.float32] | npt.NDArray[np.float32],
         npt.NDArray[np.float32] | np.float32,
```

### Comparing `erlab-1.6.5/src/erlab/interactive/kspace.py` & `erlab-2.0.0/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/interactive/ktool.ui` & `erlab-2.0.0/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/interactive/masktool.py` & `erlab-2.0.0/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/interactive/utilities.py` & `erlab-2.0.0/src/erlab/interactive/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/io/__init__.py` & `erlab-2.0.0/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/io/dataloader.py` & `erlab-2.0.0/src/erlab/io/dataloader.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/io/igor.py` & `erlab-2.0.0/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/io/plugins/__init__.py` & `erlab-2.0.0/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/io/plugins/da30.py` & `erlab-2.0.0/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/io/plugins/kriss.py` & `erlab-2.0.0/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/io/plugins/merlin.py` & `erlab-2.0.0/src/erlab/io/plugins/merlin.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/io/plugins/ssrl52.py` & `erlab-2.0.0/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/io/utilities.py` & `erlab-2.0.0/src/erlab/io/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/lattice.py` & `erlab-2.0.0/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/parallel.py` & `erlab-2.0.0/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.0.0/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.0.0/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.0.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.0.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.0.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.0.0/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.0.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.0.0/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.0.0/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.0.0/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/__init__.py` & `erlab-2.0.0/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/annotations.py` & `erlab-2.0.0/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/atoms.py` & `erlab-2.0.0/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/bz.py` & `erlab-2.0.0/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/colors.py` & `erlab-2.0.0/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/erplot.py` & `erlab-2.0.0/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/general.py` & `erlab-2.0.0/src/erlab/plotting/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,14 +412,15 @@
     lnorm: mcolors.Normalize | None = None,
     cnorm: mcolors.Normalize | None = None,
     background: Sequence[float] | None = None,
     colorbar: bool = True,
     cax: matplotlib.axes.Axes | None = None,
     colorbar_kw: dict | None = None,
     imshow_kw: dict | None = None,
+    N: int = 256,
     **indexers_kwargs: dict,
 ):
     if lnorm is None:
         lnorm = plt.Normalize()
     else:
         lnorm = copy.deepcopy(lnorm)
     if cnorm is None:
@@ -452,15 +453,21 @@
         if not np.iterable(ylim):
             ylim = (-ylim, ylim)
         sel_kw[larr.dims[0]] = slice(*ylim)
     larr = larr.sel(**sel_kw)
     carr = carr.sel(**sel_kw)
 
     cmap_img, img = gen_2d_colormap(
-        larr.values, carr.values, cmap, lnorm=lnorm, cnorm=cnorm, background=background
+        larr.values,
+        carr.values,
+        cmap,
+        lnorm=lnorm,
+        cnorm=cnorm,
+        background=background,
+        N=N,
     )
 
     if colorbar:
         if cax is None:
             colorbar_kw.setdefault("aspect", 2)
             colorbar_kw.setdefault("anchor", (0, 1))
             colorbar_kw.setdefault("panchor", (0, 1))
```

### Comparing `erlab-1.6.5/src/erlab/plotting/plot3d.py` & `erlab-2.0.0/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.0.0/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.0.0/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.0.0/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.0.0/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.0.0/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.0.0/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/src/erlab.egg-info/PKG-INFO` & `erlab-2.0.0/src/erlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 1.6.5
+Version: 2.0.0
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,34 +690,34 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.22.0
-Requires-Dist: numba>=0.56.2
-Requires-Dist: numbagg
-Requires-Dist: numba-progress
-Requires-Dist: joblib
-Requires-Dist: scipy>=1.8.0
-Requires-Dist: lmfit>=1.2.0
-Requires-Dist: uncertainties>=3.0.1
+Requires-Dist: h5netcdf>=1.2.0
+Requires-Dist: igor2>=0.5.6
 Requires-Dist: iminuit>=2.25.2
+Requires-Dist: joblib>=1.3.2
+Requires-Dist: lmfit>=1.2.0
 Requires-Dist: matplotlib>=3.8.0
-Requires-Dist: xarray
-Requires-Dist: h5netcdf
-Requires-Dist: varname
-Requires-Dist: tqdm
-Requires-Dist: pyperclip
-Requires-Dist: qtpy
+Requires-Dist: numba-progress>=1.0.0
+Requires-Dist: numba>=0.59.0
+Requires-Dist: numbagg>=0.8.1
+Requires-Dist: numpy>=1.26.0
+Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: pyqtgraph>=0.13.1
-Requires-Dist: qtawesome
-Requires-Dist: superqt
-Requires-Dist: importlib-metadata; python_version >= "3.11"
+Requires-Dist: qtawesome>=1.3.1
+Requires-Dist: qtpy>=2.4.1
+Requires-Dist: scipy>=1.12.0
+Requires-Dist: superqt>=0.6.2
+Requires-Dist: tqdm>=4.66.2
+Requires-Dist: uncertainties>=3.0.1
+Requires-Dist: varname>=0.13.0
+Requires-Dist: xarray>=2024.02.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # ERLabPy
```

### Comparing `erlab-1.6.5/src/erlab.egg-info/SOURCES.txt` & `erlab-2.0.0/src/erlab.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 src/erlab.egg-info/SOURCES.txt
 src/erlab.egg-info/dependency_links.txt
 src/erlab.egg-info/requires.txt
 src/erlab.egg-info/top_level.txt
 src/erlab/analysis/__init__.py
 src/erlab/analysis/correlation.py
 src/erlab/analysis/gold.py
+src/erlab/analysis/image.py
 src/erlab/analysis/interpolate.py
 src/erlab/analysis/kspace.py
 src/erlab/analysis/transform.py
 src/erlab/analysis/utilities.py
 src/erlab/analysis/fit/__init__.py
 src/erlab/analysis/fit/minuit.py
 src/erlab/analysis/fit/models.py
@@ -124,10 +125,17 @@
 src/erlab/plotting/IgorCT/morgenstemning.ibw
 src/erlab/plotting/stylelib/fira.mplstyle
 src/erlab/plotting/stylelib/firalight.mplstyle
 src/erlab/plotting/stylelib/khan.mplstyle
 src/erlab/plotting/stylelib/nature.mplstyle
 src/erlab/plotting/stylelib/poster.mplstyle
 src/erlab/plotting/stylelib/times.mplstyle
+templates/.macros.j2
+templates/.release_notes.md.j2
+templates/CHANGELOG.md.j2
 tests/test_fastbinning.py
+tests/test_fit_functions_dynamic.py
+tests/test_fit_functions_general.py
+tests/test_image.py
 tests/test_interpolate.py
-tests/test_kspace.py
+tests/test_kspace.py
+tests/test_utilities.py
```

### Comparing `erlab-1.6.5/tests/test_fastbinning.py` & `erlab-2.0.0/tests/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/tests/test_interpolate.py` & `erlab-2.0.0/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.5/tests/test_kspace.py` & `erlab-2.0.0/tests/test_kspace.py`

 * *Files identical despite different names*

