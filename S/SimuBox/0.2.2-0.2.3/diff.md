# Comparing `tmp/simubox-0.2.2.tar.gz` & `tmp/simubox-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simubox-0.2.2.tar", max compression
+gzip compressed data, was "simubox-0.2.3.tar", max compression
```

## Comparing `simubox-0.2.2.tar` & `simubox-0.2.3.tar`

### file list

```diff
@@ -1,103 +1,61 @@
--rw-r--r--   0        0        0     1093 2023-12-15 10:21:19.938760 simubox-0.2.2/LICENSE
--rw-r--r--   0        0        0     1306 2024-04-03 14:57:54.022478 simubox-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1041 2024-03-31 14:56:23.293212 simubox-0.2.2/README.md
--rw-r--r--   0        0        0      121 2024-03-27 15:55:02.995962 simubox-0.2.2/SimuBox/__init__.py
--rw-r--r--   0        0        0      123 2023-12-15 06:14:16.190366 simubox-0.2.2/SimuBox/artist/__init__.py
--rw-r--r--   0        0        0      349 2023-12-16 12:36:51.060186 simubox-0.2.2/SimuBox/artist/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16341 2024-03-27 14:37:31.902620 simubox-0.2.2/SimuBox/artist/__pycache__/compare.cpython-311.pyc
--rw-r--r--   0        0        0    11781 2024-04-03 13:22:01.628417 simubox-0.2.2/SimuBox/artist/__pycache__/isosurface.cpython-311.pyc
--rw-r--r--   0        0        0    15122 2024-04-03 13:20:27.256228 simubox-0.2.2/SimuBox/artist/__pycache__/landscape.cpython-311.pyc
--rw-r--r--   0        0        0    28412 2024-04-03 13:48:55.642974 simubox-0.2.2/SimuBox/artist/__pycache__/phase.cpython-311.pyc
--rw-r--r--   0        0        0     7600 2024-03-27 07:18:20.947746 simubox-0.2.2/SimuBox/artist/__pycache__/plotter.cpython-311.pyc
--rw-r--r--   0        0        0    11867 2024-03-27 14:22:19.156738 simubox-0.2.2/SimuBox/artist/compare.py
--rw-r--r--   0        0        0     7517 2024-04-03 10:55:55.772588 simubox-0.2.2/SimuBox/artist/isosurface.py
--rw-r--r--   0        0        0     9899 2024-04-03 10:55:55.760588 simubox-0.2.2/SimuBox/artist/landscape.py
--rw-r--r--   0        0        0    23671 2024-04-03 13:48:54.363411 simubox-0.2.2/SimuBox/artist/phase.py
--rw-r--r--   0        0        0     3939 2024-03-27 06:33:49.453914 simubox-0.2.2/SimuBox/artist/plotter.py
--rw-r--r--   0        0        0       90 2023-12-15 06:14:16.182366 simubox-0.2.2/SimuBox/calculator/__init__.py
--rw-r--r--   0        0        0      315 2023-12-16 12:36:50.973187 simubox-0.2.2/SimuBox/calculator/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8682 2024-04-03 13:22:02.266551 simubox-0.2.2/SimuBox/calculator/__pycache__/peak.cpython-311.pyc
--rw-r--r--   0        0        0     9168 2024-03-30 13:53:39.106115 simubox-0.2.2/SimuBox/calculator/__pycache__/scatter.cpython-311.pyc
--rw-r--r--   0        0        0    37861 2024-03-30 13:53:40.051251 simubox-0.2.2/SimuBox/calculator/__pycache__/topo.cpython-311.pyc
--rw-r--r--   0        0        0    17589 2024-03-30 13:53:37.025659 simubox-0.2.2/SimuBox/calculator/__pycache__/voronoi.cpython-311.pyc
--rw-r--r--   0        0        0     4478 2024-04-03 10:55:55.752589 simubox-0.2.2/SimuBox/calculator/peak.py
--rw-r--r--   0        0        0     5485 2024-03-27 15:55:02.982758 simubox-0.2.2/SimuBox/calculator/scatter.py
--rw-r--r--   0        0        0    26322 2024-03-27 15:55:02.975777 simubox-0.2.2/SimuBox/calculator/topo.py
--rw-r--r--   0        0        0    11281 2024-03-27 15:55:02.985758 simubox-0.2.2/SimuBox/calculator/voronoi.py
--rw-r--r--   0        0        0       70 2024-04-03 10:11:34.170669 simubox-0.2.2/SimuBox/runner/__init__.py
--rw-r--r--   0        0        0      286 2024-04-03 10:35:11.919414 simubox-0.2.2/SimuBox/runner/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    13355 2024-04-03 10:35:11.935246 simubox-0.2.2/SimuBox/runner/__pycache__/manager.cpython-311.pyc
--rw-r--r--   0        0        0     5176 2024-04-03 10:35:11.926591 simubox-0.2.2/SimuBox/runner/__pycache__/phases.cpython-311.pyc
--rw-r--r--   0        0        0      175 2023-11-28 10:41:26.055035 simubox-0.2.2/SimuBox/runner/agents/__init__.py
--rw-r--r--   0        0        0      473 2023-12-16 12:36:53.403339 simubox-0.2.2/SimuBox/runner/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4294 2023-12-16 12:36:53.405338 simubox-0.2.2/SimuBox/runner/agents/__pycache__/ABC.cpython-311.pyc
--rw-r--r--   0        0        0     5690 2024-04-03 10:35:11.929260 simubox-0.2.2/SimuBox/runner/agents/__pycache__/ABC_ABC.cpython-311.pyc
--rw-r--r--   0        0        0     4864 2024-04-03 10:35:11.931247 simubox-0.2.2/SimuBox/runner/agents/__pycache__/BABCB.cpython-311.pyc
--rw-r--r--   0        0        0     1727 2023-12-16 12:36:53.420340 simubox-0.2.2/SimuBox/runner/agents/__pycache__/Mask_AB_A.cpython-311.pyc
--rw-r--r--   0        0        0     1863 2023-12-16 12:36:53.421338 simubox-0.2.2/SimuBox/runner/agents/__pycache__/Mask_AB_AB.cpython-311.pyc
--rw-r--r--   0        0        0     5531 2024-04-03 10:35:11.923591 simubox-0.2.2/SimuBox/runner/agents/__pycache__/MixinModel.cpython-311.pyc
--rw-r--r--   0        0        0     4272 2023-11-27 15:25:46.282729 simubox-0.2.2/SimuBox/runner/agents/ABC.py
--rw-r--r--   0        0        0     5250 2024-04-03 10:14:35.582991 simubox-0.2.2/SimuBox/runner/agents/ABC_ABC.py
--rw-r--r--   0        0        0     4707 2024-04-03 10:15:02.275022 simubox-0.2.2/SimuBox/runner/agents/BABCB.py
--rw-r--r--   0        0        0     1115 2023-11-27 15:27:54.239348 simubox-0.2.2/SimuBox/runner/agents/Mask_AB_A.py
--rw-r--r--   0        0        0     1226 2023-11-27 15:27:54.236347 simubox-0.2.2/SimuBox/runner/agents/Mask_AB_AB.py
--rw-r--r--   0        0        0     2125 2024-04-03 10:11:34.173663 simubox-0.2.2/SimuBox/runner/agents/MixinModel.py
--rw-r--r--   0        0        0     8023 2024-03-27 15:35:53.930084 simubox-0.2.2/SimuBox/runner/manager.py
--rw-r--r--   0        0        0    14973 2023-08-31 09:07:40.697135 simubox-0.2.2/SimuBox/runner/phases.py
--rw-r--r--   0        0        0       91 2024-03-27 06:33:49.409890 simubox-0.2.2/SimuBox/schema/__init__.py
--rw-r--r--   0        0        0      312 2024-03-27 07:17:01.284000 simubox-0.2.2/SimuBox/schema/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1641 2024-03-27 14:36:51.896843 simubox-0.2.2/SimuBox/schema/__pycache__/labels.cpython-311.pyc
--rw-r--r--   0        0        0      797 2024-04-03 13:20:26.787918 simubox-0.2.2/SimuBox/schema/__pycache__/types.cpython-311.pyc
--rw-r--r--   0        0        0      100 2024-03-27 15:28:15.928633 simubox-0.2.2/SimuBox/schema/enums/__init__.py
--rw-r--r--   0        0        0      329 2024-03-27 15:35:54.898985 simubox-0.2.2/SimuBox/schema/enums/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2672 2024-03-27 14:36:51.220564 simubox-0.2.2/SimuBox/schema/enums/__pycache__/MixinEnums.cpython-311.pyc
--rw-r--r--   0        0        0     2492 2024-03-27 15:35:54.901985 simubox-0.2.2/SimuBox/schema/enums/__pycache__/Modes.cpython-311.pyc
--rw-r--r--   0        0        0     1503 2024-03-27 15:35:54.904985 simubox-0.2.2/SimuBox/schema/enums/__pycache__/OtherEnums.cpython-311.pyc
--rw-r--r--   0        0        0     1374 2024-03-27 15:38:31.041914 simubox-0.2.2/SimuBox/schema/enums/__pycache__/SCFTEnums.cpython-311.pyc
--rw-r--r--   0        0        0      955 2024-03-27 14:18:43.001269 simubox-0.2.2/SimuBox/schema/enums/MixinEnums.py
--rw-r--r--   0        0        0     1167 2024-03-27 15:27:06.701601 simubox-0.2.2/SimuBox/schema/enums/Modes.py
--rw-r--r--   0        0        0      560 2024-03-27 15:28:15.922643 simubox-0.2.2/SimuBox/schema/enums/OtherEnums.py
--rw-r--r--   0        0        0      525 2024-03-27 15:36:57.283600 simubox-0.2.2/SimuBox/schema/enums/SCFTEnums.py
--rw-r--r--   0        0        0     1787 2024-03-27 14:18:43.242800 simubox-0.2.2/SimuBox/schema/labels.py
--rw-r--r--   0        0        0      168 2024-03-27 15:36:35.497459 simubox-0.2.2/SimuBox/schema/structs/__init__.py
--rw-r--r--   0        0        0      407 2024-03-27 15:38:31.043914 simubox-0.2.2/SimuBox/schema/structs/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3863 2024-03-27 14:36:51.620609 simubox-0.2.2/SimuBox/schema/structs/__pycache__/ChartElement.cpython-311.pyc
--rw-r--r--   0        0        0     4110 2024-03-27 14:36:51.628615 simubox-0.2.2/SimuBox/schema/structs/__pycache__/ComputedRes.cpython-311.pyc
--rw-r--r--   0        0        0    11753 2024-03-31 13:25:05.993963 simubox-0.2.2/SimuBox/schema/structs/__pycache__/DataFile.cpython-311.pyc
--rw-r--r--   0        0        0     1499 2024-03-27 14:36:51.229567 simubox-0.2.2/SimuBox/schema/structs/__pycache__/MixinStructs.cpython-311.pyc
--rw-r--r--   0        0        0     1517 2024-04-03 13:53:57.781385 simubox-0.2.2/SimuBox/schema/structs/__pycache__/OtherStructs.cpython-311.pyc
--rw-r--r--   0        0        0     2767 2024-03-27 15:35:57.965475 simubox-0.2.2/SimuBox/schema/structs/__pycache__/SCFTStructs.cpython-311.pyc
--rw-r--r--   0        0        0     1736 2024-03-27 13:56:42.637867 simubox-0.2.2/SimuBox/schema/structs/ChartElement.py
--rw-r--r--   0        0        0     1556 2024-03-27 13:56:42.621775 simubox-0.2.2/SimuBox/schema/structs/ComputedRes.py
--rw-r--r--   0        0        0     6653 2024-03-31 13:00:07.546755 simubox-0.2.2/SimuBox/schema/structs/DataFile.py
--rw-r--r--   0        0        0      539 2024-03-27 14:10:13.621470 simubox-0.2.2/SimuBox/schema/structs/MixinStructs.py
--rw-r--r--   0        0        0      724 2024-04-03 13:53:56.680819 simubox-0.2.2/SimuBox/schema/structs/OtherStructs.py
--rw-r--r--   0        0        0     1384 2024-03-27 15:33:02.256233 simubox-0.2.2/SimuBox/schema/structs/SCFTStructs.py
--rw-r--r--   0        0        0      395 2024-04-03 11:46:43.830219 simubox-0.2.2/SimuBox/schema/types.py
--rw-r--r--   0        0        0     1376 2024-03-30 13:54:41.972260 simubox-0.2.2/SimuBox/scripts/__pycache__/web.cpython-311.pyc
--rw-r--r--   0        0        0    10088 2024-03-27 16:07:33.010245 simubox-0.2.2/SimuBox/scripts/extractor.py
--rw-r--r--   0        0        0     7048 2023-11-27 14:34:10.698773 simubox-0.2.2/SimuBox/scripts/JSON/ABC_ABC.json
--rw-r--r--   0        0        0     5195 2023-08-31 09:07:40.762862 simubox-0.2.2/SimuBox/scripts/JSON/BABCB.json
--rw-r--r--   0        0        0      762 2024-03-27 15:45:09.773000 simubox-0.2.2/SimuBox/scripts/push_job.py
--rw-r--r--   0        0        0     1177 2024-03-27 16:07:33.006243 simubox-0.2.2/SimuBox/scripts/setenv.py
--rw-r--r--   0        0        0      721 2024-03-27 16:02:20.309904 simubox-0.2.2/SimuBox/scripts/web.py
--rw-r--r--   0        0        0       96 2024-03-30 13:53:03.208828 simubox-0.2.2/SimuBox/toolkits/__init__.py
--rw-r--r--   0        0        0      319 2024-03-30 13:53:34.064029 simubox-0.2.2/SimuBox/toolkits/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5824 2024-04-03 13:53:57.785384 simubox-0.2.2/SimuBox/toolkits/__pycache__/function.cpython-311.pyc
--rw-r--r--   0        0        0    18649 2024-04-03 13:20:25.500768 simubox-0.2.2/SimuBox/toolkits/__pycache__/reader.cpython-311.pyc
--rw-r--r--   0        0        0     3360 2024-03-31 14:54:12.302611 simubox-0.2.2/SimuBox/toolkits/__pycache__/vector.cpython-311.pyc
--rw-r--r--   0        0        0     9742 2024-04-03 10:35:08.059803 simubox-0.2.2/SimuBox/toolkits/__pycache__/xmltrans.cpython-311.pyc
--rw-r--r--   0        0        0     3786 2024-04-03 13:52:28.451854 simubox-0.2.2/SimuBox/toolkits/function.py
--rw-r--r--   0        0        0    12058 2024-04-03 12:27:05.411475 simubox-0.2.2/SimuBox/toolkits/reader.py
--rw-r--r--   0        0        0     2544 2024-03-31 14:52:59.828684 simubox-0.2.2/SimuBox/toolkits/vector.py
--rw-r--r--   0        0        0     5008 2024-04-03 03:44:10.626375 simubox-0.2.2/SimuBox/toolkits/xmltrans.py
--rw-r--r--   0        0        0    74833 2024-03-31 14:46:18.268516 simubox-0.2.2/SimuBox/web/cache/iso3d_NaCl_phin_0.svg
--rw-r--r--   0        0        0     1702 2024-03-27 14:41:55.709897 simubox-0.2.2/SimuBox/web/Homepage.py
--rw-r--r--   0        0        0     7440 2024-03-31 14:46:11.631170 simubox-0.2.2/SimuBox/web/pages/1_Structure.py
--rw-r--r--   0        0        0     8275 2024-03-27 14:42:26.986772 simubox-0.2.2/SimuBox/web/pages/2_Scatter.py
--rw-r--r--   0        0        0     8964 2024-03-27 14:41:55.704414 simubox-0.2.2/SimuBox/web/pages/3_Voronoi.py
--rw-r--r--   0        0        0     6080 2024-03-27 14:41:55.694890 simubox-0.2.2/SimuBox/web/pages/4_Curve.py
--rw-r--r--   0        0        0     7409 2024-03-27 14:41:55.707413 simubox-0.2.2/SimuBox/web/pages/5_Peaks.py
--rw-r--r--   0        0        0     7029 2024-03-27 14:41:55.698889 simubox-0.2.2/SimuBox/web/pages/6_Topology.py
--rw-r--r--   0        0        0     4057 2024-03-27 14:41:55.701413 simubox-0.2.2/SimuBox/web/pages/7_Landscape.py
--rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 simubox-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-12-15 10:21:19.938760 simubox-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1306 2024-04-08 13:52:19.103630 simubox-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1041 2024-03-31 14:56:23.293212 simubox-0.2.3/README.md
+-rw-r--r--   0        0        0      120 2024-04-06 14:56:53.385803 simubox-0.2.3/SimuBox/__init__.py
+-rw-r--r--   0        0        0      123 2023-12-15 06:14:16.190366 simubox-0.2.3/SimuBox/artist/__init__.py
+-rw-r--r--   0        0        0    11866 2024-04-06 14:56:53.391791 simubox-0.2.3/SimuBox/artist/compare.py
+-rw-r--r--   0        0        0     7516 2024-04-06 14:56:53.403311 simubox-0.2.3/SimuBox/artist/isosurface.py
+-rw-r--r--   0        0        0     9898 2024-04-06 14:56:53.407312 simubox-0.2.3/SimuBox/artist/landscape.py
+-rw-r--r--   0        0        0    23670 2024-04-06 14:56:53.397800 simubox-0.2.3/SimuBox/artist/phase.py
+-rw-r--r--   0        0        0     3939 2024-03-27 06:33:49.453914 simubox-0.2.3/SimuBox/artist/plotter.py
+-rw-r--r--   0        0        0       90 2023-12-15 06:14:16.182366 simubox-0.2.3/SimuBox/calculator/__init__.py
+-rw-r--r--   0        0        0     4478 2024-04-03 10:55:55.752589 simubox-0.2.3/SimuBox/calculator/peak.py
+-rw-r--r--   0        0        0     5484 2024-04-06 14:56:53.416335 simubox-0.2.3/SimuBox/calculator/scatter.py
+-rw-r--r--   0        0        0    26322 2024-03-27 15:55:02.975777 simubox-0.2.3/SimuBox/calculator/topo.py
+-rw-r--r--   0        0        0    11280 2024-04-06 14:56:53.412310 simubox-0.2.3/SimuBox/calculator/voronoi.py
+-rw-r--r--   0        0        0       70 2024-04-03 10:11:34.170669 simubox-0.2.3/SimuBox/runner/__init__.py
+-rw-r--r--   0        0        0      175 2023-11-28 10:41:26.055035 simubox-0.2.3/SimuBox/runner/agents/__init__.py
+-rw-r--r--   0        0        0     4272 2023-11-27 15:25:46.282729 simubox-0.2.3/SimuBox/runner/agents/ABC.py
+-rw-r--r--   0        0        0     5250 2024-04-03 10:14:35.582991 simubox-0.2.3/SimuBox/runner/agents/ABC_ABC.py
+-rw-r--r--   0        0        0     4707 2024-04-03 10:15:02.275022 simubox-0.2.3/SimuBox/runner/agents/BABCB.py
+-rw-r--r--   0        0        0     1115 2023-11-27 15:27:54.239348 simubox-0.2.3/SimuBox/runner/agents/Mask_AB_A.py
+-rw-r--r--   0        0        0     1226 2023-11-27 15:27:54.236347 simubox-0.2.3/SimuBox/runner/agents/Mask_AB_AB.py
+-rw-r--r--   0        0        0     2125 2024-04-03 10:11:34.173663 simubox-0.2.3/SimuBox/runner/agents/MixinModel.py
+-rw-r--r--   0        0        0     8023 2024-03-27 15:35:53.930084 simubox-0.2.3/SimuBox/runner/manager.py
+-rw-r--r--   0        0        0    14973 2023-08-31 09:07:40.697135 simubox-0.2.3/SimuBox/runner/phases.py
+-rw-r--r--   0        0        0       91 2024-03-27 06:33:49.409890 simubox-0.2.3/SimuBox/schema/__init__.py
+-rw-r--r--   0        0        0      100 2024-03-27 15:28:15.928633 simubox-0.2.3/SimuBox/schema/enums/__init__.py
+-rw-r--r--   0        0        0      955 2024-03-27 14:18:43.001269 simubox-0.2.3/SimuBox/schema/enums/MixinEnums.py
+-rw-r--r--   0        0        0     1167 2024-03-27 15:27:06.701601 simubox-0.2.3/SimuBox/schema/enums/Modes.py
+-rw-r--r--   0        0        0      560 2024-03-27 15:28:15.922643 simubox-0.2.3/SimuBox/schema/enums/OtherEnums.py
+-rw-r--r--   0        0        0      525 2024-03-27 15:36:57.283600 simubox-0.2.3/SimuBox/schema/enums/SCFTEnums.py
+-rw-r--r--   0        0        0     1787 2024-03-27 14:18:43.242800 simubox-0.2.3/SimuBox/schema/labels.py
+-rw-r--r--   0        0        0      168 2024-03-27 15:36:35.497459 simubox-0.2.3/SimuBox/schema/structs/__init__.py
+-rw-r--r--   0        0        0     1736 2024-03-27 13:56:42.637867 simubox-0.2.3/SimuBox/schema/structs/ChartElement.py
+-rw-r--r--   0        0        0     1556 2024-03-27 13:56:42.621775 simubox-0.2.3/SimuBox/schema/structs/ComputedRes.py
+-rw-r--r--   0        0        0     6653 2024-03-31 13:00:07.546755 simubox-0.2.3/SimuBox/schema/structs/DataFile.py
+-rw-r--r--   0        0        0      539 2024-03-27 14:10:13.621470 simubox-0.2.3/SimuBox/schema/structs/MixinStructs.py
+-rw-r--r--   0        0        0      724 2024-04-03 13:53:56.680819 simubox-0.2.3/SimuBox/schema/structs/OtherStructs.py
+-rw-r--r--   0        0        0     1428 2024-04-04 09:02:53.467218 simubox-0.2.3/SimuBox/schema/structs/SCFTStructs.py
+-rw-r--r--   0        0        0      395 2024-04-03 11:46:43.830219 simubox-0.2.3/SimuBox/schema/types.py
+-rw-r--r--   0        0        0    10336 2024-04-08 13:48:36.367296 simubox-0.2.3/SimuBox/script/extractor.py
+-rw-r--r--   0        0        0      814 2024-04-06 15:48:07.272692 simubox-0.2.3/SimuBox/script/help.py
+-rw-r--r--   0        0        0     7048 2023-11-27 14:34:10.698773 simubox-0.2.3/SimuBox/script/JSON/ABC_ABC.json
+-rw-r--r--   0        0        0     5195 2023-08-31 09:07:40.762862 simubox-0.2.3/SimuBox/script/JSON/BABCB.json
+-rw-r--r--   0        0        0      661 2024-04-04 10:29:51.574406 simubox-0.2.3/SimuBox/script/push_job.py
+-rw-r--r--   0        0        0     1655 2024-04-06 15:49:41.998603 simubox-0.2.3/SimuBox/script/setenv.py
+-rw-r--r--   0        0        0      848 2024-04-06 15:09:04.736704 simubox-0.2.3/SimuBox/script/web.py
+-rw-r--r--   0        0        0       96 2024-03-30 13:53:03.208828 simubox-0.2.3/SimuBox/toolkit/__init__.py
+-rw-r--r--   0        0        0     3786 2024-04-03 13:52:28.451854 simubox-0.2.3/SimuBox/toolkit/function.py
+-rw-r--r--   0        0        0    12058 2024-04-03 12:27:05.411475 simubox-0.2.3/SimuBox/toolkit/reader.py
+-rw-r--r--   0        0        0     2544 2024-03-31 14:52:59.828684 simubox-0.2.3/SimuBox/toolkit/vector.py
+-rw-r--r--   0        0        0     5008 2024-04-03 03:44:10.626375 simubox-0.2.3/SimuBox/toolkit/xmltrans.py
+-rw-r--r--   0        0        0     1702 2024-03-27 14:41:55.709897 simubox-0.2.3/SimuBox/web/Homepage.py
+-rw-r--r--   0        0        0     7440 2024-03-31 14:46:11.631170 simubox-0.2.3/SimuBox/web/pages/1_Structure.py
+-rw-r--r--   0        0        0     8275 2024-03-27 14:42:26.986772 simubox-0.2.3/SimuBox/web/pages/2_Scatter.py
+-rw-r--r--   0        0        0     8964 2024-03-27 14:41:55.704414 simubox-0.2.3/SimuBox/web/pages/3_Voronoi.py
+-rw-r--r--   0        0        0     6080 2024-03-27 14:41:55.694890 simubox-0.2.3/SimuBox/web/pages/4_Curve.py
+-rw-r--r--   0        0        0     7409 2024-03-27 14:41:55.707413 simubox-0.2.3/SimuBox/web/pages/5_Peaks.py
+-rw-r--r--   0        0        0     7029 2024-03-27 14:41:55.698889 simubox-0.2.3/SimuBox/web/pages/6_Topology.py
+-rw-r--r--   0        0        0     4057 2024-03-27 14:41:55.701413 simubox-0.2.3/SimuBox/web/pages/7_Landscape.py
+-rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 simubox-0.2.3/PKG-INFO
```

### Comparing `simubox-0.2.2/LICENSE` & `simubox-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/pyproject.toml` & `simubox-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SimuBox"
-version = "0.2.2"
+version = "0.2.3"
 description = "Free python package to do some science calculation."
 authors = ["Alkaid Yuan <kryuan@qq.com>"]
 maintainers = ["Alkaid Yuan <kryuan@qq.com>"]
 license = "./LICENSE"
 readme = "./README.md"
 repository  = "https://github.com/KangruiYuan/SimuBox"
 homepage = "https://pypi.org/project/SimuBox/"
```

### Comparing `simubox-0.2.2/README.md` & `simubox-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/artist/compare.py` & `simubox-0.2.3/SimuBox/artist/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from cycler import cycler
 
 from collections import ChainMap
 
-from ..toolkits import read_csv
+from ..toolkit import read_csv
 from ..schema import AbsCommonLabels, DiffCommonLabels, LineCompareResult, Line, PathLike
 from .plotter import plot_trans, plot_legend, plot_locators, plot_savefig
 
 COMPARE_PLOT_CONFIG = {
     "font.family": "Times New Roman",
     # "font.family":'serif',
     "font.serif": ["SimSun"],
```

### Comparing `simubox-0.2.2/SimuBox/artist/isosurface.py` & `simubox-0.2.3/SimuBox/artist/isosurface.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pyvista as pv
 from skimage.measure import marching_cubes
 
 from .plotter import plot_savefig
 from ..schema import Density, RealNum, PathLike, DensityParseResult
-from ..toolkits import parse_density
+from ..toolkit import parse_density
 
 __all__ = ["iso2D", "iso3D"]
 
 def iso3D(
     density: Union[Density, DensityParseResult],
     target: Optional[Union[int, Iterable[int]]] = 0,
     permute: Optional[Iterable[int]] = None,
```

### Comparing `simubox-0.2.2/SimuBox/artist/landscape.py` & `simubox-0.2.3/SimuBox/artist/landscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import pandas as pd
 from scipy.interpolate import griddata
 from shapely.geometry import Polygon
 
 from .plotter import plot_locators, plot_savefig
 from ..schema import LandscapeResult, PathLike, CommonLabels, RealNum, Vector, Contour
-from ..toolkits import read_csv, find_nearest_1d
+from ..toolkit import read_csv, find_nearest_1d
 
 LAND_PLOT_CONFIG = {
     "font.family": "Times New Roman",
     "font.size": 16,
     "mathtext.fontset": "stix",
     "font.serif": ["SimSun"],
     "axes.unicode_minus": False,
```

### Comparing `simubox-0.2.2/SimuBox/artist/phase.py` & `simubox-0.2.3/SimuBox/artist/phase.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Point,
     CommonLabels,
     PathLike,
     Operation,
     RealNum,
     ColorMode,
 )
-from ..toolkits import read_csv
+from ..toolkit import read_csv
 
 __all__ = ["PHASE_PLOT_CONFIG", "PhaseDiagram"]
 
 PHASE_PLOT_CONFIG = {
     "font.family": "Times New Roman",
     "font.serif": ["SimSun"],
     "font.size": 16,
```

### Comparing `simubox-0.2.2/SimuBox/artist/plotter.py` & `simubox-0.2.3/SimuBox/artist/plotter.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/calculator/peak.py` & `simubox-0.2.3/SimuBox/calculator/peak.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/calculator/scatter.py` & `simubox-0.2.3/SimuBox/calculator/scatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.signal as sg
 
 from .peak import gaussian_expansion
 from ..artist import plot_locators, plot_savefig
 from ..schema import ScatterResult, ScatterPlot, Density, PathLike
-from ..toolkits import parse_density
+from ..toolkit import parse_density
 
 SCATTER_PLOT_CONFIG = {
     "font.family": "Times New Roman",
     # "font.family": "serif",
     "font.serif": ["SimSun"],
     "font.size": 16,
     "mathtext.fontset": "stix",
```

### Comparing `simubox-0.2.2/SimuBox/calculator/topo.py` & `simubox-0.2.3/SimuBox/calculator/topo.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/calculator/voronoi.py` & `simubox-0.2.3/SimuBox/calculator/voronoi.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     OpenCVResult,
     AnalyzeMode,
     ColorMode,
     WeightedMode,
     VoronoiAnalyzeResult,
     PathLike,
 )
-from ..toolkits import parse_density
+from ..toolkit import parse_density
 from ..artist import plot_savefig
 
 
 class VoronoiCell:
     @staticmethod
     def OpenCV(
         density: Density,
```

### Comparing `simubox-0.2.2/SimuBox/runner/agents/ABC.py` & `simubox-0.2.3/SimuBox/runner/agents/ABC.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/runner/agents/ABC_ABC.py` & `simubox-0.2.3/SimuBox/runner/agents/ABC_ABC.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/runner/agents/BABCB.py` & `simubox-0.2.3/SimuBox/runner/agents/BABCB.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/runner/agents/Mask_AB_A.py` & `simubox-0.2.3/SimuBox/runner/agents/Mask_AB_A.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/runner/agents/Mask_AB_AB.py` & `simubox-0.2.3/SimuBox/runner/agents/Mask_AB_AB.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/runner/agents/MixinModel.py` & `simubox-0.2.3/SimuBox/runner/agents/MixinModel.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/runner/manager.py` & `simubox-0.2.3/SimuBox/runner/manager.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/runner/phases.py` & `simubox-0.2.3/SimuBox/runner/phases.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/schema/enums/MixinEnums.py` & `simubox-0.2.3/SimuBox/schema/enums/MixinEnums.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/schema/enums/Modes.py` & `simubox-0.2.3/SimuBox/schema/enums/Modes.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/schema/enums/OtherEnums.py` & `simubox-0.2.3/SimuBox/schema/enums/OtherEnums.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/schema/enums/SCFTEnums.py` & `simubox-0.2.3/SimuBox/schema/enums/SCFTEnums.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/schema/labels.py` & `simubox-0.2.3/SimuBox/schema/labels.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/schema/structs/ChartElement.py` & `simubox-0.2.3/SimuBox/schema/structs/ChartElement.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/schema/structs/ComputedRes.py` & `simubox-0.2.3/SimuBox/schema/structs/ComputedRes.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/schema/structs/DataFile.py` & `simubox-0.2.3/SimuBox/schema/structs/DataFile.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/schema/structs/MixinStructs.py` & `simubox-0.2.3/SimuBox/schema/structs/MixinStructs.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/schema/structs/OtherStructs.py` & `simubox-0.2.3/SimuBox/schema/structs/OtherStructs.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/schema/structs/SCFTStructs.py` & `simubox-0.2.3/SimuBox/schema/structs/SCFTStructs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from pathlib import Path
 from ..enums.SCFTEnums import Ensemble, Servers
-from typing import Union, Callable, Any
+from typing import Union, Callable, Any, Sequence
 from collections import OrderedDict
+
+
 class Options:
     filedir: Path = Path.cwd()
     name: str = "WORKING_DIR"
 
     json_name: str = "input.json"
 
     cell: bool = True
@@ -16,28 +18,27 @@
 
     function: Union[Callable, Any]
 
     clean: bool = True
 
     combine_paradict: OrderedDict[str, list[Any]] = OrderedDict()
 
-    init_phin: list[str] = []
-    gpuTOPS_require: list[str] = []
-    gpuSCFT_require: list[str] = []
-
+    init_phin: Sequence[str] = []
     server: Servers = Servers.cpuTOPS
+    gpuTOPS_require: Sequence[str] = []
+    gpuSCFT_require: Sequence[str] = []
 
     phase_base: str = ""
 
     para_file: str = "param_list.txt"
 
     @property
     def workdir(self):
         return self.filedir / self.name
 
     @property
     def worker(self):
         return dict(
-            cpuTOPS=f"srun --partition=intel_2080ti,amd_3090,intel_Xeon --cpus-per-task=2 /home/share/TOPS2020/TOPS2020 -j -i={self.json_name} >aa.txt 2>&1 &",
-            gpuSCFT=f"srun --partition=intel_2080,intel_2080ti,amd_3090 --nodes=1 --gpus=1 /home/share/scft2022 -i={self.json_name} >aa.txt 2>&1 &",
+            cpuTOPS=f"srun --partition=intel_Xeon,amd_4090,amd_3090,intel_2080ti --cpus-per-task=2 /home/share/TOPS2020/TOPS2020 -j -i={self.json_name} >aa.txt 2>&1 &",
+            gpuSCFT=f"srun --partition=amd_4090,amd_3090,intel_2080ti,intel_2080 --nodes=1 --gpus=1 /home/share/scft2024 -i={self.json_name} >aa.txt 2>&1 &",
             gpuTOPS=f"srun --gpus=rtx_3090:1 --cpus-per-gpu=1 --partition=amd_3090 --gpus=1 -w gpu04 /home/share/TOPS2020/TOPS_device -j -i={self.json_name} > aa.txt 2>&1 &",
-        )
+        )
```

### Comparing `simubox-0.2.2/SimuBox/scripts/extractor.py` & `simubox-0.2.3/SimuBox/script/extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 import re
 import subprocess as sp
 from collections import OrderedDict, defaultdict
 from itertools import combinations
 from pathlib import Path
 from typing import Any, Union, Sequence
 from tqdm import tqdm
-
-from push_job import opts
+from ..schema.structs.SCFTStructs import Options as opts
 
 
 def check_files(files: list[Union[str, Path]]):
     for file in files:
         if not os.path.isfile(file):
             print(f"Absent: {file}".center(50, "*"))
             return False
     return True
 
 
 def check_result(res: dict):
-    if res["phase"] == "C4" and round(res["ly"] / res["lz"], 3) != 1.0:
-        res["phase"] = "Crect"
-    elif res["phase"] == "Crect" and round(res["ly"] / res["lz"], 3) == 1.0:
-        res["phase"] = "C4"
+    if "phase" in res:
+        if res["phase"] == "C4" and round(res["ly"] / res["lz"], 3) != 1.0:
+            res["phase"] = "Crect"
+        elif res["phase"] == "Crect" and round(res["ly"] / res["lz"], 3) == 1.0:
+            res["phase"] = "C4"
 
     if round(res["freeE_dis"] - res["freeE"], 3) == 0:
         res["phase"] = "Disorder"
 
     if (res["server"] == "cpu" and res["target_comp"] < res["CompMax"]) or (
         res["server"] == "gpu" and res["target_comp"] * 1e3 < res["CompMax"]
     ):
@@ -93,19 +93,19 @@
         os.chdir(subdir)
         if not check_files(files=["printout.txt", opts.json_name]):
             continue
         with open(opts.json_name, mode="r") as fp:
             json_data = json.load(fp, object_pairs_hook=OrderedDict)
 
         data = {}
-        scripts = json_data["Scripts"]
+        scripts = json_data.get("Scripts", {})
         data.update(scripts)
         stats_res = stats_component(json_data)
         data.update(stats_res)
-        server_before = json_data["Scripts"].get("cal_type", "cpu")
+        server_before = scripts.get("cal_type", "cpu")
         data["server"] = server_before
         data["target_comp"] = json_data["Iteration"]["IncompressibilityTarget"]
         if server_before == "cpu":
             popen_freeE_MaxC = sp.Popen(
                 cmd_freeE_MaxC, shell=True, stdout=sp.PIPE, stderr=sp.PIPE
             )
             popen_freeE_MaxC.wait()
@@ -192,35 +192,37 @@
         return
     mode = input("删除(d) / 续跑(c) / 重投(r) / 跳过(其他任意键)? (d/c/r/[pass])") or "pass"
     if mode == "c":
         for mission in missions:
             mission_folder = mission["path"]
             os.chdir(mission_folder)
             with open(opts.json_name, mode="r") as fp:
-                json_base = json.load(fp, object_pairs_hook=OrderedDict)
+                json_data = json.load(fp, object_pairs_hook=OrderedDict)
             server = args.server or mission["server"]
-            json_base["Scripts"]["cal_type"] = (
+            if "Scripts" not in json_data:
+                json_data["Scripts"] = {}
+            json_data["Scripts"]["cal_type"] = (
                 server if os.path.isfile("phout.txt") else "cpu"
             )
-            json_base["Iteration"]["MaxStep"] = mission["step"]
-            json_base["Initializer"]["UnitCell"]["Length"] = mission["lxlylz"]
+            json_data["Iteration"]["MaxStep"] = mission["step"]
+            json_data["Initializer"]["UnitCell"]["Length"] = mission["lxlylz"]
             if os.path.isfile("phout.txt"):
                 sp.call("cp phout.txt phin.txt", shell=True, stdout=sp.PIPE)
-                json_base["Initializer"]["Mode"] = "FILE"
-                json_base["Initializer"]["FileInitializer"] = {
+                json_data["Initializer"]["Mode"] = "FILE"
+                json_data["Initializer"]["FileInitializer"] = {
                     "Mode": "OMEGA",
                     "Path": "phin.txt",
                     "SkipLineNumber": 1 if mission["server"] == "cpu" else 2,
                 }
-                json_base["Iteration"]["AndersonMixing"]["Switch"] = "AUTO"
+                json_data["Iteration"]["AndersonMixing"]["Switch"] = "AUTO"
 
                 with open(opts.json_name, "w") as f:
-                    json.dump(json_base, f, indent=4, separators=(",", ": "))
+                    json.dump(json_data, f, indent=4, separators=(",", ": "))
 
-            if json_base["Scripts"]["cal_type"] == "gpu":
+            if json_data["Scripts"]["cal_type"] == "gpu":
                 job = sp.Popen(opts.worker["gpuSCFT"], shell=True, stdout=sp.PIPE)
             else:
                 job = sp.Popen(opts.worker["cpuTOPS"], shell=True, stdout=sp.PIPE)
             print(f"续跑任务({job.pid}):{mission_folder}")
     elif mode == "r":
         for mission in missions:
             mission_folder = mission["path"]
@@ -253,22 +255,27 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("-n", "--name", default="", type=str)
     parser.add_argument("-t", "--terminal", default="WORKING_DIR", type=str)
     parser.add_argument("-s", "--server", default="", type=str)
     parser.add_argument("-a", "--all", action="store_true", default=False)
     args = parser.parse_args()
 
+    exclude = ("Density", "old")
     cmd_lxlylz = "tail -3 printout.txt | head -1"
     cmd_freeE_MaxC = "tail -1 printout.txt | head -1"
     lxlylz_re = re.compile("[.0-9]+(?!e)")
     freeE_re = re.compile("[.0-9e+-]+")
 
     parent_folder = Path.cwd()
     working_directory = parent_folder / args.terminal
-    subdirectories = [item for item in working_directory.iterdir() if item.is_dir()]
+    subdirectories = [
+        item
+        for item in working_directory.iterdir()
+        if item.is_dir() and item.stem not in exclude
+    ]
 
     output_csv_name = args.name or parent_folder.name
     output_csv_path = parent_folder / output_csv_name
     if output_csv_path.suffix != ".csv":
         output_csv_path = str(output_csv_path) + ".csv"
 
     datas, columns, missions_list = collect(subdirectories, args)
```

### Comparing `simubox-0.2.2/SimuBox/scripts/JSON/ABC_ABC.json` & `simubox-0.2.3/SimuBox/script/JSON/ABC_ABC.json`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/scripts/JSON/BABCB.json` & `simubox-0.2.3/SimuBox/script/JSON/BABCB.json`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/scripts/setenv.py` & `simubox-0.2.3/SimuBox/script/setenv.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 import os
 import subprocess
 from pathlib import Path
+import platform
 
-abs_current_dir = Path(__file__).parent.absolute()
-json_files = (abs_current_dir / "JSON").iterdir()
+if __name__ == "__main__":
 
-alias_list = [
-    'alias pj="ls | grep push_job | xargs -i python3 {}"',
-    'alias pjs="ls | grep push_job | xargs -i python3 {} >aa.txt 2>&1 &"',
-    f'alias prep="cp {abs_current_dir / "extractor.py"} ./;cp {abs_current_dir / "push_job.py"}"',
-]
-
-for json_file in json_files:
-    name = json_file.stem.lower()
-    alias_list.append(f'alias {name}="cp {json_file.absolute()} ./input.json"')
-    alias_list.append(f'alias prep_{name}="prep;{name}"')
-
-
-bashrc_path = os.path.expanduser("~/.bashrc")
-with open(bashrc_path, "r") as bashrc_file:
-    cont = bashrc_file.read()
-
-with open(bashrc_path, "a") as bashrc_append_file:
-    for element in alias_list:
-        # 检查.bashrc是否已经包含该alias，如果不存在则添加
-        if element not in cont:
-            bashrc_append_file.write(f"{element}\n")
-            print(f"{element} added to .bashrc")
-        else:
-            print(f"{element} already exists in .bashrc")
+    abs_current_dir = Path(__file__).parent.absolute()
+    json_files = (abs_current_dir / "JSON").iterdir()
 
-# 执行 source ~/.bashrc 命令
-subprocess.run("source ~/.bashrc", shell=True)
+    alias_list = [
+        'alias web="python -m SimuBox.script.web"',
+        'alias ext="python -m SimuBox.script.extractor"',
+        'alias pj="ls | grep push_job | xargs -i python3 {}"',
+        'alias pjs="ls | grep push_job | xargs -i python3 {} >aa.txt 2>&1 &"',
+        f'alias prep="cp {abs_current_dir / "push_job.py"}" ./',
+        # f'alias prep="cp {abs_current_dir / "extractor.py"} ./;cp {abs_current_dir / "push_job.py"}"',
+    ]
+
+    for json_file in json_files:
+        name = json_file.stem.lower()
+        alias_list.append(f'alias {name}="cp {json_file.absolute()} ./input.json"')
+        alias_list.append(f'alias prep_{name}="prep;{name}"')
+
+
+    if platform.system() == "Linux":
+        bashrc_path = os.path.expanduser("~/.bashrc")
+        with open(bashrc_path, "r") as bashrc_file:
+            cont = bashrc_file.read()
+
+        with open(bashrc_path, "a") as bashrc_append_file:
+            for element in alias_list:
+                # 检查.bashrc是否已经包含该alias，如果不存在则添加
+                if element not in cont:
+                    bashrc_append_file.write(f"{element}\n")
+                    print(f"{element} added to .bashrc")
+                else:
+                    print(f"{element} already exists in .bashrc")
+
+        # 执行 source ~/.bashrc 命令
+        subprocess.run("source ~/.bashrc", shell=True)
+    else:
+        for element in alias_list:
+            print(element)
```

### Comparing `simubox-0.2.2/SimuBox/scripts/web.py` & `simubox-0.2.3/SimuBox/script/web.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from pathlib import Path
 import argparse
 import os
+import platform
 
-os.environ["NUMEXPR_MAX_THREADS"] = "16"
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="启动SimuBox的网页端服务")
     parser.add_argument("-a", "--app", type=str, default="Homepage.py", help="主页面文件")
     parser.add_argument("-p", "--port", type=int, default=9998)
     parser.add_argument(
         "-l",
         "--log_level",
         type=str,
         default="error",
         choices=["error", "warning", "info", "debug"],
     )
     args = parser.parse_args()
     app_path = Path(__file__).parents[1] / "web" / args.app
+
+    if platform.system() == "Windows":
+        os.environ["NUMEXPR_MAX_THREADS"] = "16"
+    else:
+        os.environ["NUMEXPR_MAX_THREADS"] = "4"
     os.system(f"python -m streamlit run {app_path} --server.port {args.port}")
```

### Comparing `simubox-0.2.2/SimuBox/toolkits/function.py` & `simubox-0.2.3/SimuBox/toolkit/function.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/toolkits/reader.py` & `simubox-0.2.3/SimuBox/toolkit/reader.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/toolkits/vector.py` & `simubox-0.2.3/SimuBox/toolkit/vector.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/toolkits/xmltrans.py` & `simubox-0.2.3/SimuBox/toolkit/xmltrans.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/web/Homepage.py` & `simubox-0.2.3/SimuBox/web/Homepage.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/web/pages/1_Structure.py` & `simubox-0.2.3/SimuBox/web/pages/1_Structure.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/web/pages/2_Scatter.py` & `simubox-0.2.3/SimuBox/web/pages/2_Scatter.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/web/pages/3_Voronoi.py` & `simubox-0.2.3/SimuBox/web/pages/3_Voronoi.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/web/pages/4_Curve.py` & `simubox-0.2.3/SimuBox/web/pages/4_Curve.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/web/pages/5_Peaks.py` & `simubox-0.2.3/SimuBox/web/pages/5_Peaks.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/web/pages/6_Topology.py` & `simubox-0.2.3/SimuBox/web/pages/6_Topology.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/SimuBox/web/pages/7_Landscape.py` & `simubox-0.2.3/SimuBox/web/pages/7_Landscape.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.2/PKG-INFO` & `simubox-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimuBox
-Version: 0.2.2
+Version: 0.2.3
 Summary: Free python package to do some science calculation.
 Home-page: https://pypi.org/project/SimuBox/
 License: ./LICENSE
 Author: Alkaid Yuan
 Author-email: kryuan@qq.com
 Maintainer: Alkaid Yuan
 Maintainer-email: kryuan@qq.com
```

