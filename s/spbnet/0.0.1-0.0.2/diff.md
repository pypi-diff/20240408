# Comparing `tmp/spbnet-0.0.1.tar.gz` & `tmp/spbnet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spbnet-0.0.1.tar", last modified: Wed Apr  3 08:32:46 2024, max compression
+gzip compressed data, was "spbnet-0.0.2.tar", last modified: Mon Apr  8 06:51:05 2024, max compression
```

## Comparing `spbnet-0.0.1.tar` & `spbnet-0.0.2.tar`

### file list

```diff
@@ -1,202 +1,204 @@
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.859916 spbnet-0.0.1/
--rw-rw-r--   0 user1     (1002) user1     (1002)     1068 2024-03-26 10:50:29.000000 spbnet-0.0.1/LICENSE.txt
--rw-r--r--   0 user1     (1002) user1     (1002)     7764 2024-04-03 08:32:46.855916 spbnet-0.0.1/PKG-INFO
--rw-rw-r--   0 user1     (1002) user1     (1002)     6951 2024-03-30 11:19:53.000000 spbnet-0.0.1/README.md
--rw-rw-r--   0 user1     (1002) user1     (1002)       38 2024-04-03 08:32:46.859916 spbnet-0.0.1/setup.cfg
--rw-rw-r--   0 user1     (1002) user1     (1002)     1542 2024-03-29 07:41:03.000000 spbnet-0.0.1/setup.py
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.535916 spbnet-0.0.1/spbnet/
--rw-rw-r--   0 user1     (1002) user1     (1002)       87 2024-04-03 08:31:34.000000 spbnet-0.0.1/spbnet/__init__.py
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.539916 spbnet-0.0.1/spbnet/cli/
--rw-rw-r--   0 user1     (1002) user1     (1002)        0 2024-03-28 02:19:24.000000 spbnet-0.0.1/spbnet/cli/__init__.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     1128 2024-03-31 04:04:45.000000 spbnet-0.0.1/spbnet/cli/attn.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     1472 2024-03-28 10:31:18.000000 spbnet-0.0.1/spbnet/cli/buildAtomGrid.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     2629 2024-03-30 05:36:29.000000 spbnet-0.0.1/spbnet/cli/buildData.py
--rw-rw-r--   0 user1     (1002) user1     (1002)      650 2024-03-30 09:00:34.000000 spbnet-0.0.1/spbnet/cli/buildModalData.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     1200 2024-03-30 05:38:12.000000 spbnet-0.0.1/spbnet/cli/calcAtomNum.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     1013 2024-03-30 05:38:30.000000 spbnet-0.0.1/spbnet/cli/calcMeanStd.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     1671 2024-03-30 05:39:18.000000 spbnet-0.0.1/spbnet/cli/checkData.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     1846 2024-04-02 09:20:21.000000 spbnet-0.0.1/spbnet/cli/filterData.py
--rw-rw-r--   0 user1     (1002) user1     (1002)      353 2024-03-30 05:40:20.000000 spbnet-0.0.1/spbnet/cli/installMake.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     3353 2024-03-30 05:55:47.000000 spbnet-0.0.1/spbnet/cli/main.py
--rw-rw-r--   0 user1     (1002) user1     (1002)      322 2024-03-30 05:40:39.000000 spbnet-0.0.1/spbnet/cli/makeGriday.py
--rw-rw-r--   0 user1     (1002) user1     (1002)      294 2024-03-30 06:06:16.000000 spbnet-0.0.1/spbnet/cli/uninstallGriday.py
--rw-rw-r--   0 user1     (1002) user1     (1002)      129 2024-03-28 11:21:02.000000 spbnet-0.0.1/spbnet/config.example.yaml
--rw-r--r--   0 user1     (1002) user1     (1002)      954 2024-03-28 12:27:42.000000 spbnet-0.0.1/spbnet/config.finetune.yaml
--rw-r--r--   0 user1     (1002) user1     (1002)      867 2024-03-30 09:38:28.000000 spbnet-0.0.1/spbnet/config.pretrain.yaml
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.539916 spbnet-0.0.1/spbnet/data/
--rw-rw-r--   0 user1     (1002) user1     (1002)        0 2024-03-27 05:06:29.000000 spbnet-0.0.1/spbnet/data/__init__.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     2460 2024-03-28 02:20:11.000000 spbnet-0.0.1/spbnet/data/buildAtomGrid.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     3016 2024-03-28 02:38:46.000000 spbnet-0.0.1/spbnet/data/buildData.py
--rw-rw-r--   0 user1     (1002) user1     (1002)      987 2024-03-28 08:41:53.000000 spbnet-0.0.1/spbnet/data/calcAtomNum.py
--rw-rw-r--   0 user1     (1002) user1     (1002)      586 2024-03-28 03:09:36.000000 spbnet-0.0.1/spbnet/data/calcMeanStd.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     2379 2024-03-28 03:19:54.000000 spbnet-0.0.1/spbnet/data/checkData.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     7991 2024-03-28 01:32:59.000000 spbnet-0.0.1/spbnet/data/dataset.py
--rw-rw-r--   0 user1     (1002) user1     (1002)    10337 2024-03-29 06:21:56.000000 spbnet-0.0.1/spbnet/data/dataset_feat.py
--rw-rw-r--   0 user1     (1002) user1     (1002)    10325 2024-03-28 01:32:59.000000 spbnet-0.0.1/spbnet/data/dataset_pretrain.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     4362 2024-03-30 08:16:53.000000 spbnet-0.0.1/spbnet/data/filterData.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     1186 2024-03-27 06:21:32.000000 spbnet-0.0.1/spbnet/data/float2int8.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     2977 2024-03-27 05:56:32.000000 spbnet-0.0.1/spbnet/data/install_griday.py
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.491917 spbnet-0.0.1/spbnet/data/libs/
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.699916 spbnet-0.0.1/spbnet/data/libs/GRIDAY/
--rw-r--r--   0 user1     (1002) user1     (1002)     2799 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/AtomTypeMap.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      654 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/AtomTypeMap.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    41784 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/AtomTypeMap.o
--rw-r--r--   0 user1     (1002) user1     (1002)     2448 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Cell.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)     7789 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/ChannelAnalyzer.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      414 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/ChannelAnalyzer.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    32976 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/ChannelAnalyzer.o
--rw-r--r--   0 user1     (1002) user1     (1002)    54588 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/EnergyGrid.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)    18619 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/EnergyGrid.cpp-backup
--rw-r--r--   0 user1     (1002) user1     (1002)     3812 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/EnergyGrid.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)   141872 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/EnergyGrid.o
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.727916 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FF/
--rw-r--r--   0 user1     (1002) user1     (1002)     4751 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FF/UFF_FF.def
--rw-r--r--   0 user1     (1002) user1     (1002)      845 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FF/UFF_Type.def
--rw-r--r--   0 user1     (1002) user1     (1002)      202 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FF/Zeolite_FF.def
--rw-r--r--   0 user1     (1002) user1     (1002)      190 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
--rw-r--r--   0 user1     (1002) user1     (1002)      228 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FF/Zeolite_Gau_O.def
--rw-r--r--   0 user1     (1002) user1     (1002)      318 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
--rw-r--r--   0 user1     (1002) user1     (1002)      228 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FF/Zeolite_Gau_Si.def
--rw-r--r--   0 user1     (1002) user1     (1002)       26 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FF/Zeolite_Type.def
--rw-r--r--   0 user1     (1002) user1     (1002)     7197 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/ForceField.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      866 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/ForceField.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    70448 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/ForceField.o
--rw-r--r--   0 user1     (1002) user1     (1002)    13991 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FourierAnalyzer.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      865 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FourierAnalyzer.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    57072 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/FourierAnalyzer.o
--rw-r--r--   0 user1     (1002) user1     (1002)     7362 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Framework.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)     1197 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Framework.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    47744 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Framework.o
--rw-r--r--   0 user1     (1002) user1     (1002)     3007 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Gaussian.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      776 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Gaussian.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    14360 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Gaussian.o
--rw-r--r--   0 user1     (1002) user1     (1002)     9534 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridMaker.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      936 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridMaker.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    83296 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridMaker.o
--rw-r--r--   0 user1     (1002) user1     (1002)      320 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Griday.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)      948 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridayException.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      669 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridayException.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    15888 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridayException.o
--rw-r--r--   0 user1     (1002) user1     (1002)      567 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridayTypes.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)     4380 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/LennardJones.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      776 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/LennardJones.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    14240 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/LennardJones.o
--rw-r--r--   0 user1     (1002) user1     (1002)      334 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Makefile
--rw-r--r--   0 user1     (1002) user1     (1002)    21824 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/MaterialGrid.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)     2366 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/MaterialGrid.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    76688 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/MaterialGrid.o
--rw-r--r--   0 user1     (1002) user1     (1002)     5664 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/NlistMaker.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      922 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/NlistMaker.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    69080 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/NlistMaker.o
--rw-r--r--   0 user1     (1002) user1     (1002)      730 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/PairEnergy.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)      570 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Random.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)     5106 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/ShiftedLJ.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      764 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/ShiftedLJ.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    14704 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/ShiftedLJ.o
--rw-r--r--   0 user1     (1002) user1     (1002)      811 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Timer.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)     2277 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/Vector.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)   705504 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/libgriday.a
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.731916 spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/
--rw-r--r--   0 user1     (1002) user1     (1002)      563 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/Makefile
--rw-r--r--   0 user1     (1002) user1     (1002)     5834 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/adsorption_properties.cpp
--rwxrwxr-x   0 user1     (1002) user1     (1002)   161448 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/grid_gen
--rw-r--r--   0 user1     (1002) user1     (1002)     1046 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/main_cota.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)     1742 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/main_make_egrid.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      900 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/main_visit.cpp
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.783916 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/
--rw-r--r--   0 user1     (1002) user1     (1002)     2799 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/AtomTypeMap.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      654 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/AtomTypeMap.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    41784 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/AtomTypeMap.o
--rw-r--r--   0 user1     (1002) user1     (1002)     2448 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Cell.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)     7789 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/ChannelAnalyzer.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      414 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/ChannelAnalyzer.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    32976 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/ChannelAnalyzer.o
--rw-r--r--   0 user1     (1002) user1     (1002)    54588 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/EnergyGrid.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)    18619 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/EnergyGrid.cpp-backup
--rw-r--r--   0 user1     (1002) user1     (1002)     3812 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/EnergyGrid.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)   141872 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/EnergyGrid.o
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.819916 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FF/
--rw-r--r--   0 user1     (1002) user1     (1002)     4751 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FF/UFF_FF.def
--rw-r--r--   0 user1     (1002) user1     (1002)      845 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FF/UFF_Type.def
--rw-r--r--   0 user1     (1002) user1     (1002)      202 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FF/Zeolite_FF.def
--rw-r--r--   0 user1     (1002) user1     (1002)      190 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FF/Zeolite_FF_Shifted.def
--rw-r--r--   0 user1     (1002) user1     (1002)      228 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FF/Zeolite_Gau_O.def
--rw-r--r--   0 user1     (1002) user1     (1002)      318 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FF/Zeolite_Gau_O_Si.def
--rw-r--r--   0 user1     (1002) user1     (1002)      228 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FF/Zeolite_Gau_Si.def
--rw-r--r--   0 user1     (1002) user1     (1002)       26 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FF/Zeolite_Type.def
--rw-r--r--   0 user1     (1002) user1     (1002)     6359 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/ForceField.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      866 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/ForceField.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    66640 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/ForceField.o
--rw-r--r--   0 user1     (1002) user1     (1002)    13991 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FourierAnalyzer.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      865 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FourierAnalyzer.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    57072 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FourierAnalyzer.o
--rw-r--r--   0 user1     (1002) user1     (1002)     7362 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Framework.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)     1197 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Framework.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    47744 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Framework.o
--rw-r--r--   0 user1     (1002) user1     (1002)     9062 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridMaker.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      936 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridMaker.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    81752 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridMaker.o
--rw-r--r--   0 user1     (1002) user1     (1002)      320 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Griday.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)      948 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridayException.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      669 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridayException.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    15888 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridayException.o
--rw-r--r--   0 user1     (1002) user1     (1002)      534 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridayTypes.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)     4332 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/LennardJones.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      747 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/LennardJones.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    17592 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/LennardJones.o
--rw-r--r--   0 user1     (1002) user1     (1002)      334 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Makefile
--rw-r--r--   0 user1     (1002) user1     (1002)    21824 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/MaterialGrid.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)     2366 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/MaterialGrid.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    76688 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/MaterialGrid.o
--rw-r--r--   0 user1     (1002) user1     (1002)     5664 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/NlistMaker.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      922 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/NlistMaker.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)    69080 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/NlistMaker.o
--rw-r--r--   0 user1     (1002) user1     (1002)      756 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/PairEnergy.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)      570 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Random.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)      811 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Timer.hpp
--rw-r--r--   0 user1     (1002) user1     (1002)     2277 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Vector.hpp
--rw-rw-r--   0 user1     (1002) user1     (1002)   672770 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/libgriday.a
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.823916 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/
--rw-r--r--   0 user1     (1002) user1     (1002)      563 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/Makefile
--rw-r--r--   0 user1     (1002) user1     (1002)     5834 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/adsorption_properties.cpp
--rwxrwxr-x   0 user1     (1002) user1     (1002)   155304 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/grid_gen
--rw-r--r--   0 user1     (1002) user1     (1002)     1046 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/main_cota.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)     1742 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/main_make_egrid.cpp
--rw-r--r--   0 user1     (1002) user1     (1002)      900 2024-03-26 11:04:24.000000 spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/main_visit.cpp
--rw-rw-r--   0 user1     (1002) user1     (1002)     8776 2024-03-27 05:27:37.000000 spbnet-0.0.1/spbnet/data/prepare_data.py
--rw-r--r--   0 user1     (1002) user1     (1002)     9946 2024-03-30 09:38:48.000000 spbnet-0.0.1/spbnet/finetune.py
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.823916 spbnet-0.0.1/spbnet/modules/
--rw-rw-r--   0 user1     (1002) user1     (1002)        0 2024-03-28 01:32:13.000000 spbnet-0.0.1/spbnet/modules/__init__.py
--rw-r--r--   0 user1     (1002) user1     (1002)    10721 2024-03-28 01:32:02.000000 spbnet-0.0.1/spbnet/modules/cgcnn.py
--rw-r--r--   0 user1     (1002) user1     (1002)     3242 2024-03-28 01:32:02.000000 spbnet-0.0.1/spbnet/modules/heads.py
--rw-r--r--   0 user1     (1002) user1     (1002)    14902 2024-03-29 06:25:48.000000 spbnet-0.0.1/spbnet/modules/module.py
--rw-r--r--   0 user1     (1002) user1     (1002)      462 2024-03-28 01:32:02.000000 spbnet-0.0.1/spbnet/modules/objectives.py
--rw-r--r--   0 user1     (1002) user1     (1002)     5395 2024-03-30 05:41:55.000000 spbnet-0.0.1/spbnet/modules/optimize.py
--rw-r--r--   0 user1     (1002) user1     (1002)      820 2024-03-28 01:32:02.000000 spbnet-0.0.1/spbnet/modules/transformer.py
--rw-r--r--   0 user1     (1002) user1     (1002)    12795 2024-03-28 01:32:02.000000 spbnet-0.0.1/spbnet/modules/vision_transformer_3d.py
--rw-r--r--   0 user1     (1002) user1     (1002)    10194 2024-03-30 05:47:57.000000 spbnet-0.0.1/spbnet/pretrain.py
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.823916 spbnet-0.0.1/spbnet/utils/
--rw-rw-r--   0 user1     (1002) user1     (1002)        0 2024-03-27 05:06:50.000000 spbnet-0.0.1/spbnet/utils/__init__.py
--rw-rw-r--   0 user1     (1002) user1     (1002)      793 2024-04-02 10:09:25.000000 spbnet-0.0.1/spbnet/utils/echo.py
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.831916 spbnet-0.0.1/spbnet/visualize/
--rw-rw-r--   0 user1     (1002) user1     (1002)        0 2024-03-29 05:21:02.000000 spbnet-0.0.1/spbnet/visualize/__init__.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     6303 2024-03-29 07:47:30.000000 spbnet-0.0.1/spbnet/visualize/agc.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     5350 2024-04-02 08:05:21.000000 spbnet-0.0.1/spbnet/visualize/attn.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     4283 2024-03-29 07:32:26.000000 spbnet-0.0.1/spbnet/visualize/buildModalData.py
--rw-r--r--   0 user1     (1002) user1     (1002)     1651 2024-03-29 06:20:49.000000 spbnet-0.0.1/spbnet/visualize/config.yaml
--rw-r--r--   0 user1     (1002) user1     (1002)    10715 2024-03-29 06:26:31.000000 spbnet-0.0.1/spbnet/visualize/feat.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     3695 2024-03-29 06:40:17.000000 spbnet-0.0.1/spbnet/visualize/predAgc.py
--rw-rw-r--   0 user1     (1002) user1     (1002)    16198 2024-03-29 07:17:01.000000 spbnet-0.0.1/spbnet/visualize/prepare_data.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     2485 2024-03-29 06:29:15.000000 spbnet-0.0.1/spbnet/visualize/self_attn.heatmap.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     2891 2024-03-29 06:29:15.000000 spbnet-0.0.1/spbnet/visualize/self_attn.lineplot.py
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.831916 spbnet-0.0.1/spbnet/visualize/template/
--rw-rw-r--   0 user1     (1002) user1     (1002)     1639 2024-03-31 02:05:53.000000 spbnet-0.0.1/spbnet/visualize/template/attn.html
--rw-rw-r--   0 user1     (1002) user1     (1002)     3651 2024-03-29 06:29:15.000000 spbnet-0.0.1/spbnet/visualize/transfer.py
--rw-rw-r--   0 user1     (1002) user1     (1002)     6055 2024-03-29 07:34:14.000000 spbnet-0.0.1/spbnet/visualize/utils.py
-drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-03 08:32:46.855916 spbnet-0.0.1/spbnet.egg-info/
--rw-r--r--   0 user1     (1002) user1     (1002)     7764 2024-04-03 08:32:46.000000 spbnet-0.0.1/spbnet.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1002) user1     (1002)     6618 2024-04-03 08:32:46.000000 spbnet-0.0.1/spbnet.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1002) user1     (1002)        1 2024-04-03 08:32:46.000000 spbnet-0.0.1/spbnet.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1002) user1     (1002)       48 2024-04-03 08:32:46.000000 spbnet-0.0.1/spbnet.egg-info/entry_points.txt
--rw-rw-r--   0 user1     (1002) user1     (1002)      272 2024-04-03 08:32:46.000000 spbnet-0.0.1/spbnet.egg-info/requires.txt
--rw-rw-r--   0 user1     (1002) user1     (1002)        7 2024-04-03 08:32:46.000000 spbnet-0.0.1/spbnet.egg-info/top_level.txt
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.427354 spbnet-0.0.2/
+-rw-rw-r--   0 user1     (1002) user1     (1002)     1068 2024-04-03 08:39:16.000000 spbnet-0.0.2/LICENSE.txt
+-rw-r--r--   0 user1     (1002) user1     (1002)    10561 2024-04-08 06:51:05.427354 spbnet-0.0.2/PKG-INFO
+-rw-rw-r--   0 user1     (1002) user1     (1002)     9748 2024-04-08 06:29:33.000000 spbnet-0.0.2/README.md
+-rw-rw-r--   0 user1     (1002) user1     (1002)       38 2024-04-08 06:51:05.427354 spbnet-0.0.2/setup.cfg
+-rw-rw-r--   0 user1     (1002) user1     (1002)     1542 2024-04-03 08:39:17.000000 spbnet-0.0.2/setup.py
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.407354 spbnet-0.0.2/spbnet/
+-rw-rw-r--   0 user1     (1002) user1     (1002)      116 2024-04-08 06:48:09.000000 spbnet-0.0.2/spbnet/__init__.py
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.411354 spbnet-0.0.2/spbnet/cli/
+-rw-rw-r--   0 user1     (1002) user1     (1002)        0 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/__init__.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     1128 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/attn.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     1472 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/buildAtomGrid.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     2629 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/buildData.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)      650 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/buildModalData.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     1200 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/calcAtomNum.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     1013 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/calcMeanStd.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     1671 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/checkData.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     1846 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/filterData.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)      353 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/installMake.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     3353 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/main.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)      322 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/makeGriday.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)      294 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/cli/uninstallGriday.py
+-rw-r--r--   0 user1     (1002) user1     (1002)      954 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/config.finetune.yaml
+-rw-rw-r--   0 user1     (1002) user1     (1002)      935 2024-04-08 05:47:58.000000 spbnet-0.0.2/spbnet/config.predict.yaml
+-rw-r--r--   0 user1     (1002) user1     (1002)      867 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/config.pretrain.yaml
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.411354 spbnet-0.0.2/spbnet/data/
+-rw-rw-r--   0 user1     (1002) user1     (1002)        0 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/__init__.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     2460 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/buildAtomGrid.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     3016 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/buildData.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)      987 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/calcAtomNum.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)      586 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/calcMeanStd.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     2379 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/checkData.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     7991 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/dataset.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)    10337 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/dataset_feat.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     7907 2024-04-08 05:59:08.000000 spbnet-0.0.2/spbnet/data/dataset_predict.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)    10325 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/dataset_pretrain.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     4362 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/filterData.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     1186 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/float2int8.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     2977 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/install_griday.py
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.407354 spbnet-0.0.2/spbnet/data/libs/
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.415354 spbnet-0.0.2/spbnet/data/libs/GRIDAY/
+-rw-r--r--   0 user1     (1002) user1     (1002)     2799 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/AtomTypeMap.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      654 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/AtomTypeMap.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    41784 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/AtomTypeMap.o
+-rw-r--r--   0 user1     (1002) user1     (1002)     2448 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Cell.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     7789 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/ChannelAnalyzer.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      414 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/ChannelAnalyzer.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    32976 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/ChannelAnalyzer.o
+-rw-r--r--   0 user1     (1002) user1     (1002)    54588 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/EnergyGrid.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)    18619 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/EnergyGrid.cpp-backup
+-rw-r--r--   0 user1     (1002) user1     (1002)     3812 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/EnergyGrid.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)   141872 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/EnergyGrid.o
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.415354 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FF/
+-rw-r--r--   0 user1     (1002) user1     (1002)     4751 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FF/UFF_FF.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      845 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FF/UFF_Type.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      202 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FF/Zeolite_FF.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      190 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      228 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FF/Zeolite_Gau_O.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      318 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      228 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FF/Zeolite_Gau_Si.def
+-rw-r--r--   0 user1     (1002) user1     (1002)       26 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FF/Zeolite_Type.def
+-rw-r--r--   0 user1     (1002) user1     (1002)     7197 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/ForceField.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      866 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/ForceField.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    70448 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/ForceField.o
+-rw-r--r--   0 user1     (1002) user1     (1002)    13991 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FourierAnalyzer.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      865 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FourierAnalyzer.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    57072 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/FourierAnalyzer.o
+-rw-r--r--   0 user1     (1002) user1     (1002)     7362 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Framework.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     1197 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Framework.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    47744 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Framework.o
+-rw-r--r--   0 user1     (1002) user1     (1002)     3007 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Gaussian.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      776 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Gaussian.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    14360 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Gaussian.o
+-rw-r--r--   0 user1     (1002) user1     (1002)     9534 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridMaker.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      936 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridMaker.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    83296 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridMaker.o
+-rw-r--r--   0 user1     (1002) user1     (1002)      320 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Griday.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      948 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridayException.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      669 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridayException.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    15888 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridayException.o
+-rw-r--r--   0 user1     (1002) user1     (1002)      567 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridayTypes.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     4380 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/LennardJones.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      776 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/LennardJones.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    14240 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/LennardJones.o
+-rw-r--r--   0 user1     (1002) user1     (1002)      334 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Makefile
+-rw-r--r--   0 user1     (1002) user1     (1002)    21824 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/MaterialGrid.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     2366 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/MaterialGrid.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    76688 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/MaterialGrid.o
+-rw-r--r--   0 user1     (1002) user1     (1002)     5664 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/NlistMaker.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      922 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/NlistMaker.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    69080 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/NlistMaker.o
+-rw-r--r--   0 user1     (1002) user1     (1002)      730 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/PairEnergy.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      570 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Random.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     5106 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/ShiftedLJ.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      764 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/ShiftedLJ.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    14704 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/ShiftedLJ.o
+-rw-r--r--   0 user1     (1002) user1     (1002)      811 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Timer.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     2277 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/Vector.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)   705504 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/libgriday.a
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.419355 spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/
+-rw-r--r--   0 user1     (1002) user1     (1002)      563 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/Makefile
+-rw-r--r--   0 user1     (1002) user1     (1002)     5834 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/adsorption_properties.cpp
+-rwxrwxr-x   0 user1     (1002) user1     (1002)   161448 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/grid_gen
+-rw-r--r--   0 user1     (1002) user1     (1002)     1046 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/main_cota.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     1742 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/main_make_egrid.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      900 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/main_visit.cpp
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.423354 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/
+-rw-r--r--   0 user1     (1002) user1     (1002)     2799 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/AtomTypeMap.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      654 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/AtomTypeMap.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    41784 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/AtomTypeMap.o
+-rw-r--r--   0 user1     (1002) user1     (1002)     2448 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Cell.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     7789 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/ChannelAnalyzer.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      414 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/ChannelAnalyzer.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    32976 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/ChannelAnalyzer.o
+-rw-r--r--   0 user1     (1002) user1     (1002)    54588 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/EnergyGrid.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)    18619 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/EnergyGrid.cpp-backup
+-rw-r--r--   0 user1     (1002) user1     (1002)     3812 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/EnergyGrid.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)   141872 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/EnergyGrid.o
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.423354 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FF/
+-rw-r--r--   0 user1     (1002) user1     (1002)     4751 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FF/UFF_FF.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      845 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FF/UFF_Type.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      202 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FF/Zeolite_FF.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      190 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FF/Zeolite_FF_Shifted.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      228 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FF/Zeolite_Gau_O.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      318 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FF/Zeolite_Gau_O_Si.def
+-rw-r--r--   0 user1     (1002) user1     (1002)      228 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FF/Zeolite_Gau_Si.def
+-rw-r--r--   0 user1     (1002) user1     (1002)       26 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FF/Zeolite_Type.def
+-rw-r--r--   0 user1     (1002) user1     (1002)     6359 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/ForceField.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      866 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/ForceField.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    66640 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/ForceField.o
+-rw-r--r--   0 user1     (1002) user1     (1002)    13991 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FourierAnalyzer.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      865 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FourierAnalyzer.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    57072 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FourierAnalyzer.o
+-rw-r--r--   0 user1     (1002) user1     (1002)     7362 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Framework.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     1197 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Framework.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    47744 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Framework.o
+-rw-r--r--   0 user1     (1002) user1     (1002)     9062 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridMaker.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      936 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridMaker.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    81752 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridMaker.o
+-rw-r--r--   0 user1     (1002) user1     (1002)      320 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Griday.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      948 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridayException.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      669 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridayException.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    15888 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridayException.o
+-rw-r--r--   0 user1     (1002) user1     (1002)      534 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridayTypes.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     4332 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/LennardJones.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      747 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/LennardJones.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    17592 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/LennardJones.o
+-rw-r--r--   0 user1     (1002) user1     (1002)      334 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Makefile
+-rw-r--r--   0 user1     (1002) user1     (1002)    21824 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/MaterialGrid.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     2366 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/MaterialGrid.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    76688 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/MaterialGrid.o
+-rw-r--r--   0 user1     (1002) user1     (1002)     5664 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/NlistMaker.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      922 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/NlistMaker.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)    69080 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/NlistMaker.o
+-rw-r--r--   0 user1     (1002) user1     (1002)      756 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/PairEnergy.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      570 2024-04-03 08:39:04.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Random.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      811 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Timer.hpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     2277 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Vector.hpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)   672770 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/libgriday.a
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.423354 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/
+-rw-r--r--   0 user1     (1002) user1     (1002)      563 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/Makefile
+-rw-r--r--   0 user1     (1002) user1     (1002)     5834 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/adsorption_properties.cpp
+-rwxrwxr-x   0 user1     (1002) user1     (1002)   155304 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/grid_gen
+-rw-r--r--   0 user1     (1002) user1     (1002)     1046 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/main_cota.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)     1742 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/main_make_egrid.cpp
+-rw-r--r--   0 user1     (1002) user1     (1002)      900 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/main_visit.cpp
+-rw-rw-r--   0 user1     (1002) user1     (1002)     8776 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/data/prepare_data.py
+-rw-r--r--   0 user1     (1002) user1     (1002)     9946 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/finetune.py
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.423354 spbnet-0.0.2/spbnet/modules/
+-rw-rw-r--   0 user1     (1002) user1     (1002)        0 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/modules/__init__.py
+-rw-r--r--   0 user1     (1002) user1     (1002)    10721 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/modules/cgcnn.py
+-rw-r--r--   0 user1     (1002) user1     (1002)     3242 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/modules/heads.py
+-rw-r--r--   0 user1     (1002) user1     (1002)    14902 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/modules/module.py
+-rw-r--r--   0 user1     (1002) user1     (1002)      462 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/modules/objectives.py
+-rw-r--r--   0 user1     (1002) user1     (1002)     5395 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/modules/optimize.py
+-rw-r--r--   0 user1     (1002) user1     (1002)      820 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/modules/transformer.py
+-rw-r--r--   0 user1     (1002) user1     (1002)    12795 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/modules/vision_transformer_3d.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     5217 2024-04-08 06:02:52.000000 spbnet-0.0.2/spbnet/predict.py
+-rw-r--r--   0 user1     (1002) user1     (1002)    10194 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/pretrain.py
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.423354 spbnet-0.0.2/spbnet/utils/
+-rw-rw-r--   0 user1     (1002) user1     (1002)        0 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/utils/__init__.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)      793 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/utils/echo.py
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.427354 spbnet-0.0.2/spbnet/visualize/
+-rw-rw-r--   0 user1     (1002) user1     (1002)        0 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/__init__.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     6303 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/agc.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     5350 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/attn.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     4283 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/buildModalData.py
+-rw-r--r--   0 user1     (1002) user1     (1002)     1651 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/config.yaml
+-rw-r--r--   0 user1     (1002) user1     (1002)    10715 2024-04-08 06:20:20.000000 spbnet-0.0.2/spbnet/visualize/feat.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     3695 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/predAgc.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)    16198 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/prepare_data.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     2485 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/self_attn.heatmap.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     2891 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/self_attn.lineplot.py
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.427354 spbnet-0.0.2/spbnet/visualize/template/
+-rw-rw-r--   0 user1     (1002) user1     (1002)     1639 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/template/attn.html
+-rw-rw-r--   0 user1     (1002) user1     (1002)     3651 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/transfer.py
+-rw-rw-r--   0 user1     (1002) user1     (1002)     6055 2024-04-03 08:39:05.000000 spbnet-0.0.2/spbnet/visualize/utils.py
+drwxrwxr-x   0 user1     (1002) user1     (1002)        0 2024-04-08 06:51:05.427354 spbnet-0.0.2/spbnet.egg-info/
+-rw-r--r--   0 user1     (1002) user1     (1002)    10561 2024-04-08 06:51:05.000000 spbnet-0.0.2/spbnet.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1002) user1     (1002)     6667 2024-04-08 06:51:05.000000 spbnet-0.0.2/spbnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1002) user1     (1002)        1 2024-04-08 06:51:05.000000 spbnet-0.0.2/spbnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1002) user1     (1002)       48 2024-04-08 06:51:05.000000 spbnet-0.0.2/spbnet.egg-info/entry_points.txt
+-rw-rw-r--   0 user1     (1002) user1     (1002)      272 2024-04-08 06:51:05.000000 spbnet-0.0.2/spbnet.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1002) user1     (1002)        7 2024-04-08 06:51:05.000000 spbnet-0.0.2/spbnet.egg-info/top_level.txt
```

### Comparing `spbnet-0.0.1/LICENSE.txt` & `spbnet-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/PKG-INFO` & `spbnet-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,64 @@
-Metadata-Version: 2.1
-Name: spbnet
-Version: 0.0.1
-Summary: spbnet
-Home-page: https://tyvanzou.github.io/spbnet/
-Download-URL: https://github.com/tyvanzou/spbnet
-Author: Jiawen Zou
-Author-email: 20307130189@fudan.edu.cn
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: ase==3.22.1
-Requires-Dist: matplotlib==3.7.5
-Requires-Dist: numpy==1.24.4
-Requires-Dist: pandas==2.0.3
-Requires-Dist: pymatgen==2023.8.10
-Requires-Dist: requests==2.31.0
-Requires-Dist: scipy==1.10.1
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: torch==2.2.2
-Requires-Dist: lightning==2.2.1
-Requires-Dist: transformers==4.39.1
-Requires-Dist: einops==0.7.0
-Requires-Dist: timm==0.9.16
-Requires-Dist: tensorboard==2.14.0
-Requires-Dist: scikit-learn==1.3.2
-Requires-Dist: seaborn==0.13.2
-Requires-Dist: colorama==0.4.6
-
 # SpbNet
 
 SpbNet is the official implementation of the paper.
 
+## The demo to fine-tune SpbNet
+
+A example to finetune SpbNet has been uploaded to [Figshare](https://figshare.com/projects/spbnet/200692). To run this demo, download the `demo.tar.gz` file and extract it. The directory should be look like
+
+```txt
+Root
+├── demo
+|  ├── ckpt
+|  ├── config.example.yaml
+|  ├── data
+|  |  ├── benchmark.csv
+|  |  ├── benchmark.filter.csv
+|  |  ├── benchmark.test.csv
+|  |  ├── benchmark.train.csv
+|  |  ├── benchmark.validate.csv
+|  |  ├── cif
+|  |  └── spbnet
+|  ├── logs
+|  |  └── hmof
+|  └── main.py
+└── demo.tar.gz
+```
+
+To finetune, you should first download the pretrained weight from [Figshare](https://figshare.com/projects/spbnet/200692). Put the weight to `demo/ckpt` directory. Then you can install spbnet and finetune spbnet.
+
+```sh
+cd demo
+# optional: conda create -n spbtest python=3.10
+# optional: conda activate spbtest
+pip install spbnet
+python ./finetune.py
+python ./predict.py
+python ./feat.py
+```
+
+The log will be put in the `logs` directory. We have provided the expected result in the `logs/CO2-298-2.5/version_0` direcotry.
+
+After fine-tuned for `30` epochs, the result should look like:
+
+```sh
+---------------------------------------
+	Test metric		DataLoader 0
+---------------------------------------
+	test_mae		1.5358973344167073
+	test_mse		3.877110533444727
+	test_r2			0.3504098369900308
+---------------------------------------
+```
+
+The predicted result can be found in the log directory, which should look like `logs/hmof/CO2-298-2.5/version_0/test_result.csv`.
+
+## Prepare
+
 To finetune spbnet, we recommend to make a new directory.
 
 ```sh
 mkdir test
 cd test
 ```
 
@@ -55,15 +80,15 @@
 
 ```shell
 pip install spbnet
 ```
 
 ### Download weight
 
-The weight has been uploaded in [Figshare](https://figshare.com).
+The weight has been uploaded in [Figshare](https://figshare.com/projects/spbnet/200692).
 
 Save the weight to your directory, such as `./ckpt/spbnet.180k.ckpt`
 
 Your directory should look like:
 
 ```txt
 - test
@@ -266,14 +291,56 @@
         ...
     - logs
         ...
     config.example.yaml
     main.py
 ```
 
+## Predict
+
+After finetune, the checkpoints and hyperparamters should be found in directory like `./tests/logs/hmof/CO2-298-2.5/version_0`. Due to that SpbNet will automatically normalize the training data during training to increase training stability. SpbNet uses mean-variance normalization. The mean and std used can be found in `.../version_0/hparams.yaml`.
+
+Based on the finetuned checkpoint and mean, std. You can predict the target property. First provide the `data_dir` and the `id_prop` csv file. The `id_prop` file should looks like
+
+```txt
+cifid
+mof1
+mof2
+...
+```
+
+Then prepare a configuration `yaml` file like
+
+```yaml
+ckpt: './logs/hmof/CO2-298-2.5/version_0/checkpoints/last.ckpt'
+data_dir: './data/spbnet'
+id_prop: './data/benchmark.test.csv' # the id_prop file
+log_dir: './predict'
+
+mean: 5.325830404166666
+std: 2.6947958848152913
+```
+
+Then predict
+
+```python
+import spbnet
+
+spbnet.predict("./config.predict.yaml")
+```
+
+The `test_results.csv` will be saved in directory like `predict/version_0`. It shoud look like
+
+```csv
+cifid,predict
+hMOF-4000155,12.504342079162598
+hMOF-5024342,2.8985860347747803
+hMOF-25731,4.6314473152160645
+```
+
 ## Visualize
 
 SpbNet provide visualization of attention score and atom grid.
 
 To visualize cif file, make a new directory and prepare a `cif` format file. Such as
 
 ```txt
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spbnet-0.0.1/setup.py` & `spbnet-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/cli/attn.py` & `spbnet-0.0.2/spbnet/cli/attn.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/cli/buildAtomGrid.py` & `spbnet-0.0.2/spbnet/cli/buildAtomGrid.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/cli/buildData.py` & `spbnet-0.0.2/spbnet/cli/buildData.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/cli/buildModalData.py` & `spbnet-0.0.2/spbnet/cli/buildModalData.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/cli/calcAtomNum.py` & `spbnet-0.0.2/spbnet/cli/calcAtomNum.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/cli/calcMeanStd.py` & `spbnet-0.0.2/spbnet/cli/calcMeanStd.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/cli/checkData.py` & `spbnet-0.0.2/spbnet/cli/checkData.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/cli/filterData.py` & `spbnet-0.0.2/spbnet/cli/filterData.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/cli/main.py` & `spbnet-0.0.2/spbnet/cli/main.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/config.finetune.yaml` & `spbnet-0.0.2/spbnet/config.finetune.yaml`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/config.pretrain.yaml` & `spbnet-0.0.2/spbnet/config.pretrain.yaml`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/buildAtomGrid.py` & `spbnet-0.0.2/spbnet/data/buildAtomGrid.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/buildData.py` & `spbnet-0.0.2/spbnet/data/buildData.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/calcAtomNum.py` & `spbnet-0.0.2/spbnet/data/calcAtomNum.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/calcMeanStd.py` & `spbnet-0.0.2/spbnet/data/calcMeanStd.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/checkData.py` & `spbnet-0.0.2/spbnet/data/checkData.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/dataset.py` & `spbnet-0.0.2/spbnet/data/dataset.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/dataset_feat.py` & `spbnet-0.0.2/spbnet/data/dataset_feat.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/dataset_pretrain.py` & `spbnet-0.0.2/spbnet/data/dataset_pretrain.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/filterData.py` & `spbnet-0.0.2/spbnet/data/filterData.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/float2int8.py` & `spbnet-0.0.2/spbnet/data/float2int8.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/install_griday.py` & `spbnet-0.0.2/spbnet/data/install_griday.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/AtomTypeMap.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/AtomTypeMap.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/AtomTypeMap.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/AtomTypeMap.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/AtomTypeMap.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/AtomTypeMap.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/Cell.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/Cell.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/ChannelAnalyzer.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/ChannelAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/ChannelAnalyzer.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/ChannelAnalyzer.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/EnergyGrid.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/EnergyGrid.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/EnergyGrid.cpp-backup` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/EnergyGrid.cpp-backup`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/EnergyGrid.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/EnergyGrid.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/EnergyGrid.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/EnergyGrid.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/FF/UFF_FF.def` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/FF/UFF_FF.def`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/FF/UFF_Type.def` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/FF/UFF_Type.def`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/ForceField.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/ForceField.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/ForceField.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/ForceField.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/ForceField.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/ForceField.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/FourierAnalyzer.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/FourierAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/FourierAnalyzer.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/FourierAnalyzer.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/FourierAnalyzer.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/FourierAnalyzer.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/Framework.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/Framework.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/Framework.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/Framework.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/Framework.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/Framework.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/Gaussian.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/Gaussian.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/Gaussian.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/Gaussian.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/Gaussian.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/Gaussian.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridMaker.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridMaker.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridMaker.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridMaker.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridMaker.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridMaker.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridayException.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridayException.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridayException.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridayException.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridayException.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridayException.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/GridayTypes.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/GridayTypes.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/LennardJones.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/LennardJones.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/LennardJones.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/LennardJones.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/LennardJones.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/LennardJones.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/MaterialGrid.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/MaterialGrid.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/MaterialGrid.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/MaterialGrid.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/MaterialGrid.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/MaterialGrid.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/NlistMaker.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/NlistMaker.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/NlistMaker.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/NlistMaker.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/NlistMaker.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/NlistMaker.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/PairEnergy.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/PairEnergy.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/Random.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/Random.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/ShiftedLJ.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/ShiftedLJ.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/ShiftedLJ.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/ShiftedLJ.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/ShiftedLJ.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/ShiftedLJ.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/Timer.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/Timer.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/Vector.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/Vector.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/libgriday.a` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/libgriday.a`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/Makefile` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/Makefile`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/adsorption_properties.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/adsorption_properties.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/grid_gen` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/grid_gen`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/main_cota.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/main_cota.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/main_make_egrid.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/main_make_egrid.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAY/scripts/main_visit.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAY/scripts/main_visit.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/AtomTypeMap.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/AtomTypeMap.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/AtomTypeMap.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/AtomTypeMap.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/AtomTypeMap.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/AtomTypeMap.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Cell.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Cell.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/ChannelAnalyzer.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/ChannelAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/ChannelAnalyzer.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/ChannelAnalyzer.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/EnergyGrid.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/EnergyGrid.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/EnergyGrid.cpp-backup` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/EnergyGrid.cpp-backup`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/EnergyGrid.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/EnergyGrid.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/EnergyGrid.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/EnergyGrid.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FF/UFF_FF.def` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FF/UFF_FF.def`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FF/UFF_Type.def` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FF/UFF_Type.def`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/ForceField.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/ForceField.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/ForceField.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/ForceField.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/ForceField.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/ForceField.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FourierAnalyzer.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FourierAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FourierAnalyzer.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FourierAnalyzer.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/FourierAnalyzer.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/FourierAnalyzer.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Framework.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Framework.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Framework.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Framework.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Framework.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Framework.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridMaker.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridMaker.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridMaker.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridMaker.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridMaker.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridMaker.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridayException.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridayException.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridayException.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridayException.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridayException.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridayException.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/GridayTypes.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/GridayTypes.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/LennardJones.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/LennardJones.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/LennardJones.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/LennardJones.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/LennardJones.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/LennardJones.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/MaterialGrid.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/MaterialGrid.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/MaterialGrid.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/MaterialGrid.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/MaterialGrid.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/MaterialGrid.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/NlistMaker.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/NlistMaker.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/NlistMaker.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/NlistMaker.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/NlistMaker.o` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/NlistMaker.o`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/PairEnergy.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/PairEnergy.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Random.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Random.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Timer.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Timer.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/Vector.hpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/Vector.hpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/libgriday.a` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/libgriday.a`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/Makefile` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/Makefile`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/adsorption_properties.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/adsorption_properties.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/grid_gen` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/grid_gen`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/main_cota.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/main_cota.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/main_make_egrid.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/main_make_egrid.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/libs/GRIDAYS/scripts/main_visit.cpp` & `spbnet-0.0.2/spbnet/data/libs/GRIDAYS/scripts/main_visit.cpp`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/data/prepare_data.py` & `spbnet-0.0.2/spbnet/data/prepare_data.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/finetune.py` & `spbnet-0.0.2/spbnet/finetune.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/modules/cgcnn.py` & `spbnet-0.0.2/spbnet/modules/cgcnn.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/modules/heads.py` & `spbnet-0.0.2/spbnet/modules/heads.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/modules/module.py` & `spbnet-0.0.2/spbnet/modules/module.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/modules/optimize.py` & `spbnet-0.0.2/spbnet/modules/optimize.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/modules/transformer.py` & `spbnet-0.0.2/spbnet/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/modules/vision_transformer_3d.py` & `spbnet-0.0.2/spbnet/modules/vision_transformer_3d.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/pretrain.py` & `spbnet-0.0.2/spbnet/pretrain.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/utils/echo.py` & `spbnet-0.0.2/spbnet/utils/echo.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/visualize/agc.py` & `spbnet-0.0.2/spbnet/visualize/agc.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/visualize/attn.py` & `spbnet-0.0.2/spbnet/visualize/attn.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/visualize/buildModalData.py` & `spbnet-0.0.2/spbnet/visualize/buildModalData.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/visualize/config.yaml` & `spbnet-0.0.2/spbnet/visualize/config.yaml`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/visualize/feat.py` & `spbnet-0.0.2/spbnet/visualize/feat.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,16 +174,16 @@
                 self.agc_labels.append(agc_label)  # [20 * B]
             if feat_name == "feat":
                 self.feats.append(feat)  # [B]
             if feat_name == "self_attn":
                 self.self_attns.append(self_attn)  # [5, 1000, 1000]
 
     def on_test_epoch_end(self) -> None:
-        save_dir = Path(self.config["save_dir"], parents=True)
-        save_dir.mkdir(exist_ok=True)
+        save_dir = Path(self.config["save_dir"])
+        save_dir.mkdir(exist_ok=True, parents=True)
 
         for feat_name in self.config["feats"]:
             if feat_name == "potential":
                 potential_feats = np.concatenate(self.potential_feats)
                 np.save(
                     save_dir / f"potential_feats.npy", potential_feats
                 )  # [N * 20, hid_dim]
```

### Comparing `spbnet-0.0.1/spbnet/visualize/predAgc.py` & `spbnet-0.0.2/spbnet/visualize/predAgc.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/visualize/prepare_data.py` & `spbnet-0.0.2/spbnet/visualize/prepare_data.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/visualize/self_attn.heatmap.py` & `spbnet-0.0.2/spbnet/visualize/self_attn.heatmap.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/visualize/self_attn.lineplot.py` & `spbnet-0.0.2/spbnet/visualize/self_attn.lineplot.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/visualize/template/attn.html` & `spbnet-0.0.2/spbnet/visualize/template/attn.html`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/visualize/transfer.py` & `spbnet-0.0.2/spbnet/visualize/transfer.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet/visualize/utils.py` & `spbnet-0.0.2/spbnet/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `spbnet-0.0.1/spbnet.egg-info/PKG-INFO` & `spbnet-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spbnet
-Version: 0.0.1
+Version: 0.0.2
 Summary: spbnet
 Home-page: https://tyvanzou.github.io/spbnet/
 Download-URL: https://github.com/tyvanzou/spbnet
 Author: Jiawen Zou
 Author-email: 20307130189@fudan.edu.cn
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -26,14 +26,67 @@
 Requires-Dist: seaborn==0.13.2
 Requires-Dist: colorama==0.4.6
 
 # SpbNet
 
 SpbNet is the official implementation of the paper.
 
+## The demo to fine-tune SpbNet
+
+A example to finetune SpbNet has been uploaded to [Figshare](https://figshare.com/projects/spbnet/200692). To run this demo, download the `demo.tar.gz` file and extract it. The directory should be look like
+
+```txt
+Root
+├── demo
+|  ├── ckpt
+|  ├── config.example.yaml
+|  ├── data
+|  |  ├── benchmark.csv
+|  |  ├── benchmark.filter.csv
+|  |  ├── benchmark.test.csv
+|  |  ├── benchmark.train.csv
+|  |  ├── benchmark.validate.csv
+|  |  ├── cif
+|  |  └── spbnet
+|  ├── logs
+|  |  └── hmof
+|  └── main.py
+└── demo.tar.gz
+```
+
+To finetune, you should first download the pretrained weight from [Figshare](https://figshare.com/projects/spbnet/200692). Put the weight to `demo/ckpt` directory. Then you can install spbnet and finetune spbnet.
+
+```sh
+cd demo
+# optional: conda create -n spbtest python=3.10
+# optional: conda activate spbtest
+pip install spbnet
+python ./finetune.py
+python ./predict.py
+python ./feat.py
+```
+
+The log will be put in the `logs` directory. We have provided the expected result in the `logs/CO2-298-2.5/version_0` direcotry.
+
+After fine-tuned for `30` epochs, the result should look like:
+
+```sh
+---------------------------------------
+	Test metric		DataLoader 0
+---------------------------------------
+	test_mae		1.5358973344167073
+	test_mse		3.877110533444727
+	test_r2			0.3504098369900308
+---------------------------------------
+```
+
+The predicted result can be found in the log directory, which should look like `logs/hmof/CO2-298-2.5/version_0/test_result.csv`.
+
+## Prepare
+
 To finetune spbnet, we recommend to make a new directory.
 
 ```sh
 mkdir test
 cd test
 ```
 
@@ -55,15 +108,15 @@
 
 ```shell
 pip install spbnet
 ```
 
 ### Download weight
 
-The weight has been uploaded in [Figshare](https://figshare.com).
+The weight has been uploaded in [Figshare](https://figshare.com/projects/spbnet/200692).
 
 Save the weight to your directory, such as `./ckpt/spbnet.180k.ckpt`
 
 Your directory should look like:
 
 ```txt
 - test
@@ -266,14 +319,56 @@
         ...
     - logs
         ...
     config.example.yaml
     main.py
 ```
 
+## Predict
+
+After finetune, the checkpoints and hyperparamters should be found in directory like `./tests/logs/hmof/CO2-298-2.5/version_0`. Due to that SpbNet will automatically normalize the training data during training to increase training stability. SpbNet uses mean-variance normalization. The mean and std used can be found in `.../version_0/hparams.yaml`.
+
+Based on the finetuned checkpoint and mean, std. You can predict the target property. First provide the `data_dir` and the `id_prop` csv file. The `id_prop` file should looks like
+
+```txt
+cifid
+mof1
+mof2
+...
+```
+
+Then prepare a configuration `yaml` file like
+
+```yaml
+ckpt: './logs/hmof/CO2-298-2.5/version_0/checkpoints/last.ckpt'
+data_dir: './data/spbnet'
+id_prop: './data/benchmark.test.csv' # the id_prop file
+log_dir: './predict'
+
+mean: 5.325830404166666
+std: 2.6947958848152913
+```
+
+Then predict
+
+```python
+import spbnet
+
+spbnet.predict("./config.predict.yaml")
+```
+
+The `test_results.csv` will be saved in directory like `predict/version_0`. It shoud look like
+
+```csv
+cifid,predict
+hMOF-4000155,12.504342079162598
+hMOF-5024342,2.8985860347747803
+hMOF-25731,4.6314473152160645
+```
+
 ## Visualize
 
 SpbNet provide visualization of attention score and atom grid.
 
 To visualize cif file, make a new directory and prepare a `cif` format file. Such as
 
 ```txt
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spbnet-0.0.1/spbnet.egg-info/SOURCES.txt` & `spbnet-0.0.2/spbnet.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 LICENSE.txt
 README.md
 setup.py
 spbnet/__init__.py
-spbnet/config.example.yaml
 spbnet/config.finetune.yaml
+spbnet/config.predict.yaml
 spbnet/config.pretrain.yaml
 spbnet/finetune.py
+spbnet/predict.py
 spbnet/pretrain.py
 spbnet.egg-info/PKG-INFO
 spbnet.egg-info/SOURCES.txt
 spbnet.egg-info/dependency_links.txt
 spbnet.egg-info/entry_points.txt
 spbnet.egg-info/requires.txt
 spbnet.egg-info/top_level.txt
@@ -30,14 +31,15 @@
 spbnet/data/buildAtomGrid.py
 spbnet/data/buildData.py
 spbnet/data/calcAtomNum.py
 spbnet/data/calcMeanStd.py
 spbnet/data/checkData.py
 spbnet/data/dataset.py
 spbnet/data/dataset_feat.py
+spbnet/data/dataset_predict.py
 spbnet/data/dataset_pretrain.py
 spbnet/data/filterData.py
 spbnet/data/float2int8.py
 spbnet/data/install_griday.py
 spbnet/data/prepare_data.py
 spbnet/data/libs/GRIDAY/AtomTypeMap.cpp
 spbnet/data/libs/GRIDAY/AtomTypeMap.hpp
```

