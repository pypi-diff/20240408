# Comparing `tmp/adani-1.0.1.tar.gz` & `tmp/adani-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adani-1.0.1.tar", last modified: Wed Apr  3 12:25:15 2024, max compression
+gzip compressed data, was "adani-1.0.2.tar", last modified: Mon Apr  8 16:54:31 2024, max compression
```

## Comparing `adani-1.0.1.tar` & `adani-1.0.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.014588 adani-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-03 12:25:07.000000 adani-1.0.1/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 12:25:07.000000 adani-1.0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:14.994588 adani-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:14.998588 adani-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-03 12:25:07.000000 adani-1.0.1/.github/workflows/pip.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-03 12:25:07.000000 adani-1.0.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-03 12:25:07.000000 adani-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-03 12:25:07.000000 adani-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-03 12:25:07.000000 adani-1.0.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 12:25:07.000000 adani-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-03 12:25:15.014588 adani-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-03 12:25:07.000000 adani-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:14.998588 adani-1.0.1/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-03 12:25:07.000000 adani-1.0.1/bin/adani-config.in
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-03 12:25:07.000000 adani-1.0.1/bin/adani.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.002588 adani-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)  2182791 2024-04-03 12:25:07.000000 adani-1.0.1/docs/Tesi_Laurenti.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   150134 2024-04-03 12:25:07.000000 adani-1.0.1/docs/approximation_smallx_nll.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    21151 2024-04-03 12:25:07.000000 adani-1.0.1/docs/approximation_smallx_nll.tex
--rw-r--r--   0 runner    (1001) docker     (127)    98460 2024-04-03 12:25:07.000000 adani-1.0.1/docs/montecarlointegration.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-03 12:25:07.000000 adani-1.0.1/docs/montecarlointegration.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.002588 adani-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-03 12:25:07.000000 adani-1.0.1/examples/test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-03 12:25:07.000000 adani-1.0.1/examples/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:14.994588 adani-1.0.1/inc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.002588 adani-1.0.1/inc/adani/
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/ApproximateCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/AsymptoticCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/CoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/Constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/Convolution.h
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/ExactCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/HighEnergyCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/HighScaleCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/HighScaleSplitLogs.h
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/MasslessCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/MatchingCondition.h
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/SpecialFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/SplittingFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/ThresholdCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/Value.h
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24502 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/adani.h
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 12:25:07.000000 adani-1.0.1/inc/adani/version.h.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.010588 adani-1.0.1/inc/adani.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-03 12:25:14.000000 adani-1.0.1/inc/adani.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-03 12:25:14.000000 adani-1.0.1/inc/adani.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:25:14.000000 adani-1.0.1/inc/adani.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 12:25:14.000000 adani-1.0.1/inc/adani.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.006588 adani-1.0.1/output/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-03 12:25:07.000000 adani-1.0.1/output/Q.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-03 12:25:07.000000 adani-1.0.1/output/output_grid.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-03 12:25:07.000000 adani-1.0.1/output/output_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.006588 adani-1.0.1/output/runcards/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 12:25:07.000000 adani-1.0.1/output/runcards/runcard_2g.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 12:25:07.000000 adani-1.0.1/output/runcards/runcard_2q.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 12:25:07.000000 adani-1.0.1/output/runcards/runcard_Lg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 12:25:07.000000 adani-1.0.1/output/runcards/runcard_Lq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-03 12:25:07.000000 adani-1.0.1/output/x.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 12:25:07.000000 adani-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.006588 adani-1.0.1/pywrap/
--rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-03 12:25:07.000000 adani-1.0.1/pywrap/pywrap.cc
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:25:15.014588 adani-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-03 12:25:07.000000 adani-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.010588 adani-1.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-04-03 12:25:07.000000 adani-1.0.1/src/ApproximateCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-03 12:25:07.000000 adani-1.0.1/src/AsymptoticCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-03 12:25:07.000000 adani-1.0.1/src/CoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)    21293 2024-04-03 12:25:07.000000 adani-1.0.1/src/Convolution.cc
--rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-03 12:25:07.000000 adani-1.0.1/src/ExactCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)    45692 2024-04-03 12:25:07.000000 adani-1.0.1/src/HighEnergyCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)   235403 2024-04-03 12:25:07.000000 adani-1.0.1/src/HighScaleCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)   215112 2024-04-03 12:25:07.000000 adani-1.0.1/src/HighScaleSplitLogs.cc
--rw-r--r--   0 runner    (1001) docker     (127)   210010 2024-04-03 12:25:07.000000 adani-1.0.1/src/MasslessCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)    46992 2024-04-03 12:25:07.000000 adani-1.0.1/src/MatchingCondition.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-04-03 12:25:07.000000 adani-1.0.1/src/SpecialFunctions.cc
--rw-r--r--   0 runner    (1001) docker     (127)    23952 2024-04-03 12:25:07.000000 adani-1.0.1/src/SplittingFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-04-03 12:25:07.000000 adani-1.0.1/src/ThresholdCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-03 12:25:07.000000 adani-1.0.1/src/Value.cc
--rw-r--r--   0 runner    (1001) docker     (127)   546646 2024-04-03 12:25:07.000000 adani-1.0.1/src/hplog.f
--rw-r--r--   0 runner    (1001) docker     (127)   747023 2024-04-03 12:25:07.000000 adani-1.0.1/src/hqcoef.f
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:25:15.010588 adani-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_approx_coeff_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_asy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_exact_coeff_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_high_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_highenergy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_massless.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_mc_integral.py
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_splitting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-03 12:25:07.000000 adani-1.0.1/tests/test_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-03 12:25:07.000000 adani-1.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.653259 adani-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-08 16:54:24.000000 adani-1.0.2/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 16:54:24.000000 adani-1.0.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.633259 adani-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.637259 adani-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-08 16:54:24.000000 adani-1.0.2/.github/workflows/pip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-08 16:54:24.000000 adani-1.0.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 16:54:24.000000 adani-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 16:54:24.000000 adani-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-08 16:54:24.000000 adani-1.0.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 16:54:24.000000 adani-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-08 16:54:31.653259 adani-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-08 16:54:24.000000 adani-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.637259 adani-1.0.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-08 16:54:24.000000 adani-1.0.2/bin/adani-config.in
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 16:54:24.000000 adani-1.0.2/bin/adani.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.641259 adani-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)  2182791 2024-04-08 16:54:24.000000 adani-1.0.2/docs/Tesi_Laurenti.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   150134 2024-04-08 16:54:24.000000 adani-1.0.2/docs/approximation_smallx_nll.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    21151 2024-04-08 16:54:24.000000 adani-1.0.2/docs/approximation_smallx_nll.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    98460 2024-04-08 16:54:24.000000 adani-1.0.2/docs/montecarlointegration.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-08 16:54:24.000000 adani-1.0.2/docs/montecarlointegration.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.641259 adani-1.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-08 16:54:24.000000 adani-1.0.2/examples/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-08 16:54:24.000000 adani-1.0.2/examples/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.637259 adani-1.0.2/inc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.645259 adani-1.0.2/inc/adani/
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/ApproximateCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/AsymptoticCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/CoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/Convolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/ExactCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11125 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/HighEnergyCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/HighScaleCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/HighScaleSplitLogs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/MasslessCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/MatchingCondition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/SpecialFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/SplittingFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/ThresholdCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/Value.h
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24502 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/adani.h
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.653259 adani-1.0.2/inc/adani.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-08 16:54:31.000000 adani-1.0.2/inc/adani.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-08 16:54:31.000000 adani-1.0.2/inc/adani.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:54:31.000000 adani-1.0.2/inc/adani.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 16:54:31.000000 adani-1.0.2/inc/adani.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.645259 adani-1.0.2/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-08 16:54:24.000000 adani-1.0.2/output/Q.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-08 16:54:24.000000 adani-1.0.2/output/output_grid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-08 16:54:24.000000 adani-1.0.2/output/output_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.649259 adani-1.0.2/output/runcards/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 16:54:24.000000 adani-1.0.2/output/runcards/runcard_2g.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 16:54:24.000000 adani-1.0.2/output/runcards/runcard_2q.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 16:54:24.000000 adani-1.0.2/output/runcards/runcard_Lg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 16:54:24.000000 adani-1.0.2/output/runcards/runcard_Lq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-08 16:54:24.000000 adani-1.0.2/output/x.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 16:54:24.000000 adani-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.649259 adani-1.0.2/pywrap/
+-rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-08 16:54:24.000000 adani-1.0.2/pywrap/pywrap.cc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:54:31.653259 adani-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-08 16:54:24.000000 adani-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.653259 adani-1.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-04-08 16:54:24.000000 adani-1.0.2/src/ApproximateCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-08 16:54:24.000000 adani-1.0.2/src/AsymptoticCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-08 16:54:24.000000 adani-1.0.2/src/CoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21313 2024-04-08 16:54:24.000000 adani-1.0.2/src/Convolution.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    22470 2024-04-08 16:54:24.000000 adani-1.0.2/src/ExactCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    45692 2024-04-08 16:54:24.000000 adani-1.0.2/src/HighEnergyCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   235407 2024-04-08 16:54:24.000000 adani-1.0.2/src/HighScaleCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   215112 2024-04-08 16:54:24.000000 adani-1.0.2/src/HighScaleSplitLogs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   210010 2024-04-08 16:54:24.000000 adani-1.0.2/src/MasslessCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    47102 2024-04-08 16:54:24.000000 adani-1.0.2/src/MatchingCondition.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-04-08 16:54:24.000000 adani-1.0.2/src/SpecialFunctions.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    23998 2024-04-08 16:54:24.000000 adani-1.0.2/src/SplittingFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-08 16:54:24.000000 adani-1.0.2/src/ThresholdCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-08 16:54:24.000000 adani-1.0.2/src/Value.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   546646 2024-04-08 16:54:24.000000 adani-1.0.2/src/hplog.f
+-rw-r--r--   0 runner    (1001) docker     (127)   747023 2024-04-08 16:54:24.000000 adani-1.0.2/src/hqcoef.f
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.653259 adani-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_approx_coeff_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_asy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_exact_coeff_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_high_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_highenergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_massless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_mc_integral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_splitting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-08 16:54:24.000000 adani-1.0.2/versioneer.py
```

### Comparing `adani-1.0.1/.clang-format` & `adani-1.0.2/.clang-format`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 IndentCaseBlocks: false
 IndentCaseLabels: false
 IndentExternBlock: Indent
 IndentGotoLabels: true
 IndentPPDirectives: None
 IndentRequiresClause: true
 IndentWidth:     4
-IndentWrappedFunctionNames: false
+IndentWrappedFunctionNames: true
 InsertBraces:    false
 InsertNewlineAtEOF: true
 InsertTrailingCommas: None
 IntegerLiteralSeparator:
   Binary:          0
   BinaryMinDigits: 0
   Decimal:         0
```

### Comparing `adani-1.0.1/.github/workflows/pip.yml` & `adani-1.0.2/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/.github/workflows/tests.yml` & `adani-1.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/CMakeLists.txt` & `adani-1.0.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/LICENSE` & `adani-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/PKG-INFO` & `adani-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adani
-Version: 1.0.1
+Version: 1.0.2
 Summary: Code computing approximate DIS N3LO coefficients
 Author: Niccolò Laurenti
 License: AGPLv3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adani Version: 1.0.1 Summary: Code computing
+Metadata-Version: 2.1 Name: adani Version: 1.0.2 Summary: Code computing
 approximate DIS N3LO coefficients Author: NiccolÃ² Laurenti License: AGPLv3
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE # ADANI ADANI (Approximate DIS At N3LO Implementation) is a C++ code
 that computes an approximation for the DIS coefficient functions at N3LO in
 heavy quark production, that are not fully known yet. ## Citation Policy When
 using this code please cite [![arXiv](https://img.shields.io/badge/arXiv-
 2401.12139-b31b1b?labelColor=222222)](https://arxiv.org/abs/2401.12139) ##
```

### Comparing `adani-1.0.1/README.md` & `adani-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/bin/adani-config.in` & `adani-1.0.2/bin/adani-config.in`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/docs/Tesi_Laurenti.pdf` & `adani-1.0.2/docs/Tesi_Laurenti.pdf`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/docs/approximation_smallx_nll.pdf` & `adani-1.0.2/docs/approximation_smallx_nll.pdf`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/docs/approximation_smallx_nll.tex` & `adani-1.0.2/docs/approximation_smallx_nll.tex`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/docs/montecarlointegration.pdf` & `adani-1.0.2/docs/montecarlointegration.pdf`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/docs/montecarlointegration.tex` & `adani-1.0.2/docs/montecarlointegration.tex`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/examples/test.cpp` & `adani-1.0.2/examples/test.cpp`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/examples/test.py` & `adani-1.0.2/examples/test.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/inc/adani/ApproximateCoefficientFunction.h` & `adani-1.0.2/inc/adani/ApproximateCoefficientFunction.h`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             const int &MCcalls = 25000
         );
         ~AbstractApproximate();
 
         double MuIndependentTerms(double x, double m2Q2, int nf) const override;
 
         Value
-        fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
+            fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
         double MuDependentTerms(
             double x, double m2Q2, double m2mu2, int nf
         ) const override;
 
     private:
         ExactCoefficientFunction *muterms_;
 };
@@ -92,16 +92,17 @@
             const bool &NLL = true, const string &highscale_version = "klmv",
             const double &abserr = 1e-3, const double &relerr = 1e-3,
             const int &dim = 1000, const bool &MCintegral = false,
             const int &MCcalls = 25000
         );
         ~ApproximateCoefficientFunction() override;
 
-        Value
-        MuIndependentTermsBand(double x, double m2Q2, int nf) const override;
+        Value MuIndependentTermsBand(
+            double x, double m2Q2, int nf
+        ) const override;
 
     private:
         ThresholdCoefficientFunction *threshold_;
         AsymptoticCoefficientFunction *asymptotic_;
 
         struct approximation_parameters approximation_;
         struct variation_parameters variation_;
@@ -124,16 +125,17 @@
             const string &highscale_version = "klmv", const bool &lowxi = false,
             const double &abserr = 1e-3, const double &relerr = 1e-3,
             const int &dim = 1000, const bool &MCintegral = false,
             const int &MCcalls = 25000
         );
         ~ApproximateCoefficientFunctionKLMV() override;
 
-        Value
-        MuIndependentTermsBand(double x, double m2Q2, int nf) const override;
+        Value MuIndependentTermsBand(
+            double x, double m2Q2, int nf
+        ) const override;
 
     private:
         ThresholdCoefficientFunction *threshold_;
         HighScaleCoefficientFunction *highscale_;
         HighEnergyCoefficientFunction *highenergy_;
 
         struct klmv_params params_A_;
```

### Comparing `adani-1.0.1/inc/adani/AsymptoticCoefficientFunction.h` & `adani-1.0.2/inc/adani/AsymptoticCoefficientFunction.h`

 * *Files 0% similar despite different names*

```diff
@@ -33,18 +33,18 @@
             const bool &NLL = true, const string &highscale_version = "klmv"
         );
         ~AsymptoticCoefficientFunction();
 
         double fx(double x, double m2Q2, double m2mu2, int nf) const override;
 
         Value
-        fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
+            fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
 
         vector<double>
-        AllVariations(double x, double m2Q2, double m2mu2, int nf) const;
+            AllVariations(double x, double m2Q2, double m2mu2, int nf) const;
 
     private:
         HighScaleCoefficientFunction *highscale_;
         PowerTermsCoefficientFunction *powerterms_;
 };
 
 #endif
```

### Comparing `adani-1.0.1/inc/adani/CoefficientFunction.h` & `adani-1.0.2/inc/adani/CoefficientFunction.h`

 * *Files 4% similar despite different names*

```diff
@@ -43,29 +43,30 @@
 
     public:
         CoefficientFunction(
             const int &order, const char &kind, const char &channel
         );
         CoefficientFunction(CoefficientFunction *coeff)
             : CoefficientFunction(
-                coeff->GetOrder(), coeff->GetKind(), coeff->GetChannel()
-            ){};
+                  coeff->GetOrder(), coeff->GetKind(), coeff->GetChannel()
+              ){};
 
         virtual ~CoefficientFunction() = 0;
 
         virtual double MuIndependentTerms(double x, double m2Q2, int nf) const;
         virtual double fx(double x, double m2Q2, double m2mu2, int nf) const;
         virtual double
-        MuDependentTerms(double x, double m2Q2, double m2mu2, int nf) const;
+            MuDependentTerms(double x, double m2Q2, double m2mu2, int nf) const;
         virtual Value
-        fxBand(double x, double m2Q2, double m2mu2, int nf) const = 0;
+            fxBand(double x, double m2Q2, double m2mu2, int nf) const = 0;
         virtual Value
-        MuIndependentTermsBand(double x, double m2Q2, int nf) const;
-        virtual Value
-        MuDependentTermsBand(double x, double m2Q2, double m2mu2, int nf) const;
+            MuIndependentTermsBand(double x, double m2Q2, int nf) const;
+        virtual Value MuDependentTermsBand(
+            double x, double m2Q2, double m2mu2, int nf
+        ) const;
 
         // get methods
         int GetOrder() const { return order_; };
         char GetKind() const { return kind_; };
         char GetChannel() const { return channel_; };
 
         // set methods
```

### Comparing `adani-1.0.1/inc/adani/Constants.h` & `adani-1.0.2/inc/adani/Constants.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/inc/adani/Convolution.h` & `adani-1.0.2/inc/adani/Convolution.h`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         double MuDependentTerms(
             double /*x*/, double /*m2Q2*/, double /*m2mu2*/, int /*nf*/
         ) const override {
             return 0.;
         };
         double fx(double x, double m2Q2, double m2mu2, int nf) const override;
         Value
-        fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
+            fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
 
     private:
         Convolution *conv_;
 };
 
 //==========================================================================================//
 //  class DoubleConvolution
```

### Comparing `adani-1.0.1/inc/adani/ExactCoefficientFunction.h` & `adani-1.0.2/inc/adani/ExactCoefficientFunction.h`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,29 @@
  *
  * =====================================================================================
  */
 
 #ifndef Exact_h
 #define Exact_h
 
+#include "adani/AsymptoticCoefficientFunction.h"
 #include "adani/CoefficientFunction.h"
 #include "adani/Convolution.h"
 #include "adani/SplittingFunction.h"
 
 #include <vector>
 
 //==========================================================================================//
+//  forward declaration of class ThresholdCoefficientFunction to avoid circular
+//  dependencies
+//------------------------------------------------------------------------------------------//
+
+class ThresholdCoefficientFunction;
+
+//==========================================================================================//
 //  class ExactCoefficientFunction
 //------------------------------------------------------------------------------------------//
 
 class ExactCoefficientFunction : public CoefficientFunction {
 
     public:
         ExactCoefficientFunction(
@@ -41,26 +49,29 @@
         double fx(double x, double m2Q2, double m2mu2, int nf) const override;
         double MuIndependentTerms(double x, double m2Q2, int nf) const override;
         double MuDependentTerms(
             double x, double m2Q2, double m2mu2, int nf
         ) const override;
 
         Value
-        fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
+            fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
 
         void SetFunctions();
 
     private:
         double (ExactCoefficientFunction::*mu_indep_)(
             double, double, int
         ) const;
         double (ExactCoefficientFunction::*mu_dep_)(
             double, double, double, int
         ) const;
 
+        AsymptoticCoefficientFunction *asy_;
+        ThresholdCoefficientFunction *thr_;
+
         std::vector<AbstractConvolution *> convolutions_lmu1_;
         std::vector<AbstractConvolution *> convolutions_lmu2_;
 
         ExactCoefficientFunction *gluon_as1_;
         ExactCoefficientFunction *gluon_as2_;
         ExactCoefficientFunction *quark_as2_;
 
@@ -104,17 +115,17 @@
 
         //==========================================================================================//
         //  Exact massive coefficient functions O(as^2):
         //  mu-dependent terms
         //------------------------------------------------------------------------------------------//
 
         double
-        C_ps2_MuDep(double x, double m2Q2, double m2mu2, int /*nf*/) const;
+            C_ps2_MuDep(double x, double m2Q2, double m2mu2, int /*nf*/) const;
         double
-        C_g2_MuDep(double x, double m2Q2, double m2mu2, int /*nf*/) const;
+            C_g2_MuDep(double x, double m2Q2, double m2mu2, int /*nf*/) const;
 
         //==========================================================================================//
         //  Exact massive coefficient functions O(as^3): terms
         //  proportional to log(mu^2/m^2)
         //------------------------------------------------------------------------------------------//
 
         double C_ps31(double x, double m2Q2, int nf) const;
```

### Comparing `adani-1.0.1/inc/adani/HighEnergyCoefficientFunction.h` & `adani-1.0.2/inc/adani/HighEnergyCoefficientFunction.h`

 * *Files 14% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         HighEnergyCoefficientFunction(
             const int &order, const char &kind, const char &channel,
             const bool &NLL = true
         );
         ~HighEnergyCoefficientFunction() override{};
 
         Value
-        fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
+            fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
 
         void SetFunctions();
 
     private:
         double (HighEnergyCoefficientFunction::*LL_)(
             double, double, double
         ) const;
@@ -102,43 +102,49 @@
         //------------------------------------------------------------------------------------------//
 
         double C2_g3_highenergyLL(double x, double m2Q2, double m2mu2) const;
         double CL_g3_highenergyLL(double x, double m2Q2, double m2mu2) const;
         double C2_ps3_highenergyLL(double x, double m2Q2, double m2mu2) const;
         double CL_ps3_highenergyLL(double x, double m2Q2, double m2mu2) const;
 
-        Value
-        C2_g3_highenergyNLL(double x, double m2Q2, double m2mu2, int nf) const;
-        Value
-        CL_g3_highenergyNLL(double x, double m2Q2, double m2mu2, int nf) const;
-        Value
-        C2_ps3_highenergyNLL(double x, double m2Q2, double m2mu2, int nf) const;
-        Value
-        CL_ps3_highenergyNLL(double x, double m2Q2, double m2mu2, int nf) const;
+        Value C2_g3_highenergyNLL(
+            double x, double m2Q2, double m2mu2, int nf
+        ) const;
+        Value CL_g3_highenergyNLL(
+            double x, double m2Q2, double m2mu2, int nf
+        ) const;
+        Value C2_ps3_highenergyNLL(
+            double x, double m2Q2, double m2mu2, int nf
+        ) const;
+        Value CL_ps3_highenergyNLL(
+            double x, double m2Q2, double m2mu2, int nf
+        ) const;
 
         //==========================================================================================//
         //                      High energy coefficient functions
         //                      O(as^3)
         //------------------------------------------------------------------------------------------//
 
         Value
-        C2_g3_highenergy(double x, double m2Q2, double m2mu2, int nf) const;
-        Value
-        C2_ps3_highenergy(double x, double m2Q2, double m2mu2, int nf) const;
-        Value
-        CL_g3_highenergy(double x, double m2Q2, double m2mu2, int nf) const;
+            C2_g3_highenergy(double x, double m2Q2, double m2mu2, int nf) const;
+        Value C2_ps3_highenergy(
+            double x, double m2Q2, double m2mu2, int nf
+        ) const;
         Value
-        CL_ps3_highenergy(double x, double m2Q2, double m2mu2, int nf) const;
+            CL_g3_highenergy(double x, double m2Q2, double m2mu2, int nf) const;
+        Value CL_ps3_highenergy(
+            double x, double m2Q2, double m2mu2, int nf
+        ) const;
 
         //==========================================================================================//
         //  Function needed to make LL_ and NLL_ point to a zero function
         //------------------------------------------------------------------------------------------//
 
-        double
-        ZeroFunction(double /*x*/, double /*m2Q2*/, double /*m2mu2*/) const {
+        double ZeroFunction(double /*x*/, double /*m2Q2*/, double /*m2mu2*/)
+            const {
             return 0.;
         };
         Value ZeroFunctionBand(
             double /*x*/, double /*m2Q2*/, double /*m2mu2*/, int /*nf*/
         ) const {
             return Value(0.);
         };
@@ -155,15 +161,15 @@
         HighEnergyHighScaleCoefficientFunction(
             const int &order, const char &kind, const char &channel,
             const bool &NLL = true
         );
         ~HighEnergyHighScaleCoefficientFunction() override{};
 
         Value
-        fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
+            fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
 
         void SetFunctions();
 
     private:
         double (HighEnergyHighScaleCoefficientFunction::*LL_)(
             double, double, double
         ) const;
@@ -172,32 +178,38 @@
         ) const;
 
         //==========================================================================================//
         //                      Q>>m limit of the high energy
         //                      coefficient functions O(as^2)
         //------------------------------------------------------------------------------------------//
 
-        double
-        C2_g2_highenergy_highscale(double x, double m2Q2, double m2mu2) const;
-        double
-        C2_ps2_highenergy_highscale(double x, double m2Q2, double m2mu2) const;
-        double
-        CL_g2_highenergy_highscale(double x, double m2Q2, double m2mu2) const;
-        double
-        CL_ps2_highenergy_highscale(double x, double m2Q2, double m2mu2) const;
+        double C2_g2_highenergy_highscale(
+            double x, double m2Q2, double m2mu2
+        ) const;
+        double C2_ps2_highenergy_highscale(
+            double x, double m2Q2, double m2mu2
+        ) const;
+        double CL_g2_highenergy_highscale(
+            double x, double m2Q2, double m2mu2
+        ) const;
+        double CL_ps2_highenergy_highscale(
+            double x, double m2Q2, double m2mu2
+        ) const;
 
         //==========================================================================================//
         //  Q>>m limit of the high energy coefficient functions
         //  O(as^3) at leading log
         //------------------------------------------------------------------------------------------//
 
-        double
-        C2_g3_highenergy_highscaleLL(double x, double m2Q2, double m2mu2) const;
-        double
-        CL_g3_highenergy_highscaleLL(double x, double m2Q2, double m2mu2) const;
+        double C2_g3_highenergy_highscaleLL(
+            double x, double m2Q2, double m2mu2
+        ) const;
+        double CL_g3_highenergy_highscaleLL(
+            double x, double m2Q2, double m2mu2
+        ) const;
         double C2_ps3_highenergy_highscaleLL(
             double x, double m2Q2, double m2mu2
         ) const;
         double CL_ps3_highenergy_highscaleLL(
             double x, double m2Q2, double m2mu2
         ) const;
 
@@ -232,16 +244,16 @@
             double x, double m2Q2, double m2mu2, int nf
         ) const;
 
         //==========================================================================================//
         //  Function needed to make LL_ and NLL_ point to a zero function
         //------------------------------------------------------------------------------------------//
 
-        double
-        ZeroFunction(double /*x*/, double /*m2Q2*/, double /*m2mu2*/) const {
+        double ZeroFunction(double /*x*/, double /*m2Q2*/, double /*m2mu2*/)
+            const {
             return 0.;
         };
         Value ZeroFunctionBand(
             double /*x*/, double /*m2Q2*/, double /*m2mu2*/, int /*nf*/
         ) const {
             return Value(0.);
         };
@@ -258,15 +270,15 @@
         PowerTermsCoefficientFunction(
             const int &order, const char &kind, const char &channel,
             const bool &NLL = true
         );
         ~PowerTermsCoefficientFunction() override;
 
         Value
-        fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
+            fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
 
     private:
         HighEnergyCoefficientFunction *highenergy_;
         HighEnergyHighScaleCoefficientFunction *highenergyhighscale_;
 };
 
 #endif
```

### Comparing `adani-1.0.1/inc/adani/HighScaleCoefficientFunction.h` & `adani-1.0.2/inc/adani/HighScaleCoefficientFunction.h`

 * *Files 8% similar despite different names*

```diff
@@ -41,18 +41,19 @@
             const string &version = "klmv"
         );
         ~HighScaleCoefficientFunction() override;
 
         double fx(double x, double m2Q2, double m2mu2, int nf) const override;
 
         Value
-        fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
+            fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
 
-        vector<double>
-        fxBand_NotOrdered(double x, double m2Q2, double m2mu2, int nf) const;
+        vector<double> fxBand_NotOrdered(
+            double x, double m2Q2, double m2mu2, int nf
+        ) const;
 
         void SetFunctions();
 
     private:
         Value (HighScaleCoefficientFunction::*fx_)(
             double, double, double, int
         ) const;
@@ -64,64 +65,64 @@
 
         //==========================================================================================//
         //                      High scale (Q^2 >> m^2) coefficient
         //                      functions O(as)
         //------------------------------------------------------------------------------------------//
 
         Value
-        C2_g1_highscale(double x, double m2Q2, double /*m2mu2*/, int /*nf*/)
-            const;
-        Value
-        CL_g1_highscale(double x, double /*m2Q2*/, double /*m2mu2*/, int /*nf*/)
-            const;
+            C2_g1_highscale(double x, double m2Q2, double /*m2mu2*/, int /*nf*/)
+                const;
+        Value CL_g1_highscale(
+            double x, double /*m2Q2*/, double /*m2mu2*/, int /*nf*/
+        ) const;
 
         double D2_g1_highscale(double x, double m2Q2) const;
         double DL_g1_highscale(double x) const;
 
         //==========================================================================================//
         //                      High scale (Q^2 >> m^2) coefficient
         //                      functions O(as^2)
         //------------------------------------------------------------------------------------------//
 
-        Value
-        C2_g2_highscale(double x, double m2Q2, double m2mu2, int /*nf*/) const;
-        Value
-        C2_ps2_highscale(double z, double m2Q2, double m2mu2, int /*nf*/) const;
+        Value C2_g2_highscale(double x, double m2Q2, double m2mu2, int /*nf*/)
+            const;
+        Value C2_ps2_highscale(double z, double m2Q2, double m2mu2, int /*nf*/)
+            const;
 
-        Value
-        CL_g2_highscale(double x, double m2Q2, double m2mu2, int /*nf*/) const;
-        Value
-        CL_ps2_highscale(double x, double m2Q2, double m2mu2, int /*nf*/) const;
+        Value CL_g2_highscale(double x, double m2Q2, double m2mu2, int /*nf*/)
+            const;
+        Value CL_ps2_highscale(double x, double m2Q2, double m2mu2, int /*nf*/)
+            const;
 
         double D2_g2_highscale(double x, double m2Q2, double m2mu2) const;
         double D2_ps2_highscale(double x, double m2Q2, double m2mu2) const;
 
         double DL_g2_highscale(double z, double m2Q2, double m2mu2) const;
         double DL_ps2_highscale(double z, double m2Q2, double m2mu2) const;
 
         //==========================================================================================//
         //                      High scale (Q^2 >> m^2) coefficient
         //                      functions O(as^3)
         //------------------------------------------------------------------------------------------//
 
         Value
-        C2_g3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
+            C2_g3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
         Value
-        C2_ps3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
+            C2_ps3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
 
         Value
-        CL_g3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
+            CL_g3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
         Value
-        CL_ps3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
+            CL_ps3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
 
         double
-        DL_g3_highscale(double z, double m2Q2, double m2mu2, int nf) const;
+            DL_g3_highscale(double z, double m2Q2, double m2mu2, int nf) const;
         double
-        DL_ps3_highscale(double z, double m2Q2, double m2mu2, int nf) const;
+            DL_ps3_highscale(double z, double m2Q2, double m2mu2, int nf) const;
 
         Value
-        D2_g3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
+            D2_g3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
         Value
-        D2_ps3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
+            D2_ps3_highscale(double x, double m2Q2, double m2mu2, int nf) const;
 };
 
 #endif
```

### Comparing `adani-1.0.1/inc/adani/HighScaleSplitLogs.h` & `adani-1.0.2/inc/adani/HighScaleSplitLogs.h`

 * *Files 0% similar despite different names*

```diff
@@ -38,21 +38,21 @@
         HighScaleSplitLogs(
             const int &order, const char &kind, const char &channel,
             const string &version = "klmv"
         );
         ~HighScaleSplitLogs() override;
 
         double
-        fx(double /*x*/, double /*m2Q2*/, double /*m2mu2*/,
-           int /*nf*/) const override;
+            fx(double /*x*/, double /*m2Q2*/, double /*m2mu2*/,
+               int /*nf*/) const override;
         double fx(double x, double m2Q2, int nf) const;
 
         Value
-        fxBand(double /*x*/, double /*m2Q2*/, double /*m2mu2*/, int /*nf*/)
-            const override;
+            fxBand(double /*x*/, double /*m2Q2*/, double /*m2mu2*/, int /*nf*/)
+                const override;
         Value fxBand(double x, double m2Q2, int nf) const;
 
         // division of the total result in the log terms
         double LL(double x, int nf) const { return (this->*LL_)(x, nf); }
         double NLL(double x, int nf) const { return (this->*NLL_)(x, nf); }
         double N2LL(double x, int nf) const { return (this->*N2LL_)(x, nf); }
         Value N3LL(double x, int nf) const { return (this->*N3LL_)(x, nf); }
```

### Comparing `adani-1.0.1/inc/adani/MasslessCoefficientFunction.h` & `adani-1.0.2/inc/adani/MasslessCoefficientFunction.h`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             const override;
         double MuIndependentTerms(double x, int nf) const;
         double MuDependentTerms(
             double /*x*/, double /*m2Q2*/, double /*m2mu2*/, int /*nf*/
         ) const override;
 
         Value
-        fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
+            fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
 
         void SetFunctions();
 
     private:
         double (MasslessCoefficientFunction::*mu_indep_)(double, int) const;
 
         //==========================================================================================//
```

### Comparing `adani-1.0.1/inc/adani/MatchingCondition.h` & `adani-1.0.2/inc/adani/MatchingCondition.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/inc/adani/SpecialFunctions.h` & `adani-1.0.2/inc/adani/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/inc/adani/SplittingFunction.h` & `adani-1.0.2/inc/adani/SplittingFunction.h`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             const int &order, const char &entry1, const char &entry2
         );
         ~SplittingFunction() override{};
 
         // overloading operators
         SplittingFunction operator*(const double &rhs) const;
         friend SplittingFunction
-        operator*(const double &lhs, const SplittingFunction &rhs);
+            operator*(const double &lhs, const SplittingFunction &rhs);
         SplittingFunction operator/(const double &rhs) const;
 
         // Components of the Splitting Function
         double Regular(double x, int nf) const override;
         double Singular(double x, int nf) const override;
         double Local(int nf) const override;
         // Integral from 0 to x of the Singular part
@@ -140,16 +140,17 @@
             const int &order1, const char &entry1, const char &entry2,
             const int &order2, const char &entry3, const char &entry4
         );
         ~ConvolutedSplittingFunctions() override{};
 
         // overloading operators
         ConvolutedSplittingFunctions operator*(const double &rhs) const;
-        friend ConvolutedSplittingFunctions
-        operator*(const double &lhs, const ConvolutedSplittingFunctions &rhs);
+        friend ConvolutedSplittingFunctions operator*(
+            const double &lhs, const ConvolutedSplittingFunctions &rhs
+        );
         ConvolutedSplittingFunctions operator/(const double &rhs) const;
 
         // Components of the Convoluted Splitting Function
         double Regular(double x, int nf) const override;
         double Singular(double /*x*/, int /*nf*/) const override { return 0.; };
         double Local(int /*nf*/) const override { return 0.; };
         // Integral from 0 to x of the Singular part
```

### Comparing `adani-1.0.1/inc/adani/ThresholdCoefficientFunction.h` & `adani-1.0.2/inc/adani/ThresholdCoefficientFunction.h`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,21 @@
  * =====================================================================================
  */
 
 #ifndef Threshold_h
 #define Threshold_h
 
 #include "adani/CoefficientFunction.h"
-#include "adani/ExactCoefficientFunction.h"
+
+//==========================================================================================//
+//  forward declaration of class ExactCoefficientFunction to avoid circular
+//  dependencies
+//------------------------------------------------------------------------------------------//
+
+class ExactCoefficientFunction;
 
 //==========================================================================================//
 //  class ThresholdCoefficientFunction
 //------------------------------------------------------------------------------------------//
 
 class ThresholdCoefficientFunction : public CoefficientFunction {
 
@@ -31,15 +37,15 @@
         ThresholdCoefficientFunction(
             const int &order, const char &kind, const char &channel
         );
         ~ThresholdCoefficientFunction() override;
 
         double fx(double x, double m2Q2, double m2mu2, int nf) const override;
         Value
-        fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
+            fxBand(double x, double m2Q2, double m2mu2, int nf) const override;
 
         double BetaIndependentTerms(double x, double m2Q2, double m2mu2) const;
 
         void SetFunctions();
 
     private:
         double (ThresholdCoefficientFunction::*fx_)(
@@ -50,43 +56,43 @@
 
         //==========================================================================================//
         //                      Threshold (s -> 4m^2) coefficient
         //                      functions O(as)
         //------------------------------------------------------------------------------------------//
 
         double
-        C2_g1_threshold(double x, double m2Q2, double /*m2mu2*/, int /*nf*/)
-            const;
+            C2_g1_threshold(double x, double m2Q2, double /*m2mu2*/, int /*nf*/)
+                const;
 
         //==========================================================================================//
         //                      Threshold (s -> 4m^2) coefficient
         //                      functions O(as^2)
         //------------------------------------------------------------------------------------------//
 
-        double
-        C2_g2_threshold(double x, double m2Q2, double m2mu2, int /*nf*/) const;
-        double
-        CL_g2_threshold(double x, double m2Q2, double m2mu2, int /*nf*/) const;
+        double C2_g2_threshold(double x, double m2Q2, double m2mu2, int /*nf*/)
+            const;
+        double CL_g2_threshold(double x, double m2Q2, double m2mu2, int /*nf*/)
+            const;
 
         double
-        threshold_expansion_g2(double x, double m2Q2, double m2mu2) const;
+            threshold_expansion_g2(double x, double m2Q2, double m2mu2) const;
         double threshold_expansion_g2_const(double m2Q2, double m2mu2) const;
 
         double C2_g2_threshold_const(double x, double m2Q2, double m2mu2) const;
         double CL_g2_threshold_const(double x, double m2Q2, double m2mu2) const;
 
         //==========================================================================================//
         //                      Threshold (s -> 4m^2) coefficient
         //                      functions O(as^3)
         //------------------------------------------------------------------------------------------//
 
         double
-        C2_g3_threshold(double x, double m2Q2, double m2mu2, int nf) const;
+            C2_g3_threshold(double x, double m2Q2, double m2mu2, int nf) const;
         double
-        CL_g3_threshold(double x, double m2Q2, double m2mu2, int nf) const;
+            CL_g3_threshold(double x, double m2Q2, double m2mu2, int nf) const;
 
         double threshold_expansion_g3(
             double x, double m2Q2, double m2mu2, int nf
         ) const;
         double threshold_expansion_g3_const(double m2Q2, double m2mu2) const;
 
         double C2_g3_threshold_const(double x, double m2Q2, double m2mu2) const;
```

### Comparing `adani-1.0.1/inc/adani/Value.h` & `adani-1.0.2/inc/adani/Value.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/inc/adani/_version.py` & `adani-1.0.2/inc/adani/_version.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/inc/adani/adani.h` & `adani-1.0.2/inc/adani/adani.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/inc/adani.egg-info/PKG-INFO` & `adani-1.0.2/inc/adani.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adani
-Version: 1.0.1
+Version: 1.0.2
 Summary: Code computing approximate DIS N3LO coefficients
 Author: Niccolò Laurenti
 License: AGPLv3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adani Version: 1.0.1 Summary: Code computing
+Metadata-Version: 2.1 Name: adani Version: 1.0.2 Summary: Code computing
 approximate DIS N3LO coefficients Author: NiccolÃ² Laurenti License: AGPLv3
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE # ADANI ADANI (Approximate DIS At N3LO Implementation) is a C++ code
 that computes an approximation for the DIS coefficient functions at N3LO in
 heavy quark production, that are not fully known yet. ## Citation Policy When
 using this code please cite [![arXiv](https://img.shields.io/badge/arXiv-
 2401.12139-b31b1b?labelColor=222222)](https://arxiv.org/abs/2401.12139) ##
```

### Comparing `adani-1.0.1/inc/adani.egg-info/SOURCES.txt` & `adani-1.0.2/inc/adani.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/output/Q.txt` & `adani-1.0.2/output/Q.txt`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/output/output_grid.cpp` & `adani-1.0.2/output/output_grid.cpp`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/output/output_grid.py` & `adani-1.0.2/output/output_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     if runcard["verbose"]:
         print(
             f"Computation of the grid for the coefficient function C{runcard['channel']} for m = {m} GeV, nf = {nf}, and µ/Q = {mufrac}"
         )
         print(f"Size of the grid (x,Q) = ({len(x_grid)},{len(Q_grid)})")
         print(
-            "This may take a while (depending on the number of threads you choose). In order to spend this time, I would suggest you this interesting view:"
+            "This may take a while (depending on the number of threads you chose). In order to spend this time, I would suggest you this interesting view:"
         )
         print("https://www.youtube.com/watch?v=53pG68KCUMI")
 
     start = time.perf_counter()
     res_vec = np.array(run(runcard["n_threads"], x_grid, Q_grid))
     if runcard["verbose"]:
         print("total running time: ", time.perf_counter() - start)
```

### Comparing `adani-1.0.1/output/x.txt` & `adani-1.0.2/output/x.txt`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/pywrap/pywrap.cc` & `adani-1.0.2/pywrap/pywrap.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/setup.py` & `adani-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/src/ApproximateCoefficientFunction.cc` & `adani-1.0.2/src/ApproximateCoefficientFunction.cc`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,17 @@
 
 //==========================================================================================//
 //  AbstractApproximate: destructor
 //------------------------------------------------------------------------------------------//
 
 AbstractApproximate::~AbstractApproximate() { delete muterms_; }
 
-double
-AbstractApproximate::MuIndependentTerms(double x, double m2Q2, int nf) const {
+double AbstractApproximate::MuIndependentTerms(
+    double x, double m2Q2, int nf
+) const {
     return MuIndependentTermsBand(x, m2Q2, nf).GetCentral();
 }
 
 //==========================================================================================//
 //  AbstractApproximate: band of the total result
 //------------------------------------------------------------------------------------------//
 
@@ -94,16 +95,16 @@
 
 ApproximateCoefficientFunction::ApproximateCoefficientFunction(
     const int &order, const char &kind, const char &channel, const bool &NLL,
     const string &highscale_version, const double &abserr, const double &relerr,
     const int &dim, const bool &MCintegral, const int &MCcalls
 )
     : AbstractApproximate(
-        order, kind, channel, abserr, relerr, dim, MCintegral, MCcalls
-    ) {
+          order, kind, channel, abserr, relerr, dim, MCintegral, MCcalls
+      ) {
 
     threshold_ = new ThresholdCoefficientFunction(order, kind, channel);
     asymptotic_ = new AsymptoticCoefficientFunction(
         order, kind, channel, NLL, highscale_version
     );
 
     if (order == 1) {
@@ -261,16 +262,16 @@
 ApproximateCoefficientFunctionKLMV::ApproximateCoefficientFunctionKLMV(
     const int &order, const char &kind, const char &channel,
     const string &highscale_version, const bool &lowxi, const double &abserr,
     const double &relerr, const int &dim, const bool &MCintegral,
     const int &MCcalls
 )
     : AbstractApproximate(
-        order, kind, channel, abserr, relerr, dim, MCintegral, MCcalls
-    ) {
+          order, kind, channel, abserr, relerr, dim, MCintegral, MCcalls
+      ) {
     if (GetOrder() == 1) {
         cout << "Error: KLMV approximation is not implemented at O(as)!"
              << endl;
         exit(-1);
     }
     if (GetKind() == 'L') {
         cout << "Error: KLMV approximation is not implemented for kind = 'L'!"
@@ -351,14 +352,19 @@
         Value he_nll = ApproximateNLL(x, m2Q2);
         res_A = ApproximationA(
             x, m2Q2, he_ll, he_nll.GetHigher(), hs[1], thr, thr_const, gamma, C
         );
         res_B = ApproximationB(
             x, m2Q2, he_ll, he_nll.GetLower(), hs[2], thr, thr_const, delta, D
         );
+    } else {
+        cout << "Error: ApproximateCoefficientFunctionKLMV is implemented only "
+                "for order = 2 or 3. Got "
+             << GetOrder() << endl;
+        exit(-1);
     }
 
     if (res_A > res_B)
         return Value(res_A, res_B);
     else
         return Value(res_B, res_A);
 }
```

### Comparing `adani-1.0.1/src/AsymptoticCoefficientFunction.cc` & `adani-1.0.2/src/AsymptoticCoefficientFunction.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/src/CoefficientFunction.cc` & `adani-1.0.2/src/CoefficientFunction.cc`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 //==========================================================================================//
 //  CoefficientFunction: set method for order: order = 1, 2, 3
 //------------------------------------------------------------------------------------------//
 
 void CoefficientFunction::SetOrder(const int &order) {
     // check order
     if (order < 1 || order > 3) {
-        cout << "Error: order must be 1,2 or 3. Got: " << order << endl;
+        cout << "Error: order must be 1, 2 or 3. Got: " << order << endl;
         exit(-1);
     }
     order_ = order;
 }
 
 //==========================================================================================//
 //  CoefficientFunction: set method for kind: kind = '2', 'L'
@@ -55,36 +55,37 @@
 void CoefficientFunction::SetChannel(const char &channel) {
     // check channel
     if (channel != 'g' && channel != 'q') {
         cout << "Error: channel must be g or q. Got: " << channel << endl;
         exit(-1);
     }
     if (channel_ == 'q' && order_ == 1) {
-        cout << "Error: quark coefficeint function at O(as) doesn't exist!"
+        cout << "Error: quark coefficient function at O(as) doesn't exist!"
              << endl;
         exit(-1);
     }
     channel_ = channel;
 }
 
 //==========================================================================================//
 //  CoefficientFunction: central value of fx
 //------------------------------------------------------------------------------------------//
 
 double
-CoefficientFunction::fx(double x, double m2Q2, double m2mu2, int nf) const {
+    CoefficientFunction::fx(double x, double m2Q2, double m2mu2, int nf) const {
     return fxBand(x, m2Q2, m2mu2, nf).GetCentral();
 }
 
 //==========================================================================================//
 //  CoefficientFunction: central value of mu independent terms
 //------------------------------------------------------------------------------------------//
 
-double
-CoefficientFunction::MuIndependentTerms(double x, double m2Q2, int nf) const {
+double CoefficientFunction::MuIndependentTerms(
+    double x, double m2Q2, int nf
+) const {
     return fx(x, m2Q2, 1., nf);
 }
 
 //==========================================================================================//
 //  CoefficientFunction: central value mu dependent terms
 //------------------------------------------------------------------------------------------//
```

### Comparing `adani-1.0.1/src/Convolution.cc` & `adani-1.0.2/src/Convolution.cc`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
 }
 
 //==========================================================================================//
 //  DoubleConvolution: integrand of the first regular part
 //------------------------------------------------------------------------------------------//
 
 double
-DoubleConvolution::regular1_integrand(double z[], size_t /*dim*/, void *p) {
+    DoubleConvolution::regular1_integrand(double z[], size_t /*dim*/, void *p) {
 
     struct function_params *params = (struct function_params *)p;
 
     double m2Q2 = (params->m2Q2);
     double x = (params->x);
     int nf = (params->nf);
 
@@ -362,15 +362,15 @@
 }
 
 //==========================================================================================//
 //  DoubleConvolution: integrand of the second regular part
 //------------------------------------------------------------------------------------------//
 
 double
-DoubleConvolution::regular2_integrand(double z[], size_t /*dim*/, void *p) {
+    DoubleConvolution::regular2_integrand(double z[], size_t /*dim*/, void *p) {
     struct function_params *params = (struct function_params *)p;
 
     double m2Q2 = (params->m2Q2);
     double x = (params->x);
     int nf = (params->nf);
 
     CoefficientFunction *coefffunc = (params->conv)->GetCoeffFunc();
@@ -463,16 +463,17 @@
     return regular1 + regular2 + regular3 + regular4;
 }
 
 //==========================================================================================//
 //  DoubleConvolution: integrand of the first singular part
 //------------------------------------------------------------------------------------------//
 
-double
-DoubleConvolution::singular1_integrand(double z[], size_t /*dim*/, void *p) {
+double DoubleConvolution::singular1_integrand(
+    double z[], size_t /*dim*/, void *p
+) {
 
     struct function_params *params = (struct function_params *)p;
 
     double m2Q2 = (params->m2Q2);
     double x = (params->x);
     int nf = (params->nf);
 
@@ -492,16 +493,17 @@
            * coefffunc->MuIndependentTerms(z2, m2Q2, nf) / z2;
 }
 
 //==========================================================================================//
 //  DoubleConvolution: integrand of the second singular part
 //------------------------------------------------------------------------------------------//
 
-double
-DoubleConvolution::singular2_integrand(double z[], size_t /*dim*/, void *p) {
+double DoubleConvolution::singular2_integrand(
+    double z[], size_t /*dim*/, void *p
+) {
 
     struct function_params *params = (struct function_params *)p;
 
     double m2Q2 = (params->m2Q2);
     double x = (params->x);
     int nf = (params->nf);
```

### Comparing `adani-1.0.1/src/ExactCoefficientFunction.cc` & `adani-1.0.2/src/ExactCoefficientFunction.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #include "adani/ExactCoefficientFunction.h"
 #include "adani/Constants.h"
 #include "adani/SpecialFunctions.h"
+#include "adani/ThresholdCoefficientFunction.h"
 
 #include <cmath>
 #include <iostream>
 
 using std::cout;
 using std::endl;
 
@@ -31,14 +32,22 @@
     Pqq0Pgq0_ = nullptr;
     Pgg1_ = nullptr;
     Pqg0_ = nullptr;
     Pgq0Pqg0_ = nullptr;
 
     delta_ = nullptr;
 
+    if (GetOrder() == 2) {
+        asy_ = new AsymptoticCoefficientFunction(order, kind, channel);
+        thr_ = new ThresholdCoefficientFunction(order, kind, channel);
+    } else {
+        asy_ = nullptr;
+        thr_ = nullptr;
+    }
+
     if (GetOrder() > 1) {
         gluon_as1_ = new ExactCoefficientFunction(1, GetKind(), 'g');
 
         Pgq0_ = new SplittingFunction(0, 'g', 'q');
         Pgg0_ = new SplittingFunction(0, 'g', 'g');
         delta_ = new Delta();
     }
@@ -142,14 +151,17 @@
     delete Pgg0Pgq0_;
     delete Pqq0Pgq0_;
     delete Pgg1_;
     delete Pqg0_;
     delete Pgq0Pqg0_;
 
     delete delta_;
+
+    delete asy_;
+    delete thr_;
 }
 
 //==========================================================================================//
 //  ExactCoefficientFunction: central value of the exact coefficient function
 //------------------------------------------------------------------------------------------//
 
 double ExactCoefficientFunction::fx(
@@ -258,15 +270,15 @@
 //==========================================================================================//
 //  Exact massive gluon coefficient functions for FL at O(as)
 //
 //  Eq. (2.9) from Ref. [arXiv:1205.5727]
 //------------------------------------------------------------------------------------------//
 
 double
-ExactCoefficientFunction::CL_g1(double x, double m2Q2, int /*nf*/) const {
+    ExactCoefficientFunction::CL_g1(double x, double m2Q2, int /*nf*/) const {
 
     double beta = sqrt(1. - 4. * m2Q2 * x / (1. - x));
     double x2 = x * x;
     double L = log((1. + beta) / (1. - beta));
 
     return 16. * TR * (x * (1. - x) * beta - 2. * x2 * m2Q2 * L);
 }
@@ -305,21 +317,33 @@
 //  at O(as^2)
 //
 //  Exact (but numerical) result from [arXiv:hep-ph/9411431].
 //  Taken from the Fortran code 'src/hqcoef.f'
 //------------------------------------------------------------------------------------------//
 
 double
-ExactCoefficientFunction::C2_ps20(double x, double m2Q2, int /*nf*/) const {
+    ExactCoefficientFunction::C2_ps20(double x, double m2Q2, int /*nf*/) const {
 
     double xi = 1. / m2Q2;
     double eta = 0.25 * xi * (1 - x) / x - 1.;
 
-    if (eta > 1e6 || eta < 1e-6 || xi < 1e-3 || xi > 1e5)
-        return 0.;
+    // using nf = nan since at O(as2) the coefficient functions don't depend on
+    // nf
+    int nf = static_cast<int>(nan(""));
+
+    if (eta < 1e-6)
+        return thr_->MuIndependentTerms(x, m2Q2, nf);
+    if (eta > 1e6 || xi > 1e5)
+        return asy_->MuIndependentTerms(x, m2Q2, nf);
+    if (xi < 1e-3) {
+        cout << "Error in ExactCoefficientFunction::C2_ps20 : max value of "
+                "m2Q2 is 1e3. Got "
+             << m2Q2 << endl;
+        exit(-1);
+    }
 
     return 16 * M_PI * xi * c2nloq_(&eta, &xi) / x;
 }
 
 //==========================================================================================//
 //  Exact massive quark coefficient functions at O(as^2):
 //  Term proportional to log(mu^2/m^2)
@@ -343,41 +367,65 @@
 //  at O(as)
 //
 //  Exact (but numerical) result from [arXiv:hep-ph/9411431].
 //  Taken from the Fortran code 'src/hqcoef.f'
 //------------------------------------------------------------------------------------------//
 
 double
-ExactCoefficientFunction::CL_ps20(double x, double m2Q2, int /*nf*/) const {
+    ExactCoefficientFunction::CL_ps20(double x, double m2Q2, int /*nf*/) const {
 
     double xi = 1. / m2Q2;
     double eta = 0.25 * xi * (1 - x) / x - 1.;
 
-    if (eta > 1e6 || eta < 1e-6 || xi < 1e-3 || xi > 1e5)
-        return 0.;
+    // using nf = nan since at O(as2) the coefficient functions don't depend on
+    // nf
+    int nf = static_cast<int>(nan(""));
+
+    if (eta < 1e-6)
+        return thr_->MuIndependentTerms(x, m2Q2, nf);
+    if (eta > 1e6 || xi > 1e5)
+        return asy_->MuIndependentTerms(x, m2Q2, nf);
+    if (xi < 1e-3) {
+        cout << "Error in ExactCoefficientFunction::CL_ps20 : max value of "
+                "m2Q2 is 1e3. Got "
+             << m2Q2 << endl;
+        exit(-1);
+    }
 
     return 16 * M_PI * xi * clnloq_(&eta, &xi) / x;
 }
 
 //==========================================================================================//
 //  mu independent part of the exact massive gluon coefficient functions for F2
 //  at O(as^2)
 //
 //  Exact (but numerical) result from [arXiv:hep-ph/9411431].
 //  Taken from the Fortran code 'src/hqcoef.f'
 //------------------------------------------------------------------------------------------//
 
 double
-ExactCoefficientFunction::C2_g20(double x, double m2Q2, int /*nf*/) const {
+    ExactCoefficientFunction::C2_g20(double x, double m2Q2, int /*nf*/) const {
 
     double xi = 1. / m2Q2;
     double eta = 0.25 * xi * (1 - x) / x - 1.;
 
-    if (eta > 1e6 || eta < 1e-6 || xi < 1e-3 || xi > 1e5)
-        return 0.;
+    // using nf = nan since at O(as2) the coefficient functions don't depend on
+    // nf
+    int nf = static_cast<int>(nan(""));
+
+    if (eta < 1e-6)
+        return thr_->MuIndependentTerms(x, m2Q2, nf);
+    if (eta > 1e6 || xi > 1e5)
+        return asy_->MuIndependentTerms(x, m2Q2, nf);
+    if (xi < 1e-3) {
+        cout << "Error in ExactCoefficientFunction::C2_g20 : max value of m2Q2 "
+                "is 1e3. Got "
+             << m2Q2 << endl;
+        exit(-1);
+    }
 
     return 16 * M_PI * xi * c2nlog_(&eta, &xi) / x;
 }
 
 //==========================================================================================//
 //  Exact massive gluon coefficient functions at O(as^2):
 //  Term proportional to log(mu^2/m^2)
@@ -401,21 +449,33 @@
 //  at O(as^2)
 //
 //  Exact (but numerical) result from [arXiv:hep-ph/9411431].
 //  Taken from the Fortran code 'src/hqcoef.f'
 //------------------------------------------------------------------------------------------//
 
 double
-ExactCoefficientFunction::CL_g20(double x, double m2Q2, int /*nf*/) const {
+    ExactCoefficientFunction::CL_g20(double x, double m2Q2, int /*nf*/) const {
 
     double xi = 1. / m2Q2;
     double eta = 0.25 * xi * (1 - x) / x - 1.;
 
-    if (eta > 1e6 || eta < 1e-6 || xi < 1e-3 || xi > 1e5)
-        return 0.;
+    // using nf = nan since at O(as2) the coefficient functions don't depend on
+    // nf
+    int nf = static_cast<int>(nan(""));
+
+    if (eta < 1e-6)
+        return thr_->MuIndependentTerms(x, m2Q2, nf);
+    if (eta > 1e6 || xi > 1e5)
+        return asy_->MuIndependentTerms(x, m2Q2, nf);
+    if (xi < 1e-3) {
+        cout << "Error in ExactCoefficientFunction::CL_g20 : max value of m2Q2 "
+                "is 1e3. Got "
+             << m2Q2 << endl;
+        exit(-1);
+    }
 
     return 16 * M_PI * xi * clnlog_(&eta, &xi) / x;
 }
 
 //==========================================================================================//
 //  ExactCoefficientFunction: mu dependent part of the exact massive gluon
 //  coefficient function at O(as^2):
@@ -535,15 +595,14 @@
     return C_ps31(x, m2Q2, nf) * lmu + C_ps32(x, m2Q2, nf) * lmu * lmu;
 }
 
 //==========================================================================================//
 //  ExactCoefficientFunction: print warning for mu independent part of O(as^3)
 //------------------------------------------------------------------------------------------//
 
-double
-ExactCoefficientFunction::WarningFunc(double /*x*/, double /*m2Q2*/, int /*nf*/)
-    const {
+double ExactCoefficientFunction::
+    WarningFunc(double /*x*/, double /*m2Q2*/, int /*nf*/) const {
     cout << "Error: mu-independent terms of the exact coefficient function at "
             "O(a_s^3) are not known!"
          << endl;
     exit(-1);
 }
```

### Comparing `adani-1.0.1/src/HighEnergyCoefficientFunction.cc` & `adani-1.0.2/src/HighEnergyCoefficientFunction.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/src/HighScaleCoefficientFunction.cc` & `adani-1.0.2/src/HighScaleCoefficientFunction.cc`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 //  High scale (Q^2 >> m^2) limit of the gluon coefficient functions for F2 at
 //  O(as) expanded in terms of \alpha_s^{[nf+1]}
 //
 //  Eq. (B.4) of Ref. [arXiv:1205.5727].
 //------------------------------------------------------------------------------------------//
 
 double
-HighScaleCoefficientFunction::D2_g1_highscale(double x, double m2Q2) const {
+    HighScaleCoefficientFunction::D2_g1_highscale(double x, double m2Q2) const {
 
     return 4 * TR * (x * x + (x - 1) * (x - 1)) * log(1. / m2Q2)
            + massless_as1_->MuIndependentTerms(x, 1);
 }
 
 //==========================================================================================//
 //  High scale (Q^2 >> m^2) limit of the gluon coefficient functions for FL at
```

### Comparing `adani-1.0.1/src/HighScaleSplitLogs.cc` & `adani-1.0.2/src/HighScaleSplitLogs.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/src/MasslessCoefficientFunction.cc` & `adani-1.0.2/src/MasslessCoefficientFunction.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/src/MatchingCondition.cc` & `adani-1.0.2/src/MatchingCondition.cc`

 * *Files 0% similar despite different names*

```diff
@@ -102,23 +102,26 @@
             higher = a_Qq_PS_30(x, 1);
             lower = a_Qq_PS_30(x, -1);
             central = 0.5 * (higher + lower);
 
             return { central, higher, lower };
         } else {
             cout << "Error: something has gone wrong in "
-                    "MatchingCondition::MuIndependentNfIndependentTerm"
+                    "MatchingCondition::NotOrdered"
                  << endl;
             exit(-1);
         }
     } else {
         int low_id;
         if (version_ == "exact") {
             central = a_Qg_30(x, 0);
             return { central, central, central };
+        } else if (version_ == "gm") {
+            central = a_Qg_30(x, 2);
+            return { central, central, central };
         } else if (version_ == "abmp")
             low_id = -1;
         else if (version_ == "klmv")
             low_id = -12;
         else {
             cout << "Error: something has gone wrong in "
                     "MatchingCondition::NotOrdered"
@@ -257,15 +260,16 @@
 //  Approximation of the nf-independent part of the mu-independent part of the
 //  unrenormalized matching condition Qg at O(as^3).
 //
 //  v = 0 : exact result
 //  v = 1 : Eq. (3.49) of Ref. [arXiv:1205.5727]
 //  v = -1 : Eq. (16) Ref. of [arXiv:1701.05838]
 //  v = -12 : Eq. (3.50) of Ref. [arXiv:1205.5727]
-//  v = 2 : approximation from Giacomo Magni, based on the results of [arXiv:2403.00513]
+//  v = 2 : approximation from Giacomo Magni, based on the results of
+//  [arXiv:2403.00513]
 //------------------------------------------------------------------------------------------//
 
 double MatchingCondition::a_Qg_30(double x, int v) const {
 
     double L = log(x);
     double L2 = L * L;
```

### Comparing `adani-1.0.1/src/SpecialFunctions.cc` & `adani-1.0.2/src/SpecialFunctions.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/src/SplittingFunction.cc` & `adani-1.0.2/src/SplittingFunction.cc`

 * *Files 1% similar despite different names*

```diff
@@ -243,42 +243,42 @@
 }
 
 //==========================================================================================//
 //  ConvolutedSplittingFunctions: overload of operator * double
 //------------------------------------------------------------------------------------------//
 
 ConvolutedSplittingFunctions
-ConvolutedSplittingFunctions::operator*(const double &rhs) const {
+    ConvolutedSplittingFunctions::operator*(const double &rhs) const {
     ConvolutedSplittingFunctions res(
         order1_, entry1_, entry2_, order2_, entry3_, entry4_
     );
     res.SetMultFact(GetMultFact() * rhs);
     return res;
 }
 
 //==========================================================================================//
 //  ConvolutedSplittingFunctions: overload of operator double *
 //------------------------------------------------------------------------------------------//
 
 ConvolutedSplittingFunctions
-operator*(const double &lhs, const ConvolutedSplittingFunctions &rhs) {
+    operator*(const double &lhs, const ConvolutedSplittingFunctions &rhs) {
     ConvolutedSplittingFunctions res(
         rhs.order1_, rhs.entry1_, rhs.entry2_, rhs.order2_, rhs.entry3_,
         rhs.entry4_
     );
     res.SetMultFact(rhs.GetMultFact() * lhs);
     return res;
 }
 
 //==========================================================================================//
 //  ConvolutedSplittingFunctions: overload of operator / double
 //------------------------------------------------------------------------------------------//
 
 ConvolutedSplittingFunctions
-ConvolutedSplittingFunctions::operator/(const double &rhs) const {
+    ConvolutedSplittingFunctions::operator/(const double &rhs) const {
     ConvolutedSplittingFunctions res(
         order1_, entry1_, entry2_, order2_, entry3_, entry4_
     );
     res.SetMultFact(GetMultFact() / rhs);
     return res;
 }
 
@@ -289,17 +289,19 @@
 
 void ConvolutedSplittingFunctions::SetFunctions() {
 
     if (order1_ == 0 && order2_ == 0) {
         if (entry1_ == 'g' && entry2_ == 'q' && entry3_ == 'q'
             && entry4_ == 'g')
             reg_ = &ConvolutedSplittingFunctions::Pgq0_x_Pqg0;
-        else if (entry1_ == 'g' && entry2_ == 'g' && entry3_ == 'g' && entry4_ == 'q')
+        else if (entry1_ == 'g' && entry2_ == 'g' && entry3_ == 'g'
+                 && entry4_ == 'q')
             reg_ = &ConvolutedSplittingFunctions::Pgg0_x_Pgq0;
-        else if (entry1_ == 'q' && entry2_ == 'q' && entry3_ == 'g' && entry4_ == 'q')
+        else if (entry1_ == 'q' && entry2_ == 'q' && entry3_ == 'g'
+                 && entry4_ == 'q')
             reg_ = &ConvolutedSplittingFunctions::Pqq0_x_Pgq0;
         else {
             cout << "Error: P" << entry1_ << entry2_ << order1_ << " x P"
                  << entry3_ << entry4_ << order2_ << " is not implemented!"
                  << endl;
             exit(-1);
         }
```

### Comparing `adani-1.0.1/src/ThresholdCoefficientFunction.cc` & `adani-1.0.2/src/ThresholdCoefficientFunction.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #include "adani/ThresholdCoefficientFunction.h"
 #include "adani/Constants.h"
+#include "adani/ExactCoefficientFunction.h"
 #include "adani/SpecialFunctions.h"
 
 #include <cmath>
 #include <iostream>
 
 using std::cout;
 using std::endl;
@@ -13,15 +14,19 @@
 //------------------------------------------------------------------------------------------//
 
 ThresholdCoefficientFunction::ThresholdCoefficientFunction(
     const int &order, const char &kind, const char &channel
 )
     : CoefficientFunction(order, kind, channel) {
 
-    exact_as1_ = new ExactCoefficientFunction(1, GetKind(), GetChannel());
+    if (GetChannel() == 'g') {
+        exact_as1_ = new ExactCoefficientFunction(1, GetKind(), GetChannel());
+    } else
+        exact_as1_ = nullptr;
+
     SetFunctions();
 }
 
 //==========================================================================================//
 //  ThresholdCoefficientFunction: destructor
 //------------------------------------------------------------------------------------------//
```

### Comparing `adani-1.0.1/src/Value.cc` & `adani-1.0.2/src/Value.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/src/hplog.f` & `adani-1.0.2/src/hplog.f`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/src/hqcoef.f` & `adani-1.0.2/src/hqcoef.f`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/tests/test_approx_coeff_func.py` & `adani-1.0.2/tests/test_approx_coeff_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,41 +100,41 @@
                                 res_old = oldad.CL_ps21(x, m2Q2) * Lmu
                         if x > xmax:
                             res_old = 0.
                         res_new = app.MuDependentTerms(x, m2Q2, m2Q2, nf)
                         np.testing.assert_allclose(res_old, res_new, rtol=1e-7)
             del app
 
-def test_mudep_as3_oldversion():
-    for channel in ['g', 'q']:
-        for kind in ['2', 'L']:
-            highscale_version = "exact" if channel == 'q' else "abmp"
-            for mf in [False]:
-                app = ad.ApproximateCoefficientFunction(3, kind, channel, True, highscale_version, 1e-3, 1e-3, 1000, mf, 25000)
-                for xi in np.geomspace(1e-2, 1e2, 10):
-                    m2Q2 = 1/xi
-                    xmax = 1/(1 + 4*m2Q2)
-                    Lmu = -np.log(m2Q2)
-                    for x in np.geomspace(1e-5, 1, 10):
-                        for nf in [3, 4]:
-                            if kind == '2':
-                                if channel == 'g':
-                                    res_old = oldad.C2_g31(x, m2Q2, nf) * Lmu + oldad.C2_g32(x, m2Q2, nf, mf) * Lmu**2
-                                if channel == 'q':
-                                    res_old = oldad.C2_ps31(x, m2Q2, nf) * Lmu + oldad.C2_ps32(x, m2Q2, nf) * Lmu**2
-                            if kind == 'L':
-                                if channel == 'g':
-                                    res_old = oldad.CL_g31(x, m2Q2, nf) * Lmu + oldad.CL_g32(x, m2Q2, nf, mf) * Lmu**2
-                                if channel == 'q':
-                                    res_old = oldad.CL_ps31(x, m2Q2, nf) * Lmu + oldad.CL_ps32(x, m2Q2, nf) * Lmu**2
-                            if x > xmax:
-                                res_old = 0.
-                            res_new = app.MuDependentTerms(x, m2Q2, m2Q2, nf)
-                            np.testing.assert_allclose(res_old, res_new, rtol=1e-7)
-                del app
+# def test_mudep_as3_oldversion():
+#     for channel in ['g', 'q']:
+#         for kind in ['2', 'L']:
+#             highscale_version = "exact" if channel == 'q' else "abmp"
+#             for mf in [False]:
+#                 app = ad.ApproximateCoefficientFunction(3, kind, channel, True, highscale_version, 1e-3, 1e-3, 1000, mf, 25000)
+#                 for xi in np.geomspace(1e-2, 1e2, 10):
+#                     m2Q2 = 1/xi
+#                     xmax = 1/(1 + 4*m2Q2)
+#                     Lmu = -np.log(m2Q2)
+#                     for x in np.geomspace(1e-5, 1, 10):
+#                         for nf in [3, 4]:
+#                             if kind == '2':
+#                                 if channel == 'g':
+#                                     res_old = oldad.C2_g31(x, m2Q2, nf) * Lmu + oldad.C2_g32(x, m2Q2, nf, mf) * Lmu**2
+#                                 if channel == 'q':
+#                                     res_old = oldad.C2_ps31(x, m2Q2, nf) * Lmu + oldad.C2_ps32(x, m2Q2, nf) * Lmu**2
+#                             if kind == 'L':
+#                                 if channel == 'g':
+#                                     res_old = oldad.CL_g31(x, m2Q2, nf) * Lmu + oldad.CL_g32(x, m2Q2, nf, mf) * Lmu**2
+#                                 if channel == 'q':
+#                                     res_old = oldad.CL_ps31(x, m2Q2, nf) * Lmu + oldad.CL_ps32(x, m2Q2, nf) * Lmu**2
+#                             if x > xmax:
+#                                 res_old = 0.
+#                             res_new = app.MuDependentTerms(x, m2Q2, m2Q2, nf)
+#                             np.testing.assert_allclose(res_old, res_new, rtol=1e-7)
+                # del app
 
 def test_klmv_as2():
     for channel in ['g', 'q']:
         app = ad.ApproximateCoefficientFunctionKLMV(2, '2', channel, "abmp")
         for xi in np.geomspace(1e-2, 1e2, 10):
             m2Q2 = 1/xi
             for x in np.geomspace(1e-5, 1, 10):
```

### Comparing `adani-1.0.1/tests/test_asy.py` & `adani-1.0.2/tests/test_asy.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/tests/test_exact_coeff_func.py` & `adani-1.0.2/tests/test_exact_coeff_func.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,37 +8,33 @@
         cf = ad.ExactCoefficientFunction(1, kind, 'g')
         for xi in np.geomspace(1e-2, 1e4, 10, endpoint=True):
             xmax = 1/(1 + 4/xi)
             for x in np.geomspace(1e-5, xmax, 100, endpoint=False):
                 res1 = cf.fx(x, 1./xi, 1./xi, nf)
                 res2 = old.C2_g1(x, 1./xi) if kind == '2' else old.CL_g1(x, 1./xi)
                 np.testing.assert_allclose(res1, res2, rtol = 1e-7)
-def eta(x, xi):
-    return 0.25 * xi * (1 - x) / x - 1
 
 def test_as2_muindep():
     nf = 1
     for kind in ['2', 'L']:
         for channel in ['g', 'q']:
             cf = ad.ExactCoefficientFunction(2, kind, channel, 1e-3, 1e-3, 1000)
             for xi in np.geomspace(1e-2, 1e4, 10, endpoint=True):
-                xmax = 1/(1 + 4/xi)
-                for x in np.geomspace(1e-5, xmax, 10, endpoint=False):
+                for eta in np.geomspace(1e-5, 1e5, 10, endpoint=False):
+                    x = 1. / (1. + 4. * 1/xi * (eta + 1))
                     res1 = cf.MuIndependentTerms(x, 1./xi, nf)
-                    if eta(x, xi) < 1e6 and eta(x, xi) > 1e-6:
-                        if kind == '2' and channel == 'g':
-                            res2 = old.C2_g20(x, 1/xi)
-                        if kind == 'L' and channel == 'g':
-                            res2 = old.CL_g20(x, 1/xi)
-                        if kind == '2' and channel == 'q':
-                            res2 = old.C2_ps20(x, 1/xi)
-                        if kind == 'L' and channel == 'q':
-                            res2 = old.CL_ps20(x, 1/xi)
-                    else:
-                        res2 = 0
+                    if kind == '2' and channel == 'g':
+                        res2 = old.C2_g20(x, 1/xi)
+                    if kind == 'L' and channel == 'g':
+                        res2 = old.CL_g20(x, 1/xi)
+                    if kind == '2' and channel == 'q':
+                        res2 = old.C2_ps20(x, 1/xi)
+                    if kind == 'L' and channel == 'q':
+                        res2 = old.CL_ps20(x, 1/xi)
+
                     np.testing.assert_allclose(res1, res2, rtol = 1e-7)
 
 def test_as2_order_mudep():
     nf = 1
     for kind in ['2', 'L']:
         for channel in ['g', 'q']:
             cf = ad.ExactCoefficientFunction(2, kind, channel, 1e-3, 1e-3, 1000)
@@ -53,26 +49,26 @@
                             res2 = old.CL_g21(x, 1/xi)
                         elif kind == '2' and channel == 'q':
                             res2 = old.C2_ps21(x, 1/xi)
                         else:
                             res2 = old.CL_ps21(x, 1/xi)
                         np.testing.assert_allclose(res1, res2 * np.log(ximu), rtol = 1e-7)
 
-def test_as3_order_mudep():
-    for kind in ['2', 'L']:
-        for channel in ['g', 'q']:
-            cf = ad.ExactCoefficientFunction(3, kind, channel, 1e-3, 1e-3, 1000, False)
-            for xi in np.geomspace(1e-2, 1e4, 5, endpoint=True):
-                for ximu in np.geomspace(1e-2, 1e4, 5, endpoint=True):
-                    xmax = 1/(1 + 4/xi)
-                    for x in np.geomspace(1e-5, xmax, 5, endpoint=False):
-                        for nf in range(4, 6 + 1):
-                            res1 = cf.MuDependentTerms(x, 1./xi, 1./ximu, nf)
-                            if kind == '2' and channel == 'g':
-                                res2 = old.C2_g31(x, 1/xi, nf) * np.log(ximu) + old.C2_g32(x, 1/xi, nf) * np.log(ximu)**2
-                            elif kind == 'L' and channel == 'g':
-                                res2 = old.CL_g31(x, 1/xi, nf) * np.log(ximu) + old.CL_g32(x, 1/xi, nf) * np.log(ximu)**2
-                            elif kind == '2' and channel == 'q':
-                                res2 = old.C2_ps31(x, 1/xi, nf) * np.log(ximu) + old.C2_ps32(x, 1/xi, nf) * np.log(ximu)**2
-                            else:
-                                res2 = old.CL_ps31(x, 1/xi, nf) * np.log(ximu) + old.CL_ps32(x, 1/xi, nf) * np.log(ximu)**2
-                            np.testing.assert_allclose(res1, res2, rtol = 1e-7)
+# def test_as3_order_mudep():
+#     for kind in ['2', 'L']:
+#         for channel in ['g', 'q']:
+#             cf = ad.ExactCoefficientFunction(3, kind, channel, 1e-3, 1e-3, 1000, False)
+#             for xi in np.geomspace(1e-2, 1e4, 5, endpoint=True):
+#                 for ximu in np.geomspace(1e-2, 1e4, 5, endpoint=True):
+#                     xmax = 1/(1 + 4/xi)
+#                     for x in np.geomspace(1e-5, xmax, 5, endpoint=False):
+#                         for nf in range(4, 6 + 1):
+#                             res1 = cf.MuDependentTerms(x, 1./xi, 1./ximu, nf)
+#                             if kind == '2' and channel == 'g':
+#                                 res2 = old.C2_g31(x, 1/xi, nf) * np.log(ximu) + old.C2_g32(x, 1/xi, nf) * np.log(ximu)**2
+#                             elif kind == 'L' and channel == 'g':
+#                                 res2 = old.CL_g31(x, 1/xi, nf) * np.log(ximu) + old.CL_g32(x, 1/xi, nf) * np.log(ximu)**2
+#                             elif kind == '2' and channel == 'q':
+#                                 res2 = old.C2_ps31(x, 1/xi, nf) * np.log(ximu) + old.C2_ps32(x, 1/xi, nf) * np.log(ximu)**2
+#                             else:
+#                                 res2 = old.CL_ps31(x, 1/xi, nf) * np.log(ximu) + old.CL_ps32(x, 1/xi, nf) * np.log(ximu)**2
+#                             np.testing.assert_allclose(res1, res2, rtol = 1e-7)
```

### Comparing `adani-1.0.1/tests/test_high_scale.py` & `adani-1.0.2/tests/test_high_scale.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/tests/test_highenergy.py` & `adani-1.0.2/tests/test_highenergy.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/tests/test_massless.py` & `adani-1.0.2/tests/test_massless.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/tests/test_mc_integral.py` & `adani-1.0.2/tests/test_mc_integral.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/tests/test_splitting_functions.py` & `adani-1.0.2/tests/test_splitting_functions.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/tests/test_threshold.py` & `adani-1.0.2/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.1/versioneer.py` & `adani-1.0.2/versioneer.py`

 * *Files identical despite different names*

