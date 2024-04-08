# Comparing `tmp/MRCpy-2.1.9.tar.gz` & `tmp/MRCpy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MRCpy-2.1.9.tar", last modified: Wed Apr  3 16:44:00 2024, max compression
+gzip compressed data, was "MRCpy-2.2.0.tar", last modified: Mon Apr  8 09:54:31 2024, max compression
```

## Comparing `MRCpy-2.1.9.tar` & `MRCpy-2.2.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-03 16:44:00.439040 MRCpy-2.1.9/
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-03 16:43:59.931137 MRCpy-2.1.9/MRCpy/
--rw-r--r--   0 kbondugula   (503) staff       (20)      245 2024-04-03 16:41:52.000000 MRCpy-2.1.9/MRCpy/__init__.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    25880 2024-04-03 16:38:29.000000 MRCpy-2.1.9/MRCpy/amrc.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    17242 2024-02-13 15:23:47.000000 MRCpy-2.1.9/MRCpy/base_mrc.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    28710 2024-02-28 16:31:33.000000 MRCpy-2.1.9/MRCpy/cmrc.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-03 16:43:59.936493 MRCpy-2.1.9/MRCpy/datasets/
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     1089 2024-01-28 20:51:11.000000 MRCpy-2.1.9/MRCpy/datasets/__init__.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-03 16:44:00.396019 MRCpy-2.1.9/MRCpy/datasets/data/
--rw-r--r--   0 kbondugula   (503) staff       (20)  7075696 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-sci_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20) 10629747 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-sci_Train.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  2002192 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-sci_shortTest.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  2002231 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  6519380 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-talk_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  9787043 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-talk_Train.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    32719 2023-04-27 10:30:22.000000 MRCpy-2.1.9/MRCpy/datasets/data/credit.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    23118 2023-04-27 10:30:22.000000 MRCpy-2.1.9/MRCpy/datasets/data/diabetes.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    16851 2023-04-27 10:30:22.000000 MRCpy-2.1.9/MRCpy/datasets/data/ecoli.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    11293 2023-04-27 10:30:22.000000 MRCpy-2.1.9/MRCpy/datasets/data/glass.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3121 2023-04-27 10:30:22.000000 MRCpy-2.1.9/MRCpy/datasets/data/haberman.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    21189 2023-04-27 10:30:22.000000 MRCpy-2.1.9/MRCpy/datasets/data/indianLiverPatient.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     4789 2023-04-27 10:30:22.000000 MRCpy-2.1.9/MRCpy/datasets/data/iris.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)   732608 2023-04-27 10:30:22.000000 MRCpy-2.1.9/MRCpy/datasets/data/letter-recognition.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    13796 2023-04-27 10:30:22.000000 MRCpy-2.1.9/MRCpy/datasets/data/mammographic.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)   834087 2023-04-27 10:30:25.000000 MRCpy-2.1.9/MRCpy/datasets/data/optdigits.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  6344664 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/rec-vs-sci_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  9534428 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/rec-vs-sci_Train.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  5788382 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/rec-vs-talk_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  8691659 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/rec-vs-talk_Train.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    85710 2023-04-27 10:30:25.000000 MRCpy-2.1.9/MRCpy/datasets/data/redwine.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  5766341 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/sci-vs-talk_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  8659812 2024-01-16 12:39:02.000000 MRCpy-2.1.9/MRCpy/datasets/data/sci-vs-talk_Train.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)   370691 2023-04-27 10:30:25.000000 MRCpy-2.1.9/MRCpy/datasets/data/segment.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)   300394 2023-04-27 10:30:25.000000 MRCpy-2.1.9/MRCpy/datasets/data/usenet2.csv
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-03 16:44:00.422389 MRCpy-2.1.9/MRCpy/datasets/descr/
--rw-r--r--   0 kbondugula   (503) staff       (20)     2106 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/adult.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     1048 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2218 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/credit.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     1102 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/diabetes.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3022 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/ecoli.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3666 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/glass.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     1535 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/haberman.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2582 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/indianLiverPatient.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2998 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/iris.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2734 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/letter-recognition.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3479 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/mammographic.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)      815 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/mnist_features_resnet18.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2388 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/optdigits.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3305 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/redwine.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     5250 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/satellite.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     2432 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/segment.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)       89 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/usenet2.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)        0 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/vehicle.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     1316 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/yearbook.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     1143 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/datasets/descr/yearbook_features_resnet18.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    52570 2024-02-09 13:02:57.000000 MRCpy-2.1.9/MRCpy/datasets/load.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    22506 2024-04-02 14:12:29.000000 MRCpy-2.1.9/MRCpy/dwgcs.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    28630 2024-02-13 15:34:58.000000 MRCpy-2.1.9/MRCpy/mrc.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-03 16:44:00.428351 MRCpy-2.1.9/MRCpy/phi/
--rw-r--r--   0 kbondugula   (503) staff       (20)      320 2024-02-09 17:31:55.000000 MRCpy-2.1.9/MRCpy/phi/__init__.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    10306 2024-01-30 14:36:53.000000 MRCpy-2.1.9/MRCpy/phi/base_phi.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     9282 2024-01-05 12:47:57.000000 MRCpy-2.1.9/MRCpy/phi/random_fourier_phi.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     9145 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/phi/random_relu_phi.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     6784 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/phi/threshold_phi.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-03 16:44:00.438304 MRCpy-2.1.9/MRCpy/solvers/
--rw-r--r--   0 kbondugula   (503) staff       (20)       82 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/solvers/__init__.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     1820 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/solvers/adam.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     9604 2024-02-12 18:48:43.000000 MRCpy-2.1.9/MRCpy/solvers/cg.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     2259 2024-02-12 18:46:27.000000 MRCpy-2.1.9/MRCpy/solvers/cvx.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    12950 2024-01-25 13:26:36.000000 MRCpy-2.1.9/MRCpy/solvers/nesterov.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     2833 2023-04-27 10:30:27.000000 MRCpy-2.1.9/MRCpy/solvers/sgd.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-03 16:43:59.934499 MRCpy-2.1.9/MRCpy.egg-info/
--rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-04-03 16:43:59.000000 MRCpy-2.1.9/MRCpy.egg-info/PKG-INFO
--rw-r--r--   0 kbondugula   (503) staff       (20)     2312 2024-04-03 16:43:59.000000 MRCpy-2.1.9/MRCpy.egg-info/SOURCES.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-04-03 16:43:59.000000 MRCpy-2.1.9/MRCpy.egg-info/dependency_links.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-04-03 16:43:59.000000 MRCpy-2.1.9/MRCpy.egg-info/not-zip-safe
--rw-r--r--   0 kbondugula   (503) staff       (20)       64 2024-04-03 16:43:59.000000 MRCpy-2.1.9/MRCpy.egg-info/requires.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)        6 2024-04-03 16:43:59.000000 MRCpy-2.1.9/MRCpy.egg-info/top_level.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-04-03 16:44:00.439547 MRCpy-2.1.9/PKG-INFO
--rw-r--r--   0 kbondugula   (503) staff       (20)     4316 2024-02-14 10:00:13.000000 MRCpy-2.1.9/README.md
--rw-r--r--   0 kbondugula   (503) staff       (20)      778 2024-04-03 16:42:34.000000 MRCpy-2.1.9/pyproject.toml
--rw-r--r--   0 kbondugula   (503) staff       (20)      160 2024-04-03 16:44:00.440568 MRCpy-2.1.9/setup.cfg
--rw-r--r--   0 kbondugula   (503) staff       (20)     2357 2024-02-14 09:37:45.000000 MRCpy-2.1.9/setup.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.810796 MRCpy-2.2.0/
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.496069 MRCpy-2.2.0/MRCpy/
+-rw-r--r--   0 kbondugula   (503) staff       (20)      245 2024-04-03 16:53:57.000000 MRCpy-2.2.0/MRCpy/__init__.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    27156 2024-04-03 16:52:42.000000 MRCpy-2.2.0/MRCpy/amrc.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    17242 2024-02-13 15:23:47.000000 MRCpy-2.2.0/MRCpy/base_mrc.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    28710 2024-02-28 16:31:33.000000 MRCpy-2.2.0/MRCpy/cmrc.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.500474 MRCpy-2.2.0/MRCpy/datasets/
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     1089 2024-01-28 20:51:11.000000 MRCpy-2.2.0/MRCpy/datasets/__init__.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.787275 MRCpy-2.2.0/MRCpy/datasets/data/
+-rw-r--r--   0 kbondugula   (503) staff       (20)  7075696 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20) 10629747 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_Train.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  2002192 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_shortTest.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  2002231 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  6519380 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-talk_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  9787043 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-talk_Train.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    32719 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/credit.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    23118 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/diabetes.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    16851 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/ecoli.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    11293 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/glass.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3121 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/haberman.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    21189 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/indianLiverPatient.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     4789 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/iris.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)   732608 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/letter-recognition.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    13796 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/mammographic.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)   834087 2023-04-27 10:30:25.000000 MRCpy-2.2.0/MRCpy/datasets/data/optdigits.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  6344664 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-sci_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  9534428 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-sci_Train.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  5788382 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-talk_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  8691659 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-talk_Train.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    85710 2023-04-27 10:30:25.000000 MRCpy-2.2.0/MRCpy/datasets/data/redwine.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  5766341 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/sci-vs-talk_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  8659812 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/sci-vs-talk_Train.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)   370691 2023-04-27 10:30:25.000000 MRCpy-2.2.0/MRCpy/datasets/data/segment.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)   300394 2023-04-27 10:30:25.000000 MRCpy-2.2.0/MRCpy/datasets/data/usenet2.csv
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.801458 MRCpy-2.2.0/MRCpy/datasets/descr/
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2106 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/adult.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1048 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2218 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/credit.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     1102 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/diabetes.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3022 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/ecoli.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3666 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/glass.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     1535 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/haberman.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2582 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/indianLiverPatient.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2998 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/iris.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2734 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/letter-recognition.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3479 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/mammographic.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)      815 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/mnist_features_resnet18.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2388 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/optdigits.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3305 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/redwine.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     5250 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/satellite.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2432 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/segment.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)       89 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/usenet2.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)        0 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/vehicle.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1316 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/yearbook.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1143 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/yearbook_features_resnet18.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    52570 2024-02-09 13:02:57.000000 MRCpy-2.2.0/MRCpy/datasets/load.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    22506 2024-04-02 14:12:29.000000 MRCpy-2.2.0/MRCpy/dwgcs.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    28630 2024-02-13 15:34:58.000000 MRCpy-2.2.0/MRCpy/mrc.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.805497 MRCpy-2.2.0/MRCpy/phi/
+-rw-r--r--   0 kbondugula   (503) staff       (20)      320 2024-02-09 17:31:55.000000 MRCpy-2.2.0/MRCpy/phi/__init__.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    10306 2024-01-30 14:36:53.000000 MRCpy-2.2.0/MRCpy/phi/base_phi.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     9282 2024-01-05 12:47:57.000000 MRCpy-2.2.0/MRCpy/phi/random_fourier_phi.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     9145 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/phi/random_relu_phi.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     6784 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/phi/threshold_phi.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.810465 MRCpy-2.2.0/MRCpy/solvers/
+-rw-r--r--   0 kbondugula   (503) staff       (20)       82 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/solvers/__init__.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1820 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/solvers/adam.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     9604 2024-02-12 18:48:43.000000 MRCpy-2.2.0/MRCpy/solvers/cg.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2259 2024-02-12 18:46:27.000000 MRCpy-2.2.0/MRCpy/solvers/cvx.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    12950 2024-01-25 13:26:36.000000 MRCpy-2.2.0/MRCpy/solvers/nesterov.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2833 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/solvers/sgd.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.499222 MRCpy-2.2.0/MRCpy.egg-info/
+-rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/PKG-INFO
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2312 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/not-zip-safe
+-rw-r--r--   0 kbondugula   (503) staff       (20)       64 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/requires.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)        6 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/top_level.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-04-08 09:54:31.810941 MRCpy-2.2.0/PKG-INFO
+-rw-r--r--   0 kbondugula   (503) staff       (20)     4316 2024-02-14 10:00:13.000000 MRCpy-2.2.0/README.md
+-rw-r--r--   0 kbondugula   (503) staff       (20)      778 2024-04-03 16:53:29.000000 MRCpy-2.2.0/pyproject.toml
+-rw-r--r--   0 kbondugula   (503) staff       (20)      160 2024-04-08 09:54:31.811552 MRCpy-2.2.0/setup.cfg
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2357 2024-02-14 09:37:45.000000 MRCpy-2.2.0/setup.py
```

### Comparing `MRCpy-2.1.9/MRCpy/amrc.py` & `MRCpy-2.2.0/MRCpy/amrc.py`

 * *Files 4% similar despite different names*

```diff
@@ -613,14 +613,52 @@
         self.minimax_risk(x, tau_, lambda_, self.n_classes)
 
         self.sample_counter = self.sample_counter + 1
 
         self.is_fitted_ = True
         return self
 
+    def predict(self, X):
+        '''
+        Predicts classes for new instances using a fitted model.
+
+        Returns the predicted classes for the given instances in `X`
+        using the probabilities given by the function `predict_proba`.
+
+        Parameters
+        ----------
+        X : `array`-like of shape (`n_features`)
+            Test instance for to predict by the AMRC model.
+
+        Returns
+        -------
+        y_pred : `int`
+            Predicted labels corresponding to the given instances.
+        '''
+
+        X = check_array(X, accept_sparse=True, ensure_2d=False)
+        check_is_fitted(self, "is_fitted_")
+
+        # Get the prediction probabilities for the classifier
+        proba = self.predict_proba(X)
+
+        if self.deterministic:
+            y_pred = np.argmax(proba)
+        else:
+            np.random.seed(self.random_state)
+            y_pred = np.random.choice(self.n_classes, p=proba)
+
+        # Check if the labels were provided for fitting
+        # (labels might be omitted if fitting is done through minimax_risk)
+        # Otherwise return the default labels i.e., from 0 to n_classes-1.
+        if hasattr(self, 'classes_'):
+            y_pred = np.asarray([self.classes_[label] for label in y_pred])
+
+        return y_pred
+
     def predict_proba(self, x):
         '''
         Conditional probabilities corresponding to each class
         for each unlabeled input instance
 
         Parameters
         ----------
```

### Comparing `MRCpy-2.1.9/MRCpy/base_mrc.py` & `MRCpy-2.2.0/MRCpy/base_mrc.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/cmrc.py` & `MRCpy-2.2.0/MRCpy/cmrc.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/__init__.py` & `MRCpy-2.2.0/MRCpy/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-sci_Test.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-sci_Train.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-sci_shortTest.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_shortTest.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-talk_Test.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-talk_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/comp-vs-talk_Train.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-talk_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/credit.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/credit.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/diabetes.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/diabetes.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/ecoli.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/ecoli.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/glass.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/glass.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/haberman.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/haberman.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/indianLiverPatient.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/indianLiverPatient.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/iris.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/iris.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/letter-recognition.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/letter-recognition.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/mammographic.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/mammographic.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/optdigits.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/optdigits.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/rec-vs-sci_Test.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-sci_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/rec-vs-sci_Train.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-sci_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/rec-vs-talk_Test.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-talk_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/rec-vs-talk_Train.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-talk_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/redwine.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/redwine.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/sci-vs-talk_Test.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/sci-vs-talk_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/sci-vs-talk_Train.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/sci-vs-talk_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/segment.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/segment.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/data/usenet2.csv` & `MRCpy-2.2.0/MRCpy/datasets/data/usenet2.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/adult.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/adult.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/credit.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/credit.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/diabetes.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/diabetes.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/ecoli.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/ecoli.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/glass.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/glass.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/haberman.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/haberman.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/indianLiverPatient.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/indianLiverPatient.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/iris.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/iris.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/letter-recognition.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/letter-recognition.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/mammographic.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/mammographic.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/mnist_features_resnet18.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/mnist_features_resnet18.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/optdigits.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/optdigits.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/redwine.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/redwine.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/satellite.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/satellite.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/segment.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/segment.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/yearbook.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/yearbook.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/descr/yearbook_features_resnet18.rst` & `MRCpy-2.2.0/MRCpy/datasets/descr/yearbook_features_resnet18.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/datasets/load.py` & `MRCpy-2.2.0/MRCpy/datasets/load.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/dwgcs.py` & `MRCpy-2.2.0/MRCpy/dwgcs.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/mrc.py` & `MRCpy-2.2.0/MRCpy/mrc.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/phi/base_phi.py` & `MRCpy-2.2.0/MRCpy/phi/base_phi.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/phi/random_fourier_phi.py` & `MRCpy-2.2.0/MRCpy/phi/random_fourier_phi.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/phi/random_relu_phi.py` & `MRCpy-2.2.0/MRCpy/phi/random_relu_phi.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/phi/threshold_phi.py` & `MRCpy-2.2.0/MRCpy/phi/threshold_phi.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/solvers/adam.py` & `MRCpy-2.2.0/MRCpy/solvers/adam.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/solvers/cg.py` & `MRCpy-2.2.0/MRCpy/solvers/cg.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/solvers/cvx.py` & `MRCpy-2.2.0/MRCpy/solvers/cvx.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/solvers/nesterov.py` & `MRCpy-2.2.0/MRCpy/solvers/nesterov.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy/solvers/sgd.py` & `MRCpy-2.2.0/MRCpy/solvers/sgd.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/MRCpy.egg-info/PKG-INFO` & `MRCpy-2.2.0/MRCpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MRCpy
-Version: 2.1.9
+Version: 2.2.0
 Summary: Library for minimax risk classifiers
 Home-page: https://github.com/MachineLearningBCAM/MRCpy
 Author-email: Kartheek Bondugula <kbondugula@bcamath.org>
 Project-URL: Homepage, https://github.com/MachineLearningBCAM/MRCpy
 Project-URL: Issues, https://github.com/MachineLearningBCAM/MRCpy/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `MRCpy-2.1.9/MRCpy.egg-info/SOURCES.txt` & `MRCpy-2.2.0/MRCpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/PKG-INFO` & `MRCpy-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MRCpy
-Version: 2.1.9
+Version: 2.2.0
 Summary: Library for minimax risk classifiers
 Home-page: https://github.com/MachineLearningBCAM/MRCpy
 Author-email: Kartheek Bondugula <kbondugula@bcamath.org>
 Project-URL: Homepage, https://github.com/MachineLearningBCAM/MRCpy
 Project-URL: Issues, https://github.com/MachineLearningBCAM/MRCpy/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `MRCpy-2.1.9/README.md` & `MRCpy-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.9/pyproject.toml` & `MRCpy-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "MRCpy"
-version = "2.1.9"
+version = "2.2.0"
 authors = [
   { name="Kartheek Bondugula", email="kbondugula@bcamath.org" },
 ]
 description = "Library for minimax risk classifiers"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `MRCpy-2.1.9/setup.py` & `MRCpy-2.2.0/setup.py`

 * *Files identical despite different names*

